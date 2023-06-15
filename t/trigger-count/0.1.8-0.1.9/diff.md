# Comparing `tmp/trigger_count-0.1.8.tar.gz` & `tmp/trigger_count-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trigger_count-0.1.8.tar", max compression
+gzip compressed data, was "trigger_count-0.1.9.tar", max compression
```

## Comparing `trigger_count-0.1.8.tar` & `trigger_count-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0        0 2023-04-20 09:07:10.209580 trigger_count-0.1.8/README.md
--rw-r--r--   0        0        0      395 2023-04-20 10:32:05.703903 trigger_count-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 09:07:10.209580 trigger_count-0.1.8/trigger_count/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 09:07:10.209580 trigger_count-0.1.8/trigger_count/daq/__init__.py
--rw-r--r--   0        0        0     3162 2023-04-20 09:16:50.245417 trigger_count-0.1.8/trigger_count/daq/labjack.py
--rw-r--r--   0        0        0        0 2023-04-20 09:32:07.572241 trigger_count-0.1.8/trigger_count/kengo/__init__.py
--rw-r--r--   0        0        0      998 2023-04-20 10:31:34.327237 trigger_count-0.1.8/trigger_count/kengo/arduino.py
--rw-r--r--   0        0        0        0 2023-04-20 09:07:10.209580 trigger_count-0.1.8/trigger_count/workaround/__init__.py
--rw-r--r--   0        0        0     6268 2023-04-20 09:55:13.764831 trigger_count-0.1.8/trigger_count/workaround/align.py
--rw-r--r--   0        0        0     3489 2023-04-20 09:07:10.209580 trigger_count-0.1.8/trigger_count/workaround/arduino.py
--rw-r--r--   0        0        0     1488 2023-04-20 09:07:10.209580 trigger_count-0.1.8/trigger_count/workaround/start_gui.py
--rw-r--r--   0        0        0     3034 2023-04-20 09:07:10.209580 trigger_count-0.1.8/trigger_count/workaround/xml.py
--rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 trigger_count-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-02-14 09:44:42.373435 trigger_count-0.1.9/README.md
+-rw-r--r--   0        0        0      395 2023-06-15 11:44:55.206259 trigger_count-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-14 09:44:42.373435 trigger_count-0.1.9/trigger_count/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-14 13:55:05.463258 trigger_count-0.1.9/trigger_count/daq/__init__.py
+-rw-r--r--   0        0        0     3157 2023-06-15 11:44:04.598111 trigger_count-0.1.9/trigger_count/daq/gui.py
+-rw-r--r--   0        0        0     4245 2023-06-13 13:55:06.899828 trigger_count-0.1.9/trigger_count/daq/labjack_t7.py
+-rw-r--r--   0        0        0        0 2023-04-26 10:39:57.117379 trigger_count-0.1.9/trigger_count/kengo/__init__.py
+-rw-r--r--   0        0        0      998 2023-04-26 10:39:57.117379 trigger_count-0.1.9/trigger_count/kengo/arduino.py
+-rw-r--r--   0        0        0        0 2023-04-26 10:39:57.117379 trigger_count-0.1.9/trigger_count/workaround/__init__.py
+-rw-r--r--   0        0        0     6268 2023-04-26 10:39:57.117379 trigger_count-0.1.9/trigger_count/workaround/align.py
+-rw-r--r--   0        0        0     3489 2023-04-26 10:39:57.117379 trigger_count-0.1.9/trigger_count/workaround/arduino.py
+-rw-r--r--   0        0        0     1488 2023-04-26 10:39:57.117379 trigger_count-0.1.9/trigger_count/workaround/start_gui.py
+-rw-r--r--   0        0        0     3034 2023-04-26 10:39:57.118379 trigger_count-0.1.9/trigger_count/workaround/xml.py
+-rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 trigger_count-0.1.9/setup.py
+-rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 trigger_count-0.1.9/PKG-INFO
```

### Comparing `trigger_count-0.1.8/trigger_count/kengo/arduino.py` & `trigger_count-0.1.9/trigger_count/kengo/arduino.py`

 * *Files identical despite different names*

### Comparing `trigger_count-0.1.8/trigger_count/workaround/align.py` & `trigger_count-0.1.9/trigger_count/workaround/align.py`

 * *Files identical despite different names*

### Comparing `trigger_count-0.1.8/trigger_count/workaround/arduino.py` & `trigger_count-0.1.9/trigger_count/workaround/arduino.py`

 * *Files identical despite different names*

### Comparing `trigger_count-0.1.8/trigger_count/workaround/start_gui.py` & `trigger_count-0.1.9/trigger_count/workaround/start_gui.py`

 * *Files identical despite different names*

### Comparing `trigger_count-0.1.8/trigger_count/workaround/xml.py` & `trigger_count-0.1.9/trigger_count/workaround/xml.py`

 * *Files identical despite different names*

