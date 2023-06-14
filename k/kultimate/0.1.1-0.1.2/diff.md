# Comparing `tmp/kultimate-0.1.1.tar.gz` & `tmp/kultimate-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kultimate-0.1.1.tar", max compression
+gzip compressed data, was "kultimate-0.1.2.tar", max compression
```

## Comparing `kultimate-0.1.1.tar` & `kultimate-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1820 2023-06-14 22:51:45.896608 kultimate-0.1.1/README.md
--rw-r--r--   0        0        0       22 2023-06-05 20:11:41.877983 kultimate-0.1.1/kultimate/__init__.py
--rw-r--r--   0        0        0     1405 2023-06-14 18:50:13.597219 kultimate-0.1.1/kultimate/app.css
--rw-r--r--   0        0        0    18118 2023-06-14 21:37:13.313178 kultimate-0.1.1/kultimate/app.py
--rw-r--r--   0        0        0       64 2023-06-14 18:50:13.597219 kultimate-0.1.1/kultimate/screens/__init__.py
--rw-r--r--   0        0        0      896 2023-06-14 18:50:13.597219 kultimate-0.1.1/kultimate/screens/addTask.py
--rw-r--r--   0        0        0      988 2023-06-14 16:24:13.233698 kultimate-0.1.1/kultimate/screens/deleteTask.py
--rw-r--r--   0        0        0      125 2023-06-09 21:48:51.262790 kultimate-0.1.1/kultimate/utils/__init__.py
--rw-r--r--   0        0        0     2068 2023-06-12 23:04:04.110731 kultimate-0.1.1/kultimate/utils/app_config.py
--rw-r--r--   0        0        0     2043 2023-06-14 21:37:13.313178 kultimate-0.1.1/kultimate/utils/html_to_markdown.py
--rw-r--r--   0        0        0     2417 2023-06-14 21:37:13.313178 kultimate-0.1.1/kultimate/utils/parser_html.py
--rw-r--r--   0        0        0     1084 2023-06-02 22:13:35.823860 kultimate-0.1.1/kultimate/utils/process_yaml.py
--rw-r--r--   0        0        0      127 2023-06-07 23:20:48.314373 kultimate-0.1.1/kultimate/widgets/__init__.py
--rw-r--r--   0        0        0      620 2023-06-09 21:48:51.266124 kultimate-0.1.1/kultimate/widgets/directory.py
--rw-r--r--   0        0        0      426 2023-06-07 21:05:08.384197 kultimate-0.1.1/kultimate/widgets/stages.py
--rw-r--r--   0        0        0      122 2023-06-07 21:03:56.964196 kultimate-0.1.1/kultimate/widgets/stagesContainer.py
--rw-r--r--   0        0        0      136 2023-06-09 19:45:57.286316 kultimate-0.1.1/kultimate/widgets/task.py
--rw-r--r--   0        0        0      606 2023-06-14 22:55:37.839947 kultimate-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2447 1970-01-01 00:00:00.000000 kultimate-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1821 2023-06-14 22:57:08.956615 kultimate-0.1.2/README.md
+-rw-r--r--   0        0        0       22 2023-06-05 20:11:41.877983 kultimate-0.1.2/kultimate/__init__.py
+-rw-r--r--   0        0        0     1405 2023-06-14 18:50:13.597219 kultimate-0.1.2/kultimate/app.css
+-rw-r--r--   0        0        0    18118 2023-06-14 21:37:13.313178 kultimate-0.1.2/kultimate/app.py
+-rw-r--r--   0        0        0       64 2023-06-14 18:50:13.597219 kultimate-0.1.2/kultimate/screens/__init__.py
+-rw-r--r--   0        0        0      896 2023-06-14 18:50:13.597219 kultimate-0.1.2/kultimate/screens/addTask.py
+-rw-r--r--   0        0        0      988 2023-06-14 16:24:13.233698 kultimate-0.1.2/kultimate/screens/deleteTask.py
+-rw-r--r--   0        0        0      125 2023-06-09 21:48:51.262790 kultimate-0.1.2/kultimate/utils/__init__.py
+-rw-r--r--   0        0        0     2068 2023-06-12 23:04:04.110731 kultimate-0.1.2/kultimate/utils/app_config.py
+-rw-r--r--   0        0        0     2043 2023-06-14 21:37:13.313178 kultimate-0.1.2/kultimate/utils/html_to_markdown.py
+-rw-r--r--   0        0        0     2417 2023-06-14 21:37:13.313178 kultimate-0.1.2/kultimate/utils/parser_html.py
+-rw-r--r--   0        0        0     1084 2023-06-02 22:13:35.823860 kultimate-0.1.2/kultimate/utils/process_yaml.py
+-rw-r--r--   0        0        0      127 2023-06-07 23:20:48.314373 kultimate-0.1.2/kultimate/widgets/__init__.py
+-rw-r--r--   0        0        0      620 2023-06-09 21:48:51.266124 kultimate-0.1.2/kultimate/widgets/directory.py
+-rw-r--r--   0        0        0      426 2023-06-07 21:05:08.384197 kultimate-0.1.2/kultimate/widgets/stages.py
+-rw-r--r--   0        0        0      122 2023-06-07 21:03:56.964196 kultimate-0.1.2/kultimate/widgets/stagesContainer.py
+-rw-r--r--   0        0        0      136 2023-06-09 19:45:57.286316 kultimate-0.1.2/kultimate/widgets/task.py
+-rw-r--r--   0        0        0      606 2023-06-14 22:59:22.633285 kultimate-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 kultimate-0.1.2/PKG-INFO
```

### Comparing `kultimate-0.1.1/README.md` & `kultimate-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Kultimate
 
-[kultimate](render1686782901985.gif)
+![kultimate](render1686782901985.gif)
 
 Aplicación CLI Python para manejar archivos markdown como tableros Kanban.
 Programado con [textual](https://textual.textualize.io/).
 
 # Instalación
 
 ```sh
```

### Comparing `kultimate-0.1.1/kultimate/app.css` & `kultimate-0.1.2/kultimate/app.css`

 * *Files identical despite different names*

### Comparing `kultimate-0.1.1/kultimate/app.py` & `kultimate-0.1.2/kultimate/app.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.1.1/kultimate/screens/addTask.py` & `kultimate-0.1.2/kultimate/screens/addTask.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.1.1/kultimate/screens/deleteTask.py` & `kultimate-0.1.2/kultimate/screens/deleteTask.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.1.1/kultimate/utils/app_config.py` & `kultimate-0.1.2/kultimate/utils/app_config.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.1.1/kultimate/utils/html_to_markdown.py` & `kultimate-0.1.2/kultimate/utils/html_to_markdown.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.1.1/kultimate/utils/parser_html.py` & `kultimate-0.1.2/kultimate/utils/parser_html.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.1.1/kultimate/utils/process_yaml.py` & `kultimate-0.1.2/kultimate/utils/process_yaml.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.1.1/kultimate/widgets/directory.py` & `kultimate-0.1.2/kultimate/widgets/directory.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.1.1/PKG-INFO` & `kultimate-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kultimate
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Felipe
 Author-email: 104157442+justafewwords4@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -14,15 +14,15 @@
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: textual[dev] (>=0.27.0,<0.28.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # Kultimate
 
-[kultimate](render1686782901985.gif)
+![kultimate](render1686782901985.gif)
 
 Aplicación CLI Python para manejar archivos markdown como tableros Kanban.
 Programado con [textual](https://textual.textualize.io/).
 
 # Instalación
 
 ```sh
```

