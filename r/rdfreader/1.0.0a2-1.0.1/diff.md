# Comparing `tmp/rdfreader-1.0.0a2.tar.gz` & `tmp/rdfreader-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfreader-1.0.0a2.tar", max compression
+gzip compressed data, was "rdfreader-1.0.1.tar", max compression
```

## Comparing `rdfreader-1.0.0a2.tar` & `rdfreader-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      738 2023-06-14 12:59:15.823827 rdfreader-1.0.0a2/pyproject.toml
--rw-r--r--   0        0        0       49 2023-05-04 09:39:42.731680 rdfreader-1.0.0a2/rdfreader/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 09:39:42.731680 rdfreader-1.0.0a2/rdfreader/chem/__init__.py
--rw-r--r--   0        0        0     4977 2023-05-09 16:08:15.935278 rdfreader-1.0.0a2/rdfreader/chem/mol.py
--rw-r--r--   0        0        0     4775 2023-05-09 16:08:15.935278 rdfreader-1.0.0a2/rdfreader/chem/reaction.py
--rw-r--r--   0        0        0      881 2023-05-09 16:08:15.935278 rdfreader-1.0.0a2/rdfreader/chem/utils.py
--rw-r--r--   0        0        0      246 2023-05-09 16:08:15.935278 rdfreader-1.0.0a2/rdfreader/exceptions.py
--rw-r--r--   0        0        0     2758 2023-05-09 16:08:15.935278 rdfreader-1.0.0a2/rdfreader/parse/molblock.py
--rw-r--r--   0        0        0     8105 2023-06-14 12:39:56.244379 rdfreader-1.0.0a2/rdfreader/parse/rxnblock.py
--rw-r--r--   0        0        0    10226 2023-05-09 16:08:15.935278 rdfreader-1.0.0a2/rdfreader/parse/utils.py
--rw-r--r--   0        0        0     4951 2023-05-09 16:08:15.935278 rdfreader-1.0.0a2/rdfreader/rdf.py
--rw-r--r--   0        0        0      985 2023-05-09 16:08:15.935278 rdfreader-1.0.0a2/rdfreader/write.py
--rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 rdfreader-1.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0     3771 2023-06-15 08:56:21.444375 rdfreader-1.0.1/README.md
+-rw-r--r--   0        0        0     1056 2023-06-15 08:56:21.448375 rdfreader-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       49 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/chem/__init__.py
+-rw-r--r--   0        0        0     4977 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/chem/mol.py
+-rw-r--r--   0        0        0     4775 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/chem/reaction.py
+-rw-r--r--   0        0        0      881 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/chem/utils.py
+-rw-r--r--   0        0        0      246 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/exceptions.py
+-rw-r--r--   0        0        0     2758 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/parse/molblock.py
+-rw-r--r--   0        0        0     8105 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/parse/rxnblock.py
+-rw-r--r--   0        0        0    10225 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/parse/utils.py
+-rw-r--r--   0        0        0     4951 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/rdf.py
+-rw-r--r--   0        0        0      985 2023-06-15 08:56:21.448375 rdfreader-1.0.1/rdfreader/write.py
+-rw-r--r--   0        0        0     4698 1970-01-01 00:00:00.000000 rdfreader-1.0.1/PKG-INFO
```

### Comparing `rdfreader-1.0.0a2/rdfreader/chem/mol.py` & `rdfreader-1.0.1/rdfreader/chem/mol.py`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.0a2/rdfreader/chem/reaction.py` & `rdfreader-1.0.1/rdfreader/chem/reaction.py`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.0a2/rdfreader/chem/utils.py` & `rdfreader-1.0.1/rdfreader/chem/utils.py`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.0a2/rdfreader/parse/molblock.py` & `rdfreader-1.0.1/rdfreader/parse/molblock.py`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.0a2/rdfreader/parse/rxnblock.py` & `rdfreader-1.0.1/rdfreader/parse/rxnblock.py`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.0a2/rdfreader/parse/utils.py` & `rdfreader-1.0.1/rdfreader/parse/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,14 @@
         A dictionary of metadata.
     """
 
     format_string_dict = parse_format_string(header_format_string)
 
     metadata = {}
     for letter, character_index in format_string_dict.items():
-
         if letter in header_field_mapping:
             field_name = header_field_mapping[letter][0]
             data_type = header_field_mapping[letter][1]
             try:
                 default_value = header_field_mapping[letter][2]
             except IndexError:
                 default_value = None
```

### Comparing `rdfreader-1.0.0a2/rdfreader/rdf.py` & `rdfreader-1.0.1/rdfreader/rdf.py`

 * *Files identical despite different names*

### Comparing `rdfreader-1.0.0a2/rdfreader/write.py` & `rdfreader-1.0.1/rdfreader/write.py`

 * *Files identical despite different names*

