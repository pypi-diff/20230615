# Comparing `tmp/ghostpip-1.0.1.tar.gz` & `tmp/ghostpip-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghostpip-1.0.1.tar", last modified: Thu Jun 15 04:30:30 2023, max compression
+gzip compressed data, was "ghostpip-1.0.2.tar", last modified: Thu Jun 15 04:36:17 2023, max compression
```

## Comparing `ghostpip-1.0.1.tar` & `ghostpip-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-15 04:30:30.875110 ghostpip-1.0.1/
--rw-rw----   0 root         (0) everybody  (9997)     1080 2023-06-15 04:10:49.000000 ghostpip-1.0.1/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)      756 2023-06-15 04:30:30.863110 ghostpip-1.0.1/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     2035 2023-06-15 04:23:17.000000 ghostpip-1.0.1/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-15 04:30:30.779110 ghostpip-1.0.1/ghostpip/
--rw-rw----   0 root         (0) everybody  (9997)      636 2023-06-15 04:29:45.000000 ghostpip-1.0.1/ghostpip/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)      538 2023-06-15 03:48:27.000000 ghostpip-1.0.1/ghostpip/balance.py
--rw-rw----   0 root         (0) everybody  (9997)      516 2023-06-15 03:50:59.000000 ghostpip-1.0.1/ghostpip/birth.py
--rw-rw----   0 root         (0) everybody  (9997)      456 2023-06-15 03:45:05.000000 ghostpip-1.0.1/ghostpip/device.py
--rw-rw----   0 root         (0) everybody  (9997)      402 2023-06-15 03:44:37.000000 ghostpip-1.0.1/ghostpip/get_user.py
--rw-rw----   0 root         (0) everybody  (9997)      455 2023-06-15 03:44:48.000000 ghostpip-1.0.1/ghostpip/location.py
--rw-rw----   0 root         (0) everybody  (9997)      507 2023-06-15 03:51:46.000000 ghostpip-1.0.1/ghostpip/nid.py
--rw-rw----   0 root         (0) everybody  (9997)      435 2023-06-15 03:48:45.000000 ghostpip-1.0.1/ghostpip/signin.py
--rw-rw----   0 root         (0) everybody  (9997)      463 2023-06-15 03:48:00.000000 ghostpip-1.0.1/ghostpip/signup.py
--rw-rw----   0 root         (0) everybody  (9997)      450 2023-06-15 03:44:57.000000 ghostpip-1.0.1/ghostpip/sim.py
--rw-rw----   0 root         (0) everybody  (9997)      488 2023-06-15 03:52:49.000000 ghostpip-1.0.1/ghostpip/simitalk.py
--rw-rw----   0 root         (0) everybody  (9997)      520 2023-06-15 03:53:28.000000 ghostpip-1.0.1/ghostpip/simiteach.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-15 04:30:30.851110 ghostpip-1.0.1/ghostpip.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      756 2023-06-15 04:30:30.000000 ghostpip-1.0.1/ghostpip.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      418 2023-06-15 04:30:30.000000 ghostpip-1.0.1/ghostpip.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-15 04:30:30.000000 ghostpip-1.0.1/ghostpip.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        9 2023-06-15 04:30:30.000000 ghostpip-1.0.1/ghostpip.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        9 2023-06-15 04:30:30.000000 ghostpip-1.0.1/ghostpip.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-15 04:30:30.875110 ghostpip-1.0.1/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      894 2023-06-15 04:30:18.000000 ghostpip-1.0.1/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-15 04:36:17.011110 ghostpip-1.0.2/
+-rw-rw----   0 root         (0) everybody  (9997)     1080 2023-06-15 04:10:49.000000 ghostpip-1.0.2/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)      756 2023-06-15 04:36:16.995110 ghostpip-1.0.2/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     2035 2023-06-15 04:23:17.000000 ghostpip-1.0.2/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-15 04:36:16.867110 ghostpip-1.0.2/ghostpip/
+-rw-rw----   0 root         (0) everybody  (9997)      633 2023-06-15 04:35:30.000000 ghostpip-1.0.2/ghostpip/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)      459 2023-06-15 04:35:14.000000 ghostpip-1.0.2/ghostpip/balance.py
+-rw-rw----   0 root         (0) everybody  (9997)      516 2023-06-15 03:50:59.000000 ghostpip-1.0.2/ghostpip/birth.py
+-rw-rw----   0 root         (0) everybody  (9997)      456 2023-06-15 03:45:05.000000 ghostpip-1.0.2/ghostpip/device.py
+-rw-rw----   0 root         (0) everybody  (9997)      401 2023-06-15 04:35:39.000000 ghostpip-1.0.2/ghostpip/getuser.py
+-rw-rw----   0 root         (0) everybody  (9997)      455 2023-06-15 03:44:48.000000 ghostpip-1.0.2/ghostpip/location.py
+-rw-rw----   0 root         (0) everybody  (9997)      507 2023-06-15 03:51:46.000000 ghostpip-1.0.2/ghostpip/nid.py
+-rw-rw----   0 root         (0) everybody  (9997)      435 2023-06-15 03:48:45.000000 ghostpip-1.0.2/ghostpip/signin.py
+-rw-rw----   0 root         (0) everybody  (9997)      463 2023-06-15 03:48:00.000000 ghostpip-1.0.2/ghostpip/signup.py
+-rw-rw----   0 root         (0) everybody  (9997)      450 2023-06-15 03:44:57.000000 ghostpip-1.0.2/ghostpip/sim.py
+-rw-rw----   0 root         (0) everybody  (9997)      488 2023-06-15 03:52:49.000000 ghostpip-1.0.2/ghostpip/simitalk.py
+-rw-rw----   0 root         (0) everybody  (9997)      520 2023-06-15 03:53:28.000000 ghostpip-1.0.2/ghostpip/simiteach.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-15 04:36:16.979110 ghostpip-1.0.2/ghostpip.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      756 2023-06-15 04:36:16.000000 ghostpip-1.0.2/ghostpip.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      417 2023-06-15 04:36:16.000000 ghostpip-1.0.2/ghostpip.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-15 04:36:16.000000 ghostpip-1.0.2/ghostpip.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        9 2023-06-15 04:36:16.000000 ghostpip-1.0.2/ghostpip.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        9 2023-06-15 04:36:16.000000 ghostpip-1.0.2/ghostpip.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-15 04:36:17.011110 ghostpip-1.0.2/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      894 2023-06-15 04:35:47.000000 ghostpip-1.0.2/setup.py
```

### Comparing `ghostpip-1.0.1/LICENSE` & `ghostpip-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ghostpip-1.0.1/PKG-INFO` & `ghostpip-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghostpip
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python module for interacting with the ghost.toxinum.xyz API
 Home-page: https://github.com/illusionghost3/ghostpip
 Author: Mohammad Alamin
 Author-email: akxvau@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ghostpip-1.0.1/README.md` & `ghostpip-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ghostpip-1.0.1/ghostpip/__init__.py` & `ghostpip-1.0.2/ghostpip/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from .signup import signup
 from .signin import signin
-from .get_user import get_user
+from .getuser import getuser
 from .location import get_location
 from .sim import get_sim_info
 from .device import get_device_info
 from .balance import get_account_balance
 from .birth import submit_birth_information
 from .nid import submit_nid_information
 from .simitalk import simulate_talk
 from .simiteach import teach_chatbot
 
 __all__ = [
     'signup',
     'signin',
-    'get_user',
+    'getuser',
     'get_location',
     'get_sim_info',
     'get_device_info',
     'get_account_balance',
     'submit_birth_information',
     'submit_nid_information',
     'simulate_talk',
```

### Comparing `ghostpip-1.0.1/ghostpip/birth.py` & `ghostpip-1.0.2/ghostpip/birth.py`

 * *Files identical despite different names*

### Comparing `ghostpip-1.0.1/ghostpip/simiteach.py` & `ghostpip-1.0.2/ghostpip/simiteach.py`

 * *Files identical despite different names*

### Comparing `ghostpip-1.0.1/ghostpip.egg-info/PKG-INFO` & `ghostpip-1.0.2/ghostpip.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghostpip
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python module for interacting with the ghost.toxinum.xyz API
 Home-page: https://github.com/illusionghost3/ghostpip
 Author: Mohammad Alamin
 Author-email: akxvau@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ghostpip-1.0.1/setup.py` & `ghostpip-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ghostpip',
-    version='1.0.1',
+    version='1.0.2',
     author='Mohammad Alamin',
     author_email='akxvau@gmail.com',
     description='A Python module for interacting with the ghost.toxinum.xyz API',
     url='https://github.com/illusionghost3/ghostpip',
     packages=find_packages(),
     install_requires=[
         'requests'
```

