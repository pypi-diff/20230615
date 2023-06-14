# Comparing `tmp/neuralprophet-1.0.0rc1.tar.gz` & `tmp/neuralprophet-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralprophet-1.0.0rc1.tar", max compression
+gzip compressed data, was "neuralprophet-1.0.0rc2.tar", max compression
```

## Comparing `neuralprophet-1.0.0rc1.tar` & `neuralprophet-1.0.0rc2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1070 2023-04-11 03:56:33.361031 neuralprophet-1.0.0rc1/LICENSE
--rw-r--r--   0        0        0     7464 2023-04-11 03:56:33.361315 neuralprophet-1.0.0rc1/README.md
--rw-r--r--   0        0        0     1394 2023-04-21 15:39:58.444129 neuralprophet-1.0.0rc1/neuralprophet/__init__.py
--rw-r--r--   0        0        0      398 2023-04-11 03:56:33.495958 neuralprophet-1.0.0rc1/neuralprophet/__main__.py
--rw-r--r--   0        0        0       80 2023-05-01 00:38:34.064106 neuralprophet-1.0.0rc1/neuralprophet/_version.py
--rw-r--r--   0        0        0      683 2023-04-11 03:56:33.496281 neuralprophet-1.0.0rc1/neuralprophet/components/README.md
--rw-r--r--   0        0        0       46 2023-04-11 03:56:33.496404 neuralprophet-1.0.0rc1/neuralprophet/components/__init__.py
--rw-r--r--   0        0        0      931 2023-04-11 03:56:33.496735 neuralprophet-1.0.0rc1/neuralprophet/components/base.py
--rw-r--r--   0        0        0       49 2023-04-11 03:56:33.496919 neuralprophet-1.0.0rc1/neuralprophet/components/future_regressors/__init__.py
--rw-r--r--   0        0        0     1475 2023-04-11 03:56:33.497045 neuralprophet-1.0.0rc1/neuralprophet/components/future_regressors/base.py
--rw-r--r--   0        0        0     3681 2023-04-11 03:56:33.497213 neuralprophet-1.0.0rc1/neuralprophet/components/future_regressors/linear.py
--rw-r--r--   0        0        0     4037 2023-04-11 03:56:33.497388 neuralprophet-1.0.0rc1/neuralprophet/components/router.py
--rw-r--r--   0        0        0       44 2023-04-11 03:56:33.497577 neuralprophet-1.0.0rc1/neuralprophet/components/seasonality/__init__.py
--rw-r--r--   0        0        0      546 2023-04-11 03:56:33.497732 neuralprophet-1.0.0rc1/neuralprophet/components/seasonality/base.py
--rw-r--r--   0        0        0     6233 2023-04-25 00:15:27.316872 neuralprophet-1.0.0rc1/neuralprophet/components/seasonality/fourier.py
--rw-r--r--   0        0        0       38 2023-04-11 03:56:33.498092 neuralprophet-1.0.0rc1/neuralprophet/components/trend/__init__.py
--rw-r--r--   0        0        0     1057 2023-04-11 03:56:33.498379 neuralprophet-1.0.0rc1/neuralprophet/components/trend/base.py
--rw-r--r--   0        0        0     3826 2023-04-11 03:56:33.498530 neuralprophet-1.0.0rc1/neuralprophet/components/trend/linear.py
--rw-r--r--   0        0        0    16977 2023-04-11 03:56:33.498689 neuralprophet-1.0.0rc1/neuralprophet/components/trend/piecewise_linear.py
--rw-r--r--   0        0        0     1192 2023-05-01 00:38:34.066678 neuralprophet-1.0.0rc1/neuralprophet/components/trend/static.py
--rw-r--r--   0        0        0    16539 2023-04-29 03:11:28.086704 neuralprophet-1.0.0rc1/neuralprophet/configure.py
--rw-r--r--   0        0        0     1841 2023-04-11 03:56:33.499338 neuralprophet-1.0.0rc1/neuralprophet/custom_loss_metrics.py
--rw-r--r--   0        0        0    30579 2023-04-26 23:04:01.544631 neuralprophet-1.0.0rc1/neuralprophet/data/process.py
--rw-r--r--   0        0        0    10167 2023-04-26 23:04:01.545927 neuralprophet-1.0.0rc1/neuralprophet/data/split.py
--rw-r--r--   0        0        0     1066 2023-04-25 00:15:27.319938 neuralprophet-1.0.0rc1/neuralprophet/data/transform.py
--rw-r--r--   0        0        0    64143 2023-04-26 23:04:01.547169 neuralprophet-1.0.0rc1/neuralprophet/df_utils.py
--rw-r--r--   0        0        0   129823 2023-05-01 00:38:34.068428 neuralprophet-1.0.0rc1/neuralprophet/forecaster.py
--rw-r--r--   0        0        0      849 2023-04-11 03:56:33.501111 neuralprophet-1.0.0rc1/neuralprophet/hdays_utils.py
--rw-r--r--   0        0        0     2635 2023-04-11 03:56:33.501254 neuralprophet-1.0.0rc1/neuralprophet/logger.py
--rw-r--r--   0        0        0      652 2023-04-25 00:15:27.325505 neuralprophet-1.0.0rc1/neuralprophet/np_types.py
--rw-r--r--   0        0        0    18839 2023-05-01 00:38:34.069551 neuralprophet-1.0.0rc1/neuralprophet/plot_forecast_matplotlib.py
--rw-r--r--   0        0        0    30131 2023-05-01 00:38:34.070758 neuralprophet-1.0.0rc1/neuralprophet/plot_forecast_plotly.py
--rw-r--r--   0        0        0    28822 2023-04-20 23:16:46.978853 neuralprophet-1.0.0rc1/neuralprophet/plot_model_parameters_matplotlib.py
--rw-r--r--   0        0        0    33763 2023-04-28 21:18:49.926179 neuralprophet-1.0.0rc1/neuralprophet/plot_model_parameters_plotly.py
--rw-r--r--   0        0        0    25991 2023-04-28 21:18:49.926766 neuralprophet-1.0.0rc1/neuralprophet/plot_utils.py
--rw-r--r--   0        0        0    30218 2023-05-01 00:38:34.072455 neuralprophet-1.0.0rc1/neuralprophet/time_dataset.py
--rw-r--r--   0        0        0    46087 2023-05-01 00:38:34.074004 neuralprophet-1.0.0rc1/neuralprophet/time_net.py
--rw-r--r--   0        0        0    20958 2023-04-11 03:56:33.504567 neuralprophet-1.0.0rc1/neuralprophet/torch_prophet.py
--rw-r--r--   0        0        0    16350 2023-05-01 00:38:34.077835 neuralprophet-1.0.0rc1/neuralprophet/uncertainty.py
--rw-r--r--   0        0        0    31338 2023-04-28 21:18:49.927939 neuralprophet-1.0.0rc1/neuralprophet/utils.py
--rw-r--r--   0        0        0     1679 2023-04-11 03:56:33.505366 neuralprophet-1.0.0rc1/neuralprophet/utils_metrics.py
--rw-r--r--   0        0        0     4697 2023-04-28 21:18:49.928323 neuralprophet-1.0.0rc1/neuralprophet/utils_torch.py
--rw-r--r--   0        0        0     2323 2023-05-01 00:43:12.288724 neuralprophet-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     9039 1970-01-01 00:00:00.000000 neuralprophet-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-11 03:56:33.361031 neuralprophet-1.0.0rc2/LICENSE
+-rw-r--r--   0        0        0     7464 2023-04-11 03:56:33.361315 neuralprophet-1.0.0rc2/README.md
+-rw-r--r--   0        0        0     1394 2023-04-21 15:39:58.444129 neuralprophet-1.0.0rc2/neuralprophet/__init__.py
+-rw-r--r--   0        0        0      398 2023-04-11 03:56:33.495958 neuralprophet-1.0.0rc2/neuralprophet/__main__.py
+-rw-r--r--   0        0        0       80 2023-05-01 00:38:34.064106 neuralprophet-1.0.0rc2/neuralprophet/_version.py
+-rw-r--r--   0        0        0      683 2023-04-11 03:56:33.496281 neuralprophet-1.0.0rc2/neuralprophet/components/README.md
+-rw-r--r--   0        0        0       46 2023-04-11 03:56:33.496404 neuralprophet-1.0.0rc2/neuralprophet/components/__init__.py
+-rw-r--r--   0        0        0      931 2023-04-11 03:56:33.496735 neuralprophet-1.0.0rc2/neuralprophet/components/base.py
+-rw-r--r--   0        0        0       49 2023-04-11 03:56:33.496919 neuralprophet-1.0.0rc2/neuralprophet/components/future_regressors/__init__.py
+-rw-r--r--   0        0        0     1475 2023-04-11 03:56:33.497045 neuralprophet-1.0.0rc2/neuralprophet/components/future_regressors/base.py
+-rw-r--r--   0        0        0     3681 2023-04-11 03:56:33.497213 neuralprophet-1.0.0rc2/neuralprophet/components/future_regressors/linear.py
+-rw-r--r--   0        0        0     4037 2023-04-11 03:56:33.497388 neuralprophet-1.0.0rc2/neuralprophet/components/router.py
+-rw-r--r--   0        0        0       44 2023-04-11 03:56:33.497577 neuralprophet-1.0.0rc2/neuralprophet/components/seasonality/__init__.py
+-rw-r--r--   0        0        0      546 2023-04-11 03:56:33.497732 neuralprophet-1.0.0rc2/neuralprophet/components/seasonality/base.py
+-rw-r--r--   0        0        0     6233 2023-04-25 00:15:27.316872 neuralprophet-1.0.0rc2/neuralprophet/components/seasonality/fourier.py
+-rw-r--r--   0        0        0       38 2023-04-11 03:56:33.498092 neuralprophet-1.0.0rc2/neuralprophet/components/trend/__init__.py
+-rw-r--r--   0        0        0     1057 2023-04-11 03:56:33.498379 neuralprophet-1.0.0rc2/neuralprophet/components/trend/base.py
+-rw-r--r--   0        0        0     3826 2023-04-11 03:56:33.498530 neuralprophet-1.0.0rc2/neuralprophet/components/trend/linear.py
+-rw-r--r--   0        0        0    16977 2023-04-11 03:56:33.498689 neuralprophet-1.0.0rc2/neuralprophet/components/trend/piecewise_linear.py
+-rw-r--r--   0        0        0     1192 2023-05-01 00:38:34.066678 neuralprophet-1.0.0rc2/neuralprophet/components/trend/static.py
+-rw-r--r--   0        0        0    16539 2023-04-29 03:11:28.086704 neuralprophet-1.0.0rc2/neuralprophet/configure.py
+-rw-r--r--   0        0        0     1841 2023-04-11 03:56:33.499338 neuralprophet-1.0.0rc2/neuralprophet/custom_loss_metrics.py
+-rw-r--r--   0        0        0    30579 2023-04-26 23:04:01.544631 neuralprophet-1.0.0rc2/neuralprophet/data/process.py
+-rw-r--r--   0        0        0    10167 2023-04-26 23:04:01.545927 neuralprophet-1.0.0rc2/neuralprophet/data/split.py
+-rw-r--r--   0        0        0     1066 2023-04-25 00:15:27.319938 neuralprophet-1.0.0rc2/neuralprophet/data/transform.py
+-rw-r--r--   0        0        0    64143 2023-04-26 23:04:01.547169 neuralprophet-1.0.0rc2/neuralprophet/df_utils.py
+-rw-r--r--   0        0        0   129823 2023-05-01 00:38:34.068428 neuralprophet-1.0.0rc2/neuralprophet/forecaster.py
+-rw-r--r--   0        0        0      849 2023-04-11 03:56:33.501111 neuralprophet-1.0.0rc2/neuralprophet/hdays_utils.py
+-rw-r--r--   0        0        0     2635 2023-04-11 03:56:33.501254 neuralprophet-1.0.0rc2/neuralprophet/logger.py
+-rw-r--r--   0        0        0      652 2023-04-25 00:15:27.325505 neuralprophet-1.0.0rc2/neuralprophet/np_types.py
+-rw-r--r--   0        0        0    18839 2023-05-01 00:38:34.069551 neuralprophet-1.0.0rc2/neuralprophet/plot_forecast_matplotlib.py
+-rw-r--r--   0        0        0    30131 2023-05-01 00:38:34.070758 neuralprophet-1.0.0rc2/neuralprophet/plot_forecast_plotly.py
+-rw-r--r--   0        0        0    28822 2023-04-20 23:16:46.978853 neuralprophet-1.0.0rc2/neuralprophet/plot_model_parameters_matplotlib.py
+-rw-r--r--   0        0        0    33763 2023-04-28 21:18:49.926179 neuralprophet-1.0.0rc2/neuralprophet/plot_model_parameters_plotly.py
+-rw-r--r--   0        0        0    25991 2023-04-28 21:18:49.926766 neuralprophet-1.0.0rc2/neuralprophet/plot_utils.py
+-rw-r--r--   0        0        0    30218 2023-05-01 00:38:34.072455 neuralprophet-1.0.0rc2/neuralprophet/time_dataset.py
+-rw-r--r--   0        0        0    46087 2023-05-01 00:38:34.074004 neuralprophet-1.0.0rc2/neuralprophet/time_net.py
+-rw-r--r--   0        0        0    20958 2023-04-11 03:56:33.504567 neuralprophet-1.0.0rc2/neuralprophet/torch_prophet.py
+-rw-r--r--   0        0        0    16350 2023-05-01 00:38:34.077835 neuralprophet-1.0.0rc2/neuralprophet/uncertainty.py
+-rw-r--r--   0        0        0    31338 2023-04-28 21:18:49.927939 neuralprophet-1.0.0rc2/neuralprophet/utils.py
+-rw-r--r--   0        0        0     1679 2023-04-11 03:56:33.505366 neuralprophet-1.0.0rc2/neuralprophet/utils_metrics.py
+-rw-r--r--   0        0        0     4697 2023-04-28 21:18:49.928323 neuralprophet-1.0.0rc2/neuralprophet/utils_torch.py
+-rw-r--r--   0        0        0     2322 2023-05-02 01:54:29.775365 neuralprophet-1.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     9032 1970-01-01 00:00:00.000000 neuralprophet-1.0.0rc2/PKG-INFO
```

### Comparing `neuralprophet-1.0.0rc1/LICENSE` & `neuralprophet-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/README.md` & `neuralprophet-1.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/__init__.py` & `neuralprophet-1.0.0rc2/neuralprophet/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/components/README.md` & `neuralprophet-1.0.0rc2/neuralprophet/components/README.md`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/components/base.py` & `neuralprophet-1.0.0rc2/neuralprophet/components/base.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/components/future_regressors/base.py` & `neuralprophet-1.0.0rc2/neuralprophet/components/future_regressors/base.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/components/future_regressors/linear.py` & `neuralprophet-1.0.0rc2/neuralprophet/components/future_regressors/linear.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/components/router.py` & `neuralprophet-1.0.0rc2/neuralprophet/components/router.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/components/seasonality/base.py` & `neuralprophet-1.0.0rc2/neuralprophet/components/seasonality/base.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/components/seasonality/fourier.py` & `neuralprophet-1.0.0rc2/neuralprophet/components/seasonality/fourier.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/components/trend/base.py` & `neuralprophet-1.0.0rc2/neuralprophet/components/trend/base.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/components/trend/linear.py` & `neuralprophet-1.0.0rc2/neuralprophet/components/trend/linear.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/components/trend/piecewise_linear.py` & `neuralprophet-1.0.0rc2/neuralprophet/components/trend/piecewise_linear.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/components/trend/static.py` & `neuralprophet-1.0.0rc2/neuralprophet/components/trend/static.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/configure.py` & `neuralprophet-1.0.0rc2/neuralprophet/configure.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/custom_loss_metrics.py` & `neuralprophet-1.0.0rc2/neuralprophet/custom_loss_metrics.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/data/process.py` & `neuralprophet-1.0.0rc2/neuralprophet/data/process.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/data/split.py` & `neuralprophet-1.0.0rc2/neuralprophet/data/split.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/data/transform.py` & `neuralprophet-1.0.0rc2/neuralprophet/data/transform.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/df_utils.py` & `neuralprophet-1.0.0rc2/neuralprophet/df_utils.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/forecaster.py` & `neuralprophet-1.0.0rc2/neuralprophet/forecaster.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/hdays_utils.py` & `neuralprophet-1.0.0rc2/neuralprophet/hdays_utils.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/logger.py` & `neuralprophet-1.0.0rc2/neuralprophet/logger.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/np_types.py` & `neuralprophet-1.0.0rc2/neuralprophet/np_types.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/plot_forecast_matplotlib.py` & `neuralprophet-1.0.0rc2/neuralprophet/plot_forecast_matplotlib.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/plot_forecast_plotly.py` & `neuralprophet-1.0.0rc2/neuralprophet/plot_forecast_plotly.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/plot_model_parameters_matplotlib.py` & `neuralprophet-1.0.0rc2/neuralprophet/plot_model_parameters_matplotlib.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/plot_model_parameters_plotly.py` & `neuralprophet-1.0.0rc2/neuralprophet/plot_model_parameters_plotly.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/plot_utils.py` & `neuralprophet-1.0.0rc2/neuralprophet/plot_utils.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/time_dataset.py` & `neuralprophet-1.0.0rc2/neuralprophet/time_dataset.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/time_net.py` & `neuralprophet-1.0.0rc2/neuralprophet/time_net.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/torch_prophet.py` & `neuralprophet-1.0.0rc2/neuralprophet/torch_prophet.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/uncertainty.py` & `neuralprophet-1.0.0rc2/neuralprophet/uncertainty.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/utils.py` & `neuralprophet-1.0.0rc2/neuralprophet/utils.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/utils_metrics.py` & `neuralprophet-1.0.0rc2/neuralprophet/utils_metrics.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/neuralprophet/utils_torch.py` & `neuralprophet-1.0.0rc2/neuralprophet/utils_torch.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-1.0.0rc1/pyproject.toml` & `neuralprophet-1.0.0rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neuralprophet"
-version = "1.0.0rc1"
+version = "1.0.0rc2"
 description = "NeuralProphet is an easy to learn framework for interpretable time series forecasting."
 authors = ["Oskar Triebe <triebe@stanford.edu>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Natural Language :: English",
@@ -21,15 +21,15 @@
 python = ">=3.8,<3.11"
 captum = "^0.6.0"
 holidays = "^0.21"
 matplotlib = "^3.5.3"
 numpy = ">=1.22.0,<1.24.0"
 pandas = "^1.3.5"
 plotly = "^5.13.1"
-kaleido = "^0.2.1"
+kaleido = "0.2.1"
 plotly-resampler = "^0.8.3.1"
 pytorch-lightning = "^1.9.4"
 tensorboard = "^2.11.2"
 torch = "^1.13.1"
 torchmetrics = "^0.11.3"
 typing-extensions = "^4.5.0"
 nbformat = ">=4.2.0"
```

### Comparing `neuralprophet-1.0.0rc1/PKG-INFO` & `neuralprophet-1.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralprophet
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: NeuralProphet is an easy to learn framework for interpretable time series forecasting.
 License: MIT
 Author: Oskar Triebe
 Author-email: triebe@stanford.edu
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: live
 Requires-Dist: captum (>=0.6.0,<0.7.0)
 Requires-Dist: holidays (>=0.21,<0.22)
-Requires-Dist: kaleido (>=0.2.1,<0.3.0)
+Requires-Dist: kaleido (==0.2.1)
 Requires-Dist: livelossplot (>=0.5.5,<0.6.0) ; extra == "live"
 Requires-Dist: matplotlib (>=3.5.3,<4.0.0)
 Requires-Dist: nbformat (>=4.2.0)
 Requires-Dist: numpy (>=1.22.0,<1.24.0)
 Requires-Dist: pandas (>=1.3.5,<2.0.0)
 Requires-Dist: plotly (>=5.13.1,<6.0.0)
 Requires-Dist: plotly-resampler (>=0.8.3.1,<0.9.0.0)
```

