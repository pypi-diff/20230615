# Comparing `tmp/fabrictestbed-extensions-1.5.0rc3.tar.gz` & `tmp/fabrictestbed-extensions-1.5.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-extensions-1.5.0rc3.tar", last modified: Mon May 22 14:08:17 2023, max compression
+gzip compressed data, was "fabrictestbed-extensions-1.5.0rc4.tar", last modified: Mon Jun 12 17:31:24 2023, max compression
```

## Comparing `fabrictestbed-extensions-1.5.0rc3.tar` & `fabrictestbed-extensions-1.5.0rc4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1025 2023-05-11 18:23:24.341681 fabrictestbed-extensions-1.5.0rc3/.github/workflows/build.yml
--rw-r--r--   0        0        0     1618 2023-05-11 18:23:24.341808 fabrictestbed-extensions-1.5.0rc3/.github/workflows/checks.yml
--rw-r--r--   0        0        0     2402 2023-05-11 18:23:24.341926 fabrictestbed-extensions-1.5.0rc3/.github/workflows/test.yml
--rw-r--r--   0        0        0     1806 2023-05-12 13:41:06.568624 fabrictestbed-extensions-1.5.0rc3/.gitignore
--rw-r--r--   0        0        0      666 2023-05-11 18:23:24.342134 fabrictestbed-extensions-1.5.0rc3/.readthedocs.yaml
--rw-r--r--   0        0        0     2670 2023-05-11 18:23:24.342247 fabrictestbed-extensions-1.5.0rc3/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2023-05-11 18:23:24.342656 fabrictestbed-extensions-1.5.0rc3/LICENSE
--rw-r--r--   0        0        0     4054 2023-05-11 18:23:24.342855 fabrictestbed-extensions-1.5.0rc3/README.md
--rw-r--r--   0        0        0      638 2023-05-11 18:23:24.343022 fabrictestbed-extensions-1.5.0rc3/docs/Makefile
--rw-r--r--   0        0        0      799 2023-05-11 18:23:24.343131 fabrictestbed-extensions-1.5.0rc3/docs/make.bat
--rw-r--r--   0        0        0     1996 2023-05-11 18:23:24.343312 fabrictestbed-extensions-1.5.0rc3/docs/source/conf.py
--rw-r--r--   0        0        0     8903 2023-05-12 13:41:06.569256 fabrictestbed-extensions-1.5.0rc3/docs/source/fablib.rst
--rw-r--r--   0        0        0     4470 2023-05-11 18:23:24.343613 fabrictestbed-extensions-1.5.0rc3/docs/source/index.rst
--rw-r--r--   0        0        0      150 2023-05-22 14:07:41.148032 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/__init__.py
--rw-r--r--   0        0        0        2 2023-05-11 18:23:24.344271 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/editors/__init__.py
--rw-r--r--   0        0        0    18044 2023-05-11 18:23:24.344572 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/editors/abc_topology_editor.py
--rw-r--r--   0        0        0     6277 2023-05-11 18:23:24.345052 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
--rw-r--r--   0        0        0    68479 2023-05-11 18:23:24.345347 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/editors/geo_topology_editor.py
--rw-r--r--   0        0        0        1 2023-05-11 18:23:24.345570 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/__init__.py
--rw-r--r--   0        0        0     4793 2023-05-11 18:23:24.345738 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/abc_fablib.py
--rw-r--r--   0        0        0    21062 2023-05-11 18:23:24.345997 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/component.py
--rw-r--r--   0        0        0    76799 2023-05-11 18:23:24.346796 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/fablib.py
--rw-r--r--   0        0        0     5807 2023-05-11 18:23:24.347162 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/facility_port.py
--rw-r--r--   0        0        0    25967 2023-05-11 18:23:24.347819 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/interface.py
--rw-r--r--   0        0        0    40005 2023-05-12 13:41:06.570962 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/network_service.py
--rw-r--r--   0        0        0    95919 2023-05-11 18:23:24.348593 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/node.py
--rw-r--r--   0        0        0    34726 2023-05-22 14:06:53.930637 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/resources.py
--rw-r--r--   0        0        0    81904 2023-05-11 18:23:24.349763 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/slice.py
--rw-r--r--   0        0        0        2 2023-05-11 18:23:24.350075 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/images/__init__.py
--rw-r--r--   0        0        0   199914 2023-05-11 18:23:24.351514 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/images/fabric_logo.png
--rw-r--r--   0        0        0     1316 2023-05-11 18:23:24.351919 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/images/server.png
--rw-r--r--   0        0        0    62250 2023-05-11 18:23:24.352243 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/images/slice_rack.png
--rw-r--r--   0        0        0        2 2023-05-11 18:23:24.352522 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/__init__.py
--rw-r--r--   0        0        0    14765 2023-05-11 18:23:24.352740 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/abc_test.py
--rw-r--r--   0        0        0    34231 2023-05-11 18:23:24.353058 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/component_tests.py
--rw-r--r--   0        0        0       85 2023-05-11 18:23:24.353250 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/dummy-token.json
--rw-r--r--   0        0        0    13366 2023-05-11 18:23:24.353667 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py
--rw-r--r--   0        0        0    10227 2023-05-11 18:23:24.353942 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/hello_fabric.py
--rw-r--r--   0        0        0    20659 2023-05-11 18:23:24.354269 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/link_benchmark.py
--rw-r--r--   0        0        0    20919 2023-05-11 18:23:24.354513 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/local_network_benchmark.py
--rw-r--r--   0        0        0    44883 2023-05-11 18:23:24.354856 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/network_benchmark_tests.py
--rw-r--r--   0        0        0    10052 2023-05-11 18:23:24.355043 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/nvme_benchmark.py
--rw-r--r--   0        0        0     5095 2023-05-11 18:23:24.355416 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/test_basic.py
--rw-r--r--   0        0        0        2 2023-05-11 18:23:24.355793 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/utils/__init__.py
--rw-r--r--   0        0        0     3082 2023-05-11 18:23:24.356170 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/utils/abc_utils.py
--rw-r--r--   0        0        0     3304 2023-05-11 18:23:24.356417 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/utils/node.py
--rw-r--r--   0        0        0     8436 2023-05-11 18:23:24.356653 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/utils/slice.py
--rw-r--r--   0        0        0     1329 2023-05-12 13:47:58.788785 fabrictestbed-extensions-1.5.0rc3/pyproject.toml
--rwxr-xr-x   0        0        0      122 2023-05-11 18:23:24.357218 fabrictestbed-extensions-1.5.0rc3/sphinx.sh
--rw-r--r--   0        0        0     5278 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.5.0rc3/PKG-INFO
+-rw-r--r--   0        0        0     1025 2023-05-11 18:23:24.341681 fabrictestbed-extensions-1.5.0rc4/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1618 2023-05-11 18:23:24.341808 fabrictestbed-extensions-1.5.0rc4/.github/workflows/checks.yml
+-rw-r--r--   0        0        0     2402 2023-05-11 18:23:24.341926 fabrictestbed-extensions-1.5.0rc4/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1806 2023-05-12 13:41:06.568624 fabrictestbed-extensions-1.5.0rc4/.gitignore
+-rw-r--r--   0        0        0      666 2023-05-11 18:23:24.342134 fabrictestbed-extensions-1.5.0rc4/.readthedocs.yaml
+-rw-r--r--   0        0        0     2897 2023-06-08 17:08:10.775764 fabrictestbed-extensions-1.5.0rc4/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2023-05-11 18:23:24.342656 fabrictestbed-extensions-1.5.0rc4/LICENSE
+-rw-r--r--   0        0        0     4054 2023-05-11 18:23:24.342855 fabrictestbed-extensions-1.5.0rc4/README.md
+-rw-r--r--   0        0        0      638 2023-05-11 18:23:24.343022 fabrictestbed-extensions-1.5.0rc4/docs/Makefile
+-rw-r--r--   0        0        0      799 2023-05-11 18:23:24.343131 fabrictestbed-extensions-1.5.0rc4/docs/make.bat
+-rw-r--r--   0        0        0     1996 2023-05-11 18:23:24.343312 fabrictestbed-extensions-1.5.0rc4/docs/source/conf.py
+-rw-r--r--   0        0        0     8903 2023-05-12 13:41:06.569256 fabrictestbed-extensions-1.5.0rc4/docs/source/fablib.rst
+-rw-r--r--   0        0        0     4470 2023-05-11 18:23:24.343613 fabrictestbed-extensions-1.5.0rc4/docs/source/index.rst
+-rw-r--r--   0        0        0      150 2023-06-12 17:31:16.009089 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/__init__.py
+-rw-r--r--   0        0        0        2 2023-05-11 18:23:24.344271 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/editors/__init__.py
+-rw-r--r--   0        0        0    18044 2023-05-11 18:23:24.344572 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/editors/abc_topology_editor.py
+-rw-r--r--   0        0        0     6277 2023-05-11 18:23:24.345052 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
+-rw-r--r--   0        0        0    68479 2023-05-11 18:23:24.345347 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/editors/geo_topology_editor.py
+-rw-r--r--   0        0        0        1 2023-05-11 18:23:24.345570 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/__init__.py
+-rw-r--r--   0        0        0     4793 2023-05-11 18:23:24.345738 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/abc_fablib.py
+-rw-r--r--   0        0        0    21402 2023-06-11 18:11:35.985267 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/component.py
+-rw-r--r--   0        0        0    77331 2023-06-12 00:53:42.710305 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/fablib.py
+-rw-r--r--   0        0        0     5821 2023-06-08 17:08:10.777119 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/facility_port.py
+-rw-r--r--   0        0        0    26262 2023-06-11 18:14:38.646369 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/interface.py
+-rw-r--r--   0        0        0    40019 2023-06-08 17:08:10.777971 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/network_service.py
+-rw-r--r--   0        0        0    96366 2023-06-10 11:36:12.662165 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/node.py
+-rw-r--r--   0        0        0    38331 2023-06-12 00:52:03.202648 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/resources.py
+-rw-r--r--   0        0        0    81762 2023-06-08 17:08:10.780745 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/slice.py
+-rw-r--r--   0        0        0        2 2023-05-11 18:23:24.350075 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/images/__init__.py
+-rw-r--r--   0        0        0   199914 2023-05-11 18:23:24.351514 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/images/fabric_logo.png
+-rw-r--r--   0        0        0     1316 2023-05-11 18:23:24.351919 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/images/server.png
+-rw-r--r--   0        0        0    62250 2023-05-11 18:23:24.352243 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/images/slice_rack.png
+-rw-r--r--   0        0        0        2 2023-05-11 18:23:24.352522 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/__init__.py
+-rw-r--r--   0        0        0    14765 2023-05-11 18:23:24.352740 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/abc_test.py
+-rw-r--r--   0        0        0    34389 2023-06-09 15:08:19.572155 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/component_tests.py
+-rw-r--r--   0        0        0       85 2023-05-11 18:23:24.353250 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/dummy-token.json
+-rw-r--r--   0        0        0    13366 2023-05-11 18:23:24.353667 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py
+-rw-r--r--   0        0        0    10227 2023-05-11 18:23:24.353942 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/hello_fabric.py
+-rw-r--r--   0        0        0    20659 2023-05-11 18:23:24.354269 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/link_benchmark.py
+-rw-r--r--   0        0        0    20919 2023-05-11 18:23:24.354513 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/local_network_benchmark.py
+-rw-r--r--   0        0        0    44883 2023-05-11 18:23:24.354856 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/network_benchmark_tests.py
+-rw-r--r--   0        0        0    10052 2023-05-11 18:23:24.355043 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/nvme_benchmark.py
+-rw-r--r--   0        0        0     5095 2023-05-11 18:23:24.355416 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/test_basic.py
+-rw-r--r--   0        0        0        2 2023-05-11 18:23:24.355793 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/utils/__init__.py
+-rw-r--r--   0        0        0     3082 2023-05-11 18:23:24.356170 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/utils/abc_utils.py
+-rw-r--r--   0        0        0     3304 2023-05-11 18:23:24.356417 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/utils/node.py
+-rw-r--r--   0        0        0     8436 2023-05-11 18:23:24.356653 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/utils/slice.py
+-rw-r--r--   0        0        0     1340 2023-06-12 17:30:38.138232 fabrictestbed-extensions-1.5.0rc4/pyproject.toml
+-rwxr-xr-x   0        0        0      122 2023-05-11 18:23:24.357218 fabrictestbed-extensions-1.5.0rc4/sphinx.sh
+-rw-r--r--   0        0        0     5275 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.5.0rc4/PKG-INFO
```

### Comparing `fabrictestbed-extensions-1.5.0rc3/.github/workflows/build.yml` & `fabrictestbed-extensions-1.5.0rc4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/.github/workflows/checks.yml` & `fabrictestbed-extensions-1.5.0rc4/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/.github/workflows/test.yml` & `fabrictestbed-extensions-1.5.0rc4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/.gitignore` & `fabrictestbed-extensions-1.5.0rc4/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/.readthedocs.yaml` & `fabrictestbed-extensions-1.5.0rc4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/CHANGELOG.md` & `fabrictestbed-extensions-1.5.0rc4/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,25 @@
 This is the changelog file for FABRIC testbed extensions.  All notable
 changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
+## [1.4.4] - 2023-05-21
+
+### Fixed
+
+- Changed some error that were printing to stdout to log instead.
+
+### Added
+
+- Added a get_public_ips call to NetworkService for user to get list of public IPs assigned to their FabNetExt
+
+
 ## [1.4.3] - 2023-04-22
 
 ### Fixed
 
 - The interface.get_ip_addr() fuction now returns address strings for devs that were manually configured. 
 
 ## [1.4.2] - 2023-04-21
```

### Comparing `fabrictestbed-extensions-1.5.0rc3/LICENSE` & `fabrictestbed-extensions-1.5.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/README.md` & `fabrictestbed-extensions-1.5.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/docs/Makefile` & `fabrictestbed-extensions-1.5.0rc4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/docs/make.bat` & `fabrictestbed-extensions-1.5.0rc4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/docs/source/conf.py` & `fabrictestbed-extensions-1.5.0rc4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/docs/source/fablib.rst` & `fabrictestbed-extensions-1.5.0rc4/docs/source/fablib.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/docs/source/index.rst` & `fabrictestbed-extensions-1.5.0rc4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/editors/abc_topology_editor.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/editors/abc_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/editors/cytoscape_topology_editor.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/editors/cytoscape_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/editors/geo_topology_editor.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/editors/geo_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/abc_fablib.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/abc_fablib.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/component.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 from __future__ import annotations
 from typing import TYPE_CHECKING
 import json
+import jinja2
 
 if TYPE_CHECKING:
     from fabrictestbed_extensions.fablib.slice import Slice
     from fabrictestbed_extensions.fablib.node import Node
     from fabrictestbed_extensions.fablib.interface import Interface
     from fabrictestbed_extensions.fablib.interface import Interface
 
@@ -49,14 +50,15 @@
         "NIC_ConnectX_5": ComponentModelType.SmartNIC_ConnectX_5,
         "NVME_P4510": ComponentModelType.NVME_P4510,
         "GPU_TeslaT4": ComponentModelType.GPU_Tesla_T4,
         "GPU_RTX6000": ComponentModelType.GPU_RTX6000,
         "GPU_A40": ComponentModelType.GPU_A40,
         "GPU_A30": ComponentModelType.GPU_A30,
         "NIC_OpenStack": ComponentModelType.SharedNIC_OpenStack_vNIC,
+        "FPGA_Xilinx_U280": ComponentModelType.FPGA_Xilinx_U280
     }
 
     def __str__(self):
         """
         Creates a tabulated string describing the properties of the component.
 
         Intended for printing component information.
@@ -97,14 +99,15 @@
             "disk": "Disk",
             "units": "Units",
             "pci_address": "PCI Address",
             "model": "Model",
             "type": "Type",
             "dev": "Device",
             "node": "Node",
+            "numa": "Numa Node",
         }
 
     def toDict(self, skip=[]):
         """
         Returns the component attributes as a dictionary
 
         :return: slice attributes as dictionary
@@ -117,14 +120,15 @@
             "disk": str(self.get_disk()),
             "units": str(self.get_unit()),
             "pci_address": str(self.get_pci_addr()),
             "model": str(self.get_model()),
             "type": str(self.get_type()),
             "dev": str(self.get_device_name()),
             "node": str(self.get_node().get_name()),
+            "numa": str(self.get_numa_node())
         }
 
     def generate_template_context(self):
         context = self.toDict()
         context["interfaces"] = []
         # for interface in self.get_interfaces():
         #    context["interfaces"].append(interface.get_name())
@@ -393,14 +397,20 @@
 
     def get_details(self) -> str:
         """
         Not intended for API use
         """
         return self.get_fim_component().details
 
+    def get_numa_node(self) -> str:
+        """
+        Get the Numa Node assigned to the device
+        """
+        return self.get_fim_component().get_property(pname="label_allocations").numa
+
     def get_disk(self) -> int:
         """
         Gets the amount of disk space on this component.
 
         :return: this component's disk space
         :rtype: int
         """
@@ -579,16 +589,15 @@
                     f"{block_device_name}"
                     f"p1 "
                     f"{mount_point}"
                 )
             )
             output.append(self.node.execute(f"df -h {mount_point}"))
         except Exception as e:
-            print(f"config_nvme Fail: {self.get_name()}")
-            # traceback.print_exc()
+            logging.error(f"config_nvme Fail: {self.get_name()}:", exc_info=True)
             raise Exception(str(output))
 
         return output
 
     def get_device_name(self) -> str:
         """
         Not for API use
```

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/fablib.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/fablib.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,17 @@
 
 from IPython import get_ipython
 
 from typing import List, Dict
 
 from typing import TYPE_CHECKING
 
+from IPython.core.display_functions import display
 from fabrictestbed.util.constants import Constants
+from fabrictestbed_extensions import __version__ as fablib_version
 import pandas as pd
 from ipaddress import IPv4Network, IPv6Network
 from tabulate import tabulate
 import json
 
 
 if TYPE_CHECKING:
@@ -78,15 +80,15 @@
 
         :return: list of site names as strings
         :rtype: list[str]
         """
         return fablib.get_default_fablib_manager().get_site_names()
 
     @staticmethod
-    def list_sites() -> str:
+    def list_sites() -> object:
         """
         Get a string used to print a tabular list of sites with state
 
         :return: tabulated string of site state
         :rtype: str
         """
         return fablib.get_default_fablib_manager().list_sites()
@@ -1021,15 +1023,16 @@
     def list_sites(
         self,
         output: str = None,
         fields: str = None,
         quiet: bool = False,
         filter_function=None,
         update: bool = True,
-        pretty_names=True,
+        pretty_names: bool = True,
+        force_refresh: bool = False,
     ) -> object:
         """
         Lists all the sites and their attributes.
 
         There are several output options: "text", "pandas", and "json" that determine the format of the
         output that is returned and (optionally) displayed/printed.
 
@@ -1050,17 +1053,20 @@
         :param fields: list of fields (table columns) to show
         :type fields: List[str]
         :param quiet: True to specify printing/display
         :type quiet: bool
         :param filter_function: lambda function
         :type filter_function: lambda
         :return: table in format specified by output parameter
+        :param update
+        :param pretty_names
+        :param force_refresh
         :rtype: Object
         """
-        return self.get_resources(update=update).list_sites(
+        return self.get_resources(update=update, force_refresh=force_refresh).list_sites(
             output=output,
             fields=fields,
             quiet=quiet,
             filter_function=filter_function,
             pretty_names=pretty_names,
         )
 
@@ -1275,24 +1281,24 @@
         if self.facility_ports is None:
             self.facility_ports = FacilityPorts(self)
         elif update:
             self.facility_ports.update()
 
         return self.facility_ports
 
-    def get_resources(self, update: bool = True) -> Resources:
+    def get_resources(self, update: bool = True, force_refresh:bool = False) -> Resources:
         """
         Get a reference to the resources object. The resources object
         is used to query for available resources and capacities.
 
         :return: the resources object
         :rtype: Resources
         """
         if not self.resources:
-            self.get_available_resources(update=update)
+            self.get_available_resources(update=update, force_refresh=force_refresh)
 
         return self.resources
 
     def get_random_site(
         self, avoid: List[str] = [], filter_function=None, update: bool = True
     ) -> str:
         """
@@ -1393,14 +1399,15 @@
             "bastion_host": "Bastion Host",
             "bastion_private_key_passphrase": "Bastion Private Key Passphrase",
             "slice_public_key_file": "Slice Public Key File",
             "slice_private_key_file": "Slice Private Key File",
             "fabric_slice_private_key_passphrase": "Slice Private Key Passphrase",
             "fablib_log_file": "Log File",
             "fablib_log_level": "Log Level",
+            "fablib_version": "Version",
         }
 
     def get_config(self) -> Dict[str, Dict[str, str]]:
         """
         Gets a dictionary mapping keywords to configured FABRIC environment
         variable values.
 
@@ -1417,14 +1424,15 @@
             "bastion_host": self.bastion_public_addr,
             "bastion_private_key_passphrase": self.bastion_passphrase,
             "slice_public_key_file": self.get_default_slice_public_key_file(),
             "slice_private_key_file": self.get_default_slice_private_key_file(),
             "fabric_slice_private_key_passphrase": self.get_default_slice_private_key_passphrase(),
             "fablib_log_file": self.get_log_file(),
             "fablib_log_level": self.get_log_level(),
+            "fablib_version": fablib_version,
         }
 
     def get_configXXX(self) -> Dict[str, Dict[str, str]]:
         """
         Gets a dictionary mapping keywords to configured FABRIC environment
         variable values.
 
@@ -1667,30 +1675,31 @@
                 "Failed to get advertised_topology: {}, {}".format(
                     return_status, topology
                 )
             )
 
         return topology.sites[site]
 
-    def get_available_resources(self, update: bool = False) -> Resources:
+    def get_available_resources(self, update: bool = False, force_refresh: bool = False) -> Resources:
         """
         Get the available resources.
 
         Optionally update the available resources by querying the FABRIC
         services. Otherwise, this method returns the existing information.
 
         :param update:
+        :param force_refresh
         :return: Available Resources object
         """
         from fabrictestbed_extensions.fablib.resources import Resources
 
         if self.resources is None:
-            self.resources = Resources(self)
+            self.resources = Resources(self, force_refresh=force_refresh)
         elif update:
-            self.resources.update()
+            self.resources.update(force_refresh=force_refresh)
 
         return self.resources
 
     def get_fim_slices(
         self, excludes: List[SliceState] = [SliceState.Dead, SliceState.Closing]
     ) -> List[OrchestratorSlice]:
         """
```

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/facility_port.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/facility_port.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 from __future__ import annotations
 
 from tabulate import tabulate
 import json
+import jinja2
 
 from fabrictestbed.slice_editor import Labels, Capacities
 from fabrictestbed_extensions.fablib.interface import Interface
 
 from typing import TYPE_CHECKING, List
 
 if TYPE_CHECKING:
```

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/interface.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 import ipaddress
 
 from fabrictestbed.slice_editor import Flags
 from tabulate import tabulate
 from ipaddress import IPv4Address
 import json
+import jinja2
 
 import logging
 
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from fabrictestbed_extensions.fablib.slice import Slice
@@ -84,14 +85,15 @@
             ["Bandwidth", self.get_bandwidth()],
             ["Mode", self.get_mode()],
             ["VLAN", self.get_vlan()],
             ["MAC", self.get_mac()],
             ["Physical Device", self.get_physical_os_interface_name()],
             ["Device", self.get_os_interface()],
             ["Address", self.get_ip_addr()],
+            ["Numa Node", self.get_numa_node()],
         ]
 
         return tabulate(table)
 
     def toJson(self):
         """
         Returns the interface attributes as a json string
@@ -118,14 +120,15 @@
             "state": "State",
             "error": "Error",
             "ssh_command": "SSH Command",
             "public_ssh_key_file": "Public SSH Key File",
             "private_ssh_key_file": "Private SSH Key File",
             "mode": "Mode",
             "ip_addr": "IP Address",
+            "numa": "Numa Node"
         }
 
     def toDict(self, skip=[]):
         """
         Returns the interface attributes as a dictionary
 
         :return: slice attributes as dictionary
@@ -168,16 +171,20 @@
             "vlan": str(self.get_vlan())
             if self.get_vlan()
             else "",  # str(self.get_vlan()),
             "mac": mac,
             "physical_dev": physical_dev,
             "dev": dev,
             "ip_addr": ip_addr,
+            "numa": str(self.get_numa_node()),
         }
 
+    def get_numa_node(self) -> str:
+        return self.get_component().get_numa_node()
+
     def generate_template_context(self):
         context = self.toDict()
         return context
 
     def get_template_context(self):
         return self.get_slice().get_template_context(self)
 
@@ -665,15 +672,15 @@
                 return links
 
             for link in links:
                 if link["ifname"] == dev:
                     return link
             return None
         except Exception as e:
-            print(f"Exception: {e}")
+            logging.warning(f"{e}")
 
     def get_ip_addr_show(self, dev=None):
         try:
             if not dev:
                 dev = self.get_os_interface()
 
             stdout, stderr = self.get_node().execute(
@@ -699,25 +706,25 @@
             stdout, stderr = self.get_node().execute("ip -j addr list", quiet=True)
 
             addrs = json.loads(stdout)
 
             dev = self.get_os_interface()
             # print(f"dev: {dev}")
 
-            if dev == None:
+            if dev is None:
                 return addrs
 
             for addr in addrs:
                 if addr["ifname"] == dev:
                     # Hack to make it backward compatible. Should return an object
                     return str(ipaddress.ip_address(addr["addr_info"][0]["local"]))
 
             return None
         except Exception as e:
-            print(f"Exception: {e}")
+            logging.warning(f"{e}")
 
     # fablib.Interface.get_ip_addr()
     def get_ips(self, family=None):
         """
         Gets a list of ips assigned to this interface.
 
         :return list of ips
@@ -734,15 +741,15 @@
             for addr_info in ip_addr["addr_info"]:
                 if family == None:
                     return_ips.append(addr_info["local"])
                 else:
                     if addr_info["family"] == family:
                         return_ips.append(addr_info["local"])
         except Exception as e:
-            print(f"Exception: {e}")
+            logging.warning(f"{e}")
 
         return return_ips
 
     def get_fim(self):
         return self.get_fim_interface()
 
     def set_user_data(self, user_data: dict):
@@ -797,14 +804,16 @@
             try:
                 addr = ipaddress.ip_address(fablib_data["addr"])
             except:
                 addr = fablib_data["addr"]
             return addr
         else:
             # get_ip_addr_ssh()
+            if self.get_mac() is None:
+                return None
             return self.get_ip_addr_ssh()
 
     def set_mode(self, mode: str = "config"):
         fablib_data = self.get_fablib_data()
         fablib_data["mode"] = mode
         self.set_fablib_data(fablib_data)
```

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/network_service.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/network_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
 from fabrictestbed.slice_editor import UserData
 from fabric_cf.orchestrator.orchestrator_proxy import Status
 
 from ipaddress import IPv4Address, IPv6Address, IPv4Network, IPv6Network
 import ipaddress
 import json
+import jinja2
 
 
 class NetworkService:
     network_service_map = {
         "L2Bridge": ServiceType.L2Bridge,
         "L2PTP": ServiceType.L2PTP,
         "L2STS": ServiceType.L2STS,
```

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/node.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,24 +27,25 @@
 import ipaddress
 import json
 import threading
 import time
 import paramiko
 import logging
 
+from IPython.core.display_functions import display
 from fabrictestbed_extensions.fablib.network_service import NetworkService
 from tabulate import tabulate
 import select
 import jinja2
 
 from concurrent.futures import ThreadPoolExecutor
 import concurrent.futures
 
 
-from typing import List, Union, Tuple
+from typing import List, Union, Tuple, Dict
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from fabrictestbed_extensions.fablib.slice import Slice
     from fabric_cf.orchestrator.swagger_client import Sliver as OrchestratorSliver
 
@@ -411,25 +412,25 @@
                     return True
             else:
                 if filter_function(x) and x["name"] in set(components):
                     return True
 
             return False
 
-        if pretty_names and len(self.self.get_components()) > 0:
-            pretty_names_dict = self.self.get_components()[0].get_pretty_name_dict()
+        if pretty_names and len(self.get_components()) > 0:
+            pretty_names_dict = self.get_components()[0].get_pretty_name_dict()
         else:
             pretty_names_dict = {}
 
         return self.get_slice().list_components(
             fields=fields,
             output=output,
             quiet=quiet,
             filter_function=combined_filter_function,
-            pretty_names_dict=pretty_names_dict,
+            pretty_names=pretty_names_dict,
         )
 
     def list_interfaces(
         self,
         fields=None,
         output=None,
         quiet=False,
@@ -948,14 +949,17 @@
         Example model include:
         - NIC_Basic: A single port 100 Gbps SR-IOV Virtual Function on a Mellanox ConnectX-6
         - NIC_ConnectX_5: A dual port 25 Gbps Mellanox ConnectX-5
         - NIC_ConnectX_6: A dual port 100 Gbps Mellanox ConnectX-6
         - NVME_P4510: NVMe Storage Device
         - GPU_TeslaT4: Tesla T4 GPU
         - GPU_RTX6000: RTX6000 GPU
+        - GPU_A30: A30 GPU
+        - GPU_A40: A40 GPU
+        - FPGA_Xilinx_U280: Xilinx U280 GPU
         :param model: the name of the component model to add
         :type model: String
         :param name: the name of the new component
         :type name: String
         :return: the new component
         :rtype: Component
         """
@@ -1204,14 +1208,15 @@
             # src_addr = (self.get_fablib_manager().get_bastion_private_ipv4_addr(), 22)
             src_addr = ("0.0.0.0", 22)
 
         elif self.validIPAddress(management_ip) == "IPv6":
             # src_addr = (self.get_fablib_manager().get_bastion_private_ipv6_addr(), 22)
             src_addr = ("0:0:0:0:0:0:0:0", 22)
         else:
+            logging.error("node.execute: Management IP Invalid:", exc_info=True)
             raise Exception(f"node.execute: Management IP Invalid: {management_ip}")
         dest_addr = (management_ip, 22)
 
         bastion_username = self.get_fablib_manager().get_bastion_username()
         bastion_key_file = self.get_fablib_manager().get_bastion_key_filename()
 
         if username != None:
@@ -1285,17 +1290,21 @@
                     rtn_stderr = str(stderr.read(), "utf-8").replace("\\n", "\n")
                     if quiet == False:
                         print(rtn_stdout, rtn_stderr)
 
                 else:
                     # Credit to Stack Overflow user tintin's post here: https://stackoverflow.com/a/32758464
                     stdout_chunks = []
-                    stdout_chunks.append(
-                        stdout.channel.recv(len(stdout.channel.in_buffer))
-                    )
+                    try:
+                        stdout_chunks.append(
+                            stdout.channel.recv(len(stdout.channel.in_buffer))
+                        )
+                    except EOFError:
+                        logging.warning('A Paramiko EOFError has occurred, '
+                                        'if this is part of a reboot sequence, it can be ignored')
                     stderr_chunks = []
 
                     while (
                         not channel.closed
                         or channel.recv_ready()
                         or channel.recv_stderr_ready()
                     ):
@@ -1370,15 +1379,15 @@
 
                 return rtn_stdout, rtn_stderr
                 # success, skip other tries
                 break
 
             except Exception as e:
                 logging.warning(
-                    f"Exception in upload_file() (attempt #{attempt} of {retry}): {e}"
+                    f"Exception in node.execute() (attempt #{attempt} of {retry}): {e}"
                 )
 
                 if attempt + 1 == retry:
                     raise e
 
                 # Fail, try again
                 if self.get_fablib_manager().get_log_level() == logging.DEBUG:
@@ -1629,15 +1638,15 @@
         management_ip = str(self.get_fim_node().get_property(pname="management_ip"))
         if self.validIPAddress(management_ip) == "IPv4":
             src_addr = ("0.0.0.0", 22)
 
         elif self.validIPAddress(management_ip) == "IPv6":
             src_addr = ("0:0:0:0:0:0:0:0", 22)
         else:
-            raise Exception(f"upload_file: Management IP Invalid: {management_ip}")
+            raise Exception(f"download_file: Management IP Invalid: {management_ip}")
         dest_addr = (management_ip, 22)
 
         for attempt in range(int(retry)):
             try:
                 key = self.get_paramiko_key(
                     private_key_file=self.get_private_key_file(),
                     get_private_key_passphrase=self.get_private_key_file(),
@@ -1932,15 +1941,14 @@
         """
         # TODO: Add docstring after doc networking classes
         # Assumes that the default route uses the management network
         logging.debug(f"{self.get_name()}->get_management_os_interface")
         stdout, stderr = self.execute("sudo ip -j route list", quiet=True)
         stdout_json = json.loads(stdout)
 
-        # print(pythonObj)
         for i in stdout_json:
             if i["dst"] == "default":
                 logging.debug(
                     f"{self.get_name()}->get_management_os_interface: management_os_interface {i['dev']}"
                 )
                 return i["dev"]
         return None
```

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/resources.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/resources.py`

 * *Files 17% similar despite different names*

```diff
@@ -66,28 +66,34 @@
         "nvme_allocated": "NVMe Allocated",
         "tesla_t4_available": "Tesla T4 Available",
         "tesla_t4_capacity": "Tesla T4 Capacity",
         "tesla_t4_allocated": "Tesla T4 Allocated",
         "rtx6000_available": "RTX6000 Available",
         "rtx6000_capacity": "RTX6000 Capacity",
         "rtx6000_allocated": "RTX6000 Allocated",
+        "a30_available": "A30 Available",
+        "a30_capacity": "A30 Capacity",
+        "a30_allocated": "A30 Allocated",
+        "a40_available": "A40 Available",
+        "a40_capacity": "A40 Capacity",
+        "a40_allocated": "A40 Allocated",
     }
 
-    def __init__(self, fablib_manager):
+    def __init__(self, fablib_manager, force_refresh: bool = False):
         """
         Constructor
         :return:
         """
         super().__init__()
 
         self.fablib_manager = fablib_manager
 
         self.topology = None
 
-        self.update()
+        self.update(force_refresh=force_refresh)
 
     def __str__(self) -> str:
         """
         Creates a tabulated string of all the available resources.
 
         Intended for printing available resources.
 
@@ -109,14 +115,17 @@
                     # self.get_location_lat_long(site_name),
                     f"{self.get_component_available(site_name,'SharedNIC-ConnectX-6')}/{self.get_component_capacity(site_name,'SharedNIC-ConnectX-6')}",
                     f"{self.get_component_available(site_name,'SmartNIC-ConnectX-6')}/{self.get_component_capacity(site_name,'SmartNIC-ConnectX-6')}",
                     f"{self.get_component_available(site_name,'SmartNIC-ConnectX-5')}/{self.get_component_capacity(site_name,'SmartNIC-ConnectX-5')}",
                     f"{self.get_component_available(site_name,'NVME-P4510')}/{self.get_component_capacity(site_name,'NVME-P4510')}",
                     f"{self.get_component_available(site_name,'GPU-Tesla T4')}/{self.get_component_capacity(site_name,'GPU-Tesla T4')}",
                     f"{self.get_component_available(site_name,'GPU-RTX6000')}/{self.get_component_capacity(site_name,'GPU-RTX6000')}",
+                    f"{self.get_component_available(site_name, 'GPU-A30')}/{self.get_component_capacity(site_name, 'GPU-A30')}",
+                    f"{self.get_component_available(site_name, 'GPU-A40')}/{self.get_component_capacity(site_name, 'GPU-A40')}",
+                    f"{self.get_component_available(site_name, 'FPGA-Xilinx-U280')}/{self.get_component_capacity(site_name, 'FPGA-Xilinx-U280')}",
                 ]
             )
 
         return tabulate(
             table,
             headers=[
                 "Name",
@@ -129,14 +138,17 @@
                 # "Location Coordinates"
                 "Basic (100 Gbps NIC)",
                 "ConnectX-6 (100 Gbps x2 NIC)",
                 "ConnectX-5 (25 Gbps x2 NIC)",
                 "P4510 (NVMe 1TB)",
                 "Tesla T4 (GPU)",
                 "RTX6000 (GPU)",
+                "A30 (GPU)",
+                "A40 (GPU)",
+                "FPGA-Xilinx-U280"
             ],
         )
 
     def show_site(
         self,
         site_name: str,
         output: str = None,
@@ -195,19 +207,20 @@
             return self.topology.sites[site_name]
         except Exception as e:
             logging.warning(f"Failed to get site {site_name}")
             return ""
 
     def get_state(self, site_name: str):
         try:
-            maint_info = self.get_topology_site(site_name).get_property("maintenance_info")
-            if maint_info.get(site_name) is None:
-                return "Active"
-            else:
-                return maint_info.get(site_name).state
+            return str(
+                self.get_topology_site(site_name)
+                .get_property("maintenance_info")
+                .get(site_name)
+                .state
+            )
         except Exception as e:
             logging.warning(f"Failed to get site state {site_name}")
             return ""
 
     def get_component_capacity(self, site_name: str, component_model_name: str) -> int:
         """
         Gets gets the total site capacity of a component by model name.
@@ -472,22 +485,22 @@
         except Exception as e:
             # logging.debug(f"Failed to get disk available {site_name}")
             return self.get_disk_capacity(site_name)
 
     def get_fablib_manager(self):
         return self.fablib_manager
 
-    def update(self):
+    def update(self, force_refresh: bool = False):
         """
         Update the available resources by querying the FABRIC services
 
         """
         logging.info(f"Updating available resources")
         return_status, topology = (
-            self.get_fablib_manager().get_slice_manager().resources()
+            self.get_fablib_manager().get_slice_manager().resources(force_refresh=force_refresh)
         )
         if return_status != Status.OK:
             raise Exception(
                 "Failed to get advertised_topology: {}, {}".format(
                     return_status, topology
                 )
             )
@@ -603,14 +616,26 @@
             "tesla_t4_capacity": self.get_component_capacity(site_name, "GPU-Tesla T4"),
             "tesla_t4_allocated": self.get_component_capacity(site_name, "GPU-Tesla T4")
             - self.get_component_available(site_name, "GPU-Tesla T4"),
             "rtx6000_available": self.get_component_available(site_name, "GPU-RTX6000"),
             "rtx6000_capacity": self.get_component_capacity(site_name, "GPU-RTX6000"),
             "rtx6000_allocated": self.get_component_capacity(site_name, "GPU-RTX6000")
             - self.get_component_available(site_name, "GPU-RTX6000"),
+            "a30_available": self.get_component_available(site_name, "GPU-A30"),
+            "a30_capacity": self.get_component_capacity(site_name, "GPU-A30"),
+            "a30_allocated": self.get_component_capacity(site_name, "GPU-A30")
+            - self.get_component_available(site_name, "GPU-A30"),
+            "a40_available": self.get_component_available(site_name, "GPU-A40"),
+            "a40_capacity": self.get_component_capacity(site_name, "GPU-A40"),
+            "a40_allocated": self.get_component_capacity(site_name, "GPU-A40")
+            - self.get_component_available(site_name, "GPU-A40"),
+            "fpga_u280_available": self.get_component_available(site_name, "FPGA-Xilinx-U280"),
+            "fpga_u280_capacity": self.get_component_capacity(site_name, "FPGA-Xilinx-U280"),
+            "fpga_u280_allocated": self.get_component_capacity(site_name, "FPGA-Xilinx-U280")
+                             - self.get_component_available(site_name, "FPGA-Xilinx-U280"),
         }
 
     def site_to_dictXXX(self, site):
         site_name = site.name
         return {
             "name": {"pretty_name": "Name", "value": site.name},
             "address": {
@@ -741,14 +766,53 @@
                 "value": self.get_component_capacity(site_name, "GPU-RTX6000"),
             },
             "rtx6000_allocated": {
                 "pretty_name": "RTX6000 Allocated",
                 "value": self.get_component_capacity(site_name, "GPU-RTX6000")
                 - self.get_component_available(site_name, "GPU-RTX6000"),
             },
+            "a30_available": {
+                "pretty_name": "A30 Available",
+                "value": self.get_component_available(site_name, "GPU-A30"),
+            },
+            "a30_capacity": {
+                "pretty_name": "A30 Capacity",
+                "value": self.get_component_capacity(site_name, "GPU-A30"),
+            },
+            "a30_allocated": {
+                "pretty_name": "A30 Allocated",
+                "value": self.get_component_capacity(site_name, "GPU-A30")
+                - self.get_component_available(site_name, "GPU-A30"),
+            },
+            "a40_available": {
+                "pretty_name": "A40 Available",
+                "value": self.get_component_available(site_name, "GPU-A40"),
+            },
+            "a40_capacity": {
+                "pretty_name": "A40 Capacity",
+                "value": self.get_component_capacity(site_name, "GPU-A40"),
+            },
+            "a40_allocated": {
+                "pretty_name": "A40 Allocated",
+                "value": self.get_component_capacity(site_name, "GPU-A40")
+                - self.get_component_available(site_name, "GPU-A40"),
+            },
+            "fpga_u280_available": {
+                "pretty_name": "FPGA U280 Available",
+                "value": self.get_component_available(site_name, "FPGA-Xilinx-U280"),
+            },
+            "fpga_u280_capacity": {
+                "pretty_name": "FPGA U280 Capacity",
+                "value": self.get_component_capacity(site_name, "FPGA-Xilinx-U280"),
+            },
+            "fpga_u280_allocated": {
+                "pretty_name": "FPGA U280 Allocated",
+                "value": self.get_component_capacity(site_name, "FPGA-Xilinx-U280")
+                         - self.get_component_available(site_name, "FPGA-Xilinx-U280"),
+            },
         }
 
     def list_sites(
         self,
         output=None,
         fields=None,
         quiet=False,
```

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/slice.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/slice.py`

 * *Files 1% similar despite different names*

```diff
@@ -1075,21 +1075,20 @@
     def get_error_messages(self) -> List[dict]:
         """
         Gets the error messages found in the sliver notices.
 
         :return: a list of error messages
         :rtype: List[Dict[String, String]]
         """
-        # strings to ingnor
+        # strings to ignore
         cascade_notice_string1 = "Closing reservation due to failure in slice"
         cascade_notice_string2 = "is in a terminal state"
 
         origin_notices = []
         for reservation_id, notice in self.get_notices().items():
-            # print(f"XXXXX: reservation_id: {reservation_id}, notice {notice}")
             if cascade_notice_string1 in notice or cascade_notice_string2 in notice:
                 continue
 
             origin_notices.append(
                 {
                     "reservation_id": reservation_id,
                     "notice": notice,
@@ -1132,15 +1131,15 @@
         # fails for topology that does not have nodes
         try:
             for node in self.get_nodes():
                 for component in node.get_components():
                     return_components.append(component)
 
         except Exception as e:
-            print(f"get_components: exception {e}")
+            logging.error(f"get_components: error {e}", exc_info=True)
             # traceback.print_exc()
             pass
         return return_components
 
     def get_nodes(self) -> List[Node]:
         """
         Gets a list of all nodes in this slice.
@@ -1288,16 +1287,15 @@
                     in NetworkService.get_fim_network_service_types()
                 ):
                     return_networks.append(
                         NetworkService(slice=self, fim_network_service=net)
                     )
 
         except Exception as e:
-            print(f"get_network_services: exception {e}")
-            # traceback.print_exc()
+            logging.error(e, exc_info=True)
             pass
         return return_networks
 
     def get_networks(self) -> List[NetworkService]:
         """
         Gets all network services (L2 and L3) in this slice
 
@@ -2006,16 +2004,14 @@
             else:
                 color = ""
             # return 'color: %s' % color
 
             return "background-color: %s" % color
 
         def highlight(x):
-            print(f"x: {x}")
-
             if x.State == "Closed":
                 # return [f'background-color: {self.get_fablib_manager().ERROR_LIGHT_COLOR}']*(len(fields))
                 color = f"{self.get_fablib_manager().ERROR_LIGHT_COLOR}"
             # elif x.State == 'None':
             #    return ['opacity: 50%']*(len(fields))
             # else:
             #    return ['background-color: ']*(len(fields))
```

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/images/fabric_logo.png` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/images/fabric_logo.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/images/server.png` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/images/server.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/images/slice_rack.png` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/images/slice_rack.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/abc_test.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/abc_test.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/component_tests.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/component_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,21 @@
 from .. import images
 
 
 class ComponentTest(AbcTest):
     COMPONENT_MODELS = {
         "GPU_Tesla_T4": ComponentModelType.GPU_Tesla_T4,
         "GPU_RTX6000": ComponentModelType.GPU_RTX6000,
+        "GPU_A30": ComponentModelType.GPU_A30,
+        "GPU_A40": ComponentModelType.GPU_A40,
         "SharedNIC_ConnectX_6": ComponentModelType.SharedNIC_ConnectX_6,
         "SmartNIC_ConnectX_6": ComponentModelType.SmartNIC_ConnectX_6,
         "SmartNIC_ConnectX_5": ComponentModelType.SmartNIC_ConnectX_5,
         "NVME_P4510": ComponentModelType.NVME_P4510,
+        "FPGA_Xilinx_U280": ComponentModelType.FPGA_Xilinx_U280
     }
 
     def __init__(self):
         """
         Constructor
         :return:
         """
```

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/hello_fabric.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/hello_fabric.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/link_benchmark.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/link_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/local_network_benchmark.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/local_network_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/network_benchmark_tests.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/network_benchmark_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/nvme_benchmark.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/nvme_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/test_basic.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/utils/abc_utils.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/utils/abc_utils.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/utils/node.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/utils/node.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/utils/slice.py` & `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/utils/slice.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc3/pyproject.toml` & `fabrictestbed-extensions-1.5.0rc4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -6,36 +6,38 @@
 name = "fabrictestbed-extensions"
 # Bump version up in top-level __init.py__.
 dynamic = ["version"]
 description = "FABRIC Python Client Library and CLI Extensions"
 authors = [
     {name="Paul Ruth", email="pruth@renci.org"},
     {name="Komal Thareja", email="kthare10@renci.org"}
-]
+    ]
+
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE" }
 requires-python = ">=3.9"
 dependencies = [
     "ipycytoscape",
     "ipywidgets",
     "ipyleaflet",
     "ipycytoscape",
     "tabulate",
-    "fabrictestbed==1.5.0rc2",
+    "fabrictestbed==1.5.0",
     "paramiko",
     "jinja2>=3.0.0",
     "pandas",
     "numpy",
     "ipython>=8.12.0"
-]
+    ]
+
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-]
+    ]
 
 [project.urls]
 Homepage = "https://fabric-testbed.net/"
 Sources = "https://github.com/fabric-testbed/fabrictestbed-extensions"
 Documentation = "https://fabric-fablib.readthedocs.io/"
 ChangeLog = "https://github.com/fabric-testbed/fabrictestbed-extensions/blob/main/CHANGELOG.md"
```

### Comparing `fabrictestbed-extensions-1.5.0rc3/PKG-INFO` & `fabrictestbed-extensions-1.5.0rc4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: fabrictestbed-extensions
-Version: 1.5.0rc3
+Version: 1.5.0rc4
 Summary: FABRIC Python Client Library and CLI Extensions
 Author-email: Paul Ruth <pruth@renci.org>, Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: ipycytoscape
 Requires-Dist: ipywidgets
 Requires-Dist: ipyleaflet
 Requires-Dist: ipycytoscape
 Requires-Dist: tabulate
-Requires-Dist: fabrictestbed==1.5.0rc2
+Requires-Dist: fabrictestbed==1.5.0
 Requires-Dist: paramiko
 Requires-Dist: jinja2>=3.0.0
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: ipython>=8.12.0
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: furo ; extra == "doc"
```

