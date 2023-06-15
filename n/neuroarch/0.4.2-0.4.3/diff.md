# Comparing `tmp/neuroarch-0.4.2.tar.gz` & `tmp/neuroarch-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/neuroarch-0.4.2.tar", last modified: Tue Aug  2 14:38:53 2022, max compression
+gzip compressed data, was "/mnt/server-home/yiyin/pypi/neuroarch/dist/.tmp-2i5fzhnx/neuroarch-0.4.3.tar", last modified: Thu Jun 15 04:45:20 2023, max compression
```

## Comparing `neuroarch-0.4.2.tar` & `neuroarch-0.4.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 yiyin     (1001) yiyin     (1001)        0 2022-08-02 14:38:53.000000 neuroarch-0.4.2/
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      366 2021-05-19 02:01:52.000000 neuroarch-0.4.2/AUTHORS.rst
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     1556 2021-05-19 02:01:52.000000 neuroarch-0.4.2/LICENSE.rst
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      895 2022-08-02 14:38:53.000000 neuroarch-0.4.2/PKG-INFO
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     2012 2021-05-19 02:01:52.000000 neuroarch-0.4.2/README.rst
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    12292 2021-02-23 14:22:58.000000 neuroarch-0.4.2/ez_setup.py
-drwxrwxr-x   0 yiyin     (1001) yiyin     (1001)        0 2022-08-02 14:38:52.000000 neuroarch-0.4.2/loaders/
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    12515 2021-02-23 14:22:58.000000 neuroarch-0.4.2/loaders/load_flycircuit.py
-drwxrwxr-x   0 yiyin     (1001) yiyin     (1001)        0 2022-08-02 14:38:52.000000 neuroarch-0.4.2/neuroarch/
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     7513 2021-02-23 14:22:58.000000 neuroarch-0.4.2/neuroarch/LPU_loader.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      350 2021-02-23 14:22:58.000000 neuroarch-0.4.2/neuroarch/__init__.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     6902 2021-02-23 14:22:58.000000 neuroarch-0.4.2/neuroarch/apply_diff.py
-drwxrwxr-x   0 yiyin     (1001) yiyin     (1001)        0 2022-08-02 14:38:53.000000 neuroarch-0.4.2/neuroarch/conv/
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)        0 2021-02-23 14:22:58.000000 neuroarch-0.4.2/neuroarch/conv/__init__.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     8107 2022-06-12 05:15:18.000000 neuroarch-0.4.2/neuroarch/conv/nx.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     7811 2022-06-12 05:15:18.000000 neuroarch-0.4.2/neuroarch/conv/pd.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     2682 2021-02-23 14:22:58.000000 neuroarch-0.4.2/neuroarch/conv/utils.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     5131 2021-02-23 14:22:58.000000 neuroarch-0.4.2/neuroarch/diff.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    11353 2021-02-23 14:22:58.000000 neuroarch-0.4.2/neuroarch/gen_generic_lpu.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    23172 2022-08-02 14:38:46.000000 neuroarch-0.4.2/neuroarch/models.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)   162925 2022-08-02 14:38:46.000000 neuroarch-0.4.2/neuroarch/na.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     3012 2021-05-19 02:01:52.000000 neuroarch-0.4.2/neuroarch/nk.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     6057 2021-02-23 14:22:58.000000 neuroarch-0.4.2/neuroarch/nk_direct.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    16146 2021-02-23 14:22:58.000000 neuroarch-0.4.2/neuroarch/nxtools.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    82358 2022-06-12 05:15:18.000000 neuroarch-0.4.2/neuroarch/query.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     4562 2021-02-23 14:22:58.000000 neuroarch-0.4.2/neuroarch/utils.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)       81 2021-02-23 14:22:58.000000 neuroarch-0.4.2/neuroarch/version.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     1486 2021-02-23 14:22:58.000000 neuroarch-0.4.2/neuroarch/vis.py
-drwxrwxr-x   0 yiyin     (1001) yiyin     (1001)        0 2022-08-02 14:38:53.000000 neuroarch-0.4.2/neuroarch.egg-info/
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      895 2022-08-02 14:38:52.000000 neuroarch-0.4.2/neuroarch.egg-info/PKG-INFO
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      780 2022-08-02 14:38:52.000000 neuroarch-0.4.2/neuroarch.egg-info/SOURCES.txt
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)        1 2022-08-02 14:38:52.000000 neuroarch-0.4.2/neuroarch.egg-info/dependency_links.txt
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)       10 2022-08-02 14:38:52.000000 neuroarch-0.4.2/neuroarch.egg-info/namespace_packages.txt
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)       57 2022-08-02 14:38:52.000000 neuroarch-0.4.2/neuroarch.egg-info/requires.txt
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)       10 2022-08-02 14:38:52.000000 neuroarch-0.4.2/neuroarch.egg-info/top_level.txt
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)       38 2022-08-02 14:38:53.000000 neuroarch-0.4.2/setup.cfg
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     2173 2022-08-02 14:38:49.000000 neuroarch-0.4.2/setup.py
-drwxrwxr-x   0 yiyin     (1001) yiyin     (1001)        0 2022-08-02 14:38:53.000000 neuroarch-0.4.2/tests/
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     5369 2021-02-23 14:22:58.000000 neuroarch-0.4.2/tests/test_conv_nx.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     5804 2021-02-23 14:22:58.000000 neuroarch-0.4.2/tests/test_conv_pd.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     2386 2021-02-23 14:22:58.000000 neuroarch-0.4.2/tests/test_conv_utils.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     9986 2021-02-23 14:22:58.000000 neuroarch-0.4.2/tests/test_diff.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    13709 2021-02-23 14:22:58.000000 neuroarch-0.4.2/tests/test_nxtools.py
+drwxrwxr-x   0 yiyin     (1001) yiyin     (1001)        0 2023-06-15 04:45:20.000000 neuroarch-0.4.3/
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      366 2021-05-19 02:01:52.000000 neuroarch-0.4.3/AUTHORS.rst
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     1556 2021-05-19 02:01:52.000000 neuroarch-0.4.3/LICENSE.rst
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      917 2023-06-15 04:45:20.000000 neuroarch-0.4.3/PKG-INFO
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     2012 2021-05-19 02:01:52.000000 neuroarch-0.4.3/README.rst
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    12292 2021-02-23 14:22:58.000000 neuroarch-0.4.3/ez_setup.py
+drwxrwxr-x   0 yiyin     (1001) yiyin     (1001)        0 2023-06-15 04:45:20.000000 neuroarch-0.4.3/loaders/
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    12515 2021-02-23 14:22:58.000000 neuroarch-0.4.3/loaders/load_flycircuit.py
+drwxrwxr-x   0 yiyin     (1001) yiyin     (1001)        0 2023-06-15 04:45:20.000000 neuroarch-0.4.3/neuroarch/
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     7513 2021-02-23 14:22:58.000000 neuroarch-0.4.3/neuroarch/LPU_loader.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      350 2021-02-23 14:22:58.000000 neuroarch-0.4.3/neuroarch/__init__.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     6902 2021-02-23 14:22:58.000000 neuroarch-0.4.3/neuroarch/apply_diff.py
+drwxrwxr-x   0 yiyin     (1001) yiyin     (1001)        0 2023-06-15 04:45:20.000000 neuroarch-0.4.3/neuroarch/conv/
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)        0 2021-02-23 14:22:58.000000 neuroarch-0.4.3/neuroarch/conv/__init__.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     8107 2022-06-12 05:15:18.000000 neuroarch-0.4.3/neuroarch/conv/nx.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     7811 2022-06-12 05:15:18.000000 neuroarch-0.4.3/neuroarch/conv/pd.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     2682 2021-02-23 14:22:58.000000 neuroarch-0.4.3/neuroarch/conv/utils.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     5131 2021-02-23 14:22:58.000000 neuroarch-0.4.3/neuroarch/diff.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    11353 2021-02-23 14:22:58.000000 neuroarch-0.4.3/neuroarch/gen_generic_lpu.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    23172 2022-08-02 14:38:46.000000 neuroarch-0.4.3/neuroarch/models.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)   165424 2023-06-15 04:40:56.000000 neuroarch-0.4.3/neuroarch/na.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     3012 2021-05-19 02:01:52.000000 neuroarch-0.4.3/neuroarch/nk.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     6057 2021-02-23 14:22:58.000000 neuroarch-0.4.3/neuroarch/nk_direct.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    16146 2021-02-23 14:22:58.000000 neuroarch-0.4.3/neuroarch/nxtools.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    82358 2022-06-12 05:15:18.000000 neuroarch-0.4.3/neuroarch/query.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     4562 2021-02-23 14:22:58.000000 neuroarch-0.4.3/neuroarch/utils.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)       81 2021-02-23 14:22:58.000000 neuroarch-0.4.3/neuroarch/version.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     1486 2021-02-23 14:22:58.000000 neuroarch-0.4.3/neuroarch/vis.py
+drwxrwxr-x   0 yiyin     (1001) yiyin     (1001)        0 2023-06-15 04:45:20.000000 neuroarch-0.4.3/neuroarch.egg-info/
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      917 2023-06-15 04:45:20.000000 neuroarch-0.4.3/neuroarch.egg-info/PKG-INFO
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      780 2023-06-15 04:45:20.000000 neuroarch-0.4.3/neuroarch.egg-info/SOURCES.txt
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)        1 2023-06-15 04:45:20.000000 neuroarch-0.4.3/neuroarch.egg-info/dependency_links.txt
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)       10 2023-06-15 04:45:20.000000 neuroarch-0.4.3/neuroarch.egg-info/namespace_packages.txt
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)       54 2023-06-15 04:45:20.000000 neuroarch-0.4.3/neuroarch.egg-info/requires.txt
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)       10 2023-06-15 04:45:20.000000 neuroarch-0.4.3/neuroarch.egg-info/top_level.txt
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)       38 2023-06-15 04:45:20.000000 neuroarch-0.4.3/setup.cfg
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     2170 2023-06-15 04:41:26.000000 neuroarch-0.4.3/setup.py
+drwxrwxr-x   0 yiyin     (1001) yiyin     (1001)        0 2023-06-15 04:45:20.000000 neuroarch-0.4.3/tests/
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     5369 2021-02-23 14:22:58.000000 neuroarch-0.4.3/tests/test_conv_nx.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     5804 2021-02-23 14:22:58.000000 neuroarch-0.4.3/tests/test_conv_pd.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     2386 2021-02-23 14:22:58.000000 neuroarch-0.4.3/tests/test_conv_utils.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     9986 2021-02-23 14:22:58.000000 neuroarch-0.4.3/tests/test_diff.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    13709 2021-02-23 14:22:58.000000 neuroarch-0.4.3/tests/test_nxtools.py
```

### Comparing `neuroarch-0.4.2/LICENSE.rst` & `neuroarch-0.4.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/PKG-INFO` & `neuroarch-0.4.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: neuroarch
-Version: 0.4.2
+Version: 0.4.3
 Summary: A graph-based platform for representing Drosophila brain architectures
 Home-page: https://github.com/fruitflybrain/neuroarch/
 Author: Lev Givon, Nikul Ukani, Yiyin Zhou
 Author-email: lev@columbia.edu, nikul@ee.columbia.edu, yiyin@ee.columbia.edu
 Maintainer: Yiyin Zhou
 Maintainer-email: yiyin@ee.columbia.edu
 License: BSD
-Description: A graph-based platform for representing Drosophila brain architectures
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
+License-File: LICENSE.rst
+License-File: AUTHORS.rst
+
+A graph-based platform for representing Drosophila brain architectures
```

### Comparing `neuroarch-0.4.2/README.rst` & `neuroarch-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/ez_setup.py` & `neuroarch-0.4.3/ez_setup.py`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/loaders/load_flycircuit.py` & `neuroarch-0.4.3/loaders/load_flycircuit.py`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/neuroarch/LPU_loader.py` & `neuroarch-0.4.3/neuroarch/LPU_loader.py`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/neuroarch/apply_diff.py` & `neuroarch-0.4.3/neuroarch/apply_diff.py`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/neuroarch/conv/nx.py` & `neuroarch-0.4.3/neuroarch/conv/nx.py`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/neuroarch/conv/pd.py` & `neuroarch-0.4.3/neuroarch/conv/pd.py`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/neuroarch/conv/utils.py` & `neuroarch-0.4.3/neuroarch/conv/utils.py`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/neuroarch/diff.py` & `neuroarch-0.4.3/neuroarch/diff.py`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/neuroarch/gen_generic_lpu.py` & `neuroarch-0.4.3/neuroarch/gen_generic_lpu.py`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/neuroarch/models.py` & `neuroarch-0.4.3/neuroarch/models.py`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/neuroarch/na.py` & `neuroarch-0.4.3/neuroarch/na.py`

 * *Files 1% similar despite different names*

```diff
@@ -845,18 +845,18 @@
         url : str
             Web URL describing the origin of the DataSource
         description : str
             A brief description of the DataSource
         species : dict or models.Species
             The species the added DataSource is for.
             If species is a dict, it must be contain the following keys:
-                {'name': str,
-                 'stage': str,
-                 'synonyms': list of str (optional)
-                }
+            {'name': str,
+            'stage': str,
+            'synonyms': list of str (optional)
+            }
 
         Returns
         -------
         datasource : models.DataSource
             created DataSource object
         """
         assert isinstance(name, str), 'name must be of str type'
@@ -913,16 +913,16 @@
             Name of the subsystem
             (abbreviation is preferred, full name can be given in the synonyms)
         synonyms : list of str
             Synonyms of the subsystem.
         morphology : dict (optional)
             Morphology of the neuropil boundary specified with a triangulated mesh,
             with fields
-                'vertices': a single list of float, every 3 entries specify (x,y,z) coordinates.
-                'faces': a single list of int, every 3 entries specify samples of vertices.
+            'vertices': a single list of float, every 3 entries specify (x,y,z) coordinates.
+            'faces': a single list of int, every 3 entries specify samples of vertices.
             Or, specify the file path to a json file that includes the definition of the mesh.
             Or, specify only a url which can be readout later on.
         data_source : models.DataSource (optional)
             The datasource. If not specified, default DataSource will be used.
 
         Returns
         -------
@@ -977,16 +977,16 @@
             Synonyms of the neuropil.
         subsystem : str or models.Subsystem (optional)
             Subsystem that owns the neuropil. Can be specified either by its name
             or the Subsytem object instance.
         morphology : dict (optional)
             Morphology of the neuropil boundary specified with a triangulated mesh,
             with fields
-                'vertices': a single list of float, every 3 entries specify (x,y,z) coordinates.
-                'faces': a single list of int, every 3 entries specify samples of vertices.
+            'vertices': a single list of float, every 3 entries specify (x,y,z) coordinates.
+            'faces': a single list of int, every 3 entries specify samples of vertices.
             Or, specify the file path to a json file that includes the definition of the mesh.
             Or, specify only a url which can be readout later on.
         data_source : models.DataSource (optional)
             The datasource. If not specified, default DataSource will be used.
 
         Returns
         -------
@@ -1068,16 +1068,16 @@
             Synonyms of the synonyms.
         neuropil : str or models.Neuropil (optional)
             Neuropil that owns the subregion. Can be specified either by its name
             or the Neuropil object instance.
         morphology : dict (optional)
             Morphology of the neuropil boundary specified with a triangulated mesh,
             with fields
-                'vertices': a single list of float, every 3 entries specify (x,y,z) coordinates.
-                'faces': a single list of int, every 3 entries specify samples of vertices.
+            'vertices': a single list of float, every 3 entries specify (x,y,z) coordinates.
+            'faces': a single list of int, every 3 entries specify samples of vertices.
             Or, specify the file path to a json file that includes the definition of the mesh.
             Or, specify only a url which can be readout later on.
         data_source : models.DataSource (optional)
             The datasource. If not specified, default DataSource will be used.
 
         Returns
         -------
@@ -1155,16 +1155,16 @@
             Name of the tract
             (abbreviation is preferred, full name can be given in the synonyms)
         synonyms : list of str
             Synonyms of the synonyms.
         morphology : dict (optional)
             Morphology of the neuropil boundary specified with a triangulated mesh,
             with fields
-                'vertices': a single list of float, every 3 entries specify (x,y,z) coordinates.
-                'faces': a single list of int, every 3 entries specify samples of vertices.
+            'vertices': a single list of float, every 3 entries specify (x,y,z) coordinates.
+            'faces': a single list of int, every 3 entries specify samples of vertices.
             Or, specify the file path to a json file that includes the definition of the mesh.
             Or, specify only a url which can be readout later on.
         data_source : models.DataSource (optional)
             The datasource. If not specified, default DataSource will be used.
 
         Returns
         -------
@@ -1295,26 +1295,26 @@
             Synonyms of the neuron
         info : dict (optional)
             Additional information about the neuron, values must be str
         morphology : list of dict (optional)
             Each dict in the list defines a type of morphology of the neuron.
             Must be loaded from a file.
             The dict must include the following key to indicate the type of morphology:
-                {'type': 'swc'/'obj'/...}
+            {'type': 'swc'/'obj'/...}
             Additional keys must be provides, either 'filename' with value
             indicating the file to be read for the morphology,
             or a full definition of the morphology according the schema.
             For swc, required fields are ['sample', 'identifier', 'x', 'y, 'z', 'r', 'parent'].
             More formats pending implementation.
         arborization : list of dict (optional)
             A list of dictionaries define the arborization pattern of
             the neuron in neuropils, subregions, and tracts, if applicable, with
             {'type': 'neuropil' or 'subregion' or 'tract',
-             'dendrites': {'EB': 20, 'FB': 2},
-             'axons': {'NO': 10, 'MB': 22}}
+            'dendrites': {'EB': 20, 'FB': 2},
+            'axons': {'NO': 10, 'MB': 22}}
             Name of the regions must already be present in the database.
         neurotransmitters : str or list of str (optional)
             The neurotransmitter(s) expressed by the neuron
         neurotransmitters_datasources : models.DataSource or list of models.DataSource (optional)
             The datasource of neurotransmitter data.
             If None, all neurotransmitter will have the same datasource of the Neuron.
             If specified, the size of the list must be the same as the size of
@@ -1467,26 +1467,26 @@
             Unique identifier in the original data source
         info : dict (optional)
             Additional information about the neuron, values must be str
         morphology : list of dict (optional)
             Each dict in the list defines a type of morphology of the neuron.
             Must be loaded from a file.
             The dict must include the following key to indicate the type of morphology:
-                {'type': 'swc'/'obj'/...}
+            {'type': 'swc'/'obj'/...}
             Additional keys must be provides, either 'filename' with value
             indicating the file to be read for the morphology,
             or a full definition of the morphology according the schema.
             For swc, required fields are ['sample', 'identifier', 'x', 'y, 'z', 'r', 'parent'].
             More formats pending implementation.
         arborization : list of dict (optional)
             A list of dictionaries define the arborization pattern of
             the neuron in neuropils, subregions, and tracts, if applicable, with
             {'type': 'neuropil' or 'subregion' or 'tract',
-             'dendrites': {'EB': 20, 'FB': 2},
-             'axons': {'NO': 10, 'MB': 22}}
+            'dendrites': {'EB': 20, 'FB': 2},
+            'axons': {'NO': 10, 'MB': 22}}
             Name of the regions must already be present in the database.
         data_source : models.DataSource (optional)
             The datasource. If not specified, default DataSource will be used.
 
         Returns
         -------
         neuron : models.NeuronFragment
@@ -1653,15 +1653,15 @@
         obj : models.BioNode or subclass
             An instance of BioNode class, e.g., Neuropil, Neuron, etc...
             to which the morphology will be associated to
         morphology : list of dict (optional)
             Each dict in the list defines a type of morphology of the neuron.
             Must be loaded from a file.
             The dict must include the following key to indicate the type of morphology:
-                {'type': 'swc'/'obj'/...}
+            {'type': 'swc'/'obj'/...}
             Additional keys must be provides, either 'filename' with value
             indicating the file to be read for the morphology,
             or a full definition of the morphology according the schema.
             For swc, required fields are ['sample', 'identifier', 'x', 'y, 'z', 'r', 'parent'].
             For mesh, requires an obj file or ['faces', 'vertices'] defined as rastered list of a wavefront obj file
         data_source : models.DataSource (optional)
             The datasource. If not specified, default DataSource will be used.
@@ -1762,16 +1762,16 @@
         ----------
         neuron : models.Neuron or subclass
             An instance of Neuron class to which the arborization data will be associated to.
         arborization : list of dict
             A list of dictionaries define the arborization pattern of
             the neuron in neuropils, subregions, and tracts, if applicable, with
             {'type': 'neuropil' or 'subregion' or 'tract',
-             'dendrites': {'EB': 20, 'FB': 2},
-             'axons': {'NO': 10, 'MB': 22}}
+            'dendrites': {'EB': 20, 'FB': 2},
+            'axons': {'NO': 10, 'MB': 22}}
             Name of the regions must already be present in the database.
         data_source : models.DataSource (optional)
             The datasource. If not specified, default DataSource will be used.
         """
         self._database_writeable_check()
         neuron = self._get_obj_from_str(neuron)
         if not isinstance(neuron, models.Neuron):
@@ -1867,28 +1867,28 @@
             The number of synapses from pre_neuron to the post_neuron.
         NHP : int (optional)
             The number of synapses that can be confirmed with a high probability
         morphology : list of dict (optional)
             Each dict in the list defines a type of morphology of the neuron.
             Must be loaded from a file.
             The dict must include the following key to indicate the type of morphology:
-                {'type': 'swc'}
+            {'type': 'swc'}
             For swc, required fields are ['sample', 'identifier', 'x', 'y, 'z', 'r', 'parent'].
             For synapses, if both postsynaptic and presynaptic sites are available,
             x, y, z, r must each be a list where the first half indicate the
             locations/radii of postsynaptic sites (on the presynaptic neuron),
             and the second half indicate the locations/radii of the presynaptic
             sites (on the postsynaptic neuron). There should be a one-to-one relation
             between the first half and second half.
             parent must be a list of -1.
         arborization : list of dict (optional)
             A list of dictionaries define the arborization pattern of
             the neuron in neuropils, subregions, and tracts, if applicable, with
             {'type': 'neuropil' or 'subregion' or 'tract',
-             'synapses': {'EB': 20, 'FB': 2}}
+            'synapses': {'EB': 20, 'FB': 2}}
             Name of the regions must already be present in the database.
         data_source : models.DataSource (optional)
             The datasource. If not specified, default DataSource will be used.
 
         Returns
         -------
         synapse : models.Synapse
@@ -2001,15 +2001,15 @@
         ----------
         synapse : neuorarch.models.synapse or subclass
             An instance of Synapse class to which the arborization data will be associated to.
         arborization : list of dict (optional)
             A list of dictionaries define the arborization pattern of
             the neuron in neuropils, subregions, and tracts, if applicable, with
             {'type': 'neuropil' or 'subregion' or 'tract',
-             'synapses': {'EB': 20, 'FB': 2}}
+            'synapses': {'EB': 20, 'FB': 2}}
             Name of the regions must already be present in the database.
         data_source : models.DataSource (optional)
             The datasource. If not specified, default DataSource will be used.
 
         """
         self._database_writeable_check()
         synapse = self._get_obj_from_str(synapse)
@@ -2074,28 +2074,28 @@
             If str, must be the uname of the postsynaptic neuron.
         N : int (optional)
             The number of synapses from pre_neuron to the post_neuron.
         morphology : list of dict (optional)
             Each dict in the list defines a type of morphology of the neuron.
             Must be loaded from a file.
             The dict must include the following key to indicate the type of morphology:
-                {'type': 'swc'}
+            {'type': 'swc'}
             For swc, required fields are ['sample', 'identifier', 'x', 'y, 'z', 'r', 'parent'].
             For synapses, if both postsynaptic and presynaptic sites are available,
             x, y, z, r must each be a list where the first half indicate the
             locations/radii of postsynaptic sites (on the presynaptic neuron),
             and the second half indicate the locations/radii of the presynaptic
             sites (on the postsynaptic neuron). There should be a one-to-one relation
             between the first half and second half.
             parent must be a list of -1.
         arborization : list of dict (optional)
             A list of dictionaries define the arborization pattern of
             the neuron in neuropils, subregions, and tracts, if applicable, with
             {'type': 'neuropil' or 'subregion' or 'tract',
-             'synapses': {'EB': 20, 'FB': 2}}
+            'synapses': {'EB': 20, 'FB': 2}}
             Name of the regions must already be present in the database.
         data_source : models.DataSource (optional)
             The datasource. If not specified, default DataSource will be used.
 
         Returns
         -------
         synapse : models.InferredSynapse
@@ -2450,29 +2450,29 @@
         else:
             post_neurons = [self._get_obj_from_str(neuron) for neuron in post_neurons]
 
         pre_neurons_objs = []
         post_neurons_objs = []
         for neuron in pre_neurons:
             if isinstance(neuron, models.Neuron):
-                pre_neuron_objs.append(neuron)
+                pre_neurons_objs.append(neuron)
             elif isinstance(neuron, str):
-                pre_neuron_objs.append(self.get('Neuron', neuron, connect_DataSource))
+                pre_neurons_objs.append(self.get('Neuron', neuron, connect_DataSource))
             else:
                 raise TypeError('Parameter neuron must be either a str or a Neuron object.')
         for neuron in post_neurons:
             if isinstance(neuron, models.Neuron):
-                post_neuron_objs.append(neuron)
+                post_neurons_objs.append(neuron)
             elif isinstance(neuron, str):
-                post_neuron_objs.append(self.get('Neuron', neuron, connect_DataSource))
+                post_neurons_objs.append(self.get('Neuron', neuron, connect_DataSource))
             else:
                 raise TypeError('Parameter neuron must be either a str or a Neuron object.')
 
-        pre_q = QueryWrapper.from_objs(self.graph, pre_objs)
-        post_q = QueryWrapper.from_objs(self.graph, post_neuron_objs)
+        pre_q = QueryWrapper.from_objs(self.graph, pre_neurons_objs)
+        post_q = QueryWrapper.from_objs(self.graph, post_neurons_objs)
         synapses = outgoing_synapses(pre_q) & incoming_synapses(post_q)
         self.remove_synapses(synapses.node_objs, safe = False)
 
     def remove_Neuropil(self):
         pass
 
     def update_Neuron(self, neuron,
@@ -2509,26 +2509,26 @@
             Synonyms of the neuron
         info : dict (optional)
             Additional information about the neuron, values must be str
         morphology : list of dict (optional)
             Each dict in the list defines a type of morphology of the neuron.
             Must be loaded from a file.
             The dict must include the following key to indicate the type of morphology:
-                {'type': 'swc'/'obj'/...}
+            {'type': 'swc'/'obj'/...}
             Additional keys must be provides, either 'filename' with value
             indicating the file to be read for the morphology,
             or a full definition of the morphology according the schema.
             For swc, required fields are ['sample', 'identifier', 'x', 'y, 'z', 'r', 'parent'].
             More formats pending implementation.
         arborization : list of dict (optional)
             A list of dictionaries define the arborization pattern of
             the neuron in neuropils, subregions, and tracts, if applicable, with
             {'type': 'neuropil' or 'subregion' or 'tract',
-             'dendrites': {'EB': 20, 'FB': 2},
-             'axons': {'NO': 10, 'MB': 22}}
+            'dendrites': {'EB': 20, 'FB': 2},
+            'axons': {'NO': 10, 'MB': 22}}
             Name of the regions must already be present in the database.
         neurotransmitters : str or list of str (optional)
             The neurotransmitter(s) expressed by the neuron
         neurotransmitters_datasources : models.DataSource or list of models.DataSource (optional)
             The datasource of neurotransmitter data.
             If None, all neurotransmitter will have the same datasource of the Neuron.
             If specified, the size of the list must be the same as the size of
@@ -2731,28 +2731,28 @@
             The number of synapses from pre_neuron to the post_neuron.
         NHP : int (optional)
             The number of synapses that can be confirmed with a high probability
         morphology : list of dict (optional)
             Each dict in the list defines a type of morphology of the neuron.
             Must be loaded from a file.
             The dict must include the following key to indicate the type of morphology:
-                {'type': 'swc'}
+            {'type': 'swc'}
             For swc, required fields are ['sample', 'identifier', 'x', 'y, 'z', 'r', 'parent'].
             For synapses, if both postsynaptic and presynaptic sites are available,
             x, y, z, r must each be a list where the first half indicate the
             locations/radii of postsynaptic sites (on the presynaptic neuron),
             and the second half indicate the locations/radii of the presynaptic
             sites (on the postsynaptic neuron). There should be a one-to-one relation
             between the first half and second half.
             parent must be a list of -1.
         arborization : list of dict (optional)
             A list of dictionaries define the arborization pattern of
             the neuron in neuropils, subregions, and tracts, if applicable, with
             {'type': 'neuropil' or 'subregion' or 'tract',
-             'synapses': {'EB': 20, 'FB': 2}}
+            'synapses': {'EB': 20, 'FB': 2}}
             Name of the regions must already be present in the database.
         data_source : models.DataSource (optional)
             The datasource. If not specified, default DataSource will be used.
 
         Returns
         -------
         bool
@@ -3366,14 +3366,104 @@
             # link(port_obj, synapse_model_obj, edge_type = 'SendsTo', variable = synapse_model_obj.link_pre)
             # else
             # port_obj = self.add_Port()
             # find pattern or create pattern
             # link(port_obj, synapse_model_obj, edge_type = 'SendsTo', variable = synapse_model_obj.link_pre)
             # link pre_port -> Pattern in port, Pattern in port to Pattern out port, Pattern out port to port_obj
         return synapse_model_obj
+    
+    def query_neuron(self, uname = None, referenceId = None):
+        """
+        Query neurons by unique name or referenceId
+        
+        Parameters
+        ----------
+        uname : str
+            Query neuron by the uname of the neuron.
+        referenceId : str
+            Query neuron by the id in the original dataset.
+        
+        Returns
+        -------
+        query.QueryWrapper
+            A query wrapper including the neurons
+        """
+        if uname is not None:
+            q = self.sql_query(""" select from Neuron where uname = "{}" """.format(uname))
+        else:
+            q = self.sql_query(""" select from Neuron where referenceId = {} """.format(referenceId))
+        return q
+
+    def query_celltype(self, celltype):
+        """
+        Query neurons by cell type.
+        
+        Parameters
+        ----------
+        celltype : str
+            Query neuron by the cell type of the neuron.
+        
+        Returns
+        -------
+        query.QueryWrapper
+            A query wrapper including the neurons
+        """
+        return self.sql_query(""" select from Neuron where name = "{}" """.format(celltype))
+    
+    def query_synapses(self, pre_name, post_name):
+        """
+        Query synapses by presynaptic and postsynaptic neuron unames
+        
+        Parameters
+        ----------
+        pre_name : str
+            Name of the presynaptic neuron.
+        post_name : str
+            Name of the postsynaptic neuron.
+        
+        Returns
+        -------
+        query.QueryWrapper
+            A query wrapper including the synapses
+        """
+        return self.sql_query(
+            """ select from Synapse where uname = "{}--{}" """.format(pre_name, post_name))
+    
+    def query_neuropil(self, neuropil):
+        """
+        Query neuropil by name.
+        
+        Parameters
+        ----------
+        neuropil : str
+            name of the neuropil
+        
+        Returns
+        -------
+        query.QueryWrapper
+            A query wrapper including the neuropil
+        """
+        return self.sql_query(""" select from Neuropil where name = "{}" """.format(neuropil))
+
+    def query_subregion(self, subregion):
+        """
+        Query subregion by name.
+        
+        Parameters
+        ----------
+        subregion : str
+            name of the subregion
+        
+        Returns
+        -------
+        query.QueryWrapper
+            A query wrapper including the subregion
+        """
+        return self.sql_query(""" select from Subregion where name = "{}" """.format(subregion))
+
 
 def outgoing_synapses(q, N = None, rel='>',include_inferred=True):
     """
     Get all the outgoing synapses from neurons in a QueryWrapper object.
 
     Parameters
     ----------
```

### Comparing `neuroarch-0.4.2/neuroarch/nk.py` & `neuroarch-0.4.3/neuroarch/nk.py`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/neuroarch/nk_direct.py` & `neuroarch-0.4.3/neuroarch/nk_direct.py`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/neuroarch/nxtools.py` & `neuroarch-0.4.3/neuroarch/nxtools.py`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/neuroarch/query.py` & `neuroarch-0.4.3/neuroarch/query.py`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/neuroarch/utils.py` & `neuroarch-0.4.3/neuroarch/utils.py`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/neuroarch/vis.py` & `neuroarch-0.4.3/neuroarch/vis.py`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/neuroarch.egg-info/PKG-INFO` & `neuroarch-0.4.3/neuroarch.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: neuroarch
-Version: 0.4.2
+Version: 0.4.3
 Summary: A graph-based platform for representing Drosophila brain architectures
 Home-page: https://github.com/fruitflybrain/neuroarch/
 Author: Lev Givon, Nikul Ukani, Yiyin Zhou
 Author-email: lev@columbia.edu, nikul@ee.columbia.edu, yiyin@ee.columbia.edu
 Maintainer: Yiyin Zhou
 Maintainer-email: yiyin@ee.columbia.edu
 License: BSD
-Description: A graph-based platform for representing Drosophila brain architectures
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
+License-File: LICENSE.rst
+License-File: AUTHORS.rst
+
+A graph-based platform for representing Drosophila brain architectures
```

### Comparing `neuroarch-0.4.2/neuroarch.egg-info/SOURCES.txt` & `neuroarch-0.4.3/neuroarch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/setup.py` & `neuroarch-0.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from ez_setup import use_setuptools
     use_setuptools()
 
 from setuptools import find_packages
 from setuptools import setup
 
 NAME =               'neuroarch'
-VERSION =            '0.4.2'
+VERSION =            '0.4.3'
 AUTHOR =             'Lev Givon, Nikul Ukani, Yiyin Zhou'
 AUTHOR_EMAIL =       'lev@columbia.edu, nikul@ee.columbia.edu, yiyin@ee.columbia.edu'
 URL =                'https://github.com/fruitflybrain/neuroarch/'
 MAINTAINER =         'Yiyin Zhou'
 MAINTAINER_EMAIL =   'yiyin@ee.columbia.edu'
 DESCRIPTION =        'A graph-based platform for representing Drosophila brain architectures'
 LONG_DESCRIPTION =   DESCRIPTION
@@ -59,15 +59,15 @@
         maintainer = MAINTAINER,
         maintainer_email = MAINTAINER_EMAIL,
         namespace_packages = NAMESPACE_PACKAGES,
         packages = PACKAGES,
         include_package_data = True,
         install_requires = [
             'daff',
-            'networkx>=2.4,<3',
+            'networkx>=2.4',
             'numpy',
             'pandas',
             'path.py',
             'deepdiff',
             'tqdm'],
         extra_requires = {
             'doc': docs_extras,
```

### Comparing `neuroarch-0.4.2/tests/test_conv_nx.py` & `neuroarch-0.4.3/tests/test_conv_nx.py`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/tests/test_conv_pd.py` & `neuroarch-0.4.3/tests/test_conv_pd.py`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/tests/test_conv_utils.py` & `neuroarch-0.4.3/tests/test_conv_utils.py`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/tests/test_diff.py` & `neuroarch-0.4.3/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `neuroarch-0.4.2/tests/test_nxtools.py` & `neuroarch-0.4.3/tests/test_nxtools.py`

 * *Files identical despite different names*

