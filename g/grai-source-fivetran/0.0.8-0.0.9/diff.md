# Comparing `tmp/grai_source_fivetran-0.0.8.tar.gz` & `tmp/grai_source_fivetran-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_fivetran-0.0.8.tar", max compression
+gzip compressed data, was "grai_source_fivetran-0.0.9.tar", max compression
```

## Comparing `grai_source_fivetran-0.0.8.tar` & `grai_source_fivetran-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      420 2023-05-25 16:20:32.597515 grai_source_fivetran-0.0.8/README.md
--rw-r--r--   0        0        0     1020 2023-05-27 15:46:22.651284 grai_source_fivetran-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      119 2023-02-14 16:39:18.542655 grai_source_fivetran-0.0.8/src/grai_source_fivetran/__init__.py
--rw-r--r--   0        0        0     6644 2023-05-19 11:07:12.931545 grai_source_fivetran-0.0.8/src/grai_source_fivetran/adapters.py
--rw-r--r--   0        0        0     2111 2023-05-26 22:51:50.125227 grai_source_fivetran-0.0.8/src/grai_source_fivetran/base.py
--rw-r--r--   0        0        0        0 2023-02-14 16:39:18.543040 grai_source_fivetran-0.0.8/src/grai_source_fivetran/fivetran_api/__init__.py
--rw-r--r--   0        0        0   436632 2023-02-14 16:39:18.545031 grai_source_fivetran-0.0.8/src/grai_source_fivetran/fivetran_api/api_models.py
--rw-r--r--   0        0        0    42232 2023-02-14 16:39:18.545359 grai_source_fivetran-0.0.8/src/grai_source_fivetran/fivetran_api/main.py
--rw-r--r--   0        0        0    13311 2023-05-27 15:45:55.987821 grai_source_fivetran-0.0.8/src/grai_source_fivetran/loader.py
--rw-r--r--   0        0        0     1668 2023-02-14 16:39:18.545711 grai_source_fivetran-0.0.8/src/grai_source_fivetran/mock_tools.py
--rw-r--r--   0        0        0     4751 2023-02-14 16:39:18.545877 grai_source_fivetran-0.0.8/src/grai_source_fivetran/models.py
--rw-r--r--   0        0        0      186 2023-02-14 16:39:18.546106 grai_source_fivetran-0.0.8/src/grai_source_fivetran/package_definitions.py
--rw-r--r--   0        0        0        0 2023-02-14 16:39:18.546143 grai_source_fivetran-0.0.8/src/grai_source_fivetran/py.typed
--rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 grai_source_fivetran-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      420 2023-05-25 16:20:32.597515 grai_source_fivetran-0.0.9/README.md
+-rw-r--r--   0        0        0     1092 2023-06-14 22:23:33.925985 grai_source_fivetran-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      142 2023-06-14 22:23:33.932002 grai_source_fivetran-0.0.9/src/grai_source_fivetran/__init__.py
+-rw-r--r--   0        0        0     8750 2023-06-14 22:10:38.525486 grai_source_fivetran-0.0.9/src/grai_source_fivetran/adapters.py
+-rw-r--r--   0        0        0     2937 2023-06-14 21:10:34.441273 grai_source_fivetran-0.0.9/src/grai_source_fivetran/base.py
+-rw-r--r--   0        0        0        0 2023-02-14 16:39:18.543040 grai_source_fivetran-0.0.9/src/grai_source_fivetran/fivetran_api/__init__.py
+-rw-r--r--   0        0        0   451222 2023-06-01 16:01:43.261936 grai_source_fivetran-0.0.9/src/grai_source_fivetran/fivetran_api/api_models.py
+-rw-r--r--   0        0        0    69211 2023-06-01 16:01:43.262231 grai_source_fivetran-0.0.9/src/grai_source_fivetran/fivetran_api/main.py
+-rw-r--r--   0        0        0    16866 2023-06-14 21:02:53.368839 grai_source_fivetran-0.0.9/src/grai_source_fivetran/loader.py
+-rw-r--r--   0        0        0     2173 2023-06-01 16:01:43.262518 grai_source_fivetran-0.0.9/src/grai_source_fivetran/mock_tools.py
+-rw-r--r--   0        0        0     5452 2023-06-14 21:02:53.331689 grai_source_fivetran-0.0.9/src/grai_source_fivetran/models.py
+-rw-r--r--   0        0        0      199 2023-06-01 16:01:43.262730 grai_source_fivetran-0.0.9/src/grai_source_fivetran/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-02-14 16:39:18.546143 grai_source_fivetran-0.0.9/src/grai_source_fivetran/py.typed
+-rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 grai_source_fivetran-0.0.9/PKG-INFO
```

### Comparing `grai_source_fivetran-0.0.8/pyproject.toml` & `grai_source_fivetran-0.0.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_fivetran"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_fivetran", from = "src" },
 ]
 readme = "README.md"
@@ -12,20 +12,20 @@
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-fivetran"
 documentation = "https://docs.grai.io/"
 
 
 [tool.poetry.dependencies]
 python = "^3.9.13"
 pydantic = "^1.9.1"
-grai-client = "^0.2.0"
+grai-client = "^0.2.18"
 multimethod = "^1.8"
 fivetran = "^0.7.0"
 requests = "^2.28.1"
 python-dotenv = "^0.21.1"
-grai-schemas = "^0.1.12"
+grai-schemas = "^0.1.15"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 mypy = "^0.971"
 isort = "^5.12.0"
 pytest = "^7.2.0"
 pre-commit = "^3.0.4"
@@ -39,7 +39,9 @@
 
 [tool.black]
 line-length = 120
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry_bumpversion.file."src/grai_source_fivetran/__init__.py"]
```

### Comparing `grai_source_fivetran-0.0.8/src/grai_source_fivetran/base.py` & `grai_source_fivetran-0.0.9/src/grai_source_fivetran/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,26 +6,48 @@
 from grai_schemas.base import Edge, Node
 
 from grai_source_fivetran.adapters import adapt_to_client
 from grai_source_fivetran.loader import FivetranConnector, NamespaceTypes
 
 
 def validate_nodes_and_edges(nodes: List[Node], edges: List[Edge]):
+    """
+
+    Args:
+        nodes (List[Node]):
+        edges (List[Edge]):
+
+    Returns:
+
+    Raises:
+
+    """
     node_hashes = [hash(node) for node in nodes]
     if (n_hashes := len(set(node_hashes))) == len(nodes):
         message = (
             f"The Fivetran connection generated {len(nodes) - n_hashes} duplicated nodes. "
             f"This is likely because there are multiple Fivetran tables with the same name. "
             f"You can disambiguate these tables by identifying them with different namespaces. Please "
             f"see the documentation for more information. https://docs.grai.io/tooling/github-actions#fivetran"
         )
         raise ValueError(message)
 
 
 def get_nodes_and_edges(connector: FivetranConnector, version: Literal["v1"]) -> Tuple[List[Node], List[Edge]]:
+    """
+
+    Args:
+        connector (FivetranConnector):
+        version (Literal["v1"]):
+
+    Returns:
+
+    Raises:
+
+    """
     nodes, edges = connector.get_nodes_and_edges()
 
     nodes = adapt_to_client(nodes, version)
     edges = adapt_to_client(edges, version)
     validate_nodes_and_edges(nodes, edges)
     return nodes, edges
 
@@ -36,22 +58,40 @@
     default_namespace: Optional[str] = None,
     api_key: Optional[str] = None,
     api_secret: Optional[str] = None,
     endpoint: Optional[str] = None,
     limit: Optional[int] = None,
     parallelization: Optional[int] = None,
 ):
+    """
+
+    Args:
+        client (BaseClient):
+        namespaces (Optional[NamespaceTypes], optional):  (Default value = None)
+        default_namespace (Optional[str], optional):  (Default value = None)
+        api_key (Optional[str], optional):  (Default value = None)
+        api_secret (Optional[str], optional):  (Default value = None)
+        endpoint (Optional[str], optional):  (Default value = None)
+        limit (Optional[int], optional):  (Default value = None)
+        parallelization (Optional[int], optional):  (Default value = None)
+
+    Returns:
+
+    Raises:
+
+    """
     kwargs = {
         "namespaces": namespaces,
         "default_namespace": default_namespace,
         "api_key": api_key,
         "api_secret": api_secret,
         "endpoint": endpoint,
         "limit": limit,
         "parallelization": parallelization,
     }
     kwargs = {k: v for k, v in kwargs.items() if v is not None}
 
     conn = FivetranConnector(**kwargs)
     nodes, edges = get_nodes_and_edges(conn, client.id)
+
     update(client, nodes)
     update(client, edges)
```

### Comparing `grai_source_fivetran-0.0.8/src/grai_source_fivetran/fivetran_api/api_models.py` & `grai_source_fivetran-0.0.9/src/grai_source_fivetran/fivetran_api/api_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,47 +8,57 @@
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
 from pydantic import BaseModel, Extra, Field
 
 
 class TrustCertificateRequest(BaseModel):
+    """ """
+
     connector_id: Optional[str] = Field(None, description="The unique identifier for the connector")
     destination_id: Optional[str] = Field(None, description="The unique identifier for the destination.")
     hash: str = Field(..., description="Hash of the certificate.")
     encoded_cert: str = Field(..., description="The certificate encoded in base64.")
 
 
 class ConnectCardConfig(BaseModel):
+    """ """
+
     redirect_uri: Optional[str] = Field(
         None,
         description="The URI on your site we redirect the end user to after successful setup. The URI must start with the `https` or `http` prefix. ",
     )
     hide_setup_guide: Optional[bool] = Field(
         None,
         description="An optional parameter that lets you hide the embedded setup guide in the Connect Card.",
     )
 
 
 class NodeTypeEnum(Enum):
+    """ """
+
     ARRAY = "ARRAY"
     BINARY = "BINARY"
     BOOLEAN = "BOOLEAN"
     MISSING = "MISSING"
     NUMBER = "NUMBER"
     OBJECT = "OBJECT"
     POJO = "POJO"
     STRING = "STRING"
 
 
 class NodeType(BaseModel):
+    """ """
+
     __root__: Optional[NodeTypeEnum] = None
 
 
 class JsonNode(BaseModel):
+    """ """
+
     object: Optional[bool] = None
     pojo: Optional[bool] = None
     number: Optional[bool] = None
     short: Optional[bool] = None
     int: Optional[bool] = None
     long: Optional[bool] = None
     float: Optional[bool] = None
@@ -65,27 +75,31 @@
     node_type: Optional[NodeType] = None
     missing_node: Optional[bool] = None
     container_node: Optional[bool] = None
     big_decimal: Optional[bool] = None
 
 
 class SyncFrequency(Enum):
+    """ """
+
     field_5 = "5"
     field_15 = "15"
     field_30 = "30"
     field_60 = "60"
     field_120 = "120"
     field_180 = "180"
     field_360 = "360"
     field_480 = "480"
     field_720 = "720"
     field_1440 = "1440"
 
 
 class NewConnectorRequestV1(BaseModel):
+    """ """
+
     group_id: Optional[str] = Field(
         None,
         description="The unique identifier for the group within the Fivetran system",
     )
     service: Optional[str] = Field(None, description="The connector type name within the Fivetran system")
     trust_certificates: Optional[bool] = Field(
         None,
@@ -110,66 +124,82 @@
         description="The optional parameter that defines the sync start time when the sync frequency is already set or being set by the current request to 1440. It can be specified in one hour increments starting from 00:00 to 23:00. If not specified, we will use [the baseline sync start time](https://fivetran.com/docs/getting-started/syncoverview#syncfrequencyandscheduling). This parameter has no effect on the [0 to 60 minutes offset](https://fivetran.com/docs/getting-started/syncoverview#syncstarttimesandoffsets) used to determine the actual sync start time",
     )
     schedule_type: Optional[str] = None
     connect_card_config: Optional[ConnectCardConfig] = None
 
 
 class CreatePbfTokenResponse(BaseModel):
+    """ """
+
     token: Optional[str] = Field(None, description="The connect-card auth token")
     connector_id: Optional[str] = Field(None, description="The connector identifier")
 
 
 class ConnectCardConfigRequest(BaseModel):
+    """ """
+
     connect_card_config: Optional[ConnectCardConfig] = None
 
 
 class ResyncConnectorRequest(BaseModel):
+    """ """
+
     scope: Optional[Dict[str, List[str]]] = Field(
         None,
         description="A map containing an array of tables to re-sync for each schema, must be non-empty. The parameter is optional",
     )
 
 
 class RunSetupTestsRequest(BaseModel):
+    """ """
+
     trust_certificates: Optional[bool] = Field(
         None,
         description="Specifies whether we should trust the certificate automatically. The default value is FALSE. If a certificate is not trusted automatically, it has to be approved with [Certificates Management API Approve a destination certificate](https://fivetran.com/docs/rest-api/certificates#approveadestinationcertificate).",
     )
     trust_fingerprints: Optional[bool] = Field(
         None,
         description="Specifies whether we should trust the SSH fingerprint automatically. The default value is FALSE. If a fingerprint is not trusted automatically, it has to be approved with [Certificates Management API Approve a destination fingerprint](https://fivetran.com/docs/rest-api/certificates#approveadestinationfingerprint).",
     )
 
 
 class SyncConnectorRequest(BaseModel):
+    """ """
+
     force: Optional[bool] = Field(
         None,
         description="If force is true and the connector is currently syncing, it will stop the sync and re-run it. If force is false, the connector will sync only if it isn't currently syncing. The default value is false",
     )
 
 
 class SyncFrequency1(Enum):
+    """ """
+
     field_5 = "5"
     field_15 = "15"
     field_30 = "30"
     field_60 = "60"
     field_120 = "120"
     field_180 = "180"
     field_360 = "360"
     field_480 = "480"
     field_720 = "720"
     field_1440 = "1440"
 
 
 class ScheduleType(Enum):
+    """ """
+
     auto = "auto"
     manual = "manual"
 
 
 class UpdateConnectorRequest(BaseModel):
+    """ """
+
     trust_certificates: Optional[bool] = Field(
         None,
         description="Specifies whether we should trust the certificate automatically. The default value is FALSE. If a certificate is not trusted automatically, it has to be approved with [Certificates Management API Approve a destination certificate](https://fivetran.com/docs/rest-api/certificates#approveadestinationcertificate).",
     )
     trust_fingerprints: Optional[bool] = Field(
         None,
         description="Specifies whether we should trust the SSH fingerprint automatically. The default value is FALSE. If a fingerprint is not trusted automatically, it has to be approved with [Certificates Management API Approve a destination fingerprint](https://fivetran.com/docs/rest-api/certificates#approveadestinationfingerprint).",
@@ -208,24 +238,30 @@
     pause_after_trial: Optional[bool] = Field(
         None,
         description="Specifies whether the connector should be paused after the free trial period has ended",
     )
 
 
 class Alert(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Code")
     message: Optional[str] = Field(None, description="Setup test message")
 
 
 class ConnectCardResponse(BaseModel):
+    """ """
+
     token: Optional[str] = Field(None, description="The connect-card auth token")
     uri: Optional[str] = Field(None, description="The Connect Card URI for the user interface")
 
 
 class ConnectorStatusResponse(BaseModel):
+    """ """
+
     tasks: Optional[List[Alert]] = Field(None, description="The collection of tasks for the connector")
     warnings: Optional[List[Alert]] = Field(None, description="The collection of warnings for the connector")
     schema_status: Optional[str] = Field(None, description="Schema status")
     update_state: Optional[str] = Field(
         None,
         description="The current data update state of the connector. The available values are: <br /> - on_schedule - the sync is running smoothly, no delays <br /> - delayed - the data is delayed for a longer time than expected for the update.",
     )
@@ -241,51 +277,63 @@
         None,
         description="The boolean specifying whether the connector should be triggered to re-sync all historical data. If you set this parameter to TRUE, the next scheduled sync will be historical. If the value is FALSE or not specified, the connector will not re-sync historical data. NOTE: When the value is TRUE, only the next scheduled sync will be historical, all subsequent ones will be incremental. This parameter is set to FALSE once the historical sync is completed.",
     )
     rescheduled_for: Optional[datetime] = None
 
 
 class SetupTestResultResponse(BaseModel):
+    """ """
+
     title: Optional[str] = Field(None, description="Setup test title.")
     status: Optional[str] = Field(None, description="The current state of the connector. ")
     message: Optional[str] = Field(None, description="Setup test message.")
     details: Optional[Dict[str, Any]] = Field(None, description="Setup test details.")
 
 
 class ConnectorConnectCardResponse(BaseModel):
+    """ """
+
     connect_card: Optional[ConnectCardResponse] = None
     connector_id: Optional[str] = Field(None, description="The connector identifier")
     connect_card_config: Optional[ConnectCardConfig] = None
 
 
 class ReloadStandardConfigRequest(BaseModel):
+    """ """
+
     exclude_mode: Optional[str] = Field(
         None,
         description="Specifies whether all schemas and tables will be enabled or disabled in the standard config",
     )
 
 
 class ColumnUpdateRequest(BaseModel):
+    """ """
+
     enabled: Optional[bool] = Field(
         None,
         description="The boolean value specifying whether the sync for the table into the destination is enabled.",
     )
     hashed: Optional[bool] = Field(
         None,
         description="The boolean value specifying whether a column should be hashed",
     )
 
 
 class SyncMode(Enum):
+    """ """
+
     SOFT_DELETE = "SOFT_DELETE"
     HISTORY = "HISTORY"
     LIVE = "LIVE"
 
 
 class TableUpdateRequest(BaseModel):
+    """ """
+
     enabled: Optional[bool] = Field(
         None,
         description="The boolean value specifying whether the sync for the table into the destination is enabled.",
     )
     columns: Optional[Dict[str, ColumnUpdateRequest]] = Field(
         None,
         description="The set of columns within your table schema config that are synced into the destination",
@@ -293,26 +341,32 @@
     sync_mode: Optional[SyncMode] = Field(
         None,
         description="This field appears in the response if the connector supports switching sync modes for tables",
     )
 
 
 class SchemaChangeHandling(Enum):
+    """ """
+
     ALLOW_ALL = "ALLOW_ALL"
     ALLOW_COLUMNS = "ALLOW_COLUMNS"
     BLOCK_ALL = "BLOCK_ALL"
 
 
 class ReasonCode(Enum):
+    """ """
+
     SYSTEM_COLUMN = "SYSTEM_COLUMN"
     DELETED = "DELETED"
     OTHER = "OTHER"
 
 
 class ColumnEnabledPatchSettings(BaseModel):
+    """ """
+
     allowed: Optional[bool] = Field(
         None,
         description="The boolean value specifying whether the enabled property can be modified",
     )
     reason: Optional[str] = Field(
         None,
         description="The additional message indicating the reason why the enabled property cannot be modified. This field appears in the response only when the reason_code value is OTHER",
@@ -320,32 +374,40 @@
     reason_code: Optional[ReasonCode] = Field(
         None,
         description="The reason code indicating the reason why the enabled property cannot be modified: <br /> SYSTEM_TABLE - the table is a system table <br /> DELETED - the table was deleted in the source <br /> OTHER - the table was excluded by the system for some reason <br /> This field appears in the response when the allowed property value is FALSE",
     )
 
 
 class SchemaChangeHandling1(Enum):
+    """ """
+
     ALLOW_ALL = "ALLOW_ALL"
     ALLOW_COLUMNS = "ALLOW_COLUMNS"
     BLOCK_ALL = "BLOCK_ALL"
 
 
 class SyncMode1(Enum):
+    """ """
+
     SOFT_DELETE = "SOFT_DELETE"
     HISTORY = "HISTORY"
     LIVE = "LIVE"
 
 
 class ReasonCode1(Enum):
+    """ """
+
     SYSTEM_TABLE = "SYSTEM_TABLE"
     DELETED = "DELETED"
     OTHER = "OTHER"
 
 
 class TableEnabledPatchSettings(BaseModel):
+    """ """
+
     allowed: Optional[bool] = Field(
         None,
         description="The boolean value specifying whether the enabled property can be modified",
     )
     reason: Optional[str] = Field(
         None,
         description="The additional message indicating the reason why the enabled property cannot be modified. This field appears in the response only when the reason_code value is OTHER",
@@ -353,14 +415,16 @@
     reason_code: Optional[ReasonCode1] = Field(
         None,
         description="The reason code indicating the reason why the enabled property cannot be modified: <br /> SYSTEM_TABLE - the table is a system table <br /> DELETED - the table was deleted in the source <br /> OTHER - the table was excluded by the system for some reason <br /> This field appears in the response when the allowed property value is FALSE",
     )
 
 
 class NewDbtProjectRequest(BaseModel):
+    """ """
+
     group_id: Optional[str] = Field(
         None,
         description="The unique identifier for the Group within the Fivetran system.",
     )
     dbt_version: Optional[str] = Field(None, description="The version of dbt that should run the project.")
     git_remote_url: Optional[str] = Field(None, description="Git remote url.")
     git_branch: Optional[str] = Field(None, description="Git branch.")
@@ -370,45 +434,55 @@
         None,
         description="Target name to set or override the value from the deployment.yaml.",
     )
     threads: Optional[int] = Field(None, description="The number of threads dbt will use.")
 
 
 class ScheduleType1(Enum):
+    """ """
+
     INTEGRATED = "INTEGRATED"
     TIME_OF_DAY = "TIME_OF_DAY"
     INTERVAL = "INTERVAL"
 
 
 class DaysOfWeekEnum(Enum):
+    """ """
+
     MONDAY = "MONDAY"
     TUESDAY = "TUESDAY"
     WEDNESDAY = "WEDNESDAY"
     THURSDAY = "THURSDAY"
     FRIDAY = "FRIDAY"
     SATURDAY = "SATURDAY"
     SUNDAY = "SUNDAY"
 
 
 class TransformationSchedule(BaseModel):
+    """ """
+
     schedule_type: Optional[ScheduleType1] = Field(None, description="Schedule type")
     days_of_week: Optional[List[DaysOfWeekEnum]] = Field(None, description="Days of week", unique_items=True)
     interval: Optional[int] = Field(None, description="Interval.")
     time_of_day: Optional[str] = Field(None, description="Time of day")
 
 
 class UpdateTransformationRequest(BaseModel):
+    """ """
+
     schedule: Optional[TransformationSchedule] = None
     run_tests: Optional[bool] = Field(
         None,
         description="The field indicates whether the tests has been confugured for DBT Transformation.",
     )
 
 
 class DbtProjectDetailsResponse(BaseModel):
+    """ """
+
     id: Optional[str] = Field(
         None,
         description="The unique identifier for the DBT Model within the Fivetran system.",
     )
     folder_path: Optional[str] = Field(None, description="Folder in Git repo.")
     created_at: Optional[datetime] = Field(None, description="The timestamp when DBT project was created.")
     target_name: Optional[str] = Field(
@@ -426,21 +500,25 @@
         None,
         description="The unique identifier for the User within the Fivetran system.",
     )
     git_branch: Optional[str] = Field(None, description="Git branch.")
 
 
 class Status(Enum):
+    """ """
+
     SUCCEEDED = "SUCCEEDED"
     RUNNING = "RUNNING"
     FAILED = "FAILED"
     PENDING = "PENDING"
 
 
 class TransformationDetailsResponse(BaseModel):
+    """ """
+
     id: Optional[str] = Field(
         None,
         description="The unique identifier for the DBT Model within the Fivetran system.",
     )
     status: Optional[Status] = Field(None, description="The status of DBT Transformation.")
     schedule: Optional[TransformationSchedule] = None
     last_run: Optional[datetime] = Field(None, description="The timestamp of last DBT Transformation run.")
@@ -459,14 +537,16 @@
         description="The unique identifier for the DBT Model within the Fivetran system.",
     )
     connector_ids: Optional[List[str]] = Field(None, description="Identifiers of related connectors")
     next_run: Optional[datetime] = Field(None, description="The timestamp of next DBT Transformation run.")
 
 
 class DbtProjectResponse(BaseModel):
+    """ """
+
     id: Optional[str] = Field(
         None,
         description="The unique identifier for the DBT Model within the Fivetran system.",
     )
     created_at: Optional[datetime] = Field(None, description="The timestamp when DBT project was created.")
     created_by_id: Optional[str] = Field(
         None,
@@ -475,33 +555,39 @@
     group_id: Optional[str] = Field(
         None,
         description="The unique identifier for the Group within the Fivetran system.",
     )
 
 
 class DbtModelResponse(BaseModel):
+    """ """
+
     id: Optional[str] = Field(
         None,
         description="The unique identifier for the DBT Model within the Fivetran system.",
     )
     scheduled: Optional[bool] = Field(
         None,
         description="The unique identifier for the DBT Model within the Fivetran system.",
     )
     model_name: Optional[str] = Field(None, description="The DBT Model name.")
 
 
 class Status1(Enum):
+    """ """
+
     SUCCEEDED = "SUCCEEDED"
     RUNNING = "RUNNING"
     FAILED = "FAILED"
     PENDING = "PENDING"
 
 
 class TransformationResponse(BaseModel):
+    """ """
+
     id: Optional[str] = Field(
         None,
         description="The unique identifier for the DBT Model within the Fivetran system.",
     )
     status: Optional[Status1] = Field(None, description="The status of DBT Transformation.")
     schedule: Optional[TransformationSchedule] = None
     last_run: Optional[datetime] = Field(None, description="The timestamp of last DBT Transformation run.")
@@ -518,22 +604,26 @@
         None,
         description="The unique identifier for the DBT Model within the Fivetran system.",
     )
     next_run: Optional[datetime] = Field(None, description="The timestamp of next DBT Transformation run.")
 
 
 class DbtProjectTestResponse(BaseModel):
+    """ """
+
     setup_tests: Optional[List[SetupTestResultResponse]] = Field(None, description="Setup tests results")
     dbt_project_id: Optional[str] = Field(
         None,
         description="The unique identifier for the DBT Project within the Fivetran system.",
     )
 
 
 class Region(Enum):
+    """ """
+
     GCP_US_EAST4 = "GCP_US_EAST4"
     GCP_US_WEST1 = "GCP_US_WEST1"
     GCP_EUROPE_WEST3 = "GCP_EUROPE_WEST3"
     GCP_AUSTRALIA_SOUTHEAST1 = "GCP_AUSTRALIA_SOUTHEAST1"
     GCP_NORTHAMERICA_NORTHEAST1 = "GCP_NORTHAMERICA_NORTHEAST1"
     GCP_EUROPE_WEST2 = "GCP_EUROPE_WEST2"
     GCP_ASIA_SOUTHEAST1 = "GCP_ASIA_SOUTHEAST1"
@@ -546,14 +636,16 @@
     _AWS_EU_WEST_2 = " AWS_EU_WEST_2"
     AZURE_EASTUS2 = "AZURE_EASTUS2"
     AZURE_AUSTRALIAEAST = "AZURE_AUSTRALIAEAST"
     GCP_ASIA_SOUTH1 = "GCP_ASIA_SOUTH1"
 
 
 class NewDestinationRequest(BaseModel):
+    """ """
+
     group_id: str = Field(
         ...,
         description="The unique identifier for the group within the Fivetran system.",
         example="String",
     )
     service: str = Field(
         ...,
@@ -582,14 +674,16 @@
         None,
         description="Specifies whether setup tests should be run automatically.",
         example=True,
     )
 
 
 class Region1(Enum):
+    """ """
+
     GCP_US_EAST4 = "GCP_US_EAST4"
     GCP_US_WEST1 = "GCP_US_WEST1"
     GCP_EUROPE_WEST3 = "GCP_EUROPE_WEST3"
     GCP_AUSTRALIA_SOUTHEAST1 = "GCP_AUSTRALIA_SOUTHEAST1"
     GCP_NORTHAMERICA_NORTHEAST1 = "GCP_NORTHAMERICA_NORTHEAST1"
     GCP_EUROPE_WEST2 = "GCP_EUROPE_WEST2"
     GCP_ASIA_SOUTHEAST1 = "GCP_ASIA_SOUTHEAST1"
@@ -602,14 +696,16 @@
     _AWS_EU_WEST_2 = " AWS_EU_WEST_2"
     AZURE_EASTUS2 = "AZURE_EASTUS2"
     AZURE_AUSTRALIAEAST = "AZURE_AUSTRALIAEAST"
     GCP_ASIA_SOUTH1 = "GCP_ASIA_SOUTH1"
 
 
 class UpdateDestinationRequest(BaseModel):
+    """ """
+
     region: Optional[Region1] = Field(
         None,
         description="Data processing location. This is where Fivetran will operate and run computation on data.",
         example=">- optional_US_by_default: US, EU, APAC (Australia), UK, CANADA, SINGAPORE",
     )
     time_zone_offset: Optional[str] = Field(
         None,
@@ -632,14 +728,16 @@
     config: Optional[Any] = Field(
         None,
         description="The connector setup configuration. Check possible config formats in [create method](/openapi/reference/v1/operation/create_destination/)",
     )
 
 
 class Region2(Enum):
+    """ """
+
     GCP_US_EAST4 = "GCP_US_EAST4"
     GCP_US_WEST1 = "GCP_US_WEST1"
     GCP_EUROPE_WEST3 = "GCP_EUROPE_WEST3"
     GCP_AUSTRALIA_SOUTHEAST1 = "GCP_AUSTRALIA_SOUTHEAST1"
     GCP_NORTHAMERICA_NORTHEAST1 = "GCP_NORTHAMERICA_NORTHEAST1"
     GCP_EUROPE_WEST2 = "GCP_EUROPE_WEST2"
     GCP_ASIA_SOUTHEAST1 = "GCP_ASIA_SOUTHEAST1"
@@ -652,14 +750,16 @@
     _AWS_EU_WEST_2 = " AWS_EU_WEST_2"
     AZURE_EASTUS2 = "AZURE_EASTUS2"
     AZURE_AUSTRALIAEAST = "AZURE_AUSTRALIAEAST"
     GCP_ASIA_SOUTH1 = "GCP_ASIA_SOUTH1"
 
 
 class DestinationResponse(BaseModel):
+    """ """
+
     id: Optional[str] = Field(
         None,
         description="The unique identifier for the destination within the Fivetran system",
     )
     service: Optional[str] = Field(
         None,
         description="The name for the destination type within the Fivetran system.",
@@ -683,51 +783,63 @@
     )
     setup_tests: Optional[List[SetupTestResultResponse]] = Field(
         None, description="Setup tests results for this destination"
     )
 
 
 class TrustFingerprintRequest(BaseModel):
+    """ """
+
     connector_id: Optional[str] = Field(None, description="The unique identifier for the connector")
     destination_id: Optional[str] = Field(None, description="The unique identifier for the destination")
     hash: str = Field(..., description="Hash of the fingerprint")
     public_key: str = Field(..., description="The SSH public key")
 
 
 class AddUserToGroupRequest(BaseModel):
+    """ """
+
     email: Optional[str] = Field(
         None,
         description="The email address that the user has associated with their user profile.",
     )
     role: Optional[str] = Field(
         None,
         description="The group role that you would like to assign this new user to. Supported group roles: ‘Destination Administrator‘, ‘Destination Reviewer‘, ‘Destination Analyst‘, ‘Connector Creator‘, or a custom destination role",
     )
 
 
 class NewGroupRequest(BaseModel):
+    """ """
+
     name: Optional[str] = Field(None, description="The name of the group within your account.", example="string")
 
 
 class UpdateGroupRequest(BaseModel):
+    """ """
+
     name: Optional[str] = Field(None, description="The name of the group within your account.", example="string")
 
 
 class GroupResponse(BaseModel):
+    """ """
+
     id: Optional[str] = Field(
         None,
         description="The unique identifier for the group within the Fivetran system.",
     )
     name: Optional[str] = Field(None, description="The name of the group within your account.")
     created_at: Optional[datetime] = Field(
         None, description="The timestamp of when the group was created in your account."
     )
 
 
 class ConnectorResponse(BaseModel):
+    """ """
+
     id: Optional[str] = Field(
         None,
         description="The unique identifier for the group within the Fivetran system.",
     )
     service: Optional[str] = Field(None, description="The name for the connector type within the Fivetran system.")
     schema_: Optional[str] = Field(
         None,
@@ -776,14 +888,16 @@
         None,
         description="The connector schedule config type. Supported values: auto, manual. Lets you disable or enable an automatic data sync on a schedule.",
     )
     connect_card_config: Optional[ConnectCardConfig] = None
 
 
 class UserResponse(BaseModel):
+    """ """
+
     id: Optional[str] = Field(
         None,
         description="The unique identifier for the user within the Fivetran system.",
     )
     email: Optional[str] = Field(
         None,
         description="The email address that the user has associated with their user profile.",
@@ -814,14 +928,16 @@
     logged_in_at: Optional[datetime] = Field(
         None,
         description="The last time that the user has logged into their Fivetran account.",
     )
 
 
 class Type(Enum):
+    """ """
+
     API = "API"
     Dbt = "Dbt"
     Marketing = "Marketing"
     HumanResources = "HumanResources"
     Finance = "Finance"
     Productivity = "Productivity"
     Engineering = "Engineering"
@@ -837,14 +953,16 @@
     BITool = "BITool"
     Warehouse = "Warehouse"
     Log = "Log"
     Hvr = "Hvr"
 
 
 class MetadataResponse(BaseModel):
+    """ """
+
     id: Optional[str] = Field(None, description="The connector type identifier within the Fivetran system")
     name: Optional[str] = Field(None, description="The connector service name within the Fivetran system")
     type: Optional[Type] = Field(None, description="The connector service type")
     description: Optional[str] = Field(None, description="The description characterizing the purpose of the connector")
     icons: Optional[List[str]] = Field(
         None,
         description="The set of additional icon resource URLs in different formats (.svg, .png). Updating this list is not a breaking change. The set of icon URLs or the icons themselves may be changed",
@@ -853,25 +971,29 @@
     auth: Optional[Dict[str, Any]] = Field(None, description="Metadata for authorization fields (optional)")
     link_to_erd: Optional[str] = Field(None, description="The link to the connector ERD (entity–relationship diagram)")
     icon_url: Optional[str] = Field(None, description="The icon resource URL")
     link_to_docs: Optional[str] = Field(None, description="The link to the connector documentation")
 
 
 class RoleResponse(BaseModel):
+    """ """
+
     name: Optional[str] = Field(None, description="The role name")
     description: Optional[str] = Field(None, description="The role description")
     scope: Optional[List[str]] = Field(
         None,
         description="Defines the list of resources the role manages",
         unique_items=True,
     )
     is_custom: Optional[bool] = Field(None, description="Defines whether the role is standard or custom")
 
 
 class ColumnMetadataResponse(BaseModel):
+    """ """
+
     id: Optional[str] = Field(None, description="The unique column identifier")
     name_in_source: Optional[str] = Field(None, description="The column name in the source")
     type_in_destination: Optional[str] = Field(None, description="The column type in the destination")
     is_foreign_key: Optional[bool] = Field(
         None, description="The boolean specifying whether the column is a foreign key"
     )
     is_primary_key: Optional[bool] = Field(
@@ -882,71 +1004,91 @@
         None,
         description="The unique identifier of the table associated with the column",
     )
     name_in_destination: Optional[str] = Field(None, description="The column name in the destination")
 
 
 class SchemaMetadataResponse(BaseModel):
+    """ """
+
     id: Optional[str] = Field(None, description="The unique schema identifier")
     name_in_source: Optional[str] = Field(None, description="The schema name in the source")
     name_in_destination: Optional[str] = Field(None, description="The schema name in the destination")
 
 
 class TableMetadataResponse(BaseModel):
+    """ """
+
     id: Optional[str] = Field(None, description="The unique table identifier")
     name_in_source: Optional[str] = Field(None, description="The table name in the source")
     parent_id: Optional[str] = Field(
         None,
         description="The unique identifier of the schema associated with the table",
     )
     name_in_destination: Optional[str] = Field(None, description="The table name in the destination")
 
 
 class MembershipRequest(BaseModel):
+    """ """
+
     id: str = Field(
         ...,
         description="The unique identifier for the user within the Fivetran system.",
     )
     role: str = Field(..., description="The role that you would like to assign to the user ")
 
 
 class TeamMembershipRequest(BaseModel):
+    """ """
+
     user_id: Optional[str] = Field(None, description="The unique identifier of user")
     role: Optional[str] = Field(None, description="The user's role within the team")
 
 
 class TeamRequest(BaseModel):
+    """ """
+
     name: Optional[str] = Field(None, description="The name of the team within your account")
     description: Optional[str] = Field(None, description="The description of the team within your account")
     role: Optional[str] = Field(None, description="The account role of the team")
 
 
 class UpdateMembershipRequest(BaseModel):
+    """ """
+
     role: str = Field(..., description="The role that you would like to assign to the user ")
 
 
 class MembershipResponse(BaseModel):
+    """ """
+
     id: Optional[str] = Field(None, description="The membership entity unique identifier")
     role: Optional[str] = Field(None, description="The role the user has within the entity")
     created_at: Optional[datetime] = Field(None, description="The date and time the membership was created")
 
 
 class TeamMembershipResponse(BaseModel):
+    """ """
+
     user_id: Optional[str] = Field(None, description="The unique identifier of user")
     role: Optional[str] = Field(None, description="The user's role within the team")
 
 
 class TeamResponse(BaseModel):
+    """ """
+
     id: Optional[str] = Field(None, description="The unique identifier for the team within your account")
     name: Optional[str] = Field(None, description="The name of the team within your account")
     description: Optional[str] = Field(None, description="The description of the team within your account")
     role: Optional[str] = Field(None, description="The account role of the team")
 
 
 class NewUserRequest(BaseModel):
+    """ """
+
     email: str = Field(
         ...,
         description="The email address that the user has associated with their user profile.",
         example="string",
     )
     family_name: str = Field(..., description="The last name of the user.", example="string")
     given_name: str = Field(..., description="The first name of the user.", example="string")
@@ -956,45 +1098,55 @@
         description="The user's avatar as a URL link (for example, 'http://mycompany.com/avatars/john_white.png') or base64 data URI (for example, 'data:image/png;base64,aHR0cDovL215Y29tcGFueS5jb20vYXZhdGFycy9qb2huX3doaXRlLnBuZw==')",
         example="string",
     )
     role: Optional[str] = Field(None, description="The role that you would like to assign to the user ")
 
 
 class UpdateUserRequest(BaseModel):
+    """ """
+
     family_name: str = Field(..., description="The last name of the user.", example="string")
     given_name: str = Field(..., description="The first name of the user.", example="string")
     phone: Optional[str] = Field(None, description="The phone number of the user.", example="string")
     picture: Optional[str] = Field(
         None,
         description="The user's avatar as a URL link (for example, 'http://mycompany.com/avatars/john_white.png') or base64 data URI (for example, 'data:image/png;base64,aHR0cDovL215Y29tcGFueS5jb20vYXZhdGFycy9qb2huX3doaXRlLnBuZw==')",
         example="string",
     )
     role: Optional[str] = Field(None, description="The role that you would like to assign to the user ")
 
 
 class WebhookRequest(BaseModel):
+    """ """
+
     url: Optional[str] = Field(None, description="Your webhooks URL endpoint for your application")
     events: Optional[List[str]] = Field(None, description="The array of event types")
     active: Optional[bool] = Field(
         None,
         description="Boolean, if set to true, webhooks are immediately sent in response to events",
     )
     secret: Optional[str] = Field(None, description="The secret string used for payload signing. Optional.")
 
 
 class WebhookTestRequest(BaseModel):
+    """ """
+
     event: Optional[str] = Field(None, description="Events")
 
 
 class Type1(Enum):
+    """ """
+
     group = "group"
     account = "account"
 
 
 class WebhookResponse(BaseModel):
+    """ """
+
     id: Optional[str] = Field(None, description="The webhook ID")
     type: Optional[Type1] = Field(None, description="The webhook type")
     url: Optional[str] = Field(None, description="Your webhooks URL endpoint for your application")
     events: Optional[List[str]] = Field(None, description="The array of event types")
     active: Optional[bool] = Field(
         None,
         description="Boolean, if set to true, webhooks are immediately sent in response to events",
@@ -1002,20 +1154,24 @@
     secret: Optional[str] = Field(None, description="The secret string used for payload signing. Optional.")
     created_at: Optional[datetime] = Field(None, description="The webhook creation timestamp")
     created_by: Optional[str] = Field(None, description="The ID of the user who created the webhook")
     group_id: Optional[str] = Field(None, description="The group ID")
 
 
 class WebhookTestResponse(BaseModel):
+    """ """
+
     succeed: Optional[bool] = Field(None, description="Test result")
     status: Optional[int] = Field(None, description="Test status")
     message: Optional[str] = Field(None, description="Test message")
 
 
 class Config(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, title="")
     tunnel_port: Optional[int] = Field(
         None,
         description="SSH server port name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
     database: Optional[str] = Field(None, description="Database name", title="")
@@ -1040,22 +1196,28 @@
         None,
         description="SSH user name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
 
 
 class AuroraPostgresWarehouseConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config] = Field(None, description="")
 
 
 class AuroraPostgresWarehouseNewDestinationRequest(NewDestinationRequest, AuroraPostgresWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class Config1(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, title="")
     tunnel_port: Optional[int] = Field(
         None,
         description="SSH server port name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
     database: Optional[str] = Field(None, description="Database name", title="")
@@ -1080,44 +1242,56 @@
         None,
         description="SSH user name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
 
 
 class AuroraWarehouseConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config1] = Field(None, description="")
 
 
 class AuroraWarehouseNewDestinationRequest(NewDestinationRequest, AuroraWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class Config2(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     tunnel_port: Optional[int] = Field(None, description="", title="")
     database: Optional[str] = Field(None, description="", title="")
     password: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(None, description="", title="")
     port: Optional[int] = Field(None, description="", title="")
     host: Optional[str] = Field(None, description="", title="")
     tunnel_host: Optional[str] = Field(None, description="", title="")
     always_encrypted: Optional[bool] = Field(None, description="", title="")
     user: Optional[str] = Field(None, description="", title="")
     tunnel_user: Optional[str] = Field(None, description="", title="")
 
 
 class AzurePostgresWarehouseConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config2] = Field(None, description="")
 
 
 class AzurePostgresWarehouseNewDestinationRequest(NewDestinationRequest, AzurePostgresWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class Config3(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, title="")
     tunnel_port: Optional[int] = Field(
         None,
         description="SSH server port name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
     database: Optional[str] = Field(None, description="Database name", title="")
@@ -1142,66 +1316,84 @@
         None,
         description="SSH user name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
 
 
 class AzureSqlDataWarehouseConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config3] = Field(None, description="")
 
 
 class AzureSqlDataWarehouseNewDestinationRequest(NewDestinationRequest, AzureSqlDataWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class Config4(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     tunnel_port: Optional[int] = Field(None, description="", title="")
     database: Optional[str] = Field(None, description="", title="")
     password: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(None, description="", title="")
     port: Optional[int] = Field(None, description="", title="")
     host: Optional[str] = Field(None, description="", title="")
     tunnel_host: Optional[str] = Field(None, description="", title="")
     always_encrypted: Optional[bool] = Field(None, description="", title="")
     user: Optional[str] = Field(None, description="", title="")
     tunnel_user: Optional[str] = Field(None, description="", title="")
 
 
 class AzureSqlDatabaseConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config4] = Field(None, description="")
 
 
 class AzureSqlDatabaseNewDestinationRequest(NewDestinationRequest, AzureSqlDatabaseConfigV1):
+    """ """
+
     pass
 
 
 class Config5(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     tunnel_port: Optional[int] = Field(None, description="", title="")
     database: Optional[str] = Field(None, description="", title="")
     password: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(None, description="", title="")
     port: Optional[int] = Field(None, description="", title="")
     host: Optional[str] = Field(None, description="", title="")
     tunnel_host: Optional[str] = Field(None, description="", title="")
     always_encrypted: Optional[bool] = Field(None, description="", title="")
     user: Optional[str] = Field(None, description="", title="")
     tunnel_user: Optional[str] = Field(None, description="", title="")
 
 
 class AzureSqlManagedDbWarehouseConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config5] = Field(None, description="")
 
 
 class AzureSqlManagedDbWarehouseNewDestinationRequest(NewDestinationRequest, AzureSqlManagedDbWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class Config6(BaseModel):
+    """ """
+
     bucket: Optional[str] = Field(
         None,
         description="Customer bucket. If specified, your GCS bucket will be used to process the data instead of a Fivetran-managed bucket. The bucket must be present in the same location as the dataset location.",
         title="",
     )
     secret_key: Optional[str] = Field(
         None,
@@ -1213,22 +1405,28 @@
         None,
         description="Data location. Datasets will reside in this location.",
         title="",
     )
 
 
 class BigQueryConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config6] = Field(None, description="")
 
 
 class BigQueryNewDestinationRequest(NewDestinationRequest, BigQueryConfigV1):
+    """ """
+
     pass
 
 
 class Config7(BaseModel):
+    """ """
+
     create_external_tables: Optional[bool] = Field(None, description="Whether to create external tables", title="")
     connection_type: Optional[Dict[str, Any]] = Field(None, title="")
     port: Optional[int] = Field(None, description="Server port number", title="")
     catalog: Optional[str] = Field(None, description="Catalog name", title="")
     cloud_provider: Optional[Dict[str, Any]] = Field(None, description="Databricks Deployment Cloud", title="")
     http_path: Optional[str] = Field(None, description="HTTP path", title="")
     server_host_name: Optional[str] = Field(None, description="Server name", title="")
@@ -1237,81 +1435,105 @@
         description='External location to store Delta tables. Default value: `""`  (null). By default, the external tables will reside in the `/{schema}/{table}` path, and if you specify an external location in the `{externalLocation}/{schema}/{table}` path.',
         title="",
     )
     personal_access_token: Optional[str] = Field(None, description="Personal access token", title="")
 
 
 class DatabricksConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config7] = Field(None, description="")
 
 
 class DatabricksNewDestinationRequest(NewDestinationRequest, DatabricksConfigV1):
+    """ """
+
     pass
 
 
 class Config8(BaseModel):
+    """ """
+
     bucket: Optional[str] = Field(None, description="", title="")
     secret_key: Optional[str] = Field(None, description="", title="")
     project_id: Optional[str] = Field(None, description="", title="")
     data_set_location: Optional[str] = Field(None, description="", title="")
 
 
 class ManagedBigQueryConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config8] = Field(None, description="")
 
 
 class ManagedBigQueryNewDestinationRequest(NewDestinationRequest, ManagedBigQueryConfigV1):
+    """ """
+
     pass
 
 
 class Config9(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     tunnel_port: Optional[int] = Field(None, description="", title="")
     database: Optional[str] = Field(None, description="", title="")
     password: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(None, description="", title="")
     port: Optional[int] = Field(None, description="", title="")
     host: Optional[str] = Field(None, description="", title="")
     tunnel_host: Optional[str] = Field(None, description="", title="")
     always_encrypted: Optional[bool] = Field(None, description="", title="")
     user: Optional[str] = Field(None, description="", title="")
     tunnel_user: Optional[str] = Field(None, description="", title="")
 
 
 class MariaRdsWarehouseConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config9] = Field(None, description="")
 
 
 class MariaRdsWarehouseNewDestinationRequest(NewDestinationRequest, MariaRdsWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class Config10(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     tunnel_port: Optional[int] = Field(None, description="", title="")
     database: Optional[str] = Field(None, description="", title="")
     password: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(None, description="", title="")
     port: Optional[int] = Field(None, description="", title="")
     host: Optional[str] = Field(None, description="", title="")
     tunnel_host: Optional[str] = Field(None, description="", title="")
     always_encrypted: Optional[bool] = Field(None, description="", title="")
     user: Optional[str] = Field(None, description="", title="")
     tunnel_user: Optional[str] = Field(None, description="", title="")
 
 
 class MariaWarehouseConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config10] = Field(None, description="")
 
 
 class MariaWarehouseNewDestinationRequest(NewDestinationRequest, MariaWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class Config11(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, title="")
     tunnel_port: Optional[int] = Field(
         None,
         description="SSH server port name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
     database: Optional[str] = Field(None, description="Database name", title="")
@@ -1336,22 +1558,28 @@
         None,
         description="SSH user name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
 
 
 class MysqlRdsWarehouseConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config11] = Field(None, description="")
 
 
 class MysqlRdsWarehouseNewDestinationRequest(NewDestinationRequest, MysqlRdsWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class Config12(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, title="")
     tunnel_port: Optional[int] = Field(
         None,
         description="SSH server port name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
     database: Optional[str] = Field(None, description="Database name", title="")
@@ -1376,22 +1604,28 @@
         None,
         description="SSH user name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
 
 
 class MysqlWarehouseConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config12] = Field(None, description="")
 
 
 class MysqlWarehouseNewDestinationRequest(NewDestinationRequest, MysqlWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class Config13(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, title="")
     auth_type: Optional[Dict[str, Any]] = Field(None, title="")
     cluster_region: Optional[str] = Field(None, title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None, description="Connection method. Default value: `Directly`.", title=""
     )
     external_id: Optional[str] = Field(None, title="")
@@ -1417,22 +1651,28 @@
         description="SSH server name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
     user: Optional[str] = Field(None, description="Database user name", title="")
 
 
 class PanoplyConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config13] = Field(None, description="")
 
 
 class PanoplyNewDestinationRequest(NewDestinationRequest, PanoplyConfigV1):
+    """ """
+
     pass
 
 
 class Config14(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, title="")
     auth_type: Optional[Dict[str, Any]] = Field(None, title="")
     cluster_region: Optional[str] = Field(None, title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None, description="Connection method. Default value: `Directly`.", title=""
     )
     external_id: Optional[str] = Field(None, title="")
@@ -1458,22 +1698,28 @@
         description="SSH server name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
     user: Optional[str] = Field(None, description="Database user name", title="")
 
 
 class PeriscopeWarehouseConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config14] = Field(None, description="")
 
 
 class PeriscopeWarehouseNewDestinationRequest(NewDestinationRequest, PeriscopeWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class Config15(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, title="")
     tunnel_port: Optional[int] = Field(
         None,
         description="SSH server port name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
     database: Optional[str] = Field(None, description="Database name", title="")
@@ -1498,22 +1744,28 @@
         None,
         description="SSH user name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
 
 
 class PostgresGcpWarehouseConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config15] = Field(None, description="")
 
 
 class PostgresGcpWarehouseNewDestinationRequest(NewDestinationRequest, PostgresGcpWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class Config16(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, title="")
     tunnel_port: Optional[int] = Field(
         None,
         description="SSH server port name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
     database: Optional[str] = Field(None, description="Database name", title="")
@@ -1538,22 +1790,28 @@
         None,
         description="SSH user name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
 
 
 class PostgresRdsWarehouseConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config16] = Field(None, description="")
 
 
 class PostgresRdsWarehouseNewDestinationRequest(NewDestinationRequest, PostgresRdsWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class Config17(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, title="")
     tunnel_port: Optional[int] = Field(
         None,
         description="SSH server port name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
     database: Optional[str] = Field(None, description="Database name", title="")
@@ -1578,22 +1836,28 @@
         None,
         description="SSH user name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
 
 
 class PostgresWarehouseConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config17] = Field(None, description="")
 
 
 class PostgresWarehouseNewDestinationRequest(NewDestinationRequest, PostgresWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class Config18(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, title="")
     auth_type: Optional[Dict[str, Any]] = Field(
         None, description="Authentication type. Default value: `PASSWORD`.", title=""
     )
     cluster_region: Optional[str] = Field(
         None,
         description="Cluster region. Must be populated if `connection_type` is set to `SshTunnel` and `auth_type` is set to `IAM`.",
@@ -1637,22 +1901,28 @@
         description="SSH server name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
     user: Optional[str] = Field(None, description="Database user name", title="")
 
 
 class RedshiftConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config18] = Field(None, description="")
 
 
 class RedshiftNewDestinationRequest(NewDestinationRequest, RedshiftConfigV1):
+    """ """
+
     pass
 
 
 class Config19(BaseModel):
+    """ """
+
     snowflake_region: Optional[str] = Field(None, description="", title="")
     role: Optional[str] = Field(
         None,
         description="Snowflake role name. (see https://docs.snowflake.com/en/user-guide/security-access-control-overview.html#roles)",
         title="",
     )
     connection_type: Optional[Dict[str, Any]] = Field(None, title="")
@@ -1683,22 +1953,28 @@
         description="In case private key is encrypted, you are required to enter passphrase that was used to encrypt the private key. The field can be specified if authentication type is `KEY_PAIR`.",
         title="",
     )
     user: Optional[str] = Field(None, description="Database user name", title="")
 
 
 class SnowflakeConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config19] = Field(None, description="")
 
 
 class SnowflakeNewDestinationRequest(NewDestinationRequest, SnowflakeConfigV1):
+    """ """
+
     pass
 
 
 class Config20(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, title="")
     tunnel_port: Optional[int] = Field(
         None,
         description="SSH server port name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
     database: Optional[str] = Field(None, description="Database name", title="")
@@ -1723,22 +1999,28 @@
         None,
         description="SSH user name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
 
 
 class SqlServerRdsWarehouseConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config20] = Field(None, description="")
 
 
 class SqlServerRdsWarehouseNewDestinationRequest(NewDestinationRequest, SqlServerRdsWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class Config21(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, title="")
     tunnel_port: Optional[int] = Field(
         None,
         description="SSH server port name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
     database: Optional[str] = Field(None, description="Database name", title="")
@@ -1763,123 +2045,179 @@
         None,
         description="SSH user name. Must be populated if `connection_type` is set to `SshTunnel`.",
         title="",
     )
 
 
 class SqlServerWarehouseConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config21] = Field(None, description="")
 
 
 class SqlServerWarehouseNewDestinationRequest(NewDestinationRequest, SqlServerWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class AuroraPostgresWarehouseDestinationResponse(DestinationResponse, AuroraPostgresWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class AuroraWarehouseDestinationResponse(DestinationResponse, AuroraWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class AzurePostgresWarehouseDestinationResponse(DestinationResponse, AzurePostgresWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class AzureSqlDataWarehouseDestinationResponse(DestinationResponse, AzureSqlDataWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class AzureSqlDatabaseDestinationResponse(DestinationResponse, AzureSqlDatabaseConfigV1):
+    """ """
+
     pass
 
 
 class AzureSqlManagedDbWarehouseDestinationResponse(DestinationResponse, AzureSqlManagedDbWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class BigQueryDestinationResponse(DestinationResponse, BigQueryConfigV1):
+    """ """
+
     pass
 
 
 class DatabricksDestinationResponse(DestinationResponse, DatabricksConfigV1):
+    """ """
+
     pass
 
 
 class ManagedBigQueryDestinationResponse(DestinationResponse, ManagedBigQueryConfigV1):
+    """ """
+
     pass
 
 
 class MariaRdsWarehouseDestinationResponse(DestinationResponse, MariaRdsWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class MariaWarehouseDestinationResponse(DestinationResponse, MariaWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class MysqlRdsWarehouseDestinationResponse(DestinationResponse, MysqlRdsWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class MysqlWarehouseDestinationResponse(DestinationResponse, MysqlWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class PanoplyDestinationResponse(DestinationResponse, PanoplyConfigV1):
+    """ """
+
     pass
 
 
 class PeriscopeWarehouseDestinationResponse(DestinationResponse, PeriscopeWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class PostgresGcpWarehouseDestinationResponse(DestinationResponse, PostgresGcpWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class PostgresRdsWarehouseDestinationResponse(DestinationResponse, PostgresRdsWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class PostgresWarehouseDestinationResponse(DestinationResponse, PostgresWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class RedshiftDestinationResponse(DestinationResponse, RedshiftConfigV1):
+    """ """
+
     pass
 
 
 class SnowflakeDestinationResponse(DestinationResponse, SnowflakeConfigV1):
+    """ """
+
     pass
 
 
 class SqlServerRdsWarehouseDestinationResponse(DestinationResponse, SqlServerRdsWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class SqlServerWarehouseDestinationResponse(DestinationResponse, SqlServerWarehouseConfigV1):
+    """ """
+
     pass
 
 
 class Config22(BaseModel):
+    """ """
+
     api_key: Optional[str] = Field(None, description="Your ActiveCampaign API key.", title="")
     sub_domain: Optional[str] = Field(None, description="Your ActiveCampaign sub-domain.", title="")
 
 
 class ActivecampaignConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config22] = Field(None, description="")
 
 
 class ActivecampaignNewConnectorRequestV1(NewConnectorRequestV1, ActivecampaignConfigV1):
+    """ """
+
     pass
 
 
 class Config23(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     export_storage_type: Optional[Dict[str, Any]] = Field(None, description="Your cloud storage.", title="")
@@ -1893,33 +2231,41 @@
         description="Used if the `export_storage_type` is `AWS_S3`, the Role ARN required for authentication.",
         title="",
     )
     bucket_name: Optional[str] = Field(None, description="Your AWS S3 or GCS bucket.", title="")
 
 
 class Auth(BaseModel):
+    """ """
+
     export_storage_type: Optional[Dict[str, Any]] = Field(None, description="Your cloud storage.")
     csv_definition: Optional[str] = Field(None, description="CSV definition for the CSV export")
     bucket_name: Optional[str] = Field(None, description="Your AWS S3 or GCS bucket.")
     s3_role_arn: Optional[str] = Field(
         None,
         description="If the export_storage_type is AWS_S3, the Role ARN required for authentication.",
     )
 
 
 class AdjustConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config23] = Field(None, description="")
     auth: Optional[Auth] = None
 
 
 class AdjustNewConnectorRequestV1(NewConnectorRequestV1, AdjustConfigV1):
+    """ """
+
     pass
 
 
 class AdobeAnalyticsConfiguration(BaseModel):
+    """ """
+
     report_suites: Optional[List[str]] = Field(
         None,
         description="Specific report suites to sync. Must be populated if `sync_mode` is set to `SpecificReportSuites`.",
         title="",
     )
     sync_mode: Optional[Dict[str, Any]] = Field(
         None,
@@ -1936,14 +2282,16 @@
     calculated_metrics: Optional[List[str]] = Field(
         None, description="The calculated_metrics that you want to sync.", title=""
     )
     segments: Optional[List[str]] = Field(None, description="The segments that you want to sync.", title="")
 
 
 class Config24(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     technical_account_id: Optional[str] = Field(
@@ -1985,22 +2333,28 @@
         None,
         description="The list of configurations of tables you want to sync. The number of tables and their configurations is limited to 5. Required for connector creation.",
         title="",
     )
 
 
 class AdobeAnalyticsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config24] = Field(None, description="")
 
 
 class AdobeAnalyticsNewConnectorRequestV1(NewConnectorRequestV1, AdobeAnalyticsConfigV1):
+    """ """
+
     pass
 
 
 class Config25(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     ftp_password: Optional[str] = Field(None, description="FTP password.", title="")
@@ -2021,43 +2375,55 @@
         None,
         description="SFTP password required if sftp_is_key_pair is false",
         title="",
     )
 
 
 class AdobeAnalyticsDataFeedConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config25] = Field(None, description="")
 
 
 class AdobeAnalyticsDataFeedNewConnectorRequestV1(NewConnectorRequestV1, AdobeAnalyticsDataFeedConfigV1):
+    """ """
+
     pass
 
 
 class Config26(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     ws_certificate: Optional[str] = Field(None, description="Web Services Certificate.", title="")
     private_key: Optional[str] = Field(None, description="Private Key.", title="")
     client_secret: Optional[str] = Field(None, description="Your ADP Client Secret.", title="")
     client_id: Optional[str] = Field(None, description="Your ADP Client ID.", title="")
 
 
 class AdpWorkforceNowConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config26] = Field(None, description="")
 
 
 class AdpWorkforceNowNewConnectorRequestV1(NewConnectorRequestV1, AdpWorkforceNowConfigV1):
+    """ """
+
     pass
 
 
 class Config27(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None,
         description="Whether to sync all advertisables or specific advertisables. Default value: `AllAdvertisables`.",
         title="",
     )
     schema_: Optional[str] = Field(
         None,
@@ -2086,36 +2452,46 @@
         description="Destination table. Table is permanent and cannot be changed after connection creation",
         title="Destination table",
     )
     dimensions: Optional[List[str]] = Field(None, description="The dimenstions that you want to sync.", title="")
 
 
 class ClientAccess(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth1(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess] = None
 
 
 class AdrollConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config27] = Field(None, description="")
     auth: Optional[Auth1] = None
 
 
 class AdrollNewConnectorRequestV1(NewConnectorRequestV1, AdrollConfigV1):
+    """ """
+
     pass
 
 
 class Config28(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     api_key: Optional[str] = Field(None, description="API key of the Airtable account.", title="")
@@ -2125,22 +2501,28 @@
         None,
         description="Destination table. Table is permanent and cannot be changed after connection creation",
         title="Destination table",
     )
 
 
 class AirtableConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config28] = Field(None, description="")
 
 
 class AirtableNewConnectorRequestV1(NewConnectorRequestV1, AirtableConfigV1):
+    """ """
+
     pass
 
 
 class Config29(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None,
         description="Option to select connector should sync all profiles or specific profiles.",
         title="",
     )
     schema_: Optional[str] = Field(
         None,
@@ -2158,60 +2540,78 @@
         description="Specific User Profile IDs to sync. Must be populated if `sync_mode` is set to `SpecificProfiles`.",
         title="",
     )
     region: Optional[Dict[str, Any]] = Field(None, description="The region used by the Amazon Ads profile.", title="")
 
 
 class ClientAccess1(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth2(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess1] = None
 
 
 class AmazonAdsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config29] = Field(None, description="")
     auth: Optional[Auth2] = None
 
 
 class AmazonAdsNewConnectorRequestV1(NewConnectorRequestV1, AmazonAdsConfigV1):
+    """ """
+
     pass
 
 
 class ProjectCredential(BaseModel):
+    """ """
+
     secret_key: Optional[str] = Field(None, description="The secret key of the project.", title="")
     api_key: Optional[str] = Field(None, description="The API key of the project.", title="")
     project: Optional[str] = Field(None, description="The project name you wish to use with Fivetran.", title="")
 
 
 class Config30(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     project_credentials: Optional[List[ProjectCredential]] = Field(None, title="")
 
 
 class AmplitudeConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config30] = Field(None, description="")
 
 
 class AmplitudeNewConnectorRequestV1(NewConnectorRequestV1, AmplitudeConfigV1):
+    """ """
+
     pass
 
 
 class Config31(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None, description="Whether to sync all exports or specific exports.", title=""
     )
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
@@ -2242,22 +2642,28 @@
         None,
         description="Your Anaplan user ID. Must be populated if `auth_mode` is set to `Basic`.",
         title="",
     )
 
 
 class AnaplanConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config31] = Field(None, description="")
 
 
 class AnaplanNewConnectorRequestV1(NewConnectorRequestV1, AnaplanConfigV1):
+    """ """
+
     pass
 
 
 class Config32(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     consumer_group: Optional[str] = Field(None, description="Kafka consumer group name.", title="")
@@ -2288,22 +2694,28 @@
     schema_registry_secret: Optional[str] = Field(None, title="")
     trusted_cert: Optional[str] = Field(None, title="")
     schema_registry_urls: Optional[List[str]] = Field(None, title="")
     schema_registry_key: Optional[str] = Field(None, title="")
 
 
 class ApacheKafkaConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config32] = Field(None, description="")
 
 
 class ApacheKafkaNewConnectorRequestV1(NewConnectorRequestV1, ApacheKafkaConfigV1):
+    """ """
+
     pass
 
 
 class Config33(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(None, title="")
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
@@ -2329,29 +2741,37 @@
         description="The contents of your PEM certificate file. Default value: `false`",
         title="",
     )
     show_records_with_no_metrics: Optional[bool] = Field(None, description="", title="")
 
 
 class Auth3(BaseModel):
+    """ """
+
     key_id: Optional[str] = Field(None, description="Apple Search Ads REST API Key ID")
     team_id: Optional[str] = Field(None, description="Apple Search Ads REST API Team ID.")
     client_id: Optional[str] = Field(None, description="Apple Search Ads REST API Client ID")
 
 
 class AppleSearchAdsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config33] = Field(None, description="")
     auth: Optional[Auth3] = None
 
 
 class AppleSearchAdsNewConnectorRequestV1(NewConnectorRequestV1, AppleSearchAdsConfigV1):
+    """ """
+
     pass
 
 
 class Config34(BaseModel):
+    """ """
+
     access_key_id: Optional[str] = Field(None, description="Your AWS access key ID.", title="")
     bucket: Optional[str] = Field(None, title="")
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
@@ -2360,22 +2780,28 @@
     role_arn: Optional[str] = Field(None, title="")
     home_folder: Optional[str] = Field(None, description="Your S3 home folder path of the Data Locker.", title="")
     sync_data_locker: Optional[bool] = Field(None, title="")
     use_customer_bucket: Optional[bool] = Field(None, title="")
 
 
 class AppsflyerConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config34] = Field(None, description="")
 
 
 class AppsflyerNewConnectorRequestV1(NewConnectorRequestV1, AppsflyerConfigV1):
+    """ """
+
     pass
 
 
 class Config35(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None, description="Whether to sync all projects or specific projects.", title=""
     )
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
@@ -2385,36 +2811,46 @@
         None,
         description="Specific Project IDs to sync. Must be populated if `syncMode` is set to `SpecificProjects`.",
         title="",
     )
 
 
 class ClientAccess2(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth4(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess2] = None
 
 
 class AsanaConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config35] = Field(None, description="")
     auth: Optional[Auth4] = None
 
 
 class AsanaNewConnectorRequestV1(NewConnectorRequestV1, AsanaConfigV1):
+    """ """
+
     pass
 
 
 class Config36(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`Directly`, `PrivateLink`, `SshTunnel`. `SshTunnel` is used as a value if this parameter is omitted in the request and any of the following parameter's values is specified: `tunnel_host`, `tunnel_port`, `tunnel_user`. Otherwise, `Directly` is used as a value if the parameter is omitted.",
         title="",
     )
     update_method: Optional[Dict[str, Any]] = Field(
@@ -2447,22 +2883,28 @@
         description="Destination schema prefix. Prefix for each replicated schema. For example with prefix 'x', source schemas 'foo' and 'bar' get replicated as 'x_foo' and 'x_bar'. The prefix is permanent and cannot be changed after connection creation",
         title="Destination schema prefix",
     )
     user: Optional[str] = Field(None, description="The user name.", title="")
 
 
 class AuroraConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config36] = Field(None, description="")
 
 
 class AuroraNewConnectorRequestV1(NewConnectorRequestV1, AuroraConfigV1):
+    """ """
+
     pass
 
 
 class Config37(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     publication_name: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`Directly`, `PrivateLink`, `SshTunnel`. `SshTunnel` is used as a value if this parameter is omitted in the request and any of the following parameter's values is specified: `tunnel_host`, `tunnel_port`, `tunnel_user`. Otherwise, `Directly` is used as a value if the parameter is omitted.",
         title="",
     )
@@ -2502,22 +2944,28 @@
         description='Replication slot name. Specify only for `"updated_method": "WAL"` or `"WAL_PGOUTPUT"`.',
         title="",
     )
     user: Optional[str] = Field(None, description="The user name.", title="")
 
 
 class AuroraPostgresConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config37] = Field(None, description="")
 
 
 class AuroraPostgresNewConnectorRequestV1(NewConnectorRequestV1, AuroraPostgresConfigV1):
+    """ """
+
     pass
 
 
 class Config38(BaseModel):
+    """ """
+
     bucket: Optional[str] = Field(
         None,
         description="The AWS bucket name which is configured for AWS CloudTrail.",
         title="",
     )
     schema_: Optional[str] = Field(
         None,
@@ -2531,22 +2979,28 @@
         None,
         description="This is the same as your `group_id`, used for authentication along with the `role_arn`.",
         title="",
     )
 
 
 class AwsCloudtrailConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config38] = Field(None, description="")
 
 
 class AwsCloudtrailNewConnectorRequestV1(NewConnectorRequestV1, AwsCloudtrailConfigV1):
+    """ """
+
     pass
 
 
 class Config39(BaseModel):
+    """ """
+
     bucket: Optional[str] = Field(
         None,
         description="The AWS bucket name that is configured for AWS Config.",
         title="",
     )
     schema_: Optional[str] = Field(
         None,
@@ -2559,27 +3013,35 @@
         None,
         description="The prefix if you used one when configuring the bucket.",
         title="",
     )
 
 
 class AwsInventoryConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config39] = Field(None, description="")
 
 
 class AwsInventoryNewConnectorRequestV1(NewConnectorRequestV1, AwsInventoryConfigV1):
+    """ """
+
     pass
 
 
 class SecretsListItem(BaseModel):
+    """ """
+
     value: Optional[str] = Field(None, description="", title="")
     key: Optional[str] = Field(None, description="", title="")
 
 
 class Config40(BaseModel):
+    """ """
+
     bucket: Optional[str] = Field(None, description="", title="")
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
@@ -2602,22 +3064,28 @@
         description="The secrets that should be passed to the function at runtime.",
         title="",
     )
     is_private_link_required: Optional[bool] = Field(None, title="")
 
 
 class AwsLambdaConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config40] = Field(None, description="")
 
 
 class AwsLambdaNewConnectorRequestV1(NewConnectorRequestV1, AwsLambdaConfigV1):
+    """ """
+
     pass
 
 
 class Config41(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     consumer_group: Optional[str] = Field(
@@ -2665,22 +3133,28 @@
         title="",
     )
     schema_registry_urls: Optional[List[str]] = Field(None, title="")
     schema_registry_key: Optional[str] = Field(None, title="")
 
 
 class AwsMskConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config41] = Field(None, description="")
 
 
 class AwsMskNewConnectorRequestV1(NewConnectorRequestV1, AwsMskConfigV1):
+    """ """
+
     pass
 
 
 class Config42(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     append_file_option: Optional[Dict[str, Any]] = Field(
@@ -2752,22 +3226,28 @@
         None,
         description="Files inside of compressed archives with filenames matching this regular expression will be synced.",
         title="",
     )
 
 
 class AzureBlobStorageConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config42] = Field(None, description="")
 
 
 class AzureBlobStorageNewConnectorRequestV1(NewConnectorRequestV1, AzureBlobStorageConfigV1):
+    """ """
+
     pass
 
 
 class Config43(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     consumer_group: Optional[str] = Field(None, description="Name of consumer group created for Fivetran.", title="")
@@ -2779,27 +3259,35 @@
         None,
         description="Connection string of the Event Hub Namespace you want to sync.",
         title="",
     )
 
 
 class AzureEventHubConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config43] = Field(None, description="")
 
 
 class AzureEventHubNewConnectorRequestV1(NewConnectorRequestV1, AzureEventHubConfigV1):
+    """ """
+
     pass
 
 
 class SecretsListItem1(BaseModel):
+    """ """
+
     value: Optional[str] = Field(None, description="", title="")
     key: Optional[str] = Field(None, description="", title="")
 
 
 class Config44(BaseModel):
+    """ """
+
     bucket: Optional[str] = Field(None, description="", title="")
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
@@ -2812,22 +3300,28 @@
         None,
         description="The secrets that should be passed to the function at runtime.",
         title="",
     )
 
 
 class AzureFunctionConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config44] = Field(None, description="")
 
 
 class AzureFunctionNewConnectorRequestV1(NewConnectorRequestV1, AzureFunctionConfigV1):
+    """ """
+
     pass
 
 
 class Config45(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     publication_name: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`Directly`, `PrivateLink`, `SshTunnel`. `SshTunnel` is used as a value if this parameter is omitted in the request and any of the following parameter's values is specified: `tunnel_host`, `tunnel_port`, `tunnel_user`. Otherwise, `Directly` is used as a value if the parameter is omitted.",
         title="",
     )
@@ -2867,22 +3361,28 @@
         description='Replication slot name. Specify only for `"updated_method": "WAL"` or `"WAL_PGOUTPUT"`.',
         title="",
     )
     user: Optional[str] = Field(None, description="The user name.", title="")
 
 
 class AzurePostgresConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config45] = Field(None, description="")
 
 
 class AzurePostgresNewConnectorRequestV1(NewConnectorRequestV1, AzurePostgresConfigV1):
+    """ """
+
     pass
 
 
 class Config46(BaseModel):
+    """ """
+
     asb_i_p: Optional[str] = Field(None, description="The IP address (or) the URL of ASB namespace", title="asb_ip")
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
@@ -2951,41 +3451,51 @@
         None,
         description="The comma-separated list of schema registry servers in the `server:port` format",
         title="schema_registry_urls",
     )
 
 
 class ClientAccess3(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth5(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess3] = None
     realm_id: Optional[str] = Field(None, description="Realm ID of your application.")
 
 
 class AzureServiceBusConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config46] = Field(None, description="")
     auth: Optional[Auth5] = None
 
 
 class AzureServiceBusNewConnectorRequestV1(NewConnectorRequestV1, AzureServiceBusConfigV1):
+    """ """
+
     pass
 
 
 class Config47(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     agent_user: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(None, description="", title="")
     agent_password: Optional[str] = Field(None, description="", title="")
     always_encrypted: Optional[bool] = Field(None, title="")
     agent_public_cert: Optional[str] = Field(None, description="", title="")
     tunnel_user: Optional[str] = Field(
@@ -3019,35 +3529,43 @@
         None,
         description="The user name.  For Azure Databases, the format must be `user@domain`.",
         title="",
     )
 
 
 class Auth6(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     realm_id: Optional[str] = Field(None, description="Realm ID of your application.")
 
 
 class AzureSqlDbConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config47] = Field(None, description="")
     auth: Optional[Auth6] = None
 
 
 class AzureSqlDbNewConnectorRequestV1(NewConnectorRequestV1, AzureSqlDbConfigV1):
+    """ """
+
     pass
 
 
 class Config48(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     agent_user: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(None, description="", title="")
     agent_password: Optional[str] = Field(None, description="", title="")
     always_encrypted: Optional[bool] = Field(None, description="", title="")
     agent_public_cert: Optional[str] = Field(None, description="", title="")
     tunnel_user: Optional[str] = Field(None, description="", title="")
@@ -3065,35 +3583,43 @@
     )
     agent_host: Optional[str] = Field(None, description="", title="")
     sap_user: Optional[str] = Field(None, description="", title="")
     user: Optional[str] = Field(None, description="", title="")
 
 
 class Auth7(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     realm_id: Optional[str] = Field(None, description="Realm ID of your application.")
 
 
 class AzureSqlManagedDbConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config48] = Field(None, description="")
     auth: Optional[Auth7] = None
 
 
 class AzureSqlManagedDbNewConnectorRequestV1(NewConnectorRequestV1, AzureSqlManagedDbConfigV1):
+    """ """
+
     pass
 
 
 class Config49(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None,
         description="Whether to sync all accounts or specific accounts. Default value: `AllAccounts`.",
         title="",
     )
     schema_: Optional[str] = Field(
         None,
@@ -3115,36 +3641,46 @@
         None,
         description="Specific accounts to sync. Must be populated if `syncMode` is set to `SpecificAccounts`.",
         title="",
     )
 
 
 class ClientAccess4(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth8(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess4] = None
 
 
 class BingadsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config49] = Field(None, description="")
     auth: Optional[Auth8] = None
 
 
 class BingadsNewConnectorRequestV1(NewConnectorRequestV1, BingadsConfigV1):
+    """ """
+
     pass
 
 
 class Config50(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     append_file_option: Optional[Dict[str, Any]] = Field(
@@ -3218,92 +3754,118 @@
         None,
         description="Destination table. Table is permanent and cannot be changed after connection creation",
         title="Destination table",
     )
 
 
 class Auth9(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     realm_id: Optional[str] = Field(None, description="Realm ID of your application.")
 
 
 class BoxConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config50] = Field(None, description="")
     auth: Optional[Auth9] = None
 
 
 class BoxNewConnectorRequestV1(NewConnectorRequestV1, BoxConfigV1):
+    """ """
+
     pass
 
 
 class Config51(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="The contents of your PEM certificate file.", title="")
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     private_key: Optional[str] = Field(None, description="The contents of your secret key file.", title="")
     merchant_id: Optional[str] = Field(None, description="Your Braintree merchant ID.", title="")
 
 
 class BraintreeConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config51] = Field(None, description="")
 
 
 class BraintreeNewConnectorRequestV1(NewConnectorRequestV1, BraintreeConfigV1):
+    """ """
+
     pass
 
 
 class Config52(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="The contents of your PEM certificate file.", title="")
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     private_key: Optional[str] = Field(None, description="The contents of your secret key file.", title="")
     merchant_id: Optional[str] = Field(None, description="Your Braintree merchant ID.", title="")
 
 
 class BraintreeSandboxConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config52] = Field(None, description="")
 
 
 class BraintreeSandboxNewConnectorRequestV1(NewConnectorRequestV1, BraintreeSandboxConfigV1):
+    """ """
+
     pass
 
 
 class Config53(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
 
 
 class BranchConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config53] = Field(None, description="")
 
 
 class BranchNewConnectorRequestV1(NewConnectorRequestV1, BranchConfigV1):
+    """ """
+
     pass
 
 
 class Config54(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     gcs_folder: Optional[str] = Field(
@@ -3348,22 +3910,28 @@
         description="Your S3 bucket required if `AWS_S3` is the `cloud_storage_type`",
         title="",
     )
     api_key: Optional[str] = Field(None, description="Your Braze API Key.", title="")
 
 
 class BrazeConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config54] = Field(None, description="")
 
 
 class BrazeNewConnectorRequestV1(NewConnectorRequestV1, BrazeConfigV1):
+    """ """
+
     pass
 
 
 class Config55(BaseModel):
+    """ """
+
     bucket: Optional[str] = Field(None, description="The bucket name for CloudFront.", title="")
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
@@ -3375,44 +3943,56 @@
         description="This is the same as your `group_id`, used for authentication along with the `role_arn`.",
         title="",
     )
     skip_after: Optional[int] = Field(None, description="", title="")
 
 
 class CloudfrontConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config55] = Field(None, description="")
 
 
 class CloudfrontNewConnectorRequestV1(NewConnectorRequestV1, CloudfrontConfigV1):
+    """ """
+
     pass
 
 
 class Config56(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     login_password: Optional[str] = Field(None, description="", title="")
     client_secret: Optional[str] = Field(None, description="", title="")
     region: Optional[str] = Field(None, description="", title="")
     client_id: Optional[str] = Field(None, description="", title="")
     username: Optional[str] = Field(None, description="", title="")
 
 
 class ConcurConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config56] = Field(None, description="")
 
 
 class ConcurNewConnectorRequestV1(NewConnectorRequestV1, ConcurConfigV1):
+    """ """
+
     pass
 
 
 class Config57(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     consumer_group: Optional[str] = Field(None, description="Confluent Cloud consumer group name.", title="")
@@ -3435,22 +4015,28 @@
     message_type: Optional[Dict[str, Any]] = Field(None, description="Confluent Cloud message type.", title="")
     api_secret: Optional[str] = Field(None, title="")
     schema_registry_urls: Optional[List[str]] = Field(None, title="")
     schema_registry_key: Optional[str] = Field(None, title="")
 
 
 class ConfluentCloudConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config57] = Field(None, description="")
 
 
 class ConfluentCloudNewConnectorRequestV1(NewConnectorRequestV1, ConfluentCloudConfigV1):
+    """ """
+
     pass
 
 
 class Config58(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     instance: Optional[str] = Field(
@@ -3460,22 +4046,28 @@
     )
     api_key: Optional[str] = Field(None, description="Your Coupa API key.", title="")
     client_secret: Optional[str] = Field(None, description="Your Coupa client_id", title="")
     client_id: Optional[str] = Field(None, description="Your Coupa client_id", title="")
 
 
 class CoupaConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config58] = Field(None, description="")
 
 
 class CoupaNewConnectorRequestV1(NewConnectorRequestV1, CoupaConfigV1):
+    """ """
+
     pass
 
 
 class Config59(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     report_timezone: Optional[str] = Field(None, description="Report Timezone", title="")
@@ -3487,39 +4079,51 @@
     currency: Optional[Dict[str, Any]] = Field(None, description="Currency", title="")
     client_secret: Optional[str] = Field(None, description="Your Criteo client secret key.", title="")
     metrics: Optional[List[str]] = Field(None, description="Metrics", title="")
     client_id: Optional[str] = Field(None, description="Your Criteo Client ID.", title="")
 
 
 class CriteoConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config59] = Field(None, description="")
 
 
 class CriteoNewConnectorRequestV1(NewConnectorRequestV1, CriteoConfigV1):
+    """ """
+
     pass
 
 
 class Config60(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
 
 
 class DelightedConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config60] = Field(None, description="")
 
 
 class DelightedNewConnectorRequestV1(NewConnectorRequestV1, DelightedConfigV1):
+    """ """
+
     pass
 
 
 class Config61(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`SshTunnel`, `PrivateLink` . `SshTunnel` is used as a value if this parameter is omitted in the request and the following parameter's values are specified: `tunnel_host`, `tunnel_port`, `tunnel_user`.",
         title="",
     )
     hosts: Optional[List[str]] = Field(None, description="", title="")
@@ -3552,28 +4156,36 @@
         description="Destination schema prefix. Prefix for each replicated schema. For example with prefix 'x', source schemas 'foo' and 'bar' get replicated as 'x_foo' and 'x_bar'. The prefix is permanent and cannot be changed after connection creation",
         title="Destination schema prefix",
     )
     user: Optional[str] = Field(None, description="The user name.", title="")
 
 
 class DocumentdbConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config61] = Field(None, description="")
 
 
 class DocumentdbNewConnectorRequestV1(NewConnectorRequestV1, DocumentdbConfigV1):
+    """ """
+
     pass
 
 
 class DimensionFilter(BaseModel):
+    """ """
+
     filter_expression: Optional[str] = Field(None, description="", title="")
     match_type: Optional[Dict[str, Any]] = Field(None, description="", title="")
     dimension: Optional[str] = Field(None, description="", title="")
 
 
 class Config62(BaseModel):
+    """ """
+
     dimension_filters: Optional[List[DimensionFilter]] = Field(None, description="", title="")
     sync_mode: Optional[Dict[str, Any]] = Field(
         None,
         description="Whether to sync all user profiles or specific ones. Default value: `AllAccounts`.",
         title="",
     )
     schema_: Optional[str] = Field(
@@ -3617,36 +4229,46 @@
         None,
         description="Report dimensions to include into a sync. The `date` dimension is mandatory for all the report types. The `advertiser` dimension is mandatory for `REACH` report type",
         title="",
     )
 
 
 class ClientAccess5(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth10(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess5] = None
 
 
 class DoubleClickCampaignManagerConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config62] = Field(None, description="")
     auth: Optional[Auth10] = None
 
 
 class DoubleClickCampaignManagerNewConnectorRequestV1(NewConnectorRequestV1, DoubleClickCampaignManagerConfigV1):
+    """ """
+
     pass
 
 
 class Config63(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     network_code: Optional[int] = Field(
@@ -3674,50 +4296,66 @@
         None,
         description="Report dimensions to include in the sync. The `date` dimension is mandatory for all the report types.",
         title="",
     )
 
 
 class ClientAccess6(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth11(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess6] = None
 
 
 class DoubleClickPublishersConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config63] = Field(None, description="")
     auth: Optional[Auth11] = None
 
 
 class DoubleClickPublishersNewConnectorRequestV1(NewConnectorRequestV1, DoubleClickPublishersConfigV1):
+    """ """
+
     pass
 
 
 class Auth12(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="", title="")
     client_id: Optional[str] = Field(None, description="", title="")
 
 
 class DriftConfigV1(BaseModel):
+    """ """
+
     config: Optional[Dict[str, Any]] = Field(None, description="")
     auth: Optional[Auth12] = Field(None, description="")
 
 
 class DriftNewConnectorRequestV1(NewConnectorRequestV1, DriftConfigV1):
+    """ """
+
     pass
 
 
 class Config64(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     is_filein_root_name_space: Optional[bool] = Field(None, title="")
@@ -3792,41 +4430,51 @@
         None,
         description="Destination table. Table is permanent and cannot be changed after connection creation",
         title="Destination table",
     )
 
 
 class ClientAccess7(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth13(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess7] = None
     realm_id: Optional[str] = Field(None, description="Realm ID of your application.")
 
 
 class DropboxConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config64] = Field(None, description="")
     auth: Optional[Auth13] = None
 
 
 class DropboxNewConnectorRequestV1(NewConnectorRequestV1, DropboxConfigV1):
+    """ """
+
     pass
 
 
 class Config65(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     domain_name: Optional[str] = Field(
@@ -3834,36 +4482,46 @@
         description="The custom domain name associated with Dynamics 365.",
         title="",
     )
     resource_u_r_l: Optional[str] = Field(None, title="")
 
 
 class ClientAccess8(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth14(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess8] = None
 
 
 class Dynamics365ConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config65] = Field(None, description="")
     auth: Optional[Auth14] = None
 
 
 class Dynamics365NewConnectorRequestV1(NewConnectorRequestV1, Dynamics365ConfigV1):
+    """ """
+
     pass
 
 
 class Config66(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     agent_user: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(None, description="", title="")
     agent_password: Optional[str] = Field(None, description="", title="")
     always_encrypted: Optional[bool] = Field(None, title="")
     agent_public_cert: Optional[str] = Field(None, description="", title="")
     tunnel_user: Optional[str] = Field(
@@ -3893,35 +4551,43 @@
     )
     agent_host: Optional[str] = Field(None, description="", title="")
     sap_user: Optional[str] = Field(None, description="", title="")
     user: Optional[str] = Field(None, description="The user name. The format must be `user@domain`.", title="")
 
 
 class Auth15(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     realm_id: Optional[str] = Field(None, description="Realm ID of your application.")
 
 
 class Dynamics365FoConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config66] = Field(None, description="")
     auth: Optional[Auth15] = None
 
 
 class Dynamics365FoNewConnectorRequestV1(NewConnectorRequestV1, Dynamics365FoConfigV1):
+    """ """
+
     pass
 
 
 class Config67(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None,
         description="Whether to sync all tables in unpacked mode only or specific tables in packed mode. Default value: `UseUnpackedModeOnly`.",
         title="",
     )
     schema_: Optional[str] = Field(
         None,
@@ -3942,52 +4608,66 @@
         description="The AWS region code for the DynamoDB instance, e.g. `us-east-1`.",
         title="",
     )
     role_a_r_n: Optional[str] = Field(None, title="")
 
 
 class DynamodbConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config67] = Field(None, description="")
 
 
 class DynamodbNewConnectorRequestV1(NewConnectorRequestV1, DynamodbConfigV1):
+    """ """
+
     pass
 
 
 class Config68(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
 
 
 class Auth16(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     realm_id: Optional[str] = Field(None, description="Realm ID of your application.")
 
 
 class EloquaConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config68] = Field(None, description="")
     auth: Optional[Auth16] = None
 
 
 class EloquaNewConnectorRequestV1(NewConnectorRequestV1, EloquaConfigV1):
+    """ """
+
     pass
 
 
 class Config69(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     append_file_option: Optional[Dict[str, Any]] = Field(None, title="")
@@ -4048,22 +4728,28 @@
         description="Files inside of compressed archives with filenames matching this regular expression will be synced.",
         title="",
     )
     email: Optional[str] = Field(None, title="")
 
 
 class EmailConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config69] = Field(None, description="")
 
 
 class EmailNewConnectorRequestV1(NewConnectorRequestV1, EmailConfigV1):
+    """ """
+
     pass
 
 
 class Config70(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     view_attribution_window: Optional[Dict[str, Any]] = Field(
@@ -4130,22 +4816,28 @@
         None,
         description="Destination table. Table is permanent and cannot be changed after connection creation",
         title="Destination table",
     )
 
 
 class FacebookConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config70] = Field(None, description="")
 
 
 class FacebookNewConnectorRequestV1(NewConnectorRequestV1, FacebookConfigV1):
+    """ """
+
     pass
 
 
 class Config71(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None,
         description="Whether to sync all accounts or specific accounts. Default value: `AllAccounts`.",
         title="",
     )
     schema_: Optional[str] = Field(
         None,
@@ -4157,22 +4849,28 @@
         None,
         description="Specific accounts to sync. Must be populated if `sync_mode` is set to `SpecificAccounts`.",
         title="",
     )
 
 
 class FacebookAdAccountConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config71] = Field(None, description="")
 
 
 class FacebookAdAccountNewConnectorRequestV1(NewConnectorRequestV1, FacebookAdAccountConfigV1):
+    """ """
+
     pass
 
 
 class CustomTable(BaseModel):
+    """ """
+
     prebuilt_report_name: Optional[str] = Field(
         None,
         description="The report name to which connector will sync the data. [Possible prebuilt_report values](/docs/applications/facebook-ads-insights/api-config#prebuiltreport).",
         title="",
     )
     view_attribution_window: Optional[Dict[str, Any]] = Field(
         None,
@@ -4220,14 +4918,16 @@
         None,
         description="The report time of action stats. [Possible action_report time values](/docs/applications/facebook-ads-insights/api-config#actionreporttime).",
         title="",
     )
 
 
 class Config72(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None,
         description="Option to select connector should sync all accounts or specific accounts. [Possible sync_mode values](/docs/applications/facebook-ads-insights/api-config#syncmode).",
         title="",
     )
     custom_tables: Optional[List[CustomTable]] = Field(
         None,
@@ -4254,40 +4954,50 @@
         None,
         description="List of accounts of which connector will sync the data.",
         title="",
     )
 
 
 class ClientAccess9(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth17(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
     client_access: Optional[ClientAccess9] = None
     user_access_token: Optional[str] = Field(
         None,
         description="The long-lived System User access token carries the information necessary to access API resources",
     )
 
 
 class FacebookAdsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config72] = Field(None, description="")
     auth: Optional[Auth17] = None
 
 
 class FacebookAdsNewConnectorRequestV1(NewConnectorRequestV1, FacebookAdsConfigV1):
+    """ """
+
     pass
 
 
 class Config73(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None,
         description="Whether to sync all accounts or specific accounts. Default value: `AllPages`.",
         title="",
     )
     schema_: Optional[str] = Field(
         None,
@@ -4299,36 +5009,46 @@
         None,
         description="Specific pages to sync. Must be populated if `sync_mode` is set to `SpecificPages`.",
         title="",
     )
 
 
 class ClientAccess10(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth18(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
     client_access: Optional[ClientAccess10] = None
 
 
 class FacebookPagesConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config73] = Field(None, description="")
     auth: Optional[Auth18] = None
 
 
 class FacebookPagesNewConnectorRequestV1(NewConnectorRequestV1, FacebookPagesConfigV1):
+    """ """
+
     pass
 
 
 class Config74(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     password: Optional[str] = Field(None, title="")
@@ -4337,57 +5057,73 @@
         description="(Optional) The custom Salesforce domain. Make sure that the `base_url` starts with `https://`.",
         title="",
     )
     username: Optional[str] = Field(None, title="")
 
 
 class ClientAccess11(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth19(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess11] = None
 
 
 class FinancialForceConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config74] = Field(None, description="")
     auth: Optional[Auth19] = None
 
 
 class FinancialForceNewConnectorRequestV1(NewConnectorRequestV1, FinancialForceConfigV1):
+    """ """
+
     pass
 
 
 class Config75(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     is_account_level_connector: Optional[bool] = Field(
         None, description="(Optional) Retrieve account-level logs.", title=""
     )
     group_name: Optional[str] = Field(None, title="")
 
 
 class FivetranLogConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config75] = Field(None, description="")
 
 
 class FivetranLogNewConnectorRequestV1(NewConnectorRequestV1, FivetranLogConfigV1):
+    """ """
+
     pass
 
 
 class Config76(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     api_key: Optional[str] = Field(None, description="Your Freshdesk API Key.", title="")
@@ -4395,53 +5131,69 @@
         None,
         description="Your company's freshdesk subdomain (usually **company**.freshdesk.com).",
         title="",
     )
 
 
 class FreshdeskConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config76] = Field(None, description="")
 
 
 class FreshdeskNewConnectorRequestV1(NewConnectorRequestV1, FreshdeskConfigV1):
+    """ """
+
     pass
 
 
 class Config77(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
 
 
 class ClientAccess12(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth20(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess12] = None
 
 
 class FrontConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config77] = Field(None, description="")
     auth: Optional[Auth20] = None
 
 
 class FrontNewConnectorRequestV1(NewConnectorRequestV1, FrontConfigV1):
+    """ """
+
     pass
 
 
 class Config78(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     append_file_option: Optional[Dict[str, Any]] = Field(
@@ -4514,41 +5266,53 @@
         None,
         description="Files inside of compressed archives with filenames matching this regular expression will be synced.",
         title="",
     )
 
 
 class FtpConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config78] = Field(None, description="")
 
 
 class FtpNewConnectorRequestV1(NewConnectorRequestV1, FtpConfigV1):
+    """ """
+
     pass
 
 
 class Config79(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     access_key: Optional[str] = Field(None, description="The access key for API authentication.", title="")
     sub_domain: Optional[str] = Field(None, description="The subdomain of your Gainsight account.", title="")
 
 
 class GainsightCustomerSuccessConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config79] = Field(None, description="")
 
 
 class GainsightCustomerSuccessNewConnectorRequestV1(NewConnectorRequestV1, GainsightCustomerSuccessConfigV1):
+    """ """
+
     pass
 
 
 class Config80(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     auth_type: Optional[Dict[str, Any]] = Field(
@@ -4627,22 +5391,28 @@
         None,
         description="Files inside of compressed archives with filenames matching this regular expression will be synced.",
         title="",
     )
 
 
 class GcsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config80] = Field(None, description="")
 
 
 class GcsNewConnectorRequestV1(NewConnectorRequestV1, GcsConfigV1):
+    """ """
+
     pass
 
 
 class Config81(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None,
         description="Whether to sync all repositories or specific repositories.",
         title="",
     )
     schema_: Optional[str] = Field(
         None,
@@ -4658,22 +5428,28 @@
         title="",
     )
     auth_mode: Optional[Dict[str, Any]] = Field(None, description="Authorization type.", title="")
     username: Optional[str] = Field(None, description="`Login` of your GitHub profile.", title="")
 
 
 class GithubConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config81] = Field(None, description="")
 
 
 class GithubNewConnectorRequestV1(NewConnectorRequestV1, GithubConfigV1):
+    """ """
+
     pass
 
 
 class Report(BaseModel):
+    """ """
+
     report_type: Optional[str] = Field(
         None,
         description="The name of the Google Ads report from which the connector will sync the data. [Possible report_type values](https://developers.google.com/adwords/api/docs/appendix/reports#report-types).",
         title="",
     )
     fields: Optional[List[str]] = Field(
         None,
@@ -4684,14 +5460,16 @@
         None,
         description="The table name within the schema to which connector will sync the data of the specific report.",
         title="",
     )
 
 
 class Config82(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None, description="Whether to sync all accounts or specific accounts.", title=""
     )
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
@@ -4726,38 +5504,48 @@
         None,
         description="A period of time in days during which a conversion is recorded.",
         title="",
     )
 
 
 class ClientAccess13(BaseModel):
+    """ """
+
     developer_token: Optional[str] = Field(None, description="Your approved Developer token to connect to the API.")
     client_secret: Optional[str] = Field(None, description="Client secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
     user_agent: Optional[str] = Field(None, description="Your company's name in your client application")
 
 
 class Auth21(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess13] = None
 
 
 class GoogleAdsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config82] = Field(None, description="")
     auth: Optional[Auth21] = None
 
 
 class GoogleAdsNewConnectorRequestV1(NewConnectorRequestV1, GoogleAdsConfigV1):
+    """ """
+
     pass
 
 
 class Report1(BaseModel):
+    """ """
+
     filter: Optional[str] = Field(
         None,
         description="String parameter restricts the data returned for your report. To use the filters parameter, specify a dimension or metric on which to filter, followed by the filter expression",
         title="",
     )
     segment_ids: Optional[List[str]] = Field(None, title="")
     prebuilt_report: Optional[Dict[str, Any]] = Field(
@@ -4785,14 +5573,16 @@
         None,
         description="A segment is a subset of your Analytics data that is made up of one or more non-destructive filters (filters that do not alter the underlying data). Those filters isolate subsets of users, sessions, and hits.",
         title="",
     )
 
 
 class Config83(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     reports: Optional[List[Report1]] = Field(
@@ -4848,56 +5638,72 @@
         None,
         description="The report dimensions to include into a sync. The `date` dimension is mandatory for all the report types.",
         title="",
     )
 
 
 class ClientAccess14(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth22(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess14] = None
 
 
 class GoogleAnalyticsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config83] = Field(None, description="")
     auth: Optional[Auth22] = None
 
 
 class GoogleAnalyticsNewConnectorRequestV1(NewConnectorRequestV1, GoogleAnalyticsConfigV1):
+    """ """
+
     pass
 
 
 class Config84(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     project_id: Optional[str] = Field(None, description="The project ID.", title="")
     dataset_id: Optional[str] = Field(None, description="The dataset ID.", title="")
     bucket_name: Optional[str] = Field(None, description="The name of the bucket.", title="")
 
 
 class GoogleAnalytics360ConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config84] = Field(None, description="")
 
 
 class GoogleAnalytics360NewConnectorRequestV1(NewConnectorRequestV1, GoogleAnalytics360ConfigV1):
+    """ """
+
     pass
 
 
 class Report2(BaseModel):
+    """ """
+
     filter_value: Optional[str] = Field(None, title="")
     prebuilt_report: Optional[Dict[str, Any]] = Field(
         None,
         description="The name of the Prebuilt Report from which the connector will sync the data.",
         title="",
     )
     filter_field_name: Optional[str] = Field(None, description="The dimension name to filter on.", title="")
@@ -4912,14 +5718,16 @@
         description="The table name within the schema to which connector will sync the data of the specific report.",
         title="",
     )
     dimensions: Optional[List[str]] = Field(None, description="The report dimensions to include into a sync.", title="")
 
 
 class Config85(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None, description="Whether to sync all accounts or specific accounts.", title=""
     )
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
@@ -4944,56 +5752,72 @@
         None,
         description="The array of strings in the `properties/{id}` format where `id` is a Google Analytics 4 property identifier. Must be populated if `sync_mode` is set to `SPECIFIC_ACCOUNTS`.",
         title="",
     )
 
 
 class ClientAccess15(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth23(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess15] = None
 
 
 class GoogleAnalytics4ConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config85] = Field(None, description="")
     auth: Optional[Auth23] = None
 
 
 class GoogleAnalytics4NewConnectorRequestV1(NewConnectorRequestV1, GoogleAnalytics4ConfigV1):
+    """ """
+
     pass
 
 
 class Config86(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     project_id: Optional[str] = Field(None, description="The Project ID.", title="")
     bucket_name: Optional[str] = Field(None, description="The name of the bucket.", title="")
     dataset_id: Optional[str] = Field(None, description="The Dataset ID.", title="")
 
 
 class GoogleAnalytics4ExportConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config86] = Field(None, description="")
 
 
 class GoogleAnalytics4ExportNewConnectorRequestV1(NewConnectorRequestV1, GoogleAnalytics4ExportConfigV1):
+    """ """
+
     pass
 
 
 class Config87(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None,
         description="Whether to sync all accounts or specific accounts. Default value: `ALL_ACCOUNTS`",
         title="",
     )
     schema_: Optional[str] = Field(
         None,
@@ -5015,41 +5839,53 @@
         None,
         description="Specific Account IDs to sync.  Must be populated if `sync_mode` is set to `SPECIFIC_ACCOUNTS`.",
         title="",
     )
 
 
 class ClientAccess16(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth24(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess16] = None
 
 
 class GoogleAnalyticsMcfConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config87] = Field(None, description="")
     auth: Optional[Auth24] = None
 
 
 class GoogleAnalyticsMcfNewConnectorRequestV1(NewConnectorRequestV1, GoogleAnalyticsMcfConfigV1):
+    """ """
+
     pass
 
 
 class SecretsListItem2(BaseModel):
+    """ """
+
     value: Optional[str] = Field(None, description="", title="")
     key: Optional[str] = Field(None, description="", title="")
 
 
 class Config88(BaseModel):
+    """ """
+
     bucket: Optional[str] = Field(None, description="", title="")
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
@@ -5061,22 +5897,28 @@
         None,
         description="The secrets that should be passed to the function at runtime.",
         title="",
     )
 
 
 class GoogleCloudFunctionConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config88] = Field(None, description="")
 
 
 class GoogleCloudFunctionNewConnectorRequestV1(NewConnectorRequestV1, GoogleCloudFunctionConfigV1):
+    """ """
+
     pass
 
 
 class Config89(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`Directly`, `PrivateLink`, `SshTunnel`. `SshTunnel` is used as a value if this parameter is omitted in the request and any of the following parameter's values is specified: `tunnel_host`, `tunnel_port`, `tunnel_user`. Otherwise, `Directly` is used as a value if the parameter is omitted.",
         title="",
     )
     update_method: Optional[Dict[str, Any]] = Field(
@@ -5109,22 +5951,28 @@
         description="Destination schema prefix. Prefix for each replicated schema. For example with prefix 'x', source schemas 'foo' and 'bar' get replicated as 'x_foo' and 'x_bar'. The prefix is permanent and cannot be changed after connection creation",
         title="Destination schema prefix",
     )
     user: Optional[str] = Field(None, description="The user name.", title="")
 
 
 class GoogleCloudMysqlConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config89] = Field(None, description="")
 
 
 class GoogleCloudMysqlNewConnectorRequestV1(NewConnectorRequestV1, GoogleCloudMysqlConfigV1):
+    """ """
+
     pass
 
 
 class Config90(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     publication_name: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`Directly`, `PrivateLink`, `SshTunnel`. `SshTunnel` is used as a value if this parameter is omitted in the request and any of the following parameter's values is specified: `tunnel_host`, `tunnel_port`, `tunnel_user`. Otherwise, `Directly` is used as a value if the parameter is omitted.",
         title="",
     )
@@ -5164,22 +6012,28 @@
         description='Replication slot name. Specify only for `"updated_method": "WAL"` or `"WAL_PGOUTPUT"`.',
         title="",
     )
     user: Optional[str] = Field(None, description="The user name.", title="")
 
 
 class GoogleCloudPostgresqlConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config90] = Field(None, description="")
 
 
 class GoogleCloudPostgresqlNewConnectorRequestV1(NewConnectorRequestV1, GoogleCloudPostgresqlConfigV1):
+    """ """
+
     pass
 
 
 class Config91(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     agent_user: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(None, description="", title="")
     agent_password: Optional[str] = Field(None, description="", title="")
     always_encrypted: Optional[bool] = Field(None, description="", title="")
     agent_public_cert: Optional[str] = Field(None, description="", title="")
     tunnel_user: Optional[str] = Field(
@@ -5213,35 +6067,43 @@
         None,
         description="The user name. For Azure Databases, the format must be `user@domain`.",
         title="",
     )
 
 
 class Auth25(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     realm_id: Optional[str] = Field(None, description="Realm ID of your application.")
 
 
 class GoogleCloudSqlserverConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config91] = Field(None, description="")
     auth: Optional[Auth25] = None
 
 
 class GoogleCloudSqlserverNewConnectorRequestV1(NewConnectorRequestV1, GoogleCloudSqlserverConfigV1):
+    """ """
+
     pass
 
 
 class Config92(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     query_id: Optional[str] = Field(
@@ -5289,30 +6151,38 @@
         None,
         description="The report dimensions (filters) to include into a sync. The dimension names are provided in the API format. This is a required parameter when `config_method` is set to `CREATE_NEW`.",
         title="",
     )
 
 
 class Auth26(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
 
 
 class GoogleDisplayAndVideo360ConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config92] = Field(None, description="")
     auth: Optional[Auth26] = None
 
 
 class GoogleDisplayAndVideo360NewConnectorRequestV1(NewConnectorRequestV1, GoogleDisplayAndVideo360ConfigV1):
+    """ """
+
     pass
 
 
 class Config93(BaseModel):
+    """ """
+
     service_account: Optional[str] = Field(None, description="", title="")
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
@@ -5387,63 +6257,81 @@
         None,
         description="Destination table. Table is permanent and cannot be changed after connection creation",
         title="Destination table",
     )
 
 
 class Auth27(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     realm_id: Optional[str] = Field(None, description="Realm ID of your application.")
 
 
 class GoogleDriveConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config93] = Field(None, description="")
     auth: Optional[Auth27] = None
 
 
 class GoogleDriveNewConnectorRequestV1(NewConnectorRequestV1, GoogleDriveConfigV1):
+    """ """
+
     pass
 
 
 class Config94(BaseModel):
+    """ """
+
     bucket: Optional[str] = Field(None, description="The Google Cloud Storage source bucket.", title="")
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
 
 
 class ClientAccess17(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth28(BaseModel):
+    """ """
+
     client_access: Optional[ClientAccess17] = None
 
 
 class GooglePlayConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config94] = Field(None, description="")
     auth: Optional[Auth28] = None
 
 
 class GooglePlayNewConnectorRequestV1(NewConnectorRequestV1, GooglePlayConfigV1):
+    """ """
+
     pass
 
 
 class Report3(BaseModel):
+    """ """
+
     aggregation: Optional[Dict[str, Any]] = Field(
         None,
         description="(Optional) Aggregation type. Supported only for the `SEARCH_RESULTS` report type",
         title="",
     )
     report_type: Optional[Dict[str, Any]] = Field(None, description="The type of report", title="")
     search_types: Optional[List[Dict[str, Any]]] = Field(
@@ -5458,14 +6346,16 @@
     )
     dimensions: Optional[List[Dict[str, Any]]] = Field(
         None, description="The report dimensions included to sync.", title=""
     )
 
 
 class Config95(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None, description="Whether to sync all sites or specific sites.", title=""
     )
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
@@ -5485,32 +6375,42 @@
         None,
         description="Specific Site URLs to sync. Must be populated if `sync_mode` is set to `SpecificSites`.",
         title="",
     )
 
 
 class ClientAccess18(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth29(BaseModel):
+    """ """
+
     client_access: Optional[ClientAccess18] = None
 
 
 class GoogleSearchConsoleConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config95] = Field(None, description="")
     auth: Optional[Auth29] = None
 
 
 class GoogleSearchConsoleNewConnectorRequestV1(NewConnectorRequestV1, GoogleSearchConsoleConfigV1):
+    """ """
+
     pass
 
 
 class Config96(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     auth_type: Optional[Dict[str, Any]] = Field(
@@ -5532,135 +6432,175 @@
         None,
         description="Destination table. Table is permanent and cannot be changed after connection creation",
         title="Destination table",
     )
 
 
 class ClientAccess19(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth30(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess19] = None
 
 
 class GoogleSheetsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config96] = Field(None, description="")
     auth: Optional[Auth30] = None
 
 
 class GoogleSheetsNewConnectorRequestV1(NewConnectorRequestV1, GoogleSheetsConfigV1):
+    """ """
+
     pass
 
 
 class Config97(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     api_key: Optional[str] = Field(None, description="Your Greenhouse API key.", title="")
 
 
 class GreenhouseConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config97] = Field(None, description="")
 
 
 class GreenhouseNewConnectorRequestV1(NewConnectorRequestV1, GreenhouseConfigV1):
+    """ """
+
     pass
 
 
 class Config98(BaseModel):
+    """ """
+
     bucket: Optional[str] = Field(None, description="The S3 bucket name.", title="")
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     role_arn: Optional[str] = Field(None, description="The Role ARN required for authentication.", title="")
 
 
 class HeapConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config98] = Field(None, description="")
 
 
 class HeapNewConnectorRequestV1(NewConnectorRequestV1, HeapConfigV1):
+    """ """
+
     pass
 
 
 class Config99(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     api_key: Optional[str] = Field(None, description="Your Height API key.", title="")
 
 
 class Auth31(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     realm_id: Optional[str] = Field(None, description="Realm ID of your application.")
 
 
 class HeightConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config99] = Field(None, description="")
     auth: Optional[Auth31] = None
 
 
 class HeightNewConnectorRequestV1(NewConnectorRequestV1, HeightConfigV1):
+    """ """
+
     pass
 
 
 class Config100(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
 
 
 class ClientAccess20(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth32(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess20] = None
 
 
 class HelpscoutConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config100] = Field(None, description="")
     auth: Optional[Auth32] = None
 
 
 class HelpscoutNewConnectorRequestV1(NewConnectorRequestV1, HelpscoutConfigV1):
+    """ """
+
     pass
 
 
 class Config101(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     consumer_group: Optional[str] = Field(None, description="Heroku Kafka consumer group name.", title="")
@@ -5682,22 +6622,28 @@
     )
     client_cert_key: Optional[str] = Field(None, title="")
     message_type: Optional[Dict[str, Any]] = Field(None, description="Heroku Kafka message type.", title="")
     trusted_cert: Optional[str] = Field(None, title="")
 
 
 class HerokuKafkaConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config101] = Field(None, description="")
 
 
 class HerokuKafkaNewConnectorRequestV1(NewConnectorRequestV1, HerokuKafkaConfigV1):
+    """ """
+
     pass
 
 
 class Config102(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     publication_name: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`Directly`, `PrivateLink`, `SshTunnel`. `SshTunnel` is used as a value if this parameter is omitted in the request and any of the following parameter's values is specified: `tunnel_host`, `tunnel_port`, `tunnel_user`. Otherwise, `Directly` is used as a value if the parameter is omitted.",
         title="",
     )
@@ -5737,53 +6683,69 @@
         description='Replication slot name. Specify only for `"updated_method": "WAL"` or `"WAL_PGOUTPUT"`.',
         title="",
     )
     user: Optional[str] = Field(None, description="The user name.", title="")
 
 
 class HerokuPostgresConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config102] = Field(None, description="")
 
 
 class HerokuPostgresNewConnectorRequestV1(NewConnectorRequestV1, HerokuPostgresConfigV1):
+    """ """
+
     pass
 
 
 class Config103(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
 
 
 class ClientAccess21(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth33(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess21] = None
 
 
 class HubspotConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config103] = Field(None, description="")
     auth: Optional[Auth33] = None
 
 
 class HubspotNewConnectorRequestV1(NewConnectorRequestV1, HubspotConfigV1):
+    """ """
+
     pass
 
 
 class Config104(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None,
         description="Whether to sync all accounts or specific accounts. Default value: `AllAccounts`.",
         title="",
     )
     schema_: Optional[str] = Field(
         None,
@@ -5800,68 +6762,90 @@
         None,
         description="Specific accounts to sync. Must be populated if `sync_mode` is set to `SpecificAccounts`.",
         title="",
     )
 
 
 class ClientAccess22(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth34(BaseModel):
+    """ """
+
     client_access: Optional[ClientAccess22] = None
 
 
 class InstagramBusinessConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config104] = Field(None, description="")
     auth: Optional[Auth34] = None
 
 
 class InstagramBusinessNewConnectorRequestV1(NewConnectorRequestV1, InstagramBusinessConfigV1):
+    """ """
+
     pass
 
 
 class Config105(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
 
 
 class IntercomConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config105] = Field(None, description="")
 
 
 class IntercomNewConnectorRequestV1(NewConnectorRequestV1, IntercomConfigV1):
+    """ """
+
     pass
 
 
 class Config106(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     endpoint: Optional[str] = Field(None, title="")
     api_key: Optional[str] = Field(None, description="Your Iterable API key.", title="")
 
 
 class IterableConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config106] = Field(None, description="")
 
 
 class IterableNewConnectorRequestV1(NewConnectorRequestV1, IterableConfigV1):
+    """ """
+
     pass
 
 
 class Config107(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     app_specific_password: Optional[str] = Field(None, description="Your app-specific password", title="")
@@ -5900,22 +6884,28 @@
         None,
         description="Specific apps to sync. Must be populated if `app_sync_mode` is set to `SpecificApps`.",
         title="",
     )
 
 
 class ItunesConnectConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config107] = Field(None, description="")
 
 
 class ItunesConnectNewConnectorRequestV1(NewConnectorRequestV1, ItunesConnectConfigV1):
+    """ """
+
     pass
 
 
 class Config108(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     path: Optional[str] = Field(
@@ -5927,22 +6917,28 @@
     port: Optional[int] = Field(None, description="The Jira service host port.", title="")
     on_premise: Optional[bool] = Field(None, description="Whether the Jira instance is local or in cloud.", title="")
     host: Optional[str] = Field(None, description="The Jira service host address.", title="")
     user: Optional[str] = Field(None, description="The Jira username.", title="")
 
 
 class JiraConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config108] = Field(None, description="")
 
 
 class JiraNewConnectorRequestV1(NewConnectorRequestV1, JiraConfigV1):
+    """ """
+
     pass
 
 
 class Config109(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     append_file_option: Optional[Dict[str, Any]] = Field(None, title="")
@@ -5971,95 +6967,125 @@
         description="Destination table. Table is permanent and cannot be changed after connection creation",
         title="Destination table",
     )
     archive_pattern: Optional[str] = Field(None, title="")
 
 
 class KinesisConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config109] = Field(None, description="")
 
 
 class KinesisNewConnectorRequestV1(NewConnectorRequestV1, KinesisConfigV1):
+    """ """
+
     pass
 
 
 class Config110(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     api_key: Optional[str] = Field(None, description="Your Klaviyo API key.", title="")
 
 
 class KlaviyoConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config110] = Field(None, description="")
 
 
 class KlaviyoNewConnectorRequestV1(NewConnectorRequestV1, KlaviyoConfigV1):
+    """ """
+
     pass
 
 
 class Config111(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(None, description="Your Kustomer API key.", title="")
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     eu_region: Optional[bool] = Field(None, title="")
     domain: Optional[str] = Field(None, title="")
 
 
 class KustomerConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config111] = Field(None, description="")
 
 
 class KustomerNewConnectorRequestV1(NewConnectorRequestV1, KustomerConfigV1):
+    """ """
+
     pass
 
 
 class Config112(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     api_key: Optional[str] = Field(None, description="Your Lever API key.", title="")
 
 
 class LeverConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config112] = Field(None, description="")
 
 
 class LeverNewConnectorRequestV1(NewConnectorRequestV1, LeverConfigV1):
+    """ """
+
     pass
 
 
 class Config113(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
 
 
 class LightSpeedRetailConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config113] = Field(None, description="")
 
 
 class LightSpeedRetailNewConnectorRequestV1(NewConnectorRequestV1, LightSpeedRetailConfigV1):
+    """ """
+
     pass
 
 
 class Config114(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None,
         description="Whether to sync all accounts or specific accounts. Default value: `AllAccounts`",
         title="",
     )
     schema_: Optional[str] = Field(
         None,
@@ -6091,67 +7117,87 @@
         None,
         description="Specific Account IDs to sync. Must be populated if `syncMode` is set to `SpecificAccounts`.",
         title="",
     )
 
 
 class ClientAccess23(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth35(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess23] = None
 
 
 class LinkedinAdsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config114] = Field(None, description="")
     auth: Optional[Auth35] = None
 
 
 class LinkedinAdsNewConnectorRequestV1(NewConnectorRequestV1, LinkedinAdsConfigV1):
+    """ """
+
     pass
 
 
 class Config115(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
 
 
 class ClientAccess24(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth36(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess24] = None
 
 
 class LinkedinCompanyPagesConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config115] = Field(None, description="")
     auth: Optional[Auth36] = None
 
 
 class LinkedinCompanyPagesNewConnectorRequestV1(NewConnectorRequestV1, LinkedinCompanyPagesConfigV1):
+    """ """
+
     pass
 
 
 class Config116(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`Directly`, `PrivateLink`, `SshTunnel`. `SshTunnel` is used as a value if this parameter is omitted in the request and any of the following parameter's values is specified: `tunnel_host`, `tunnel_port`, `tunnel_user`. Otherwise, `Directly` is used as a value if the parameter is omitted.",
         title="",
     )
     update_method: Optional[Dict[str, Any]] = Field(
@@ -6184,22 +7230,28 @@
         description="Destination schema prefix. Prefix for each replicated schema. For example with prefix 'x', source schemas 'foo' and 'bar' get replicated as 'x_foo' and 'x_bar'. The prefix is permanent and cannot be changed after connection creation",
         title="Destination schema prefix",
     )
     user: Optional[str] = Field(None, description="The user name.", title="")
 
 
 class MagentoMysqlConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config116] = Field(None, description="")
 
 
 class MagentoMysqlNewConnectorRequestV1(NewConnectorRequestV1, MagentoMysqlConfigV1):
+    """ """
+
     pass
 
 
 class Config117(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`Directly`, `PrivateLink`, `SshTunnel`. `SshTunnel` is used as a value if this parameter is omitted in the request and any of the following parameter's values is specified: `tunnel_host`, `tunnel_port`, `tunnel_user`. Otherwise, `Directly` is used as a value if the parameter is omitted.",
         title="",
     )
     update_method: Optional[Dict[str, Any]] = Field(
@@ -6232,39 +7284,51 @@
         description="Destination schema prefix. Prefix for each replicated schema. For example with prefix 'x', source schemas 'foo' and 'bar' get replicated as 'x_foo' and 'x_bar'. The prefix is permanent and cannot be changed after connection creation",
         title="Destination schema prefix",
     )
     user: Optional[str] = Field(None, description="The user name.", title="")
 
 
 class MagentoMysqlRdsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config117] = Field(None, description="")
 
 
 class MagentoMysqlRdsNewConnectorRequestV1(NewConnectorRequestV1, MagentoMysqlRdsConfigV1):
+    """ """
+
     pass
 
 
 class Config118(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
 
 
 class MailchimpConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config118] = Field(None, description="")
 
 
 class MailchimpNewConnectorRequestV1(NewConnectorRequestV1, MailchimpConfigV1):
+    """ """
+
     pass
 
 
 class Config119(BaseModel):
+    """ """
+
     use_api_keys: Optional[bool] = Field(
         None, description="Whether to use multiple API keys for interaction.", title=""
     )
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
@@ -6275,22 +7339,28 @@
         None,
         description="Comma-separated list of API keys.  Required if `use_api_keys` is set to `true`.",
         title="",
     )
 
 
 class MandrillConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config119] = Field(None, description="")
 
 
 class MandrillNewConnectorRequestV1(NewConnectorRequestV1, MandrillConfigV1):
+    """ """
+
     pass
 
 
 class Config120(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`Directly`, `PrivateLink`, `SshTunnel`. `SshTunnel` is used as a value if this parameter is omitted in the request and any of the following parameter's values is specified: `tunnel_host`, `tunnel_port`, `tunnel_user`. Otherwise, `Directly` is used as a value if the parameter is omitted.",
         title="",
     )
     update_method: Optional[Dict[str, Any]] = Field(
@@ -6323,22 +7393,28 @@
         description="Destination schema prefix. Prefix for each replicated schema. For example with prefix 'x', source schemas 'foo' and 'bar' get replicated as 'x_foo' and 'x_bar'. The prefix is permanent and cannot be changed after connection creation",
         title="Destination schema prefix",
     )
     user: Optional[str] = Field(None, description="The user name.", title="")
 
 
 class MariaConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config120] = Field(None, description="")
 
 
 class MariaNewConnectorRequestV1(NewConnectorRequestV1, MariaConfigV1):
+    """ """
+
     pass
 
 
 class Config121(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`Directly`, `PrivateLink`, `SshTunnel`. `SshTunnel` is used as a value if this parameter is omitted in the request and any of the following parameter's values is specified: `tunnel_host`, `tunnel_port`, `tunnel_user`. Otherwise, `Directly` is used as a value if the parameter is omitted.",
         title="",
     )
     update_method: Optional[Dict[str, Any]] = Field(
@@ -6371,22 +7447,28 @@
         description="Destination schema prefix. Prefix for each replicated schema. For example with prefix 'x', source schemas 'foo' and 'bar' get replicated as 'x_foo' and 'x_bar'. The prefix is permanent and cannot be changed after connection creation",
         title="Destination schema prefix",
     )
     user: Optional[str] = Field(None, description="The user name.", title="")
 
 
 class MariaAzureConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config121] = Field(None, description="")
 
 
 class MariaAzureNewConnectorRequestV1(NewConnectorRequestV1, MariaAzureConfigV1):
+    """ """
+
     pass
 
 
 class Config122(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`Directly`, `PrivateLink`, `SshTunnel`. `SshTunnel` is used as a value if this parameter is omitted in the request and any of the following parameter's values is specified: `tunnel_host`, `tunnel_port`, `tunnel_user`. Otherwise, `Directly` is used as a value if the parameter is omitted.",
         title="",
     )
     update_method: Optional[Dict[str, Any]] = Field(
@@ -6419,44 +7501,56 @@
         description="Destination schema prefix. Prefix for each replicated schema. For example with prefix 'x', source schemas 'foo' and 'bar' get replicated as 'x_foo' and 'x_bar'. The prefix is permanent and cannot be changed after connection creation",
         title="Destination schema prefix",
     )
     user: Optional[str] = Field(None, description="The user name.", title="")
 
 
 class MariaRdsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config122] = Field(None, description="")
 
 
 class MariaRdsNewConnectorRequestV1(NewConnectorRequestV1, MariaRdsConfigV1):
+    """ """
+
     pass
 
 
 class Config123(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     password: Optional[str] = Field(None, description="The Marin user's password.", title="")
     port: Optional[int] = Field(None, title="")
     prefix: Optional[str] = Field(None, description="Folder path to the Marin manifest file.", title="")
     host: Optional[str] = Field(None, description="The Marin host address.", title="")
     user: Optional[str] = Field(None, description="The Marin username.", title="")
 
 
 class MarinConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config123] = Field(None, description="")
 
 
 class MarinNewConnectorRequestV1(NewConnectorRequestV1, MarinConfigV1):
+    """ """
+
     pass
 
 
 class Config124(BaseModel):
+    """ """
+
     soap_uri: Optional[str] = Field(None, title="")
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
@@ -6471,69 +7565,89 @@
     bulk_api_quota: Optional[float] = Field(None, title="")
     encryption_key: Optional[str] = Field(None, title="")
     client_secret: Optional[str] = Field(None, description="Marketo REST API Client Secret.", title="")
     client_id: Optional[str] = Field(None, description="Marketo REST API Client Id.", title="")
 
 
 class MarketoConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config124] = Field(None, description="")
 
 
 class MarketoNewConnectorRequestV1(NewConnectorRequestV1, MarketoConfigV1):
+    """ """
+
     pass
 
 
 class Config125(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
 
 
 class MavenlinkConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config125] = Field(None, description="")
 
 
 class MavenlinkNewConnectorRequestV1(NewConnectorRequestV1, MavenlinkConfigV1):
+    """ """
+
     pass
 
 
 class Config126(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     domain_type: Optional[str] = Field(None, description="Domain type of your Medallia URL", title="")
     subdomain: Optional[str] = Field(None, description="Medallia subdomain", title="")
     client_secret: Optional[str] = Field(None, description="Medallia Client Secret key", title="")
     client_name: Optional[str] = Field(None, description="Medallia company name", title="")
     client_id: Optional[str] = Field(None, description="Medallia Client ID", title="")
 
 
 class Auth37(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
 
 
 class MedalliaConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config126] = Field(None, description="")
     auth: Optional[Auth37] = None
 
 
 class MedalliaNewConnectorRequestV1(NewConnectorRequestV1, MedalliaConfigV1):
+    """ """
+
     pass
 
 
 class Config127(BaseModel):
+    """ """
+
     site_name: Optional[str] = Field(
         None,
         description="The Name of the SharePoint site. The Site Name is the `name` field in the Graph API response for sites.",
         title="",
     )
     schema_: Optional[str] = Field(
         None,
@@ -6545,50 +7659,66 @@
         None,
         description="The Site ID of the SharePoint site from which you want to sync your lists. The Site ID is the `id` field in the [Graph API](https://docs.microsoft.com/en-us/graph/api/site-search?view=graph-rest-1.0&tabs=http) response for sites.",
         title="",
     )
 
 
 class ClientAccess25(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth38(BaseModel):
+    """ """
+
     client_access: Optional[ClientAccess25] = None
 
 
 class MicrosoftListsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config127] = Field(None, description="")
     auth: Optional[Auth38] = None
 
 
 class MicrosoftListsNewConnectorRequestV1(NewConnectorRequestV1, MicrosoftListsConfigV1):
+    """ """
+
     pass
 
 
 class Config128(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     api_secret: Optional[str] = Field(None, description="Mixpanel API Secret.", title="")
 
 
 class MixpanelConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config128] = Field(None, description="")
 
 
 class MixpanelNewConnectorRequestV1(NewConnectorRequestV1, MixpanelConfigV1):
+    """ """
+
     pass
 
 
 class Config129(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, title="")
     packed_mode_tables: Optional[List[str]] = Field(
         None,
         description="List of tables to be synced in packed mode; format:`<db>.<table>`(case-sensitive).",
         title="",
     )
     packing_mode: Optional[Dict[str, Any]] = Field(
@@ -6631,22 +7761,28 @@
         description="Destination schema prefix. Prefix for each replicated schema. For example with prefix 'x', source schemas 'foo' and 'bar' get replicated as 'x_foo' and 'x_bar'. The prefix is permanent and cannot be changed after connection creation",
         title="Destination schema prefix",
     )
     user: Optional[str] = Field(None, description="The user name.", title="")
 
 
 class MongoConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config129] = Field(None, description="")
 
 
 class MongoNewConnectorRequestV1(NewConnectorRequestV1, MongoConfigV1):
+    """ """
+
     pass
 
 
 class Config130(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, title="")
     packed_mode_tables: Optional[List[str]] = Field(
         None,
         description="List of tables to be synced in packed mode; format:`<db>.<table>`(case-sensitive).",
         title="",
     )
     packing_mode: Optional[Dict[str, Any]] = Field(
@@ -6689,22 +7825,28 @@
         description="Destination schema prefix. Prefix for each replicated schema. For example with prefix 'x', source schemas 'foo' and 'bar' get replicated as 'x_foo' and 'x_bar'. The prefix is permanent and cannot be changed after connection creation",
         title="Destination schema prefix",
     )
     user: Optional[str] = Field(None, description="The user name.", title="")
 
 
 class MongoShardedConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config130] = Field(None, description="")
 
 
 class MongoShardedNewConnectorRequestV1(NewConnectorRequestV1, MongoShardedConfigV1):
+    """ """
+
     pass
 
 
 class Config131(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`Directly`, `PrivateLink`, `SshTunnel`. `SshTunnel` is used as a value if this parameter is omitted in the request and any of the following parameter's values is specified: `tunnel_host`, `tunnel_port`, `tunnel_user`. Otherwise, `Directly` is used as a value if the parameter is omitted.",
         title="",
     )
     update_method: Optional[Dict[str, Any]] = Field(
@@ -6737,22 +7879,28 @@
         description="Destination schema prefix. Prefix for each replicated schema. For example with prefix 'x', source schemas 'foo' and 'bar' get replicated as 'x_foo' and 'x_bar'. The prefix is permanent and cannot be changed after connection creation",
         title="Destination schema prefix",
     )
     user: Optional[str] = Field(None, description="The user name.", title="")
 
 
 class MysqlConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config131] = Field(None, description="")
 
 
 class MysqlNewConnectorRequestV1(NewConnectorRequestV1, MysqlConfigV1):
+    """ """
+
     pass
 
 
 class Config132(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`Directly`, `PrivateLink`, `SshTunnel`. `SshTunnel` is used as a value if this parameter is omitted in the request and any of the following parameter's values is specified: `tunnel_host`, `tunnel_port`, `tunnel_user`. Otherwise, `Directly` is used as a value if the parameter is omitted.",
         title="",
     )
     update_method: Optional[Dict[str, Any]] = Field(
@@ -6785,22 +7933,28 @@
         description="Destination schema prefix. Prefix for each replicated schema. For example with prefix 'x', source schemas 'foo' and 'bar' get replicated as 'x_foo' and 'x_bar'. The prefix is permanent and cannot be changed after connection creation",
         title="Destination schema prefix",
     )
     user: Optional[str] = Field(None, description="The user name.", title="")
 
 
 class MysqlAzureConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config132] = Field(None, description="")
 
 
 class MysqlAzureNewConnectorRequestV1(NewConnectorRequestV1, MysqlAzureConfigV1):
+    """ """
+
     pass
 
 
 class Config133(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`Directly`, `PrivateLink`, `SshTunnel`. `SshTunnel` is used as a value if this parameter is omitted in the request and any of the following parameter's values is specified: `tunnel_host`, `tunnel_port`, `tunnel_user`. Otherwise, `Directly` is used as a value if the parameter is omitted.",
         title="",
     )
     update_method: Optional[Dict[str, Any]] = Field(
@@ -6833,22 +7987,28 @@
         description="Destination schema prefix. Prefix for each replicated schema. For example with prefix 'x', source schemas 'foo' and 'bar' get replicated as 'x_foo' and 'x_bar'. The prefix is permanent and cannot be changed after connection creation",
         title="Destination schema prefix",
     )
     user: Optional[str] = Field(None, description="The user name.", title="")
 
 
 class MysqlRdsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config133] = Field(None, description="")
 
 
 class MysqlRdsNewConnectorRequestV1(NewConnectorRequestV1, MysqlRdsConfigV1):
+    """ """
+
     pass
 
 
 class Config134(BaseModel):
+    """ """
+
     consumer_key: Optional[str] = Field(None, title="")
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
@@ -6861,22 +8021,28 @@
     host: Optional[str] = Field(None, description="The NetSuite service host address.", title="")
     token_key: Optional[str] = Field(None, title="")
     account: Optional[str] = Field(None, description="The NetSuite Account ID.", title="")
     email: Optional[str] = Field(None, description="The NetSuite user's email address.", title="")
 
 
 class NetsuiteSuiteanalyticsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config134] = Field(None, description="")
 
 
 class NetsuiteSuiteanalyticsNewConnectorRequestV1(NewConnectorRequestV1, NetsuiteSuiteanalyticsConfigV1):
+    """ """
+
     pass
 
 
 class Config135(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     append_file_option: Optional[Dict[str, Any]] = Field(None, title="")
@@ -6893,69 +8059,89 @@
     file_type: Optional[Dict[str, Any]] = Field(None, title="")
     on_error: Optional[Dict[str, Any]] = Field(None, title="")
     compression: Optional[Dict[str, Any]] = Field(None, title="")
     archive_pattern: Optional[str] = Field(None, title="")
 
 
 class ClientAccess26(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth39(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess26] = None
 
 
 class OneDriveConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config135] = Field(None, description="")
     auth: Optional[Auth39] = None
 
 
 class OneDriveNewConnectorRequestV1(NewConnectorRequestV1, OneDriveConfigV1):
+    """ """
+
     pass
 
 
 class Config136(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     account_id: Optional[str] = Field(None, description="Your Optimizely account ID.", title="")
     enriched_export: Optional[str] = Field(None, title="")
 
 
 class ClientAccess27(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth40(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess27] = None
 
 
 class OptimizelyConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config136] = Field(None, description="")
     auth: Optional[Auth40] = None
 
 
 class OptimizelyNewConnectorRequestV1(NewConnectorRequestV1, OptimizelyConfigV1):
+    """ """
+
     pass
 
 
 class Config137(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     agent_user: Optional[str] = Field(None, title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`Directly`, `PrivateLink`, `SshTunnel`. `SshTunnel` is used as a value if this parameter is omitted in the request and any of the following parameter's values is specified: `tunnel_host`, `tunnel_port`, `tunnel_user`. Otherwise, `Directly` is used as a value if the parameter is omitted.",
         title="",
     )
@@ -6995,22 +8181,28 @@
     sap_user: Optional[str] = Field(None, description="", title="")
     agent_host: Optional[str] = Field(None, title="")
     user: Optional[str] = Field(None, description="The user name.", title="")
     asm_password: Optional[str] = Field(None, title="")
 
 
 class OracleConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config137] = Field(None, description="")
 
 
 class OracleNewConnectorRequestV1(NewConnectorRequestV1, OracleConfigV1):
+    """ """
+
     pass
 
 
 class Config138(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     agent_user: Optional[str] = Field(None, title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`Directly`, `PrivateLink`, `SshTunnel`. `SshTunnel` is used as a value if this parameter is omitted in the request and any of the following parameter's values is specified: `tunnel_host`, `tunnel_port`, `tunnel_user`. Otherwise, `Directly` is used as a value if the parameter is omitted.",
         title="",
     )
@@ -7050,22 +8242,28 @@
     sap_user: Optional[str] = Field(None, description="", title="")
     agent_host: Optional[str] = Field(None, title="")
     user: Optional[str] = Field(None, description="The user name.", title="")
     asm_password: Optional[str] = Field(None, title="")
 
 
 class OracleEbsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config138] = Field(None, description="")
 
 
 class OracleEbsNewConnectorRequestV1(NewConnectorRequestV1, OracleEbsConfigV1):
+    """ """
+
     pass
 
 
 class Config139(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     agent_user: Optional[str] = Field(None, title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`Directly`, `PrivateLink`, `SshTunnel`. `SshTunnel` is used as a value if this parameter is omitted in the request and any of the following parameter's values is specified: `tunnel_host`, `tunnel_port`, `tunnel_user`. Otherwise, `Directly` is used as a value if the parameter is omitted.",
         title="",
     )
@@ -7109,22 +8307,28 @@
     sap_user: Optional[str] = Field(None, description="", title="")
     agent_host: Optional[str] = Field(None, title="")
     user: Optional[str] = Field(None, description="The user name.", title="")
     asm_password: Optional[str] = Field(None, title="")
 
 
 class OracleHvaConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config139] = Field(None, description="")
 
 
 class OracleHvaNewConnectorRequestV1(NewConnectorRequestV1, OracleHvaConfigV1):
+    """ """
+
     pass
 
 
 class Config140(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     agent_user: Optional[str] = Field(None, title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`Directly`, `PrivateLink`, `SshTunnel`. `SshTunnel` is used as a value if this parameter is omitted in the request and any of the following parameter's values is specified: `tunnel_host`, `tunnel_port`, `tunnel_user`. Otherwise, `Directly` is used as a value if the parameter is omitted.",
         title="",
     )
@@ -7164,22 +8368,28 @@
     sap_user: Optional[str] = Field(None, description="", title="")
     agent_host: Optional[str] = Field(None, title="")
     user: Optional[str] = Field(None, description="The user name.", title="")
     asm_password: Optional[str] = Field(None, title="")
 
 
 class OracleRacConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config140] = Field(None, description="")
 
 
 class OracleRacNewConnectorRequestV1(NewConnectorRequestV1, OracleRacConfigV1):
+    """ """
+
     pass
 
 
 class Config141(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     agent_user: Optional[str] = Field(None, title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`Directly`, `PrivateLink`, `SshTunnel`. `SshTunnel` is used as a value if this parameter is omitted in the request and any of the following parameter's values is specified: `tunnel_host`, `tunnel_port`, `tunnel_user`. Otherwise, `Directly` is used as a value if the parameter is omitted.",
         title="",
     )
@@ -7219,127 +8429,165 @@
     sap_user: Optional[str] = Field(None, description="", title="")
     agent_host: Optional[str] = Field(None, title="")
     user: Optional[str] = Field(None, description="The user name.", title="")
     asm_password: Optional[str] = Field(None, title="")
 
 
 class OracleRdsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config141] = Field(None, description="")
 
 
 class OracleRdsNewConnectorRequestV1(NewConnectorRequestV1, OracleRdsConfigV1):
+    """ """
+
     pass
 
 
 class Config142(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     password: Optional[str] = Field(None, description="The Outbrain user's password.", title="")
     timeframe_months: Optional[Dict[str, Any]] = Field(None, title="")
     user: Optional[str] = Field(None, description="The username or email of the Outbrain user.", title="")
 
 
 class OutbrainConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config142] = Field(None, description="")
 
 
 class OutbrainNewConnectorRequestV1(NewConnectorRequestV1, OutbrainConfigV1):
+    """ """
+
     pass
 
 
 class Config143(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
 
 
 class Auth41(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
 
 
 class OutreachConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config143] = Field(None, description="")
     auth: Optional[Auth41] = None
 
 
 class OutreachNewConnectorRequestV1(NewConnectorRequestV1, OutreachConfigV1):
+    """ """
+
     pass
 
 
 class Config144(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     password: Optional[str] = Field(None, description="The Pardot user's password.", title="")
     business_unit_id: Optional[str] = Field(None, description="Business Unit Id", title="")
     user_key: Optional[str] = Field(None, description="The Pardot user's API key.", title="")
     api_version: Optional[Dict[str, Any]] = Field(None, description="API Version", title="")
     email: Optional[str] = Field(None, description="The email of the Pardot user.", title="")
 
 
 class PardotConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config144] = Field(None, description="")
 
 
 class PardotNewConnectorRequestV1(NewConnectorRequestV1, PardotConfigV1):
+    """ """
+
     pass
 
 
 class Config145(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     secret_key: Optional[str] = Field(None, description="`Client Secret` of your PayPal client application.", title="")
     client_id: Optional[str] = Field(None, description="`Client ID` of your PayPal client application.", title="")
 
 
 class PaypalConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config145] = Field(None, description="")
 
 
 class PaypalNewConnectorRequestV1(NewConnectorRequestV1, PaypalConfigV1):
+    """ """
+
     pass
 
 
 class Config146(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     secret_key: Optional[str] = Field(None, description="`Client Secret` of your PayPal client application.", title="")
     client_id: Optional[str] = Field(None, description="`Client ID` of your PayPal client application.", title="")
 
 
 class PaypalSandboxConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config146] = Field(None, description="")
 
 
 class PaypalSandboxNewConnectorRequestV1(NewConnectorRequestV1, PaypalSandboxConfigV1):
+    """ """
+
     pass
 
 
 class Config147(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None,
         description="Whether to sync all App IDs or specific App IDs. Default value: `AllAppIds`.",
         title="",
     )
     schema_: Optional[str] = Field(
         None,
@@ -7353,22 +8601,28 @@
         description="Specific App IDs to sync. Must be populated if `sync_mode` is set to `SpecificAppIds`.",
         title="",
     )
     region: Optional[Dict[str, Any]] = Field(None, description="The Pendo account region.", title="")
 
 
 class PendoConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config147] = Field(None, description="")
 
 
 class PendoNewConnectorRequestV1(NewConnectorRequestV1, PendoConfigV1):
+    """ """
+
     pass
 
 
 class Config148(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None,
         description="Whether to sync all advertisers or specific advertisers.",
         title="",
     )
     schema_: Optional[str] = Field(
         None,
@@ -7405,66 +8659,86 @@
         None,
         description="The number of days to use as the conversion attribution window for a 'click' action.",
         title="",
     )
 
 
 class ClientAccess28(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth42(BaseModel):
+    """ """
+
     client_access: Optional[ClientAccess28] = None
 
 
 class PinterestAdsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config148] = Field(None, description="")
     auth: Optional[Auth42] = None
 
 
 class PinterestAdsNewConnectorRequestV1(NewConnectorRequestV1, PinterestAdsConfigV1):
+    """ """
+
     pass
 
 
 class Config149(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     webhook_url: Optional[str] = Field(None, title="")
     api_token: Optional[str] = Field(None, description="(Optional)Your Pipedrive personal API token", title="")
     domain: Optional[str] = Field(None, description="Your Pipedrive domain.", title="")
 
 
 class ClientAccess29(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth43(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess29] = None
 
 
 class PipedriveConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config149] = Field(None, description="")
     auth: Optional[Auth43] = None
 
 
 class PipedriveNewConnectorRequestV1(NewConnectorRequestV1, PipedriveConfigV1):
+    """ """
+
     pass
 
 
 class Config150(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     publication_name: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`Directly`, `PrivateLink`, `SshTunnel`. `SshTunnel` is used as a value if this parameter is omitted in the request and any of the following parameter's values is specified: `tunnel_host`, `tunnel_port`, `tunnel_user`. Otherwise, `Directly` is used as a value if the parameter is omitted.",
         title="",
     )
@@ -7504,22 +8778,28 @@
         description='Replication slot name. Specify only for `"updated_method": "WAL"` or `"WAL_PGOUTPUT"`.',
         title="",
     )
     user: Optional[str] = Field(None, description="The user name.", title="")
 
 
 class PostgresConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config150] = Field(None, description="")
 
 
 class PostgresNewConnectorRequestV1(NewConnectorRequestV1, PostgresConfigV1):
+    """ """
+
     pass
 
 
 class Config151(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     publication_name: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(
         None,
         description="Possible values:`Directly`, `PrivateLink`, `SshTunnel`. `SshTunnel` is used as a value if this parameter is omitted in the request and any of the following parameter's values is specified: `tunnel_host`, `tunnel_port`, `tunnel_user`. Otherwise, `Directly` is used as a value if the parameter is omitted.",
         title="",
     )
@@ -7559,22 +8839,28 @@
         description='Replication slot name. Specify only for `"updated_method": "WAL"` or `"WAL_PGOUTPUT"`.',
         title="",
     )
     user: Optional[str] = Field(None, description="The user name.", title="")
 
 
 class PostgresRdsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config151] = Field(None, description="")
 
 
 class PostgresRdsNewConnectorRequestV1(NewConnectorRequestV1, PostgresRdsConfigV1):
+    """ """
+
     pass
 
 
 class Config152(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     api_token: Optional[str] = Field(None, description="API token of the Qualtrics account.", title="")
@@ -7582,91 +8868,119 @@
         None,
         description="Data center ID of the Qualtrics account. Can be found in the URL before `qualtrics.com`. (For example, if your URL is `youraccount.ca1.qualtrics.com`, then the data center is `ca1`.)",
         title="",
     )
 
 
 class QualtricsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config152] = Field(None, description="")
 
 
 class QualtricsNewConnectorRequestV1(NewConnectorRequestV1, QualtricsConfigV1):
+    """ """
+
     pass
 
 
 class Config153(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
 
 
 class ClientAccess30(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth44(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess30] = None
     realm_id: Optional[str] = Field(None, description="Realm ID of your application.")
 
 
 class QuickbooksConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config153] = Field(None, description="")
     auth: Optional[Auth44] = None
 
 
 class QuickbooksNewConnectorRequestV1(NewConnectorRequestV1, QuickbooksConfigV1):
+    """ """
+
     pass
 
 
 class Config154(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     api_token: Optional[str] = Field(None, description="The Recharge API token.", title="")
 
 
 class RechargeConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config154] = Field(None, description="")
 
 
 class RechargeNewConnectorRequestV1(NewConnectorRequestV1, RechargeConfigV1):
+    """ """
+
     pass
 
 
 class Config155(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     api_key: Optional[str] = Field(None, description="The Recurly API key.", title="")
     sub_domain: Optional[str] = Field(None, description="Your company's Recurly subdomain.", title="")
 
 
 class RecurlyConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config155] = Field(None, description="")
 
 
 class RecurlyNewConnectorRequestV1(NewConnectorRequestV1, RecurlyConfigV1):
+    """ """
+
     pass
 
 
 class CustomReport(BaseModel):
+    """ """
+
     custom_events_included: Optional[bool] = Field(
         None,
         description="The boolean value specifying whether the custom events are included in event conversions report. Default value: `false`",
         title="",
     )
     conversions_report_included: Optional[bool] = Field(
         None,
@@ -7687,14 +9001,16 @@
         None,
         description="The table name within the schema to which connector syncs the data of the specific report.",
         title="",
     )
 
 
 class Config156(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     timeframe_months: Optional[Dict[str, Any]] = Field(
@@ -7706,41 +9022,51 @@
         None,
         description="The list of custom report configurations. Each report corresponds to a table within the schema to which connector will sync the data.",
         title="",
     )
 
 
 class ClientAccess31(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth45(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess31] = None
     realm_id: Optional[str] = Field(None, description="Realm ID of your application.")
 
 
 class RedditAdsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config156] = Field(None, description="")
     auth: Optional[Auth45] = None
 
 
 class RedditAdsNewConnectorRequestV1(NewConnectorRequestV1, RedditAdsConfigV1):
+    """ """
+
     pass
 
 
 class Config157(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     append_file_option: Optional[Dict[str, Any]] = Field(
@@ -7821,22 +9147,28 @@
         None,
         description="Files inside of compressed archives with filenames matching this regular expression will be synced.",
         title="",
     )
 
 
 class S3ConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config157] = Field(None, description="")
 
 
 class S3NewConnectorRequestV1(NewConnectorRequestV1, S3ConfigV1):
+    """ """
+
     pass
 
 
 class Config158(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     login_password: Optional[str] = Field(
@@ -7845,22 +9177,28 @@
         title="",
     )
     user_i_d: Optional[str] = Field(None, title="")
     company_i_d: Optional[str] = Field(None, title="")
 
 
 class SageIntacctConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config158] = Field(None, description="")
 
 
 class SageIntacctNewConnectorRequestV1(NewConnectorRequestV1, SageIntacctConfigV1):
+    """ """
+
     pass
 
 
 class Config159(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     s3path: Optional[str] = Field(None, title="")
@@ -7868,22 +9206,28 @@
     is_sailthru_connect_enabled: Optional[bool] = Field(None, title="")
     is_valid_credential: Optional[bool] = Field(None, title="")
     api_secret: Optional[str] = Field(None, description="The Sailthru API secret.", title="")
     group_region: Optional[Dict[str, Any]] = Field(None, title="")
 
 
 class SailthruConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config159] = Field(None, description="")
 
 
 class SailthruNewConnectorRequestV1(NewConnectorRequestV1, SailthruConfigV1):
+    """ """
+
     pass
 
 
 class Config160(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     password: Optional[str] = Field(None, title="")
@@ -7892,36 +9236,46 @@
         description="(Optional) The custom Salesforce domain. Make sure that the `base_url` starts with `https://`.",
         title="",
     )
     username: Optional[str] = Field(None, title="")
 
 
 class ClientAccess32(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth46(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess32] = None
 
 
 class SalesforceConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config160] = Field(None, description="")
     auth: Optional[Auth46] = None
 
 
 class SalesforceNewConnectorRequestV1(NewConnectorRequestV1, SalesforceConfigV1):
+    """ """
+
     pass
 
 
 class Config161(BaseModel):
+    """ """
+
     is_new_package: Optional[bool] = Field(
         None,
         description="Indicates that that your installed package uses OAuth 2.0. Default value: `false`",
         title="",
     )
     schema_: Optional[str] = Field(
         None,
@@ -7933,22 +9287,28 @@
     instance: Optional[str] = Field(None, description="The Salesforce Marketing Cloud instance ID", title="")
     sub_domain: Optional[str] = Field(None, title="")
     client_secret: Optional[str] = Field(None, description="The Salesforce Marketing Cloud client secret.", title="")
     client_id: Optional[str] = Field(None, description="The Salesforce Marketing Cloud client ID.", title="")
 
 
 class SalesforceMarketingCloudConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config161] = Field(None, description="")
 
 
 class SalesforceMarketingCloudNewConnectorRequestV1(NewConnectorRequestV1, SalesforceMarketingCloudConfigV1):
+    """ """
+
     pass
 
 
 class Config162(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     password: Optional[str] = Field(None, title="")
@@ -7957,56 +9317,72 @@
         description="(Optional) The custom Salesforce domain. Make sure that the `base_url` starts with `https://`.",
         title="",
     )
     username: Optional[str] = Field(None, title="")
 
 
 class ClientAccess33(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth47(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess33] = None
 
 
 class SalesforceSandboxConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config162] = Field(None, description="")
     auth: Optional[Auth47] = None
 
 
 class SalesforceSandboxNewConnectorRequestV1(NewConnectorRequestV1, SalesforceSandboxConfigV1):
+    """ """
+
     pass
 
 
 class Config163(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     password: Optional[str] = Field(None, description="The SAP Business ByDesign password.", title="")
     instance_url: Optional[str] = Field(None, description="The SAP Business ByDesign instance URL.", title="")
     username: Optional[str] = Field(None, description="The SAP Business ByDesign username.", title="")
 
 
 class SapBusinessByDesignConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config163] = Field(None, description="")
 
 
 class SapBusinessByDesignNewConnectorRequestV1(NewConnectorRequestV1, SapBusinessByDesignConfigV1):
+    """ """
+
     pass
 
 
 class Config164(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     append_file_option: Optional[Dict[str, Any]] = Field(None, title="")
@@ -8038,62 +9414,80 @@
     on_error: Optional[Dict[str, Any]] = Field(None, title="")
     compression: Optional[Dict[str, Any]] = Field(None, title="")
     table: Optional[str] = Field(None, title="")
     archive_pattern: Optional[str] = Field(None, title="")
 
 
 class SegmentConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config164] = Field(None, description="")
 
 
 class SegmentNewConnectorRequestV1(NewConnectorRequestV1, SegmentConfigV1):
+    """ """
+
     pass
 
 
 class Config165(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     api_key: Optional[str] = Field(None, description="The SendGrid API key.", title="")
 
 
 class SendgridConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config165] = Field(None, description="")
 
 
 class SendgridNewConnectorRequestV1(NewConnectorRequestV1, SendgridConfigV1):
+    """ """
+
     pass
 
 
 class Config166(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     password: Optional[str] = Field(None, description="Your account password.", title="")
     instance: Optional[str] = Field(None, description="ServiceNow Instance ID.", title="")
     client_secret: Optional[str] = Field(None, description="ServiceNow Client Secret.", title="")
     client_id: Optional[str] = Field(None, description="ServiceNow Client ID.", title="")
     username: Optional[str] = Field(None, description="Your ServiceNow User ID (username).", title="")
 
 
 class ServicenowConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config166] = Field(None, description="")
 
 
 class ServicenowNewConnectorRequestV1(NewConnectorRequestV1, ServicenowConfigV1):
+    """ """
+
     pass
 
 
 class Config167(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, title="")
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
@@ -8171,22 +9565,28 @@
         description="The secrets that should be passed to the function at runtime.",
         title="",
     )
     user: Optional[str] = Field(None, description="SFTP user.", title="")
 
 
 class SftpConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config167] = Field(None, description="")
 
 
 class SftpNewConnectorRequestV1(NewConnectorRequestV1, SftpConfigV1):
+    """ """
+
     pass
 
 
 class Config168(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     append_file_option: Optional[Dict[str, Any]] = Field(
@@ -8264,71 +9664,89 @@
         None,
         description="Destination table. Table is permanent and cannot be changed after connection creation",
         title="Destination table",
     )
 
 
 class ClientAccess34(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth48(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess34] = None
 
 
 class SharePointConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config168] = Field(None, description="")
     auth: Optional[Auth48] = None
 
 
 class SharePointNewConnectorRequestV1(NewConnectorRequestV1, SharePointConfigV1):
+    """ """
+
     pass
 
 
 class Config169(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     shop: Optional[str] = Field(
         None,
         description="The Shopify shop name. Can be found in the URL before **.myshopify.com**.",
         title="",
     )
 
 
 class Auth49(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     realm_id: Optional[str] = Field(None, description="Realm ID of your application.")
 
 
 class ShopifyConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config169] = Field(None, description="")
     auth: Optional[Auth49] = None
 
 
 class ShopifyNewConnectorRequestV1(NewConnectorRequestV1, ShopifyConfigV1):
+    """ """
+
     pass
 
 
 class Config170(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None,
         description="Whether to sync all organizations or specific organizations. Default value: `AllOrganizations`.",
         title="",
     )
     schema_: Optional[str] = Field(
         None,
@@ -8355,77 +9773,99 @@
         None,
         description="Specific organizations IDs to sync. Must be populated if `syncMode` is set to `SpecificOrganizations`.",
         title="",
     )
 
 
 class ClientAccess35(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth50(BaseModel):
+    """ """
+
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess35] = None
 
 
 class SnapchatAdsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config170] = Field(None, description="")
     auth: Optional[Auth50] = None
 
 
 class SnapchatAdsNewConnectorRequestV1(NewConnectorRequestV1, SnapchatAdsConfigV1):
+    """ """
+
     pass
 
 
 class Config171(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     endpoint: Optional[str] = Field(None, title="")
     config_repository_u_r_l: Optional[str] = Field(None, title="")
     enable_enrichments: Optional[bool] = Field(None, title="")
 
 
 class SnowplowConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config171] = Field(None, description="")
 
 
 class SnowplowNewConnectorRequestV1(NewConnectorRequestV1, SnowplowConfigV1):
+    """ """
+
     pass
 
 
 class Config172(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     password: Optional[str] = Field(None, description="The Splunk user's password.", title="")
     port: Optional[int] = Field(None, description="The Splunk service host port.", title="")
     host: Optional[str] = Field(None, description="The Splunk service host address.", title="")
     user: Optional[str] = Field(None, description="The Splunk username.", title="")
 
 
 class SplunkConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config172] = Field(None, description="")
 
 
 class SplunkNewConnectorRequestV1(NewConnectorRequestV1, SplunkConfigV1):
+    """ """
+
     pass
 
 
 class Config173(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     agent_user: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(None, description="", title="")
     agent_password: Optional[str] = Field(None, description="", title="")
     always_encrypted: Optional[bool] = Field(None, title="")
     agent_public_cert: Optional[str] = Field(None, description="", title="")
     tunnel_user: Optional[str] = Field(
@@ -8459,35 +9899,43 @@
         None,
         description="The user name.  For Azure Databases, the format must be `user@domain`.",
         title="",
     )
 
 
 class Auth51(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     realm_id: Optional[str] = Field(None, description="Realm ID of your application.")
 
 
 class SqlServerConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config173] = Field(None, description="")
     auth: Optional[Auth51] = None
 
 
 class SqlServerNewConnectorRequestV1(NewConnectorRequestV1, SqlServerConfigV1):
+    """ """
+
     pass
 
 
 class Config174(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     agent_user: Optional[str] = Field(None, title="")
     connection_type: Optional[Dict[str, Any]] = Field(None, description="", title="")
     agent_password: Optional[str] = Field(None, title="")
     always_encrypted: Optional[bool] = Field(None, title="")
     agent_public_cert: Optional[str] = Field(None, title="")
     tunnel_user: Optional[str] = Field(
@@ -8521,35 +9969,43 @@
         None,
         description="The user name.  For Azure Databases, the format must be `user@domain`.",
         title="",
     )
 
 
 class Auth52(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     realm_id: Optional[str] = Field(None, description="Realm ID of your application.")
 
 
 class SqlServerHvaConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config174] = Field(None, description="")
     auth: Optional[Auth52] = None
 
 
 class SqlServerHvaNewConnectorRequestV1(NewConnectorRequestV1, SqlServerHvaConfigV1):
+    """ """
+
     pass
 
 
 class Config175(BaseModel):
+    """ """
+
     public_key: Optional[str] = Field(None, description="", title="")
     agent_user: Optional[str] = Field(None, description="", title="")
     connection_type: Optional[Dict[str, Any]] = Field(None, description="", title="")
     agent_password: Optional[str] = Field(None, description="", title="")
     always_encrypted: Optional[bool] = Field(None, title="")
     agent_public_cert: Optional[str] = Field(None, description="", title="")
     tunnel_user: Optional[str] = Field(
@@ -8583,35 +10039,43 @@
         None,
         description="The user name.  For Azure Databases, the format must be `user@domain`.",
         title="",
     )
 
 
 class Auth53(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     realm_id: Optional[str] = Field(None, description="Realm ID of your application.")
 
 
 class SqlServerRdsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config175] = Field(None, description="")
     auth: Optional[Auth53] = None
 
 
 class SqlServerRdsNewConnectorRequestV1(NewConnectorRequestV1, SqlServerRdsConfigV1):
+    """ """
+
     pass
 
 
 class Config176(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     api_access_token: Optional[str] = Field(
@@ -8619,22 +10083,28 @@
         description="Square App user the access token specific to your Application.",
         title="",
     )
     client_id: Optional[str] = Field(None, description="The Application ID specific to your organization.", title="")
 
 
 class SquareConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config176] = Field(None, description="")
 
 
 class SquareNewConnectorRequestV1(NewConnectorRequestV1, SquareConfigV1):
+    """ """
+
     pass
 
 
 class Config177(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     support_connected_accounts_sync: Optional[bool] = Field(
@@ -8642,30 +10112,38 @@
         description="Sync Connected Accounts. Connected Account Documentation - https://stripe.com/docs/api/connected_accounts.",
         title="",
     )
     api_key: Optional[str] = Field(None, description="Restricted API key", title="")
 
 
 class Auth54(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
 
 
 class StripeConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config177] = Field(None, description="")
     auth: Optional[Auth54] = None
 
 
 class StripeNewConnectorRequestV1(NewConnectorRequestV1, StripeConfigV1):
+    """ """
+
     pass
 
 
 class Config178(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     support_connected_accounts_sync: Optional[bool] = Field(
@@ -8673,66 +10151,84 @@
         description="Sync Connected Accounts. Connected Account Documentation - https://stripe.com/docs/api/connected_accounts.",
         title="",
     )
     api_key: Optional[str] = Field(None, description="Restricted API key", title="")
 
 
 class Auth55(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
 
 
 class StripeTestConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config178] = Field(None, description="")
     auth: Optional[Auth55] = None
 
 
 class StripeTestNewConnectorRequestV1(NewConnectorRequestV1, StripeTestConfigV1):
+    """ """
+
     pass
 
 
 class Config179(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     eu_region: Optional[bool] = Field(
         None,
         description="The SurveyMonkey account region. Specify `true`, if your account is hosted in the EU region. Default value is `false`.",
         title="",
     )
 
 
 class ClientAccess36(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth56(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
     client_access: Optional[ClientAccess36] = None
 
 
 class SurveyMonkeyConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config179] = Field(None, description="")
     auth: Optional[Auth56] = None
 
 
 class SurveyMonkeyNewConnectorRequestV1(NewConnectorRequestV1, SurveyMonkeyConfigV1):
+    """ """
+
     pass
 
 
 class Config180(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None, description="Whether to sync all accounts or specific accounts.", title=""
     )
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
@@ -8745,22 +10241,28 @@
     )
     timeframe_months: Optional[Dict[str, Any]] = Field(None, title="")
     client_secret: Optional[str] = Field(None, description="The Taboola client secret.", title="")
     client_id: Optional[str] = Field(None, description="The Taboola client ID.", title="")
 
 
 class TaboolaConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config180] = Field(None, description="")
 
 
 class TaboolaNewConnectorRequestV1(NewConnectorRequestV1, TaboolaConfigV1):
+    """ """
+
     pass
 
 
 class Config181(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None,
         description="Whether to sync all advertiser accounts or specific accounts.",
         title="",
     )
     schema_: Optional[str] = Field(
         None,
@@ -8777,36 +10279,46 @@
         None,
         description="Specific accounts to sync.  Must be populated if `sync_mode` is set to `SpecificAccounts`.",
         title="",
     )
 
 
 class ClientAccess37(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth57(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
     client_access: Optional[ClientAccess37] = None
 
 
 class TiktokAdsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config181] = Field(None, description="")
     auth: Optional[Auth57] = None
 
 
 class TiktokAdsNewConnectorRequestV1(NewConnectorRequestV1, TiktokAdsConfigV1):
+    """ """
+
     pass
 
 
 class Config182(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None, description="Whether to sync all accounts or specific accounts.", title=""
     )
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
@@ -8818,22 +10330,28 @@
         description="Specific Accounts to sync.  Must be populated if `sync_mode` is set to `SpecificAccounts`.",
         title="",
     )
     sid: Optional[str] = Field(None, description="The Twilio API key SID", title="")
 
 
 class TwilioConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config182] = Field(None, description="")
 
 
 class TwilioNewConnectorRequestV1(NewConnectorRequestV1, TwilioConfigV1):
+    """ """
+
     pass
 
 
 class Config183(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None,
         description="Whether to sync all accounts or specific accounts. Default value: `AllAccounts`.",
         title="",
     )
     consumer_key: Optional[str] = Field(None, description="", title="")
     schema_: Optional[str] = Field(
@@ -8852,42 +10370,52 @@
         None,
         description="Specific accounts to sync. Must be populated if `sync_mode` is set to `SpecificAccounts`.",
         title="",
     )
 
 
 class ClientAccess38(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth58(BaseModel):
+    """ """
+
     consumer_key: Optional[str] = Field(None, description="API Key of your app")
     consumer_secret: Optional[str] = Field(None, description="API Secret of your app")
     client_access: Optional[ClientAccess38] = None
     oauth_token: Optional[str] = Field(
         None,
         description="The Access token carries the information necessary to access API resources",
     )
     oauth_token_secret: Optional[str] = Field(
         None,
         description="The Access token secret carry the information necessary to access API resources.",
     )
 
 
 class TwitterConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config183] = Field(None, description="")
     auth: Optional[Auth58] = None
 
 
 class TwitterNewConnectorRequestV1(NewConnectorRequestV1, TwitterConfigV1):
+    """ """
+
     pass
 
 
 class Config184(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None, description="Whether to sync all accounts or specific accounts.", title=""
     )
     consumer_key: Optional[str] = Field(None, description="The Twitter App consumer key.", title="")
     schema_: Optional[str] = Field(
         None,
         alias="schema",
@@ -8903,77 +10431,97 @@
         None,
         description="Specific Accounts to sync.  Must be populated if `sync_mode` is set to `SpecificAccounts`.",
         title="",
     )
 
 
 class ClientAccess39(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth59(BaseModel):
+    """ """
+
     consumer_key: Optional[str] = Field(None, description="API Key of your app")
     consumer_secret: Optional[str] = Field(None, description="API Secret of your app")
     client_access: Optional[ClientAccess39] = None
     oauth_token: Optional[str] = Field(
         None,
         description="The Access token carries the information necessary to access API resources",
     )
     oauth_token_secret: Optional[str] = Field(
         None,
         description="The Access token secret carry the information necessary to access API resources.",
     )
 
 
 class TwitterAdsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config184] = Field(None, description="")
     auth: Optional[Auth59] = None
 
 
 class TwitterAdsNewConnectorRequestV1(NewConnectorRequestV1, TwitterAdsConfigV1):
+    """ """
+
     pass
 
 
 class Config185(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
 
 
 class ClientAccess40(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth60(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     client_access: Optional[ClientAccess40] = None
 
 
 class TypeformConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config185] = Field(None, description="")
     auth: Optional[Auth60] = None
 
 
 class TypeformNewConnectorRequestV1(NewConnectorRequestV1, TypeformConfigV1):
+    """ """
+
     pass
 
 
 class Config186(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     domain: Optional[str] = Field(
@@ -8982,22 +10530,28 @@
         title="",
     )
     secret: Optional[str] = Field(None, description="The UserVoice API secret.", title="")
     key: Optional[str] = Field(None, description="The UserVoice API key.", title="")
 
 
 class UservoiceConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config186] = Field(None, description="")
 
 
 class UservoiceNewConnectorRequestV1(NewConnectorRequestV1, UservoiceConfigV1):
+    """ """
+
     pass
 
 
 class Config187(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     endpoint: Optional[str] = Field(
@@ -9039,36 +10593,48 @@
         None,
         description="Destination table. Table is permanent and cannot be changed after connection creation",
         title="Destination table",
     )
 
 
 class WebhooksConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config187] = Field(None, description="")
 
 
 class WebhooksNewConnectorRequestV1(NewConnectorRequestV1, WebhooksConfigV1):
+    """ """
+
     pass
 
 
 class Config188(BaseModel):
+    """ """
+
     consumer_key: Optional[str] = Field(None, description="Your WooCommerce Consumer key.", title="")
     consumer_secret: Optional[str] = Field(None, description="Your WooCommerce Consumer secret.", title="")
     sub_domain: Optional[str] = Field(None, description="Your WooCommerce sub-domain.", title="")
 
 
 class WoocommerceConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config188] = Field(None, description="")
 
 
 class WoocommerceNewConnectorRequestV1(NewConnectorRequestV1, WoocommerceConfigV1):
+    """ """
+
     pass
 
 
 class Config189(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     password: Optional[str] = Field(None, description="Workday password.", title="")
@@ -9079,59 +10645,77 @@
         None,
         description="Destination table. Table is permanent and cannot be changed after connection creation",
         title="Destination table",
     )
 
 
 class WorkdayConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config189] = Field(None, description="")
 
 
 class WorkdayNewConnectorRequestV1(NewConnectorRequestV1, WorkdayConfigV1):
+    """ """
+
     pass
 
 
 class Config190(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     password: Optional[str] = Field(None, description="Workday password.", title="")
     domain_host_name: Optional[str] = Field(None, description="Workday host name.", title="")
     username: Optional[str] = Field(None, title="")
 
 
 class WorkdayHcmConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config190] = Field(None, description="")
 
 
 class WorkdayHcmNewConnectorRequestV1(NewConnectorRequestV1, WorkdayHcmConfigV1):
+    """ """
+
     pass
 
 
 class Config191(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
 
 
 class XeroConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config191] = Field(None, description="")
 
 
 class XeroNewConnectorRequestV1(NewConnectorRequestV1, XeroConfigV1):
+    """ """
+
     pass
 
 
 class Config192(BaseModel):
+    """ """
+
     sync_mode: Optional[Dict[str, Any]] = Field(
         None,
         description="Whether to sync all accounts or specific accounts. Default value: `SpecificAccounts`.",
         title="",
     )
     schema_: Optional[str] = Field(
         None,
@@ -9148,32 +10732,42 @@
         None,
         description="Specific Advertiser IDs to sync. Must be populated if `syncMode` is set to `SpecificAccounts`.",
         title="",
     )
 
 
 class ClientAccess41(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth61(BaseModel):
+    """ """
+
     client_access: Optional[ClientAccess41] = None
 
 
 class YahooGeminiConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config192] = Field(None, description="")
     auth: Optional[Auth61] = None
 
 
 class YahooGeminiNewConnectorRequestV1(NewConnectorRequestV1, YahooGeminiConfigV1):
+    """ """
+
     pass
 
 
 class Config193(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     report_type: Optional[str] = Field(
@@ -9190,32 +10784,42 @@
         None,
         description="Destination table. Table is permanent and cannot be changed after connection creation",
         title="Destination table",
     )
 
 
 class ClientAccess42(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth62(BaseModel):
+    """ """
+
     client_access: Optional[ClientAccess42] = None
 
 
 class YoutubeAnalyticsConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config193] = Field(None, description="")
     auth: Optional[Auth62] = None
 
 
 class YoutubeAnalyticsNewConnectorRequestV1(NewConnectorRequestV1, YoutubeAnalyticsConfigV1):
+    """ """
+
     pass
 
 
 class Config194(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     domain: Optional[str] = Field(None, description="Zendesk domain.", title="")
@@ -9225,88 +10829,112 @@
         title="",
     )
     email: Optional[str] = Field(None, description="Zendesk email.", title="")
     api_usage: Optional[float] = Field(None, description="Maximum Zendesk Api Usage allowed", title="")
 
 
 class Auth63(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
 
 
 class ZendeskConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config194] = Field(None, description="")
     auth: Optional[Auth63] = None
 
 
 class ZendeskNewConnectorRequestV1(NewConnectorRequestV1, ZendeskConfigV1):
+    """ """
+
     pass
 
 
 class Config195(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     subdomain: Optional[str] = Field(None, description="Your Zendesk domain.", title="")
     client_secret: Optional[str] = Field(None, description="Your Zendesk client secret.", title="")
     client_id: Optional[str] = Field(None, description="Your Zendesk client ID.", title="")
 
 
 class Auth64(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
 
 
 class ZendeskChatConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config195] = Field(None, description="")
     auth: Optional[Auth64] = None
 
 
 class ZendeskChatNewConnectorRequestV1(NewConnectorRequestV1, ZendeskChatConfigV1):
+    """ """
+
     pass
 
 
 class Config196(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
 
 
 class Auth65(BaseModel):
+    """ """
+
     access_token: Optional[str] = Field(
         None,
         description="The long-lived Access token carries the information necessary to access API resources",
     )
     refresh_token: Optional[str] = Field(
         None,
         description="The long-lived Refresh token carry the information necessary to get a new access token for API resources.",
     )
     realm_id: Optional[str] = Field(None, description="Realm ID of your application.")
 
 
 class ZendeskSellConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config196] = Field(None, description="")
     auth: Optional[Auth65] = None
 
 
 class ZendeskSellNewConnectorRequestV1(NewConnectorRequestV1, ZendeskSellConfigV1):
+    """ """
+
     pass
 
 
 class Config197(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     api_token: Optional[str] = Field(
@@ -9315,50 +10943,66 @@
         title="",
     )
     domain: Optional[str] = Field(None, description="Zendesk domain.", title="")
     email: Optional[str] = Field(None, description="Zendesk email.", title="")
 
 
 class ZendeskSunshineConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config197] = Field(None, description="")
 
 
 class ZendeskSunshineNewConnectorRequestV1(NewConnectorRequestV1, ZendeskSunshineConfigV1):
+    """ """
+
     pass
 
 
 class Config198(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     data_center: Optional[str] = Field(None, description="", title="")
 
 
 class ClientAccess43(BaseModel):
+    """ """
+
     client_secret: Optional[str] = Field(None, description="Client Secret of your client application.")
     client_id: Optional[str] = Field(None, description="Client ID of your client application.")
 
 
 class Auth66(BaseModel):
+    """ """
+
     client_access: Optional[ClientAccess43] = None
 
 
 class ZohoCrmConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config198] = Field(None, description="")
     auth: Optional[Auth66] = None
 
 
 class ZohoCrmNewConnectorRequestV1(NewConnectorRequestV1, ZohoCrmConfigV1):
+    """ """
+
     pass
 
 
 class Config199(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     is_multi_entity_feature_enabled: Optional[bool] = Field(
@@ -9372,22 +11016,28 @@
         description="If `is_multi_entity_feature_enabled` is `true`, then it's `EntityId`.",
         title="",
     )
     client_id: Optional[str] = Field(None, description="Zuora Client ID.", title="")
 
 
 class ZuoraConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config199] = Field(None, description="")
 
 
 class ZuoraNewConnectorRequestV1(NewConnectorRequestV1, ZuoraConfigV1):
+    """ """
+
     pass
 
 
 class Config200(BaseModel):
+    """ """
+
     schema_: Optional[str] = Field(
         None,
         alias="schema",
         description="Destination schema. Schema is permanent and cannot be changed after connection creation",
         title="Destination schema",
     )
     is_multi_entity_feature_enabled: Optional[bool] = Field(
@@ -9401,545 +11051,741 @@
         description="If `is_multi_entity_feature_enabled` is `true`, then it's `EntityId`.",
         title="",
     )
     client_id: Optional[str] = Field(None, description="Zuora Client ID.", title="")
 
 
 class ZuoraSandboxConfigV1(BaseModel):
+    """ """
+
     config: Optional[Config200] = Field(None, description="")
 
 
 class ZuoraSandboxNewConnectorRequestV1(NewConnectorRequestV1, ZuoraSandboxConfigV1):
+    """ """
+
     pass
 
 
 class Data(BaseModel):
+    """ """
+
     items: Optional[List[MembershipResponse]] = Field(None, description="The collection of return items")
     nextCursor: Optional[str] = Field(None, description="The value of the cursor parameter for the next page")
 
 
 class V1TeamsTeamIdConnectorsGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[Data] = None
 
 
 class V1TeamsTeamIdConnectorsPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[MembershipResponse] = None
 
 
 class V1TeamsTeamIdUsersUserIdGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[TeamMembershipResponse] = None
 
 
 class V1TeamsTeamIdUsersUserIdDeleteResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class V1TeamsTeamIdUsersUserIdPatchResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class Data1(BaseModel):
+    """ """
+
     items: Optional[List[UserResponse]] = Field(None, description="The collection of return items")
     nextCursor: Optional[str] = Field(None, description="The value of the cursor parameter for the next page")
 
 
 class V1UsersGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[Data1] = None
 
 
 class V1UsersPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[UserResponse] = None
 
 
 class V1TeamsTeamIdGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[TeamResponse] = None
 
 
 class V1TeamsTeamIdDeleteResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class V1TeamsTeamIdPatchResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[TeamResponse] = None
 
 
 class V1TeamsTeamIdRoleDeleteResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class Data2(BaseModel):
+    """ """
+
     items: Optional[List[MembershipResponse]] = Field(None, description="The collection of return items")
     nextCursor: Optional[str] = Field(None, description="The value of the cursor parameter for the next page")
 
 
 class V1UsersUserIdGroupsGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[Data2] = None
 
 
 class V1UsersUserIdGroupsPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[MembershipResponse] = None
 
 
 class Data3(BaseModel):
+    """ """
+
     items: Optional[List[MembershipResponse]] = Field(None, description="The collection of return items")
     nextCursor: Optional[str] = Field(None, description="The value of the cursor parameter for the next page")
 
 
 class V1TeamsTeamIdGroupsGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[Data3] = None
 
 
 class V1TeamsTeamIdGroupsPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[MembershipResponse] = None
 
 
 class V1CertificatesPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class V1DestinationsPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[DestinationResponse] = None
 
 
 class V1UsersIdDeleteResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class V1UsersUserIdGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[UserResponse] = None
 
 
 class V1UsersUserIdPatchResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[UserResponse] = None
 
 
 class V1GroupsGroupIdGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[GroupResponse] = None
 
 
 class V1GroupsGroupIdDeleteResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class V1GroupsGroupIdPatchResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[GroupResponse] = None
 
 
 class V1UsersUserIdConnectorsConnectorIdGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[MembershipResponse] = None
 
 
 class V1UsersUserIdConnectorsConnectorIdDeleteResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[MembershipResponse] = None
 
 
 class V1UsersUserIdConnectorsConnectorIdPatchResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[MembershipResponse] = None
 
 
 class V1ConnectorsConnectorIdConnectCardPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[ConnectorConnectCardResponse] = None
 
 
 class Data4(BaseModel):
+    """ """
+
     items: Optional[List[MetadataResponse]] = Field(None, description="The collection of return items")
     nextCursor: Optional[str] = Field(None, description="The value of the cursor parameter for the next page")
 
 
 class V1MetadataNameGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[Data4] = None
 
 
 class V1DbtTransformationsTransformationIdGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[TransformationDetailsResponse] = None
 
 
 class V1DbtTransformationsTransformationIdDeleteResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class V1DbtTransformationsTransformationIdPatchResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[TransformationDetailsResponse] = None
 
 
 class V1DbtProjectsProjectIdGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[DbtProjectDetailsResponse] = None
 
 
 class V1TeamsTeamIdGroupsGroupIdGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[MembershipResponse] = None
 
 
 class V1TeamsTeamIdGroupsGroupIdDeleteResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class V1TeamsTeamIdGroupsGroupIdPatchResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class V1ConnectorsConnectorIdResyncPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class V1UsersUserIdRoleDeleteResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class Data5(BaseModel):
+    """ """
+
     items: Optional[List[UserResponse]] = Field(None, description="The collection of return items")
     nextCursor: Optional[str] = Field(None, description="The value of the cursor parameter for the next page")
 
 
 class V1GroupsGroupIdUsersGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[Data5] = None
 
 
 class V1GroupsGroupIdUsersPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class V1ConnectorsConnectorIdSchemasTablesResyncPostRequest(BaseModel):
+    """ """
+
     pass
 
     class Config:
+        """ """
+
         extra = Extra.allow
 
 
 class V1ConnectorsConnectorIdSchemasTablesResyncPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class V1DestinationsDestinationIdTestPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[DestinationResponse] = None
 
 
 class Data6(BaseModel):
+    """ """
+
     items: Optional[List[SchemaMetadataResponse]] = Field(None, description="The collection of return items")
     nextCursor: Optional[str] = Field(None, description="The value of the cursor parameter for the next page")
 
 
 class V1MetadataConnectorsConnectorIdSchemasGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[Data6] = None
 
 
 class Data7(BaseModel):
+    """ """
+
     items: Optional[List[GroupResponse]] = Field(None, description="The collection of return items")
     nextCursor: Optional[str] = Field(None, description="The value of the cursor parameter for the next page")
 
 
 class V1GroupsGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[Data7] = None
 
 
 class V1GroupsPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[GroupResponse] = None
 
 
 class V1FingerprintsPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class V1ConnectorsConnectorIdDeleteResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class V1MetadataNameServiceGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[MetadataResponse] = None
 
 
 class Data8(BaseModel):
+    """ """
+
     items: Optional[List[TeamResponse]] = Field(None, description="The collection of return items")
     nextCursor: Optional[str] = Field(None, description="The value of the cursor parameter for the next page")
 
 
 class V1TeamsGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[Data8] = None
 
 
 class V1TeamsPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[TeamResponse] = None
 
 
 class V1DbtProjectsProjectIdTestPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[DbtProjectTestResponse] = None
 
 
 class V1ConnectorsConnectorIdSyncPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class V1GroupsGroupIdUsersUserIdDeleteResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class Data9(BaseModel):
+    """ """
+
     items: Optional[List[ColumnMetadataResponse]] = Field(None, description="The collection of return items")
     nextCursor: Optional[str] = Field(None, description="The value of the cursor parameter for the next page")
 
 
 class V1MetadataConnectorsConnectorIdColumnsGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[Data9] = None
 
 
 class Data10(BaseModel):
+    """ """
+
     items: Optional[List[TableMetadataResponse]] = Field(None, description="The collection of return items")
     nextCursor: Optional[str] = Field(None, description="The value of the cursor parameter for the next page")
 
 
 class V1MetadataConnectorsConnectorIdTablesGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[Data10] = None
 
 
 class Data11(BaseModel):
+    """ """
+
     items: Optional[List[TransformationResponse]] = Field(None, description="The collection of return items")
     nextCursor: Optional[str] = Field(None, description="The value of the cursor parameter for the next page")
 
 
 class V1DbtProjectsProjectIdTransformationsGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[Data11] = None
 
 
 class V1DbtProjectsProjectIdTransformationsPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[TransformationDetailsResponse] = None
 
 
 class Data12(BaseModel):
+    """ """
+
     items: Optional[List[DbtProjectResponse]] = Field(None, description="The collection of return items")
     nextCursor: Optional[str] = Field(None, description="The value of the cursor parameter for the next page")
 
 
 class V1DbtProjectsGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[Data12] = None
 
 
 class V1DbtProjectsPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[DbtProjectDetailsResponse] = None
 
 
 class Data13(BaseModel):
+    """ """
+
     items: Optional[List[RoleResponse]] = Field(None, description="The collection of return items")
     nextCursor: Optional[str] = Field(None, description="The value of the cursor parameter for the next page")
 
 
 class V1RolesGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[Data13] = None
 
 
 class Data14(BaseModel):
+    """ """
+
     items: Optional[List[DbtModelResponse]] = Field(None, description="The collection of return items")
     nextCursor: Optional[str] = Field(None, description="The value of the cursor parameter for the next page")
 
 
 class V1DbtProjectsProjectIdModelsGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[Data14] = None
 
 
 class V1TeamsTeamIdConnectorsConnectorIdGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[MembershipResponse] = None
 
 
 class V1TeamsTeamIdConnectorsConnectorIdDeleteResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class V1TeamsTeamIdConnectorsConnectorIdPatchResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class Data15(BaseModel):
+    """ """
+
     items: Optional[List[ConnectorResponse]] = Field(None, description="The collection of return items")
     nextCursor: Optional[str] = Field(None, description="The value of the cursor parameter for the next page")
 
 
 class V1GroupsGroupIdConnectorsGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[Data15] = None
 
 
 class V1DestinationsDestinationIdGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[DestinationResponse] = None
 
 
 class V1DestinationsDestinationIdDeleteResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class V1DestinationsDestinationIdPatchResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[DestinationResponse] = None
 
 
 class V1WebhooksGetResponse(BaseModel):
+    """ """
+
     items: Optional[List[WebhookResponse]] = Field(None, description="The collection of return items")
     nextCursor: Optional[str] = Field(None, description="The value of the cursor parameter for the next page")
 
 
 class Data16(BaseModel):
+    """ """
+
     items: Optional[List[TeamMembershipResponse]] = Field(None, description="The collection of return items")
     nextCursor: Optional[str] = Field(None, description="The value of the cursor parameter for the next page")
 
 
 class V1TeamsTeamIdUsersGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[Data16] = None
 
 
 class V1TeamsTeamIdUsersPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[TeamMembershipResponse] = None
 
 
 class V1UsersUserIdGroupsGroupIdGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[MembershipResponse] = None
 
 
 class V1UsersUserIdGroupsGroupIdDeleteResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class V1UsersUserIdGroupsGroupIdPatchResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
 
 
 class Data17(BaseModel):
+    """ """
+
     items: Optional[List[MembershipResponse]] = Field(None, description="The collection of return items")
     nextCursor: Optional[str] = Field(None, description="The value of the cursor parameter for the next page")
 
 
 class V1UsersUserIdConnectorsGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[Data17] = None
 
 
 class V1DbtModelsModelIdGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[DbtModelResponse] = None
 
 
 class ConnectorResponseV1(BaseModel):
+    """ """
+
     id: Optional[str] = Field(
         None,
         description="The unique identifier for the connector within the Fivetran system",
     )
     service: Optional[str] = Field(None, description="The connector type name within the Fivetran system")
     schema_: Optional[str] = Field(
         None,
@@ -9990,36 +11836,42 @@
         None,
         description="The connector schedule configuration type. Supported values: auto, manual",
     )
     connect_card_config: Optional[ConnectCardConfig] = None
 
 
 class SchemaUpdateRequest(BaseModel):
+    """ """
+
     enabled: Optional[bool] = Field(
         None,
         description="The boolean value specifying whether the sync for the table into the destination is enabled.",
     )
     tables: Optional[Dict[str, TableUpdateRequest]] = Field(
         None,
         description="The set of tables within your database schema config that are synced into the destination",
     )
 
 
 class StandardConfigUpdateRequest(BaseModel):
+    """ """
+
     schemas: Optional[Dict[str, SchemaUpdateRequest]] = Field(
         None,
         description="The set of schemas within your connector schema config that are synced into the destination",
     )
     schema_change_handling: Optional[SchemaChangeHandling] = Field(
         None,
         description="The possible values for the schema_change_handling parameter are as follows: <br /> ALLOW_ALL - all new schemas, tables, and columns which appear in the source after the initial setup are included in syncs <br /> ALLOW_COLUMNS - all new schemas and tables which appear in the source after the initial setup are excluded from syncs, but new columns are included <br /> BLOCK_ALL - all new schemas, tables, and columns which appear in the source after the initial setup are excluded from syncs",
     )
 
 
 class ColumnConfigResponse(BaseModel):
+    """ """
+
     name_in_destination: Optional[str] = Field(
         None,
         description="The schema name within your destination in accordance with Fivetran conventional rules",
     )
     enabled: Optional[bool] = Field(
         None,
         description="The boolean value specifying whether the sync for the table into the destination is enabled.",
@@ -10028,14 +11880,16 @@
         None,
         description="The boolean value specifying whether a column should be hashed",
     )
     enabled_patch_settings: Optional[ColumnEnabledPatchSettings] = None
 
 
 class TableConfigResponse(BaseModel):
+    """ """
+
     sync_mode: Optional[SyncMode1] = Field(
         None,
         description="This field appears in the response if the connector supports switching sync modes for tables",
     )
     name_in_destination: Optional[str] = Field(
         None,
         description="The schema name within your destination in accordance with Fivetran conventional rules",
@@ -10048,783 +11902,1159 @@
         None,
         description="The set of columns within your table schema config that are synced into the destination",
     )
     enabled_patch_settings: Optional[TableEnabledPatchSettings] = None
 
 
 class TableColumnsConfigResponse(BaseModel):
+    """ """
+
     columns: Optional[Dict[str, ColumnConfigResponse]] = Field(
         None,
         description="The set of columns within your table schema config that are synced into the destination",
     )
 
 
 class NewTransformationRequest(BaseModel):
+    """ """
+
     dbt_model_id: Optional[str] = Field(
         None,
         description="The unique identifier for the DBT Model within the Fivetran system.",
     )
     schedule: Optional[TransformationSchedule] = None
     run_tests: Optional[bool] = Field(
         None,
         description="The field indicates whether the tests has been confugured for DBT Transformation.",
     )
 
 
 class ActivecampaignConnectorResponseV1(ConnectorResponseV1, ActivecampaignConfigV1):
+    """ """
+
     pass
 
 
 class AdjustConnectorResponseV1(ConnectorResponseV1, AdjustConfigV1):
+    """ """
+
     pass
 
 
 class AdobeAnalyticsConnectorResponseV1(ConnectorResponseV1, AdobeAnalyticsConfigV1):
+    """ """
+
     pass
 
 
 class AdobeAnalyticsDataFeedConnectorResponseV1(ConnectorResponseV1, AdobeAnalyticsDataFeedConfigV1):
+    """ """
+
     pass
 
 
 class AdpWorkforceNowConnectorResponseV1(ConnectorResponseV1, AdpWorkforceNowConfigV1):
+    """ """
+
     pass
 
 
 class AdrollConnectorResponseV1(ConnectorResponseV1, AdrollConfigV1):
+    """ """
+
     pass
 
 
 class AirtableConnectorResponseV1(ConnectorResponseV1, AirtableConfigV1):
+    """ """
+
     pass
 
 
 class AmazonAdsConnectorResponseV1(ConnectorResponseV1, AmazonAdsConfigV1):
+    """ """
+
     pass
 
 
 class AmplitudeConnectorResponseV1(ConnectorResponseV1, AmplitudeConfigV1):
+    """ """
+
     pass
 
 
 class AnaplanConnectorResponseV1(ConnectorResponseV1, AnaplanConfigV1):
+    """ """
+
     pass
 
 
 class ApacheKafkaConnectorResponseV1(ConnectorResponseV1, ApacheKafkaConfigV1):
+    """ """
+
     pass
 
 
 class AppleSearchAdsConnectorResponseV1(ConnectorResponseV1, AppleSearchAdsConfigV1):
+    """ """
+
     pass
 
 
 class AppsflyerConnectorResponseV1(ConnectorResponseV1, AppsflyerConfigV1):
+    """ """
+
     pass
 
 
 class AsanaConnectorResponseV1(ConnectorResponseV1, AsanaConfigV1):
+    """ """
+
     pass
 
 
 class AuroraConnectorResponseV1(ConnectorResponseV1, AuroraConfigV1):
+    """ """
+
     pass
 
 
 class AuroraPostgresConnectorResponseV1(ConnectorResponseV1, AuroraPostgresConfigV1):
+    """ """
+
     pass
 
 
 class AwsCloudtrailConnectorResponseV1(ConnectorResponseV1, AwsCloudtrailConfigV1):
+    """ """
+
     pass
 
 
 class AwsInventoryConnectorResponseV1(ConnectorResponseV1, AwsInventoryConfigV1):
+    """ """
+
     pass
 
 
 class AwsLambdaConnectorResponseV1(ConnectorResponseV1, AwsLambdaConfigV1):
+    """ """
+
     pass
 
 
 class AwsMskConnectorResponseV1(ConnectorResponseV1, AwsMskConfigV1):
+    """ """
+
     pass
 
 
 class AzureBlobStorageConnectorResponseV1(ConnectorResponseV1, AzureBlobStorageConfigV1):
+    """ """
+
     pass
 
 
 class AzureEventHubConnectorResponseV1(ConnectorResponseV1, AzureEventHubConfigV1):
+    """ """
+
     pass
 
 
 class AzureFunctionConnectorResponseV1(ConnectorResponseV1, AzureFunctionConfigV1):
+    """ """
+
     pass
 
 
 class AzurePostgresConnectorResponseV1(ConnectorResponseV1, AzurePostgresConfigV1):
+    """ """
+
     pass
 
 
 class AzureServiceBusConnectorResponseV1(ConnectorResponseV1, AzureServiceBusConfigV1):
+    """ """
+
     pass
 
 
 class AzureSqlDbConnectorResponseV1(ConnectorResponseV1, AzureSqlDbConfigV1):
+    """ """
+
     pass
 
 
 class AzureSqlManagedDbConnectorResponseV1(ConnectorResponseV1, AzureSqlManagedDbConfigV1):
+    """ """
+
     pass
 
 
 class BingadsConnectorResponseV1(ConnectorResponseV1, BingadsConfigV1):
+    """ """
+
     pass
 
 
 class BoxConnectorResponseV1(ConnectorResponseV1, BoxConfigV1):
+    """ """
+
     pass
 
 
 class BraintreeConnectorResponseV1(ConnectorResponseV1, BraintreeConfigV1):
+    """ """
+
     pass
 
 
 class BraintreeSandboxConnectorResponseV1(ConnectorResponseV1, BraintreeSandboxConfigV1):
+    """ """
+
     pass
 
 
 class BranchConnectorResponseV1(ConnectorResponseV1, BranchConfigV1):
+    """ """
+
     pass
 
 
 class BrazeConnectorResponseV1(ConnectorResponseV1, BrazeConfigV1):
+    """ """
+
     pass
 
 
 class CloudfrontConnectorResponseV1(ConnectorResponseV1, CloudfrontConfigV1):
+    """ """
+
     pass
 
 
 class ConcurConnectorResponseV1(ConnectorResponseV1, ConcurConfigV1):
+    """ """
+
     pass
 
 
 class ConfluentCloudConnectorResponseV1(ConnectorResponseV1, ConfluentCloudConfigV1):
+    """ """
+
     pass
 
 
 class CoupaConnectorResponseV1(ConnectorResponseV1, CoupaConfigV1):
+    """ """
+
     pass
 
 
 class CriteoConnectorResponseV1(ConnectorResponseV1, CriteoConfigV1):
+    """ """
+
     pass
 
 
 class DelightedConnectorResponseV1(ConnectorResponseV1, DelightedConfigV1):
+    """ """
+
     pass
 
 
 class DocumentdbConnectorResponseV1(ConnectorResponseV1, DocumentdbConfigV1):
+    """ """
+
     pass
 
 
 class DoubleClickCampaignManagerConnectorResponseV1(ConnectorResponseV1, DoubleClickCampaignManagerConfigV1):
+    """ """
+
     pass
 
 
 class DoubleClickPublishersConnectorResponseV1(ConnectorResponseV1, DoubleClickPublishersConfigV1):
+    """ """
+
     pass
 
 
 class DriftConnectorResponseV1(ConnectorResponseV1, DriftConfigV1):
+    """ """
+
     pass
 
 
 class DropboxConnectorResponseV1(ConnectorResponseV1, DropboxConfigV1):
+    """ """
+
     pass
 
 
 class Dynamics365ConnectorResponseV1(ConnectorResponseV1, Dynamics365ConfigV1):
+    """ """
+
     pass
 
 
 class Dynamics365FoConnectorResponseV1(ConnectorResponseV1, Dynamics365FoConfigV1):
+    """ """
+
     pass
 
 
 class DynamodbConnectorResponseV1(ConnectorResponseV1, DynamodbConfigV1):
+    """ """
+
     pass
 
 
 class EloquaConnectorResponseV1(ConnectorResponseV1, EloquaConfigV1):
+    """ """
+
     pass
 
 
 class EmailConnectorResponseV1(ConnectorResponseV1, EmailConfigV1):
+    """ """
+
     pass
 
 
 class FacebookConnectorResponseV1(ConnectorResponseV1, FacebookConfigV1):
+    """ """
+
     pass
 
 
 class FacebookAdAccountConnectorResponseV1(ConnectorResponseV1, FacebookAdAccountConfigV1):
+    """ """
+
     pass
 
 
 class FacebookAdsConnectorResponseV1(ConnectorResponseV1, FacebookAdsConfigV1):
+    """ """
+
     pass
 
 
 class FacebookPagesConnectorResponseV1(ConnectorResponseV1, FacebookPagesConfigV1):
+    """ """
+
     pass
 
 
 class FinancialForceConnectorResponseV1(ConnectorResponseV1, FinancialForceConfigV1):
+    """ """
+
     pass
 
 
 class FivetranLogConnectorResponseV1(ConnectorResponseV1, FivetranLogConfigV1):
+    """ """
+
     pass
 
 
 class FreshdeskConnectorResponseV1(ConnectorResponseV1, FreshdeskConfigV1):
+    """ """
+
     pass
 
 
 class FrontConnectorResponseV1(ConnectorResponseV1, FrontConfigV1):
+    """ """
+
     pass
 
 
 class FtpConnectorResponseV1(ConnectorResponseV1, FtpConfigV1):
+    """ """
+
     pass
 
 
 class GainsightCustomerSuccessConnectorResponseV1(ConnectorResponseV1, GainsightCustomerSuccessConfigV1):
+    """ """
+
     pass
 
 
 class GcsConnectorResponseV1(ConnectorResponseV1, GcsConfigV1):
+    """ """
+
     pass
 
 
 class GithubConnectorResponseV1(ConnectorResponseV1, GithubConfigV1):
+    """ """
+
     pass
 
 
 class GoogleAdsConnectorResponseV1(ConnectorResponseV1, GoogleAdsConfigV1):
+    """ """
+
     pass
 
 
 class GoogleAnalyticsConnectorResponseV1(ConnectorResponseV1, GoogleAnalyticsConfigV1):
+    """ """
+
     pass
 
 
 class GoogleAnalytics360ConnectorResponseV1(ConnectorResponseV1, GoogleAnalytics360ConfigV1):
+    """ """
+
     pass
 
 
 class GoogleAnalytics4ConnectorResponseV1(ConnectorResponseV1, GoogleAnalytics4ConfigV1):
+    """ """
+
     pass
 
 
 class GoogleAnalytics4ExportConnectorResponseV1(ConnectorResponseV1, GoogleAnalytics4ExportConfigV1):
+    """ """
+
     pass
 
 
 class GoogleAnalyticsMcfConnectorResponseV1(ConnectorResponseV1, GoogleAnalyticsMcfConfigV1):
+    """ """
+
     pass
 
 
 class GoogleCloudFunctionConnectorResponseV1(ConnectorResponseV1, GoogleCloudFunctionConfigV1):
+    """ """
+
     pass
 
 
 class GoogleCloudMysqlConnectorResponseV1(ConnectorResponseV1, GoogleCloudMysqlConfigV1):
+    """ """
+
     pass
 
 
 class GoogleCloudPostgresqlConnectorResponseV1(ConnectorResponseV1, GoogleCloudPostgresqlConfigV1):
+    """ """
+
     pass
 
 
 class GoogleCloudSqlserverConnectorResponseV1(ConnectorResponseV1, GoogleCloudSqlserverConfigV1):
+    """ """
+
     pass
 
 
 class GoogleDisplayAndVideo360ConnectorResponseV1(ConnectorResponseV1, GoogleDisplayAndVideo360ConfigV1):
+    """ """
+
     pass
 
 
 class GoogleDriveConnectorResponseV1(ConnectorResponseV1, GoogleDriveConfigV1):
+    """ """
+
     pass
 
 
 class GooglePlayConnectorResponseV1(ConnectorResponseV1, GooglePlayConfigV1):
+    """ """
+
     pass
 
 
 class GoogleSearchConsoleConnectorResponseV1(ConnectorResponseV1, GoogleSearchConsoleConfigV1):
+    """ """
+
     pass
 
 
 class GoogleSheetsConnectorResponseV1(ConnectorResponseV1, GoogleSheetsConfigV1):
+    """ """
+
     pass
 
 
 class GreenhouseConnectorResponseV1(ConnectorResponseV1, GreenhouseConfigV1):
+    """ """
+
     pass
 
 
 class HeapConnectorResponseV1(ConnectorResponseV1, HeapConfigV1):
+    """ """
+
     pass
 
 
 class HeightConnectorResponseV1(ConnectorResponseV1, HeightConfigV1):
+    """ """
+
     pass
 
 
 class HelpscoutConnectorResponseV1(ConnectorResponseV1, HelpscoutConfigV1):
+    """ """
+
     pass
 
 
 class HerokuKafkaConnectorResponseV1(ConnectorResponseV1, HerokuKafkaConfigV1):
+    """ """
+
     pass
 
 
 class HerokuPostgresConnectorResponseV1(ConnectorResponseV1, HerokuPostgresConfigV1):
+    """ """
+
     pass
 
 
 class HubspotConnectorResponseV1(ConnectorResponseV1, HubspotConfigV1):
+    """ """
+
     pass
 
 
 class InstagramBusinessConnectorResponseV1(ConnectorResponseV1, InstagramBusinessConfigV1):
+    """ """
+
     pass
 
 
 class IntercomConnectorResponseV1(ConnectorResponseV1, IntercomConfigV1):
+    """ """
+
     pass
 
 
 class IterableConnectorResponseV1(ConnectorResponseV1, IterableConfigV1):
+    """ """
+
     pass
 
 
 class ItunesConnectConnectorResponseV1(ConnectorResponseV1, ItunesConnectConfigV1):
+    """ """
+
     pass
 
 
 class JiraConnectorResponseV1(ConnectorResponseV1, JiraConfigV1):
+    """ """
+
     pass
 
 
 class KinesisConnectorResponseV1(ConnectorResponseV1, KinesisConfigV1):
+    """ """
+
     pass
 
 
 class KlaviyoConnectorResponseV1(ConnectorResponseV1, KlaviyoConfigV1):
+    """ """
+
     pass
 
 
 class KustomerConnectorResponseV1(ConnectorResponseV1, KustomerConfigV1):
+    """ """
+
     pass
 
 
 class LeverConnectorResponseV1(ConnectorResponseV1, LeverConfigV1):
+    """ """
+
     pass
 
 
 class LightSpeedRetailConnectorResponseV1(ConnectorResponseV1, LightSpeedRetailConfigV1):
+    """ """
+
     pass
 
 
 class LinkedinAdsConnectorResponseV1(ConnectorResponseV1, LinkedinAdsConfigV1):
+    """ """
+
     pass
 
 
 class LinkedinCompanyPagesConnectorResponseV1(ConnectorResponseV1, LinkedinCompanyPagesConfigV1):
+    """ """
+
     pass
 
 
 class MagentoMysqlConnectorResponseV1(ConnectorResponseV1, MagentoMysqlConfigV1):
+    """ """
+
     pass
 
 
 class MagentoMysqlRdsConnectorResponseV1(ConnectorResponseV1, MagentoMysqlRdsConfigV1):
+    """ """
+
     pass
 
 
 class MailchimpConnectorResponseV1(ConnectorResponseV1, MailchimpConfigV1):
+    """ """
+
     pass
 
 
 class MandrillConnectorResponseV1(ConnectorResponseV1, MandrillConfigV1):
+    """ """
+
     pass
 
 
 class MariaConnectorResponseV1(ConnectorResponseV1, MariaConfigV1):
+    """ """
+
     pass
 
 
 class MariaAzureConnectorResponseV1(ConnectorResponseV1, MariaAzureConfigV1):
+    """ """
+
     pass
 
 
 class MariaRdsConnectorResponseV1(ConnectorResponseV1, MariaRdsConfigV1):
+    """ """
+
     pass
 
 
 class MarinConnectorResponseV1(ConnectorResponseV1, MarinConfigV1):
+    """ """
+
     pass
 
 
 class MarketoConnectorResponseV1(ConnectorResponseV1, MarketoConfigV1):
+    """ """
+
     pass
 
 
 class MavenlinkConnectorResponseV1(ConnectorResponseV1, MavenlinkConfigV1):
+    """ """
+
     pass
 
 
 class MedalliaConnectorResponseV1(ConnectorResponseV1, MedalliaConfigV1):
+    """ """
+
     pass
 
 
 class MicrosoftListsConnectorResponseV1(ConnectorResponseV1, MicrosoftListsConfigV1):
+    """ """
+
     pass
 
 
 class MixpanelConnectorResponseV1(ConnectorResponseV1, MixpanelConfigV1):
+    """ """
+
     pass
 
 
 class MongoConnectorResponseV1(ConnectorResponseV1, MongoConfigV1):
+    """ """
+
     pass
 
 
 class MongoShardedConnectorResponseV1(ConnectorResponseV1, MongoShardedConfigV1):
+    """ """
+
     pass
 
 
 class MysqlConnectorResponseV1(ConnectorResponseV1, MysqlConfigV1):
+    """ """
+
     pass
 
 
 class MysqlAzureConnectorResponseV1(ConnectorResponseV1, MysqlAzureConfigV1):
+    """ """
+
     pass
 
 
 class MysqlRdsConnectorResponseV1(ConnectorResponseV1, MysqlRdsConfigV1):
+    """ """
+
     pass
 
 
 class NetsuiteSuiteanalyticsConnectorResponseV1(ConnectorResponseV1, NetsuiteSuiteanalyticsConfigV1):
+    """ """
+
     pass
 
 
 class OneDriveConnectorResponseV1(ConnectorResponseV1, OneDriveConfigV1):
+    """ """
+
     pass
 
 
 class OptimizelyConnectorResponseV1(ConnectorResponseV1, OptimizelyConfigV1):
+    """ """
+
     pass
 
 
 class OracleConnectorResponseV1(ConnectorResponseV1, OracleConfigV1):
+    """ """
+
     pass
 
 
 class OracleEbsConnectorResponseV1(ConnectorResponseV1, OracleEbsConfigV1):
+    """ """
+
     pass
 
 
 class OracleHvaConnectorResponseV1(ConnectorResponseV1, OracleHvaConfigV1):
+    """ """
+
     pass
 
 
 class OracleRacConnectorResponseV1(ConnectorResponseV1, OracleRacConfigV1):
+    """ """
+
     pass
 
 
 class OracleRdsConnectorResponseV1(ConnectorResponseV1, OracleRdsConfigV1):
+    """ """
+
     pass
 
 
 class OutbrainConnectorResponseV1(ConnectorResponseV1, OutbrainConfigV1):
+    """ """
+
     pass
 
 
 class OutreachConnectorResponseV1(ConnectorResponseV1, OutreachConfigV1):
+    """ """
+
     pass
 
 
 class PardotConnectorResponseV1(ConnectorResponseV1, PardotConfigV1):
+    """ """
+
     pass
 
 
 class PaypalConnectorResponseV1(ConnectorResponseV1, PaypalConfigV1):
+    """ """
+
     pass
 
 
 class PaypalSandboxConnectorResponseV1(ConnectorResponseV1, PaypalSandboxConfigV1):
+    """ """
+
     pass
 
 
 class PendoConnectorResponseV1(ConnectorResponseV1, PendoConfigV1):
+    """ """
+
     pass
 
 
 class PinterestAdsConnectorResponseV1(ConnectorResponseV1, PinterestAdsConfigV1):
+    """ """
+
     pass
 
 
 class PipedriveConnectorResponseV1(ConnectorResponseV1, PipedriveConfigV1):
+    """ """
+
     pass
 
 
 class PostgresConnectorResponseV1(ConnectorResponseV1, PostgresConfigV1):
+    """ """
+
     pass
 
 
 class PostgresRdsConnectorResponseV1(ConnectorResponseV1, PostgresRdsConfigV1):
+    """ """
+
     pass
 
 
 class QualtricsConnectorResponseV1(ConnectorResponseV1, QualtricsConfigV1):
+    """ """
+
     pass
 
 
 class QuickbooksConnectorResponseV1(ConnectorResponseV1, QuickbooksConfigV1):
+    """ """
+
     pass
 
 
 class RechargeConnectorResponseV1(ConnectorResponseV1, RechargeConfigV1):
+    """ """
+
     pass
 
 
 class RecurlyConnectorResponseV1(ConnectorResponseV1, RecurlyConfigV1):
+    """ """
+
     pass
 
 
 class RedditAdsConnectorResponseV1(ConnectorResponseV1, RedditAdsConfigV1):
+    """ """
+
     pass
 
 
 class S3ConnectorResponseV1(ConnectorResponseV1, S3ConfigV1):
+    """ """
+
     pass
 
 
 class SageIntacctConnectorResponseV1(ConnectorResponseV1, SageIntacctConfigV1):
+    """ """
+
     pass
 
 
 class SailthruConnectorResponseV1(ConnectorResponseV1, SailthruConfigV1):
+    """ """
+
     pass
 
 
 class SalesforceConnectorResponseV1(ConnectorResponseV1, SalesforceConfigV1):
+    """ """
+
     pass
 
 
 class SalesforceMarketingCloudConnectorResponseV1(ConnectorResponseV1, SalesforceMarketingCloudConfigV1):
+    """ """
+
     pass
 
 
 class SalesforceSandboxConnectorResponseV1(ConnectorResponseV1, SalesforceSandboxConfigV1):
+    """ """
+
     pass
 
 
 class SapBusinessByDesignConnectorResponseV1(ConnectorResponseV1, SapBusinessByDesignConfigV1):
+    """ """
+
     pass
 
 
 class SegmentConnectorResponseV1(ConnectorResponseV1, SegmentConfigV1):
+    """ """
+
     pass
 
 
 class SendgridConnectorResponseV1(ConnectorResponseV1, SendgridConfigV1):
+    """ """
+
     pass
 
 
 class ServicenowConnectorResponseV1(ConnectorResponseV1, ServicenowConfigV1):
+    """ """
+
     pass
 
 
 class SftpConnectorResponseV1(ConnectorResponseV1, SftpConfigV1):
+    """ """
+
     pass
 
 
 class SharePointConnectorResponseV1(ConnectorResponseV1, SharePointConfigV1):
+    """ """
+
     pass
 
 
 class ShopifyConnectorResponseV1(ConnectorResponseV1, ShopifyConfigV1):
+    """ """
+
     pass
 
 
 class SnapchatAdsConnectorResponseV1(ConnectorResponseV1, SnapchatAdsConfigV1):
+    """ """
+
     pass
 
 
 class SnowplowConnectorResponseV1(ConnectorResponseV1, SnowplowConfigV1):
+    """ """
+
     pass
 
 
 class SplunkConnectorResponseV1(ConnectorResponseV1, SplunkConfigV1):
+    """ """
+
     pass
 
 
 class SqlServerConnectorResponseV1(ConnectorResponseV1, SqlServerConfigV1):
+    """ """
+
     pass
 
 
 class SqlServerHvaConnectorResponseV1(ConnectorResponseV1, SqlServerHvaConfigV1):
+    """ """
+
     pass
 
 
 class SqlServerRdsConnectorResponseV1(ConnectorResponseV1, SqlServerRdsConfigV1):
+    """ """
+
     pass
 
 
 class SquareConnectorResponseV1(ConnectorResponseV1, SquareConfigV1):
+    """ """
+
     pass
 
 
 class StripeConnectorResponseV1(ConnectorResponseV1, StripeConfigV1):
+    """ """
+
     pass
 
 
 class StripeTestConnectorResponseV1(ConnectorResponseV1, StripeTestConfigV1):
+    """ """
+
     pass
 
 
 class SurveyMonkeyConnectorResponseV1(ConnectorResponseV1, SurveyMonkeyConfigV1):
+    """ """
+
     pass
 
 
 class TaboolaConnectorResponseV1(ConnectorResponseV1, TaboolaConfigV1):
+    """ """
+
     pass
 
 
 class TiktokAdsConnectorResponseV1(ConnectorResponseV1, TiktokAdsConfigV1):
+    """ """
+
     pass
 
 
 class TwilioConnectorResponseV1(ConnectorResponseV1, TwilioConfigV1):
+    """ """
+
     pass
 
 
 class TwitterConnectorResponseV1(ConnectorResponseV1, TwitterConfigV1):
+    """ """
+
     pass
 
 
 class TwitterAdsConnectorResponseV1(ConnectorResponseV1, TwitterAdsConfigV1):
+    """ """
+
     pass
 
 
 class TypeformConnectorResponseV1(ConnectorResponseV1, TypeformConfigV1):
+    """ """
+
     pass
 
 
 class UservoiceConnectorResponseV1(ConnectorResponseV1, UservoiceConfigV1):
+    """ """
+
     pass
 
 
 class WebhooksConnectorResponseV1(ConnectorResponseV1, WebhooksConfigV1):
+    """ """
+
     pass
 
 
 class WoocommerceConnectorResponseV1(ConnectorResponseV1, WoocommerceConfigV1):
+    """ """
+
     pass
 
 
 class WorkdayConnectorResponseV1(ConnectorResponseV1, WorkdayConfigV1):
+    """ """
+
     pass
 
 
 class WorkdayHcmConnectorResponseV1(ConnectorResponseV1, WorkdayHcmConfigV1):
+    """ """
+
     pass
 
 
 class XeroConnectorResponseV1(ConnectorResponseV1, XeroConfigV1):
+    """ """
+
     pass
 
 
 class YahooGeminiConnectorResponseV1(ConnectorResponseV1, YahooGeminiConfigV1):
+    """ """
+
     pass
 
 
 class YoutubeAnalyticsConnectorResponseV1(ConnectorResponseV1, YoutubeAnalyticsConfigV1):
+    """ """
+
     pass
 
 
 class ZendeskConnectorResponseV1(ConnectorResponseV1, ZendeskConfigV1):
+    """ """
+
     pass
 
 
 class ZendeskChatConnectorResponseV1(ConnectorResponseV1, ZendeskChatConfigV1):
+    """ """
+
     pass
 
 
 class ZendeskSellConnectorResponseV1(ConnectorResponseV1, ZendeskSellConfigV1):
+    """ """
+
     pass
 
 
 class ZendeskSunshineConnectorResponseV1(ConnectorResponseV1, ZendeskSunshineConfigV1):
+    """ """
+
     pass
 
 
 class ZohoCrmConnectorResponseV1(ConnectorResponseV1, ZohoCrmConfigV1):
+    """ """
+
     pass
 
 
 class ZuoraConnectorResponseV1(ConnectorResponseV1, ZuoraConfigV1):
+    """ """
+
     pass
 
 
 class ZuoraSandboxConnectorResponseV1(ConnectorResponseV1, ZuoraSandboxConfigV1):
+    """ """
+
     pass
 
 
 class V1ConnectorsConnectorIdTestPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[ConnectorResponseV1] = None
 
 
 class V1ConnectorsConnectorIdSchemasSchemaTablesTableColumnsGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[TableColumnsConfigResponse] = None
 
 
 class V1ConnectorsConnectorIdGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[ConnectorResponseV1] = None
 
 
 class V1ConnectorsConnectorIdPatchResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[ConnectorResponseV1] = None
 
 
 class V1ConnectorsPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[ConnectorResponseV1] = None
 
 
 class SchemaConfigResponse(BaseModel):
+    """ """
+
     name_in_destination: Optional[str] = Field(
         None,
         description="The schema name within your destination in accordance with Fivetran conventional rules",
     )
     enabled: Optional[bool] = Field(
         None,
         description="The boolean value specifying whether the sync for the table into the destination is enabled.",
@@ -10832,14 +13062,16 @@
     tables: Optional[Dict[str, TableConfigResponse]] = Field(
         None,
         description="The set of tables within your database schema config that are synced into the destination",
     )
 
 
 class StandardConfigResponse(BaseModel):
+    """ """
+
     enable_new_by_default: Optional[bool] = Field(
         None,
         description="The boolean value specifying whether to enable new schemas, tables, and columns by default",
     )
     schemas: Optional[Dict[str, SchemaConfigResponse]] = Field(
         None,
         description="The set of schemas within your connector schema config that are synced into the destination",
@@ -10847,40 +13079,52 @@
     schema_change_handling: Optional[SchemaChangeHandling1] = Field(
         None,
         description="The possible values for the schema_change_handling parameter are as follows: <br /> ALLOW_ALL - all new schemas, tables, and columns which appear in the source after the initial setup are included in syncs <br /> ALLOW_COLUMNS - all new schemas and tables which appear in the source after the initial setup are excluded from syncs, but new columns are included <br /> BLOCK_ALL - all new schemas, tables, and columns which appear in the source after the initial setup are excluded from syncs",
     )
 
 
 class V1ConnectorsConnectorIdSchemasSchemaNameTablesTableNameColumnsColumnNamePatchResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[StandardConfigResponse] = None
 
 
 class V1ConnectorsConnectorIdSchemasGetResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[StandardConfigResponse] = None
 
 
 class V1ConnectorsConnectorIdSchemasPatchResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[StandardConfigResponse] = None
 
 
 class V1ConnectorsConnectorIdSchemasSchemaNamePatchResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[StandardConfigResponse] = None
 
 
 class V1ConnectorsConnectorIdSchemasReloadPostResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[StandardConfigResponse] = None
 
 
 class V1ConnectorsConnectorIdSchemasSchemaNameTablesTableNamePatchResponse(BaseModel):
+    """ """
+
     code: Optional[str] = Field(None, description="Response status code")
     message: Optional[str] = Field(None, description="Response status text")
     data: Optional[StandardConfigResponse] = None
```

### Comparing `grai_source_fivetran-0.0.8/src/grai_source_fivetran/mock_tools.py` & `grai_source_fivetran-0.0.9/src/grai_source_fivetran/mock_tools.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,52 +11,99 @@
 if has_faker:
     from faker import Faker
 
     fake = Faker()
 
 
 def faker_dep_wrapper(fn: Callable[..., T]):
+    """
+
+    Args:
+        fn (Callable[..., T]):
+
+    Returns:
+
+    Raises:
+
+    """
+
     @wraps(fn)
     def inner(*args, **kwargs) -> T:
+        """
+
+        Args:
+            *args:
+            **kwargs:
+
+        Returns:
+
+        Raises:
+
+        """
         if not has_faker:
             raise ModuleNotFoundError("Mock testing tools require `faker`. Try running `pip install faker`")
         return fn(*args, **kwargs)
 
     return inner
 
 
 class MockFivetranObjects:
+    """ """
+
     @staticmethod
     @faker_dep_wrapper
     def mock_column():
+        """ """
         return Column(
             name=fake.name(),
             namespace=fake.color_name(),
             table_name=fake.name(),
             table_schema=fake.emoji(),
             is_primary_key=fake.boolean(),
             is_foreign_key=fake.boolean(),
             fivetran_id=fake.uuid4(),
             fivetran_table_id=fake.uuid4(),
         )
 
     @staticmethod
     @faker_dep_wrapper
     def mock_table():
+        """ """
         return Table(
             name=fake.name(),
             namespace=fake.color_name(),
             schema_name=fake.emoji(),
             fivetran_id=fake.uuid4(),
         )
 
     @classmethod
     @faker_dep_wrapper
     def mock_edge(cls, type: str = "cc"):
+        """
+
+        Args:
+            type (str, optional):  (Default value = "cc")
+
+        Returns:
+
+        Raises:
+
+        """
+
         def mock_node(type: str):
+            """
+
+            Args:
+                type (str):
+
+            Returns:
+
+            Raises:
+
+            """
             if type == "c":
                 return cls.mock_column()
             elif type == "t":
                 return cls.mock_table()
 
         source = mock_node(type[0])
         destination = mock_node(type[1])
```

### Comparing `grai_source_fivetran-0.0.8/src/grai_source_fivetran/models.py` & `grai_source_fivetran-0.0.9/src/grai_source_fivetran/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,120 +7,160 @@
     ColumnMetadataResponse,
     SchemaMetadataResponse,
     TableMetadataResponse,
 )
 
 
 class TableResult(BaseModel):
+    """ """
+
     id: str
     name_in_source: str
     parent_id: str
     name_in_destination: str
 
 
 class ColumnResult(BaseModel):
+    """ """
+
     id: str
     name_in_source: str
     type_in_source: str
     is_foreign_key: bool
     is_primary_key: bool
     name_in_destination: str
     type_in_destination: str
     parent_id: str
 
 
 class SchemaResult(BaseModel):
+    """ """
+
     id: str
     name_in_source: str
     name_in_destination: str
 
 
 class DestinationConfig(BaseModel):
+    """ """
+
     host: str
     port: int
     database: str
     auth: str
     user: str
     password: str
 
 
 class DestinationMetadata(BaseModel):
+    """ """
+
     id: str  # e.x. decent_dropsy
     group_id: str  # e.x. decent_dropsy
     service: str  # e.x. snowflake
     region: str  # e.x. GCP_US_EAST4
     time_zone_offset: int  # e.x. -5
     setup_status: str  # e.x. connected
     config: DestinationConfig
 
 
 class ConnectorTablePatchSettings(BaseModel):
+    """ """
+
     allowed: bool
     reason: str
     reason_code: str
 
 
 class ConnectorTableColumnSchema(BaseModel):
+    """ """
+
     name_in_destination: str
     enabled: bool
     hashed: bool
     enabled_patch_settings: ConnectorTablePatchSettings
 
 
 class ConnectorTableSchema(BaseModel):
+    """ """
+
     sync_mode: str
     name_in_destination: str
     enabled: bool
     enabled_patch_settings: ConnectorTablePatchSettings
     columns: Dict[str, ConnectorTableColumnSchema]
 
 
 class ConnectorSchema(BaseModel):
+    """ """
+
     name_in_destination: str
     enabled: bool
     tables: Dict[str, ConnectorTableSchema]
 
 
 class ConnectorMetadata(BaseModel):
+    """ """
+
     enable_new_by_default: bool
     schema_change_handling: str
     schemas: Dict[str, ConnectorSchema]
 
 
 class SourceTableColumnMetadata(BaseModel):
+    """ """
+
     columns: Dict[str, ConnectorTableColumnSchema]
 
 
 class NamespaceIdentifier(BaseModel):
+    """ """
+
     source: str
     destination: str
 
 
 class Column(BaseModel):
+    """ """
+
     name: str
     namespace: str
     fivetran_id: str
     fivetran_table_id: str
     table_name: str
     table_schema: str
     is_primary_key: bool
     is_foreign_key: bool
 
     @property
     def full_name(self):
+        """ """
         return f"{self.table_schema}.{self.table_name}.{self.name}"
 
     @classmethod
     def from_fivetran_models(
         cls,
         schema: SchemaMetadataResponse,
         table: TableMetadataResponse,
         column: ColumnMetadataResponse,
         namespace: NamespaceIdentifier,
     ):
+        """
+
+        Args:
+            schema (SchemaMetadataResponse):
+            table (TableMetadataResponse):
+            column (ColumnMetadataResponse):
+            namespace (NamespaceIdentifier):
+
+        Returns:
+
+        Raises:
+
+        """
         source_values = {
             "name": column.name_in_source,
             "fivetran_id": column.id,
             "fivetran_table_id": column.parent_id,
             "is_primary_key": column.is_primary_key,
             "is_foreign_key": column.is_foreign_key,
             "table_name": table.name_in_source,
@@ -137,30 +177,45 @@
             "table_schema": schema.name_in_destination,
             "namespace": namespace.destination,
         }
         return cls(**source_values), cls(**destination_values)
 
 
 class Table(BaseModel):
+    """ """
+
     name: str
     namespace: str
     fivetran_id: str
     schema_name: str
 
     @property
     def full_name(self):
+        """ """
         return f"{self.schema_name}.{self.name}"
 
     @classmethod
     def from_fivetran_models(
         cls,
         schema: SchemaMetadataResponse,
         table: TableMetadataResponse,
         namespace: NamespaceIdentifier,
     ):
+        """
+
+        Args:
+            schema (SchemaMetadataResponse):
+            table (TableMetadataResponse):
+            namespace (NamespaceIdentifier):
+
+        Returns:
+
+        Raises:
+
+        """
         source_values = {
             "name": table.name_in_source,
             "schema_name": schema.name_in_source,
             "fivetran_id": table.id,
             "namespace": namespace.source,
         }
         destination_values = {
@@ -169,22 +224,26 @@
             "fivetran_id": table.id,
             "namespace": namespace.destination,
         }
         return cls(**source_values), cls(**destination_values)
 
 
 class Constraint(str, Enum):
+    """ """
+
     belongs_to = "bt"
     copy = "c"
 
 
 NodeTypes = Union[Column, Table]
 
 
 class Edge(BaseModel):
+    """ """
+
     source: NodeTypes
     destination: NodeTypes
     definition: Optional[str]
     constraint_type: Constraint
     metadata: Optional[Dict] = None
 
     def __hash__(self):
```

### Comparing `grai_source_fivetran-0.0.8/PKG-INFO` & `grai_source_fivetran-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: grai-source-fivetran
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.9.13,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fivetran (>=0.7.0,<0.8.0)
-Requires-Dist: grai-client (>=0.2.0,<0.3.0)
-Requires-Dist: grai-schemas (>=0.1.12,<0.2.0)
+Requires-Dist: grai-client (>=0.2.18,<0.3.0)
+Requires-Dist: grai-schemas (>=0.1.15,<0.2.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-fivetran
 Description-Content-Type: text/markdown
```

