# Comparing `tmp/pynuml-23.5.2.tar.gz` & `tmp/pynuml-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynuml-23.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pynuml-23.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pynuml-23.5.2.tar` & `pynuml-23.6.0.tar`

### file list

```diff
@@ -1,31 +1,34 @@
--rw-r--r--   0        0        0       17 2022-08-22 18:40:35.802435 pynuml-23.5.2/.gitignore
--rw-r--r--   0        0        0     1074 2023-05-22 19:32:38.886857 pynuml-23.5.2/LICENSE
--rw-r--r--   0        0        0     5647 2023-05-22 19:32:38.886857 pynuml-23.5.2/README.md
--rw-r--r--   0        0        0      170 2022-08-22 18:40:35.802435 pynuml-23.5.2/doc/README.md
--rw-r--r--   0        0        0     9267 2022-08-22 18:40:35.802435 pynuml-23.5.2/doc/graph_create.md
--rw-r--r--   0        0        0     2903 2022-08-22 18:40:35.802435 pynuml-23.5.2/doc/python_env.md
--rw-r--r--   0        0        0      638 2023-05-22 19:32:38.886857 pynuml-23.5.2/docs/Makefile
--rw-r--r--   0        0        0      804 2023-05-22 19:32:38.886857 pynuml-23.5.2/docs/make.bat
--rw-r--r--   0        0        0      916 2023-05-22 19:32:38.886857 pynuml-23.5.2/docs/source/conf.py
--rw-r--r--   0        0        0      671 2023-05-22 19:32:38.886857 pynuml-23.5.2/docs/source/index.rst
--rw-r--r--   0        0        0      581 2022-08-22 15:18:00.634737 pynuml-23.5.2/example/plot.py
--rwxr-xr-x   0        0        0     2089 2022-11-15 22:26:27.438225 pynuml-23.5.2/example/process.py
--rw-r--r--   0        0        0     1169 2022-08-22 18:40:35.802435 pynuml-23.5.2/h5merge.py
--rw-r--r--   0        0        0       38 2022-11-15 18:40:24.677584 pynuml-23.5.2/pynuml/.gitignore
--rw-r--r--   0        0        0      164 2023-05-23 15:12:32.529985 pynuml-23.5.2/pynuml/__init__.py
--rw-r--r--   0        0        0       97 2023-05-19 18:59:36.039498 pynuml-23.5.2/pynuml/io/__init__.py
--rw-r--r--   0        0        0    33647 2023-05-23 15:09:52.742521 pynuml-23.5.2/pynuml/io/file.py
--rw-r--r--   0        0        0     3290 2023-05-22 19:32:38.886857 pynuml-23.5.2/pynuml/io/h5interface.py
--rw-r--r--   0        0        0     4089 2023-05-23 15:09:52.742521 pynuml-23.5.2/pynuml/io/out.py
--rw-r--r--   0        0        0       69 2023-05-22 19:32:38.890858 pynuml-23.5.2/pynuml/labels/__init__.py
--rw-r--r--   0        0        0     1476 2022-11-15 18:40:24.677584 pynuml-23.5.2/pynuml/labels/ccqe.py
--rw-r--r--   0        0        0      779 2023-05-22 19:32:38.890858 pynuml-23.5.2/pynuml/labels/simple.py
--rw-r--r--   0        0        0    10392 2023-05-22 19:52:38.317160 pynuml-23.5.2/pynuml/labels/standard.py
--rw-r--r--   0        0        0       28 2023-05-22 19:32:38.890858 pynuml-23.5.2/pynuml/plot/__init__.py
--rw-r--r--   0        0        0     5246 2023-05-22 19:32:38.890858 pynuml-23.5.2/pynuml/plot/graph.py
--rw-r--r--   0        0        0       39 2023-02-28 00:57:35.995625 pynuml-23.5.2/pynuml/process/__init__.py
--rw-r--r--   0        0        0      463 2023-02-28 00:57:35.995625 pynuml-23.5.2/pynuml/process/base.py
--rw-r--r--   0        0        0     6105 2023-05-23 15:09:52.742521 pynuml-23.5.2/pynuml/process/hitgraph.py
--rw-r--r--   0        0        0     3780 2022-11-15 18:40:24.677584 pynuml-23.5.2/pynuml/process/spmap.py
--rw-r--r--   0        0        0      585 2023-05-22 19:32:38.890858 pynuml-23.5.2/pyproject.toml
--rw-r--r--   0        0        0     6181 1970-01-01 00:00:00.000000 pynuml-23.5.2/PKG-INFO
+-rw-r--r--   0        0        0       17 2022-08-22 18:47:46.562567 pynuml-23.6.0/.gitignore
+-rw-r--r--   0        0        0      824 2023-06-15 20:05:13.774670 pynuml-23.6.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1074 2023-05-23 17:23:11.333385 pynuml-23.6.0/LICENSE
+-rw-r--r--   0        0        0     5647 2023-05-11 17:09:33.660248 pynuml-23.6.0/README.md
+-rw-r--r--   0        0        0      170 2022-08-22 18:47:46.563031 pynuml-23.6.0/doc/README.md
+-rw-r--r--   0        0        0     9267 2022-08-22 18:47:46.563254 pynuml-23.6.0/doc/graph_create.md
+-rw-r--r--   0        0        0     2903 2022-08-22 18:47:46.563416 pynuml-23.6.0/doc/python_env.md
+-rw-r--r--   0        0        0      638 2023-05-23 17:23:11.333546 pynuml-23.6.0/docs/Makefile
+-rw-r--r--   0        0        0      923 2023-06-15 20:05:13.774909 pynuml-23.6.0/docs/conf.py
+-rw-r--r--   0        0        0      673 2023-06-15 20:05:13.775100 pynuml-23.6.0/docs/index.rst
+-rw-r--r--   0        0        0     1413 2023-06-15 20:05:13.775357 pynuml-23.6.0/docs/install/installation.rst
+-rw-r--r--   0        0        0      804 2023-05-23 17:23:11.333683 pynuml-23.6.0/docs/make.bat
+-rw-r--r--   0        0        0      581 2022-08-22 18:47:46.563608 pynuml-23.6.0/example/plot.py
+-rwxr-xr-x   0        0        0     2089 2022-11-30 18:31:20.903706 pynuml-23.6.0/example/process.py
+-rw-r--r--   0        0        0     1169 2022-08-22 18:47:46.563858 pynuml-23.6.0/h5merge.py
+-rw-r--r--   0        0        0       38 2022-10-01 15:34:05.362452 pynuml-23.6.0/pynuml/.gitignore
+-rw-r--r--   0        0        0      164 2023-06-15 20:05:13.776439 pynuml-23.6.0/pynuml/__init__.py
+-rw-r--r--   0        0        0       97 2023-02-27 22:44:16.230810 pynuml-23.6.0/pynuml/io/__init__.py
+-rw-r--r--   0        0        0    33647 2023-05-23 17:23:11.334552 pynuml-23.6.0/pynuml/io/file.py
+-rw-r--r--   0        0        0     3290 2023-05-23 17:23:11.334785 pynuml-23.6.0/pynuml/io/h5interface.py
+-rw-r--r--   0        0        0     4089 2023-05-23 17:23:11.334967 pynuml-23.6.0/pynuml/io/out.py
+-rw-r--r--   0        0        0      102 2023-06-15 20:05:13.776689 pynuml-23.6.0/pynuml/labels/__init__.py
+-rw-r--r--   0        0        0     1476 2022-10-01 15:34:05.363366 pynuml-23.6.0/pynuml/labels/ccqe.py
+-rw-r--r--   0        0        0     1156 2023-06-15 20:05:13.776860 pynuml-23.6.0/pynuml/labels/flavor.py
+-rw-r--r--   0        0        0      779 2023-05-23 17:23:11.335229 pynuml-23.6.0/pynuml/labels/simple.py
+-rw-r--r--   0        0        0    10593 2023-06-15 15:41:12.568618 pynuml-23.6.0/pynuml/labels/standard.py
+-rw-r--r--   0        0        0       28 2023-05-23 17:23:11.335591 pynuml-23.6.0/pynuml/plot/__init__.py
+-rw-r--r--   0        0        0     5246 2023-05-23 17:23:11.335785 pynuml-23.6.0/pynuml/plot/graph.py
+-rw-r--r--   0        0        0       39 2023-02-27 22:44:16.231786 pynuml-23.6.0/pynuml/process/__init__.py
+-rw-r--r--   0        0        0      463 2023-02-27 22:44:16.231898 pynuml-23.6.0/pynuml/process/base.py
+-rw-r--r--   0        0        0     6682 2023-06-15 20:05:13.778385 pynuml-23.6.0/pynuml/process/hitgraph.py
+-rw-r--r--   0        0        0     3780 2022-10-01 15:34:05.363995 pynuml-23.6.0/pynuml/process/spmap.py
+-rw-r--r--   0        0        0      599 2023-06-15 15:15:22.011325 pynuml-23.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6203 1970-01-01 00:00:00.000000 pynuml-23.6.0/PKG-INFO
```

### Comparing `pynuml-23.5.2/LICENSE` & `pynuml-23.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.2/README.md` & `pynuml-23.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.2/doc/graph_create.md` & `pynuml-23.6.0/doc/graph_create.md`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.2/doc/python_env.md` & `pynuml-23.6.0/doc/python_env.md`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.2/docs/Makefile` & `pynuml-23.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.2/docs/make.bat` & `pynuml-23.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.2/docs/source/conf.py` & `pynuml-23.6.0/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 exclude_patterns = []
 
 
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
-html_theme = 'alabaster'
+html_theme = 'sphinx_rtd_theme'
 html_static_path = ['_static']
```

### Comparing `pynuml-23.5.2/docs/source/index.rst` & `pynuml-23.6.0/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 :github_url: https://github.com/vhewes/pynuml
 
 pynuml Documentation
 ====================
 
-**pynuml** is a python package providing a data interface for machine learning in neutrino physics. It utilises the :NuML: HDF5 event file format to efficiently preprocess physics events into ML objects for training neural networks. It is designed to abstract away many aspects of a typical ML workflow:
+**pynuml** is a python package providing a data interface for machine learning in neutrino physics. It utilises the **NuML** HDF5 event file format to efficiently preprocess physics events into ML objects for training neural networks. It is designed to abstract away many aspects of a typical ML workflow:
+
 - Efficiently iterate over large HDF5 datasets
 - Generate semantic and instance labels for particles
 - Preprocess events into ML objects
 
 .. toctree::
    :maxdepth: 1
    :caption: Installation
 
    install/installation
 
 .. toctree::
    :maxdepth: 1
-   :caption: Getting Started
+   :caption: Getting Started
```

### Comparing `pynuml-23.5.2/example/plot.py` & `pynuml-23.6.0/example/plot.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.2/example/process.py` & `pynuml-23.6.0/example/process.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.2/h5merge.py` & `pynuml-23.6.0/h5merge.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.2/pynuml/io/file.py` & `pynuml-23.6.0/pynuml/io/file.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.2/pynuml/io/h5interface.py` & `pynuml-23.6.0/pynuml/io/h5interface.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.2/pynuml/io/out.py` & `pynuml-23.6.0/pynuml/io/out.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.2/pynuml/labels/ccqe.py` & `pynuml-23.6.0/pynuml/labels/ccqe.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.2/pynuml/labels/simple.py` & `pynuml-23.6.0/pynuml/labels/simple.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.2/pynuml/labels/standard.py` & `pynuml-23.6.0/pynuml/labels/standard.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,25 +107,24 @@
                     if part.start_process == 'primary':
                         sl = self.shower
                         slc = self.shower
                     elif abs(parent_type) == 13 and (part.start_process == 'muMinusCaptureAtRest' \
                         or part.start_process == 'muPlusCaptureAtRest' or part.start_process == 'Decay'):
                         sl = self.michel
                         slc = self.michel
-
                     elif part.start_process == 'conv' or part.end_process == 'conv' \
                         or part.start_process == 'compt' or part.end_process == 'compt':
                         if part.momentum >= self._gamma_threshold:
                             sl = self.shower
                             slc = self.shower
                         else:
                             sl = self.diffuse
                             slc = self.diffuse
                     elif part.start_process == 'eBrem' or part.end_process == 'phot' \
-                        or part.end_process == 'photonNuclear':
+                        or part.end_process == 'photonNuclear' or part.end_process == 'eIoni':
                         sl = self.diffuse
                         slc = None
                     elif part.start_process == 'muIoni' or part.start_process == 'hIoni' \
                         or part.start_process == 'eIoni':
                         if part.momentum <= 0.01:
                             if part.start_process == 'muIoni':
                                 sl = self.muon
@@ -171,20 +170,24 @@
                     return sl, slc
 
                 def unlabeled_particle(part, parent_type):
                     raise Exception(f"particle not recognised! PDG code {part.type}, parent PDG code {parent_type}, start process {part.start_process}, end process {part.end_process}")
 
                 particle_processor = {
                     211: pion_labeler,
+                    221: pion_labeler,
+                    331: pion_labeler,
+                    223: pion_labeler,
                     13: muon_labeler,
                     321: kaon_labeler,
                     111: neutral_pions_kaons_labeler,
                     311: neutral_pions_kaons_labeler,
                     310: neutral_pions_kaons_labeler,
                     130: neutral_pions_kaons_labeler,
+                    113: neutral_pions_kaons_labeler,
                     11: electron_positron_labeler,
                     22: gamma_labeler
                 }
 
                 if particle.pdgid.charge(part.type) == 0 and part.end_process == 'CoupledTransportation':
                     # neutral particle left the volume boundary
                     sl = self.invisible
```

### Comparing `pynuml-23.5.2/pynuml/plot/graph.py` & `pynuml-23.6.0/pynuml/plot/graph.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.2/pynuml/process/hitgraph.py` & `pynuml-23.6.0/pynuml/process/hitgraph.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,73 +1,77 @@
-import sys
 from typing import Any, Callable
 import numpy as np
 import pandas as pd
-from mpi4py import MPI
 
 import torch
 import torch_geometric as pyg
 
 from .base import ProcessorBase
 
 class HitGraphProducer(ProcessorBase):
     '''Process event into graphs'''
 
     def __init__(self,
                  file: 'pynuml.io.File',
-                 labeller: Callable = None,
+                 semantic_labeller: Callable = None,
+                 event_labeller: Callable = None,
                  planes: list[str] = ['u','v','y'],
                  node_pos: list[str] = ['local_wire','local_time'],
                  pos_norm: list[float] = [0.3,0.055],
                  node_feats: list[str] = ['integral','rms'],
                  lower_bound: int = 20,
                  filter_hits: bool = False):
 
-        self.labeller = labeller
+        self.semantic_labeller = semantic_labeller
+        self.event_labeller = event_labeller
         self.planes = planes
         self.node_pos = node_pos
         self.pos_norm = torch.tensor(pos_norm).float()
         self.node_feats = node_feats
         self.lower_bound = lower_bound
         self.filter_hits = filter_hits
 
         self.transform = pyg.transforms.Compose((
             pyg.transforms.Delaunay(),
             pyg.transforms.FaceToEdge()))
 
-        super(HitGraphProducer, self).__init__(file)
+        super().__init__(file)
 
     @property
     def columns(self) -> dict[str, list[str]]:
         groups = {
             'hit_table': ['hit_id','local_plane','local_time','local_wire','integral','rms'],
             'spacepoint_table': ['spacepoint_id','hit_id']
         }
-        if self.labeller:
+        if self.semantic_labeller:
             groups['particle_table'] = ['g4_id','parent_id','type','momentum','start_process','end_process']
             groups['edep_table'] = []
+        if self.event_labeller:
+            groups['event_table'] = ['is_cc', 'nu_pdg']
         return groups
 
     @property
     def metadata(self):
         metadata = { 'planes': self.planes }
-        if self.labeller is not None:
-            metadata['classes'] = self.labeller.labels[:-1]
+        if self.semantic_labeller is not None:
+            metadata['semantic_classes'] = self.semantic_labeller.labels[:-1]
+        if self.event_labeller is not None:
+            metadata['event_classes'] = self.event_labeller.labels
         return metadata
 
     def __call__(self, evt: 'pynuml.io.Event') -> tuple[str, Any]:
 
         event_id = evt.event_id
         name = f'r{event_id[0]}_sr{event_id[1]}_evt{event_id[2]}'
 
         hits = evt['hit_table']
         spacepoints = evt['spacepoint_table'].reset_index(drop=True)
 
         # handle energy depositions
-        if self.filter_hits or self.labeller:
+        if self.filter_hits or self.semantic_labeller:
             edeps = evt['edep_table']
             energy_col = 'energy' if 'energy' in edeps.columns else 'energy_fraction' # for backwards compatibility
             edeps = edeps.sort_values(by=[energy_col],
                                       ascending=False,
                                       kind='mergesort').drop_duplicates('hit_id')
             hits = edeps.merge(hits, on='hit_id', how='right')
 
@@ -88,37 +92,44 @@
         spacepoints = spacepoints.reset_index(names='index_3d')
 
         # skip events with fewer than lower_bnd simulated hits in any plane.
         # note that we can't just do a pandas groupby here, because that will
         # skip over any planes with zero hits
         for i in range(len(self.planes)):
             planehits = hits[hits.local_plane==i]
-            nhits = planehits.filter_label.sum() if self.labeller else planehits.shape[0]
+            nhits = planehits.filter_label.sum() if self.semantic_labeller else planehits.shape[0]
             if nhits < self.lower_bound:
                 return evt.name, None
 
         # get labels for each particle
-        if self.labeller:
-            particles = self.labeller(evt['particle_table'])
-            hits = hits.merge(particles, on='g4_id', how='left')
+        if self.semantic_labeller:
+            particles = self.semantic_labeller(evt['particle_table'])
+            try:
+                hits = hits.merge(particles, on='g4_id', how='left')
+            except:
+                print('exception occurred when merging hits and particles')
+                print('hit table:', hits)
+                print('particle table:', particles)
+                print('skipping this event')
+                return evt.name, None
             mask = (~hits.g4_id.isnull()) & (hits.semantic_label.isnull())
             if mask.any():
                 print(f'found {mask.sum()} orphaned hits.')
                 return evt.name, None
             del mask
 
         data = pyg.data.HeteroData()
 
         # event metadata
         data['metadata'].run = event_id[0]
         data['metadata'].subrun = event_id[1]
         data['metadata'].event = event_id[2]
 
         # spacepoint nodes
-        data['sp'].x = torch.empty(spacepoints.shape[0], 0)
+        data['sp'].num_nodes = spacepoints.shape[0]
 
         # draw graph edges
         for i, plane_hits in hits.groupby('local_plane'):
 
             p = self.planes[i]
             plane_hits = plane_hits.reset_index(drop=True).reset_index(names='index_2d')
 
@@ -142,15 +153,14 @@
                                        on=f'hit_id_{p}',
                                        how='inner')
             edge3d = edge3d[[f'index_2d_{p}','index_3d']].values.transpose()
             edge3d = torch.tensor(edge3d) if edge3d.size else torch.empty((2,0))
             data[p, 'nexus', 'sp'].edge_index = edge3d.long()
 
             # truth information
-            if self.labeller:
-                data[p].y_f = torch.tensor(plane_hits['filter_label'].values).bool()
-                filtered = plane_hits[plane_hits['filter_label']]
-                data[p].y_s = torch.tensor(filtered['semantic_label'].values).long()
-                self.labeller.validate(data[p].y_s)
-                data[p].y_i = torch.tensor(filtered['instance_label'].values).long()
+            if self.semantic_labeller:
+                data[p].y_semantic = torch.tensor(plane_hits['semantic_label'].fillna(-1).values).long()
+                data[p].y_instance = torch.tensor(plane_hits['instance_label'].fillna(-1).values).long()
+            if self.event_labeller:
+                data['evt'].y = self.event_labeller(evt['event_table'])
 
         return evt.name, data
```

### Comparing `pynuml-23.5.2/pynuml/process/spmap.py` & `pynuml-23.6.0/pynuml/process/spmap.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.2/pyproject.toml` & `pynuml-23.6.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
     "h5py>=3.7.0",
     "mpi4py",
     "pandas",
     "particle",
+    "plotly",
     "torch>=1.12.1",
     "torch-geometric>=2.1.0",
 ]
 dynamic = ["version", "description"]
 
 [project.urls]
 Home = "https://github.com/vhewes/pynuml"
```

### Comparing `pynuml-23.5.2/PKG-INFO` & `pynuml-23.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pynuml
-Version: 23.5.2
+Version: 23.6.0
 Summary: Standardised ML input processing for particle physics
 Author-email: v hewes <vhewes@fnal.gov>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: h5py>=3.7.0
 Requires-Dist: mpi4py
 Requires-Dist: pandas
 Requires-Dist: particle
+Requires-Dist: plotly
 Requires-Dist: torch>=1.12.1
 Requires-Dist: torch-geometric>=2.1.0
 Project-URL: Home, https://github.com/vhewes/pynuml
 
 # PyNuML: HDF5 IO and ML processing for neutrino physics
 
 PyNuML is a Python toolkit for processing machine learning (ML) inputs from neutrino physics simulation datasets. It offers efficient MPI parallel processing of datasets, including standardised solutions for generating semantic and instance labels from low-level particle simulation, and constructing PyTorch ML inputs such as pixel maps and graphs. The package uses a modular design to maximise flexibility and extensibility, allowing the user to write custom labelling and/or object formation code in place of the algorithms provided.
```

