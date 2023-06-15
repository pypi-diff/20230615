# Comparing `tmp/pandasflow-0.6.1.tar.gz` & `tmp/pandasflow-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasflow-0.6.1.tar", last modified: Tue Jun  6 08:55:48 2023, max compression
+gzip compressed data, was "pandasflow-0.7.0.tar", last modified: Thu Jun 15 12:47:24 2023, max compression
```

## Comparing `pandasflow-0.6.1.tar` & `pandasflow-0.7.0.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 08:55:48.275485 pandasflow-0.6.1/
--rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.6.1/LICENCE
--rw-rw-rw-   0        0        0      869 2023-06-06 08:55:48.275485 pandasflow-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-05-15 11:35:26.000000 pandasflow-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 08:55:48.260525 pandasflow-0.6.1/pandasflow/
--rw-rw-rw-   0        0        0      391 2023-06-06 08:55:34.000000 pandasflow-0.6.1/pandasflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 08:55:48.263516 pandasflow-0.6.1/pandasflow/dev/
--rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.6.1/pandasflow/dev/__init__.py
--rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.6.1/pandasflow/dev/err_mean_diff.py
--rw-rw-rw-   0        0        0      387 2023-05-30 09:54:40.000000 pandasflow-0.6.1/pandasflow/get_import.py
--rw-rw-rw-   0        0        0      480 2023-05-15 09:05:23.000000 pandasflow-0.6.1/pandasflow/get_psql.py
--rw-rw-rw-   0        0        0      208 2023-05-15 09:29:01.000000 pandasflow-0.6.1/pandasflow/get_sqlt.py
-drwxrwxrwx   0        0        0        0 2023-06-06 08:55:48.267507 pandasflow-0.6.1/pandasflow/metrics/
--rw-rw-rw-   0        0        0      340 2023-06-06 08:47:33.000000 pandasflow-0.6.1/pandasflow/metrics/__init__.py
--rw-rw-rw-   0        0        0      801 2023-06-06 08:45:10.000000 pandasflow-0.6.1/pandasflow/metrics/best_thr_f1.py
--rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.6.1/pandasflow/metrics/conf_mat.py
--rw-rw-rw-   0        0        0     2173 2023-05-15 11:57:58.000000 pandasflow-0.6.1/pandasflow/metrics/lloss_up.py
--rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.6.1/pandasflow/metrics/mean_error.py
--rw-rw-rw-   0        0        0      721 2023-05-07 08:19:28.000000 pandasflow-0.6.1/pandasflow/metrics/precision_recall.py
--rw-rw-rw-   0        0        0      658 2023-06-06 08:47:33.000000 pandasflow-0.6.1/pandasflow/metrics/roc_auc.py
-drwxrwxrwx   0        0        0        0 2023-06-06 08:55:48.267507 pandasflow-0.6.1/pandasflow/model/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:16:13.000000 pandasflow-0.6.1/pandasflow/model/__init__.py
--rw-rw-rw-   0        0        0      622 2023-05-15 12:17:31.000000 pandasflow-0.6.1/pandasflow/reset_mi.py
-drwxrwxrwx   0        0        0        0 2023-06-06 08:55:48.268504 pandasflow-0.6.1/pandasflow/services/
--rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.6.1/pandasflow/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 08:55:48.269501 pandasflow-0.6.1/pandasflow/split/
--rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.6.1/pandasflow/split/__init__.py
--rw-rw-rw-   0        0        0     2835 2023-05-15 10:13:46.000000 pandasflow-0.6.1/pandasflow/split/train_test.py
--rw-rw-rw-   0        0        0     3944 2023-05-15 10:24:18.000000 pandasflow-0.6.1/pandasflow/split/train_valid_test.py
-drwxrwxrwx   0        0        0        0 2023-06-06 08:55:48.262520 pandasflow-0.6.1/pandasflow.egg-info/
--rw-rw-rw-   0        0        0      869 2023-06-06 08:55:48.000000 pandasflow-0.6.1/pandasflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      974 2023-06-06 08:55:48.000000 pandasflow-0.6.1/pandasflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 08:55:48.000000 pandasflow-0.6.1/pandasflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-06 08:55:48.000000 pandasflow-0.6.1/pandasflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 08:55:48.000000 pandasflow-0.6.1/pandasflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 08:55:48.275485 pandasflow-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 08:55:48.274488 pandasflow-0.6.1/test/
--rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.6.1/test/__init__.py
--rw-rw-rw-   0        0        0      764 2023-06-06 08:45:10.000000 pandasflow-0.6.1/test/best_thr_f1_test.py
--rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.6.1/test/conf_mat_test.py
--rw-rw-rw-   0        0        0      620 2023-05-15 11:59:08.000000 pandasflow-0.6.1/test/lloss_up_test.py
--rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.6.1/test/mean_error_test.py
--rw-rw-rw-   0        0        0     1296 2023-05-07 08:19:28.000000 pandasflow-0.6.1/test/precision_recall_test.py
--rw-rw-rw-   0        0        0     1261 2023-06-06 08:49:02.000000 pandasflow-0.6.1/test/roc_auc_test.py
--rw-rw-rw-   0        0        0      498 2023-05-15 10:14:07.000000 pandasflow-0.6.1/test/split_tt_test.py
--rw-rw-rw-   0        0        0      782 2023-05-15 10:24:03.000000 pandasflow-0.6.1/test/split_tvt_test.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:47:24.330175 pandasflow-0.7.0/
+-rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.7.0/LICENCE
+-rw-rw-rw-   0        0        0      869 2023-06-15 12:47:24.330175 pandasflow-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-05-15 11:35:26.000000 pandasflow-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 12:47:24.306089 pandasflow-0.7.0/pandasflow/
+-rw-rw-rw-   0        0        0      419 2023-06-15 12:47:06.000000 pandasflow-0.7.0/pandasflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:47:24.311075 pandasflow-0.7.0/pandasflow/dev/
+-rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.7.0/pandasflow/dev/__init__.py
+-rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.7.0/pandasflow/dev/err_mean_diff.py
+-rw-rw-rw-   0        0        0      387 2023-05-30 09:54:40.000000 pandasflow-0.7.0/pandasflow/get_import.py
+-rw-rw-rw-   0        0        0      480 2023-05-15 09:05:23.000000 pandasflow-0.7.0/pandasflow/get_psql.py
+-rw-rw-rw-   0        0        0      208 2023-05-15 09:29:01.000000 pandasflow-0.7.0/pandasflow/get_sqlt.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:47:24.316651 pandasflow-0.7.0/pandasflow/metrics/
+-rw-rw-rw-   0        0        0      340 2023-06-06 08:47:33.000000 pandasflow-0.7.0/pandasflow/metrics/__init__.py
+-rw-rw-rw-   0        0        0      801 2023-06-06 08:45:10.000000 pandasflow-0.7.0/pandasflow/metrics/best_thr_f1.py
+-rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.7.0/pandasflow/metrics/conf_mat.py
+-rw-rw-rw-   0        0        0     2173 2023-05-15 11:57:58.000000 pandasflow-0.7.0/pandasflow/metrics/lloss_up.py
+-rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.7.0/pandasflow/metrics/mean_error.py
+-rw-rw-rw-   0        0        0      721 2023-05-07 08:19:28.000000 pandasflow-0.7.0/pandasflow/metrics/precision_recall.py
+-rw-rw-rw-   0        0        0      658 2023-06-06 08:47:33.000000 pandasflow-0.7.0/pandasflow/metrics/roc_auc.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:47:24.318176 pandasflow-0.7.0/pandasflow/model/
+-rw-rw-rw-   0        0        0       88 2023-06-15 10:21:12.000000 pandasflow-0.7.0/pandasflow/model/__init__.py
+-rw-rw-rw-   0        0        0      414 2023-06-15 12:43:42.000000 pandasflow-0.7.0/pandasflow/model/calc_class_from_score.py
+-rw-rw-rw-   0        0        0      622 2023-05-15 12:17:31.000000 pandasflow-0.7.0/pandasflow/reset_mi.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:47:24.318782 pandasflow-0.7.0/pandasflow/services/
+-rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.7.0/pandasflow/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:47:24.320199 pandasflow-0.7.0/pandasflow/split/
+-rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.7.0/pandasflow/split/__init__.py
+-rw-rw-rw-   0        0        0     2835 2023-05-15 10:13:46.000000 pandasflow-0.7.0/pandasflow/split/train_test.py
+-rw-rw-rw-   0        0        0     3944 2023-05-15 10:24:18.000000 pandasflow-0.7.0/pandasflow/split/train_valid_test.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:47:24.309080 pandasflow-0.7.0/pandasflow.egg-info/
+-rw-rw-rw-   0        0        0      869 2023-06-15 12:47:24.000000 pandasflow-0.7.0/pandasflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1051 2023-06-15 12:47:24.000000 pandasflow-0.7.0/pandasflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 12:47:24.000000 pandasflow-0.7.0/pandasflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-15 12:47:24.000000 pandasflow-0.7.0/pandasflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-15 12:47:24.000000 pandasflow-0.7.0/pandasflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 12:47:24.331172 pandasflow-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:47:24.329177 pandasflow-0.7.0/test/
+-rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.7.0/test/__init__.py
+-rw-rw-rw-   0        0        0      764 2023-06-15 10:06:46.000000 pandasflow-0.7.0/test/best_thr_f1_test.py
+-rw-rw-rw-   0        0        0      988 2023-06-15 12:45:29.000000 pandasflow-0.7.0/test/calc_class_from_score_test.py
+-rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.7.0/test/conf_mat_test.py
+-rw-rw-rw-   0        0        0      620 2023-05-15 11:59:08.000000 pandasflow-0.7.0/test/lloss_up_test.py
+-rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.7.0/test/mean_error_test.py
+-rw-rw-rw-   0        0        0     1296 2023-05-07 08:19:28.000000 pandasflow-0.7.0/test/precision_recall_test.py
+-rw-rw-rw-   0        0        0     1261 2023-06-06 08:49:02.000000 pandasflow-0.7.0/test/roc_auc_test.py
+-rw-rw-rw-   0        0        0      498 2023-05-15 10:14:07.000000 pandasflow-0.7.0/test/split_tt_test.py
+-rw-rw-rw-   0        0        0      782 2023-05-15 10:24:03.000000 pandasflow-0.7.0/test/split_tvt_test.py
```

### Comparing `pandasflow-0.6.1/LICENCE` & `pandasflow-0.7.0/LICENCE`

 * *Files identical despite different names*

### Comparing `pandasflow-0.6.1/PKG-INFO` & `pandasflow-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.6.1
+Version: 0.7.0
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.6.1/pandasflow/dev/err_mean_diff.py` & `pandasflow-0.7.0/pandasflow/dev/err_mean_diff.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.6.1/pandasflow/metrics/best_thr_f1.py` & `pandasflow-0.7.0/pandasflow/metrics/best_thr_f1.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.6.1/pandasflow/metrics/conf_mat.py` & `pandasflow-0.7.0/pandasflow/metrics/conf_mat.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.6.1/pandasflow/metrics/lloss_up.py` & `pandasflow-0.7.0/pandasflow/metrics/lloss_up.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.6.1/pandasflow/metrics/precision_recall.py` & `pandasflow-0.7.0/pandasflow/metrics/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.6.1/pandasflow/metrics/roc_auc.py` & `pandasflow-0.7.0/pandasflow/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.6.1/pandasflow/reset_mi.py` & `pandasflow-0.7.0/pandasflow/reset_mi.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.6.1/pandasflow/split/train_test.py` & `pandasflow-0.7.0/pandasflow/split/train_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.6.1/pandasflow/split/train_valid_test.py` & `pandasflow-0.7.0/pandasflow/split/train_valid_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.6.1/pandasflow.egg-info/PKG-INFO` & `pandasflow-0.7.0/pandasflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.6.1
+Version: 0.7.0
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.6.1/pandasflow.egg-info/SOURCES.txt` & `pandasflow-0.7.0/pandasflow.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,20 +18,22 @@
 pandasflow/metrics/best_thr_f1.py
 pandasflow/metrics/conf_mat.py
 pandasflow/metrics/lloss_up.py
 pandasflow/metrics/mean_error.py
 pandasflow/metrics/precision_recall.py
 pandasflow/metrics/roc_auc.py
 pandasflow/model/__init__.py
+pandasflow/model/calc_class_from_score.py
 pandasflow/services/__init__.py
 pandasflow/split/__init__.py
 pandasflow/split/train_test.py
 pandasflow/split/train_valid_test.py
 test/__init__.py
 test/best_thr_f1_test.py
+test/calc_class_from_score_test.py
 test/conf_mat_test.py
 test/lloss_up_test.py
 test/mean_error_test.py
 test/precision_recall_test.py
 test/roc_auc_test.py
 test/split_tt_test.py
 test/split_tvt_test.py
```

### Comparing `pandasflow-0.6.1/setup.py` & `pandasflow-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.6.1/test/best_thr_f1_test.py` & `pandasflow-0.7.0/test/best_thr_f1_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.6.1/test/conf_mat_test.py` & `pandasflow-0.7.0/test/conf_mat_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.6.1/test/lloss_up_test.py` & `pandasflow-0.7.0/test/lloss_up_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.6.1/test/precision_recall_test.py` & `pandasflow-0.7.0/test/precision_recall_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.6.1/test/roc_auc_test.py` & `pandasflow-0.7.0/test/roc_auc_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.6.1/test/split_tvt_test.py` & `pandasflow-0.7.0/test/split_tvt_test.py`

 * *Files identical despite different names*

