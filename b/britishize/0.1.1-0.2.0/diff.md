# Comparing `tmp/britishize-0.1.1.tar.gz` & `tmp/britishize-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "britishize-0.1.1.tar", max compression
+gzip compressed data, was "britishize-0.2.0.tar", max compression
```

## Comparing `britishize-0.1.1.tar` & `britishize-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      318 2023-06-15 14:23:55.092237 britishize-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       21 2023-06-15 14:17:08.439865 britishize-0.1.1/readme.md
--rw-r--r--   0        0        0     1539 2023-06-15 14:10:53.321684 britishize-0.1.1/src/britishize/britishize.py
--rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 britishize-0.1.1/setup.py
--rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 britishize-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      395 2023-06-15 14:34:57.835244 britishize-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-15 14:17:08.439865 britishize-0.2.0/readme.md
+-rw-r--r--   0        0        0     1691 2023-06-15 14:32:14.995351 britishize-0.2.0/src/britishize/britishize.py
+-rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 britishize-0.2.0/setup.py
+-rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 britishize-0.2.0/PKG-INFO
```

### Comparing `britishize-0.1.1/src/britishize/britishize.py` & `britishize-0.2.0/src/britishize/britishize.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,7 +25,18 @@
     for i in range(len(words)):
         if words[i] in us2gb:
             brand_new_words.append(us2gb[words[i]])
         else:
             brand_new_words.append(words[i])
 
     return " ".join(brand_new_words)
+
+import typer
+
+app = typer.Typer()
+
+@app.command()
+def translate(american_english: str):
+    print(britishize(american_english))
+
+def main():
+    app()
```

### Comparing `britishize-0.1.1/setup.py` & `britishize-0.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,25 +6,33 @@
 
 packages = \
 ['britishize']
 
 package_data = \
 {'': ['*']}
 
+install_requires = \
+['typer>=0.9.0,<0.10.0']
+
+entry_points = \
+{'console_scripts': ['brit = britishize.britishize:main']}
+
 setup_kwargs = {
     'name': 'britishize',
-    'version': '0.1.1',
+    'version': '0.2.0',
     'description': 'Write poorer english',
     'long_description': 'Write proper english\n',
     'author': 'Antonio Feregrino',
     'author_email': 'antonio.feregrino@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
+    'install_requires': install_requires,
+    'entry_points': entry_points,
     'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `britishize-0.1.1/PKG-INFO` & `britishize-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: britishize
-Version: 0.1.1
+Version: 0.2.0
 Summary: Write poorer english
 License: MIT
 Author: Antonio Feregrino
 Author-email: antonio.feregrino@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 Write proper english
```

