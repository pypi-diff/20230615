# Comparing `tmp/Geode_Hybrid-2.0.4rc1-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Hybrid-2.0.4rc2-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,10 @@
-Zip file size: 2409 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      170 b- defN 23-Jun-14 22:12 geode_hybrid/__init__.py
--rw-rw-rw-  2.0 fat      234 b- defN 23-Jun-14 22:12 geode_hybrid/brep.py
--rw-rw-rw-  2.0 fat     2245 b- defN 23-Jun-14 22:12 Geode_Hybrid-2.0.4rc1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-14 22:12 Geode_Hybrid-2.0.4rc1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Jun-14 22:12 Geode_Hybrid-2.0.4rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      487 b- defN 23-Jun-14 22:12 Geode_Hybrid-2.0.4rc1.dist-info/RECORD
-6 files, 3249 bytes uncompressed, 1523 bytes compressed:  53.1%
+Zip file size: 145695 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-14 22:45 geode_hybrid/__init__.py
+-rw-r--r--  2.0 unx      225 b- defN 23-Jun-14 22:45 geode_hybrid/brep.py
+-rwxr-xr-x  2.0 unx   138784 b- defN 23-Jun-14 22:46 geode_hybrid/lib64/geode_hybrid_py_brep.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   213704 b- defN 23-Jun-14 22:46 geode_hybrid/lib64/libGeode-Hybrid_brep.so
+-rw-r--r--  2.0 unx     2182 b- defN 23-Jun-14 22:46 Geode_Hybrid-2.0.4rc2.dist-info/METADATA
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-14 22:46 Geode_Hybrid-2.0.4rc2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-14 22:46 Geode_Hybrid-2.0.4rc2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      716 b- defN 23-Jun-14 22:46 Geode_Hybrid-2.0.4rc2.dist-info/RECORD
+8 files, 355793 bytes uncompressed, 144433 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -1,19 +1,25 @@
 Filename: geode_hybrid/__init__.py
 Comment: 
 
 Filename: geode_hybrid/brep.py
 Comment: 
 
-Filename: Geode_Hybrid-2.0.4rc1.dist-info/METADATA
+Filename: geode_hybrid/lib64/geode_hybrid_py_brep.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: Geode_Hybrid-2.0.4rc1.dist-info/WHEEL
+Filename: geode_hybrid/lib64/libGeode-Hybrid_brep.so
 Comment: 
 
-Filename: Geode_Hybrid-2.0.4rc1.dist-info/top_level.txt
+Filename: Geode_Hybrid-2.0.4rc2.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Hybrid-2.0.4rc1.dist-info/RECORD
+Filename: Geode_Hybrid-2.0.4rc2.dist-info/WHEEL
+Comment: 
+
+Filename: Geode_Hybrid-2.0.4rc2.dist-info/top_level.txt
+Comment: 
+
+Filename: Geode_Hybrid-2.0.4rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_hybrid/__init__.py

```diff
@@ -1,6 +1,3 @@
-## Copyright (c) 2019 - 2023 Geode-solutions
-
-import os, pathlib
-os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
-
-from .brep import *
+## Copyright (c) 2019 - 2023 Geode-solutions
+
+from .brep import *
```

## geode_hybrid/brep.py

```diff
@@ -1,11 +1,11 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-import geode_numerics
-import geode_simplex
-
-from .bin.geode_hybrid_py_brep import *
-HybridBRepLibrary.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+import geode_numerics
+import geode_simplex
+
+from .lib64.geode_hybrid_py_brep import *
+HybridBRepLibrary.initialize()
```

## Comparing `Geode_Hybrid-2.0.4rc1.dist-info/METADATA` & `Geode_Hybrid-2.0.4rc2.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,40 @@
-Metadata-Version: 2.1
-Name: Geode-Hybrid
-Version: 2.0.4rc1
-Summary: Hybrid remeshing Geode-solutions OpenGeode module
-Home-page: https://github.com/Geode-solutions/Geode-Hybrid
-Author: Geode-solutions
-Author-email: contact@geode-solutions.com
-License: Proprietary
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Requires-Dist: geode-background (==7.*,>=7.2.1)
-Requires-Dist: geode-common (==26.*,>=26.1.0rc2)
-Requires-Dist: geode-numerics (==3.*,>=3.0.5)
-Requires-Dist: geode-simplex (==6.*,>=6.0.12rc2)
-Requires-Dist: opengeode-core (==14.*,>=14.3.2rc3)
-
-<h1 align="center">Geode-ModuleTemplate_private<sup><i>by Geode-solutions</i></sup></h1>
-<h3 align="center">Template for creating your own OpenGeode private module</h3>
-
-<p align="center">
-  <img src="https://github.com/Geode-solutions/Geode-ModuleTemplate_private/workflows/CI/badge.svg" alt="Build Status">
-  <img src="https://github.com/Geode-solutions/Geode-ModuleTemplate_private/workflows/CD/badge.svg" alt="Deploy Status">
-  <img src="https://codecov.io/gh/Geode-solutions/Geode-ModuleTemplate_private/branch/master/graph/badge.svg" alt="Coverage Status">
-  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-ModuleTemplate_private.svg" alt="Version">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
-  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
-  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
-  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
-  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
-  <a href="https://opengeode-slack-invite.herokuapp.com">
-    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
-  </a>
-
-Copyright (c) 2019 - 2023, Geode-solutions
-
-
+Metadata-Version: 2.1
+Name: Geode-Hybrid
+Version: 2.0.4rc2
+Summary: Hybrid remeshing Geode-solutions OpenGeode module
+Home-page: https://github.com/Geode-solutions/Geode-Hybrid
+Author: Geode-solutions
+Author-email: contact@geode-solutions.com
+License: Proprietary
+Description-Content-Type: text/markdown
+Requires-Dist: geode-background (==7.*,>=7.2.1)
+Requires-Dist: geode-common (==26.*,>=26.1.0rc2)
+Requires-Dist: geode-numerics (==3.*,>=3.0.5)
+Requires-Dist: geode-simplex (==6.*,>=6.0.12rc2)
+Requires-Dist: opengeode-core (==14.*,>=14.3.2rc3)
+
+<h1 align="center">Geode-ModuleTemplate_private<sup><i>by Geode-solutions</i></sup></h1>
+<h3 align="center">Template for creating your own OpenGeode private module</h3>
+
+<p align="center">
+  <img src="https://github.com/Geode-solutions/Geode-ModuleTemplate_private/workflows/CI/badge.svg" alt="Build Status">
+  <img src="https://github.com/Geode-solutions/Geode-ModuleTemplate_private/workflows/CD/badge.svg" alt="Deploy Status">
+  <img src="https://codecov.io/gh/Geode-solutions/Geode-ModuleTemplate_private/branch/master/graph/badge.svg" alt="Coverage Status">
+  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-ModuleTemplate_private.svg" alt="Version">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
+  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
+  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
+  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
+  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
+  <a href="https://opengeode-slack-invite.herokuapp.com">
+    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
+  </a>
+
+Copyright (c) 2019 - 2023, Geode-solutions
```

### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: Geode-Hybrid Version: 2.0.4rc1 Summary: Hybrid
+Metadata-Version: 2.1 Name: Geode-Hybrid Version: 2.0.4rc2 Summary: Hybrid
 remeshing Geode-solutions OpenGeode module Home-page: https://github.com/Geode-
 solutions/Geode-Hybrid Author: Geode-solutions Author-email: contact@geode-
-solutions.com License: Proprietary Platform: UNKNOWN Description-Content-Type:
-text/markdown Requires-Dist: geode-background (==7.*,>=7.2.1) Requires-Dist:
-geode-common (==26.*,>=26.1.0rc2) Requires-Dist: geode-numerics (==3.*,>=3.0.5)
-Requires-Dist: geode-simplex (==6.*,>=6.0.12rc2) Requires-Dist: opengeode-core
+solutions.com License: Proprietary Description-Content-Type: text/markdown
+Requires-Dist: geode-background (==7.*,>=7.2.1) Requires-Dist: geode-common
+(==26.*,>=26.1.0rc2) Requires-Dist: geode-numerics (==3.*,>=3.0.5) Requires-
+Dist: geode-simplex (==6.*,>=6.0.12rc2) Requires-Dist: opengeode-core
 (==14.*,>=14.3.2rc3)
          ****** Geode-ModuleTemplate_privateby Geode-solutions ******
        **** Template for creating your own OpenGeode private module ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
              [Windows support] [Ubuntu support] [Red Hat support]
   [Language] [License] [Semantic-release] [Slack_invite] Copyright (c) 2019 -
                             2023, Geode-solutions
```

