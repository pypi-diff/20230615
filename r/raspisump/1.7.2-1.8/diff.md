# Comparing `tmp/raspisump-1.7.2.tar.gz` & `tmp/raspisump-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspisump-1.7.2.tar", last modified: Wed Jun  7 16:46:07 2023, max compression
+gzip compressed data, was "raspisump-1.8.tar", last modified: Thu Jun 15 16:26:18 2023, max compression
```

## Comparing `raspisump-1.7.2.tar` & `raspisump-1.8.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.920452 raspisump-1.7.2/
--rw-r--r--   0 al        (1000) users      (984)     1073 2023-06-02 22:51:18.000000 raspisump-1.7.2/LICENSE
--rw-r--r--   0 al        (1000) users      (984)      251 2023-06-02 22:51:18.000000 raspisump-1.7.2/MANIFEST.in
--rw-r--r--   0 al        (1000) users      (984)     3948 2023-06-07 16:46:07.920452 raspisump-1.7.2/PKG-INFO
--rw-r--r--   0 al        (1000) users      (984)     3174 2023-06-02 22:51:18.000000 raspisump-1.7.2/README.md
--rw-r--r--   0 al        (1000) users      (984)       24 2023-06-07 16:45:05.000000 raspisump-1.7.2/VERSION
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.910452 raspisump-1.7.2/bin/
--rw-r--r--   0 al        (1000) users      (984)      362 2023-06-02 22:51:18.000000 raspisump-1.7.2/bin/emailtest
--rwxr-xr-x   0 al        (1000) users      (984)      962 2023-06-07 16:45:05.000000 raspisump-1.7.2/bin/rsump.py
--rwxr-xr-x   0 al        (1000) users      (984)      638 2023-06-07 16:45:05.000000 raspisump-1.7.2/bin/rsumpchart.py
--rwxr-xr-x   0 al        (1000) users      (984)      538 2023-06-07 16:45:05.000000 raspisump-1.7.2/bin/rsumpmonitor.py
--rwxr-xr-x   0 al        (1000) users      (984)      705 2023-06-07 16:45:05.000000 raspisump-1.7.2/bin/rsumpwebchart.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.910452 raspisump-1.7.2/conf/
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.910452 raspisump-1.7.2/conf/charts/
--rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.7.2/conf/charts/README.md
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.910452 raspisump-1.7.2/conf/csv/
--rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.7.2/conf/csv/README.md
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.913786 raspisump-1.7.2/conf/logs/
--rw-r--r--   0 al        (1000) users      (984)      217 2023-06-02 22:51:18.000000 raspisump-1.7.2/conf/logs/README.md
--rw-r--r--   0 al        (1000) users      (984)     5687 2023-06-02 22:51:18.000000 raspisump-1.7.2/conf/raspisump.conf
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.913786 raspisump-1.7.2/conf/web/
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.913786 raspisump-1.7.2/conf/web/css/
--rw-r--r--   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.7.2/conf/web/css/index.html
--rw-r--r--   0 al        (1000) users      (984)      614 2023-06-02 22:51:18.000000 raspisump-1.7.2/conf/web/css/raspi.css
--rw-r--r--   0 al        (1000) users      (984)      690 2023-06-02 22:51:18.000000 raspisump-1.7.2/conf/web/css/raspi.css~
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.913786 raspisump-1.7.2/conf/web/images/
--rw-r--r--   0 al        (1000) users      (984)    51981 2023-06-02 22:51:18.000000 raspisump-1.7.2/conf/web/images/logo.png
--rwxr-xr-x   0 al        (1000) users      (984)      906 2023-06-02 22:51:18.000000 raspisump-1.7.2/conf/web/index.html
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.913786 raspisump-1.7.2/cron/
--rw-r--r--   0 al        (1000) users      (984)      140 2023-06-02 22:51:18.000000 raspisump-1.7.2/cron/README.md
--rw-r--r--   0 al        (1000) users      (984)      258 2023-06-02 22:51:18.000000 raspisump-1.7.2/cron/picrontab
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.917119 raspisump-1.7.2/docs/
--rw-r--r--   0 al        (1000) users      (984)      275 2023-06-02 22:51:18.000000 raspisump-1.7.2/docs/README.md
--rw-r--r--   0 al        (1000) users      (984)    10745 2023-06-02 22:51:18.000000 raspisump-1.7.2/docs/install.md
--rw-r--r--   0 al        (1000) users      (984)   133806 2023-06-02 22:51:18.000000 raspisump-1.7.2/docs/install.pdf
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.917119 raspisump-1.7.2/raspisump/
--rwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.7.2/raspisump/__init__.py
--rw-r--r--   0 al        (1000) users      (984)     4680 2023-06-07 16:45:05.000000 raspisump-1.7.2/raspisump/alerts.py
--rw-r--r--   0 al        (1000) users      (984)     2068 2023-06-02 22:51:18.000000 raspisump-1.7.2/raspisump/checkpid.py
--rw-r--r--   0 al        (1000) users      (984)     1965 2023-06-07 16:45:05.000000 raspisump-1.7.2/raspisump/emailtest.py
--rw-r--r--   0 al        (1000) users      (984)     4190 2023-06-07 16:45:05.000000 raspisump-1.7.2/raspisump/heartbeat.py
--rw-r--r--   0 al        (1000) users      (984)      844 2023-06-07 16:45:05.000000 raspisump-1.7.2/raspisump/log.py
--rw-r--r--   0 al        (1000) users      (984)     2799 2023-06-07 16:45:05.000000 raspisump-1.7.2/raspisump/reading.py
--rw-r--r--   0 al        (1000) users      (984)     2045 2023-06-07 16:45:05.000000 raspisump-1.7.2/raspisump/todaychart.py
--rw-r--r--   0 al        (1000) users      (984)     1414 2023-06-07 16:45:05.000000 raspisump-1.7.2/raspisump/webchart.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.920452 raspisump-1.7.2/raspisump.egg-info/
--rw-r--r--   0 al        (1000) users      (984)     3948 2023-06-07 16:46:07.000000 raspisump-1.7.2/raspisump.egg-info/PKG-INFO
--rw-r--r--   0 al        (1000) users      (984)      808 2023-06-07 16:46:07.000000 raspisump-1.7.2/raspisump.egg-info/SOURCES.txt
--rw-r--r--   0 al        (1000) users      (984)        1 2023-06-07 16:46:07.000000 raspisump-1.7.2/raspisump.egg-info/dependency_links.txt
--rw-r--r--   0 al        (1000) users      (984)       13 2023-06-07 16:46:07.000000 raspisump-1.7.2/raspisump.egg-info/requires.txt
--rw-r--r--   0 al        (1000) users      (984)       10 2023-06-07 16:46:07.000000 raspisump-1.7.2/raspisump.egg-info/top_level.txt
--rw-r--r--   0 al        (1000) users      (984)       38 2023-06-07 16:46:07.920452 raspisump-1.7.2/setup.cfg
--rwxr-xr-x   0 al        (1000) users      (984)     2303 2023-06-07 16:45:05.000000 raspisump-1.7.2/setup.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.920452 raspisump-1.7.2/tests/
--rw-r--r--   0 al        (1000) users      (984)     1346 2023-06-07 16:45:05.000000 raspisump-1.7.2/tests/tests_logging.py
--rw-r--r--   0 al        (1000) users      (984)     2342 2023-06-07 16:45:05.000000 raspisump-1.7.2/tests/tests_sump.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.572954 raspisump-1.8/
+-rw-r--r--   0 al        (1000) users      (984)     1073 2023-06-02 22:51:18.000000 raspisump-1.8/LICENSE
+-rw-r--r--   0 al        (1000) users      (984)      284 2023-06-15 16:24:24.000000 raspisump-1.8/MANIFEST.in
+-rw-r--r--   0 al        (1000) users      (984)     3969 2023-06-15 16:26:18.572954 raspisump-1.8/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)     3197 2023-06-15 16:24:24.000000 raspisump-1.8/README.md
+-rw-r--r--   0 al        (1000) users      (984)       11 2023-06-15 16:24:24.000000 raspisump-1.8/VERSION
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.562954 raspisump-1.8/bin/
+-rw-r--r--   0 al        (1000) users      (984)      362 2023-06-02 22:51:18.000000 raspisump-1.8/bin/emailtest
+-rwxr-xr-x   0 al        (1000) users      (984)      962 2023-06-07 16:45:05.000000 raspisump-1.8/bin/rsump.py
+-rwxr-xr-x   0 al        (1000) users      (984)      638 2023-06-07 16:45:05.000000 raspisump-1.8/bin/rsumpchart.py
+-rwxr-xr-x   0 al        (1000) users      (984)      538 2023-06-07 16:45:05.000000 raspisump-1.8/bin/rsumpmonitor.py
+-rwxr-xr-x   0 al        (1000) users      (984)      705 2023-06-07 16:45:05.000000 raspisump-1.8/bin/rsumpwebchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.562954 raspisump-1.8/conf/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.562954 raspisump-1.8/conf/charts/
+-rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.8/conf/charts/README.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.562954 raspisump-1.8/conf/csv/
+-rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.8/conf/csv/README.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.562954 raspisump-1.8/conf/logs/
+-rw-r--r--   0 al        (1000) users      (984)      217 2023-06-02 22:51:18.000000 raspisump-1.8/conf/logs/README.md
+-rw-r--r--   0 al        (1000) users      (984)     5687 2023-06-02 22:51:18.000000 raspisump-1.8/conf/raspisump.conf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.562954 raspisump-1.8/conf/web/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.566287 raspisump-1.8/conf/web/css/
+-rw-r--r--   0 al        (1000) users      (984)      379 2023-06-15 16:24:24.000000 raspisump-1.8/conf/web/css/includes.js
+-rw-r--r--   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.8/conf/web/css/index.html
+-rw-r--r--   0 al        (1000) users      (984)      472 2023-06-15 16:24:24.000000 raspisump-1.8/conf/web/css/raspi.css
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.566287 raspisump-1.8/conf/web/images/
+-rw-r--r--   0 al        (1000) users      (984)    51981 2023-06-02 22:51:18.000000 raspisump-1.8/conf/web/images/logo.png
+-rw-r--r--   0 al        (1000) users      (984)     2940 2023-06-15 16:24:24.000000 raspisump-1.8/conf/web/index.html
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.566287 raspisump-1.8/cron/
+-rw-r--r--   0 al        (1000) users      (984)      140 2023-06-02 22:51:18.000000 raspisump-1.8/cron/README.md
+-rw-r--r--   0 al        (1000) users      (984)      258 2023-06-02 22:51:18.000000 raspisump-1.8/cron/picrontab
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.566287 raspisump-1.8/docs/
+-rw-r--r--   0 al        (1000) users      (984)      275 2023-06-02 22:51:18.000000 raspisump-1.8/docs/README.md
+-rw-r--r--   0 al        (1000) users      (984)    10745 2023-06-02 22:51:18.000000 raspisump-1.8/docs/install.md
+-rw-r--r--   0 al        (1000) users      (984)   133806 2023-06-02 22:51:18.000000 raspisump-1.8/docs/install.pdf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.569621 raspisump-1.8/raspisump/
+-rwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.8/raspisump/__init__.py
+-rw-r--r--   0 al        (1000) users      (984)     4680 2023-06-07 16:45:05.000000 raspisump-1.8/raspisump/alerts.py
+-rw-r--r--   0 al        (1000) users      (984)     2068 2023-06-02 22:51:18.000000 raspisump-1.8/raspisump/checkpid.py
+-rw-r--r--   0 al        (1000) users      (984)     1965 2023-06-07 16:45:05.000000 raspisump-1.8/raspisump/emailtest.py
+-rw-r--r--   0 al        (1000) users      (984)     4190 2023-06-07 16:45:05.000000 raspisump-1.8/raspisump/heartbeat.py
+-rw-r--r--   0 al        (1000) users      (984)      844 2023-06-07 16:45:05.000000 raspisump-1.8/raspisump/log.py
+-rw-r--r--   0 al        (1000) users      (984)     2799 2023-06-07 16:45:05.000000 raspisump-1.8/raspisump/reading.py
+-rw-r--r--   0 al        (1000) users      (984)     2126 2023-06-15 16:24:24.000000 raspisump-1.8/raspisump/todaychart.py
+-rw-r--r--   0 al        (1000) users      (984)     1414 2023-06-07 16:45:05.000000 raspisump-1.8/raspisump/webchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.572954 raspisump-1.8/raspisump.egg-info/
+-rw-r--r--   0 al        (1000) users      (984)     3969 2023-06-15 16:26:18.000000 raspisump-1.8/raspisump.egg-info/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)      809 2023-06-15 16:26:18.000000 raspisump-1.8/raspisump.egg-info/SOURCES.txt
+-rw-r--r--   0 al        (1000) users      (984)        1 2023-06-15 16:26:18.000000 raspisump-1.8/raspisump.egg-info/dependency_links.txt
+-rw-r--r--   0 al        (1000) users      (984)       13 2023-06-15 16:26:18.000000 raspisump-1.8/raspisump.egg-info/requires.txt
+-rw-r--r--   0 al        (1000) users      (984)       10 2023-06-15 16:26:18.000000 raspisump-1.8/raspisump.egg-info/top_level.txt
+-rw-r--r--   0 al        (1000) users      (984)       38 2023-06-15 16:26:18.572954 raspisump-1.8/setup.cfg
+-rwxr-xr-x   0 al        (1000) users      (984)     2402 2023-06-15 16:24:24.000000 raspisump-1.8/setup.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.572954 raspisump-1.8/tests/
+-rw-r--r--   0 al        (1000) users      (984)     1346 2023-06-07 16:45:05.000000 raspisump-1.8/tests/tests_logging.py
+-rw-r--r--   0 al        (1000) users      (984)     2342 2023-06-07 16:45:05.000000 raspisump-1.8/tests/tests_sump.py
```

### Comparing `raspisump-1.7.2/LICENSE` & `raspisump-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.2/PKG-INFO` & `raspisump-1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.7.2
+Version: 1.8
 Summary: A sump pit monitoring system for Raspberry Pi
 Home-page: https://www.linuxnorth.org/raspi-sump/
 Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,15 @@
 Classifier: Topic :: Home Automation
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Raspi-sump is a sump pit water level monitoring system using a Raspberry Pi and an Ultrasonic Sensor (HC-SR04).
 
-![Chart](https://raspisump.linuxnorth.org/static/today.png)
+![MobileScreenshot](https://www.linuxnorth.org/raspi-sump/images/rsump_mobile.jpg)
 
 
 Currently the system monitors the water level in your pit at defined intervals. It sends
 email sms alerts if the water reaches a critical level, indicating a possible sump pump failure.
 
 # What's New
```

### Comparing `raspisump-1.7.2/README.md` & `raspisump-1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Raspi-sump is a sump pit water level monitoring system using a Raspberry Pi and an Ultrasonic Sensor (HC-SR04).
 
-![Chart](https://raspisump.linuxnorth.org/static/today.png)
+![MobileScreenshot](https://www.linuxnorth.org/raspi-sump/images/rsump_mobile.jpg)
 
 
 Currently the system monitors the water level in your pit at defined intervals. It sends
 email sms alerts if the water reaches a critical level, indicating a possible sump pump failure.
 
 # What's New
```

### Comparing `raspisump-1.7.2/bin/rsump.py` & `raspisump-1.8/bin/rsump.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.2/bin/rsumpchart.py` & `raspisump-1.8/bin/rsumpchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.2/bin/rsumpmonitor.py` & `raspisump-1.8/bin/rsumpmonitor.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.2/bin/rsumpwebchart.py` & `raspisump-1.8/bin/rsumpwebchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.2/conf/raspisump.conf` & `raspisump-1.8/conf/raspisump.conf`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.2/conf/web/images/logo.png` & `raspisump-1.8/conf/web/images/logo.png`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.2/docs/install.md` & `raspisump-1.8/docs/install.md`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.2/docs/install.pdf` & `raspisump-1.8/docs/install.pdf`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.2/raspisump/alerts.py` & `raspisump-1.8/raspisump/alerts.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.2/raspisump/checkpid.py` & `raspisump-1.8/raspisump/checkpid.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.2/raspisump/emailtest.py` & `raspisump-1.8/raspisump/emailtest.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.2/raspisump/heartbeat.py` & `raspisump-1.8/raspisump/heartbeat.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.2/raspisump/log.py` & `raspisump-1.8/raspisump/log.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.2/raspisump/reading.py` & `raspisump-1.8/raspisump/reading.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.2/raspisump/todaychart.py` & `raspisump-1.8/raspisump/todaychart.py`

 * *Files 20% similar despite different names*

```diff
@@ -56,23 +56,24 @@
         x=date,
         y=value,
         ls="solid",
         linewidth=2,
         color="#" + configs["line_color"],
         fmt=":",
     )
-    title = f"Sump Pit Water Level {time.strftime('%Y-%m-%d %H:%M')}"
+    title = f"Water Level {time.strftime('%Y-%m-%d %H:%M')}"
     title_set = plt.title(title)
+    title_set.set_fontsize(20.0)
     title_set.set_y(1.09)
     plt.subplots_adjust(top=0.86)
 
     if unit == "imperial":
-        plt.ylabel("inches")
+        plt.ylabel("inches", fontsize=16)
     if unit == "metric":
-        plt.ylabel("centimeters")
+        plt.ylabel("centimeters", fontsize=16)
 
-    plt.xlabel("Time of Day")
+    plt.xlabel("Time of Day", fontsize=16)
     plt.xticks(rotation=30)
     plt.grid(True, color="#ECE5DE", linestyle="solid")
     plt.tick_params(axis="x", bottom=False, top=False)
     plt.tick_params(axis="y", left=False, right=False)
-    plt.savefig(filename, dpi=72)
+    plt.savefig(filename, transparent=True, dpi=72)
```

### Comparing `raspisump-1.7.2/raspisump/webchart.py` & `raspisump-1.8/raspisump/webchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.2/raspisump.egg-info/PKG-INFO` & `raspisump-1.8/raspisump.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.7.2
+Version: 1.8
 Summary: A sump pit monitoring system for Raspberry Pi
 Home-page: https://www.linuxnorth.org/raspi-sump/
 Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,15 @@
 Classifier: Topic :: Home Automation
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Raspi-sump is a sump pit water level monitoring system using a Raspberry Pi and an Ultrasonic Sensor (HC-SR04).
 
-![Chart](https://raspisump.linuxnorth.org/static/today.png)
+![MobileScreenshot](https://www.linuxnorth.org/raspi-sump/images/rsump_mobile.jpg)
 
 
 Currently the system monitors the water level in your pit at defined intervals. It sends
 email sms alerts if the water reaches a critical level, indicating a possible sump pump failure.
 
 # What's New
```

### Comparing `raspisump-1.7.2/raspisump.egg-info/SOURCES.txt` & `raspisump-1.8/raspisump.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 bin/rsumpmonitor.py
 bin/rsumpwebchart.py
 conf/raspisump.conf
 conf/charts/README.md
 conf/csv/README.md
 conf/logs/README.md
 conf/web/index.html
+conf/web/css/includes.js
 conf/web/css/index.html
 conf/web/css/raspi.css
-conf/web/css/raspi.css~
 conf/web/images/logo.png
 cron/README.md
 cron/picrontab
 docs/README.md
 docs/install.md
 docs/install.pdf
 raspisump/__init__.py
```

### Comparing `raspisump-1.7.2/setup.py` & `raspisump-1.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-version = "1.7.2"
+version = "1.8"
 user = os.getlogin()
 
 homedir = "/home/" + user + "/raspi-sump/"
 
 if os.path.isfile(homedir + "raspisump.conf"):
     cmd = "cp -u " + homedir + "raspisump.conf " + homedir + "raspisump.conf.save"
     os.system(cmd)
@@ -27,15 +27,17 @@
     (homedir + "docs", ["docs/install.md"]),
     (homedir + "cron", ["cron/README.md"]),
     (homedir + "cron", ["cron/picrontab"]),
     (homedir + "web", ["conf/web/index.html"]),
     (homedir + "web/images", ["conf/web/images/logo.png"]),
     (homedir + "web/css", ["conf/web/css/index.html"]),
     (homedir + "web/css", ["conf/web/css/raspi.css"]),
+    (homedir + "web/css", ["conf/web/css/includes.js"]),
     (homedir, ["VERSION"]),
+    (homedir + "web/css/inc", ["VERSION"]),
 ]
 
 setup(
     name="raspisump",
     version=version,
     description="A sump pit monitoring system for Raspberry Pi",
     long_description_content_type="text/markdown",
```

### Comparing `raspisump-1.7.2/tests/tests_logging.py` & `raspisump-1.8/tests/tests_logging.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.2/tests/tests_sump.py` & `raspisump-1.8/tests/tests_sump.py`

 * *Files identical despite different names*

