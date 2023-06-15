# Comparing `tmp/fudan_utils-0.1.3.tar.gz` & `tmp/fudan_utils-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fudan_utils-0.1.3.tar", max compression
+gzip compressed data, was "fudan_utils-0.1.4.tar", max compression
```

## Comparing `fudan_utils-0.1.3.tar` & `fudan_utils-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1579 2023-06-15 06:36:41.231566 fudan_utils-0.1.3/README.md
--rw-r--r--   0        0        0       21 2023-06-15 06:37:58.683378 fudan_utils-0.1.3/fudan_utils/__init__.py
--rw-r--r--   0        0        0       77 2023-06-15 06:07:40.832259 fudan_utils-0.1.3/fudan_utils/config.py
--rw-r--r--   0        0        0     7703 2023-06-15 06:26:16.496167 fudan_utils-0.1.3/fudan_utils/fudan.py
--rwxr-xr-x   0        0        0     1122 2023-06-15 06:26:37.079823 fudan_utils-0.1.3/fudan_utils/fudan_grades.py
--rw-r--r--   0        0        0      963 2023-06-15 06:37:58.682430 fudan_utils-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2417 1970-01-01 00:00:00.000000 fudan_utils-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1647 2023-06-15 06:38:54.978496 fudan_utils-0.1.4/README.md
+-rw-r--r--   0        0        0       21 2023-06-15 06:38:59.833243 fudan_utils-0.1.4/fudan_utils/__init__.py
+-rw-r--r--   0        0        0       77 2023-06-15 06:07:40.832259 fudan_utils-0.1.4/fudan_utils/config.py
+-rw-r--r--   0        0        0     7703 2023-06-15 06:26:16.496167 fudan_utils-0.1.4/fudan_utils/fudan.py
+-rwxr-xr-x   0        0        0     1122 2023-06-15 06:26:37.079823 fudan_utils-0.1.4/fudan_utils/fudan_grades.py
+-rw-r--r--   0        0        0      963 2023-06-15 06:38:59.832587 fudan_utils-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2485 1970-01-01 00:00:00.000000 fudan_utils-0.1.4/PKG-INFO
```

### Comparing `fudan_utils-0.1.3/README.md` & `fudan_utils-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 Get Fudan grades from jwfw
 
 options:
   -h, --help  show this help message and exit
 
 
-$ fudan-grades
+$ fudan-grades # don't forget to supply your credentials via environment variables
 
 学年学期      课程代码      课程序号        课程名称     课程类别        学分     最终      绩点
 -----------  ----------  -------------  ----------  ------------  ------  ------  ------
 2022-2023 2  GTHB139999  GTHB139999.01  毕业论文     专业必修课程          6  F           0
 ```
```

### Comparing `fudan_utils-0.1.3/fudan_utils/fudan.py` & `fudan_utils-0.1.4/fudan_utils/fudan.py`

 * *Files identical despite different names*

### Comparing `fudan_utils-0.1.3/fudan_utils/fudan_grades.py` & `fudan_utils-0.1.4/fudan_utils/fudan_grades.py`

 * *Files identical despite different names*

### Comparing `fudan_utils-0.1.3/pyproject.toml` & `fudan_utils-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fudan-utils"
-version = "0.1.3"
+version = "0.1.4"
 description = "Fudan UIS Login Utilities and More"
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "fudan_utils" }]
 license = "MIT"
 homepage = "https://github.com/tddschn/fudan-utils"
 repository = "https://github.com/tddschn/fudan-utils"
```

### Comparing `fudan_utils-0.1.3/PKG-INFO` & `fudan_utils-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fudan-utils
-Version: 0.1.3
+Version: 0.1.4
 Summary: Fudan UIS Login Utilities and More
 Home-page: https://github.com/tddschn/fudan-utils
 License: MIT
 Keywords: Fudan University
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
@@ -71,15 +71,15 @@
 
 Get Fudan grades from jwfw
 
 options:
   -h, --help  show this help message and exit
 
 
-$ fudan-grades
+$ fudan-grades # don't forget to supply your credentials via environment variables
 
 学年学期      课程代码      课程序号        课程名称     课程类别        学分     最终      绩点
 -----------  ----------  -------------  ----------  ------------  ------  ------  ------
 2022-2023 2  GTHB139999  GTHB139999.01  毕业论文     专业必修课程          6  F           0
 ```
```

