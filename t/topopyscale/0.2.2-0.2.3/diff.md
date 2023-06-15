# Comparing `tmp/topopyscale-0.2.2.tar.gz` & `tmp/topopyscale-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topopyscale-0.2.2.tar", last modified: Sat May 13 17:28:09 2023, max compression
+gzip compressed data, was "dist/topopyscale-0.2.3.tar", last modified: Thu Jun 15 14:51:59 2023, max compression
```

## Comparing `topopyscale-0.2.2.tar` & `topopyscale-0.2.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 simonfi  (264780) simonfi  (231366)        0 2023-05-13 17:28:09.409811 topopyscale-0.2.2/
-drwxrwxr-x   0 simonfi  (264780) simonfi  (231366)        0 2023-05-13 17:28:09.401811 topopyscale-0.2.2/.github/
-drwxrwxr-x   0 simonfi  (264780) simonfi  (231366)        0 2023-05-13 17:28:09.405811 topopyscale-0.2.2/.github/workflows/
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)      737 2023-05-12 08:59:46.000000 topopyscale-0.2.2/.github/workflows/draft-pdf.yml
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     1082 2022-11-11 15:15:36.000000 topopyscale-0.2.2/.github/workflows/python-publish.yml
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     1435 2023-05-12 14:15:58.000000 topopyscale-0.2.2/.github/workflows/test_topopyscale.yml
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     1866 2021-11-05 08:58:50.000000 topopyscale-0.2.2/.gitignore
-drwxrwxr-x   0 simonfi  (264780) simonfi  (231366)        0 2023-05-13 17:28:09.405811 topopyscale-0.2.2/JOSS/
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)   110899 2022-12-14 14:07:56.000000 topopyscale-0.2.2/JOSS/figure2.png
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)    17303 2022-12-16 08:48:45.000000 topopyscale-0.2.2/JOSS/paper.bib
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     8357 2022-12-23 10:22:53.000000 topopyscale-0.2.2/JOSS/paper.md
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)  3156813 2022-12-14 14:07:56.000000 topopyscale-0.2.2/JOSS/temperature_comparison_crop_scaled.jpg
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     1101 2022-11-08 15:22:59.000000 topopyscale-0.2.2/LICENSE
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)       18 2021-08-25 13:16:00.000000 topopyscale-0.2.2/MANIFEST.in
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     8175 2023-05-13 17:28:09.409811 topopyscale-0.2.2/PKG-INFO
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     7077 2023-05-12 08:59:46.000000 topopyscale-0.2.2/README.md
-drwxrwxr-x   0 simonfi  (264780) simonfi  (231366)        0 2023-05-13 17:28:09.409811 topopyscale-0.2.2/TopoPyScale/
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)        0 2021-09-27 15:27:21.000000 topopyscale-0.2.2/TopoPyScale/__init__.py
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     6428 2022-03-16 13:31:57.000000 topopyscale-0.2.2/TopoPyScale/fetch_dem.py
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)    11239 2023-03-20 11:33:37.000000 topopyscale-0.2.2/TopoPyScale/fetch_era5.py
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     6256 2023-05-05 07:46:03.000000 topopyscale-0.2.2/TopoPyScale/meteo_util.py
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)      846 2022-02-17 15:07:15.000000 topopyscale-0.2.2/TopoPyScale/precip_orographic.py
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     3761 2023-05-11 09:47:51.000000 topopyscale-0.2.2/TopoPyScale/solar_geom.py
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     7786 2023-01-11 18:09:18.000000 topopyscale-0.2.2/TopoPyScale/topo_compare.py
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)    39212 2023-05-11 15:47:15.000000 topopyscale-0.2.2/TopoPyScale/topo_da.py
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)    28688 2023-05-11 15:52:16.000000 topopyscale-0.2.2/TopoPyScale/topo_export.py
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     8560 2023-01-11 11:16:20.000000 topopyscale-0.2.2/TopoPyScale/topo_obs.py
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     9814 2023-05-11 09:47:51.000000 topopyscale-0.2.2/TopoPyScale/topo_param.py
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     3733 2023-05-13 17:13:41.000000 topopyscale-0.2.2/TopoPyScale/topo_plot.py
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)    24323 2023-05-12 14:43:18.000000 topopyscale-0.2.2/TopoPyScale/topo_scale.py
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)    24569 2023-05-12 12:48:57.000000 topopyscale-0.2.2/TopoPyScale/topo_sim.py
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)    12429 2023-02-06 12:58:13.000000 topopyscale-0.2.2/TopoPyScale/topo_sub.py
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     6756 2023-05-11 16:13:13.000000 topopyscale-0.2.2/TopoPyScale/topo_utils.py
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)    35685 2023-05-13 15:51:40.000000 topopyscale-0.2.2/TopoPyScale/topoclass.py
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     6102 2023-05-11 15:58:03.000000 topopyscale-0.2.2/environment.yml
--rw-r--r--   0 simonfi  (264780) simonfi  (231366)    18619 2022-11-10 16:25:16.000000 topopyscale-0.2.2/logo.svg
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)      131 2023-05-13 17:28:09.409811 topopyscale-0.2.2/setup.cfg
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     2624 2023-05-13 17:17:38.000000 topopyscale-0.2.2/setup.py
-drwxrwxr-x   0 simonfi  (264780) simonfi  (231366)        0 2023-05-13 17:28:09.409811 topopyscale-0.2.2/topopyscale.egg-info/
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     8175 2023-05-13 17:28:09.000000 topopyscale-0.2.2/topopyscale.egg-info/PKG-INFO
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)      894 2023-05-13 17:28:09.000000 topopyscale-0.2.2/topopyscale.egg-info/SOURCES.txt
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)        1 2023-05-13 17:28:09.000000 topopyscale-0.2.2/topopyscale.egg-info/dependency_links.txt
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)      130 2023-05-13 17:28:09.000000 topopyscale-0.2.2/topopyscale.egg-info/requires.txt
--rw-rw-r--   0 simonfi  (264780) simonfi  (231366)       12 2023-05-13 17:28:09.000000 topopyscale-0.2.2/topopyscale.egg-info/top_level.txt
+drwxrwxr-x   0 simonfi  (264780) simonfi  (231366)        0 2023-06-15 14:51:59.854338 topopyscale-0.2.3/
+drwxrwxr-x   0 simonfi  (264780) simonfi  (231366)        0 2023-06-15 14:51:59.850338 topopyscale-0.2.3/.github/
+drwxrwxr-x   0 simonfi  (264780) simonfi  (231366)        0 2023-06-15 14:51:59.850338 topopyscale-0.2.3/.github/workflows/
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)      737 2023-05-12 08:59:46.000000 topopyscale-0.2.3/.github/workflows/draft-pdf.yml
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     1082 2022-11-11 15:15:36.000000 topopyscale-0.2.3/.github/workflows/python-publish.yml
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     1435 2023-05-12 14:15:58.000000 topopyscale-0.2.3/.github/workflows/test_topopyscale.yml
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     1866 2021-11-05 08:58:50.000000 topopyscale-0.2.3/.gitignore
+drwxrwxr-x   0 simonfi  (264780) simonfi  (231366)        0 2023-06-15 14:51:59.850338 topopyscale-0.2.3/JOSS/
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)   110899 2022-12-14 14:07:56.000000 topopyscale-0.2.3/JOSS/figure2.png
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)    17141 2023-05-22 08:04:14.000000 topopyscale-0.2.3/JOSS/paper.bib
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)    10181 2023-06-15 14:40:27.000000 topopyscale-0.2.3/JOSS/paper.md
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)  3156813 2022-12-14 14:07:56.000000 topopyscale-0.2.3/JOSS/temperature_comparison_crop_scaled.jpg
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     1101 2022-11-08 15:22:59.000000 topopyscale-0.2.3/LICENSE
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)       18 2021-08-25 13:16:00.000000 topopyscale-0.2.3/MANIFEST.in
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     8310 2023-06-15 14:51:59.854338 topopyscale-0.2.3/PKG-INFO
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     7219 2023-05-16 13:36:13.000000 topopyscale-0.2.3/README.md
+drwxrwxr-x   0 simonfi  (264780) simonfi  (231366)        0 2023-06-15 14:51:59.854338 topopyscale-0.2.3/TopoPyScale/
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)        0 2021-09-27 15:27:21.000000 topopyscale-0.2.3/TopoPyScale/__init__.py
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     6694 2023-06-02 12:48:14.000000 topopyscale-0.2.3/TopoPyScale/fetch_dem.py
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)    12413 2023-06-15 14:23:07.000000 topopyscale-0.2.3/TopoPyScale/fetch_era5.py
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     6256 2023-05-05 07:46:03.000000 topopyscale-0.2.3/TopoPyScale/meteo_util.py
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)      846 2022-02-17 15:07:15.000000 topopyscale-0.2.3/TopoPyScale/precip_orographic.py
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     3776 2023-05-24 08:51:16.000000 topopyscale-0.2.3/TopoPyScale/solar_geom.py
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     7786 2023-01-11 18:09:18.000000 topopyscale-0.2.3/TopoPyScale/topo_compare.py
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)    39342 2023-06-13 14:14:39.000000 topopyscale-0.2.3/TopoPyScale/topo_da.py
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)    30248 2023-06-14 10:40:12.000000 topopyscale-0.2.3/TopoPyScale/topo_export.py
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     8577 2023-06-02 12:46:20.000000 topopyscale-0.2.3/TopoPyScale/topo_obs.py
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     9801 2023-05-24 08:51:16.000000 topopyscale-0.2.3/TopoPyScale/topo_param.py
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     3733 2023-05-13 17:13:41.000000 topopyscale-0.2.3/TopoPyScale/topo_plot.py
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)    24391 2023-06-15 14:23:07.000000 topopyscale-0.2.3/TopoPyScale/topo_scale.py
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)    33375 2023-06-14 11:24:49.000000 topopyscale-0.2.3/TopoPyScale/topo_sim.py
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)    12429 2023-02-06 12:58:13.000000 topopyscale-0.2.3/TopoPyScale/topo_sub.py
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     8473 2023-06-14 09:20:32.000000 topopyscale-0.2.3/TopoPyScale/topo_utils.py
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)    37000 2023-06-15 14:23:07.000000 topopyscale-0.2.3/TopoPyScale/topoclass.py
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)      796 2023-06-15 14:46:44.000000 topopyscale-0.2.3/environment.yml
+-rw-r--r--   0 simonfi  (264780) simonfi  (231366)    18619 2022-11-10 16:25:16.000000 topopyscale-0.2.3/logo.svg
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)      131 2023-06-15 14:51:59.858337 topopyscale-0.2.3/setup.cfg
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     2617 2023-06-15 14:28:07.000000 topopyscale-0.2.3/setup.py
+drwxrwxr-x   0 simonfi  (264780) simonfi  (231366)        0 2023-06-15 14:51:59.854338 topopyscale-0.2.3/topopyscale.egg-info/
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)     8310 2023-06-15 14:51:59.000000 topopyscale-0.2.3/topopyscale.egg-info/PKG-INFO
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)      894 2023-06-15 14:51:59.000000 topopyscale-0.2.3/topopyscale.egg-info/SOURCES.txt
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)        1 2023-06-15 14:51:59.000000 topopyscale-0.2.3/topopyscale.egg-info/dependency_links.txt
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)      130 2023-06-15 14:51:59.000000 topopyscale-0.2.3/topopyscale.egg-info/requires.txt
+-rw-rw-r--   0 simonfi  (264780) simonfi  (231366)       12 2023-06-15 14:51:59.000000 topopyscale-0.2.3/topopyscale.egg-info/top_level.txt
```

### Comparing `topopyscale-0.2.2/.github/workflows/draft-pdf.yml` & `topopyscale-0.2.3/.github/workflows/draft-pdf.yml`

 * *Files identical despite different names*

### Comparing `topopyscale-0.2.2/.github/workflows/python-publish.yml` & `topopyscale-0.2.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `topopyscale-0.2.2/.github/workflows/test_topopyscale.yml` & `topopyscale-0.2.3/.github/workflows/test_topopyscale.yml`

 * *Files identical despite different names*

### Comparing `topopyscale-0.2.2/.gitignore` & `topopyscale-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `topopyscale-0.2.2/JOSS/figure2.png` & `topopyscale-0.2.3/JOSS/figure2.png`

 * *Files identical despite different names*

### Comparing `topopyscale-0.2.2/JOSS/paper.bib` & `topopyscale-0.2.3/JOSS/paper.bib`

 * *Files 3% similar despite different names*

```diff
@@ -51,29 +51,27 @@
 VOLUME = {2022},
 YEAR = {2022},
 PAGES = {1--28},
 URL = {https://esurf.copernicus.org/preprints/esurf-2022-39/},
 DOI = {10.5194/esurf-2022-39}
 }
 
-@article{alonso-gonzalezMuSAMultiscaleSnow2022,
-  title = {{{MuSA}}: {{The Multiscale Snow Data Assimilation System}} (v1.0)},
-  shorttitle = {{{MuSA}}},
-  author = {{Alonso-Gonz{\'a}lez}, Esteban and Aalstad, Kristoffer and Baba, Mohamed Wassim and Revuelto, Jes{\'u}s and {L{\'o}pez-Moreno}, Juan Ignacio and Fiddes, Joel and Essery, Richard and Gascoin, Simon},
-  year = {2022},
-  month = aug,
-  journal = {Geoscientific Model Development Discussions},
-  pages = {1--43},
-  publisher = {{Copernicus GmbH}},
-  issn = {1991-959X},
-  doi = {10.5194/gmd-2022-137},
-  langid = {english},
-  keywords = {assimilation,fsm,musa,snow},
+@Article{gmd-15-9127-2022,
+AUTHOR = {Alonso-Gonz\'alez, E. and Aalstad, K. and Baba, M. W. and Revuelto, J. and L\'opez-Moreno, J. I. and Fiddes, J. and Essery, R. and Gascoin, S.},
+TITLE = {The Multiple Snow Data Assimilation System (MuSA v1.0)},
+JOURNAL = {Geoscientific Model Development},
+VOLUME = {15},
+YEAR = {2022},
+NUMBER = {24},
+PAGES = {9127--9155},
+URL = {https://gmd.copernicus.org/articles/15/9127/2022/},
+DOI = {10.5194/gmd-15-9127-2022}
 }
 
+
 @Article{gmd-8-3867-2015,
 AUTHOR = {Essery, R.},
 TITLE = {A factorial snowpack model (FSM 1.0)},
 JOURNAL = {Geoscientific Model Development},
 VOLUME = {8},
 YEAR = {2015},
 NUMBER = {12},
@@ -324,23 +322,26 @@
   year = {2021},
   month = sep,
   journal = {Journal of Hydrometeorology},
   issn = {1525-755X, 1525-7541},
   doi = {10.1175/JHM-D-21-0070.1},
   langid = {english},
 }
-@Article{gmd-2022-127,
+
+
+@Article{gmd-16-2607-2023,
 AUTHOR = {Westermann, S. and Ingeman-Nielsen, T. and Scheer, J. and Aalstad, K. and Aga, J. and Chaudhary, N. and Etzelm\"uller, B. and Filhol, S. and K\"a\"ab, A. and Renette, C. and Schmidt, L. S. and Schuler, T. V. and Zweigel, R. B. and Martin, L. and Morard, S. and Ben-Asher, M. and Angelopoulos, M. and Boike, J. and Groenke, B. and Miesner, F. and Nitzbon, J. and Overduin, P. and Stuenzi, S. M. and Langer, M.},
 TITLE = {The CryoGrid community model (version 1.0) -- a multi-physics toolbox for climate-driven simulations in the terrestrial cryosphere},
-JOURNAL = {Geoscientific Model Development Discussions},
-VOLUME = {2022},
-YEAR = {2022},
-PAGES = {1--61},
-URL = {https://gmd.copernicus.org/preprints/gmd-2022-127/},
-DOI = {10.5194/gmd-2022-127}
+JOURNAL = {Geoscientific Model Development},
+VOLUME = {16},
+YEAR = {2023},
+NUMBER = {9},
+PAGES = {2607--2647},
+URL = {https://gmd.copernicus.org/articles/16/2607/2023/},
+DOI = {10.5194/gmd-16-2607-2023}
 }
 
 @Article{hess-2022-241,
 AUTHOR = {Martin, L. C. P. and Westermann, S. and Magni, M. and Brun, F. and Fiddes, J. and Lei, Y. and Kraaijenbrink, P. and Mathys, T. and Langer, M. and Allen, S. and Immerzeel, W. W.},
 TITLE = {Recent ground thermo-hydrological changes in a Tibetan endorheic catchment and implications for lake level changes},
 JOURNAL = {Hydrology and Earth System Sciences Discussions},
 VOLUME = {2022},
```

### Comparing `topopyscale-0.2.2/JOSS/temperature_comparison_crop_scaled.jpg` & `topopyscale-0.2.3/JOSS/temperature_comparison_crop_scaled.jpg`

 * *Files identical despite different names*

### Comparing `topopyscale-0.2.2/LICENSE` & `topopyscale-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `topopyscale-0.2.2/PKG-INFO` & `topopyscale-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: topopyscale
-Version: 0.2.2
-Summary: A Python package to perform climate downscaling at the hillslope scale
+Version: 0.2.3
+Summary: TopoPyScale: A Python Package for Hillslope Climate Downscaling
 Home-page: https://github.com/ArcticSnow/TopoPyScale
 Download-URL: https://github.com/ArcticSnow/TopoPyScale/releases/latest
 Author: ['Simon Filhol', 'Joel Fiddes', 'Kristoffer Aalstad']
 Author-email: simon.filhol@geo.uio.no
 License: MIT
 Project-URL: Documentation, https://topopyscale.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ArcticSnow/TopoPyScale
@@ -27,14 +27,16 @@
 [![DOI](https://zenodo.org/badge/411249045.svg)](https://zenodo.org/badge/latestdoi/411249045)
 [![GitHub license](https://img.shields.io/github/license/ArcticSnow/TopoPyScale)](https://github.com/ArcticSnow/TopoPyScale/blob/main/LICENSE)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/ArcticSnow/TopoPyScale)
 <a href="https://joss.theoj.org/papers/91621581b2d0c097495fdd1e58179e87"><img src="https://joss.theoj.org/papers/91621581b2d0c097495fdd1e58179e87/status.svg"></a>
 [![][docs-dev-img]][docs-dev-url]
 ![Test](https://github.com/ArcticSnow/TopoPyScale/actions/workflows/test_topopyscale.yml/badge.svg)
 
+Binder Notebooks Examples: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ArcticSnow/TopoPyScale_examples/HEAD)
+
 [docs-dev-img]: https://img.shields.io/badge/docs-latest-blue.svg
 [docs-dev-url]: https://topopyscale.readthedocs.io
 
 # TopoPyScale
 Python version of Toposcale packaged as a Pypi library. Toposcale is an original idea of Joel Fiddes to perform topography-based downscaling of climate data to the hillslope scale.
 
 Documentation avalaible: https://topopyscale.readthedocs.io
```

#### html2text {}

```diff
@@ -1,31 +1,33 @@
-Metadata-Version: 2.1 Name: topopyscale Version: 0.2.2 Summary: A Python
-package to perform climate downscaling at the hillslope scale Home-page: https:
-//github.com/ArcticSnow/TopoPyScale Download-URL: https://github.com/
-ArcticSnow/TopoPyScale/releases/latest Author: ['Simon Filhol', 'Joel Fiddes',
-'Kristoffer Aalstad'] Author-email: simon.filhol@geo.uio.no License: MIT
-Project-URL: Documentation, https://topopyscale.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/ArcticSnow/TopoPyScale Project-URL:
-Examples, https://github.com/ArcticSnow/TopoPyScale_examples Keywords:
+Metadata-Version: 2.1 Name: topopyscale Version: 0.2.3 Summary: TopoPyScale: A
+Python Package for Hillslope Climate Downscaling Home-page: https://github.com/
+ArcticSnow/TopoPyScale Download-URL: https://github.com/ArcticSnow/TopoPyScale/
+releases/latest Author: ['Simon Filhol', 'Joel Fiddes', 'Kristoffer Aalstad']
+Author-email: simon.filhol@geo.uio.no License: MIT Project-URL: Documentation,
+https://topopyscale.readthedocs.io/en/latest/ Project-URL: Source, https://
+github.com/ArcticSnow/TopoPyScale Project-URL: Examples, https://github.com/
+ArcticSnow/TopoPyScale_examples Keywords:
 climate,downscaling,meteorology,xarray Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering :: Visualization Classifier: Topic :: Scientific/
 Engineering :: Hydrology Classifier: Topic :: Scientific/Engineering ::
 Atmospheric Science Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9 Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE [![DOI](https://
 zenodo.org/badge/411249045.svg)](https://zenodo.org/badge/latestdoi/411249045)
 [![GitHub license](https://img.shields.io/github/license/ArcticSnow/
 TopoPyScale)](https://github.com/ArcticSnow/TopoPyScale/blob/main/LICENSE) !
 [GitHub release (latest by date)](https://img.shields.io/github/v/release/
 ArcticSnow/TopoPyScale) [https://joss.theoj.org/papers/
 91621581b2d0c097495fdd1e58179e87/status.svg] [![][docs-dev-img]][docs-dev-url]
 ![Test](https://github.com/ArcticSnow/TopoPyScale/actions/workflows/
-test_topopyscale.yml/badge.svg) [docs-dev-img]: https://img.shields.io/badge/
-docs-latest-blue.svg [docs-dev-url]: https://topopyscale.readthedocs.io #
+test_topopyscale.yml/badge.svg) Binder Notebooks Examples: [![Binder](https://
+mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ArcticSnow/
+TopoPyScale_examples/HEAD) [docs-dev-img]: https://img.shields.io/badge/docs-
+latest-blue.svg [docs-dev-url]: https://topopyscale.readthedocs.io #
 TopoPyScale Python version of Toposcale packaged as a Pypi library. Toposcale
 is an original idea of Joel Fiddes to perform topography-based downscaling of
 climate data to the hillslope scale. Documentation avalaible: https://
 topopyscale.readthedocs.io ![](https://github.com/ArcticSnow/TopoPyScale/blob/
 main/JOSS/temperature_comparison_crop_scaled.jpg) **References:** - Fiddes, J.
 and Gruber, S.: TopoSCALE v.1.0: downscaling gridded climate data in complex
 terrain, Geosci. Model Dev., 7, 387â405, https://doi.org/10.5194/gmd-7-387-
```

### Comparing `topopyscale-0.2.2/README.md` & `topopyscale-0.2.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 [![DOI](https://zenodo.org/badge/411249045.svg)](https://zenodo.org/badge/latestdoi/411249045)
 [![GitHub license](https://img.shields.io/github/license/ArcticSnow/TopoPyScale)](https://github.com/ArcticSnow/TopoPyScale/blob/main/LICENSE)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/ArcticSnow/TopoPyScale)
 <a href="https://joss.theoj.org/papers/91621581b2d0c097495fdd1e58179e87"><img src="https://joss.theoj.org/papers/91621581b2d0c097495fdd1e58179e87/status.svg"></a>
 [![][docs-dev-img]][docs-dev-url]
 ![Test](https://github.com/ArcticSnow/TopoPyScale/actions/workflows/test_topopyscale.yml/badge.svg)
 
+Binder Notebooks Examples: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ArcticSnow/TopoPyScale_examples/HEAD)
+
 [docs-dev-img]: https://img.shields.io/badge/docs-latest-blue.svg
 [docs-dev-url]: https://topopyscale.readthedocs.io
 
 # TopoPyScale
 Python version of Toposcale packaged as a Pypi library. Toposcale is an original idea of Joel Fiddes to perform topography-based downscaling of climate data to the hillslope scale.
 
 Documentation avalaible: https://topopyscale.readthedocs.io
```

#### html2text {}

```diff
@@ -1,16 +1,18 @@
  [![DOI](https://zenodo.org/badge/411249045.svg)](https://zenodo.org/badge/
 latestdoi/411249045) [![GitHub license](https://img.shields.io/github/license/
 ArcticSnow/TopoPyScale)](https://github.com/ArcticSnow/TopoPyScale/blob/main/
 LICENSE) ![GitHub release (latest by date)](https://img.shields.io/github/v/
 release/ArcticSnow/TopoPyScale) [https://joss.theoj.org/papers/
 91621581b2d0c097495fdd1e58179e87/status.svg] [![][docs-dev-img]][docs-dev-url]
 ![Test](https://github.com/ArcticSnow/TopoPyScale/actions/workflows/
-test_topopyscale.yml/badge.svg) [docs-dev-img]: https://img.shields.io/badge/
-docs-latest-blue.svg [docs-dev-url]: https://topopyscale.readthedocs.io #
+test_topopyscale.yml/badge.svg) Binder Notebooks Examples: [![Binder](https://
+mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ArcticSnow/
+TopoPyScale_examples/HEAD) [docs-dev-img]: https://img.shields.io/badge/docs-
+latest-blue.svg [docs-dev-url]: https://topopyscale.readthedocs.io #
 TopoPyScale Python version of Toposcale packaged as a Pypi library. Toposcale
 is an original idea of Joel Fiddes to perform topography-based downscaling of
 climate data to the hillslope scale. Documentation avalaible: https://
 topopyscale.readthedocs.io ![](https://github.com/ArcticSnow/TopoPyScale/blob/
 main/JOSS/temperature_comparison_crop_scaled.jpg) **References:** - Fiddes, J.
 and Gruber, S.: TopoSCALE v.1.0: downscaling gridded climate data in complex
 terrain, Geosci. Model Dev., 7, 387â405, https://doi.org/10.5194/gmd-7-387-
```

### Comparing `topopyscale-0.2.2/TopoPyScale/fetch_dem.py` & `topopyscale-0.2.3/TopoPyScale/fetch_dem.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 - [ ] Norwegian DEM
 
 """
 
 import sys
 import os
 
-def fetch_dem(dem_dir, extent, dem_epsg, dem_file):
+def fetch_dem(dem_dir, extent, dem_epsg, dem_file, dem_resol=None):
     """
     Function to fetch DEM data from SRTM and potentially other sources
 
     Args:
         dem_dir (str): path to dem folder
-        extent (list): list of spatial extent in lat-lon [latN, latS, lonW, lonE]
+        extent (dict): list of spatial extent in lat-lon [latN, latS, lonW, lonE]
         epsg (int): epsg projection code
         dem_file (str): filename of the downloaded DEM. must be myfile.tif
     """
 
     ymax = extent.get('latN')
     ymin = extent.get('latS')
     xmin = extent.get('lonW')
@@ -50,15 +50,19 @@
             return RuntimeError
         # os.system('eio clean')
 
 
 
         # target_epsg = input("---> provide target EPSG (default: 32632):") or '32645'
         # crop to extent defined by "-te <xmin ymin xmax ymax>" flag to ensure rectangulatr output with no NAs. -te_srs  states the epsg of crop parameeters (WGS84)
-        cmd_2 = 'gdalwarp -tr 30 30 -r bilinear -s_srs epsg:4326 -t_srs epsg:{} -te_srs epsg:{} -te {} {} {} {} {} {}'.format(dem_epsg,
+        if dem_resol is not None:
+            res = dem_resol
+        else:
+            res = 30
+        cmd_2 = 'gdalwarp -tr '+str(res) + ' ' + str(res) +  ' -r bilinear -s_srs epsg:4326 -t_srs epsg:{} -te_srs epsg:{} -te {} {} {} {} {} {}'.format(dem_epsg,
                                                                                                                 4326,
                                                                                                                  xmin,
                                                                                                                  ymin,
                                                                                                                  xmax,
                                                                                                                  ymax,
                                                                                                dem_dir + 'dem_SRTM1.tif',
                                                                                                dem_dir  + dem_file,
@@ -85,15 +89,19 @@
                                                                                          0.2)
         print('>===== command to download DEM  from SRTM3 ====<')
         print('eio clean')
         os.system(cmd_1)
         print('eio clean')
         #target_epsg = input("---> provide target EPSG (default: 32632):") or '32632'
 
-        cmd_2 = 'gdalwarp -tr 90 90 -r bilinear -s_srs epsg:4326 -t_srs epsg:{} -te_srs epsg:{} -te {} {} {} {} {} {}'.format(dem_epsg,
+        if dem_resol is not None:
+            res = dem_resol
+        else:
+            res = 90
+        cmd_2 = 'gdalwarp -tr ' +str(res) + ' ' + str(res) +   ' -r bilinear -s_srs epsg:4326 -t_srs epsg:{} -te_srs epsg:{} -te {} {} {} {} {} {}'.format(dem_epsg,
                                                                                                                 4326,
                                                                                                                  xmin,
                                                                                                                  ymin,
                                                                                                                  xmax,
                                                                                                                  ymax,
                                                                                                dem_dir + 'dem_SRTM3.tif',
                                                                                                dem_dir + dem_file,
```

### Comparing `topopyscale-0.2.2/TopoPyScale/fetch_era5.py` & `topopyscale-0.2.3/TopoPyScale/fetch_era5.py`

 * *Files 9% similar despite different names*

```diff
@@ -269,46 +269,90 @@
 							 '21:00', '22:00', '23:00']
 
 	target = eraDir + "/PLEV_%04d%02d.nc" % (currentYear, currentMonth)
 	plevels = plevels
 	era5_request_plev(dataset, currentYear, currentMonth, bbox, target, product, time, plevels)
 
 
-def return_latest_date():
-	# method to return latest full date available in CDS
-	
-	print("WARNING: Ignore the following warning - this is due to requesting todays date with the intention to harvest the date returned in error message. There must be a cleaner way to get latest date....")
-	c = cdsapi.Client()
-
-	# how to retrieve latest date that era5 data is available
-	try:
-	    # this will always fail but return the latest date in error message
-	    # should be a cleaner way of doing this with api?
-
-		c = cdsapi.Client()
-
-		# Retrieve the list of available files for the ERA5 dataset
-		res = c.retrieve("reanalysis-era5-single-levels", {
-		    "variable": "2m_temperature",
-		    "product_type": "reanalysis",
-		    "format": "json"
-		})
-
-	except Exception as e:
-	    # Extract the latest date from the exception object
-	    exc_type = type(e).__name__
-	    exc_msg = str(e)
-	    print(f"Caught {exc_type} with message '{exc_msg}'")
-
-	# Example string representing a date and time within a string
-	date_string = exc_msg
-	# Define the format string to match the input string
-	format_string = 'the request you have submitted is not valid. None of the data you have requested is available yet, please revise the period requested. The latest date available for this dataset is: %Y-%m-%d %H:%M:%S.%f.' 
-	# Parse the date string and create a datetime object
-	latest_date = datetime.strptime(date_string, format_string)
-
-	if latest_date.hour < 23:
-		# Subtract one day from the datetime object
-		latest_date = latest_date - timedelta(days=1)
-		# Print the updated datetime object
+# def return_latest_date():
+# 	# method to return latest full date available in CDS
+#
+# 	print("WARNING: Ignore the following warning - this is due to requesting todays date with the intention to harvest the date returned in error message. There must be a cleaner way to get latest date....")
+# 	c = cdsapi.Client()
+#
+# 	# how to retrieve latest date that era5 data is available
+# 	try:
+# 	    # this will always fail but return the latest date in error message
+# 	    # should be a cleaner way of doing this with api?
+#
+# 		c = cdsapi.Client()
+#
+# 		# Retrieve the list of available files for the ERA5 dataset
+# 		res = c.retrieve("reanalysis-era5-single-levels", {
+# 		    "variable": "2m_temperature",
+# 		    "product_type": "reanalysis",
+# 		    "format": "json"
+# 		})
+#
+# 	except Exception as e:
+# 	    # Extract the latest date from the exception object
+# 	    exc_type = type(e).__name__
+# 	    exc_msg = str(e)
+# 	    print(f"Caught {exc_type} with message '{exc_msg}'")
+#
+# 	# Example string representing a date and time within a string
+# 	date_string = exc_msg
+# 	# Define the format string to match the input string
+# 	format_string = 'the request you have submitted is not valid. None of the data you have requested is available yet, please revise the period requested. The latest date available for this dataset is: %Y-%m-%d %H:%M:%S.%f.'
+# 	# Parse the date string and create a datetime object
+# 	latest_date = datetime.strptime(date_string, format_string)
+#
+# 	if latest_date.hour < 23:
+# 		# Subtract one day from the datetime object
+# 		latest_date = latest_date - timedelta(days=1)
+# 		# Print the updated datetime object
+#
+# 	return(latest_date)
+
+def return_last_fullday():
+	# Get current UTC time
+	current_time_utc = datetime.utcnow()
+
+	# Round down to the nearest hour
+	rounded_time_utc = current_time_utc.replace(minute=0, second=0, microsecond=0)
+
+	# Get time 5 days ago in UTC
+	five_days_ago_utc = rounded_time_utc - timedelta(days=5)
+
+	# Format the time strings
+	current_time_utc_str = rounded_time_utc.strftime("%Y-%m-%d %H:%M:%S UTC")
+	five_days_ago_utc_str = five_days_ago_utc.strftime("%Y-%m-%d %H:%M:%S UTC")
+
+	# Print the results
+	five_days_ago_utc = datetime.strptime(five_days_ago_utc_str, "%Y-%m-%d %H:%M:%S UTC")
+
+	# if 5 days ago is an incomplete day h<23, Subtract one day from the datetime object to get last full day of data
+	if five_days_ago_utc.hour < 23:
+		last_fullday_data = five_days_ago_utc - timedelta(days=1)
+
+	last_fullday_data_str = last_fullday_data.strftime("%Y-%m-%d %H:%M:%S UTC")
+	print("Current time (rounded down) in UTC:", current_time_utc_str)
+	print("Last ERA5T data in UTC:", five_days_ago_utc_str)
+	print("Last full day ERA5T data in UTC:", last_fullday_data_str)
+
+	return (last_fullday_data)
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
 
-	return(latest_date)
```

### Comparing `topopyscale-0.2.2/TopoPyScale/meteo_util.py` & `topopyscale-0.2.3/TopoPyScale/meteo_util.py`

 * *Files identical despite different names*

### Comparing `topopyscale-0.2.2/TopoPyScale/precip_orographic.py` & `topopyscale-0.2.3/TopoPyScale/precip_orographic.py`

 * *Files identical despite different names*

### Comparing `topopyscale-0.2.2/TopoPyScale/solar_geom.py` & `topopyscale-0.2.3/TopoPyScale/solar_geom.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     ds = xr.Dataset(
         {
             "zenith": (["point_id", "time"], np.deg2rad(arr_val[:, 0, :])),
             "azimuth": (["point_id", "time"], np.deg2rad(arr_val[:,1,:] - 180)),
             "elevation": (["point_id", "time"], np.deg2rad(arr_val[:, 2, :])),
         },
         coords={
-            "point_id": df_position.index,
+            "point_id":(("point_id"), df_position.index),
             "time": pd.date_range(start_date, pd.to_datetime(end_date)+pd.to_timedelta('1D'), freq=tstep, inclusive='left'),
             "reference_time": pd.Timestamp(start_date),
         },
     )
 
     ds['mu0'] = np.cos(ds.zenith) * (np.cos(ds.zenith)>0)
     S0 = 1370 # Solar constat (total TOA solar irradiance) [Wm^-2] used in ECMWF's IFS
```

### Comparing `topopyscale-0.2.2/TopoPyScale/topo_compare.py` & `topopyscale-0.2.3/TopoPyScale/topo_compare.py`

 * *Files identical despite different names*

### Comparing `topopyscale-0.2.2/TopoPyScale/topo_da.py` & `topopyscale-0.2.3/TopoPyScale/topo_da.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 import glob
 import re
 import pandas as pd
 import numpy as np
 from matplotlib import pyplot as plt
 import copy
 import rasterio as rio
+from rasterio.plot import show
 from osgeo import gdal
 from osgeo import osr 
 from scipy.interpolate import interp1d
 from TopoPyScale import topo_sim as sim
 from datetime import datetime
 import xarray as xr
 import rioxarray
+from scipy.special import logsumexp
 
 
 # import gdal
 
 
 def lognormDraws_kris(n, med, s):
     """
@@ -153,15 +155,15 @@
         ds_perturb["tp"] = ds.tp * perturb.pbias[N_ens]
         ds_perturb["SW"] = ds.SW * perturb.swbias[N_ens]
         ds_perturb["LW"] = ds.LW * perturb.lwbias[N_ens]
 
     return ds_perturb
 
 
-def construct_HX(wdir, startDA, endDA):
+def construct_HX(wdir, startDA, endDA, ncol):
     """
     Function to generate HX matrix of ensembleSamples x day
 
     Args:
         wdir: working directory
         DAyear: year of data assimilation yyyy
         startDA: start of data assimilation window  yyyy-mm-dd
@@ -190,16 +192,16 @@
     #     sys.exit("daYear does not exist in simulation period")
     # if len(endIndex) == 0:
     #     sys.exit("daYear does not exist in simulation period")
 
     # construct a list as long as samples x ensembles (sampleEnsembles)
     data = []
     for file_path in file_list:
-        # column 7 (index 6) is snow water equiv
-        data.append(np.genfromtxt(file_path, usecols=6)[int(startIndex):int(endIndex) + 1])
+        # column 7 (ncol 6) is snow water equiv
+        data.append(np.genfromtxt(file_path, usecols=ncol)[int(startIndex):int(endIndex) + 1])
 
     myarray = np.asarray(data)  # sampleEnsembles x days
     ensembRes = pd.DataFrame(myarray.transpose())
 
     mydates = df.iloc[:, 0][int(startIndex):int(endIndex) + 1]
 
     return ensembRes, mydates
@@ -291,14 +293,15 @@
 
 
     """
 
 
 def pymodis_download(wdir, vert, horiz, STARTDATE, ENDDATE):
     # http://www.pymodis.org/scripts/modis_download.html
+    # pip inpip install pyModis
 
     USER = "jfiddes"  # os.getenv('user')
     PWD = "sT0kkang!"  # os.getenv('pwd')
     MODPATH = wdir + "/modis/"
     HOST = "https://n5eil01u.ecs.nsidc.org/"
     FOLDER = "MOST"
     PRODUCT = "MOD10A1F.061"
@@ -573,17 +576,15 @@
 
     LH = np.exp(-0.5 * EObj)  # Scaled likelihood.
 
     # Calculate the posterior weights as the normalized likelihood.
     w = LH / sum(LH)
 
 
-import numpy as np
-import matplotlib.pyplot as plt
-from scipy.special import logsumexp
+
 
 
 def EnKA(prior, obs, pred, alpha, R):
     """
     EnKA: Implmentation of the Ensemble Kalman Analysis
     Inputs:
         prior: Prior ensemble matrix (n x N array)
@@ -733,15 +734,15 @@
 
     # pdb.set_trace()
     # Residual and log-likelihood
     if m == 1:
         residual = obs - pred
         llh = -0.5 * ((residual ** 2) * (1 / R))
     else:
-        residual = obs[:, None] - pred
+        residual = np.array(obs)[:, None] - pred
         # pdb.set_trace()
         llh = -0.5 * ((1 / R) @ (residual ** 2))
 
     # Log of normalizing constant
     # A properly scaled version of this could be output for model comparison.
     lZ = logsumexp(llh)  # from scipy.special import logsumexp
 
@@ -752,15 +753,15 @@
         pass
     else:
         raise Exception('Something went wrong with the PBS, try pdb.set_trace()')
 
     return w
 
 
-def da_plots(HX1, HX2, W, mydates, myobs):
+def da_plots(HX1, HX2,noDA,  W, mydates, myobs):
     """
     Function to extract mean fSSCA from domain
 
     Args:
         HX1:
         HX2:
         weights: weights output from PBS (dims 1 x NENS)
@@ -786,31 +787,31 @@
             dfOrder = df.sort_values('mu')
             y_interp = interp1d(np.cumsum(dfOrder.wfill), dfOrder.mu, fill_value="extrapolate")
             med = y_interp(percentile)
             med_post.append(med)
 
         return np.array(med_post)
 
-    # for prior all ensemble members considered equally likely therefore weights are all
+    # for prior all ensemble members considered equally likely therefore weights are all equal
     weights = [1/HX1.shape[1]] * HX1.shape[1]
     prior_med = percentile_plot(HX1, weights, 0.5)
     prior_low = percentile_plot(HX1, weights, 0.1)
     prior_high = percentile_plot(HX1, weights, 0.8)
 
     # for posterior weights are given by the output of PBS, W
     post_med = percentile_plot(HX1, W, 0.5)
     post_low = percentile_plot(HX1, W, 0.1)
     post_high = percentile_plot(HX1, W, 0.8)
 
     plt.subplot(1, 2, 1)
     plt.fill_between(mydates, prior_low, prior_high, alpha=0.2)
-    plt.plot(mydates, prior_med)
+    plt.plot(mydates, prior_med, label="prior median")
     plt.fill_between(mydates, post_low, post_high, alpha=0.2)
-    plt.plot(mydates, post_med)
-    plt.plot(mydates, myobs)
+    plt.plot(mydates, post_med, label = "posterior median")
+    plt.plot(mydates, myobs, label= "observations")
     plt.xlabel("Date")
     plt.ylabel("fSCA")
     plt.legend()
 
     # for prior all ensemble members considered equally likely therefore weights are all
     weights = [1/HX1.shape[1]] *  HX1.shape[1]
     prior_med = percentile_plot(HX2, weights, 0.5)
@@ -820,17 +821,18 @@
     # for posterior weights are given by the output of PBS, W
     post_med = percentile_plot(HX2, W, 0.5)
     post_low = percentile_plot(HX2, W, 0.1)
     post_high = percentile_plot(HX2, W, 0.9)
 
     plt.subplot(1, 2, 2)
     plt.fill_between(mydates, prior_low, prior_high, alpha=0.2)
-    plt.plot(mydates, prior_med)
+    plt.plot(mydates, prior_med, label="prior median")
     plt.fill_between(mydates, post_low, post_high, alpha=0.2)
-    plt.plot(mydates, post_med)
+    plt.plot(mydates, post_med, label="posterior median")
+    plt.plot(mydates, noDA, label="no DA")
     plt.xlabel("Date")
     plt.ylabel("HS (m)")
     plt.legend()
     plt.show()
 
 
 def fsca_plots(wdir, plotDay, df_mean):
@@ -863,15 +865,15 @@
 
 
     modis_file = glob.glob(wdir + "modis/transformed/MOD10A1F.A" + juldate + "*")
 
     src = rio.open(modis_file[0])
     fig, (axrgb, axhist) = plt.subplots(1, 2, figsize=(14,7))
 
-    rio.plot.show(src, ax=axrgb,vmin=0, vmax=100)
+    show(src, ax=axrgb,vmin=0, vmax=100)
     cbar1 = plt.imshow(src.read(1), cmap='viridis', vmin=0, vmax=100)
     fig.colorbar(cbar1, ax=axrgb)
 
     nclust = len(df_mean)
     lookup = np.arange(nclust, dtype=np.uint16)
 
     for i in range(0, nclust):
@@ -885,23 +887,23 @@
         # Reclassify in a single operation using broadcasting
         array = lookup[array]
         # binary map
         array[array <= 0] = 0
         array[array > 0] = 1
 
 
-    # rasterio.plot.show(array, cmap='viridis')
+    # rasteshow(array, cmap='viridis')
     # plt.show()
 
     with rio.open('output_raster.tif', 'w', **profile) as dst:
         # Write to disk
         dst.write(array.astype(rio.int16))
 
     src1 = rio.open("output_raster.tif")
-    rio.plot.show(src1, ax=axhist)
+    show(src1, ax=axhist)
     cbar2 = plt.imshow(src1.read(1), cmap='viridis')
     fig.colorbar(cbar2, ax=axhist)
     plt.show()
 
 
 # def spatial_plots(df_mean, plot=False):
 #     """
@@ -940,24 +942,24 @@
 #         # Reclassify in a single operation using broadcasting
 #         array = lookup[array]
 #         # binary map
 #         array[array <= 0] = 0
 #         array[array > 0] = 1
 #
 #
-#     # rasterio.plot.show(array, cmap='viridis')
+#     # rasteshow(array, cmap='viridis')
 #     # plt.show()
 #
 #     with rio.open('output_raster.tif', 'w', **profile) as dst:
 #         # Write to disk
 #         dst.write(array.astype(rasterio.int16))
 #
 #     if plot:
 #         src1 = rio.open("output_raster.tif")
-#         rio.plot.show(src1, ax=axhist)
+#         show(src1, ax=axhist)
 #         cbar2 = plt.imshow(src1.read(1), cmap='viridis')
 #         fig.colorbar(cbar2, ax=axhist)
 #         plt.show()
 
 def da_compare_plot(wdir, plotDay, df_mean_open, df_mean_da):
     """
     Function to plot side by side observed fSCA 500m [0-1] and modelled SCA 30 m [0,1]
@@ -983,88 +985,88 @@
     # set up plot axis
     fig, ([axmod1, axopen], [axmod2, axda]) = plt.subplots(2, 2, figsize=(14, 7))
 
     # convert data YYYY-mm-dd to YYYYddd
     dt = datetime.strptime(plotDay, "%Y-%m-%d")
     doy = dt.timetuple().tm_yday
     year = dt.year
-    juldate = str(year)+str(doy)
+    juldate = str(year)+str(f'{doy:03d}')
 
     # plot modis
-    modis_file = glob.glob(wdir + "modis/transformed/MOD10A1F.A" + juldate + "*")
+    modis_file = glob.glob(wdir + "/modis/transformed/MOD10A1F.A" + juldate + "*")
     src = rio.open(modis_file[0])
-    rio.plot.show(src, ax=axmod1,vmin=0, vmax=100)
+    show(src, ax=axmod1,vmin=0, vmax=100)
     cbar1 = plt.imshow(src.read(1), cmap='viridis', vmin=0, vmax=100)
     fig.colorbar(cbar1, ax=axmod1)
 
     # compute and plot open loop
     nclust = len(df_mean_open)
     lookup = np.arange(nclust, dtype=np.uint16)
 
     for i in range(0, nclust):
         lookup[i] = df_mean_open[i]
 
-    with rio.open('landform.tif') as src:
+    with rio.open('outputs/landform.tif') as src:
         # Read as numpy array
         array = src.read()
         profile = src.profile
 
         # Reclassify in a single operation using broadcasting
         array = lookup[array]
         # binary map
-        #array[array <= 0] = 0
-        #array[array > 0] = 1
+        array[array <= 0] = 0
+        array[array > 0] = 1
 
 
-    # rio.plot.show(array, cmap='viridis')
+    # show(array, cmap='viridis')
     # plt.show()
 
     with rio.open('output_raster.tif', 'w', **profile) as dst:
         # Write to disk
         dst.write(array.astype(rio.int16))
 
     src1 = rio.open("output_raster.tif")
-    rio.plot.show(src1, ax=axopen)
+    show(src1, ax=axopen)
     cbar2 = plt.imshow(src1.read(1), cmap='viridis')
     fig.colorbar(cbar2, ax=axopen)
 
     # plot modis again
     src = rio.open(modis_file[0])
-    rio.plot.show(src, ax=axmod2,vmin=0, vmax=100)
+    show(src, ax=axmod2,vmin=0, vmax=100)
     cbar1 = plt.imshow(src.read(1), cmap='viridis', vmin=0, vmax=100)
     fig.colorbar(cbar1, ax=axmod2)
 
     # compute and plot DA
     nclust = len(df_mean_da)
     lookup = np.arange(nclust, dtype=np.uint16)
 
     for i in range(0, nclust):
         lookup[i] = df_mean_da[i]
 
-    with rio.open('landform.tif') as src:
+    with rio.open('outputs/landform.tif') as src:
         # Read as numpy array
         array = src.read()
         profile = src.profile
 
         # Reclassify in a single operation using broadcasting
         array = lookup[array]
         # binary map
-        #array[array <= 0] = 0
-        #array[array > 0] = 1
+        array[array <= 0] = 0
+        array[array > 0] = 1
 
 
-    # rio.plot.show(array, cmap='viridis')
+    # show(array, cmap='viridis')
     # plt.show()
 
     with rio.open('output_raster.tif', 'w', **profile) as dst:
         # Write to disk
         dst.write(array.astype(rio.int16))
 
     src1 = rio.open("output_raster.tif")
-    rio.plot.show(src1, ax=axda)
+    show(src1, ax=axda)
     cbar2 = plt.imshow(src1.read(1), cmap='viridis')
     fig.colorbar(cbar2, ax=axda)
     plt.show()
 
 def build_modis_cube(wdir):
     geotiff_list_unsorted = glob.glob(wdir + "modis/transformed/MOD10A1F.A*")
     # Natural sort to get correct order ensemb * samples
```

### Comparing `topopyscale-0.2.2/TopoPyScale/topo_export.py` & `topopyscale-0.2.3/TopoPyScale/topo_export.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import sys, csv
 import numpy as np
 import pandas as pd
 import datetime as dt
 import xarray as xr
 from scipy import io
 from TopoPyScale import meteo_util as mu
+from TopoPyScale import topo_utils as tu
 from multiprocessing.dummy import Pool as ThreadPool
 import multiprocessing as mproc
 
 
 def compute_scaling_and_offset(da, n=16):
     """
     Compute offset and scale factor for int conversion
@@ -32,35 +33,36 @@
     # stretch/compress data to the available packed range
     scale_factor = (vmax - vmin) / (2 ** n - 1)
     # translate the range to be symmetric about zero
     add_offset = vmin + 2 ** (n - 1) * scale_factor
 
     return scale_factor, add_offset
 
-def to_netcdf(ds, fname='output.nc', variables=None):
+def to_netcdf(ds, fname='output.nc', variables=None, complevel=9):
         """
         Generic function to save a datatset to one single compressed netcdf file
 
         Args:
             fname (str): name of export file
             variables (list str): list of variable to export. Default exports all variables
+            complevel (int): Compression level. 1-9
         """
 
         encod_dict = {}
         if variables is None:
             variables = list(ds.keys())
 
         for var in variables:
             scale_factor, add_offset = compute_scaling_and_offset(ds[var], n=10)
             if str(ds[var].dtype)[:3] == 'int':
                 encod_dict.update({var:{
                                    'dtype':ds[var].dtype}})
             else:
                 encod_dict.update({var:{"zlib": True,
-                                       "complevel": 9,
+                                       "complevel": complevel,
                                        'dtype':'int16',
                                        'scale_factor':scale_factor,
                                        'add_offset':add_offset}})
         ds[variables].to_netcdf(fname, encoding=encod_dict, engine='h5netcdf')
 
         print(f'---> File {fname} saved')
 
@@ -81,14 +83,16 @@
         da_labels:
         fname:
         path:
 
     Returns:
         Save downscaled timeseries and toposub cluster mapping
     """
+    ver_dict = tu.get_versionning()
+    
     if da_label is not None:
     	da_label.to_netcdf(path + fname_labels)
 
     da_label.to_netcdf(path + fname_labels)
 
     fo = xr.Dataset()
     fo['tair'] = ds['t'].T
@@ -110,14 +114,17 @@
     fo.sw.attrs = {'units':'W/m^2', 'standard_name':'sw', 'long_name':'Surface Incident Direct Shortwave Radiation', '_FillValue': -9999999.0}
     fo.lw.attrs = {'units':'W/m^2', 'standard_name':'lw', 'long_name':'Surface Incident Longtwave Radiation', '_FillValue': -9999999.0}
     fo.p.attrs = {'units':'Pa', 'standard_name':'p', 'long_name':'Surface Pressure', '_FillValue': -9999999.0}
 
     fo.attrs = {'title':'Forcing for MuSa assimilation scheme',
                 'source': 'Data from {} downscaled with TopoPyScale'.format(climate_dataset_name),
                 'creator_name':'Dataset created by {}'.format(project_authors),
+                'package_version':ver_dict.get('package_version'),
+                'url_TopoPyScale': 'https://github.com/ArcticSnow/TopoPyScale',
+                'git_commit': ver_dict.get('git_commit'),
                 'date_created':dt.datetime.now().strftime('%Y/%m/%d %H:%M:%S')}
     encod_dict = {}
     for var in list(fo.keys()):
         scale_factor, add_offset = compute_scaling_and_offset(fo[var], n=10)
         encod_dict.update({var:{"zlib": True,
                                "complevel": 9,
                                'dtype':'int16',
@@ -155,14 +162,16 @@
         fname_format (str): file name for output
         path (str): path where to export files
         label_map (bool): export cluster_label map
         da_label (dataarray):(optional) dataarray containing label value for each pixel of the DEM
     
     """
     # Add logic to save maps of cluster labels in case of usage of topo_sub
+    
+    ver_dict = tu.get_versionning()
     if label_map:
         if da_label is None:
             print('ERROR: no cluster label (da_label) provided')
             sys.exit()
         else:
             da_label.to_netcdf(path + 'cluster_labels_map.nc')
 
@@ -191,14 +200,17 @@
         fo.Sin.attrs = {'units':'W/m^2', 'standard_name':'Sin', 'long_name':'Surface Incident Direct Shortwave Radiation', '_FillValue': -9999999.0}
         fo.Lin.attrs = {'units':'W/m^2', 'standard_name':'Lin', 'long_name':'Surface Incident Longtwave Radiation', '_FillValue': -9999999.0}
         fo.p.attrs = {'units':'Pa', 'standard_name':'p', 'long_name':'Surface Pressure', '_FillValue': -9999999.0}
 
         fo.attrs = {'title':'Forcing for Cryogrid Community model',
                     'source': 'Data from {} downscaled with TopoPyScale'.format(climate_dataset_name),
                     'creator_name':'Dataset created by {}'.format(project_author),
+                    'package_version':ver_dict.get('package_version'),
+                    'url_TopoPyScale': 'https://github.com/ArcticSnow/TopoPyScale',
+                    'git_commit': ver_dict.get('git_commit'),
                     'date_created':dt.datetime.now().strftime('%Y/%m/%d %H:%M:%S')}
         encod_dict = {}
         for var in list(fo.keys()):
             scale_factor, add_offset = compute_scaling_and_offset(fo[var], n=10)
             encod_dict.update({var:{"zlib": True,
                                    "complevel": 9,
                                    'dtype':'int16',
@@ -209,14 +221,37 @@
         fo['elevation'] = df_pts.elevation.iloc[pt]
         fo.latitude.attrs = {'units':'deg', 'standard_name':'latitude'}
         fo.longitude.attrs = {'units':'deg', 'standard_name':'longitude'}
         fo.elevation.attrs = {'units':'m', 'standard_name':'elevation'}
         fo.to_netcdf(foutput, encoding=encod_dict)
         print('---> File {} saved'.format(foutput))
 
+def steepSnowReduce_all(snow, slope):
+    # ======================================================================================
+    # # linearly reduce snow to zero in steep slopes
+    # if steepSnowReduce=="TRUE": # make this an option if need that in future
+    # ======================================================================================
+
+    snowSMIN = 30.
+    snowSMAX = 80.
+
+    # partial snow removal
+    k = (snowSMAX - slope) / (snowSMAX - snowSMIN)
+
+    # no snow removal
+    a = slope < snowSMIN
+    k[~a] = 1
+
+    # all snow removal
+    a = slope > snowSMIN
+    k[~a] = 0
+
+    steepSnow = snow.transpose() * np.array(k).transpose()
+
+    return (steepSnow)
 
 def to_fsm(ds, fname_format='FSM_pt_*.tx', snow_partition_method='continuous'):
     """
     Function to export data for FSM.
 
     Args:
         ds (dataset): downscaled_pts,
@@ -336,14 +371,16 @@
         climate_dataset_name (str): name of original climate dataset. Default 'ERA5',
         project_author (str): name of project author(s)
         snow_partition_method (str): snow/rain partitioning method: default 'jennings2018_trivariate'
 
     """
     # create one file per point_id
     n_digits = len(str(ds.point_id.values.max()))
+    ver_dict = tu.get_versionning()
+    
     for pt in ds.point_id.values:
         foutput = fname_format.split('*')[0] + str(pt).zfill(n_digits) + fname_format.split('*')[1]
         ds_pt = ds.sel(point_id=pt).copy()
         df = pd.DataFrame()
         df['time'] = ds_pt.time.values
         df['Tair'] = ds_pt.t.values
         df['DIR_SWdown'] = ds_pt.SW.values
@@ -385,14 +422,17 @@
         fo.CO2air.attrs = {'units':'kg/m3', 'standard_name':'CO2air', 'long_name':'Near Surface CO2 Concentration', '_FillValue': -9999999.0}
         fo.NEB.attrs = {'units':'between 0 and 1', 'standard_name':'NEB', 'long_name':'Nebulosity', '_FillValue': -9999999.0}
 
 
         fo.attrs = {'title':'Forcing for SURFEX CROCUS',
                     'source': 'data from {} downscaled with TopoPyScale ready for CROCUS'.format(climate_dataset_name),
                     'creator_name':'Dataset created by {}'.format(project_author),
+                    'package_version':ver_dict.get('package_version'),
+                    'git_commit': ver_dict.get('git_commit'),
+                    'url_TopoPyScale': 'https://github.com/ArcticSnow/TopoPyScale', 
                     'date_created':dt.datetime.now().strftime('%Y/%m/%d %H:%M:%S')}
 
         fo['ZS'] = np.float64(df_pts.iloc[pt].elevation)
         fo['aspect'] = np.float64(np.rad2deg(df_pts.iloc[pt].aspect))
         fo['slope'] = np.float64(np.rad2deg(df_pts.iloc[pt].slope))
         fo['massif_number'] = np.float64(0)
         fo['LAT'] = df_pts.iloc[pt].latitude
```

### Comparing `topopyscale-0.2.2/TopoPyScale/topo_obs.py` & `topopyscale-0.2.3/TopoPyScale/topo_obs.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     """
     df_obs = pd.concat(map(pd.read_pickle, glob.glob(os.path.join('', path + fnames))))
     df = pd.pivot_table(df_obs, columns=['elementId'],values=['value'], index=['sourceId', 'referenceTime'])
     ds = df.xs('value', axis=1, level=0).to_xarray()
     return ds
 
 
-def fetch_WMO_insitu_observations(years, months, bbox, target_path='./inputs/observations'):
+def fetch_WMO_insitu_observations(years, months, bbox, target_path='./inputs/observations', product='sub_daily'):
     """
     Function to download WMO in-situ data from land surface in-situ observations from Copernicus.
     https://cds.climate.copernicus.eu/cdsapp#!/dataset/insitu-observations-surface-land?tab=overview
 
     Args:
         year (str or list): year(s) to download
         month (str or list): month(s) to download
@@ -118,15 +118,15 @@
         print(f'ERROR: path "{target_path}" does not exist')
         return False
 
     c = cdsapi.Client()
     c.retrieve(
         'insitu-observations-surface-land',
         {
-            'time_aggregation': 'sub_daily',
+            'time_aggregation': product,
             'variable': [
                 'air_pressure', 'air_pressure_at_sea_level', 'air_temperature',
                 'dew_point_temperature', 'wind_from_direction', 'wind_speed'
             ],
             'usage_restrictions': 'restricted',
             'data_quality': 'passed',
             'year': years,
```

### Comparing `topopyscale-0.2.2/TopoPyScale/topo_param.py` & `topopyscale-0.2.3/TopoPyScale/topo_param.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             da_idw = xr.DataArray(data=weights,
                                   coords={
                                     "y": ds_param_pt.y.values,
                                     "x": ds_param_pt.x.values,
                               },
                               dims=["y", "x"]
                               )
-            dw = xr.core.weighted.DatasetWeighted(ds_param_pt, da_idw)
+            dw = xr.Dataset.weighted(ds_param_pt, da_idw)
             d_mini = dw.sum(['x', 'y'], keep_attrs=True)
             df_pts.loc[i, ['elevation', 'slope', 'aspect', 'aspect_cos', 'aspect_sin', 'svf']] = np.array((d_mini.elevation.values,
                                                                                                    d_mini.slope.values,
                                                                                                    d_mini.aspect.values,
                                                                                                    d_mini.aspect_cos,
                                                                                                    d_mini.aspect_sin,
                                                                                                  d_mini.svf.values))
```

### Comparing `topopyscale-0.2.2/TopoPyScale/topo_plot.py` & `topopyscale-0.2.3/TopoPyScale/topo_plot.py`

 * *Files identical despite different names*

### Comparing `topopyscale-0.2.2/TopoPyScale/topo_scale.py` & `topopyscale-0.2.3/TopoPyScale/topo_scale.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,74 +37,42 @@
 import pdb
 
 import pandas as pd
 import xarray as xr
 from pyproj import Transformer
 import numpy as np
 import sys, time
+import datetime as dt
 from TopoPyScale import meteo_util as mu
-from multiprocessing import Pool
-from multiprocessing.dummy import Pool as ThreadPool
-import multiprocessing as mproc
+from TopoPyScale import topo_utils as tu
+
 import os, glob
+from pathlib import Path
+from typing import Union
+
 
 # Physical constants
-g = 9.81    #  Acceleration of gravity [ms^-1]
-R = 287.05  #  Gas constant for dry air [JK^-1kg^-1]
+g = 9.81  # Acceleration of gravity [ms^-1]
+R = 287.05  # Gas constant for dry air [JK^-1kg^-1]
 
-def multicore_pooling(fun, fun_param, n_cores):
-    '''
-    Function to perform multiprocessing on n_cores
-    Args:
-        fun (obj): function to distribute
-        fun_param zip(list): zip list of functino arguments
-        n_core (int): number o cores
-    '''
-    if n_cores is None:
-        n_cores = mproc.cpu_count() - 2
-        print(f'WARNING: number of cores to use not provided. By default {n_cores} cores will be used')
-    elif n_cores > mproc.cpu_count():
-        n_cores = mproc.cpu_count() - 2
-        print(f'WARNING: Only {mproc.cpu_count()} cores available on this machine, reducing n_cores to {n_cores} ')
-
-    # make sure it will run on one core at least
-    if n_cores == 0:
-        n_cores = 1
-
-
-    pool = Pool(n_cores)
-    pool.starmap(fun, fun_param)
-    pool.close()
-    pool.join()
-    pool = None
-
-def multithread_pooling(fun, fun_param, n_threads):
-    '''
-    Function to perform multiprocessing on n_threads
-    Args:
-        fun (obj): function to distribute
-        fun_param zip(list): zip list of functino arguments
-        n_core (int): number of threads
-    '''
-    tpool = ThreadPool(n_threads)
-    tpool.starmap(fun, fun_param)
-    tpool.close()
-    tpool.join()
-    tpool = None
-
-def clear_files(path):
-    # Clear outputs/tmp/ folder
-    for dirpath, dirnames, filenames in os.walk(path):
-        # Remove regular files, ignore directories
-        for filename in filenames:
-            os.unlink(os.path.join(dirpath, filename))
-        print(f'{path} cleaned')
+
+
+def clear_files(path: Union[Path, str]):
+    if not isinstance(path, Path):
+        path = Path(path)
+
+    files = [f for f in path.rglob('*') if f.is_file()]
+    for file in files:
+        file.unlink()
+    print(f'{path} cleaned')
 
 
 def downscale_climate(project_directory,
+                      climate_directory,
+                      downscaled_directory,
                       df_centroids,
                       horizon_da,
                       ds_solar,
                       target_EPSG,
                       start_date,
                       end_date,
                       interp_method='idw',
@@ -140,24 +108,20 @@
     start_time = time.time()
     tstep_dict = {'1H': 1, '3H': 3, '6H': 6}
     n_digits = len(str(df_centroids.index.max()))
 
     # =========== Open dataset with Dask =================
     tvec = pd.date_range(start_date, pd.to_datetime(end_date) + pd.to_timedelta('1D'), freq=tstep, inclusive='left')
 
-    flist_PLEV = (f'{project_directory}inputs/climate/PLEV*.nc')
-    flist_SURF = (f'{project_directory}inputs/climate/SURF*.nc')
-
+    flist_PLEV = glob.glob(f'{climate_directory}/PLEV*.nc')
+    flist_SURF = glob.glob(f'{climate_directory}/SURF*.nc')
 
     def _open_dataset_climate(flist):
-    
-
-        ds_ = xr.open_mfdataset(flist, parallel=True)
-
 
+        ds_ = xr.open_mfdataset(flist, parallel=False, concat_dim="time", combine='nested', coords='minimal')
 
         # this block handles the expver dimension that is in downloaded ERA5 data if data is ERA5/ERA5T mix. If only ERA5 or
         # only ERA5T it is not present. ERA5T data can be present in the timewindow T-5days to T -3months, where T is today.
         # https://code.mpimet.mpg.de/boards/1/topics/8961
         # https://confluence.ecmwf.int/display/CUSF/ERA5+CDS+requests+which+return+a+mixture+of+ERA5+and+ERA5T+data
         try:
             # in case of there being an expver dimension and it has two or more values, select first value
@@ -172,23 +136,25 @@
         return ds_
 
     def _subset_climate_dataset(ds_, row, type='plev', pt_id=0):
         print('Preparing {} for point {}'.format(type, row.name))
         # =========== Extract the 3*3 cells centered on a given point ============
         ind_lat = np.abs(ds_.latitude - row.lat).argmin()
         ind_lon = np.abs(ds_.longitude - row.lon).argmin()
-        #from remote_pdb import set_trace
-        #set_trace()
-        ds_tmp = ds_.isel(latitude=[ind_lat-1, ind_lat, ind_lat+1], longitude=[ind_lon-1, ind_lon, ind_lon+1]).copy()
+        # from remote_pdb import set_trace
+        # set_trace()
+        ds_tmp = ds_.isel(latitude=[ind_lat - 1, ind_lat, ind_lat + 1],
+                          longitude=[ind_lon - 1, ind_lon, ind_lon + 1]).copy()
         # convert geopotential height to elevation (in m), normalizing by g
-        ds_tmp['z'] = ds_tmp.z/g
+        ds_tmp['z'] = ds_tmp.z / g
 
         comp = dict(zlib=True, complevel=5)
         encoding = {var: comp for var in ds_tmp.data_vars}
-        ds_tmp.to_netcdf(f'{project_directory}outputs/tmp/ds_{type}_pt_{pt_id}.nc', engine='h5netcdf', encoding=encoding)
+        ds_tmp.to_netcdf(f'{project_directory}outputs/tmp/ds_{type}_pt_{pt_id}.nc', engine='h5netcdf',
+                         encoding=encoding)
         ds_ = None
         ds_tmp = None
 
     ds_plev = _open_dataset_climate(flist_PLEV).sel(time=tvec.values)
     # Check tvec is within time period of ds_plev.time or return error
     if ds_plev.time.min() > tvec.min():
         print(f'ERROR: start date {tvec[0].strftime(format="%Y-%m-%d")} not covered in climate forcing.')
@@ -201,25 +167,27 @@
 
     row_list = []
     ds_list = []
     for _, row in df_centroids.iterrows():
         row_list.append(row)
         ds_list.append(ds_plev)
 
-    fun_param = zip(ds_list, row_list,  ['plev'] * len(row_list), df_centroids.index.values) # construct here the tuple that goes into the pooling for arguments
-    multithread_pooling(_subset_climate_dataset, fun_param, n_threads=n_core)
+    fun_param = zip(ds_list, row_list, ['plev'] * len(row_list),
+                    df_centroids.index.values)  # construct here the tuple that goes into the pooling for arguments
+    tu.multithread_pooling(_subset_climate_dataset, fun_param, n_threads=n_core)
     fun_param = None
     ds_plev = None
     ds_surf = _open_dataset_climate(flist_SURF).sel(time=tvec.values)
     ds_list = []
     for _, row in df_centroids.iterrows():
         ds_list.append(ds_surf)
 
-    fun_param = zip(ds_list, row_list, ['surf']*len(row_list), range(0,len(row_list))) # construct here the tuple that goes into the pooling for arguments
-    multithread_pooling(_subset_climate_dataset, fun_param, n_threads=n_core)
+    fun_param = zip(ds_list, row_list, ['surf'] * len(row_list),
+                    range(0, len(row_list)))  # construct here the tuple that goes into the pooling for arguments
+    tu.multithread_pooling(_subset_climate_dataset, fun_param, n_threads=n_core)
     fun_param = None
     ds_surf = None
 
     # Preparing list to feed into Pooling
     surf_pt_list = []
     plev_pt_list = []
     ds_solar_list = []
@@ -228,298 +196,310 @@
     meta_list = []
     for i, row in df_centroids.iterrows():
         surf_pt_list.append(xr.open_dataset(f'{project_directory}outputs/tmp/ds_surf_pt_{i}.nc', engine='h5netcdf'))
         plev_pt_list.append(xr.open_dataset(f'{project_directory}outputs/tmp/ds_plev_pt_{i}.nc', engine='h5netcdf'))
         ds_solar_list.append(ds_solar.sel(point_id=row.name))
         horizon_da_list.append(horizon_da)
         row_list.append(row)
-        meta_list.append({'interp_method':interp_method,
-                          'lw_terrain_flag':lw_terrain_flag,
-                          'tstep':tstep_dict.get(tstep),
-                          'n_digits':n_digits,
-                          'file_pattern':file_pattern})
+        meta_list.append({'interp_method': interp_method,
+                          'lw_terrain_flag': lw_terrain_flag,
+                          'tstep': tstep_dict.get(tstep),
+                          'n_digits': n_digits,
+                          'file_pattern': file_pattern})
 
     def pt_downscale_interp(row, ds_plev_pt, ds_surf_pt, meta):
-        pt_id = np.int32(row.point_id)
-        print(f'Downscaling t,q,p,tp,ws,wd for point: {pt_id+1}')
+        pt_id = row.point_id
+        print(f'Downscaling t,q,p,tp,ws, wd for point: {pt_id}')
 
         # ====== Horizontal interpolation ====================
         interp_method = meta.get('interp_method')
-        n_digits = meta.get('n_digits')
 
         # convert gridcells coordinates from WGS84 to DEM projection
         lons, lats = np.meshgrid(ds_plev_pt.longitude.values, ds_plev_pt.latitude.values)
         trans = Transformer.from_crs("epsg:4326", "epsg:" + str(target_EPSG), always_xy=True)
         Xs, Ys = trans.transform(lons.flatten(), lats.flatten())
         Xs = Xs.reshape(lons.shape)
         Ys = Ys.reshape(lons.shape)
 
-        dist = np.sqrt((row.x - Xs)**2 + (row.y - Ys)**2)
+        dist = np.sqrt((row.x - Xs) ** 2 + (row.y - Ys) ** 2)
         if interp_method == 'idw':
-            idw = 1/(dist**2)
+            idw = 1 / (dist ** 2)
             weights = idw / np.sum(idw)  # normalize idw to sum(idw) = 1
         elif interp_method == 'linear':
             weights = dist / np.sum(dist)
         else:
             sys.exit('ERROR: interpolation method not available')
 
         # create a dataArray of weights to then propagate through the dataset
-        da_idw = xr.DataArray(data = weights,
+        da_idw = xr.DataArray(data=weights,
                               coords={
                                   "latitude": ds_plev_pt.latitude.values,
                                   "longitude": ds_plev_pt.longitude.values,
                               },
                               dims=["latitude", "longitude"]
                               )
         dw = xr.Dataset.weighted(ds_plev_pt, da_idw)
-        plev_interp = dw.sum(['longitude', 'latitude'], keep_attrs=True)    # compute horizontal inverse weighted horizontal interpolation
+        plev_interp = dw.sum(['longitude', 'latitude'],
+                             keep_attrs=True)  # compute horizontal inverse weighted horizontal interpolation
         dww = xr.Dataset.weighted(ds_surf_pt, da_idw)
-        surf_interp = dww.sum(['longitude', 'latitude'], keep_attrs=True)    # compute horizontal inverse weighted horizontal interpolation
+        surf_interp = dww.sum(['longitude', 'latitude'],
+                              keep_attrs=True)  # compute horizontal inverse weighted horizontal interpolation
 
         # ========= Converting z from [m**2 s**-2] to [m] asl =======
-        #plev_interp.z.values = plev_interp.z.values / g
-        #plev_interp.z.attrs = {'units': 'm', 'standard_name': 'Elevation', 'Long_name': 'Elevation of plevel'}
+        # plev_interp.z.values = plev_interp.z.values / g
+        # plev_interp.z.attrs = {'units': 'm', 'standard_name': 'Elevation', 'Long_name': 'Elevation of plevel'}
 
-        #surf_interp.z.values = surf_interp.z.values / g  # convert geopotential height to elevation (in m), normalizing by g
-        #surf_interp.z.attrs = {'units': 'm', 'standard_name': 'Elevation', 'Long_name': 'Elevation of ERA5 surface'}
+        # surf_interp.z.values = surf_interp.z.values / g  # convert geopotential height to elevation (in m), normalizing by g
+        # surf_interp.z.attrs = {'units': 'm', 'standard_name': 'Elevation', 'Long_name': 'Elevation of ERA5 surface'}
 
         # ============ Extract specific humidity (q) for both dataset ============
         surf_interp = mu.dewT_2_q_magnus(surf_interp, mu.var_era_surf)
         plev_interp = mu.t_rh_2_dewT(plev_interp, mu.var_era_plevel)
 
         down_pt = xr.Dataset(coords={
-                'time': plev_interp.time,
-                'point_id': pt_id
-            })
+            'time': plev_interp.time,
+            'point_id': pd.to_numeric(pt_id, errors='ignore')
+        })
 
         if (row.elevation < plev_interp.z.isel(level=-1)).sum():
             print("---> WARNING: Point {} is {} m lower than the {} hPa geopotential\n=> "
                   "Values sampled from Psurf and lowest Plevel. No vertical interpolation".
                   format(i,
-                         np.round(np.min(row.elevation - plev_interp.z.isel(level=-1).values),0),
+                         np.round(np.min(row.elevation - plev_interp.z.isel(level=-1).values), 0),
                          plev_interp.isel(level=-1).level.data))
             ind_z_top = (plev_interp.where(plev_interp.z > row.elevation).z - row.elevation).argmin('level')
             top = plev_interp.isel(level=ind_z_top)
 
             down_pt['t'] = top['t']
             down_pt['u'] = top.u
             down_pt['v'] = top.v
             down_pt['q'] = top.q
-            down_pt['p'] = top.level*(10**2) * np.exp(-(row.elevation-top.z) / (0.5 * (top.t + down_pt.t) * R / g))  # Pressure in bar
+            down_pt['p'] = top.level * (10 ** 2) * np.exp(
+                -(row.elevation - top.z) / (0.5 * (top.t + down_pt.t) * R / g))  # Pressure in bar
 
         else:
             # ========== Vertical interpolation at the DEM surface z  ===============
             ind_z_bot = (plev_interp.where(plev_interp.z < row.elevation).z - row.elevation).argmax('level')
 
             # In case upper pressure level elevation is not high enough, stop process and print error
             try:
                 ind_z_top = (plev_interp.where(plev_interp.z > row.elevation).z - row.elevation).argmin('level')
             except:
-                print(f'ERROR: Upper pressure level {plev_interp.level.min().values} hPa geopotential is lower than cluster mean elevation')
+                print(
+                    f'ERROR: Upper pressure level {plev_interp.level.min().values} hPa geopotential is lower than cluster mean elevation')
 
             top = plev_interp.isel(level=ind_z_top)
             bot = plev_interp.isel(level=ind_z_bot)
 
             # Preparing interpolation weights for linear interpolation =======================
             dist = np.array([np.abs(bot.z - row.elevation).values, np.abs(top.z - row.elevation).values])
-            #idw = 1/dist**2
-            #weights = idw / np.sum(idw, axis=0)
+            # idw = 1/dist**2
+            # weights = idw / np.sum(idw, axis=0)
             weights = dist / np.sum(dist, axis=0)
 
             # ============ Creating a dataset containing the downscaled timeseries ========================
             down_pt['t'] = bot.t * weights[1] + top.t * weights[0]
             down_pt['u'] = bot.u * weights[1] + top.u * weights[0]
             down_pt['v'] = bot.v * weights[1] + top.v * weights[0]
             down_pt['q'] = bot.q * weights[1] + top.q * weights[0]
-            down_pt['p'] = top.level*(10**2) * np.exp(-(row.elevation-top.z) / (0.5 * (top.t + down_pt.t) * R / g))  # Pressure in bar
+            down_pt['p'] = top.level * (10 ** 2) * np.exp(
+                -(row.elevation - top.z) / (0.5 * (top.t + down_pt.t) * R / g))  # Pressure in bar
 
         # ======= logic  to compute ws, wd without loading data in memory, and maintaining the power of dask
         down_pt['month'] = ('time', down_pt.time.dt.month.data)
         if precip_lapse_rate_flag:
             monthly_coeffs = xr.Dataset(
                 {
                     'coef': (['month'], [0.35, 0.35, 0.35, 0.3, 0.25, 0.2, 0.2, 0.2, 0.2, 0.25, 0.3, 0.35])
                 },
-                coords={'month': [1,2,3,4,5,6,7,8,9,10,11,12]}
+                coords={'month': [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]}
             )
-            down_pt['precip_lapse_rate'] = (1 + monthly_coeffs.coef.sel(month=down_pt.month.values).data * (row.elevation - surf_interp.z) * 1e-3) / \
-                                           (1 - monthly_coeffs.coef.sel(month=down_pt.month.values).data * (row.elevation - surf_interp.z) * 1e-3)
+            down_pt['precip_lapse_rate'] = (1 + monthly_coeffs.coef.sel(month=down_pt.month.values).data * (
+                    row.elevation - surf_interp.z) * 1e-3) / \
+                                           (1 - monthly_coeffs.coef.sel(month=down_pt.month.values).data * (
+                                                   row.elevation - surf_interp.z) * 1e-3)
         else:
             down_pt['precip_lapse_rate'] = down_pt.t * 0 + 1
 
-        down_pt['tp'] = down_pt.precip_lapse_rate * surf_interp.tp  * 1 / meta.get('tstep') * 10**3 # Convert to mm/hr
+        down_pt['tp'] = down_pt.precip_lapse_rate * surf_interp.tp * 1 / meta.get('tstep') * 10 ** 3  # Convert to mm/hr
         down_pt['theta'] = np.arctan2(-down_pt.u, -down_pt.v)
         down_pt['theta_neg'] = (down_pt.theta < 0) * (down_pt.theta + 2 * np.pi)
         down_pt['theta_pos'] = (down_pt.theta >= 0) * down_pt.theta
         down_pt = down_pt.drop('theta')
         down_pt['wd'] = (down_pt.theta_pos + down_pt.theta_neg)  # direction in Rad
-        down_pt['ws'] = np.sqrt(down_pt.u ** 2 + down_pt.v**2)
+        down_pt['ws'] = np.sqrt(down_pt.u ** 2 + down_pt.v ** 2)
         down_pt = down_pt.drop(['theta_pos', 'theta_neg', 'month'])
 
         down_pt.t.attrs = {'units': 'K', 'long_name': 'Temperature', 'standard_name': 'air_temperature'}
         down_pt.q.attrs = {'units': 'kg kg**-1', 'long_name': 'Specific humidity', 'standard_name': 'specific_humidity'}
         down_pt.u.attrs = {'units': 'm s**-1', 'long_name': 'U component of wind', 'standard_name': 'eastward_wind'}
         down_pt.v.attrs = {'units': 'm s**-1', 'long_name': 'V component of wind', 'standard_name': 'northward wind'}
         down_pt.p.attrs = {'units': 'bar', 'long_name': 'Pression atmospheric', 'standard_name': 'pression_atmospheric'}
 
         down_pt.ws.attrs = {'units': 'm s**-1', 'long_name': 'Wind speed', 'standard_name': 'wind_speed'}
         down_pt.wd.attrs = {'units': 'deg', 'long_name': 'Wind direction', 'standard_name': 'wind_direction'}
         down_pt.tp.attrs = {'units': 'mm hr**-1', 'long_name': 'Precipitation', 'standard_name': 'precipitation'}
-        down_pt.precip_lapse_rate.attrs = {'units': 'mm hr**-1', 'long_name': 'Precipitation after lapse-rate correction', 'standard_name': 'precipitation_after_lapse-rate_correction'}
+        down_pt.precip_lapse_rate.attrs = {'units': 'mm hr**-1',
+                                           'long_name': 'Precipitation after lapse-rate correction',
+                                           'standard_name': 'precipitation_after_lapse-rate_correction'}
+
+        down_pt.attrs = {'title':'Downscale point using TopoPyScale',
+                          'date_created':dt.datetime.now().strftime('%Y/%m/%d %H:%M:%S')}
 
         print(f'---> Storing point {pt_id} to outputs/tmp/')
 
         comp = dict(zlib=True, complevel=5)
         encoding = {var: comp for var in down_pt.data_vars}
-        down_pt.to_netcdf(project_directory + 'outputs/tmp/down_pt_{}.nc'.format(str(pt_id).zfill(n_digits)), engine='h5netcdf', encoding=encoding)
+        down_pt.to_netcdf(project_directory + f'outputs/tmp/down_pt_{pt_id}.nc',
+                          engine='h5netcdf', encoding=encoding)
 
         comp = dict(zlib=True, complevel=5)
         encoding = {var: comp for var in surf_interp.data_vars}
-        surf_interp.to_netcdf(project_directory + 'outputs/tmp/surf_interp_{}.nc'.format(str(pt_id).zfill(n_digits)), engine='h5netcdf', encoding=encoding)
+        surf_interp.to_netcdf(project_directory + f'outputs/tmp/surf_interp_{pt_id}.nc',
+                              engine='h5netcdf', encoding=encoding)
         down_pt = None
         surf_interp = None
         top, bot = None, None
 
-    fun_param = zip(row_list, plev_pt_list, surf_pt_list, meta_list) # construct here the tuple that goes into the pooling for arguments
-    multicore_pooling(pt_downscale_interp, fun_param, n_core)
+    fun_param = zip(row_list, plev_pt_list, surf_pt_list,
+                    meta_list)  # construct here the tuple that goes into the pooling for arguments
+    tu.multicore_pooling(pt_downscale_interp, fun_param, n_core)
     fun_param = None
     plev_pt_list = None
     surf_pt_list = None
 
-
     def pt_downscale_radiations(row, ds_solar, horizon_da, meta):
         # insrt here downscaling routine for sw and lw
         # save file final file
-        pt_id = np.int32(row.point_id)
-        n_digits = meta.get('n_digits')
+        pt_id = row.point_id
         file_pattern = meta.get('file_pattern')
-        print(f'Downscaling LW, SW for point: {pt_id+1}')
-
-        down_pt = xr.open_dataset('{}outputs/tmp/down_pt_{}.nc'.format(project_directory, str(pt_id).zfill(n_digits)), engine='h5netcdf')
-        surf_interp = xr.open_dataset('{}outputs/tmp/surf_interp_{}.nc'.format(project_directory, str(pt_id).zfill(n_digits)), engine='h5netcdf')
+        print(f'Downscaling LW, SW for point: {pt_id}')
 
+        down_pt = xr.open_dataset(f'{project_directory}outputs/tmp/down_pt_{pt_id}.nc',
+                                  engine='h5netcdf')
+        surf_interp = xr.open_dataset(
+            f'{project_directory}outputs/tmp/surf_interp_{pt_id}.nc', engine='h5netcdf')
 
         # ======== Longwave downward radiation ===============
         x1, x2 = 0.43, 5.7
         sbc = 5.67e-8
 
         down_pt = mu.mixing_ratio(down_pt, mu.var_era_plevel)
         down_pt = mu.vapor_pressure(down_pt, mu.var_era_plevel)
         surf_interp = mu.mixing_ratio(surf_interp, mu.var_era_surf)
         surf_interp = mu.vapor_pressure(surf_interp, mu.var_era_surf)
 
         # ========= Compute clear sky emissivity ===============
         down_pt['cse'] = 0.23 + x1 * (down_pt.vp / down_pt.t) ** (1 / x2)
         surf_interp['cse'] = 0.23 + x1 * (surf_interp.vp / surf_interp.t2m) ** (1 / x2)
         # Calculate the "cloud" emissivity, UNIT OF STRD (J/m2)
-        surf_interp['cle'] = (surf_interp.strd/pd.Timedelta('1H').seconds) / (sbc * surf_interp.t2m**4) - surf_interp['cse']
+        surf_interp['cle'] = (surf_interp.strd / pd.Timedelta('1H').seconds) / (sbc * surf_interp.t2m ** 4) - \
+                             surf_interp['cse']
         # Use the former cloud emissivity to compute the all sky emissivity at subgrid.
         surf_interp['aef'] = down_pt['cse'] + surf_interp['cle']
         if lw_terrain_flag:
             down_pt['LW'] = row.svf * surf_interp['aef'] * sbc * down_pt.t ** 4 + \
-                            0.5 * (1 + np.cos(row.slope)) * (1 - row.svf) * 0.99 * 5.67e-8 * (273.15**4)
+                            0.5 * (1 + np.cos(row.slope)) * (1 - row.svf) * 0.99 * 5.67e-8 * (273.15 ** 4)
         else:
             down_pt['LW'] = row.svf * surf_interp['aef'] * sbc * down_pt.t ** 4
 
         kt = surf_interp.ssrd * 0
-        sunset = ds_solar.sunset.astype(bool)
+        sunset = ds_solar.sunset.astype(bool).compute()
         mu0 = ds_solar.mu0
         SWtoa = ds_solar.SWtoa
 
-
-        #pdb.set_trace()
-        kt[~sunset] = (surf_interp.ssrd[~sunset]/pd.Timedelta('1H').seconds) / SWtoa[~sunset]     # clearness index
+        # pdb.set_trace()
+        kt[~sunset] = (surf_interp.ssrd[~sunset] / pd.Timedelta('1H').seconds) / SWtoa[~sunset]  # clearness index
         kt[kt < 0] = 0
         kt[kt > 1] = 1
-        kd = 0.952 - 1.041 * np.exp(-1 * np.exp(2.3 - 4.702 * kt))    # Diffuse index
+        kd = 0.952 - 1.041 * np.exp(-1 * np.exp(2.3 - 4.702 * kt))  # Diffuse index
 
-        surf_interp['SW'] = surf_interp.ssrd/pd.Timedelta('1H').seconds
+        surf_interp['SW'] = surf_interp.ssrd / pd.Timedelta('1H').seconds
         surf_interp['SW'][surf_interp['SW'] < 0] = 0
         surf_interp['SW_diffuse'] = kd * surf_interp.SW
         down_pt['SW_diffuse'] = row.svf * surf_interp.SW_diffuse
 
         surf_interp['SW_direct'] = surf_interp.SW - surf_interp.SW_diffuse
         # scale direct solar radiation using Beer's law (see Aalstad 2019, Appendix A)
         ka = surf_interp.ssrd * 0
-        #pdb.set_trace()
-        ka[~sunset] = (g * mu0[~sunset]/down_pt.p)*np.log(SWtoa[~sunset]/surf_interp.SW_direct[~sunset])
+        # pdb.set_trace()
+        ka[~sunset] = (g * mu0[~sunset] / down_pt.p) * np.log(SWtoa[~sunset] / surf_interp.SW_direct[~sunset])
         # Illumination angle
-        down_pt['cos_illumination_tmp'] = mu0 * np.cos(row.slope) + np.sin(ds_solar.zenith) *\
+        down_pt['cos_illumination_tmp'] = mu0 * np.cos(row.slope) + np.sin(ds_solar.zenith) * \
                                           np.sin(row.slope) * np.cos(ds_solar.azimuth - row.aspect)
-        down_pt['cos_illumination'] = down_pt.cos_illumination_tmp * (down_pt.cos_illumination_tmp > 0)  # remove selfdowing ccuring when |Solar.azi - aspect| > 90
+        down_pt['cos_illumination'] = down_pt.cos_illumination_tmp * (
+                down_pt.cos_illumination_tmp > 0)  # remove selfdowing ccuring when |Solar.azi - aspect| > 90
         down_pt = down_pt.drop(['cos_illumination_tmp'])
-        down_pt['cos_illumination'][down_pt['cos_illumination'] < 0 ] =0
+        illumination_mask = down_pt['cos_illumination'] < 0
+        illumination_mask = illumination_mask.compute()
+        down_pt['cos_illumination'][illumination_mask] = 0
 
         # Binary shadow masks.
         horizon = horizon_da.sel(x=row.x, y=row.y, azimuth=np.rad2deg(ds_solar.azimuth), method='nearest')
         shade = (horizon > ds_solar.elevation)
         down_pt['SW_direct_tmp'] = down_pt.t * 0
-        down_pt['SW_direct_tmp'][~sunset] = SWtoa[~sunset] * np.exp(-ka[~sunset] * down_pt.p[~sunset] / (g * mu0[~sunset]))
+        down_pt['SW_direct_tmp'][~sunset] = SWtoa[~sunset] * np.exp(
+            -ka[~sunset] * down_pt.p[~sunset] / (g * mu0[~sunset]))
         down_pt['SW_direct'] = down_pt.t * 0
-        down_pt['SW_direct'][~sunset] = down_pt.SW_direct_tmp[~sunset] * (down_pt.cos_illumination[~sunset] / mu0[~sunset]) * (1 - shade)
+        down_pt['SW_direct'][~sunset] = down_pt.SW_direct_tmp[~sunset] * (
+                down_pt.cos_illumination[~sunset] / mu0[~sunset]) * (1 - shade)
         down_pt['SW'] = down_pt.SW_diffuse + down_pt.SW_direct
 
         # currently drop azimuth and level as they are coords. Could be passed to variables instead.
         # round(5) required to sufficiently represent specific humidty, q (eg typical value 0.00078)
         down_pt = down_pt.drop(['level']).round(5)
 
         # adding metadata
-        down_pt.LW.attrs = {'units': 'W m**-2', 'long_name': 'Surface longwave radiation downwards','standard_name': 'longwave_radiation_downward'}
+        down_pt.LW.attrs = {'units': 'W m**-2', 'long_name': 'Surface longwave radiation downwards',
+                            'standard_name': 'longwave_radiation_downward'}
         down_pt.cse.attrs = {'units': 'xxx', 'standard_name': 'Clear sky emissivity'}
         down_pt = down_pt.drop(['SW_direct_tmp'])
-        down_pt.SW.attrs = {'units': 'W m**-2', 'long_name': 'Surface solar radiation downwards', 'standard_name': 'shortwave_radiation_downward'}
-        down_pt.SW_diffuse.attrs = {'units': 'W m**-2', 'long_name': 'Surface solar diffuse radiation downwards', 'standard_name': 'shortwave_diffuse_radiation_downward'}
+        down_pt.SW.attrs = {'units': 'W m**-2', 'long_name': 'Surface solar radiation downwards',
+                            'standard_name': 'shortwave_radiation_downward'}
+        down_pt.SW_diffuse.attrs = {'units': 'W m**-2', 'long_name': 'Surface solar diffuse radiation downwards',
+                                    'standard_name': 'shortwave_diffuse_radiation_downward'}
+        ver_dict = tu.get_versionning()
+        down_pt.attrs = {'title': 'Downscaled timeseries with TopoPyScale',
+                         'created with': 'TopoPyScale, see more at https://topopyscale.readthedocs.io',
+                          'package_version':ver_dict.get('package_version'),
+                          'git_commit': ver_dict.get('git_commit'),
+                         'url_TopoPyScale': 'https://github.com/ArcticSnow/TopoPyScale',
+                         'date_created': dt.datetime.now().strftime('%Y/%m/%d %H:%M:%S')}
 
-        num = str(pt_id).zfill(n_digits)
         comp = dict(zlib=True, complevel=5)
         encoding = {var: comp for var in down_pt.data_vars}
-        down_pt.to_netcdf(f'{project_directory}outputs/downscaled/{file_pattern.split("*")[0]}{num}{file_pattern.split("*")[1]}', engine='h5netcdf', encoding=encoding, mode='a')
-
+        down_pt.to_netcdf(f'{downscaled_directory}/{file_pattern.replace("*", pt_id)}',
+                          engine='h5netcdf', encoding=encoding, mode='a')
         # Clear memory
         down_pt, surf_interp = None, None
         ds_solar = None
-        kt , ka, kd, sunset = None, None, None, None
+        kt, ka, kd, sunset = None, None, None, None
         sunset = None
         horizon = None
         shade = None
 
-    fun_param = zip(row_list, ds_solar_list, horizon_da_list, meta_list)  # construct here tuple to feed pool function's argument
-    multicore_pooling(pt_downscale_radiations, fun_param, n_core)
+    fun_param = zip(row_list, ds_solar_list, horizon_da_list,
+                    meta_list)  # construct here tuple to feed pool function's argument
+    tu.multicore_pooling(pt_downscale_radiations, fun_param, n_core)
     fun_param = None
     ds_solar_list = None
     horizon_da_list = None
 
-    #clear_files(f'{project_directory}outputs/tmp')
+    # clear_files(f'{project_directory}outputs/tmp')
 
     # print timer to console
-    print('---> Downscaling finished in {}s'.format(np.round(time.time()-start_time), 1))
+    print('---> Downscaling finished in {}s'.format(np.round(time.time() - start_time), 1))
 
 
 def read_downscaled(path='outputs/down_pt*.nc'):
     """
     Function to read downscaled points saved into netcdf files into one single dataset using Dask
 
     Args:
         path (str): path and pattern to use into xr.open_mfdataset
 
     Returns:
         dataset: merged dataset readily to use and loaded in chuncks via Dask
     """
-    flist = glob.glob(path)
-    flist.sort()
 
-    ds_list = []
-    for file in flist:
-       ds_list.append(xr.open_dataset(file))
-    down_pts = xr.concat(ds_list, dim='point_id')
+    down_pts = xr.open_mfdataset(path, concat_dim='point_id', combine='nested', parallel=False)
     return down_pts
-
-
-
-
-
-
-
-
-
-
-
```

### Comparing `topopyscale-0.2.2/TopoPyScale/topo_sim.py` & `topopyscale-0.2.3/TopoPyScale/topo_sim.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 from matplotlib import pyplot as plt
 import xarray as xr
 #from TopoPyScale import topo_da as da
 import matplotlib.pyplot as plt
 from datetime import datetime
 from matplotlib.backends.backend_pdf import PdfPages
 import datetime as dt
+from TopoPyScale import topo_utils as tu
+from TopoPyScale import topo_export as te
+
 def fsm_nlst(nconfig, metfile, nave):
     """
     Function to generate namelist parameter file that is required to run the FSM model.
     https://github.com/RichardEssery/FSM
 
     Args:
         nconfig (int): which FSm configuration to run (integer 1-31)
@@ -106,23 +109,93 @@
             "point_id": point_id,
             "time": df.index,
             "reference_time": pd.Timestamp(df.index[0])
         })
 
     return ds
 
+
+def to_netcdf(fname_fsm_sim, complevel=9):
+    '''
+    Function to convert a single FSM simulation output file (.txt) to a compressed netcdf file (.nc)
+
+    Args:
+        fname_fsm_sim(str): filename to convert from txt to nc
+        complevel (int): Compression level. 1-9
+
+    Returns:
+        NULL (FSM simulation file written to disk)
+    '''
+    ver_dict = tu.get_versionning()
+
+    ds = txt2ds(fname_fsm_sim)
+    ds.albedo.attrs = {'units':'ratio', 'standard_name':'albedo', 'long_name':'Surface Effective Albedo', '_FillValue': -9999999.0}
+    ds.runoff.attrs = {'units':'kg m-2', 'standard_name':'runoff', 'long_name':'Cumulated runoff from snow', '_FillValue': -9999999.0}
+    ds.snd.attrs = {'units':'m', 'standard_name':'snd', 'long_name':'Average snow depth', '_FillValue': -9999999.0}
+    ds.swe.attrs = {'units':'kg m-2', 'standard_name':'swe', 'long_name':'Average snow water equivalent', '_FillValue': -9999999.0}
+    ds.t_surface.attrs = {'units':'°C', 'standard_name':'t_surface', 'long_name':'Average surface temperature', '_FillValue': -9999999.0}
+    ds.t_surface.attrs = {'units':'°C', 'standard_name':'t_soil', 'long_name':'Average soil temperature at 20 cm depth', '_FillValue': -9999999.0}
+    ds.attrs = {'title':'FSM simulation outputs',
+                'source': 'Data downscaled with TopoPyScale and simulated with FSM',
+                'package_version':ver_dict.get('package_version'),
+                'url_TopoPyScale': 'https://github.com/ArcticSnow/TopoPyScale',
+                'url_FSM': 'https://github.com/RichardEssery/FSM',
+                'git_commit': ver_dict.get('git_commit'),
+                'date_created':dt.datetime.now().strftime('%Y/%m/%d %H:%M:%S')}
+    fout = f"{fname_fsm_sim[:-4]}.nc"
+    te.to_netcdf(ds, fout, complevel=complevel)
+    print(f"File {fout} saved")
+
+
+def to_netcdf_parallel(fsm_sims='./fsm_sims/sim_FSM*.txt',
+                       n_core=6,
+                       complevel=9,
+                       delete_txt_files=False):
+    '''
+    Function to convert FSM simulation output (.txt files) to compressed netcdf. This function parallelize jobs on n_core
+
+    Args:
+        fsm_sims (str or list): file pattern or list of file output of FSM. Note that must be in short relative path!. Default = 'fsm_sims/sim_FSM_pt*.txt'
+        n_core (int): number of cores. Default = 6:
+        complevel (int): Compression level. 1-9
+        delete_txt_files (bool): delete simulation txt files or not. Default=True
+
+    Returns:
+        NULL (FSM simulation file written to disk)
+    '''
+    print('---> Run FSM simulation in parallel')
+    # 1. create all nlsit_files
+    if isinstance(fsm_sims, str):
+        flist = glob.glob(fsm_sims)
+    elif isinstance(fsm_sims, list):
+        flist = fsm_sims
+    else:
+        print('ERROR: fsm_input must either be a list of file path or a string of file pattern')
+        return
+
+    fun_param = zip(flist, [complevel]*len(flist))
+    tu.multicore_pooling(to_netcdf, fun_param, n_core)
+    print('---> All FSM simulations stored as netcdf')
+
+    if delete_txt_files:
+        print('---> Removing FSM simulation .txt file')
+        for file in flist:
+            os.remove(file)
+
+
+
 def to_dataset(fname_pattern='sim_FSM_pt*.txt', fsm_path = "./fsm_sims/"):
     '''
     Function to read FSM outputs of one simulation into a single dataset.
     Args:
         fname_pattern:
         fsm_path:
 
     Returns:
-
+        dataset (xarray)
     '''
     fnames = glob.glob(fsm_path + fname_pattern)
     fnames.sort()
 
     ds = xr.concat([txt2ds(fname) for fname in fnames],'point_id')
 
     ds.albedo.attrs = {'units':'ratio', 'standard_name':'albedo', 'long_name':'Surface Effective Albedo', '_FillValue': -9999999.0}
@@ -152,30 +225,92 @@
                 header=0,
                 index_col='time',
                 parse_dates = {'time': [0, 1, 2, 3]},
                 date_format = '%Y %m %d %H.000')
     fsm.columns = ['albedo', 'runoff', 'snd', 'swe', 't_surface', 't_soil']
     return fsm
 
+def _run_fsm(fsm_exec, nlstfile):
+    '''
+    function to execute FSM
+    Args:
+        fsm_exec (str): path to FSM executable
+        nlstfile (str): path to FSM simulation config file
+
+    Returns:
+        NULL (FSM simulation file written to disk)
+    '''
+    os.system(fsm_exec + ' < ' + nlstfile)
+    print('Simulation done: ' + nlstfile)
+
+def fsm_sim_parallel(fsm_input='outputs/FSM_pt*.txt',
+                     fsm_nconfig=31,
+                     fsm_nave=24,  # for daily output
+                     fsm_exec='./FSM',
+                     n_core=6,
+                     n_thread=100,
+                     delete_nlst_files=True):
+    '''
+    Function to run parallelised simulations of FSM
+
+    Args:
+        fsm_input (str or list): file pattern or list of file input to FSM. Note that must be in short relative path!. Default = 'outputs/FSM_pt*.txt'
+        fsm_nconfig (int):  FSM configuration number. See FSM README.md: https://github.com/RichardEssery/FSM. Default = 31
+        fsm_nave (int): number of timestep to average for outputs. e.g. If input is hourly and fsm_nave=24, outputs will be daily. Default = 24
+        fsm_exec (str): path to FSM executable. Default = './FSM'
+        n_core (int): number of cores. Default = 6
+        n_thread (int): number of threads when creating simulation configuration files. Default=100
+        delete_nlst_files (bool): delete simulation configuration files or not. Default=True
+
+    Returns:
+        NULL (FSM simulation file written to disk)
+    '''
+    print('---> Run FSM simulation in parallel')
+    # 1. create all nlsit_files
+    if isinstance(fsm_input, str):
+        met_flist = glob.glob(fsm_input)
+    elif isinstance(fsm_input, list):
+        met_list = fsm_input
+    else:
+        print('ERROR: fsm_input must either be a list of file path or a string of file pattern')
+        return
+
+    fun_param = zip([fsm_nconfig]*len(met_flist), met_flist, [fsm_nave]*len(met_flist) )
+    tu.multithread_pooling(fsm_nlst, fun_param, n_thread)
+    print('nlst files ready')
+
+    # 2. execute FSM on multicore
+    nlst_flist = glob.glob('fsm_sims/nlst_*.txt')
+    fun_param = zip([fsm_exec]*len(nlst_flist), nlst_flist)
+    tu.multicore_pooling(_run_fsm, fun_param, n_core)
+    print('---> FSM simulations finished.')
+
+    # 3. remove nlist files
+    if delete_nlst_files:
+        print('---> Removing FSM simulation config file')
+        for file in nlst_flist:
+            os.remove(file)
+
 
 def fsm_sim(nlstfile, fsm_exec):
     """
     Function to simulate the FSM model
     https://github.com/RichardEssery/FSM
 
     Args:
         nlstfile (int): which FSm configuration to run (integer 1-31)
         fsm_exec (str): path to input tscale file (relative as Fortran fails with long strings (max 21 chars?))
     
     Returns: 
         NULL (FSM simulation file written to disk)
     """
-    print('Simulation done: ' + nlstfile)
+
     os.system(fsm_exec + ' < ' + nlstfile)
     os.remove(nlstfile)
+    print('Simulation done: ' + nlstfile)
 
 
 
 
 
 def agg_by_var_fsm(ncol=None, var='gst', fsm_path = "./fsm_sims"):
     """
@@ -202,20 +337,20 @@
 
 
     def natural_sort(l):
         def convert(text): return int(text) if text.isdigit() else text.lower()
         def alphanum_key(key): return [convert(c) for c in re.split('([0-9]+)', key)]
         return sorted(l, key=alphanum_key)
 
-    fsm_columns = {'alb':4,
-                   'rof':5,
-                   'snd':6,
-                   'swe':7,
-                   'gst':8.,
-                   'tsl':9}
+    fsm_columns = {'alb':3,
+                   'rof':4,
+                   'snd':5,
+                   'swe':6,
+                   'gst':7,
+                   'tsl':8}
 
     if ncol is None and var is not None:
         if var.lower() in ['alb', 'rof', 'snd', 'swe', 'gst', 'tsl']:
             ncol = int(fsm_columns.get(var))
         else:
             print("indicate ncol or var within ['alb', 'rof', 'snd', 'swe', 'gst', 'tsl']")
 
@@ -241,15 +376,16 @@
     myarray = np.asarray(data)  # samples x days
     df = pd.DataFrame(myarray.transpose())
 
 
     # add timestamp
     df.insert(0, 'Datetime', mydates)
     df = df.set_index("Datetime")
-    print(f'Variable {list(fsm_columns)[ncol-4]} extracted')
+
+    print(f'Variable {list(fsm_columns)[ncol-3]} extracted')
     return df
     # df.to_csv('./fsm_sims/'+ varname +'.csv', index=False, header=True)
 
 
 def agg_by_var_fsm_ensemble(ncol=None, var='gst', W=1):
     """
     Function to make single variable multi cluster files as preprocessing step before spatialisation. This is much more efficient than looping over individual simulation files per cluster.
@@ -269,20 +405,20 @@
         6 = swe
         7 = gst
 
     """
 
     # find all simulation files and natural sort https://en.wikipedia.org/wiki/Natural_sort_order
     a = glob.glob("./fsm_sims/sim_ENS*_FSM_pt*")
-    fsm_columns = {'alb':4,
-                   'rof':5,
-                   'snd':6,
-                   'swe':7,
-                   'gst':8.,
-                   'tsl':9}
+    fsm_columns = {'alb':3,
+                   'rof':4,
+                   'snd':5,
+                   'swe':6,
+                   'gst':7.,
+                   'tsl':8}
     if ncol is None and var is not None:
         if var.lower() in ['alb', 'rof', 'snd', 'swe', 'gst', 'tsl']:
             ncol = int(fsm_columns.get(var))
         else:
             print("indicate ncol or var within ['alb', 'rof', 'snd', 'swe', 'gst', 'tsl']")
 
 
@@ -325,15 +461,15 @@
     dfreshape_weight_sum = dfreshape_weight.sum(2)
 
     df = pd.DataFrame(dfreshape_weight_sum)
     # add timestamp
     df.insert(0, 'Datetime', mydates)
     df = df.set_index("Datetime")
 
-    print(f'Variable {list(fsm_columns)[ncol-4]} extracted')
+    print(f'Variable {list(fsm_columns)[ncol-3]} extracted')
     return df
     # df.to_csv('./fsm_sims/'+ varname +'.csv', index=False, header=True)
 
 
 def timeseries_means_period(df, start_date, end_date):
     """
     Function to extract results vectors from simulation results. This can be entire time period some subset or sing day.
@@ -541,16 +677,97 @@
     #
     # src = rasterio.open("output_raster.tif")
     # plt.imshow(src.read(1), cmap='viridis')
     # plt.colorbar()
     # plt.show()
 
 
+def topo_map_sim(ds_var, n_decimals=2, dtype='float32', new_res=None):
+    """
+    Function to map sim results to toposub clusters generating gridded results
+
+    Args:
+        ds_var: single variable of ds eg. mp.downscaled_pts.t
+        n_decimals (int): number of decimal to round vairable. default 2
+        dtype (str): dtype to export raster. default 'float32'
+        new_res (float): optional parameter to resample output to (in units of projection
+
+    Return:
+        grid_stack: stack of grids with dimension Time x Y x X
 
-def write_ncdf(wdir, grid_stack, var, units, longname, mytime, lats, lons, mydtype):
+    Here
+    's an approach for arbitrary reclassification of integer rasters that avoids using a million calls to np.where. Rasterio bits taken from @Aaron'
+    s answer:
+    https://gis.stackexchange.com/questions/163007/raster-reclassify-using-python-gdal-and-numpy
+    """
+
+    # Build a "lookup array" where the index is the original value and the value
+    # is the reclassified value.  Setting all of the reclassified values is cheap
+    # because the memory is only allocated once for the lookup array.
+    nclust = ds_var.shape[1]
+    lookup = np.arange(nclust, dtype=dtype)
+
+    # replicate looup through timedimens (dims Time X sample )
+    lookup2D = np.tile(lookup, (ds_var.shape[0], 1))
+
+    for i in range(0, nclust):
+        lookup2D[:, i] = ds_var[i]
+
+    from osgeo import gdal
+    inputFile = "outputs/landform.tif"
+    outputFile = "outputs/landform_newres.tif"
+
+    # check if new_res is declared - if so resample landform and therefore output
+    if new_res is not None:
+        xres = new_res
+        yres = new_res
+        resample_alg = gdal.GRA_NearestNeighbour
+
+        ds = gdal.Warp(destNameOrDestDS=outputFile,
+                       srcDSOrSrcDSTab=inputFile,
+                       format='GTiff',
+                       xRes=xres,
+                       yRes=yres,
+                       resampleAlg=resample_alg)
+        del ds
+        landformfile = "outputs/landform_newres.tif"
+    else:
+        landformfile = "outputs/landform.tif"
+
+    with rasterio.open(landformfile) as src:
+
+        # new res
+        # upscale_factor = src.res[0] / new_res
+        # # resample data to target shape
+        # array = src.read(
+        #     out_shape=(
+        #         src.count,
+        #         int(src.height * upscale_factor),
+        #         int(src.width * upscale_factor)
+        #     ),
+        #     resampling=Resampling.nearest
+        # )
+
+        # return coords of resampled grid here (this does not preserve dimensions perfectly (can be 1pix out))
+        array = src.read()
+        min_E, min_N, max_E, max_N = src.bounds
+        lons = np.arange(min_E, max_E, src.res[0])
+        lats = np.arange(min_N, max_N, src.res[1])
+        lats = lats[::-1]
+
+    array2 = lookup2D.transpose()[array]  # Reclassify in a single operation using broadcasting
+    try:
+        grid_stack = np.round(array2.squeeze().transpose(2, 0, 1), n_decimals)  # transpose to Time x Y x X
+    except:  # the case where we gen annual grids (no time dimension)
+        grid_stack = np.round(array2.squeeze(), n_decimals)  # transpose to Time x Y x X
+    return grid_stack, lats, lons
+
+
+
+def write_ncdf(wdir, grid_stack, var, units,epsg,res,  mytime, lats, lons, mydtype,newfile, outname=None):
     # https://www.earthinversion.com/utilities/Writing-NetCDF4-Data-using-Python/
 
     # # coords
     # with rasterio.open("landform.tif") as src:
     #     # bounding box of image
     #     min_E, min_N, max_E, max_N = src.bounds
     #     # resolution of image
@@ -559,15 +776,15 @@
     # lats = np.arange(min_N, max_N, res[1])
     # lats = lats[::-1]
 
     try:
         ds = xr.Dataset(
              {var: (("Time", "northing", "easting"), grid_stack)},
              coords={
-                 "Time":  mytime.data,
+                 "Time":  mytime,
                  "northing": lats,
                  "easting": lons
 
              },
          )
     except:
         ds = xr.Dataset(
@@ -575,27 +792,22 @@
             coords={
                 "northing": lats,
                 "easting": lons
 
             },
         )
 
-    ds.attrs["units"] = units  # add epsg here
-    if var == "ta" or var=="tas" or var=="TA":
-        ds.to_netcdf( wdir + "/outputs/"+str(mytime[0].values).split("-")[0]+str(mytime[0].values).split("-")[1]+".nc",
-                      mode="w",
-                      encoding={var: {"dtype": mydtype, 'zlib': True, 'complevel': 5}},
-                      engine='h5netcdf')
-    else:
-        ds.to_netcdf( wdir + "/outputs/"+str(mytime[0].values).split("-")[0]+str(mytime[0].values).split("-")[1]+".nc",
-                      mode="a",
-                      encoding={var: {"dtype": mydtype, 'zlib': True, 'complevel': 5}},
-                      engine='h5netcdf')
-
+    ds.attrs["units"] = units 
+    ds.attrs["epsg_code"] = epsg # add epsg here
+    ds.attrs["resolution_m"] = str(res) # add epsg here
 
+    if newfile == True:
+        ds.to_netcdf( wdir + "/outputs/"+str(mytime[0]).split("-")[0]+str(mytime[0]).split("-")[1]+"_"+outname+".nc", mode="w", encoding={var: {"dtype": mydtype, 'zlib': True, 'complevel': 5} })
+    else:
+        ds.to_netcdf( wdir + "/outputs/"+str(mytime[0]).split("-")[0]+str(mytime[0]).split("-")[1]+"_"+outname+".nc", mode="a", encoding={var: {"dtype": mydtype, 'zlib': True, 'complevel': 5} })
 def agg_stats(df ):
     # generate aggregated stats from the simulation
     # USAGE:
     # HS = sim.agg_by_var_fsm(6)
     # SWE = sim.agg_by_var_fsm(5)
     # HSdf = agg_stats(HS)
     # SWEdf = agg_stats(SWE)
```

### Comparing `topopyscale-0.2.2/TopoPyScale/topo_sub.py` & `topopyscale-0.2.3/TopoPyScale/topo_sub.py`

 * *Files identical despite different names*

### Comparing `topopyscale-0.2.2/TopoPyScale/topo_utils.py` & `topopyscale-0.2.3/TopoPyScale/topo_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,24 +2,83 @@
 import pyproj
 import rasterio
 import linecache
 from matplotlib import pyplot as plt
 import numpy as np
 import glob
 from TopoPyScale import topo_da as da
+import git
+from multiprocessing import Pool
+from multiprocessing.dummy import Pool as ThreadPool
+import multiprocessing as mproc
+
+def multicore_pooling(fun, fun_param, n_cores):
+    '''
+    Function to perform multiprocessing on n_cores
+    Args:
+        fun (obj): function to distribute
+        fun_param zip(list): zip list of functino arguments
+        n_core (int): number o cores
+    '''
+    if n_cores is None:
+        n_cores = mproc.cpu_count() - 2
+        print(f'WARNING: number of cores to use not provided. By default {n_cores} cores will be used')
+    elif n_cores > mproc.cpu_count():
+        n_cores = mproc.cpu_count() - 2
+        print(f'WARNING: Only {mproc.cpu_count()} cores available on this machine, reducing n_cores to {n_cores} ')
+
+    # make sure it will run on one core at least
+    if n_cores == 0:
+        n_cores = 1
+
+    pool = Pool(n_cores)
+    pool.starmap(fun, fun_param)
+    pool.close()
+    pool.join()
+    pool = None
+
+
+def multithread_pooling(fun, fun_param, n_threads):
+    '''
+    Function to perform multiprocessing on n_threads
+    Args:
+        fun (obj): function to distribute
+        fun_param zip(list): zip list of functino arguments
+        n_core (int): number of threads
+    '''
+    tpool = ThreadPool(n_threads)
+    tpool.starmap(fun, fun_param)
+    tpool.close()
+    tpool.join()
+    tpool = None
+
+def get_versionning():
+    import TopoPyScale as tps
+    from importlib import metadata
+    try:
+        repo = git.Repo(path=tps.__file__, search_parent_directories=True)
+        hash = repo.head.object.hexsha
+    except:
+        hash = 'Not available'
+    version = metadata.version('TopoPyScale')
+    ver_dic = {'git_commit': hash,
+               'package_version': version}
+    return ver_dic
+
+
 
 def FsmMetParser(file, freq="1h", resample=False):
     '''
     Parses FSM forcing files from toposcale sims
     '''
 
     df = pd.read_csv(file, delim_whitespace=True,
                      header=None, index_col='datetime',
                      parse_dates={'datetime': [0, 1, 2, 3]},
-                     date_parser=lambda x: pd.datetime.strptime(x, '%Y %m %d %H'))
+                     date_format=('%Y %m %d %H'))
 
     df.columns = ['ISWR', 'ILWR', 'Sf', 'Rf', 'TA', 'RH', 'VW', 'P']
 
     if resample == "TRUE":
         print('ERROR: line 24 to be fixed!')
         #df = df.resample(freq).apply(resample_func)
```

### Comparing `topopyscale-0.2.2/TopoPyScale/topoclass.py` & `topopyscale-0.2.3/TopoPyScale/topoclass.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,61 +7,67 @@
     config.ini
     -> input/
         -> dem/
         -> climate/
     -> output/
 
 """
-import glob, os, sys, shutil
-import pdb
-from pathlib import Path
+import glob
+import os
 import re
-from munch import DefaultMunch
+import shutil
+import sys
+from pathlib import Path
+
+import matplotlib.pyplot as plt
+import numpy as np
 import pandas as pd
 import xarray as xr
-import numpy as np
-import matplotlib.pyplot as plt
-from TopoPyScale import fetch_era5 as fe
-from TopoPyScale import topo_param as tp
-from TopoPyScale import topo_sub as ts
+from munch import DefaultMunch
+from sklearn.preprocessing import StandardScaler
+
 from TopoPyScale import fetch_dem as fd
+from TopoPyScale import fetch_era5 as fe
 from TopoPyScale import solar_geom as sg
-from TopoPyScale import topo_scale as ta
 from TopoPyScale import topo_export as te
-from TopoPyScale import topo_plot as tpl
 from TopoPyScale import topo_obs as tpo
-
-from sklearn.preprocessing import StandardScaler
+from TopoPyScale import topo_param as tp
+from TopoPyScale import topo_plot as tpl
+from TopoPyScale import topo_scale as ta
+from TopoPyScale import topo_sub as ts
 
 
 class Topoclass(object):
     """
     A python class to bring the typical use-case of toposcale in a user friendly object
     """
 
     def __init__(self, config_file):
 
         try:
             with open(config_file, 'r') as f:
                 self.config = DefaultMunch.fromYAML(f)
 
-
             if self.config.project.directory is None:
                 self.config.project.directory = os.getcwd() + '/'
 
         except IOError:
-            print(f'ERROR: config file does not exist. \n\t Current file path: {config_file}\n\t Current working directory: {os.getcwd()}')
+            print(
+                f'ERROR: config file does not exist. \n\t Current file path: {config_file}\n\t Current working directory: {os.getcwd()}')
+
+        self.config.outputs.path = Path(self.config.project.directory, 'outputs')
+        self.config.outputs.tmp_path = self.config.outputs.path / 'tmp'
 
         if self.config.outputs.file.clean_outputs:
             # remove outputs directory because if results already exist this causes concat of netcdf files
             try:
-                shutil.rmtree(self.config.project.directory + '/outputs/')
+                shutil.rmtree(self.config.outputs.path)
                 print('---> Output directory cleaned')
             except:
-                os.makedirs('/'.join((self.config.project.directory, 'outputs/')))
+                os.makedirs(self.config.outputs.path)
 
         # remove output fsm directory
         if self.config.outputs.file.clean_FSM:
             try:
                 shutil.rmtree(self.config.project.directory + '/fsm_sims/')
                 print('---> FSM directory cleaned')
             except:
@@ -69,33 +75,38 @@
 
             # remove output fsm directory
             try:
                 shutil.rmtree(self.config.project.directory + '/ensemble/')
                 print("---> Ensemble directory cleaned")
             except:
                 print("---> no ensemble directory to clean")
+
+        # directory where to store the downscaled data
+        if self.config.outputs.directory:
+            self.config.outputs.downscaled = Path(self.config.outputs.directory)
+        else:
+            self.config.outputs.downscaled = self.config.outputs.path / 'downscaled'
+
+        # climate path
+        if os.path.isabs(self.config.climate.era5.path):
+            self.config.climate.path = self.config.climate.era5.path
+        else:
+            self.config.climate.path = '/'.join((self.config.project.directory, 'inputs/climate/'))
+        self.config.climate.tmp_path = '/'.join((self.config.climate.path, 'tmp'))
+
         # check if tree directory exists. If not create it
-        if not os.path.exists('/'.join((self.config.project.directory, 'inputs/'))):
-            os.makedirs('/'.join((self.config.project.directory, 'inputs/')))
-        if not os.path.exists('/'.join((self.config.project.directory, 'outputs/'))):
-            os.makedirs('/'.join((self.config.project.directory, 'outputs/')))
-
-        self.config.climate.path = self.config.project.directory + 'inputs/climate/'
-        if not os.path.exists('/'.join((self.config.project.directory, 'inputs/climate/'))):
-            os.makedirs('/'.join((self.config.project.directory, 'inputs/climate')))
-        if not os.path.exists('/'.join((self.config.project.directory, 'inputs/climate/tmp/'))):
-            os.makedirs('/'.join((self.config.project.directory, 'inputs/climate/tmp')))
-        if not os.path.exists('/'.join((self.config.project.directory, 'outputs/tmp/'))):
-            os.makedirs('/'.join((self.config.project.directory, 'outputs/tmp')))
-        if not os.path.exists('/'.join((self.config.project.directory, 'outputs/downscaled'))):
-            os.makedirs('/'.join((self.config.project.directory, 'outputs/downscaled')))
-
-        self.config.dem.path = self.config.project.directory + '/inputs/dem/'
-        if not os.path.exists('/'.join((self.config.project.directory, 'inputs/dem/'))):
-            os.makedirs('/'.join((self.config.project.directory, 'inputs/dem')))
+        os.makedirs(self.config.climate.path, exist_ok=True)
+        os.makedirs(self.config.climate.tmp_path, exist_ok=True)
+        os.makedirs(self.config.outputs.path, exist_ok=True)
+        os.makedirs(self.config.outputs.tmp_path, exist_ok=True)
+        os.makedirs(self.config.outputs.downscaled, exist_ok=True)
+
+        if not self.config.dem.path:
+            self.config.dem.path = self.config.project.directory + '/inputs/dem/'
+        os.makedirs(self.config.dem.path, exist_ok=True)
 
         self.config.dem.filepath = self.config.dem.path + self.config.dem.file
         if not os.path.isfile(self.config.dem.filepath):
 
             if self.config.project.extent is not None:
                 self.config.project.extent = dict(zip(['latN', 'latS', 'lonW', 'lonE'], self.config.project.extent))
             else:
@@ -169,19 +180,19 @@
         if os.path.isfile(self.config.project.directory + 'outputs/' + self.config.outputs.file.da_horizon):
             self.da_horizon = xr.open_dataarray(
                 self.config.project.directory + 'outputs/' + self.config.outputs.file.da_horizon)
             print(f'---> Horizon file {self.config.outputs.file.da_horizon} exists and loaded')
         else:
             print(f'-> WARNING: Horizon file {self.config.outputs.file.da_horizon} not found')
 
-        flist = glob.glob(f'{self.config.project.directory}outputs/downscaled/{self.config.outputs.file.downscaled_pt}')
+        flist = glob.glob(f'{self.config.outputs.downscaled}/{self.config.outputs.file.downscaled_pt}')
         if len(flist) > 0:
             print('---> Loading downscaled points \n ...')
             self.downscaled_pts = xr.open_mfdataset(
-                f'{self.config.project.directory}outputs/downscaled/{self.config.outputs.file.downscaled_pt}',
+                f'{self.config.outputs.downscaled}/{self.config.outputs.file.downscaled_pt}',
                 concat_dim='point_id',
                 combine='nested',
                 parallel=True)
             print(f'---> Downscaled point files {self.config.outputs.file.ds_param} exists and loaded')
         else:
             print(f'-> WARNING: Downscale point files {self.config.outputs.file.downscaled_pt} not found')
 
@@ -251,20 +262,27 @@
 
         Args:
             df (dataFrame):
             method (str): method of sampling
             **kwargs: pd.read_csv() parameters
         Returns:
         """
-        self.toposub.df_centroids = pd.read_csv(
-            self.config.project.directory + 'inputs/dem/' + self.config.sampling.points.csv_file, **kwargs)
-        self.toposub.df_centroids['point_id'] = self.toposub.df_centroids.index.astype(int)
-        self.toposub.df_centroids = tp.extract_pts_param(self.toposub.df_centroids, self.toposub.ds_param,
-                                                         method=method)
-
+        if not os.path.isabs(self.config.sampling.points.csv_file):
+            self.config.sampling.points.csv_file = self.config.project.directory + 'inputs/dem/' + self.config.sampling.points.csv_file
+        df_centroids = pd.read_csv(self.config.sampling.points.csv_file, **kwargs)
+        if self.config.sampling.points.ID_col:
+            ID_col = df_centroids[self.config.sampling.points.ID_col]
+            df_centroids['point_id'] = pd.to_numeric(ID_col, errors='ignore').astype(str)
+        else:
+            df_centroids['point_id'] = df_centroids.index + 1
+            n_digits = len(str(df_centroids.point_id.max()))
+            df_centroids['point_id'] = df_centroids.point_id.astype(str).str.zfill(n_digits)
+        df_centroids = tp.extract_pts_param(df_centroids, self.toposub.ds_param,
+                                            method=method)
+        self.toposub.df_centroids = df_centroids
 
     def extract_topo_cluster_param(self):
         """
         Function to segment a DEM in clusters and retain only the centroids of each cluster.
 
         :return:
 
@@ -297,15 +315,17 @@
         feature_list = self.config.sampling.toposub.clustering_features.keys()
         flist = list(feature_list)
         flist.append('cluster_labels')
         if len(df_param.columns) > len(flist):
             tmp = df_param.groupby('cluster_labels').mean()
             for var in df_param.drop(flist, axis=1).columns:
                 self.toposub.df_centroids[var] = tmp[var]
-        self.toposub.df_centroids['point_id'] = self.toposub.df_centroids.index.astype(int)
+        n_digits = len(str(self.toposub.df_centroids.index.max()))
+        self.toposub.df_centroids['point_id'] = self.toposub.df_centroids.index.astype(int).astype(str).str.zfill(
+            n_digits)
         self.toposub.ds_param['cluster_labels'] = (
             ["y", "x"], np.reshape(df_param.cluster_labels.values, self.toposub.ds_param.slope.shape))
 
         # update file
         fname = self.config.project.directory + 'outputs/' + self.config.outputs.file.ds_param
         te.to_netcdf(self.toposub.ds_param, fname=fname)
 
@@ -319,29 +339,32 @@
         if os.path.isfile(self.config.project.directory + 'outputs/' + self.config.outputs.file.df_centroids):
             self.toposub.df_centroids = pd.read_pickle(
                 self.config.project.directory + 'outputs/' + self.config.outputs.file.df_centroids)
             print(f'---> Centroids file {self.config.outputs.file.df_centroids} exists and loaded')
         else:
             if self.config.sampling.method in ['points', 'point']:
                 self.extract_pts_param()
+                # if self.config.sampling.points.ID_col:
+                #     self.config.sampling.pt_names = list(
+                #         self.toposub.df_centroids[self.config.sampling.points.ID_col])
             elif self.config.sampling.method == 'toposub':
                 self.extract_topo_cluster_param()
             elif self.config.sampling.method == 'both':
 
                 # implement the case one wann run both toposub and a list of points
                 print('ERROR: method not yet implemented')
 
             else:
                 print('ERROR: Extraction method not available')
 
-
-            self.toposub.df_centroids['lon'], self.toposub.df_centroids['lat'] = tp.convert_epsg_pts(self.toposub.df_centroids.x,
-                                                                                              self.toposub.df_centroids.y,
-                                                                                              self.config.dem.epsg,
-                                                                                              4326)
+            self.toposub.df_centroids['lon'], self.toposub.df_centroids['lat'] = tp.convert_epsg_pts(
+                self.toposub.df_centroids.x,
+                self.toposub.df_centroids.y,
+                self.config.dem.epsg,
+                4326)
 
             # Store dataframe to pickle
             self.toposub.df_centroids.to_pickle(
                 self.config.project.directory + 'outputs/' + self.config.outputs.file.df_centroids)
             print(f'---> Centroids file {self.config.outputs.file.df_centroids} saved')
 
     class TimeSplitter():
@@ -427,32 +450,40 @@
                                                                                        method='nearest').values.flatten()
             # update df_centroid file with horizons angle
             self.toposub.df_centroids.to_pickle(
                 self.config.project.directory + 'outputs/' + self.config.outputs.file.df_centroids)
             print(f'---> Centroids file {self.config.outputs.file.df_centroids} updated with horizons')
 
     def downscale_climate(self):
-        downscaled_dir = Path(self.config.project.directory, 'outputs', 'downscaled')
+        downscaled_dir = self.config.outputs.downscaled
         f_pattern = self.config.outputs.file.downscaled_pt
 
         if '*' not in f_pattern:
             raise ValueError(
                 f'The filepattern for the downscaled files does need to have a * in the name. You provided {f_pattern}')
 
+        # clean directory from files with the same downscaled output file pattern (so they get replaced)
+        existing_files = sorted(downscaled_dir.glob(f_pattern))
+        for file in existing_files:
+            file.unlink()
+            print(f'existing file {file.name} removed.')
+
         if self.config.project.split.IO:
             for i, start in enumerate(self.time_splitter.start_list):
                 print()
                 end = self.time_splitter.end_list[i]
                 fname = self.time_splitter.downscaled_flist[i]
 
                 self.ds_solar = None
                 self.ds_solar = xr.open_dataset(
                     self.config.project.directory + 'outputs/' + self.time_splitter.ds_solar_flist[i])
 
                 ta.downscale_climate(self.config.project.directory,
+                                     self.config.climate.path,
+                                     self.config.outputs.downscaled,
                                      self.toposub.df_centroids,
                                      self.da_horizon,
                                      self.ds_solar,
                                      self.config.dem.epsg,
                                      start,
                                      end,
                                      self.config.toposcale.interpolation_method,
@@ -460,82 +491,89 @@
                                      self.config.climate[self.config.project.climate].timestep,
                                      self.config.climate.precip_lapse_rate,
                                      fname,
                                      self.config.project.CPU_cores)
 
             # Concatenate time-splitted outputs along time-dimension
             # TODO: modify code below to concatenate to be parallelized.
-            n_digits = len(str(self.toposub.df_centroids.index.max()))
-
-            # clean directory from files with the same downscaled output file pattern (so they get replaced)
-            f_pattern_regex = f_pattern.replace('*', '\d+')
-            existing_files = sorted(
-                [file for file in downscaled_dir.glob('**/*') if re.match(f_pattern_regex, file.name)])
-            for file in existing_files:
-                file.unlink()
-                print(f'existing file {file.name} removed.')
 
             for pt_id in self.toposub.df_centroids.point_id.values:
                 print(f'Concatenating point {pt_id}')
-                num = str(pt_id).zfill(n_digits)
-                filename = Path(f_pattern.replace('*', num))
-                flist = sorted([file for file in downscaled_dir.glob(f'**/{filename.stem}*')])
+                filename = Path(f_pattern.replace('*', pt_id))
+                flist = sorted([file for file in downscaled_dir.rglob(f'{filename.stem}_*')])
                 ds_list = [xr.open_dataset(file, engine='h5netcdf') for file in flist]
 
                 fout = Path(downscaled_dir, filename)
                 ds = xr.concat(ds_list, dim='time')
                 ds.to_netcdf(fout, engine='h5netcdf')
                 del ds
 
             # Delete time slice files.
             for fpat in self.time_splitter.downscaled_flist:
-                flist = glob.glob(f'{self.config.project.directory}outputs/downscaled/{fpat}')
+                flist = glob.glob(f'{self.config.outputs.downscaled}/{fpat}')
                 for file in flist:
                     os.remove(file)
 
         else:
             ta.downscale_climate(self.config.project.directory,
+                                 self.config.climate.path,
+                                 self.config.outputs.downscaled,
                                  self.toposub.df_centroids,
                                  self.da_horizon,
                                  self.ds_solar,
                                  self.config.dem.epsg,
                                  self.config.project.start,
                                  self.config.project.end,
                                  self.config.toposcale.interpolation_method,
                                  self.config.toposcale.LW_terrain_contribution,
                                  self.config.climate[self.config.project.climate].timestep,
                                  self.config.climate.precip_lapse_rate,
                                  self.config.outputs.file.downscaled_pt,
                                  self.config.project.CPU_cores)
 
-        self.downscaled_pts = ta.read_downscaled(
-            self.config.project.directory + 'outputs/downscaled/' + self.config.outputs.file.downscaled_pt)
+        self.downscaled_pts = ta.read_downscaled(f'{downscaled_dir}/{f_pattern}')
         # update plotting class variables
         self.plot.ds_down = self.downscaled_pts
 
+        # delete tmp directories
+        if self.config.clean_up.delete_tmp_dirs:
+            shutil.rmtree(self.config.outputs.tmp_path, ignore_errors=True)
+            shutil.rmtree(self.config.climate.tmp_path, ignore_errors=True)
+
     def get_era5(self):
         """
         Funtion to call fetching of ERA5 data
         TODO:
         - merge monthly data into one file (cdo?)- this creates massive slow down!
         """
         lonW = self.config.project.extent.get('lonW') - 0.4
         lonE = self.config.project.extent.get('lonE') + 0.4
         latN = self.config.project.extent.get('latN') + 0.4
         latS = self.config.project.extent.get('latS') - 0.4
 
         # if keyword exists in config set realtime to value (True/False)
         if self.config.climate[self.config.project.climate].realtime:
-            realtime=self.config.climate[self.config.project.climate].realtime
+            realtime = self.config.climate[self.config.project.climate].realtime
         # else set realtime to False
         else:
-            realtime=False
-
+            realtime = False
 
+        if realtime: # make sure end date is correct
+            lastdate = fe.return_last_fullday()
+            # 5th day will always be incomplete so we got to last fullday
+            self.config.project.end = self.config.project.end.replace(year=lastdate.year, month=lastdate.month, day=lastdate.day)
 
+            # remove existing results (temporary results are ok and updated but cannot append to final files eg .outputs/downscaled/down_pt_0.nc)
+            try:
+                shutil.rmtree(self.config.outputs.path / "downscaled")
+                print('---> Downscaled directory cleaned')
+                os.makedirs(self.config.outputs.path / "downscaled")
+            except:
+                os.makedirs(self.config.outputs.path / "downscaled")
+        realtime = False
         # retreive ERA5 surface data
         fe.retrieve_era5(
             self.config.climate[self.config.project.climate].product,
             self.config.project.start,
             self.config.project.end,
             self.config.climate.path,
             latN, latS, lonE, lonW,
@@ -649,15 +687,17 @@
         """
         if variables is None:
             if (type(self.config.outputs.variables) is not list) or (self.config.outputs.variables is None):
                 variables = list(self.downscaled_pts.keys())
             else:
                 variables = self.config.outputs.variables
 
-        te.to_netcdf(self.downscaled_pts[variables], f'{self.config.project.directory}outputs/' + file_out, variables)
+        out_path = Path(self.config.outputs.path, file_out)
+
+        te.to_netcdf(self.downscaled_pts[variables], out_path, variables)
         print('---> File {} saved'.format(file_out))
 
     def to_snowpack(self, fname_format='smet_pt_*.smet'):
         """
         function to export toposcale output to FSM format
         """
         te.to_snowpack(self.downscaled_pts, f'{self.config.project.directory}outputs/' + fname_format)
```

### Comparing `topopyscale-0.2.2/logo.svg` & `topopyscale-0.2.3/logo.svg`

 * *Files identical despite different names*

### Comparing `topopyscale-0.2.2/setup.py` & `topopyscale-0.2.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name='topopyscale',
-    version='0.2.2',
-    description='A Python package to perform climate downscaling at the hillslope scale',
+    version='0.2.3',
+    description='TopoPyScale: A Python Package for Hillslope Climate Downscaling',
     long_description=long_description,
 
     # The project's main homepage.
     url='https://github.com/ArcticSnow/TopoPyScale',
     download_url = 'https://github.com/ArcticSnow/TopoPyScale/releases/latest',
     project_urls={
         'Documentation':'https://topopyscale.readthedocs.io/en/latest/',
```

### Comparing `topopyscale-0.2.2/topopyscale.egg-info/PKG-INFO` & `topopyscale-0.2.3/topopyscale.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: topopyscale
-Version: 0.2.2
-Summary: A Python package to perform climate downscaling at the hillslope scale
+Version: 0.2.3
+Summary: TopoPyScale: A Python Package for Hillslope Climate Downscaling
 Home-page: https://github.com/ArcticSnow/TopoPyScale
 Download-URL: https://github.com/ArcticSnow/TopoPyScale/releases/latest
 Author: ['Simon Filhol', 'Joel Fiddes', 'Kristoffer Aalstad']
 Author-email: simon.filhol@geo.uio.no
 License: MIT
 Project-URL: Documentation, https://topopyscale.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ArcticSnow/TopoPyScale
@@ -27,14 +27,16 @@
 [![DOI](https://zenodo.org/badge/411249045.svg)](https://zenodo.org/badge/latestdoi/411249045)
 [![GitHub license](https://img.shields.io/github/license/ArcticSnow/TopoPyScale)](https://github.com/ArcticSnow/TopoPyScale/blob/main/LICENSE)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/ArcticSnow/TopoPyScale)
 <a href="https://joss.theoj.org/papers/91621581b2d0c097495fdd1e58179e87"><img src="https://joss.theoj.org/papers/91621581b2d0c097495fdd1e58179e87/status.svg"></a>
 [![][docs-dev-img]][docs-dev-url]
 ![Test](https://github.com/ArcticSnow/TopoPyScale/actions/workflows/test_topopyscale.yml/badge.svg)
 
+Binder Notebooks Examples: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ArcticSnow/TopoPyScale_examples/HEAD)
+
 [docs-dev-img]: https://img.shields.io/badge/docs-latest-blue.svg
 [docs-dev-url]: https://topopyscale.readthedocs.io
 
 # TopoPyScale
 Python version of Toposcale packaged as a Pypi library. Toposcale is an original idea of Joel Fiddes to perform topography-based downscaling of climate data to the hillslope scale.
 
 Documentation avalaible: https://topopyscale.readthedocs.io
```

#### html2text {}

```diff
@@ -1,31 +1,33 @@
-Metadata-Version: 2.1 Name: topopyscale Version: 0.2.2 Summary: A Python
-package to perform climate downscaling at the hillslope scale Home-page: https:
-//github.com/ArcticSnow/TopoPyScale Download-URL: https://github.com/
-ArcticSnow/TopoPyScale/releases/latest Author: ['Simon Filhol', 'Joel Fiddes',
-'Kristoffer Aalstad'] Author-email: simon.filhol@geo.uio.no License: MIT
-Project-URL: Documentation, https://topopyscale.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/ArcticSnow/TopoPyScale Project-URL:
-Examples, https://github.com/ArcticSnow/TopoPyScale_examples Keywords:
+Metadata-Version: 2.1 Name: topopyscale Version: 0.2.3 Summary: TopoPyScale: A
+Python Package for Hillslope Climate Downscaling Home-page: https://github.com/
+ArcticSnow/TopoPyScale Download-URL: https://github.com/ArcticSnow/TopoPyScale/
+releases/latest Author: ['Simon Filhol', 'Joel Fiddes', 'Kristoffer Aalstad']
+Author-email: simon.filhol@geo.uio.no License: MIT Project-URL: Documentation,
+https://topopyscale.readthedocs.io/en/latest/ Project-URL: Source, https://
+github.com/ArcticSnow/TopoPyScale Project-URL: Examples, https://github.com/
+ArcticSnow/TopoPyScale_examples Keywords:
 climate,downscaling,meteorology,xarray Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering :: Visualization Classifier: Topic :: Scientific/
 Engineering :: Hydrology Classifier: Topic :: Scientific/Engineering ::
 Atmospheric Science Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9 Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE [![DOI](https://
 zenodo.org/badge/411249045.svg)](https://zenodo.org/badge/latestdoi/411249045)
 [![GitHub license](https://img.shields.io/github/license/ArcticSnow/
 TopoPyScale)](https://github.com/ArcticSnow/TopoPyScale/blob/main/LICENSE) !
 [GitHub release (latest by date)](https://img.shields.io/github/v/release/
 ArcticSnow/TopoPyScale) [https://joss.theoj.org/papers/
 91621581b2d0c097495fdd1e58179e87/status.svg] [![][docs-dev-img]][docs-dev-url]
 ![Test](https://github.com/ArcticSnow/TopoPyScale/actions/workflows/
-test_topopyscale.yml/badge.svg) [docs-dev-img]: https://img.shields.io/badge/
-docs-latest-blue.svg [docs-dev-url]: https://topopyscale.readthedocs.io #
+test_topopyscale.yml/badge.svg) Binder Notebooks Examples: [![Binder](https://
+mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ArcticSnow/
+TopoPyScale_examples/HEAD) [docs-dev-img]: https://img.shields.io/badge/docs-
+latest-blue.svg [docs-dev-url]: https://topopyscale.readthedocs.io #
 TopoPyScale Python version of Toposcale packaged as a Pypi library. Toposcale
 is an original idea of Joel Fiddes to perform topography-based downscaling of
 climate data to the hillslope scale. Documentation avalaible: https://
 topopyscale.readthedocs.io ![](https://github.com/ArcticSnow/TopoPyScale/blob/
 main/JOSS/temperature_comparison_crop_scaled.jpg) **References:** - Fiddes, J.
 and Gruber, S.: TopoSCALE v.1.0: downscaling gridded climate data in complex
 terrain, Geosci. Model Dev., 7, 387â405, https://doi.org/10.5194/gmd-7-387-
```

### Comparing `topopyscale-0.2.2/topopyscale.egg-info/SOURCES.txt` & `topopyscale-0.2.3/topopyscale.egg-info/SOURCES.txt`

 * *Files identical despite different names*

