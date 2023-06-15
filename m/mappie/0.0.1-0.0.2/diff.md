# Comparing `tmp/mappie-0.0.1.tar.gz` & `tmp/mappie-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mappie-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mappie-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mappie-0.0.1.tar` & `mappie-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0      622 2023-06-13 00:00:05.424119 mappie-0.0.1/.builds/main.yml
--rw-r--r--   0        0        0      615 2023-06-13 00:00:05.424119 mappie-0.0.1/.builds/mockbuild-epel9.yml
--rw-r--r--   0        0        0      620 2023-06-13 00:00:05.424119 mappie-0.0.1/.builds/mockbuild.yml
--rw-r--r--   0        0        0      252 2023-06-13 00:00:05.424119 mappie-0.0.1/.copr/Makefile
--rw-r--r--   0        0        0      147 2023-06-13 00:00:05.424119 mappie-0.0.1/.gitignore
--rw-r--r--   0        0        0     1676 2023-06-13 00:00:05.424119 mappie-0.0.1/CONTRIBUTING.md
-lrwxr-xr-x   0        0        0        0 2023-06-13 00:11:18.253471 mappie-0.0.1/LICENSE -> LICENSES/MIT.txt
--rw-r--r--   0        0        0     1078 2023-06-13 00:00:05.424119 mappie-0.0.1/LICENSES/MIT.txt
--rw-r--r--   0        0        0      157 2023-06-13 00:14:59.674593 mappie-0.0.1/NEWS.md
--rw-r--r--   0        0        0     1348 2023-06-13 00:00:05.424119 mappie-0.0.1/README.md
--rwxr-xr-x   0        0        0      912 2023-06-13 00:00:05.424119 mappie-0.0.1/contrib/fedoraify.py
--rw-r--r--   0        0        0     4393 2023-06-13 00:11:45.866362 mappie-0.0.1/noxfile.py
--rw-r--r--   0        0        0     1992 2023-06-13 00:00:05.425119 mappie-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1148 2023-06-13 00:14:59.044595 mappie-0.0.1/python-mappie.spec
--rw-r--r--   0        0        0      694 2023-06-13 00:00:05.425119 mappie-0.0.1/ruff.toml
--rw-r--r--   0        0        0     5865 2023-06-13 00:14:48.140639 mappie-0.0.1/src/mappie/__init__.py
--rw-r--r--   0        0        0       80 2023-06-13 00:00:05.425119 mappie-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     3242 2023-06-13 00:00:05.548118 mappie-0.0.1/tests/test_mappie.py
--rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 mappie-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      672 2023-06-13 00:57:44.504070 mappie-0.0.2/.builds/main.yml
+-rw-r--r--   0        0        0      615 2023-06-13 00:40:41.885378 mappie-0.0.2/.builds/mockbuild-epel9.yml
+-rw-r--r--   0        0        0      620 2023-06-13 00:40:41.883378 mappie-0.0.2/.builds/mockbuild.yml
+-rw-r--r--   0        0        0      252 2023-06-13 00:00:05.424119 mappie-0.0.2/.copr/Makefile
+-rw-r--r--   0        0        0      147 2023-06-13 00:00:05.424119 mappie-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1676 2023-06-13 00:00:05.424119 mappie-0.0.2/CONTRIBUTING.md
+lrwxr-xr-x   0        0        0        0 2023-06-13 00:40:41.892378 mappie-0.0.2/LICENSE -> LICENSES/MIT.txt
+-rw-r--r--   0        0        0     1078 2023-06-13 00:00:05.424119 mappie-0.0.2/LICENSES/MIT.txt
+-rw-r--r--   0        0        0      304 2023-06-15 20:09:00.413993 mappie-0.0.2/NEWS.md
+-rw-r--r--   0        0        0     1348 2023-06-13 00:00:05.424119 mappie-0.0.2/README.md
+-rwxr-xr-x   0        0        0      912 2023-06-13 00:00:05.424119 mappie-0.0.2/contrib/fedoraify.py
+-rw-r--r--   0        0        0     4395 2023-06-13 00:25:05.463160 mappie-0.0.2/noxfile.py
+-rw-r--r--   0        0        0     1992 2023-06-13 00:00:05.425119 mappie-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1245 2023-06-15 20:09:00.008994 mappie-0.0.2/python-mappie.spec
+-rw-r--r--   0        0        0      694 2023-06-13 00:00:05.425119 mappie-0.0.2/ruff.toml
+-rw-r--r--   0        0        0     5865 2023-06-15 20:08:54.661005 mappie-0.0.2/src/mappie/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 19:54:33.674885 mappie-0.0.2/src/mappie/py.typed
+-rw-r--r--   0        0        0       80 2023-06-13 00:00:05.425119 mappie-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     3242 2023-06-13 00:00:05.548118 mappie-0.0.2/tests/test_mappie.py
+-rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 mappie-0.0.2/PKG-INFO
```

### Comparing `mappie-0.0.1/.builds/mockbuild-epel9.yml` & `mappie-0.0.2/.builds/mockbuild-epel9.yml`

 * *Files identical despite different names*

### Comparing `mappie-0.0.1/.builds/mockbuild.yml` & `mappie-0.0.2/.builds/mockbuild.yml`

 * *Files identical despite different names*

### Comparing `mappie-0.0.1/CONTRIBUTING.md` & `mappie-0.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mappie-0.0.1/LICENSES/MIT.txt` & `mappie-0.0.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `mappie-0.0.1/README.md` & `mappie-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mappie-0.0.1/contrib/fedoraify.py` & `mappie-0.0.2/contrib/fedoraify.py`

 * *Files identical despite different names*

### Comparing `mappie-0.0.1/noxfile.py` & `mappie-0.0.2/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,30 +108,30 @@
     session.run("releaserr", "build", "--sign", "--backend", "flit_core")
 
 
 @nox.session
 def publish(session: nox.Session):
     # Setup
     install(session, RELEASERR)
-    session.run("releaserr", "check-clean")
+    session.run("releaserr", "ensure-clean")
 
     # Upload to PyPI
     session.run("releaserr", "upload")
 
     # Push to git, publish artifacts to sourcehut, and release to copr
     if not session.interactive or input(
         "Push to Sourcehut and copr build (Y/n)"
     ).lower() in ("", "y"):
         git(session, "push", "--follow-tags")
         session.run("hut", "git", "artifact", "upload", *iglob("dist/*"), external=True)
         copr_release(session)
 
     # Post-release bump
-    session.run("releaserr", "post-version", "-s", "pyproject.toml")
-    git(session, "add", "pyproject.toml")
+    session.run("releaserr", "post-version", "-s", "file")
+    git(session, "add", "src/{PROJECT}/__init__.py")
     git(session, "commit", "-S", "-m", "Post release version bump")
 
 
 @nox.session
 def copr_release(session: nox.Session):
     install(session, "copr-cli", "requests-gssapi", "specfile")
     tmp = Path(session.create_tmp())
```

### Comparing `mappie-0.0.1/pyproject.toml` & `mappie-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mappie-0.0.1/python-mappie.spec` & `mappie-0.0.2/python-mappie.spec`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # SPDX-FileCopyrightText: 2023 Maxwell G <maxwell@gtmx.me>
 # SPDX-License-Identifier: MIT
 # License text: https://spdx.org/licenses/MIT
 
 Name:           python-mappie
-Version:        0.0.1
+Version:        0.0.2
 Release:        1%{?dist}
 Summary:        Python library with collections, frozen mappings, and more
 
 License:        MIT
 URL:            https://sr.ht/~gotmax23/mappie
 %global furl    https://git.sr.ht/~gotmax23/mappie
 Source0:        %{furl}/refs/download/v%{version}/mappie-%{version}.tar.gz
 
 BuildArch:      noarch
 
+BuildRequires:  gnupg2
 BuildRequires:  python3-devel
 
 %global _description %{expand:
 mappie is a python library with collections, frozen mappings, and more.}
 
 %description %_description
 
@@ -50,9 +51,12 @@
 
 %files -n python3-mappie -f %{pyproject_files}
 %doc README.md
 %license LICENSES/*
 
 
 %changelog
+* Thu Jun 15 2023 Maxwell G <maxwell@gtmx.me> - 0.0.2-1
+- Release 0.0.2.
+
 * Tue Jun 13 2023 Maxwell G <maxwell@gtmx.me> - 0.0.1-1
 - Release 0.0.1.
```

### Comparing `mappie-0.0.1/ruff.toml` & `mappie-0.0.2/ruff.toml`

 * *Files identical despite different names*

### Comparing `mappie-0.0.1/src/mappie/__init__.py` & `mappie-0.0.2/src/mappie/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # We deliberately import Mapping from typing.
 # Older Pythons don't have __class_getitem__ at runtime.
 from typing import TYPE_CHECKING, Any, Generic, Mapping, TypeVar
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 _T = TypeVar("_T")
 _T2 = TypeVar("_T2")
 
 
 def _copy_dict(mapping: Mapping[_T, _T2] | _UnsafeDict) -> dict[_T, _T2]:
     if isinstance(mapping, _UnsafeDict):
```

### Comparing `mappie-0.0.1/tests/test_mappie.py` & `mappie-0.0.2/tests/test_mappie.py`

 * *Files identical despite different names*

### Comparing `mappie-0.0.1/PKG-INFO` & `mappie-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mappie
-Version: 0.0.1
+Version: 0.0.2
 Summary: Collections, frozen mappings, and more
 Author-email: Maxwell G <maxwell@gtmx.me>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

