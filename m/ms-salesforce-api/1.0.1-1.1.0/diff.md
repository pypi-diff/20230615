# Comparing `tmp/ms_salesforce_api-1.0.1.tar.gz` & `tmp/ms_salesforce_api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_salesforce_api-1.0.1.tar", max compression
+gzip compressed data, was "ms_salesforce_api-1.1.0.tar", max compression
```

## Comparing `ms_salesforce_api-1.0.1.tar` & `ms_salesforce_api-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35149 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/LICENSE
--rw-r--r--   0        0        0     5631 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/__init__.py
--rw-r--r--   0        0        0     1491 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/Auth.py
--rw-r--r--   0        0        0      982 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/JWTGenerator.py
--rw-r--r--   0        0        0     2713 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
--rw-r--r--   0        0        0        0 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/__tests__/__init__.py
--rw-r--r--   0        0        0     2749 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/__tests__/test_Auth.py
--rw-r--r--   0        0        0     2395 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
--rw-r--r--   0        0        0     5168 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
--rw-r--r--   0        0        0     3347 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/__tests__/__init__.py
--rw-r--r--   0        0        0    15402 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
--rw-r--r--   0        0        0     7675 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/constants.py
--rw-r--r--   0        0        0     3804 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
--rw-r--r--   0        0        0    20445 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
--rw-r--r--   0        0        0     2166 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
--rw-r--r--   0        0        0        0 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/dto/__init__.py
--rw-r--r--   0        0        0    22589 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
--rw-r--r--   0        0        0     8894 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
--rw-r--r--   0        0        0        0 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/export_data/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
--rw-r--r--   0        0        0    17755 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
--rw-r--r--   0        0        0    13717 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
--rw-r--r--   0        0        0      303 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/helpers.py
--rw-r--r--   0        0        0     1055 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6407 1970-01-01 00:00:00.000000 ms_salesforce_api-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/LICENSE
+-rw-r--r--   0        0        0     8325 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/__init__.py
+-rw-r--r--   0        0        0     1491 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/Auth.py
+-rw-r--r--   0        0        0      982 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/JWTGenerator.py
+-rw-r--r--   0        0        0     2713 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/__tests__/__init__.py
+-rw-r--r--   0        0        0     2749 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py
+-rw-r--r--   0        0        0     2205 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
+-rw-r--r--   0        0        0     5168 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
+-rw-r--r--   0        0        0     3338 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/__tests__/__init__.py
+-rw-r--r--   0        0        0    15342 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
+-rw-r--r--   0        0        0     7675 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/constants.py
+-rw-r--r--   0        0        0     3804 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
+-rw-r--r--   0        0        0    20445 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
+-rw-r--r--   0        0        0     2166 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/dto/__init__.py
+-rw-r--r--   0        0        0    23105 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
+-rw-r--r--   0        0        0     9263 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
+-rw-r--r--   0        0        0    17755 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
+-rw-r--r--   0        0        0    13717 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
+-rw-r--r--   0        0        0      303 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/helpers.py
+-rw-r--r--   0        0        0     1055 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9101 1970-01-01 00:00:00.000000 ms_salesforce_api-1.1.0/PKG-INFO
```

### Comparing `ms_salesforce_api-1.0.1/LICENSE` & `ms_salesforce_api-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/Auth.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/JWTGenerator.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/__tests__/test_Auth.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,15 +29,14 @@
             audience,
             session_duration_hours,
         )
 
         token = jwt_generator.generate_token()
         self.assertIsNotNone(token)
 
-        # Verify that the generated token has the correct data
         decoded_payload = jwt.decode(
             token, self.public_key, algorithms="RS256", audience=audience
         )
         self.assertEqual(decoded_payload["iss"], client_id)
         self.assertEqual(decoded_payload["sub"], username)
         self.assertEqual(decoded_payload["aud"], audience)
 
@@ -54,20 +53,18 @@
             audience,
             session_duration_hours,
         )
 
         token = jwt_generator.generate_token()
         self.assertIsNotNone(token)
 
-        # Verify that the generated token has the correct data
         decoded_payload = jwt.decode(
             token, self.public_key, algorithms="RS256", audience=audience
         )
         self.assertEqual(decoded_payload["iss"], client_id)
         self.assertEqual(decoded_payload["sub"], username)
         self.assertEqual(decoded_payload["aud"], audience)
 
-        # Verify that the token has the custom session duration
         token_duration_seconds = int(decoded_payload["exp"]) - int(time.time())
         self.assertAlmostEqual(
             token_duration_seconds, session_duration_hours * 3600, delta=10
         )
```

### Comparing `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/__init__.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     SalesforceQueryExecutor,
 )
 
 logging.basicConfig(
     level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s"
 )
 
-MAX_PROJECT_IDS_PER_QUERY = 50
+MAX_PROJECT_IDS_PER_QUERY = 200
 
 
 class Project(SalesforceQueryExecutor):
     def fetch_billing_lines(self, project_ids):
         billing_lines = []
         query = DEFAULT_PROJECT_BILLING_LINE_QUERY.format(
             project_id="','".join(project_ids)
@@ -36,15 +36,15 @@
         return billing_lines
 
     def get_batches(self, lst, n):
         """Yield successive n-sized chunks from lst."""
         for i in range(0, len(lst), n):
             yield lst[i : i + n]  # noqa: E203
 
-    def get_opportunities(
+    def get_all(
         self,
         last_executed_at: str = None,
         query: str = DEFAULT_PROJECT_OPPORTUNITY_QUERY,
         format: str = "json",
     ):
         try:
             if last_executed_at:
```

### Comparing `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/__tests__/test_Project.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/__tests__/test_Project.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,30 +142,30 @@
 
 
 class TestProject(unittest.TestCase):
     @patch(
         "ms_salesforce_api.salesforce.project.SalesforceQueryExecutor.authenticate"  # noqa: E501
     )
     @patch.object(Project, "fetch_data", side_effect=mock_fetch_data)
-    def test_get_opportunities(self, mock_make_request, mock_authenticate):
+    def test_get_all(self, mock_make_request, mock_authenticate):
         mock_authenticate.return_value = "access_token"
 
         client_id = "client_id"
         username = "username"
         domain = "https://auth.example.com"
         private_key = "private_key"
 
         project = Project(
             client_id,
             username,
             domain,
             private_key,
             audience="https://login.salesforce.com",
         )
-        opportunities = project.get_opportunities(format="dto")
+        opportunities = project.get_all(format="dto")
         self.assertEqual(len(opportunities), 1)
 
         opportunity = opportunities[0]
         self.assertIsInstance(opportunity, OpportunityDTO)
         self.assertEqual(
             opportunity.account_business_name,
             "ESMProjectAcc",
@@ -243,30 +243,30 @@
 
         mock_make_request.assert_called()
 
     @patch(
         "ms_salesforce_api.salesforce.project.SalesforceQueryExecutor.authenticate"  # noqa: E501
     )
     @patch.object(Project, "fetch_data", side_effect=mock_fetch_data)
-    def test_get_opportunities(self, mock_make_request, mock_authenticate):
+    def test_get_all(self, mock_make_request, mock_authenticate):
         mock_authenticate.return_value = "access_token"
 
         client_id = "client_id"
         username = "username"
         domain = "https://auth.example.com"
         private_key = "private_key"
 
         project = Project(
             client_id,
             username,
             domain,
             private_key,
             audience="https://login.salesforce.com",
         )
-        opportunities = project.get_opportunities()
+        opportunities = project.get_all()
         self.assertEqual(len(opportunities), 1)
 
         opportunity = opportunities[0]
         self.assertIsInstance(opportunity, dict)
         self.assertEqual(
             opportunity["account_business_name"],
             "ESMProjectAcc",
@@ -351,15 +351,15 @@
 
     @patch(
         "ms_salesforce_api.salesforce.project.SalesforceQueryExecutor.authenticate"  # noqa: E501
     )
     @patch(
         "ms_salesforce_api.salesforce.project.SalesforceQueryExecutor._make_request"  # noqa: E501
     )
-    def test_get_opportunities_empty_on_failure(
+    def test_get_all_empty_on_failure(
         self, mock_make_request, mock_authenticate
     ):
         mock_authenticate.return_value = "access_token"
         mock_make_request.return_value = None
 
         client_id = "client_id"
         username = "username"
@@ -371,11 +371,11 @@
             username,
             domain,
             private_key,
             audience="https://login.salesforce.com",
         )
         query = "SELECT * FROM Opportunity"
 
-        opportunities = project.get_opportunities(query=query)
+        opportunities = project.get_all(query=query)
         self.assertEqual(opportunities, [])
 
         mock_make_request.assert_called()
```

### Comparing `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/constants.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/constants.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/export_data/Bigquery.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/export_data/Bigquery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 from itertools import islice
 from urllib.parse import quote
 
 from gc_google_services_api.bigquery import BigQueryManager
 
 
 class BigQueryExporter:
+    """
+    Initializes the Bigquery exporter with the given project ID and dataset ID.
+
+    Args:
+        project_id (str): The ID of the Google Cloud project.
+        dataset_id (str): The ID of the BigQuery dataset.
+    """
+
     def __init__(self, project_id, dataset_id):
         self.project_id = project_id
         self.dataset_id = dataset_id
         self.client = BigQueryManager(
             project_id=project_id, dataset_id=dataset_id
         )
         self.batch_size = 200
@@ -606,7 +614,14 @@
             self._export_opportunities(batch)
 
             self._export_billing_lines(batch)
 
             self._export_PLIs(batch)
 
             self._export_accounts(batch)
+
+    def delete_all_rows(self):
+        table_names = self.schemas.keys()
+        for table_name in table_names:
+            delete_query_table = f"DELETE FROM `{self.project_id}.{self.dataset_id}.{table_name}` WHERE true"
+
+            self.client.execute_query(delete_query_table, None)
```

### Comparing `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,25 @@
 
 logging.basicConfig(
     level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s"
 )
 
 
 class CloudSQL:
+    """
+    Connect with a Postgres Database with the given
+    host name, database name, username, and password.
+
+    Args:
+        host (str): The host name for the Postgres database.
+        user (str): The username for accessing the database.
+        password (str): The password for accessing the database.
+        dbname (str): The name of the database.
+    """
+
     BATCH_SIZE = 200
 
     def __init__(self, host, user, password, dbname, debug_mode=False):
         self.debug_mode = debug_mode
 
         self.check_and_create_database(host, user, password, dbname)
```

### Comparing `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.1/pyproject.toml` & `ms_salesforce_api-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-salesforce-api"
-version = "1.0.1"
+version = "1.1.0"
 description = "Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres."
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_salesforce_api"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

