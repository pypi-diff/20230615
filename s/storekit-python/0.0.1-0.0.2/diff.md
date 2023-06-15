# Comparing `tmp/storekit_python-0.0.1.tar.gz` & `tmp/storekit_python-0.0.2.tar.gz`

## Comparing `storekit_python-0.0.1.tar` & `storekit_python-0.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 storekit_python-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 storekit_python-0.0.1/Makefile
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 storekit_python-0.0.1/README_zh.md
--rw-r--r--   0        0        0   130676 2020-02-02 00:00:00.000000 storekit_python-0.0.1/pdm.lock
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 storekit_python-0.0.1/.github/workflows/ci.yaml
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 storekit_python-0.0.1/.github/workflows/release.yml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 storekit_python-0.0.1/storekit/__init__.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 storekit_python-0.0.1/storekit/exceptions.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 storekit_python-0.0.1/storekit/jws.py
--rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 storekit_python-0.0.1/storekit/models.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 storekit_python-0.0.1/storekit/app_store_receipts/__init__.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 storekit_python-0.0.1/storekit/app_store_receipts/client.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 storekit_python-0.0.1/storekit/app_store_receipts/exceptions.py
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 storekit_python-0.0.1/storekit/app_store_receipts/verify_receipt_response.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 storekit_python-0.0.1/storekit/app_store_server_api/__init__.py
--rw-r--r--   0        0        0     5433 2020-02-02 00:00:00.000000 storekit_python-0.0.1/storekit/app_store_server_api/client.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 storekit_python-0.0.1/storekit/app_store_server_api/exceptions.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 storekit_python-0.0.1/storekit/app_store_server_api/history_response.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 storekit_python-0.0.1/storekit/app_store_server_api/order_look_up_response.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 storekit_python-0.0.1/storekit/app_store_server_api/status_response.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 storekit_python-0.0.1/storekit/app_store_server_api/transaction_info_response.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 storekit_python-0.0.1/storekit/app_store_server_notifications/__init__.py
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 storekit_python-0.0.1/storekit/app_store_server_notifications/response_body.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 storekit_python-0.0.1/storekit/utils/__init__.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 storekit_python-0.0.1/storekit/utils/enum.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 storekit_python-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     5794 2020-02-02 00:00:00.000000 storekit_python-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 storekit_python-0.0.1/tests/test_jws.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 storekit_python-0.0.1/tests/test_app_store_receipts/__init__.py
--rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 storekit_python-0.0.1/tests/test_app_store_receipts/test_verify_receipt_response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 storekit_python-0.0.1/tests/test_app_store_server_api/__init__.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 storekit_python-0.0.1/tests/test_app_store_server_api/test_history_response.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 storekit_python-0.0.1/tests/test_app_store_server_api/test_order_look_up_response.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 storekit_python-0.0.1/tests/test_app_store_server_api/test_status_response.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 storekit_python-0.0.1/tests/test_app_store_server_api/test_transaction_info_response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 storekit_python-0.0.1/tests/test_app_store_server_notifications/__init__.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 storekit_python-0.0.1/tests/test_app_store_server_notifications/test_response_body.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 storekit_python-0.0.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 storekit_python-0.0.1/LICENSE
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 storekit_python-0.0.1/README.md
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 storekit_python-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 storekit_python-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 storekit_python-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 storekit_python-0.0.2/Makefile
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 storekit_python-0.0.2/README_zh.md
+-rw-r--r--   0        0        0   130676 2020-02-02 00:00:00.000000 storekit_python-0.0.2/pdm.lock
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 storekit_python-0.0.2/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 storekit_python-0.0.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 storekit_python-0.0.2/storekit/__init__.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 storekit_python-0.0.2/storekit/exceptions.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 storekit_python-0.0.2/storekit/jws.py
+-rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 storekit_python-0.0.2/storekit/models.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 storekit_python-0.0.2/storekit/app_store_receipts/__init__.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 storekit_python-0.0.2/storekit/app_store_receipts/client.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 storekit_python-0.0.2/storekit/app_store_receipts/exceptions.py
+-rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 storekit_python-0.0.2/storekit/app_store_receipts/verify_receipt_response.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 storekit_python-0.0.2/storekit/app_store_server_api/__init__.py
+-rw-r--r--   0        0        0     5433 2020-02-02 00:00:00.000000 storekit_python-0.0.2/storekit/app_store_server_api/client.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 storekit_python-0.0.2/storekit/app_store_server_api/exceptions.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 storekit_python-0.0.2/storekit/app_store_server_api/history_response.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 storekit_python-0.0.2/storekit/app_store_server_api/order_look_up_response.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 storekit_python-0.0.2/storekit/app_store_server_api/status_response.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 storekit_python-0.0.2/storekit/app_store_server_api/transaction_info_response.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 storekit_python-0.0.2/storekit/app_store_server_notifications/__init__.py
+-rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 storekit_python-0.0.2/storekit/app_store_server_notifications/response_body.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 storekit_python-0.0.2/storekit/utils/__init__.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 storekit_python-0.0.2/storekit/utils/enum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 storekit_python-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     5794 2020-02-02 00:00:00.000000 storekit_python-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 storekit_python-0.0.2/tests/test_jws.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 storekit_python-0.0.2/tests/test_app_store_receipts/__init__.py
+-rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 storekit_python-0.0.2/tests/test_app_store_receipts/test_verify_receipt_response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 storekit_python-0.0.2/tests/test_app_store_server_api/__init__.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 storekit_python-0.0.2/tests/test_app_store_server_api/test_history_response.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 storekit_python-0.0.2/tests/test_app_store_server_api/test_order_look_up_response.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 storekit_python-0.0.2/tests/test_app_store_server_api/test_status_response.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 storekit_python-0.0.2/tests/test_app_store_server_api/test_transaction_info_response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 storekit_python-0.0.2/tests/test_app_store_server_notifications/__init__.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 storekit_python-0.0.2/tests/test_app_store_server_notifications/test_response_body.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 storekit_python-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 storekit_python-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 storekit_python-0.0.2/README.md
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 storekit_python-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 storekit_python-0.0.2/PKG-INFO
```

### Comparing `storekit_python-0.0.1/.pre-commit-config.yaml` & `storekit_python-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/README_zh.md` & `storekit_python-0.0.2/README_zh.md`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/pdm.lock` & `storekit_python-0.0.2/pdm.lock`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/.github/workflows/ci.yaml` & `storekit_python-0.0.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/.github/workflows/release.yml` & `storekit_python-0.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/storekit/jws.py` & `storekit_python-0.0.2/storekit/jws.py`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/storekit/models.py` & `storekit_python-0.0.2/storekit/models.py`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/storekit/app_store_receipts/client.py` & `storekit_python-0.0.2/storekit/app_store_receipts/client.py`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/storekit/app_store_receipts/exceptions.py` & `storekit_python-0.0.2/storekit/app_store_receipts/exceptions.py`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/storekit/app_store_receipts/verify_receipt_response.py` & `storekit_python-0.0.2/storekit/app_store_receipts/verify_receipt_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     https://developer.apple.com/documentation/appstorereceipts/responsebody/receipt
     """
 
     adam_id: int = 0
     app_item_id: int = 0
     application_version: str = ""
     bundle_id: str = ""
-    download_id: int = 0
+    download_id: Optional[int] = None
     expiration_date: str = ""
     expiration_date_ms: int = 0
     expiration_date_pst: str = ""
     in_app: List[Transaction] = []
     original_application_version: str = ""
     original_purchase_date: str = ""
     original_purchase_date_ms: int = 0
```

### Comparing `storekit_python-0.0.1/storekit/app_store_server_api/client.py` & `storekit_python-0.0.2/storekit/app_store_server_api/client.py`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/storekit/app_store_server_api/exceptions.py` & `storekit_python-0.0.2/storekit/app_store_server_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/storekit/app_store_server_api/history_response.py` & `storekit_python-0.0.2/storekit/app_store_server_api/history_response.py`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/storekit/app_store_server_api/order_look_up_response.py` & `storekit_python-0.0.2/storekit/app_store_server_api/order_look_up_response.py`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/storekit/app_store_server_api/status_response.py` & `storekit_python-0.0.2/storekit/app_store_server_api/status_response.py`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/storekit/app_store_server_notifications/response_body.py` & `storekit_python-0.0.2/storekit/app_store_server_notifications/response_body.py`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/storekit/utils/enum.py` & `storekit_python-0.0.2/storekit/utils/enum.py`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/tests/conftest.py` & `storekit_python-0.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/tests/test_jws.py` & `storekit_python-0.0.2/tests/test_jws.py`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/tests/test_app_store_receipts/test_verify_receipt_response.py` & `storekit_python-0.0.2/tests/test_app_store_receipts/test_verify_receipt_response.py`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/tests/test_app_store_server_api/test_history_response.py` & `storekit_python-0.0.2/tests/test_app_store_server_api/test_history_response.py`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/tests/test_app_store_server_api/test_order_look_up_response.py` & `storekit_python-0.0.2/tests/test_app_store_server_api/test_order_look_up_response.py`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/tests/test_app_store_server_api/test_status_response.py` & `storekit_python-0.0.2/tests/test_app_store_server_api/test_status_response.py`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/tests/test_app_store_server_notifications/test_response_body.py` & `storekit_python-0.0.2/tests/test_app_store_server_notifications/test_response_body.py`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/LICENSE` & `storekit_python-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/README.md` & `storekit_python-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `storekit_python-0.0.1/pyproject.toml` & `storekit_python-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "storekit-python"
-version = "0.0.1"
+version = "0.0.2"
 description = "The Storekit Python library provides support for in-app purchases and interactions with the App Store."
 authors = [
     { name = "crowser", email = "xuwendi@xiachufang.com" },
 ]
 dependencies = [
     "requests>=2.12.0",
     "pydantic>=1.9.0",
```

### Comparing `storekit_python-0.0.1/PKG-INFO` & `storekit_python-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storekit-python
-Version: 0.0.1
+Version: 0.0.2
 Summary: The Storekit Python library provides support for in-app purchases and interactions with the App Store.
 Author-email: crowser <xuwendi@xiachufang.com>
 License: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

