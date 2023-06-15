# Comparing `tmp/pacsman-0.1.7.tar.gz` & `tmp/pacsman-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pacsman-0.1.7.tar", last modified: Fri Jan 27 18:26:22 2023, max compression
+gzip compressed data, was "pacsman-0.1.8.tar", last modified: Thu Jun 15 15:00:13 2023, max compression
```

## Comparing `pacsman-0.1.7.tar` & `pacsman-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 18:26:22.788188 pacsman-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-01-27 18:26:10.000000 pacsman-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-01-27 18:26:22.788188 pacsman-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-01-27 18:26:10.000000 pacsman-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 18:26:22.788188 pacsman-0.1.7/pacsman/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-01-27 18:26:10.000000 pacsman-0.1.7/pacsman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-01-27 18:26:10.000000 pacsman-0.1.7/pacsman/base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-01-27 18:26:10.000000 pacsman-0.1.7/pacsman/base_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    25690 2023-01-27 18:26:10.000000 pacsman-0.1.7/pacsman/dcmtk_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-01-27 18:26:10.000000 pacsman-0.1.7/pacsman/dcmtk_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-01-27 18:26:10.000000 pacsman-0.1.7/pacsman/filesystem_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-01-27 18:26:10.000000 pacsman-0.1.7/pacsman/filesystem_dev_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-01-27 18:26:10.000000 pacsman-0.1.7/pacsman/integration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22544 2023-01-27 18:26:10.000000 pacsman-0.1.7/pacsman/pynetdicom_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-01-27 18:26:10.000000 pacsman-0.1.7/pacsman/upload_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-01-27 18:26:10.000000 pacsman-0.1.7/pacsman/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-01-27 18:26:10.000000 pacsman-0.1.7/pacsman/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 18:26:22.788188 pacsman-0.1.7/pacsman.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-01-27 18:26:22.000000 pacsman-0.1.7/pacsman.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-01-27 18:26:22.000000 pacsman-0.1.7/pacsman.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-27 18:26:22.000000 pacsman-0.1.7/pacsman.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-27 18:26:22.000000 pacsman-0.1.7/pacsman.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-27 18:26:22.000000 pacsman-0.1.7/pacsman.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 18:26:22.788188 pacsman-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-01-27 18:26:10.000000 pacsman-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:00:13.735091 pacsman-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-15 15:00:05.000000 pacsman-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-15 15:00:13.735091 pacsman-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-15 15:00:05.000000 pacsman-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:00:13.735091 pacsman-0.1.8/pacsman/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-15 15:00:05.000000 pacsman-0.1.8/pacsman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-15 15:00:05.000000 pacsman-0.1.8/pacsman/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-06-15 15:00:05.000000 pacsman-0.1.8/pacsman/base_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25794 2023-06-15 15:00:05.000000 pacsman-0.1.8/pacsman/dcmtk_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-15 15:00:05.000000 pacsman-0.1.8/pacsman/dcmtk_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-15 15:00:05.000000 pacsman-0.1.8/pacsman/filesystem_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-06-15 15:00:05.000000 pacsman-0.1.8/pacsman/filesystem_dev_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-06-15 15:00:05.000000 pacsman-0.1.8/pacsman/integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22544 2023-06-15 15:00:05.000000 pacsman-0.1.8/pacsman/pynetdicom_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-15 15:00:05.000000 pacsman-0.1.8/pacsman/upload_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-15 15:00:05.000000 pacsman-0.1.8/pacsman/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-15 15:00:05.000000 pacsman-0.1.8/pacsman/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:00:13.735091 pacsman-0.1.8/pacsman.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-15 15:00:13.000000 pacsman-0.1.8/pacsman.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-15 15:00:13.000000 pacsman-0.1.8/pacsman.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 15:00:13.000000 pacsman-0.1.8/pacsman.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 15:00:13.000000 pacsman-0.1.8/pacsman.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 15:00:13.000000 pacsman-0.1.8/pacsman.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 15:00:13.735091 pacsman-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-15 15:00:05.000000 pacsman-0.1.8/setup.py
```

### Comparing `pacsman-0.1.7/LICENSE` & `pacsman-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pacsman-0.1.7/PKG-INFO` & `pacsman-0.1.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pacsman
-Version: 0.1.7
+Version: 0.1.8
 Summary: pacsman: Picture Archiving and Communication System Manager And Numpifier
 Home-page: https://github.com/innolitics/pacsman
 Author: Innolitics, LLC
 Author-email: info@innolitics.com
 License: MIT
 Keywords: scientific image
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pacsman-0.1.7/README.md` & `pacsman-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pacsman-0.1.7/pacsman/base_client.py` & `pacsman-0.1.8/pacsman/base_client.py`

 * *Files identical despite different names*

### Comparing `pacsman-0.1.7/pacsman/base_client_test.py` & `pacsman-0.1.8/pacsman/base_client_test.py`

 * *Files identical despite different names*

### Comparing `pacsman-0.1.7/pacsman/dcmtk_client.py` & `pacsman-0.1.8/pacsman/dcmtk_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         remote_ae,
         pacs_url,
         pacs_port,
         dicom_dir,
         dicom_tmp_dir=None,
         dcmtk_profile: str = "AllDICOM",
         timeout=20,
+        listener_port=str(11113),
         storescp_extra_args=None,
         movescu_extra_args=None,
         findscu_extra_args=None,
         retry_timeouts_with_backoff=False,
         *args, **kwargs,
     ):
         """
@@ -78,14 +79,15 @@
             needs to be registered with the remote PACS in order for C-MOVE to work
         :param pacs_url: Remote PACS URL
         :param pacs_port: Remote PACS port (usually 11112)
         :param dicom_dir: Root dir for storage of *.dcm files.
         :param dicom_tmp_dir: Root dir that stores temporary *.dcm files.
         :param dcmtk_profile: Profile name from storescp.cfg to use
         :param timeout: Connection and DICOM timeout in seconds
+        :param listener_port: Port to run the storescp listener on
         :param storescp_extra_args: Optional array of extra arguments to supply to the `storescp` invocation
         :param findscu_extra_args: Optional array of extra arguments to supply to the `findscu` invocation
         :param movescu_extra_args: Optional array of extra arguments to supply to the `movescu` invocation
         :param retry_timeouts_with_backoff: If true, will retry failures due to timeout, with a longer timeout period.
             default=False
 
         Note: the `dcmtk_profile` variable refers to the profile name defined
@@ -112,15 +114,15 @@
         self.client_ae = client_ae
         self.remote_ae = remote_ae
         self.pacs_url = pacs_url
         self.pacs_port = str(pacs_port)
         self.dicom_dir = dicom_dir
         self.dicom_tmp_dir = dicom_tmp_dir if dicom_tmp_dir else os.path.join(self.dicom_dir, 'tmp')
         self.timeout = timeout
-        self.listener_port = str(11113)
+        self.listener_port = listener_port
         self.storescp_extra_args = storescp_extra_args or []
         self.findscu_extra_args = findscu_extra_args or []
         self.movescu_extra_args = movescu_extra_args or []
         self.retry_timeouts_with_backoff = retry_timeouts_with_backoff
         self.dcmtk_profile = dcmtk_profile
         if logger.getEffectiveLevel() <= logging.DEBUG:
             self.logger_args = ['-v', '-d']
```

### Comparing `pacsman-0.1.7/pacsman/dcmtk_client_test.py` & `pacsman-0.1.8/pacsman/dcmtk_client_test.py`

 * *Files identical despite different names*

### Comparing `pacsman-0.1.7/pacsman/filesystem_client_test.py` & `pacsman-0.1.8/pacsman/filesystem_client_test.py`

 * *Files identical despite different names*

### Comparing `pacsman-0.1.7/pacsman/filesystem_dev_client.py` & `pacsman-0.1.8/pacsman/filesystem_dev_client.py`

 * *Files identical despite different names*

### Comparing `pacsman-0.1.7/pacsman/integration_test.py` & `pacsman-0.1.8/pacsman/integration_test.py`

 * *Files identical despite different names*

### Comparing `pacsman-0.1.7/pacsman/pynetdicom_client.py` & `pacsman-0.1.8/pacsman/pynetdicom_client.py`

 * *Files identical despite different names*

### Comparing `pacsman-0.1.7/pacsman/upload_test.py` & `pacsman-0.1.8/pacsman/upload_test.py`

 * *Files identical despite different names*

### Comparing `pacsman-0.1.7/pacsman/utils.py` & `pacsman-0.1.8/pacsman/utils.py`

 * *Files identical despite different names*

### Comparing `pacsman-0.1.7/pacsman/utils_test.py` & `pacsman-0.1.8/pacsman/utils_test.py`

 * *Files identical despite different names*

### Comparing `pacsman-0.1.7/pacsman.egg-info/PKG-INFO` & `pacsman-0.1.8/pacsman.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pacsman
-Version: 0.1.7
+Version: 0.1.8
 Summary: pacsman: Picture Archiving and Communication System Manager And Numpifier
 Home-page: https://github.com/innolitics/pacsman
 Author: Innolitics, LLC
 Author-email: info@innolitics.com
 License: MIT
 Keywords: scientific image
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pacsman-0.1.7/setup.py` & `pacsman-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 here = path.abspath(path.dirname(__file__))
 
 description = 'pacsman: Picture Archiving and Communication System Manager And Numpifier'
 
 setup(
     name='pacsman',
-    version='0.1.7',
+    version='0.1.8',
     description=description,
     long_description=description,
     url='https://github.com/innolitics/pacsman',
     author='Innolitics, LLC',
     author_email='info@innolitics.com',
     license='MIT',
     classifiers=[
```

