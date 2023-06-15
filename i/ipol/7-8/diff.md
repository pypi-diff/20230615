# Comparing `tmp/ipol-7.tar.gz` & `tmp/ipol-8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipol-7.tar", last modified: Mon Jun 12 07:23:07 2023, max compression
+gzip compressed data, was "ipol-8.tar", last modified: Thu Jun 15 17:10:04 2023, max compression
```

## Comparing `ipol-7.tar` & `ipol-8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-12 07:23:07.034428 ipol-7/
--rw-rw-r--   0 coco      (1000) coco      (1000)      516 2023-06-12 07:23:07.034428 ipol-7/PKG-INFO
--rw-rw-r--   0 coco      (1000) coco      (1000)     5382 2023-06-07 14:47:16.000000 ipol-7/README
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-12 07:23:07.034428 ipol-7/idl/
--rw-rw-r--   0 coco      (1000) coco      (1000)      543 2023-06-07 15:25:08.000000 ipol-7/idl/ace.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      769 2023-06-07 15:32:52.000000 ipol-7/idl/bm3d.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      545 2023-06-06 13:51:32.000000 ipol-7/idl/dctdenoise.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      756 2023-06-08 13:41:08.000000 ipol-7/idl/ffdnet.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      280 2020-12-08 23:32:50.000000 ipol-7/idl/lsd.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      996 2023-06-06 13:02:24.000000 ipol-7/idl/msdctd.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      677 2023-06-07 15:27:57.000000 ipol-7/idl/nlbayes.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      482 2023-06-07 15:14:38.000000 ipol-7/idl/nlm.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      283 2023-06-07 14:25:58.000000 ipol-7/idl/phs.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      441 2020-12-08 18:01:47.000000 ipol-7/idl/scb.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      537 2023-06-07 18:11:57.000000 ipol-7/idl/tvdenoise.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      376 2023-06-07 14:25:05.000000 ipol-7/idl/tvl1.Dockerfile
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-12 07:23:07.034428 ipol-7/ipol.egg-info/
--rw-rw-r--   0 coco      (1000) coco      (1000)      516 2023-06-12 07:23:07.000000 ipol-7/ipol.egg-info/PKG-INFO
--rw-rw-r--   0 coco      (1000) coco      (1000)      388 2023-06-12 07:23:07.000000 ipol-7/ipol.egg-info/SOURCES.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-06-12 07:23:07.000000 ipol-7/ipol.egg-info/dependency_links.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)        5 2023-06-12 07:23:07.000000 ipol-7/ipol.egg-info/top_level.txt
--rwxrwxr-x   0 coco      (1000) coco      (1000)    18980 2023-06-12 07:22:51.000000 ipol-7/ipol.py
--rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-06-12 07:23:07.034428 ipol-7/setup.cfg
--rw-rw-r--   0 coco      (1000) coco      (1000)      641 2023-06-12 07:22:27.000000 ipol-7/setup.py
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-15 17:10:04.759934 ipol-8/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      516 2023-06-15 17:10:04.759934 ipol-8/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5382 2023-06-07 14:47:16.000000 ipol-8/README
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-15 17:10:04.755934 ipol-8/idl/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      543 2023-06-07 15:25:08.000000 ipol-8/idl/ace.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      769 2023-06-07 15:32:52.000000 ipol-8/idl/bm3d.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      545 2023-06-06 13:51:32.000000 ipol-8/idl/dctdenoise.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      756 2023-06-08 13:41:08.000000 ipol-8/idl/ffdnet.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      280 2020-12-08 23:32:50.000000 ipol-8/idl/lsd.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      996 2023-06-06 13:02:24.000000 ipol-8/idl/msdctd.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      677 2023-06-07 15:27:57.000000 ipol-8/idl/nlbayes.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      482 2023-06-07 15:14:38.000000 ipol-8/idl/nlm.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      283 2023-06-07 14:25:58.000000 ipol-8/idl/phs.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      441 2020-12-08 18:01:47.000000 ipol-8/idl/scb.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      537 2023-06-07 18:11:57.000000 ipol-8/idl/tvdenoise.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      376 2023-06-07 14:25:05.000000 ipol-8/idl/tvl1.Dockerfile
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-15 17:10:04.759934 ipol-8/ipol.egg-info/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      516 2023-06-15 17:10:04.000000 ipol-8/ipol.egg-info/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)      388 2023-06-15 17:10:04.000000 ipol-8/ipol.egg-info/SOURCES.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-06-15 17:10:04.000000 ipol-8/ipol.egg-info/dependency_links.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        5 2023-06-15 17:10:04.000000 ipol-8/ipol.egg-info/top_level.txt
+-rwxrwxr-x   0 coco      (1000) coco      (1000)    19280 2023-06-15 17:07:26.000000 ipol-8/ipol.py
+-rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-06-15 17:10:04.759934 ipol-8/setup.cfg
+-rw-rw-r--   0 coco      (1000) coco      (1000)      641 2023-06-15 17:07:37.000000 ipol-8/setup.py
```

### Comparing `ipol-7/PKG-INFO` & `ipol-8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipol
-Version: 7
+Version: 8
 Summary: python interface to some IPOL journal algorithms
 Home-page: https://git.sr.ht/~coco/clipol
 Author: Enric Meinhardt-Llopis
 Author-email: enric.meinhardt@ens-paris-saclay.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `ipol-7/README` & `ipol-8/README`

 * *Files identical despite different names*

### Comparing `ipol-7/idl/ace.Dockerfile` & `ipol-8/idl/ace.Dockerfile`

 * *Files identical despite different names*

### Comparing `ipol-7/idl/bm3d.Dockerfile` & `ipol-8/idl/bm3d.Dockerfile`

 * *Files identical despite different names*

### Comparing `ipol-7/idl/dctdenoise.Dockerfile` & `ipol-8/idl/dctdenoise.Dockerfile`

 * *Files identical despite different names*

### Comparing `ipol-7/idl/ffdnet.Dockerfile` & `ipol-8/idl/ffdnet.Dockerfile`

 * *Files identical despite different names*

### Comparing `ipol-7/idl/msdctd.Dockerfile` & `ipol-8/idl/msdctd.Dockerfile`

 * *Files identical despite different names*

### Comparing `ipol-7/idl/nlbayes.Dockerfile` & `ipol-8/idl/nlbayes.Dockerfile`

 * *Files identical despite different names*

### Comparing `ipol-7/idl/tvdenoise.Dockerfile` & `ipol-8/idl/tvdenoise.Dockerfile`

 * *Files identical despite different names*

### Comparing `ipol-7/ipol.egg-info/PKG-INFO` & `ipol-8/ipol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipol
-Version: 7
+Version: 8
 Summary: python interface to some IPOL journal algorithms
 Home-page: https://git.sr.ht/~coco/clipol
 Author: Enric Meinhardt-Llopis
 Author-email: enric.meinhardt@ens-paris-saclay.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `ipol-7/ipol.py` & `ipol-8/ipol.py`

 * *Files 2% similar despite different names*

```diff
@@ -525,28 +525,28 @@
 
 
 def main_status():
 	import os
 	config_dir = IPOL_CONFIG
 	config_idl = "%s/idl" % config_dir
 	idls = os.listdir(config_idl)
-	dprint('Config dir "%s" contains %d programs' % (config_idl, len(idls)))
+	print('Config dir "%s" contains %d programs' % (config_idl, len(idls)))
 	cache_dir = IPOL_CACHE
 	cacs = os.listdir(cache_dir)
-	dprint('Cache dir "%s" contains %d programs' % (cache_dir, len(cacs)))
+	print('Cache dir "%s" contains %d programs' % (cache_dir, len(cacs)))
 	return 0
 
 def main_list():
 	import os
 	config_dir = IPOL_CONFIG
 	config_idl = "%s/idl" % config_dir
 	idls = os.listdir(config_idl)
 	for x in idls:
 		p = ipol_parse_idl("%s/%s" % (config_idl, x))
-		dprint("\t%s\t%s" % (p['NAME'], p['TITLE']))
+		print("\t%s\t%s" % (p['NAME'], p['TITLE']))
 	return 0
 
 def main_dump(x):
 	config_dir = IPOL_CONFIG
 	config_x = "%s/idl/%s" % (config_dir, x)
 	p = ipol_parse_idl(config_x)
 	print(p)
@@ -602,25 +602,37 @@
 	config_dir = IPOL_CONFIG
 	config_x = "%s/idl/%s" % (config_dir, x)
 	p = ipol_parse_idl(config_x)
 	if not ipol_is_built(p):
 		ipol_build_interface(p)
 	return 0
 
+def main_buildall():
+	import os
+	idls = os.listdir(f"{IPOL_CONFIG}/idl")
+	DEBUG_LEVEL = 1
+	for x in idls:
+		p = ipol_parse_idl(f"{IPOL_CONFIG}/idl/{x}")
+		if not ipol_is_built(p):
+			ipol_build_interface(p)
+	return 0
+
 # sub-commands:
 #	list       list all the sub-commands available (default action)
 #	status     print various global status statistics
 #	dump id    dump the dictionary associated to sub-command "id"
 #	info id    pretty-print the data associated to sub-command "id"
 #	id         run the sub-command "id"
 
 def main():
 	import sys
 	if len(sys.argv) < 2 or sys.argv[1] == "list":
 		return main_list()
+	if sys.argv[1] == "buildall":
+		return main_buildall() if len(sys.argv) == 2 else 1
 	if sys.argv[1] == "status":
 		return main_status()
 	if sys.argv[1] == "dump":
 		return main_dump(sys.argv[2]) if len(sys.argv) == 3 else 1
 	if sys.argv[1] == "gron":
 		return main_gron(sys.argv[2]) if len(sys.argv) == 3 else 1
 	if sys.argv[1] == "json":
@@ -652,10 +664,10 @@
 	idls = os.listdir(f"{IPOL_CONFIG}/idl")
 	idls = [ x[:-11] if x.endswith(".Dockerfile") else x for x in idls ]
 	for i in idls:
 		export_article_interface(i)
 
 
 # API
-version = 7
+version = 8
 
 # vim: sw=8 ts=8 sts=0 noexpandtab:
```

### Comparing `ipol-7/setup.py` & `ipol-8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def data_files():
 	import glob
 	return glob.glob("idl/*.Dockerfile")
 
 setuptools.setup(
 	name = "ipol",
-	version = "7",
+	version = "8",
 	author = "Enric Meinhardt-Llopis",
 	author_email = "enric.meinhardt@ens-paris-saclay.fr",
 	description = "python interface to some IPOL journal algorithms",
 	url = "https://git.sr.ht/~coco/clipol",
 	classifiers = [
 		"Operating System :: OS Independent",
 		"License :: OSI Approved :: GNU Affero General Public License v3",
```

