# Comparing `tmp/EzGM-1.6.6.2.tar.gz` & `tmp/EzGM-1.6.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EzGM-1.6.6.2.tar", last modified: Tue Jun 13 08:43:19 2023, max compression
+gzip compressed data, was "EzGM-1.6.6.3.tar", last modified: Thu Jun 15 07:59:34 2023, max compression
```

## Comparing `EzGM-1.6.6.2.tar` & `EzGM-1.6.6.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 08:43:19.911844 EzGM-1.6.6.2/
-drwxrwxrwx   0        0        0        0 2023-06-13 08:43:19.889760 EzGM-1.6.6.2/EzGM/
--rw-rw-rw-   0        0        0      105 2022-10-20 15:03:59.000000 EzGM-1.6.6.2/EzGM/__init__.py
--rw-rw-rw-   0        0        0   180770 2023-06-01 20:34:44.000000 EzGM-1.6.6.2/EzGM/selection.py
--rw-rw-rw-   0        0        0    22786 2023-06-01 17:18:21.000000 EzGM-1.6.6.2/EzGM/signal.py
--rw-rw-rw-   0        0        0    55844 2023-06-01 17:20:06.000000 EzGM-1.6.6.2/EzGM/utility.py
--rw-rw-rw-   0        0        0    26111 2023-06-01 20:23:19.000000 EzGM-1.6.6.2/EzGM/webdriverdownloader.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:43:19.910848 EzGM-1.6.6.2/EzGM.egg-info/
--rw-rw-rw-   0        0        0     6801 2023-06-13 08:43:19.000000 EzGM-1.6.6.2/EzGM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-06-13 08:43:19.000000 EzGM-1.6.6.2/EzGM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 08:43:19.000000 EzGM-1.6.6.2/EzGM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2023-06-13 08:43:19.000000 EzGM-1.6.6.2/EzGM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-13 08:43:19.000000 EzGM-1.6.6.2/EzGM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2022-10-20 15:03:59.000000 EzGM-1.6.6.2/LICENSE
--rw-rw-rw-   0        0        0     6801 2023-06-13 08:43:19.911844 EzGM-1.6.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     6174 2023-03-09 12:54:15.000000 EzGM-1.6.6.2/README.md
--rw-rw-rw-   0        0        0      108 2022-10-20 15:03:59.000000 EzGM-1.6.6.2/pyproject.toml
--rw-rw-rw-   0        0        0      893 2023-06-13 08:43:19.913845 EzGM-1.6.6.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-15 07:59:34.541960 EzGM-1.6.6.3/
+drwxrwxrwx   0        0        0        0 2023-06-15 07:59:34.499436 EzGM-1.6.6.3/EzGM/
+-rw-rw-rw-   0        0        0      105 2022-10-20 15:03:59.000000 EzGM-1.6.6.3/EzGM/__init__.py
+-rw-rw-rw-   0        0        0   180460 2023-06-15 07:17:54.000000 EzGM-1.6.6.3/EzGM/selection.py
+-rw-rw-rw-   0        0        0    22786 2023-06-01 17:18:21.000000 EzGM-1.6.6.3/EzGM/signal.py
+-rw-rw-rw-   0        0        0    55186 2023-06-15 07:54:21.000000 EzGM-1.6.6.3/EzGM/utility.py
+-rw-rw-rw-   0        0        0    26111 2023-06-01 20:23:19.000000 EzGM-1.6.6.3/EzGM/webdriverdownloader.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:59:34.540960 EzGM-1.6.6.3/EzGM.egg-info/
+-rw-rw-rw-   0        0        0     6801 2023-06-15 07:59:34.000000 EzGM-1.6.6.3/EzGM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-06-15 07:59:34.000000 EzGM-1.6.6.3/EzGM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 07:59:34.000000 EzGM-1.6.6.3/EzGM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2023-06-15 07:59:34.000000 EzGM-1.6.6.3/EzGM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-15 07:59:34.000000 EzGM-1.6.6.3/EzGM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2022-10-20 15:03:59.000000 EzGM-1.6.6.3/LICENSE
+-rw-rw-rw-   0        0        0     6801 2023-06-15 07:59:34.543081 EzGM-1.6.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6174 2023-03-09 12:54:15.000000 EzGM-1.6.6.3/README.md
+-rw-rw-rw-   0        0        0      108 2022-10-20 15:03:59.000000 EzGM-1.6.6.3/pyproject.toml
+-rw-rw-rw-   0        0        0      893 2023-06-15 07:59:34.553099 EzGM-1.6.6.3/setup.cfg
```

### Comparing `EzGM-1.6.6.2/EzGM/selection.py` & `EzGM-1.6.6.3/EzGM/selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -455,19 +455,14 @@
         plt.rc('font', size=SMALL_SIZE)  # controls default text sizes
         plt.rc('axes', titlesize=SMALL_SIZE)  # fontsize of the axes title
         plt.rc('axes', labelsize=BIG_SIZE)  # fontsize of the x and y labels
         plt.rc('xtick', labelsize=SMALL_SIZE)  # fontsize of the tick labels
         plt.rc('ytick', labelsize=SMALL_SIZE)  # fontsize of the tick labels
         plt.rc('legend', fontsize=MEDIUM_SIZE)  # legend fontsize
         plt.rc('figure', titlesize=BIGGER_SIZE)  # fontsize of the figure title
-        plt.rc('font', **{'family': 'serif', 'serif': ['Times New Roman']})
-        plt.rcParams['mathtext.it']= 'Times New Roman:italic'
-        plt.rcParams['mathtext.cal']= 'Times New Roman:italic'
-        plt.rcParams['mathtext.default'] = 'regular'
-        plt.rcParams["mathtext.fontset"] ='custom'
         plt.ioff()
 
         if type(self).__name__ == 'conditional_spectrum':
 
             # xticks and yticks to use for plotting
             xticks = [self.T[0]]
             for x in [0.01, 0.1, 0.2, 0.5, 1, 2, 4, 7, 10]:
```

### Comparing `EzGM-1.6.6.2/EzGM/signal.py` & `EzGM-1.6.6.3/EzGM/signal.py`

 * *Files identical despite different names*

### Comparing `EzGM-1.6.6.2/EzGM/utility.py` & `EzGM-1.6.6.3/EzGM/utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,20 +52,14 @@
         flag to show figure (1 or 0)
 
     Returns
     -------
     None.
     """
 
-    plt.rc('font', **{'family': 'serif', 'serif': ['Times New Roman']})
-    plt.rcParams['mathtext.it']= 'Times New Roman:italic'
-    plt.rcParams['mathtext.cal']= 'Times New Roman:italic'
-    plt.rcParams['mathtext.default'] = 'regular'
-    plt.rcParams["mathtext.fontset"] ='custom'
-
     # Initialise some lists
     lat = []
     lon = []
     im = []
     iml_data = []
     poe_data = []
     id_no = []
@@ -180,27 +174,24 @@
         flag to show figure (1 or 0)
 
     Returns
     -------
     None.
     """
 
-    plt.rc('font', **{'family': 'serif', 'serif': ['Times New Roman']})
-    plt.rcParams['mathtext.it']= 'Times New Roman:italic'
-    plt.rcParams['mathtext.cal']= 'Times New Roman:italic'
-    plt.rcParams['mathtext.default'] = 'regular'
-    plt.rcParams["mathtext.fontset"] ='custom'
-
     # lets add the plotting options to make everything clearer
     cmap = cm.get_cmap('jet')  # Get desired colormap
 
     for file in os.listdir(path_disagg_results):
         if file.startswith(filename) and 'Mag_Dist_Eps' not in file:
             # Load the dataframe
             df = pd.read_csv(''.join([path_disagg_results, '/', file]), skiprows=1)
+            for key in df.keys():
+                if key.startswith('rlz'):
+                    hz_key = key
             poes = np.unique(df['poe']).tolist()
             poes.sort(reverse=True)
             # Get some salient values
             f = open(''.join([path_disagg_results, '/', file]), "r")
             ff = f.readline().split(',')
             lon = float(list(filter(lambda x: 'lon=' in x, ff))[0].replace(" lon=", ""))
             lat = float(list(filter(lambda x: 'lat=' in x, ff))[0].replace(" lat=", "").replace("\"\n", ""))
@@ -212,15 +203,15 @@
                 Tr = []
                 modeLst, meanLst = [], []
                 for poe in poes:
                     Tr.append(round(-inv_t / np.log(1 - poe)))
                     data = {}
                     data['mag'] = df['mag'][(df['poe'] == poe) & (df['imt'] == imt)]
                     data['dist'] = df['dist'][(df['poe'] == poe) & (df['imt'] == imt)]
-                    data['hz_cont'] = df.iloc[:, 4][(df['poe'] == poe) & (df['imt'] == imt)]
+                    data['hz_cont'] = df[hz_key][(df['poe'] == poe) & (df['imt'] == imt)]
                     hz_cont.append(data['hz_cont'] / data['hz_cont'].sum())
                     data['hz_cont'] = hz_cont[-1]
                     data = pd.DataFrame(data)
                     # Compute the modal values (highest hazard contribution)
                     mode = data.sort_values(by='hz_cont', ascending=False)[0:1]
                     modeLst.append([mode['mag'].values[0], mode['dist'].values[0]])
                     # Compute the mean value
@@ -328,30 +319,27 @@
         flag to show figure (1 or 0)
 
     Returns
     -------
     None.
     """
 
-    plt.rc('font', **{'family': 'serif', 'serif': ['Times New Roman']})
-    plt.rcParams['mathtext.it']= 'Times New Roman:italic'
-    plt.rcParams['mathtext.cal']= 'Times New Roman:italic'
-    plt.rcParams['mathtext.default'] = 'regular'
-    plt.rcParams["mathtext.fontset"] ='custom'
-
     # lets add the plotting options to make everything clearer
     cmap = cm.get_cmap('jet')  # Get desired colormap
 
     mags = []
     dists = []
 
     for file in os.listdir(path_disagg_results):
         if file.startswith(filename):
             # Load the dataframe
             df = pd.read_csv(''.join([path_disagg_results, '/', file]), skiprows=1)
+            for key in df.keys():
+                if key.startswith('rlz'):
+                    hz_key = key
             poes = np.unique(df['poe']).tolist()
             poes.sort(reverse=True)
             # Get some salient values
             f = open(''.join([path_disagg_results, '/', file]), "r")
             ff = f.readline().split(',')
             lon = float(list(filter(lambda x: 'lon=' in x, ff))[0].replace(" lon=", ""))
             lat = float(list(filter(lambda x: 'lat=' in x, ff))[0].replace(" lat=", "").replace("\"\n", ""))
@@ -364,15 +352,15 @@
                 M, R, eps = [], [], []
                 for poe in poes:
                     Tr.append(round(-inv_t / np.log(1 - poe)))
                     data = {}
                     data['mag'] = df['mag'][(df['poe'] == poe) & (df['imt'] == imt)]
                     data['dist'] = df['dist'][(df['poe'] == poe) & (df['imt'] == imt)]
                     data['eps'] = df['eps'][(df['poe'] == poe) & (df['imt'] == imt)]
-                    data['hz_cont'] = df.iloc[:, 5][(df['poe'] == poe) & (df['imt'] == imt)]
+                    data['hz_cont'] = df[hz_key][(df['poe'] == poe) & (df['imt'] == imt)]
                     hz_cont.append(np.array(data['hz_cont'] / data['hz_cont'].sum()))
                     data['hz_cont'] = hz_cont[-1]
                     data = pd.DataFrame(data)
                     data_reduced = data.groupby(['mag', 'dist']).agg(['sum'])[('hz_cont', 'sum')].reset_index().droplevel(1, axis=1)
                     # Compute the modal value (highest poe)
                     mode = data_reduced.sort_values(by='hz_cont', ascending=False)[0:1]
                     modeLst.append([mode['mag'].values[0], mode['dist'].values[0]])
```

### Comparing `EzGM-1.6.6.2/EzGM/webdriverdownloader.py` & `EzGM-1.6.6.3/EzGM/webdriverdownloader.py`

 * *Files identical despite different names*

### Comparing `EzGM-1.6.6.2/EzGM.egg-info/PKG-INFO` & `EzGM-1.6.6.3/EzGM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EzGM
-Version: 1.6.6.2
+Version: 1.6.6.3
 Summary: Toolbox for ground motion record selection and processing
 Home-page: https://github.com/volkanozsarac/EzGM
 Author: Volkan Ozsarac
 Author-email: volkan.ozsarac@iusspavia.it
 Project-URL: Bug Tracker, https://github.com/volkanozsarac/EzGM/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `EzGM-1.6.6.2/LICENSE` & `EzGM-1.6.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `EzGM-1.6.6.2/PKG-INFO` & `EzGM-1.6.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EzGM
-Version: 1.6.6.2
+Version: 1.6.6.3
 Summary: Toolbox for ground motion record selection and processing
 Home-page: https://github.com/volkanozsarac/EzGM
 Author: Volkan Ozsarac
 Author-email: volkan.ozsarac@iusspavia.it
 Project-URL: Bug Tracker, https://github.com/volkanozsarac/EzGM/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `EzGM-1.6.6.2/README.md` & `EzGM-1.6.6.3/README.md`

 * *Files identical despite different names*

### Comparing `EzGM-1.6.6.2/setup.cfg` & `EzGM-1.6.6.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2045 7a47 4d0d 0a76 6572 7369 6f6e   = EzGM..version
-00000020: 203d 2031 2e36 2e36 2e32 0d0a 6175 7468   = 1.6.6.2..auth
+00000020: 203d 2031 2e36 2e36 2e33 0d0a 6175 7468   = 1.6.6.3..auth
 00000030: 6f72 203d 2056 6f6c 6b61 6e20 4f7a 7361  or = Volkan Ozsa
 00000040: 7261 630d 0a61 7574 686f 725f 656d 6169  rac..author_emai
 00000050: 6c20 3d20 766f 6c6b 616e 2e6f 7a73 6172  l = volkan.ozsar
 00000060: 6163 4069 7573 7370 6176 6961 2e69 740d  ac@iusspavia.it.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2054  .description = T
 00000080: 6f6f 6c62 6f78 2066 6f72 2067 726f 756e  oolbox for groun
 00000090: 6420 6d6f 7469 6f6e 2072 6563 6f72 6420  d motion record
```

