# Comparing `tmp/decodanda-0.6.4.tar.gz` & `tmp/decodanda-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decodanda-0.6.4.tar", last modified: Wed Apr 26 18:03:23 2023, max compression
+gzip compressed data, was "decodanda-0.6.5.tar", last modified: Thu Jun 15 20:54:12 2023, max compression
```

## Comparing `decodanda-0.6.4.tar` & `decodanda-0.6.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-26 18:03:23.321115 decodanda-0.6.4/
--rw-r--r--   0 lorenzo    (501) staff       (20)    35149 2023-02-15 23:52:18.000000 decodanda-0.6.4/LICENSE.md
--rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-04-26 18:03:23.320786 decodanda-0.6.4/PKG-INFO
--rw-r--r--   0 lorenzo    (501) staff       (20)    36482 2023-04-19 18:21:22.000000 decodanda-0.6.4/README.md
-drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-26 18:03:23.317613 decodanda-0.6.4/decodanda/
--rw-r--r--   0 lorenzo    (501) staff       (20)      251 2023-02-17 22:21:32.000000 decodanda-0.6.4/decodanda/__init__.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    98954 2023-04-26 18:00:57.000000 decodanda-0.6.4/decodanda/classes.py
--rw-r--r--   0 lorenzo    (501) staff       (20)     1194 2023-02-15 00:18:50.000000 decodanda-0.6.4/decodanda/imports.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    11247 2023-02-17 19:33:24.000000 decodanda-0.6.4/decodanda/in_time.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    39339 2023-02-17 17:08:36.000000 decodanda-0.6.4/decodanda/utilities.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    24405 2023-04-26 17:59:31.000000 decodanda-0.6.4/decodanda/visualize.py
-drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-26 18:03:23.320340 decodanda-0.6.4/decodanda.egg-info/
--rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-04-26 18:03:23.000000 decodanda-0.6.4/decodanda.egg-info/PKG-INFO
--rw-r--r--   0 lorenzo    (501) staff       (20)      324 2023-04-26 18:03:23.000000 decodanda-0.6.4/decodanda.egg-info/SOURCES.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)        1 2023-04-26 18:03:23.000000 decodanda-0.6.4/decodanda.egg-info/dependency_links.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)      109 2023-04-26 18:03:23.000000 decodanda-0.6.4/decodanda.egg-info/requires.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)       10 2023-04-26 18:03:23.000000 decodanda-0.6.4/decodanda.egg-info/top_level.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)       38 2023-04-26 18:03:23.321233 decodanda-0.6.4/setup.cfg
--rw-r--r--   0 lorenzo    (501) staff       (20)     1388 2023-04-26 18:01:26.000000 decodanda-0.6.4/setup.py
+drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-06-15 20:54:12.589273 decodanda-0.6.5/
+-rw-r--r--   0 lorenzo    (501) staff       (20)    35149 2023-02-15 23:52:18.000000 decodanda-0.6.5/LICENSE.md
+-rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-06-15 20:54:12.588648 decodanda-0.6.5/PKG-INFO
+-rw-r--r--   0 lorenzo    (501) staff       (20)    36482 2023-04-19 18:21:22.000000 decodanda-0.6.5/README.md
+drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-06-15 20:54:12.583535 decodanda-0.6.5/decodanda/
+-rw-r--r--   0 lorenzo    (501) staff       (20)      251 2023-02-17 22:21:32.000000 decodanda-0.6.5/decodanda/__init__.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)   101066 2023-06-15 20:52:53.000000 decodanda-0.6.5/decodanda/classes.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)     1194 2023-02-15 00:18:50.000000 decodanda-0.6.5/decodanda/imports.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    11247 2023-02-17 19:33:24.000000 decodanda-0.6.5/decodanda/in_time.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    40617 2023-06-08 16:31:08.000000 decodanda-0.6.5/decodanda/utilities.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    24405 2023-04-26 17:59:31.000000 decodanda-0.6.5/decodanda/visualize.py
+drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-06-15 20:54:12.587949 decodanda-0.6.5/decodanda.egg-info/
+-rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-06-15 20:54:12.000000 decodanda-0.6.5/decodanda.egg-info/PKG-INFO
+-rw-r--r--   0 lorenzo    (501) staff       (20)      324 2023-06-15 20:54:12.000000 decodanda-0.6.5/decodanda.egg-info/SOURCES.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)        1 2023-06-15 20:54:12.000000 decodanda-0.6.5/decodanda.egg-info/dependency_links.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)      109 2023-06-15 20:54:12.000000 decodanda-0.6.5/decodanda.egg-info/requires.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)       10 2023-06-15 20:54:12.000000 decodanda-0.6.5/decodanda.egg-info/top_level.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)       38 2023-06-15 20:54:12.589463 decodanda-0.6.5/setup.cfg
+-rw-r--r--   0 lorenzo    (501) staff       (20)     1388 2023-06-15 20:53:07.000000 decodanda-0.6.5/setup.py
```

### Comparing `decodanda-0.6.4/LICENSE.md` & `decodanda-0.6.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.4/PKG-INFO` & `decodanda-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decodanda
-Version: 0.6.4
+Version: 0.6.5
 Summary: A python package for neural decoding with built-in best practices.
 Home-page: https://github.com/lposani/decodanda
 Author: Lorenzo Posani
 Author-email: lorenzo.posani@gmail.com
 Keywords: python,decoding,neuroscience,ccgp,neural activity,population activity,neural decoding,geometry
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `decodanda-0.6.4/README.md` & `decodanda-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.4/decodanda/classes.py` & `decodanda-0.6.5/decodanda/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -412,14 +412,43 @@
                     self.decoding_weights_null[dic_key] = []
                 self.decoding_weights_null[dic_key].append(self.classifier.coef_)
 
         performance = self._test(testing_array_A, testing_array_B, label_A, label_B)
 
         return performance
 
+    # Sampling functions
+
+    def balanced_resample(self, ndata=None):
+        """
+
+        Parameters
+        ----------
+        ndata: optional, number of resampled activity vectors per condition. If not specified,
+        the maximum number of activity vectors across all conditions is used.
+
+        Returns
+        -------
+        balanced resampled rasters
+        """
+        if ndata is None:
+            ndata = self._max_conditioned_data
+
+        resampled_rasters = {}
+        for key in self.conditioned_rasters:
+            condition_key = self._semantic_vectors[key]
+            resampled_rasters[condition_key] = []
+            for n in range(self.n_brains):
+                x = self.conditioned_rasters[key][n]
+                sampling_index = np.random.randint(0, x.shape[0], ndata)
+                resampled_rasters[condition_key].append(x[sampling_index])
+            resampled_rasters[condition_key] = np.hstack(resampled_rasters[condition_key])
+
+        return resampled_rasters
+
     # Dichotomy analysis functions
 
     def decode_dichotomy(self, dichotomy: Union[str, list], training_fraction: float,
                          cross_validations: int = 10, ndata: Optional[int] = None,
                          shuffled: bool = False, parallel: bool = False,
                          testing_trials: Optional[list] = None,
                          dic_key: Optional[str] = None, **kwargs) -> ndarray:
@@ -525,23 +554,32 @@
             log_dichotomy(self, dic, ndata, 'Decoding')
             count = tqdm(range(cross_validations))
         else:
             count = range(cross_validations)
 
         if parallel:
             pool = Pool()
-            performances = pool.map(CrossValidator(classifier=self.classifier,
-                                                   conditioned_rasters=self.conditioned_rasters,
-                                                   conditioned_trial_index=self.conditioned_trial_index,
-                                                   dic=dic,
-                                                   training_fraction=training_fraction,
-                                                   ndata=ndata,
-                                                   subset=self.subset,
-                                                   semantic_vectors=self._semantic_vectors),
-                                    range(cross_validations))
+            res = pool.map(CrossValidator(classifier=self.classifier,
+                                          conditioned_rasters=self.conditioned_rasters,
+                                          conditioned_trial_index=self.conditioned_trial_index,
+                                          dic=dic,
+                                          training_fraction=training_fraction,
+                                          ndata=ndata,
+                                          subset=self.subset,
+                                          semantic_vectors=self._semantic_vectors,
+                                          z_score=self._zscore,
+                                          dic_key=dic_key),
+                           range(cross_validations))
+            performances = np.asarray([r[0] for r in res])
+
+            if len(res[0][1]):
+                key = list(res[0][1].keys())[0]
+                weights = {key: [r[1][key] for r in res]}
+
+            print(performances, weights)
 
         else:
             performances = np.zeros(cross_validations)
             if self._verbose and not shuffled:
                 print('\nLooping over decoding cross validation folds:')
             for i in count:
                 performances[i] = self._one_cv_step(dic=dic, training_fraction=training_fraction, ndata=ndata,
@@ -551,15 +589,16 @@
             self._order_conditioned_rasters()
         return np.asarray(performances)
 
     def CCGP_dichotomy(self, dichotomy: Union[str, list],
                        resamplings: int = 3,
                        ndata: Optional[int] = None,
                        max_semantic_dist: int = 1,
-                       shuffled: bool = False):
+                       shuffled: bool = False,
+                       **kwargs):
         """
         Function that performs the cross-condition generalization performance analysis (CCGP, Bernardi et al. 2020, Cell)
         for a given variable, specified through its corresponding dichotomy. This function tests how well a given
         coding strategy for the given variable generalizes when the other variables are changed.
 
 
         Parameters
@@ -698,15 +737,16 @@
                             rotation_B = np.arange(testing_array_B.shape[1]).astype(int)
                             np.random.shuffle(rotation_A)
                             np.random.shuffle(rotation_B)
                             testing_array_A = testing_array_A[:, rotation_A]
                             testing_array_B = testing_array_B[:, rotation_A]
 
                         if self._zscore:
-                            big_raster = np.vstack([training_array_A, training_array_B])  # z-scoring using the training data
+                            big_raster = np.vstack(
+                                [training_array_A, training_array_B])  # z-scoring using the training data
                             big_mean = np.nanmean(big_raster, 0)
                             big_std = np.nanstd(big_raster, 0)
                             big_std[big_std == 0] = np.inf
                             training_array_A = (training_array_A - big_mean) / big_std
                             training_array_B = (training_array_B - big_mean) / big_std
                             testing_array_A = (testing_array_A - big_mean) / big_std
                             testing_array_B = (testing_array_B - big_mean) / big_std
@@ -787,15 +827,16 @@
                               cross_validations: int = 10,
                               nshuffles: int = 10,
                               ndata: Optional[int] = None,
                               parallel: bool = False,
                               return_CV: bool = False,
                               testing_trials: Optional[list] = None,
                               plot: bool = False,
-                              dic_key: Optional[str] = None) -> Tuple[Union[list, ndarray], ndarray]:
+                              dic_key: Optional[str] = None,
+                              **kwargs) -> Tuple[Union[list, ndarray], ndarray]:
         """
         Function that performs cross-validated decoding of a specific dichotomy and compares the resulting values with
         a null model where the relationship between the neural data and the two sides of the dichotomy is
         shuffled.
 
         Decoding is performed by sampling a balanced amount of data points from each condition in each class of the
         dichotomy, so to ensure that only the desired variable is analyzed by balancing confounds.
@@ -922,30 +963,32 @@
         for n in count:
             performances = self.decode_dichotomy(dichotomy=dic,
                                                  training_fraction=training_fraction,
                                                  cross_validations=cross_validations,
                                                  ndata=ndata,
                                                  parallel=parallel,
                                                  testing_trials=testing_trials,
-                                                 shuffled=True)
+                                                 shuffled=True,
+                                                 dic_key=dic_key)
 
             null_model_performances[n] = np.nanmean(performances)
 
         if plot:
             visualize_decoding(self, dic, d_performances, null_model_performances,
                                training_fraction=training_fraction, ndata=ndata, testing_trials=testing_trials)
 
         return data_performance, null_model_performances
 
     def CCGP_with_nullmodel(self, dichotomy: Union[str, list],
                             resamplings: int = 5,
                             nshuffles: int = 25,
                             ndata: Optional[int] = None,
                             max_semantic_dist: int = 1,
-                            return_combinations: bool = False):
+                            return_combinations: bool = False,
+                            **kwargs):
 
         """
                 Function that performs the cross-condition generalization performance analysis (CCGP, Bernardi et al. 2020, Cell)
                 for a given variable, specified through its corresponding dichotomy.
 
                     This function tests how well a given coding strategy for the given variable generalizes
                 when the other variables are changed and compares the
@@ -1061,15 +1104,16 @@
 
         return ccgp, shuffled_ccgp
 
     def PS_with_nullmodel(self, dichotomy: Union[str, list],
                           nshuffles: int = 25,
                           max_semantic_dist: int = 1,
                           method: str = 'pearson',
-                          return_combinations: bool = False):
+                          return_combinations: bool = False,
+                          **kwargs):
 
         scores = self.parallelism_score_dichotomy(dichotomy=dichotomy,
                                                   method=method,
                                                   max_semantic_dist=max_semantic_dist,
                                                   return_combinations=return_combinations)
 
         if self._verbose and nshuffles:
@@ -1579,15 +1623,15 @@
                 # select bins conditioned on the semantic behavioural vector
                 conditioned_raster = array[mask, :]
 
                 # Define trial logic
                 def condition_no(cond):
                     no = 0
                     for i in range(len(cond)):
-                        no += cond[i] * 10 ** (i + 2)
+                        no += cond[i] * 10 ** (i + 3)
                     return no
 
                 if self._trial_attr is not None:
                     conditioned_trial = getattr(session, self._trial_attr)[mask]
                 elif self._trial_chunk is None:
                     if self._verbose:
                         print('[Decodanda]\tUsing contiguous chunks of the same labels as trials.')
@@ -1628,17 +1672,20 @@
 
                 if self._verbose:
                     semantic_vector_string = []
                     for i, sk in enumerate(self._semantic_keys):
                         semantic_values = list(self.conditions[sk])
                         semantic_vector_string.append("%s = %s" % (sk, semantic_values[condition_vec[i]]))
                     semantic_vector_string = ', '.join(semantic_vector_string)
-                    print("\t\t\t(%s):\tSelected %u time bin out of %u, divided into %u trials "
-                          % (semantic_vector_string, conditioned_raster.shape[0], len(array),
-                             len(np.unique(conditioned_trial))))
+                    if len(conditioned_raster):
+                        print("\t\t\t(%s):\tSelected %u time bin out of %u, divided into %u trials - %u neurons"
+                              % (semantic_vector_string, conditioned_raster.shape[0], len(array),
+                                 len(np.unique(conditioned_trial)), conditioned_raster.shape[1]))
+                    else:
+                        print("\t\t\t(%s):\tNo data found" % semantic_vector_string)
 
             session_conditioned_data = [r.shape[0] for r in list(session_conditioned_rasters.values())]
             session_conditioned_trials = [len(np.unique(c)) for c in list(session_conditioned_trial_index.values())]
 
             self._max_conditioned_data = max([self._max_conditioned_data, np.max(session_conditioned_data)])
             self._min_conditioned_data = min([self._min_conditioned_data, np.min(session_conditioned_data)])
 
@@ -1909,14 +1956,18 @@
                 if self._debug:
                     print(k, 'raster %u:' % i, np.unique(ti).shape[0])
                     print(ti)
                 if np.unique(ti).shape[0] < 2:
                     return False
         return True
 
+    def _reset_weight_arrays(self):
+        self.decoding_weights = {}
+        self.decoding_weights_null = {}
+
 
 # Wrapper for decoding
 
 def decoding_analysis(data, conditions, decodanda_params, analysis_params, parallel=False, plot=False, ax=None):
     """
     Function that performs a balanced decoding analyses of the
     data set passed in the ``data`` argument, using variables and values
@@ -2098,18 +2149,22 @@
         self.analysis_params = analysis_params
 
     def __call__(self, i):
         self.i = i
         self.randomstate = RandomState(i)
         dec = Decodanda(data=self.data, conditions=self.conditions, **self.decodanda_params)
         semantic_dics, semantic_keys = dec._find_semantic_dichotomies()
-        if 'XOR' in self.analysis_params.keys():
-            if self.analysis_params['XOR'] and len(self.conditions) == 2:
+        if 'non_semantic' in self.analysis_params.keys():
+            if self.analysis_params['non_semantic'] and len(self.conditions) == 2:
                 semantic_dics.append([['01', '10'], ['00', '11']])
                 semantic_keys.append('XOR')
+            if self.analysis_params['non_semantic'] and len(self.conditions) > 2:
+                dics = dec.all_dichotomies(balanced=True)
+                semantic_dics = list(dics.values())
+                semantic_keys = list(dics.keys())
 
         perfs = {}
         for key, dic in zip(semantic_keys, semantic_dics):
             if dec._verbose:
                 print("\nTesting null decoding performance for semantic dichotomy: ", key)
             dec._shuffle_conditioned_arrays(dic)
             performance = dec.decode_dichotomy(dic, **self.analysis_params)
```

### Comparing `decodanda-0.6.4/decodanda/imports.py` & `decodanda-0.6.5/decodanda/imports.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.4/decodanda/in_time.py` & `decodanda-0.6.5/decodanda/in_time.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.4/decodanda/utilities.py` & `decodanda-0.6.5/decodanda/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,27 @@
 import scipy.stats
 
 from .imports import *
 
 
 # Classes
 
-
 class CrossValidator(object):
     # necessary for parallelization of cross validation repetitions
     # TODO: fix parallelization by fixing this
-    def __init__(self, classifier, conditioned_rasters, conditioned_trial_index, dic, training_fraction, ndata, subset,
-                 semantic_vectors):
+    def __init__(self, classifier, conditioned_rasters, conditioned_trial_index, dic,
+                 training_fraction, ndata, subset,
+                 semantic_vectors, dic_key, z_score):
+
         self.classifier = classifier
         self.conditioned_rasters = deepcopy(conditioned_rasters)
         self.conditioned_trial_index = deepcopy(conditioned_trial_index)
         self.dic = dic
+        self.dic_key = dic_key
+        self.z_score = z_score
         self.training_fraction = training_fraction
         self.ndata = ndata
         self.subset = subset
         self.semantic_vectors = semantic_vectors
 
     def __call__(self, i):
         self.i = i
@@ -48,15 +51,19 @@
         testing_raster = np.vstack([testing_raster_A, testing_raster_B])
         testing_labels = np.hstack([testing_labels_A, testing_labels_B])
 
         testing_raster = testing_raster[:, self.subset]
         performance = self.classifier.score(testing_raster, testing_labels)
         return performance
 
-    def one_cv_step(self, dic, training_fraction, ndata):
+    def one_cv_step(self, dic, training_fraction, ndata, testing_trials=None):
+
+        if self.dic_key is None:
+            self.dic_key = compute_dic_key(dic)
+
         set_A = dic[0]
         label_A = ''
         for d in set_A:
             label_A += (self.semantic_vectors[d] + ' ')
         label_A = label_A[:-1]
 
         set_B = dic[1]
@@ -66,41 +73,60 @@
         label_B = label_B[:-1]
 
         training_array_A = []
         training_array_B = []
         testing_array_A = []
         testing_array_B = []
 
+        # allow for unbalanced dichotomies
+        n_conditions_A = float(len(dic[0]))
+        n_conditions_B = float(len(dic[1]))
+        fraction = n_conditions_A / n_conditions_B
+
         for d in set_A:
             training, testing = sample_training_testing_from_rasters(self.conditioned_rasters[d],
-                                                                     ndata,
+                                                                     int(ndata / fraction),
                                                                      training_fraction,
                                                                      self.conditioned_trial_index[d],
-                                                                     randomstate=self.randomstate)
+                                                                     testing_trials=testing_trials)
+
             training_array_A.append(training)
             testing_array_A.append(testing)
 
         for d in set_B:
             training, testing = sample_training_testing_from_rasters(self.conditioned_rasters[d],
-                                                                     ndata,
+                                                                     int(ndata),
                                                                      training_fraction,
-                                                                     self.conditioned_trial_index[d])
+                                                                     self.conditioned_trial_index[d],
+                                                                     testing_trials=testing_trials)
             training_array_B.append(training)
             testing_array_B.append(testing)
 
         training_array_A = np.vstack(training_array_A)
         training_array_B = np.vstack(training_array_B)
         testing_array_A = np.vstack(testing_array_A)
         testing_array_B = np.vstack(testing_array_B)
 
-        self._train(training_array_A, training_array_B, label_A, label_B)
-
-        performance = self._test(testing_array_A, testing_array_B, label_A, label_B)
-
-        return performance
+        if self.z_score:
+            big_raster = np.vstack([training_array_A, training_array_B])  # z-scoring using the training data
+            big_mean = np.nanmean(big_raster, 0)
+            big_std = np.nanstd(big_raster, 0)
+            big_std[big_std == 0] = np.inf
+            training_array_A = (training_array_A - big_mean) / big_std
+            training_array_B = (training_array_B - big_mean) / big_std
+            testing_array_A = (testing_array_A - big_mean) / big_std
+            testing_array_B = (testing_array_B - big_mean) / big_std
+
+        self.train(training_array_A, training_array_B, label_A, label_B)
+
+        performance = self.test(testing_array_A, testing_array_B, label_A, label_B)
+        weights = {}
+        if hasattr(self.classifier, 'coef_'):
+            weights[self.dic_key] = self.classifier.coef_
+        return [performance, weights]
 
 
 class DictSession:
     """
     Translator from dictionary to session object with getattr
 
     """
@@ -657,14 +683,18 @@
     # norm, hence I call half the max range the plot radius.
     plot_radius = 0.5 * max([x_range, y_range, z_range])
     ax.set_xlim3d([x_middle - plot_radius, x_middle + plot_radius])
     ax.set_ylim3d([y_middle - plot_radius, y_middle + plot_radius])
     ax.set_zlim3d([z_middle - plot_radius, z_middle + plot_radius])
 
 
+def compute_dic_key(dic):
+    return '_'.join(dic[0]) + '_v_' + '_'.join(dic[1])
+
+
 def log_dichotomy(dec, dic, ndata, s='Decoding'):
     set_A = dic[0]
     label_A = ''
     for d in set_A:
         label_A += (dec._semantic_vectors[d] + ' ')
     label_A = label_A[:-1]
```

### Comparing `decodanda-0.6.4/decodanda/visualize.py` & `decodanda-0.6.5/decodanda/visualize.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.4/decodanda.egg-info/PKG-INFO` & `decodanda-0.6.5/decodanda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decodanda
-Version: 0.6.4
+Version: 0.6.5
 Summary: A python package for neural decoding with built-in best practices.
 Home-page: https://github.com/lposani/decodanda
 Author: Lorenzo Posani
 Author-email: lorenzo.posani@gmail.com
 Keywords: python,decoding,neuroscience,ccgp,neural activity,population activity,neural decoding,geometry
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `decodanda-0.6.4/setup.py` & `decodanda-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.6.4'
+VERSION = '0.6.5'
 DESCRIPTION = 'A python package for neural decoding with built-in best practices.'
 LONG_DESCRIPTION = 'Decodanda (dog latin for "to be decoded") is a best-practices-made-easy Python package for decoding neural data. Decodanda is designed to expose a user-friendly and flexible interface for population activity decoding, with a series of built-in best practices to avoid the most common pitfalls. In addition, Decodanda exposes a series of functions to compute the Cross-Condition Generalization Performance (CCGP, Bernardi et al. 2020) for the geometrical analysis of neural population activity.'
 
 setup(
     name="decodanda",
     version=VERSION,
     author="Lorenzo Posani",
```

