# Comparing `tmp/p4python-2022.2.2428370.tar.gz` & `tmp/p4python-2023.1.2454917.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\p4python-2022.2.2428370.tar", last modified: Thu Apr 13 20:30:59 2023, max compression
+gzip compressed data, was "dist\p4python-2023.1.2454917.tar", last modified: Thu Jun 15 14:38:00 2023, max compression
```

## Comparing `p4python-2022.2.2428370.tar` & `p4python-2023.1.2454917.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 20:30:59.331750 p4python-2022.2.2428370/
--rw-rw-rw-   0        0        0    21560 2021-05-11 08:48:41.000000 p4python-2022.2.2428370/LICENSE.txt
--rw-rw-rw-   0        0        0    38175 2022-06-09 21:28:16.000000 p4python-2022.2.2428370/P4.py
--rw-rw-rw-   0        0        0    47440 2020-07-15 12:24:50.000000 p4python-2022.2.2428370/P4API.cpp
--rw-rw-rw-   0        0        0     9512 2019-05-13 22:27:04.000000 p4python-2022.2.2428370/P4MapMaker.cpp
--rw-rw-rw-   0        0        0     2461 2019-05-13 22:33:26.000000 p4python-2022.2.2428370/P4MapMaker.h
--rw-rw-rw-   0        0        0     3873 2020-06-22 08:59:33.000000 p4python-2022.2.2428370/P4PythonDebug.cpp
--rw-rw-rw-   0        0        0     2466 2014-10-20 13:25:21.000000 p4python-2022.2.2428370/P4PythonDebug.h
--rw-rw-rw-   0        0        0     6570 2020-07-15 16:42:08.000000 p4python-2022.2.2428370/P4Result.cpp
--rw-rw-rw-   0        0        0     3172 2019-05-13 22:01:44.000000 p4python-2022.2.2428370/P4Result.h
--rw-rw-rw-   0        0        0     1162 2023-04-13 20:30:59.331750 p4python-2022.2.2428370/PKG-INFO
--rw-rw-rw-   0        0        0     3884 2012-01-10 14:38:46.000000 p4python-2022.2.2428370/PythonActionMergeData.cpp
--rw-rw-rw-   0        0        0     2278 2012-01-10 14:39:08.000000 p4python-2022.2.2428370/PythonActionMergeData.h
--rw-rw-rw-   0        0        0    31402 2020-07-15 12:31:14.000000 p4python-2022.2.2428370/PythonClientAPI.cpp
--rw-rw-rw-   0        0        0    11794 2019-05-13 22:39:28.000000 p4python-2022.2.2428370/PythonClientAPI.h
--rw-rw-rw-   0        0        0     4287 2015-12-18 16:26:12.000000 p4python-2022.2.2428370/PythonClientProgress.cpp
--rw-rw-rw-   0        0        0     2046 2012-07-19 20:07:01.000000 p4python-2022.2.2428370/PythonClientProgress.h
--rw-rw-rw-   0        0        0    22220 2019-05-13 22:43:14.000000 p4python-2022.2.2428370/PythonClientUser.cpp
--rw-rw-rw-   0        0        0     4531 2019-05-13 22:38:13.000000 p4python-2022.2.2428370/PythonClientUser.h
--rw-rw-rw-   0        0        0     4537 2012-02-24 11:23:48.000000 p4python-2022.2.2428370/PythonMergeData.cpp
--rw-rw-rw-   0        0        0     2540 2011-12-22 10:54:55.000000 p4python-2022.2.2428370/PythonMergeData.h
--rw-rw-rw-   0        0        0     3384 2019-05-13 22:47:37.000000 p4python-2022.2.2428370/PythonMessage.cpp
--rw-rw-rw-   0        0        0     2274 2019-05-13 22:41:23.000000 p4python-2022.2.2428370/PythonMessage.h
--rw-rw-rw-   0        0        0     5665 2022-05-04 15:35:00.000000 p4python-2022.2.2428370/PythonSpecData.cpp
--rw-rw-rw-   0        0        0     2373 2016-06-10 13:11:59.000000 p4python-2022.2.2428370/PythonSpecData.h
--rw-rw-rw-   0        0        0     2417 2009-01-29 11:22:22.000000 p4python-2022.2.2428370/PythonThreadGuard.h
--rw-rw-rw-   0        0        0     2784 2019-05-13 22:31:53.000000 p4python-2022.2.2428370/PythonTypes.h
--rw-rw-rw-   0        0        0    23502 2023-03-07 14:14:52.000000 p4python-2022.2.2428370/SpecMgr.cpp
--rw-rw-rw-   0        0        0     4105 2019-05-13 22:35:53.000000 p4python-2022.2.2428370/SpecMgr.h
--rw-rw-rw-   0        0        0       66 2023-04-13 20:30:28.000000 p4python-2022.2.2428370/Version
--rw-rw-rw-   0        0        0     1057 2017-08-23 20:17:46.000000 p4python-2022.2.2428370/devnotes.txt
--rw-rw-rw-   0        0        0     1257 2020-07-01 07:19:30.000000 p4python-2022.2.2428370/job_trigger.py
--rw-rw-rw-   0        0        0    55429 2021-05-06 10:45:17.000000 p4python-2022.2.2428370/p4test.py
--rw-rw-rw-   0        0        0     2875 2014-10-06 19:20:07.000000 p4python-2022.2.2428370/python2to3.h
--rw-rw-rw-   0        0        0      194 2022-05-03 10:52:22.000000 p4python-2022.2.2428370/setup.cfg
--rw-rw-rw-   0        0        0    19070 2022-10-06 12:00:23.000000 p4python-2022.2.2428370/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:30:59.331750 p4python-2022.2.2428370/tools/
--rw-rw-rw-   0        0        0     9153 2019-09-25 10:38:29.000000 p4python-2022.2.2428370/tools/P4APIFtp.py
--rw-rw-rw-   0        0        0     2346 2022-10-05 16:02:04.000000 p4python-2022.2.2428370/tools/P4APIHttps.py
--rw-rw-rw-   0        0        0     8310 2023-03-27 09:33:08.000000 p4python-2022.2.2428370/tools/PlatformInfo.py
--rw-rw-rw-   0        0        0     1854 2017-06-27 09:52:13.000000 p4python-2022.2.2428370/tools/Version.py
--rw-rw-rw-   0        0        0     2497 2019-03-15 18:55:25.000000 p4python-2022.2.2428370/tools/VersionInfo.py
--rw-rw-rw-   0        0        0       44 2017-06-27 09:04:52.000000 p4python-2022.2.2428370/tools/__init__.py
--rw-rw-rw-   0        0        0     2609 2015-12-14 20:09:07.000000 p4python-2022.2.2428370/undefdups.h
+drwxrwxrwx   0        0        0        0 2023-06-15 14:38:00.736236 p4python-2023.1.2454917/
+-rw-rw-rw-   0        0        0    21560 2021-05-11 08:48:41.000000 p4python-2023.1.2454917/LICENSE.txt
+-rw-rw-rw-   0        0        0    38175 2022-06-09 21:28:16.000000 p4python-2023.1.2454917/P4.py
+-rw-rw-rw-   0        0        0    47440 2020-07-15 12:24:50.000000 p4python-2023.1.2454917/P4API.cpp
+-rw-rw-rw-   0        0        0     9512 2019-05-13 22:27:04.000000 p4python-2023.1.2454917/P4MapMaker.cpp
+-rw-rw-rw-   0        0        0     2461 2019-05-13 22:33:26.000000 p4python-2023.1.2454917/P4MapMaker.h
+-rw-rw-rw-   0        0        0     3873 2020-06-22 08:59:33.000000 p4python-2023.1.2454917/P4PythonDebug.cpp
+-rw-rw-rw-   0        0        0     2466 2014-10-20 13:25:21.000000 p4python-2023.1.2454917/P4PythonDebug.h
+-rw-rw-rw-   0        0        0     6570 2020-07-15 16:42:08.000000 p4python-2023.1.2454917/P4Result.cpp
+-rw-rw-rw-   0        0        0     3172 2019-05-13 22:01:44.000000 p4python-2023.1.2454917/P4Result.h
+-rw-rw-rw-   0        0        0     1162 2023-06-15 14:38:00.736236 p4python-2023.1.2454917/PKG-INFO
+-rw-rw-rw-   0        0        0     3884 2012-01-10 14:38:46.000000 p4python-2023.1.2454917/PythonActionMergeData.cpp
+-rw-rw-rw-   0        0        0     2278 2012-01-10 14:39:08.000000 p4python-2023.1.2454917/PythonActionMergeData.h
+-rw-rw-rw-   0        0        0    31402 2020-07-15 12:31:14.000000 p4python-2023.1.2454917/PythonClientAPI.cpp
+-rw-rw-rw-   0        0        0    11794 2019-05-13 22:39:28.000000 p4python-2023.1.2454917/PythonClientAPI.h
+-rw-rw-rw-   0        0        0     4287 2015-12-18 16:26:12.000000 p4python-2023.1.2454917/PythonClientProgress.cpp
+-rw-rw-rw-   0        0        0     2046 2012-07-19 20:07:01.000000 p4python-2023.1.2454917/PythonClientProgress.h
+-rw-rw-rw-   0        0        0    22220 2019-05-13 22:43:14.000000 p4python-2023.1.2454917/PythonClientUser.cpp
+-rw-rw-rw-   0        0        0     4531 2019-05-13 22:38:13.000000 p4python-2023.1.2454917/PythonClientUser.h
+-rw-rw-rw-   0        0        0     4537 2012-02-24 11:23:48.000000 p4python-2023.1.2454917/PythonMergeData.cpp
+-rw-rw-rw-   0        0        0     2540 2011-12-22 10:54:55.000000 p4python-2023.1.2454917/PythonMergeData.h
+-rw-rw-rw-   0        0        0     3384 2019-05-13 22:47:37.000000 p4python-2023.1.2454917/PythonMessage.cpp
+-rw-rw-rw-   0        0        0     2274 2019-05-13 22:41:23.000000 p4python-2023.1.2454917/PythonMessage.h
+-rw-rw-rw-   0        0        0     5665 2022-05-04 15:35:00.000000 p4python-2023.1.2454917/PythonSpecData.cpp
+-rw-rw-rw-   0        0        0     2373 2016-06-10 13:11:59.000000 p4python-2023.1.2454917/PythonSpecData.h
+-rw-rw-rw-   0        0        0     2417 2009-01-29 11:22:22.000000 p4python-2023.1.2454917/PythonThreadGuard.h
+-rw-rw-rw-   0        0        0     2784 2019-05-13 22:31:53.000000 p4python-2023.1.2454917/PythonTypes.h
+-rw-rw-rw-   0        0        0    23525 2023-06-05 06:48:41.000000 p4python-2023.1.2454917/SpecMgr.cpp
+-rw-rw-rw-   0        0        0     4105 2019-05-13 22:35:53.000000 p4python-2023.1.2454917/SpecMgr.h
+-rw-rw-rw-   0        0        0       66 2023-06-15 14:26:58.000000 p4python-2023.1.2454917/Version
+-rw-rw-rw-   0        0        0     1057 2017-08-23 20:17:46.000000 p4python-2023.1.2454917/devnotes.txt
+-rw-rw-rw-   0        0        0     1257 2020-07-01 07:19:30.000000 p4python-2023.1.2454917/job_trigger.py
+-rw-rw-rw-   0        0        0    55429 2021-05-06 10:45:17.000000 p4python-2023.1.2454917/p4test.py
+-rw-rw-rw-   0        0        0     2875 2014-10-06 19:20:07.000000 p4python-2023.1.2454917/python2to3.h
+-rw-rw-rw-   0        0        0      194 2022-05-03 10:52:22.000000 p4python-2023.1.2454917/setup.cfg
+-rw-rw-rw-   0        0        0    19070 2023-06-06 06:16:56.000000 p4python-2023.1.2454917/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:38:00.735233 p4python-2023.1.2454917/tools/
+-rw-rw-rw-   0        0        0     9153 2019-09-25 10:38:29.000000 p4python-2023.1.2454917/tools/P4APIFtp.py
+-rw-rw-rw-   0        0        0     2346 2022-10-05 16:02:04.000000 p4python-2023.1.2454917/tools/P4APIHttps.py
+-rw-rw-rw-   0        0        0     8310 2023-03-27 09:33:08.000000 p4python-2023.1.2454917/tools/PlatformInfo.py
+-rw-rw-rw-   0        0        0     1854 2017-06-27 09:52:13.000000 p4python-2023.1.2454917/tools/Version.py
+-rw-rw-rw-   0        0        0     2497 2019-03-15 18:55:25.000000 p4python-2023.1.2454917/tools/VersionInfo.py
+-rw-rw-rw-   0        0        0       44 2017-06-27 09:04:52.000000 p4python-2023.1.2454917/tools/__init__.py
+-rw-rw-rw-   0        0        0     2609 2015-12-14 20:09:07.000000 p4python-2023.1.2454917/undefdups.h
```

### Comparing `p4python-2022.2.2428370/LICENSE.txt` & `p4python-2023.1.2454917/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `p4python-2022.2.2428370/P4.py` & `p4python-2023.1.2454917/P4.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import print_function
 
 """A Python version of the Perforce "p4" client.
     
     This uses the Python type P4API.P4Adapter, which is a wrapper for the
     Perforce ClientApi object.
     
-    $Id: //depot/r22.2/p4-python/P4.py#1 $
+    $Id: //depot/r23.1/p4-python/P4.py#1 $
     
     #*******************************************************************************
     # Copyright (c) 2007-2010, Perforce Software, Inc.  All rights reserved.
     # Portions Copyright (c) 1999, Mike Meyer. All rights reserved.
     # Portions Copyright (c) 2004-2007, Robert Cowham. All rights reserved.
     #
     # Redistribution and use in source and binary forms, with or without
```

### Comparing `p4python-2022.2.2428370/P4API.cpp` & `p4python-2023.1.2454917/P4API.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  * DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  * 
- * $Id: //depot/r22.2/p4-python/P4API.cpp#1 $
+ * $Id: //depot/r23.1/p4-python/P4API.cpp#1 $
  *
  * Build instructions:
  *  Use Distutils - see accompanying setup.py
  *
  *      python setup.py install
  *
  */
```

### Comparing `p4python-2022.2.2428370/P4MapMaker.cpp` & `p4python-2023.1.2454917/P4MapMaker.cpp`

 * *Files identical despite different names*

### Comparing `p4python-2022.2.2428370/P4MapMaker.h` & `p4python-2023.1.2454917/P4MapMaker.h`

 * *Files identical despite different names*

### Comparing `p4python-2022.2.2428370/P4PythonDebug.cpp` & `p4python-2023.1.2454917/P4PythonDebug.cpp`

 * *Files identical despite different names*

### Comparing `p4python-2022.2.2428370/P4PythonDebug.h` & `p4python-2023.1.2454917/P4PythonDebug.h`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 * DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 *
-* $Id: //depot/r22.2/p4-python/P4PythonDebug.h#1 $
+* $Id: //depot/r23.1/p4-python/P4PythonDebug.h#1 $
 *
 *******************************************************************************/
 
 #ifndef P4PYTHONDEBUG_H
 # define P4PYTHONDEBUG_H
 
 # define P4PYDBG_COMMANDS	1
```

### Comparing `p4python-2022.2.2428370/P4Result.cpp` & `p4python-2023.1.2454917/P4Result.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-$Id: //depot/r22.2/p4-python/P4Result.cpp#1 $
+$Id: //depot/r23.1/p4-python/P4Result.cpp#1 $
 *******************************************************************************/
 
 #include <Python.h>
 #include <bytesobject.h>
 #include "undefdups.h"
 #include "python2to3.h"
 #include <clientapi.h>
```

### Comparing `p4python-2022.2.2428370/P4Result.h` & `p4python-2023.1.2454917/P4Result.h`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  * DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  * 
- * $Id: //depot/r22.2/p4-python/P4Result.h#1 $
+ * $Id: //depot/r23.1/p4-python/P4Result.h#1 $
  *
  */
 
 #ifndef P4RESULT_H
 #define P4RESULT_H
 
 namespace p4py
```

### Comparing `p4python-2022.2.2428370/PKG-INFO` & `p4python-2023.1.2454917/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p4python
-Version: 2022.2.2428370
+Version: 2023.1.2454917
 Summary: P4Python - Python interface to Perforce API
 Home-page: http://www.perforce.com
 Author: Perforce Software Inc
 Author-email: support@perforce.com
 Maintainer: Perforce Software Inc
 Maintainer-email: support@perforce.com
 License: LICENSE.txt
```

### Comparing `p4python-2022.2.2428370/PythonActionMergeData.cpp` & `p4python-2023.1.2454917/PythonActionMergeData.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  * DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  *
- * $Id: //depot/r22.2/p4-python/PythonActionMergeData.cpp#1 $
+ * $Id: //depot/r23.1/p4-python/PythonActionMergeData.cpp#1 $
  */
 
 #include <Python.h>
 #include <bytesobject.h>
 #include "undefdups.h"
 #include "python2to3.h"
 #include <clientapi.h>
```

### Comparing `p4python-2022.2.2428370/PythonActionMergeData.h` & `p4python-2023.1.2454917/PythonActionMergeData.h`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  * DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  *
- * $Id: //depot/r22.2/p4-python/PythonActionMergeData.h#1 $
+ * $Id: //depot/r23.1/p4-python/PythonActionMergeData.h#1 $
  */
 
 #ifndef PYTHONACTIONMERGEDATA_H_
 #define PYTHONACTIONMERGEDATA_H_
 
 class PythonActionMergeData
 {
```

### Comparing `p4python-2022.2.2428370/PythonClientAPI.cpp` & `p4python-2023.1.2454917/PythonClientAPI.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-$Id: //depot/r22.2/p4-python/PythonClientAPI.cpp#1 $
+$Id: //depot/r23.1/p4-python/PythonClientAPI.cpp#1 $
 *******************************************************************************/
  
 #include <Python.h>
 #include <bytesobject.h>
 #include "undefdups.h"
 #include "python2to3.h"
 #include <clientapi.h>
```

### Comparing `p4python-2022.2.2428370/PythonClientAPI.h` & `p4python-2023.1.2454917/PythonClientAPI.h`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  * DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  * 
- * $Id: //depot/r22.2/p4-python/PythonClientAPI.h#1 $
+ * $Id: //depot/r23.1/p4-python/PythonClientAPI.h#1 $
  *
  * Build instructions:
  *  Use Distutils - see accompanying setup.py
  *
  *      python setup.py install
  *
  */
```

### Comparing `p4python-2022.2.2428370/PythonClientProgress.cpp` & `p4python-2023.1.2454917/PythonClientProgress.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
  * Name		: PythonClientProgress.cpp
  *
  * Author	: Sven Erik Knop <sknop@perforce.com>
  *
  * Description	: C++ Subclass for ClientProgress used by Python ClientProgress.
  * 		  Allows Perforce API to indicate progress of calls to P4Python
  *
- * 		  $Id: //depot/r22.2/p4-python/PythonClientProgress.cpp#1 $
+ * 		  $Id: //depot/r23.1/p4-python/PythonClientProgress.cpp#1 $
  *
  ******************************************************************************/
 
 #include <Python.h>
 #include <bytesobject.h>
 #include "undefdups.h"
 #include "python2to3.h"
```

### Comparing `p4python-2022.2.2428370/PythonClientProgress.h` & `p4python-2023.1.2454917/PythonClientProgress.h`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  * DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  *
- * $Id: //depot/r22.2/p4-python/PythonClientProgress.h#1 $
+ * $Id: //depot/r23.1/p4-python/PythonClientProgress.h#1 $
  *
  */
 
 
 #ifndef PYTHONCLIENTPROGRESS_H_
 #define PYTHONCLIENTPROGRESS_H_
```

### Comparing `p4python-2022.2.2428370/PythonClientUser.cpp` & `p4python-2023.1.2454917/PythonClientUser.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-$Id: //depot/r22.2/p4-python/PythonClientUser.cpp#1 $
+$Id: //depot/r23.1/p4-python/PythonClientUser.cpp#1 $
 
 *******************************************************************************/
  
 #include <Python.h>
 #include <bytesobject.h>
 #include "undefdups.h"
 #include "python2to3.h"
```

### Comparing `p4python-2022.2.2428370/PythonClientUser.h` & `p4python-2023.1.2454917/PythonClientUser.h`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  * DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  * 
- * $Id: //depot/r22.2/p4-python/PythonClientUser.h#1 $
+ * $Id: //depot/r23.1/p4-python/PythonClientUser.h#1 $
  *
  * Build instructions:
  *  Use Distutils - see accompanying setup.py
  *
  *      python setup.py install
  *
  */
```

### Comparing `p4python-2022.2.2428370/PythonMergeData.cpp` & `p4python-2023.1.2454917/PythonMergeData.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-$Id: //depot/r22.2/p4-python/PythonMergeData.cpp#1 $
+$Id: //depot/r23.1/p4-python/PythonMergeData.cpp#1 $
 
 *******************************************************************************/
 
 #include <Python.h>
 #include <bytesobject.h>
 #include "undefdups.h"
 #include "python2to3.h"
```

### Comparing `p4python-2022.2.2428370/PythonMergeData.h` & `p4python-2023.1.2454917/PythonMergeData.h`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  * DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  * 
- * $Id: //depot/r22.2/p4-python/PythonMergeData.h#1 $
+ * $Id: //depot/r23.1/p4-python/PythonMergeData.h#1 $
  *
  * Build instructions:
  *  Use Distutils - see accompanying setup.py
  *
  *      python setup.py install
  *
  */
```

### Comparing `p4python-2022.2.2428370/PythonMessage.cpp` & `p4python-2023.1.2454917/PythonMessage.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  * DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  *
- * $Id: //depot/r22.2/p4-python/PythonMessage.cpp#1 $
+ * $Id: //depot/r23.1/p4-python/PythonMessage.cpp#1 $
  *
  */
 
 /*******************************************************************************
  * Name		: PythonMessage.cpp
  *
  * Author	: Sven Erik Knop <sknop@perforce.com>
```

### Comparing `p4python-2022.2.2428370/PythonMessage.h` & `p4python-2023.1.2454917/PythonMessage.h`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  * DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  *
- * $Id: //depot/r22.2/p4-python/PythonMessage.h#1 $
+ * $Id: //depot/r23.1/p4-python/PythonMessage.h#1 $
  *
  */
 
 /*******************************************************************************
  * Name		: PythonMessage.h
  *
  * Author	: Sven Erik Knop <sknop@perforce.com>
```

### Comparing `p4python-2022.2.2428370/PythonSpecData.cpp` & `p4python-2023.1.2454917/PythonSpecData.cpp`

 * *Files identical despite different names*

### Comparing `p4python-2022.2.2428370/PythonSpecData.h` & `p4python-2023.1.2454917/PythonSpecData.h`

 * *Files identical despite different names*

### Comparing `p4python-2022.2.2428370/PythonThreadGuard.h` & `p4python-2023.1.2454917/PythonThreadGuard.h`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  * DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  * 
- * $Id: //depot/r22.2/p4-python/PythonThreadGuard.h#1 $
+ * $Id: //depot/r23.1/p4-python/PythonThreadGuard.h#1 $
  *
  * Build instructions:
  *  Use Distutils - see accompanying setup.py
  *
  *      python setup.py install
  *
  */
```

### Comparing `p4python-2022.2.2428370/PythonTypes.h` & `p4python-2023.1.2454917/PythonTypes.h`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  * DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  * 
- * $Id: //depot/r22.2/p4-python/PythonTypes.h#1 $
+ * $Id: //depot/r23.1/p4-python/PythonTypes.h#1 $
  *
  * Build instructions:
  *  Use Distutils - see accompanying setup.py
  *
  *      python setup.py install
  *
  */
```

### Comparing `p4python-2022.2.2428370/SpecMgr.cpp` & `p4python-2023.1.2454917/SpecMgr.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
  (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
- $Id: //depot/r22.2/p4-python/SpecMgr.cpp#1 $
+ $Id: //depot/r23.1/p4-python/SpecMgr.cpp#1 $
  *******************************************************************************/
 
 /*******************************************************************************
  * Name		: SpecMgr.cpp
  *
  * Description	: Python bindings for the Perforce API. Class for handling
  * 		  Perforce specs. This class provides other classes with
@@ -97,15 +97,16 @@
 	"Owner;code:304;seq:3;fmt:R;len:32;;"
 	"Host;code:305;seq:5;fmt:R;len:32;;"
 	"Description;code:306;type:text;len:128;;"
 	"Root;code:307;rq;type:line;len:64;;"
 	"AltRoots;code:308;type:llist;len:64;;"
 	"Options;code:309;type:line;len:64;val:"
 	"noallwrite/allwrite,noclobber/clobber,nocompress/compress,"
-	"unlocked/locked,nomodtime/modtime,normdir/rmdir;;"
+	"unlocked/locked,nomodtime/modtime,normdir/rmdir,"
+	"noaltsync/altsync;;"
 	"SubmitOptions;code:313;type:select;fmt:L;len:25;val:"
 	"submitunchanged/submitunchanged+reopen/revertunchanged/"
 	"revertunchanged+reopen/leaveunchanged/leaveunchanged+reopen;;"
 	"LineEnd;code:310;type:select;fmt:L;len:12;val:"
 	"local/unix/mac/win/share;;"
 	"Stream;code:314;type:line;len:64;;"
 	"StreamAtChange;code:316;type:line;len:64;;"
```

### Comparing `p4python-2022.2.2428370/SpecMgr.h` & `p4python-2023.1.2454917/SpecMgr.h`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-$Id: //depot/r22.2/p4-python/SpecMgr.h#1 $
+$Id: //depot/r23.1/p4-python/SpecMgr.h#1 $
 *******************************************************************************/
 
 /*******************************************************************************
  * Name		: SpecMgr.h
  *
  * Description	: Python bindings for the Perforce API. Class for handling
  * 		  Perforce specs. This class provides other classes with
```

### Comparing `p4python-2022.2.2428370/devnotes.txt` & `p4python-2023.1.2454917/devnotes.txt`

 * *Files identical despite different names*

### Comparing `p4python-2022.2.2428370/job_trigger.py` & `p4python-2023.1.2454917/job_trigger.py`

 * *Files identical despite different names*

### Comparing `p4python-2022.2.2428370/p4test.py` & `p4python-2023.1.2454917/p4test.py`

 * *Files identical despite different names*

### Comparing `p4python-2022.2.2428370/python2to3.h` & `p4python-2023.1.2454917/python2to3.h`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  * DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  * 
- * $Id: //depot/r22.2/p4-python/python2to3.h#1 $
+ * $Id: //depot/r23.1/p4-python/python2to3.h#1 $
  *
  * Build instructions:
  *  Use Distutils - see accompanying setup.py
  *
  *      python setup.py install
  *
  */
```

### Comparing `p4python-2022.2.2428370/setup.py` & `p4python-2023.1.2454917/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     from configparser import ConfigParser
 
 global_dist_directory = "p4python-"
 
 doclines = __doc__.split("\n")
 
 NAME = "p4python"
-VERSION = "2022.1"
+VERSION = "2023.1"
 PY_MODULES = ["P4"]
 P4_API_DIR = "p4api"
 DESCRIPTION = doclines[0]
 AUTHOR = "Perforce Software Inc"
 MAINTAINER = "Perforce Software Inc"
 AUTHOR_EMAIL = "support@perforce.com"
 MAINTAINER_EMAIL = "support@perforce.com"
```

### Comparing `p4python-2022.2.2428370/tools/P4APIFtp.py` & `p4python-2023.1.2454917/tools/P4APIFtp.py`

 * *Files identical despite different names*

### Comparing `p4python-2022.2.2428370/tools/P4APIHttps.py` & `p4python-2023.1.2454917/tools/P4APIHttps.py`

 * *Files identical despite different names*

### Comparing `p4python-2022.2.2428370/tools/PlatformInfo.py` & `p4python-2023.1.2454917/tools/PlatformInfo.py`

 * *Files identical despite different names*

### Comparing `p4python-2022.2.2428370/tools/Version.py` & `p4python-2023.1.2454917/tools/Version.py`

 * *Files identical despite different names*

### Comparing `p4python-2022.2.2428370/tools/VersionInfo.py` & `p4python-2023.1.2454917/tools/VersionInfo.py`

 * *Files identical despite different names*

### Comparing `p4python-2022.2.2428370/undefdups.h` & `p4python-2023.1.2454917/undefdups.h`

 * *Files identical despite different names*

