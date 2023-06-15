# Comparing `tmp/login_gmail_selenium-1.1.8.tar.gz` & `tmp/login_gmail_selenium-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\login_gmail_selenium-1.1.8.tar", last modified: Wed Jun 14 09:45:19 2023, max compression
+gzip compressed data, was "dist\login_gmail_selenium-1.1.9.tar", last modified: Thu Jun 15 03:51:26 2023, max compression
```

## Comparing `login_gmail_selenium-1.1.8.tar` & `login_gmail_selenium-1.1.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 09:45:19.518118 login_gmail_selenium-1.1.8/
--rw-rw-rw-   0        0        0     1105 2023-01-10 09:15:32.000000 login_gmail_selenium-1.1.8/LICENSE
--rw-rw-rw-   0        0        0     2380 2023-06-14 09:45:19.517122 login_gmail_selenium-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1870 2023-03-07 08:43:52.000000 login_gmail_selenium-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 09:45:19.455288 login_gmail_selenium-1.1.8/login_gmail_selenium/
--rw-rw-rw-   0        0        0       42 2023-01-10 09:15:32.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:45:19.481217 login_gmail_selenium-1.1.8/login_gmail_selenium/common/
--rw-rw-rw-   0        0        0       24 2023-01-10 09:15:32.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/common/__init__.py
--rw-rw-rw-   0        0        0     1362 2023-06-14 09:30:06.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/common/constant.py
--rw-rw-rw-   0        0        0      628 2023-02-27 08:57:32.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/common/log.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:45:19.509143 login_gmail_selenium-1.1.8/login_gmail_selenium/extension/
--rw-rw-rw-   0        0        0    38852 2022-12-16 03:14:21.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/extension/always_active.zip
--rw-rw-rw-   0        0        0     5260 2022-12-16 03:14:21.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/extension/fingerprint_defender.zip
--rw-rw-rw-   0        0        0   120399 2022-12-16 03:14:21.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/extension/spoof_timezone.zip
--rw-rw-rw-   0        0        0  5601639 2023-03-14 08:09:16.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/extension/veepn.zip
--rw-rw-rw-   0        0        0    45183 2022-12-16 03:14:21.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/extension/webrtc_control.zip
-drwxrwxrwx   0        0        0        0 2023-06-14 09:45:19.514130 login_gmail_selenium-1.1.8/login_gmail_selenium/util/
--rw-rw-rw-   0        0        0       45 2023-01-10 09:15:32.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/util/__init__.py
--rw-rw-rw-   0        0        0      706 2023-03-24 10:39:03.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/util/driver.py
--rw-rw-rw-   0        0        0     4719 2023-03-24 08:28:57.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/util/helper.py
--rw-rw-rw-   0        0        0    17201 2023-06-14 09:43:09.000000 login_gmail_selenium-1.1.8/login_gmail_selenium/util/profile.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:45:19.477227 login_gmail_selenium-1.1.8/login_gmail_selenium.egg-info/
--rw-rw-rw-   0        0        0     2380 2023-06-14 09:45:19.000000 login_gmail_selenium-1.1.8/login_gmail_selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-06-14 09:45:19.000000 login_gmail_selenium-1.1.8/login_gmail_selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 09:45:19.000000 login_gmail_selenium-1.1.8/login_gmail_selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-06-14 09:45:19.000000 login_gmail_selenium-1.1.8/login_gmail_selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-14 09:45:19.000000 login_gmail_selenium-1.1.8/login_gmail_selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 09:45:19.518118 login_gmail_selenium-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      909 2023-06-14 09:45:15.000000 login_gmail_selenium-1.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:45:19.515130 login_gmail_selenium-1.1.8/test/
--rw-rw-rw-   0        0        0     1230 2023-03-28 10:06:33.000000 login_gmail_selenium-1.1.8/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-15 03:51:26.250870 login_gmail_selenium-1.1.9/
+-rw-rw-rw-   0        0        0     1105 2023-01-10 09:15:32.000000 login_gmail_selenium-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0     2380 2023-06-15 03:51:26.249872 login_gmail_selenium-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1870 2023-03-07 08:43:52.000000 login_gmail_selenium-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 03:51:25.943691 login_gmail_selenium-1.1.9/login_gmail_selenium/
+-rw-rw-rw-   0        0        0       42 2023-01-10 09:15:32.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 03:51:26.057386 login_gmail_selenium-1.1.9/login_gmail_selenium/common/
+-rw-rw-rw-   0        0        0       24 2023-01-10 09:15:32.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/common/__init__.py
+-rw-rw-rw-   0        0        0     1362 2023-06-14 09:30:06.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/common/constant.py
+-rw-rw-rw-   0        0        0      628 2023-02-27 08:57:32.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/common/log.py
+drwxrwxrwx   0        0        0        0 2023-06-15 03:51:26.165100 login_gmail_selenium-1.1.9/login_gmail_selenium/extension/
+-rw-rw-rw-   0        0        0    38852 2022-12-16 03:14:21.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/extension/always_active.zip
+-rw-rw-rw-   0        0        0     5260 2022-12-16 03:14:21.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/extension/fingerprint_defender.zip
+-rw-rw-rw-   0        0        0   120399 2022-12-16 03:14:21.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/extension/spoof_timezone.zip
+-rw-rw-rw-   0        0        0  5601639 2023-03-14 08:09:16.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/extension/veepn.zip
+-rw-rw-rw-   0        0        0    45183 2022-12-16 03:14:21.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/extension/webrtc_control.zip
+drwxrwxrwx   0        0        0        0 2023-06-15 03:51:26.227931 login_gmail_selenium-1.1.9/login_gmail_selenium/util/
+-rw-rw-rw-   0        0        0       45 2023-01-10 09:15:32.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/util/__init__.py
+-rw-rw-rw-   0        0        0      706 2023-03-24 10:39:03.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/util/driver.py
+-rw-rw-rw-   0        0        0     4719 2023-03-24 08:28:57.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/util/helper.py
+-rw-rw-rw-   0        0        0    17155 2023-06-15 01:30:52.000000 login_gmail_selenium-1.1.9/login_gmail_selenium/util/profile.py
+drwxrwxrwx   0        0        0        0 2023-06-15 03:51:26.016497 login_gmail_selenium-1.1.9/login_gmail_selenium.egg-info/
+-rw-rw-rw-   0        0        0     2380 2023-06-15 03:51:25.000000 login_gmail_selenium-1.1.9/login_gmail_selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2023-06-15 03:51:25.000000 login_gmail_selenium-1.1.9/login_gmail_selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 03:51:25.000000 login_gmail_selenium-1.1.9/login_gmail_selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-06-15 03:51:25.000000 login_gmail_selenium-1.1.9/login_gmail_selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-15 03:51:25.000000 login_gmail_selenium-1.1.9/login_gmail_selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 03:51:26.250870 login_gmail_selenium-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      909 2023-06-15 03:51:23.000000 login_gmail_selenium-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 03:51:26.247879 login_gmail_selenium-1.1.9/test/
+-rw-rw-rw-   0        0        0     1230 2023-03-28 10:06:33.000000 login_gmail_selenium-1.1.9/test/test.py
```

### Comparing `login_gmail_selenium-1.1.8/LICENSE` & `login_gmail_selenium-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.8/PKG-INFO` & `login_gmail_selenium-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: login_gmail_selenium
-Version: 1.1.8
+Version: 1.1.9
 Summary: A python package for login google by selenium
 Home-page: https://github.com/ngminhhoang1412/LoginGmailSelenium
 Author: Minh Hoang
 Author-email: ngminhhoang1412@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `login_gmail_selenium-1.1.8/README.md` & `login_gmail_selenium-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.8/login_gmail_selenium/common/constant.py` & `login_gmail_selenium-1.1.9/login_gmail_selenium/common/constant.py`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.8/login_gmail_selenium/common/log.py` & `login_gmail_selenium-1.1.9/login_gmail_selenium/common/log.py`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.8/login_gmail_selenium/extension/always_active.zip` & `login_gmail_selenium-1.1.9/login_gmail_selenium/extension/always_active.zip`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.8/login_gmail_selenium/extension/fingerprint_defender.zip` & `login_gmail_selenium-1.1.9/login_gmail_selenium/extension/fingerprint_defender.zip`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.8/login_gmail_selenium/extension/spoof_timezone.zip` & `login_gmail_selenium-1.1.9/login_gmail_selenium/extension/spoof_timezone.zip`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.8/login_gmail_selenium/extension/veepn.zip` & `login_gmail_selenium-1.1.9/login_gmail_selenium/extension/veepn.zip`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.8/login_gmail_selenium/extension/webrtc_control.zip` & `login_gmail_selenium-1.1.9/login_gmail_selenium/extension/webrtc_control.zip`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.8/login_gmail_selenium/util/driver.py` & `login_gmail_selenium-1.1.9/login_gmail_selenium/util/driver.py`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.8/login_gmail_selenium/util/helper.py` & `login_gmail_selenium-1.1.9/login_gmail_selenium/util/helper.py`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.8/login_gmail_selenium/util/profile.py` & `login_gmail_selenium-1.1.9/login_gmail_selenium/util/profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,14 @@
         username_xpath = '//*[@id="identifierId"]'
         login_text_retrieve_script = 'return document.querySelector("input[type=\'email\']");'
         try:
             # First time login on device, type username
             type_text(driver=self.driver, text=self.email, xpath=username_xpath, loading=True,
                       script=login_text_retrieve_script, paste_text=100)
         except NoSuchElementException:
-            # TODO: this site can't be reach
             raise
         except (Exception, ValueError):
             # Profile already has at least 1 username, choose profile with correct email
             if "signinchooser" in driver.current_url:
                 desired_profile = driver.find_element(By.XPATH, f"//div[contains(text(), '{self.email}')]")
                 if desired_profile:
                     desired_profile.click()
```

### Comparing `login_gmail_selenium-1.1.8/login_gmail_selenium.egg-info/PKG-INFO` & `login_gmail_selenium-1.1.9/login_gmail_selenium.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: login-gmail-selenium
-Version: 1.1.8
+Version: 1.1.9
 Summary: A python package for login google by selenium
 Home-page: https://github.com/ngminhhoang1412/LoginGmailSelenium
 Author: Minh Hoang
 Author-email: ngminhhoang1412@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `login_gmail_selenium-1.1.8/login_gmail_selenium.egg-info/SOURCES.txt` & `login_gmail_selenium-1.1.9/login_gmail_selenium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `login_gmail_selenium-1.1.8/setup.py` & `login_gmail_selenium-1.1.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt', 'r', encoding='utf-16') as f:
     requirements = [line.rstrip('\n') for line in f]
 
 setuptools.setup(
     name="login_gmail_selenium",
-    version="1.1.8",
+    version="1.1.9",
     author="Minh Hoang",
     author_email="ngminhhoang1412@gmail.com",
     description="A python package for login google by selenium",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ngminhhoang1412/LoginGmailSelenium",
     include_package_data=True,
```

### Comparing `login_gmail_selenium-1.1.8/test/test.py` & `login_gmail_selenium-1.1.9/test/test.py`

 * *Files identical despite different names*

