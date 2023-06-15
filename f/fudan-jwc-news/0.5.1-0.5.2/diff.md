# Comparing `tmp/fudan-jwc-news-0.5.1.tar.gz` & `tmp/fudan_jwc_news-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fudan-jwc-news-0.5.1.tar", max compression
+gzip compressed data, was "fudan_jwc_news-0.5.2.tar", max compression
```

## Comparing `fudan-jwc-news-0.5.1.tar` & `fudan_jwc_news-0.5.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1113 2022-04-30 16:01:35.401928 fudan-jwc-news-0.5.1/LICENSE
--rw-r--r--   0        0        0     1462 2022-04-30 16:40:47.420863 fudan-jwc-news-0.5.1/README.md
--rw-r--r--   0        0        0      331 2022-05-01 08:23:53.046466 fudan-jwc-news-0.5.1/fudan_jwc_news/__init__.py
--rwxr-xr-x   0        0        0     4067 2022-05-01 07:44:56.957964 fudan-jwc-news-0.5.1/fudan_jwc_news/jwc_news.py
--rw-r--r--   0        0        0      954 2022-05-01 08:23:53.045996 fudan-jwc-news-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2411 2022-05-01 08:23:57.431201 fudan-jwc-news-0.5.1/setup.py
--rw-r--r--   0        0        0     2287 2022-05-01 08:23:57.431590 fudan-jwc-news-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1113 2023-06-15 06:36:21.770227 fudan_jwc_news-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1588 2023-06-15 06:37:21.910967 fudan_jwc_news-0.5.2/README.md
+-rw-r--r--   0        0        0      331 2023-06-15 06:37:50.417725 fudan_jwc_news-0.5.2/fudan_jwc_news/__init__.py
+-rwxr-xr-x   0        0        0     4067 2023-06-15 06:36:21.772270 fudan_jwc_news-0.5.2/fudan_jwc_news/jwc_news.py
+-rw-r--r--   0        0        0      954 2023-06-15 06:37:50.416340 fudan_jwc_news-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2464 1970-01-01 00:00:00.000000 fudan_jwc_news-0.5.2/PKG-INFO
```

### Comparing `fudan-jwc-news-0.5.1/LICENSE` & `fudan_jwc_news-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fudan-jwc-news-0.5.1/README.md` & `fudan_jwc_news-0.5.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 - [fudan-jwc-news](#fudan-jwc-news)
   - [Installation](#installation)
     - [pipx](#pipx)
     - [pip](#pip)
   - [Usage](#usage)
   - [Example output](#example-output)
+  - [See also](#see-also)
 
 ## Installation
 
 ### pipx
 
 ```
 pipx install fudan-jwc-news
@@ -51,7 +52,11 @@
 04-29 关于2022年春季学期复旦大学水平测试(补测试)考试通知
 http://www.jwc.fudan.edu.cn/bf/be/c25325a442302/page.htm
 
 04-29 2022年春季学期本科学生转专业报名名单
 http://www.jwc.fudan.edu.cn/bf/bc/c25325a442300/page.htm
 
 ```
+
+## See also
+
+- https://github.com/tddschn/fudan-utils : Get your grades from command line, and more
```

### Comparing `fudan-jwc-news-0.5.1/fudan_jwc_news/jwc_news.py` & `fudan_jwc_news-0.5.2/fudan_jwc_news/jwc_news.py`

 * *Files identical despite different names*

### Comparing `fudan-jwc-news-0.5.1/pyproject.toml` & `fudan_jwc_news-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fudan-jwc-news"
-version = "0.5.1"
+version = "0.5.2"
 description = "Read Fudan JWC news from your terminal"
 authors = ["Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tddschn/fudan-jwc-news"
 repository = "https://github.com/tddschn/fudan-jwc-news"
 classifiers = [
```

### Comparing `fudan-jwc-news-0.5.1/PKG-INFO` & `fudan_jwc_news-0.5.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: fudan-jwc-news
-Version: 0.5.1
+Version: 0.5.2
 Summary: Read Fudan JWC news from your terminal
 Home-page: https://github.com/tddschn/fudan-jwc-news
 License: MIT
 Keywords: fudan,news
 Author: Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: pyinstrument (>=4.1.1,<5.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: typer (>=0.4.1,<0.5.0)
 Project-URL: Bug Tracker, https://github.com/tddschn/fudan-jwc-news/issues
 Project-URL: Repository, https://github.com/tddschn/fudan-jwc-news
@@ -29,14 +30,15 @@
 
 - [fudan-jwc-news](#fudan-jwc-news)
   - [Installation](#installation)
     - [pipx](#pipx)
     - [pip](#pip)
   - [Usage](#usage)
   - [Example output](#example-output)
+  - [See also](#see-also)
 
 ## Installation
 
 ### pipx
 
 ```
 pipx install fudan-jwc-news
@@ -74,7 +76,10 @@
 http://www.jwc.fudan.edu.cn/bf/be/c25325a442302/page.htm
 
 04-29 2022年春季学期本科学生转专业报名名单
 http://www.jwc.fudan.edu.cn/bf/bc/c25325a442300/page.htm
 
 ```
 
+## See also
+
+- https://github.com/tddschn/fudan-utils : Get your grades from command line, and more
```

