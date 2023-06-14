# Comparing `tmp/graphkb-1.8.0.tar.gz` & `tmp/graphkb-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphkb-1.8.0.tar", last modified: Wed Nov  2 21:06:17 2022, max compression
+gzip compressed data, was "graphkb-1.9.0.tar", last modified: Wed Feb 22 22:39:15 2023, max compression
```

## Comparing `graphkb-1.8.0.tar` & `graphkb-1.9.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 21:06:17.661580 graphkb-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-11-02 21:05:51.000000 graphkb-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-11-02 21:05:51.000000 graphkb-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2259 2022-11-02 21:06:17.661580 graphkb-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1890 2022-11-02 21:05:51.000000 graphkb-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 21:06:17.661580 graphkb-1.8.0/graphkb/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-11-02 21:05:51.000000 graphkb-1.8.0/graphkb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3385 2022-11-02 21:05:51.000000 graphkb-1.8.0/graphkb/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     5040 2022-11-02 21:05:51.000000 graphkb-1.8.0/graphkb/genes.py
--rw-r--r--   0 runner    (1001) docker     (121)    18107 2022-11-02 21:05:51.000000 graphkb-1.8.0/graphkb/match.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 21:05:51.000000 graphkb-1.8.0/graphkb/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-11-02 21:05:51.000000 graphkb-1.8.0/graphkb/statement.py
--rw-r--r--   0 runner    (1001) docker     (121)     2037 2022-11-02 21:05:51.000000 graphkb-1.8.0/graphkb/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     8691 2022-11-02 21:05:51.000000 graphkb-1.8.0/graphkb/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     6535 2022-11-02 21:05:51.000000 graphkb-1.8.0/graphkb/vocab.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 21:06:17.661580 graphkb-1.8.0/graphkb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2259 2022-11-02 21:06:17.000000 graphkb-1.8.0/graphkb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-11-02 21:06:17.000000 graphkb-1.8.0/graphkb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-11-02 21:06:17.000000 graphkb-1.8.0/graphkb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-11-02 21:06:17.000000 graphkb-1.8.0/graphkb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-02 21:06:17.000000 graphkb-1.8.0/graphkb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-02 21:05:51.000000 graphkb-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-11-02 21:06:17.661580 graphkb-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-02 21:05:51.000000 graphkb-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 21:06:17.661580 graphkb-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 21:05:51.000000 graphkb-1.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2022 2022-11-02 21:05:51.000000 graphkb-1.8.0/tests/test_genes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-11-02 21:05:51.000000 graphkb-1.8.0/tests/test_graphkb.py
--rw-r--r--   0 runner    (1001) docker     (121)    16976 2022-11-02 21:05:51.000000 graphkb-1.8.0/tests/test_match.py
--rw-r--r--   0 runner    (1001) docker     (121)     2841 2022-11-02 21:05:51.000000 graphkb-1.8.0/tests/test_statement.py
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-11-02 21:05:51.000000 graphkb-1.8.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     2607 2022-11-02 21:05:51.000000 graphkb-1.8.0/tests/test_vocab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 22:39:15.724264 graphkb-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-22 22:39:07.000000 graphkb-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-22 22:39:07.000000 graphkb-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-02-22 22:39:15.724264 graphkb-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-02-22 22:39:07.000000 graphkb-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 22:39:15.724264 graphkb-1.9.0/graphkb/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-22 22:39:07.000000 graphkb-1.9.0/graphkb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-02-22 22:39:07.000000 graphkb-1.9.0/graphkb/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-02-22 22:39:07.000000 graphkb-1.9.0/graphkb/genes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18414 2023-02-22 22:39:07.000000 graphkb-1.9.0/graphkb/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 22:39:07.000000 graphkb-1.9.0/graphkb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-02-22 22:39:07.000000 graphkb-1.9.0/graphkb/statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-02-22 22:39:07.000000 graphkb-1.9.0/graphkb/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11557 2023-02-22 22:39:07.000000 graphkb-1.9.0/graphkb/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-02-22 22:39:07.000000 graphkb-1.9.0/graphkb/vocab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 22:39:15.724264 graphkb-1.9.0/graphkb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-02-22 22:39:15.000000 graphkb-1.9.0/graphkb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-02-22 22:39:15.000000 graphkb-1.9.0/graphkb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-22 22:39:15.000000 graphkb-1.9.0/graphkb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-02-22 22:39:15.000000 graphkb-1.9.0/graphkb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-22 22:39:15.000000 graphkb-1.9.0/graphkb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-22 22:39:07.000000 graphkb-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-02-22 22:39:15.728264 graphkb-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 22:39:07.000000 graphkb-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 22:39:15.724264 graphkb-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 22:39:07.000000 graphkb-1.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-02-22 22:39:07.000000 graphkb-1.9.0/tests/test_genes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-02-22 22:39:07.000000 graphkb-1.9.0/tests/test_graphkb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18815 2023-02-22 22:39:07.000000 graphkb-1.9.0/tests/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-02-22 22:39:07.000000 graphkb-1.9.0/tests/test_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-02-22 22:39:07.000000 graphkb-1.9.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-02-22 22:39:07.000000 graphkb-1.9.0/tests/test_vocab.py
```

### Comparing `graphkb-1.8.0/LICENSE` & `graphkb-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graphkb-1.8.0/PKG-INFO` & `graphkb-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphkb
-Version: 1.8.0
+Version: 1.9.0
 Summary: python adapter for interacting with the GraphKB API
 Home-page: https://github.com/bcgsc/pori_graphkb_python
 Author-email: graphkb@bcgsc.ca
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: deploy
 Provides-Extra: test
```

### Comparing `graphkb-1.8.0/README.md` & `graphkb-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `graphkb-1.8.0/graphkb/constants.py` & `graphkb-1.9.0/graphkb/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import argparse
 
 from .types import CategoryBaseTermMapping
 
 DEFAULT_LIMIT = 1000
-
 GKB_BASE_URL = "https://graphkb-api.bcgsc.ca/api"
 GKB_STAGING_URL = "https://graphkbstaging-api.bcgsc.ca/api"
 GKB_DEV_URL = "https://graphkbdev-api.bcgsc.ca/api"
 DEFAULT_URL = GKB_BASE_URL
 
+PREFERRED_GENE_SOURCE = "#39:5"  # HGNC
 
 BASE_RETURN_PROPERTIES = ['@rid', '@class']
 
 GENERIC_RETURN_PROPERTIES = [
     'name',
     'sourceId',
     'sourceIdVersion',
@@ -57,26 +57,33 @@
     + ['reviewStatus']
 )
 
 
 ONCOKB_SOURCE_NAME = 'oncokb'
 ONCOGENE = 'oncogenic'
 TUMOUR_SUPPRESSIVE = 'tumour suppressive'
-
 FUSION_NAMES = ['structural variant', 'fusion']
+
+PHARMACOGENOMIC_SOURCE_EXCLUDE_LIST = ["cancer genome interpreter", "civic"]
+
 BASE_THERAPEUTIC_TERMS = ['therapeutic efficacy', 'eligibility']
 # the order here is the order these are applied, the first category matched is returned
 RELEVANCE_BASE_TERMS: CategoryBaseTermMapping = [
     ('therapeutic', BASE_THERAPEUTIC_TERMS),
     ('diagnostic', ['diagnostic indicator']),
     ('prognostic', ['prognostic indicator']),
     ('pharmacogenomic', ['metabolism', 'toxicity', 'dosage']),
     ('cancer predisposition', ['pathogenic']),
     ('biological', ['functional effect', 'tumourigenesis', 'predisposing']),
 ]
+FAILED_REVIEW_STATUS = 'failed'
+
+CHROMOSOMES_HG38 = [f"chr{i}" for i in range(1, 23)] + ['chrX', 'chrY', 'chrM']
+CHROMOSOMES_HG19 = [str(i) for i in range(1, 23)] + ['x', 'y', 'mt']
+CHROMOSOMES = CHROMOSOMES_HG38 + CHROMOSOMES_HG19
 
 AMBIGUOUS_AA = ['x', '?', 'X']
 AA_3to1_MAPPING = {
     'Ala': 'A',
     'Arg': 'R',
     'Asn': 'N',
     'Asp': 'D',
```

### Comparing `graphkb-1.8.0/graphkb/match.py` & `graphkb-1.9.0/graphkb/match.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,30 +8,29 @@
     AMBIGUOUS_AA,
     INPUT_COPY_CATEGORIES,
     INPUT_EXPRESSION_CATEGORIES,
     POS_VARIANT_RETURN_PROPERTIES,
     VARIANT_RETURN_PROPERTIES,
 )
 from .types import BasicPosition, Ontology, ParsedVariant, PositionalVariant, Record, Variant
-from .util import FeatureNotFoundError, convert_to_rid_list, looks_like_rid
+from .util import FeatureNotFoundError, convert_to_rid_list, logger, looks_like_rid
 from .vocab import get_term_tree
 
 FEATURES_CACHE: Set[str] = set()
 
 
 def get_equivalent_features(
     conn: GraphKBConnection,
     gene_name: str,
     ignore_cache: bool = False,
     is_source_id: bool = False,
     source: str = '',
     source_id_version: str = '',
 ) -> List[Ontology]:
-    """
-    Match an equivalent list of features given some input feature name (or ID)
+    """Match an equivalent list of features given some input feature name (or ID).
 
     Args:
         gene_name: the gene name to search features by
         ignore_cache (bool, optional): bypass the cache to always force a new request
         is_source_id: treat the gene_name as the gene ID from the source database (ex. ENSG001)
         source_id_version: the version of the source_id
         source: the name of the source database the gene definition is from (ex. ensembl)
@@ -58,22 +57,27 @@
             ),
         )
 
     filters: List[Dict] = []
     if source:
         filters.append({'source': {'target': 'Source', 'filters': {'name': source}}})
 
+    if gene_name.count('.') == 1 and gene_name.split('.')[-1].isnumeric():
+        # eg. ENSG00000133703.11 or NM_033360.4
+        logger.debug(
+            f"Assuming {gene_name} has a .version_format - ignoring the version for equivalent features"
+        )
+        gene_name = gene_name.split('.')[0]
+
     if is_source_id or source_id_version:
         filters.append({'sourceId': gene_name})
-
         if source_id_version:
             filters.append(
                 {'OR': [{'sourceIdVersion': source_id_version}, {'sourceIdVersion': None}]}
             )
-
     elif FEATURES_CACHE and gene_name.lower() not in FEATURES_CACHE and not ignore_cache:
         return []
     else:
         filters.append({'OR': [{'sourceId': gene_name}, {'name': gene_name}]})
 
     return cast(
         List[Ontology],
```

### Comparing `graphkb-1.8.0/graphkb/types.py` & `graphkb-1.9.0/graphkb/types.py`

 * *Files identical despite different names*

### Comparing `graphkb-1.8.0/graphkb/util.py` & `graphkb-1.9.0/graphkb/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import hashlib
 import json
 import logging
 import re
+import time
 from datetime import datetime
 from typing import Any, Dict, Iterable, List, Optional, cast
 
 import requests
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 
@@ -96,15 +97,21 @@
         self,
         url: str = DEFAULT_URL,
         username: str = '',
         password: str = '',
         use_global_cache: bool = True,
     ):
         self.http = requests.Session()
-        retries = Retry(total=3, backoff_factor=1, status_forcelist=[429, 500, 502, 503, 504])
+        retries = Retry(
+            total=100,
+            connect=5,
+            status=5,
+            backoff_factor=5,
+            status_forcelist=[429, 500, 502, 503, 504],
+        )
         self.http.mount("https://", HTTPAdapter(max_retries=retries))
 
         self.token = ''
         self.url = url
         self.username = username
         self.password = password
         self.headers = {'Accept': 'application/json', 'Content-Type': 'application/json'}
@@ -119,38 +126,78 @@
     def load(self) -> Optional[float]:
         if self.first_request and self.last_request:
             return (
                 self.request_count * 1000 / millis_interval(self.first_request, self.last_request)
             )
         return None
 
-    def request(self, endpoint: str, method: str = 'GET', **kwargs) -> Dict:
+    def request(
+        self,
+        endpoint: str,
+        method: str = 'GET',
+        **kwargs,
+    ) -> Dict:
         """Request wrapper to handle adding common headers and logging.
 
         Args:
             endpoint (string): api endpoint, excluding the base uri
             method (str, optional): the http method. Defaults to 'GET'.
 
         Returns:
             dict: the json response as a python dict
         """
         url = join_url(self.url, endpoint)
         self.request_count += 1
+        connect_timeout = 7
+        read_timeout = 61
+
+        # don't want to use a read timeout if the request is not idempotent
+        # otherwise you may wind up making unintended changes
+        timeout = None
+        if endpoint in ['query', 'parse']:
+            timeout = (connect_timeout, read_timeout)
+
         start_time = datetime.now()
+
         if not self.first_request:
             self.first_request = start_time
         self.last_request = start_time
-        resp = requests.request(method, url, headers=self.headers, **kwargs)
 
-        if resp.status_code == 401 or resp.status_code == 403:
-            # try to re-login if the token expired
+        # using a manual retry as well as using the requests Retry() object because
+        # a ConnectionError or OSError might be thrown and we still want to retry in those cases.
+        # about catching OSError as well as ConnectionError:
+        # https://stackoverflow.com/questions/74253820
+        attempts = range(15)
+        for attempt in attempts:
+            if attempt > 0:
+                time.sleep(2)  # wait between retries
+            try:
+                self.refresh_login()
+                self.request_count += 1
+                resp = requests.request(
+                    method,
+                    url,
+                    headers=self.headers,
+                    timeout=timeout,
+                    **kwargs,
+                )
+                if resp.status_code == 401 or resp.status_code == 403:
+                    logger.debug(f'/{endpoint} - {resp.status_code} - retrying')
+                    # try to re-login if the token expired
+                    continue
+                else:
+                    break
+            except (requests.exceptions.ConnectionError, OSError) as err:
+                if attempt < len(attempts) - 1:
+                    logger.debug(f'/{endpoint} - {str(err)} - retrying')
+                    continue
+                raise err
+            except Exception as err2:
+                raise err2
 
-            self.refresh_login()
-            self.request_count += 1
-            resp = requests.request(method, url, headers=self.headers, **kwargs)
         timing = millis_interval(start_time, datetime.now())
         logger.debug(f'/{endpoint} - {resp.status_code} - {timing} ms')  # type: ignore
 
         try:
             resp.raise_for_status()
         except requests.exceptions.HTTPError as err:
             # try to get more error details
@@ -167,23 +214,39 @@
     def post(self, uri: str, data: Dict = {}, **kwargs) -> Dict:
         """Convenience method for making post requests."""
         return self.request(uri, method='POST', data=json.dumps(data), **kwargs)
 
     def login(self, username: str, password: str) -> None:
         self.username = username
         self.password = password
+        connect_timeout = 7
+        read_timeout = 61
 
         # use requests package directly to avoid recursion loop on login failure
-        self.request_count += 1
-        resp = requests.request(
-            url=f'{self.url}/token',
-            method='POST',
-            headers=self.headers,
-            data=json.dumps({'username': username, 'password': password}),
-        )
+        attempts = range(10)
+        for attempt in attempts:
+            if attempt > 0:
+                time.sleep(2)  # wait between retries
+            try:
+                self.request_count += 1
+                resp = requests.request(
+                    url=f'{self.url}/token',
+                    method='POST',
+                    headers=self.headers,
+                    timeout=(connect_timeout, read_timeout),
+                    data=json.dumps({'username': username, 'password': password}),
+                )
+                break
+            except (requests.exceptions.ConnectionError, OSError) as err:
+                if attempt < len(attempts) - 1:
+                    logger.debug(f'/login - {str(err)} - retrying')
+                    continue
+                raise err
+            except Exception as err2:
+                raise err2
         resp.raise_for_status()
         content = resp.json()
         self.token = content['kbToken']
         self.headers['Authorization'] = self.token
 
     def refresh_login(self) -> None:
         self.login(self.username, self.password)
@@ -209,15 +272,18 @@
 
         if not ignore_cache and paginate:
             hash_code = cache_key(request_body)
             if hash_code in self.cache and not force_refresh:
                 return self.cache[hash_code]
 
         while True:
-            content = self.post('query', data={**request_body, 'limit': limit, 'skip': len(result)})
+            content = self.post(
+                'query',
+                data={**request_body, 'limit': limit, 'skip': len(result)},
+            )
             records = content['result']
             result.extend(records)
             if len(records) < limit or not paginate:
                 break
 
         if not ignore_cache and paginate:
             self.cache[hash_code] = result
@@ -244,7 +310,31 @@
         return result[0]
 
     def get_source(self, name: str) -> Record:
         source = self.query({'target': 'Source', 'filters': {'name': name}})
         if len(source) != 1:
             raise AssertionError(f'Unable to unqiuely identify source with name {name}')
         return source[0]
+
+
+def get_rid(conn: GraphKBConnection, target: str, name: str) -> str:
+    """
+    Retrieve a record by name and target
+
+    Args:
+        conn: GraphKBConnection
+        target: record type to query
+        name: the name of the record to retrieve
+
+    Returns:
+        str: @rid of the record
+
+    Raises:
+        AssertionError: if the term was not found or more than 1 match was found (expected to be unique)
+    """
+    result = conn.query(
+        {"target": target, "filters": {"name": name}, "returnProperties": ["@rid"]},
+        ignore_cache=False,
+    )
+    assert len(result) == 1, f"unable to find unique '{target}' ID for '{name}'"
+
+    return result[0]["@rid"]
```

### Comparing `graphkb-1.8.0/graphkb/vocab.py` & `graphkb-1.9.0/graphkb/vocab.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,18 +183,16 @@
         raise AssertionError(f'unable to find term ({name}) by name')
     return cast(Ontology, result[0])
 
 
 def get_terms_set(
     graphkb_conn: GraphKBConnection, base_terms: Iterable[str], ignore_cache: bool = False
 ) -> Set[str]:
-    """
-    Get a set of terms of vocabulary given some base/parent term names. Returns the record
-    IDs for the resulting terms
-    """
+    """Get a set of vocabulary rids given some base/parent term names."""
+    base_terms = [base_terms] if isinstance(base_terms, str) else base_terms
     cache_key = tuple(sorted(base_terms))
     if graphkb_conn.cache.get(cache_key, None) and not ignore_cache:
         return graphkb_conn.cache[cache_key]
     terms = set()
     for base_term in base_terms:
         terms.update(
             convert_to_rid_list(
```

### Comparing `graphkb-1.8.0/graphkb.egg-info/PKG-INFO` & `graphkb-1.9.0/graphkb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphkb
-Version: 1.8.0
+Version: 1.9.0
 Summary: python adapter for interacting with the GraphKB API
 Home-page: https://github.com/bcgsc/pori_graphkb_python
 Author-email: graphkb@bcgsc.ca
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: deploy
 Provides-Extra: test
```

### Comparing `graphkb-1.8.0/graphkb.egg-info/SOURCES.txt` & `graphkb-1.9.0/graphkb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphkb-1.8.0/setup.cfg` & `graphkb-1.9.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 line_length = 100
 multi_line_output = 3
 include_trailing_comma = true
 
 [metadata]
 name = graphkb
 url = https://github.com/bcgsc/pori_graphkb_python
-version = 1.8.0
+version = 1.9.0
 author_email = graphkb@bcgsc.ca
 description = python adapter for interacting with the GraphKB API
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 packages = find:
```

### Comparing `graphkb-1.8.0/tests/test_graphkb.py` & `graphkb-1.9.0/tests/test_graphkb.py`

 * *Files identical despite different names*

### Comparing `graphkb-1.8.0/tests/test_match.py` & `graphkb-1.9.0/tests/test_match.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from unittest.mock import MagicMock
 
 import pytest
 
 from graphkb import GraphKBConnection, match
 from graphkb.util import FeatureNotFoundError
 
+EXCLUDE_INTEGRATION_TESTS = os.environ.get('EXCLUDE_INTEGRATION_TESTS') == '1'
+
 INCREASE_PREFIXES = ['up', 'increase', 'over', 'gain', 'amp']
 DECREASE_PREFIXES = ['down', 'decrease', 'reduce', 'under', 'loss', 'delet']
 GENERAL_MUTATION = 'mutation'
 
 
 def has_prefix(word: str, prefixes: List[str]) -> bool:
     for prefix in prefixes:
@@ -43,14 +45,39 @@
         assert 'NM_033360' in kras
         assert 'ENST00000311936' in kras
 
     def test_expands_generalizations(self, kras):
         assert 'NM_033360.4' in kras
         assert 'ENSG00000133703.11' in kras
 
+    def test_expands_generalizations_kras(self, kras):
+        assert 'NM_033360.4' in kras
+        assert 'NM_033360' in kras
+        assert 'ENSG00000133703.11' in kras
+        assert 'ENSG00000133703' in kras
+
+    @pytest.mark.parametrize(
+        'alt_rep', ('NM_033360.4', 'NM_033360', 'ENSG00000133703.11', 'ENSG00000133703')
+    )
+    def test_expands_generalizations_refseq(self, alt_rep, conn):
+        kras = [f['displayName'] for f in match.get_equivalent_features(conn, alt_rep)]
+        assert 'NM_033360.4' in kras
+        assert 'NM_033360' in kras
+        assert 'ENSG00000133703.11' in kras
+        assert 'ENSG00000133703' in kras
+
+    def test_checks_by_source_id_kras(self, conn):
+        kras = [
+            f['displayName']
+            for f in match.get_equivalent_features(
+                conn, 'nm_033360', source='refseq', source_id_version='4', is_source_id=True
+            )
+        ]
+        assert 'KRAS' in kras
+
 
 class TestMatchCopyVariant:
     def test_bad_category(self, conn):
         with pytest.raises(ValueError):
             match.match_copy_variant(conn, 'kras', 'not a copy number')
 
     def test_bad_gene_name(self, conn):
@@ -100,14 +127,17 @@
         assert GENERAL_MUTATION not in types_selected
         assert match.INPUT_COPY_CATEGORIES.AMP in types_selected
         assert match.INPUT_COPY_CATEGORIES.ANY_LOSS not in types_selected
 
         for variant_type in types_selected:
             assert not has_prefix(variant_type, DECREASE_PREFIXES)
 
+    @pytest.mark.skipif(
+        EXCLUDE_INTEGRATION_TESTS, reason="excluding long running integration tests"
+    )
     def test_low_gain_excludes_amplification(self, conn):
         matches = match.match_copy_variant(conn, 'KRAS', match.INPUT_COPY_CATEGORIES.GAIN)
 
         types_selected = {record['type']['name'] for record in matches}
 
         assert match.INPUT_COPY_CATEGORIES.AMP not in types_selected
         assert match.INPUT_COPY_CATEGORIES.LOSS not in types_selected
@@ -146,14 +176,17 @@
 
     def test_bad_gene_name(self, conn):
         with pytest.raises(FeatureNotFoundError):
             match.match_expression_variant(
                 conn, 'not a real gene name', match.INPUT_EXPRESSION_CATEGORIES.UP
             )
 
+    @pytest.mark.skipif(
+        EXCLUDE_INTEGRATION_TESTS, reason="excluding long running integration tests"
+    )
     def test_known_reduced_expression(self, conn):
         matches = match.match_expression_variant(
             conn, 'PTEN', match.INPUT_EXPRESSION_CATEGORIES.DOWN
         )
         assert matches
 
         types_selected = {record['type']['name'] for record in matches}
@@ -175,14 +208,17 @@
 
         assert match.INPUT_EXPRESSION_CATEGORIES.UP not in types_selected
         assert GENERAL_MUTATION not in types_selected
 
         for variant_type in types_selected:
             assert not has_prefix(variant_type, INCREASE_PREFIXES)
 
+    @pytest.mark.skipif(
+        EXCLUDE_INTEGRATION_TESTS, reason="excluding long running integration tests"
+    )
     def test_known_increased_expression(self, conn):
         matches = match.match_expression_variant(conn, 'CA9', match.INPUT_EXPRESSION_CATEGORIES.UP)
         assert matches
 
         types_selected = {record['type']['name'] for record in matches}
 
         assert match.INPUT_EXPRESSION_CATEGORIES.UP not in types_selected
@@ -336,22 +372,28 @@
             )
 
     def test_match_explicit_reference1(self, conn):
         reference1 = conn.query({'target': 'Feature', 'filters': {'name': 'KRAS'}})[0]['@rid']
         matches = match.match_positional_variant(conn, 'p.G12D', reference1=reference1)
         assert matches
 
+    @pytest.mark.skipif(
+        EXCLUDE_INTEGRATION_TESTS, reason="excluding long running integration tests"
+    )
     def test_match_explicit_references(self, conn):
         reference1 = conn.query({'target': 'Feature', 'filters': {'name': 'BCR'}})[0]['@rid']
         reference2 = conn.query({'target': 'Feature', 'filters': {'name': 'ABL1'}})[0]['@rid']
         matches = match.match_positional_variant(
             conn, 'fusion(e.13,e.3)', reference1=reference1, reference2=reference2
         )
         assert matches
 
+    @pytest.mark.skipif(
+        EXCLUDE_INTEGRATION_TESTS, reason="excluding long running integration tests"
+    )
     @pytest.mark.parametrize(
         'known_variant,related_variants,unrelated_variants',
         [
             ['KRAS:p.G12D', ['KRAS:p.G12X', 'chr12:g.25398284C>T'], ['KRAS:p.G12V']],
             ['KRAS:p.G13D', ['KRAS:p.?13mut'], []],
             ['chr12:g.25398284C>T', ['KRAS:p.G12D'], ['KRAS:p.G12V']],
             ['EGFR:p.E746_S752delinsI', ['EGFR mutation'], ['EGFR copy variant']],
@@ -393,19 +435,25 @@
         novel_specific = 'CDKN2A:p.T18888888888888888888M'
         matches = match.match_positional_variant(conn, novel_specific)
         names = {m['displayName'] for m in matches}
         assert matches
         assert novel_specific not in names
         assert 'CDKN2A mutation' in names
 
+    @pytest.mark.skipif(
+        EXCLUDE_INTEGRATION_TESTS, reason="excluding long running integration tests"
+    )
     def test_genomic_coordinates(self, conn):
         genomic = 'X:g.100611165A>T'
         match.match_positional_variant(conn, genomic)
         # no assert b/c checking for no error rather than the result
 
+    @pytest.mark.skipif(
+        EXCLUDE_INTEGRATION_TESTS, reason="excluding long running integration tests"
+    )
     def test_tert_promoter(self, conn):
         assert match.match_positional_variant(conn, 'TERT:c.-124C>T')
 
     @pytest.mark.skipif(
         True, reason="GERO-303 - technically incorrect notation for GSC backwards compatibility."
     )
     def test_tert_promoter_leading_one_alt_notation(self, conn):
```

### Comparing `graphkb-1.8.0/tests/test_statement.py` & `graphkb-1.9.0/tests/test_statement.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from unittest.mock import Mock
 
+import os
 import pytest
 
 from graphkb import statement
 
+from .test_match import conn
+
+EXCLUDE_INTEGRATION_TESTS = os.environ.get('EXCLUDE_INTEGRATION_TESTS') == '1'
+
 
 @pytest.fixture()
 def graphkb_conn():
     def make_rid_list(*values):
         return [{'@rid': v} for v in values]
 
     def term_tree_calls(*final_values):
@@ -75,7 +80,19 @@
         )
         assert category == ''
 
         category = statement.categorize_relevance(
             graphkb_conn, '1', [('blargh', ['some', 'blargh'])]
         )
         assert category == 'blargh'
+
+
+@pytest.mark.skipif(EXCLUDE_INTEGRATION_TESTS, reason="excluding long running integration tests")
+class TestStatementMatch:
+    def test_truncating_categories(self, conn):
+        variant = {
+            '@class': 'CategoryVariant',
+            '@rid': '#161:429',
+            'displayName': 'RB1 truncating',
+        }
+        statements = statement.get_statements_from_variants(conn, [variant])
+        assert statements
```

### Comparing `graphkb-1.8.0/tests/test_util.py` & `graphkb-1.9.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `graphkb-1.8.0/tests/test_vocab.py` & `graphkb-1.9.0/tests/test_vocab.py`

 * *Files identical despite different names*

