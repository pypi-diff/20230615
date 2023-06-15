# Comparing `tmp/biorefineries-2.9.3.tar.gz` & `tmp/biorefineries-2.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\biorefineries-2.9.3.tar", last modified: Fri Apr 24 02:09:59 2020, max compression
+gzip compressed data, was "dist\biorefineries-2.9.4.tar", last modified: Fri Apr 24 16:37:27 2020, max compression
```

## Comparing `biorefineries-2.9.3.tar` & `biorefineries-2.9.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2020-04-24 02:09:59.000000 biorefineries-2.9.3/
--rw-rw-rw-   0        0        0     2999 2020-04-24 02:09:59.000000 biorefineries-2.9.3/PKG-INFO
--rw-rw-rw-   0        0        0     1510 2020-02-05 17:03:42.000000 biorefineries-2.9.3/README.rst
-drwxrwxrwx   0        0        0        0 2020-04-24 02:09:59.000000 biorefineries-2.9.3/biorefineries/
-drwxrwxrwx   0        0        0        0 2020-04-24 02:09:59.000000 biorefineries-2.9.3/biorefineries/cornstover/
--rw-rw-rw-   0        0        0  3342696 2020-04-14 19:02:05.000000 biorefineries-2.9.3/biorefineries/cornstover/Monte Carlo cornstover.xlsx
--rw-rw-rw-   0        0        0    12055 2020-04-14 19:02:05.000000 biorefineries-2.9.3/biorefineries/cornstover/Spearman correlation cornstover.xlsx
--rw-rw-rw-   0        0        0      206 2020-01-24 16:20:24.000000 biorefineries-2.9.3/biorefineries/cornstover/__init__.py
--rw-rw-rw-   0        0        0      478 2020-04-14 16:09:53.000000 biorefineries-2.9.3/biorefineries/cornstover/_analysis.py
--rw-rw-rw-   0        0        0    15562 2020-04-03 16:55:37.000000 biorefineries-2.9.3/biorefineries/cornstover/_humbird2011.xlsx
--rw-rw-rw-   0        0        0     2019 2019-09-27 08:38:09.000000 biorefineries-2.9.3/biorefineries/cornstover/_plot_bars.py
--rw-rw-rw-   0        0        0     2817 2019-11-18 07:42:30.000000 biorefineries-2.9.3/biorefineries/cornstover/_plot_spearman.py
--rw-rw-rw-   0        0        0     6662 2019-10-07 11:41:34.000000 biorefineries-2.9.3/biorefineries/cornstover/_plot_uncertainty_bottom.py
--rw-rw-rw-   0        0        0     8901 2020-04-10 17:38:51.000000 biorefineries-2.9.3/biorefineries/cornstover/_plot_uncertainty_top.py
--rw-rw-rw-   0        0        0    10496 2020-04-24 01:58:18.000000 biorefineries-2.9.3/biorefineries/cornstover/chemicals.py
--rw-rw-rw-   0        0        0     3687 2020-02-10 03:04:58.000000 biorefineries-2.9.3/biorefineries/cornstover/model.py
--rw-rw-rw-   0        0        0     1489 2020-04-10 19:03:12.000000 biorefineries-2.9.3/biorefineries/cornstover/process_settings.py
--rw-rw-rw-   0        0        0    26955 2020-04-14 19:51:43.000000 biorefineries-2.9.3/biorefineries/cornstover/system.py
--rw-rw-rw-   0        0        0     3469 2020-04-14 18:34:37.000000 biorefineries-2.9.3/biorefineries/cornstover/tea.py
--rw-rw-rw-   0        0        0    23874 2020-04-14 17:31:01.000000 biorefineries-2.9.3/biorefineries/cornstover/units.py
-drwxrwxrwx   0        0        0        0 2020-04-24 02:09:59.000000 biorefineries-2.9.3/biorefineries/lipidcane/
--rw-rw-rw-   0        0        0    16783 2020-04-14 19:53:38.000000 biorefineries-2.9.3/biorefineries/lipidcane/Monte Carlo across lipid fraction.xlsx
--rw-rw-rw-   0        0        0     6782 2020-04-14 19:53:38.000000 biorefineries-2.9.3/biorefineries/lipidcane/Monte Carlo sugarcane.xlsx
--rw-rw-rw-   0        0        0     8304 2020-03-04 08:40:33.000000 biorefineries-2.9.3/biorefineries/lipidcane/Spearman correlation lipidcane.xlsx
--rw-rw-rw-   0        0        0      163 2020-02-06 08:55:18.000000 biorefineries-2.9.3/biorefineries/lipidcane/__init__.py
--rw-rw-rw-   0        0        0     2297 2020-04-11 21:42:11.000000 biorefineries-2.9.3/biorefineries/lipidcane/_analysis.py
--rw-rw-rw-   0        0        0     2843 2019-11-18 17:14:19.000000 biorefineries-2.9.3/biorefineries/lipidcane/_plot_spearman.py
--rw-rw-rw-   0        0        0    11316 2020-03-17 04:36:55.000000 biorefineries-2.9.3/biorefineries/lipidcane/_plot_uncertainty.py
--rw-rw-rw-   0        0        0     4563 2020-04-23 23:33:07.000000 biorefineries-2.9.3/biorefineries/lipidcane/chemicals.py
--rw-rw-rw-   0        0        0     4810 2020-02-12 05:47:19.000000 biorefineries-2.9.3/biorefineries/lipidcane/model.py
--rw-rw-rw-   0        0        0     1284 2020-03-12 03:54:41.000000 biorefineries-2.9.3/biorefineries/lipidcane/process_settings.py
--rw-rw-rw-   0        0        0    25861 2020-04-14 19:53:18.000000 biorefineries-2.9.3/biorefineries/lipidcane/system.py
--rw-rw-rw-   0        0        0     3723 2020-03-16 04:14:46.000000 biorefineries-2.9.3/biorefineries/lipidcane/tea.py
-drwxrwxrwx   0        0        0        0 2020-04-24 02:09:59.000000 biorefineries-2.9.3/biorefineries/lipidcane/utils/
--rw-rw-rw-   0        0        0      186 2020-02-06 08:53:58.000000 biorefineries-2.9.3/biorefineries/lipidcane/utils/__init__.py
--rw-rw-rw-   0        0        0     3490 2020-03-10 12:36:05.000000 biorefineries-2.9.3/biorefineries/lipidcane/utils/composition.py
-drwxrwxrwx   0        0        0        0 2020-04-24 02:09:59.000000 biorefineries-2.9.3/biorefineries.egg-info/
--rw-rw-rw-   0        0        0     2999 2020-04-24 02:09:59.000000 biorefineries-2.9.3/biorefineries.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1439 2020-04-24 02:09:59.000000 biorefineries-2.9.3/biorefineries.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-04-24 02:09:59.000000 biorefineries-2.9.3/biorefineries.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2020-04-24 02:09:59.000000 biorefineries-2.9.3/biorefineries.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2020-04-24 02:09:59.000000 biorefineries-2.9.3/biorefineries.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-04-24 02:09:59.000000 biorefineries-2.9.3/setup.cfg
--rw-rw-rw-   0        0        0     1734 2020-04-24 01:50:56.000000 biorefineries-2.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2020-04-24 16:37:27.000000 biorefineries-2.9.4/
+-rw-rw-rw-   0        0        0     2999 2020-04-24 16:37:27.000000 biorefineries-2.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1510 2020-02-05 17:03:42.000000 biorefineries-2.9.4/README.rst
+drwxrwxrwx   0        0        0        0 2020-04-24 16:37:27.000000 biorefineries-2.9.4/biorefineries/
+drwxrwxrwx   0        0        0        0 2020-04-24 16:37:27.000000 biorefineries-2.9.4/biorefineries/cornstover/
+-rw-rw-rw-   0        0        0  3342696 2020-04-14 19:02:05.000000 biorefineries-2.9.4/biorefineries/cornstover/Monte Carlo cornstover.xlsx
+-rw-rw-rw-   0        0        0    12055 2020-04-14 19:02:05.000000 biorefineries-2.9.4/biorefineries/cornstover/Spearman correlation cornstover.xlsx
+-rw-rw-rw-   0        0        0      206 2020-01-24 16:20:24.000000 biorefineries-2.9.4/biorefineries/cornstover/__init__.py
+-rw-rw-rw-   0        0        0      478 2020-04-14 16:09:53.000000 biorefineries-2.9.4/biorefineries/cornstover/_analysis.py
+-rw-rw-rw-   0        0        0    15562 2020-04-03 16:55:37.000000 biorefineries-2.9.4/biorefineries/cornstover/_humbird2011.xlsx
+-rw-rw-rw-   0        0        0     2019 2019-09-27 08:38:09.000000 biorefineries-2.9.4/biorefineries/cornstover/_plot_bars.py
+-rw-rw-rw-   0        0        0     2817 2019-11-18 07:42:30.000000 biorefineries-2.9.4/biorefineries/cornstover/_plot_spearman.py
+-rw-rw-rw-   0        0        0     6662 2019-10-07 11:41:34.000000 biorefineries-2.9.4/biorefineries/cornstover/_plot_uncertainty_bottom.py
+-rw-rw-rw-   0        0        0     8901 2020-04-10 17:38:51.000000 biorefineries-2.9.4/biorefineries/cornstover/_plot_uncertainty_top.py
+-rw-rw-rw-   0        0        0    10211 2020-04-24 16:28:51.000000 biorefineries-2.9.4/biorefineries/cornstover/chemicals.py
+-rw-rw-rw-   0        0        0     3687 2020-02-10 03:04:58.000000 biorefineries-2.9.4/biorefineries/cornstover/model.py
+-rw-rw-rw-   0        0        0     1489 2020-04-10 19:03:12.000000 biorefineries-2.9.4/biorefineries/cornstover/process_settings.py
+-rw-rw-rw-   0        0        0    26955 2020-04-14 19:51:43.000000 biorefineries-2.9.4/biorefineries/cornstover/system.py
+-rw-rw-rw-   0        0        0     3469 2020-04-14 18:34:37.000000 biorefineries-2.9.4/biorefineries/cornstover/tea.py
+-rw-rw-rw-   0        0        0    23874 2020-04-14 17:31:01.000000 biorefineries-2.9.4/biorefineries/cornstover/units.py
+drwxrwxrwx   0        0        0        0 2020-04-24 16:37:27.000000 biorefineries-2.9.4/biorefineries/lipidcane/
+-rw-rw-rw-   0        0        0    16783 2020-04-14 19:53:38.000000 biorefineries-2.9.4/biorefineries/lipidcane/Monte Carlo across lipid fraction.xlsx
+-rw-rw-rw-   0        0        0     6782 2020-04-14 19:53:38.000000 biorefineries-2.9.4/biorefineries/lipidcane/Monte Carlo sugarcane.xlsx
+-rw-rw-rw-   0        0        0     8304 2020-03-04 08:40:33.000000 biorefineries-2.9.4/biorefineries/lipidcane/Spearman correlation lipidcane.xlsx
+-rw-rw-rw-   0        0        0      163 2020-02-06 08:55:18.000000 biorefineries-2.9.4/biorefineries/lipidcane/__init__.py
+-rw-rw-rw-   0        0        0     2297 2020-04-11 21:42:11.000000 biorefineries-2.9.4/biorefineries/lipidcane/_analysis.py
+-rw-rw-rw-   0        0        0     2843 2019-11-18 17:14:19.000000 biorefineries-2.9.4/biorefineries/lipidcane/_plot_spearman.py
+-rw-rw-rw-   0        0        0    11316 2020-03-17 04:36:55.000000 biorefineries-2.9.4/biorefineries/lipidcane/_plot_uncertainty.py
+-rw-rw-rw-   0        0        0     4558 2020-04-24 16:31:18.000000 biorefineries-2.9.4/biorefineries/lipidcane/chemicals.py
+-rw-rw-rw-   0        0        0     4810 2020-02-12 05:47:19.000000 biorefineries-2.9.4/biorefineries/lipidcane/model.py
+-rw-rw-rw-   0        0        0     1284 2020-03-12 03:54:41.000000 biorefineries-2.9.4/biorefineries/lipidcane/process_settings.py
+-rw-rw-rw-   0        0        0    25861 2020-04-14 19:53:18.000000 biorefineries-2.9.4/biorefineries/lipidcane/system.py
+-rw-rw-rw-   0        0        0     3723 2020-03-16 04:14:46.000000 biorefineries-2.9.4/biorefineries/lipidcane/tea.py
+drwxrwxrwx   0        0        0        0 2020-04-24 16:37:27.000000 biorefineries-2.9.4/biorefineries/lipidcane/utils/
+-rw-rw-rw-   0        0        0      186 2020-02-06 08:53:58.000000 biorefineries-2.9.4/biorefineries/lipidcane/utils/__init__.py
+-rw-rw-rw-   0        0        0     3490 2020-03-10 12:36:05.000000 biorefineries-2.9.4/biorefineries/lipidcane/utils/composition.py
+drwxrwxrwx   0        0        0        0 2020-04-24 16:37:27.000000 biorefineries-2.9.4/biorefineries.egg-info/
+-rw-rw-rw-   0        0        0     2999 2020-04-24 16:37:27.000000 biorefineries-2.9.4/biorefineries.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1439 2020-04-24 16:37:27.000000 biorefineries-2.9.4/biorefineries.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-04-24 16:37:27.000000 biorefineries-2.9.4/biorefineries.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2020-04-24 16:37:27.000000 biorefineries-2.9.4/biorefineries.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2020-04-24 16:37:27.000000 biorefineries-2.9.4/biorefineries.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2020-04-24 16:37:27.000000 biorefineries-2.9.4/setup.cfg
+-rw-rw-rw-   0        0        0     1734 2020-04-24 16:31:40.000000 biorefineries-2.9.4/setup.py
```

### Comparing `biorefineries-2.9.3/PKG-INFO` & `biorefineries-2.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: biorefineries
-Version: 2.9.3
+Version: 2.9.4
 Summary: Biorefinery models in BioSTEAM
 Home-page: https://github.com/BioSTEAMDevelopmentGroup/Bioindustrial-Park/tree/master/biorefineries/BioSTEAM 2.x.x/biorefineries
 Author: Yoel Cortes-Pena
 Author-email: yoelcortes@gmail.com
 License: MIT
 Download-URL: https://github.com/BioSTEAMDevelopmentGroup/Bioindustrial-Park/tree/master/biorefineries/BioSTEAM 2.x.x/biorefineries
 Description: =============================================
```

### Comparing `biorefineries-2.9.3/README.rst` & `biorefineries-2.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/cornstover/Monte Carlo cornstover.xlsx` & `biorefineries-2.9.4/biorefineries/cornstover/Monte Carlo cornstover.xlsx`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/cornstover/Spearman correlation cornstover.xlsx` & `biorefineries-2.9.4/biorefineries/cornstover/Spearman correlation cornstover.xlsx`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/cornstover/_humbird2011.xlsx` & `biorefineries-2.9.4/biorefineries/cornstover/_humbird2011.xlsx`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/cornstover/_plot_bars.py` & `biorefineries-2.9.4/biorefineries/cornstover/_plot_bars.py`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/cornstover/_plot_spearman.py` & `biorefineries-2.9.4/biorefineries/cornstover/_plot_spearman.py`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/cornstover/_plot_uncertainty_bottom.py` & `biorefineries-2.9.4/biorefineries/cornstover/_plot_uncertainty_bottom.py`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/cornstover/_plot_uncertainty_top.py` & `biorefineries-2.9.4/biorefineries/cornstover/_plot_uncertainty_top.py`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/cornstover/chemicals.py` & `biorefineries-2.9.4/biorefineries/cornstover/chemicals.py`

 * *Files 12% similar despite different names*

```diff
@@ -105,19 +105,19 @@
 # Will remain in the vapor phase
 extend_single_phase_chemicals(['N2', 'NH3', 'O2', 'CH4', 'H2S', 'SO2'])
 append_single_phase_chemical('CO2')
 
 # Analagous vapors
 append_new_single_phase_chemical('NO2', chems.N2,
                                  formula='NO2',
-                                 MW=46.01, Hf=7925*cal2joule)
+                                 Hf=7925*cal2joule)
 append_new_single_phase_chemical('NO', chems.N2,
                                  formula='NO',
-                                 MW=30.01, Hf=82.05)
-append_single_phase_chemical('CO', 'Carbon monoxide', MW=28.01, Hf=-110.522)
+                                 Hf=82.05)
+append_single_phase_chemical('CO', 'Carbon monoxide', Hf=-110.522)
 
 # Will remain as  solid
 extend_single_phase_chemicals(['Glucose', 'Xylose', 'Sucrose'])
 append_single_phase_chemical('CaSO4')
 
 subgroup = chems['Glucose', 'Xylose', 'Sucrose', 'CaSO4', 'AmmoniumSulfate']
 for chemical in subgroup: set_Cp(chemical, Cp_cellulosic)
@@ -145,48 +145,46 @@
 set_Cp(chems.Lignin, Cp_cellulosic)
 append_chemical_copy('SolubleLignin', chems.Lignin)
 
 # Create structural carbohydrates
 append_chemical_copy('GlucoseOligomer', chems.Glucose)
 set_Cp(chems.GlucoseOligomer, Cp_cellulosic)
 chems.GlucoseOligomer.formula = "C6H10O5"
-chems.GlucoseOligomer.MW = 162.1424
 chems.GlucoseOligomer.Hf = -233200*cal2joule
 
 append_chemical_copy('GalactoseOligomer', chems.GlucoseOligomer)
 append_chemical_copy('MannoseOligomer', chems.GlucoseOligomer)
 append_chemical_copy('XyloseOligomer', chems.Xylose)
 set_Cp(chems.XyloseOligomer, Cp_cellulosic)
 chems.XyloseOligomer.formula = "C5H8O4"
-chems.XyloseOligomer.MW = 132.11612
 chems.XyloseOligomer.Hf = -182100*cal2joule
 
 append_chemical_copy('ArabinoseOligomer', chems.XyloseOligomer)
 
 # Other
 append_new_single_phase_chemical('Z_mobilis', formula="CH1.8O0.5N0.2",
-                                 MW=24.6265, Hf=-31169.39*cal2joule)
+                                 Hf=-31169.39*cal2joule)
 append_new_single_phase_chemical('T_reesei', formula="CH1.645O0.445N0.205S0.005",
-                                 MW=23.8204, Hf=-23200.01*cal2joule)
+                                 Hf=-23200.01*cal2joule)
 append_new_single_phase_chemical('Biomass', formula="CH1.64O0.39N0.23S0.0035",
-                                 MW=23.238, Hf=-23200.01*cal2joule)
+                                 Hf=-23200.01*cal2joule)
 append_new_single_phase_chemical('Cellulose', formula="C6H10O5", # Glucose monomer minus water
-                                 MW=162.1406, Hf=-233200.06*cal2joule)
+                                 Hf=-233200.06*cal2joule)
 append_new_single_phase_chemical('Protein', formula="CH1.57O0.31N0.29S0.007",
-                                 MW=22.8396, Hf=-17618*cal2joule)
+                                 Hf=-17618*cal2joule)
 append_new_single_phase_chemical('Enzyme', formula="CH1.59O0.42N0.24S0.01",
-                                 MW=24.0156, Hf=-17618*cal2joule)
+                                 Hf=-17618*cal2joule)
 append_new_single_phase_chemical('Glucan', formula='C6H10O5',
-                                 MW=162.14, Hf=-233200*cal2joule)
+                                 Hf=-233200*cal2joule)
 append_new_single_phase_chemical('Xylan', formula="C5H8O4",
-                                 MW=132.12, Hf=-182100*cal2joule)
+                                 Hf=-182100*cal2joule)
 append_new_single_phase_chemical('Xylitol', formula="C5H12O5",
-                                 MW=152.15, Hf=-243145*cal2joule)
+                                 Hf=-243145*cal2joule)
 append_new_single_phase_chemical('Cellobiose', formula="C12H22O11",
-                                 MW=342.30, Hf=-480900*cal2joule)
+                                 Hf=-480900*cal2joule)
 append_new_single_phase_chemical('CSL', MW=1,
                                  Hf=(chems.Protein.Hf/4
                                      + chems.Water.Hf/2
                                      + chems.LacticAcid.Hf/4))
 append_chemical_copy('DenaturedEnzyme', chems.Enzyme)
 append_chemical_copy('Arabinan', chems.Xylan)
 append_chemical_copy('Mannan',   chems.Glucan)
@@ -194,17 +192,14 @@
 
 # %% TODO: Maybe remove this
 
 # For waste water
 append_chemical_copy('WWTsludge', chems.Biomass)
 append_chemical_copy('Cellulase', chems.Enzyme)
 
-for i in chems: 
-    if i.formula: i.reset_combustion_data()
-
 # %% Grouped chemicals
 
 chemical_groups = dict(
     OtherSugars = ('Arabinose',
                    'Mannose',
                    'Galactose',
                    'Cellobiose',
```

### Comparing `biorefineries-2.9.3/biorefineries/cornstover/model.py` & `biorefineries-2.9.4/biorefineries/cornstover/model.py`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/cornstover/process_settings.py` & `biorefineries-2.9.4/biorefineries/cornstover/process_settings.py`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/cornstover/system.py` & `biorefineries-2.9.4/biorefineries/cornstover/system.py`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/cornstover/tea.py` & `biorefineries-2.9.4/biorefineries/cornstover/tea.py`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/cornstover/units.py` & `biorefineries-2.9.4/biorefineries/cornstover/units.py`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/lipidcane/Monte Carlo across lipid fraction.xlsx` & `biorefineries-2.9.4/biorefineries/lipidcane/Monte Carlo across lipid fraction.xlsx`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/lipidcane/Monte Carlo sugarcane.xlsx` & `biorefineries-2.9.4/biorefineries/lipidcane/Monte Carlo sugarcane.xlsx`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/lipidcane/Spearman correlation lipidcane.xlsx` & `biorefineries-2.9.4/biorefineries/lipidcane/Spearman correlation lipidcane.xlsx`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/lipidcane/_analysis.py` & `biorefineries-2.9.4/biorefineries/lipidcane/_analysis.py`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/lipidcane/_plot_spearman.py` & `biorefineries-2.9.4/biorefineries/lipidcane/_plot_spearman.py`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/lipidcane/_plot_uncertainty.py` & `biorefineries-2.9.4/biorefineries/lipidcane/_plot_uncertainty.py`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/lipidcane/chemicals.py` & `biorefineries-2.9.4/biorefineries/lipidcane/chemicals.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,16 +102,15 @@
 CaO.Cn.add_model(1.02388 * CaO.MW) 
 Cellulose.Cn.add_model(1.364 * Cellulose.MW) 
 Hemicellulose.Cn.add_model(1.364 * Hemicellulose.MW)
 Flocculant.Cn.add_model(4.184 * Flocculant.MW)
 Lignin.Cn.add_model(1.364 * Lignin.MW)
 Solids.Cn.add_model(1.100 * Solids.MW)
 
-for chemical in lipidcane_chemicals:
-    chemical.default()
+for chemical in lipidcane_chemicals: chemical.default()
 
 lipidcane_chemicals.compile()
 lipidcane_chemicals.set_synonym('Water', 'H2O')
 
 pretreatment_chemicals = lipidcane_chemicals.subgroup(
     ['Lipid', 'Ash', 'Cellulose',
      'Flocculant', 'Hemicellulose',
```

### Comparing `biorefineries-2.9.3/biorefineries/lipidcane/model.py` & `biorefineries-2.9.4/biorefineries/lipidcane/model.py`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/lipidcane/process_settings.py` & `biorefineries-2.9.4/biorefineries/lipidcane/process_settings.py`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/lipidcane/system.py` & `biorefineries-2.9.4/biorefineries/lipidcane/system.py`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/lipidcane/tea.py` & `biorefineries-2.9.4/biorefineries/lipidcane/tea.py`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries/lipidcane/utils/composition.py` & `biorefineries-2.9.4/biorefineries/lipidcane/utils/composition.py`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/biorefineries.egg-info/PKG-INFO` & `biorefineries-2.9.4/biorefineries.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: biorefineries
-Version: 2.9.3
+Version: 2.9.4
 Summary: Biorefinery models in BioSTEAM
 Home-page: https://github.com/BioSTEAMDevelopmentGroup/Bioindustrial-Park/tree/master/biorefineries/BioSTEAM 2.x.x/biorefineries
 Author: Yoel Cortes-Pena
 Author-email: yoelcortes@gmail.com
 License: MIT
 Download-URL: https://github.com/BioSTEAMDevelopmentGroup/Bioindustrial-Park/tree/master/biorefineries/BioSTEAM 2.x.x/biorefineries
 Description: =============================================
```

### Comparing `biorefineries-2.9.3/biorefineries.egg-info/SOURCES.txt` & `biorefineries-2.9.4/biorefineries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biorefineries-2.9.3/setup.py` & `biorefineries-2.9.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from setuptools import setup
 
 setup(
     name='biorefineries',
     packages=['biorefineries'],
     license='MIT',
-    version='2.9.3',
+    version='2.9.4',
     description="Biorefinery models in BioSTEAM",
     long_description=open('README.rst').read(),
     author='Yoel Cortes-Pena',
     install_requires=['biosteam>=2.13.0',
                       'lazypkg==1.4'],
     python_requires=">=3.6",
     package_data=
```

