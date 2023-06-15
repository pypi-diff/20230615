# Comparing `tmp/cuscom-1.0.0.tar.gz` & `tmp/cuscom-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cuscom-1.0.0.tar", last modified: Mon Jun  5 08:49:10 2023, max compression
+gzip compressed data, was "dist/cuscom-1.0.1.tar", last modified: Thu Jun 15 09:42:10 2023, max compression
```

## Comparing `cuscom-1.0.0.tar` & `cuscom-1.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:49:10.000000 cuscom-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1100 2023-06-05 08:48:50.000000 cuscom-1.0.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-06-05 08:48:50.000000 cuscom-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      495 2023-06-05 08:49:10.000000 cuscom-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-06-05 08:48:50.000000 cuscom-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-05 08:49:00.000000 cuscom-1.0.0/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:49:10.000000 cuscom-1.0.0/cuscom.egg-info/
--rw-r--r--   0 root         (0) root         (0)      495 2023-06-05 08:49:10.000000 cuscom-1.0.0/cuscom.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      548 2023-06-05 08:49:10.000000 cuscom-1.0.0/cuscom.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 08:49:10.000000 cuscom-1.0.0/cuscom.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-06-05 08:49:10.000000 cuscom-1.0.0/cuscom.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-05 08:49:10.000000 cuscom-1.0.0/cuscom.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:49:10.000000 cuscom-1.0.0/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:49:10.000000 cuscom-1.0.0/docs/source/
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-05 08:48:50.000000 cuscom-1.0.0/docs/source/description.rst
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-05 08:48:50.000000 cuscom-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 08:49:10.000000 cuscom-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1209 2023-06-05 08:48:50.000000 cuscom-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:49:10.000000 cuscom-1.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:49:10.000000 cuscom-1.0.0/src/cuscom/
--rw-rw-rw-   0 root         (0) root         (0)      229 2023-06-05 08:48:50.000000 cuscom-1.0.0/src/cuscom/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:49:10.000000 cuscom-1.0.0/src/cuscom/clients/
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-06-05 08:48:50.000000 cuscom-1.0.0/src/cuscom/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1175 2023-06-05 08:48:50.000000 cuscom-1.0.0/src/cuscom/clients/base_client.py
--rw-rw-rw-   0 root         (0) root         (0)      729 2023-06-05 08:48:50.000000 cuscom-1.0.0/src/cuscom/clients/task_client.py
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-06-05 08:48:50.000000 cuscom-1.0.0/src/cuscom/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:49:10.000000 cuscom-1.0.0/src/cuscom/hooks/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-05 08:48:50.000000 cuscom-1.0.0/src/cuscom/hooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-06-05 08:48:50.000000 cuscom-1.0.0/src/cuscom/hooks/slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 08:49:10.000000 cuscom-1.0.0/src/cuscom/operators/
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-05 08:48:50.000000 cuscom-1.0.0/src/cuscom/operators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1334 2023-06-05 08:48:50.000000 cuscom-1.0.0/src/cuscom/operators/custom_kubernetes_pod_operator.py
--rw-rw-rw-   0 root         (0) root         (0)     1663 2023-06-05 08:48:50.000000 cuscom-1.0.0/src/cuscom/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:42:10.000000 cuscom-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1100 2023-06-15 09:41:50.000000 cuscom-1.0.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-06-15 09:41:50.000000 cuscom-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      495 2023-06-15 09:42:10.000000 cuscom-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-06-15 09:41:50.000000 cuscom-1.0.1/README.md
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-15 09:42:01.000000 cuscom-1.0.1/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:42:10.000000 cuscom-1.0.1/cuscom.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      495 2023-06-15 09:42:10.000000 cuscom-1.0.1/cuscom.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      548 2023-06-15 09:42:10.000000 cuscom-1.0.1/cuscom.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 09:42:10.000000 cuscom-1.0.1/cuscom.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-15 09:42:10.000000 cuscom-1.0.1/cuscom.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-15 09:42:10.000000 cuscom-1.0.1/cuscom.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:42:10.000000 cuscom-1.0.1/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:42:10.000000 cuscom-1.0.1/docs/source/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-15 09:41:50.000000 cuscom-1.0.1/docs/source/description.rst
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-15 09:41:50.000000 cuscom-1.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 09:42:10.000000 cuscom-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1209 2023-06-15 09:41:50.000000 cuscom-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:42:10.000000 cuscom-1.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:42:10.000000 cuscom-1.0.1/src/cuscom/
+-rw-rw-rw-   0 root         (0) root         (0)      229 2023-06-15 09:41:50.000000 cuscom-1.0.1/src/cuscom/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:42:10.000000 cuscom-1.0.1/src/cuscom/clients/
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-06-15 09:41:50.000000 cuscom-1.0.1/src/cuscom/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1175 2023-06-15 09:41:50.000000 cuscom-1.0.1/src/cuscom/clients/base_client.py
+-rw-rw-rw-   0 root         (0) root         (0)      729 2023-06-15 09:41:50.000000 cuscom-1.0.1/src/cuscom/clients/task_client.py
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-06-15 09:41:50.000000 cuscom-1.0.1/src/cuscom/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:42:10.000000 cuscom-1.0.1/src/cuscom/hooks/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-15 09:41:50.000000 cuscom-1.0.1/src/cuscom/hooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-06-15 09:41:50.000000 cuscom-1.0.1/src/cuscom/hooks/slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:42:10.000000 cuscom-1.0.1/src/cuscom/operators/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-15 09:41:50.000000 cuscom-1.0.1/src/cuscom/operators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1334 2023-06-15 09:41:50.000000 cuscom-1.0.1/src/cuscom/operators/custom_kubernetes_pod_operator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1725 2023-06-15 09:41:50.000000 cuscom-1.0.1/src/cuscom/utils.py
```

### Comparing `cuscom-1.0.0/LICENSE` & `cuscom-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cuscom-1.0.0/cuscom.egg-info/SOURCES.txt` & `cuscom-1.0.1/cuscom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cuscom-1.0.0/setup.py` & `cuscom-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `cuscom-1.0.0/src/cuscom/clients/base_client.py` & `cuscom-1.0.1/src/cuscom/clients/base_client.py`

 * *Files identical despite different names*

### Comparing `cuscom-1.0.0/src/cuscom/clients/task_client.py` & `cuscom-1.0.1/src/cuscom/clients/task_client.py`

 * *Files identical despite different names*

### Comparing `cuscom-1.0.0/src/cuscom/hooks/slack.py` & `cuscom-1.0.1/src/cuscom/hooks/slack.py`

 * *Files identical despite different names*

### Comparing `cuscom-1.0.0/src/cuscom/operators/custom_kubernetes_pod_operator.py` & `cuscom-1.0.1/src/cuscom/operators/custom_kubernetes_pod_operator.py`

 * *Files identical despite different names*

### Comparing `cuscom-1.0.0/src/cuscom/utils.py` & `cuscom-1.0.1/src/cuscom/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,22 +34,24 @@
 def from_kebab_case_key(d):
     return {k.replace("-", "_"): v for (k, v) in d.items()}
 
 
 def trigger_dag(dag_id, conf, run_id):
     # pylint: disable=unexpected-keyword-arg
     try:
-        run = DagRun(dag_id=dag_id, conf=conf, run_id=run_id, external_trigger=True)
+        run = DagRun(
+            dag_id=dag_id, conf=conf, run_id=run_id, external_trigger=True, run_type="scheduled"
+        )
         session = settings.Session()
         session.add(run)
         log.info("Triggering run %s of dag %s", run_id, dag_id)
         session.commit()
-    except SQLAlchemyError:
+    except SQLAlchemyError as e:
         session.rollback()
-        log.info("Failed to trigger DAG run %s of %s", run_id, dag_id)
+        log.info("Failed to trigger DAG run %s of %s: %s", run_id, dag_id, repr(e))
     finally:
         session.close()
 
 
 def mask(config):
     if config:
         mask_config = config.copy()
```

