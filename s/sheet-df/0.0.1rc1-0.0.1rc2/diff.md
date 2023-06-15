# Comparing `tmp/sheet_df-0.0.1rc1.tar.gz` & `tmp/sheet_df-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sheet_df-0.0.1rc1.tar", last modified: Fri Jun  9 19:52:54 2023, max compression
+gzip compressed data, was "sheet_df-0.0.1rc2.tar", last modified: Fri Jun  9 23:42:24 2023, max compression
```

## Comparing `sheet_df-0.0.1rc1.tar` & `sheet_df-0.0.1rc2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-09 19:52:54.056301 sheet_df-0.0.1rc1/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     3557 2023-04-12 20:53:55.000000 sheet_df-0.0.1rc1/CONTRIBUTING.rst
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1070 2023-04-12 20:53:55.000000 sheet_df-0.0.1rc1/LICENSE
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      222 2023-06-09 19:17:35.000000 sheet_df-0.0.1rc1/MANIFEST.in
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1803 2023-06-09 19:52:54.056301 sheet_df-0.0.1rc1/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1108 2023-06-09 19:52:33.000000 sheet_df-0.0.1rc1/README.rst
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       38 2023-06-09 19:52:54.056301 sheet_df-0.0.1rc1/setup.cfg
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1249 2023-06-09 19:44:04.000000 sheet_df-0.0.1rc1/setup.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-09 19:52:54.056301 sheet_df-0.0.1rc1/sheet_df/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-09 19:26:34.000000 sheet_df-0.0.1rc1/sheet_df/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1568 2023-06-09 19:44:17.000000 sheet_df-0.0.1rc1/sheet_df/sheet_df.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-09 19:52:54.056301 sheet_df-0.0.1rc1/sheet_df.egg-info/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1803 2023-06-09 19:52:53.000000 sheet_df-0.0.1rc1/sheet_df.egg-info/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      306 2023-06-09 19:52:53.000000 sheet_df-0.0.1rc1/sheet_df.egg-info/SOURCES.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-09 19:52:53.000000 sheet_df-0.0.1rc1/sheet_df.egg-info/dependency_links.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-09 19:52:53.000000 sheet_df-0.0.1rc1/sheet_df.egg-info/not-zip-safe
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      106 2023-06-09 19:52:53.000000 sheet_df-0.0.1rc1/sheet_df.egg-info/requires.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        9 2023-06-09 19:52:53.000000 sheet_df-0.0.1rc1/sheet_df.egg-info/top_level.txt
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-09 19:52:54.056301 sheet_df-0.0.1rc1/tests/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-09 19:23:05.000000 sheet_df-0.0.1rc1/tests/__init__.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-09 23:42:24.423479 sheet_df-0.0.1rc2/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     3535 2023-06-09 23:11:39.000000 sheet_df-0.0.1rc2/CONTRIBUTING.rst
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1070 2023-04-12 20:53:55.000000 sheet_df-0.0.1rc2/LICENSE
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      222 2023-06-09 19:17:35.000000 sheet_df-0.0.1rc2/MANIFEST.in
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1762 2023-06-09 23:42:24.419479 sheet_df-0.0.1rc2/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1067 2023-06-09 23:15:04.000000 sheet_df-0.0.1rc2/README.rst
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       38 2023-06-09 23:42:24.423479 sheet_df-0.0.1rc2/setup.cfg
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1249 2023-06-09 23:41:58.000000 sheet_df-0.0.1rc2/setup.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-09 23:42:24.419479 sheet_df-0.0.1rc2/sheet_df/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-09 19:26:34.000000 sheet_df-0.0.1rc2/sheet_df/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1612 2023-06-09 23:41:23.000000 sheet_df-0.0.1rc2/sheet_df/sheet_df.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-09 23:42:24.419479 sheet_df-0.0.1rc2/sheet_df.egg-info/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1762 2023-06-09 23:42:24.000000 sheet_df-0.0.1rc2/sheet_df.egg-info/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      306 2023-06-09 23:42:24.000000 sheet_df-0.0.1rc2/sheet_df.egg-info/SOURCES.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-09 23:42:24.000000 sheet_df-0.0.1rc2/sheet_df.egg-info/dependency_links.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-09 23:42:24.000000 sheet_df-0.0.1rc2/sheet_df.egg-info/not-zip-safe
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      106 2023-06-09 23:42:24.000000 sheet_df-0.0.1rc2/sheet_df.egg-info/requires.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        9 2023-06-09 23:42:24.000000 sheet_df-0.0.1rc2/sheet_df.egg-info/top_level.txt
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-09 23:42:24.419479 sheet_df-0.0.1rc2/tests/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-09 19:23:05.000000 sheet_df-0.0.1rc2/tests/__init__.py
```

### Comparing `sheet_df-0.0.1rc1/CONTRIBUTING.rst` & `sheet_df-0.0.1rc2/CONTRIBUTING.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-.. highlight:: shell
-
 ============
 Contributing
 ============
 
 Contributions are welcome, and they are greatly appreciated! Every little bit
 helps, and credit will always be given.
```

### Comparing `sheet_df-0.0.1rc1/LICENSE` & `sheet_df-0.0.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `sheet_df-0.0.1rc1/PKG-INFO` & `sheet_df-0.0.1rc2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheet_df
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: Google sheet to dataframe
 Home-page: https://github.com/neo-andrew-moss/sheet_df
 Author: Andrew Moss
 Author-email: andrew.moss@neofinancial.com
 License: MIT license
 Keywords: sheet_df
 Platform: UNKNOWN
@@ -32,26 +32,23 @@
 ----------
 
 This Python program connects to the google sheets api and creates a pandas dataframe from the target sheet.
 
 Usage
 -----
 
-.. code-block:: bash
-
-   python -m sheet_df --directory <directory> --include_non_join_keys <True/False>
-
 .. code-block:: python
 
-   df = read_google_sheet_into_dataframe(sheet_id, range_name)
+   df = read_google_sheet_into_dataframe(sheet_id, range_name, credentials_path)
 
 Config
 ------
 
-You must have SHEET_ID and RANGE_NAME env vars. You will also need a credentials.json and a token.pickle from google.
+You must have `SHEET_ID`` and `RANGE_NAME`` env vars. You will also need a `credentials.json` from google. The `credentials_path`
+arg defaults to "credentials.json"
 
 DEV
 ---
 
 Create venv
 ~~~~~~~~~~~~
```

### Comparing `sheet_df-0.0.1rc1/README.rst` & `sheet_df-0.0.1rc2/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -11,26 +11,23 @@
 ----------
 
 This Python program connects to the google sheets api and creates a pandas dataframe from the target sheet.
 
 Usage
 -----
 
-.. code-block:: bash
-
-   python -m sheet_df --directory <directory> --include_non_join_keys <True/False>
-
 .. code-block:: python
 
-   df = read_google_sheet_into_dataframe(sheet_id, range_name)
+   df = read_google_sheet_into_dataframe(sheet_id, range_name, credentials_path)
 
 Config
 ------
 
-You must have SHEET_ID and RANGE_NAME env vars. You will also need a credentials.json and a token.pickle from google.
+You must have `SHEET_ID`` and `RANGE_NAME`` env vars. You will also need a `credentials.json` from google. The `credentials_path`
+arg defaults to "credentials.json"
 
 DEV
 ---
 
 Create venv
 ~~~~~~~~~~~~
```

### Comparing `sheet_df-0.0.1rc1/setup.py` & `sheet_df-0.0.1rc2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,10 +33,10 @@
     include_package_data=True,
     keywords="sheet_df",
     name="sheet_df",
     packages=find_packages(include=["sheet_df", "sheet_df.*"]),
     test_suite="tests",
     tests_require=["pytest"],
     url="https://github.com/neo-andrew-moss/sheet_df",
-    version="0.0.1rc1",
+    version="0.0.1rc2",
     zip_safe=False,
 )
```

### Comparing `sheet_df-0.0.1rc1/sheet_df/sheet_df.py` & `sheet_df-0.0.1rc2/sheet_df/sheet_df.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import pickle
 import os
 import os.path
 
 import pandas as pd
+from pandas import DataFrame
 from dotenv import load_dotenv
 from google.auth.transport.requests import Request
 from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
 
 load_dotenv()
 
 
-def read_google_sheet_into_dataframe(sheet_id, range_name):
+def read_google_sheet_into_dataframe(
+    sheet_id: str, range_name: str, credentials_path="credentials.json"
+) -> DataFrame:
     creds = None
     token_path = "token.pickle"
-    credentials_path = "credentials.json"
 
     if os.path.exists(token_path):
         with open(token_path, "rb") as token:
             creds = pickle.load(token)
 
     if not creds or not creds.valid:
         if creds and creds.expired and creds.refresh_token:
@@ -36,16 +38,15 @@
     service = build("sheets", "v4", credentials=creds)
 
     sheet = service.spreadsheets()
     result = sheet.values().get(spreadsheetId=sheet_id, range=range_name).execute()
     values = result.get("values", [])
 
     if not values:
-        print("No data found in the Google Sheet.")
-        return None
+        raise ValueError("No data found in the Google Sheet.")
 
     df = pd.DataFrame(values[1:], columns=values[0])
     return df
 
 
 if __name__ == "__main__":
     sheet_id = os.environ.get("SHEET_ID")
```

### Comparing `sheet_df-0.0.1rc1/sheet_df.egg-info/PKG-INFO` & `sheet_df-0.0.1rc2/sheet_df.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheet-df
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: Google sheet to dataframe
 Home-page: https://github.com/neo-andrew-moss/sheet_df
 Author: Andrew Moss
 Author-email: andrew.moss@neofinancial.com
 License: MIT license
 Keywords: sheet_df
 Platform: UNKNOWN
@@ -32,26 +32,23 @@
 ----------
 
 This Python program connects to the google sheets api and creates a pandas dataframe from the target sheet.
 
 Usage
 -----
 
-.. code-block:: bash
-
-   python -m sheet_df --directory <directory> --include_non_join_keys <True/False>
-
 .. code-block:: python
 
-   df = read_google_sheet_into_dataframe(sheet_id, range_name)
+   df = read_google_sheet_into_dataframe(sheet_id, range_name, credentials_path)
 
 Config
 ------
 
-You must have SHEET_ID and RANGE_NAME env vars. You will also need a credentials.json and a token.pickle from google.
+You must have `SHEET_ID`` and `RANGE_NAME`` env vars. You will also need a `credentials.json` from google. The `credentials_path`
+arg defaults to "credentials.json"
 
 DEV
 ---
 
 Create venv
 ~~~~~~~~~~~~
```

