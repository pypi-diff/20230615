# Comparing `tmp/intellect_core-0.1.4.tar.gz` & `tmp/intellect_core-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intellect_core-0.1.4.tar", max compression
+gzip compressed data, was "intellect_core-0.1.5.tar", max compression
```

## Comparing `intellect_core-0.1.4.tar` & `intellect_core-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      186 2023-05-29 14:14:55.721473 intellect_core-0.1.4/LICENSE
--rw-r--r--   0        0        0      171 2023-04-10 11:56:09.609658 intellect_core-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-05-29 14:10:28.656955 intellect_core-0.1.4/intellect_core/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 12:57:45.552839 intellect_core-0.1.4/intellect_core/dto/__init__.py
--rw-r--r--   0        0        0     2335 2023-06-13 13:18:22.425868 intellect_core-0.1.4/intellect_core/dto/dto.py
--rw-r--r--   0        0        0     1023 2023-05-29 14:54:49.902384 intellect_core-0.1.4/intellect_core/handler.py
--rw-r--r--   0        0        0     5342 2023-06-14 13:37:57.848403 intellect_core-0.1.4/intellect_core/intelletct_server.py
--rw-r--r--   0        0        0      307 2023-06-14 13:38:13.044242 intellect_core-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 intellect_core-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      186 2023-05-29 14:14:55.721473 intellect_core-0.1.5/LICENSE
+-rw-r--r--   0        0        0      171 2023-04-10 11:56:09.609658 intellect_core-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 14:10:28.656955 intellect_core-0.1.5/intellect_core/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:57:45.552839 intellect_core-0.1.5/intellect_core/dto/__init__.py
+-rw-r--r--   0        0        0     2365 2023-06-15 08:08:32.439329 intellect_core-0.1.5/intellect_core/dto/dto.py
+-rw-r--r--   0        0        0     1023 2023-05-29 14:54:49.902384 intellect_core-0.1.5/intellect_core/handler.py
+-rw-r--r--   0        0        0     5342 2023-06-14 13:37:57.848403 intellect_core-0.1.5/intellect_core/intelletct_server.py
+-rw-r--r--   0        0        0      307 2023-06-15 08:09:46.514645 intellect_core-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 intellect_core-0.1.5/PKG-INFO
```

### Comparing `intellect_core-0.1.4/intellect_core/dto/dto.py` & `intellect_core-0.1.5/intellect_core/dto/dto.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,14 +65,15 @@
         phone: str | None  # phone
         visit_birthplace: str | None  # place_of_birth
         visit_reg: str | None  # registration
         facility_code: str | None
         level_id: int | None  # access_level
         visit_purpose: str | None
         card: str | None
+        temp_card: str | None
 
 
 class IntellectDepartmentDto:
     class Create(BaseModel):
         objid: str
         name: str  # unique_name
         schedule_id: str | None
```

### Comparing `intellect_core-0.1.4/intellect_core/handler.py` & `intellect_core-0.1.5/intellect_core/handler.py`

 * *Files identical despite different names*

### Comparing `intellect_core-0.1.4/intellect_core/intelletct_server.py` & `intellect_core-0.1.5/intellect_core/intelletct_server.py`

 * *Files identical despite different names*

### Comparing `intellect_core-0.1.4/PKG-INFO` & `intellect_core-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intellect-core
-Version: 0.1.4
+Version: 0.1.5
 Summary: Модуль интеграции с Интеллект
 Author: Mrkorogod
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

