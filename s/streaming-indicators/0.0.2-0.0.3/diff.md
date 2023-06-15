# Comparing `tmp/streaming_indicators-0.0.2.tar.gz` & `tmp/streaming_indicators-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streaming_indicators-0.0.2.tar", last modified: Fri May 12 17:51:55 2023, max compression
+gzip compressed data, was "streaming_indicators-0.0.3.tar", last modified: Thu Jun 15 09:07:42 2023, max compression
```

## Comparing `streaming_indicators-0.0.2.tar` & `streaming_indicators-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 17:51:55.911376 streaming_indicators-0.0.2/
--rw-rw-rw-   0        0        0     1082 2023-05-12 14:45:21.000000 streaming_indicators-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2824 2023-05-12 17:51:55.912381 streaming_indicators-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2023-05-12 15:11:06.000000 streaming_indicators-0.0.2/README.md
--rw-rw-rw-   0        0        0       86 2023-05-12 14:44:06.000000 streaming_indicators-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      847 2023-05-12 17:51:55.914379 streaming_indicators-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-12 17:51:55.875339 streaming_indicators-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-12 17:51:55.887377 streaming_indicators-0.0.2/src/streaming_indicators/
--rw-rw-rw-   0        0        0       35 2023-05-12 17:50:29.000000 streaming_indicators-0.0.2/src/streaming_indicators/__init__.py
--rw-rw-rw-   0        0        0     2966 2023-05-12 13:57:04.000000 streaming_indicators-0.0.2/src/streaming_indicators/streaming_indicators.py
-drwxrwxrwx   0        0        0        0 2023-05-12 17:51:55.910344 streaming_indicators-0.0.2/src/streaming_indicators.egg-info/
--rw-rw-rw-   0        0        0     2824 2023-05-12 17:51:55.000000 streaming_indicators-0.0.2/src/streaming_indicators.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-05-12 17:51:55.000000 streaming_indicators-0.0.2/src/streaming_indicators.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 17:51:55.000000 streaming_indicators-0.0.2/src/streaming_indicators.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-12 17:51:55.000000 streaming_indicators-0.0.2/src/streaming_indicators.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-12 17:51:55.000000 streaming_indicators-0.0.2/src/streaming_indicators.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 09:07:41.969957 streaming_indicators-0.0.3/
+-rw-rw-rw-   0        0        0     1082 2023-05-12 14:45:21.000000 streaming_indicators-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3040 2023-06-15 09:07:41.969957 streaming_indicators-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1283 2023-06-15 08:59:38.000000 streaming_indicators-0.0.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-12 14:44:06.000000 streaming_indicators-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      847 2023-06-15 09:07:42.001960 streaming_indicators-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-15 09:07:41.795809 streaming_indicators-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-15 09:07:41.857708 streaming_indicators-0.0.3/src/streaming_indicators/
+-rw-rw-rw-   0        0        0       35 2023-05-12 17:50:29.000000 streaming_indicators-0.0.3/src/streaming_indicators/__init__.py
+-rw-rw-rw-   0        0        0     6194 2023-06-15 08:56:53.000000 streaming_indicators-0.0.3/src/streaming_indicators/streaming_indicators.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:07:41.969957 streaming_indicators-0.0.3/src/streaming_indicators.egg-info/
+-rw-rw-rw-   0        0        0     3040 2023-06-15 09:07:41.000000 streaming_indicators-0.0.3/src/streaming_indicators.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-06-15 09:07:41.000000 streaming_indicators-0.0.3/src/streaming_indicators.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 09:07:41.000000 streaming_indicators-0.0.3/src/streaming_indicators.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-15 09:07:41.000000 streaming_indicators-0.0.3/src/streaming_indicators.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-15 09:07:41.000000 streaming_indicators-0.0.3/src/streaming_indicators.egg-info/top_level.txt
```

### Comparing `streaming_indicators-0.0.2/LICENSE.txt` & `streaming_indicators-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streaming_indicators-0.0.2/PKG-INFO` & `streaming_indicators-0.0.3/src/streaming_indicators.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: streaming_indicators
-Version: 0.0.2
+Name: streaming-indicators
+Version: 0.0.3
 Summary: A python library for computing technical analysis indicators on streaming data.
 Home-page: https://github.com/mr-easy/streaming_indicators
 Author: Rishabh Gupta
 Author-email: rishabhg1997@gmail.com
 Project-URL: Bug Tracker, https://github.com/mr-easy/streaming_indicators/issues
 Project-URL: Code, https://github.com/mr-easy/streaming_indicators
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,19 @@
 ```
 from streaming_indicators import SMA
 
 sma = SMA(10)
 for i in range(20):
     print(i, sma.update(i))
 ```
+## TODO
+- Not all indicators current support compute method.
+- Add documentation.
+- HeikinAshi depends on key names, eg ('open','close'). Should be independent, i.e. given in input.
+- Implement more indicators.
 MIT License
 
 Copyright (c) [2023] [Rishabh Gupta]
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `streaming_indicators-0.0.2/setup.cfg` & `streaming_indicators-0.0.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7472 6561 6d69 6e67 5f69 6e64   = streaming_ind
 00000020: 6963 6174 6f72 730d 0a76 6572 7369 6f6e  icators..version
-00000030: 203d 2030 2e30 2e32 0d0a 6175 7468 6f72   = 0.0.2..author
+00000030: 203d 2030 2e30 2e33 0d0a 6175 7468 6f72   = 0.0.3..author
 00000040: 203d 2052 6973 6861 6268 2047 7570 7461   = Rishabh Gupta
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2072 6973 6861 6268 6731 3939 3740 676d   rishabhg1997@gm
 00000070: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
 00000080: 7469 6f6e 203d 2041 2070 7974 686f 6e20  tion = A python 
 00000090: 6c69 6272 6172 7920 666f 7220 636f 6d70  library for comp
 000000a0: 7574 696e 6720 7465 6368 6e69 6361 6c20  uting technical
```

### Comparing `streaming_indicators-0.0.2/src/streaming_indicators.egg-info/PKG-INFO` & `streaming_indicators-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: streaming-indicators
-Version: 0.0.2
+Name: streaming_indicators
+Version: 0.0.3
 Summary: A python library for computing technical analysis indicators on streaming data.
 Home-page: https://github.com/mr-easy/streaming_indicators
 Author: Rishabh Gupta
 Author-email: rishabhg1997@gmail.com
 Project-URL: Bug Tracker, https://github.com/mr-easy/streaming_indicators/issues
 Project-URL: Code, https://github.com/mr-easy/streaming_indicators
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,19 @@
 ```
 from streaming_indicators import SMA
 
 sma = SMA(10)
 for i in range(20):
     print(i, sma.update(i))
 ```
+## TODO
+- Not all indicators current support compute method.
+- Add documentation.
+- HeikinAshi depends on key names, eg ('open','close'). Should be independent, i.e. given in input.
+- Implement more indicators.
 MIT License
 
 Copyright (c) [2023] [Rishabh Gupta]
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

