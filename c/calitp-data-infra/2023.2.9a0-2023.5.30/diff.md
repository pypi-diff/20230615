# Comparing `tmp/calitp_data_infra-2023.2.9a0.tar.gz` & `tmp/calitp_data_infra-2023.5.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calitp_data_infra-2023.2.9a0.tar", max compression
+gzip compressed data, was "calitp_data_infra-2023.5.30.tar", max compression
```

## Comparing `calitp_data_infra-2023.2.9a0.tar` & `calitp_data_infra-2023.5.30.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-02-09 21:42:54.825182 calitp_data_infra-2023.2.9a0/calitp_data_infra/__init__.py
--rw-r--r--   0        0        0     1184 2023-02-09 20:39:18.071442 calitp_data_infra-2023.2.9a0/calitp_data_infra/auth.py
--rw-r--r--   0        0        0    24886 2023-02-09 20:37:46.237424 calitp_data_infra-2023.2.9a0/calitp_data_infra/storage.py
--rw-r--r--   0        0        0      639 2023-02-09 21:42:54.825397 calitp_data_infra-2023.2.9a0/pyproject.toml
--rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 calitp_data_infra-2023.2.9a0/setup.py
--rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 calitp_data_infra-2023.2.9a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-06 19:38:05.139171 calitp_data_infra-2023.5.30/calitp_data_infra/__init__.py
+-rw-r--r--   0        0        0     1154 2023-03-06 19:38:05.139399 calitp_data_infra-2023.5.30/calitp_data_infra/auth.py
+-rw-r--r--   0        0        0    23867 2023-06-02 19:33:40.910652 calitp_data_infra-2023.5.30/calitp_data_infra/storage.py
+-rw-r--r--   0        0        0      751 2023-06-02 19:33:40.910966 calitp_data_infra-2023.5.30/pyproject.toml
+-rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 calitp_data_infra-2023.5.30/setup.py
+-rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 calitp_data_infra-2023.5.30/PKG-INFO
```

### Comparing `calitp_data_infra-2023.2.9a0/calitp_data_infra/auth.py` & `calitp_data_infra-2023.5.30/calitp_data_infra/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,15 @@
     secret_values = {}
 
     # once we get on at least 2.0.0 of secret manager, we can filter server-side
     for secret in client.list_secrets(parent=project):
         if label in secret.labels:
             version = f"{secret.name}/versions/latest"
             response = client.access_secret_version(version)
-            secret_values[secret.name.split("/")[-1]] = response.payload.data.decode(
-                "UTF-8"
-            ).strip()
+            secret_values[secret.name.split("/")[-1]] = response.payload.data.decode("UTF-8").strip()
 
     return secret_values
 
 
 if __name__ == "__main__":
     print("loading secrets...")
     get_secret_by_name("BEAR_TRANSIT_KEY")
```

### Comparing `calitp_data_infra-2023.2.9a0/calitp_data_infra/storage.py` & `calitp_data_infra-2023.5.30/calitp_data_infra/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     get_type_hints,
 )
 
 import backoff
 import gcsfs
 import humanize
 import pendulum
+from calitp_data.config import get_bucket, require_pipeline
+from calitp_data.storage import get_fs
 from google.cloud import storage
 from google.cloud.storage import Blob
 from pydantic import (
     BaseModel,
     Extra,
     Field,
     HttpUrl,
@@ -38,29 +40,18 @@
     validator,
 )
 from pydantic.class_validators import root_validator
 from pydantic.tools import parse_obj_as
 from requests import Request, Session
 from typing_extensions import Annotated, Literal
 
-from calitp.config import get_bucket, is_cloud, require_pipeline
-
 JSONL_EXTENSION = ".jsonl"
 JSONL_GZIP_EXTENSION = f"{JSONL_EXTENSION}.gz"
 
 
-def get_fs(gcs_project="", **kwargs):
-    if is_cloud():
-        return gcsfs.GCSFileSystem(project=gcs_project, token="cloud", **kwargs)
-    else:
-        return gcsfs.GCSFileSystem(
-            project=gcs_project, token="google_default", **kwargs
-        )
-
-
 @require_pipeline("save_to_gcfs")
 def save_to_gcfs(
     src_path,
     dst_path,
     gcs_project="cal-itp-data-infra",
     bucket=None,
     use_pipe=False,
@@ -149,18 +140,15 @@
 
 
 def partition_map(path) -> Dict[str, PartitionType]:
     return {key: value for key, value in re.findall(r"/(\w+)=([\w\-:=+.]+)(?=/)", path)}
 
 
 def serialize_partitions(partitions: Dict[str, PartitionType]) -> List[str]:
-    return [
-        f"{name}={PARTITION_SERIALIZERS[type(value)](value)}"
-        for name, value in partitions.items()
-    ]
+    return [f"{name}={PARTITION_SERIALIZERS[type(value)](value)}" for name, value in partitions.items()]
 
 
 class GTFSFeedType(str, Enum):
     schedule = "schedule"
     service_alerts = "service_alerts"
     trip_updates = "trip_updates"
     vehicle_positions = "vehicle_positions"
@@ -227,39 +215,29 @@
         """
         Defines the partitions into which this artifact is organized.
         The order does matter!
         """
 
     @property
     def serialized_partitions(self) -> List[str]:
-        return serialize_partitions(
-            {name: getattr(self, name) for name in self.partition_names}
-        )
+        return serialize_partitions({name: getattr(self, name) for name in self.partition_names})
 
     @property
     def partition_types(self) -> Dict[str, Type[PartitionType]]:
         return {}
 
     @root_validator(allow_reuse=True)
     def check_partitions(cls, values):
         # TODO: this isn't great but some partition_names are properties
         if isinstance(cls.partition_names, property):
             return values
-        cls_properties = [
-            name for name in dir(cls) if isinstance(getattr(cls, name), property)
-        ]
-        missing = [
-            name
-            for name in cls.partition_names
-            if name not in values and name not in cls_properties
-        ]
+        cls_properties = [name for name in dir(cls) if isinstance(getattr(cls, name), property)]
+        missing = [name for name in cls.partition_names if name not in values and name not in cls_properties]
         if missing:
-            raise ValueError(
-                f"all partition names must exist as fields or properties; missing {missing}"
-            )
+            raise ValueError(f"all partition names must exist as fields or properties; missing {missing}")
         return values
 
     @property
     def name(self):
         return os.path.join(
             self.table,
             *self.serialized_partitions,
@@ -288,31 +266,27 @@
             fs.setxattrs(
                 path=self.path,
                 # This syntax seems silly but it's so we pass the _value_ of PARTITIONED_ARTIFACT_METADATA_KEY
                 **{PARTITIONED_ARTIFACT_METADATA_KEY: self.json(exclude=exclude)},
             )
 
         if client:
-            logging.info(
-                f"saving {humanize.naturalsize(len(content))} to {self.bucket} {self.name}"
-            )
+            logging.info(f"saving {humanize.naturalsize(len(content))} to {self.bucket} {self.name}")
             blob = storage.Blob(
                 name=self.name,
                 bucket=client.bucket(self.bucket.replace("gs://", "")),
             )
 
             blob.upload_from_string(
                 data=content,
                 content_type="application/octet-stream",
                 client=client,
             )
 
-            set_metadata_func = (
-                set_metadata_with_retry if retry_metadata else set_metadata
-            )
+            set_metadata_func = set_metadata_with_retry if retry_metadata else set_metadata
             set_metadata_func(
                 blob=blob,
                 model=self,
                 exclude=exclude,
             )
 
 
@@ -324,53 +298,43 @@
     table: str = None,
     verbose=False,
 ) -> Tuple[List[PartitionedGCSArtifact], List[Blob], List[Blob]]:
     if not bucket:
         bucket = cls.bucket
 
         if not isinstance(bucket, str):
-            raise TypeError(
-                f"must either pass bucket, or the bucket must resolve to a string; got {type(bucket)}"
-            )
+            raise TypeError(f"must either pass bucket, or the bucket must resolve to a string; got {type(bucket)}")
 
     if not table:
         table = cls.table
 
         if not isinstance(table, str):
-            raise TypeError(
-                f"must either pass table, or the table must resolve to a string; got {type(table)}"
-            )
+            raise TypeError(f"must either pass table, or the table must resolve to a string; got {type(table)}")
 
     prefix = "/".join(
         [
             table,
             *serialize_partitions(partitions),
             "",
         ]
     )
     if verbose:
         print(f"listing all files in {bucket}/{prefix}")
     client = storage.Client()
     # once Airflow is upgraded to Python 3.9, can use:
     # files = client.list_blobs(bucket.removeprefix("gs://"), prefix=prefix, delimiter=None)
-    files = client.list_blobs(
-        re.sub(r"^gs://", "", bucket), prefix=prefix, delimiter=None
-    )
+    files = client.list_blobs(re.sub(r"^gs://", "", bucket), prefix=prefix, delimiter=None)
 
     parsed: List[PartitionedGCSArtifact] = []
     blobs_with_missing_metadata: List[Blob] = []
     blobs_with_invalid_metadata: List[Blob] = []
 
     for file in files:
         try:
-            parsed.append(
-                parse_obj_as(
-                    cls, json.loads(file.metadata[PARTITIONED_ARTIFACT_METADATA_KEY])
-                )
-            )
+            parsed.append(parse_obj_as(cls, json.loads(file.metadata[PARTITIONED_ARTIFACT_METADATA_KEY])))
         except (TypeError, KeyError):
             logging.exception(f"metadata missing on {bucket}/{file.name}")
             blobs_with_missing_metadata.append(file)
         except ValidationError:
             logging.exception(f"invalid metadata found on {bucket}/{file.name}")
             blobs_with_invalid_metadata.append(file)
 
@@ -426,17 +390,15 @@
 
     @property
     def partition(self) -> Dict[str, str]:
         return partition_map(self.name + "/")
 
     def children(self, fs) -> List["GCSObjectInfo"]:
         # TODO: this should work with a discriminated type but idk why it's not
-        return parse_obj_as(
-            GCSObjectInfoList, [fs.info(child) for child in fs.ls(self.name)]
-        ).__root__
+        return parse_obj_as(GCSObjectInfoList, [fs.info(child) for child in fs.ls(self.name)]).__root__
 
 
 GCSObjectInfo = Annotated[
     Union[GCSFileInfo, GCSDirectoryInfo],
     Field(discriminator="type"),
 ]
 
@@ -449,93 +411,75 @@
     table: str,
     prefix_partitions: Dict[str, PartitionType],
     partition_types: Dict[str, Type[PartitionType]],
 ) -> GCSFileInfo:
     fs = get_fs()
     fs.invalidate_cache()
 
-    prefix_info = fs.info(
-        "/".join([bucket, table, *serialize_partitions(prefix_partitions), ""])
-    )
+    prefix_info = fs.info("/".join([bucket, table, *serialize_partitions(prefix_partitions), ""]))
     directory = GCSDirectoryInfo(**prefix_info)
 
     for key, typ in partition_types.items():
         directory = sorted(
             directory.children(fs),
             key=lambda o: PARTITION_DESERIALIZERS[typ](o.partition[key]),
             reverse=True,
         )[0]
 
     children = directory.children(fs)
     # This is just a convention for us for now; we could also label files with metadata if desired
     if len(children) != 1:
-        raise ValueError(
-            f"found {len(directory.children(fs))} files rather than 1 in the directory {directory.name}"
-        )
+        raise ValueError(f"found {len(directory.children(fs))} files rather than 1 in the directory {directory.name}")
 
     ret = children[0]
 
     # is there a way to have pydantic check this?
     if not isinstance(ret, GCSFileInfo):
-        raise ValueError(
-            f"encountered unexpected type {type(ret)} rather than GCSFileInfo"
-        )
+        raise ValueError(f"encountered unexpected type {type(ret)} rather than GCSFileInfo")
 
     return ret
 
 
 def get_latest(
     cls: Type[PartitionedGCSArtifact],
     bucket: str = None,
     table: str = None,
     partition_names: List[str] = None,
 ) -> PartitionedGCSArtifact:
     if not bucket:
         bucket = cls.bucket
 
         if not isinstance(bucket, str):
-            raise TypeError(
-                f"must either pass bucket, or the bucket must resolve to a string; got {type(bucket)}"
-            )
+            raise TypeError(f"must either pass bucket, or the bucket must resolve to a string; got {type(bucket)}")
 
     if not table:
         table = cls.table
 
         if not isinstance(table, str):
-            raise TypeError(
-                f"must either pass table, or the table must resolve to a string; got {type(table)}"
-            )
+            raise TypeError(f"must either pass table, or the table must resolve to a string; got {type(table)}")
 
     if not partition_names:
         partition_names = cls.partition_names
 
         if not isinstance(partition_names, list):
             raise TypeError(
                 f"must either pass partition names, or the partition names must resolve to a list; got {type(partition_names)}"
             )
 
     latest = get_latest_file(
         bucket,
         table,
         prefix_partitions={},
         # TODO: this doesn't pick up the type hint of dt since it's a property; it's fine as a string but we should fix
-        partition_types={
-            name: get_type_hints(cls).get(name, str) for name in partition_names
-        },
+        partition_types={name: get_type_hints(cls).get(name, str) for name in partition_names},
     )
 
     logging.info(f"identified {latest.name} as the most recent extract of {cls}")
 
-    return cls(
-        **json.loads(
-            get_fs().getxattr(
-                path=f"gs://{latest.name}", attr=PARTITIONED_ARTIFACT_METADATA_KEY
-            )
-        )
-    )
+    return cls(**json.loads(get_fs().getxattr(path=f"gs://{latest.name}", attr=PARTITIONED_ARTIFACT_METADATA_KEY)))
 
 
 class AirtableGTFSDataRecord(BaseModel):
     id: str
     name: str
     uri: Optional[str]
     pipeline_url: Optional[str]
@@ -568,33 +512,26 @@
     @classmethod
     def get_latest(cls) -> "AirtableGTFSDataExtract":
         latest = get_latest_file(
             cls.bucket,
             cls.table,
             prefix_partitions={},
             # TODO: this doesn't pick up the type hint of dt since it's a property; it's fine as a string but we should fix
-            partition_types={
-                name: get_type_hints(cls).get(name, str) for name in cls.partition_names
-            },
+            partition_types={name: get_type_hints(cls).get(name, str) for name in cls.partition_names},
         )
 
-        logging.info(
-            f"identified {latest.name} as the most recent extract of gtfs datasets"
-        )
+        logging.info(f"identified {latest.name} as the most recent extract of gtfs datasets")
 
         with get_fs().open(latest.name, "rb") as f:
             content = gzip.decompress(f.read())
 
         return AirtableGTFSDataExtract(
             filename=latest.filename,
             ts=pendulum.parse(latest.partition["ts"], exact=True),
-            records=[
-                AirtableGTFSDataRecord(**json.loads(row))
-                for row in content.decode().splitlines()
-            ],
+            records=[AirtableGTFSDataRecord(**json.loads(row)) for row in content.decode().splitlines()],
         )
 
 
 # forbid here as we want to be super careful/strict
 class GTFSDownloadConfig(BaseModel, extra=Extra.forbid):
     extracted_at: Optional[pendulum.DateTime]
     name: Optional[str]
@@ -628,17 +565,15 @@
         return v
 
     def build_request(self, auth_dict: Mapping[str, str]) -> Request:
         params = {k: auth_dict[v] for k, v in self.auth_query_params.items()}
         headers = {k: auth_dict[v] for k, v in self.auth_headers.items()}
 
         # some web servers require user agents or they will throw a 4XX error
-        headers[
-            "User-Agent"
-        ] = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.12; rv:55.0) Gecko/20100101 Firefox/55.0"
+        headers["User-Agent"] = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.12; rv:55.0) Gecko/20100101 Firefox/55.0"
 
         # inspired by: https://stackoverflow.com/questions/18869074/create-url-without-request-execution
         return Request(
             "GET",
             url=self.url,
             params=params,
             headers=headers,
@@ -650,17 +585,15 @@
         # we care about replacing slashes for GCS object names
         # can use: https://www.base64url.com/ to test encoding/decoding
         # convert in bigquery: https://cloud.google.com/bigquery/docs/reference/standard-sql/string_functions#from_base64
         return base64.urlsafe_b64encode(self.url.encode()).decode()
 
     @property
     def base64_validation_url(self) -> str:
-        return base64.urlsafe_b64encode(
-            self.schedule_url_for_validation.encode()
-        ).decode()
+        return base64.urlsafe_b64encode(self.schedule_url_for_validation.encode()).decode()
 
 
 class GTFSDownloadConfigExtract(PartitionedGCSArtifact):
     bucket: ClassVar[str] = GTFS_DOWNLOAD_CONFIG_BUCKET
     table: ClassVar[str] = "gtfs_download_configs"
     partition_names: ClassVar[List[str]] = ["dt", "ts"]
     ts: pendulum.DateTime
@@ -750,36 +683,30 @@
     **request_kwargs,
 ) -> Tuple[GTFSFeedExtract, bytes]:
     s = Session()
     r = s.prepare_request(config.build_request(auth_dict))
     resp = s.send(r, **request_kwargs)
     resp.raise_for_status()
 
-    disposition_header = resp.headers.get(
-        "content-disposition", resp.headers.get("Content-Disposition")
-    )
+    disposition_header = resp.headers.get("content-disposition", resp.headers.get("Content-Disposition"))
 
     if disposition_header:
         if disposition_header.startswith("filename="):
             # sorry; cgi won't parse unless it's prefixed with the disposition type
             disposition_header = f"attachment; {disposition_header}"
         _, params = cgi.parse_header(disposition_header)
         disposition_filename = params.get("filename")
     else:
         disposition_filename = None
 
     filename = (
-        disposition_filename
-        or (os.path.basename(resp.url) if resp.url.endswith(".zip") else None)
-        or default_filename
+        disposition_filename or (os.path.basename(resp.url) if resp.url.endswith(".zip") else None) or default_filename
     )
 
-    extract_class = (
-        GTFSRTFeedExtract if config.feed_type.is_rt else GTFSScheduleFeedExtract
-    )
+    extract_class = GTFSRTFeedExtract if config.feed_type.is_rt else GTFSScheduleFeedExtract
     extract = extract_class(
         filename=filename,
         config=config,
         response_code=resp.status_code,
         response_headers=resp.headers,
         ts=ts,
     )
@@ -791,28 +718,24 @@
     # just some useful testing stuff
     latest = AirtableGTFSDataExtract.get_latest()
     print(latest.path, len(latest.records))
     extract = get_latest(GTFSDownloadConfigExtract)
     fs = get_fs()
     with fs.open(extract.path, "rb") as f:
         content = gzip.decompress(f.read())
-    records = [
-        GTFSDownloadConfig(**json.loads(row)) for row in content.decode().splitlines()
-    ]
+    records = [GTFSDownloadConfig(**json.loads(row)) for row in content.decode().splitlines()]
     download_feed(records[0], auth_dict={}, ts=pendulum.now(), timeout=1)
     print("downloaded a thing!")
     sys.exit(0)
 
     # use Etc/UTC instead of UTC
     # Etc/UTC is what the pods get as a timezone... and it serializes to 2022-08-18T00:00:00+00:00
     # whereas UTC serializes to 2022-08-18T00:00:00Z
     # this should probably be checked in the partitioned artifact?
-    yesterday_noon = pendulum.yesterday("Etc/UTC").replace(
-        minute=0, second=0, microsecond=0
-    )
+    yesterday_noon = pendulum.yesterday("Etc/UTC").replace(minute=0, second=0, microsecond=0)
     vp_files, _, _ = fetch_all_in_partition(
         cls=GTFSRTFeedExtract,
         fs=get_fs(),
         partitions={
             "dt": yesterday_noon.date(),
             "hour": yesterday_noon,
         },
```

### Comparing `calitp_data_infra-2023.2.9a0/setup.py` & `calitp_data_infra-2023.5.30/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 ['calitp_data_infra']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['backoff>=2.2.1,<3.0.0',
- 'calitp==2023.2.9',
- 'google-api-core>=1.32.0,<2.0.0dev',
- 'google-cloud-bigquery-storage==2.14.1',
+ 'calitp-data==2023.2.15.1',
+ 'google-api-core>=1.31.4',
+ 'google-cloud-secret-manager>=1.0.0,<1.1.0',
  'humanize>=4.6.0,<5.0.0',
  'pendulum>=2.1.2,<3.0.0',
- 'pydantic>=1.10.4,<2.0.0',
+ 'pydantic>=1.9,<1.10',
  'tqdm>=4.64.1,<5.0.0',
- 'typing-extensions>=4.4.0,<5.0.0']
+ 'typing-extensions>=3.10.0.2']
 
 setup_kwargs = {
     'name': 'calitp-data-infra',
-    'version': '2023.2.9a0',
-    'description': '',
+    'version': '2023.5.30',
+    'description': 'Shared code for developing data pipelines that process Cal-ITP data.',
     'long_description': 'None',
     'author': 'Andrew Vaccaro',
-    'author_email': 'atvaccaro@gmail.com',
+    'author_email': 'andrew.v@jarv.us',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.9,<3.10',
+    'python_requires': '>=3.8,<3.10',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `calitp_data_infra-2023.2.9a0/PKG-INFO` & `calitp_data_infra-2023.5.30/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: calitp-data-infra
-Version: 2023.2.9a0
-Summary: 
+Version: 2023.5.30
+Summary: Shared code for developing data pipelines that process Cal-ITP data.
 Author: Andrew Vaccaro
-Author-email: atvaccaro@gmail.com
-Requires-Python: >=3.9,<3.10
+Author-email: andrew.v@jarv.us
+Requires-Python: >=3.8,<3.10
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
-Requires-Dist: calitp (==2023.2.9)
-Requires-Dist: google-api-core (>=1.32.0,<2.0.0dev)
-Requires-Dist: google-cloud-bigquery-storage (==2.14.1)
+Requires-Dist: calitp-data (==2023.2.15.1)
+Requires-Dist: google-api-core (>=1.31.4)
+Requires-Dist: google-cloud-secret-manager (>=1.0.0,<1.1.0)
 Requires-Dist: humanize (>=4.6.0,<5.0.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
+Requires-Dist: pydantic (>=1.9,<1.10)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
-Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
+Requires-Dist: typing-extensions (>=3.10.0.2)
```

