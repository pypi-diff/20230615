# Comparing `tmp/matgl-0.5.5.tar.gz` & `tmp/matgl-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matgl-0.5.5.tar", last modified: Tue Jun 13 19:39:49 2023, max compression
+gzip compressed data, was "matgl-0.5.6.tar", last modified: Thu Jun 15 04:34:46 2023, max compression
```

## Comparing `matgl-0.5.5.tar` & `matgl-0.5.6.tar`

### file list

```diff
@@ -1,53 +1,56 @@
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-13 19:39:49.623075 matgl-0.5.5/
--rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-06-13 15:50:33.000000 matgl-0.5.5/LICENSE
--rw-r--r--   0 shyue      (501) staff       (20)    10799 2023-06-13 19:39:49.622886 matgl-0.5.5/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)     9630 2023-06-13 15:50:27.000000 matgl-0.5.5/README.md
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-13 19:39:49.613849 matgl-0.5.5/matgl/
--rw-r--r--   0 shyue      (501) staff       (20)      394 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/__init__.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-13 19:39:49.615036 matgl-0.5.5/matgl/apps/
--rw-r--r--   0 shyue      (501) staff       (20)      180 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/apps/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     4169 2023-06-13 19:16:50.000000 matgl-0.5.5/matgl/apps/pes.py
--rw-r--r--   0 shyue      (501) staff       (20)     1873 2023-06-13 19:21:16.000000 matgl-0.5.5/matgl/config.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-13 19:39:49.615516 matgl-0.5.5/matgl/data/
--rw-r--r--   0 shyue      (501) staff       (20)       55 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/data/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2503 2023-06-13 19:04:59.000000 matgl-0.5.5/matgl/data/transformer.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-13 19:39:49.616344 matgl-0.5.5/matgl/ext/
--rw-r--r--   0 shyue      (501) staff       (20)      118 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/ext/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    15474 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/ext/ase.py
--rw-r--r--   0 shyue      (501) staff       (20)     5268 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/ext/pymatgen.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-13 19:39:49.617581 matgl-0.5.5/matgl/graph/
--rw-r--r--   0 shyue      (501) staff       (20)       52 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/graph/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     5101 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/graph/compute.py
--rw-r--r--   0 shyue      (501) staff       (20)      513 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/graph/converters.py
--rw-r--r--   0 shyue      (501) staff       (20)    11483 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/graph/data.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-13 19:39:49.620021 matgl-0.5.5/matgl/layers/
--rw-r--r--   0 shyue      (501) staff       (20)      645 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/layers/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2008 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/layers/_activations.py
--rw-r--r--   0 shyue      (501) staff       (20)     3541 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/layers/_atom_ref.py
--rw-r--r--   0 shyue      (501) staff       (20)     2184 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/layers/_bond.py
--rw-r--r--   0 shyue      (501) staff       (20)     6029 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/layers/_core.py
--rw-r--r--   0 shyue      (501) staff       (20)     3509 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/layers/_embedding.py
--rw-r--r--   0 shyue      (501) staff       (20)    16496 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/layers/_graph_convolution.py
--rw-r--r--   0 shyue      (501) staff       (20)     3872 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/layers/_readout.py
--rw-r--r--   0 shyue      (501) staff       (20)     3609 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/layers/_three_body.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-13 19:39:49.620928 matgl-0.5.5/matgl/models/
--rw-r--r--   0 shyue      (501) staff       (20)      187 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/models/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    11362 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/models/_m3gnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     9539 2023-06-13 19:23:41.000000 matgl-0.5.5/matgl/models/_megnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     2148 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/models/_wrappers.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-13 19:39:49.622524 matgl-0.5.5/matgl/utils/
--rw-r--r--   0 shyue      (501) staff       (20)       61 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/utils/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)      799 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/utils/cutoff.py
--rw-r--r--   0 shyue      (501) staff       (20)    10578 2023-06-13 19:32:30.000000 matgl-0.5.5/matgl/utils/io.py
--rw-r--r--   0 shyue      (501) staff       (20)    16610 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/utils/maths.py
--rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-03-22 18:49:07.000000 matgl-0.5.5/matgl/utils/sb_roots.npy
--rw-r--r--   0 shyue      (501) staff       (20)    12546 2023-06-13 19:01:28.000000 matgl-0.5.5/matgl/utils/training.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-13 19:39:49.614575 matgl-0.5.5/matgl.egg-info/
--rw-r--r--   0 shyue      (501) staff       (20)    10799 2023-06-13 19:39:49.000000 matgl-0.5.5/matgl.egg-info/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)      935 2023-06-13 19:39:49.000000 matgl-0.5.5/matgl.egg-info/SOURCES.txt
--rw-r--r--   0 shyue      (501) staff       (20)        1 2023-06-13 19:39:49.000000 matgl-0.5.5/matgl.egg-info/dependency_links.txt
--rw-r--r--   0 shyue      (501) staff       (20)       41 2023-06-13 19:39:49.000000 matgl-0.5.5/matgl.egg-info/requires.txt
--rw-r--r--   0 shyue      (501) staff       (20)        6 2023-06-13 19:39:49.000000 matgl-0.5.5/matgl.egg-info/top_level.txt
--rw-r--r--   0 shyue      (501) staff       (20)     2343 2023-06-13 19:04:33.000000 matgl-0.5.5/pyproject.toml
--rw-r--r--   0 shyue      (501) staff       (20)       38 2023-06-13 19:39:49.623128 matgl-0.5.5/setup.cfg
--rw-r--r--   0 shyue      (501) staff       (20)     1913 2023-06-13 19:31:57.000000 matgl-0.5.5/setup.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.364474 matgl-0.5.6/
+-rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-06-13 15:50:33.000000 matgl-0.5.6/LICENSE
+-rw-r--r--   0 shyue      (501) staff       (20)    12119 2023-06-15 04:34:46.364309 matgl-0.5.6/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)    10950 2023-06-15 04:33:22.000000 matgl-0.5.6/README.md
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.359264 matgl-0.5.6/matgl/
+-rw-r--r--   0 shyue      (501) staff       (20)      394 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.360303 matgl-0.5.6/matgl/apps/
+-rw-r--r--   0 shyue      (501) staff       (20)      180 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/apps/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4169 2023-06-13 19:16:50.000000 matgl-0.5.6/matgl/apps/pes.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1996 2023-06-14 22:12:57.000000 matgl-0.5.6/matgl/config.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.360553 matgl-0.5.6/matgl/data/
+-rw-r--r--   0 shyue      (501) staff       (20)       55 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/data/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2503 2023-06-13 19:04:59.000000 matgl-0.5.6/matgl/data/transformer.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.360888 matgl-0.5.6/matgl/ext/
+-rw-r--r--   0 shyue      (501) staff       (20)      118 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/ext/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    15898 2023-06-14 19:28:56.000000 matgl-0.5.6/matgl/ext/ase.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5268 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/ext/pymatgen.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.361328 matgl-0.5.6/matgl/graph/
+-rw-r--r--   0 shyue      (501) staff       (20)       52 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/graph/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5101 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/graph/compute.py
+-rw-r--r--   0 shyue      (501) staff       (20)      513 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/graph/converters.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11483 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/graph/data.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.362559 matgl-0.5.6/matgl/layers/
+-rw-r--r--   0 shyue      (501) staff       (20)      676 2023-06-15 04:03:30.000000 matgl-0.5.6/matgl/layers/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2030 2023-06-14 19:29:50.000000 matgl-0.5.6/matgl/layers/_activations.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3541 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/layers/_atom_ref.py
+-rw-r--r--   0 shyue      (501) staff       (20)     9428 2023-06-15 04:30:45.000000 matgl-0.5.6/matgl/layers/_basis.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2186 2023-06-15 03:59:01.000000 matgl-0.5.6/matgl/layers/_bond.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6029 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/layers/_core.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3509 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/layers/_embedding.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16554 2023-06-14 19:31:44.000000 matgl-0.5.6/matgl/layers/_graph_convolution.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3872 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/layers/_readout.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3912 2023-06-15 04:31:02.000000 matgl-0.5.6/matgl/layers/_three_body.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.362992 matgl-0.5.6/matgl/models/
+-rw-r--r--   0 shyue      (501) staff       (20)      187 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/models/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11480 2023-06-14 15:48:06.000000 matgl-0.5.6/matgl/models/_m3gnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     9539 2023-06-14 15:46:44.000000 matgl-0.5.6/matgl/models/_megnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2147 2023-06-15 04:29:37.000000 matgl-0.5.6/matgl/models/_wrappers.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.363726 matgl-0.5.6/matgl/utils/
+-rw-r--r--   0 shyue      (501) staff       (20)       61 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/utils/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)      799 2023-06-13 19:01:28.000000 matgl-0.5.6/matgl/utils/cutoff.py
+-rw-r--r--   0 shyue      (501) staff       (20)    10527 2023-06-14 19:27:59.000000 matgl-0.5.6/matgl/utils/io.py
+-rw-r--r--   0 shyue      (501) staff       (20)     7147 2023-06-15 04:31:50.000000 matgl-0.5.6/matgl/utils/maths.py
+-rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-03-22 18:49:07.000000 matgl-0.5.6/matgl/utils/sb_roots.npy
+-rw-r--r--   0 shyue      (501) staff       (20)    12839 2023-06-14 19:36:00.000000 matgl-0.5.6/matgl/utils/training.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.359866 matgl-0.5.6/matgl.egg-info/
+-rw-r--r--   0 shyue      (501) staff       (20)    12119 2023-06-15 04:34:46.000000 matgl-0.5.6/matgl.egg-info/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)      979 2023-06-15 04:34:46.000000 matgl-0.5.6/matgl.egg-info/SOURCES.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        1 2023-06-15 04:34:46.000000 matgl-0.5.6/matgl.egg-info/dependency_links.txt
+-rw-r--r--   0 shyue      (501) staff       (20)       41 2023-06-15 04:34:46.000000 matgl-0.5.6/matgl.egg-info/requires.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        6 2023-06-15 04:34:46.000000 matgl-0.5.6/matgl.egg-info/top_level.txt
+-rw-r--r--   0 shyue      (501) staff       (20)     2427 2023-06-14 21:01:08.000000 matgl-0.5.6/pyproject.toml
+-rw-r--r--   0 shyue      (501) staff       (20)       38 2023-06-15 04:34:46.364520 matgl-0.5.6/setup.cfg
+-rw-r--r--   0 shyue      (501) staff       (20)     1913 2023-06-15 04:17:12.000000 matgl-0.5.6/setup.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-15 04:34:46.363836 matgl-0.5.6/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)      160 2023-06-14 22:12:57.000000 matgl-0.5.6/tests/test_config.py
```

### Comparing `matgl-0.5.5/LICENSE` & `matgl-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `matgl-0.5.5/PKG-INFO` & `matgl-0.5.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,12 @@
-Metadata-Version: 2.1
-Name: matgl
-Version: 0.5.5
-Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
-Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong
-Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
-Maintainer: Shyue Ping Ong
-Maintainer-email: ongsp@ucsd.edu
-Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
 [![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing%20-%20main/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
+[![Coverage Status](https://coveralls.io/repos/github/materialsvirtuallab/matgl/badge.svg?branch=main)](https://coveralls.io/github/materialsvirtuallab/matgl?branch=main)
 
 <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MatGL.png?raw=true" alt="matgl" width="30%" style="float: right">
 
 # Materials Graph Library
 
 Official Documentation: [link][doc]
 
@@ -61,33 +38,34 @@
 - v0.1.0 (Feb 16 2023): Initial implementations of M3GNet and MEGNet architectures have been completed. Expect
   bugs!
 
 ## Architectures
 
 <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic" width="50%">
 
-## MEGNet
+### MEGNet
 
-The [MatErials Graph Network (MEGNet)][megnet] is an implementation of DeepMind's [graph networks][graphnetwork] for
+[MatErials Graph Network (MEGNet)][megnet] is an implementation of DeepMind's [graph networks][graphnetwork] for
 machine learning in materials science. We have demonstrated its success in achieving low prediction errors in a broad
 array of properties in both [molecules and crystals][megnet]. New releases have included our recent work on
 [multi-fidelity materials property modeling][mfimegnet]. Figure 1 shows the sequential update steps of the graph
 network, whereby bonds, atoms, and global state attributes are updated using information from each other, generating an output graph.
 
-## M3GNet
+### M3GNet
 
-[M3GNet][m3gnet] is a new materials graph neural network architecture that incorporates 3-body interactions in MEGNet. An additional difference is the addition of the coordinates for atoms and
+[Materials 3-body Graph Network (M3GNet)][m3gnet] is a new materials graph neural network architecture that
+incorporates 3-body interactions in MEGNet. An additional difference is the addition of the coordinates for atoms and
 the 3×3 lattice matrix in crystals, which are necessary for obtaining tensorial quantities such as forces and
 stresses via auto-differentiation. As a framework, M3GNet has diverse applications, including:
 
 - **Interatomic potential development.** With the same training data, M3GNet performs similarly to state-of-the-art
   machine learning interatomic potentials (MLIPs). However, a key feature of a graph representation is its
   flexibility to scale to diverse chemical spaces. One of the key accomplishments of M3GNet is the development of a
-  *universal IP* that can work across the entire periodic table of the elements by training on relaxations performed
-  in the [Materials Project][mp].
+  [*universal IP*][m3gnet] that can work across the entire periodic table of the elements by training on relaxations
+  performed in the [Materials Project][mp].
 - **Surrogate models for property predictions.** Like the previous MEGNet architecture, M3GNet can be used to develop
   surrogate models for property predictions, achieving in many cases accuracies that are better or similar to other
   state-of-the-art ML models.
 
 For detailed performance benchmarks, please refer to the publications in the [References](#references) section.
 
 ## Installation
@@ -131,16 +109,16 @@
 ```
 
 ## Resources
 
 - [Jupyter notebooks][jupyternb] on the use of MatGL. These notebooks can be run on [Google Colab][colab]. This will
   be the primary form of tutorials for now.
 - [API documentation][apidocs] for all classes and methods.
-- [Developer's Guide](developer.md) has been written to outline the key design elements of matgl. This serves
-as a guiding documentation for developers wishing to train and contribute matgl models.
+- [Developer Guide](developer.md) outlines the key design elements of matgl, especially for developers wishing to
+  train and contribute matgl models.
 
 ## References
 
 A MatGL publication is currently being written. For now, pls refer to the CITATION.cff file for the citation
 information. If you are using any of the pretrained models, please cite the relevant works below:
 
 > **MEGNet**
@@ -156,37 +134,55 @@
 > **M3GNet**
 >
 > Chen, C., Ong, S.P. _A universal graph deep learning interatomic potential for the periodic table._ Nature
 > Computational Science, 2023, 2, 718–728. DOI: [10.1038/s43588-022-00349-3][m3gnet].
 
 ## FAQs
 
-1. The `M3GNet-MP-2021.2.8-PES` differs from the original tensorflow (TF) implementation!
+1. **The `M3GNet-MP-2021.2.8-PES` differs from the original tensorflow (TF) implementation!**
 
    Answer: `M3GNet-MP-2021.2.8-PES` is a refitted model with some data improvements and minor architectural changes.
    Porting over the weights from the TF version to DGL/PyTorch is non-trivial. We have performed reasonable benchmarking
    to ensure that the new implementation reproduces the broad error characteristics of the original TF implementation
    (see [examples][jupyternb]). However, it is not expected to reproduce the TF version exactly. This refitted model
    serves as a baseline for future model improvements. We do not believe there is value in expending the resources
    to reproduce the TF version exactly.
 
-2. I am getting errors with `matgl.load_model()`!
+2. **I am getting errors with `matgl.load_model()`!**
 
    Answer: The most likely reason is that you have a cached older version of the model. We often refactor models to
    ensure the best implementation. This can usually be solved by updating your matgl to the latest version
    and clearing your cache using:
 
    ```bash
    pip install matgl --upgrade
    python -c "import matgl; matgl.clear_cache()"
    ```
 
    On the next run, the latest model will be downloaded. With effect from v0.5.2, we have implemented a model
    versioning scheme that will detect code vs model version conflicts and alert the user of such problems.
 
+3. **What pre-trained models should I be using?**
+
+   Answer: There is no one definitive answer. In general, the newer the architecture and dataset, the more likely
+   the model performs better. However, it should also be noted that a model operating on a more diverse dataset may
+   compromise on  performance on a specific system. The best way is to look at the READMEs included with each model
+   and do some tests on the systems you are interested in.
+
+4. **How do I contribute to matgl?**
+
+   Answer: For code contributions, please fork and submit pull requests. You should read the [developer guide]
+   (developer) to understand the general design guidelines.
+
+   We welcome pre-trained model contributions as well, which should also be submitted via PRs. Please follow the
+   folder structure of the pretrained models. In particular, we expect all models to come with a README and notebook
+   documenting its use and its key performance metrics. Also, we expect contributions to be on new properties
+   or systems or to significantly outperform the existing models. We will develop an alternative means for model
+   sharing in the future.
+
 ## Acknowledgments
 
 This work was primarily supported by the [Materials Project][mp], funded by the U.S. Department of Energy, Office of
 Science, Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
 DE-AC02-05-CH11231: Materials Project program KC23MP. This work used the Expanse supercomputing cluster at the Extreme
 Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number
 ACI-1548562.
```

### Comparing `matgl-0.5.5/README.md` & `matgl-0.5.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,36 @@
+Metadata-Version: 2.1
+Name: matgl
+Version: 0.5.6
+Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
+Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong
+Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
+Maintainer: Shyue Ping Ong
+Maintainer-email: ongsp@ucsd.edu
+Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Chemistry
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
 [![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing%20-%20main/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
+[![Coverage Status](https://coveralls.io/repos/github/materialsvirtuallab/matgl/badge.svg?branch=main)](https://coveralls.io/github/materialsvirtuallab/matgl?branch=main)
 
 <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MatGL.png?raw=true" alt="matgl" width="30%" style="float: right">
 
 # Materials Graph Library
 
 Official Documentation: [link][doc]
 
@@ -37,33 +62,34 @@
 - v0.1.0 (Feb 16 2023): Initial implementations of M3GNet and MEGNet architectures have been completed. Expect
   bugs!
 
 ## Architectures
 
 <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic" width="50%">
 
-## MEGNet
+### MEGNet
 
-The [MatErials Graph Network (MEGNet)][megnet] is an implementation of DeepMind's [graph networks][graphnetwork] for
+[MatErials Graph Network (MEGNet)][megnet] is an implementation of DeepMind's [graph networks][graphnetwork] for
 machine learning in materials science. We have demonstrated its success in achieving low prediction errors in a broad
 array of properties in both [molecules and crystals][megnet]. New releases have included our recent work on
 [multi-fidelity materials property modeling][mfimegnet]. Figure 1 shows the sequential update steps of the graph
 network, whereby bonds, atoms, and global state attributes are updated using information from each other, generating an output graph.
 
-## M3GNet
+### M3GNet
 
-[M3GNet][m3gnet] is a new materials graph neural network architecture that incorporates 3-body interactions in MEGNet. An additional difference is the addition of the coordinates for atoms and
+[Materials 3-body Graph Network (M3GNet)][m3gnet] is a new materials graph neural network architecture that
+incorporates 3-body interactions in MEGNet. An additional difference is the addition of the coordinates for atoms and
 the 3×3 lattice matrix in crystals, which are necessary for obtaining tensorial quantities such as forces and
 stresses via auto-differentiation. As a framework, M3GNet has diverse applications, including:
 
 - **Interatomic potential development.** With the same training data, M3GNet performs similarly to state-of-the-art
   machine learning interatomic potentials (MLIPs). However, a key feature of a graph representation is its
   flexibility to scale to diverse chemical spaces. One of the key accomplishments of M3GNet is the development of a
-  *universal IP* that can work across the entire periodic table of the elements by training on relaxations performed
-  in the [Materials Project][mp].
+  [*universal IP*][m3gnet] that can work across the entire periodic table of the elements by training on relaxations
+  performed in the [Materials Project][mp].
 - **Surrogate models for property predictions.** Like the previous MEGNet architecture, M3GNet can be used to develop
   surrogate models for property predictions, achieving in many cases accuracies that are better or similar to other
   state-of-the-art ML models.
 
 For detailed performance benchmarks, please refer to the publications in the [References](#references) section.
 
 ## Installation
@@ -107,16 +133,16 @@
 ```
 
 ## Resources
 
 - [Jupyter notebooks][jupyternb] on the use of MatGL. These notebooks can be run on [Google Colab][colab]. This will
   be the primary form of tutorials for now.
 - [API documentation][apidocs] for all classes and methods.
-- [Developer's Guide](developer.md) has been written to outline the key design elements of matgl. This serves
-as a guiding documentation for developers wishing to train and contribute matgl models.
+- [Developer Guide](developer.md) outlines the key design elements of matgl, especially for developers wishing to
+  train and contribute matgl models.
 
 ## References
 
 A MatGL publication is currently being written. For now, pls refer to the CITATION.cff file for the citation
 information. If you are using any of the pretrained models, please cite the relevant works below:
 
 > **MEGNet**
@@ -132,37 +158,55 @@
 > **M3GNet**
 >
 > Chen, C., Ong, S.P. _A universal graph deep learning interatomic potential for the periodic table._ Nature
 > Computational Science, 2023, 2, 718–728. DOI: [10.1038/s43588-022-00349-3][m3gnet].
 
 ## FAQs
 
-1. The `M3GNet-MP-2021.2.8-PES` differs from the original tensorflow (TF) implementation!
+1. **The `M3GNet-MP-2021.2.8-PES` differs from the original tensorflow (TF) implementation!**
 
    Answer: `M3GNet-MP-2021.2.8-PES` is a refitted model with some data improvements and minor architectural changes.
    Porting over the weights from the TF version to DGL/PyTorch is non-trivial. We have performed reasonable benchmarking
    to ensure that the new implementation reproduces the broad error characteristics of the original TF implementation
    (see [examples][jupyternb]). However, it is not expected to reproduce the TF version exactly. This refitted model
    serves as a baseline for future model improvements. We do not believe there is value in expending the resources
    to reproduce the TF version exactly.
 
-2. I am getting errors with `matgl.load_model()`!
+2. **I am getting errors with `matgl.load_model()`!**
 
    Answer: The most likely reason is that you have a cached older version of the model. We often refactor models to
    ensure the best implementation. This can usually be solved by updating your matgl to the latest version
    and clearing your cache using:
 
    ```bash
    pip install matgl --upgrade
    python -c "import matgl; matgl.clear_cache()"
    ```
 
    On the next run, the latest model will be downloaded. With effect from v0.5.2, we have implemented a model
    versioning scheme that will detect code vs model version conflicts and alert the user of such problems.
 
+3. **What pre-trained models should I be using?**
+
+   Answer: There is no one definitive answer. In general, the newer the architecture and dataset, the more likely
+   the model performs better. However, it should also be noted that a model operating on a more diverse dataset may
+   compromise on  performance on a specific system. The best way is to look at the READMEs included with each model
+   and do some tests on the systems you are interested in.
+
+4. **How do I contribute to matgl?**
+
+   Answer: For code contributions, please fork and submit pull requests. You should read the [developer guide]
+   (developer) to understand the general design guidelines.
+
+   We welcome pre-trained model contributions as well, which should also be submitted via PRs. Please follow the
+   folder structure of the pretrained models. In particular, we expect all models to come with a README and notebook
+   documenting its use and its key performance metrics. Also, we expect contributions to be on new properties
+   or systems or to significantly outperform the existing models. We will develop an alternative means for model
+   sharing in the future.
+
 ## Acknowledgments
 
 This work was primarily supported by the [Materials Project][mp], funded by the U.S. Department of Energy, Office of
 Science, Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
 DE-AC02-05-CH11231: Materials Project program KC23MP. This work used the Expanse supercomputing cluster at the Extreme
 Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number
 ACI-1548562.
```

### Comparing `matgl-0.5.5/matgl/apps/pes.py` & `matgl-0.5.6/matgl/apps/pes.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.5/matgl/config.py` & `matgl-0.5.6/matgl/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -102,17 +102,21 @@
 MATGL_CACHE = Path(os.path.expanduser("~")) / ".cache/matgl"
 os.makedirs(MATGL_CACHE, exist_ok=True)
 
 # Download url for pre-trained models.
 PRETRAINED_MODELS_BASE_URL = "https://github.com/materialsvirtuallab/matgl/raw/main/pretrained_models/"
 
 
-def clear_cache():
-    """Deletes all files in the matgl.cache. This is used to clean out downloaded models."""
-    answer = ""
+def clear_cache(confirm: bool = True):
+    """Deletes all files in the matgl.cache. This is used to clean out downloaded models.
+
+    Args:
+        confirm: Whether to ask for confirmation. Default is True.
+    """
+    answer = "" if confirm else "y"
     while answer not in ("y", "n"):
         answer = input(f"Do you really want to delete everything in {MATGL_CACHE} (y|n)? ").lower().strip()
     if answer == "y":
         try:
             shutil.rmtree(MATGL_CACHE)
         except FileNotFoundError:
             print(f"matgl cache dir {MATGL_CACHE!r} not found")
```

### Comparing `matgl-0.5.5/matgl/data/transformer.py` & `matgl-0.5.6/matgl/data/transformer.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.5/matgl/ext/ase.py` & `matgl-0.5.6/matgl/ext/ase.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,31 +104,34 @@
         g.ndata["volume"] = tensor([volume for i in range(atomic_number.shape[0])])
         state_attr = [0.0, 0.0]
         g.edata["pbc_offshift"] = torch.matmul(tensor(images), tensor(lattice_matrix))
         return g, state_attr
 
 
 class M3GNetCalculator(Calculator):
-    """M3GNet calculator based on ase Calculator."""
+    """M3GNet calculator for ASE."""
 
     implemented_properties = ["energy", "free_energy", "forces", "stress", "hessian"]
 
     def __init__(
         self,
         potential: Potential,
         state_attr: torch.tensor = None,
         stress_weight: float = 1.0,
         **kwargs,
     ):
-        r"""Args:
-        potential (Potential): m3gnet.models.Potential
-        state_attr (tensor): State attribute
-        compute_stress (bool): whether to calculate the stress
-        stress_weight (float): the stress weight.
-        **kwargs: Kwargs pass through to super().__init__().
+        """
+        Init M3GNetCalculator with a Potential.
+
+        Args:
+            potential (Potential): m3gnet.models.Potential
+            state_attr (tensor): State attribute
+            compute_stress (bool): whether to calculate the stress
+            stress_weight (float): the stress weight.
+            **kwargs: Kwargs pass through to super().__init__().
         """
         super().__init__(**kwargs)
         self.potential = potential
         self.compute_stress = potential.calc_stresses
         self.compute_hessian = potential.calc_hessian
         self.stress_weight = stress_weight
         self.state_attr = state_attr
@@ -137,20 +140,23 @@
 
     def calculate(
         self,
         atoms: Atoms | None = None,
         properties: list | None = None,
         system_changes: list | None = None,
     ):
-        """Args:
-        atoms (ase.Atoms): ase Atoms object
-        properties (list): list of properties to calculate
-        system_changes (list): monitor which properties of atoms were
-        changed for new calculation. If not, the previous calculation
-        results will be loaded.
+        """
+        Perform calculation for an input Atoms.
+
+        Args:
+            atoms (ase.Atoms): ase Atoms object
+            properties (list): list of properties to calculate
+            system_changes (list): monitor which properties of atoms were
+                changed for new calculation. If not, the previous calculation
+                results will be loaded.
         """
         properties = properties or ["energy"]
         system_changes = system_changes or all_changes
         super().calculate(atoms=atoms, properties=properties, system_changes=system_changes)
         graph, state_attr_default = Atoms2Graph(self.element_types, self.cutoff).get_graph(atoms)  # type: ignore
         if self.state_attr is not None:
             energies, forces, stresses, hessians = self.potential(graph, self.state_attr)
@@ -174,22 +180,23 @@
         self,
         potential: Potential = None,
         state_attr: torch.tensor = None,
         optimizer: Optimizer | str = "FIRE",
         relax_cell: bool = True,
         stress_weight: float = 0.01,
     ):
-        """Args:
-        potential (Potential): a M3GNet potential, a str path to a saved model or a short name for saved model
-        that comes with M3GNet distribution
-        state_attr (torch.tensor): State attr.
-        optimizer (str or ase Optimizer): the optimization algorithm.
-        Defaults to "FIRE"
-        relax_cell (bool): whether to relax the lattice cell
-        stress_weight (float): the stress weight for relaxation.
+        """
+        Args:
+            potential (Potential): a M3GNet potential, a str path to a saved model or a short name for saved model
+            that comes with M3GNet distribution
+            state_attr (torch.tensor): State attr.
+            optimizer (str or ase Optimizer): the optimization algorithm.
+            Defaults to "FIRE"
+            relax_cell (bool): whether to relax the lattice cell
+            stress_weight (float): the stress weight for relaxation.
         """
         if isinstance(optimizer, str):
             optimizer_obj = OPTIMIZERS.get(optimizer, None)
         elif optimizer is None:
             raise ValueError("Optimizer cannot be None")
         else:
             optimizer_obj = optimizer
@@ -208,23 +215,26 @@
         fmax: float = 0.1,
         steps: int = 500,
         traj_file: str = None,
         interval=1,
         verbose=False,
         **kwargs,
     ):
-        r"""Args:
-        atoms (Atoms): the atoms for relaxation
-        fmax (float): total force tolerance for relaxation convergence.
-        Here fmax is a sum of force and stress forces
-        steps (int): max number of steps for relaxation
-        traj_file (str): the trajectory file for saving
-        interval (int): the step interval for saving the trajectories
-        verbose (bool): Whether to have verbose output.
-        **kwargs: Kwargs pass-through to optimizer.
+        """
+        Relax an input Atoms.
+
+        Args:
+            atoms (Atoms): the atoms for relaxation
+            fmax (float): total force tolerance for relaxation convergence.
+            Here fmax is a sum of force and stress forces
+            steps (int): max number of steps for relaxation
+            traj_file (str): the trajectory file for saving
+            interval (int): the step interval for saving the trajectories
+            verbose (bool): Whether to have verbose output.
+            kwargs: Kwargs pass-through to optimizer.
         """
         if isinstance(atoms, (Structure, Molecule)):
             atoms = self.ase_adaptor.get_atoms(atoms)
         atoms.set_calculator(self.calculator)
         stream = sys.stdout if verbose else io.StringIO()
         with contextlib.redirect_stdout(stream):
             obs = TrajectoryObserver(atoms)
@@ -247,16 +257,19 @@
 
 class TrajectoryObserver:
     """Trajectory observer is a hook in the relaxation process that saves the
     intermediate structures.
     """
 
     def __init__(self, atoms: Atoms) -> None:
-        """Args:
-        atoms (Atoms): the structure to observe.
+        """
+        Init the Trajectory Observer from a Atoms.
+
+        Args:
+            atoms (Atoms): Structure to observe.
         """
         self.atoms = atoms
         self.energies: list[float] = []
         self.forces: list[np.ndarray] = []
         self.stresses: list[np.ndarray] = []
         self.atom_positions: list[np.ndarray] = []
         self.cells: list[np.ndarray] = []
@@ -271,15 +284,16 @@
 
     def compute_energy(self) -> float:
         """Calculate the potential energy."""
         energy = self.atoms.get_potential_energy()
         return energy
 
     def save(self, filename: str) -> None:
-        """Save the trajectory to file
+        """Save the trajectory to file.
+
         Args:
             filename (str): filename to save the trajectory.
         """
         out = {
             "energy": self.energies,
             "forces": self.forces,
             "stresses": self.stresses,
@@ -307,31 +321,34 @@
         taup: float | None = None,
         compressibility_au: float | None = None,
         trajectory: str | Trajectory | None = None,
         logfile: str | None = None,
         loginterval: int = 1,
         append_trajectory: bool = False,
     ):
-        """Args:
-        atoms (Atoms): atoms to run the MD
-        potential (Potential): potential for calculating the energy, force,
-        stress of the atoms
-        state_attr (torch.tensor): State attr.
-        ensemble (str): choose from 'nvt' or 'npt'. NPT is not tested,
-        use with extra caution
-        temperature (float): temperature for MD simulation, in K
-        timestep (float): time step in fs
-        pressure (float): pressure in eV/A^3
-        taut (float): time constant for Berendsen temperature coupling
-        taup (float): time constant for pressure coupling
-        compressibility_au (float): compressibility of the material in A^3/eV
-        trajectory (str or Trajectory): Attach trajectory object
-        logfile (str): open this file for recording MD outputs
-        loginterval (int): write to log file every interval steps
-        append_trajectory (bool): Whether to append to prev trajectory.
+        """
+        Init the MD simulation.
+
+        Args:
+            atoms (Atoms): atoms to run the MD
+            potential (Potential): potential for calculating the energy, force,
+            stress of the atoms
+            state_attr (torch.tensor): State attr.
+            ensemble (str): choose from 'nvt' or 'npt'. NPT is not tested,
+            use with extra caution
+            temperature (float): temperature for MD simulation, in K
+            timestep (float): time step in fs
+            pressure (float): pressure in eV/A^3
+            taut (float): time constant for Berendsen temperature coupling
+            taup (float): time constant for pressure coupling
+            compressibility_au (float): compressibility of the material in A^3/eV
+            trajectory (str or Trajectory): Attach trajectory object
+            logfile (str): open this file for recording MD outputs
+            loginterval (int): write to log file every interval steps
+            append_trajectory (bool): Whether to append to prev trajectory.
         """
         if isinstance(atoms, (Structure, Molecule)):
             atoms = AseAtomsAdaptor().get_atoms(atoms)
         self.atoms = atoms
         self.atoms.set_calculator(M3GNetCalculator(potential=potential, state_attr=state_attr))
 
         if taut is None:
@@ -410,15 +427,16 @@
 
         Args:
             steps (int): number of MD steps
         """
         self.dyn.run(steps)
 
     def set_atoms(self, atoms: Atoms):
-        """Set new atoms to run MD
+        """Set new atoms to run MD.
+
         Args:
             atoms (Atoms): new atoms for running MD.
         """
         calculator = self.atoms.calc
         self.atoms = atoms
         self.dyn.atoms = atoms
         self.dyn.atoms.set_calculator(calculator)
```

### Comparing `matgl-0.5.5/matgl/ext/pymatgen.py` & `matgl-0.5.6/matgl/ext/pymatgen.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.5/matgl/graph/compute.py` & `matgl-0.5.6/matgl/graph/compute.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.5/matgl/graph/converters.py` & `matgl-0.5.6/matgl/graph/converters.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.5/matgl/graph/data.py` & `matgl-0.5.6/matgl/graph/data.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.5/matgl/layers/__init__.py` & `matgl-0.5.6/matgl/layers/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """This package implements the layers for M*GNet."""
 from __future__ import annotations
 
 from matgl.layers._activations import SoftExponential, SoftPlus2
 from matgl.layers._atom_ref import AtomRef
+from matgl.layers._basis import SphericalBesselWithHarmonics
 from matgl.layers._bond import BondExpansion
 from matgl.layers._core import MLP, EdgeSet2Set, GatedMLP
 from matgl.layers._embedding import EmbeddingBlock
 from matgl.layers._graph_convolution import M3GNetBlock, M3GNetGraphConv, MEGNetBlock, MEGNetGraphConv
 from matgl.layers._readout import ReduceReadOut, Set2SetReadOut, WeightedReadOut, WeightedReadOutPair
-from matgl.layers._three_body import SphericalBesselWithHarmonics, ThreeBodyInteractions
+from matgl.layers._three_body import ThreeBodyInteractions
```

### Comparing `matgl-0.5.5/matgl/layers/_activations.py` & `matgl-0.5.6/matgl/layers/_activations.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,24 +32,23 @@
 
 class SoftExponential(nn.Module):
     """Soft exponential activation.
     When x < 0, SoftExponential(x,alpha) = -log(1-alpha(x+alpha))/alpha
     When x = 0, SoftExponential(x,alpha) = 0
     When x > 0, SoftExponential(x,alpha) = (exp(alpha*x)-1)/alpha + alpha.
 
-
-    References:
-        - See related paper:
-        https://arxiv.org/pdf/1602.01321.pdf
-
+    References: https://arxiv.org/pdf/1602.01321.pdf
     """
 
     def __init__(self, alpha: float = None):
-        """Args:
-        alpha (float): adjustable Torch parameter during the training.
+        """
+        Init SoftExponential with alpha value.
+
+        Args:
+            alpha (float): adjustable Torch parameter during the training.
         """
         super().__init__()
 
         # initialize alpha
         if alpha is None:
             self.alpha = nn.Parameter(torch.tensor(0.0))
         else:
```

### Comparing `matgl-0.5.5/matgl/layers/_atom_ref.py` & `matgl-0.5.6/matgl/layers/_atom_ref.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.5/matgl/layers/_bond.py` & `matgl-0.5.6/matgl/layers/_bond.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Generate bond features based on spherical bessel functions or gaussian expansion."""
 from __future__ import annotations
 
 import torch
 from torch import nn
 
-from matgl.utils.maths import GaussianExpansion, SphericalBesselFunction
+from matgl.layers._basis import GaussianExpansion, SphericalBesselFunction
 
 
 class BondExpansion(nn.Module):
     """Expand pair distances into a set of spherical bessel or gaussian functions."""
 
     def __init__(
         self,
```

### Comparing `matgl-0.5.5/matgl/layers/_core.py` & `matgl-0.5.6/matgl/layers/_core.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.5/matgl/layers/_embedding.py` & `matgl-0.5.6/matgl/layers/_embedding.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.5/matgl/layers/_graph_convolution.py` & `matgl-0.5.6/matgl/layers/_graph_convolution.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,21 +131,24 @@
 
 class MEGNetBlock(Module):
     """A MEGNet block comprising a sequence of update operations."""
 
     def __init__(
         self, dims: list[int], conv_hiddens: list[int], act: Module, dropout: float | None = None, skip: bool = True
     ) -> None:
-        """TODO: Add docs.
-        :param dims: architecture of dense layers before graph convolution
-        :param conv_hiddens: architecture of graph convolution
-        :param act: activation type
-        :param dropout: Randomly zeroes some elements in the input tensor with given probability (0 < x < 1) according
-            to a Bernoulli distribution
-        :param skip: residual block.
+        """
+        Init the MEGNet block with key parameters.
+
+        Args:
+            dims: Dimension of dense layers before graph convolution.
+            conv_hiddens: Architecture of hidden layers of graph convolution.
+            act: Activation type.
+            dropout: Randomly zeroes some elements in the input tensor with given probability (0 < x < 1) according
+                to a Bernoulli distribution.
+            skip: Residual block.
         """
         super().__init__()
         self.has_dense = len(dims) > 1
         self.activation = act
         conv_dim = dims[-1]
         out_dim = conv_hiddens[-1]
```

### Comparing `matgl-0.5.5/matgl/layers/_readout.py` & `matgl-0.5.6/matgl/layers/_readout.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.5/matgl/layers/_three_body.py` & `matgl-0.5.6/matgl/layers/_three_body.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,85 +1,57 @@
 """Three-Body interaction implementations."""
 
 from __future__ import annotations
 
 import dgl
+import numpy as np
 import torch
 from torch import nn
 
 from matgl.utils.maths import (
-    SphericalBesselFunction,
-    SphericalHarmonicsFunction,
-    combine_sbf_shf,
+    _block_repeat,
     get_segment_indices_from_n,
     scatter_sum,
 )
 
 
-class SphericalBesselWithHarmonics(nn.Module):
-    """Expansion of basis using Spherical Bessel and Harmonics."""
-
-    def __init__(self, max_n: int, max_l: int, cutoff: float, use_smooth: bool, use_phi: bool):
-        """:param max_n: Degree of radial basis functions
-        :param max_l: Degree of angular basis functions
-        :param cutoff: Cutoff sphere
-        :param use_smooth: Whether using smooth version of SBFs or not
-        :param use_phi: using phi as angular basis functions
-        """
-        super().__init__()
-
-        assert max_n <= 64
-        self.max_n = max_n
-        self.max_l = max_l
-        self.cutoff = cutoff
-        self.use_phi = use_phi
-        self.use_smooth = use_smooth
-
-        # retrieve formulas
-        self.shf = SphericalHarmonicsFunction(self.max_l, self.use_phi)
-        if self.use_smooth:
-            self.sbf = SphericalBesselFunction(self.max_l, self.max_n * self.max_l, self.cutoff, self.use_smooth)
-        else:
-            self.sbf = SphericalBesselFunction(self.max_l, self.max_n, self.cutoff, self.use_smooth)
-
-    def forward(self, line_graph):
-        sbf = self.sbf(line_graph.edata["triple_bond_lengths"])
-        shf = self.shf(line_graph.edata["cos_theta"], line_graph.edata["phi"])
-        return combine_sbf_shf(sbf, shf, max_n=self.max_n, max_l=self.max_l, use_phi=self.use_phi)
-
-
 class ThreeBodyInteractions(nn.Module):
     """Include 3D interactions to the bond update."""
 
     def __init__(self, update_network_atom: nn.Module, update_network_bond: nn.Module, **kwargs):
-        r"""Args:
-        update_network_atom: MLP for node features in Eq.2
-        update_network_bond: Gated-MLP for edge features in Eq.3
-        **kwargs: Kwargs pass-through to nn.Module.__init__().
+        """Init ThreeBodyInteractions.
+
+        Args:
+            update_network_atom: MLP for node features in Eq.2
+            update_network_bond: Gated-MLP for edge features in Eq.3
+            **kwargs: Kwargs pass-through to nn.Module.__init__().
         """
         super().__init__(**kwargs)
         self.update_network_atom = update_network_atom
         self.update_network_bond = update_network_bond
 
     def forward(
         self,
         graph: dgl.DGLGraph,
         line_graph: dgl.DGLGraph,
         three_basis: torch.tensor,
         three_cutoff: float,
         node_feat: torch.tensor,
         edge_feat: torch.tensor,
     ):
-        """Args:
-        graph: dgl graph
-        line_graph: line graph.
-        three_basis: three body basis expansion
-        three_cutoff: cutoff radius
-        node_feat: node features
-        edge_feat: edge features.
+        """
+        Forward function for ThreeBodyInteractions.
+
+        Args:
+            graph: dgl graph
+            line_graph: line graph.
+            three_basis: three body basis expansion
+            three_cutoff: cutoff radius
+            node_feat: node features
+            edge_feat: edge features.
         """
         end_atom_index = torch.gather(graph.edges()[1], 0, line_graph.edges()[1].to(torch.int64))
         atoms = self.update_network_atom(node_feat)
         end_atom_index = torch.unsqueeze(end_atom_index, 1)
         atoms = torch.squeeze(atoms[end_atom_index])
         basis = three_basis * atoms
         three_cutoff = torch.unsqueeze(three_cutoff, dim=1)
@@ -92,7 +64,47 @@
             basis.to(torch.float32),
             segment_ids=get_segment_indices_from_n(line_graph.ndata["n_triple_ij"]),
             num_segments=graph.num_edges(),
             dim=0,
         )
         edge_feat_updated = edge_feat + self.update_network_bond(new_bonds)
         return edge_feat_updated
+
+
+def combine_sbf_shf(sbf, shf, max_n: int, max_l: int, use_phi: bool):
+    """Combine the spherical Bessel function and the spherical Harmonics function.
+
+    For the spherical Bessel function, the column is ordered by
+        [n=[0, ..., max_n-1], n=[0, ..., max_n-1], ...], max_l blocks,
+
+    For the spherical Harmonics function, the column is ordered by
+        [m=[0], m=[-1, 0, 1], m=[-2, -1, 0, 1, 2], ...] max_l blocks, and each
+        block has 2*l + 1
+        if use_phi is False, then the columns become
+        [m=[0], m=[0], ...] max_l columns
+
+    Args:
+        sbf: torch.tensor spherical bessel function results
+        shf: torch.tensor spherical harmonics function results
+        max_n: int, max number of n
+        max_l: int, max number of l
+        use_phi: whether to use phi
+    Returns:
+    """
+    if sbf.size()[0] == 0:
+        return sbf
+
+    if not use_phi:
+        repeats_sbf = torch.tensor([1] * max_l * max_n)
+        block_size = [1] * max_l
+    else:
+        # [1, 1, 1, ..., 1, 3, 3, 3, ..., 3, ...]
+        repeats_sbf = torch.tensor(np.repeat(2 * np.arange(max_l) + 1, repeats=max_n))
+        # tf.repeat(2 * tf.range(max_l) + 1, repeats=max_n)
+        block_size = 2 * np.arange(max_l) + 1  # type: ignore
+        # 2 * tf.range(max_l) + 1
+    expanded_sbf = torch.repeat_interleave(sbf, repeats_sbf, 1)
+    expanded_shf = _block_repeat(shf, block_size=block_size, repeats=[max_n] * max_l)
+    shape = max_n * max_l
+    if use_phi:
+        shape *= max_l
+    return torch.reshape(expanded_sbf * expanded_shf, [-1, shape])
```

### Comparing `matgl-0.5.5/matgl/models/_m3gnet.py` & `matgl-0.5.6/matgl/models/_m3gnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Implementation of Materials 3-body Graph Network (M3GNet) model.
 
 The main improvement over MEGNet is the addition of many-body interactios terms, which improves efficiency of
 representation of local interactions for applications such as interatomic potentials. For more details on M3GNet,
 please refer to::
 
-```
-Chen, C., Ong, S.P. _A universal graph deep learning interatomic potential for the periodic table._ Nature
-Computational Science, 2023, 2, 718-728. DOI: 10.1038/s43588-022-00349-3.
-```
+    Chen, C., Ong, S.P. _A universal graph deep learning interatomic potential for the periodic table._ Nature
+    Computational Science, 2023, 2, 718-728. DOI: 10.1038/s43588-022-00349-3.
+
 """
 from __future__ import annotations
 
 import logging
 
 import dgl
 import torch
@@ -73,42 +72,43 @@
         niters_set2set: int = 3,
         nlayers_set2set: int = 3,
         field: str = "node_feat",
         include_state: bool = False,
         activation_type: str = "swish",
         **kwargs,
     ):
-        r"""Args:
-        element_types (tuple): list of elements appearing in the dataset
-        dim_node_embedding (int): number of embedded atomic features
-        dim_edge_embedding (int): number of edge features
-        dim_state_embedding (int): number of hidden neurons in state embedding
-        dim_state_feats (int): number of state features after linear layer
-        dim_state_types (int): number of state labels
-        max_n (int): number of radial basis expansion
-        max_l (int): number of angular expansion
-        nblocks (int): number of convolution blocks
-        rbf_type (str): radial basis function. choose from 'Gaussian' or 'SphericalBessel'
-        is_intensive (bool): whether the prediction is intensive
-        readout_type (str): the readout function type. choose from `set2set`,
-        `weighted_atom` and `reduce_atom`, default to `weighted_atom`
-        task_type (str): `classification` or `regression`, default to
-        `regression`
-        cutoff (float): cutoff radius of the graph
-        threebody_cutoff (float): cutoff radius for 3 body interaction
-        units (int): number of neurons in each MLP layer
-        ntargets (int): number of target properties
-        use_smooth (bool): whether using smooth Bessel functions
-        use_phi (bool): whether using phi angle
-        field (str): using either "node_feat" or "edge_feat" for Set2Set and Reduced readout
-        niters_set2set (int): number of set2set iterations
-        nlayers_set2set (int): number of set2set layers
-        include_state (bool): whether to include states features
-        activation_type (str): activation type. choose from 'swish', 'tanh', 'sigmoid', 'softplus2', 'softexp'
-        **kwargs: For future flexibility. Not used at the moment.
+        r"""
+        Args:
+            element_types (tuple): list of elements appearing in the dataset
+            dim_node_embedding (int): number of embedded atomic features
+            dim_edge_embedding (int): number of edge features
+            dim_state_embedding (int): number of hidden neurons in state embedding
+            dim_state_feats (int): number of state features after linear layer
+            dim_state_types (int): number of state labels
+            max_n (int): number of radial basis expansion
+            max_l (int): number of angular expansion
+            nblocks (int): number of convolution blocks
+            rbf_type (str): radial basis function. choose from 'Gaussian' or 'SphericalBessel'
+            is_intensive (bool): whether the prediction is intensive
+            readout_type (str): the readout function type. choose from `set2set`,
+            `weighted_atom` and `reduce_atom`, default to `weighted_atom`
+            task_type (str): `classification` or `regression`, default to
+            `regression`
+            cutoff (float): cutoff radius of the graph
+            threebody_cutoff (float): cutoff radius for 3 body interaction
+            units (int): number of neurons in each MLP layer
+            ntargets (int): number of target properties
+            use_smooth (bool): whether using smooth Bessel functions
+            use_phi (bool): whether using phi angle
+            field (str): using either "node_feat" or "edge_feat" for Set2Set and Reduced readout
+            niters_set2set (int): number of set2set iterations
+            nlayers_set2set (int): number of set2set layers
+            include_state (bool): whether to include states features
+            activation_type (str): activation type. choose from 'swish', 'tanh', 'sigmoid', 'softplus2', 'softexp'
+            **kwargs: For future flexibility. Not used at the moment.
         """
         super().__init__()
 
         self.save_args(locals(), kwargs)
 
         if activation_type == "swish":
             activation = nn.SiLU()  # type: ignore
```

### Comparing `matgl-0.5.5/matgl/models/_megnet.py` & `matgl-0.5.6/matgl/models/_megnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Implementation of MatErials Graph Network (MEGNet) model.
 
 Graph networks are a new machine learning (ML) paradigm that supports both relational reasoning and combinatorial
 generalization. For more details on MEGNet, please refer to::
 
-```
-Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. _Graph Networks as a Universal Machine Learning Framework for
-Molecules and Crystals._ Chem. Mater. 2019, 31 (9), 3564-3572. DOI: 10.1021/acs.chemmater.9b01294.
-```
+    Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. _Graph Networks as a Universal Machine Learning Framework for
+    Molecules and Crystals._ Chem. Mater. 2019, 31 (9), 3564-3572. DOI: 10.1021/acs.chemmater.9b01294.
 """
 from __future__ import annotations
 
 import logging
 
 import dgl
 import torch
```

### Comparing `matgl-0.5.5/matgl/models/_wrappers.py` & `matgl-0.5.6/matgl/models/_wrappers.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         """
         super().__init__()
         self.save_args(locals())
         self.model = model
         self.transformer = target_transformer
 
     def forward(self, *args, **kwargs):
-        r"""Args:
+        """Args:
             *args: Passthrough to parent model.forward method.
             **kwargs: Passthrough to parent model.forward method.
 
         Returns:
             Inverse transformed output.
         """
         output = self.model.forward(*args, **kwargs)
```

### Comparing `matgl-0.5.5/matgl/utils/cutoff.py` & `matgl-0.5.6/matgl/utils/cutoff.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.5/matgl/utils/io.py` & `matgl-0.5.6/matgl/utils/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,19 @@
 logger = logging.getLogger(__file__)
 
 
 class IOMixIn:
     """Mixin class for model saving and loading.
 
     For proper usage, models should subclass nn.Module and IOMix and the `save_args` method should be called
-    immediately after the `super().__init__()` call.
+    immediately after the `super().__init__()` call::
+
+        super().__init__()
+        self.save_args(locals(), kwargs)
 
-    ```
-    super().__init__()
-    self.save_args(locals(), kwargs)
-    ```
     """
 
     def save_args(self, locals: dict, kwargs: dict | None = None) -> None:
         r"""Method to save args into a private _init_args variable.
 
         This should be called after super in the __init__ method, e.g., `self.save_args(locals(), kwargs)`.
 
@@ -86,26 +85,28 @@
 
     @classmethod
     def load(cls, path: str | Path | dict, **kwargs):
         """Load the model weights from a directory.
 
         Args:
             path (str|path|dict): Path to saved model or name of pre-trained model. If it is a dict, it is assumed to
-                be of the form
-                {
-                    "model.pt": path to model.pt file,
-                    "state.pt": path to state file,
-                    "model.json": path to model.json file
-                }
+                be of the form::
+
+                    {
+                        "model.pt": path to model.pt file,
+                        "state.pt": path to state file,
+                        "model.json": path to model.json file
+                    }
+
                 Otherwise, the search order is path, followed by download from PRETRAINED_MODELS_BASE_URL
                 (with caching).
-            kwargs: Additional kwargs passed to RemoteFile class. E.g., a useful one might be force_download if you
+            **kwargs: Additional kwargs passed to RemoteFile class. E.g., a useful one might be force_download if you
                 want to update the model.
 
-        Returns: model_object if include_json is false. (model_object, dict) if include_json is True.
+        Returns: model_object.
         """
         fpaths = path if isinstance(path, dict) else _get_file_paths(Path(path), **kwargs)
 
         with open(fpaths["model.json"]) as f:
             model_data = json.load(f)
 
         _check_ver(cls, model_data)
```

### Comparing `matgl-0.5.5/matgl/utils/sb_roots.npy` & `matgl-0.5.6/matgl/utils/sb_roots.npy`

 * *Files identical despite different names*

### Comparing `matgl-0.5.5/matgl/utils/training.py` & `matgl-0.5.6/matgl/utils/training.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 from matgl.models import M3GNet
 
 
 class TrainerMixin:
     """Mix-in class implementing common functions for training."""
 
     def training_step(self, batch: tuple, batch_idx: int):
-        """Args:
+        """Training step.
+
+        Args:
             batch: Data batch.
             batch_idx: Batch index.
 
         Returns:
            Total loss.
         """
         results, batch_size = self.step(batch)  # type: ignore
@@ -41,31 +43,35 @@
 
     def on_train_epoch_end(self):
         """Step scheduler every epoch."""
         sch = self.lr_schedulers()
         sch.step()
 
     def validation_step(self, batch: tuple, batch_idx: int):
-        """Args:
-        batch: Data batch.
-        batch_idx: Batch index.
+        """Validation step.
+
+        Args:
+            batch: Data batch.
+            batch_idx: Batch index.
         """
         results, batch_size = self.step(batch)  # type: ignore
         self.log_dict(  # type: ignore
             {f"val_{key}": val for key, val in results.items()},
             batch_size=batch_size,
             on_epoch=True,
             on_step=False,
             prog_bar=True,
         )
 
     def test_step(self, batch: tuple, batch_idx: int):
-        """Args:
-        batch: Data batch.
-        batch_idx: Batch index.
+        """Test step.
+
+        Args:
+            batch: Data batch.
+            batch_idx: Batch index.
         """
         results, batch_size = self.step(batch)  # type: ignore
         self.log_dict(  # type: ignore
             {f"test_{key}": val for key, val in results.items()},
             batch_size=batch_size,
             on_epoch=True,
             on_step=False,
@@ -93,23 +99,29 @@
         return [
             optimizer,
         ], [
             scheduler,
         ]
 
     def on_test_model_eval(self, *args, **kwargs):
-        r"""Args:
-        *args: Pass-through
-        **kwargs: Pass-through.
+        """
+        Executed on model testing.
+
+        Args:
+            *args: Pass-through
+            **kwargs: Pass-through.
         """
         super().on_test_model_eval(*args, **kwargs)
         torch.set_grad_enabled(True)
 
     def predict_step(self, batch, batch_idx, dataloader_idx=0):
-        """Args:
+        """
+        Prediction step.
+
+        Args:
             batch: Data batch.
             batch_idx: Batch index.
             dataloader_idx: Data loader index.
 
         Returns:
             Prediction
         """
@@ -226,29 +238,32 @@
         loss: str = "mse_loss",
         optimizer: Optimizer | None = None,
         scheduler: lr_scheduler | None = None,
         lr: float = 0.001,
         decay_steps: int = 1000,
         decay_alpha: float = 0.01,
     ):
-        """Args:
-        model: Which type of the model for training
-        element_refs: element offset for PES
-        energy_weight: relative importance of energy
-        force_weight: relative importance of force
-        stress_weight: relative importance of stress
-        data_mean: average of training data
-        data_std: standard deviation of training data
-        calc_stress: whether stress calculation is required
-        loss: loss function used for training
-        optimizer: optimizer for training
-        scheduler: scheduler for training
-        lr: learning rate for training
-        decay_steps: number of steps for decaying learning rate
-        decay_alpha: parameter determines the minimum learning rate.
+        """
+        Init PotentialTrainer with key parameters.
+
+        Args:
+            model: Which type of the model for training
+            element_refs: element offset for PES
+            energy_weight: relative importance of energy
+            force_weight: relative importance of force
+            stress_weight: relative importance of stress
+            data_mean: average of training data
+            data_std: standard deviation of training data
+            calc_stress: whether stress calculation is required
+            loss: loss function used for training
+            optimizer: optimizer for training
+            scheduler: scheduler for training
+            lr: learning rate for training
+            decay_steps: number of steps for decaying learning rate
+            decay_alpha: parameter determines the minimum learning rate.
         """
         super().__init__()
 
         self.model = Potential(model=model, element_refs=element_refs, calc_stresses=calc_stress)
 
         self.mae = torchmetrics.MeanAbsoluteError()
         self.rmse = torchmetrics.MeanSquaredError(squared=False)
@@ -328,24 +343,26 @@
             labels: Labels.
             preds: Predictions
             energy_weight: Weight for energy loss.
             force_weight: Weight for force loss.
             stress_weight: Weight for stress loss.
             num_atoms: Number of atoms.
 
-        Returns:
+        Returns::
+
             {
                 "Total_Loss": total_loss,
                 "Energy_MAE": e_mae,
                 "Force_MAE": f_mae,
                 "Stress_MAE": s_mae,
                 "Energy_RMSE": e_rmse,
                 "Force_RMSE": f_rmse,
                 "Stress_RMSE": s_rmse,
             }
+
         """
         e_target, f_target, s_target = labels
         pred_e, pred_f, pred_s = preds
 
         e_loss = self.loss(e_target / num_atoms, pred_e / num_atoms)
         f_loss = self.loss(f_target, pred_f)
```

### Comparing `matgl-0.5.5/matgl.egg-info/PKG-INFO` & `matgl-0.5.6/matgl.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.5.5
+Version: 0.5.6
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong
 Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -22,14 +22,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
 [![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing%20-%20main/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
+[![Coverage Status](https://coveralls.io/repos/github/materialsvirtuallab/matgl/badge.svg?branch=main)](https://coveralls.io/github/materialsvirtuallab/matgl?branch=main)
 
 <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MatGL.png?raw=true" alt="matgl" width="30%" style="float: right">
 
 # Materials Graph Library
 
 Official Documentation: [link][doc]
 
@@ -61,33 +62,34 @@
 - v0.1.0 (Feb 16 2023): Initial implementations of M3GNet and MEGNet architectures have been completed. Expect
   bugs!
 
 ## Architectures
 
 <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic" width="50%">
 
-## MEGNet
+### MEGNet
 
-The [MatErials Graph Network (MEGNet)][megnet] is an implementation of DeepMind's [graph networks][graphnetwork] for
+[MatErials Graph Network (MEGNet)][megnet] is an implementation of DeepMind's [graph networks][graphnetwork] for
 machine learning in materials science. We have demonstrated its success in achieving low prediction errors in a broad
 array of properties in both [molecules and crystals][megnet]. New releases have included our recent work on
 [multi-fidelity materials property modeling][mfimegnet]. Figure 1 shows the sequential update steps of the graph
 network, whereby bonds, atoms, and global state attributes are updated using information from each other, generating an output graph.
 
-## M3GNet
+### M3GNet
 
-[M3GNet][m3gnet] is a new materials graph neural network architecture that incorporates 3-body interactions in MEGNet. An additional difference is the addition of the coordinates for atoms and
+[Materials 3-body Graph Network (M3GNet)][m3gnet] is a new materials graph neural network architecture that
+incorporates 3-body interactions in MEGNet. An additional difference is the addition of the coordinates for atoms and
 the 3×3 lattice matrix in crystals, which are necessary for obtaining tensorial quantities such as forces and
 stresses via auto-differentiation. As a framework, M3GNet has diverse applications, including:
 
 - **Interatomic potential development.** With the same training data, M3GNet performs similarly to state-of-the-art
   machine learning interatomic potentials (MLIPs). However, a key feature of a graph representation is its
   flexibility to scale to diverse chemical spaces. One of the key accomplishments of M3GNet is the development of a
-  *universal IP* that can work across the entire periodic table of the elements by training on relaxations performed
-  in the [Materials Project][mp].
+  [*universal IP*][m3gnet] that can work across the entire periodic table of the elements by training on relaxations
+  performed in the [Materials Project][mp].
 - **Surrogate models for property predictions.** Like the previous MEGNet architecture, M3GNet can be used to develop
   surrogate models for property predictions, achieving in many cases accuracies that are better or similar to other
   state-of-the-art ML models.
 
 For detailed performance benchmarks, please refer to the publications in the [References](#references) section.
 
 ## Installation
@@ -131,16 +133,16 @@
 ```
 
 ## Resources
 
 - [Jupyter notebooks][jupyternb] on the use of MatGL. These notebooks can be run on [Google Colab][colab]. This will
   be the primary form of tutorials for now.
 - [API documentation][apidocs] for all classes and methods.
-- [Developer's Guide](developer.md) has been written to outline the key design elements of matgl. This serves
-as a guiding documentation for developers wishing to train and contribute matgl models.
+- [Developer Guide](developer.md) outlines the key design elements of matgl, especially for developers wishing to
+  train and contribute matgl models.
 
 ## References
 
 A MatGL publication is currently being written. For now, pls refer to the CITATION.cff file for the citation
 information. If you are using any of the pretrained models, please cite the relevant works below:
 
 > **MEGNet**
@@ -156,37 +158,55 @@
 > **M3GNet**
 >
 > Chen, C., Ong, S.P. _A universal graph deep learning interatomic potential for the periodic table._ Nature
 > Computational Science, 2023, 2, 718–728. DOI: [10.1038/s43588-022-00349-3][m3gnet].
 
 ## FAQs
 
-1. The `M3GNet-MP-2021.2.8-PES` differs from the original tensorflow (TF) implementation!
+1. **The `M3GNet-MP-2021.2.8-PES` differs from the original tensorflow (TF) implementation!**
 
    Answer: `M3GNet-MP-2021.2.8-PES` is a refitted model with some data improvements and minor architectural changes.
    Porting over the weights from the TF version to DGL/PyTorch is non-trivial. We have performed reasonable benchmarking
    to ensure that the new implementation reproduces the broad error characteristics of the original TF implementation
    (see [examples][jupyternb]). However, it is not expected to reproduce the TF version exactly. This refitted model
    serves as a baseline for future model improvements. We do not believe there is value in expending the resources
    to reproduce the TF version exactly.
 
-2. I am getting errors with `matgl.load_model()`!
+2. **I am getting errors with `matgl.load_model()`!**
 
    Answer: The most likely reason is that you have a cached older version of the model. We often refactor models to
    ensure the best implementation. This can usually be solved by updating your matgl to the latest version
    and clearing your cache using:
 
    ```bash
    pip install matgl --upgrade
    python -c "import matgl; matgl.clear_cache()"
    ```
 
    On the next run, the latest model will be downloaded. With effect from v0.5.2, we have implemented a model
    versioning scheme that will detect code vs model version conflicts and alert the user of such problems.
 
+3. **What pre-trained models should I be using?**
+
+   Answer: There is no one definitive answer. In general, the newer the architecture and dataset, the more likely
+   the model performs better. However, it should also be noted that a model operating on a more diverse dataset may
+   compromise on  performance on a specific system. The best way is to look at the READMEs included with each model
+   and do some tests on the systems you are interested in.
+
+4. **How do I contribute to matgl?**
+
+   Answer: For code contributions, please fork and submit pull requests. You should read the [developer guide]
+   (developer) to understand the general design guidelines.
+
+   We welcome pre-trained model contributions as well, which should also be submitted via PRs. Please follow the
+   folder structure of the pretrained models. In particular, we expect all models to come with a README and notebook
+   documenting its use and its key performance metrics. Also, we expect contributions to be on new properties
+   or systems or to significantly outperform the existing models. We will develop an alternative means for model
+   sharing in the future.
+
 ## Acknowledgments
 
 This work was primarily supported by the [Materials Project][mp], funded by the U.S. Department of Energy, Office of
 Science, Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
 DE-AC02-05-CH11231: Materials Project program KC23MP. This work used the Expanse supercomputing cluster at the Extreme
 Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number
 ACI-1548562.
```

### Comparing `matgl-0.5.5/matgl.egg-info/SOURCES.txt` & `matgl-0.5.6/matgl.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 matgl/graph/__init__.py
 matgl/graph/compute.py
 matgl/graph/converters.py
 matgl/graph/data.py
 matgl/layers/__init__.py
 matgl/layers/_activations.py
 matgl/layers/_atom_ref.py
+matgl/layers/_basis.py
 matgl/layers/_bond.py
 matgl/layers/_core.py
 matgl/layers/_embedding.py
 matgl/layers/_graph_convolution.py
 matgl/layers/_readout.py
 matgl/layers/_three_body.py
 matgl/models/__init__.py
@@ -34,8 +35,9 @@
 matgl/models/_megnet.py
 matgl/models/_wrappers.py
 matgl/utils/__init__.py
 matgl/utils/cutoff.py
 matgl/utils/io.py
 matgl/utils/maths.py
 matgl/utils/sb_roots.npy
-matgl/utils/training.py
+matgl/utils/training.py
+tests/test_config.py
```

### Comparing `matgl-0.5.5/pyproject.toml` & `matgl-0.5.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -71,15 +71,19 @@
 ]
 pydocstyle.convention = "google"
 isort.required-imports = ["from __future__ import annotations"]
 extend-exclude = ["tests"]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
+"setup.py" = ["D"]
 "tasks.py" = ["D"]
+"tests/**/*" = ["D"]
+"docs/**/*" = ["D"]
+"examples/**/*" = ["D"]
 
 [tool.pytest.ini_options]
 addopts = "--durations=30 --quiet -rXs --color=yes -p no:warnings"
 
 [tool.mypy]
 ignore_missing_imports = true
 explicit_package_bases = true
```

### Comparing `matgl-0.5.5/setup.py` & `matgl-0.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 this_dir = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(this_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="matgl",
-    version="0.5.5",
+    version="0.5.6",
     author="Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong",
     author_email="t1ko@ucsd.edu, ongsp@ucsd.edu",
     maintainer="Shyue Ping Ong",
     maintainer_email="ongsp@ucsd.edu",
     description="MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

