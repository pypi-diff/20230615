# Comparing `tmp/cpumodel-0.0.1.tar.gz` & `tmp/cpumodel-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpumodel-0.0.1.tar", max compression
+gzip compressed data, was "cpumodel-0.0.2.tar", max compression
```

## Comparing `cpumodel-0.0.1.tar` & `cpumodel-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2274 2023-06-14 14:50:19.261502 cpumodel-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-14 14:50:19.261502 cpumodel-0.0.1/cpumodel/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 14:50:19.261502 cpumodel-0.0.1/cpumodel/__main__.py
--rw-r--r--   0        0        0     2084 2023-06-14 14:50:19.261502 cpumodel-0.0.1/cpumodel/amd.py
--rw-r--r--   0        0        0     2629 2023-06-14 14:50:19.261502 cpumodel-0.0.1/cpumodel/cpumodel.py
--rw-r--r--   0        0        0     5202 2023-06-14 14:50:19.261502 cpumodel-0.0.1/cpumodel/intel.py
--rw-r--r--   0        0        0      435 2023-06-14 14:50:41.473961 cpumodel-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2735 1970-01-01 00:00:00.000000 cpumodel-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     4521 2023-06-15 11:41:57.719245 cpumodel-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-15 11:41:57.719245 cpumodel-0.0.2/cpumodel/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 11:41:57.719245 cpumodel-0.0.2/cpumodel/__main__.py
+-rw-r--r--   0        0        0     2078 2023-06-15 11:41:57.719245 cpumodel-0.0.2/cpumodel/amd.py
+-rw-r--r--   0        0        0     3371 2023-06-15 11:41:57.719245 cpumodel-0.0.2/cpumodel/cpumodel.py
+-rw-r--r--   0        0        0     5506 2023-06-15 11:41:57.719245 cpumodel-0.0.2/cpumodel/intel.py
+-rw-r--r--   0        0        0      455 2023-06-15 11:42:21.788808 cpumodel-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5023 1970-01-01 00:00:00.000000 cpumodel-0.0.2/PKG-INFO
```

### Comparing `cpumodel-0.0.1/cpumodel/amd.py` & `cpumodel-0.0.2/cpumodel/amd.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,30 +21,30 @@
         cpulabels['cpuFamily'] = result.group(2)
         cpulabels['cpuGeneration'] = result.group(3)
         cpulabels['cpuLetter'] = result.group(4)
     elif 'EPYC' in cpu:
         # AMD EPYC 7J13 64-Core Processor
         # AMD EPYC 7742 64-Core Processor
         # AMD EPYC 7551P 32-Core Processor
-        result = re.search(r"AMD ((\w+ \d) (\d)\w{3}([A-Z]?))", cpu)
+        result = re.search(r"AMD ((\w+) (\d)\w{3}([A-Z]?))", cpu)
         cpulabels['cpuModel'] = result.group(1)
         cpulabels['cpuFamily'] = result.group(2)
         cpulabels['cpuGeneration'] = result.group(3)
         cpulabels['cpuLetter'] = result.group(4)
     elif 'Opteron' in cpu:
         # AMD Opteron(tm) Processor 4133
         # AMD Opteron(tm) Processor 4310 EE
         # AMD Opteron(tm) Processor 6366 HE
         # Quad-Core AMD Opteron(tm) Processor 8356
         # Six-Core AMD Opteron(tm) Processor 8431
-        result = re.search(r"AMD ((\w+) (\d{4}) ?([A-Z]{1,2}?)))", cpu)
+        result = re.search(r"AMD ((\w+) (\d{4}) ?([A-Z]{1,2}?))", cpu)
         cpulabels['cpuModel'] = result.group(1)
         cpulabels['cpuFamily'] = result.group(2)
         cpulabels['cpuGeneration'] = result.group(3)
         cpulabels['cpuLetter'] = result.group(4)
     elif 'APU' in cpu:
         # AMD Athlon(tm) 5350 APU with Radeon(tm) R3
-        result = re.search(r"AMD (((\w+) (\d)\d+) APU)", cpu)
+        result = re.search(r"AMD ((\w+) (\d)\d+ APU)", cpu)
         cpulabels['cpuModel'] = result.group(1)
         cpulabels['cpuFamily'] = result.group(2)
         cpulabels['cpuGeneration'] = result.group(3)
     return cpulabels
```

### Comparing `cpumodel-0.0.1/cpumodel/cpumodel.py` & `cpumodel-0.0.2/cpumodel/cpumodel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 A Python library to parse and return various attributes from the CPU string
 """
 import re
+import argparse
 from cpuinfo import get_cpu_info
 from .intel import parse_intel_cpu
 from .amd import parse_amd_cpu
 
 def map_vendor(vendor):
     """
     Rewrite vendor name
@@ -14,14 +15,23 @@
         returnval = 'Intel'
     elif vendor == 'AuthenticAMD':
         returnval = 'AMD'
     else:
         returnval = vendor
     return returnval
 
+def guess_vendor(cpustring):
+    """
+    Attempt to guess a CPU vendor from its string
+    """
+    if 'Intel' in cpustring:
+        vendor = 'Intel'
+    elif 'AMD' in cpustring:
+        vendor = 'AMD'
+    return vendor
 
 def clean_cpu_string(brand):
     """
     Rewrite CPU string more neatly.
     
     This:
         Intel(R) Core(TM) i5-6300U CPU @ 2.40GHz
@@ -31,23 +41,26 @@
     # Strip annoying chars
     brand = brand.replace('(R)', '')
     brand = brand.replace('(TM)', '')
     brand = brand.replace('(tm)', '')
     brand = brand.replace('CPU', '')
     brand = brand.replace('Processor', '')
 
-    # Delete multiple spaces
-    re.sub(' +', ' ', brand)
-
     # Drop the '@ 2.40GHz' suffix
     brand = brand.split('@')[0]
 
     # Drop the 'with Radeon Graphics' suffix
     brand = brand.split('with')[0]
+
+    # Drop '64-Core'
+    brand = re.sub(r"\d+-Core", '', brand)
+
+    # Delete multiple spaces
     brand = brand.strip()
+    brand = re.sub(r'\s+', ' ', brand)
 
     return brand
 
 
 def drop_nones_inplace(d: dict) -> dict:
     """Recursively drop Nones in dict d in-place and return original dict"""
     dd = drop_nones(d)
@@ -68,20 +81,27 @@
             dd[k] = type(v)(drop_nones(vv) if isinstance(vv, dict) else vv
                             for vv in v)
         elif v is not None:
             dd[k] = v
     return dd
 
 
-def get_cpu_model():
+def get_cpu_model(cpustring):
     """
     Get info about the CPU model and return it as a dict
     """
-    # Fetch CPU info
-    cpuinfo = get_cpu_info()
+
+    if cpustring:
+        # Use supplied CPU string
+        cpuinfo = {}
+        cpuinfo['vendor_id_raw'] = guess_vendor(cpustring)
+        cpuinfo['brand_raw'] = cpustring
+    else:
+        # Fetch CPU info from system
+        cpuinfo = get_cpu_info()
 
     # Generate basic labels
     labels = {}
     labels['cpuVendor'] = map_vendor(cpuinfo['vendor_id_raw'])
     labels['cpuString'] = clean_cpu_string(cpuinfo['brand_raw'])
 
     # Calculate some extra labels
@@ -95,12 +115,18 @@
 
     return labels
 
 def main():
     """
     Display CPU model info to a human user
     """
-    labels = get_cpu_model()
+
+    # Read in args
+    parser = argparse.ArgumentParser()
+    parser.add_argument('-t', '--test', help="Supply a CPU string rather than obtaining it from the system", type=str)
+    args = parser.parse_args()
+
+    labels = get_cpu_model(args.test)
     print(labels)
 
 if __name__ == '__main__':
     main()
```

### Comparing `cpumodel-0.0.1/cpumodel/intel.py` & `cpumodel-0.0.2/cpumodel/intel.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         # Intel(R) Xeon(R) Bronze 3104 CPU @ 1.70GHz
         result = re.search(r"Intel ((Xeon \w+) (\d)\d{3}(\w)?)", cpu)
         cpulabels['cpuModel'] = result.group(1)
         cpulabels['cpuFamily'] = result.group(2)
         cpulabels['cpuGeneration'] = result.group(3)
         cpulabels['cpuLetter'] = result.group(4)
 
-    elif 'E5' in cpu or 'E3' in cpu:
+    elif 'E5-' in cpu or 'E3-' in cpu:
         # Intel(R) Xeon(R) CPU E5-2670 0 @ 2.60GHz
         # Intel(R) Xeon(R) CPU E5-2430L 0 @ 2.00GHz
         # Intel(R) Xeon(R) CPU E5-2687W 0 @ 3.10GHz
         # Intel(R) Xeon(R) CPU E5-4640 v2 @ 2.20GHz
         # Intel(R) Xeon(R) CPU E5-2630 v3 @ 2.40GHz
         # Intel(R) Xeon(R) CPU E5-2630 v4 @ 2.20GHz
         # Intel(R) Xeon(R) CPU E3-1220 v5 @ 3.00GHz
@@ -76,16 +76,23 @@
         # Intel(R) Xeon(R) W-2125 CPU @ 4.00GHz
         result = re.search(r"Intel ((Xeon \w)-?(\d)\d{3}(\w)?)", cpu)
         cpulabels['cpuModel'] = result.group(1)
         cpulabels['cpuFamily'] = result.group(2)
         cpulabels['cpuGeneration'] = result.group(3)
         cpulabels['cpuLetter'] = result.group(4)
 
-    elif 'Core' in cpu:
+    elif 'i7 ' in cpu or 'i5 ' in cpu or 'i3 ' in cpu:
         # Intel(R) Core(TM) i7 CPU         920  @ 2.67GHz
+        result = re.search(r"(Core i\d) \d{3}(\w)?", cpu)
+        cpulabels['cpuModel'] = result.group(0)
+        cpulabels['cpuFamily'] = result.group(1)
+        cpulabels['cpuGeneration'] = 1
+        cpulabels['cpuLetter'] = result.group(2)
+
+    elif 'Core' in cpu:
         # Intel(R) Core(TM) i7-2600 CPU @ 3.40GHz
         # Intel(R) Core(TM) i7-2600S CPU @ 2.80GHz
         # Intel(R) Core(TM) i5-2410M CPU @ 2.30GHz
         # Intel(R) Core(TM) i5-3470T CPU @ 2.90GHz
         # Intel(R) Core(TM) i7-3770 CPU @ 3.40GHz
         # Intel(R) Core(TM) i7-3770S CPU @ 3.10GHz
         # Intel(R) Core(TM) i5-4590T CPU @ 2.00GHz
@@ -102,14 +109,14 @@
         # Intel(R) Core(TM) i7-8086K CPU @ 4.00GHz
         # Intel(R) Core(TM) i3-9100 CPU @ 3.60GHz
         # Intel(R) Core(TM) i9-9900K CPU @ 3.60GHz
         # Intel(R) Core(TM) i7-10700K CPU @ 3.80GHz
         # Intel(R) Core(TM) i9-10900 CPU @ 2.80GHz
         # Intel(R) Core(TM) i9-10900X CPU @ 3.70GHz
         # Intel(R) Core(TM) i9-10980XE CPU @ 3.00GHz
-        result = re.search(r"(Core i\d)-(\d)?\d{3,4}(\w)?", cpu)
+        result = re.search(r"(Core i\d)-(\d{1,2})?\d{3}(\w)?", cpu)
         cpulabels['cpuModel'] = result.group(0)
         cpulabels['cpuFamily'] = result.group(1)
         cpulabels['cpuGeneration'] = result.group(2)
         cpulabels['cpuLetter'] = result.group(3)
 
     return cpulabels
```

