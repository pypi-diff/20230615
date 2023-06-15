# Comparing `tmp/foliantcontrib.dbmldoc-0.3.3.tar.gz` & `tmp/foliantcontrib.dbmldoc-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foliantcontrib.dbmldoc-0.3.3.tar", last modified: Sun Dec 11 11:16:09 2022, max compression
+gzip compressed data, was "foliantcontrib.dbmldoc-0.3.4.tar", last modified: Thu Jun 15 17:27:48 2023, max compression
```

## Comparing `foliantcontrib.dbmldoc-0.3.3.tar` & `foliantcontrib.dbmldoc-0.3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-12-11 11:16:09.450859 foliantcontrib.dbmldoc-0.3.3/
--rwxr-xr-x   0 user      (1000) user      (1000)     1056 2022-11-19 15:14:35.000000 foliantcontrib.dbmldoc-0.3.3/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     4920 2022-12-11 11:16:09.450859 foliantcontrib.dbmldoc-0.3.3/PKG-INFO
--rwxr-xr-x   0 user      (1000) user      (1000)     4304 2022-12-04 11:34:55.000000 foliantcontrib.dbmldoc-0.3.3/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-12-11 11:16:09.447526 foliantcontrib.dbmldoc-0.3.3/foliant/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-12-11 11:16:09.447526 foliantcontrib.dbmldoc-0.3.3/foliant/preprocessors/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-12-11 11:16:09.447526 foliantcontrib.dbmldoc-0.3.3/foliant/preprocessors/dbmldoc/
--rw-r--r--   0 user      (1000) user      (1000)       33 2022-11-19 15:14:35.000000 foliantcontrib.dbmldoc-0.3.3/foliant/preprocessors/dbmldoc/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     6032 2022-12-04 11:27:51.000000 foliantcontrib.dbmldoc-0.3.3/foliant/preprocessors/dbmldoc/dbmldoc.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-12-11 11:16:09.447526 foliantcontrib.dbmldoc-0.3.3/foliant/preprocessors/dbmldoc/template/
--rw-r--r--   0 user      (1000) user      (1000)     2423 2022-12-11 11:05:57.000000 foliantcontrib.dbmldoc-0.3.3/foliant/preprocessors/dbmldoc/template/dbml.j2
--rw-r--r--   0 user      (1000) user      (1000)      730 2022-12-04 11:24:16.000000 foliantcontrib.dbmldoc-0.3.3/foliant/preprocessors/dbmldoc/template/scheme.j2
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-12-11 11:16:09.450859 foliantcontrib.dbmldoc-0.3.3/foliantcontrib.dbmldoc.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     4920 2022-12-11 11:16:09.000000 foliantcontrib.dbmldoc-0.3.3/foliantcontrib.dbmldoc.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      434 2022-12-11 11:16:09.000000 foliantcontrib.dbmldoc-0.3.3/foliantcontrib.dbmldoc.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2022-12-11 11:16:09.000000 foliantcontrib.dbmldoc-0.3.3/foliantcontrib.dbmldoc.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       64 2022-12-11 11:16:09.000000 foliantcontrib.dbmldoc-0.3.3/foliantcontrib.dbmldoc.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2022-12-11 11:16:09.000000 foliantcontrib.dbmldoc-0.3.3/foliantcontrib.dbmldoc.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2022-12-11 11:16:09.450859 foliantcontrib.dbmldoc-0.3.3/setup.cfg
--rwxr-xr-x   0 user      (1000) user      (1000)     1191 2022-12-11 11:06:08.000000 foliantcontrib.dbmldoc-0.3.3/setup.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-06-15 17:27:48.260008 foliantcontrib.dbmldoc-0.3.4/
+-rwxr-xr-x   0 user       (502) staff       (20)     1056 2023-06-15 17:07:29.000000 foliantcontrib.dbmldoc-0.3.4/LICENSE
+-rw-r--r--   0 user       (502) staff       (20)     4941 2023-06-15 17:27:48.259490 foliantcontrib.dbmldoc-0.3.4/PKG-INFO
+-rwxr-xr-x   0 user       (502) staff       (20)     4304 2023-06-15 17:07:29.000000 foliantcontrib.dbmldoc-0.3.4/README.md
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-06-15 17:27:48.241705 foliantcontrib.dbmldoc-0.3.4/foliant/
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-06-15 17:27:48.241852 foliantcontrib.dbmldoc-0.3.4/foliant/preprocessors/
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-06-15 17:27:48.245230 foliantcontrib.dbmldoc-0.3.4/foliant/preprocessors/dbmldoc/
+-rw-r--r--   0 user       (502) staff       (20)       33 2023-06-15 17:07:29.000000 foliantcontrib.dbmldoc-0.3.4/foliant/preprocessors/dbmldoc/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     6032 2023-06-15 17:07:29.000000 foliantcontrib.dbmldoc-0.3.4/foliant/preprocessors/dbmldoc/dbmldoc.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-06-15 17:27:48.246457 foliantcontrib.dbmldoc-0.3.4/foliant/preprocessors/dbmldoc/template/
+-rw-r--r--   0 user       (502) staff       (20)     2421 2023-06-15 17:20:41.000000 foliantcontrib.dbmldoc-0.3.4/foliant/preprocessors/dbmldoc/template/dbml.j2
+-rw-r--r--   0 user       (502) staff       (20)      808 2023-06-15 17:20:38.000000 foliantcontrib.dbmldoc-0.3.4/foliant/preprocessors/dbmldoc/template/scheme.j2
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-06-15 17:27:48.258398 foliantcontrib.dbmldoc-0.3.4/foliantcontrib.dbmldoc.egg-info/
+-rw-r--r--   0 user       (502) staff       (20)     4941 2023-06-15 17:27:48.000000 foliantcontrib.dbmldoc-0.3.4/foliantcontrib.dbmldoc.egg-info/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)      434 2023-06-15 17:27:48.000000 foliantcontrib.dbmldoc-0.3.4/foliantcontrib.dbmldoc.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (502) staff       (20)        1 2023-06-15 17:27:48.000000 foliantcontrib.dbmldoc-0.3.4/foliantcontrib.dbmldoc.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (502) staff       (20)       64 2023-06-15 17:27:48.000000 foliantcontrib.dbmldoc-0.3.4/foliantcontrib.dbmldoc.egg-info/requires.txt
+-rw-r--r--   0 user       (502) staff       (20)        8 2023-06-15 17:27:48.000000 foliantcontrib.dbmldoc-0.3.4/foliantcontrib.dbmldoc.egg-info/top_level.txt
+-rw-r--r--   0 user       (502) staff       (20)       38 2023-06-15 17:27:48.260203 foliantcontrib.dbmldoc-0.3.4/setup.cfg
+-rwxr-xr-x   0 user       (502) staff       (20)     1191 2023-06-15 17:25:35.000000 foliantcontrib.dbmldoc-0.3.4/setup.py
```

### Comparing `foliantcontrib.dbmldoc-0.3.3/LICENSE` & `foliantcontrib.dbmldoc-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `foliantcontrib.dbmldoc-0.3.3/PKG-INFO` & `foliantcontrib.dbmldoc-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: foliantcontrib.dbmldoc
-Version: 0.3.3
+Version: 0.3.4
 Summary: Documentation generator for DBML specification format
+Home-page: UNKNOWN
 Author: Daniil Minukhin
 Author-email: ddddsa@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -117,7 +118,9 @@
 ## Customizing output
 
 The output markdown is generated by the [Jinja2](http://jinja.pocoo.org/) template. Inside the template all data from the parsed DBML file is available under the `data` variable. It is in fact a `PyDBMLParseResults` object, as returned by [PyDBML](https://github.com/Vanderhoof/PyDBML) (see the docs to find out which attributes are available).
 
 To customize the output create a template which suits your needs. Then supply the path to it in the `template` parameter. Same goes for the scheme template, which is defined in the `scheme_template` parameter.
 
 If you wish to use the default template as a starting point, build the foliant project with `dbmldoc` preprocessor turned on. After the first build the default templates will appear in your foliant project dir under the names `dbml.j2` and `scheme.j2`.
+
+
```

### Comparing `foliantcontrib.dbmldoc-0.3.3/README.md` & `foliantcontrib.dbmldoc-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `foliantcontrib.dbmldoc-0.3.3/foliant/preprocessors/dbmldoc/dbmldoc.py` & `foliantcontrib.dbmldoc-0.3.4/foliant/preprocessors/dbmldoc/dbmldoc.py`

 * *Files identical despite different names*

### Comparing `foliantcontrib.dbmldoc-0.3.3/foliant/preprocessors/dbmldoc/template/dbml.j2` & `foliantcontrib.dbmldoc-0.3.4/foliant/preprocessors/dbmldoc/template/dbml.j2`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {# Template should be initialized with data environment variable:
 
-  data = Database object
+  data = Database object (of PyDBML)
 
   For available attributes refer to https://github.com/Vanderhoof/PyDBML
 #}
 {%- macro render_table_ref(ref, col) -%}
 {%- for ref_col in ref.col1 -%}
     {%- if ref_col == col %} [{{ ref.table2.name}}](#{{ref.table2.name.lower()}}).(
         {%- for rr_col in ref.col2 %}{% if loop.index > 1 %}, {% endif%}{{ rr_col.name }}{% endfor -%}
@@ -20,15 +20,15 @@
 {%- macro render_table(table, db) -%}
 ## {{ table.name }}
 
 {% set refs = {} %}
 {% for r in table.get_references_for_sql() %}
     {%  set _ = refs.setdefault(r.col2[0].name if r.type == '<' else r.col1[0].name, []).append(r) %}
 {%  endfor %}
-    {{ refs }}
+
 ```sql
 {{ table.sql }}
 ```
 
 {{ table.note or table.comment or '' }}
 
 column | properties | type | descr | fkey
```

### Comparing `foliantcontrib.dbmldoc-0.3.3/foliant/preprocessors/dbmldoc/template/scheme.j2` & `foliantcontrib.dbmldoc-0.3.4/foliant/preprocessors/dbmldoc/template/scheme.j2`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 {# Template should be initialized with data environment variable:
 
-  data = PyDBMLParseResults object
+  data = Database object (of PyDBML)
+
+  For available attributes refer to https://github.com/Vanderhoof/PyDBML
 #}
 
 # Database Scheme
 
 <plantuml>
 @startuml
 {% for table in data.tables %}
@@ -13,14 +15,14 @@
 {{ column.name|indent(8) }} [{{ column.type }}]
 {% endfor %}{# {% for column in table %} #}
     }
 {% endfor %}{# {% for table in tables %} #}
 
 {% for table in data.tables -%}
 {% for ref in table.get_refs() -%}
-{{ table.name|indent }} --> {{ ref.table2.name }} : {% for c in ref.col %}
+{{ table.name|indent }} --> {{ ref.table2.name }} : {% for c in ref.col2 %}
     {%- if loop.index > 1 %}, {% endif%}{{c.name}}
 {%- endfor %}{# {% for c in ref.col %} #}
 {% endfor -%}{# {% for ref in table.refs -%} #}
 {%- endfor -%}{# {% for table in tables -%} #}
     @enduml
-</plantuml>
+</plantuml>
```

### Comparing `foliantcontrib.dbmldoc-0.3.3/foliantcontrib.dbmldoc.egg-info/PKG-INFO` & `foliantcontrib.dbmldoc-0.3.4/foliantcontrib.dbmldoc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: foliantcontrib.dbmldoc
-Version: 0.3.3
+Version: 0.3.4
 Summary: Documentation generator for DBML specification format
+Home-page: UNKNOWN
 Author: Daniil Minukhin
 Author-email: ddddsa@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -117,7 +118,9 @@
 ## Customizing output
 
 The output markdown is generated by the [Jinja2](http://jinja.pocoo.org/) template. Inside the template all data from the parsed DBML file is available under the `data` variable. It is in fact a `PyDBMLParseResults` object, as returned by [PyDBML](https://github.com/Vanderhoof/PyDBML) (see the docs to find out which attributes are available).
 
 To customize the output create a template which suits your needs. Then supply the path to it in the `template` parameter. Same goes for the scheme template, which is defined in the `scheme_template` parameter.
 
 If you wish to use the default template as a starting point, build the foliant project with `dbmldoc` preprocessor turned on. After the first build the default templates will appear in your foliant project dir under the names `dbml.j2` and `scheme.j2`.
+
+
```

### Comparing `foliantcontrib.dbmldoc-0.3.3/setup.py` & `foliantcontrib.dbmldoc-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 setup(
     name='foliantcontrib.dbmldoc',
     description=SHORT_DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
-    version='0.3.3',
+    version='0.3.4',
     author='Daniil Minukhin',
     author_email='ddddsa@gmail.com',
     packages=['foliant.preprocessors.dbmldoc'],
     package_data={'foliant.preprocessors.dbmldoc': ['template/*.j2']},
     license='MIT',
     platforms='any',
     install_requires=[
```

