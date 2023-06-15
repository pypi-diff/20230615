# Comparing `tmp/pandasflow-0.7.1.tar.gz` & `tmp/pandasflow-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasflow-0.7.1.tar", last modified: Thu Jun 15 13:06:53 2023, max compression
+gzip compressed data, was "pandasflow-0.7.2.tar", last modified: Thu Jun 15 13:37:52 2023, max compression
```

## Comparing `pandasflow-0.7.1.tar` & `pandasflow-0.7.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 13:06:53.593093 pandasflow-0.7.1/
--rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.7.1/LICENCE
--rw-rw-rw-   0        0        0      869 2023-06-15 13:06:53.593093 pandasflow-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-05-15 11:35:26.000000 pandasflow-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 13:06:53.576358 pandasflow-0.7.1/pandasflow/
--rw-rw-rw-   0        0        0      419 2023-06-15 13:06:47.000000 pandasflow-0.7.1/pandasflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:06:53.579349 pandasflow-0.7.1/pandasflow/dev/
--rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.7.1/pandasflow/dev/__init__.py
--rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.7.1/pandasflow/dev/err_mean_diff.py
--rw-rw-rw-   0        0        0      387 2023-05-30 09:54:40.000000 pandasflow-0.7.1/pandasflow/get_import.py
--rw-rw-rw-   0        0        0      480 2023-05-15 09:05:23.000000 pandasflow-0.7.1/pandasflow/get_psql.py
--rw-rw-rw-   0        0        0      208 2023-05-15 09:29:01.000000 pandasflow-0.7.1/pandasflow/get_sqlt.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:06:53.584115 pandasflow-0.7.1/pandasflow/metrics/
--rw-rw-rw-   0        0        0      340 2023-06-06 08:47:33.000000 pandasflow-0.7.1/pandasflow/metrics/__init__.py
--rw-rw-rw-   0        0        0      748 2023-06-15 13:05:36.000000 pandasflow-0.7.1/pandasflow/metrics/best_thr_f1.py
--rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.7.1/pandasflow/metrics/conf_mat.py
--rw-rw-rw-   0        0        0     2173 2023-05-15 11:57:58.000000 pandasflow-0.7.1/pandasflow/metrics/lloss_up.py
--rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.7.1/pandasflow/metrics/mean_error.py
--rw-rw-rw-   0        0        0      721 2023-05-07 08:19:28.000000 pandasflow-0.7.1/pandasflow/metrics/precision_recall.py
--rw-rw-rw-   0        0        0      658 2023-06-06 08:47:33.000000 pandasflow-0.7.1/pandasflow/metrics/roc_auc.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:06:53.585114 pandasflow-0.7.1/pandasflow/model/
--rw-rw-rw-   0        0        0       88 2023-06-15 10:21:12.000000 pandasflow-0.7.1/pandasflow/model/__init__.py
--rw-rw-rw-   0        0        0      520 2023-06-15 12:57:32.000000 pandasflow-0.7.1/pandasflow/model/calc_class_from_score.py
--rw-rw-rw-   0        0        0      622 2023-05-15 12:17:31.000000 pandasflow-0.7.1/pandasflow/reset_mi.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:06:53.585114 pandasflow-0.7.1/pandasflow/services/
--rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.7.1/pandasflow/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:06:53.586111 pandasflow-0.7.1/pandasflow/split/
--rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.7.1/pandasflow/split/__init__.py
--rw-rw-rw-   0        0        0     2835 2023-05-15 10:13:46.000000 pandasflow-0.7.1/pandasflow/split/train_test.py
--rw-rw-rw-   0        0        0     3944 2023-05-15 10:24:18.000000 pandasflow-0.7.1/pandasflow/split/train_valid_test.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:06:53.579349 pandasflow-0.7.1/pandasflow.egg-info/
--rw-rw-rw-   0        0        0      869 2023-06-15 13:06:53.000000 pandasflow-0.7.1/pandasflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1051 2023-06-15 13:06:53.000000 pandasflow-0.7.1/pandasflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 13:06:53.000000 pandasflow-0.7.1/pandasflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-15 13:06:53.000000 pandasflow-0.7.1/pandasflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-15 13:06:53.000000 pandasflow-0.7.1/pandasflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 13:06:53.593093 pandasflow-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:06:53.592097 pandasflow-0.7.1/test/
--rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.7.1/test/__init__.py
--rw-rw-rw-   0        0        0      751 2023-06-15 13:05:46.000000 pandasflow-0.7.1/test/best_thr_f1_test.py
--rw-rw-rw-   0        0        0      998 2023-06-15 13:06:11.000000 pandasflow-0.7.1/test/calc_class_from_score_test.py
--rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.7.1/test/conf_mat_test.py
--rw-rw-rw-   0        0        0      620 2023-05-15 11:59:08.000000 pandasflow-0.7.1/test/lloss_up_test.py
--rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.7.1/test/mean_error_test.py
--rw-rw-rw-   0        0        0     1296 2023-05-07 08:19:28.000000 pandasflow-0.7.1/test/precision_recall_test.py
--rw-rw-rw-   0        0        0     1261 2023-06-06 08:49:02.000000 pandasflow-0.7.1/test/roc_auc_test.py
--rw-rw-rw-   0        0        0      498 2023-05-15 10:14:07.000000 pandasflow-0.7.1/test/split_tt_test.py
--rw-rw-rw-   0        0        0      782 2023-05-15 10:24:03.000000 pandasflow-0.7.1/test/split_tvt_test.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:37:52.561198 pandasflow-0.7.2/
+-rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.7.2/LICENCE
+-rw-rw-rw-   0        0        0      869 2023-06-15 13:37:52.561198 pandasflow-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-05-15 11:35:26.000000 pandasflow-0.7.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 13:37:52.543245 pandasflow-0.7.2/pandasflow/
+-rw-rw-rw-   0        0        0      419 2023-06-15 13:37:17.000000 pandasflow-0.7.2/pandasflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:37:52.547235 pandasflow-0.7.2/pandasflow/dev/
+-rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.7.2/pandasflow/dev/__init__.py
+-rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.7.2/pandasflow/dev/err_mean_diff.py
+-rw-rw-rw-   0        0        0      387 2023-05-30 09:54:40.000000 pandasflow-0.7.2/pandasflow/get_import.py
+-rw-rw-rw-   0        0        0      480 2023-05-15 09:05:23.000000 pandasflow-0.7.2/pandasflow/get_psql.py
+-rw-rw-rw-   0        0        0      208 2023-05-15 09:29:01.000000 pandasflow-0.7.2/pandasflow/get_sqlt.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:37:52.552221 pandasflow-0.7.2/pandasflow/metrics/
+-rw-rw-rw-   0        0        0      340 2023-06-06 08:47:33.000000 pandasflow-0.7.2/pandasflow/metrics/__init__.py
+-rw-rw-rw-   0        0        0      844 2023-06-15 13:30:38.000000 pandasflow-0.7.2/pandasflow/metrics/best_thr_f1.py
+-rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.7.2/pandasflow/metrics/conf_mat.py
+-rw-rw-rw-   0        0        0     2173 2023-05-15 11:57:58.000000 pandasflow-0.7.2/pandasflow/metrics/lloss_up.py
+-rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.7.2/pandasflow/metrics/mean_error.py
+-rw-rw-rw-   0        0        0      721 2023-05-07 08:19:28.000000 pandasflow-0.7.2/pandasflow/metrics/precision_recall.py
+-rw-rw-rw-   0        0        0      658 2023-06-06 08:47:33.000000 pandasflow-0.7.2/pandasflow/metrics/roc_auc.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:37:52.553219 pandasflow-0.7.2/pandasflow/model/
+-rw-rw-rw-   0        0        0       88 2023-06-15 10:21:12.000000 pandasflow-0.7.2/pandasflow/model/__init__.py
+-rw-rw-rw-   0        0        0      414 2023-06-15 13:37:42.000000 pandasflow-0.7.2/pandasflow/model/calc_class_from_score.py
+-rw-rw-rw-   0        0        0      622 2023-05-15 12:17:31.000000 pandasflow-0.7.2/pandasflow/reset_mi.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:37:52.553219 pandasflow-0.7.2/pandasflow/services/
+-rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.7.2/pandasflow/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:37:52.555213 pandasflow-0.7.2/pandasflow/split/
+-rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.7.2/pandasflow/split/__init__.py
+-rw-rw-rw-   0        0        0     2835 2023-05-15 10:13:46.000000 pandasflow-0.7.2/pandasflow/split/train_test.py
+-rw-rw-rw-   0        0        0     3944 2023-05-15 10:24:18.000000 pandasflow-0.7.2/pandasflow/split/train_valid_test.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:37:52.546237 pandasflow-0.7.2/pandasflow.egg-info/
+-rw-rw-rw-   0        0        0      869 2023-06-15 13:37:52.000000 pandasflow-0.7.2/pandasflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1051 2023-06-15 13:37:52.000000 pandasflow-0.7.2/pandasflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 13:37:52.000000 pandasflow-0.7.2/pandasflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-15 13:37:52.000000 pandasflow-0.7.2/pandasflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-15 13:37:52.000000 pandasflow-0.7.2/pandasflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 13:37:52.561198 pandasflow-0.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:37:52.560202 pandasflow-0.7.2/test/
+-rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.7.2/test/__init__.py
+-rw-rw-rw-   0        0        0      751 2023-06-15 13:30:47.000000 pandasflow-0.7.2/test/best_thr_f1_test.py
+-rw-rw-rw-   0        0        0     1002 2023-06-15 13:28:13.000000 pandasflow-0.7.2/test/calc_class_from_score_test.py
+-rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.7.2/test/conf_mat_test.py
+-rw-rw-rw-   0        0        0      620 2023-05-15 11:59:08.000000 pandasflow-0.7.2/test/lloss_up_test.py
+-rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.7.2/test/mean_error_test.py
+-rw-rw-rw-   0        0        0     1296 2023-05-07 08:19:28.000000 pandasflow-0.7.2/test/precision_recall_test.py
+-rw-rw-rw-   0        0        0     1261 2023-06-06 08:49:02.000000 pandasflow-0.7.2/test/roc_auc_test.py
+-rw-rw-rw-   0        0        0      498 2023-05-15 10:14:07.000000 pandasflow-0.7.2/test/split_tt_test.py
+-rw-rw-rw-   0        0        0      782 2023-05-15 10:24:03.000000 pandasflow-0.7.2/test/split_tvt_test.py
```

### Comparing `pandasflow-0.7.1/LICENCE` & `pandasflow-0.7.2/LICENCE`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.1/PKG-INFO` & `pandasflow-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.7.1
+Version: 0.7.2
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.7.1/pandasflow/dev/err_mean_diff.py` & `pandasflow-0.7.2/pandasflow/dev/err_mean_diff.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.1/pandasflow/metrics/best_thr_f1.py` & `pandasflow-0.7.2/pandasflow/metrics/best_thr_f1.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-
+import os
 import pandas as pd
 from sklearn.metrics import f1_score
-from tqdm import tqdm
 
+if 'google-cloud-sdk' in os.environ['PATH']:
+	from tqdm.notebook import tqdm
+else:
+	from tqdm import tqdm
 
 def best_thr_f1(y_true:pd.Series, score:pd.Series, out:int=1):
 	thrs = list(score.unique())
 	thrs = [max(min(thrs) - 0.000001, 0.000001)] + thrs
 	
 	df = pd.concat([y_true, score], axis=1)
```

### Comparing `pandasflow-0.7.1/pandasflow/metrics/conf_mat.py` & `pandasflow-0.7.2/pandasflow/metrics/conf_mat.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.1/pandasflow/metrics/lloss_up.py` & `pandasflow-0.7.2/pandasflow/metrics/lloss_up.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.1/pandasflow/metrics/precision_recall.py` & `pandasflow-0.7.2/pandasflow/metrics/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.1/pandasflow/metrics/roc_auc.py` & `pandasflow-0.7.2/pandasflow/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.1/pandasflow/reset_mi.py` & `pandasflow-0.7.2/pandasflow/reset_mi.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.1/pandasflow/split/train_test.py` & `pandasflow-0.7.2/pandasflow/split/train_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.1/pandasflow/split/train_valid_test.py` & `pandasflow-0.7.2/pandasflow/split/train_valid_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.1/pandasflow.egg-info/PKG-INFO` & `pandasflow-0.7.2/pandasflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.7.1
+Version: 0.7.2
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.7.1/pandasflow.egg-info/SOURCES.txt` & `pandasflow-0.7.2/pandasflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.1/setup.py` & `pandasflow-0.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.1/test/best_thr_f1_test.py` & `pandasflow-0.7.2/test/best_thr_f1_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.1/test/calc_class_from_score_test.py` & `pandasflow-0.7.2/test/calc_class_from_score_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pandasflow as pdf
 import pandas as pd
 
+
 df = pd.read_csv('test_data.csv')
 
 train, valid, test = pdf.split.train_valid_test(df, target='Exited', stratify='Exited')
 train['age_group'] = pd.cut(train['Age'], [0, 31, 35, 40, 45, float('inf')])
 model = train.groupby(['NumOfProducts', 'age_group'])['Exited'].mean().reset_index()
 model = model.rename({'Exited': 'score_prod_age'}, axis=1)
 train = train.merge(model, how='left', on=['NumOfProducts', 'age_group'])
@@ -17,7 +18,8 @@
 thr = pdf.metrics.best_thr_f1(test['Exited'], test['score_prod_age'])
 print()
 print(thr)
 print('\nv1')
 a = pdf.model.calc_class_from_score(test['score_prod_age'], y_true=test['Exited'])
 print('\nv2')
 a = pdf.model.calc_class_from_score(test['score_prod_age'], thr, y_true=test['Exited'])
+
```

### Comparing `pandasflow-0.7.1/test/conf_mat_test.py` & `pandasflow-0.7.2/test/conf_mat_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.1/test/lloss_up_test.py` & `pandasflow-0.7.2/test/lloss_up_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.1/test/precision_recall_test.py` & `pandasflow-0.7.2/test/precision_recall_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.1/test/roc_auc_test.py` & `pandasflow-0.7.2/test/roc_auc_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.1/test/split_tvt_test.py` & `pandasflow-0.7.2/test/split_tvt_test.py`

 * *Files identical despite different names*

