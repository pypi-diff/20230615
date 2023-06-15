# Comparing `tmp/problem_bank_scripts-0.5.0.tar.gz` & `tmp/problem_bank_scripts-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "problem_bank_scripts-0.5.0.tar", max compression
+gzip compressed data, was "problem_bank_scripts-0.6.0.tar", max compression
```

## Comparing `problem_bank_scripts-0.5.0.tar` & `problem_bank_scripts-0.6.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0        1 2021-05-16 14:07:02.985176 problem_bank_scripts-0.5.0/LICENSE
--rw-r--r--   0        0        0     1244 2021-05-17 01:13:34.351180 problem_bank_scripts-0.5.0/README.md
--rw-r--r--   0        0        0     1052 2023-06-14 21:39:32.611573 problem_bank_scripts-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       59 2023-06-14 21:39:35.225325 problem_bank_scripts-0.5.0/src/problem_bank_scripts/__init__.py
--rw-r--r--   0        0        0    13476 2021-08-13 04:07:58.134898 problem_bank_scripts-0.5.0/src/problem_bank_scripts/prairielearn.py
--rw-r--r--   0        0        0    43948 2023-06-14 21:36:06.930925 problem_bank_scripts-0.5.0/src/problem_bank_scripts/problem_bank_scripts.py
--rw-r--r--   0        0        0      129 2022-06-24 05:48:29.289246 problem_bank_scripts-0.5.0/src/problem_bank_scripts/qti_export.py
--rw-r--r--   0        0        0    19225 2022-06-24 07:32:56.504377 problem_bank_scripts-0.5.0/src/problem_bank_scripts/webwork_to_md.py
--rw-r--r--   0        0        0     2263 2023-06-14 21:40:22.378440 problem_bank_scripts-0.5.0/setup.py
--rw-r--r--   0        0        0     2318 2023-06-14 21:40:22.378661 problem_bank_scripts-0.5.0/PKG-INFO
+-rwxr-xr-x   0        0        0        1 2021-05-16 14:07:02.985176 problem_bank_scripts-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1605 2023-06-15 01:42:11.784217 problem_bank_scripts-0.6.0/README.md
+-rw-r--r--   0        0        0     1052 2023-06-15 05:06:41.661080 problem_bank_scripts-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-06-15 05:07:04.296824 problem_bank_scripts-0.6.0/src/problem_bank_scripts/__init__.py
+-rw-r--r--   0        0        0    13476 2021-08-13 04:07:58.134898 problem_bank_scripts-0.6.0/src/problem_bank_scripts/prairielearn.py
+-rw-r--r--   0        0        0    43948 2023-06-14 21:36:06.930925 problem_bank_scripts-0.6.0/src/problem_bank_scripts/problem_bank_scripts.py
+-rw-r--r--   0        0        0      129 2022-06-24 05:48:29.289246 problem_bank_scripts-0.6.0/src/problem_bank_scripts/qti_export.py
+-rw-r--r--   0        0        0    19225 2022-06-24 07:32:56.504377 problem_bank_scripts-0.6.0/src/problem_bank_scripts/webwork_to_md.py
+-rw-r--r--   0        0        0     2647 2023-06-15 05:08:32.893855 problem_bank_scripts-0.6.0/setup.py
+-rw-r--r--   0        0        0     2679 2023-06-15 05:08:32.894114 problem_bank_scripts-0.6.0/PKG-INFO
```

### Comparing `problem_bank_scripts-0.5.0/README.md` & `problem_bank_scripts-0.6.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,37 @@
 
 ## Installation
 
 ```bash
 $ pip install -i https://test.pypi.org/simple/ problem_bank_scripts
 ```
 
+## Update version
+
+Here are the steps to increment the version (replace patch with major/minor/patch)
+
+```
+poetry version patch
+
+pico src/problem_bank_scripts/__init__.py
+
+pico tests/test_problem_bank_scripts.py
+
+poetry run pytest
+
+cd docs; poetry run make html; cd ..
+
+git add .; git commit -m "increment version"; git push
+
+poetry build
+
+poetry publish
+```
+
+
 ## Features
 
 - TODO
 
 ## Dependencies
 
 - TODO
```

### Comparing `problem_bank_scripts-0.5.0/pyproject.toml` & `problem_bank_scripts-0.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "problem_bank_scripts"
-version = "0.5.0"
+version = "0.6.0"
 description = "A package with useful functions to convert between different problem bank formats."
 authors = ["Open Problem Bank Team"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://problem_bank_scripts.readthedocs.io/en/latest/"
 homepage = "https://github.com/open-resources/problem_bank_scripts"
 repository = "https://github.com/open-resources/problem_bank_scripts"
```

### Comparing `problem_bank_scripts-0.5.0/src/problem_bank_scripts/prairielearn.py` & `problem_bank_scripts-0.6.0/src/problem_bank_scripts/prairielearn.py`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.5.0/src/problem_bank_scripts/problem_bank_scripts.py` & `problem_bank_scripts-0.6.0/src/problem_bank_scripts/problem_bank_scripts.py`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.5.0/src/problem_bank_scripts/webwork_to_md.py` & `problem_bank_scripts-0.6.0/src/problem_bank_scripts/webwork_to_md.py`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.5.0/setup.py` & `problem_bank_scripts-0.6.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,17 +18,17 @@
  'numpy>=1.22,<2.0',
  'pandas>=1.2.4,<2.0.0',
  'problem-bank-helpers>=0.1.12,<0.2.0',
  'sympy>=1.8,<2.0']
 
 setup_kwargs = {
     'name': 'problem-bank-scripts',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': 'A package with useful functions to convert between different problem bank formats.',
-    'long_description': '# Problem Bank Scripts \n\n[![Python](https://img.shields.io/badge/python-3.9-blue)]()\n[![codecov](https://codecov.io/gh/open-resources/problem_bank_scripts/branch/main/graph/badge.svg)](https://codecov.io/gh/open-resources/problem_bank_scripts)\n[![Documentation Status](https://readthedocs.org/projects/problem_bank_scripts/badge/?version=latest)](https://problem_bank_scripts.readthedocs.io/en/latest/?badge=latest)\n\n\n## Installation\n\n```bash\n$ pip install -i https://test.pypi.org/simple/ problem_bank_scripts\n```\n\n## Features\n\n- TODO\n\n## Dependencies\n\n- TODO\n\n## Usage\n\n- TODO\n\n## Documentation\n\nThe official documentation is hosted on Read the Docs: https://problem_bank_scripts.readthedocs.io/en/latest/\n\n## Contributors\n\nWe welcome and recognize all contributions. You can see a list of current contributors in the [contributors tab](https://github.com/open-resources/problem_bank_scripts/graphs/contributors).\n\n### Credits\n\nThis package was created with Cookiecutter and the UBC-MDS/cookiecutter-ubc-mds project template, modified from the [pyOpenSci/cookiecutter-pyopensci](https://github.com/pyOpenSci/cookiecutter-pyopensci) project template and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).\n',
+    'long_description': '# Problem Bank Scripts \n\n[![Python](https://img.shields.io/badge/python-3.9-blue)]()\n[![codecov](https://codecov.io/gh/open-resources/problem_bank_scripts/branch/main/graph/badge.svg)](https://codecov.io/gh/open-resources/problem_bank_scripts)\n[![Documentation Status](https://readthedocs.org/projects/problem_bank_scripts/badge/?version=latest)](https://problem_bank_scripts.readthedocs.io/en/latest/?badge=latest)\n\n\n## Installation\n\n```bash\n$ pip install -i https://test.pypi.org/simple/ problem_bank_scripts\n```\n\n## Update version\n\nHere are the steps to increment the version (replace patch with major/minor/patch)\n\n```\npoetry version patch\n\npico src/problem_bank_scripts/__init__.py\n\npico tests/test_problem_bank_scripts.py\n\npoetry run pytest\n\ncd docs; poetry run make html; cd ..\n\ngit add .; git commit -m "increment version"; git push\n\npoetry build\n\npoetry publish\n```\n\n\n## Features\n\n- TODO\n\n## Dependencies\n\n- TODO\n\n## Usage\n\n- TODO\n\n## Documentation\n\nThe official documentation is hosted on Read the Docs: https://problem_bank_scripts.readthedocs.io/en/latest/\n\n## Contributors\n\nWe welcome and recognize all contributions. You can see a list of current contributors in the [contributors tab](https://github.com/open-resources/problem_bank_scripts/graphs/contributors).\n\n### Credits\n\nThis package was created with Cookiecutter and the UBC-MDS/cookiecutter-ubc-mds project template, modified from the [pyOpenSci/cookiecutter-pyopensci](https://github.com/pyOpenSci/cookiecutter-pyopensci) project template and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).\n',
     'author': 'Open Problem Bank Team',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/open-resources/problem_bank_scripts',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `problem_bank_scripts-0.5.0/PKG-INFO` & `problem_bank_scripts-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: problem-bank-scripts
-Version: 0.5.0
+Version: 0.6.0
 Summary: A package with useful functions to convert between different problem bank formats.
 Home-page: https://github.com/open-resources/problem_bank_scripts
 License: MIT
 Author: Open Problem Bank Team
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -32,14 +32,37 @@
 
 ## Installation
 
 ```bash
 $ pip install -i https://test.pypi.org/simple/ problem_bank_scripts
 ```
 
+## Update version
+
+Here are the steps to increment the version (replace patch with major/minor/patch)
+
+```
+poetry version patch
+
+pico src/problem_bank_scripts/__init__.py
+
+pico tests/test_problem_bank_scripts.py
+
+poetry run pytest
+
+cd docs; poetry run make html; cd ..
+
+git add .; git commit -m "increment version"; git push
+
+poetry build
+
+poetry publish
+```
+
+
 ## Features
 
 - TODO
 
 ## Dependencies
 
 - TODO
```

