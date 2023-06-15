# Comparing `tmp/tutor-jupyter-15.0.2.tar.gz` & `tmp/tutor-jupyter-16.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tutor-jupyter-15.0.2.tar", last modified: Wed May 24 21:11:35 2023, max compression
+gzip compressed data, was "tutor-jupyter-16.0.0.tar", last modified: Thu Jun 15 08:46:19 2023, max compression
```

## Comparing `tutor-jupyter-15.0.2.tar` & `tutor-jupyter-16.0.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/
--rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/LICENSE.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       84 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     6018 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     5117 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/pyproject.toml
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1774 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutor_jupyter.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     6018 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutor_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     1149 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutor_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutor_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       48 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutor_jupyter.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       48 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutor_jupyter.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       13 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutor_jupyter.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutorjupyter/
--rw-r--r--   0 ci        (1000) ci        (1000)       23 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutorjupyter/patches/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/patches/.gitignore
--rw-r--r--   0 ci        (1000) ci        (1000)       78 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/patches/caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)       84 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/patches/dev-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)      297 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/patches/local-docker-compose-jobs-services
--rw-r--r--   0 ci        (1000) ci        (1000)      464 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/patches/local-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)      193 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/patches/openedx-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      176 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/patches/openedx-dockerfile-post-python-requirements
--rw-r--r--   0 ci        (1000) ci        (1000)     4145 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/apps/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/apps/.gitignore
--rw-r--r--   0 ci        (1000) ci        (1000)     4185 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/apps/jupyterhub_config.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/build/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/build/.gitignore
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/build/hub/
--rw-r--r--   0 ci        (1000) ci        (1000)      410 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/build/hub/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/build/lab/
--rw-r--r--   0 ci        (1000) ci        (1000)      838 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/build/lab/Dockerfile
--rw-r--r--   0 ci        (1000) ci        (1000)      295 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/build/lab/config.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/jobs/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/jobs/init/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/jobs/init/.gitignore
--rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/jobs/init/jupyterhub.sh
--rw-r--r--   0 ci        (1000) ci        (1000)      862 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/jobs/init/mysql.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.647487 tutor-jupyter-16.0.0/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       84 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     6018 2023-06-15 08:46:19.644153 tutor-jupyter-16.0.0/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     5117 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/pyproject.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-15 08:46:19.647487 tutor-jupyter-16.0.0/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1774 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.640820 tutor-jupyter-16.0.0/tutor_jupyter.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     6018 2023-06-15 08:46:19.000000 tutor-jupyter-16.0.0/tutor_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     1149 2023-06-15 08:46:19.000000 tutor-jupyter-16.0.0/tutor_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-06-15 08:46:19.000000 tutor-jupyter-16.0.0/tutor_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       48 2023-06-15 08:46:19.000000 tutor-jupyter-16.0.0/tutor_jupyter.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       48 2023-06-15 08:46:19.000000 tutor-jupyter-16.0.0/tutor_jupyter.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       13 2023-06-15 08:46:19.000000 tutor-jupyter-16.0.0/tutor_jupyter.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.640820 tutor-jupyter-16.0.0/tutorjupyter/
+-rw-r--r--   0 ci        (1000) ci        (1000)      175 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.644153 tutor-jupyter-16.0.0/tutorjupyter/patches/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/patches/.gitignore
+-rw-r--r--   0 ci        (1000) ci        (1000)       78 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/patches/caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)       84 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/patches/dev-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      297 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      464 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/patches/local-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      193 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/patches/openedx-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      176 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/patches/openedx-dockerfile-post-python-requirements
+-rw-r--r--   0 ci        (1000) ci        (1000)     4145 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.634153 tutor-jupyter-16.0.0/tutorjupyter/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.637487 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.644153 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/apps/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/apps/.gitignore
+-rw-r--r--   0 ci        (1000) ci        (1000)     4185 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/apps/jupyterhub_config.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.644153 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/build/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/build/.gitignore
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.644153 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/build/hub/
+-rw-r--r--   0 ci        (1000) ci        (1000)      410 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/build/hub/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.644153 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/build/lab/
+-rw-r--r--   0 ci        (1000) ci        (1000)      838 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/build/lab/Dockerfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      295 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/build/lab/config.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.637487 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/jobs/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.644153 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/jobs/init/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/jobs/init/.gitignore
+-rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/jobs/init/jupyterhub.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)      862 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/jobs/init/mysql.sh
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tutor-jupyter-15.0.2/LICENSE.txt` & `tutor-jupyter-16.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-15.0.2/PKG-INFO` & `tutor-jupyter-16.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-jupyter
-Version: 15.0.2
+Version: 16.0.0
 Summary: Jupyter Notebook plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-jupyter
 Author: Overhang.IO
 Maintainer: Régis Behmo
 Maintainer-email: regis@overhang.io
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-jupyter
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 
 Jupyter Notebook plugin for `Tutor <https://docs.tutor.overhang.io>`__
 ======================================================================
 
 This is a plugin for Tutor that makes it easy to integrate `Jupyter <https://jupyter.org/>`__ notebooks in `Open edX <https://openedx.org>`__. It achieves the following:
```

### Comparing `tutor-jupyter-15.0.2/README.rst` & `tutor-jupyter-16.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-15.0.2/setup.py` & `tutor-jupyter-16.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,16 @@
     author="Overhang.IO",
     maintainer="Régis Behmo",
     maintainer_email="regis@overhang.io",
     description="Jupyter Notebook plugin for Tutor",
     long_description=load_readme(),
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
-    python_requires=">=3.7",
-    install_requires=["tutor>=15.0.0,<16.0.0", "tutor-mfe>=15.0.0,<16.0.0"],
+    python_requires=">=3.8",
+    install_requires=["tutor>=16.0.0,<17.0.0", "tutor-mfe>=16.0.0,<17.0.0"],
     entry_points={
         "tutor.plugin.v1": [
             "jupyter = tutorjupyter.plugin"
         ]
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `tutor-jupyter-15.0.2/tutor_jupyter.egg-info/PKG-INFO` & `tutor-jupyter-16.0.0/tutor_jupyter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-jupyter
-Version: 15.0.2
+Version: 16.0.0
 Summary: Jupyter Notebook plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-jupyter
 Author: Overhang.IO
 Maintainer: Régis Behmo
 Maintainer-email: regis@overhang.io
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-jupyter
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 
 Jupyter Notebook plugin for `Tutor <https://docs.tutor.overhang.io>`__
 ======================================================================
 
 This is a plugin for Tutor that makes it easy to integrate `Jupyter <https://jupyter.org/>`__ notebooks in `Open edX <https://openedx.org>`__. It achieves the following:
```

### Comparing `tutor-jupyter-15.0.2/tutor_jupyter.egg-info/SOURCES.txt` & `tutor-jupyter-16.0.0/tutor_jupyter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-15.0.2/tutorjupyter/plugin.py` & `tutor-jupyter-16.0.0/tutorjupyter/plugin.py`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/apps/jupyterhub_config.py` & `tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/apps/jupyterhub_config.py`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/build/lab/Dockerfile` & `tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/build/lab/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/jobs/init/mysql.sh` & `tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/jobs/init/mysql.sh`

 * *Files identical despite different names*

