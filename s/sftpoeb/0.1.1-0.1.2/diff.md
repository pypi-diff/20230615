# Comparing `tmp/sftpoeb-0.1.1.tar.gz` & `tmp/sftpoeb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sftpoeb-0.1.1.tar", last modified: Wed Jun 14 06:41:32 2023, max compression
+gzip compressed data, was "sftpoeb-0.1.2.tar", last modified: Thu Jun 15 12:03:14 2023, max compression
```

## Comparing `sftpoeb-0.1.1.tar` & `sftpoeb-0.1.2.tar`

### file list

```diff
@@ -1,52 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.161103 sftpoeb-0.1.1/
--rw-rw-rw-   0        0        0      609 2023-06-14 06:41:02.000000 sftpoeb-0.1.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1031 2023-06-14 06:41:32.160103 sftpoeb-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.1.1/README.txt
--rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 06:41:32.161103 sftpoeb-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      603 2023-06-14 06:41:14.000000 sftpoeb-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.040118 sftpoeb-0.1.1/sftpoeb/
--rw-rw-rw-   0        0        0       72 2023-06-14 03:50:21.000000 sftpoeb-0.1.1/sftpoeb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.073103 sftpoeb-0.1.1/sftpoeb/config/
--rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.1.1/sftpoeb/config/variable.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.078111 sftpoeb-0.1.1/sftpoeb/mainclass/
--rw-rw-rw-   0        0        0       21 2023-06-14 03:49:30.000000 sftpoeb-0.1.1/sftpoeb/mainclass/__init__.py
--rw-rw-rw-   0        0        0     1527 2023-06-14 04:59:52.000000 sftpoeb-0.1.1/sftpoeb/mainclass/c_sftp.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.099127 sftpoeb-0.1.1/sftpoeb/method/
--rw-rw-rw-   0        0        0       74 2023-06-14 03:49:57.000000 sftpoeb-0.1.1/sftpoeb/method/__init__.py
--rw-rw-rw-   0        0        0     4793 2023-06-14 04:14:04.000000 sftpoeb-0.1.1/sftpoeb/method/callservice.py
--rw-rw-rw-   0        0        0      546 2023-06-09 11:32:38.000000 sftpoeb-0.1.1/sftpoeb/method/checkpath.py
--rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.1.1/sftpoeb/method/debug.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.122109 sftpoeb-0.1.1/sftpoeb/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.1.1/sftpoeb/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.1.1/sftpoeb/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.1.1/sftpoeb/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.1.1/sftpoeb/sftpoeb.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.125105 sftpoeb-0.1.1/sftpoeb/subclass/
--rw-rw-rw-   0        0        0      109 2023-06-14 03:50:15.000000 sftpoeb-0.1.1/sftpoeb/subclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.132122 sftpoeb-0.1.1/sftpoeb/subclass/file/
--rw-rw-rw-   0        0        0       57 2023-06-14 03:50:45.000000 sftpoeb-0.1.1/sftpoeb/subclass/file/__init__.py
--rw-rw-rw-   0        0        0     2892 2023-06-14 04:00:58.000000 sftpoeb-0.1.1/sftpoeb/subclass/file/s_c_file.py
--rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.1.1/sftpoeb/subclass/file/s_c_file_transfer.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.137105 sftpoeb-0.1.1/sftpoeb/subclass/input/
--rw-rw-rw-   0        0        0       24 2023-06-14 03:50:57.000000 sftpoeb-0.1.1/sftpoeb/subclass/input/__init__.py
--rw-rw-rw-   0        0        0     1162 2023-06-14 04:01:07.000000 sftpoeb-0.1.1/sftpoeb/subclass/input/s_c_input.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.141105 sftpoeb-0.1.1/sftpoeb/subclass/output/
--rw-rw-rw-   0        0        0       25 2023-06-14 03:51:08.000000 sftpoeb-0.1.1/sftpoeb/subclass/output/__init__.py
--rw-rw-rw-   0        0        0     1171 2023-06-14 04:01:13.000000 sftpoeb-0.1.1/sftpoeb/subclass/output/s_c_output.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.153105 sftpoeb-0.1.1/sftpoeb/subclass/path/
--rw-rw-rw-   0        0        0      103 2023-06-14 03:51:28.000000 sftpoeb-0.1.1/sftpoeb/subclass/path/__init__.py
--rw-rw-rw-   0        0        0     4508 2023-06-14 04:47:33.000000 sftpoeb-0.1.1/sftpoeb/subclass/path/s_c_setgetdestination.py
--rw-rw-rw-   0        0        0     3999 2023-06-14 04:01:25.000000 sftpoeb-0.1.1/sftpoeb/subclass/path/s_c_setgetlocal.py
--rw-rw-rw-   0        0        0     1875 2023-06-14 04:59:14.000000 sftpoeb-0.1.1/sftpoeb/subclass/path/s_c_setgetrecovery.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.157103 sftpoeb-0.1.1/sftpoeb/subclass/process/
--rw-rw-rw-   0        0        0       36 2023-06-14 03:51:39.000000 sftpoeb-0.1.1/sftpoeb/subclass/process/__init__.py
--rw-rw-rw-   0        0        0    29080 2023-06-14 04:01:40.000000 sftpoeb-0.1.1/sftpoeb/subclass/process/s_c_process_package_1.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.066109 sftpoeb-0.1.1/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0     1031 2023-06-14 06:41:31.000000 sftpoeb-0.1.1/sftpoeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1140 2023-06-14 06:41:31.000000 sftpoeb-0.1.1/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 06:41:31.000000 sftpoeb-0.1.1/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-06-14 06:41:31.000000 sftpoeb-0.1.1/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-14 06:41:31.000000 sftpoeb-0.1.1/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.920023 sftpoeb-0.1.2/
+-rw-rw-rw-   0        0        0      661 2023-06-15 12:02:57.000000 sftpoeb-0.1.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1083 2023-06-15 12:03:14.919027 sftpoeb-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.1.2/README.txt
+-rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 12:03:14.920023 sftpoeb-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      603 2023-06-15 12:02:49.000000 sftpoeb-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.750018 sftpoeb-0.1.2/sftpoeb/
+-rw-rw-rw-   0        0        0       72 2023-06-15 12:00:06.000000 sftpoeb-0.1.2/sftpoeb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.782023 sftpoeb-0.1.2/sftpoeb/config/
+-rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.1.2/sftpoeb/config/variable.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.790026 sftpoeb-0.1.2/sftpoeb/mainclass/
+-rw-rw-rw-   0        0        0       48 2023-06-15 12:01:46.000000 sftpoeb-0.1.2/sftpoeb/mainclass/__init__.py
+-rw-rw-rw-   0        0        0     1805 2023-06-15 12:00:49.000000 sftpoeb-0.1.2/sftpoeb/mainclass/c_recovery.py
+-rw-rw-rw-   0        0        0     3558 2023-06-15 08:31:33.000000 sftpoeb-0.1.2/sftpoeb/mainclass/c_sftp.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.802017 sftpoeb-0.1.2/sftpoeb/method/
+-rw-rw-rw-   0        0        0       95 2023-06-14 12:04:10.000000 sftpoeb-0.1.2/sftpoeb/method/__init__.py
+-rw-rw-rw-   0        0        0     4839 2023-06-14 11:11:17.000000 sftpoeb-0.1.2/sftpoeb/method/callservice.py
+-rw-rw-rw-   0        0        0      601 2023-06-14 06:57:02.000000 sftpoeb-0.1.2/sftpoeb/method/checkpath.py
+-rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.1.2/sftpoeb/method/debug.py
+-rw-rw-rw-   0        0        0     9657 2023-06-15 07:54:02.000000 sftpoeb-0.1.2/sftpoeb/method/mail.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.837021 sftpoeb-0.1.2/sftpoeb/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.1.2/sftpoeb/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.1.2/sftpoeb/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.1.2/sftpoeb/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.1.2/sftpoeb/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.839024 sftpoeb-0.1.2/sftpoeb/subclass/
+-rw-rw-rw-   0        0        0      131 2023-06-15 08:04:07.000000 sftpoeb-0.1.2/sftpoeb/subclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.843020 sftpoeb-0.1.2/sftpoeb/subclass/alert/
+-rw-rw-rw-   0        0        0       24 2023-06-15 07:57:29.000000 sftpoeb-0.1.2/sftpoeb/subclass/alert/__init__.py
+-rw-rw-rw-   0        0        0     1515 2023-06-15 11:41:55.000000 sftpoeb-0.1.2/sftpoeb/subclass/alert/s_c_alert.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.851018 sftpoeb-0.1.2/sftpoeb/subclass/file/
+-rw-rw-rw-   0        0        0       57 2023-06-14 03:50:45.000000 sftpoeb-0.1.2/sftpoeb/subclass/file/__init__.py
+-rw-rw-rw-   0        0        0     2892 2023-06-14 04:00:58.000000 sftpoeb-0.1.2/sftpoeb/subclass/file/s_c_file.py
+-rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.1.2/sftpoeb/subclass/file/s_c_file_transfer.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.871020 sftpoeb-0.1.2/sftpoeb/subclass/input/
+-rw-rw-rw-   0        0        0       24 2023-06-14 03:50:57.000000 sftpoeb-0.1.2/sftpoeb/subclass/input/__init__.py
+-rw-rw-rw-   0        0        0     1162 2023-06-14 04:01:07.000000 sftpoeb-0.1.2/sftpoeb/subclass/input/s_c_input.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.887017 sftpoeb-0.1.2/sftpoeb/subclass/output/
+-rw-rw-rw-   0        0        0       25 2023-06-14 03:51:08.000000 sftpoeb-0.1.2/sftpoeb/subclass/output/__init__.py
+-rw-rw-rw-   0        0        0     1171 2023-06-14 04:01:13.000000 sftpoeb-0.1.2/sftpoeb/subclass/output/s_c_output.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.903025 sftpoeb-0.1.2/sftpoeb/subclass/path/
+-rw-rw-rw-   0        0        0      103 2023-06-14 03:51:28.000000 sftpoeb-0.1.2/sftpoeb/subclass/path/__init__.py
+-rw-rw-rw-   0        0        0     5206 2023-06-14 10:57:49.000000 sftpoeb-0.1.2/sftpoeb/subclass/path/s_c_setgetdestination.py
+-rw-rw-rw-   0        0        0     4239 2023-06-14 10:57:44.000000 sftpoeb-0.1.2/sftpoeb/subclass/path/s_c_setgetlocal.py
+-rw-rw-rw-   0        0        0     2042 2023-06-15 11:58:34.000000 sftpoeb-0.1.2/sftpoeb/subclass/path/s_c_setgetrecovery.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.908021 sftpoeb-0.1.2/sftpoeb/subclass/process/
+-rw-rw-rw-   0        0        0       36 2023-06-14 03:51:39.000000 sftpoeb-0.1.2/sftpoeb/subclass/process/__init__.py
+-rw-rw-rw-   0        0        0    30032 2023-06-15 08:48:28.000000 sftpoeb-0.1.2/sftpoeb/subclass/process/s_c_process_package_1.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.781020 sftpoeb-0.1.2/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0     1083 2023-06-15 12:03:14.000000 sftpoeb-0.1.2/sftpoeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1274 2023-06-15 12:03:14.000000 sftpoeb-0.1.2/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 12:03:14.000000 sftpoeb-0.1.2/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-06-15 12:03:14.000000 sftpoeb-0.1.2/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-15 12:03:14.000000 sftpoeb-0.1.2/sftpoeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1107 2023-06-15 08:22:57.000000 sftpoeb-0.1.2/test.py
```

### Comparing `sftpoeb-0.1.1/CHANGELOG.txt` & `sftpoeb-0.1.2/CHANGELOG.txt`

 * *Files 6% similar despite different names*

```diff
@@ -39,8 +39,12 @@
 
 0.1.0 (14/06/2023)
 ------------------
 - Fixbug
 
 0.1.1 (14/06/2023)
 ------------------
+- Fixbug
+
+0.1.2 (15/06/2023)
+------------------
 - Fixbug
```

### Comparing `sftpoeb-0.1.1/LICENSE.txt` & `sftpoeb-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.1/PKG-INFO` & `sftpoeb-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.1.1
+Version: 0.1.2
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
@@ -59,7 +59,11 @@
 ------------------
 - Fixbug
 
 0.1.1 (14/06/2023)
 ------------------
 - Fixbug
 
+0.1.2 (15/06/2023)
+------------------
+- Fixbug
+
```

### Comparing `sftpoeb-0.1.1/setup.py` & `sftpoeb-0.1.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
         name='sftpoeb',
-        version='0.1.1',
+        version='0.1.2',
         url='',
         license='MIT',
         author='Natthawut Thawisombat',
         author_email='natthawut.th@inet.co.th',
         description='To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling',
         packages=find_packages(),
         long_description=open('README.txt').read() +  '\n\n' + open('CHANGELOG.txt').read(),
```

### Comparing `sftpoeb-0.1.1/sftpoeb/mainclass/c_sftp.py` & `sftpoeb-0.1.2/sftpoeb/mainclass/c_recovery.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 from ..subclass.path.s_c_setgetlocal import *
 from ..subclass.path.s_c_setgetdestination import *
 from ..subclass.path.s_c_setgetrecovery import *
 from ..subclass.file.s_c_file import *
 from ..subclass.process.s_c_process_package_1 import *
+from ..subclass import *
 from datetime import date, datetime
 from ..subclass.input.s_c_input import *
-class SFTP():
-    def __init__(self,myPath="None",sftpPath="None",custPath="None",payloadData="None"):
+from ..method.mail import *
+from ..method.debug import *
+
+class RECOVERY():
+    def __init__(self,myPath="None",sftpPath="None",custPath="None",payloadData="None",userSftp="None",groupSftp ="None"):
         self.myPath = myPath
         self.sftpPath = sftpPath
         self.custPath = custPath
+        self.userSftp = userSftp
+        self.groupSftp = groupSftp
         self.dateNow = datetime.now().strftime("%Y%m%d")
         self.timeNow = datetime.now().strftime("%H%M%S")
+        self.process_now = str(self.dateNow + self.timeNow)
         self.payloadData = payloadData
         ### Local
         self.local = setgetlocal(self.myPath,self.sftpPath,self.dateNow,self.timeNow)
         ### Destination
         self.destination = setgetdestination(self.custPath,self.sftpPath,self.dateNow,self.timeNow)
         ### Recovery
         self.recovery = setgetrecovery(self.myPath,self.sftpPath,self.dateNow,self.timeNow)
-        ### inputFile
-        self.input = inputFile(self.local,self.destination,self.dateNow,self.timeNow)
+        ### alert
+        self.alert = alert()
 
-    def package1(self,quantityThread):
+    def formation1(self):
+        try:
 
-        ### เปิดคลาสกระบวนการดำเนินการไฟล์
-        c_process = packageprocess(self.local,self.destination,self.recovery,self.payloadData,self.dateNow,self.timeNow)
-        c_process.runThreadProcess(quantityThread)
-        c_process.writelog()
-        c_process.finalProcess()
+            print(str(self.dateNow + self.timeNow) + '>> API Recovery : Process Recovery done.')
+            result = {"status": "OK", "message": "Process Recovery done."}
+        except Exception as e:
+            print(str(self.dateNow + self.timeNow) + '>> API Recovery error : ' + str(debug_row(e)))
+            result = {"status": "ER","errorCode":"PR999", "errorMessage": 'API Recovery error : '+str(debug_row(e))}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sftpoeb-0.1.1/sftpoeb/method/callservice.py` & `sftpoeb-0.1.2/sftpoeb/method/callservice.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 import os,requests,time,urllib3
 urllib3.disable_warnings()
 
-def serviceSigning(data, fileNameText, fileNamePDF, pathFile,round,serviceCode):
+def serviceSigning(data, fileNameText, fileNamePDF, pathFile,round,serviceCode,URL):
     multipart_data = MultipartEncoder(
         fields={
             "SellerTaxId": data['SellerTaxid'],
             "SellerBranchId": data['SellerBranchId'],
             "APIKey": data['APIKey'],
             "UserCode": data['UserCode'],
             "AccessKey": data['AccessKey'],
             "ServiceCode": serviceCode,
             "TextContent": (fileNameText, open(os.path.abspath(os.path.join(pathFile + '/' + fileNameText)), 'rb'), "multipart/form-data"),
-            "PDFContent": (fileNamePDF, open(os.path.abspath(os.path.join(pathFile + '/' + fileNamePDF)), 'rb'), "multipart/form-data"),
+            # "PDFContent": (fileNamePDF, open(os.path.abspath(os.path.join(pathFile + '/' + fileNamePDF)), 'rb'), "multipart/form-data"),
             "SendMail": "YES"
             # "PdfTemplateId":PdfTemplateId
         }
     )
     headers = {
         'Content-Type': multipart_data.content_type,
         'Authorization': data['Authorization']
     }
     try:
-        response = requests.post("", data=multipart_data, headers=headers, verify=False)
+        response = requests.post(URL, data=multipart_data, headers=headers, verify=False)
         if response.status_code == 200:
             result = response.json()
         else:
             if round < 3:
                 time.sleep(0.5)
                 result = serviceSigning(data, fileNameText, fileNamePDF, pathFile,round+1,serviceCode)
             else:
@@ -43,47 +43,47 @@
             result = {
                 "status": "ER",
                 "errorCode": "EXC001",
                 "errorMessage": "send_for_getfile : " + str(e)
             }
     return result
     
-def checkStatus(data,TransactionCode,round):
+def checkStatus(data,TransactionCode,round,serviceCode,URL):
     multipart_data = MultipartEncoder(
         fields={
             "SellerTaxId":data['SellerTaxid'],
             "SellerBranchId": data['SellerBranchId'],
             "APIKey": data['APIKey'],
             "UserCode": data['UserCode'],
             "AccessKey": data['AccessKey'],
             "TransactionCode": TransactionCode,
-            "ServiceCode": "S06"
+            "ServiceCode": serviceCode
         }
     )
     headers = {
         'Content-Type': multipart_data.content_type,
         'Authorization': data['Authorization']
     }
     try:
-        response = requests.post("", data=multipart_data, headers=headers, verify=True)
+        response = requests.post(URL, data=multipart_data, headers=headers, verify=True)
         if response.status_code == 200:
             result = response.json()
             print(result)
             if result['status'] == "OK":
                 return result
             elif round == 20:
                 result = {
                     "status": "PR",
                     "errorMessage": "Service Check transaction 20 rounds",
                     "errorCode": "ERPC002"
                 }
                 return result
             elif result['status'] == "PC":
                 time.sleep(0.5 + (round / 2))
-                result = checkStatus(data,TransactionCode,round+1)
+                result = checkStatus(data,TransactionCode,round+1,serviceCode,URL)
             else:
                 print("Service Stamp [PC] failed.")
                 return result
         else:
             res = response.json()
             print(res)
             result = {
```

### Comparing `sftpoeb-0.1.1/sftpoeb/method/checkpath.py` & `sftpoeb-0.1.2/sftpoeb/method/checkpath.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os, sys
 
 def check_path(path):
-    split_path = path.split('/')
-    mix_path = ""
-    for i in split_path:
-        if i != "":
-            mix_path = mix_path + "/" + i
-            # print(mix_path)
-            try:
-                if not os.path.exists(mix_path):
-                    os.mkdir(mix_path)
-                    print("Create path " + mix_path)
-            except Exception as e:
-                print("Check path => "+ str(e))
+    # split_path = path.split('/')
+    # mix_path = ""
+    # for i in split_path:
+    #     if i != "":
+    #         mix_path = mix_path + "/" + i
+    #         # print(mix_path)
+    #         try:
+    #             if not os.path.exists(mix_path):
+    #                 os.mkdir(mix_path)
+    #                 print("Create path " + mix_path)
+    #         except Exception as e:
+    #             print("Check path => "+ str(e))
     if os.path.exists(path):
         return True
     else:
+        os.makedirs(path,777)
         return False
```

### Comparing `sftpoeb-0.1.1/sftpoeb/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.1.2/sftpoeb/sftpoeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.1/sftpoeb/subclass/file/s_c_file.py` & `sftpoeb-0.1.2/sftpoeb/subclass/file/s_c_file.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.1/sftpoeb/subclass/file/s_c_file_transfer.py` & `sftpoeb-0.1.2/sftpoeb/subclass/file/s_c_file_transfer.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.1/sftpoeb/subclass/input/s_c_input.py` & `sftpoeb-0.1.2/sftpoeb/subclass/input/s_c_input.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.1/sftpoeb/subclass/output/s_c_output.py` & `sftpoeb-0.1.2/sftpoeb/subclass/output/s_c_output.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.1/sftpoeb/subclass/path/s_c_setgetdestination.py` & `sftpoeb-0.1.2/sftpoeb/subclass/path/s_c_setgetdestination.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from datetime import datetime
 from ...method.checkpath import *
 class setgetdestination():
     def __init__(self,custPath,sftpPath,dateNow,timeNow):
         self.formatOld = '%Y%m%d'
         self.formatNew = '%Y-%m-%d'
         self.destinationPath = custPath + "/" + sftpPath + "/"
+        self.destinationInbound = custPath + "/" + sftpPath + "/Inbound/"
         self.destinationPathCSV = custPath + "/" + sftpPath + "/Inbound/CSV/"
         self.destinationPathPDF = custPath + "/" + sftpPath + "/Inbound/PDF/"
+        self.destinationHistory = custPath + "/" + sftpPath + '/History/' + self.transformDate(dateNow) + '/'
         self.destinationCsvArchivePath = custPath + "/" + sftpPath + '/History/' + self.transformDate(dateNow) + '/CSV/Archived_File/'
         self.destinationCsvErrorPath = custPath + "/" + sftpPath + '/History/' + self.transformDate(dateNow) + '/CSV/Error_File/'
         self.destinationPdfArchivePath = custPath + "/" + sftpPath + '/History/' + self.transformDate(dateNow) + '/PDF/Archived_File/'
         self.destinationPdfErrorPath = custPath + "/" + sftpPath + '/History/' + self.transformDate(dateNow) + '/PDF/Error_File/'
         self.destinationOutputPdfPath = custPath + "/" + sftpPath + '/Outbound/' + self.transformDate(dateNow) + '/PDF/'
         self.destinationOutputXmlPath = custPath + "/" + sftpPath + '/Outbound/' + self.transformDate(dateNow) + '/XML/'
         self.destinationLogPath = custPath + "/" + sftpPath + '/Outbound/' + self.transformDate(dateNow) + '/Logfile/'
@@ -51,17 +53,33 @@
     def setDestinationOutputXmlPath(self,path):
         self.destinationOutputXmlPath = path
         return self.destinationOutputXmlPath
 
     def setDestinationLogPath(self,path):
         self.destinationLogPath = path
         return self.destinationLogPath
+    
+    def setDestinationHistory(self,path):
+        self.destinationHistory = path
+        return self.destinationHistory
+    
+    def setDestinationInbound(self,path):
+        self.destinationInbound = path
+        return self.destinationInbound
 ########## END SET ############
 
 ########## GET ############
+    def getDestinationInbound(self):
+        check_path(self.destinationInbound)
+        return self.destinationInbound
+    
+    def getDestinationHistory(self):
+        check_path(self.destinationHistory)
+        return self.destinationHistory
+
     def getDestinationPath(self):
         check_path(self.destinationPath)
         return self.destinationPath
 
     def getDestinationPathCSV(self):
         check_path(self.destinationPathCSV)
         return self.destinationPathCSV
```

### Comparing `sftpoeb-0.1.1/sftpoeb/subclass/path/s_c_setgetlocal.py` & `sftpoeb-0.1.2/sftpoeb/subclass/path/s_c_setgetlocal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from datetime import datetime
 from ...method.checkpath import *
 class setgetlocal():
     def __init__(self,myPath,sftpPath,dateNow,timeNow):
         self.formatOld = '%Y%m%d'
         self.formatNew = '%Y-%m-%d'
+        self.myPath = myPath
         self.localPath = myPath + "/" + sftpPath + "/Inbound/"
         self.localFilerun = self.localPath+ '/Filerun/' + self.transformDate(dateNow) + '/'
         self.localPathNow = self.localPath + "/" + str( dateNow + timeNow ) + "/"
+        self.localHistory = myPath + "/" + sftpPath + "/History/" + self.transformDate(dateNow) + '/'
         self.localCsvArchivePath = myPath + "/" + sftpPath + "/History/" + self.transformDate(dateNow) + '/CSV/Archived_File/'
         self.localCsvErrorPath = myPath + "/" + sftpPath + "/History/" + self.transformDate(dateNow) + '/CSV/Error_File/'
         self.localPdfArchivePath = myPath + "/" + sftpPath + "/History/" + self.transformDate(dateNow) + '/PDF/Archived_File/'
         self.localPdfErrorPath = myPath + "/" + sftpPath + "/History/" + self.transformDate(dateNow) + '/PDF/Error_File/'
         self.localOutputPdfPath = myPath + "/" + sftpPath + "/Outbound/" + self.transformDate(dateNow) + '/PDF/'
         self.localOutputXmlPath = myPath + "/" + sftpPath + "/Outbound/" + self.transformDate(dateNow) + '/XML/'
         self.localLogPath = myPath + "/" + sftpPath + "/Outbound/" + self.transformDate(dateNow) + '/Logfile/'
@@ -51,14 +53,18 @@
     def setLocalLogPath(self,path):
         self.localLogPath = path
         return self.localLogPath
     
 ########## END SET ############
 
 ########## GET ############
+    def getLocalHistory(self):
+        check_path(self.localHistory)
+        return self.localHistory
+
     def getLocalPath(self):
         check_path(self.localPath)
         return self.localPath
 
     def getLocalFileRun(self):
         check_path(self.localFilerun)
         return self.localFilerun
```

### Comparing `sftpoeb-0.1.1/sftpoeb/subclass/process/s_c_process_package_1.py` & `sftpoeb-0.1.2/sftpoeb/subclass/process/s_c_process_package_1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from ...method.callservice import *
 from ...method.debug import *
 from os import listdir
 from os.path import isfile, join, isdir
 import threading
 import shutil,json
 class packageprocess():
-    def __init__(self,local,destination,recovery,payloadData,dateNow,timeNow):
+    def __init__(self,local,destination,recovery,payloadData,dateNow,timeNow,usersftp,groupsftp):
         self.local = local
+        self.usersftp = usersftp
+        self.groupsftp = groupsftp
         self.destination = destination
         self.payloadData = payloadData
         self.recovery = recovery
         self.dateNow = dateNow
         self.timeNow = timeNow
 
         self.countInvoice = 0
@@ -22,42 +24,53 @@
 
         ### เก็บข้อมูลการทำงานรอบ recover
         self.success_recovery_message = []
         self.success_recovery = 0
         self.fail_recovery_message = []
         self.fail_recovery = 0
 
+        ### URL
+        self.SERVICE_SIGNING_URL = "https://uatservice-etax.one.th/etaxdocumentws/etaxsigndocument"
+        self.SERVICE_CHECKSTATUS_URL = "https://uatservice-etax.one.th/etaxdocumentws/etaxgetdocumentstatus"
     def process(self,dataProcess):
         for filename in dataProcess:
             name = str(filename).split('.')[0]
+            serviceCode = 'S03'
             try:
-                serviceCode = 'S06'
-                shutil.move(self.destination.getDestinationPathPDF() + name + '.pdf', self.local.getLocalPathNow() + name + '.pdf')  #### วนหยิบ PDF ตามชื่อ text ที่แตกดป็น 1:1 แล้ว
-                service = serviceSigning(self.payloadData, filename, name + '.pdf', self.local.getLocalPathNow() , 0, serviceCode)
+                ### ทำการ copy file ไปไว้ที่ History และ ย้ายไป path local
+                shutil.copy(self.destination.destinationInbound + name + '.csv', self.local.getLocalHistory() + name + '.csv')
+                shutil.copy(self.destination.destinationInbound + name + '.csv', self.destination.getDestinationHistory() + name + '.csv')
+                shutil.move(self.destination.destinationInbound + name + '.csv', self.local.getLocalPathNow() + name + '.csv')  #### วนหยิบ PDF ตามชื่อ text ที่แตกดป็น 1:1 แล้ว
+                
+                ### นำส่งไฟล์ไปทำ E-Tax Invoice ผ่าน API
+                service = serviceSigning(self.payloadData, filename, name + '.pdf', self.local.getLocalPathNow() , 0, serviceCode,self.SERVICE_SIGNING_URL)
                 if service['status'] == 'OK':
                     self.success = self.success + 1
                     print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Service signing success.')
+                    
                     save_pdf = saveFile(service['pdfURL'], self.local.getLocalOutputPdfPath(), name + '.pdf', 0)
                     if save_pdf['status'] == 'OK':
                         print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Save file.pdf success.')
                         shutil.copy(self.local.getLocalOutputPdfPath() + name + '.pdf', self.destination.getDestinationOutputPdfPath() + name + '.pdf')
                         print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Put file.pdf success.')
                         pdf_result = 'OK'  ### เก็บ สถานะการทำงานในส่วน PDF
                     else:
                         print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Save file.pdf failed. : ' + str(save_pdf['errorMessage']))
                         pdf_result = 'ER'  ### เก็บ สถานะการทำงานในส่วน PDF
+                    
                     save_xml = saveFile(service['xmlURL'],self.local.getLocalOutputXmlPath(), name + '.xml', 0)
                     if save_xml['status'] == 'OK':
                         print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Save file.xml success.')
                         shutil.copy(self.local.getLocalOutputXmlPath() + name + '.xml',self.destination.getDestinationOutputXmlPath() + name + '.xml')
                         print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Put file.xml success.')
                         xml_result = 'OK'  ### เก็บ สถานะการทำงานในส่วน XML
                     else:
                         print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Save file.xml failed. : ' + str(save_xml['errorMessage']))
                         xml_result = 'ER'  ### เก็บ สถานะการทำงานในส่วน XML
+                    
                     ##########นับว่า สำเร็จ หรือ ไม่สำเร็จ #######
                     if pdf_result != 'OK' and xml_result != 'OK':  ### ถ้าสถานะของทั้ง xml และ pdf สำเร็จทั้งคู่จึงจะนับว่า invoice นั้นสำเร็จ
                         with open(self.recovery.getRecoverySavePath() + filename, 'w',encoding='UTF-8') as recover_file: ### สร้างไฟล์เพื่อ recover save
                             recover_file.write(json.dumps({"transactionCode": service['transactionCode']}, indent=4, sort_keys=False,ensure_ascii=False))
                     
                     
                     try:  ##### ขั้นตอนไป filerun
@@ -68,28 +81,28 @@
                     ### เก็บไว้ส่งในส่วนของการส่งคืนลูกค้า
                     # try:  ##### ขั้นตอนไป filerun
                     #     shutil.copy(self.destination.getDestinationCsvArchivePath() + filename, self.local.getLocalCsvArchivePath() + filename)
                     # except Exception as e:
                     #     print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Copy CSV input to Archived_File failed : ' + str(e))
                     
                     
-                    try:  ##### ขั้นตอนไป filerun
-                        shutil.move(self.local.getLocalPathNow() + name + '.pdf', self.local.getLocalPdfArchivePath() + name + '.pdf')  #### วาง PDF ที่ error ที่ path filerun error ฝั่งลูกค้า
-                    except Exception as e:
-                        print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Move PDF input to Archived_File failed : ' + str(e))
+                    # try:  ##### ขั้นตอนไป filerun
+                    #     shutil.move(self.local.getLocalPathNow() + name + '.pdf', self.local.getLocalPdfArchivePath() + name + '.pdf')  #### วาง PDF ที่ error ที่ path filerun error ฝั่งลูกค้า
+                    # except Exception as e:
+                    #     print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Move PDF input to Archived_File failed : ' + str(e))
                     
                     ### เก็บไว้ส่งในส่วนของการส่งคืนลูกค้า
                     # try:  ##### ขั้นตอนไป filerun
                     #     shutil.copy(self.destination.getDestinationPdfArchivePath() + name + '.pdf', self.local.getLocalPdfArchivePath() + name + '.pdf')  #### วาง PDF ที่ error ที่ path filerun error ฝั่งลูกค้า
                     # except Exception as e:
                     #     print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Copy PDF input to Archived_File failed : ' + str(e))
                 
                 elif service['status'] == 'PC':
                     print(str(service['transactionCode']))
-                    pc_result = checkStatus(self.payloadData, service['transactionCode'], 0)
+                    pc_result = checkStatus(self.payloadData, service['transactionCode'], 0,serviceCode,self.SERVICE_CHECKSTATUS_URL)
                     print(pc_result)
                     if pc_result['status'] == 'OK':
                         self.success = self.success + 1
                         print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Service signing success.')
                         save_pdf_pc = saveFile(pc_result['pdfURL'], self.local.getLocalOutputPdfPath(), name + '.pdf', 0)
                         if save_pdf_pc['status'] == 'OK':
                             print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Save file.pdf success.')
@@ -199,26 +212,26 @@
                         self.recover_count += 1
                         self.recover.append({
                             "invoiceNo": name,
                             "errorCode": str(service["errorCode"]),
                             "errorMessage": str(service["errorMessage"])
                         })
                         shutil.move(self.local.getLocalPathNow() + filename, self.recovery.getRecoverySignPath()+ filename)
-                        shutil.move(self.local.getLocalPathNow() + name + '.pdf', self.recovery.getRecoverySignPath()+ name + '.pdf')
+                        # shutil.move(self.local.getLocalPathNow() + name + '.pdf', self.recovery.getRecoverySignPath()+ name + '.pdf')
                     elif service['errorCode'] == "ER021" or service['errorCode'] == "EX01" or service['errorCode'] == "ER004" or service['errorCode'] == "PC001" or service['errorCode'] == "ERPC002":
                         self.recover_count += 1
                         self.recover.append({
                             "invoiceNo": name,
                             "errorCode": str(service["errorCode"]),
                             "errorMessage": str(service["errorMessage"])
                         })
                         with open(self.recovery.getRecoveryCheckPath() + name + '.txt', 'w',encoding='UTF-8') as recover_file: ### สร้างไฟล์เพื่อ recover check
                             recover_file.write(json.dumps({"transactionCode": service['transactionCode']}, indent=4, sort_keys=False,ensure_ascii=False))
                         shutil.move(self.local.getLocalPathNow() + filename, self.recovery.getPeddingPath()+ filename)
-                        shutil.move(self.local.getLocalPathNow() + name + '.pdf', self.recovery.getPeddingPath()+ name + '.pdf')
+                        # shutil.move(self.local.getLocalPathNow() + name + '.pdf', self.recovery.getPeddingPath()+ name + '.pdf')
                     else:
                         self.fail = self.fail + 1
                         print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Service singning failed. : ' + str(service['errorMessage']))
                         self.losemessage.append({
                             'InvoiceName': str(name),
                             'Process DTM': str(self.dateNow + self.timeNow),
                             'errorCode': service['errorCode'],
@@ -240,18 +253,18 @@
                             print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Move CSV input to Error_File failed : ' + str(e))
                         # try:  ##### ขั้นตอนไป filerun
                         #     shutil.copy(self.destination.getDestinationCsvErrorPath() + filename, self.local.getLocalCsvErrorPath() + filename)
                         # except Exception as e:
                         #     print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Copy CSV input to Error_File failed : ' + str(e))
                         
                         
-                        try:  ##### ขั้นตอนไป filerun
-                            shutil.move(self.local.getLocalPathNow() + name + '.pdf', self.local.getLocalPdfErrorPath()  + name + '.pdf')  #### วาง PDF ที่ error ที่ path filerun error ฝั่งลูกค้า
-                        except Exception as e:
-                            print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Move PDF input to Error_File failed : ' + str(e))
+                        # try:  ##### ขั้นตอนไป filerun
+                        #     shutil.move(self.local.getLocalPathNow() + name + '.pdf', self.local.getLocalPdfErrorPath()  + name + '.pdf')  #### วาง PDF ที่ error ที่ path filerun error ฝั่งลูกค้า
+                        # except Exception as e:
+                        #     print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Move PDF input to Error_File failed : ' + str(e))
                         # try:  ##### ขั้นตอนไป filerun
                         #     shutil.copy(self.destination.getDestinationPdfErrorPath() + name + '.pdf', self.local.getLocalPdfErrorPath() + name + '.pdf')  #### วาง PDF ที่ error ที่ path filerun error ฝั่งลูกค้า
                         # except Exception as e:
                         #     print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Copy PDF input to Error_File failed : ' + str(e))
             except KeyError as ke:
                 self.recover_count += 1
                 self.recover.append({
@@ -290,16 +303,16 @@
                 #     print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Copy PDF input to Error_File failed : ' + str(e))
 
     def testprocess(self,var):
         print("var == " + str(var))
 
     def runThreadProcess(self,quantityThread=1):
         try:
-            allCSV = [f for f in listdir(self.local.getLocalPathNow()) if isfile(join(self.local.getLocalPathNow(), f))]
-            # allCSV = ["1","2","3","4"]
+            allCSV = [f for f in listdir(self.destination.destinationInbound) if isfile(join(self.destination.destinationInbound, f))]
+
             self.countInvoice = len(allCSV)
             divInvoice = (self.countInvoice // quantityThread)
             arrVariable = []
             for i in range(quantityThread):
                 arrVariable.append("ThreadProcess" + str(i))
             
             try:
@@ -363,11 +376,11 @@
                 print(str(self.dateNow + self.timeNow) + '>>  Put log path error : ' + str(e))
         except Exception as e:
             print(str(self.dateNow + self.timeNow) + '>>  Write log path error : ' + str(e))
 
     def finalProcess(self):
         try:
             shutil.rmtree(self.local.getLocalPathNow())  ### เมื่อทำงานครบรอบแล้วจะลบ folder input ของรอบนั้นทิ้ง
-            os.system("sudo chown -R kpc.prd:sftpuser " + str(self.local.myPath))
+            os.system("sudo chown -R "+self.usersftp+":"+self.groupsftp+" " + str(self.local.myPath))
         except Exception as e:
             print(str(self.dateNow + self.timeNow) + '>>  Remove Processed Round Folder failed. : ' + str(e))
             result = {"status": "OK", "message": "End of process."}
```

### Comparing `sftpoeb-0.1.1/sftpoeb.egg-info/PKG-INFO` & `sftpoeb-0.1.2/sftpoeb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.1.1
+Version: 0.1.2
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
@@ -59,7 +59,11 @@
 ------------------
 - Fixbug
 
 0.1.1 (14/06/2023)
 ------------------
 - Fixbug
 
+0.1.2 (15/06/2023)
+------------------
+- Fixbug
+
```

### Comparing `sftpoeb-0.1.1/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.1.2/sftpoeb.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 CHANGELOG.txt
 LICENSE.txt
 MANIFEST.in
 README.txt
 requirements.txt
 setup.py
+test.py
 sftpoeb/__init__.py
 sftpoeb.egg-info/PKG-INFO
 sftpoeb.egg-info/SOURCES.txt
 sftpoeb.egg-info/dependency_links.txt
 sftpoeb.egg-info/requires.txt
 sftpoeb.egg-info/top_level.txt
 sftpoeb/config/variable.py
 sftpoeb/mainclass/__init__.py
+sftpoeb/mainclass/c_recovery.py
 sftpoeb/mainclass/c_sftp.py
 sftpoeb/method/__init__.py
 sftpoeb/method/callservice.py
 sftpoeb/method/checkpath.py
 sftpoeb/method/debug.py
+sftpoeb/method/mail.py
 sftpoeb/sftpoeb.egg-info/SOURCES.txt
 sftpoeb/sftpoeb.egg-info/dependency_links.txt
 sftpoeb/sftpoeb.egg-info/requires.txt
 sftpoeb/sftpoeb.egg-info/top_level.txt
 sftpoeb/subclass/__init__.py
+sftpoeb/subclass/alert/__init__.py
+sftpoeb/subclass/alert/s_c_alert.py
 sftpoeb/subclass/file/__init__.py
 sftpoeb/subclass/file/s_c_file.py
 sftpoeb/subclass/file/s_c_file_transfer.py
 sftpoeb/subclass/input/__init__.py
 sftpoeb/subclass/input/s_c_input.py
 sftpoeb/subclass/output/__init__.py
 sftpoeb/subclass/output/s_c_output.py
```

