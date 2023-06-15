# Comparing `tmp/qqbot-linger-0.1.1.tar.gz` & `tmp/qqbot_linger-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qqbot-linger-0.1.1.tar", last modified: Mon Mar  1 14:08:22 2021, max compression
+gzip compressed data, was "qqbot_linger-0.2.0a1.tar", max compression
```

## Comparing `qqbot-linger-0.1.1.tar` & `qqbot_linger-0.2.0a1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0      588 2021-02-07 20:20:12.102029 qqbot-linger-0.1.1/README.md
--rw-r--r--   0        0        0     1211 2021-02-07 14:46:35.984052 qqbot-linger-0.1.1/UNLICENSE
--rw-r--r--   0        0        0      984 2021-03-01 14:06:45.348560 qqbot-linger-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2021-03-01 14:06:54.236958 qqbot-linger-0.1.1/qqbot_linger/__init__.py
--rw-r--r--   0        0        0      446 2021-03-01 14:03:05.692293 qqbot-linger-0.1.1/qqbot_linger/main.py
--rw-r--r--   0        0        0     1472 2021-03-01 14:08:22.502412 qqbot-linger-0.1.1/setup.py
--rw-r--r--   0        0        0     1446 2021-03-01 14:08:22.502642 qqbot-linger-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-15 15:28:05.364651 qqbot_linger-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-06-15 14:33:17.187189 qqbot_linger-0.2.0a1/qqbot_linger/__init__.py
+-rw-r--r--   0        0        0      429 2023-06-15 15:28:41.514858 qqbot_linger-0.2.0a1/qqbot_linger/main.py
+-rw-r--r--   0        0        0      588 2023-06-14 17:38:38.474357 qqbot_linger-0.2.0a1/README.md
+-rw-r--r--   0        0        0     1211 2023-06-14 17:38:38.474357 qqbot_linger-0.2.0a1/UNLICENSE
+-rw-r--r--   0        0        0     1554 1970-01-01 00:00:00.000000 qqbot_linger-0.2.0a1/PKG-INFO
```

### Comparing `qqbot-linger-0.1.1/README.md` & `qqbot_linger-0.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `qqbot-linger-0.1.1/UNLICENSE` & `qqbot_linger-0.2.0a1/UNLICENSE`

 * *Files identical despite different names*

### Comparing `qqbot-linger-0.1.1/pyproject.toml` & `qqbot_linger-0.2.0a1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 [tool.poetry]
 name = "qqbot-linger"
-version = "0.1.1"
+version = "0.2.0a1"
 description = "My QQ Bot for personal use"
 authors = ["7sDream <i@7sdre.am>"]
 license = "Unlicense"
 readme = "README.md"
 homepage = "https://github.com/7sDream/qqbot-linger"
 repository = "https://github.com/7sDream/qqbot-linger"
 keywords = ["nonebot", "bilibili", "qqbot"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: The Unlicense (Unlicense)",
 ]
 include = [
     "UNLICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pydantic = "1.7.3"
-nonebot2 = {version = "^2.0.0a10", allow-prereleases = true}
-nonebot-plugin-bam = "^0.1.4"
-nonebot-plugin-7s-roll = "^0.1.2"
+pydantic = "1.10.9"
+nonebot2 = {extras = ["fastapi"], version = "2.0.0"}
+nonebot-plugin-7s-roll = "^0.2.0a1"
+nonebot-plugin-bam = "^0.2.0a1"
 
-[tool.poetry.dev-dependencies]
-rope = "^0.18.0"
-black = "^20.8b1"
-pylint = "^2.7.2"
+[tool.poetry.group.dev.dependencies]
+pylint = "^2.17.4"
+black = "^23.3.0"
+rope = "^1.8.0"
 
 [tool.poetry.scripts]
 linger = 'qqbot_linger.main:main'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `qqbot-linger-0.1.1/PKG-INFO` & `qqbot_linger-0.2.0a1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: qqbot-linger
-Version: 0.1.1
+Version: 0.2.0a1
 Summary: My QQ Bot for personal use
 Home-page: https://github.com/7sDream/qqbot-linger
 License: Unlicense
 Keywords: nonebot,bilibili,qqbot
 Author: 7sDream
 Author-email: i@7sdre.am
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: nonebot-plugin-7s-roll (>=0.1.2,<0.2.0)
-Requires-Dist: nonebot-plugin-bam (>=0.1.4,<0.2.0)
-Requires-Dist: nonebot2 (>=2.0.0a10,<3.0.0)
-Requires-Dist: pydantic (==1.7.3)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: nonebot-plugin-7s-roll (>=0.2.0a1,<0.3.0)
+Requires-Dist: nonebot-plugin-bam (>=0.2.0a1,<0.3.0)
+Requires-Dist: nonebot2[fastapi] (==2.0.0)
+Requires-Dist: pydantic (==1.10.9)
 Project-URL: Repository, https://github.com/7sDream/qqbot-linger
 Description-Content-Type: text/markdown
 
 # 玲儿
 
 自用 QQ 机器人。
```

