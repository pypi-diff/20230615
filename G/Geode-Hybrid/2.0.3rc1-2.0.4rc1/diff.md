# Comparing `tmp/Geode_Hybrid-2.0.3rc1-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Hybrid-2.0.4rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,8 @@
-Zip file size: 1111029 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      170 b- defN 23-May-31 11:34 geode_hybrid/__init__.py
--rw-rw-rw-  2.0 fat      234 b- defN 23-May-31 11:34 geode_hybrid/brep.py
--rw-rw-rw-  2.0 fat  2164224 b- defN 23-May-31 11:34 geode_hybrid/bin/Geode-Hybrid_brep.dll
--rw-rw-rw-  2.0 fat   136704 b- defN 23-May-31 11:34 geode_hybrid/bin/geode_hybrid_py_brep.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2249 b- defN 23-May-31 11:34 Geode_Hybrid-2.0.3rc1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-31 11:34 Geode_Hybrid-2.0.3rc1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-May-31 11:34 Geode_Hybrid-2.0.3rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      700 b- defN 23-May-31 11:34 Geode_Hybrid-2.0.3rc1.dist-info/RECORD
-8 files, 2304394 bytes uncompressed, 1109803 bytes compressed:  51.8%
+Zip file size: 2409 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      170 b- defN 23-Jun-14 22:12 geode_hybrid/__init__.py
+-rw-rw-rw-  2.0 fat      234 b- defN 23-Jun-14 22:12 geode_hybrid/brep.py
+-rw-rw-rw-  2.0 fat     2245 b- defN 23-Jun-14 22:12 Geode_Hybrid-2.0.4rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-14 22:12 Geode_Hybrid-2.0.4rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Jun-14 22:12 Geode_Hybrid-2.0.4rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      487 b- defN 23-Jun-14 22:12 Geode_Hybrid-2.0.4rc1.dist-info/RECORD
+6 files, 3249 bytes uncompressed, 1523 bytes compressed:  53.1%
```

## zipnote {}

```diff
@@ -1,25 +1,19 @@
 Filename: geode_hybrid/__init__.py
 Comment: 
 
 Filename: geode_hybrid/brep.py
 Comment: 
 
-Filename: geode_hybrid/bin/Geode-Hybrid_brep.dll
+Filename: Geode_Hybrid-2.0.4rc1.dist-info/METADATA
 Comment: 
 
-Filename: geode_hybrid/bin/geode_hybrid_py_brep.cp39-win_amd64.pyd
+Filename: Geode_Hybrid-2.0.4rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Hybrid-2.0.3rc1.dist-info/METADATA
+Filename: Geode_Hybrid-2.0.4rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Hybrid-2.0.3rc1.dist-info/WHEEL
-Comment: 
-
-Filename: Geode_Hybrid-2.0.3rc1.dist-info/top_level.txt
-Comment: 
-
-Filename: Geode_Hybrid-2.0.3rc1.dist-info/RECORD
+Filename: Geode_Hybrid-2.0.4rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `Geode_Hybrid-2.0.3rc1.dist-info/METADATA` & `Geode_Hybrid-2.0.4rc1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: Geode-Hybrid
-Version: 2.0.3rc1
+Version: 2.0.4rc1
 Summary: Hybrid remeshing Geode-solutions OpenGeode module
 Home-page: https://github.com/Geode-solutions/Geode-Hybrid
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: geode-background (==7.*,>=7.2.0rc2)
-Requires-Dist: geode-common (==26.*,>=26.0.0rc1)
-Requires-Dist: geode-numerics (==3.*,>=3.0.4)
-Requires-Dist: geode-simplex (==6.*,>=6.0.11rc1)
-Requires-Dist: opengeode-core (==14.*,>=14.1.10rc5)
+Requires-Dist: geode-background (==7.*,>=7.2.1)
+Requires-Dist: geode-common (==26.*,>=26.1.0rc2)
+Requires-Dist: geode-numerics (==3.*,>=3.0.5)
+Requires-Dist: geode-simplex (==6.*,>=6.0.12rc2)
+Requires-Dist: opengeode-core (==14.*,>=14.3.2rc3)
 
 <h1 align="center">Geode-ModuleTemplate_private<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Template for creating your own OpenGeode private module</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/Geode-ModuleTemplate_private/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/Geode-ModuleTemplate_private/workflows/CD/badge.svg" alt="Deploy Status">
```

### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: Geode-Hybrid Version: 2.0.3rc1 Summary: Hybrid
+Metadata-Version: 2.1 Name: Geode-Hybrid Version: 2.0.4rc1 Summary: Hybrid
 remeshing Geode-solutions OpenGeode module Home-page: https://github.com/Geode-
 solutions/Geode-Hybrid Author: Geode-solutions Author-email: contact@geode-
 solutions.com License: Proprietary Platform: UNKNOWN Description-Content-Type:
-text/markdown Requires-Dist: geode-background (==7.*,>=7.2.0rc2) Requires-Dist:
-geode-common (==26.*,>=26.0.0rc1) Requires-Dist: geode-numerics (==3.*,>=3.0.4)
-Requires-Dist: geode-simplex (==6.*,>=6.0.11rc1) Requires-Dist: opengeode-core
-(==14.*,>=14.1.10rc5)
+text/markdown Requires-Dist: geode-background (==7.*,>=7.2.1) Requires-Dist:
+geode-common (==26.*,>=26.1.0rc2) Requires-Dist: geode-numerics (==3.*,>=3.0.5)
+Requires-Dist: geode-simplex (==6.*,>=6.0.12rc2) Requires-Dist: opengeode-core
+(==14.*,>=14.3.2rc3)
          ****** Geode-ModuleTemplate_privateby Geode-solutions ******
        **** Template for creating your own OpenGeode private module ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
              [Windows support] [Ubuntu support] [Red Hat support]
   [Language] [License] [Semantic-release] [Slack_invite] Copyright (c) 2019 -
                             2023, Geode-solutions
```

