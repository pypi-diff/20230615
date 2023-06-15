# Comparing `tmp/selenium-simplified-0.6.tar.gz` & `tmp/selenium-simplified-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-simplified-0.6.tar", last modified: Tue Jun 13 17:19:17 2023, max compression
+gzip compressed data, was "selenium-simplified-0.7.tar", last modified: Thu Jun 15 16:46:17 2023, max compression
```

## Comparing `selenium-simplified-0.6.tar` & `selenium-simplified-0.7.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 17:19:17.604597 selenium-simplified-0.6/
--rw-rw-rw-   0        0        0     4264 2023-06-13 17:19:17.603629 selenium-simplified-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3782 2023-06-13 17:18:33.000000 selenium-simplified-0.6/README.md
--rw-rw-rw-   0        0        0       97 2023-06-12 17:04:36.000000 selenium-simplified-0.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-13 17:19:17.597672 selenium-simplified-0.6/selenium_simplified.egg-info/
--rw-rw-rw-   0        0        0     4264 2023-06-13 17:19:17.000000 selenium-simplified-0.6/selenium_simplified.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-06-13 17:19:17.000000 selenium-simplified-0.6/selenium_simplified.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 17:19:17.000000 selenium-simplified-0.6/selenium_simplified.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-13 17:19:17.000000 selenium-simplified-0.6/selenium_simplified.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-13 17:19:17.000000 selenium-simplified-0.6/selenium_simplified.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 17:19:17.604597 selenium-simplified-0.6/setup.cfg
--rw-rw-rw-   0        0        0      787 2023-06-13 17:18:53.000000 selenium-simplified-0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:19:17.602678 selenium-simplified-0.6/simplified/
--rw-rw-rw-   0        0        0     1566 2023-06-13 17:01:15.000000 selenium-simplified-0.6/simplified/UserActivities.py
--rw-rw-rw-   0        0        0     1848 2023-06-13 17:01:30.000000 selenium-simplified-0.6/simplified/__init__.py
--rw-rw-rw-   0        0        0      950 2023-06-13 17:17:38.000000 selenium-simplified-0.6/simplified/testLibrary.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:46:17.663764 selenium-simplified-0.7/
+-rw-rw-rw-   0        0        0     4488 2023-06-15 16:46:17.662438 selenium-simplified-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4006 2023-06-14 14:02:21.000000 selenium-simplified-0.7/README.md
+-rw-rw-rw-   0        0        0      103 2023-06-15 16:03:52.000000 selenium-simplified-0.7/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-15 16:46:17.654450 selenium-simplified-0.7/selenium_simplified.egg-info/
+-rw-rw-rw-   0        0        0     4488 2023-06-15 16:46:17.000000 selenium-simplified-0.7/selenium_simplified.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-06-15 16:46:17.000000 selenium-simplified-0.7/selenium_simplified.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 16:46:17.000000 selenium-simplified-0.7/selenium_simplified.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-15 16:46:17.000000 selenium-simplified-0.7/selenium_simplified.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-15 16:46:17.000000 selenium-simplified-0.7/selenium_simplified.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 16:46:17.663764 selenium-simplified-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-06-15 16:45:13.000000 selenium-simplified-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:46:17.657605 selenium-simplified-0.7/simplified/
+-rw-rw-rw-   0        0        0     1567 2023-06-15 16:32:34.000000 selenium-simplified-0.7/simplified/UserActivities.py
+-rw-rw-rw-   0        0        0     1846 2023-06-15 16:15:59.000000 selenium-simplified-0.7/simplified/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:46:17.657605 selenium-simplified-0.7/simplified/locator/
+-rw-rw-rw-   0        0        0      952 2023-06-15 16:35:30.000000 selenium-simplified-0.7/simplified/locator/TagsLocator.py
+-rw-rw-rw-   0        0        0      455 2023-06-15 16:42:40.000000 selenium-simplified-0.7/simplified/locator/__init__.py
```

### Comparing `selenium-simplified-0.6/PKG-INFO` & `selenium-simplified-0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-Metadata-Version: 2.1
-Name: selenium-simplified
-Version: 0.6
-Summary: A free, open-source web automation library for the Chrome browser using Selenium Python
-Home-page: https://github.com/raajrajnish/SeleniumSimplified.git
-Author: rajnish kumar
-Author-email: raajrajnish@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 # SeleniumSimplified 
 <p align="center">
   <img src="https://github.com/raajrajnish/SeleniumSimplified/blob/master/assets/Se.png?raw=true" alt="Logo-SeleniumSimplified" height=300 width=300/>
 </p>
 
 
-***A free, open-source web automation library for the Chrome browser using Selenium Python.***
+***A free, open-source web automation library to do anything and everything on the Chrome browser using Python.***
+
+    USE SELENIUM SIMPLIFIED FOR
+
+    1. Browser Automation or Web Scrapping
+    2. API automation or Data Scrapping using API
+    3. Headless Browser automation
+
+    and many more uses cases
+
+
 
 ### Description
 This library is created keeping those developers in mind who wish to automate their website for a task but do not wish to spend an excessive amount of time learning a new library.We made every effort when creating this toolkit to make web automation as simple and efficient as possible. This library's backend is the Python client for [Selenium](https://www.selenium.dev/). Selenium is the standard library for web automation and is quite powerful.
 
 In order to make things simple and easy to understand for anyone with a background in selenium, we have made an effort to keep the function name as close to the original selenium functions as possible.
 
 ### Advantages
@@ -88,8 +86,8 @@
 print(driver.get_tab_title())
 
 # How to close the current browser tab
 driver.close_current_tab()
 
 # How to close browser
 driver.close_browser()
-```
+```
```

### Comparing `selenium-simplified-0.6/README.md` & `selenium-simplified-0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,36 @@
+Metadata-Version: 2.1
+Name: selenium-simplified
+Version: 0.7
+Summary: A free, open-source web automation library for the Chrome browser using Selenium Python
+Home-page: https://github.com/raajrajnish/SeleniumSimplified.git
+Author: rajnish kumar
+Author-email: raajrajnish@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+
 # SeleniumSimplified 
 <p align="center">
   <img src="https://github.com/raajrajnish/SeleniumSimplified/blob/master/assets/Se.png?raw=true" alt="Logo-SeleniumSimplified" height=300 width=300/>
 </p>
 
 
-***A free, open-source web automation library for the Chrome browser using Selenium Python.***
+***A free, open-source web automation library to do anything and everything on the Chrome browser using Python.***
+
+    USE SELENIUM SIMPLIFIED FOR
+
+    1. Browser Automation or Web Scrapping
+    2. API automation or Data Scrapping using API
+    3. Headless Browser automation
+
+    and many more uses cases
+
+
 
 ### Description
 This library is created keeping those developers in mind who wish to automate their website for a task but do not wish to spend an excessive amount of time learning a new library.We made every effort when creating this toolkit to make web automation as simple and efficient as possible. This library's backend is the Python client for [Selenium](https://www.selenium.dev/). Selenium is the standard library for web automation and is quite powerful.
 
 In order to make things simple and easy to understand for anyone with a background in selenium, we have made an effort to keep the function name as close to the original selenium functions as possible.
 
 ### Advantages
@@ -76,8 +98,8 @@
 print(driver.get_tab_title())
 
 # How to close the current browser tab
 driver.close_current_tab()
 
 # How to close browser
 driver.close_browser()
-```
+```
```

### Comparing `selenium-simplified-0.6/selenium_simplified.egg-info/PKG-INFO` & `selenium-simplified-0.7/selenium_simplified.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-simplified
-Version: 0.6
+Version: 0.7
 Summary: A free, open-source web automation library for the Chrome browser using Selenium Python
 Home-page: https://github.com/raajrajnish/SeleniumSimplified.git
 Author: rajnish kumar
 Author-email: raajrajnish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,25 @@
 
 # SeleniumSimplified 
 <p align="center">
   <img src="https://github.com/raajrajnish/SeleniumSimplified/blob/master/assets/Se.png?raw=true" alt="Logo-SeleniumSimplified" height=300 width=300/>
 </p>
 
 
-***A free, open-source web automation library for the Chrome browser using Selenium Python.***
+***A free, open-source web automation library to do anything and everything on the Chrome browser using Python.***
+
+    USE SELENIUM SIMPLIFIED FOR
+
+    1. Browser Automation or Web Scrapping
+    2. API automation or Data Scrapping using API
+    3. Headless Browser automation
+
+    and many more uses cases
+
+
 
 ### Description
 This library is created keeping those developers in mind who wish to automate their website for a task but do not wish to spend an excessive amount of time learning a new library.We made every effort when creating this toolkit to make web automation as simple and efficient as possible. This library's backend is the Python client for [Selenium](https://www.selenium.dev/). Selenium is the standard library for web automation and is quite powerful.
 
 In order to make things simple and easy to understand for anyone with a background in selenium, we have made an effort to keep the function name as close to the original selenium functions as possible.
 
 ### Advantages
```

### Comparing `selenium-simplified-0.6/setup.py` & `selenium-simplified-0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="selenium-simplified",
-    version="0.6",
+    version="0.7",
     author="rajnish kumar",
     author_email="raajrajnish@gmail.com",
     description="A free, open-source web automation library for the Chrome browser using Selenium Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/raajrajnish/SeleniumSimplified.git",
     packages=setuptools.find_packages(),
-    # packages=['simplified'],
-    install_requires=['selenium'],
+    install_requires=['selenium','bs4'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `selenium-simplified-0.6/simplified/UserActivities.py` & `selenium-simplified-0.7/simplified/UserActivities.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     original_style = element.get_attribute('style')
     apply_style("background: blue; border: 2px solid orange;")
     time.sleep(.3)
     apply_style(original_style)
 
 
 class CommonActivities:
-    def __init__(self,driver):
+    def __init__(self, driver):
         self.driver = driver
 
     def open_url(self, url):
         self.driver.get(url)
 
     def get_title(self):
         return self.driver.title
```

### Comparing `selenium-simplified-0.6/simplified/__init__.py` & `selenium-simplified-0.7/simplified/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     driver.implicitly_wait(universal_wait)
     # maximizing the window
     driver.maximize_window()
     # return the driver instance
     return driver
 
 
-class SeleniumSimplified():
+class SeleniumSimplified:
     def __init__(self):
         driver = open_chrome()
         base_functions = CommonActivities(driver)
         self.base_functions = base_functions
 
     def open_url(self, url):
         self.base_functions.open_url(url=url)
```

