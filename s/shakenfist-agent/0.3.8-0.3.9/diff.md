# Comparing `tmp/shakenfist-agent-0.3.8.tar.gz` & `tmp/shakenfist-agent-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shakenfist-agent-0.3.8.tar", last modified: Fri Jun  9 06:39:32 2023, max compression
+gzip compressed data, was "shakenfist-agent-0.3.9.tar", last modified: Sat Jun 10 06:40:35 2023, max compression
```

## Comparing `shakenfist-agent-0.3.8.tar` & `shakenfist-agent-0.3.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-09 06:39:32.904024 shakenfist-agent-0.3.8/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      266 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.8/.coveragerc
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-09 06:39:32.896024 shakenfist-agent-0.3.8/.github/
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-09 06:39:32.900024 shakenfist-agent-0.3.8/.github/workflows/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1301 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.8/.github/workflows/python-unit-tests.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       55 2022-03-31 06:16:40.000000 shakenfist-agent-0.3.8/.stestr.conf
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       60 2023-06-09 06:39:32.000000 shakenfist-agent-0.3.8/AUTHORS
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    11357 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.8/LICENSE
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      907 2023-06-09 06:39:32.904024 shakenfist-agent-0.3.8/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      190 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.8/README.md
--rwxrwxr-x   0 parallels  (1000) parallels  (1000)      857 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.8/release.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      249 2023-05-31 09:10:23.000000 shakenfist-agent-0.3.8/requirements.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      729 2023-06-09 06:39:32.904024 shakenfist-agent-0.3.8/setup.cfg
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1148 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.8/setup.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-09 06:39:32.900024 shakenfist-agent-0.3.8/shakenfist_agent/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.8/shakenfist_agent/__init__.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-09 06:39:32.904024 shakenfist-agent-0.3.8/shakenfist_agent/commandline/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8562 2023-06-09 06:39:11.000000 shakenfist-agent-0.3.8/shakenfist_agent/commandline/daemon.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      613 2022-08-07 23:05:27.000000 shakenfist-agent-0.3.8/shakenfist_agent/main.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8598 2023-06-09 06:39:11.000000 shakenfist-agent-0.3.8/shakenfist_agent/protocol.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-09 06:39:32.904024 shakenfist-agent-0.3.8/shakenfist_agent/tests/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-03-31 06:16:40.000000 shakenfist-agent-0.3.8/shakenfist_agent/tests/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4848 2023-03-08 21:01:13.000000 shakenfist-agent-0.3.8/shakenfist_agent/tests/test_daemon.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3815 2023-03-06 10:12:52.000000 shakenfist-agent-0.3.8/shakenfist_agent/tests/test_protocol.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-09 06:39:32.904024 shakenfist-agent-0.3.8/shakenfist_agent.egg-info/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      907 2023-06-09 06:39:32.000000 shakenfist-agent-0.3.8/shakenfist_agent.egg-info/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      738 2023-06-09 06:39:32.000000 shakenfist-agent-0.3.8/shakenfist_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-06-09 06:39:32.000000 shakenfist-agent-0.3.8/shakenfist_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       56 2023-06-09 06:39:32.000000 shakenfist-agent-0.3.8/shakenfist_agent.egg-info/entry_points.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-06-09 06:39:32.000000 shakenfist-agent-0.3.8/shakenfist_agent.egg-info/not-zip-safe
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       46 2023-06-09 06:39:32.000000 shakenfist-agent-0.3.8/shakenfist_agent.egg-info/pbr.json
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      101 2023-06-09 06:39:32.000000 shakenfist-agent-0.3.8/shakenfist_agent.egg-info/requires.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       17 2023-06-09 06:39:32.000000 shakenfist-agent-0.3.8/shakenfist_agent.egg-info/top_level.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      164 2022-08-07 23:05:27.000000 shakenfist-agent-0.3.8/test-requirements.txt
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-09 06:39:32.904024 shakenfist-agent-0.3.8/tools/
--rwxrwxr-x   0 parallels  (1000) parallels  (1000)      573 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.8/tools/flake8wrap.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      867 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.8/tox.ini
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-10 06:40:35.049809 shakenfist-agent-0.3.9/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      266 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.9/.coveragerc
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-10 06:40:35.041810 shakenfist-agent-0.3.9/.github/
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-10 06:40:35.045809 shakenfist-agent-0.3.9/.github/workflows/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1301 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.9/.github/workflows/python-unit-tests.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       55 2022-03-31 06:16:40.000000 shakenfist-agent-0.3.9/.stestr.conf
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       60 2023-06-10 06:40:34.000000 shakenfist-agent-0.3.9/AUTHORS
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    11357 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.9/LICENSE
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      907 2023-06-10 06:40:35.049809 shakenfist-agent-0.3.9/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      190 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.9/README.md
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)      857 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.9/release.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      249 2023-05-31 09:10:23.000000 shakenfist-agent-0.3.9/requirements.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      729 2023-06-10 06:40:35.049809 shakenfist-agent-0.3.9/setup.cfg
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1148 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.9/setup.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-10 06:40:35.045809 shakenfist-agent-0.3.9/shakenfist_agent/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.9/shakenfist_agent/__init__.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-10 06:40:35.049809 shakenfist-agent-0.3.9/shakenfist_agent/commandline/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8562 2023-06-10 06:40:20.000000 shakenfist-agent-0.3.9/shakenfist_agent/commandline/daemon.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      613 2022-08-07 23:05:27.000000 shakenfist-agent-0.3.9/shakenfist_agent/main.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8581 2023-06-10 06:40:20.000000 shakenfist-agent-0.3.9/shakenfist_agent/protocol.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-10 06:40:35.049809 shakenfist-agent-0.3.9/shakenfist_agent/tests/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-03-31 06:16:40.000000 shakenfist-agent-0.3.9/shakenfist_agent/tests/__init__.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4848 2023-03-08 21:01:13.000000 shakenfist-agent-0.3.9/shakenfist_agent/tests/test_daemon.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3815 2023-03-06 10:12:52.000000 shakenfist-agent-0.3.9/shakenfist_agent/tests/test_protocol.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-10 06:40:35.049809 shakenfist-agent-0.3.9/shakenfist_agent.egg-info/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      907 2023-06-10 06:40:34.000000 shakenfist-agent-0.3.9/shakenfist_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      738 2023-06-10 06:40:35.000000 shakenfist-agent-0.3.9/shakenfist_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-06-10 06:40:34.000000 shakenfist-agent-0.3.9/shakenfist_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       56 2023-06-10 06:40:34.000000 shakenfist-agent-0.3.9/shakenfist_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-06-10 06:40:34.000000 shakenfist-agent-0.3.9/shakenfist_agent.egg-info/not-zip-safe
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       46 2023-06-10 06:40:34.000000 shakenfist-agent-0.3.9/shakenfist_agent.egg-info/pbr.json
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      101 2023-06-10 06:40:34.000000 shakenfist-agent-0.3.9/shakenfist_agent.egg-info/requires.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       17 2023-06-10 06:40:34.000000 shakenfist-agent-0.3.9/shakenfist_agent.egg-info/top_level.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      164 2022-08-07 23:05:27.000000 shakenfist-agent-0.3.9/test-requirements.txt
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-10 06:40:35.049809 shakenfist-agent-0.3.9/tools/
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)      573 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.9/tools/flake8wrap.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      867 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.9/tox.ini
```

### Comparing `shakenfist-agent-0.3.8/.github/workflows/python-unit-tests.yml` & `shakenfist-agent-0.3.9/.github/workflows/python-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.8/LICENSE` & `shakenfist-agent-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.8/PKG-INFO` & `shakenfist-agent-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shakenfist-agent
-Version: 0.3.8
+Version: 0.3.9
 Summary: An in-guest agent for instances running on Shaken Fist
 Home-page: https://madebymikal.com/shakenfist
 Author: Michael Still
 Author-email: mikal@stillhq.com
 License: Apache2
 Description: Python side channel agent for Shaken Fist
         =========================================
```

### Comparing `shakenfist-agent-0.3.8/release.sh` & `shakenfist-agent-0.3.9/release.sh`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.8/setup.cfg` & `shakenfist-agent-0.3.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.8/setup.py` & `shakenfist-agent-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.8/shakenfist_agent/commandline/daemon.py` & `shakenfist-agent-0.3.9/shakenfist_agent/commandline/daemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,21 +106,21 @@
 
         if 'chunk' not in packet:
             # A metadata packet
             self.incomplete_file_puts[path].update(packet['stat_result'])
             return
 
         if packet['chunk'] is None:
-            self.incomplete_file_gets[path]['flo'].close()
-            del self.incomplete_file_gets[path]
+            self.incomplete_file_puts[path]['flo'].close()
+            del self.incomplete_file_puts[path]
             self.log.with_fields(packet).info('File put complete')
             return
 
         d = base64.b64decode(packet['chunk'])
-        self.incomplete_file_gets[path]['flo'].write(d)
+        self.incomplete_file_puts[path]['flo'].write(d)
 
     def chmod(self, packet):
         os.chmod(packet['path'],
                  symbolicmode.symbolic_to_numeric_permissions(packet['mode']))
         self.send_packet({
             'command': 'chmod-response',
             'path': packet['path']
```

### Comparing `shakenfist-agent-0.3.8/shakenfist_agent/main.py` & `shakenfist-agent-0.3.9/shakenfist_agent/main.py`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.8/shakenfist_agent/protocol.py` & `shakenfist-agent-0.3.9/shakenfist_agent/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,16 +161,15 @@
                 })
 
     def noop(self, packet):
         return
 
     def log_error_packet(self, packet):
         if self.log:
-            self.log.with_fields(packet).error(
-                'Received a packet indicating an error')
+            self.log.with_fields(packet).error('Received a packet indicating an error')
 
     def send_ping(self, unique=None):
         if not unique:
             unique = random.randint(0, 65535)
 
         self.send_packet({
             'command': 'ping',
```

### Comparing `shakenfist-agent-0.3.8/shakenfist_agent/tests/test_daemon.py` & `shakenfist-agent-0.3.9/shakenfist_agent/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.8/shakenfist_agent/tests/test_protocol.py` & `shakenfist-agent-0.3.9/shakenfist_agent/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.8/shakenfist_agent.egg-info/PKG-INFO` & `shakenfist-agent-0.3.9/shakenfist_agent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shakenfist-agent
-Version: 0.3.8
+Version: 0.3.9
 Summary: An in-guest agent for instances running on Shaken Fist
 Home-page: https://madebymikal.com/shakenfist
 Author: Michael Still
 Author-email: mikal@stillhq.com
 License: Apache2
 Description: Python side channel agent for Shaken Fist
         =========================================
```

### Comparing `shakenfist-agent-0.3.8/shakenfist_agent.egg-info/SOURCES.txt` & `shakenfist-agent-0.3.9/shakenfist_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.8/tools/flake8wrap.sh` & `shakenfist-agent-0.3.9/tools/flake8wrap.sh`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.8/tox.ini` & `shakenfist-agent-0.3.9/tox.ini`

 * *Files identical despite different names*

