# Comparing `tmp/lektorlib-1.2.0.tar.gz` & `tmp/lektorlib-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lektorlib-1.2.0.tar", last modified: Fri Jun  2 20:51:24 2023, max compression
+gzip compressed data, was "lektorlib-1.2.1.tar", last modified: Thu Jun 15 17:39:02 2023, max compression
```

## Comparing `lektorlib-1.2.0.tar` & `lektorlib-1.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      567 2023-06-02 20:51:07.394074 lektorlib-1.2.0/CHANGES.md
--rw-r--r--   0        0        0     1062 2023-06-02 20:51:07.394074 lektorlib-1.2.0/LICENSE
--rw-r--r--   0        0        0     2204 2023-06-02 20:51:07.394074 lektorlib-1.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-02 20:51:07.394074 lektorlib-1.2.0/lektorlib/__init__.py
--rw-r--r--   0        0        0     1219 2023-06-02 20:51:07.394074 lektorlib-1.2.0/lektorlib/context.py
--rw-r--r--   0        0        0        0 2023-06-02 20:51:07.394074 lektorlib-1.2.0/lektorlib/py.typed
--rw-r--r--   0        0        0     6155 2023-06-02 20:51:07.394074 lektorlib-1.2.0/lektorlib/query.py
--rw-r--r--   0        0        0     1056 2023-06-02 20:51:07.394074 lektorlib-1.2.0/lektorlib/recordcache.py
--rw-r--r--   0        0        0      749 2023-06-02 20:51:07.394074 lektorlib-1.2.0/lektorlib/testing.py
--rw-r--r--   0        0        0      753 2023-06-02 20:51:07.398074 lektorlib-1.2.0/pdm_build.py
--rw-r--r--   0        0        0     4963 2023-06-02 20:51:24.386522 lektorlib-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1014 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/conftest.py
--rw-r--r--   0        0        0       27 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test-site/Test Site.lektorproject
--rw-r--r--   0        0        0      538 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test-site/assets/static/style.css
--rw-r--r--   0        0        0      144 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test-site/content/about/contents.lr
--rw-r--r--   0        0        0      135 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test-site/content/contents.lr
--rw-r--r--   0        0        0       96 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test-site/content/projects/contents.lr
--rw-r--r--   0        0        0      133 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test-site/models/page.ini
--rw-r--r--   0        0        0      804 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test-site/templates/layout.html
--rw-r--r--   0        0        0      475 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test-site/templates/macros/pagination.html
--rw-r--r--   0        0        0      154 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test-site/templates/page.html
--rw-r--r--   0        0        0     2103 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test_context.py
--rw-r--r--   0        0        0     8876 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test_query.py
--rw-r--r--   0        0        0     2087 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test_recordcache.py
--rw-r--r--   0        0        0      727 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test_testing.py
--rw-r--r--   0        0        0     1178 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tox.ini
--rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 lektorlib-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      762 2023-06-15 17:38:47.118280 lektorlib-1.2.1/CHANGES.md
+-rw-r--r--   0        0        0     1062 2023-06-15 17:38:47.118280 lektorlib-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2204 2023-06-15 17:38:47.118280 lektorlib-1.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-15 17:38:47.118280 lektorlib-1.2.1/lektorlib/__init__.py
+-rw-r--r--   0        0        0     1219 2023-06-15 17:38:47.118280 lektorlib-1.2.1/lektorlib/context.py
+-rw-r--r--   0        0        0        0 2023-06-15 17:38:47.118280 lektorlib-1.2.1/lektorlib/py.typed
+-rw-r--r--   0        0        0     6295 2023-06-15 17:38:47.118280 lektorlib-1.2.1/lektorlib/query.py
+-rw-r--r--   0        0        0     1686 2023-06-15 17:38:47.118280 lektorlib-1.2.1/lektorlib/recordcache.py
+-rw-r--r--   0        0        0      749 2023-06-15 17:38:47.118280 lektorlib-1.2.1/lektorlib/testing.py
+-rw-r--r--   0        0        0      753 2023-06-15 17:38:47.118280 lektorlib-1.2.1/pdm_build.py
+-rw-r--r--   0        0        0     5165 2023-06-15 17:39:02.318410 lektorlib-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1014 2023-06-15 17:38:47.118280 lektorlib-1.2.1/tests/conftest.py
+-rw-r--r--   0        0        0       27 2023-06-15 17:38:47.118280 lektorlib-1.2.1/tests/test-site/Test Site.lektorproject
+-rw-r--r--   0        0        0      538 2023-06-15 17:38:47.118280 lektorlib-1.2.1/tests/test-site/assets/static/style.css
+-rw-r--r--   0        0        0      144 2023-06-15 17:38:47.118280 lektorlib-1.2.1/tests/test-site/content/about/contents.lr
+-rw-r--r--   0        0        0      135 2023-06-15 17:38:47.118280 lektorlib-1.2.1/tests/test-site/content/contents.lr
+-rw-r--r--   0        0        0       96 2023-06-15 17:38:47.118280 lektorlib-1.2.1/tests/test-site/content/projects/contents.lr
+-rw-r--r--   0        0        0      133 2023-06-15 17:38:47.118280 lektorlib-1.2.1/tests/test-site/models/page.ini
+-rw-r--r--   0        0        0      804 2023-06-15 17:38:47.118280 lektorlib-1.2.1/tests/test-site/templates/layout.html
+-rw-r--r--   0        0        0      475 2023-06-15 17:38:47.118280 lektorlib-1.2.1/tests/test-site/templates/macros/pagination.html
+-rw-r--r--   0        0        0      154 2023-06-15 17:38:47.118280 lektorlib-1.2.1/tests/test-site/templates/page.html
+-rw-r--r--   0        0        0     2103 2023-06-15 17:38:47.118280 lektorlib-1.2.1/tests/test_context.py
+-rw-r--r--   0        0        0     8876 2023-06-15 17:38:47.118280 lektorlib-1.2.1/tests/test_query.py
+-rw-r--r--   0        0        0     2087 2023-06-15 17:38:47.118280 lektorlib-1.2.1/tests/test_recordcache.py
+-rw-r--r--   0        0        0      727 2023-06-15 17:38:47.118280 lektorlib-1.2.1/tests/test_testing.py
+-rw-r--r--   0        0        0     1178 2023-06-15 17:38:47.118280 lektorlib-1.2.1/tox.ini
+-rw-r--r--   0        0        0     5133 1970-01-01 00:00:00.000000 lektorlib-1.2.1/PKG-INFO
```

### Comparing `lektorlib-1.2.0/CHANGES.md` & `lektorlib-1.2.1/CHANGES.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 ## Changelog
 
+### Release 1.2.1 (2023-06-15)
+
+#### Type Annotations
+
+- Narrow the return type of `lektorlib.recordcache.get_or_create_virtual`.
+- Convert `lektorlib.query.PrecomputedQuery` to a generic type.
+
 ### Release 1.2.0 (2023-06-02)
 
 - Added type annotations
 - Use PDM instead of setuptools to build distribution
 - Configured pre-commit
 - Run black and reorder-python-imports on the code
```

### Comparing `lektorlib-1.2.0/LICENSE` & `lektorlib-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lektorlib-1.2.0/README.md` & `lektorlib-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lektorlib-1.2.0/lektorlib/context.py` & `lektorlib-1.2.1/lektorlib/context.py`

 * *Files identical despite different names*

### Comparing `lektorlib-1.2.0/lektorlib/query.py` & `lektorlib-1.2.1/lektorlib/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 
 """
 from __future__ import annotations
 
 import sys
 from collections import OrderedDict
 from typing import Generator
+from typing import Generic
 from typing import Iterable
 from typing import Sequence
 from typing import TYPE_CHECKING
+from typing import TypeVar
 
 from lektor.db import Pad
 from lektor.db import Query
 from lektor.db import Record
 from lektor.environment import PRIMARY_ALT
 from lektor.sourceobj import VirtualSourceObject
 
@@ -26,15 +28,15 @@
 
 def get_source(
     pad: Pad,
     path: str,
     alt: str = PRIMARY_ALT,
     page_num: int | None = None,
     persist: bool = True,
-) -> Record | VirtualSourceObject:
+) -> Record | VirtualSourceObject | None:
     """Like Pad.get() but works for paginated virtual sources as well as
     concrete records.
 
     """
     # lektor.db.Pad.get does not support page_num on a virtual path.
     # This is mostly because there seems to be no official syntax for
     # contructing a virtual path with a page number.
@@ -65,15 +67,18 @@
         return None
 
     paginated_source = pagination.for_page(page_num)
     pad.db.track_record_dependency(paginated_source)
     return paginated_source
 
 
-class PrecomputedQuery(Query):  # type: ignore[misc]
+_DBSourceObject = TypeVar("_DBSourceObject", bound="Record | VirtualSourceObject")
+
+
+class PrecomputedQuery(Generic[_DBSourceObject], Query):  # type: ignore[misc]
     """This is a Query which yields a pre-computed sequence of children.
 
     This is useful in (at least) two circumstances:
 
     First, when the children to be queried are virtual source objects,
     the standard ``lektor.db.Query`` will not work.  This version will.
 
@@ -103,27 +108,27 @@
         self.__assert_is_not_attachment_query()
 
     def _get(
         self,
         id: str,
         persist: bool = True,
         page_num: int | None | EllipsisType = Ellipsis,
-    ) -> Record | VirtualSourceObject:
+    ) -> _DBSourceObject | None:
         """Low level record access."""
         if id not in self.__child_ids:
             return None  # not in our query set
         return get_source(
             self.pad,
             path=f"{self.path}/{id}",
             page_num=self._page_num if page_num is Ellipsis else page_num,
             alt=self.alt,
             persist=persist,
         )
 
-    def _iterate(self) -> Generator[Record | VirtualSourceObject, None, None]:
+    def _iterate(self) -> Generator[_DBSourceObject, None, None]:
         self.__assert_is_not_attachment_query()
         # note dependencies
         self_record = self.pad.get(self.path, alt=self.alt)
         if self_record is not None:
             self.pad.db.track_record_dependency(self_record)
 
         for id in self.__child_ids:
@@ -156,15 +161,15 @@
         if self._pristine:
             # optimization
             return len(self.__child_ids)
         return super().count()  # type: ignore[no-any-return]
 
     def get(
         self, id: str, page_num: int | None | EllipsisType = Ellipsis
-    ) -> Record | VirtualSourceObject | None:
+    ) -> _DBSourceObject | None:
         # optimization
         if id in self.__child_ids:
             return self._get(id, page_num=page_num)
         return None
 
     def __bool__(self) -> bool:
         if self._pristine:
```

### Comparing `lektorlib-1.2.0/lektorlib/testing.py` & `lektorlib-1.2.1/lektorlib/testing.py`

 * *Files identical despite different names*

### Comparing `lektorlib-1.2.0/pdm_build.py` & `lektorlib-1.2.1/pdm_build.py`

 * *Files identical despite different names*

### Comparing `lektorlib-1.2.0/pyproject.toml` & `lektorlib-1.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -27,24 +27,24 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Framework :: Lektor",
     "Environment :: Plugins",
     "Topic :: Software Development :: Libraries",
 ]
 requires-python = ">=3.7"
-version = "1.2.0"
+version = "1.2.1"
 
 [project.urls]
 Home = "https://github.com/dairiki/lektorlib"
 
 [project.license]
 file = "LICENSE"
 
 [project.readme]
-text = "# Lektorlib\n\n[![PyPI version](https://img.shields.io/pypi/v/lektorlib.svg)](https://pypi.org/project/lektorlib/)\n[![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/lektorlib.svg)](https://pypi.python.org/pypi/lektorlib/)\n[![GitHub license](https://img.shields.io/github/license/dairiki/lektorlib)](https://github.com/dairiki/lektorlib/blob/master/LICENSE)\n[![GitHub Actions (Tests)](https://github.com/dairiki/lektorlib/workflows/Tests/badge.svg)](https://github.com/dairiki/lektorlib)\n[![Trackgit Views](https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/lhaqecdxux7krt01vbsl)](https://trackgit.com)\n\nA few bits which may possibly be useful to developers of [Lektor][] plugins.\n\n## Bits Included\n\n### `lektorlib.query.PrecomputedQuery`\n\nA subclass of `lektor.db.Query` which yields a pre-computed\nsequence of children.\n\nThis is useful in (at least) two circumstances:\n\nFirst, when the children to be queried are virtual source objects,\nthe standard `lektor.db.Query` will not work.  This version will.\n\nSecond, when we would like to generate a query of a pre-computed\nsubset of a resource's children, this prevents intruducing\nunnecessary build dependencies.  If we used a standard query with\na filter applied, it still iterates over all of the parent node’s\nchildren, registering dependencies on all of them.\n\n### `lektorlib.context.disable_dependency_recording`\n\nA python context manager which (temporarily) disables lektor’s\ndependency recording system.\n\n### `lektorlib.recordcache.get_or_create_virtual`\n\nThis function is a helper to streamline the caching of virtual\nsource objects in the lektor record cache.\n\n`Lektor.db.Pad.get()` handles caching for regular records.\nAt present, however, it does not appear that it ever caches\nvirtual source objects, even though its record cache is perfectly\ncapable of doing so.\n\n### `lektorlib.testing.assert_no_dependencies(match=None)`\n\nThis context manager is a testing helper which can be used to\ncheck that no dependencies are recorded with lektor’s dependency\ntracking system.\n\n## Author\n\nJeff Dairiki <dairiki@dairiki.org>\n\n[Lektor]: <https://www.getlektor.com/> \"Lektor Static Content Management System\"\n\n## Changelog\n\n### Release 1.2.0 (2023-06-02)\n\n- Added type annotations\n- Use PDM instead of setuptools to build distribution\n- Configured pre-commit\n- Run black and reorder-python-imports on the code\n\n### Release 1.1.0 (2023-04-20)\n\nFixes for Lektor 3.4 (in pre-release).\n\nWe now test under Lektor 3.3 and Lektor 3.4 (pre-release).\n\n### Release 1.0 (2022-01-28)\n\nDrop support for python < 3.7. Test under python 3.10.\n\n### Release 0.1 (2021-02-05)\n\nNo code changes.\n\nRelease is now classified as \"production/stable\".\n\n### Release 0.1a1 (2020-05-05)\n\nInitial release.\n"
+text = "# Lektorlib\n\n[![PyPI version](https://img.shields.io/pypi/v/lektorlib.svg)](https://pypi.org/project/lektorlib/)\n[![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/lektorlib.svg)](https://pypi.python.org/pypi/lektorlib/)\n[![GitHub license](https://img.shields.io/github/license/dairiki/lektorlib)](https://github.com/dairiki/lektorlib/blob/master/LICENSE)\n[![GitHub Actions (Tests)](https://github.com/dairiki/lektorlib/workflows/Tests/badge.svg)](https://github.com/dairiki/lektorlib)\n[![Trackgit Views](https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/lhaqecdxux7krt01vbsl)](https://trackgit.com)\n\nA few bits which may possibly be useful to developers of [Lektor][] plugins.\n\n## Bits Included\n\n### `lektorlib.query.PrecomputedQuery`\n\nA subclass of `lektor.db.Query` which yields a pre-computed\nsequence of children.\n\nThis is useful in (at least) two circumstances:\n\nFirst, when the children to be queried are virtual source objects,\nthe standard `lektor.db.Query` will not work.  This version will.\n\nSecond, when we would like to generate a query of a pre-computed\nsubset of a resource's children, this prevents intruducing\nunnecessary build dependencies.  If we used a standard query with\na filter applied, it still iterates over all of the parent node’s\nchildren, registering dependencies on all of them.\n\n### `lektorlib.context.disable_dependency_recording`\n\nA python context manager which (temporarily) disables lektor’s\ndependency recording system.\n\n### `lektorlib.recordcache.get_or_create_virtual`\n\nThis function is a helper to streamline the caching of virtual\nsource objects in the lektor record cache.\n\n`Lektor.db.Pad.get()` handles caching for regular records.\nAt present, however, it does not appear that it ever caches\nvirtual source objects, even though its record cache is perfectly\ncapable of doing so.\n\n### `lektorlib.testing.assert_no_dependencies(match=None)`\n\nThis context manager is a testing helper which can be used to\ncheck that no dependencies are recorded with lektor’s dependency\ntracking system.\n\n## Author\n\nJeff Dairiki <dairiki@dairiki.org>\n\n[Lektor]: <https://www.getlektor.com/> \"Lektor Static Content Management System\"\n\n## Changelog\n\n### Release 1.2.1 (2023-06-15)\n\n#### Type Annotations\n\n- Narrow the return type of `lektorlib.recordcache.get_or_create_virtual`.\n- Convert `lektorlib.query.PrecomputedQuery` to a generic type.\n\n### Release 1.2.0 (2023-06-02)\n\n- Added type annotations\n- Use PDM instead of setuptools to build distribution\n- Configured pre-commit\n- Run black and reorder-python-imports on the code\n\n### Release 1.1.0 (2023-04-20)\n\nFixes for Lektor 3.4 (in pre-release).\n\nWe now test under Lektor 3.3 and Lektor 3.4 (pre-release).\n\n### Release 1.0 (2022-01-28)\n\nDrop support for python < 3.7. Test under python 3.10.\n\n### Release 0.1 (2021-02-05)\n\nNo code changes.\n\nRelease is now classified as \"production/stable\".\n\n### Release 0.1a1 (2020-05-05)\n\nInitial release.\n"
 content-type = "text/markdown"
 
 [tool.pdm.version]
 source = "scm"
 
 [tool.pdm.build]
 excludes = [
```

### Comparing `lektorlib-1.2.0/tests/conftest.py` & `lektorlib-1.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lektorlib-1.2.0/tests/test-site/assets/static/style.css` & `lektorlib-1.2.1/tests/test-site/assets/static/style.css`

 * *Files identical despite different names*

### Comparing `lektorlib-1.2.0/tests/test-site/templates/layout.html` & `lektorlib-1.2.1/tests/test-site/templates/layout.html`

 * *Files identical despite different names*

### Comparing `lektorlib-1.2.0/tests/test_context.py` & `lektorlib-1.2.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `lektorlib-1.2.0/tests/test_query.py` & `lektorlib-1.2.1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `lektorlib-1.2.0/tests/test_recordcache.py` & `lektorlib-1.2.1/tests/test_recordcache.py`

 * *Files identical despite different names*

### Comparing `lektorlib-1.2.0/tests/test_testing.py` & `lektorlib-1.2.1/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `lektorlib-1.2.0/tox.ini` & `lektorlib-1.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `lektorlib-1.2.0/PKG-INFO` & `lektorlib-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lektorlib
-Version: 1.2.0
+Version: 1.2.1
 Summary: A few bits which are potentially useful to developers of Lektor plugins
 Keywords: Lektor utilities
 Author-Email: Jeff Dairiki <dairiki@dairiki.org>
 License: Copyright © 2020 Geoffrey T. Dairiki
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
@@ -94,14 +94,21 @@
 
 Jeff Dairiki <dairiki@dairiki.org>
 
 [Lektor]: <https://www.getlektor.com/> "Lektor Static Content Management System"
 
 ## Changelog
 
+### Release 1.2.1 (2023-06-15)
+
+#### Type Annotations
+
+- Narrow the return type of `lektorlib.recordcache.get_or_create_virtual`.
+- Convert `lektorlib.query.PrecomputedQuery` to a generic type.
+
 ### Release 1.2.0 (2023-06-02)
 
 - Added type annotations
 - Use PDM instead of setuptools to build distribution
 - Configured pre-commit
 - Run black and reorder-python-imports on the code
```

