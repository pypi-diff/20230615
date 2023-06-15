# Comparing `tmp/starbug2-0.4.2.tar.gz` & `tmp/starbug2-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starbug2-0.4.2.tar", last modified: Wed Jun 14 16:14:37 2023, max compression
+gzip compressed data, was "starbug2-0.4.4.tar", last modified: Thu Jun 15 16:01:57 2023, max compression
```

## Comparing `starbug2-0.4.2.tar` & `starbug2-0.4.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:14:37.595449 starbug2-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-14 16:14:17.000000 starbug2-0.4.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 16:14:17.000000 starbug2-0.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-14 16:14:17.000000 starbug2-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-14 16:14:37.595449 starbug2-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-14 16:14:17.000000 starbug2-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:14:37.591449 starbug2-0.4.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    13797 2023-06-14 16:14:17.000000 starbug2-0.4.2/bin/starbug2
--rwxr-xr-x   0 runner    (1001) docker     (123)     7374 2023-06-14 16:14:17.000000 starbug2-0.4.2/bin/starbug2-match
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:14:37.591449 starbug2-0.4.2/extras/
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-14 16:14:17.000000 starbug2-0.4.2/extras/starbug2.completion
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-14 16:14:17.000000 starbug2-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-14 16:14:37.595449 starbug2-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-14 16:14:17.000000 starbug2-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:14:37.591449 starbug2-0.4.2/starbug2/
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-06-14 16:14:17.000000 starbug2-0.4.2/starbug2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-14 16:14:17.000000 starbug2-0.4.2/starbug2/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-06-14 16:14:17.000000 starbug2-0.4.2/starbug2/matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-06-14 16:14:17.000000 starbug2-0.4.2/starbug2/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:14:37.595449 starbug2-0.4.2/starbug2/param/
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-14 16:14:17.000000 starbug2-0.4.2/starbug2/param/default.param
--rw-r--r--   0 runner    (1001) docker     (123)    28598 2023-06-14 16:14:17.000000 starbug2-0.4.2/starbug2/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    31810 2023-06-14 16:14:17.000000 starbug2-0.4.2/starbug2/starbug.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-14 16:14:17.000000 starbug2-0.4.2/starbug2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:14:37.595449 starbug2-0.4.2/starbug2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-14 16:14:37.000000 starbug2-0.4.2/starbug2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-14 16:14:37.000000 starbug2-0.4.2/starbug2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:14:37.000000 starbug2-0.4.2/starbug2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 16:14:37.000000 starbug2-0.4.2/starbug2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 16:14:37.000000 starbug2-0.4.2/starbug2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:14:37.595449 starbug2-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-14 16:14:17.000000 starbug2-0.4.2/tests/test_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-14 16:14:17.000000 starbug2-0.4.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:01:57.097130 starbug2-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-15 16:01:45.000000 starbug2-0.4.4/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 16:01:45.000000 starbug2-0.4.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-15 16:01:45.000000 starbug2-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-15 16:01:57.097130 starbug2-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-15 16:01:45.000000 starbug2-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:01:57.093130 starbug2-0.4.4/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13797 2023-06-15 16:01:45.000000 starbug2-0.4.4/bin/starbug2
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7096 2023-06-15 16:01:45.000000 starbug2-0.4.4/bin/starbug2-match
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:01:57.093130 starbug2-0.4.4/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-15 16:01:45.000000 starbug2-0.4.4/extras/starbug2.completion
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-15 16:01:45.000000 starbug2-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-15 16:01:57.097130 starbug2-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-15 16:01:45.000000 starbug2-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:01:57.093130 starbug2-0.4.4/starbug2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-06-15 16:01:45.000000 starbug2-0.4.4/starbug2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-15 16:01:45.000000 starbug2-0.4.4/starbug2/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-06-15 16:01:45.000000 starbug2-0.4.4/starbug2/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-06-15 16:01:45.000000 starbug2-0.4.4/starbug2/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:01:57.097130 starbug2-0.4.4/starbug2/param/
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-15 16:01:45.000000 starbug2-0.4.4/starbug2/param/default.param
+-rw-r--r--   0 runner    (1001) docker     (123)    28598 2023-06-15 16:01:45.000000 starbug2-0.4.4/starbug2/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31810 2023-06-15 16:01:45.000000 starbug2-0.4.4/starbug2/starbug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10451 2023-06-15 16:01:45.000000 starbug2-0.4.4/starbug2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:01:57.097130 starbug2-0.4.4/starbug2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-15 16:01:57.000000 starbug2-0.4.4/starbug2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-15 16:01:57.000000 starbug2-0.4.4/starbug2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:01:57.000000 starbug2-0.4.4/starbug2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 16:01:57.000000 starbug2-0.4.4/starbug2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 16:01:57.000000 starbug2-0.4.4/starbug2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:01:57.097130 starbug2-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-15 16:01:45.000000 starbug2-0.4.4/tests/test_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-15 16:01:45.000000 starbug2-0.4.4/tests/test_utils.py
```

### Comparing `starbug2-0.4.2/LICENSE.txt` & `starbug2-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.2/PKG-INFO` & `starbug2-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starbug2
-Version: 0.4.2
+Version: 0.4.4
 Summary: JWST PSF photometry in complex crowded fields.
 Author: Conor Nally
 Author-email: conor.nally@ed.ac.uk
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 
 # StarBugII
```

### Comparing `starbug2-0.4.2/README.md` & `starbug2-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.2/bin/starbug2` & `starbug2-0.4.4/bin/starbug2`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.2/bin/starbug2-match` & `starbug2-0.4.4/bin/starbug2-match`

 * *Files 1% similar despite different names*

```diff
@@ -125,25 +125,20 @@
             utils.printf("-> %s: Removing %d sources\n"%(fltr, sum(mask)))
             tables[i].remove_rows(mask)
         else:
             utils.perror("Unable to determine filter of \"%s\"\n"%args[i])
 
 
 if options & BANDMATCH:
-    filters=[]
+    #filters=[]
     tomatch={ starbug2.NIRCAM:[], starbug2.MIRI:[] }
     fname=output if output else "out.fits"
     _colnames=["RA","DEC"]
 
-    for i,tab in enumerate(tables):
-        if not ( (fltr:=tab.meta.get("FILTER")) and fltr in list(starbug2.filters.keys())):
-            if not (fltr:= set(tab.colnames) & set(starbug2.filters.keys()) ):
-                perror("Unable to determine FILTER for \"%s\"\n"%args[i])
-                continue
-        filters.append(fltr)
+    for i,(tab,fltr) in enumerate(zip(tables,filters)):
         tomatch[starbug2.filters[fltr].instr].append(tab)
         _colnames+=([fltr,"e%s"%fltr])
     
     if tomatch[starbug2.NIRCAM] and tomatch[starbug2.MIRI]:
         utils.printf("Detected NIRCam to MIRI matching\n")
 
         nircam_matched=matching.band_match(tomatch[starbug2.NIRCAM], colnames=_colnames)
```

### Comparing `starbug2-0.4.2/extras/starbug2.completion` & `starbug2-0.4.4/extras/starbug2.completion`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.2/starbug2/__init__.py` & `starbug2-0.4.4/starbug2/__init__.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.2/starbug2/mask.py` & `starbug2-0.4.4/starbug2/mask.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.2/starbug2/matching.py` & `starbug2-0.4.4/starbug2/matching.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,19 +319,19 @@
     for name in colnames:
         all_cols=find_colnames(tab,name)
         #if not (all_cols:=find_colnames(tab,name)): continue
         if not all_cols: continue
         col=Column(None, name=name)
         ar=tab2array(tab, colnames=all_cols)
         if name=="flux":
-            col=Column(np.nanmean(ar,axis=1), name=name)
-            median=np.nanmedian(ar,axis=1)
+            col=Column(np.nanmedian(ar,axis=1), name=name)
+            mean=np.nanmean(ar,axis=1)
             if "stdflux" not in colnames: av.add_column(Column(np.nanstd(ar,axis=1),name="stdflux")) 
             ## if median and mean are >5% different, flag as SRC_VAR
-            flags[ np.abs(median-col)>(col/5.0)] |= starbug2.SRC_VAR
+            flags[ np.abs(mean-col)>(col/5.0)] |= starbug2.SRC_VAR
         elif name== "eflux":
             col=Column(np.sqrt(np.nansum(ar*ar, axis=1)), name=name)
         elif name=="stdflux": 
             col=Column(np.nanmax(ar,axis=1),name=name)
         elif name=="flag":
             col=Column(flags, name=name)
             for fcol in ar.T: col|=fcol.astype(np.uint16)
```

### Comparing `starbug2-0.4.2/starbug2/misc.py` & `starbug2-0.4.4/starbug2/misc.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.2/starbug2/param/default.param` & `starbug2-0.4.4/starbug2/param/default.param`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.2/starbug2/routines.py` & `starbug2-0.4.4/starbug2/routines.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.2/starbug2/starbug.py` & `starbug2-0.4.4/starbug2/starbug.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.2/starbug2/utils.py` & `starbug2-0.4.4/starbug2/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,21 +171,22 @@
     """
     """
     tab=None
     if os.path.exists(fname):
         if os.path.splitext(fname)[1]==".fits":
             tab=Table.read(fname,format="fits")
             tmp=Table()
-            
-            if "flag" in tab.colnames:
-                tmp.add_column(tab["flag"])
-                tab.remove_columns("flag")
-            if "NUM" in tab.colnames:
-                tmp.add_column(tab["NUM"])
-                tab.remove_columns("NUM")
+
+            names=[]
+            for index in range(len(tab.dtype.names)):
+                if tab.dtype[index].kind!='f':
+                    name=tab.colnames[index]
+                    names.append(name)
+                    tmp.add_column( tab[name] )
+            tab.remove_columns( names )
             tab=tab.filled(np.nan)
             if tmp: tab=hstack((tab,tmp))
 
         else: perror("Table must fits format\n")
     else: perror("Unable to locate \"%s\"\n"%fname)
     return tab
```

### Comparing `starbug2-0.4.2/starbug2.egg-info/PKG-INFO` & `starbug2-0.4.4/starbug2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starbug2
-Version: 0.4.2
+Version: 0.4.4
 Summary: JWST PSF photometry in complex crowded fields.
 Author: Conor Nally
 Author-email: conor.nally@ed.ac.uk
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 
 # StarBugII
```

### Comparing `starbug2-0.4.2/tests/test_routines.py` & `starbug2-0.4.4/tests/test_routines.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.2/tests/test_utils.py` & `starbug2-0.4.4/tests/test_utils.py`

 * *Files identical despite different names*

