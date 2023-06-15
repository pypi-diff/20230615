# Comparing `tmp/perfect_localizer-1.3.tar.gz` & `tmp/perfect_localizer-1.4.tar.gz`

## Comparing `perfect_localizer-1.3.tar` & `perfect_localizer-1.4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 perfect_localizer-1.3/FileHandler.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 perfect_localizer-1.3/__init__.py
--rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 perfect_localizer-1.3/examples.py
--rw-r--r--   0        0        0     8853 2020-02-02 00:00:00.000000 perfect_localizer-1.3/language_pack.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 perfect_localizer-1.3/print_replace.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 perfect_localizer-1.3/requirements.txt
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/Makefile
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/make.bat
--rw-r--r--   0        0        0   249894 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/doctrees/environment.pickle
--rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/doctrees/index.doctree
--rw-r--r--   0        0        0   100843 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/doctrees/localizer.doctree
--rw-r--r--   0        0        0    40956 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/doctrees/localizer.supported_file_types.doctree
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/doctrees/modules.doctree
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/.buildinfo
--rw-r--r--   0        0        0    20870 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/genindex.html
--rw-r--r--   0        0        0    15301 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/index.html
--rw-r--r--   0        0        0    51240 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/localizer.html
--rw-r--r--   0        0        0    25314 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/localizer.supported_file_types.html
--rw-r--r--   0        0        0    18143 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/modules.html
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/objects.inv
--rw-r--r--   0        0        0    12748 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/py-modindex.html
--rw-r--r--   0        0        0    10765 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/search.html
--rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/searchindex.js
--rw-r--r--   0        0        0    11069 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_modules/index.html
--rw-r--r--   0        0        0    14498 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_modules/localizer/FileHandler.html
--rw-r--r--   0        0        0    29423 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_modules/localizer/examples.html
--rw-r--r--   0        0        0    42376 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_modules/localizer/language_pack.html
--rw-r--r--   0        0        0    21512 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_modules/localizer/print_replace.html
--rw-r--r--   0        0        0    18434 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_modules/localizer/supported_file_types/dot_csv.html
--rw-r--r--   0        0        0    15123 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_modules/localizer/supported_file_types/dot_json.html
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_sources/localizer.rst.txt
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_sources/localizer.supported_file_types.rst.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_static/basic.css
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_static/debug.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_static/doctools.js
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_static/file.png
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_static/plus.png
--rw-r--r--   0        0        0    21326 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_static/skeleton.css
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_static/scripts/furo-extensions.js
--rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_static/scripts/furo.js
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_static/scripts/furo.js.LICENSE.txt
--rw-r--r--   0        0        0    28242 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_static/scripts/furo.js.map
--rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_static/styles/furo-extensions.css
--rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_static/styles/furo-extensions.css.map
--rw-r--r--   0        0        0    48512 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_static/styles/furo.css
--rw-r--r--   0        0        0    73326 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/build/html/_static/styles/furo.css.map
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/source/conf.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/source/index.rst
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/source/localizer.rst
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/source/localizer.supported_file_types.rst
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 perfect_localizer-1.3/documentation/source/modules.rst
--rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 perfect_localizer-1.3/scripts/localizer_pack_fill.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 perfect_localizer-1.3/scripts/update_version.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 perfect_localizer-1.3/supported_file_types/__init__.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 perfect_localizer-1.3/supported_file_types/dot_csv.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 perfect_localizer-1.3/supported_file_types/dot_json.py
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 perfect_localizer-1.3/tests/file_handlers.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 perfect_localizer-1.3/tests/language_pack.py
--rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 perfect_localizer-1.3/tests/print_replace.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 perfect_localizer-1.3/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 perfect_localizer-1.3/LICENSE
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 perfect_localizer-1.3/README.md
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 perfect_localizer-1.3/pyproject.toml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 perfect_localizer-1.3/PKG-INFO
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 perfect_localizer-1.4/FileHandler.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 perfect_localizer-1.4/__init__.py
+-rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 perfect_localizer-1.4/examples.py
+-rw-r--r--   0        0        0     8853 2020-02-02 00:00:00.000000 perfect_localizer-1.4/language_pack.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 perfect_localizer-1.4/print_replace.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 perfect_localizer-1.4/requirements.txt
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/Makefile
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/make.bat
+-rw-r--r--   0        0        0   249894 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/doctrees/index.doctree
+-rw-r--r--   0        0        0   100843 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/doctrees/localizer.doctree
+-rw-r--r--   0        0        0    40956 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/doctrees/localizer.supported_file_types.doctree
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/doctrees/modules.doctree
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/.buildinfo
+-rw-r--r--   0        0        0    20870 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/genindex.html
+-rw-r--r--   0        0        0    15301 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/index.html
+-rw-r--r--   0        0        0    51240 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/localizer.html
+-rw-r--r--   0        0        0    25314 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/localizer.supported_file_types.html
+-rw-r--r--   0        0        0    18143 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/modules.html
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/objects.inv
+-rw-r--r--   0        0        0    12748 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/py-modindex.html
+-rw-r--r--   0        0        0    10765 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/search.html
+-rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/searchindex.js
+-rw-r--r--   0        0        0    11069 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_modules/index.html
+-rw-r--r--   0        0        0    14498 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_modules/localizer/FileHandler.html
+-rw-r--r--   0        0        0    29423 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_modules/localizer/examples.html
+-rw-r--r--   0        0        0    42376 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_modules/localizer/language_pack.html
+-rw-r--r--   0        0        0    21512 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_modules/localizer/print_replace.html
+-rw-r--r--   0        0        0    18434 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_modules/localizer/supported_file_types/dot_csv.html
+-rw-r--r--   0        0        0    15123 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_modules/localizer/supported_file_types/dot_json.html
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_sources/localizer.rst.txt
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_sources/localizer.supported_file_types.rst.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_static/basic.css
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_static/debug.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_static/file.png
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_static/plus.png
+-rw-r--r--   0        0        0    21326 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_static/skeleton.css
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_static/scripts/furo-extensions.js
+-rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_static/scripts/furo.js
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_static/scripts/furo.js.LICENSE.txt
+-rw-r--r--   0        0        0    28242 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_static/scripts/furo.js.map
+-rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_static/styles/furo-extensions.css
+-rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_static/styles/furo-extensions.css.map
+-rw-r--r--   0        0        0    48512 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_static/styles/furo.css
+-rw-r--r--   0        0        0    73326 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/build/html/_static/styles/furo.css.map
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/source/conf.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/source/index.rst
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/source/localizer.rst
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/source/localizer.supported_file_types.rst
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 perfect_localizer-1.4/documentation/source/modules.rst
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 perfect_localizer-1.4/scripts/localizer_pack_fill.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 perfect_localizer-1.4/scripts/update_version.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 perfect_localizer-1.4/supported_file_types/__init__.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 perfect_localizer-1.4/supported_file_types/dot_csv.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 perfect_localizer-1.4/supported_file_types/dot_json.py
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 perfect_localizer-1.4/tests/file_handlers.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 perfect_localizer-1.4/tests/language_pack.py
+-rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 perfect_localizer-1.4/tests/print_replace.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 perfect_localizer-1.4/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 perfect_localizer-1.4/LICENSE
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 perfect_localizer-1.4/README.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 perfect_localizer-1.4/pyproject.toml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 perfect_localizer-1.4/PKG-INFO
```

### Comparing `perfect_localizer-1.3/FileHandler.py` & `perfect_localizer-1.4/FileHandler.py`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/examples.py` & `perfect_localizer-1.4/examples.py`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/language_pack.py` & `perfect_localizer-1.4/language_pack.py`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/print_replace.py` & `perfect_localizer-1.4/print_replace.py`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/Makefile` & `perfect_localizer-1.4/documentation/Makefile`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/make.bat` & `perfect_localizer-1.4/documentation/make.bat`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/doctrees/environment.pickle` & `perfect_localizer-1.4/documentation/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/doctrees/index.doctree` & `perfect_localizer-1.4/documentation/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/doctrees/localizer.doctree` & `perfect_localizer-1.4/documentation/build/doctrees/localizer.doctree`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/doctrees/localizer.supported_file_types.doctree` & `perfect_localizer-1.4/documentation/build/doctrees/localizer.supported_file_types.doctree`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/doctrees/modules.doctree` & `perfect_localizer-1.4/documentation/build/doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/genindex.html` & `perfect_localizer-1.4/documentation/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/index.html` & `perfect_localizer-1.4/documentation/build/html/index.html`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/localizer.html` & `perfect_localizer-1.4/documentation/build/html/localizer.html`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/localizer.supported_file_types.html` & `perfect_localizer-1.4/documentation/build/html/localizer.supported_file_types.html`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/modules.html` & `perfect_localizer-1.4/documentation/build/html/modules.html`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/objects.inv` & `perfect_localizer-1.4/documentation/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/py-modindex.html` & `perfect_localizer-1.4/documentation/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/search.html` & `perfect_localizer-1.4/documentation/build/html/search.html`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/searchindex.js` & `perfect_localizer-1.4/documentation/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_modules/index.html` & `perfect_localizer-1.4/documentation/build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_modules/localizer/FileHandler.html` & `perfect_localizer-1.4/documentation/build/html/_modules/localizer/FileHandler.html`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_modules/localizer/examples.html` & `perfect_localizer-1.4/documentation/build/html/_modules/localizer/examples.html`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_modules/localizer/language_pack.html` & `perfect_localizer-1.4/documentation/build/html/_modules/localizer/language_pack.html`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_modules/localizer/print_replace.html` & `perfect_localizer-1.4/documentation/build/html/_modules/localizer/print_replace.html`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_modules/localizer/supported_file_types/dot_csv.html` & `perfect_localizer-1.4/documentation/build/html/_modules/localizer/supported_file_types/dot_csv.html`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_modules/localizer/supported_file_types/dot_json.html` & `perfect_localizer-1.4/documentation/build/html/_modules/localizer/supported_file_types/dot_json.html`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_sources/localizer.rst.txt` & `perfect_localizer-1.4/documentation/build/html/_sources/localizer.rst.txt`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_sources/localizer.supported_file_types.rst.txt` & `perfect_localizer-1.4/documentation/build/html/_sources/localizer.supported_file_types.rst.txt`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_static/basic.css` & `perfect_localizer-1.4/documentation/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_static/debug.css` & `perfect_localizer-1.4/documentation/build/html/_static/debug.css`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_static/doctools.js` & `perfect_localizer-1.4/documentation/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_static/language_data.js` & `perfect_localizer-1.4/documentation/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_static/pygments.css` & `perfect_localizer-1.4/documentation/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_static/searchtools.js` & `perfect_localizer-1.4/documentation/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_static/skeleton.css` & `perfect_localizer-1.4/documentation/build/html/_static/skeleton.css`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_static/sphinx_highlight.js` & `perfect_localizer-1.4/documentation/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_static/scripts/furo.js` & `perfect_localizer-1.4/documentation/build/html/_static/scripts/furo.js`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_static/scripts/furo.js.map` & `perfect_localizer-1.4/documentation/build/html/_static/scripts/furo.js.map`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_static/styles/furo-extensions.css` & `perfect_localizer-1.4/documentation/build/html/_static/styles/furo-extensions.css`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_static/styles/furo-extensions.css.map` & `perfect_localizer-1.4/documentation/build/html/_static/styles/furo-extensions.css.map`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_static/styles/furo.css` & `perfect_localizer-1.4/documentation/build/html/_static/styles/furo.css`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/build/html/_static/styles/furo.css.map` & `perfect_localizer-1.4/documentation/build/html/_static/styles/furo.css.map`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/source/conf.py` & `perfect_localizer-1.4/documentation/source/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'Localizer'
 copyright = '2023, Vbrawl'
 author = 'Vbrawl'
-release = '1.3'
+release  = "1.4"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ["sphinx.ext.autodoc", "sphinx.ext.viewcode"]
 
 templates_path = ['_templates']
```

### Comparing `perfect_localizer-1.3/documentation/source/localizer.rst` & `perfect_localizer-1.4/documentation/source/localizer.rst`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/documentation/source/localizer.supported_file_types.rst` & `perfect_localizer-1.4/documentation/source/localizer.supported_file_types.rst`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/scripts/localizer_pack_fill.py` & `perfect_localizer-1.4/scripts/localizer_pack_fill.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,93 +10,97 @@
 
 def get_next(it:Iterator[str]) -> Optional[str]:
     try:
         return next(it)
     except StopIteration:
         return None
 
-parser = argparse.ArgumentParser(description="Create a language pack for the Python package `Localizer`.", add_help=True, exit_on_error=False)
-parser.add_argument("language_pack_file", type=str, help="The language_pack file, this is going to be updated if it doesn't exist.")
-parser.add_argument("--external_file", "-ef", type=str, nargs="*", help="Other language_packs(to get the original texts only), or new_texts files.")
-parser.add_argument("--translator", "-t", action="store_true", help="Use a translator API to provide translation recommendations.")
-parser.add_argument("--quick-translator", "-qt", action="store_true", help="Use a translator API to automatically translate everything. (Automated translation!)")
-parser.add_argument("--from-lang", "-fl", type=str, default="auto", help="The language of the original text (language code).")
-parser.add_argument("--to-lang", "-tl", type=str, help="The language of the translated text (language code).")
-
-args = parser.parse_args()
-
-lpf = args.language_pack_file
-efs = args.external_file
-translator = args.translator
-qtranslator = args.quick_translator
-fl = args.from_lang
-tl = args.to_lang
-
-lp = LanguagePack()
-lp.auto_translate = False
-lp.translate_from_language = fl
-lp.translate_to_language = tl
-
-if lp.get_file_extension(lpf) is None:
-    print("Error: Unsupported file extension.")
-    print("Please select one of the following extensions: ")
-    print(''.join(map(lambda x: f"\t* {x}\n", lp.supported_file_types.keys())))
-    exit()
-
-if translator and qtranslator:
-    print("Error: Cannot enable translator and quick-translator at the same time.")
-    exit()
-
-if (translator or qtranslator) and not tl:
-    print("Error: --to-lang needs to be specified.")
-    exit()
-
-if os.path.exists(lpf):
-    lp.parse_file(lpf)
-
-if efs:
-    for f in efs:
-        try:
-            tmp_lp = LanguagePack()
-            tmp_lp.parse_file(f)
-            for o in tmp_lp.o_t.keys():
-                if o not in lp.o_t.keys():
-                    lp.new_texts.add(o)
-            for nt in tmp_lp.new_texts:
-                lp.new_texts.add(nt)
-        except TypeError or PermissionError:
-            print(f"Error: external_file({f}) doesn't exist. Ignoring...")
-
-it = iter(lp.new_texts)
-prompt = "{original}{recommendation} => "
-iterator_ended = False
-answer = False
-
-while not iterator_ended or answer:
-    if not iterator_ended:
-        original = get_next(it)
-    else:
-        original = input("Original text: ")
+
+
+
+def main():
+    parser = argparse.ArgumentParser(description="Create a language pack for the Python package `Localizer`.", add_help=True, exit_on_error=False)
+    parser.add_argument("language_pack_file", type=str, help="The language_pack file, this is going to be updated if it doesn't exist.")
+    parser.add_argument("--external_file", "-ef", type=str, nargs="*", help="Other language_packs(to get the original texts only), or new_texts files.")
+    parser.add_argument("--translator", "-t", action="store_true", help="Use a translator API to provide translation recommendations.")
+    parser.add_argument("--quick-translator", "-qt", action="store_true", help="Use a translator API to automatically translate everything. (Automated translation!)")
+    parser.add_argument("--from-lang", "-fl", type=str, default="auto", help="The language of the original text (language code).")
+    parser.add_argument("--to-lang", "-tl", type=str, help="The language of the translated text (language code).")
+
+    args = parser.parse_args()
+
+    lpf = args.language_pack_file
+    efs = args.external_file
+    translator = args.translator
+    qtranslator = args.quick_translator
+    fl = args.from_lang
+    tl = args.to_lang
+
+    lp = LanguagePack()
+    lp.auto_translate = False
+    lp.translate_from_language = fl
+    lp.translate_to_language = tl
+
+    if lp.get_file_extension(lpf) is None:
+        print("Error: Unsupported file extension.")
+        print("Please select one of the following extensions: ")
+        print(''.join(map(lambda x: f"\t* {x}\n", lp.supported_file_types.keys())))
+        return
+
+    if translator and qtranslator:
+        print("Error: Cannot enable translator and quick-translator at the same time.")
+        return
+
+    if (translator or qtranslator) and not tl:
+        print("Error: --to-lang needs to be specified.")
+        return
+
+    if os.path.exists(lpf):
+        lp.parse_file(lpf)
+
+    if efs:
+        for f in efs:
+            try:
+                tmp_lp = LanguagePack()
+                tmp_lp.parse_file(f)
+                for o in tmp_lp.o_t.keys():
+                    if o not in lp.o_t.keys():
+                        lp.new_texts.add(o)
+                for nt in tmp_lp.new_texts:
+                    lp.new_texts.add(nt)
+            except TypeError or PermissionError:
+                print(f"Error: external_file({f}) doesn't exist. Ignoring...")
+
+    it = iter(lp.new_texts)
+    prompt = "{original}{recommendation} => "
+    iterator_ended = False
+    answer = False
+
+    while not iterator_ended or answer:
+        if not iterator_ended:
+            original = get_next(it)
+        else:
+            original = input("Original text: ")
     
-    if original:
-        recommendation = lp.translate(original, auto_add=False) if translator else None
-        translated = get_translation(original, recommendation, prompt) if not qtranslator else None
-
-        lp.add_translation(original, translated)
-    elif not original and not iterator_ended:
-        iterator_ended = True
-        yes_NO = input("Would you like to add more texts? [yes/NO]: ")
-        if yes_NO and yes_NO.upper() == "YES":
-            print("To stop adding more texts, enter a blank original text.")
-            print("You can add a new text by not providing a translation for an original text.")
-            prompt = "Translated Text{recommendation}: "
-            answer = True
-    else:
-        answer = False
-
-if qtranslator:
-    print("Translating All New Texts...")
-    lp.translate_all()
-    print("Translation Finished.")
-print("Saving Changes...")
-lp.export_file(lpf)
-print("Changes Saved.")
+        if original:
+            recommendation = lp.translate(original, auto_add=False) if translator else None
+            translated = get_translation(original, recommendation, prompt) if not qtranslator else None
+
+            lp.add_translation(original, translated)
+        elif not original and not iterator_ended:
+            iterator_ended = True
+            yes_NO = input("Would you like to add more texts? [yes/NO]: ")
+            if yes_NO and yes_NO.upper() == "YES":
+                print("To stop adding more texts, enter a blank original text.")
+                print("You can add a new text by not providing a translation for an original text.")
+                prompt = "Translated Text{recommendation}: "
+                answer = True
+        else:
+            answer = False
+
+    if qtranslator:
+        print("Translating All New Texts...")
+        lp.translate_all()
+        print("Translation Finished.")
+    print("Saving Changes...")
+    lp.export_file(lpf)
+    print("Changes Saved.")
```

### Comparing `perfect_localizer-1.3/scripts/update_version.py` & `perfect_localizer-1.4/scripts/update_version.py`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/supported_file_types/dot_csv.py` & `perfect_localizer-1.4/supported_file_types/dot_csv.py`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/supported_file_types/dot_json.py` & `perfect_localizer-1.4/supported_file_types/dot_json.py`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/tests/file_handlers.py` & `perfect_localizer-1.4/tests/file_handlers.py`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/tests/language_pack.py` & `perfect_localizer-1.4/tests/language_pack.py`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/tests/print_replace.py` & `perfect_localizer-1.4/tests/print_replace.py`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/LICENSE` & `perfect_localizer-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `perfect_localizer-1.3/pyproject.toml` & `perfect_localizer-1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "perfect_localizer"
-version = "1.3"
+version  = "1.4"
 authors = [
     {name="Vbrawl", email="konstantosjim@gmail.com"},
 ]
 description = "An easy way to translate the application interfaces."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.scripts]
-localizer_pack_fill = "localizer.scripts.localizer_pack_fill.py"
+localizer_pack_fill = "localizer.scripts.localizer_pack_fill.py:main"
 
 [project.urls]
 "Homepage" = "https://github.com/Vbrawl/localizer"
```

### Comparing `perfect_localizer-1.3/PKG-INFO` & `perfect_localizer-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perfect_localizer
-Version: 1.3
+Version: 1.4
 Summary: An easy way to translate the application interfaces.
 Project-URL: Homepage, https://github.com/Vbrawl/localizer
 Author-email: Vbrawl <konstantosjim@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

