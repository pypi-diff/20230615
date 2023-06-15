# Comparing `tmp/pyarmor.cli.core.themida-3.2.5-cp39-none-any.whl.zip` & `tmp/pyarmor.cli.core.themida-3.2.6-cp39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7831969 bytes, number of entries: 7
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-08 00:21 pyarmor/cli/core/themida/__init__.py
--rwxr-xr-x  2.0 unx  3840030 b- defN 23-Jun-08 00:21 pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd
--rwxr-xr-x  2.0 unx  4941840 b- defN 23-Jun-08 00:21 pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd
--rw-r--r--  2.0 unx      773 b- defN 23-Jun-08 00:21 pyarmor.cli.core.themida-3.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-08 00:21 pyarmor.cli.core.themida-3.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-08 00:21 pyarmor.cli.core.themida-3.2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      690 b- defN 23-Jun-08 00:21 pyarmor.cli.core.themida-3.2.5.dist-info/RECORD
-7 files, 8783456 bytes uncompressed, 7830721 bytes compressed:  10.8%
+Zip file size: 7975751 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-15 04:30 pyarmor/cli/core/themida/__init__.py
+-rwxr-xr-x  2.0 unx  4014110 b- defN 23-Jun-15 04:30 pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd
+-rwxr-xr-x  2.0 unx  4913168 b- defN 23-Jun-15 04:30 pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd
+-rw-r--r--  2.0 unx      773 b- defN 23-Jun-15 04:30 pyarmor.cli.core.themida-3.2.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-15 04:30 pyarmor.cli.core.themida-3.2.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-15 04:30 pyarmor.cli.core.themida-3.2.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      690 b- defN 23-Jun-15 04:30 pyarmor.cli.core.themida-3.2.6.dist-info/RECORD
+7 files, 8928864 bytes uncompressed, 7974503 bytes compressed:  10.7%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd
 Comment: 
 
 Filename: pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd
 Comment: 
 
-Filename: pyarmor.cli.core.themida-3.2.5.dist-info/METADATA
+Filename: pyarmor.cli.core.themida-3.2.6.dist-info/METADATA
 Comment: 
 
-Filename: pyarmor.cli.core.themida-3.2.5.dist-info/WHEEL
+Filename: pyarmor.cli.core.themida-3.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: pyarmor.cli.core.themida-3.2.5.dist-info/top_level.txt
+Filename: pyarmor.cli.core.themida-3.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: pyarmor.cli.core.themida-3.2.5.dist-info/RECORD
+Filename: pyarmor.cli.core.themida-3.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyarmor/cli/core/themida/__init__.py

```diff
@@ -1 +1 @@
-__VERSION__ = '3.2.5'
+__VERSION__ = '3.2.6'
```

## Comparing `pyarmor.cli.core.themida-3.2.5.dist-info/METADATA` & `pyarmor.cli.core.themida-3.2.6.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarmor.cli.core.themida
-Version: 3.2.5
+Version: 3.2.6
 Summary: Provide extension module pytransform3 for Pyarmor
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pyarmor.cli.core.themida-3.2.5.dist-info/RECORD` & `pyarmor.cli.core.themida-3.2.6.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-pyarmor/cli/core/themida/__init__.py,sha256=J1hdDnxUFUK4kXQSX36fVlrqnTdkaiD__YHllZu6Nzs,22
-pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd,sha256=NPa3pjY-GSqRM_nOjUBLkox6EGsHK7CnxZWcioj7B_0,3840030
-pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd,sha256=pXvjl4PTIKqdQfUR-zXqHSLzvg6adyGsvg85l1Zy2fI,4941840
-pyarmor.cli.core.themida-3.2.5.dist-info/METADATA,sha256=E-eY3SOgugpFpSlguMhHsXpp9G88-r_7EczyOzcAX1g,773
-pyarmor.cli.core.themida-3.2.5.dist-info/WHEEL,sha256=QbbyyBnlPXzoGKd-349G69XkCwSd1NFnt4kuAN58gNs,93
-pyarmor.cli.core.themida-3.2.5.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
-pyarmor.cli.core.themida-3.2.5.dist-info/RECORD,,
+pyarmor/cli/core/themida/__init__.py,sha256=EEOS7QK-aUBPMbsbHCO4KWvy47RPymoUq5zl-Ijg6N8,22
+pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd,sha256=i5eQaG25MzsTq8yBDPlHd6MTlmC1A-m48FQDWPfoqwI,4014110
+pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd,sha256=j323gMj04i6CEQsjfsTuTdXLnfeA3QwKvrKMoI83cew,4913168
+pyarmor.cli.core.themida-3.2.6.dist-info/METADATA,sha256=rkBX4eLkeFTNTAQohB3deZLj3VOrup6CBBo38odezic,773
+pyarmor.cli.core.themida-3.2.6.dist-info/WHEEL,sha256=QbbyyBnlPXzoGKd-349G69XkCwSd1NFnt4kuAN58gNs,93
+pyarmor.cli.core.themida-3.2.6.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
+pyarmor.cli.core.themida-3.2.6.dist-info/RECORD,,
```

