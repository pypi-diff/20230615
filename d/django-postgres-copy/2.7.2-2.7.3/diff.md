# Comparing `tmp/django-postgres-copy-2.7.2.tar.gz` & `tmp/django-postgres-copy-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-postgres-copy-2.7.2.tar", last modified: Tue Feb 21 21:26:16 2023, max compression
+gzip compressed data, was "django-postgres-copy-2.7.3.tar", last modified: Thu Jun 15 13:31:50 2023, max compression
```

## Comparing `django-postgres-copy-2.7.2.tar` & `django-postgres-copy-2.7.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:26:16.628990 django-postgres-copy-2.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:26:16.624990 django-postgres-copy-2.7.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:26:16.624990 django-postgres-copy-2.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/.github/workflows/continuous-deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-02-21 21:26:16.628990 django-postgres-copy-2.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    39644 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:26:16.624990 django-postgres-copy-2.7.2/django_postgres_copy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-02-21 21:26:16.000000 django-postgres-copy-2.7.2/django_postgres_copy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-02-21 21:26:16.000000 django-postgres-copy-2.7.2/django_postgres_copy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 21:26:16.000000 django-postgres-copy-2.7.2/django_postgres_copy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-21 21:26:16.000000 django-postgres-copy-2.7.2/django_postgres_copy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:26:16.624990 django-postgres-copy-2.7.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:26:16.624990 django-postgres-copy-2.7.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:26:16.624990 django-postgres-copy-2.7.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    22552 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:26:16.624990 django-postgres-copy-2.7.2/postgres_copy/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/postgres_copy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/postgres_copy/copy_from.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/postgres_copy/copy_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/postgres_copy/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-21 21:26:16.628990 django-postgres-copy-2.7.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4963 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:26:16.628990 django-postgres-copy-2.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:26:16.628990 django-postgres-copy-2.7.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/tests/data/backwards.csv
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/tests/data/blanknulls.csv
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/tests/data/foreignkeys.csv
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/tests/data/matching_headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/tests/data/names.csv
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/tests/data/nulls.csv
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/tests/data/pipes.csv
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/tests/data/quote.csv
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/tests/data/secondary_db.csv
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/tests/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/tests/router.py
--rw-r--r--   0 runner    (1001) docker     (123)    30259 2023-02-21 21:26:05.000000 django-postgres-copy-2.7.2/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:50.408537 django-postgres-copy-2.7.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:50.408537 django-postgres-copy-2.7.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:50.408537 django-postgres-copy-2.7.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/.github/workflows/continuous-deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-15 13:31:50.412536 django-postgres-copy-2.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    39299 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:50.408537 django-postgres-copy-2.7.3/django_postgres_copy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-15 13:31:50.000000 django-postgres-copy-2.7.3/django_postgres_copy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-15 13:31:50.000000 django-postgres-copy-2.7.3/django_postgres_copy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:31:50.000000 django-postgres-copy-2.7.3/django_postgres_copy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 13:31:50.000000 django-postgres-copy-2.7.3/django_postgres_copy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:50.408537 django-postgres-copy-2.7.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:50.404536 django-postgres-copy-2.7.3/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:50.408537 django-postgres-copy-2.7.3/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22552 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:50.408537 django-postgres-copy-2.7.3/postgres_copy/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/postgres_copy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/postgres_copy/copy_from.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/postgres_copy/copy_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/postgres_copy/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-15 13:31:50.412536 django-postgres-copy-2.7.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4963 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:50.408537 django-postgres-copy-2.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:50.408537 django-postgres-copy-2.7.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/tests/data/backwards.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/tests/data/blanknulls.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/tests/data/foreignkeys.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/tests/data/matching_headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/tests/data/names.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/tests/data/nulls.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/tests/data/pipes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/tests/data/quote.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/tests/data/secondary_db.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/tests/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/tests/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30259 2023-06-15 13:31:41.000000 django-postgres-copy-2.7.3/tests/tests.py
```

### Comparing `django-postgres-copy-2.7.2/.github/workflows/continuous-deployment.yaml` & `django-postgres-copy-2.7.3/.github/workflows/continuous-deployment.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
           POSTGRES_DB: postgres
         ports:
           - 5432:5432
         # needed because the postgres container does not provide a healthcheck
         options: --health-cmd pg_isready --health-interval 10s --health-timeout 5s --health-retries 5
     strategy:
       matrix:
-        python: ["3.8", "3.9", "3.10"]
+        python: ["3.8", "3.9", "3.10", "3.11"]
     steps:
       - name: Checkout the repo
         uses: actions/checkout@v3
 
       - name: psycopg2 prerequisites
         run: sudo apt-get install libpq-dev postgresql-client
```

### Comparing `django-postgres-copy-2.7.2/.github/workflows/docs.yml` & `django-postgres-copy-2.7.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `django-postgres-copy-2.7.2/CODE_OF_CONDUCT.md` & `django-postgres-copy-2.7.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-postgres-copy-2.7.2/LICENSE` & `django-postgres-copy-2.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-postgres-copy-2.7.2/PKG-INFO` & `django-postgres-copy-2.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-postgres-copy
-Version: 2.7.2
+Version: 2.7.3
 Summary: Quickly import and export delimited data with Django support for PostgreSQL’s COPY command
 Home-page: https://palewi.re/docs/django-postgres-copy/
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: MIT
 Project-URL: Documentation, https://palewi.re/docs/django-postgres-copy/
 Project-URL: Source, https://github.com/palewire/django-postgres-copy
```

### Comparing `django-postgres-copy-2.7.2/Pipfile.lock` & `django-postgres-copy-2.7.3/Pipfile.lock`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9009730069052102%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'3974239001614c9ddacd22020efb10243aafa5f1363eb046d743e7a60037138b'}}",*

 * * "'default'": "{'asgiref': {'hashes': "*

 * *              "['sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e', "*

 * *              "'sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed'], "*

 * *              "'version': '==3.7.2'}, 'django': {'hashes': "*

 * *              "['sha256:2a6b6fbff5b59dd07bef10bcb019bee2ea97a30b2a656d51346596724324badf', "*

 * *              […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "5963b30eca17c877fad2650529856a2352a4bbdf0cf251f46bdf10e2ce896699"
+            "sha256": "3974239001614c9ddacd22020efb10243aafa5f1363eb046d743e7a60037138b"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.9"
         },
         "sources": [
             {
@@ -14,19 +14,19 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "asgiref": {
             "hashes": [
-                "sha256:1d2880b792ae8757289136f1db2b7b99100ce959b2aa57fd69dab783d05afac4",
-                "sha256:4a29362a6acebe09bf1d6640db38c1dc3d9217c68e6f9f6204d72667fc19a424"
+                "sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e",
+                "sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.5.2"
+            "version": "==3.7.2"
         },
         "backports.zoneinfo": {
             "hashes": [
                 "sha256:17746bd546106fa389c51dbea67c8b7c8f0d14b5526a579ca6ccf5ed72c526cf",
                 "sha256:1b13e654a55cd45672cb54ed12148cd33628f672548f373963b0bff67b217328",
                 "sha256:1c5742112073a563c81f786e77514969acb58649bcdf6cdf0b4ed31a348d4546",
                 "sha256:4a0f800587060bf8880f954dbef70de6c11bbe59c673c3d818921f042f9954a6",
@@ -44,267 +44,251 @@
                 "sha256:fadbfe37f74051d024037f223b8e001611eac868b5c5b06144ef4d8b799862f2"
             ],
             "index": "pypi",
             "version": "==0.2.1"
         },
         "django": {
             "hashes": [
-                "sha256:678bbfc8604eb246ed54e2063f0765f13b321a50526bdc8cb1f943eda7fa31f1",
-                "sha256:6b1de6886cae14c7c44d188f580f8ba8da05750f544c80ae5ad43375ab293cd5"
+                "sha256:2a6b6fbff5b59dd07bef10bcb019bee2ea97a30b2a656d51346596724324badf",
+                "sha256:672b3fa81e1f853bb58be1b51754108ab4ffa12a77c06db86aa8df9ed0c46fe5"
             ],
             "index": "pypi",
-            "version": "==4.1.3"
+            "version": "==4.2.2"
         },
         "psycopg2": {
             "hashes": [
-                "sha256:093e3894d2d3c592ab0945d9eba9d139c139664dcf83a1c440b8a7aa9bb21955",
-                "sha256:190d51e8c1b25a47484e52a79638a8182451d6f6dff99f26ad9bd81e5359a0fa",
-                "sha256:1a5c7d7d577e0eabfcf15eb87d1e19314c8c4f0e722a301f98e0e3a65e238b4e",
-                "sha256:1e5a38aa85bd660c53947bd28aeaafb6a97d70423606f1ccb044a03a1203fe4a",
-                "sha256:322fd5fca0b1113677089d4ebd5222c964b1760e361f151cbb2706c4912112c5",
-                "sha256:4cb9936316d88bfab614666eb9e32995e794ed0f8f6b3b718666c22819c1d7ee",
-                "sha256:920bf418000dd17669d2904472efeab2b20546efd0548139618f8fa305d1d7ad",
-                "sha256:922cc5f0b98a5f2b1ff481f5551b95cd04580fd6f0c72d9b22e6c0145a4840e0",
-                "sha256:a5246d2e683a972e2187a8714b5c2cf8156c064629f9a9b1a873c1730d9e245a",
-                "sha256:b9ac1b0d8ecc49e05e4e182694f418d27f3aedcfca854ebd6c05bb1cffa10d6d",
-                "sha256:d3ef67e630b0de0779c42912fe2cbae3805ebaba30cda27fea2a3de650a9414f",
-                "sha256:f5b6320dbc3cf6cfb9f25308286f9f7ab464e65cfb105b64cc9c52831748ced2",
-                "sha256:fc04dd5189b90d825509caa510f20d1d504761e78b8dfb95a0ede180f71d50e5"
+                "sha256:11aca705ec888e4f4cea97289a0bf0f22a067a32614f6ef64fcf7b8bfbc53744",
+                "sha256:1861a53a6a0fd248e42ea37c957d36950da00266378746588eab4f4b5649e95f",
+                "sha256:2362ee4d07ac85ff0ad93e22c693d0f37ff63e28f0615a16b6635a645f4b9214",
+                "sha256:36c941a767341d11549c0fbdbb2bf5be2eda4caf87f65dfcd7d146828bd27f39",
+                "sha256:53f4ad0a3988f983e9b49a5d9765d663bbe84f508ed655affdb810af9d0972ad",
+                "sha256:869776630c04f335d4124f120b7fb377fe44b0a7645ab3c34b4ba42516951889",
+                "sha256:a8ad4a47f42aa6aec8d061fdae21eaed8d864d4bb0f0cade5ad32ca16fcd6258",
+                "sha256:b81fcb9ecfc584f661b71c889edeae70bae30d3ef74fa0ca388ecda50b1222b7",
+                "sha256:d24ead3716a7d093b90b27b3d73459fe8cd90fd7065cf43b3c40966221d8c394",
+                "sha256:ded2faa2e6dfb430af7713d87ab4abbfc764d8d7fb73eafe96a24155f906ebf5",
+                "sha256:f15158418fd826831b28585e2ab48ed8df2d0d98f502a2b4fe619e7d5ca29011",
+                "sha256:f75001a1cbbe523e00b0ef896a5a1ada2da93ccd752b7636db5a99bc57c44494",
+                "sha256:f7a7a5ee78ba7dc74265ba69e010ae89dae635eea0e97b055fb641a01a31d2b1"
             ],
             "index": "pypi",
-            "version": "==2.9.5"
+            "version": "==2.9.6"
         },
         "sqlparse": {
             "hashes": [
-                "sha256:0323c0ec29cd52bceabc1b4d9d579e311f3e4961b98d174201d5622a23b85e34",
-                "sha256:69ca804846bb114d2ec380e4360a8a340db83f0ccf3afceeb1404df028f57268"
+                "sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3",
+                "sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c"
             ],
             "markers": "python_version >= '3.5'",
-            "version": "==0.4.3"
+            "version": "==0.4.4"
+        },
+        "typing-extensions": {
+            "hashes": [
+                "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26",
+                "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
+            ],
+            "markers": "python_version < '3.11'",
+            "version": "==4.6.3"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
-                "sha256:446438bdcca0e05bd45ea2de1668c1d9b032e1a9154c2c259092d77031ddd359",
-                "sha256:a661d72d58e6ea8a57f7a86e37d86716863ee5e92788398526d58b26a4e4dc02"
+                "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
+                "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
             ],
-            "version": "==0.7.12"
+            "markers": "python_version >= '3.6'",
+            "version": "==0.7.13"
         },
         "babel": {
             "hashes": [
-                "sha256:1ad3eca1c885218f6dce2ab67291178944f810a10a9b5f3cb8382a5a232b64fe",
-                "sha256:5ef4b3226b0180dedded4229651c8b0e1a3a6a2837d45a073272f313e4cf97f6"
+                "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
+                "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.11.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.12.1"
         },
         "bleach": {
             "hashes": [
-                "sha256:085f7f33c15bd408dd9b17a4ad77c577db66d76203e5984b1bd59baeee948b2a",
-                "sha256:0d03255c47eb9bd2f26aa9bb7f2107732e7e8fe195ca2f64709fcf3b0a4a085c"
+                "sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414",
+                "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==5.0.1"
+            "version": "==6.0.0"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
-            ],
-            "index": "pypi",
-            "version": "==2022.12.7"
-        },
-        "cffi": {
-            "hashes": [
-                "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
-                "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
-                "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
-                "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
-                "sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405",
-                "sha256:198caafb44239b60e252492445da556afafc7d1e3ab7a1fb3f0584ef6d742375",
-                "sha256:1e74c6b51a9ed6589199c787bf5f9875612ca4a8a0785fb2d4a84429badaf22a",
-                "sha256:2012c72d854c2d03e45d06ae57f40d78e5770d252f195b93f581acf3ba44496e",
-                "sha256:21157295583fe8943475029ed5abdcf71eb3911894724e360acff1d61c1d54bc",
-                "sha256:2470043b93ff09bf8fb1d46d1cb756ce6132c54826661a32d4e4d132e1977adf",
-                "sha256:285d29981935eb726a4399badae8f0ffdff4f5050eaa6d0cfc3f64b857b77185",
-                "sha256:30d78fbc8ebf9c92c9b7823ee18eb92f2e6ef79b45ac84db507f52fbe3ec4497",
-                "sha256:320dab6e7cb2eacdf0e658569d2575c4dad258c0fcc794f46215e1e39f90f2c3",
-                "sha256:33ab79603146aace82c2427da5ca6e58f2b3f2fb5da893ceac0c42218a40be35",
-                "sha256:3548db281cd7d2561c9ad9984681c95f7b0e38881201e157833a2342c30d5e8c",
-                "sha256:3799aecf2e17cf585d977b780ce79ff0dc9b78d799fc694221ce814c2c19db83",
-                "sha256:39d39875251ca8f612b6f33e6b1195af86d1b3e60086068be9cc053aa4376e21",
-                "sha256:3b926aa83d1edb5aa5b427b4053dc420ec295a08e40911296b9eb1b6170f6cca",
-                "sha256:3bcde07039e586f91b45c88f8583ea7cf7a0770df3a1649627bf598332cb6984",
-                "sha256:3d08afd128ddaa624a48cf2b859afef385b720bb4b43df214f85616922e6a5ac",
-                "sha256:3eb6971dcff08619f8d91607cfc726518b6fa2a9eba42856be181c6d0d9515fd",
-                "sha256:40f4774f5a9d4f5e344f31a32b5096977b5d48560c5592e2f3d2c4374bd543ee",
-                "sha256:4289fc34b2f5316fbb762d75362931e351941fa95fa18789191b33fc4cf9504a",
-                "sha256:470c103ae716238bbe698d67ad020e1db9d9dba34fa5a899b5e21577e6d52ed2",
-                "sha256:4f2c9f67e9821cad2e5f480bc8d83b8742896f1242dba247911072d4fa94c192",
-                "sha256:50a74364d85fd319352182ef59c5c790484a336f6db772c1a9231f1c3ed0cbd7",
-                "sha256:54a2db7b78338edd780e7ef7f9f6c442500fb0d41a5a4ea24fff1c929d5af585",
-                "sha256:5635bd9cb9731e6d4a1132a498dd34f764034a8ce60cef4f5319c0541159392f",
-                "sha256:59c0b02d0a6c384d453fece7566d1c7e6b7bae4fc5874ef2ef46d56776d61c9e",
-                "sha256:5d598b938678ebf3c67377cdd45e09d431369c3b1a5b331058c338e201f12b27",
-                "sha256:5df2768244d19ab7f60546d0c7c63ce1581f7af8b5de3eb3004b9b6fc8a9f84b",
-                "sha256:5ef34d190326c3b1f822a5b7a45f6c4535e2f47ed06fec77d3d799c450b2651e",
-                "sha256:6975a3fac6bc83c4a65c9f9fcab9e47019a11d3d2cf7f3c0d03431bf145a941e",
-                "sha256:6c9a799e985904922a4d207a94eae35c78ebae90e128f0c4e521ce339396be9d",
-                "sha256:70df4e3b545a17496c9b3f41f5115e69a4f2e77e94e1d2a8e1070bc0c38c8a3c",
-                "sha256:7473e861101c9e72452f9bf8acb984947aa1661a7704553a9f6e4baa5ba64415",
-                "sha256:8102eaf27e1e448db915d08afa8b41d6c7ca7a04b7d73af6514df10a3e74bd82",
-                "sha256:87c450779d0914f2861b8526e035c5e6da0a3199d8f1add1a665e1cbc6fc6d02",
-                "sha256:8b7ee99e510d7b66cdb6c593f21c043c248537a32e0bedf02e01e9553a172314",
-                "sha256:91fc98adde3d7881af9b59ed0294046f3806221863722ba7d8d120c575314325",
-                "sha256:94411f22c3985acaec6f83c6df553f2dbe17b698cc7f8ae751ff2237d96b9e3c",
-                "sha256:98d85c6a2bef81588d9227dde12db8a7f47f639f4a17c9ae08e773aa9c697bf3",
-                "sha256:9ad5db27f9cabae298d151c85cf2bad1d359a1b9c686a275df03385758e2f914",
-                "sha256:a0b71b1b8fbf2b96e41c4d990244165e2c9be83d54962a9a1d118fd8657d2045",
-                "sha256:a0f100c8912c114ff53e1202d0078b425bee3649ae34d7b070e9697f93c5d52d",
-                "sha256:a591fe9e525846e4d154205572a029f653ada1a78b93697f3b5a8f1f2bc055b9",
-                "sha256:a5c84c68147988265e60416b57fc83425a78058853509c1b0629c180094904a5",
-                "sha256:a66d3508133af6e8548451b25058d5812812ec3798c886bf38ed24a98216fab2",
-                "sha256:a8c4917bd7ad33e8eb21e9a5bbba979b49d9a97acb3a803092cbc1133e20343c",
-                "sha256:b3bbeb01c2b273cca1e1e0c5df57f12dce9a4dd331b4fa1635b8bec26350bde3",
-                "sha256:cba9d6b9a7d64d4bd46167096fc9d2f835e25d7e4c121fb2ddfc6528fb0413b2",
-                "sha256:cc4d65aeeaa04136a12677d3dd0b1c0c94dc43abac5860ab33cceb42b801c1e8",
-                "sha256:ce4bcc037df4fc5e3d184794f27bdaab018943698f4ca31630bc7f84a7b69c6d",
-                "sha256:cec7d9412a9102bdc577382c3929b337320c4c4c4849f2c5cdd14d7368c5562d",
-                "sha256:d400bfb9a37b1351253cb402671cea7e89bdecc294e8016a707f6d1d8ac934f9",
-                "sha256:d61f4695e6c866a23a21acab0509af1cdfd2c013cf256bbf5b6b5e2695827162",
-                "sha256:db0fbb9c62743ce59a9ff687eb5f4afbe77e5e8403d6697f7446e5f609976f76",
-                "sha256:dd86c085fae2efd48ac91dd7ccffcfc0571387fe1193d33b6394db7ef31fe2a4",
-                "sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e",
-                "sha256:e229a521186c75c8ad9490854fd8bbdd9a0c9aa3a524326b55be83b54d4e0ad9",
-                "sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6",
-                "sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b",
-                "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
-                "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
-            "version": "==1.15.1"
+            "markers": "python_version >= '3.6'",
+            "version": "==2023.5.7"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:5a3d016c7c547f69d6f81fb0db9449ce888b418b5b9952cc5e6e66843e9dd845",
-                "sha256:83e9a75d1911279afd89352c68b45348559d1fc0506b054b346651b5e7fee29f"
+                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
+                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
+                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
+                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
+                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
+                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
+                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
+                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
+                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
+                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
+                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
+                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
+                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
+                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
+                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
+                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
+                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
+                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
+                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
+                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
+                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
+                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
+                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
+                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
+                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
+                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
+                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
+                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
+                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
+                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
+                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
+                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
+                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
+                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
+                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
+                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
+                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
+                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
+                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
+                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
+                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
+                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
+                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
+                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
+                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
+                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
+                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
+                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
+                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
+                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
+                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
+                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
+                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
+                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
+                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
+                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
+                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
+                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
+                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
+                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
+                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
+                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
+                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
+                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
+                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
+                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
+                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
+                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
+                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
+                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
+                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
+                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
+                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
+                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
+                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.1.1"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==3.1.0"
         },
         "colorama": {
             "hashes": [
                 "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44",
                 "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
             "version": "==0.4.6"
         },
-        "commonmark": {
-            "hashes": [
-                "sha256:452f9dc859be7f06631ddcb328b6919c67984aca654e5fefb3914d54691aed60",
-                "sha256:da2f38c92590f83de410ba1a3cbceafbc74fee9def35f9251ba9a971d6d66fd9"
-            ],
-            "version": "==0.9.1"
-        },
         "coverage": {
             "hashes": [
-                "sha256:027018943386e7b942fa832372ebc120155fd970837489896099f5cfa2890f79",
-                "sha256:11b990d520ea75e7ee8dcab5bc908072aaada194a794db9f6d7d5cfd19661e5a",
-                "sha256:12adf310e4aafddc58afdb04d686795f33f4d7a6fa67a7a9d4ce7d6ae24d949f",
-                "sha256:1431986dac3923c5945271f169f59c45b8802a114c8f548d611f2015133df77a",
-                "sha256:1ef221513e6f68b69ee9e159506d583d31aa3567e0ae84eaad9d6ec1107dddaa",
-                "sha256:20c8ac5386253717e5ccc827caad43ed66fea0efe255727b1053a8154d952398",
-                "sha256:2198ea6fc548de52adc826f62cb18554caedfb1d26548c1b7c88d8f7faa8f6ba",
-                "sha256:255758a1e3b61db372ec2736c8e2a1fdfaf563977eedbdf131de003ca5779b7d",
-                "sha256:265de0fa6778d07de30bcf4d9dc471c3dc4314a23a3c6603d356a3c9abc2dfcf",
-                "sha256:33a7da4376d5977fbf0a8ed91c4dffaaa8dbf0ddbf4c8eea500a2486d8bc4d7b",
-                "sha256:42eafe6778551cf006a7c43153af1211c3aaab658d4d66fa5fcc021613d02518",
-                "sha256:4433b90fae13f86fafff0b326453dd42fc9a639a0d9e4eec4d366436d1a41b6d",
-                "sha256:4a5375e28c5191ac38cca59b38edd33ef4cc914732c916f2929029b4bfb50795",
-                "sha256:4a8dbc1f0fbb2ae3de73eb0bdbb914180c7abfbf258e90b311dcd4f585d44bd2",
-                "sha256:59f53f1dc5b656cafb1badd0feb428c1e7bc19b867479ff72f7a9dd9b479f10e",
-                "sha256:5dbec3b9095749390c09ab7c89d314727f18800060d8d24e87f01fb9cfb40b32",
-                "sha256:633713d70ad6bfc49b34ead4060531658dc6dfc9b3eb7d8a716d5873377ab745",
-                "sha256:6b07130585d54fe8dff3d97b93b0e20290de974dc8177c320aeaf23459219c0b",
-                "sha256:6c4459b3de97b75e3bd6b7d4b7f0db13f17f504f3d13e2a7c623786289dd670e",
-                "sha256:6d4817234349a80dbf03640cec6109cd90cba068330703fa65ddf56b60223a6d",
-                "sha256:723e8130d4ecc8f56e9a611e73b31219595baa3bb252d539206f7bbbab6ffc1f",
-                "sha256:784f53ebc9f3fd0e2a3f6a78b2be1bd1f5575d7863e10c6e12504f240fd06660",
-                "sha256:7b6be138d61e458e18d8e6ddcddd36dd96215edfe5f1168de0b1b32635839b62",
-                "sha256:7ccf362abd726b0410bf8911c31fbf97f09f8f1061f8c1cf03dfc4b6372848f6",
-                "sha256:83516205e254a0cb77d2d7bb3632ee019d93d9f4005de31dca0a8c3667d5bc04",
-                "sha256:851cf4ff24062c6aec510a454b2584f6e998cada52d4cb58c5e233d07172e50c",
-                "sha256:8f830ed581b45b82451a40faabb89c84e1a998124ee4212d440e9c6cf70083e5",
-                "sha256:94e2565443291bd778421856bc975d351738963071e9b8839ca1fc08b42d4bef",
-                "sha256:95203854f974e07af96358c0b261f1048d8e1083f2de9b1c565e1be4a3a48cfc",
-                "sha256:97117225cdd992a9c2a5515db1f66b59db634f59d0679ca1fa3fe8da32749cae",
-                "sha256:98e8a10b7a314f454d9eff4216a9a94d143a7ee65018dd12442e898ee2310578",
-                "sha256:a1170fa54185845505fbfa672f1c1ab175446c887cce8212c44149581cf2d466",
-                "sha256:a6b7d95969b8845250586f269e81e5dfdd8ff828ddeb8567a4a2eaa7313460c4",
-                "sha256:a8fb6cf131ac4070c9c5a3e21de0f7dc5a0fbe8bc77c9456ced896c12fcdad91",
-                "sha256:af4fffaffc4067232253715065e30c5a7ec6faac36f8fc8d6f64263b15f74db0",
-                "sha256:b4a5be1748d538a710f87542f22c2cad22f80545a847ad91ce45e77417293eb4",
-                "sha256:b5604380f3415ba69de87a289a2b56687faa4fe04dbee0754bfcae433489316b",
-                "sha256:b9023e237f4c02ff739581ef35969c3739445fb059b060ca51771e69101efffe",
-                "sha256:bc8ef5e043a2af066fa8cbfc6e708d58017024dc4345a1f9757b329a249f041b",
-                "sha256:c4ed2820d919351f4167e52425e096af41bfabacb1857186c1ea32ff9983ed75",
-                "sha256:cca4435eebea7962a52bdb216dec27215d0df64cf27fc1dd538415f5d2b9da6b",
-                "sha256:d900bb429fdfd7f511f868cedd03a6bbb142f3f9118c09b99ef8dc9bf9643c3c",
-                "sha256:d9ecf0829c6a62b9b573c7bb6d4dcd6ba8b6f80be9ba4fc7ed50bf4ac9aecd72",
-                "sha256:dbdb91cd8c048c2b09eb17713b0c12a54fbd587d79adcebad543bc0cd9a3410b",
-                "sha256:de3001a203182842a4630e7b8d1a2c7c07ec1b45d3084a83d5d227a3806f530f",
-                "sha256:e07f4a4a9b41583d6eabec04f8b68076ab3cd44c20bd29332c6572dda36f372e",
-                "sha256:ef8674b0ee8cc11e2d574e3e2998aea5df5ab242e012286824ea3c6970580e53",
-                "sha256:f4f05d88d9a80ad3cac6244d36dd89a3c00abc16371769f1340101d3cb899fc3",
-                "sha256:f642e90754ee3e06b0e7e51bce3379590e76b7f76b708e1a71ff043f87025c84",
-                "sha256:fc2af30ed0d5ae0b1abdb4ebdce598eafd5b35397d4d75deb341a614d333d987"
-            ],
-            "index": "pypi",
-            "version": "==6.5.0"
-        },
-        "cryptography": {
-            "hashes": [
-                "sha256:0e70da4bdff7601b0ef48e6348339e490ebfb0cbe638e083c9c41fb49f00c8bd",
-                "sha256:10652dd7282de17990b88679cb82f832752c4e8237f0c714be518044269415db",
-                "sha256:175c1a818b87c9ac80bb7377f5520b7f31b3ef2a0004e2420319beadedb67290",
-                "sha256:1d7e632804a248103b60b16fb145e8df0bc60eed790ece0d12efe8cd3f3e7744",
-                "sha256:1f13ddda26a04c06eb57119caf27a524ccae20533729f4b1e4a69b54e07035eb",
-                "sha256:2ec2a8714dd005949d4019195d72abed84198d877112abb5a27740e217e0ea8d",
-                "sha256:2fa36a7b2cc0998a3a4d5af26ccb6273f3df133d61da2ba13b3286261e7efb70",
-                "sha256:2fb481682873035600b5502f0015b664abc26466153fab5c6bc92c1ea69d478b",
-                "sha256:3178d46f363d4549b9a76264f41c6948752183b3f587666aff0555ac50fd7876",
-                "sha256:4367da5705922cf7070462e964f66e4ac24162e22ab0a2e9d31f1b270dd78083",
-                "sha256:4eb85075437f0b1fd8cd66c688469a0c4119e0ba855e3fef86691971b887caf6",
-                "sha256:50a1494ed0c3f5b4d07650a68cd6ca62efe8b596ce743a5c94403e6f11bf06c1",
-                "sha256:53049f3379ef05182864d13bb9686657659407148f901f3f1eee57a733fb4b00",
-                "sha256:6391e59ebe7c62d9902c24a4d8bcbc79a68e7c4ab65863536127c8a9cd94043b",
-                "sha256:67461b5ebca2e4c2ab991733f8ab637a7265bb582f07c7c88914b5afb88cb95b",
-                "sha256:78e47e28ddc4ace41dd38c42e6feecfdadf9c3be2af389abbfeef1ff06822285",
-                "sha256:80ca53981ceeb3241998443c4964a387771588c4e4a5d92735a493af868294f9",
-                "sha256:8a4b2bdb68a447fadebfd7d24855758fe2d6fecc7fed0b78d190b1af39a8e3b0",
-                "sha256:8e45653fb97eb2f20b8c96f9cd2b3a0654d742b47d638cf2897afbd97f80fa6d",
-                "sha256:998cd19189d8a747b226d24c0207fdaa1e6658a1d3f2494541cb9dfbf7dcb6d2",
-                "sha256:a10498349d4c8eab7357a8f9aa3463791292845b79597ad1b98a543686fb1ec8",
-                "sha256:b4cad0cea995af760f82820ab4ca54e5471fc782f70a007f31531957f43e9dee",
-                "sha256:bfe6472507986613dc6cc00b3d492b2f7564b02b3b3682d25ca7f40fa3fd321b",
-                "sha256:c9e0d79ee4c56d841bd4ac6e7697c8ff3c8d6da67379057f29e66acffcd1e9a7",
-                "sha256:ca57eb3ddaccd1112c18fc80abe41db443cc2e9dcb1917078e02dfa010a4f353",
-                "sha256:ce127dd0a6a0811c251a6cddd014d292728484e530d80e872ad9806cfb1c5b3c"
+                "sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f",
+                "sha256:06fb182e69f33f6cd1d39a6c597294cff3143554b64b9825d1dc69d18cc2fff2",
+                "sha256:0a5f9e1dbd7fbe30196578ca36f3fba75376fb99888c395c5880b355e2875f8a",
+                "sha256:0e1f928eaf5469c11e886fe0885ad2bf1ec606434e79842a879277895a50942a",
+                "sha256:171717c7cb6b453aebac9a2ef603699da237f341b38eebfee9be75d27dc38e01",
+                "sha256:1e9d683426464e4a252bf70c3498756055016f99ddaec3774bf368e76bbe02b6",
+                "sha256:201e7389591af40950a6480bd9edfa8ed04346ff80002cec1a66cac4549c1ad7",
+                "sha256:245167dd26180ab4c91d5e1496a30be4cd721a5cf2abf52974f965f10f11419f",
+                "sha256:2aee274c46590717f38ae5e4650988d1af340fe06167546cc32fe2f58ed05b02",
+                "sha256:2e07b54284e381531c87f785f613b833569c14ecacdcb85d56b25c4622c16c3c",
+                "sha256:31563e97dae5598556600466ad9beea39fb04e0229e61c12eaa206e0aa202063",
+                "sha256:33d6d3ea29d5b3a1a632b3c4e4f4ecae24ef170b0b9ee493883f2df10039959a",
+                "sha256:3d376df58cc111dc8e21e3b6e24606b5bb5dee6024f46a5abca99124b2229ef5",
+                "sha256:419bfd2caae268623dd469eff96d510a920c90928b60f2073d79f8fe2bbc5959",
+                "sha256:48c19d2159d433ccc99e729ceae7d5293fbffa0bdb94952d3579983d1c8c9d97",
+                "sha256:49969a9f7ffa086d973d91cec8d2e31080436ef0fb4a359cae927e742abfaaa6",
+                "sha256:52edc1a60c0d34afa421c9c37078817b2e67a392cab17d97283b64c5833f427f",
+                "sha256:537891ae8ce59ef63d0123f7ac9e2ae0fc8b72c7ccbe5296fec45fd68967b6c9",
+                "sha256:54b896376ab563bd38453cecb813c295cf347cf5906e8b41d340b0321a5433e5",
+                "sha256:58c2ccc2f00ecb51253cbe5d8d7122a34590fac9646a960d1430d5b15321d95f",
+                "sha256:5b7540161790b2f28143191f5f8ec02fb132660ff175b7747b95dcb77ac26562",
+                "sha256:5baa06420f837184130752b7c5ea0808762083bf3487b5038d68b012e5937dbe",
+                "sha256:5e330fc79bd7207e46c7d7fd2bb4af2963f5f635703925543a70b99574b0fea9",
+                "sha256:61b9a528fb348373c433e8966535074b802c7a5d7f23c4f421e6c6e2f1697a6f",
+                "sha256:63426706118b7f5cf6bb6c895dc215d8a418d5952544042c8a2d9fe87fcf09cb",
+                "sha256:6d040ef7c9859bb11dfeb056ff5b3872436e3b5e401817d87a31e1750b9ae2fb",
+                "sha256:6f48351d66575f535669306aa7d6d6f71bc43372473b54a832222803eb956fd1",
+                "sha256:7ee7d9d4822c8acc74a5e26c50604dff824710bc8de424904c0982e25c39c6cb",
+                "sha256:81c13a1fc7468c40f13420732805a4c38a105d89848b7c10af65a90beff25250",
+                "sha256:8d13c64ee2d33eccf7437961b6ea7ad8673e2be040b4f7fd4fd4d4d28d9ccb1e",
+                "sha256:8de8bb0e5ad103888d65abef8bca41ab93721647590a3f740100cd65c3b00511",
+                "sha256:8fa03bce9bfbeeef9f3b160a8bed39a221d82308b4152b27d82d8daa7041fee5",
+                "sha256:924d94291ca674905fe9481f12294eb11f2d3d3fd1adb20314ba89e94f44ed59",
+                "sha256:975d70ab7e3c80a3fe86001d8751f6778905ec723f5b110aed1e450da9d4b7f2",
+                "sha256:976b9c42fb2a43ebf304fa7d4a310e5f16cc99992f33eced91ef6f908bd8f33d",
+                "sha256:9e31cb64d7de6b6f09702bb27c02d1904b3aebfca610c12772452c4e6c21a0d3",
+                "sha256:a342242fe22407f3c17f4b499276a02b01e80f861f1682ad1d95b04018e0c0d4",
+                "sha256:a3d33a6b3eae87ceaefa91ffdc130b5e8536182cd6dfdbfc1aa56b46ff8c86de",
+                "sha256:a895fcc7b15c3fc72beb43cdcbdf0ddb7d2ebc959edac9cef390b0d14f39f8a9",
+                "sha256:afb17f84d56068a7c29f5fa37bfd38d5aba69e3304af08ee94da8ed5b0865833",
+                "sha256:b1c546aca0ca4d028901d825015dc8e4d56aac4b541877690eb76490f1dc8ed0",
+                "sha256:b29019c76039dc3c0fd815c41392a044ce555d9bcdd38b0fb60fb4cd8e475ba9",
+                "sha256:b46517c02ccd08092f4fa99f24c3b83d8f92f739b4657b0f146246a0ca6a831d",
+                "sha256:b7aa5f8a41217360e600da646004f878250a0d6738bcdc11a0a39928d7dc2050",
+                "sha256:b7b4c971f05e6ae490fef852c218b0e79d4e52f79ef0c8475566584a8fb3e01d",
+                "sha256:ba90a9563ba44a72fda2e85302c3abc71c5589cea608ca16c22b9804262aaeb6",
+                "sha256:cb017fd1b2603ef59e374ba2063f593abe0fc45f2ad9abdde5b4d83bd922a353",
+                "sha256:d22656368f0e6189e24722214ed8d66b8022db19d182927b9a248a2a8a2f67eb",
+                "sha256:d2c2db7fd82e9b72937969bceac4d6ca89660db0a0967614ce2481e81a0b771e",
+                "sha256:d39b5b4f2a66ccae8b7263ac3c8170994b65266797fb96cbbfd3fb5b23921db8",
+                "sha256:d62a5c7dad11015c66fbb9d881bc4caa5b12f16292f857842d9d1871595f4495",
+                "sha256:e7d9405291c6928619403db1d10bd07888888ec1abcbd9748fdaa971d7d661b2",
+                "sha256:e84606b74eb7de6ff581a7915e2dab7a28a0517fbe1c9239eb227e1354064dcd",
+                "sha256:eb393e5ebc85245347950143969b241d08b52b88a3dc39479822e073a1a8eb27",
+                "sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1",
+                "sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818",
+                "sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4",
+                "sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e",
+                "sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850",
+                "sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==38.0.4"
+            "index": "pypi",
+            "version": "==7.2.7"
         },
         "docutils": {
             "hashes": [
-                "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6",
-                "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"
+                "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
+                "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.19"
+            "version": "==0.20.1"
         },
         "flake8": {
             "hashes": [
                 "sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7",
                 "sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181"
             ],
             "index": "pypi",
@@ -324,245 +308,242 @@
                 "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:d5059f9f1e8e41f80e9c56c2ee58811450c31984dfa625329ffd7c0dad88a73b",
-                "sha256:d84d17e21670ec07990e1044a99efe8d615d860fd176fc29ef5c306068fda313"
+                "sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed",
+                "sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705"
             ],
             "markers": "python_version < '3.10'",
-            "version": "==5.1.0"
+            "version": "==6.6.0"
         },
         "jaraco.classes": {
             "hashes": [
                 "sha256:2353de3288bc6b82120752201c6b1c1a14b058267fa424ed5ce5984e3b922158",
                 "sha256:89559fa5c1d3c34eff6f631ad80bb21f378dbcbb35dd161fd2c6b93f5be2f98a"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.2.3"
         },
-        "jeepney": {
-            "hashes": [
-                "sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806",
-                "sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755"
-            ],
-            "markers": "sys_platform == 'linux'",
-            "version": "==0.8.0"
-        },
         "jinja2": {
             "hashes": [
                 "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
                 "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.2"
         },
         "keyring": {
             "hashes": [
-                "sha256:3dd30011d555f1345dec2c262f0153f2f0ca6bca041fb1dc4588349bb4c0ac1e",
-                "sha256:ad192263e2cdd5f12875dedc2da13534359a7e760e77f8d04b50968a821c2361"
+                "sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd",
+                "sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.11.0"
+            "version": "==23.13.1"
         },
         "livereload": {
             "hashes": [
-                "sha256:776f2f865e59fde56490a56bcc6773b6917366bce0c267c60ee8aaf1a0959869"
+                "sha256:776f2f865e59fde56490a56bcc6773b6917366bce0c267c60ee8aaf1a0959869",
+                "sha256:ad4ac6f53b2d62bb6ce1a5e6e96f1f00976a32348afedcb4b6d68df2a1d346e4"
             ],
             "version": "==2.6.3"
         },
+        "markdown-it-py": {
+            "hashes": [
+                "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1",
+                "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==3.0.0"
+        },
         "markupsafe": {
             "hashes": [
-                "sha256:0212a68688482dc52b2d45013df70d169f542b7394fc744c02a57374a4207003",
-                "sha256:089cf3dbf0cd6c100f02945abeb18484bd1ee57a079aefd52cffd17fba910b88",
-                "sha256:10c1bfff05d95783da83491be968e8fe789263689c02724e0c691933c52994f5",
-                "sha256:33b74d289bd2f5e527beadcaa3f401e0df0a89927c1559c8566c066fa4248ab7",
-                "sha256:3799351e2336dc91ea70b034983ee71cf2f9533cdff7c14c90ea126bfd95d65a",
-                "sha256:3ce11ee3f23f79dbd06fb3d63e2f6af7b12db1d46932fe7bd8afa259a5996603",
-                "sha256:421be9fbf0ffe9ffd7a378aafebbf6f4602d564d34be190fc19a193232fd12b1",
-                "sha256:43093fb83d8343aac0b1baa75516da6092f58f41200907ef92448ecab8825135",
-                "sha256:46d00d6cfecdde84d40e572d63735ef81423ad31184100411e6e3388d405e247",
-                "sha256:4a33dea2b688b3190ee12bd7cfa29d39c9ed176bda40bfa11099a3ce5d3a7ac6",
-                "sha256:4b9fe39a2ccc108a4accc2676e77da025ce383c108593d65cc909add5c3bd601",
-                "sha256:56442863ed2b06d19c37f94d999035e15ee982988920e12a5b4ba29b62ad1f77",
-                "sha256:671cd1187ed5e62818414afe79ed29da836dde67166a9fac6d435873c44fdd02",
-                "sha256:694deca8d702d5db21ec83983ce0bb4b26a578e71fbdbd4fdcd387daa90e4d5e",
-                "sha256:6a074d34ee7a5ce3effbc526b7083ec9731bb3cbf921bbe1d3005d4d2bdb3a63",
-                "sha256:6d0072fea50feec76a4c418096652f2c3238eaa014b2f94aeb1d56a66b41403f",
-                "sha256:6fbf47b5d3728c6aea2abb0589b5d30459e369baa772e0f37a0320185e87c980",
-                "sha256:7f91197cc9e48f989d12e4e6fbc46495c446636dfc81b9ccf50bb0ec74b91d4b",
-                "sha256:86b1f75c4e7c2ac2ccdaec2b9022845dbb81880ca318bb7a0a01fbf7813e3812",
-                "sha256:8dc1c72a69aa7e082593c4a203dcf94ddb74bb5c8a731e4e1eb68d031e8498ff",
-                "sha256:8e3dcf21f367459434c18e71b2a9532d96547aef8a871872a5bd69a715c15f96",
-                "sha256:8e576a51ad59e4bfaac456023a78f6b5e6e7651dcd383bcc3e18d06f9b55d6d1",
-                "sha256:96e37a3dc86e80bf81758c152fe66dbf60ed5eca3d26305edf01892257049925",
-                "sha256:97a68e6ada378df82bc9f16b800ab77cbf4b2fada0081794318520138c088e4a",
-                "sha256:99a2a507ed3ac881b975a2976d59f38c19386d128e7a9a18b7df6fff1fd4c1d6",
-                "sha256:a49907dd8420c5685cfa064a1335b6754b74541bbb3706c259c02ed65b644b3e",
-                "sha256:b09bf97215625a311f669476f44b8b318b075847b49316d3e28c08e41a7a573f",
-                "sha256:b7bd98b796e2b6553da7225aeb61f447f80a1ca64f41d83612e6139ca5213aa4",
-                "sha256:b87db4360013327109564f0e591bd2a3b318547bcef31b468a92ee504d07ae4f",
-                "sha256:bcb3ed405ed3222f9904899563d6fc492ff75cce56cba05e32eff40e6acbeaa3",
-                "sha256:d4306c36ca495956b6d568d276ac11fdd9c30a36f1b6eb928070dc5360b22e1c",
-                "sha256:d5ee4f386140395a2c818d149221149c54849dfcfcb9f1debfe07a8b8bd63f9a",
-                "sha256:dda30ba7e87fbbb7eab1ec9f58678558fd9a6b8b853530e176eabd064da81417",
-                "sha256:e04e26803c9c3851c931eac40c695602c6295b8d432cbe78609649ad9bd2da8a",
-                "sha256:e1c0b87e09fa55a220f058d1d49d3fb8df88fbfab58558f1198e08c1e1de842a",
-                "sha256:e72591e9ecd94d7feb70c1cbd7be7b3ebea3f548870aa91e2732960fa4d57a37",
-                "sha256:e8c843bbcda3a2f1e3c2ab25913c80a3c5376cd00c6e8c4a86a89a28c8dc5452",
-                "sha256:efc1913fd2ca4f334418481c7e595c00aad186563bbc1ec76067848c7ca0a933",
-                "sha256:f121a1420d4e173a5d96e47e9a0c0dcff965afdf1626d28de1460815f7c4ee7a",
-                "sha256:fc7b548b17d238737688817ab67deebb30e8073c95749d55538ed473130ec0c7"
+                "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e",
+                "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e",
+                "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431",
+                "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686",
+                "sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559",
+                "sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc",
+                "sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c",
+                "sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0",
+                "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4",
+                "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9",
+                "sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575",
+                "sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba",
+                "sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d",
+                "sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3",
+                "sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00",
+                "sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155",
+                "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac",
+                "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52",
+                "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f",
+                "sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8",
+                "sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b",
+                "sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24",
+                "sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea",
+                "sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198",
+                "sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0",
+                "sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee",
+                "sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be",
+                "sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2",
+                "sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707",
+                "sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6",
+                "sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58",
+                "sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779",
+                "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636",
+                "sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c",
+                "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad",
+                "sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee",
+                "sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc",
+                "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2",
+                "sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48",
+                "sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7",
+                "sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e",
+                "sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b",
+                "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa",
+                "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5",
+                "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e",
+                "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb",
+                "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9",
+                "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57",
+                "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc",
+                "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.1.1"
+            "version": "==2.1.3"
         },
         "mccabe": {
             "hashes": [
                 "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325",
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.0"
         },
+        "mdurl": {
+            "hashes": [
+                "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
+                "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.1.2"
+        },
         "mock": {
             "hashes": [
-                "sha256:122fcb64ee37cfad5b3f48d7a7d51875d7031aaf3d8be7c42e2bee25044eee62",
-                "sha256:7d3fbbde18228f4ff2f1f119a45cdffa458b4c0dee32eb4d2bb2f82554bac7bc"
+                "sha256:06f18d7d65b44428202b145a9a36e99c2ee00d1eb992df0caf881d4664377891",
+                "sha256:0e0bc5ba78b8db3667ad636d964eb963dc97a59f04c6f6214c5f0e4a8f726c56"
             ],
             "index": "pypi",
-            "version": "==4.0.3"
+            "version": "==5.0.2"
         },
         "more-itertools": {
             "hashes": [
-                "sha256:250e83d7e81d0c87ca6bd942e6aeab8cc9daa6096d12c5308f3f92fa5e5c1f41",
-                "sha256:5a6257e40878ef0520b1803990e3e22303a41b5714006c32a3fd8304b26ea1ab"
+                "sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d",
+                "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==9.0.0"
+            "version": "==9.1.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:2198ec20bd4c017b8f9717e00f0c8714076fc2fd93816750ab48e2c41de2cfd3",
-                "sha256:957e2148ba0e1a3b282772e791ef1d8083648bc131c8ab0c1feba110ce1146c3"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==22.0"
+            "version": "==23.1"
         },
         "pkginfo": {
             "hashes": [
-                "sha256:ac03e37e4d601aaee40f8087f63fc4a2a6c9814dda2c8fa6aab1b1829653bdfa",
-                "sha256:d580059503f2f4549ad6e4c106d7437356dbd430e2c7df99ee1efe03d75f691e"
+                "sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546",
+                "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==1.9.2"
+            "version": "==1.9.6"
         },
         "pycodestyle": {
             "hashes": [
                 "sha256:347187bdb476329d98f695c213d7295a846d1152ff4fe9bacb8a9590b8ee7053",
                 "sha256:8a4eaf0d0495c7395bdab3589ac2db602797d76207242c17d470186815706610"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2.10.0"
         },
-        "pycparser": {
-            "hashes": [
-                "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
-                "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
-            ],
-            "version": "==2.21"
-        },
         "pyflakes": {
             "hashes": [
                 "sha256:ec55bf7fe21fff7f1ad2f7da62363d749e2a470500eab1b555334b67aa1ef8cf",
                 "sha256:ec8b276a6b60bd80defed25add7e439881c19e64850afd9b346283d4165fd0fd"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==3.0.1"
         },
         "pygments": {
             "hashes": [
-                "sha256:56a8508ae95f98e2b9bdf93a6be5ae3f7d8af858b43e02c5a2ff083726be40c1",
-                "sha256:f643f331ab57ba3c9d89212ee4a2dabc6e94f117cf4eefde99a0574720d14c42"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.13.0"
-        },
-        "pytz": {
-            "hashes": [
-                "sha256:222439474e9c98fced559f1709d89e6c9cbf8d79c794ff3eb9f8800064291427",
-                "sha256:e89512406b793ca39f5971bc999cc538ce125c0e51c27941bef4568b460095e2"
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
-            "version": "==2022.6"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.1"
         },
         "readme-renderer": {
             "hashes": [
                 "sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273",
                 "sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==37.3"
         },
         "requests": {
             "hashes": [
-                "sha256:7c5599b102feddaa661c826c56ab4fee28bfd17f5abca1ebbe3e7f19d7c97983",
-                "sha256:8fefa2a1a1365bf5520aac41836fbee479da67864514bdb821f31ce07ce65349"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "index": "pypi",
-            "version": "==2.28.1"
+            "version": "==2.31.0"
         },
         "requests-toolbelt": {
             "hashes": [
-                "sha256:18565aa58116d9951ac39baa288d3adb5b3ff975c4f25eee78555d89e8f247f7",
-                "sha256:62e09f7ff5ccbda92772a29f394a49c3ad6cb181d568b1337626b2abb628a63d"
+                "sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6",
+                "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.10.1"
+            "version": "==1.0.0"
         },
         "rfc3986": {
             "hashes": [
                 "sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd",
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:a4eb26484f2c82589bd9a17c73d32a010b1e29d89f1604cd9bf3a2097b81bb5e",
-                "sha256:ba3a3775974105c221d31141f2c116f4fd65c5ceb0698657a11e9f295ec93fd0"
-            ],
-            "markers": "python_full_version >= '3.6.3' and python_full_version < '4.0.0'",
-            "version": "==12.6.0"
-        },
-        "secretstorage": {
-            "hashes": [
-                "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
-                "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
+                "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
+                "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
             ],
-            "markers": "sys_platform == 'linux'",
-            "version": "==3.3.3"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==13.4.2"
         },
         "setuptools": {
             "hashes": [
-                "sha256:57f6f22bde4e042978bcd50176fdb381d7c21a9efa4041202288d3737a0c6a54",
-                "sha256:a7620757bf984b58deaf32fc8a4577a9bbc0850cf92c20e1ce41c38c19e5fb75"
+                "sha256:5df61bf30bb10c6f756eb19e7c9f3b473051f48db77fddbe06ff2ca307df9a6f",
+                "sha256:62642358adc77ffa87233bc4d2354c4b2682d214048f500964dbe760ccedf102"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==65.6.3"
+            "version": "==67.8.0"
         },
         "setuptools-scm": {
             "hashes": [
-                "sha256:031e13af771d6f892b941adb6ea04545bbf91ebc5ce68c78aaf3fff6e1fb4844",
-                "sha256:7930f720905e03ccd1e1d821db521bff7ec2ac9cf0ceb6552dd73d24a45d3b02"
+                "sha256:6c508345a771aad7d56ebff0e70628bf2b0ec7573762be9960214730de278f27",
+                "sha256:73988b6d848709e2af142aa48c986ea29592bbcfca5375678064708205253d8e"
             ],
             "index": "pypi",
-            "version": "==7.0.5"
+            "version": "==7.1.0"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -573,51 +554,51 @@
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:060ca5c9f7ba57a08a1219e547b269fadf125ae25b06b9fa7f66768efb652d6d",
-                "sha256:51026de0a9ff9fc13c05d74913ad66047e104f56a129ff73e174eb5c3ee794b5"
+                "sha256:60c5e04756c1709a98845ed27a2eed7a556af3993afb66e77fec48189f742616",
+                "sha256:61e025f788c5977d9412587e733733a289e2b9fdc2fef8868ddfbfc4ccfe881d"
             ],
             "index": "pypi",
-            "version": "==5.3.0"
+            "version": "==7.0.1"
         },
         "sphinx-autobuild": {
             "hashes": [
                 "sha256:8fe8cbfdb75db04475232f05187c776f46f6e9e04cacf1e49ce81bdac649ccac",
                 "sha256:de1ca3b66e271d2b5b5140c35034c89e47f263f2cd5db302c9217065f7443f05"
             ],
             "index": "pypi",
             "version": "==2021.3.14"
         },
         "sphinxcontrib-applehelp": {
             "hashes": [
-                "sha256:806111e5e962be97c29ec4c1e7fe277bfd19e9652fb1a4392105b43e01af885a",
-                "sha256:a072735ec80e7675e3f432fcae8610ecf509c5f1869d17e2eecff44389cdbc58"
+                "sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228",
+                "sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e"
             ],
-            "markers": "python_version >= '3.5'",
-            "version": "==1.0.2"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.0.4"
         },
         "sphinxcontrib-devhelp": {
             "hashes": [
                 "sha256:8165223f9a335cc1af7ffe1ed31d2871f325254c0423bc0c4c7cd1c1e4734a2e",
                 "sha256:ff7f1afa7b9642e7060379360a67e9c41e8f3121f2ce9164266f61b9f4b338e4"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.2"
         },
         "sphinxcontrib-htmlhelp": {
             "hashes": [
-                "sha256:d412243dfb797ae3ec2b59eca0e52dac12e75a241bf0e4eb861e450d06c6ed07",
-                "sha256:f5f8bb2d0d629f398bf47d0d69c07bc13b65f75a81ad9e2f71a63d4b7a2f6db2"
+                "sha256:0cbdd302815330058422b98a113195c9249825d681e18f11e8b1f78a2f11efff",
+                "sha256:c38cb46dccf316c79de6e5515e1770414b797162b23cd3d06e67020e1d2a6903"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.0.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.0.1"
         },
         "sphinxcontrib-jsmath": {
             "hashes": [
                 "sha256:2ec2eaebfb78f3f2078e73666b1415417a116cc848b72e5172e596c871103178",
                 "sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8"
             ],
             "markers": "python_version >= '3.5'",
@@ -640,76 +621,76 @@
             "version": "==1.1.5"
         },
         "tomli": {
             "hashes": [
                 "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
-            "markers": "python_version >= '3.7'",
+            "markers": "python_version < '3.11'",
             "version": "==2.0.1"
         },
         "tornado": {
             "hashes": [
-                "sha256:1d54d13ab8414ed44de07efecb97d4ef7c39f7438cf5e976ccd356bebb1b5fca",
-                "sha256:20f638fd8cc85f3cbae3c732326e96addff0a15e22d80f049e00121651e82e72",
-                "sha256:5c87076709343557ef8032934ce5f637dbb552efa7b21d08e89ae7619ed0eb23",
-                "sha256:5f8c52d219d4995388119af7ccaa0bcec289535747620116a58d830e7c25d8a8",
-                "sha256:6fdfabffd8dfcb6cf887428849d30cf19a3ea34c2c248461e1f7d718ad30b66b",
-                "sha256:87dcafae3e884462f90c90ecc200defe5e580a7fbbb4365eda7c7c1eb809ebc9",
-                "sha256:9b630419bde84ec666bfd7ea0a4cb2a8a651c2d5cccdbdd1972a0c859dfc3c13",
-                "sha256:b8150f721c101abdef99073bf66d3903e292d851bee51910839831caba341a75",
-                "sha256:ba09ef14ca9893954244fd872798b4ccb2367c165946ce2dd7376aebdde8e3ac",
-                "sha256:d3a2f5999215a3a06a4fc218026cd84c61b8b2b40ac5296a6db1f1451ef04c1e",
-                "sha256:e5f923aa6a47e133d1cf87d60700889d7eae68988704e20c75fb2d65677a8e4b"
+                "sha256:05615096845cf50a895026f749195bf0b10b8909f9be672f50b0fe69cba368e4",
+                "sha256:0c325e66c8123c606eea33084976c832aa4e766b7dff8aedd7587ea44a604cdf",
+                "sha256:29e71c847a35f6e10ca3b5c2990a52ce38b233019d8e858b755ea6ce4dcdd19d",
+                "sha256:4b927c4f19b71e627b13f3db2324e4ae660527143f9e1f2e2fb404f3a187e2ba",
+                "sha256:5b17b1cf5f8354efa3d37c6e28fdfd9c1c1e5122f2cb56dac121ac61baa47cbe",
+                "sha256:6a0848f1aea0d196a7c4f6772197cbe2abc4266f836b0aac76947872cd29b411",
+                "sha256:7efcbcc30b7c654eb6a8c9c9da787a851c18f8ccd4a5a3a95b05c7accfa068d2",
+                "sha256:834ae7540ad3a83199a8da8f9f2d383e3c3d5130a328889e4cc991acc81e87a0",
+                "sha256:b46a6ab20f5c7c1cb949c72c1994a4585d2eaa0be4853f50a03b5031e964fc7c",
+                "sha256:c2de14066c4a38b4ecbbcd55c5cc4b5340eb04f1c5e81da7451ef555859c833f",
+                "sha256:c367ab6c0393d71171123ca5515c61ff62fe09024fa6bf299cd1339dc9456829"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==6.2"
+            "markers": "python_version > '2.7'",
+            "version": "==6.3.2"
         },
         "twine": {
             "hashes": [
                 "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
                 "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
             "version": "==4.0.2"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa",
-                "sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e"
+                "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26",
+                "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
             ],
-            "index": "pypi",
-            "version": "==4.4.0"
+            "markers": "python_version < '3.11'",
+            "version": "==4.6.3"
         },
         "urllib3": {
             "hashes": [
-                "sha256:47cc05d99aaa09c9e72ed5809b60e7ba354e64b59c9c173ac3018642d8bb41fc",
-                "sha256:c083dd0dce68dbfbe1129d5271cb90f9447dea7d52097c6e0126120c521ddea8"
+                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
+                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
             ],
             "index": "pypi",
-            "version": "==1.26.13"
+            "version": "==2.0.3"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
         },
         "wheel": {
             "hashes": [
-                "sha256:965f5259b566725405b05e7cf774052044b1ed30119b5d586b2703aafe8719ac",
-                "sha256:b60533f3f5d530e971d6737ca6d58681ee434818fab630c83a734bb10c083ce8"
+                "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873",
+                "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"
             ],
             "index": "pypi",
-            "version": "==0.38.4"
+            "version": "==0.40.0"
         },
         "zipp": {
             "hashes": [
-                "sha256:83a28fcb75844b5c0cdaf5aa4003c2d728c77e05f5aeabe8e95e56727005fbaa",
-                "sha256:a7a22e05929290a67401440b39690ae6563279bced5f314609d9d03798f56766"
+                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
+                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.11.0"
+            "version": "==3.15.0"
         }
     }
 }
```

### Comparing `django-postgres-copy-2.7.2/README.md` & `django-postgres-copy-2.7.3/README.md`

 * *Files identical despite different names*

### Comparing `django-postgres-copy-2.7.2/django_postgres_copy.egg-info/PKG-INFO` & `django-postgres-copy-2.7.3/django_postgres_copy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-postgres-copy
-Version: 2.7.2
+Version: 2.7.3
 Summary: Quickly import and export delimited data with Django support for PostgreSQL’s COPY command
 Home-page: https://palewi.re/docs/django-postgres-copy/
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: MIT
 Project-URL: Documentation, https://palewi.re/docs/django-postgres-copy/
 Project-URL: Source, https://github.com/palewire/django-postgres-copy
```

### Comparing `django-postgres-copy-2.7.2/django_postgres_copy.egg-info/SOURCES.txt` & `django-postgres-copy-2.7.3/django_postgres_copy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-postgres-copy-2.7.2/docs/Makefile` & `django-postgres-copy-2.7.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-postgres-copy-2.7.2/docs/_static/css/custom.css` & `django-postgres-copy-2.7.3/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `django-postgres-copy-2.7.2/docs/conf.py` & `django-postgres-copy-2.7.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-postgres-copy-2.7.2/docs/index.rst` & `django-postgres-copy-2.7.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-postgres-copy-2.7.2/docs/make.bat` & `django-postgres-copy-2.7.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-postgres-copy-2.7.2/postgres_copy/copy_from.py` & `django-postgres-copy-2.7.3/postgres_copy/copy_from.py`

 * *Files identical despite different names*

### Comparing `django-postgres-copy-2.7.2/postgres_copy/copy_to.py` & `django-postgres-copy-2.7.3/postgres_copy/copy_to.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 logger = logging.getLogger(__name__)
 
 
 class SQLCopyToCompiler(SQLCompiler):
     """
     Custom SQL compiler for creating a COPY TO query (postgres backend only).
     """
-    def setup_query(self):
+    def setup_query(self, **kwargs):
         """
         Extend the default SQLCompiler.setup_query to add re-ordering of items in select.
         """
-        super(SQLCopyToCompiler, self).setup_query()
+        super(SQLCopyToCompiler, self).setup_query(**kwargs)
         if self.query.copy_to_fields:
             self.select = []
             for field in self.query.copy_to_fields:
                 # raises error if field is not available
                 expression = self.query.resolve_ref(field)
                 selection = (
                     expression,
```

### Comparing `django-postgres-copy-2.7.2/postgres_copy/managers.py` & `django-postgres-copy-2.7.3/postgres_copy/managers.py`

 * *Files identical despite different names*

### Comparing `django-postgres-copy-2.7.2/setup.py` & `django-postgres-copy-2.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `django-postgres-copy-2.7.2/tests/models.py` & `django-postgres-copy-2.7.3/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-postgres-copy-2.7.2/tests/tests.py` & `django-postgres-copy-2.7.3/tests/tests.py`

 * *Files identical despite different names*

