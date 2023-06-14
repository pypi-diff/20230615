# Comparing `tmp/PH-units-1.1.2.tar.gz` & `tmp/PH-units-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PH-units-1.1.2.tar", last modified: Fri Jun  9 13:54:58 2023, max compression
+gzip compressed data, was "dist/PH-units-1.1.3.tar", last modified: Wed Jun 14 23:40:00 2023, max compression
```

## Comparing `PH-units-1.1.2.tar` & `PH-units-1.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-09 13:54:58.000000 PH-units-1.1.2/
--rw-r--r--   0 runner     (501) staff       (20)       66 2023-06-09 13:53:32.000000 PH-units-1.1.2/.gitattributes
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-09 13:54:58.000000 PH-units-1.1.2/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-09 13:54:58.000000 PH-units-1.1.2/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     1781 2023-06-09 13:53:32.000000 PH-units-1.1.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner     (501) staff       (20)    35129 2023-06-09 13:53:32.000000 PH-units-1.1.2/LICENSE
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-09 13:54:58.000000 PH-units-1.1.2/PH_units.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2776 2023-06-09 13:54:58.000000 PH-units-1.1.2/PH_units.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      638 2023-06-09 13:54:58.000000 PH-units-1.1.2/PH_units.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-06-09 13:54:58.000000 PH-units-1.1.2/PH_units.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        9 2023-06-09 13:54:58.000000 PH-units-1.1.2/PH_units.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     2776 2023-06-09 13:54:58.000000 PH-units-1.1.2/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1689 2023-06-09 13:53:32.000000 PH-units-1.1.2/README.md
--rw-r--r--   0 runner     (501) staff       (20)       50 2023-06-09 13:53:32.000000 PH-units-1.1.2/dev-requirements.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-09 13:54:58.000000 PH-units-1.1.2/ph_units/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-09 13:53:32.000000 PH-units-1.1.2/ph_units/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5159 2023-06-09 13:53:32.000000 PH-units-1.1.2/ph_units/converter.py
--rw-r--r--   0 runner     (501) staff       (20)     1908 2023-06-09 13:53:32.000000 PH-units-1.1.2/ph_units/parser.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-09 13:54:58.000000 PH-units-1.1.2/ph_units/unit_types/
--rw-r--r--   0 runner     (501) staff       (20)     2784 2023-06-09 13:53:32.000000 PH-units-1.1.2/ph_units/unit_types/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      371 2023-06-09 13:53:32.000000 PH-units-1.1.2/ph_units/unit_types/_base.py
--rw-r--r--   0 runner     (501) staff       (20)      442 2023-06-09 13:53:32.000000 PH-units-1.1.2/ph_units/unit_types/area.py
--rw-r--r--   0 runner     (501) staff       (20)     2655 2023-06-09 13:53:32.000000 PH-units-1.1.2/ph_units/unit_types/energy.py
--rw-r--r--   0 runner     (501) staff       (20)     2571 2023-06-09 13:53:32.000000 PH-units-1.1.2/ph_units/unit_types/envelope.py
--rw-r--r--   0 runner     (501) staff       (20)     1459 2023-06-09 13:53:32.000000 PH-units-1.1.2/ph_units/unit_types/length.py
--rw-r--r--   0 runner     (501) staff       (20)     2093 2023-06-09 13:53:32.000000 PH-units-1.1.2/ph_units/unit_types/power.py
--rw-r--r--   0 runner     (501) staff       (20)     1176 2023-06-09 13:53:32.000000 PH-units-1.1.2/ph_units/unit_types/speed.py
--rw-r--r--   0 runner     (501) staff       (20)      796 2023-06-09 13:53:32.000000 PH-units-1.1.2/ph_units/unit_types/temperature.py
--rw-r--r--   0 runner     (501) staff       (20)      917 2023-06-09 13:53:32.000000 PH-units-1.1.2/ph_units/unit_types/volume.py
--rw-r--r--   0 runner     (501) staff       (20)     1705 2023-06-09 13:53:32.000000 PH-units-1.1.2/ph_units/unit_types/volume_flow.py
--rw-r--r--   0 runner     (501) staff       (20)      219 2023-06-09 13:53:32.000000 PH-units-1.1.2/sandbox.py
--rw-r--r--   0 runner     (501) staff       (20)      832 2023-06-09 13:54:58.000000 PH-units-1.1.2/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      263 2023-06-09 13:53:32.000000 PH-units-1.1.2/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 23:40:00.000000 PH-units-1.1.3/
+-rw-r--r--   0 runner     (501) staff       (20)       66 2023-06-14 23:38:11.000000 PH-units-1.1.3/.gitattributes
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 23:40:00.000000 PH-units-1.1.3/.github/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 23:40:00.000000 PH-units-1.1.3/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     1781 2023-06-14 23:38:11.000000 PH-units-1.1.3/.github/workflows/ci.yaml
+-rw-r--r--   0 runner     (501) staff       (20)    35129 2023-06-14 23:38:11.000000 PH-units-1.1.3/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 23:40:00.000000 PH-units-1.1.3/PH_units.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     2776 2023-06-14 23:39:59.000000 PH-units-1.1.3/PH_units.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      638 2023-06-14 23:40:00.000000 PH-units-1.1.3/PH_units.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-06-14 23:39:59.000000 PH-units-1.1.3/PH_units.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        9 2023-06-14 23:39:59.000000 PH-units-1.1.3/PH_units.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     2776 2023-06-14 23:40:00.000000 PH-units-1.1.3/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1689 2023-06-14 23:38:11.000000 PH-units-1.1.3/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       50 2023-06-14 23:38:11.000000 PH-units-1.1.3/dev-requirements.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 23:40:00.000000 PH-units-1.1.3/ph_units/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5159 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/converter.py
+-rw-r--r--   0 runner     (501) staff       (20)     1908 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/parser.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 23:40:00.000000 PH-units-1.1.3/ph_units/unit_types/
+-rw-r--r--   0 runner     (501) staff       (20)     2784 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      371 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/_base.py
+-rw-r--r--   0 runner     (501) staff       (20)      442 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/area.py
+-rw-r--r--   0 runner     (501) staff       (20)     4466 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/energy.py
+-rw-r--r--   0 runner     (501) staff       (20)     2571 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/envelope.py
+-rw-r--r--   0 runner     (501) staff       (20)     1459 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/length.py
+-rw-r--r--   0 runner     (501) staff       (20)     2093 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/power.py
+-rw-r--r--   0 runner     (501) staff       (20)     1176 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/speed.py
+-rw-r--r--   0 runner     (501) staff       (20)      796 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/temperature.py
+-rw-r--r--   0 runner     (501) staff       (20)      917 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/volume.py
+-rw-r--r--   0 runner     (501) staff       (20)     1705 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/volume_flow.py
+-rw-r--r--   0 runner     (501) staff       (20)      219 2023-06-14 23:38:11.000000 PH-units-1.1.3/sandbox.py
+-rw-r--r--   0 runner     (501) staff       (20)      832 2023-06-14 23:40:00.000000 PH-units-1.1.3/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      263 2023-06-14 23:38:11.000000 PH-units-1.1.3/setup.py
```

### Comparing `PH-units-1.1.2/.github/workflows/ci.yaml` & `PH-units-1.1.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.2/LICENSE` & `PH-units-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.2/PH_units.egg-info/PKG-INFO` & `PH-units-1.1.3/PH_units.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PH-units
-Version: 1.1.2
+Version: 1.1.3
 Summary: Tools for working with common Passive House unit types
 Home-page: https://github.com/PH-Tools/PH_units
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # PH-Units:
         A package for converting common Passive House unit types (IP | SI).
```

### Comparing `PH-units-1.1.2/PH_units.egg-info/SOURCES.txt` & `PH-units-1.1.3/PH_units.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.2/PKG-INFO` & `PH-units-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PH-units
-Version: 1.1.2
+Version: 1.1.3
 Summary: Tools for working with common Passive House unit types
 Home-page: https://github.com/PH-Tools/PH_units
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # PH-Units:
         A package for converting common Passive House unit types (IP | SI).
```

### Comparing `PH-units-1.1.2/README.md` & `PH-units-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.2/ph_units/converter.py` & `PH-units-1.1.3/ph_units/converter.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.2/ph_units/parser.py` & `PH-units-1.1.3/ph_units/parser.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.2/ph_units/unit_types/__init__.py` & `PH-units-1.1.3/ph_units/unit_types/__init__.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.2/ph_units/unit_types/energy.py` & `PH-units-1.1.3/ph_units/unit_types/energy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,104 @@
 # -*- coding: utf-8 -*-
 # -*- Python Version: 2.7 -*-
 
 from ph_units.unit_types._base import Base_UnitType
 
 
-class WattHoursPerMeterCubed(Base_UnitType):
-    """WH/M3"""
+class WattHour(Base_UnitType):
+    """Wh"""
 
-    __symbol__ = "WH/M3"
+    __symbol__ = "WH"
     __aliases__ = []
-    __factors__ = {"WH/M3": "{}*1", "W/CFM": "{}*1.699010796"}
+    __factors__ = {
+        "WH": "{}*1",
+        "KWH": "{}*0.001",
+        "BTU": "{}*3.41214",
+        "KBTU": "{}*0.00341214",
+        "MJ": "{}*0.0036",
+        "KJ": "{}*3.6",
+    }
+
+
+class KiloWattHour(Base_UnitType):
+    """KWH"""
+
+    __symbol__ = "KWH"
+    __aliases__ = []
+    __factors__ = {
+        "WH": "{}*1000",
+        "KWH": "{}*1",
+        "BTU": "{}*3412.14",
+        "KBTU": "{}*3.41214",
+        "MJ": "{}*3.6",
+        "KJ": "{}*3600",
+    }
+
+
+class BTU(Base_UnitType):
+    """BTU"""
+
+    __symbol__ = "BTU"
+    __aliases__ = []
+    __factors__ = {
+        "WH": "{}*0.293071",
+        "KWH": "{}*0.000293071",
+        "BTU": "{}*1",
+        "KBTU": "{}*0.001",
+        "MJ": "{}*0.00105506",
+        "KJ": "{}*1.05506",
+    }
+
+
+class KiloBTU(Base_UnitType):
+    """KBTU"""
+
+    __symbol__ = "KBTU"
+    __aliases__ = []
+    __factors__ = {
+        "WH": "{}*293.071",
+        "KWH": "{}*0.293071",
+        "BTU": "{}*1000",
+        "KBTU": "{}*1",
+        "MJ": "{}*1.05506",
+        "KJ": "{}*1055.06",
+    }
+
+
+class MegaJoule(Base_UnitType):
+    """MJ"""
+
+    __symbol__ = "MJ"
+    __aliases__ = []
+    __factors__ = {
+        "WH": "{}*277.778",
+        "KWH": "{}*0.277778",
+        "BTU": "{}*947.817",
+        "KBTU": "{}*0.947817",
+        "MJ": "{}*1",
+        "KJ": "{}*1000",
+    }
+
+
+class KiloJoule(Base_UnitType):
+    """KJ"""
+
+    __symbol__ = "KJ"
+    __aliases__ = []
+    __factors__ = {
+        "WH": "{}*0.277778",
+        "KWH": "{}*0.000277778",
+        "BTU": "{}*0.947817",
+        "KBTU": "{}*0.000947817",
+        "MJ": "{}*0.001",
+        "KJ": "{}*1",
+    }
+
+
+# ----------------- Energy Per Area -----------------
 
 
 class WattHoursPerKilometerSquared(Base_UnitType):
     """WH/KM2"""
 
     __symbol__ = "WH/KM2"
     __aliases__ = []
@@ -106,13 +191,24 @@
         "KWH/M2": "{}*0.00315459",
         "KWH/FT2": "{}*0.000293071",
         "BTU/FT2": "{}*1",
         "KBTU/FT2": "{}*0.001",
     }
 
 
+# ----------------- Energy Per Volume -----------------
+
+
+class WattHoursPerMeterCubed(Base_UnitType):
+    """WH/M3"""
+
+    __symbol__ = "WH/M3"
+    __aliases__ = []
+    __factors__ = {"WH/M3": "{}*1", "W/CFM": "{}*1.699010796"}
+
+
 class MegaJoulePerMeterCubedKelvin(Base_UnitType):
     """MJ/M3K"""
 
     __symbol__ = "MJ/M3K"
     __aliases__ = []
     __factors__ = {"MJ/M3K": "{}*1", "BTU/FT3-F": "{}*14.91066014"}
```

### Comparing `PH-units-1.1.2/ph_units/unit_types/envelope.py` & `PH-units-1.1.3/ph_units/unit_types/envelope.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.2/ph_units/unit_types/length.py` & `PH-units-1.1.3/ph_units/unit_types/length.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.2/ph_units/unit_types/power.py` & `PH-units-1.1.3/ph_units/unit_types/power.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.2/ph_units/unit_types/speed.py` & `PH-units-1.1.3/ph_units/unit_types/speed.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.2/ph_units/unit_types/temperature.py` & `PH-units-1.1.3/ph_units/unit_types/temperature.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.2/ph_units/unit_types/volume.py` & `PH-units-1.1.3/ph_units/unit_types/volume.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.2/ph_units/unit_types/volume_flow.py` & `PH-units-1.1.3/ph_units/unit_types/volume_flow.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.2/setup.cfg` & `PH-units-1.1.3/setup.cfg`

 * *Files identical despite different names*

