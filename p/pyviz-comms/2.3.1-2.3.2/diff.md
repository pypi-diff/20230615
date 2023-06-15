# Comparing `tmp/pyviz_comms-2.3.1.tar.gz` & `tmp/pyviz_comms-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyviz_comms-2.3.1.tar", last modified: Thu Jun  8 14:10:12 2023, max compression
+gzip compressed data, was "dist/pyviz_comms-2.3.2.tar", last modified: Thu Jun 15 14:20:30 2023, max compression
```

## Comparing `pyviz_comms-2.3.1.tar` & `pyviz_comms-2.3.2.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/install.json
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/
--rw-r--r--   0 runner    (1001) docker     (123)    19946 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/pyviz_comms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/pyviz_comms/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/schemas/@pyviz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-08 14:10:10.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/package.json.orig
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-08 14:10:10.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/static/445.8dcc8508e7796b2d5680.js
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/static/747.0551e937e8f929740f5d.js
--rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/static/remoteEntry.75aa6a6489839cbfc067.js
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-08 14:10:10.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/pyviz_comms/notebook.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/pyviz_comms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/pyviz_comms/tests/test_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/src/icons.ts
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/src/manager.ts
--rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/src/plugin.ts
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/src/preview.tsx
--rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/src/renderer.ts
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/src/svg.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:20:30.000000 pyviz_comms-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-15 14:06:55.000000 pyviz_comms-2.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-15 14:06:55.000000 pyviz_comms-2.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-15 14:20:30.000000 pyviz_comms-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-15 14:06:55.000000 pyviz_comms-2.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-15 14:06:55.000000 pyviz_comms-2.3.2/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-15 14:06:55.000000 pyviz_comms-2.3.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-15 14:06:55.000000 pyviz_comms-2.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:20:30.000000 pyviz_comms-2.3.2/pyviz_comms/
+-rw-r--r--   0 runner    (1001) docker     (123)    19946 2023-06-15 14:06:55.000000 pyviz_comms-2.3.2/pyviz_comms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-15 14:06:55.000000 pyviz_comms-2.3.2/pyviz_comms/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:20:30.000000 pyviz_comms-2.3.2/pyviz_comms/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-15 14:20:29.000000 pyviz_comms-2.3.2/pyviz_comms/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:20:30.000000 pyviz_comms-2.3.2/pyviz_comms/labextension/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:20:30.000000 pyviz_comms-2.3.2/pyviz_comms/labextension/schemas/@pyviz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:20:30.000000 pyviz_comms-2.3.2/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-15 14:20:26.000000 pyviz_comms-2.3.2/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/package.json.orig
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-15 14:20:26.000000 pyviz_comms-2.3.2/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:20:30.000000 pyviz_comms-2.3.2/pyviz_comms/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20476 2023-06-15 14:20:29.000000 pyviz_comms-2.3.2/pyviz_comms/labextension/static/47.700864e51bfa92f76faf.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43380 2023-06-15 14:20:29.000000 pyviz_comms-2.3.2/pyviz_comms/labextension/static/479.f8613002a4a279797a83.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-15 14:20:29.000000 pyviz_comms-2.3.2/pyviz_comms/labextension/static/747.0551e937e8f929740f5d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-06-15 14:20:29.000000 pyviz_comms-2.3.2/pyviz_comms/labextension/static/remoteEntry.936b971eda36f85d6cca.js
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-15 14:20:26.000000 pyviz_comms-2.3.2/pyviz_comms/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-15 14:20:29.000000 pyviz_comms-2.3.2/pyviz_comms/labextension/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-06-15 14:06:55.000000 pyviz_comms-2.3.2/pyviz_comms/notebook.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:20:30.000000 pyviz_comms-2.3.2/pyviz_comms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:06:55.000000 pyviz_comms-2.3.2/pyviz_comms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-06-15 14:06:55.000000 pyviz_comms-2.3.2/pyviz_comms/tests/test_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:20:30.000000 pyviz_comms-2.3.2/pyviz_comms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-15 14:20:29.000000 pyviz_comms-2.3.2/pyviz_comms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-15 14:20:29.000000 pyviz_comms-2.3.2/pyviz_comms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:20:29.000000 pyviz_comms-2.3.2/pyviz_comms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-15 14:20:29.000000 pyviz_comms-2.3.2/pyviz_comms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 14:20:29.000000 pyviz_comms-2.3.2/pyviz_comms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 14:20:30.000000 pyviz_comms-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-15 14:06:55.000000 pyviz_comms-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:20:30.000000 pyviz_comms-2.3.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-15 14:06:55.000000 pyviz_comms-2.3.2/src/icons.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 14:06:55.000000 pyviz_comms-2.3.2/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-15 14:06:55.000000 pyviz_comms-2.3.2/src/manager.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-06-15 14:06:55.000000 pyviz_comms-2.3.2/src/plugin.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-15 14:06:55.000000 pyviz_comms-2.3.2/src/preview.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-06-15 14:06:55.000000 pyviz_comms-2.3.2/src/renderer.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-15 14:06:55.000000 pyviz_comms-2.3.2/src/svg.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-15 14:06:55.000000 pyviz_comms-2.3.2/tsconfig.json
```

### Comparing `pyviz_comms-2.3.1/LICENSE.txt` & `pyviz_comms-2.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.3.1/PKG-INFO` & `pyviz_comms-2.3.2/pyviz_comms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyviz_comms
-Version: 2.3.1
+Name: pyviz-comms
+Version: 2.3.2
 Summary: Bidirectional communication for the HoloViz ecosystem.
 Home-page: https://holoviz.org
 Author: Philipp Rudiger
 Author-email: philipp.jfr@gmail.com
 Maintainer: HoloViz
 Maintainer-email: developers@holoviz.org
 License: BSD
```

### Comparing `pyviz_comms-2.3.1/README.md` & `pyviz_comms-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.3.1/package.json` & `pyviz_comms-2.3.2/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9742063492063493%*

 * *Differences: {"'dependencies'": "{'tippy.js': '^6'}", "'version'": "'2.3.2'"}*

```diff
@@ -10,15 +10,16 @@
         "@jupyterlab/docregistry": "^3.1.0",
         "@jupyterlab/fileeditor": "^3.1.0",
         "@jupyterlab/mainmenu": "^3.1.0",
         "@jupyterlab/notebook": "^3.1.0",
         "@jupyterlab/settingregistry": "^3.1.0",
         "@jupyterlab/ui-components": "^3.1.0",
         "@lumino/coreutils": "^1.5.3",
-        "@lumino/signaling": "^1.4.3"
+        "@lumino/signaling": "^1.4.3",
+        "tippy.js": "^6"
     },
     "description": "A JupyterLab extension for rendering HoloViz content.",
     "devDependencies": {
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6",
         "@jupyter-widgets/jupyterlab-manager": "^5.0.7",
         "@jupyterlab/builder": "^3.0.0",
         "@jupyterlab/testutils": "^3.0.0",
@@ -98,9 +99,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.3.1"
+    "version": "2.3.2"
 }
```

### Comparing `pyviz_comms-2.3.1/pyviz_comms/__init__.py` & `pyviz_comms-2.3.2/pyviz_comms/__init__.py`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.3.1/pyviz_comms/labextension/package.json` & `pyviz_comms-2.3.2/pyviz_comms/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9738095238095239%*

 * *Differences: {"'dependencies'": "{'tippy.js': '^6'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.936b971eda36f85d6cca.js'}}",*

 * * "'version'": "'2.3.2'"}*

```diff
@@ -10,15 +10,16 @@
         "@jupyterlab/docregistry": "^3.1.0",
         "@jupyterlab/fileeditor": "^3.1.0",
         "@jupyterlab/mainmenu": "^3.1.0",
         "@jupyterlab/notebook": "^3.1.0",
         "@jupyterlab/settingregistry": "^3.1.0",
         "@jupyterlab/ui-components": "^3.1.0",
         "@lumino/coreutils": "^1.5.3",
-        "@lumino/signaling": "^1.4.3"
+        "@lumino/signaling": "^1.4.3",
+        "tippy.js": "^6"
     },
     "description": "A JupyterLab extension for rendering HoloViz content.",
     "devDependencies": {
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6",
         "@jupyter-widgets/jupyterlab-manager": "^5.0.7",
         "@jupyterlab/builder": "^3.0.0",
         "@jupyterlab/testutils": "^3.0.0",
@@ -40,15 +41,15 @@
         "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/holoviz/pyviz_comms",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.75aa6a6489839cbfc067.js",
+            "load": "static/remoteEntry.936b971eda36f85d6cca.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "pyviz_comms/labextension",
         "schemaDir": "schema",
         "sharedPackages": {
             "@jupyter-widgets/base": {
@@ -103,9 +104,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.3.1"
+    "version": "2.3.2"
 }
```

### Comparing `pyviz_comms-2.3.1/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/package.json.orig` & `pyviz_comms-2.3.2/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/package.json.orig`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9742063492063493%*

 * *Differences: {"'dependencies'": "{'tippy.js': '^6'}", "'version'": "'2.3.2'"}*

```diff
@@ -10,15 +10,16 @@
         "@jupyterlab/docregistry": "^3.1.0",
         "@jupyterlab/fileeditor": "^3.1.0",
         "@jupyterlab/mainmenu": "^3.1.0",
         "@jupyterlab/notebook": "^3.1.0",
         "@jupyterlab/settingregistry": "^3.1.0",
         "@jupyterlab/ui-components": "^3.1.0",
         "@lumino/coreutils": "^1.5.3",
-        "@lumino/signaling": "^1.4.3"
+        "@lumino/signaling": "^1.4.3",
+        "tippy.js": "^6"
     },
     "description": "A JupyterLab extension for rendering HoloViz content.",
     "devDependencies": {
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6",
         "@jupyter-widgets/jupyterlab-manager": "^5.0.7",
         "@jupyterlab/builder": "^3.0.0",
         "@jupyterlab/testutils": "^3.0.0",
@@ -98,9 +99,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.3.1"
+    "version": "2.3.2"
 }
```

### Comparing `pyviz_comms-2.3.1/pyviz_comms/labextension/static/747.0551e937e8f929740f5d.js` & `pyviz_comms-2.3.2/pyviz_comms/labextension/static/747.0551e937e8f929740f5d.js`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.3.1/pyviz_comms/labextension/static/remoteEntry.75aa6a6489839cbfc067.js` & `pyviz_comms-2.3.2/pyviz_comms/labextension/static/remoteEntry.936b971eda36f85d6cca.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, l, s, d, p, f, c, v, h, y, b, g, m, j, w, S = {
+    var e, r, t, n, a, o, i, u, l, f, d, s, p, c, v, h, y, b, g, m, j, w, S, _ = {
             281: (e, r, t) => {
                 var n = {
-                        "./index": () => t.e(445).then((() => () => t(445))),
-                        "./extension": () => t.e(445).then((() => () => t(445))),
+                        "./index": () => t.e(47).then((() => () => t(47))),
+                        "./extension": () => t.e(47).then((() => () => t(47))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
@@ -21,113 +21,116 @@
                     };
                 t.d(r, {
                     get: () => a,
                     init: () => o
                 })
             }
         },
-        _ = {};
+        k = {};
 
-    function k(e) {
-        var r = _[e];
+    function E(e) {
+        var r = k[e];
         if (void 0 !== r) return r.exports;
-        var t = _[e] = {
+        var t = k[e] = {
             id: e,
             exports: {}
         };
-        return S[e](t, t.exports, k), t.exports
+        return _[e](t, t.exports, E), t.exports
     }
-    k.m = S, k.c = _, k.n = e => {
+    E.m = _, E.c = k, E.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return k.d(r, {
+        return E.d(r, {
             a: r
         }), r
-    }, k.d = (e, r) => {
-        for (var t in r) k.o(r, t) && !k.o(e, t) && Object.defineProperty(e, t, {
+    }, E.d = (e, r) => {
+        for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, k.f = {}, k.e = e => Promise.all(Object.keys(k.f).reduce(((r, t) => (k.f[t](e, r), r)), [])), k.u = e => e + "." + {
-        445: "8dcc8508e7796b2d5680",
+    }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
+        47: "700864e51bfa92f76faf",
+        479: "f8613002a4a279797a83",
         747: "0551e937e8f929740f5d"
     } [e] + ".js?v=" + {
-        445: "8dcc8508e7796b2d5680",
+        47: "700864e51bfa92f76faf",
+        479: "f8613002a4a279797a83",
         747: "0551e937e8f929740f5d"
-    } [e], k.g = function() {
+    } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), k.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@pyviz/jupyterlab_pyviz:", k.l = (t, n, a, o) => {
+    }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@pyviz/jupyterlab_pyviz:", E.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== a)
-                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var d = l[s];
+                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
+                    var d = l[f];
                     if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + a) {
                         i = d;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, k.nc && i.setAttribute("nonce", k.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var p = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(f);
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
+            var s = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(p);
                     var a = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                f = setTimeout(p.bind(null, void 0, {
+                p = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = p.bind(null, i.onerror), i.onload = p.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, k.r = e => {
+    }, E.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        k.S = {};
+        E.S = {};
         var e = {},
             r = {};
-        k.I = (t, n) => {
+        E.I = (t, n) => {
             n || (n = []);
             var a = r[t];
             if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
                 if (n.push(a), e[t]) return e[t];
-                k.o(k.S, t) || (k.S[t] = {});
-                var o = k.S[t],
+                E.o(E.S, t) || (E.S[t] = {});
+                var o = E.S[t],
                     i = "@pyviz/jupyterlab_pyviz",
-                    u = [];
-                return "default" === t && ((e, r, t, n) => {
-                    var a = o[e] = o[e] || {},
-                        u = a[r];
-                    (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (a[r] = {
-                        get: () => k.e(445).then((() => () => k(445))),
-                        from: i,
-                        eager: !1
-                    })
-                })("@pyviz/jupyterlab_pyviz", "2.3.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                    u = (e, r, t, n) => {
+                        var a = o[e] = o[e] || {},
+                            u = a[r];
+                        (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (a[r] = {
+                            get: t,
+                            from: i,
+                            eager: !!n
+                        })
+                    },
+                    l = [];
+                return "default" === t && (u("@pyviz/jupyterlab_pyviz", "2.3.2", (() => E.e(47).then((() => () => E(47))))), u("tippy.js", "6.3.7", (() => E.e(479).then((() => () => E(479)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        k.g.importScripts && (e = k.g.location + "");
-        var r = k.g.document;
+        E.g.importScripts && (e = E.g.location + "");
+        var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             if (t.length)
                 for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), k.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), E.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -164,136 +167,140 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 a = n < 0;
             a && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, d, p = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !l || ("u" == p ? u > n && !a : "" == p != a);
+                var f, d, s = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !l || ("u" == s ? u > n && !a : "" == s != a);
                 if ("u" == d) {
-                    if (!l || "u" != p) return !1
+                    if (!l || "u" != s) return !1
                 } else if (l)
-                    if (p == d)
+                    if (s == d)
                         if (u <= n) {
-                            if (s != e[u]) return !1
+                            if (f != e[u]) return !1
                         } else {
-                            if (a ? s > e[u] : s < e[u]) return !1;
-                            s != e[u] && (l = !1)
+                            if (a ? f > e[u] : f < e[u]) return !1;
+                            f != e[u] && (l = !1)
                         }
-                else if ("s" != p && "n" != p) {
+                else if ("s" != s && "n" != s) {
                     if (a || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || d < p != a) return !1;
+                    if (u <= n || d < s != a) return !1;
                     l = !1
-                } else "s" != p && "n" != p && (l = !1, u--)
+                } else "s" != s && "n" != s && (l = !1, u--)
             }
         }
-        var f = [],
-            c = f.pop.bind(f);
+        var p = [],
+            c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var v = e[i];
-            f.push(1 == v ? c() | c() : 2 == v ? c() & c() : v ? o(v, r) : !c())
+            p.push(1 == v ? c() | c() : 2 == v ? c() & c() : v ? o(v, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
-        var t = k.S[e];
-        if (!t || !k.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = E.S[e];
+        if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", d = (e, r, t, n) => {
+    }, f = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", d = (e, r, t, n) => {
         var a = l(e, t);
-        return o(n, a) || c(s(e, t, a, n)), h(e[t][a])
-    }, p = (e, r, t) => {
+        return o(n, a) || c(f(e, t, a, n)), h(e[t][a])
+    }, s = (e, r, t) => {
         var a = e[r];
         return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
-    }, f = (e, r, t, n) => {
+    }, p = (e, r, t, n) => {
         var o = e[t];
         return "No satisfying version (" + a(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
     }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, v = (e, r, t, n) => {
-        c(f(e, r, t, n))
+        c(p(e, r, t, n))
     }, h = e => (e.loaded = 1, e.get()), b = (y = e => function(r, t, n, a) {
-        var o = k.I(r);
-        return o && o.then ? o.then(e.bind(e, r, k.S[r], t, n, a)) : e(r, k.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), h(p(r, t, n) || v(r, e, t, n) || u(r, t))))), g = y(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), m = {}, j = {
+        var o = E.I(r);
+        return o && o.then ? o.then(e.bind(e, r, E.S[r], t, n, a)) : e(r, E.S[r], t, n, a)
+    })(((e, r, t, n) => (i(e, t), h(s(r, t, n) || v(r, e, t, n) || u(r, t))))), g = y(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), m = y(((e, r, t, n, a) => {
+        var o = r && E.o(r, t) && s(r, t, n);
+        return o ? h(o) : a()
+    })), j = {}, w = {
         58: () => g("default", "@jupyterlab/coreutils", [1, 5, 6, 4]),
         85: () => g("default", "@jupyterlab/settingregistry", [1, 3, 6, 4]),
         175: () => g("default", "@jupyterlab/application", [1, 3, 6, 4]),
+        181: () => m("default", "tippy.js", [1, 6], (() => E.e(479).then((() => () => E(479))))),
         263: () => g("default", "@jupyterlab/docmanager", [1, 3, 6, 4]),
         271: () => g("default", "react", [1, 17, 0, 1]),
         294: () => g("default", "@jupyter-widgets/jupyterlab-manager", [1, 5, 0, 4]),
-        308: () => g("default", "@jupyterlab/mainmenu", [1, 3, 6, 4]),
+        312: () => g("default", "@jupyterlab/mainmenu", [1, 3, 6, 4]),
         526: () => g("default", "@lumino/coreutils", [1, 1, 11, 0]),
         667: () => g("default", "@jupyterlab/ui-components", [1, 3, 6, 4]),
         676: () => b("default", "@jupyterlab/docregistry", [1, 3, 6, 4]),
         764: () => g("default", "@jupyterlab/apputils", [1, 3, 6, 4]),
         779: () => g("default", "@jupyterlab/notebook", [1, 3, 6, 4]),
         832: () => g("default", "@lumino/widgets", [1, 1, 37, 2]),
         840: () => g("default", "@lumino/signaling", [1, 1, 10, 0]),
         923: () => g("default", "@lumino/disposable", [1, 1, 10, 0])
-    }, w = {
-        445: [58, 85, 175, 263, 271, 294, 308, 526, 667, 676, 764, 779, 832, 840, 923]
-    }, k.f.consumes = (e, r) => {
-        k.o(w, e) && w[e].forEach((e => {
-            if (k.o(m, e)) return r.push(m[e]);
+    }, S = {
+        47: [58, 85, 175, 181, 263, 271, 294, 312, 526, 667, 676, 764, 779, 832, 840, 923]
+    }, E.f.consumes = (e, r) => {
+        E.o(S, e) && S[e].forEach((e => {
+            if (E.o(j, e)) return r.push(j[e]);
             var t = r => {
-                    m[e] = 0, k.m[e] = t => {
-                        delete k.c[e], t.exports = r()
+                    j[e] = 0, E.m[e] = t => {
+                        delete E.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete m[e], k.m[e] = t => {
-                        throw delete k.c[e], r
+                    delete j[e], E.m[e] = t => {
+                        throw delete E.c[e], r
                     }
                 };
             try {
-                var a = j[e]();
-                a.then ? r.push(m[e] = a.then(t).catch(n)) : t(a)
+                var a = w[e]();
+                a.then ? r.push(j[e] = a.then(t).catch(n)) : t(a)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             924: 0
         };
-        k.f.j = (r, t) => {
-            var n = k.o(e, r) ? e[r] : void 0;
+        E.f.j = (r, t) => {
+            var n = E.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var a = new Promise(((t, a) => n = e[r] = [t, a]));
                     t.push(n[2] = a);
-                    var o = k.p + k.u(r),
+                    var o = E.p + E.u(r),
                         i = new Error;
-                    k.l(o, (t => {
-                        if (k.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                    E.l(o, (t => {
+                        if (E.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var a = t && ("load" === t.type ? "missing" : t.type),
                                 o = t && t.target && t.target.src;
                             i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, a, [o, i, u] = t,
                     l = 0;
                 if (o.some((r => 0 !== e[r]))) {
-                    for (n in i) k.o(i, n) && (k.m[n] = i[n]);
-                    u && u(k)
+                    for (n in i) E.o(i, n) && (E.m[n] = i[n]);
+                    u && u(E)
                 }
-                for (r && r(t); l < o.length; l++) a = o[l], k.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); l < o.length; l++) a = o[l], E.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunk_pyviz_jupyterlab_pyviz = self.webpackChunk_pyviz_jupyterlab_pyviz || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), k.nc = void 0;
-    var E = k(281);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@pyviz/jupyterlab_pyviz"] = E
+    })(), E.nc = void 0;
+    var z = E(281);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@pyviz/jupyterlab_pyviz"] = z
 })();
```

### Comparing `pyviz_comms-2.3.1/pyviz_comms/notebook.js` & `pyviz_comms-2.3.2/pyviz_comms/notebook.js`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.3.1/pyviz_comms/tests/test_extension.py` & `pyviz_comms-2.3.2/pyviz_comms/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.3.1/pyviz_comms.egg-info/PKG-INFO` & `pyviz_comms-2.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyviz-comms
-Version: 2.3.1
+Name: pyviz_comms
+Version: 2.3.2
 Summary: Bidirectional communication for the HoloViz ecosystem.
 Home-page: https://holoviz.org
 Author: Philipp Rudiger
 Author-email: philipp.jfr@gmail.com
 Maintainer: HoloViz
 Maintainer-email: developers@holoviz.org
 License: BSD
```

### Comparing `pyviz_comms-2.3.1/pyviz_comms.egg-info/SOURCES.txt` & `pyviz_comms-2.3.2/pyviz_comms.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 pyviz_comms.egg-info/SOURCES.txt
 pyviz_comms.egg-info/dependency_links.txt
 pyviz_comms.egg-info/requires.txt
 pyviz_comms.egg-info/top_level.txt
 pyviz_comms/labextension/package.json
 pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/package.json.orig
 pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/plugin.json
-pyviz_comms/labextension/static/445.8dcc8508e7796b2d5680.js
+pyviz_comms/labextension/static/47.700864e51bfa92f76faf.js
+pyviz_comms/labextension/static/479.f8613002a4a279797a83.js
 pyviz_comms/labextension/static/747.0551e937e8f929740f5d.js
-pyviz_comms/labextension/static/remoteEntry.75aa6a6489839cbfc067.js
+pyviz_comms/labextension/static/remoteEntry.936b971eda36f85d6cca.js
 pyviz_comms/labextension/static/style.js
 pyviz_comms/labextension/static/third-party-licenses.json
 pyviz_comms/tests/__init__.py
 pyviz_comms/tests/test_extension.py
 src/icons.ts
 src/index.ts
 src/manager.ts
```

### Comparing `pyviz_comms-2.3.1/setup.py` & `pyviz_comms-2.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.3.1/src/manager.ts` & `pyviz_comms-2.3.2/src/manager.ts`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.3.1/src/plugin.ts` & `pyviz_comms-2.3.2/src/plugin.ts`

 * *Files 7% similar despite different names*

```diff
@@ -52,14 +52,17 @@
 } from './renderer';
 
 export type INBWidgetExtension = DocumentRegistry.IWidgetExtension<
   NotebookPanel,
   INotebookModel
 >;
 
+import tippy from 'tippy.js';
+import 'tippy.js/dist/tippy.css'; // optional for styling
+
 let registerWidgetManager: any = null;
 try {
   const jlm = require('@jupyter-widgets/jupyterlab-manager');
   registerWidgetManager = jlm.registerWidgetManager;
 } catch (_) {
   console.log('Could not load ipywidgets support for @pyviz/jupyterlab_pyviz');
 }
@@ -73,14 +76,23 @@
   export const panelOpen = 'notebook:open-with-panel';
 
   export const lumenRender = 'notebook:render-with-lumen';
 
   export const lumenOpen = 'notebook:open-with-lumen';
 }
 
+const TOOLTIP_CONTENT = `
+<span>Preview with Panel<span>
+<br>
+<br>
+<span>
+  <b>Note:</b> Your notebook must publish Panel contents with .servable().
+<span>
+`;
+
 /**
  * A notebook widget extension that adds a panel preview button to the toolbar.
  */
 class PanelRenderButton
   implements DocumentRegistry.IWidgetExtension<NotebookPanel, INotebookModel> {
   /**
    * Instantiate a new PanelRenderButton.
@@ -92,21 +104,31 @@
 
   /**
    * Create a new extension object.
    */
   createNew(panel: NotebookPanel): IDisposable {
     const button = new ToolbarButton({
       className: 'panelRender',
-      tooltip: 'Render with Panel',
       icon: panelIcon,
       onClick: (): void => {
         this._commands.execute(CommandIDs.panelRender);
       }
     });
 
+    setTimeout(() => {
+      requestAnimationFrame(() => {
+        tippy(button.node, {
+          allowHTML: true,
+          arrow: true,
+          content: TOOLTIP_CONTENT,
+          placement: 'bottom'
+        });
+      });
+    }, 0);
+
     panel.toolbar.insertAfter('cellType', 'panelRender', button);
     return button;
   }
 
   private _commands: CommandRegistry;
 }
 
@@ -125,21 +147,30 @@
 
   /**
    * Create a new extension object.
    */
   createNew(panel: NotebookPanel): IDisposable {
     const button = new ToolbarButton({
       className: 'lumenRender',
-      tooltip: 'Render with Lumen',
       icon: panelIcon,
       onClick: () => {
         this._commands.execute(CommandIDs.lumenRender);
       }
     });
 
+    setTimeout(() => {
+      requestAnimationFrame(() => {
+        tippy(button.node, {
+          arrow: true,
+          content: 'Preview with Lumen',
+          placement: 'bottom'
+        });
+      });
+    }, 0);
+
     panel.toolbar.addItem('lumenRender', button);
     return button;
   }
 
   private _commands: CommandRegistry;
 }
 
@@ -314,15 +345,15 @@
 
     app.docRegistry.addWidgetFactory(factory);
     app.docRegistry.addWidgetFactory(lumenFactory);
 
     const { commands, docRegistry } = app;
 
     commands.addCommand(CommandIDs.panelRender, {
-      label: 'Render Notebook with Panel',
+      label: 'Preview Notebook with Panel',
       execute: async args => {
         const current = getCurrent(args);
         let context: DocumentRegistry.IContext<INotebookModel>;
         if (current) {
           context = current.context;
           await context.save();
```

### Comparing `pyviz_comms-2.3.1/src/preview.tsx` & `pyviz_comms-2.3.2/src/preview.tsx`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.3.1/src/renderer.ts` & `pyviz_comms-2.3.2/src/renderer.ts`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.3.1/tsconfig.json` & `pyviz_comms-2.3.2/tsconfig.json`

 * *Files identical despite different names*

