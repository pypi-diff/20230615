# Comparing `tmp/pyPhasesRecordloader-0.3.8.tar.gz` & `tmp/pyPhasesRecordloader-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesRecordloader-0.3.8.tar", last modified: Fri Mar 24 09:46:06 2023, max compression
+gzip compressed data, was "pyPhasesRecordloader-0.3.9.tar", last modified: Sat Mar 25 12:46:56 2023, max compression
```

## Comparing `pyPhasesRecordloader-0.3.8.tar` & `pyPhasesRecordloader-0.3.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 09:46:06.385662 pyPhasesRecordloader-0.3.8/
--rw-rw-rw-   0 root         (0) root         (0)     1086 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1549 2023-03-24 09:46:06.384663 pyPhasesRecordloader-0.3.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 09:46:06.377665 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/Event.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/NormalizeRecordSignal.py
--rw-rw-rw-   0 root         (0) root         (0)     3330 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     7294 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/RecordLoader.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/RecordManager.py
--rw-rw-rw-   0 root         (0) root         (0)    16936 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/RecordSignal.py
--rw-rw-rw-   0 root         (0) root         (0)    17252 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/Signal.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 09:46:06.381664 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/downloader/
--rw-rw-rw-   0 root         (0) root         (0)     4641 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/downloader/Downloader.py
--rw-rw-rw-   0 root         (0) root         (0)     1980 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/downloader/FolderDownloader.py
--rw-rw-rw-   0 root         (0) root         (0)     4433 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/downloader/ListDownloader.py
--rw-rw-rw-   0 root         (0) root         (0)     3971 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/downloader/NSRRDownloader.py
--rw-rw-rw-   0 root         (0) root         (0)     1546 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/downloader/S3Downloader.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/downloader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 09:46:06.383663 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/recordLoaders/
--rw-rw-rw-   0 root         (0) root         (0)     6693 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/recordLoaders/EDFRecordLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     1647 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/recordLoaders/H5RecordLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     1223 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/recordLoaders/MatRecordLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     3088 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/recordLoaders/WFDBRecordLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/recordLoaders/XMLAnnotationLoader.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/recordLoaders/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 09:46:06.384663 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/util/
--rw-rw-rw-   0 root         (0) root         (0)     1098 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/util/DynamicModule.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 09:46:06.379665 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1549 2023-03-24 09:46:06.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1247 2023-03-24 09:46:06.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-24 09:46:06.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-03-24 09:46:06.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-03-24 09:46:06.000000 pyPhasesRecordloader-0.3.8/pyPhasesRecordloader.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-03-24 09:45:42.000000 pyPhasesRecordloader-0.3.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-24 09:46:06.385662 pyPhasesRecordloader-0.3.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-03-24 09:45:43.000000 pyPhasesRecordloader-0.3.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-25 12:46:56.170235 pyPhasesRecordloader-0.3.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1549 2023-03-25 12:46:56.170235 pyPhasesRecordloader-0.3.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-25 12:46:56.162234 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/
+-rw-rw-rw-   0 root         (0) root         (0)     1887 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/Event.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/NormalizeRecordSignal.py
+-rw-rw-rw-   0 root         (0) root         (0)     3330 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     7294 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/RecordLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/RecordManager.py
+-rw-rw-rw-   0 root         (0) root         (0)    16936 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/RecordSignal.py
+-rw-rw-rw-   0 root         (0) root         (0)    17252 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/Signal.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-25 12:46:56.166234 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/downloader/
+-rw-rw-rw-   0 root         (0) root         (0)     4641 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/downloader/Downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1980 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/downloader/FolderDownloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     4433 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/downloader/ListDownloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     3971 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/downloader/NSRRDownloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1546 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/downloader/S3Downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/downloader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-25 12:46:56.169234 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/recordLoaders/
+-rw-rw-rw-   0 root         (0) root         (0)     6693 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/recordLoaders/EDFRecordLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1647 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/recordLoaders/H5RecordLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1223 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/recordLoaders/MatRecordLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     3088 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/recordLoaders/WFDBRecordLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/recordLoaders/XMLAnnotationLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/recordLoaders/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-25 12:46:56.169234 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/util/
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/util/DynamicModule.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-25 12:46:56.164234 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1549 2023-03-25 12:46:56.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1247 2023-03-25 12:46:56.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-25 12:46:56.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-03-25 12:46:56.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-03-25 12:46:56.000000 pyPhasesRecordloader-0.3.9/pyPhasesRecordloader.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-03-25 12:46:31.000000 pyPhasesRecordloader-0.3.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-25 12:46:56.170235 pyPhasesRecordloader-0.3.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-03-25 12:46:32.000000 pyPhasesRecordloader-0.3.9/setup.py
```

### Comparing `pyPhasesRecordloader-0.3.8/LICENSE` & `pyPhasesRecordloader-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.3.8/PKG-INFO` & `pyPhasesRecordloader-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesRecordloader
-Version: 0.3.8
+Version: 0.3.9
 Summary: Adds a record loaders to the pyPhases package
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesrecordloader/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesRecordloader-0.3.8/README.md` & `pyPhasesRecordloader-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/Event.py` & `pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/Event.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,14 +33,22 @@
             "power": self.power,
             "frequency": self.frequency,
             "owner": self.owner,
             "manual": self.manual,
             "data": self.data,
         }
 
+    @classmethod
+    def fromdict(cls, d):
+        return cls(
+            name=d["name"] if "name" in d else "",
+            start=d["start"] if "start" in d else 0,
+            duration=d["duration"] if "duration" in d else 0,
+        )
+
 
 class RecordEvents:
     events: dict = {}
     recordId: str = ""
 
     def __init__(self, recordId) -> None:
         self.recordId = recordId
```

### Comparing `pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/NormalizeRecordSignal.py` & `pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/NormalizeRecordSignal.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/Plugin.py` & `pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/RecordLoader.py` & `pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/RecordLoader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/RecordManager.py` & `pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/RecordManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/RecordSignal.py` & `pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/RecordSignal.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/Signal.py` & `pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/Signal.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/downloader/Downloader.py` & `pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/downloader/Downloader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/downloader/FolderDownloader.py` & `pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/downloader/FolderDownloader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/downloader/ListDownloader.py` & `pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/downloader/ListDownloader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/downloader/NSRRDownloader.py` & `pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/downloader/NSRRDownloader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/downloader/S3Downloader.py` & `pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/downloader/S3Downloader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/recordLoaders/EDFRecordLoader.py` & `pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/recordLoaders/EDFRecordLoader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/recordLoaders/H5RecordLoader.py` & `pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/recordLoaders/H5RecordLoader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/recordLoaders/MatRecordLoader.py` & `pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/recordLoaders/MatRecordLoader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/recordLoaders/WFDBRecordLoader.py` & `pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/recordLoaders/WFDBRecordLoader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/recordLoaders/XMLAnnotationLoader.py` & `pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/recordLoaders/XMLAnnotationLoader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.3.8/pyPhasesRecordloader/util/DynamicModule.py` & `pyPhasesRecordloader-0.3.9/pyPhasesRecordloader/util/DynamicModule.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.3.8/pyPhasesRecordloader.egg-info/PKG-INFO` & `pyPhasesRecordloader-0.3.9/pyPhasesRecordloader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesRecordloader
-Version: 0.3.8
+Version: 0.3.9
 Summary: Adds a record loaders to the pyPhases package
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesrecordloader/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesRecordloader-0.3.8/pyPhasesRecordloader.egg-info/SOURCES.txt` & `pyPhasesRecordloader-0.3.9/pyPhasesRecordloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.3.8/setup.py` & `pyPhasesRecordloader-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesRecordloader",
-    version="v0.3.8"[1:],
+    version="v0.3.9"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="Adds a record loaders to the pyPhases package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesrecordloader/",
     packages=setuptools.find_packages(),
```

