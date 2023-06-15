# Comparing `tmp/ghostpip-1.1.0.tar.gz` & `tmp/ghostpip-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghostpip-1.1.0.tar", last modified: Thu Jun 15 05:07:15 2023, max compression
+gzip compressed data, was "ghostpip-1.1.1.tar", last modified: Thu Jun 15 05:10:24 2023, max compression
```

## Comparing `ghostpip-1.1.0.tar` & `ghostpip-1.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-15 05:07:15.074428 ghostpip-1.1.0/
--rw-rw----   0 root         (0) everybody  (9997)     1080 2023-06-15 04:10:49.000000 ghostpip-1.1.0/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)      756 2023-06-15 05:07:15.058428 ghostpip-1.1.0/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     2750 2023-06-15 05:05:53.000000 ghostpip-1.1.0/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-15 05:07:14.942428 ghostpip-1.1.0/ghostpip/
--rw-rw----   0 root         (0) everybody  (9997)      633 2023-06-15 04:35:30.000000 ghostpip-1.1.0/ghostpip/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)      459 2023-06-15 04:35:14.000000 ghostpip-1.1.0/ghostpip/balance.py
--rw-rw----   0 root         (0) everybody  (9997)      516 2023-06-15 03:50:59.000000 ghostpip-1.1.0/ghostpip/birth.py
--rw-rw----   0 root         (0) everybody  (9997)      456 2023-06-15 03:45:05.000000 ghostpip-1.1.0/ghostpip/device.py
--rw-rw----   0 root         (0) everybody  (9997)      401 2023-06-15 04:35:39.000000 ghostpip-1.1.0/ghostpip/getuser.py
--rw-rw----   0 root         (0) everybody  (9997)      455 2023-06-15 03:44:48.000000 ghostpip-1.1.0/ghostpip/location.py
--rw-rw----   0 root         (0) everybody  (9997)      507 2023-06-15 03:51:46.000000 ghostpip-1.1.0/ghostpip/nid.py
--rw-rw----   0 root         (0) everybody  (9997)      435 2023-06-15 03:48:45.000000 ghostpip-1.1.0/ghostpip/signin.py
--rw-rw----   0 root         (0) everybody  (9997)      463 2023-06-15 03:48:00.000000 ghostpip-1.1.0/ghostpip/signup.py
--rw-rw----   0 root         (0) everybody  (9997)      450 2023-06-15 03:44:57.000000 ghostpip-1.1.0/ghostpip/sim.py
--rw-rw----   0 root         (0) everybody  (9997)      488 2023-06-15 03:52:49.000000 ghostpip-1.1.0/ghostpip/simitalk.py
--rw-rw----   0 root         (0) everybody  (9997)      520 2023-06-15 03:53:28.000000 ghostpip-1.1.0/ghostpip/simiteach.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-15 05:07:15.022428 ghostpip-1.1.0/ghostpip.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      756 2023-06-15 05:07:14.000000 ghostpip-1.1.0/ghostpip.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      417 2023-06-15 05:07:14.000000 ghostpip-1.1.0/ghostpip.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-15 05:07:14.000000 ghostpip-1.1.0/ghostpip.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        9 2023-06-15 05:07:14.000000 ghostpip-1.1.0/ghostpip.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        9 2023-06-15 05:07:14.000000 ghostpip-1.1.0/ghostpip.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-15 05:07:15.074428 ghostpip-1.1.0/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      894 2023-06-15 05:07:07.000000 ghostpip-1.1.0/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-15 05:10:24.326428 ghostpip-1.1.1/
+-rw-rw----   0 root         (0) everybody  (9997)     1080 2023-06-15 04:10:49.000000 ghostpip-1.1.1/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)     3590 2023-06-15 05:10:24.314428 ghostpip-1.1.1/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     2750 2023-06-15 05:05:53.000000 ghostpip-1.1.1/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-15 05:10:24.238428 ghostpip-1.1.1/ghostpip/
+-rw-rw----   0 root         (0) everybody  (9997)      633 2023-06-15 04:35:30.000000 ghostpip-1.1.1/ghostpip/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)      459 2023-06-15 04:35:14.000000 ghostpip-1.1.1/ghostpip/balance.py
+-rw-rw----   0 root         (0) everybody  (9997)      516 2023-06-15 03:50:59.000000 ghostpip-1.1.1/ghostpip/birth.py
+-rw-rw----   0 root         (0) everybody  (9997)      456 2023-06-15 03:45:05.000000 ghostpip-1.1.1/ghostpip/device.py
+-rw-rw----   0 root         (0) everybody  (9997)      401 2023-06-15 04:35:39.000000 ghostpip-1.1.1/ghostpip/getuser.py
+-rw-rw----   0 root         (0) everybody  (9997)      455 2023-06-15 03:44:48.000000 ghostpip-1.1.1/ghostpip/location.py
+-rw-rw----   0 root         (0) everybody  (9997)      507 2023-06-15 03:51:46.000000 ghostpip-1.1.1/ghostpip/nid.py
+-rw-rw----   0 root         (0) everybody  (9997)      435 2023-06-15 03:48:45.000000 ghostpip-1.1.1/ghostpip/signin.py
+-rw-rw----   0 root         (0) everybody  (9997)      463 2023-06-15 03:48:00.000000 ghostpip-1.1.1/ghostpip/signup.py
+-rw-rw----   0 root         (0) everybody  (9997)      450 2023-06-15 03:44:57.000000 ghostpip-1.1.1/ghostpip/sim.py
+-rw-rw----   0 root         (0) everybody  (9997)      488 2023-06-15 03:52:49.000000 ghostpip-1.1.1/ghostpip/simitalk.py
+-rw-rw----   0 root         (0) everybody  (9997)      520 2023-06-15 03:53:28.000000 ghostpip-1.1.1/ghostpip/simiteach.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-15 05:10:24.306428 ghostpip-1.1.1/ghostpip.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     3590 2023-06-15 05:10:23.000000 ghostpip-1.1.1/ghostpip.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      417 2023-06-15 05:10:23.000000 ghostpip-1.1.1/ghostpip.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-15 05:10:23.000000 ghostpip-1.1.1/ghostpip.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        9 2023-06-15 05:10:23.000000 ghostpip-1.1.1/ghostpip.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        9 2023-06-15 05:10:23.000000 ghostpip-1.1.1/ghostpip.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-15 05:10:24.326428 ghostpip-1.1.1/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1124 2023-06-15 05:10:07.000000 ghostpip-1.1.1/setup.py
```

### Comparing `ghostpip-1.1.0/LICENSE` & `ghostpip-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ghostpip-1.1.0/README.md` & `ghostpip-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ghostpip-1.1.0/ghostpip/__init__.py` & `ghostpip-1.1.1/ghostpip/__init__.py`

 * *Files identical despite different names*

### Comparing `ghostpip-1.1.0/ghostpip/birth.py` & `ghostpip-1.1.1/ghostpip/birth.py`

 * *Files identical despite different names*

### Comparing `ghostpip-1.1.0/ghostpip/simiteach.py` & `ghostpip-1.1.1/ghostpip/simiteach.py`

 * *Files identical despite different names*

