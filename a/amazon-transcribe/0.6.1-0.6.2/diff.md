# Comparing `tmp/amazon-transcribe-0.6.1.tar.gz` & `tmp/amazon-transcribe-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-transcribe-0.6.1.tar", last modified: Tue Oct  4 18:26:22 2022, max compression
+gzip compressed data, was "amazon-transcribe-0.6.2.tar", last modified: Thu Jun 15 16:13:02 2023, max compression
```

## Comparing `amazon-transcribe-0.6.1.tar` & `amazon-transcribe-0.6.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 natepr     (504) staff       (20)        0 2022-10-04 18:26:22.979156 amazon-transcribe-0.6.1/
--rw-r--r--   0 natepr     (504) staff       (20)    10142 2022-10-04 17:22:12.000000 amazon-transcribe-0.6.1/LICENSE
--rw-r--r--   0 natepr     (504) staff       (20)       35 2022-10-04 17:22:12.000000 amazon-transcribe-0.6.1/MANIFEST.in
--rw-r--r--   0 natepr     (504) staff       (20)       67 2022-10-04 17:22:12.000000 amazon-transcribe-0.6.1/NOTICE
--rw-r--r--   0 natepr     (504) staff       (20)     6361 2022-10-04 18:26:22.979282 amazon-transcribe-0.6.1/PKG-INFO
--rw-r--r--   0 natepr     (504) staff       (20)     5446 2022-10-04 17:22:12.000000 amazon-transcribe-0.6.1/README.md
-drwxr-xr-x   0 natepr     (504) staff       (20)        0 2022-10-04 18:26:22.978397 amazon-transcribe-0.6.1/amazon_transcribe/
--rw-r--r--   0 natepr     (504) staff       (20)      749 2022-10-04 18:07:29.000000 amazon-transcribe-0.6.1/amazon_transcribe/__init__.py
--rw-r--r--   0 natepr     (504) staff       (20)     1726 2022-10-04 17:22:12.000000 amazon-transcribe-0.6.1/amazon_transcribe/auth.py
--rw-r--r--   0 natepr     (504) staff       (20)    10059 2022-10-04 17:22:12.000000 amazon-transcribe-0.6.1/amazon_transcribe/client.py
--rw-r--r--   0 natepr     (504) staff       (20)     9488 2022-10-04 17:22:12.000000 amazon-transcribe-0.6.1/amazon_transcribe/deserialize.py
--rw-r--r--   0 natepr     (504) staff       (20)     1364 2022-10-04 17:22:12.000000 amazon-transcribe-0.6.1/amazon_transcribe/endpoints.py
--rw-r--r--   0 natepr     (504) staff       (20)    26515 2022-10-04 17:22:12.000000 amazon-transcribe-0.6.1/amazon_transcribe/eventstream.py
--rw-r--r--   0 natepr     (504) staff       (20)     2267 2022-10-04 17:22:12.000000 amazon-transcribe-0.6.1/amazon_transcribe/exceptions.py
--rw-r--r--   0 natepr     (504) staff       (20)     1447 2022-10-04 17:22:12.000000 amazon-transcribe-0.6.1/amazon_transcribe/handlers.py
--rw-r--r--   0 natepr     (504) staff       (20)     7424 2022-10-04 17:22:12.000000 amazon-transcribe-0.6.1/amazon_transcribe/httpsession.py
--rw-r--r--   0 natepr     (504) staff       (20)    16375 2022-10-04 17:22:12.000000 amazon-transcribe-0.6.1/amazon_transcribe/model.py
--rw-r--r--   0 natepr     (504) staff       (20)        7 2022-10-04 17:22:12.000000 amazon-transcribe-0.6.1/amazon_transcribe/py.typed
--rw-r--r--   0 natepr     (504) staff       (20)     5830 2022-10-04 17:22:12.000000 amazon-transcribe-0.6.1/amazon_transcribe/request.py
--rw-r--r--   0 natepr     (504) staff       (20)      884 2022-10-04 17:22:12.000000 amazon-transcribe-0.6.1/amazon_transcribe/response.py
--rw-r--r--   0 natepr     (504) staff       (20)     5363 2022-10-04 17:22:12.000000 amazon-transcribe-0.6.1/amazon_transcribe/serialize.py
--rw-r--r--   0 natepr     (504) staff       (20)     2950 2022-10-04 17:22:12.000000 amazon-transcribe-0.6.1/amazon_transcribe/signer.py
--rw-r--r--   0 natepr     (504) staff       (20)     3050 2022-10-04 17:22:12.000000 amazon-transcribe-0.6.1/amazon_transcribe/structures.py
--rw-r--r--   0 natepr     (504) staff       (20)     2086 2022-10-04 17:22:12.000000 amazon-transcribe-0.6.1/amazon_transcribe/utils.py
-drwxr-xr-x   0 natepr     (504) staff       (20)        0 2022-10-04 18:26:22.979032 amazon-transcribe-0.6.1/amazon_transcribe.egg-info/
--rw-r--r--   0 natepr     (504) staff       (20)     6361 2022-10-04 18:26:22.000000 amazon-transcribe-0.6.1/amazon_transcribe.egg-info/PKG-INFO
--rw-r--r--   0 natepr     (504) staff       (20)      766 2022-10-04 18:26:22.000000 amazon-transcribe-0.6.1/amazon_transcribe.egg-info/SOURCES.txt
--rw-r--r--   0 natepr     (504) staff       (20)        1 2022-10-04 18:26:22.000000 amazon-transcribe-0.6.1/amazon_transcribe.egg-info/dependency_links.txt
--rw-r--r--   0 natepr     (504) staff       (20)       15 2022-10-04 18:26:22.000000 amazon-transcribe-0.6.1/amazon_transcribe.egg-info/requires.txt
--rw-r--r--   0 natepr     (504) staff       (20)       18 2022-10-04 18:26:22.000000 amazon-transcribe-0.6.1/amazon_transcribe.egg-info/top_level.txt
--rw-r--r--   0 natepr     (504) staff       (20)      141 2022-10-04 18:26:22.979636 amazon-transcribe-0.6.1/setup.cfg
--rw-r--r--   0 natepr     (504) staff       (20)     1731 2022-10-04 18:07:29.000000 amazon-transcribe-0.6.1/setup.py
+drwxr-xr-x   0 davidlm    (504) staff       (20)        0 2023-06-15 16:13:02.962036 amazon-transcribe-0.6.2/
+-rw-r--r--   0 davidlm    (504) staff       (20)    10142 2023-06-14 17:10:23.000000 amazon-transcribe-0.6.2/LICENSE
+-rw-r--r--   0 davidlm    (504) staff       (20)       35 2023-06-14 17:10:23.000000 amazon-transcribe-0.6.2/MANIFEST.in
+-rw-r--r--   0 davidlm    (504) staff       (20)       67 2023-06-14 17:10:23.000000 amazon-transcribe-0.6.2/NOTICE
+-rw-r--r--   0 davidlm    (504) staff       (20)     6341 2023-06-15 16:13:02.962128 amazon-transcribe-0.6.2/PKG-INFO
+-rw-r--r--   0 davidlm    (504) staff       (20)     5446 2023-06-14 17:10:23.000000 amazon-transcribe-0.6.2/README.md
+drwxr-xr-x   0 davidlm    (504) staff       (20)        0 2023-06-15 16:13:02.961174 amazon-transcribe-0.6.2/amazon_transcribe/
+-rw-r--r--   0 davidlm    (504) staff       (20)      749 2023-06-14 21:17:30.000000 amazon-transcribe-0.6.2/amazon_transcribe/__init__.py
+-rw-r--r--   0 davidlm    (504) staff       (20)     1726 2023-06-14 17:10:23.000000 amazon-transcribe-0.6.2/amazon_transcribe/auth.py
+-rw-r--r--   0 davidlm    (504) staff       (20)    10059 2023-06-14 17:10:23.000000 amazon-transcribe-0.6.2/amazon_transcribe/client.py
+-rw-r--r--   0 davidlm    (504) staff       (20)     9488 2023-06-14 17:10:23.000000 amazon-transcribe-0.6.2/amazon_transcribe/deserialize.py
+-rw-r--r--   0 davidlm    (504) staff       (20)     1364 2023-06-14 17:10:23.000000 amazon-transcribe-0.6.2/amazon_transcribe/endpoints.py
+-rw-r--r--   0 davidlm    (504) staff       (20)    26515 2023-06-14 17:10:23.000000 amazon-transcribe-0.6.2/amazon_transcribe/eventstream.py
+-rw-r--r--   0 davidlm    (504) staff       (20)     2267 2023-06-14 17:10:23.000000 amazon-transcribe-0.6.2/amazon_transcribe/exceptions.py
+-rw-r--r--   0 davidlm    (504) staff       (20)     1447 2023-06-14 17:10:23.000000 amazon-transcribe-0.6.2/amazon_transcribe/handlers.py
+-rw-r--r--   0 davidlm    (504) staff       (20)     7424 2023-06-14 17:10:23.000000 amazon-transcribe-0.6.2/amazon_transcribe/httpsession.py
+-rw-r--r--   0 davidlm    (504) staff       (20)    16375 2023-06-14 17:10:23.000000 amazon-transcribe-0.6.2/amazon_transcribe/model.py
+-rw-r--r--   0 davidlm    (504) staff       (20)        7 2023-06-14 17:10:23.000000 amazon-transcribe-0.6.2/amazon_transcribe/py.typed
+-rw-r--r--   0 davidlm    (504) staff       (20)     5830 2023-06-14 17:10:23.000000 amazon-transcribe-0.6.2/amazon_transcribe/request.py
+-rw-r--r--   0 davidlm    (504) staff       (20)      884 2023-06-14 17:10:23.000000 amazon-transcribe-0.6.2/amazon_transcribe/response.py
+-rw-r--r--   0 davidlm    (504) staff       (20)     5363 2023-06-14 17:10:23.000000 amazon-transcribe-0.6.2/amazon_transcribe/serialize.py
+-rw-r--r--   0 davidlm    (504) staff       (20)     2950 2023-06-14 17:10:23.000000 amazon-transcribe-0.6.2/amazon_transcribe/signer.py
+-rw-r--r--   0 davidlm    (504) staff       (20)     3050 2023-06-14 17:10:23.000000 amazon-transcribe-0.6.2/amazon_transcribe/structures.py
+-rw-r--r--   0 davidlm    (504) staff       (20)     2086 2023-06-14 17:10:23.000000 amazon-transcribe-0.6.2/amazon_transcribe/utils.py
+drwxr-xr-x   0 davidlm    (504) staff       (20)        0 2023-06-15 16:13:02.961863 amazon-transcribe-0.6.2/amazon_transcribe.egg-info/
+-rw-r--r--   0 davidlm    (504) staff       (20)     6341 2023-06-15 16:13:02.000000 amazon-transcribe-0.6.2/amazon_transcribe.egg-info/PKG-INFO
+-rw-r--r--   0 davidlm    (504) staff       (20)      766 2023-06-15 16:13:02.000000 amazon-transcribe-0.6.2/amazon_transcribe.egg-info/SOURCES.txt
+-rw-r--r--   0 davidlm    (504) staff       (20)        1 2023-06-15 16:13:02.000000 amazon-transcribe-0.6.2/amazon_transcribe.egg-info/dependency_links.txt
+-rw-r--r--   0 davidlm    (504) staff       (20)       15 2023-06-15 16:13:02.000000 amazon-transcribe-0.6.2/amazon_transcribe.egg-info/requires.txt
+-rw-r--r--   0 davidlm    (504) staff       (20)       18 2023-06-15 16:13:02.000000 amazon-transcribe-0.6.2/amazon_transcribe.egg-info/top_level.txt
+-rw-r--r--   0 davidlm    (504) staff       (20)      141 2023-06-15 16:13:02.962464 amazon-transcribe-0.6.2/setup.cfg
+-rw-r--r--   0 davidlm    (504) staff       (20)     1731 2023-06-14 21:17:30.000000 amazon-transcribe-0.6.2/setup.py
```

### Comparing `amazon-transcribe-0.6.1/LICENSE` & `amazon-transcribe-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-transcribe-0.6.1/PKG-INFO` & `amazon-transcribe-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: amazon-transcribe
-Version: 0.6.1
+Version: 0.6.2
 Summary: Async Python SDK for Amazon Transcribe Streaming
 Home-page: https://github.com/awslabs/amazon-transcribe-streaming-sdk
 Author: Amazon Web Services
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -163,9 +162,7 @@
 ## Security
 
 See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.
 
 ## License
 
 This project is licensed under the Apache-2.0 License.
-
-
```

### Comparing `amazon-transcribe-0.6.1/README.md` & `amazon-transcribe-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `amazon-transcribe-0.6.1/amazon_transcribe/__init__.py` & `amazon-transcribe-0.6.2/amazon_transcribe/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 
 from awscrt.io import ClientBootstrap
 
 
 class AWSCRTEventLoop:
     def __init__(self):
         self.bootstrap = ClientBootstrap.get_or_create_static_default()
```

### Comparing `amazon-transcribe-0.6.1/amazon_transcribe/auth.py` & `amazon-transcribe-0.6.2/amazon_transcribe/auth.py`

 * *Files identical despite different names*

### Comparing `amazon-transcribe-0.6.1/amazon_transcribe/client.py` & `amazon-transcribe-0.6.2/amazon_transcribe/client.py`

 * *Files identical despite different names*

### Comparing `amazon-transcribe-0.6.1/amazon_transcribe/deserialize.py` & `amazon-transcribe-0.6.2/amazon_transcribe/deserialize.py`

 * *Files identical despite different names*

### Comparing `amazon-transcribe-0.6.1/amazon_transcribe/endpoints.py` & `amazon-transcribe-0.6.2/amazon_transcribe/endpoints.py`

 * *Files identical despite different names*

### Comparing `amazon-transcribe-0.6.1/amazon_transcribe/eventstream.py` & `amazon-transcribe-0.6.2/amazon_transcribe/eventstream.py`

 * *Files identical despite different names*

### Comparing `amazon-transcribe-0.6.1/amazon_transcribe/exceptions.py` & `amazon-transcribe-0.6.2/amazon_transcribe/exceptions.py`

 * *Files identical despite different names*

### Comparing `amazon-transcribe-0.6.1/amazon_transcribe/handlers.py` & `amazon-transcribe-0.6.2/amazon_transcribe/handlers.py`

 * *Files identical despite different names*

### Comparing `amazon-transcribe-0.6.1/amazon_transcribe/httpsession.py` & `amazon-transcribe-0.6.2/amazon_transcribe/httpsession.py`

 * *Files identical despite different names*

### Comparing `amazon-transcribe-0.6.1/amazon_transcribe/model.py` & `amazon-transcribe-0.6.2/amazon_transcribe/model.py`

 * *Files identical despite different names*

### Comparing `amazon-transcribe-0.6.1/amazon_transcribe/request.py` & `amazon-transcribe-0.6.2/amazon_transcribe/request.py`

 * *Files identical despite different names*

### Comparing `amazon-transcribe-0.6.1/amazon_transcribe/response.py` & `amazon-transcribe-0.6.2/amazon_transcribe/response.py`

 * *Files identical despite different names*

### Comparing `amazon-transcribe-0.6.1/amazon_transcribe/serialize.py` & `amazon-transcribe-0.6.2/amazon_transcribe/serialize.py`

 * *Files identical despite different names*

### Comparing `amazon-transcribe-0.6.1/amazon_transcribe/signer.py` & `amazon-transcribe-0.6.2/amazon_transcribe/signer.py`

 * *Files identical despite different names*

### Comparing `amazon-transcribe-0.6.1/amazon_transcribe/structures.py` & `amazon-transcribe-0.6.2/amazon_transcribe/structures.py`

 * *Files identical despite different names*

### Comparing `amazon-transcribe-0.6.1/amazon_transcribe/utils.py` & `amazon-transcribe-0.6.2/amazon_transcribe/utils.py`

 * *Files identical despite different names*

### Comparing `amazon-transcribe-0.6.1/amazon_transcribe.egg-info/PKG-INFO` & `amazon-transcribe-0.6.2/amazon_transcribe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: amazon-transcribe
-Version: 0.6.1
+Version: 0.6.2
 Summary: Async Python SDK for Amazon Transcribe Streaming
 Home-page: https://github.com/awslabs/amazon-transcribe-streaming-sdk
 Author: Amazon Web Services
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -163,9 +162,7 @@
 ## Security
 
 See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.
 
 ## License
 
 This project is licensed under the Apache-2.0 License.
-
-
```

### Comparing `amazon-transcribe-0.6.1/amazon_transcribe.egg-info/SOURCES.txt` & `amazon-transcribe-0.6.2/amazon_transcribe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon-transcribe-0.6.1/setup.py` & `amazon-transcribe-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     version_file = read(*file_paths)
     version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", version_file, re.M)
     if version_match:
         return version_match.group(1)
     raise RuntimeError("Unable to find version string.")
 
 
-requires = ["awscrt~=0.14.0"]
+requires = ["awscrt~=0.16.0"]
 
 setup(
     name="amazon-transcribe",
     version=find_version("amazon_transcribe", "__init__.py"),
     description="Async Python SDK for Amazon Transcribe Streaming",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
```

