# Comparing `tmp/indexed-png-stats-0.0.1.tar.gz` & `tmp/indexed-png-stats-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indexed-png-stats-0.0.1.tar", last modified: Wed Jun 14 04:56:16 2023, max compression
+gzip compressed data, was "indexed-png-stats-0.0.2.tar", last modified: Thu Jun 15 00:27:00 2023, max compression
```

## Comparing `indexed-png-stats-0.0.1.tar` & `indexed-png-stats-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-06-14 04:56:16.331990 indexed-png-stats-0.0.1/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      685 2023-06-14 04:56:16.331990 indexed-png-stats-0.0.1/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1129 2023-06-14 04:53:54.000000 indexed-png-stats-0.0.1/README.md
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2023-06-14 04:56:16.331990 indexed-png-stats-0.0.1/setup.cfg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1154 2023-06-14 04:50:52.000000 indexed-png-stats-0.0.1/setup.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-06-14 04:56:16.331990 indexed-png-stats-0.0.1/src/
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-06-14 04:56:16.331990 indexed-png-stats-0.0.1/src/indexed_png_stats/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2023-06-14 03:58:34.000000 indexed-png-stats-0.0.1/src/indexed_png_stats/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5744 2023-06-14 04:50:25.000000 indexed-png-stats-0.0.1/src/indexed_png_stats/generate.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-06-14 04:56:16.331990 indexed-png-stats-0.0.1/src/indexed_png_stats.egg-info/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      685 2023-06-14 04:56:16.000000 indexed-png-stats-0.0.1/src/indexed_png_stats.egg-info/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      358 2023-06-14 04:56:16.000000 indexed-png-stats-0.0.1/src/indexed_png_stats.egg-info/SOURCES.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2023-06-14 04:56:16.000000 indexed-png-stats-0.0.1/src/indexed_png_stats.egg-info/dependency_links.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       75 2023-06-14 04:56:16.000000 indexed-png-stats-0.0.1/src/indexed_png_stats.egg-info/entry_points.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       13 2023-06-14 04:56:16.000000 indexed-png-stats-0.0.1/src/indexed_png_stats.egg-info/requires.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       18 2023-06-14 04:56:16.000000 indexed-png-stats-0.0.1/src/indexed_png_stats.egg-info/top_level.txt
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-06-15 00:27:00.141223 indexed-png-stats-0.0.2/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      198 2023-06-15 00:25:51.000000 indexed-png-stats-0.0.2/CHANGES.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       48 2023-06-14 03:58:06.000000 indexed-png-stats-0.0.2/DESCRIPTION.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 indexed-png-stats-0.0.2/MANIFEST.in
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      860 2023-06-15 00:27:00.141223 indexed-png-stats-0.0.2/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1159 2023-06-15 00:25:51.000000 indexed-png-stats-0.0.2/README.md
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2023-06-15 00:27:00.141223 indexed-png-stats-0.0.2/setup.cfg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1154 2023-06-15 00:26:16.000000 indexed-png-stats-0.0.2/setup.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-06-15 00:27:00.141223 indexed-png-stats-0.0.2/src/
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-06-15 00:27:00.141223 indexed-png-stats-0.0.2/src/indexed_png_stats/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2023-06-14 03:58:34.000000 indexed-png-stats-0.0.2/src/indexed_png_stats/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6014 2023-06-15 00:24:47.000000 indexed-png-stats-0.0.2/src/indexed_png_stats/generate.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-06-15 00:27:00.141223 indexed-png-stats-0.0.2/src/indexed_png_stats.egg-info/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      860 2023-06-15 00:26:59.000000 indexed-png-stats-0.0.2/src/indexed_png_stats.egg-info/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      398 2023-06-15 00:27:00.000000 indexed-png-stats-0.0.2/src/indexed_png_stats.egg-info/SOURCES.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2023-06-15 00:26:59.000000 indexed-png-stats-0.0.2/src/indexed_png_stats.egg-info/dependency_links.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       75 2023-06-15 00:26:59.000000 indexed-png-stats-0.0.2/src/indexed_png_stats.egg-info/entry_points.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       13 2023-06-15 00:26:59.000000 indexed-png-stats-0.0.2/src/indexed_png_stats.egg-info/requires.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       18 2023-06-15 00:26:59.000000 indexed-png-stats-0.0.2/src/indexed_png_stats.egg-info/top_level.txt
```

### Comparing `indexed-png-stats-0.0.1/README.md` & `indexed-png-stats-0.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 ```
 pip install indexed-png-stats
 ```
 
 ## Command-line
 
 ```
-usage: indexed-png-stats [-h] -d DIR [-r] [-t {summary,per-file}]
+usage: indexed-png-stats [-h] -d DIR [DIR ...] [-r] [-t {summary,per-file}]
                          [-f {plain-text,json}] [-o FILE] [-v]
 
 Generates statistics from indexed PNG files.
 
 optional arguments:
   -h, --help            show this help message and exit
-  -d DIR, --image_dir DIR
+  -d DIR [DIR ...], --image_dir DIR [DIR ...]
                         the directory with the PNG files (default: None)
   -r, --recursive       whether to scan the directory recursively (default:
                         False)
   -t {summary,per-file}, --stats_type {summary,per-file}
                         the type of statistics to generate (default: summary)
   -f {plain-text,json}, --output_format {plain-text,json}
                         how to present the statistics (default: plain-text)
```

### Comparing `indexed-png-stats-0.0.1/setup.py` & `indexed-png-stats-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     },
     packages=find_namespace_packages(where='src'),
     entry_points={
         "console_scripts": [
             "indexed-png-stats=indexed_png_stats.generate:sys_main",
         ]
     },
-    version="0.0.1",
+    version="0.0.2",
     author='Peter Reutemann',
     author_email='fracpete@waikato.ac.nz',
     install_requires=[
         "pillow",
         "numpy",
     ]
 )
```

### Comparing `indexed-png-stats-0.0.1/src/indexed_png_stats/generate.py` & `indexed-png-stats-0.0.2/src/indexed_png_stats/generate.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,84 +21,86 @@
     OUTPUT_FORMAT_JSON,
 ]
 
 
 SUMMARY_ENTRY = "all"
 
 
-def collect(stats, image_dir, recursive=False, stats_type=STATS_TYPE_SUMMARY, verbose=False):
+def collect(stats, image_dirs, recursive=False, stats_type=STATS_TYPE_SUMMARY, verbose=False):
     """
     Collects the statistics from the indexed PNG files.
 
     :param stats: the stats to append to
     :type stats: dict
-    :param image_dir: the directory to look for PNG files
-    :type image_dir: str
+    :param image_dirs: the directory to look for PNG files
+    :type image_dirs: str
     :param recursive: whether to search recursively for PNG files
     :type recursive: bool
     :param stats_type: the type of stats to generate
     :type stats_type: str
     :param verbose: whether to output some logging information
     :type verbose: bool
     """
-    if verbose:
-        print("Entering: %s" % image_dir)
-    for f in os.listdir(image_dir):
-        full = os.path.join(image_dir, f)
-
-        # recurse?
-        if recursive and os.path.isdir(full):
-            collect(stats, full, recursive=True, stats_type=stats_type)
-            print("Back in: %s" % image_dir)
-
-        # png?
-        if f.lower().endswith(".png"):
-            if verbose:
-                print("%s" % f)
-
-            # indexed?
-            try:
-                img = Image.open(full)
-                p = img.getpalette()
-            except:
-                p = None
-            if p is None:
+    for image_dir in image_dirs:
+        if verbose:
+            print("Entering: %s" % image_dir)
+        for f in os.listdir(image_dir):
+            full = os.path.join(image_dir, f)
+
+            # recurse?
+            if recursive and os.path.isdir(full):
+                collect(stats, full, recursive=True, stats_type=stats_type)
+                print("Back in: %s" % image_dir)
+
+            # png?
+            if f.lower().endswith(".png"):
                 if verbose:
-                    print("  no palette information")
-                continue
+                    print("%s" % f)
 
-            # get stats
-            img = np.array(img)
-            unique, counts = np.unique(img, return_counts=True)
-
-            # summary
-            if stats_type == STATS_TYPE_SUMMARY:
-                for i in range(len(unique)):
-                    v = unique[i]
-                    c = counts[i]
-                    l = str(v)
-                    if len(stats) == 0:
-                        stats[SUMMARY_ENTRY] = dict()
-                    if l not in stats[SUMMARY_ENTRY]:
-                        stats[SUMMARY_ENTRY][l] = 0
-                    stats[SUMMARY_ENTRY][l] += int(c)
-                pass
-
-            # per file
-            elif stats_type == STATS_TYPE_PERFILE:
-                stats[full] = dict()
-                for i in range(len(unique)):
-                    v = unique[i]
-                    c = counts[i]
-                    l = str(v)
-                    stats[full][l] = int(c)
-
-            # unsupported
-            else:
-                raise Exception("Unsupported stats type: %s" % stats_type)
+                # indexed?
+                try:
+                    img = Image.open(full)
+                    p = img.getpalette()
+                except:
+                    img = None
+                    p = None
+                if p is None:
+                    if verbose:
+                        print("  no palette information")
+                    continue
+
+                # get stats
+                img = np.array(img)
+                unique, counts = np.unique(img, return_counts=True)
+
+                # summary
+                if stats_type == STATS_TYPE_SUMMARY:
+                    for i in range(len(unique)):
+                        v = unique[i]
+                        c = counts[i]
+                        l = str(v)
+                        if len(stats) == 0:
+                            stats[SUMMARY_ENTRY] = dict()
+                        if l not in stats[SUMMARY_ENTRY]:
+                            stats[SUMMARY_ENTRY][l] = 0
+                        stats[SUMMARY_ENTRY][l] += int(c)
+                    pass
+
+                # per file
+                elif stats_type == STATS_TYPE_PERFILE:
+                    stats[full] = dict()
+                    for i in range(len(unique)):
+                        v = unique[i]
+                        c = counts[i]
+                        l = str(v)
+                        stats[full][l] = int(c)
+
+                # unsupported
+                else:
+                    raise Exception("Unsupported stats type: %s" % stats_type)
 
 
 def output_stats(stats, output_format=OUTPUT_FORMAT_PLAINTEXT, output_file=None):
     # plain text
     if output_format == OUTPUT_FORMAT_PLAINTEXT:
         output = []
         for k in stats:
@@ -139,15 +141,15 @@
     :param args: the commandline arguments, uses sys.argv if not supplied
     :type args: list
     """
     parser = argparse.ArgumentParser(
         description="Generates statistics from indexed PNG files.",
         prog="indexed-png-stats",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    parser.add_argument("-d", "--image_dir", metavar="DIR", help="the directory with the PNG files", required=True)
+    parser.add_argument("-d", "--image_dir", metavar="DIR", nargs="+", help="the directory with the PNG files", required=True)
     parser.add_argument("-r", "--recursive", action="store_true", help="whether to scan the directory recursively", required=False)
     parser.add_argument("-t", "--stats_type", choices=STATS_TYPES, default=STATS_TYPE_SUMMARY, help="the type of statistics to generate", required=False)
     parser.add_argument("-f", "--output_format", choices=OUTPUT_FORMATS, default=OUTPUT_FORMAT_PLAINTEXT, help="how to present the statistics", required=False)
     parser.add_argument("-o", "--output_file", metavar="FILE", default=None, help="the file to store the generated statistics in", required=False)
     parser.add_argument("-v", "--verbose", action="store_true", help="whether to be more verbose with the processing", required=False)
     parsed = parser.parse_args(args=args)
     stats = dict()
```

