# Comparing `tmp/ilcdlib-0.6.0.tar.gz` & `tmp/ilcdlib-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilcdlib-0.6.0.tar", max compression
+gzip compressed data, was "ilcdlib-0.7.0.tar", max compression
```

## Comparing `ilcdlib-0.6.0.tar` & `ilcdlib-0.7.0.tar`

### file list

```diff
@@ -1,55 +1,57 @@
--rw-r--r--   0        0        0    11357 2023-06-14 09:45:31.524799 ilcdlib-0.6.0/LICENSE
--rw-r--r--   0        0        0     4949 2023-06-14 09:45:31.524799 ilcdlib-0.6.0/README.md
--rw-r--r--   0        0        0     3425 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      837 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/__init__.py
--rw-r--r--   0        0        0      910 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/__main__.py
--rw-r--r--   0        0        0      855 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/__version__.py
--rw-r--r--   0        0        0     2959 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/cli.py
--rw-r--r--   0        0        0    17034 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/common.py
--rw-r--r--   0        0        0     1357 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/const.py
--rw-r--r--   0        0        0   172140 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/data/ilcd_epd_ref.zip
--rw-r--r--   0        0        0     3121 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/dto.py
--rw-r--r--   0        0        0      837 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/__init__.py
--rw-r--r--   0        0        0     6395 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/base_scope_set_reader.py
--rw-r--r--   0        0        0     2665 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/category.py
--rw-r--r--   0        0        0     3052 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/compliance.py
--rw-r--r--   0        0        0     5639 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/contact.py
--rw-r--r--   0        0        0     3648 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/exchage.py
--rw-r--r--   0        0        0     7981 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/flow.py
--rw-r--r--   0        0        0     2748 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/lcia.py
--rw-r--r--   0        0        0     5213 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/material.py
--rw-r--r--   0        0        0     3924 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/pcr.py
--rw-r--r--   0        0        0     3437 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/source.py
--rw-r--r--   0        0        0     3774 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/unit.py
--rw-r--r--   0        0        0      837 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/epd/__init__.py
--rw-r--r--   0        0        0    10064 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/epd/cli.py
--rw-r--r--   0        0        0      837 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/epd/dialect/__init__.py
--rw-r--r--   0        0        0     2596 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/epd/dialect/environdec.py
--rw-r--r--   0        0        0     1329 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/epd/dialect/indata.py
--rw-r--r--   0        0        0     1991 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/epd/dialect/oekobaudat.py
--rw-r--r--   0        0        0     3328 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/epd/factory.py
--rw-r--r--   0        0        0    30739 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/epd/reader.py
--rw-r--r--   0        0        0     1707 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/extension.py
--rw-r--r--   0        0        0     7667 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/http_common.py
--rw-r--r--   0        0        0      837 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/mapping/__init__.py
--rw-r--r--   0        0        0     1900 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/mapping/common.py
--rw-r--r--   0        0        0     1168 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/mapping/compliance.py
--rw-r--r--   0        0        0     1512 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/mapping/flows.py
--rw-r--r--   0        0        0     1892 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/mapping/impacts.py
--rw-r--r--   0        0        0     1651 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/mapping/indicators.py
--rw-r--r--   0        0        0     1212 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/mapping/properties.py
--rw-r--r--   0        0        0     1737 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/mapping/units.py
--rw-r--r--   0        0        0      837 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/medium/__init__.py
--rw-r--r--   0        0        0     7531 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/medium/archive.py
--rw-r--r--   0        0        0     6496 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/medium/soda4lca.py
--rw-r--r--   0        0        0        0 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/py.typed
--rw-r--r--   0        0        0     1435 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/reference_data.py
--rw-r--r--   0        0        0      837 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/sanitizing/__init__.py
--rw-r--r--   0        0        0     1705 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/sanitizing/domain.py
--rw-r--r--   0        0        0     1336 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/sanitizing/phone.py
--rw-r--r--   0        0        0      837 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/soda4lca/__init__.py
--rw-r--r--   0        0        0     8855 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/soda4lca/api_client.py
--rw-r--r--   0        0        0     1206 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/type.py
--rw-r--r--   0        0        0     3329 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/utils.py
--rw-r--r--   0        0        0     2399 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/xml_parser.py
--rw-r--r--   0        0        0     6055 1970-01-01 00:00:00.000000 ilcdlib-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-15 12:34:54.790989 ilcdlib-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4949 2023-06-15 12:34:54.790989 ilcdlib-0.7.0/README.md
+-rw-r--r--   0        0        0     3453 2023-06-15 12:34:54.794989 ilcdlib-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-06-15 12:34:54.794989 ilcdlib-0.7.0/src/ilcdlib/__init__.py
+-rw-r--r--   0        0        0      910 2023-06-15 12:34:54.794989 ilcdlib-0.7.0/src/ilcdlib/__main__.py
+-rw-r--r--   0        0        0      855 2023-06-15 12:34:54.794989 ilcdlib-0.7.0/src/ilcdlib/__version__.py
+-rw-r--r--   0        0        0     2959 2023-06-15 12:34:54.794989 ilcdlib-0.7.0/src/ilcdlib/cli.py
+-rw-r--r--   0        0        0    17041 2023-06-15 12:34:54.794989 ilcdlib-0.7.0/src/ilcdlib/common.py
+-rw-r--r--   0        0        0     1773 2023-06-15 12:34:54.794989 ilcdlib-0.7.0/src/ilcdlib/const.py
+-rw-r--r--   0        0        0   172140 2023-06-15 12:34:54.794989 ilcdlib-0.7.0/src/ilcdlib/data/ilcd_epd_ref.zip
+-rw-r--r--   0        0        0     4474 2023-06-15 12:34:54.794989 ilcdlib-0.7.0/src/ilcdlib/dto.py
+-rw-r--r--   0        0        0      837 2023-06-15 12:34:54.794989 ilcdlib-0.7.0/src/ilcdlib/entity/__init__.py
+-rw-r--r--   0        0        0     6375 2023-06-15 12:34:54.794989 ilcdlib-0.7.0/src/ilcdlib/entity/base_scope_set_reader.py
+-rw-r--r--   0        0        0     2665 2023-06-15 12:34:54.794989 ilcdlib-0.7.0/src/ilcdlib/entity/category.py
+-rw-r--r--   0        0        0     3052 2023-06-15 12:34:54.794989 ilcdlib-0.7.0/src/ilcdlib/entity/compliance.py
+-rw-r--r--   0        0        0     6003 2023-06-15 12:34:54.794989 ilcdlib-0.7.0/src/ilcdlib/entity/contact.py
+-rw-r--r--   0        0        0     3638 2023-06-15 12:34:54.794989 ilcdlib-0.7.0/src/ilcdlib/entity/exchage.py
+-rw-r--r--   0        0        0     7981 2023-06-15 12:34:54.794989 ilcdlib-0.7.0/src/ilcdlib/entity/flow.py
+-rw-r--r--   0        0        0     2738 2023-06-15 12:34:54.794989 ilcdlib-0.7.0/src/ilcdlib/entity/lcia.py
+-rw-r--r--   0        0        0     5213 2023-06-15 12:34:54.794989 ilcdlib-0.7.0/src/ilcdlib/entity/material.py
+-rw-r--r--   0        0        0     3930 2023-06-15 12:34:54.794989 ilcdlib-0.7.0/src/ilcdlib/entity/pcr.py
+-rw-r--r--   0        0        0     3437 2023-06-15 12:34:54.794989 ilcdlib-0.7.0/src/ilcdlib/entity/source.py
+-rw-r--r--   0        0        0     3774 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/entity/unit.py
+-rw-r--r--   0        0        0     3331 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/entity/validation.py
+-rw-r--r--   0        0        0      837 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/epd/__init__.py
+-rw-r--r--   0        0        0    10064 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/epd/cli.py
+-rw-r--r--   0        0        0      837 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/epd/dialect/__init__.py
+-rw-r--r--   0        0        0     2596 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/epd/dialect/environdec.py
+-rw-r--r--   0        0        0     1329 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/epd/dialect/indata.py
+-rw-r--r--   0        0        0     2003 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/epd/dialect/oekobaudat.py
+-rw-r--r--   0        0        0     3328 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/epd/factory.py
+-rw-r--r--   0        0        0    31787 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/epd/reader.py
+-rw-r--r--   0        0        0     2050 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/extension.py
+-rw-r--r--   0        0        0     7667 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/http_common.py
+-rw-r--r--   0        0        0      837 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/mapping/__init__.py
+-rw-r--r--   0        0        0     1900 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/mapping/common.py
+-rw-r--r--   0        0        0     1168 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/mapping/compliance.py
+-rw-r--r--   0        0        0     1512 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/mapping/flows.py
+-rw-r--r--   0        0        0     1892 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/mapping/impacts.py
+-rw-r--r--   0        0        0     1651 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/mapping/indicators.py
+-rw-r--r--   0        0        0     1212 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/mapping/properties.py
+-rw-r--r--   0        0        0     1737 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/mapping/units.py
+-rw-r--r--   0        0        0      837 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/medium/__init__.py
+-rw-r--r--   0        0        0     7531 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/medium/archive.py
+-rw-r--r--   0        0        0     6496 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/medium/soda4lca.py
+-rw-r--r--   0        0        0        0 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/py.typed
+-rw-r--r--   0        0        0     1435 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/reference_data.py
+-rw-r--r--   0        0        0      837 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/sanitizing/__init__.py
+-rw-r--r--   0        0        0     1705 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/sanitizing/domain.py
+-rw-r--r--   0        0        0     1336 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/sanitizing/phone.py
+-rw-r--r--   0        0        0     1122 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/sanitizing/text.py
+-rw-r--r--   0        0        0      837 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/soda4lca/__init__.py
+-rw-r--r--   0        0        0     8856 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/soda4lca/api_client.py
+-rw-r--r--   0        0        0     1206 2023-06-15 12:34:54.798989 ilcdlib-0.7.0/src/ilcdlib/type.py
+-rw-r--r--   0        0        0     3329 2023-06-15 12:34:54.802989 ilcdlib-0.7.0/src/ilcdlib/utils.py
+-rw-r--r--   0        0        0     2399 2023-06-15 12:34:54.802989 ilcdlib-0.7.0/src/ilcdlib/xml_parser.py
+-rw-r--r--   0        0        0     6055 1970-01-01 00:00:00.000000 ilcdlib-0.7.0/PKG-INFO
```

### Comparing `ilcdlib-0.6.0/LICENSE` & `ilcdlib-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/README.md` & `ilcdlib-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/pyproject.toml` & `ilcdlib-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ilcdlib"
-version = "0.6.0"
+version = "0.7.0"
 license = "Apache-2.0"
 description = "A toolkit for reading and writing ILCD format and it's derivatives"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <support@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/ilcdlib"
 keywords = []
 classifiers = [
@@ -22,15 +22,15 @@
 [tool.poetry.scripts]
 ilcdtool = { callable = "ilcdlib:cli.entrypoint", extras = ["cli"] }
 
 [tool.poetry.dependencies]
 python = "^3.11"
 urllib3 = { version = ">=1.26.16,<2.0.0" }
 requests = { version = ">=2.1.0,<3.0.0" }
-openepd = { version = ">=0.10.0,<1.0.0" }
+openepd = { version = ">=0.11.0,<1.0.0" }
 
 # Optional dependencies
 lxml = { version = "~=4.9.2", optional = true }
 cli-rack = { version = ">=1.0.6", optional = true }
 
 [tool.poetry.dev-dependencies]
 # Unit tests
@@ -59,15 +59,15 @@
 types-urllib3 = ">=1.26.2"
 
 [tool.poetry.extras]
 lxml = ["lxml"]
 cli = ["cli-rack"]
 
 [tool.commitizen]
-version = "0.6.0"
+version = "0.7.0"
 bump_version = "bump: version $current_version → $new_version"
 update_changelog_on_bump = true
 pre_bump_hooks = []
 version_files = [
     "pyproject.toml",
     "src/ilcdlib/__version__.py",
 ]
@@ -128,13 +128,14 @@
 show_error_codes = true
 ignore_errors = false
 warn_return_any = false
 disallow_any_generics = false
 pretty = true
 mypy_path = "$MYPY_CONFIG_FILE_DIR/stubs"
 exclude = ["test_.*\\.py$", ]
+plugins = ["pydantic.mypy"]
 
 [[tool.mypy.overrides]]
 # External libs which doesn't have type hints (py.typed marker)
 module = ["cli_rack.*"]
 ignore_missing_imports = true
 follow_imports = "skip"
```

### Comparing `ilcdlib-0.6.0/src/ilcdlib/__init__.py` & `ilcdlib-0.7.0/src/ilcdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/__main__.py` & `ilcdlib-0.7.0/src/ilcdlib/__main__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/__version__.py` & `ilcdlib-0.7.0/src/ilcdlib/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "0.6.0"
+VERSION = "0.7.0"
```

### Comparing `ilcdlib-0.6.0/src/ilcdlib/cli.py` & `ilcdlib-0.7.0/src/ilcdlib/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/common.py` & `ilcdlib-0.7.0/src/ilcdlib/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,19 +19,18 @@
 #
 import abc
 import datetime
 from typing import IO, Literal, Self, Sequence, TextIO, overload
 
 from openepd.model.epd import Epd
 from openepd.model.lcia import Impacts
-from openepd.model.org import Org
 from openepd.model.pcr import Pcr
 
 from ilcdlib.const import IlcdDatasetType
-from ilcdlib.dto import IlcdReference
+from ilcdlib.dto import IlcdReference, OpenEpdIlcdOrg
 from ilcdlib.reference_data import get_ilcd_epd_reference_data_provider
 from ilcdlib.type import LangDef, LocalizedStr
 from ilcdlib.xml_parser import T_ET, XmlParser
 
 XmlPath = str | tuple[str, ...] | list[str]
 
 
@@ -380,15 +379,17 @@
         return self.data_provider.get_entity_stream(ref.entity_type, ref.entity_id, ref.entity_version, binary=True)
 
 
 class OpenEpdContactSupportReader(metaclass=abc.ABCMeta):
     """Base class for adding OpenEPD export support."""
 
     @abc.abstractmethod
-    def to_openepd_org(self, lang: LangDef, base_url: str | None = None, provider_domain: str | None = None) -> Org:
+    def to_openepd_org(
+        self, lang: LangDef, base_url: str | None = None, provider_domain: str | None = None
+    ) -> OpenEpdIlcdOrg:
         """Read as openEPD Org object."""
         pass
 
 
 class OpenEpdPcrSupportReader(metaclass=abc.ABCMeta):
     """Base class for adding openEPD export support."""
```

### Comparing `ilcdlib-0.6.0/src/ilcdlib/const.py` & `ilcdlib-0.7.0/src/ilcdlib/mapping/properties.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,29 +13,20 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from enum import StrEnum
+from ilcdlib.mapping.common import SimpleDataMapper
 
-ILCD_IDENTIFICATION: tuple[str] = ("ILCD_EPD",)
-PDF_ATTACHMENT = "PDF"
 
+class PropertiesUUIDMapper(SimpleDataMapper[str]):
+    """A data mapper that maps units ILCD UUIDs to standartized names."""
 
-class IlcdContactClass(StrEnum):
-    """Enumeration of ILCD contact classes."""
+    DATABASE = {
+        "7e18d0ad-e78e-47a0-8e96-1c0a581902e2": "mass",
+        "838aaa23-0117-11db-92e3-0800200c9a66": "length",
+    }
 
-    Person = "Persons"
-    Company = "Organisations"
 
-
-class IlcdDatasetType(StrEnum):
-    """Enumeration of ILCD datasets."""
-
-    Contacts = "contact data set"
-    Sources = "source data set"
-    Flows = "flow data set"
-    Processes = "process data set"
-    UnitGroups = "unit group data set"
-    FlowProperty = "flow property data set"
+default_properties_uuid_mapper = PropertiesUUIDMapper()
```

### Comparing `ilcdlib-0.6.0/src/ilcdlib/data/ilcd_epd_ref.zip` & `ilcdlib-0.7.0/src/ilcdlib/data/ilcd_epd_ref.zip`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/dto.py` & `ilcdlib-0.7.0/src/ilcdlib/dto.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,16 +16,19 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from dataclasses import dataclass
 from typing import Any, Generic, NamedTuple
 
+from openepd.model.base import BaseOpenEpdSchema
 from openepd.model.org import Org
+import pydantic as pyd
 
+from ilcdlib.const import IlcdTypeOfReview
 from ilcdlib.utils import T
 
 
 class IlcdReference(NamedTuple):
     """A reference to an ILCD entity."""
 
     entity_type: str
@@ -97,16 +100,47 @@
 
 class ProcessSearchResponse(BaseSearchResponse[ProcessBasicInfo]):
     """A search response for processes."""
 
     pass
 
 
+class IlcdContactInfo(BaseOpenEpdSchema):
+    """Contact information extracted from ILCD contact."""
+
+    contact_person: str | None = pyd.Field(description="Name of the contact person", example="John Doe", default=None)
+    email: pyd.EmailStr | None = pyd.Field(description="Email", example="contact@c-change-labs.com", default=None)
+    phone: str | None = pyd.Field(description="Phone number", example="+15263327352", default=None)
+    website: pyd.AnyUrl | None = pyd.Field(
+        description="Url of the website", example="http://buildingtransparency.org", default=None
+    )
+    address: str | None = pyd.Field(description="Address", example="123 Main St, San Francisco, CA 94105", default=None)
+
+
+class OpenEpdIlcdOrg(Org):
+    """Org object with ILCD specific extension."""
+
+    def get_contact(self) -> IlcdContactInfo | None:
+        """Return ILCD contact information from extension field if any."""
+        from ilcdlib.extension import IlcdOrgExtension
+
+        ext = self.get_ext(IlcdOrgExtension)
+        return ext.contact if ext else None
+
+
 @dataclass(kw_only=True)
 class ComplianceDto:
     """Basic information about a Compliance."""
 
     uuid: str
     short_name: str | None
     name: str | None
     link: str | None
-    issuer: Org | None
+    issuer: OpenEpdIlcdOrg | None
+
+
+@dataclass(kw_only=True)
+class ValidationDto:
+    """Basic information about a Compliance."""
+
+    validation_type: IlcdTypeOfReview | None
+    org: OpenEpdIlcdOrg
```

### Comparing `ilcdlib-0.6.0/src/ilcdlib/entity/__init__.py` & `ilcdlib-0.7.0/src/ilcdlib/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/entity/base_scope_set_reader.py` & `ilcdlib-0.7.0/src/ilcdlib/entity/base_scope_set_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             unit_name = self._get_text(
                 el, ("common:other", "epd2013:referenceToUnitGroupDataSet", "common:shortDescription")
             )
         if unit_name is None:
             return None
         # Stages
         scopes = self.__extract_scopes(el, unit_name, scenario_names)
-        return ScopeSet.construct(**scopes), impact_name  # type: ignore
+        return ScopeSet(**scopes), impact_name  # type: ignore
 
     def __extract_scopes(
         self, el: T_ET.Element, unit_name: str, scenario_names: dict[str, str]
     ) -> dict[str, Measurement | dict | list]:
         """Extract all scopes from scope set element."""
         ext: dict[str, Measurement] = {}
         scopes: dict[str, Measurement | dict | list] = {"ext": ext}
@@ -130,15 +130,15 @@
                 return None
 
             scenarios = scopes.get("C_scenarios") or list()
             scenario: dict[str, Measurement | str] = dict(
                 name=scenario_names[scenario_name],
             )
             scenario[module_name] = measurement
-            scenarios.append(EolScenario.construct(**scenario))  # type: ignore
+            scenarios.append(EolScenario(**scenario))  # type: ignore
             scopes["C_scenarios"] = scenarios
 
     @staticmethod
     def __map_module_name(module_name: str | None) -> str | None:
         if module_name == "A1-A3":
             return "A1A2A3"
         return module_name
```

### Comparing `ilcdlib-0.6.0/src/ilcdlib/entity/category.py` & `ilcdlib-0.7.0/src/ilcdlib/entity/category.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/entity/compliance.py` & `ilcdlib-0.7.0/src/ilcdlib/entity/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/entity/contact.py` & `ilcdlib-0.7.0/src/ilcdlib/entity/contact.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,20 +13,22 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from openepd.model.org import Contact, Org
+
+from openepd.model.common import Location
 
 from ilcdlib.common import BaseIlcdMediumSpecificReader, IlcdXmlReader, OpenEpdContactSupportReader
 from ilcdlib.const import IlcdContactClass
-from ilcdlib.dto import IlcdReference
-from ilcdlib.sanitizing.domain import domain_from_url
+from ilcdlib.dto import IlcdContactInfo, IlcdReference, OpenEpdIlcdOrg
+from ilcdlib.extension import IlcdOrgExtension
+from ilcdlib.sanitizing.domain import cleanup_website, domain_from_url
 from ilcdlib.sanitizing.phone import cleanup_phone
 from ilcdlib.type import LangDef
 from ilcdlib.utils import create_openepd_attachments, none_throws, provider_domain_name_from_url
 from ilcdlib.xml_parser import T_ET
 
 
 class IlcdContactReader(OpenEpdContactSupportReader, IlcdXmlReader):
@@ -104,25 +106,32 @@
 
     def get_address(self) -> str | None:
         """Get the address of the contact described by this data set."""
         return self._get_text(
             self._entity, ("contact:contactInformation", "contact:dataSetInformation", "contact:contactAddress")
         )
 
-    def to_openepd_org(self, lang: LangDef, base_url: str | None = None, provider_domain: str | None = None) -> Org:
+    def to_openepd_org(
+        self, lang: LangDef, base_url: str | None = None, provider_domain: str | None = None
+    ) -> OpenEpdIlcdOrg:
         """Convert this data set to an OpenEPD org object."""
-        open_epd_contact = Contact.construct(
-            email=self.get_email(),
+        open_epd_contact = IlcdContactInfo(
+            email=self.get_email(),  # type: ignore
             phone=cleanup_phone(self.get_phone()),
-            website=self.get_website(),
+            website=cleanup_website(self.get_website()),  # type: ignore
             address=self.get_address(),
         )
-        org = Org.construct(
+        org = OpenEpdIlcdOrg(
             name=self.get_name(lang),
-            web_domain=domain_from_url(self.get_website()),
-            contacts=open_epd_contact if open_epd_contact.has_values() else None,
-            attachments=create_openepd_attachments(self.get_own_reference(), base_url) if base_url else None,
+            web_domain=domain_from_url(self.get_website()),  # type: ignore
+            attachments=create_openepd_attachments(self.get_own_reference(), base_url)
+            if base_url
+            else None,  # type: ignore
         )
         if provider_domain is None:
             provider_domain = provider_domain_name_from_url(base_url)
+        if open_epd_contact.address:
+            org.hq_location = Location(address=open_epd_contact.address)
         org.set_alt_id(provider_domain, self.get_uuid())
+        if open_epd_contact.has_values():
+            org.set_ext(IlcdOrgExtension(contact=open_epd_contact))
         return org
```

### Comparing `ilcdlib-0.6.0/src/ilcdlib/entity/exchage.py` & `ilcdlib-0.7.0/src/ilcdlib/entity/exchage.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,8 +83,8 @@
                     ext=ext,
                     mapper=mapper,
                     scenario_names=scenario_names,
                 )
 
         if len(ext) == 0:
             del scope_sets["ext"]
-        return scope_set_type.construct(**scope_sets)  # type: ignore
+        return scope_set_type(**scope_sets)  # type: ignore
```

### Comparing `ilcdlib-0.6.0/src/ilcdlib/entity/flow.py` & `ilcdlib-0.7.0/src/ilcdlib/entity/flow.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/entity/lcia.py` & `ilcdlib-0.7.0/src/ilcdlib/entity/lcia.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                 scope_set_dict=impacts,
                 ext=ext,
                 mapper=self.impact_mapper,
                 scenario_names=scenario_names,
             )
         if len(ext) == 0:
             del impacts["ext"]
-        return ImpactSet.construct(**impacts)  # type: ignore
+        return ImpactSet(**impacts)  # type: ignore
 
     def to_openepd_impacts(
         self,
         scenario_names: dict[str, str],
         lcia_method: str | None = None,
         base_url: str | None = None,
         provider_domain: str | None = None,
```

### Comparing `ilcdlib-0.6.0/src/ilcdlib/entity/material.py` & `ilcdlib-0.7.0/src/ilcdlib/entity/material.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/entity/pcr.py` & `ilcdlib-0.7.0/src/ilcdlib/entity/pcr.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,18 +75,18 @@
         return [el.attrib["uri"] for el in els if el.attrib and "uri" in el.attrib]
 
     def to_openepd_pcr(self, lang: LangDef, base_url: str | None = None, provider_domain: str | None = None) -> Pcr:
         """Read as OpenEPD Pcr object."""
         issuer_reader = self.get_reference_to_contact_reader()
         issuer = issuer_reader.to_openepd_org(lang) if issuer_reader is not None else None
         reference = self.get_own_reference()
-        pcr = Pcr.construct(
+        pcr = Pcr(
             name=self.get_name(lang),
             issuer=issuer,
-            attachments=create_openepd_attachments(reference, base_url) if base_url else None,
+            attachments=create_openepd_attachments(reference, base_url) if base_url else None,  # type: ignore
         )
         if provider_domain is None:
             provider_domain = provider_domain_name_from_url(base_url)
         digital_files = self.get_references_to_digital_files()
         if len(digital_files) > 0 and reference is not None:
             pdf_url = self.data_provider.resolve_entity_url(reference, digital_files[0])
             pcr.set_attachment_if_any(const.PDF_ATTACHMENT, pdf_url)
```

### Comparing `ilcdlib-0.6.0/src/ilcdlib/entity/source.py` & `ilcdlib-0.7.0/src/ilcdlib/entity/source.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/entity/unit.py` & `ilcdlib-0.7.0/src/ilcdlib/entity/unit.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/epd/__init__.py` & `ilcdlib-0.7.0/src/ilcdlib/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/epd/cli.py` & `ilcdlib-0.7.0/src/ilcdlib/epd/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/epd/dialect/__init__.py` & `ilcdlib-0.7.0/src/ilcdlib/epd/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/epd/dialect/environdec.py` & `ilcdlib-0.7.0/src/ilcdlib/epd/dialect/environdec.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/epd/dialect/indata.py` & `ilcdlib-0.7.0/src/ilcdlib/epd/dialect/indata.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/epd/dialect/oekobaudat.py` & `ilcdlib-0.7.0/src/ilcdlib/epd/dialect/oekobaudat.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     """Reader for EPDs in the Oekobau.DAT specific ILCD XML format."""
 
     @classmethod
     def is_known_url(cls, url: str) -> bool:
         """Return whether the URL recognized as a known Environdec URL."""
         return "oekobaudat" in url.lower()
 
-    def _product_classes_to_openepd(self, classes: dict[str, list[ProductClassDef]]) -> dict[str, str]:
+    def _product_classes_to_openepd(self, classes: dict[str, list[ProductClassDef]]) -> dict[str, list[str] | str]:
         """
         Convert the product classes to OpenEPD format.
 
         The Oekobau.DAT format according to openEPD is a string containing full id and
         the name of the most specific class. Example: "1.1.01 Cement"
         """
         result = super()._product_classes_to_openepd(classes)
```

### Comparing `ilcdlib-0.6.0/src/ilcdlib/epd/factory.py` & `ilcdlib-0.7.0/src/ilcdlib/epd/factory.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/epd/reader.py` & `ilcdlib-0.7.0/src/ilcdlib/epd/reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,31 +19,32 @@
 #
 import datetime
 from typing import IO, Sequence, Type
 
 from openepd.model.common import Amount, Measurement
 from openepd.model.epd import Epd
 from openepd.model.lcia import Impacts, ImpactSet, OutputFlowSet, ResourceUseSet
-from openepd.model.org import Org
 from openepd.model.specs import Specs
 from openepd.model.standard import Standard
 
 from ilcdlib import const
 from ilcdlib.common import BaseIlcdMediumSpecificReader, IlcdXmlReader, OpenEpdEdpSupportReader
-from ilcdlib.const import IlcdDatasetType
-from ilcdlib.dto import ComplianceDto, IlcdReference, ProductClassDef
+from ilcdlib.const import IlcdDatasetType, IlcdTypeOfReview
+from ilcdlib.dto import ComplianceDto, IlcdReference, OpenEpdIlcdOrg, ProductClassDef, ValidationDto
 from ilcdlib.entity.compliance import IlcdComplianceListReader
 from ilcdlib.entity.contact import IlcdContactReader
 from ilcdlib.entity.exchage import IlcdExchangesReader
 from ilcdlib.entity.flow import IlcdExchangeDto, IlcdFlowReader
 from ilcdlib.entity.lcia import IlcdLciaResultsReader
 from ilcdlib.entity.material import MatMlMaterial
 from ilcdlib.entity.pcr import IlcdPcrReader
-from ilcdlib.extension import Ec3EpdExtension, IlcdEpdExtension
+from ilcdlib.entity.validation import IlcdValidationListReader
+from ilcdlib.extension import IlcdEpdExtension
 from ilcdlib.mapping.compliance import StandardNameToLCIAMethodMapper, default_standard_names_to_lcia_mapper
+from ilcdlib.sanitizing.text import trim_text
 from ilcdlib.type import LangDef
 from ilcdlib.utils import (
     MarkdownSectionBuilder,
     create_ext,
     create_openepd_attachments,
     none_throws,
     provider_domain_name_from_url,
@@ -62,23 +63,25 @@
         contact_reader_cls: Type[IlcdContactReader] = IlcdContactReader,
         pcr_reader_cls: Type[IlcdPcrReader] = IlcdPcrReader,
         flow_reader_cls: Type[IlcdFlowReader] = IlcdFlowReader,
         lcia_results_reader_cls: Type[IlcdLciaResultsReader] = IlcdLciaResultsReader,
         exchanges_reader_cls: Type[IlcdExchangesReader] = IlcdExchangesReader,
         compliance_reader_cls: Type[IlcdComplianceListReader] = IlcdComplianceListReader,
         standard_names_to_lcia_mapper: StandardNameToLCIAMethodMapper = default_standard_names_to_lcia_mapper,
+        validation_reader_cls: Type[IlcdValidationListReader] = IlcdValidationListReader,
     ):
         super().__init__(data_provider)
         self.contact_reader_cls = contact_reader_cls
         self.pcr_reader_cls = pcr_reader_cls
         self.flow_reader_cls = flow_reader_cls
         self.lcia_results_reader_cls = lcia_results_reader_cls
         self.compliance_reader_cls = compliance_reader_cls
         self.exchanges_reader_cls = exchanges_reader_cls
         self.standard_names_to_lcia_mapper = standard_names_to_lcia_mapper
+        self.validation_reader_cls = validation_reader_cls
         if epd_process_id is None:
             entities = data_provider.list_entities(IlcdDatasetType.Processes)
             self.__epd_entity_ref = entities[0]
         else:
             self.__epd_entity_ref = IlcdReference(IlcdDatasetType.Processes, epd_process_id, epd_version)
         self.epd_el_tree = self.get_xml_tree(*self.__epd_entity_ref, allow_static_datasets=False)
         self.post_init()
@@ -299,26 +302,24 @@
         )
 
         if el is None:
             return None
 
         return el.attrib.get("location") if el.attrib else None
 
-    def get_external_verifier_reader(self) -> IlcdContactReader | None:
+    def get_validation_reader(self) -> IlcdValidationListReader | None:
         """Return the reader for the reviewer."""
-        element = self._get_external_tree(
+        element = self._get_el(
             self.epd_el_tree,
             (
                 "process:modellingAndValidation",
                 "process:validation",
-                "process:review",
-                "common:referenceToNameOfReviewerAndInstitution",
             ),
         )
-        return self.contact_reader_cls(element, self.data_provider) if element is not None else None
+        return self.validation_reader_cls(element, self.data_provider) if element is not None else None
 
     def get_manufacturer_reader(self) -> IlcdContactReader | None:
         """Return the reader for the manufacturer."""
         element = self._get_external_tree(
             self.epd_el_tree,
             (
                 "process:administrativeInformation",
@@ -360,15 +361,15 @@
                 "process:administrativeInformation",
                 "process:dataEntryBy",
                 "common:referenceToPersonOrEntityEnteringTheData",
             ),
         )
         return self.contact_reader_cls(element, self.data_provider) if element is not None else None
 
-    def get_data_entry_by(self, lang: LangDef, base_url: str | None = None) -> Org | None:
+    def get_data_entry_by(self, lang: LangDef, base_url: str | None = None) -> OpenEpdIlcdOrg | None:
         """Return the data entry by org."""
         data_entry_by_reader = self.get_data_entry_by_reader()
         return data_entry_by_reader.to_openepd_org(lang, base_url) if data_entry_by_reader else None
 
     def get_compliance_reader(self) -> IlcdComplianceListReader | None:
         """Return the reader for the standard included in compliance declarations."""
         element = self._get_el(
@@ -388,23 +389,42 @@
         return reader.get_compliances(lang, base_url)
 
     def get_openepd_compliance(self, lang: LangDef, base_url: str | None = None) -> list[Standard]:
         """Return list of OpenEPD Standards."""
         result = []
         for compliance in self.get_compliance_declarations(lang, base_url):
             result.append(
-                Standard.construct(
-                    short_name=compliance.short_name,
+                Standard(
+                    short_name=none_throws(compliance.short_name),
                     name=compliance.name,
-                    link=compliance.link,  # FIXME: incompatible type "Optional[str]"; expected "Optional[AnyUrl]"
+                    link=compliance.link,  # type: ignore
                     issuer=compliance.issuer,
                 )
             )
         return result
 
+    def get_ilcd_validations(
+        self, lang: LangDef, base_url: str | None = None, provider_domain: str | None = None
+    ) -> list[ValidationDto]:
+        """Return list of all verifiers."""
+        reader = self.get_validation_reader()
+        if reader is None:
+            return []
+        return reader.get_validations(lang, base_url, provider_domain)
+
+    def get_third_party_verifier(self, validations: list[ValidationDto]) -> OpenEpdIlcdOrg | None:
+        """Return first third party verifier."""
+        for verifier in validations:
+            if verifier.validation_type in (
+                IlcdTypeOfReview.IndependentExternalReview,
+                IlcdTypeOfReview.AccreditedThirdPartyReview,
+            ):
+                return verifier.org
+        return None
+
     def get_pcr_reader(self) -> IlcdPcrReader | None:
         """Return the reader for the PCR."""
         element = self._get_external_tree(
             self.epd_el_tree,
             (
                 "process:modellingAndValidation",
                 "process:LCIMethodAndAllocation",
@@ -601,16 +621,16 @@
     def get_output_flows(self, scenario_names: dict[str, str]) -> OutputFlowSet | None:
         """Return output flows."""
         reader = self.get_exchanges_reader()
         if reader is None:
             return None
         return reader.get_output_flows(scenario_names)
 
-    def _product_classes_to_openepd(self, classes: dict[str, list[ProductClassDef]]) -> dict[str, str]:
-        result: dict[str, str] = {}
+    def _product_classes_to_openepd(self, classes: dict[str, list[ProductClassDef]]) -> dict[str, list[str] | str]:
+        result: dict[str, list[str] | str] = {}
         for classification_name, class_defs in classes.items():
             if len(class_defs) > 0:
                 result[classification_name] = (
                     (class_defs[-1].id or "") + " " + " / ".join([none_throws(x.name) for x in class_defs])
                 ).strip()
         return result
 
@@ -629,20 +649,14 @@
         )
         publisher_reader = self.get_publisher_reader()
         publisher = publisher_reader.to_openepd_org(lang, base_url, provider_domain) if publisher_reader else None
         program_operator_reader = self.get_program_operator_reader()
         program_operator = (
             program_operator_reader.to_openepd_org(lang, base_url, provider_domain) if program_operator_reader else None
         )
-        external_verifier_reader = self.get_external_verifier_reader()
-        external_verifier = (
-            external_verifier_reader.to_openepd_org(lang, base_url, provider_domain)
-            if external_verifier_reader
-            else None
-        )
         pcr_reader = self.get_pcr_reader()
         pcr = pcr_reader.to_openepd_pcr(lang, base_url) if pcr_reader else None
         declared_unit = self.get_declared_unit()
         quantitative_props = self.get_quantitative_product_props_str(lang)
         own_ref = self.get_own_reference()
         product_name = self.get_product_name(lang)
         if product_name and quantitative_props:
@@ -666,31 +680,36 @@
         lcia_method: str | None = None
         for c in compliance:
             mapped = self.standard_names_to_lcia_mapper.map(c.short_name, None)
             if mapped:
                 lcia_method = mapped
                 break
 
-        epd = Epd.construct(
-            doctype="openEPD",
+        epd_developer = self.get_data_entry_by(lang, base_url)
+        epd_developer_contact = epd_developer.get_contact() if epd_developer else None
+        ilcd_validations = self.get_ilcd_validations(lang, base_url, provider_domain)
+        epd = Epd(
+            doctype="OpenEPD",
             language=lang_code,
-            attachments=create_openepd_attachments(own_ref, base_url) if base_url else None,
-            declaration_url=own_ref.to_url(base_url) if own_ref and base_url else None,
+            attachments=create_openepd_attachments(own_ref, base_url) if base_url else None,  # type: ignore
+            declaration_url=own_ref.to_url(base_url) if own_ref and base_url else None,  # type: ignore
             product_name=product_name,
-            product_description=self.get_product_description(lang),
-            date_published=self.get_date_published(),
+            product_description=trim_text(self.get_product_description(lang), 2000, ellipsis="..."),
+            date_of_issue=self.get_date_published(),
             valid_until=self.get_validity_ends_date(),
             program_operator_doc_id=self.get_program_operator_id(),
             manufacturer=manufacturer,
+            epd_developer=epd_developer,
+            epd_developer_email=epd_developer_contact.email if epd_developer_contact else None,
             program_operator=program_operator,
             product_classes=self._product_classes_to_openepd(self.get_product_classes()),
             manufacturing_description=self.get_technology_description(lang),
             product_usage_description=self.get_technological_applicability(lang),
             lca_discussion=self.get_lca_discussion(lang),
-            third_party_verifier=external_verifier,
+            third_party_verifier=self.get_third_party_verifier(ilcd_validations),
             pcr=pcr,
             declared_unit=declared_unit,
             impacts=self.get_impacts(scenario_names, lca_method=lcia_method),
             resource_uses=self.get_resource_uses(scenario_names),
             output_flows=self.get_output_flows(scenario_names),
             specs=specs,
             compliance=compliance,
@@ -702,21 +721,19 @@
         epd.set_attachment_if_any(const.PDF_ATTACHMENT, pdf_url)
 
         ilcd_ext = IlcdEpdExtension(
             dataset_type=self.get_dataset_type(),
             dataset_version=self.get_version(),
             dataset_uuid=self.get_uuid(),
             production_location=self.get_production_location(),
+            epd_verifiers=ilcd_validations,
         )
-        ec3_ext = Ec3EpdExtension.construct(
-            epd_developer=self.get_data_entry_by(lang, base_url),
-            epd_publisher=publisher,
-        )
+        if publisher:
+            ilcd_ext.epd_publishers.append(publisher)
         epd.set_ext(ilcd_ext)
-        epd.set_ext(ec3_ext)
         return epd
 
     @classmethod
     def is_known_url(cls, url: str) -> bool:
         """
         Return whether the URL recognized by this particular reader.
```

### Comparing `ilcdlib-0.6.0/src/ilcdlib/extension.py` & `ilcdlib-0.7.0/src/ilcdlib/extension.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,36 +14,40 @@
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.model.base import OpenEpdExtension
-from openepd.model.org import Org
+import pydantic as pyd
 
 from ilcdlib import const
+from ilcdlib.dto import IlcdContactInfo, OpenEpdIlcdOrg, ValidationDto
 
 
 class IlcdEpdExtension(OpenEpdExtension):
     """An ILCD extension for OpenEPD Epd object."""
 
     dataset_type: str | None = None
     dataset_version: str | None = None
     dataset_uuid: str | None = None
     production_location: str | None = None
+    epd_publishers: list[OpenEpdIlcdOrg] = pyd.Field(default_factory=list, description="List of EPD publishers")
+    epd_verifiers: list[ValidationDto] = pyd.Field(
+        default_factory=list, description="List of EPD verifiers (both, external and internal)"
+    )
 
     @classmethod
     def get_extension_name(cls) -> str:
         """Return the name of the extension to be used as a key in ext dict."""
         return const.ILCD_IDENTIFICATION[0]
 
 
-class Ec3EpdExtension(OpenEpdExtension):
-    """An EC3 extension for OpenEPD Epd object."""
+class IlcdOrgExtension(OpenEpdExtension):
+    """Extension to the Org object to store ILCD specific information."""
 
-    epd_publisher: Org | None = None
-    epd_developer: Org | None = None
+    contact: IlcdContactInfo | None = None
 
     @classmethod
     def get_extension_name(cls) -> str:
         """Return the name of the extension to be used as a key in ext dict."""
-        return "ec3"
+        return const.ILCD_IDENTIFICATION[0]
```

### Comparing `ilcdlib-0.6.0/src/ilcdlib/http_common.py` & `ilcdlib-0.7.0/src/ilcdlib/http_common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/mapping/__init__.py` & `ilcdlib-0.7.0/src/ilcdlib/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/mapping/common.py` & `ilcdlib-0.7.0/src/ilcdlib/mapping/common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/mapping/compliance.py` & `ilcdlib-0.7.0/src/ilcdlib/mapping/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/mapping/flows.py` & `ilcdlib-0.7.0/src/ilcdlib/mapping/flows.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/mapping/impacts.py` & `ilcdlib-0.7.0/src/ilcdlib/mapping/impacts.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/mapping/indicators.py` & `ilcdlib-0.7.0/src/ilcdlib/mapping/indicators.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/mapping/units.py` & `ilcdlib-0.7.0/src/ilcdlib/mapping/units.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/medium/__init__.py` & `ilcdlib-0.7.0/src/ilcdlib/medium/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/medium/archive.py` & `ilcdlib-0.7.0/src/ilcdlib/medium/archive.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/medium/soda4lca.py` & `ilcdlib-0.7.0/src/ilcdlib/medium/soda4lca.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/reference_data.py` & `ilcdlib-0.7.0/src/ilcdlib/reference_data.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/sanitizing/__init__.py` & `ilcdlib-0.7.0/src/ilcdlib/sanitizing/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/sanitizing/domain.py` & `ilcdlib-0.7.0/src/ilcdlib/sanitizing/domain.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/sanitizing/phone.py` & `ilcdlib-0.7.0/src/ilcdlib/sanitizing/phone.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/soda4lca/__init__.py` & `ilcdlib-0.7.0/src/ilcdlib/soda4lca/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/soda4lca/api_client.py` & `ilcdlib-0.7.0/src/ilcdlib/soda4lca/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         :return:
         """
         params = dict(
             format="json",
             startIndex=offset,
             pageSize=page_size,
             search="true",
-            *other_params,
+            **other_params,
         )
         if lang is not None:
             params["lang"] = lang
             params["langFallback"] = True
         response = self._do_request("get", "/processes", params=params)
         obj = response.json()
         meta = ListResponseMeta(
```

### Comparing `ilcdlib-0.6.0/src/ilcdlib/type.py` & `ilcdlib-0.7.0/src/ilcdlib/type.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/utils.py` & `ilcdlib-0.7.0/src/ilcdlib/utils.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/src/ilcdlib/xml_parser.py` & `ilcdlib-0.7.0/src/ilcdlib/xml_parser.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.6.0/PKG-INFO` & `ilcdlib-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilcdlib
-Version: 0.6.0
+Version: 0.7.0
 Summary: A toolkit for reading and writing ILCD format and it's derivatives
 Home-page: https://github.com/cchangelabs/ilcdlib
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: support@c-change-labs.com
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: cli
 Provides-Extra: lxml
 Requires-Dist: cli-rack (>=1.0.6) ; extra == "cli"
 Requires-Dist: lxml (>=4.9.2,<4.10.0) ; extra == "lxml"
-Requires-Dist: openepd (>=0.10.0,<1.0.0)
+Requires-Dist: openepd (>=0.11.0,<1.0.0)
 Requires-Dist: requests (>=2.1.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Project-URL: Repository, https://github.com/cchangelabs/ilcdlib
 Description-Content-Type: text/markdown
 
 # ILCD Lib
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: ilcdlib Version: 0.6.0 Summary: A toolkit for
+Metadata-Version: 2.1 Name: ilcdlib Version: 0.7.0 Summary: A toolkit for
 reading and writing ILCD format and it's derivatives Home-page: https://
 github.com/cchangelabs/ilcdlib License: Apache-2.0 Author: C-Change Labs
 Author-email: support@c-change-labs.com Maintainer: C-Change Labs Maintainer-
 email: support@c-change-labs.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Provides-Extra: cli
 Provides-Extra: lxml Requires-Dist: cli-rack (>=1.0.6) ; extra == "cli"
 Requires-Dist: lxml (>=4.9.2,<4.10.0) ; extra == "lxml" Requires-Dist: openepd
-(>=0.10.0,<1.0.0) Requires-Dist: requests (>=2.1.0,<3.0.0) Requires-Dist:
+(>=0.11.0,<1.0.0) Requires-Dist: requests (>=2.1.0,<3.0.0) Requires-Dist:
 urllib3 (>=1.26.16,<2.0.0) Project-URL: Repository, https://github.com/
 cchangelabs/ilcdlib Description-Content-Type: text/markdown # ILCD Lib
      [https://img.shields.io/pypi/l/ilcdlib?style=for-the-badge] [https://
      img.shields.io/pypi/pyversions/ilcdlib?style=for-the-badge] [https://
  img.shields.io/badge/Code%20Style-black-black?style=for-the-badge] [https://
   img.shields.io/pypi/v/ilcdlib?style=for-the-badge] [https://img.shields.io/
                      pypi/dm/ilcdlib?style=for-the-badge]
```

