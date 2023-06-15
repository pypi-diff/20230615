# Comparing `tmp/pandasflow-0.7.6.tar.gz` & `tmp/pandasflow-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasflow-0.7.6.tar", last modified: Thu Jun 15 15:40:31 2023, max compression
+gzip compressed data, was "pandasflow-0.7.7.tar", last modified: Thu Jun 15 15:42:31 2023, max compression
```

## Comparing `pandasflow-0.7.6.tar` & `pandasflow-0.7.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 15:40:31.388090 pandasflow-0.7.6/
--rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.7.6/LICENCE
--rw-rw-rw-   0        0        0      869 2023-06-15 15:40:31.388090 pandasflow-0.7.6/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-05-15 11:35:26.000000 pandasflow-0.7.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 15:40:31.366545 pandasflow-0.7.6/pandasflow/
--rw-rw-rw-   0        0        0      419 2023-06-15 15:40:19.000000 pandasflow-0.7.6/pandasflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:40:31.371532 pandasflow-0.7.6/pandasflow/dev/
--rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.7.6/pandasflow/dev/__init__.py
--rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.7.6/pandasflow/dev/err_mean_diff.py
--rw-rw-rw-   0        0        0      387 2023-05-30 09:54:40.000000 pandasflow-0.7.6/pandasflow/get_import.py
--rw-rw-rw-   0        0        0      480 2023-05-15 09:05:23.000000 pandasflow-0.7.6/pandasflow/get_psql.py
--rw-rw-rw-   0        0        0      208 2023-05-15 09:29:01.000000 pandasflow-0.7.6/pandasflow/get_sqlt.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:40:31.375742 pandasflow-0.7.6/pandasflow/metrics/
--rw-rw-rw-   0        0        0      282 2023-06-15 15:39:37.000000 pandasflow-0.7.6/pandasflow/metrics/__init__.py
--rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.7.6/pandasflow/metrics/conf_mat.py
--rw-rw-rw-   0        0        0     2173 2023-05-15 11:57:58.000000 pandasflow-0.7.6/pandasflow/metrics/lloss_up.py
--rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.7.6/pandasflow/metrics/mean_error.py
--rw-rw-rw-   0        0        0      721 2023-05-07 08:19:28.000000 pandasflow-0.7.6/pandasflow/metrics/precision_recall.py
--rw-rw-rw-   0        0        0      654 2023-06-15 15:38:41.000000 pandasflow-0.7.6/pandasflow/metrics/roc_auc.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:40:31.376740 pandasflow-0.7.6/pandasflow/model/
--rw-rw-rw-   0        0        0      142 2023-06-15 15:39:49.000000 pandasflow-0.7.6/pandasflow/model/__init__.py
--rw-rw-rw-   0        0        0      751 2023-06-15 13:40:11.000000 pandasflow-0.7.6/pandasflow/model/best_thr_f1.py
--rw-rw-rw-   0        0        0      605 2023-06-15 13:53:15.000000 pandasflow-0.7.6/pandasflow/model/calc_class_from_score.py
--rw-rw-rw-   0        0        0      622 2023-05-15 12:17:31.000000 pandasflow-0.7.6/pandasflow/reset_mi.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:40:31.377738 pandasflow-0.7.6/pandasflow/services/
--rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.7.6/pandasflow/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:40:31.379425 pandasflow-0.7.6/pandasflow/split/
--rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.7.6/pandasflow/split/__init__.py
--rw-rw-rw-   0        0        0     2835 2023-05-15 10:13:46.000000 pandasflow-0.7.6/pandasflow/split/train_test.py
--rw-rw-rw-   0        0        0     3944 2023-05-15 10:24:18.000000 pandasflow-0.7.6/pandasflow/split/train_valid_test.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:40:31.370535 pandasflow-0.7.6/pandasflow.egg-info/
--rw-rw-rw-   0        0        0      869 2023-06-15 15:40:31.000000 pandasflow-0.7.6/pandasflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1049 2023-06-15 15:40:31.000000 pandasflow-0.7.6/pandasflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 15:40:31.000000 pandasflow-0.7.6/pandasflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-15 15:40:31.000000 pandasflow-0.7.6/pandasflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-15 15:40:31.000000 pandasflow-0.7.6/pandasflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 15:40:31.388090 pandasflow-0.7.6/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.7.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:40:31.387092 pandasflow-0.7.6/test/
--rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.7.6/test/__init__.py
--rw-rw-rw-   0        0        0      749 2023-06-15 15:40:02.000000 pandasflow-0.7.6/test/best_thr_f1_test.py
--rw-rw-rw-   0        0        0     1002 2023-06-15 13:28:13.000000 pandasflow-0.7.6/test/calc_class_from_score_test.py
--rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.7.6/test/conf_mat_test.py
--rw-rw-rw-   0        0        0      620 2023-05-15 11:59:08.000000 pandasflow-0.7.6/test/lloss_up_test.py
--rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.7.6/test/mean_error_test.py
--rw-rw-rw-   0        0        0     1296 2023-05-07 08:19:28.000000 pandasflow-0.7.6/test/precision_recall_test.py
--rw-rw-rw-   0        0        0     1261 2023-06-06 08:49:02.000000 pandasflow-0.7.6/test/roc_auc_test.py
--rw-rw-rw-   0        0        0      498 2023-05-15 10:14:07.000000 pandasflow-0.7.6/test/split_tt_test.py
--rw-rw-rw-   0        0        0      782 2023-05-15 10:24:03.000000 pandasflow-0.7.6/test/split_tvt_test.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:42:31.126924 pandasflow-0.7.7/
+-rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.7.7/LICENCE
+-rw-rw-rw-   0        0        0      869 2023-06-15 15:42:31.127946 pandasflow-0.7.7/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-05-15 11:35:26.000000 pandasflow-0.7.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 15:42:31.110412 pandasflow-0.7.7/pandasflow/
+-rw-rw-rw-   0        0        0      419 2023-06-15 15:42:28.000000 pandasflow-0.7.7/pandasflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:42:31.113404 pandasflow-0.7.7/pandasflow/dev/
+-rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.7.7/pandasflow/dev/__init__.py
+-rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.7.7/pandasflow/dev/err_mean_diff.py
+-rw-rw-rw-   0        0        0      387 2023-05-30 09:54:40.000000 pandasflow-0.7.7/pandasflow/get_import.py
+-rw-rw-rw-   0        0        0      480 2023-05-15 09:05:23.000000 pandasflow-0.7.7/pandasflow/get_psql.py
+-rw-rw-rw-   0        0        0      208 2023-05-15 09:29:01.000000 pandasflow-0.7.7/pandasflow/get_sqlt.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:42:31.116396 pandasflow-0.7.7/pandasflow/metrics/
+-rw-rw-rw-   0        0        0      282 2023-06-15 15:39:37.000000 pandasflow-0.7.7/pandasflow/metrics/__init__.py
+-rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.7.7/pandasflow/metrics/conf_mat.py
+-rw-rw-rw-   0        0        0     2173 2023-05-15 11:57:58.000000 pandasflow-0.7.7/pandasflow/metrics/lloss_up.py
+-rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.7.7/pandasflow/metrics/mean_error.py
+-rw-rw-rw-   0        0        0      721 2023-05-07 08:19:28.000000 pandasflow-0.7.7/pandasflow/metrics/precision_recall.py
+-rw-rw-rw-   0        0        0      654 2023-06-15 15:38:41.000000 pandasflow-0.7.7/pandasflow/metrics/roc_auc.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:42:31.117393 pandasflow-0.7.7/pandasflow/model/
+-rw-rw-rw-   0        0        0      142 2023-06-15 15:39:49.000000 pandasflow-0.7.7/pandasflow/model/__init__.py
+-rw-rw-rw-   0        0        0      751 2023-06-15 13:40:11.000000 pandasflow-0.7.7/pandasflow/model/best_thr_f1.py
+-rw-rw-rw-   0        0        0      603 2023-06-15 15:42:21.000000 pandasflow-0.7.7/pandasflow/model/calc_class_from_score.py
+-rw-rw-rw-   0        0        0      622 2023-05-15 12:17:31.000000 pandasflow-0.7.7/pandasflow/reset_mi.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:42:31.118390 pandasflow-0.7.7/pandasflow/services/
+-rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.7.7/pandasflow/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:42:31.119388 pandasflow-0.7.7/pandasflow/split/
+-rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.7.7/pandasflow/split/__init__.py
+-rw-rw-rw-   0        0        0     2835 2023-05-15 10:13:46.000000 pandasflow-0.7.7/pandasflow/split/train_test.py
+-rw-rw-rw-   0        0        0     3944 2023-05-15 10:24:18.000000 pandasflow-0.7.7/pandasflow/split/train_valid_test.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:42:31.112407 pandasflow-0.7.7/pandasflow.egg-info/
+-rw-rw-rw-   0        0        0      869 2023-06-15 15:42:31.000000 pandasflow-0.7.7/pandasflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1049 2023-06-15 15:42:31.000000 pandasflow-0.7.7/pandasflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 15:42:31.000000 pandasflow-0.7.7/pandasflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-15 15:42:31.000000 pandasflow-0.7.7/pandasflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-15 15:42:31.000000 pandasflow-0.7.7/pandasflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 15:42:31.127946 pandasflow-0.7.7/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.7.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:42:31.126924 pandasflow-0.7.7/test/
+-rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.7.7/test/__init__.py
+-rw-rw-rw-   0        0        0      749 2023-06-15 15:40:02.000000 pandasflow-0.7.7/test/best_thr_f1_test.py
+-rw-rw-rw-   0        0        0     1000 2023-06-15 15:42:21.000000 pandasflow-0.7.7/test/calc_class_from_score_test.py
+-rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.7.7/test/conf_mat_test.py
+-rw-rw-rw-   0        0        0      620 2023-05-15 11:59:08.000000 pandasflow-0.7.7/test/lloss_up_test.py
+-rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.7.7/test/mean_error_test.py
+-rw-rw-rw-   0        0        0     1296 2023-05-07 08:19:28.000000 pandasflow-0.7.7/test/precision_recall_test.py
+-rw-rw-rw-   0        0        0     1261 2023-06-06 08:49:02.000000 pandasflow-0.7.7/test/roc_auc_test.py
+-rw-rw-rw-   0        0        0      498 2023-05-15 10:14:07.000000 pandasflow-0.7.7/test/split_tt_test.py
+-rw-rw-rw-   0        0        0      782 2023-05-15 10:24:03.000000 pandasflow-0.7.7/test/split_tvt_test.py
```

### Comparing `pandasflow-0.7.6/LICENCE` & `pandasflow-0.7.7/LICENCE`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.6/PKG-INFO` & `pandasflow-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.7.6
+Version: 0.7.7
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.7.6/pandasflow/dev/err_mean_diff.py` & `pandasflow-0.7.7/pandasflow/dev/err_mean_diff.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.6/pandasflow/metrics/conf_mat.py` & `pandasflow-0.7.7/pandasflow/metrics/conf_mat.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.6/pandasflow/metrics/lloss_up.py` & `pandasflow-0.7.7/pandasflow/metrics/lloss_up.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.6/pandasflow/metrics/precision_recall.py` & `pandasflow-0.7.7/pandasflow/metrics/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.6/pandasflow/metrics/roc_auc.py` & `pandasflow-0.7.7/pandasflow/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.6/pandasflow/model/best_thr_f1.py` & `pandasflow-0.7.7/pandasflow/model/best_thr_f1.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.6/pandasflow/model/calc_class_from_score.py` & `pandasflow-0.7.7/pandasflow/model/calc_class_from_score.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def calc_class_from_score(score:pd.Series, thr=0.5, y_true:pd.Series | None = None) -> pd.Series:
 	df = pd.DataFrame({'score': score, 'y_true': y_true})
 	
 	_thr = thr
 	
 	if thr in [True, 0, 'best']:
 		if y_true is not None:
-			_thr = pdf.metrics.best_thr_f1(df['y_true'], df['score'])
+			_thr = pdf.model.best_thr_f1(df['y_true'], df['score'])
 		else:
 			print('incorrect thr, y_true is lost')
 	
 	df['y_pred'] = (df['score'] > _thr) * 1
 	
 	if y_true is not None:
 		print(classification_report(df['y_true'], df['y_pred']))
```

### Comparing `pandasflow-0.7.6/pandasflow/reset_mi.py` & `pandasflow-0.7.7/pandasflow/reset_mi.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.6/pandasflow/split/train_test.py` & `pandasflow-0.7.7/pandasflow/split/train_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.6/pandasflow/split/train_valid_test.py` & `pandasflow-0.7.7/pandasflow/split/train_valid_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.6/pandasflow.egg-info/PKG-INFO` & `pandasflow-0.7.7/pandasflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.7.6
+Version: 0.7.7
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.7.6/pandasflow.egg-info/SOURCES.txt` & `pandasflow-0.7.7/pandasflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.6/setup.py` & `pandasflow-0.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.6/test/best_thr_f1_test.py` & `pandasflow-0.7.7/test/best_thr_f1_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.6/test/calc_class_from_score_test.py` & `pandasflow-0.7.7/test/calc_class_from_score_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 train = train.merge(model, how='left', on=['NumOfProducts', 'age_group'])
 test['age_group'] = pd.cut(test['Age'], [0, 31, 35, 40, 45, float('inf')])
 test = test.merge(model, how='left', on=['NumOfProducts', 'age_group'])
 test['y_pred'] = (test['score_prod_age'] > 0.5) * 1
 
 print(test['Exited'])
 
-thr = pdf.metrics.best_thr_f1(test['Exited'], test['score_prod_age'])
+thr = pdf.model.best_thr_f1(test['Exited'], test['score_prod_age'])
 print()
 print(thr)
 print('\nv1')
 a = pdf.model.calc_class_from_score(test['score_prod_age'], y_true=test['Exited'])
 print('\nv2')
 a = pdf.model.calc_class_from_score(test['score_prod_age'], thr, y_true=test['Exited'])
```

### Comparing `pandasflow-0.7.6/test/conf_mat_test.py` & `pandasflow-0.7.7/test/conf_mat_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.6/test/lloss_up_test.py` & `pandasflow-0.7.7/test/lloss_up_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.6/test/precision_recall_test.py` & `pandasflow-0.7.7/test/precision_recall_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.6/test/roc_auc_test.py` & `pandasflow-0.7.7/test/roc_auc_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.7.6/test/split_tvt_test.py` & `pandasflow-0.7.7/test/split_tvt_test.py`

 * *Files identical despite different names*

