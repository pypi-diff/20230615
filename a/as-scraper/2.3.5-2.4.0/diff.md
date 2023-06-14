# Comparing `tmp/as-scraper-2.3.5.tar.gz` & `tmp/as-scraper-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "as-scraper-2.3.5.tar", last modified: Wed Jun 14 21:54:14 2023, max compression
+gzip compressed data, was "as-scraper-2.4.0.tar", last modified: Wed Jun 14 22:12:58 2023, max compression
```

## Comparing `as-scraper-2.3.5.tar` & `as-scraper-2.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:54:14.376363 as-scraper-2.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-14 21:53:54.000000 as-scraper-2.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-14 21:54:14.376363 as-scraper-2.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-06-14 21:53:54.000000 as-scraper-2.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:54:14.376363 as-scraper-2.3.5/as_scraper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 21:53:54.000000 as-scraper-2.3.5/as_scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:54:14.376363 as-scraper-2.3.5/as_scraper/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-14 21:53:54.000000 as-scraper-2.3.5/as_scraper/crawlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-14 21:53:54.000000 as-scraper-2.3.5/as_scraper/crawlers/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-14 21:53:54.000000 as-scraper-2.3.5/as_scraper/crawlers/tree_crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-14 21:53:54.000000 as-scraper-2.3.5/as_scraper/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-14 21:53:54.000000 as-scraper-2.3.5/as_scraper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-14 21:53:54.000000 as-scraper-2.3.5/as_scraper/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-06-14 21:53:54.000000 as-scraper-2.3.5/as_scraper/scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:54:14.376363 as-scraper-2.3.5/as_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-14 21:54:14.000000 as-scraper-2.3.5/as_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-14 21:54:14.000000 as-scraper-2.3.5/as_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:54:14.000000 as-scraper-2.3.5/as_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-14 21:54:14.000000 as-scraper-2.3.5/as_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 21:54:14.000000 as-scraper-2.3.5/as_scraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:54:14.376363 as-scraper-2.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-14 21:53:54.000000 as-scraper-2.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:12:58.724637 as-scraper-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-14 22:12:40.000000 as-scraper-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-14 22:12:58.724637 as-scraper-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-06-14 22:12:40.000000 as-scraper-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:12:58.724637 as-scraper-2.4.0/as_scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 22:12:40.000000 as-scraper-2.4.0/as_scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:12:58.724637 as-scraper-2.4.0/as_scraper/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-14 22:12:40.000000 as-scraper-2.4.0/as_scraper/crawlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-14 22:12:40.000000 as-scraper-2.4.0/as_scraper/crawlers/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-14 22:12:40.000000 as-scraper-2.4.0/as_scraper/crawlers/tree_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-14 22:12:40.000000 as-scraper-2.4.0/as_scraper/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-14 22:12:40.000000 as-scraper-2.4.0/as_scraper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-14 22:12:40.000000 as-scraper-2.4.0/as_scraper/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-06-14 22:12:40.000000 as-scraper-2.4.0/as_scraper/scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:12:58.724637 as-scraper-2.4.0/as_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-14 22:12:58.000000 as-scraper-2.4.0/as_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-14 22:12:58.000000 as-scraper-2.4.0/as_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 22:12:58.000000 as-scraper-2.4.0/as_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-14 22:12:58.000000 as-scraper-2.4.0/as_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 22:12:58.000000 as-scraper-2.4.0/as_scraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 22:12:58.724637 as-scraper-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-14 22:12:40.000000 as-scraper-2.4.0/setup.py
```

### Comparing `as-scraper-2.3.5/LICENSE` & `as-scraper-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `as-scraper-2.3.5/PKG-INFO` & `as-scraper-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: as-scraper
-Version: 2.3.5
+Version: 2.4.0
 Summary: Python library for scraping with Selenium.
 Home-page: https://github.com/Avila-Systems/as-scraper
 Author: Alvaro Avila
 Author-email: almiavicas@gmail.com
 Project-URL: Github Project, https://github.com/Avila-Systems/as-scraper
 Project-URL: Issue Tracker, https://github.com/Avila-Systems/as-scraper/issues
 Classifier: Intended Audience :: Developers
```

### Comparing `as-scraper-2.3.5/README.md` & `as-scraper-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `as-scraper-2.3.5/as_scraper/crawlers/crawler.py` & `as-scraper-2.4.0/as_scraper/crawlers/crawler.py`

 * *Files identical despite different names*

### Comparing `as-scraper-2.3.5/as_scraper/crawlers/tree_crawler.py` & `as-scraper-2.4.0/as_scraper/crawlers/tree_crawler.py`

 * *Files identical despite different names*

### Comparing `as-scraper-2.3.5/as_scraper/scraper.py` & `as-scraper-2.4.0/as_scraper/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,40 +32,42 @@
     LOAD_JAVASCRIPT = False
     LOG_PATH = None
     ERROR_THRESHOLD = 0.05
     RESET_AFTER = None
     LOAD_TIMEOUT = None
     TEST_MODE = False
     DTYPES = None
+    HEADLESS = True
+    LOAD_IMAGES = False
 
     def __init__(self, urls: Optional[List[str]] = None, test_mode: Optional[bool] = None):
         self.headers = HEADERS
         self.urls = urls
         self._driver = None
         self._session = None
         if test_mode is not None:
-            self.TEST_MODE = test_mode
+            self.HEADLESS = not test_mode
 
     @property
     def driver(self):
         'Create a Firefox driver for selenium'
         if self._driver is None:
             firefox_options = FirefoxOptions()
             firefox_options.set_preference('browser.cache.disk.enable', False)
             firefox_options.set_preference(
                 'browser.cache.memory.enable', False)
             firefox_options.set_preference(
                 'browser.cache.offline.enable', False)
             firefox_options.set_preference('network.http.use-cache', False)
             firefox_options.set_preference('permissions.default.image', 2)
-            firefox_options.set_preference(
-                'dom.ipc.plugins.enabled.libflashplayer.so', 'false')
+            if not self.LOAD_IMAGES:
+                firefox_options.set_preference('dom.ipc.plugins.enabled.libflashplayer.so', 'false')
             firefox_options.set_preference(
                 'general.useragent.override', HEADERS['User-Agent'])
-            if not self.TEST_MODE:
+            if self.HEADLESS:
                 firefox_options.add_argument('--headless')
             else:
                 log.warning('Creating driver without headless mode')
                 if self.LOG_PATH is None:
                     self.LOG_PATH = 'geckodriver.log'
             service = Service(log_path=self.LOG_PATH)
             self._driver = Firefox(options=firefox_options, service=service)
```

### Comparing `as-scraper-2.3.5/as_scraper.egg-info/PKG-INFO` & `as-scraper-2.4.0/as_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: as-scraper
-Version: 2.3.5
+Version: 2.4.0
 Summary: Python library for scraping with Selenium.
 Home-page: https://github.com/Avila-Systems/as-scraper
 Author: Alvaro Avila
 Author-email: almiavicas@gmail.com
 Project-URL: Github Project, https://github.com/Avila-Systems/as-scraper
 Project-URL: Issue Tracker, https://github.com/Avila-Systems/as-scraper/issues
 Classifier: Intended Audience :: Developers
```

### Comparing `as-scraper-2.3.5/setup.py` & `as-scraper-2.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def get_long_description():
     with open('README.md') as file:
         return file.read()
 
 
 setup(
     name='as-scraper',
-    version='2.3.5',
+    version='2.4.0',
     description='Python library for scraping with Selenium.',
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
     author='Alvaro Avila',
     author_email='almiavicas@gmail.com',
     url='https://github.com/Avila-Systems/as-scraper',
     project_urls={
```

