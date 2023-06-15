# Comparing `tmp/lucidtech-las-cli-9.4.0.tar.gz` & `tmp/lucidtech-las-cli-9.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lucidtech-las-cli-9.4.0.tar", last modified: Mon Feb 27 13:23:42 2023, max compression
+gzip compressed data, was "lucidtech-las-cli-9.5.0.tar", last modified: Fri Apr 21 13:11:35 2023, max compression
```

## Comparing `lucidtech-las-cli-9.4.0.tar` & `lucidtech-las-cli-9.5.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:23:42.983270 lucidtech-las-cli-9.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-02-27 13:23:42.983270 lucidtech-las-cli-9.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:23:42.979270 lucidtech-las-cli-9.4.0/lascli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/lascli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/lascli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/lascli/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:23:42.979270 lucidtech-las-cli-9.4.0/lascli/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/lascli/actions/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:23:42.983270 lucidtech-las-cli-9.4.0/lascli/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/lascli/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/lascli/parser/app_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/lascli/parser/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)    17907 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/lascli/parser/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/lascli/parser/documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/lascli/parser/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/lascli/parser/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/lascli/parser/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/lascli/parser/payment_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/lascli/parser/plans.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/lascli/parser/predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/lascli/parser/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/lascli/parser/transitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/lascli/parser/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/lascli/parser/workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/lascli/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:23:42.983270 lucidtech-las-cli-9.4.0/lucidtech_las_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-02-27 13:23:42.000000 lucidtech-las-cli-9.4.0/lucidtech_las_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-02-27 13:23:42.000000 lucidtech-las-cli-9.4.0/lucidtech_las_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 13:23:42.000000 lucidtech-las-cli-9.4.0/lucidtech_las_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-27 13:23:42.000000 lucidtech-las-cli-9.4.0/lucidtech_las_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-27 13:23:42.000000 lucidtech-las-cli-9.4.0/lucidtech_las_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-27 13:23:42.000000 lucidtech-las-cli-9.4.0/lucidtech_las_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-27 13:23:42.983270 lucidtech-las-cli-9.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-02-27 13:23:33.000000 lucidtech-las-cli-9.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:11:35.333146 lucidtech-las-cli-9.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-21 13:11:35.333146 lucidtech-las-cli-9.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:11:35.333146 lucidtech-las-cli-9.5.0/lascli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/lascli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/lascli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/lascli/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:11:35.333146 lucidtech-las-cli-9.5.0/lascli/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/lascli/actions/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:11:35.333146 lucidtech-las-cli-9.5.0/lascli/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/lascli/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/lascli/parser/app_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/lascli/parser/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17903 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/lascli/parser/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/lascli/parser/deployment_environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/lascli/parser/documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/lascli/parser/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/lascli/parser/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/lascli/parser/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/lascli/parser/payment_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/lascli/parser/plans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/lascli/parser/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/lascli/parser/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/lascli/parser/transitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/lascli/parser/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/lascli/parser/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/lascli/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:11:35.333146 lucidtech-las-cli-9.5.0/lucidtech_las_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-21 13:11:35.000000 lucidtech-las-cli-9.5.0/lucidtech_las_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-21 13:11:35.000000 lucidtech-las-cli-9.5.0/lucidtech_las_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:11:35.000000 lucidtech-las-cli-9.5.0/lucidtech_las_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-21 13:11:35.000000 lucidtech-las-cli-9.5.0/lucidtech_las_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-21 13:11:35.000000 lucidtech-las-cli-9.5.0/lucidtech_las_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 13:11:35.000000 lucidtech-las-cli-9.5.0/lucidtech_las_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-21 13:11:35.333146 lucidtech-las-cli-9.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-21 13:11:24.000000 lucidtech-las-cli-9.5.0/setup.py
```

### Comparing `lucidtech-las-cli-9.4.0/LICENSE.md` & `lucidtech-las-cli-9.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lucidtech-las-cli-9.4.0/PKG-INFO` & `lucidtech-las-cli-9.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lucidtech-las-cli
-Version: 9.4.0
+Version: 9.5.0
 Summary: CLI for Lucidtech AI Services
 Home-page: https://github.com/LucidtechAI/las-cli
 Author: Lucidtech
 Author-email: hello@lucidtech.ai
 Maintainer: Magnus Aarskaug Rud
 Maintainer-email: magnus@lucidtech.ai
 License: Apache 2.0
```

### Comparing `lucidtech-las-cli-9.4.0/README.md` & `lucidtech-las-cli-9.5.0/README.md`

 * *Files identical despite different names*

### Comparing `lucidtech-las-cli-9.4.0/lascli/__main__.py` & `lucidtech-las-cli-9.5.0/lascli/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from .__version__ import __version__
 from .util import NotProvided
 from .parser import (
     create_app_clients_parser,
     create_assets_parser,
     create_datasets_parser,
+    create_deployment_environments_parser,
     create_documents_parser,
     create_logs_parser,
     create_models_parser,
     create_organizations_parser,
     create_payment_methods_parser,
     create_plans_parser,
     create_predictions_parser,
@@ -44,14 +45,15 @@
     parser.add_argument('--verbose', '-v', action='count', default=0)
     parser.add_argument('--version', action='version', version=f'%(prog)s {__version__}')
     subparsers = parser.add_subparsers()
 
     create_app_clients_parser(subparsers)
     create_assets_parser(subparsers)
     create_datasets_parser(subparsers)
+    create_deployment_environments_parser(subparsers)
     create_documents_parser(subparsers)
     create_logs_parser(subparsers)
     create_models_parser(subparsers)
     create_organizations_parser(subparsers)
     create_payment_methods_parser(subparsers)
     create_plans_parser(subparsers)
     create_predictions_parser(subparsers)
```

### Comparing `lucidtech-las-cli-9.4.0/lascli/actions/workflows.py` & `lucidtech-las-cli-9.5.0/lascli/actions/workflows.py`

 * *Files identical despite different names*

### Comparing `lucidtech-las-cli-9.4.0/lascli/parser/__init__.py` & `lucidtech-las-cli-9.5.0/lascli/parser/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .app_clients import create_app_clients_parser
 from .assets import create_assets_parser
 from .datasets import create_datasets_parser
+from .deployment_environments import create_deployment_environments_parser
 from .documents import create_documents_parser
 from .logs import create_logs_parser
 from .models import create_models_parser
 from .organizations import create_organizations_parser
 from .payment_methods import create_payment_methods_parser
 from .plans import create_plans_parser
 from .predictions import create_predictions_parser
```

### Comparing `lucidtech-las-cli-9.4.0/lascli/parser/app_clients.py` & `lucidtech-las-cli-9.5.0/lascli/parser/app_clients.py`

 * *Files identical despite different names*

### Comparing `lucidtech-las-cli-9.4.0/lascli/parser/assets.py` & `lucidtech-las-cli-9.5.0/lascli/parser/assets.py`

 * *Files identical despite different names*

### Comparing `lucidtech-las-cli-9.4.0/lascli/parser/datasets.py` & `lucidtech-las-cli-9.5.0/lascli/parser/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -366,15 +366,15 @@
 
     create_dataset_parser = subparsers.add_parser('create')
     create_dataset_parser.add_argument('--description')
     create_dataset_parser.add_argument('--name')
     create_dataset_parser.add_argument(
         '--metadata',
         type=json_path,
-        help='path to json file with whatever you need, maximum limit 4kB',
+        help='path to json file with custom metadata, maximum limit 4kB',
     )
     create_dataset_parser.set_defaults(cmd=post_datasets)
 
     list_datasets_parser = subparsers.add_parser('list')
     list_datasets_parser.add_argument('--max-results', '-m', type=int, default=None)
     list_datasets_parser.add_argument('--next-token', '-n', default=None)
     list_datasets_parser.set_defaults(cmd=list_datasets)
@@ -386,15 +386,15 @@
     update_dataset_parser = subparsers.add_parser('update')
     update_dataset_parser.add_argument('dataset_id')
     update_dataset_parser.add_argument('--name', type=nullable(str), default=NotProvided)
     update_dataset_parser.add_argument('--description', type=nullable(str), default=NotProvided)
     update_dataset_parser.add_argument(
         '--metadata',
         type=json_path,
-        help='path to json file with whatever you need, maximum limit 4kB',
+        help='path to json file with custom metadata, maximum limit 4kB',
     )
     update_dataset_parser.set_defaults(cmd=update_dataset)
 
     delete_dataset_parser = subparsers.add_parser('delete')
     delete_dataset_parser.add_argument('dataset_id')
     delete_dataset_parser.add_argument('--delete-documents', action='store_true', default=False)
     delete_dataset_parser.set_defaults(cmd=delete_dataset)
```

### Comparing `lucidtech-las-cli-9.4.0/lascli/parser/documents.py` & `lucidtech-las-cli-9.5.0/lascli/parser/documents.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     create_document_parser.add_argument('document_path')
     create_document_parser.add_argument('--content-type')
     create_document_parser.add_argument('--consent-id')
     create_document_parser.add_argument('--dataset-id')
     create_document_parser.add_argument(
         '--metadata',
         type=json_path,
-        help='path to json file with whatever you need, maximum limit 4kB',
+        help='path to json file with custom metadata, maximum limit 4kB',
     )
     create_document_ground_truth_group = create_document_parser.add_mutually_exclusive_group(required=False)
     create_document_ground_truth_group.add_argument('--ground-truth-fields', metavar='KEY=VALUE', nargs='+')
     create_document_ground_truth_group.add_argument('--ground-truth-path', type=str, help='Path to JSON file')
     create_document_parser.set_defaults(cmd=create_document)
 
     update_document_parser = subparsers.add_parser('update')
@@ -135,15 +135,15 @@
     update_document_parser.add_argument('--dataset-id')
     update_document_ground_truth_group = update_document_parser.add_mutually_exclusive_group(required=False)
     update_document_ground_truth_group.add_argument('--ground-truth-fields', metavar='KEY=VALUE', nargs='+')
     update_document_ground_truth_group.add_argument('--ground-truth-path', type=str, help='Path to JSON file')
     update_document_parser.add_argument(
         '--metadata',
         type=json_path,
-        help='path to json file with whatever you need, maximum limit 4kB',
+        help='path to json file with custom metadata, maximum limit 4kB',
     )
     update_document_parser.set_defaults(cmd=update_document)
 
     delete_document_parser = subparsers.add_parser('delete')
     delete_document_parser.add_argument('document_id')
     delete_document_parser.set_defaults(cmd=delete_document)
```

### Comparing `lucidtech-las-cli-9.4.0/lascli/parser/logs.py` & `lucidtech-las-cli-9.5.0/lascli/parser/logs.py`

 * *Files identical despite different names*

### Comparing `lucidtech-las-cli-9.4.0/lascli/parser/organizations.py` & `lucidtech-las-cli-9.5.0/lascli/parser/organizations.py`

 * *Files identical despite different names*

### Comparing `lucidtech-las-cli-9.4.0/lascli/parser/payment_methods.py` & `lucidtech-las-cli-9.5.0/lascli/parser/payment_methods.py`

 * *Files identical despite different names*

### Comparing `lucidtech-las-cli-9.4.0/lascli/parser/plans.py` & `lucidtech-las-cli-9.5.0/lascli/parser/plans.py`

 * *Files identical despite different names*

### Comparing `lucidtech-las-cli-9.4.0/lascli/parser/predictions.py` & `lucidtech-las-cli-9.5.0/lascli/parser/predictions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 import textwrap
 from argparse import RawTextHelpFormatter
 
 from las import Client
 
+from lascli.util import json_or_json_path
+
 
 def post_predictions(las_client: Client, document_id, model_id, **optional_args):
     return las_client.create_prediction(document_id, model_id, **optional_args)
 
 
 def list_predictions(las_client: Client, **optional_args):
     return las_client.list_predictions(**optional_args)
@@ -21,16 +23,16 @@
     create_predicton_parser.add_argument('document_id')
     create_predicton_parser.add_argument('model_id', help='Id of model to use for predictions')
     create_predicton_parser.add_argument('--training-id', help='Id of training to use for predictions')
     create_predicton_parser.add_argument('--auto-rotate', action='store_true', default=False)
     create_predicton_parser.add_argument('--max-pages', type=int)
     create_predicton_parser.add_argument('--rotation', type=int)
     create_predicton_parser.add_argument('--image-quality', type=str, choices={'LOW', 'HIGH'})
-    create_predicton_parser.add_argument('--postprocess-config', type=json.loads, help=textwrap.dedent('''
-        Post processing configuration for predictions
+    create_predicton_parser.add_argument('--postprocess-config', type=json_or_json_path, help=textwrap.dedent('''
+        Path or inline JSON with the post processing configuration for this prediction
         {
             "strategy": "BEST_FIRST" | "BEST_N_PAGES",  (required)
             "parameters": {                             (required if strategy=BEST_N_PAGES, omit otherwise)
                 "n": int,                               (required if strategy=BEST_N_PAGES, omit otherwise)
                 "collapse": true | false (default)      (optional if strategy=BEST_N_PAGES, omit otherwise)
             }
         }
```

### Comparing `lucidtech-las-cli-9.4.0/lascli/parser/secrets.py` & `lucidtech-las-cli-9.5.0/lascli/parser/secrets.py`

 * *Files identical despite different names*

### Comparing `lucidtech-las-cli-9.4.0/lascli/parser/transitions.py` & `lucidtech-las-cli-9.5.0/lascli/parser/transitions.py`

 * *Files identical despite different names*

### Comparing `lucidtech-las-cli-9.4.0/lascli/parser/users.py` & `lucidtech-las-cli-9.5.0/lascli/parser/users.py`

 * *Files identical despite different names*

### Comparing `lucidtech-las-cli-9.4.0/lascli/parser/workflows.py` & `lucidtech-las-cli-9.5.0/lascli/parser/workflows.py`

 * *Files identical despite different names*

### Comparing `lucidtech-las-cli-9.4.0/lascli/util.py` & `lucidtech-las-cli-9.5.0/lascli/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,24 +28,39 @@
     except:
         if error_msg:
             print(error_msg)
 
         raise
     finally:
         print(end_msg)
-    
+
 
 def capture_return(dest: list):
     def inner(f):
         @contextlib.wraps(f)
         def wrapper(*args, **kwargs):
-            nonlocal dest 
+            nonlocal dest
 
             val = f(*args, **kwargs)
             dest += val if isinstance(val, (list, tuple)) else [val]
             return val
-    
+
         return wrapper
 
     return inner
 
 
+def json_or_json_path(value):
+    if not value:
+        return
+
+    try:
+        return json.loads(value)
+    except json.JSONDecodeError:
+        pass
+
+    try:
+        return json.loads(Path(value).read_text())
+    except (json.JSONDecodeError, FileNotFoundError):
+        pass
+
+    raise Exception('Could not interpret input as neither JSON nor a path containing JSON')
```

### Comparing `lucidtech-las-cli-9.4.0/lucidtech_las_cli.egg-info/PKG-INFO` & `lucidtech-las-cli-9.5.0/lucidtech_las_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lucidtech-las-cli
-Version: 9.4.0
+Version: 9.5.0
 Summary: CLI for Lucidtech AI Services
 Home-page: https://github.com/LucidtechAI/las-cli
 Author: Lucidtech
 Author-email: hello@lucidtech.ai
 Maintainer: Magnus Aarskaug Rud
 Maintainer-email: magnus@lucidtech.ai
 License: Apache 2.0
```

### Comparing `lucidtech-las-cli-9.4.0/lucidtech_las_cli.egg-info/SOURCES.txt` & `lucidtech-las-cli-9.5.0/lucidtech_las_cli.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 lascli/__version__.py
 lascli/util.py
 lascli/actions/workflows.py
 lascli/parser/__init__.py
 lascli/parser/app_clients.py
 lascli/parser/assets.py
 lascli/parser/datasets.py
+lascli/parser/deployment_environments.py
 lascli/parser/documents.py
 lascli/parser/logs.py
 lascli/parser/models.py
 lascli/parser/organizations.py
 lascli/parser/payment_methods.py
 lascli/parser/plans.py
 lascli/parser/predictions.py
```

### Comparing `lucidtech-las-cli-9.4.0/setup.py` & `lucidtech-las-cli-9.5.0/setup.py`

 * *Files identical despite different names*

