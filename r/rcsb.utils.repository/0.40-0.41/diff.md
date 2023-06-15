# Comparing `tmp/rcsb.utils.repository-0.40.tar.gz` & `tmp/rcsb.utils.repository-0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.repository-0.40.tar", last modified: Mon May 22 13:48:37 2023, max compression
+gzip compressed data, was "rcsb.utils.repository-0.41.tar", last modified: Thu Jun 15 19:35:09 2023, max compression
```

## Comparing `rcsb.utils.repository-0.40.tar` & `rcsb.utils.repository-0.41.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:48:37.645387 rcsb.utils.repository-0.40/
--rw-r--r--   0 vsts      (1001) docker     (122)     3079 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      114 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1941 2023-05-22 13:48:37.645387 rcsb.utils.repository-0.40/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1242 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:48:37.641387 rcsb.utils.repository-0.40/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:48:37.641387 rcsb.utils.repository-0.40/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:48:37.645387 rcsb.utils.repository-0.40/rcsb/utils/repository/
--rw-r--r--   0 vsts      (1001) docker     (122)    14690 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/rcsb/utils/repository/CurrentHoldingsProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15458 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/rcsb/utils/repository/RemovedHoldingsProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    64933 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/rcsb/utils/repository/RepositoryProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19042 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/rcsb/utils/repository/ScanRepoUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5420 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/rcsb/utils/repository/UnreleasedHoldingsProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4113 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/rcsb/utils/repository/UpdateHoldingsProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)      154 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/rcsb/utils/repository/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:48:37.641387 rcsb.utils.repository-0.40/rcsb.utils.repository.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1941 2023-05-22 13:48:37.000000 rcsb.utils.repository-0.40/rcsb.utils.repository.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      699 2023-05-22 13:48:37.000000 rcsb.utils.repository-0.40/rcsb.utils.repository.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-22 13:48:37.000000 rcsb.utils.repository-0.40/rcsb.utils.repository.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-22 13:48:36.000000 rcsb.utils.repository-0.40/rcsb.utils.repository.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-05-22 13:48:37.000000 rcsb.utils.repository-0.40/rcsb.utils.repository.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-22 13:48:37.000000 rcsb.utils.repository-0.40/rcsb.utils.repository.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      165 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-05-22 13:48:37.645387 rcsb.utils.repository-0.40/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2236 2023-05-22 13:41:22.000000 rcsb.utils.repository-0.40/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-15 19:35:09.021176 rcsb.utils.repository-0.41/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3155 2023-06-15 19:24:19.000000 rcsb.utils.repository-0.41/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-06-15 19:24:19.000000 rcsb.utils.repository-0.41/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      114 2023-06-15 19:24:19.000000 rcsb.utils.repository-0.41/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1941 2023-06-15 19:35:09.021176 rcsb.utils.repository-0.41/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1242 2023-06-15 19:24:19.000000 rcsb.utils.repository-0.41/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-15 19:35:09.021176 rcsb.utils.repository-0.41/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-15 19:24:19.000000 rcsb.utils.repository-0.41/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-15 19:35:09.021176 rcsb.utils.repository-0.41/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-15 19:24:19.000000 rcsb.utils.repository-0.41/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-15 19:35:09.021176 rcsb.utils.repository-0.41/rcsb/utils/repository/
+-rw-r--r--   0 vsts      (1001) docker     (122)    14788 2023-06-15 19:24:19.000000 rcsb.utils.repository-0.41/rcsb/utils/repository/CurrentHoldingsProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15556 2023-06-15 19:24:19.000000 rcsb.utils.repository-0.41/rcsb/utils/repository/RemovedHoldingsProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    64927 2023-06-15 19:24:19.000000 rcsb.utils.repository-0.41/rcsb/utils/repository/RepositoryProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19042 2023-06-15 19:24:19.000000 rcsb.utils.repository-0.41/rcsb/utils/repository/ScanRepoUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5518 2023-06-15 19:24:19.000000 rcsb.utils.repository-0.41/rcsb/utils/repository/UnreleasedHoldingsProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4211 2023-06-15 19:24:19.000000 rcsb.utils.repository-0.41/rcsb/utils/repository/UpdateHoldingsProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      154 2023-06-15 19:24:19.000000 rcsb.utils.repository-0.41/rcsb/utils/repository/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-15 19:35:09.021176 rcsb.utils.repository-0.41/rcsb.utils.repository.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1941 2023-06-15 19:35:08.000000 rcsb.utils.repository-0.41/rcsb.utils.repository.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      699 2023-06-15 19:35:08.000000 rcsb.utils.repository-0.41/rcsb.utils.repository.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-15 19:35:08.000000 rcsb.utils.repository-0.41/rcsb.utils.repository.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-15 19:35:07.000000 rcsb.utils.repository-0.41/rcsb.utils.repository.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-06-15 19:35:08.000000 rcsb.utils.repository-0.41/rcsb.utils.repository.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-06-15 19:35:08.000000 rcsb.utils.repository-0.41/rcsb.utils.repository.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      165 2023-06-15 19:24:19.000000 rcsb.utils.repository-0.41/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-06-15 19:35:09.025176 rcsb.utils.repository-0.41/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2236 2023-06-15 19:24:19.000000 rcsb.utils.repository-0.41/setup.py
```

### Comparing `rcsb.utils.repository-0.40/HISTORY.txt` & `rcsb.utils.repository-0.41/HISTORY.txt`

 * *Files 3% similar despite different names*

```diff
@@ -30,7 +30,8 @@
                     Update getSupersededBy method to recursively return all superseded entries
 20-Apr-2022 - V0.35 Fix issue in RepositoryProvider for mapping source and internal computed-model IDs
 03-Aug-2022 - V0.36 Enable retrieval of specific model files with input
 23-Dec-2022 - V0.37 Configuration changes to support tox 4
 14-Feb-2023 - V0.38 Add support for requesting specific inputIdCodeList/idCodeList for CSMs
 22-Mar-2023 - V0.39 Update references to py-rcsb_exdb_assets master branch
 19-May-2023 - V0.40 Update DNS to PDB archive
+12-Jun-2023 - V0.41 Disable useCache for holdings files to force re-download
```

### Comparing `rcsb.utils.repository-0.40/LICENSE` & `rcsb.utils.repository-0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.repository-0.40/PKG-INFO` & `rcsb.utils.repository-0.41/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.repository
-Version: 0.40
+Version: 0.41
 Summary: RCSB Python Repository Data Management Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_repository
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.repository-0.40/README.md` & `rcsb.utils.repository-0.41/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.repository-0.40/rcsb/utils/repository/CurrentHoldingsProvider.py` & `rcsb.utils.repository-0.41/rcsb/utils/repository/CurrentHoldingsProvider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 ##
 #  File:  CurrentHoldingsProvider.py
 #  Date:  18-May-2021 jdw
 #
 #  Updates:
+#   12-Jun-2023  dwp Set useCache default to False to force redownloading of holdings files
 #
 ##
 """Provide inventory of current repository content.
 """
 
 import datetime
 import logging
@@ -20,15 +21,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class CurrentHoldingsProvider(object):
     """Provide inventory of current repository content."""
 
-    def __init__(self, cachePath, useCache, **kwargs):
+    def __init__(self, cachePath, useCache=False, **kwargs):
         self.__cachePath = cachePath
         self.__dirPath = os.path.join(cachePath, "holdings")
         #
         edMapsLocator = kwargs.get("edmapsLocator", "https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/fall_back/edmaps.json")
         #
         baseUrl = kwargs.get("holdingsTargetUrl", "https://files.wwpdb.org/pub/pdb/holdings")
         fallbackUrl = kwargs.get("holdingsFallbackUrl", "https://files.wwpdb.org/pub/pdb/holdings")
```

### Comparing `rcsb.utils.repository-0.40/rcsb/utils/repository/RemovedHoldingsProvider.py` & `rcsb.utils.repository-0.41/rcsb/utils/repository/RemovedHoldingsProvider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ##
 #  File:  RemovedHoldingsProvider.py
 #  Date:  18-May-2021 jdw
 #
 #  Updates:
 #   18-Apr-2022  dwp Update getSupersededBy method to recursively return all superseded entries
+#   12-Jun-2023  dwp Set useCache default to False to force redownloading of holdings files
 ##
 """Provide an inventory of removed repository content.
 """
 import logging
 import os.path
 
 import dateutil.parser
@@ -16,15 +17,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class RemovedHoldingsProvider(object):
     """Provide an inventory of removed repository content."""
 
-    def __init__(self, cachePath, useCache, **kwargs):
+    def __init__(self, cachePath, useCache=False, **kwargs):
         self.__cachePath = cachePath
         self.__dirPath = os.path.join(self.__cachePath, "holdings")
         self.__filterType = kwargs.get("filterType", "")
         self.__assignDates = "assign-dates" in self.__filterType
         baseUrl = kwargs.get("holdingsTargetUrl", "https://files.wwpdb.org/pub/pdb/holdings")
         fallbackUrl = kwargs.get("holdingsFallbackUrl", "https://files.wwpdb.org/pub/pdb/holdings")
         #
```

### Comparing `rcsb.utils.repository-0.40/rcsb/utils/repository/RepositoryProvider.py` & `rcsb.utils.repository-0.41/rcsb/utils/repository/RepositoryProvider.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 #    8-Oct-2021  jdw pass configuration URLs to CurrentHoldingsProvider and RemoveHoldingsProvider
 #                    ValidationReportProvider() migrated to ValidationReportAdapter()
 #    8-Oct-2021  jdw add warning messages for empty read/merge container results in method __mergeContainers()
 #    5-Apr-2022  dwp Add support for loading id code lists for bird_chem_comp_core (mainly used for Azure testing)
 #   13-Apr-2022  dwp Update methods for obtaining list of computed-model files
 #    3-Aug-2022  dwp Enable retrieval of specific computed-model files with input
 #    2-Feb-2023  dwp add support for requesting specific inputIdCodeList/idCodeList for CSMs
+#   12-Jun-2023  dwp disable useCache for holdings files to force fresh re-download
 ##
 """
 Utilities for scanning and accessing data in PDBx/mmCIF data in common repository file systems or via remote repository services.
 
 """
 __docformat__ = "restructuredtext en"
 __author__ = "John Westbrook"
@@ -529,15 +530,15 @@
         return pth
 
     # JDW ---  URI code ----
     def __getEntryUriList(self, idCodeList=None, mergeContentTypes=None):
         uL = []
         try:
             if not self.__chP:
-                self.__chP = CurrentHoldingsProvider(self.__topCachePath, useCache=True, **self.__kwD)
+                self.__chP = CurrentHoldingsProvider(self.__topCachePath, **self.__kwD)
             #
             tIdL = self.__chP.getEntryIdList()
             if idCodeList:
                 tIdD = dict.fromkeys(tIdL, True)
                 tIdL = [idCode.upper() for idCode in idCodeList if idCode.upper() in tIdD]
                 # idCodeList = [t.upper() for t in idCodeList]
                 # tIdL = list(set(tIdL).intersection(idCodeList))
@@ -556,15 +557,15 @@
             logger.exception("Failing with %s", str(e))
         return self.__applyLimit(uL)
 
     def __getObsoleteEntryUriList(self, idCodeList=None):
         uL = []
         try:
             if not self.__rhP:
-                self.__rhP = RemovedHoldingsProvider(self.__topCachePath, useCache=True, **self.__kwD)
+                self.__rhP = RemovedHoldingsProvider(self.__topCachePath, **self.__kwD)
             #
             tIdL = self.__rhP.getEntryByStatus("OBS")
             if idCodeList:
                 tIdD = dict.fromkeys(tIdL, True)
                 tIdL = [idCode.upper() for idCode in idCodeList if idCode.upper() in tIdD]
                 logger.info("idCodeList selected: %r", tIdL)
             #
@@ -576,15 +577,15 @@
             logger.exception("Failing with %s", str(e))
         return self.__applyLimit(uL)
 
     def __getBirdUriList(self, idCodeList=None):
         uL = []
         try:
             if not self.__chP:
-                self.__chP = CurrentHoldingsProvider(self.__topCachePath, useCache=True, **self.__kwD)
+                self.__chP = CurrentHoldingsProvider(self.__topCachePath, **self.__kwD)
             #
             tIdL = self.__chP.getBirdIdList()
             if idCodeList:
                 tIdD = dict.fromkeys(tIdL, True)
                 tIdL = [idCode.upper() for idCode in idCodeList if idCode.upper() in tIdD]
                 logger.info("idCodeList selected: %r", tIdL)
             #
@@ -595,15 +596,15 @@
             logger.exception("Failing with %s", str(e))
         return self.__applyLimit(uL)
 
     def __getBirdFamilyUriList(self, idCodeList=None):
         uL = []
         try:
             if not self.__chP:
-                self.__chP = CurrentHoldingsProvider(self.__topCachePath, useCache=True, **self.__kwD)
+                self.__chP = CurrentHoldingsProvider(self.__topCachePath, **self.__kwD)
             #
             tIdL = self.__chP.getBirdFamilyIdList()
             if idCodeList:
                 tIdD = dict.fromkeys(tIdL, True)
                 tIdL = [idCode.upper() for idCode in idCodeList if idCode.upper() in tIdD]
                 logger.info("idCodeList selected: %r", tIdL)
             #
@@ -614,15 +615,15 @@
             logger.exception("Failing with %s", str(e))
         return self.__applyLimit(uL)
 
     def __getChemCompUriList(self, idCodeList=None):
         uL = []
         try:
             if not self.__chP:
-                self.__chP = CurrentHoldingsProvider(self.__topCachePath, useCache=True, **self.__kwD)
+                self.__chP = CurrentHoldingsProvider(self.__topCachePath, **self.__kwD)
             #
             tIdL = self.__chP.getChemCompIdList()
             if idCodeList:
                 tIdD = dict.fromkeys(tIdL, True)
                 tIdL = [idCode.upper() for idCode in idCodeList if idCode.upper() in tIdD]
                 logger.info("idCodeList selected: %r", tIdL)
             #
@@ -633,15 +634,15 @@
             logger.exception("Failing with %s", str(e))
         return self.__applyLimit(uL)
 
     def __getBirdChemCompUriList(self, idCodeList=None):
         uL = []
         try:
             if not self.__chP:
-                self.__chP = CurrentHoldingsProvider(self.__topCachePath, useCache=True, **self.__kwD)
+                self.__chP = CurrentHoldingsProvider(self.__topCachePath, **self.__kwD)
             #
             tIdL = self.__chP.getBirdChemCompIdList()
             if idCodeList:
                 tIdD = dict.fromkeys(tIdL, True)
                 tIdL = [idCode.upper() for idCode in idCodeList if idCode.upper() in tIdD]
                 logger.info("idCodeList selected: %r", tIdL)
             #
```

### Comparing `rcsb.utils.repository-0.40/rcsb/utils/repository/ScanRepoUtil.py` & `rcsb.utils.repository-0.41/rcsb/utils/repository/ScanRepoUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.repository-0.40/rcsb/utils/repository/UnreleasedHoldingsProvider.py` & `rcsb.utils.repository-0.41/rcsb/utils/repository/UnreleasedHoldingsProvider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 ##
 #  File:  UnreleasedHoldingsProvider.py
 #  Date:  24-Sep-2021 jdw
 #
 #  Updates:
+#   12-Jun-2023  dwp Set useCache default to False to force redownloading of holdings files
 #
 ##
 """Provide an inventory of unreleased repository content.
 """
 
 import logging
 import os.path
@@ -17,15 +18,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class UnreleasedHoldingsProvider(object):
     """Provide an inventory of unreleased repository content."""
 
-    def __init__(self, cachePath, useCache, **kwargs):
+    def __init__(self, cachePath, useCache=False, **kwargs):
         self.__dirPath = os.path.join(cachePath, "holdings")
         self.__filterType = kwargs.get("filterType", "")
         self.__assignDates = "assign-dates" in self.__filterType
         baseUrl = kwargs.get("holdingsTargetUrl", "https://files.wwpdb.org/pub/pdb/holdings")
         fallbackUrl = kwargs.get("holdingsFallbackUrl", "https://files.wwpdb.org/pub/pdb/holdings")
         #
         urlTarget = os.path.join(baseUrl, "unreleased_entries.json.gz")
```

### Comparing `rcsb.utils.repository-0.40/rcsb/utils/repository/UpdateHoldingsProvider.py` & `rcsb.utils.repository-0.41/rcsb/utils/repository/UpdateHoldingsProvider.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 ##
 #  File:  UpdateHoldingsProvider.py
 #  Date:  18-Sep-2021 jdw
 #
 #  Updates:
+#   12-Jun-2023  dwp Set useCache default to False to force redownloading of holdings files
 #
 ##
 """Provide inventory of current repository update.
 """
 
 import collections
 import logging
@@ -16,15 +17,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class UpdateHoldingsProvider(object):
     """Provide inventory of the current repository update."""
 
-    def __init__(self, cachePath, useCache, **kwargs):
+    def __init__(self, cachePath, useCache=False, **kwargs):
         self.__dirPath = os.path.join(cachePath, "holdings")
         #
         baseUrl = kwargs.get("updateTargetUrl", "https://files.wwpdb.org/pub/pdb/data/status/latest")
         fallbackUrl = kwargs.get("updateFallbackUrl", "https://files.wwpdb.org/pub/pdb/data/status/latest")
         #
         self.__mU = MarshalUtil(workPath=self.__dirPath)
         self.__updD = self.__reloadUpdateLists(baseUrl, fallbackUrl, self.__dirPath, useCache=useCache)
```

### Comparing `rcsb.utils.repository-0.40/rcsb.utils.repository.egg-info/PKG-INFO` & `rcsb.utils.repository-0.41/rcsb.utils.repository.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.repository
-Version: 0.40
+Version: 0.41
 Summary: RCSB Python Repository Data Management Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_repository
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.repository-0.40/rcsb.utils.repository.egg-info/SOURCES.txt` & `rcsb.utils.repository-0.41/rcsb.utils.repository.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.repository-0.40/setup.py` & `rcsb.utils.repository-0.41/setup.py`

 * *Files identical despite different names*

