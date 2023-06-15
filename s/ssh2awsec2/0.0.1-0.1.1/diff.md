# Comparing `tmp/ssh2awsec2-0.0.1.tar.gz` & `tmp/ssh2awsec2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh2awsec2-0.0.1.tar", last modified: Wed Jun 14 02:03:52 2023, max compression
+gzip compressed data, was "ssh2awsec2-0.1.1.tar", last modified: Thu Jun 15 00:50:55 2023, max compression
```

## Comparing `ssh2awsec2-0.0.1.tar` & `ssh2awsec2-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,51 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 02:03:52.261653 ssh2awsec2-0.0.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      484 2023-06-14 01:47:24.000000 ssh2awsec2-0.0.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-06-14 01:25:39.000000 ssh2awsec2-0.0.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      318 2023-06-14 01:25:39.000000 ssh2awsec2-0.0.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     3638 2023-06-14 02:03:52.261505 ssh2awsec2-0.0.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     2598 2023-06-14 01:55:28.000000 ssh2awsec2-0.0.1/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      465 2023-06-14 01:52:24.000000 ssh2awsec2-0.0.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)       37 2023-05-23 02:30:18.000000 ssh2awsec2-0.0.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-14 01:34:51.000000 ssh2awsec2-0.0.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-14 01:34:32.000000 ssh2awsec2-0.0.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-14 01:31:48.000000 ssh2awsec2-0.0.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       29 2023-06-14 01:30:43.000000 ssh2awsec2-0.0.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-14 02:03:52.261697 ssh2awsec2-0.0.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7510 2023-06-14 01:42:16.000000 ssh2awsec2-0.0.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 02:03:52.258992 ssh2awsec2-0.0.1/ssh2awsec2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      331 2023-06-14 01:41:44.000000 ssh2awsec2-0.0.1/ssh2awsec2/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-14 01:25:39.000000 ssh2awsec2-0.0.1/ssh2awsec2/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-14 01:41:26.000000 ssh2awsec2-0.0.1/ssh2awsec2/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 02:03:52.260104 ssh2awsec2-0.0.1/ssh2awsec2/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-14 01:25:39.000000 ssh2awsec2-0.0.1/ssh2awsec2/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      657 2023-05-22 19:25:03.000000 ssh2awsec2-0.0.1/ssh2awsec2/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 02:03:52.260552 ssh2awsec2-0.0.1/ssh2awsec2/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-05-22 19:25:03.000000 ssh2awsec2-0.0.1/ssh2awsec2/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-05-23 01:08:52.000000 ssh2awsec2-0.0.1/ssh2awsec2/tests/helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 02:03:52.261029 ssh2awsec2-0.0.1/ssh2awsec2/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-14 01:31:56.000000 ssh2awsec2-0.0.1/ssh2awsec2/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-23 00:54:22.000000 ssh2awsec2-0.0.1/ssh2awsec2/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 02:03:52.259952 ssh2awsec2-0.0.1/ssh2awsec2.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     3638 2023-06-14 02:03:52.000000 ssh2awsec2-0.0.1/ssh2awsec2.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      608 2023-06-14 02:03:52.000000 ssh2awsec2-0.0.1/ssh2awsec2.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-14 02:03:52.000000 ssh2awsec2-0.0.1/ssh2awsec2.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      168 2023-06-14 02:03:52.000000 ssh2awsec2-0.0.1/ssh2awsec2.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       11 2023-06-14 02:03:52.000000 ssh2awsec2-0.0.1/ssh2awsec2.egg-info/top_level.txt
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 02:03:52.261248 ssh2awsec2-0.0.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      214 2023-06-14 01:42:42.000000 ssh2awsec2-0.0.1/tests/test_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 00:50:55.485524 ssh2awsec2-0.1.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      637 2023-06-15 00:44:02.000000 ssh2awsec2-0.1.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-06-14 01:25:39.000000 ssh2awsec2-0.1.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      318 2023-06-14 01:25:39.000000 ssh2awsec2-0.1.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     8536 2023-06-15 00:50:55.485348 ssh2awsec2-0.1.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7394 2023-06-15 00:40:54.000000 ssh2awsec2-0.1.1/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      919 2023-06-15 00:49:42.000000 ssh2awsec2-0.1.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)       37 2023-05-23 02:30:18.000000 ssh2awsec2-0.1.1/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-14 01:34:51.000000 ssh2awsec2-0.1.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-14 01:34:32.000000 ssh2awsec2-0.1.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-14 01:31:48.000000 ssh2awsec2-0.1.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      101 2023-06-14 19:10:33.000000 ssh2awsec2-0.1.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-15 00:50:55.485568 ssh2awsec2-0.1.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7771 2023-06-15 00:42:25.000000 ssh2awsec2-0.1.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 00:50:55.480675 ssh2awsec2-0.1.1/ssh2awsec2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      439 2023-06-15 00:43:39.000000 ssh2awsec2-0.1.1/ssh2awsec2/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-15 00:49:47.000000 ssh2awsec2-0.1.1/ssh2awsec2/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      237 2023-06-14 22:58:37.000000 ssh2awsec2-0.1.1/ssh2awsec2/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      514 2023-06-14 14:42:08.000000 ssh2awsec2-0.1.1/ssh2awsec2/better_boto.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      246 2023-06-14 16:34:47.000000 ssh2awsec2-0.1.1/ssh2awsec2/boto_ses.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      113 2023-06-14 15:22:45.000000 ssh2awsec2-0.1.1/ssh2awsec2/cache.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 00:50:55.482845 ssh2awsec2-0.1.1/ssh2awsec2/cli/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-14 21:57:30.000000 ssh2awsec2-0.1.1/ssh2awsec2/cli/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      520 2023-06-15 00:36:53.000000 ssh2awsec2-0.1.1/ssh2awsec2/cli/commands.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1384 2023-06-15 00:36:59.000000 ssh2awsec2-0.1.1/ssh2awsec2/cli/config.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      341 2023-06-15 00:37:18.000000 ssh2awsec2-0.1.1/ssh2awsec2/cli/main.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     8472 2023-06-15 00:33:12.000000 ssh2awsec2-0.1.1/ssh2awsec2/cli/ssh.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1098 2023-06-15 00:37:48.000000 ssh2awsec2-0.1.1/ssh2awsec2/config.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 00:50:55.483147 ssh2awsec2-0.1.1/ssh2awsec2/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-14 01:25:39.000000 ssh2awsec2-0.1.1/ssh2awsec2/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      140 2023-06-14 19:17:29.000000 ssh2awsec2-0.1.1/ssh2awsec2/logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1065 2023-06-14 22:53:30.000000 ssh2awsec2-0.1.1/ssh2awsec2/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2210 2023-06-14 23:06:50.000000 ssh2awsec2-0.1.1/ssh2awsec2/pem_file.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3659 2023-06-15 00:33:36.000000 ssh2awsec2-0.1.1/ssh2awsec2/recent.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 00:50:55.483611 ssh2awsec2-0.1.1/ssh2awsec2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-05-22 19:25:03.000000 ssh2awsec2-0.1.1/ssh2awsec2/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-05-23 01:08:52.000000 ssh2awsec2-0.1.1/ssh2awsec2/tests/helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 00:50:55.484569 ssh2awsec2-0.1.1/ssh2awsec2/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-14 01:31:56.000000 ssh2awsec2-0.1.1/ssh2awsec2/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    17911 2023-06-14 19:16:51.000000 ssh2awsec2-0.1.1/ssh2awsec2/vendor/nested_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-23 00:54:22.000000 ssh2awsec2-0.1.1/ssh2awsec2/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 00:50:55.481546 ssh2awsec2-0.1.1/ssh2awsec2.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     8536 2023-06-15 00:50:55.000000 ssh2awsec2-0.1.1/ssh2awsec2.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      982 2023-06-15 00:50:55.000000 ssh2awsec2-0.1.1/ssh2awsec2.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-15 00:50:55.000000 ssh2awsec2-0.1.1/ssh2awsec2.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       88 2023-06-15 00:50:55.000000 ssh2awsec2-0.1.1/ssh2awsec2.egg-info/entry_points.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      240 2023-06-15 00:50:55.000000 ssh2awsec2-0.1.1/ssh2awsec2.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       11 2023-06-15 00:50:55.000000 ssh2awsec2-0.1.1/ssh2awsec2.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 00:50:55.484982 ssh2awsec2-0.1.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      352 2023-06-14 22:59:11.000000 ssh2awsec2-0.1.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1714 2023-06-14 23:05:57.000000 ssh2awsec2-0.1.1/tests/test_pem_file.py
```

### Comparing `ssh2awsec2-0.0.1/LICENSE.txt` & `ssh2awsec2-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssh2awsec2-0.0.1/requirements-doc.txt` & `ssh2awsec2-0.1.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `ssh2awsec2-0.0.1/setup.py` & `ssh2awsec2-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,15 @@
     except:
         GITHUB_USERNAME = "Unknown-Github-Username"
 
     # Short description will be the description on PyPI
     try:
         SHORT_DESCRIPTION = package.__short_description__  # GitHub Short Description
     except:
-        print(
-            "'__short_description__' not found in '%s.__init__.py'!" % PKG_NAME)
+        print("'__short_description__' not found in '%s.__init__.py'!" % PKG_NAME)
         SHORT_DESCRIPTION = "No short description!"
 
     # Long description will be the body of content on PyPI page
     try:
         LONG_DESCRIPTION = open("README.rst", "rb").read().decode("utf-8")
     except:
         LONG_DESCRIPTION = "No long description!"
@@ -61,47 +60,52 @@
 
     try:
         MAINTAINER_EMAIL = package.__maintainer_email__
     except:
         MAINTAINER_EMAIL = None
 
     PACKAGES, INCLUDE_PACKAGE_DATA, PACKAGE_DATA, PY_MODULES = (
-        None, None, None, None,
+        None,
+        None,
+        None,
+        None,
     )
 
     # It's a directory style package
     if os.path.exists(__file__[:-8] + PKG_NAME):
         # Include all sub packages in package directory
         PACKAGES = [PKG_NAME] + [
-            "%s.%s" % (PKG_NAME, i)
-            for i in find_packages(PKG_NAME)
+            "%s.%s" % (PKG_NAME, i) for i in find_packages(PKG_NAME)
         ]
 
         # Include everything in package directory
         INCLUDE_PACKAGE_DATA = True
         PACKAGE_DATA = {
             "": ["*.*"],
         }
 
     # It's a single script style package
     elif os.path.exists(__file__[:-8] + PKG_NAME + ".py"):
-        PY_MODULES = [PKG_NAME, ]
+        PY_MODULES = [
+            PKG_NAME,
+        ]
 
     # The project directory name is the GitHub repository name
     repository_name = os.path.basename(os.path.dirname(os.path.abspath(__file__)))
 
     # Project Url
     URL = "https://github.com/{0}/{1}".format(GITHUB_USERNAME, repository_name)
 
     # Use todays date as GitHub release tag
     github_release_tag = str(date.today())
 
     # Source code download url
     DOWNLOAD_URL = "https://pypi.python.org/pypi/{0}/{1}#downloads".format(
-        PKG_NAME, VERSION)
+        PKG_NAME, VERSION
+    )
 
     try:
         LICENSE = package.__license__
     except:
         print("'__license__' not found in '%s.__init__.py'!" % PKG_NAME)
         LICENSE = ""
 
@@ -119,14 +123,15 @@
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS",
         "Operating System :: Unix",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
     ]
     """
     Full list can be found at: https://pypi.python.org/pypi?%3Aaction=list_classifiers
     """
 
     def read_requirements_file(path):
@@ -134,20 +139,19 @@
         Read requirements.txt, ignore comments
         """
         requires = list()
         f = open(path, "rb")
         for line in f.read().decode("utf-8").split("\n"):
             line = line.strip()
             if "#" in line:
-                line = line[:line.find("#")].strip()
+                line = line[: line.find("#")].strip()
             if line:
                 requires.append(line)
         return requires
 
-
     try:
         REQUIRES = read_requirements_file("requirements.txt")
     except:
         print("'requirements.txt' not found!")
         REQUIRES = list()
 
     EXTRA_REQUIRE = dict()
@@ -178,14 +182,20 @@
         url=URL,
         download_url=DOWNLOAD_URL,
         classifiers=CLASSIFIERS,
         platforms=PLATFORMS,
         license=LICENSE,
         install_requires=REQUIRES,
         extras_require=EXTRA_REQUIRE,
+        entry_points={
+            "console_scripts": [
+                "ssh2awsec2=ssh2awsec2.cli.main:run",
+                "sshec2=ssh2awsec2.cli.main:run",
+            ],
+        },
     )
 
 """
 Appendix
 --------
 Frequent used classifiers List::
```

### Comparing `ssh2awsec2-0.0.1/ssh2awsec2/vendor/pytest_cov_helper.py` & `ssh2awsec2-0.1.1/ssh2awsec2/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

