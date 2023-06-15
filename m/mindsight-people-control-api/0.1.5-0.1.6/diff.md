# Comparing `tmp/mindsight_people_control_api-0.1.5.tar.gz` & `tmp/mindsight_people_control_api-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindsight_people_control_api-0.1.5.tar", max compression
+gzip compressed data, was "mindsight_people_control_api-0.1.6.tar", max compression
```

## Comparing `mindsight_people_control_api-0.1.5.tar` & `mindsight_people_control_api-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1081 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/LICENSE
--rw-r--r--   0        0        0     1342 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/README.md
--rw-r--r--   0        0        0      407 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/mindsight_people_control_api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/mindsight_people_control_api/helpers/__init__.py
--rw-r--r--   0        0        0     5225 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/mindsight_people_control_api/helpers/base_requests.py
--rw-r--r--   0        0        0      392 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/mindsight_people_control_api/helpers/exceptions.py
--rw-r--r--   0        0        0     1869 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/mindsight_people_control_api/helpers/models.py
--rw-r--r--   0        0        0      783 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/__init__.py
--rw-r--r--   0        0        0     4566 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/area_records.py
--rw-r--r--   0        0        0     7415 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/areas.py
--rw-r--r--   0        0        0     5513 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/employee_areas.py
--rw-r--r--   0        0        0     5591 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/employee_managers.py
--rw-r--r--   0        0        0     5623 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/employee_positions.py
--rw-r--r--   0        0        0     4896 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/employee_records.py
--rw-r--r--   0        0        0    12367 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/employees.py
--rw-r--r--   0        0        0     4721 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/parent_areas.py
--rw-r--r--   0        0        0     7060 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/positions.py
--rw-r--r--   0        0        0     7654 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/users.py
--rw-r--r--   0        0        0      843 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/mindsight_people_control_api/settings.py
--rw-r--r--   0        0        0        0 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/mindsight_people_control_api/utils/__init__.py
--rw-r--r--   0        0        0      308 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/mindsight_people_control_api/utils/aux_functions.py
--rw-r--r--   0        0        0      543 2023-06-09 01:00:29.651666 mindsight_people_control_api-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2114 1970-01-01 00:00:00.000000 mindsight_people_control_api-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1342 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/README.md
+-rw-r--r--   0        0        0      407 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/helpers/__init__.py
+-rw-r--r--   0        0        0     5225 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/helpers/base_requests.py
+-rw-r--r--   0        0        0      392 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/helpers/exceptions.py
+-rw-r--r--   0        0        0     1869 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/helpers/models.py
+-rw-r--r--   0        0        0      783 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/__init__.py
+-rw-r--r--   0        0        0     4566 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/area_records.py
+-rw-r--r--   0        0        0     7415 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/areas.py
+-rw-r--r--   0        0        0     5513 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/employee_areas.py
+-rw-r--r--   0        0        0     5591 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/employee_managers.py
+-rw-r--r--   0        0        0     5623 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/employee_positions.py
+-rw-r--r--   0        0        0     4896 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/employee_records.py
+-rw-r--r--   0        0        0    12367 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/employees.py
+-rw-r--r--   0        0        0     4721 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/parent_areas.py
+-rw-r--r--   0        0        0     7060 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/positions.py
+-rw-r--r--   0        0        0     7654 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/users.py
+-rw-r--r--   0        0        0      843 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/settings.py
+-rw-r--r--   0        0        0        0 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/utils/__init__.py
+-rw-r--r--   0        0        0      308 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/utils/aux_functions.py
+-rw-r--r--   0        0        0      699 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2227 1970-01-01 00:00:00.000000 mindsight_people_control_api-0.1.6/PKG-INFO
```

### Comparing `mindsight_people_control_api-0.1.5/LICENSE` & `mindsight_people_control_api-0.1.6/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Diogo de Amorim da Silva
+Copyright (c) 2023 Stone
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mindsight_people_control_api-0.1.5/README.md` & `mindsight_people_control_api-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.5/mindsight_people_control_api/helpers/base_requests.py` & `mindsight_people_control_api-0.1.6/mindsight_people_control_api/helpers/base_requests.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.5/mindsight_people_control_api/helpers/models.py` & `mindsight_people_control_api-0.1.6/mindsight_people_control_api/helpers/models.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/__init__.py` & `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/area_records.py` & `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/area_records.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/areas.py` & `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/areas.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/employee_areas.py` & `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/employee_areas.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/employee_managers.py` & `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/employee_managers.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/employee_positions.py` & `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/employee_positions.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/employee_records.py` & `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/employee_records.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/employees.py` & `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/employees.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/parent_areas.py` & `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/parent_areas.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/positions.py` & `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/positions.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.5/mindsight_people_control_api/scripts/users.py` & `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/users.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.5/mindsight_people_control_api/settings.py` & `mindsight_people_control_api-0.1.6/mindsight_people_control_api/settings.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.5/PKG-INFO` & `mindsight_people_control_api-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: mindsight-people-control-api
-Version: 0.1.5
+Version: 0.1.6
 Summary: Mindsight People Control API to create, update and delete records
-Home-page: https://github.com/Diogo56/mindsight-people-control-api
+Home-page: https://github.com/people-analytics-tech/mindsight-people-control-api
 License: MIT
-Author: Diogo56
-Author-email: diogo.amorim2001@gmail.com
+Author: stone_people_analytics
+Author-email: systems-techpeople@stone.com.br
+Maintainer: diogo56
+Maintainer-email: diogo.amorim2001@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: python-decouple (>=3.8,<4.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Project-URL: Repository, https://github.com/Diogo56/mindsight-people-control-api
+Project-URL: Repository, https://github.com/people-analytics-tech/mindsight-people-control-api
 Description-Content-Type: text/markdown
 
 # Mindsight People Control API
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mindsight-people-control-api.svg)](https://pypi.org/project/mindsight-people-control-api/)
 
 Use mindsight people control functionalities in your python application.
 ## Instalation
```

