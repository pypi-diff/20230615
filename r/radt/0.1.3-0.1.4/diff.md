# Comparing `tmp/radt-0.1.3.tar.gz` & `tmp/radt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radt-0.1.3.tar", last modified: Thu Jun 15 15:28:16 2023, max compression
+gzip compressed data, was "radt-0.1.4.tar", last modified: Thu Jun 15 15:30:59 2023, max compression
```

## Comparing `radt-0.1.3.tar` & `radt-0.1.4.tar`

### file list

```diff
@@ -1,72 +1,4 @@
--rw-r--r--   0        0        0     1956 2023-06-15 15:25:53.013963 radt-0.1.3/.gitignore
--rw-r--r--   0        0        0     3602 2023-06-15 15:25:53.013963 radt-0.1.3/README.md
--rwxr-xr-x   0        0        0      252 2023-06-15 15:25:53.013963 radt-0.1.3/clean_mlflow_envs.sh
--rw-r--r--   0        0        0     2063 2023-06-15 15:25:53.013963 radt-0.1.3/docker-compose.yml
--rw-r--r--   0        0        0      184 2023-06-15 15:25:53.013963 radt-0.1.3/environments/mxnet.yaml
--rw-r--r--   0        0        0      219 2023-06-15 15:25:53.013963 radt-0.1.3/environments/pytorch.yaml
--rw-r--r--   0        0        0      203 2023-06-15 15:25:53.013963 radt-0.1.3/environments/tensorflow.yaml
--rw-r--r--   0        0        0      197 2023-06-15 15:25:53.013963 radt-0.1.3/examples/csv/experiment_double.csv
--rw-r--r--   0        0        0      197 2023-06-15 15:25:53.013963 radt-0.1.3/examples/csv/experiment_live.csv
--rw-r--r--   0        0        0        8 2023-06-15 15:25:53.013963 radt-0.1.3/examples/mxnet/readme.md
--rw-r--r--   0        0        0     2656 2023-06-15 15:25:53.013963 radt-0.1.3/examples/pytorch/cifar10.py
--rw-r--r--   0        0        0      550 2023-06-15 15:25:53.013963 radt-0.1.3/examples/pytorch/conda.yaml
--rw-r--r--   0        0        0      175 2023-06-15 15:25:53.013963 radt-0.1.3/examples/pytorch/experiment_folder.csv
--rw-r--r--   0        0        0     2742 2023-06-15 15:25:53.013963 radt-0.1.3/examples/readme.md
--rw-r--r--   0        0        0       13 2023-06-15 15:25:53.013963 radt-0.1.3/examples/tensorflow/readme.md
--rw-r--r--   0        0        0       19 2023-06-15 15:25:53.013963 radt-0.1.3/frontend/.dockerignore
--rw-r--r--   0        0        0      315 2023-06-15 15:25:53.013963 radt-0.1.3/frontend/.gitignore
--rw-r--r--   0        0        0      600 2023-06-15 15:25:53.013963 radt-0.1.3/frontend/Dockerfile
--rw-r--r--   0        0        0      942 2023-06-15 15:25:53.013963 radt-0.1.3/frontend/README.md
--rw-r--r--   0        0        0      150 2023-06-15 15:25:53.013963 radt-0.1.3/frontend/nginx.conf
--rw-r--r--   0        0        0  1200712 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/package-lock.json
--rw-r--r--   0        0        0     1005 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/package.json
--rw-r--r--   0        0        0     3870 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/public/favicon.ico
--rw-r--r--   0        0        0     1721 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/public/index.html
--rw-r--r--   0        0        0     5347 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/public/logo192.png
--rw-r--r--   0        0        0     9664 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/public/logo512.png
--rw-r--r--   0        0        0      492 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/public/manifest.json
--rw-r--r--   0        0        0       67 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/public/robots.txt
--rw-r--r--   0        0        0     4337 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/src/api.js
--rw-r--r--   0        0        0      980 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/src/components/App.js
--rw-r--r--   0        0        0    28907 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/src/components/Chart.js
--rw-r--r--   0        0        0     8642 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/src/components/ChartPicker.js
--rw-r--r--   0        0        0    10701 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/src/components/ChartTester.js
--rw-r--r--   0        0        0    14893 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/src/components/DataPicker.js
--rw-r--r--   0        0        0     1218 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/src/components/LocalDataTest.js
--rw-r--r--   0        0        0  3595959 2023-06-15 15:25:53.157964 radt-0.1.3/frontend/src/data/test_11523.json
--rw-r--r--   0        0        0  3013864 2023-06-15 15:25:53.161964 radt-0.1.3/frontend/src/data/test_12f6a.json
--rw-r--r--   0        0        0  6199800 2023-06-15 15:25:53.177964 radt-0.1.3/frontend/src/data/test_7aa59.json
--rw-r--r--   0        0        0  3914877 2023-06-15 15:25:53.185964 radt-0.1.3/frontend/src/data/test_e3052.json
--rw-r--r--   0        0        0  3590990 2023-06-15 15:25:53.193964 radt-0.1.3/frontend/src/data/test_f1974.json
--rw-r--r--   0        0        0 78472645 2023-06-15 15:25:53.265964 radt-0.1.3/frontend/src/data/test_stress_09fda.json
--rw-r--r--   0        0        0     2159 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/images/cogwheel.svg
--rw-r--r--   0        0        0     1579 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/images/data.svg
--rw-r--r--   0        0        0     2341 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/images/download.svg
--rw-r--r--   0        0        0    19782 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/images/loading.gif
--rw-r--r--   0        0        0     2608 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/images/pie.svg
--rw-r--r--   0        0        0     2543 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/images/upload.svg
--rw-r--r--   0        0        0     1043 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/index.js
--rw-r--r--   0        0        0      362 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/reportWebVitals.js
--rw-r--r--   0        0        0      241 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/setupTests.js
--rw-r--r--   0        0        0     1007 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/styles/App.css
--rw-r--r--   0        0        0     3852 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/styles/Chart.css
--rw-r--r--   0        0        0     4045 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/styles/ChartPicker.css
--rw-r--r--   0        0        0     7988 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/styles/DataPicker.css
--rw-r--r--   0        0        0      257 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/testing/App.test.js
--rw-r--r--   0        0        0    70280 2023-06-15 15:25:53.269964 radt-0.1.3/media/data-collection-white.png
--rw-r--r--   0        0        0   111941 2023-06-15 15:25:53.269964 radt-0.1.3/media/dataflow-white.png
--rw-r--r--   0        0        0    22142 2023-06-15 15:25:53.269964 radt-0.1.3/media/logo_rad.png
--rw-r--r--   0        0        0      465 2023-06-15 15:25:53.269964 radt-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    20811 2023-06-15 15:25:53.269964 radt-0.1.3/radt.py
--rw-r--r--   0        0        0      144 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/README.md
--rw-r--r--   0        0        0      433 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/pyproject.toml
--rw-r--r--   0        0        0      149 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/radtrun/__init__.py
--rw-r--r--   0        0        0       63 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/radtrun/__main__.py
--rw-r--r--   0        0        0        0 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/radtrun/listeners/__init__.py
--rw-r--r--   0        0        0     2165 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/radtrun/listeners/dcgmi_listener.py
--rw-r--r--   0        0        0     1155 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/radtrun/listeners/ps_listener.py
--rw-r--r--   0        0        0     1559 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/radtrun/listeners/smi_listener.py
--rw-r--r--   0        0        0     2705 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/radtrun/listeners/top_listener.py
--rw-r--r--   0        0        0     3156 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/radtrun/mldgpu.py
--rw-r--r--   0        0        0     4871 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/radtrun/radtrun.py
--rw-r--r--   0        0        0     3977 1970-01-01 00:00:00.000000 radt-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      967 2023-06-15 15:30:22.691256 radt-0.1.4/README.md
+-rw-r--r--   0        0        0      465 2023-06-15 15:30:29.443288 radt-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    20811 2023-06-15 15:30:32.691304 radt-0.1.4/radt.py
+-rw-r--r--   0        0        0     1342 1970-01-01 00:00:00.000000 radt-0.1.4/PKG-INFO
```

### Comparing `radt-0.1.3/radt.py` & `radt-0.1.4/radt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Resource-Aware Data systems Tracker (radT) for automatically tracking and training machine learning software"""
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 import argparse
 import numpy as np
 import pandas as pd
 import os
 import sys
 import time
```

