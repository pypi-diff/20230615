# Comparing `tmp/aishield-0.1.3.tar.gz` & `tmp/aishield-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aishield-0.1.3.tar", last modified: Wed Mar 29 14:03:19 2023, max compression
+gzip compressed data, was "aishield-0.1.4.tar", last modified: Thu Jun 15 13:54:43 2023, max compression
```

## Comparing `aishield-0.1.3.tar` & `aishield-0.1.4.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 14:03:19.071272 aishield-0.1.3/
--rw-rw-rw-   0        0        0     3443 2023-03-29 14:03:19.069276 aishield-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2770 2023-03-29 11:56:07.000000 aishield-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-29 14:03:18.987495 aishield-0.1.3/aishield/
--rw-rw-rw-   0        0        0     1780 2022-12-14 06:23:58.000000 aishield-0.1.3/aishield/__init__.py
--rw-rw-rw-   0        0        0    15155 2023-03-20 09:17:07.000000 aishield-0.1.3/aishield/aishield_api.py
--rw-rw-rw-   0        0        0     5070 2023-01-17 09:49:00.000000 aishield-0.1.3/aishield/configs.py
--rw-rw-rw-   0        0        0    12777 2023-03-29 12:12:00.000000 aishield-0.1.3/aishield/connection.py
--rw-rw-rw-   0        0        0     1460 2023-01-19 13:29:16.000000 aishield-0.1.3/aishield/constants.py
-drwxrwxrwx   0        0        0        0 2023-03-29 14:03:19.025397 aishield-0.1.3/aishield/image_classification/
--rw-rw-rw-   0        0        0        0 2022-11-25 15:26:32.000000 aishield-0.1.3/aishield/image_classification/__init__.py
--rw-rw-rw-   0        0        0     2917 2023-03-29 13:26:08.000000 aishield-0.1.3/aishield/image_classification/base_ic.py
--rw-rw-rw-   0        0        0     1305 2023-03-29 13:27:06.000000 aishield-0.1.3/aishield/image_classification/evasion.py
--rw-rw-rw-   0        0        0     1988 2023-03-29 13:38:09.000000 aishield-0.1.3/aishield/image_classification/extraction.py
--rw-rw-rw-   0        0        0      720 2023-03-29 13:36:39.000000 aishield-0.1.3/aishield/image_classification/poision.py
-drwxrwxrwx   0        0        0        0 2023-03-29 14:03:19.041353 aishield-0.1.3/aishield/tabular_classification/
--rw-rw-rw-   0        0        0        0 2022-11-25 15:26:32.000000 aishield-0.1.3/aishield/tabular_classification/__init__.py
--rw-rw-rw-   0        0        0     4344 2023-03-24 12:45:35.000000 aishield-0.1.3/aishield/tabular_classification/base_tc.py
--rw-rw-rw-   0        0        0      539 2023-03-24 12:45:52.000000 aishield-0.1.3/aishield/tabular_classification/evasion.py
--rw-rw-rw-   0        0        0     1195 2023-03-24 12:46:00.000000 aishield-0.1.3/aishield/tabular_classification/extraction.py
-drwxrwxrwx   0        0        0        0 2023-03-29 14:03:19.057311 aishield-0.1.3/aishield/utils/
--rw-rw-rw-   0        0        0        0 2022-10-17 19:21:54.000000 aishield-0.1.3/aishield/utils/__init__.py
--rw-rw-rw-   0        0        0      816 2022-10-25 15:02:47.000000 aishield-0.1.3/aishield/utils/exceptions.py
--rw-rw-rw-   0        0        0      559 2022-11-29 05:18:14.000000 aishield-0.1.3/aishield/utils/logger.py
--rw-rw-rw-   0        0        0     3318 2023-01-13 09:56:26.000000 aishield-0.1.3/aishield/utils/util.py
-drwxrwxrwx   0        0        0        0 2023-03-29 14:03:19.005447 aishield-0.1.3/aishield.egg-info/
--rw-rw-rw-   0        0        0     3443 2023-03-29 14:03:18.000000 aishield-0.1.3/aishield.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      837 2023-03-29 14:03:18.000000 aishield-0.1.3/aishield.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 14:03:18.000000 aishield-0.1.3/aishield.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-29 14:03:18.000000 aishield-0.1.3/aishield.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-03-29 14:03:18.000000 aishield-0.1.3/aishield.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      572 2022-11-18 10:08:05.000000 aishield-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-29 14:03:19.071272 aishield-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1296 2023-03-29 12:25:23.000000 aishield-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-29 14:03:19.066286 aishield-0.1.3/tests/
--rw-rw-rw-   0        0        0        0 2022-10-23 18:04:29.000000 aishield-0.1.3/tests/__init__.py
--rw-rw-rw-   0        0        0      931 2022-11-29 05:22:31.000000 aishield-0.1.3/tests/test_aishield_api.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:54:43.755033 aishield-0.1.4/
+-rw-rw-rw-   0        0        0     3541 2023-06-15 13:54:43.754056 aishield-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2866 2023-06-15 13:50:40.000000 aishield-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 13:54:43.555311 aishield-0.1.4/aishield/
+-rw-rw-rw-   0        0        0     1780 2022-12-14 06:23:58.000000 aishield-0.1.4/aishield/__init__.py
+-rw-rw-rw-   0        0        0    15410 2023-05-24 06:52:11.000000 aishield-0.1.4/aishield/aishield_api.py
+-rw-rw-rw-   0        0        0     5070 2023-01-17 09:49:00.000000 aishield-0.1.4/aishield/configs.py
+-rw-rw-rw-   0        0        0    12777 2023-03-29 12:12:00.000000 aishield-0.1.4/aishield/connection.py
+-rw-rw-rw-   0        0        0     1463 2023-05-24 12:22:21.000000 aishield-0.1.4/aishield/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:54:43.636320 aishield-0.1.4/aishield/image_classification/
+-rw-rw-rw-   0        0        0        0 2022-11-25 15:26:32.000000 aishield-0.1.4/aishield/image_classification/__init__.py
+-rw-rw-rw-   0        0        0     2917 2023-03-29 13:26:08.000000 aishield-0.1.4/aishield/image_classification/base_ic.py
+-rw-rw-rw-   0        0        0     1305 2023-03-29 13:27:06.000000 aishield-0.1.4/aishield/image_classification/evasion.py
+-rw-rw-rw-   0        0        0     1988 2023-03-29 13:38:09.000000 aishield-0.1.4/aishield/image_classification/extraction.py
+-rw-rw-rw-   0        0        0      720 2023-03-29 13:36:39.000000 aishield-0.1.4/aishield/image_classification/poision.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:54:43.670479 aishield-0.1.4/aishield/tabular_classification/
+-rw-rw-rw-   0        0        0        0 2022-11-25 15:26:32.000000 aishield-0.1.4/aishield/tabular_classification/__init__.py
+-rw-rw-rw-   0        0        0     4344 2023-03-24 12:45:35.000000 aishield-0.1.4/aishield/tabular_classification/base_tc.py
+-rw-rw-rw-   0        0        0      539 2023-03-24 12:45:52.000000 aishield-0.1.4/aishield/tabular_classification/evasion.py
+-rw-rw-rw-   0        0        0     1195 2023-03-24 12:46:00.000000 aishield-0.1.4/aishield/tabular_classification/extraction.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:54:43.698818 aishield-0.1.4/aishield/timeseries_forecasting/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:03:16.000000 aishield-0.1.4/aishield/timeseries_forecasting/__init__.py
+-rw-rw-rw-   0        0        0     2919 2023-05-26 09:44:19.000000 aishield-0.1.4/aishield/timeseries_forecasting/base_tsf.py
+-rw-rw-rw-   0        0        0     1198 2023-05-24 06:49:21.000000 aishield-0.1.4/aishield/timeseries_forecasting/extraction.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:54:43.733920 aishield-0.1.4/aishield/utils/
+-rw-rw-rw-   0        0        0        0 2022-10-17 19:21:54.000000 aishield-0.1.4/aishield/utils/__init__.py
+-rw-rw-rw-   0        0        0      816 2022-10-25 15:02:47.000000 aishield-0.1.4/aishield/utils/exceptions.py
+-rw-rw-rw-   0        0        0      559 2022-11-29 05:18:14.000000 aishield-0.1.4/aishield/utils/logger.py
+-rw-rw-rw-   0        0        0     3318 2023-01-13 09:56:26.000000 aishield-0.1.4/aishield/utils/util.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:54:43.572880 aishield-0.1.4/aishield.egg-info/
+-rw-rw-rw-   0        0        0     3541 2023-06-15 13:54:43.000000 aishield-0.1.4/aishield.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2023-06-15 13:54:43.000000 aishield-0.1.4/aishield.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 13:54:43.000000 aishield-0.1.4/aishield.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 13:54:43.000000 aishield-0.1.4/aishield.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-15 13:54:43.000000 aishield-0.1.4/aishield.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      572 2022-11-18 10:08:05.000000 aishield-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-15 13:54:43.756009 aishield-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1296 2023-05-26 10:54:48.000000 aishield-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:54:43.750151 aishield-0.1.4/tests/
+-rw-rw-rw-   0        0        0        0 2022-10-23 18:04:29.000000 aishield-0.1.4/tests/__init__.py
+-rw-rw-rw-   0        0        0      931 2022-11-29 05:22:31.000000 aishield-0.1.4/tests/test_aishield_api.py
```

### Comparing `aishield-0.1.3/PKG-INFO` & `aishield-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aishield
-Version: 0.1.3
+Version: 0.1.4
 Summary: AIShield provides the Python convenience package to allow users to seamlessly integrate AIShield Vulnerability Assessment and Defense capabilities into their AI development workflows.
 Home-page: https://www.boschaishield.com/
 Author: Contact AIShield
 Author-email: aishield.contact@bosch.com
 License: Apache License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -50,14 +50,16 @@
    
 ## More about AIShield
 
 - Website:  https://www.boschaishield.com/
 - Email:   <AIShield.Contact@bosch.com>
 
 ## Version History
+### 0.1.4
+- Added vulnerability analysis for time series forecasting: model extraction attack
 
 ### 0.1.3
 - Updated to be compatible with latest AIShield API version
 - Added vulnerability analysis for tabular classification: model evasion attack
 
 ### 0.1.2
 - Added vulnerability analysis for image classification: model evasion & model poisoning attack
```

### Comparing `aishield-0.1.3/README.md` & `aishield-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
    
 ## More about AIShield
 
 - Website:  https://www.boschaishield.com/
 - Email:   <AIShield.Contact@bosch.com>
 
 ## Version History
+### 0.1.4
+- Added vulnerability analysis for time series forecasting: model extraction attack
 
 ### 0.1.3
 - Updated to be compatible with latest AIShield API version
 - Added vulnerability analysis for tabular classification: model evasion attack
 
 ### 0.1.2
 - Added vulnerability analysis for image classification: model evasion & model poisoning attack
```

### Comparing `aishield-0.1.3/aishield/__init__.py` & `aishield-0.1.4/aishield/__init__.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.3/aishield/aishield_api.py` & `aishield-0.1.4/aishield/aishield_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     evasion as ic_evasion,
     poision as ic_poison
 )
 from aishield.tabular_classification import (
     extraction as tc_extraction,
     evasion as tc_evasion
 )
+from aishield.timeseries_forecasting import extraction as tsf_extraction
 from aishield.utils.util import (
     uri_validator,
     get_all_keys_by_val
 )
 from aishield.utils.util import delete_keys_from_dict
 
 
@@ -72,15 +73,18 @@
             if analysis_type == Attack.EXTRACTION:
                 vul_config_obj = tc_extraction.VulnConfig(defense_generate)
             elif analysis_type == Attack.EVASION:
                 vul_config_obj = tc_evasion.VulnConfig(defense_generate)
             else:
                 raise NotImplementedError('Feature coming soon')
         elif task_type == Task.TIMESERIES_FORECAST:
-            raise NotImplementedError('Feature coming soon')
+            if analysis_type == Attack.EXTRACTION:
+                vul_config_obj = tsf_extraction.VulnConfig(defense_generate)
+            else:
+                raise NotImplementedError('Feature coming soon')
         elif task_type == Task.NLP:
             raise NotImplementedError('Feature coming soon')
         elif task_type == Task.IMAGE_SEGMENTATION:
             raise NotImplementedError('Feature coming soon')
         else:
             raise NotImplementedError('New task-pairs would be added soon')
         return vul_config_obj
@@ -149,15 +153,15 @@
         self.job_details.model_upload_uri = response_json_urls[UploadURIKeys.MODEL_UPLOAD_URI_KEY.value]
         if task_type == Task.IMAGE_CLASSIFICATION:
             self.job_details.label_upload_uri = response_json_urls[UploadURIKeys.LABEL_UPLOAD_URI_KEY.value]
             if analysis_type == Attack.POISONING:
                 clean_model_upload_uris = [response_json_urls[UploadURIKeys.CLEAN_MODEL1_UPLOAD_URI_KEY.value],
                                            response_json_urls[UploadURIKeys.CLEAN_MODEL2_UPLOAD_URI_KEY.value]]
                 self.job_details.clean_model_upload_uris = clean_model_upload_uris
-        elif task_type == Task.TABULAR_CLASSIFICATION:
+        elif task_type in [Task.TABULAR_CLASSIFICATION, Task.TIMESERIES_FORECAST]:
             self.job_details.minmax_upload_uri = response_json_urls[UploadURIKeys.MINMAX_UPLOAD_URI_KEY.value]
         else:
             raise NotImplementedError('New task-pairs would be added soon')
         return status, self.job_details
 
     def upload_input_artifacts(self, job_details: JobDetails, data_path: str = None, label_path: str = None,
                                minmax_path: str = None, model_path: str = None, clean_model_paths: list = None) -> list:
```

### Comparing `aishield-0.1.3/aishield/configs.py` & `aishield-0.1.4/aishield/configs.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.3/aishield/connection.py` & `aishield-0.1.4/aishield/connection.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.3/aishield/constants.py` & `aishield-0.1.4/aishield/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     INFERENCE = 'inference'
     POISONING = 'poisoning'
 
 
 class Task(ExtendedEnum):
     IMAGE_CLASSIFICATION = 'image_classification'
     IMAGE_SEGMENTATION = 'image_segmentation'
-    TIMESERIES_FORECAST = 'timeseries_forecast'
+    TIMESERIES_FORECAST = 'timeseries_forecasting'
     NLP = 'nlp'
     TABULAR_CLASSIFICATION = 'tabular_classification'
 
 
 class ReportType(ExtendedEnum):
     VULNERABILITY = 'vulnerability'
     DEFENSE = 'defense'
```

### Comparing `aishield-0.1.3/aishield/image_classification/base_ic.py` & `aishield-0.1.4/aishield/image_classification/base_ic.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.3/aishield/image_classification/evasion.py` & `aishield-0.1.4/aishield/image_classification/evasion.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.3/aishield/image_classification/extraction.py` & `aishield-0.1.4/aishield/image_classification/extraction.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.3/aishield/image_classification/poision.py` & `aishield-0.1.4/aishield/image_classification/poision.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.3/aishield/tabular_classification/base_tc.py` & `aishield-0.1.4/aishield/tabular_classification/base_tc.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.3/aishield/tabular_classification/evasion.py` & `aishield-0.1.4/aishield/tabular_classification/evasion.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.3/aishield/tabular_classification/extraction.py` & `aishield-0.1.4/aishield/tabular_classification/extraction.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.3/aishield/utils/exceptions.py` & `aishield-0.1.4/aishield/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.3/aishield/utils/logger.py` & `aishield-0.1.4/aishield/utils/logger.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.3/aishield/utils/util.py` & `aishield-0.1.4/aishield/utils/util.py`

 * *Files identical despite different names*

### Comparing `aishield-0.1.3/aishield.egg-info/PKG-INFO` & `aishield-0.1.4/aishield.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aishield
-Version: 0.1.3
+Version: 0.1.4
 Summary: AIShield provides the Python convenience package to allow users to seamlessly integrate AIShield Vulnerability Assessment and Defense capabilities into their AI development workflows.
 Home-page: https://www.boschaishield.com/
 Author: Contact AIShield
 Author-email: aishield.contact@bosch.com
 License: Apache License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -50,14 +50,16 @@
    
 ## More about AIShield
 
 - Website:  https://www.boschaishield.com/
 - Email:   <AIShield.Contact@bosch.com>
 
 ## Version History
+### 0.1.4
+- Added vulnerability analysis for time series forecasting: model extraction attack
 
 ### 0.1.3
 - Updated to be compatible with latest AIShield API version
 - Added vulnerability analysis for tabular classification: model evasion attack
 
 ### 0.1.2
 - Added vulnerability analysis for image classification: model evasion & model poisoning attack
```

### Comparing `aishield-0.1.3/aishield.egg-info/SOURCES.txt` & `aishield-0.1.4/aishield.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,13 +16,16 @@
 aishield/image_classification/evasion.py
 aishield/image_classification/extraction.py
 aishield/image_classification/poision.py
 aishield/tabular_classification/__init__.py
 aishield/tabular_classification/base_tc.py
 aishield/tabular_classification/evasion.py
 aishield/tabular_classification/extraction.py
+aishield/timeseries_forecasting/__init__.py
+aishield/timeseries_forecasting/base_tsf.py
+aishield/timeseries_forecasting/extraction.py
 aishield/utils/__init__.py
 aishield/utils/exceptions.py
 aishield/utils/logger.py
 aishield/utils/util.py
 tests/__init__.py
 tests/test_aishield_api.py
```

### Comparing `aishield-0.1.3/pyproject.toml` & `aishield-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aishield-0.1.3/setup.py` & `aishield-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="aishield",
-    version="0.1.3",
+    version="0.1.4",
     description="AIShield provides the Python convenience package to allow users to seamlessly integrate AIShield Vulnerability Assessment and Defense capabilities into their AI development workflows.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://www.boschaishield.com/',
     author="Contact AIShield",
     author_email="aishield.contact@bosch.com",
     license="Apache License",
```

### Comparing `aishield-0.1.3/tests/test_aishield_api.py` & `aishield-0.1.4/tests/test_aishield_api.py`

 * *Files identical despite different names*

