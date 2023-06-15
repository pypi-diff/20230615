# Comparing `tmp/whatsapp-chatbot-python-0.2.2.tar.gz` & `tmp/whatsapp-chatbot-python-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-chatbot-python-0.2.2.tar", last modified: Thu Jun  8 08:55:13 2023, max compression
+gzip compressed data, was "whatsapp-chatbot-python-0.2.3.tar", last modified: Thu Jun 15 04:46:38 2023, max compression
```

## Comparing `whatsapp-chatbot-python-0.2.2.tar` & `whatsapp-chatbot-python-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 08:55:13.025522 whatsapp-chatbot-python-0.2.2/
--rw-rw-rw-   0        0        0    18829 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     9060 2023-06-08 08:55:13.025522 whatsapp-chatbot-python-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     8035 2023-06-08 08:50:01.000000 whatsapp-chatbot-python-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-08 08:55:13.025522 whatsapp-chatbot-python-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1405 2023-06-08 08:51:43.000000 whatsapp-chatbot-python-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:55:13.012488 whatsapp-chatbot-python-0.2.2/tests/
--rw-rw-rw-   0        0        0     1224 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.2/tests/test_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:55:13.016498 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/
--rw-rw-rw-   0        0        0      184 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/__init__.py
--rw-rw-rw-   0        0        0     1020 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/bot.py
--rw-rw-rw-   0        0        0     3569 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/filters.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:55:13.023517 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/manager/
--rw-rw-rw-   0        0        0        0 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/manager/__init__.py
--rw-rw-rw-   0        0        0     3277 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/manager/handler.py
--rw-rw-rw-   0        0        0     1821 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/manager/observer.py
--rw-rw-rw-   0        0        0     1144 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/manager/router.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:55:13.020509 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python.egg-info/
--rw-rw-rw-   0        0        0     9060 2023-06-08 08:55:12.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2023-06-08 08:55:13.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 08:55:12.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-08 08:55:12.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-08 08:55:12.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 04:46:38.808624 whatsapp-chatbot-python-0.2.3/
+-rw-rw-rw-   0        0        0    18829 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     9060 2023-06-15 04:46:38.807622 whatsapp-chatbot-python-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8035 2023-06-08 08:50:01.000000 whatsapp-chatbot-python-0.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 04:46:38.808624 whatsapp-chatbot-python-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1405 2023-06-15 04:43:42.000000 whatsapp-chatbot-python-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 04:46:38.795589 whatsapp-chatbot-python-0.2.3/tests/
+-rw-rw-rw-   0        0        0     1224 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.3/tests/test_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-15 04:46:38.798597 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/
+-rw-rw-rw-   0        0        0      184 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/__init__.py
+-rw-rw-rw-   0        0        0     1020 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/bot.py
+-rw-rw-rw-   0        0        0     3569 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/filters.py
+drwxrwxrwx   0        0        0        0 2023-06-15 04:46:38.806618 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/manager/
+-rw-rw-rw-   0        0        0        0 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/manager/__init__.py
+-rw-rw-rw-   0        0        0     3277 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/manager/handler.py
+-rw-rw-rw-   0        0        0     1821 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/manager/observer.py
+-rw-rw-rw-   0        0        0     1144 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/manager/router.py
+drwxrwxrwx   0        0        0        0 2023-06-15 04:46:38.802609 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python.egg-info/
+-rw-rw-rw-   0        0        0     9060 2023-06-15 04:46:38.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2023-06-15 04:46:38.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 04:46:38.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-15 04:46:38.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-15 04:46:38.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python.egg-info/top_level.txt
```

### Comparing `whatsapp-chatbot-python-0.2.2/LICENSE` & `whatsapp-chatbot-python-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.2/PKG-INFO` & `whatsapp-chatbot-python-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chatbot-python
-Version: 0.2.2
+Version: 0.2.3
 Summary: This library helps you easily create a Python chatbot with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-chatbot-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `whatsapp-chatbot-python-0.2.2/README.md` & `whatsapp-chatbot-python-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.2/setup.py` & `whatsapp-chatbot-python-0.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="whatsapp-chatbot-python",
-    version="0.2.2",
+    version="0.2.3",
     description=(
         "This library helps you easily create"
         " a Python chatbot with WhatsApp API."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="GREEN API",
@@ -29,10 +29,10 @@
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Application Frameworks"
     ],
     license=(
         "Creative Commons Attribution-NoDerivatives 4.0 International"
         " (CC BY-ND 4.0)"
     ),
-    install_requires=["whatsapp-api-client-python==0.0.36"],
+    install_requires=["whatsapp-api-client-python==0.0.37"],
     python_requires=">=3.7"
 )
```

### Comparing `whatsapp-chatbot-python-0.2.2/tests/test_manager.py` & `whatsapp-chatbot-python-0.2.3/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/bot.py` & `whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/bot.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/filters.py` & `whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/filters.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/manager/handler.py` & `whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/manager/handler.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/manager/observer.py` & `whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/manager/observer.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/manager/router.py` & `whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/manager/router.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python.egg-info/PKG-INFO` & `whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chatbot-python
-Version: 0.2.2
+Version: 0.2.3
 Summary: This library helps you easily create a Python chatbot with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-chatbot-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python.egg-info/SOURCES.txt` & `whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

