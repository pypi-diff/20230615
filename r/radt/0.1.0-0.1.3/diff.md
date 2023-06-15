# Comparing `tmp/radt-0.1.0.tar.gz` & `tmp/radt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radt-0.1.0.tar", last modified: Thu Jun 15 14:45:34 2023, max compression
+gzip compressed data, was "radt-0.1.3.tar", last modified: Thu Jun 15 15:28:16 2023, max compression
```

## Comparing `radt-0.1.0.tar` & `radt-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,72 @@
--rw-r--r--   0        0        0     1812 2023-06-14 14:03:38.352773 radt-0.1.0/.gitignore
--rw-r--r--   0        0        0       18 2023-06-14 13:00:59.313811 radt-0.1.0/README.md
--rwxr-xr-x   0        0        0      252 2023-06-14 17:56:09.472952 radt-0.1.0/clean_mlflow_envs.sh
--rw-r--r--   0        0        0      382 2023-06-15 08:29:40.010403 radt-0.1.0/examples/csv/experiment_double.csv
--rw-r--r--   0        0        0      193 2023-06-14 17:59:42.917754 radt-0.1.0/examples/csv/experiment_live.csv
--rw-r--r--   0        0        0        8 2023-06-14 13:21:21.505684 radt-0.1.0/examples/mxnet/readme.md
--rw-r--r--   0        0        0      386 2023-06-15 14:05:38.975082 radt-0.1.0/examples/pytorch/MLproject
--rw-r--r--   0        0        0     2656 2023-06-14 13:21:21.505684 radt-0.1.0/examples/pytorch/cifar10.py
--rw-r--r--   0        0        0      550 2023-06-14 17:59:52.369792 radt-0.1.0/examples/pytorch/conda.yaml
--rw-r--r--   0        0        0      175 2023-06-15 10:51:21.727001 radt-0.1.0/examples/pytorch/experiment_folder.csv
--rw-r--r--   0        0        0     2662 2023-06-14 13:21:21.509684 radt-0.1.0/examples/readme.md
--rw-r--r--   0        0        0       13 2023-06-14 13:21:21.509684 radt-0.1.0/examples/tensorflow/readme.md
--rw-r--r--   0        0        0      465 2023-06-15 14:42:52.014440 radt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    20811 2023-06-15 14:19:17.879306 radt-0.1.0/radt.py
--rw-r--r--   0        0        0      144 2023-06-15 14:44:17.450860 radt-0.1.0/radtrun/README.md
--rw-r--r--   0        0        0      433 2023-06-15 14:04:00.478621 radt-0.1.0/radtrun/pyproject.toml
--rw-r--r--   0        0        0       37 2023-06-14 18:45:45.433879 radt-0.1.0/radtrun/radtrun/__init__.py
--rw-r--r--   0        0        0       63 2023-06-14 18:44:41.625589 radt-0.1.0/radtrun/radtrun/__main__.py
--rw-r--r--   0        0        0        0 2023-06-14 18:10:26.872470 radt-0.1.0/radtrun/radtrun/listeners/__init__.py
--rw-r--r--   0        0        0     2165 2023-06-15 10:33:28.277851 radt-0.1.0/radtrun/radtrun/listeners/dcgmi_listener.py
--rw-r--r--   0        0        0     1155 2023-06-14 18:48:25.738606 radt-0.1.0/radtrun/radtrun/listeners/ps_listener.py
--rw-r--r--   0        0        0     1559 2023-06-14 18:48:28.674620 radt-0.1.0/radtrun/radtrun/listeners/smi_listener.py
--rw-r--r--   0        0        0     2705 2023-06-14 18:48:32.002635 radt-0.1.0/radtrun/radtrun/listeners/top_listener.py
--rw-r--r--   0        0        0     3156 2023-06-14 18:47:21.690315 radt-0.1.0/radtrun/radtrun/mldgpu.py
--rw-r--r--   0        0        0     4871 2023-06-15 14:42:51.694439 radt-0.1.0/radtrun/radtrun/radtrun.py
--rw-r--r--   0        0        0      393 1970-01-01 00:00:00.000000 radt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1956 2023-06-15 15:25:53.013963 radt-0.1.3/.gitignore
+-rw-r--r--   0        0        0     3602 2023-06-15 15:25:53.013963 radt-0.1.3/README.md
+-rwxr-xr-x   0        0        0      252 2023-06-15 15:25:53.013963 radt-0.1.3/clean_mlflow_envs.sh
+-rw-r--r--   0        0        0     2063 2023-06-15 15:25:53.013963 radt-0.1.3/docker-compose.yml
+-rw-r--r--   0        0        0      184 2023-06-15 15:25:53.013963 radt-0.1.3/environments/mxnet.yaml
+-rw-r--r--   0        0        0      219 2023-06-15 15:25:53.013963 radt-0.1.3/environments/pytorch.yaml
+-rw-r--r--   0        0        0      203 2023-06-15 15:25:53.013963 radt-0.1.3/environments/tensorflow.yaml
+-rw-r--r--   0        0        0      197 2023-06-15 15:25:53.013963 radt-0.1.3/examples/csv/experiment_double.csv
+-rw-r--r--   0        0        0      197 2023-06-15 15:25:53.013963 radt-0.1.3/examples/csv/experiment_live.csv
+-rw-r--r--   0        0        0        8 2023-06-15 15:25:53.013963 radt-0.1.3/examples/mxnet/readme.md
+-rw-r--r--   0        0        0     2656 2023-06-15 15:25:53.013963 radt-0.1.3/examples/pytorch/cifar10.py
+-rw-r--r--   0        0        0      550 2023-06-15 15:25:53.013963 radt-0.1.3/examples/pytorch/conda.yaml
+-rw-r--r--   0        0        0      175 2023-06-15 15:25:53.013963 radt-0.1.3/examples/pytorch/experiment_folder.csv
+-rw-r--r--   0        0        0     2742 2023-06-15 15:25:53.013963 radt-0.1.3/examples/readme.md
+-rw-r--r--   0        0        0       13 2023-06-15 15:25:53.013963 radt-0.1.3/examples/tensorflow/readme.md
+-rw-r--r--   0        0        0       19 2023-06-15 15:25:53.013963 radt-0.1.3/frontend/.dockerignore
+-rw-r--r--   0        0        0      315 2023-06-15 15:25:53.013963 radt-0.1.3/frontend/.gitignore
+-rw-r--r--   0        0        0      600 2023-06-15 15:25:53.013963 radt-0.1.3/frontend/Dockerfile
+-rw-r--r--   0        0        0      942 2023-06-15 15:25:53.013963 radt-0.1.3/frontend/README.md
+-rw-r--r--   0        0        0      150 2023-06-15 15:25:53.013963 radt-0.1.3/frontend/nginx.conf
+-rw-r--r--   0        0        0  1200712 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/package-lock.json
+-rw-r--r--   0        0        0     1005 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/package.json
+-rw-r--r--   0        0        0     3870 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/public/favicon.ico
+-rw-r--r--   0        0        0     1721 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/public/index.html
+-rw-r--r--   0        0        0     5347 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/public/logo192.png
+-rw-r--r--   0        0        0     9664 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/public/logo512.png
+-rw-r--r--   0        0        0      492 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/public/manifest.json
+-rw-r--r--   0        0        0       67 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/public/robots.txt
+-rw-r--r--   0        0        0     4337 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/src/api.js
+-rw-r--r--   0        0        0      980 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/src/components/App.js
+-rw-r--r--   0        0        0    28907 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/src/components/Chart.js
+-rw-r--r--   0        0        0     8642 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/src/components/ChartPicker.js
+-rw-r--r--   0        0        0    10701 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/src/components/ChartTester.js
+-rw-r--r--   0        0        0    14893 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/src/components/DataPicker.js
+-rw-r--r--   0        0        0     1218 2023-06-15 15:25:53.017963 radt-0.1.3/frontend/src/components/LocalDataTest.js
+-rw-r--r--   0        0        0  3595959 2023-06-15 15:25:53.157964 radt-0.1.3/frontend/src/data/test_11523.json
+-rw-r--r--   0        0        0  3013864 2023-06-15 15:25:53.161964 radt-0.1.3/frontend/src/data/test_12f6a.json
+-rw-r--r--   0        0        0  6199800 2023-06-15 15:25:53.177964 radt-0.1.3/frontend/src/data/test_7aa59.json
+-rw-r--r--   0        0        0  3914877 2023-06-15 15:25:53.185964 radt-0.1.3/frontend/src/data/test_e3052.json
+-rw-r--r--   0        0        0  3590990 2023-06-15 15:25:53.193964 radt-0.1.3/frontend/src/data/test_f1974.json
+-rw-r--r--   0        0        0 78472645 2023-06-15 15:25:53.265964 radt-0.1.3/frontend/src/data/test_stress_09fda.json
+-rw-r--r--   0        0        0     2159 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/images/cogwheel.svg
+-rw-r--r--   0        0        0     1579 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/images/data.svg
+-rw-r--r--   0        0        0     2341 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/images/download.svg
+-rw-r--r--   0        0        0    19782 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/images/loading.gif
+-rw-r--r--   0        0        0     2608 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/images/pie.svg
+-rw-r--r--   0        0        0     2543 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/images/upload.svg
+-rw-r--r--   0        0        0     1043 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/index.js
+-rw-r--r--   0        0        0      362 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/reportWebVitals.js
+-rw-r--r--   0        0        0      241 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/setupTests.js
+-rw-r--r--   0        0        0     1007 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/styles/App.css
+-rw-r--r--   0        0        0     3852 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/styles/Chart.css
+-rw-r--r--   0        0        0     4045 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/styles/ChartPicker.css
+-rw-r--r--   0        0        0     7988 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/styles/DataPicker.css
+-rw-r--r--   0        0        0      257 2023-06-15 15:25:53.269964 radt-0.1.3/frontend/src/testing/App.test.js
+-rw-r--r--   0        0        0    70280 2023-06-15 15:25:53.269964 radt-0.1.3/media/data-collection-white.png
+-rw-r--r--   0        0        0   111941 2023-06-15 15:25:53.269964 radt-0.1.3/media/dataflow-white.png
+-rw-r--r--   0        0        0    22142 2023-06-15 15:25:53.269964 radt-0.1.3/media/logo_rad.png
+-rw-r--r--   0        0        0      465 2023-06-15 15:25:53.269964 radt-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    20811 2023-06-15 15:25:53.269964 radt-0.1.3/radt.py
+-rw-r--r--   0        0        0      144 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/README.md
+-rw-r--r--   0        0        0      433 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/pyproject.toml
+-rw-r--r--   0        0        0      149 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/radtrun/__init__.py
+-rw-r--r--   0        0        0       63 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/radtrun/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/radtrun/listeners/__init__.py
+-rw-r--r--   0        0        0     2165 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/radtrun/listeners/dcgmi_listener.py
+-rw-r--r--   0        0        0     1155 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/radtrun/listeners/ps_listener.py
+-rw-r--r--   0        0        0     1559 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/radtrun/listeners/smi_listener.py
+-rw-r--r--   0        0        0     2705 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/radtrun/listeners/top_listener.py
+-rw-r--r--   0        0        0     3156 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/radtrun/mldgpu.py
+-rw-r--r--   0        0        0     4871 2023-06-15 15:25:53.269964 radt-0.1.3/radtrun/radtrun/radtrun.py
+-rw-r--r--   0        0        0     3977 1970-01-01 00:00:00.000000 radt-0.1.3/PKG-INFO
```

### Comparing `radt-0.1.0/.gitignore` & `radt-0.1.3/.gitignore`

 * *Files 16% similar despite different names*

```diff
@@ -123,9 +123,25 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+*pth.tar
+*_metric.csv
+*_metric.xlsx
+
+.DS_Store
+*.xlsx
+mlruns
+output
+
+temp
+*.temp
+pretrained-bert
+pretrainer-bert
+screenlog*
+_run_temp.csv
 .vscode
-data
+MLproject
```

### Comparing `radt-0.1.0/examples/pytorch/cifar10.py` & `radt-0.1.3/examples/pytorch/cifar10.py`

 * *Files identical despite different names*

### Comparing `radt-0.1.0/examples/pytorch/conda.yaml` & `radt-0.1.3/examples/pytorch/conda.yaml`

 * *Files identical despite different names*

### Comparing `radt-0.1.0/examples/readme.md` & `radt-0.1.3/examples/readme.md`

 * *Files 10% similar despite different names*

```diff
@@ -85,83 +85,88 @@
 00000540: 6874 7470 733a 2f2f 6875 622e 646f 636b  https://hub.dock
 00000550: 6572 2e63 6f6d 2f5f 2f70 6f73 7467 7265  er.com/_/postgre
 00000560: 7329 0a2d 205b 506f 7374 6752 4553 545d  s).- [PostgREST]
 00000570: 2868 7474 7073 3a2f 2f68 7562 2e64 6f63  (https://hub.doc
 00000580: 6b65 722e 636f 6d2f 722f 706f 7374 6772  ker.com/r/postgr
 00000590: 6573 742f 706f 7374 6772 6573 742f 290a  est/postgrest/).
 000005a0: 2d20 5b52 4144 5420 5669 7375 616c 6973  - [RADT Visualis
-000005b0: 6174 696f 6e20 544f 444f 5d28 6874 7470  ation TODO](http
-000005c0: 733a 2f2f 4c49 4e4b 5f4d 4953 5349 4e47  s://LINK_MISSING
-000005d0: 290a 0a23 2323 202a 2a33 2e20 4672 6f6d  )..### **3. From
-000005e0: 2073 6f75 7263 652a 2a0a 0a49 6620 796f   source**..If yo
-000005f0: 7520 646f 206e 6f74 2077 616e 7420 746f  u do not want to
-00000600: 2075 7365 2063 6f6e 7461 696e 6572 732c   use containers,
-00000610: 2079 6f75 2063 616e 2064 6570 6c6f 7920   you can deploy 
-00000620: 7468 6520 736f 6674 7761 7265 206d 616e  the software man
-00000630: 7561 6c6c 792e 0a43 6c6f 6e65 2074 6869  ually..Clone thi
-00000640: 7320 7265 706f 7369 746f 7279 2061 6e64  s repository and
-00000650: 2066 6f6c 6c6f 7720 7468 6520 696e 7374   follow the inst
-00000660: 7275 6374 696f 6e73 2069 6e20 5b76 6973  ructions in [vis
-00000670: 7561 6c69 7a61 7469 6f6e 5d28 2f76 6973  ualization](/vis
-00000680: 7561 6c69 7a61 7469 6f6e 2920 746f 2062  ualization) to b
-00000690: 7569 6c64 2074 6865 2076 6973 7561 6c69  uild the visuali
-000006a0: 7a61 7469 6f6e 2065 6e76 6972 6f6e 6d65  zation environme
-000006b0: 6e74 206d 616e 7561 6c6c 792e 0a0a 2323  nt manually...##
-000006c0: 2043 6c69 656e 7420 636f 6e66 6967 7572   Client configur
-000006d0: 6174 696f 6e0a 0a42 6566 6f72 6520 7275  ation..Before ru
-000006e0: 6e6e 696e 6720 6578 616d 706c 6573 206d  nning examples m
-000006f0: 616b 6520 7375 7265 2079 6f75 2069 6e73  ake sure you ins
-00000700: 7461 6c6c 2074 6865 2072 6571 7569 7265  tall the require
-00000710: 6d65 6e74 732e 2057 6520 7265 636f 6d6d  ments. We recomm
-00000720: 656e 6420 7573 696e 6720 416e 6163 6f6e  end using Anacon
-00000730: 6461 2066 6f72 2065 6e76 6972 6f6e 6d65  da for environme
-00000740: 6e74 206d 616e 6167 656d 656e 742e 2045  nt management. E
-00000750: 7861 6d70 6c65 7320 636f 6d65 2062 756e  xamples come bun
-00000760: 646c 6564 2077 6974 6820 6120 6063 6f6e  dled with a `con
-00000770: 6461 2e79 616d 6c60 2066 696c 6520 7768  da.yaml` file wh
-00000780: 6963 6820 6361 6e20 6265 2075 7365 6420  ich can be used 
-00000790: 746f 2063 7265 6174 6520 7468 6520 7265  to create the re
-000007a0: 7175 6973 6974 6520 656e 7669 726f 6e6d  quisite environm
-000007b0: 656e 743a 0a0a 6060 6062 6173 680a 636f  ent:..```bash.co
-000007c0: 6e64 6120 656e 7620 6372 6561 7465 202d  nda env create -
-000007d0: 6620 636f 6e64 612e 7961 6d6c 0a60 6060  f conda.yaml.```
-000007e0: 0a0a 4675 7274 6865 726d 6f72 652c 204d  ..Furthermore, M
-000007f0: 4c46 6c6f 7720 7265 7175 6972 6573 2061  LFlow requires a
-00000800: 2073 656c 6563 7469 6f6e 206f 6620 656e   selection of en
-00000810: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
-00000820: 6c65 7320 746f 2062 6520 7365 7420 696e  les to be set in
-00000830: 2074 6865 2065 6e76 6972 6f6e 6d65 6e74   the environment
-00000840: 2062 6566 6f72 6520 6f70 6572 6174 696f   before operatio
-00000850: 6e3a 0a0a 6060 6062 6173 680a 636f 6e64  n:..```bash.cond
-00000860: 6120 656e 7620 636f 6e66 6967 2076 6172  a env config var
-00000870: 7320 7365 7420 4d4c 464c 4f57 5f54 5241  s set MLFLOW_TRA
-00000880: 434b 494e 475f 5553 4552 4e41 4d45 3d0a  CKING_USERNAME=.
-00000890: 636f 6e64 6120 656e 7620 636f 6e66 6967  conda env config
-000008a0: 2076 6172 7320 7365 7420 4d4c 464c 4f57   vars set MLFLOW
-000008b0: 5f54 5241 434b 494e 475f 5041 5353 574f  _TRACKING_PASSWO
-000008c0: 5244 3d0a 636f 6e64 6120 656e 7620 636f  RD=.conda env co
-000008d0: 6e66 6967 2076 6172 7320 7365 7420 4d4c  nfig vars set ML
-000008e0: 464c 4f57 5f53 335f 454e 4450 4f49 4e54  FLOW_S3_ENDPOINT
-000008f0: 5f55 524c 3d0a 636f 6e64 6120 656e 7620  _URL=.conda env 
-00000900: 636f 6e66 6967 2076 6172 7320 7365 7420  config vars set 
-00000910: 4157 535f 4143 4345 5353 5f4b 4559 5f49  AWS_ACCESS_KEY_I
-00000920: 443d 0a63 6f6e 6461 2065 6e76 2063 6f6e  D=.conda env con
-00000930: 6669 6720 7661 7273 2073 6574 2041 5753  fig vars set AWS
-00000940: 5f53 4543 5245 545f 4143 4345 5353 5f4b  _SECRET_ACCESS_K
-00000950: 4559 3d0a 636f 6e64 6120 656e 7620 636f  EY=.conda env co
-00000960: 6e66 6967 2076 6172 7320 7365 7420 4d4c  nfig vars set ML
-00000970: 464c 4f57 5f54 5241 434b 494e 475f 5552  FLOW_TRACKING_UR
-00000980: 493d 0a60 6060 0a0a 2323 2052 756e 6e69  I=.```..## Runni
-00000990: 6e67 2045 7861 6d70 6c65 730a 0a41 6c6c  ng Examples..All
-000009a0: 2065 7861 6d70 6c65 7320 7368 6f75 6c64   examples should
-000009b0: 2072 756e 2076 6961 2060 7261 6474 206d   run via `radt m
-000009c0: 6169 6e2e 7079 6020 756e 6c65 7373 2073  ain.py` unless s
-000009d0: 7065 6369 6669 6564 2e0a 0a2a 2a45 7861  pecified...**Exa
-000009e0: 6d70 6c65 7320 7368 6f75 6c64 2077 6f72  mples should wor
-000009f0: 6b20 6f75 7420 6f66 2074 6865 2062 6f78  k out of the box
-00000a00: 2075 7369 6e67 2074 6865 2073 7570 706c   using the suppl
-00000a10: 6965 6420 636f 6e64 6120 656e 7669 726f  ied conda enviro
-00000a20: 6e6d 656e 7421 2a2a 0a0a 2323 204f 7468  nment!**..## Oth
-00000a30: 6572 2045 7861 6d70 6c65 730a 0a50 6c65  er Examples..Ple
-00000a40: 6173 6520 6665 656c 2066 7265 6520 746f  ase feel free to
-00000a50: 2063 6f6e 7472 6962 7574 6520 6578 616d   contribute exam
-00000a60: 706c 6573 210a                           ples!.
+000005b0: 6174 696f 6e5d 2868 7474 7073 3a2f 2f4c  ation](https://L
+000005c0: 494e 4b5f 4d49 5353 494e 4729 0a0a 2323  INK_MISSING)..##
+000005d0: 2320 2a2a 332e 2046 726f 6d20 736f 7572  # **3. From sour
+000005e0: 6365 2a2a 0a0a 4966 2079 6f75 2064 6f20  ce**..If you do 
+000005f0: 6e6f 7420 7761 6e74 2074 6f20 7573 6520  not want to use 
+00000600: 636f 6e74 6169 6e65 7273 2c20 796f 7520  containers, you 
+00000610: 6361 6e20 6465 706c 6f79 2074 6865 2073  can deploy the s
+00000620: 6f66 7477 6172 6520 6d61 6e75 616c 6c79  oftware manually
+00000630: 2e0a 436c 6f6e 6520 7468 6973 2072 6570  ..Clone this rep
+00000640: 6f73 6974 6f72 7920 616e 6420 666f 6c6c  ository and foll
+00000650: 6f77 2074 6865 2069 6e73 7472 7563 7469  ow the instructi
+00000660: 6f6e 7320 696e 205b 7669 7375 616c 697a  ons in [visualiz
+00000670: 6174 696f 6e5d 282f 7669 7375 616c 697a  ation](/visualiz
+00000680: 6174 696f 6e29 2074 6f20 6275 696c 6420  ation) to build 
+00000690: 7468 6520 7669 7375 616c 697a 6174 696f  the visualizatio
+000006a0: 6e20 656e 7669 726f 6e6d 656e 7420 6d61  n environment ma
+000006b0: 6e75 616c 6c79 2e0a 0a23 2320 436c 6965  nually...## Clie
+000006c0: 6e74 2063 6f6e 6669 6775 7261 7469 6f6e  nt configuration
+000006d0: 0a0a 4265 666f 7265 2072 756e 6e69 6e67  ..Before running
+000006e0: 2065 7861 6d70 6c65 7320 6d61 6b65 2073   examples make s
+000006f0: 7572 6520 796f 7520 696e 7374 616c 6c20  ure you install 
+00000700: 7468 6520 7265 7175 6972 656d 656e 7473  the requirements
+00000710: 2e20 5765 2072 6563 6f6d 6d65 6e64 2075  . We recommend u
+00000720: 7369 6e67 2041 6e61 636f 6e64 6120 666f  sing Anaconda fo
+00000730: 7220 656e 7669 726f 6e6d 656e 7420 6d61  r environment ma
+00000740: 6e61 6765 6d65 6e74 2e20 4578 616d 706c  nagement. Exampl
+00000750: 6573 2063 6f6d 6520 6275 6e64 6c65 6420  es come bundled 
+00000760: 7769 7468 2061 2060 636f 6e64 612e 7961  with a `conda.ya
+00000770: 6d6c 6020 6669 6c65 2077 6869 6368 2063  ml` file which c
+00000780: 616e 2062 6520 7573 6564 2074 6f20 6372  an be used to cr
+00000790: 6561 7465 2074 6865 2072 6571 7569 7369  eate the requisi
+000007a0: 7465 2065 6e76 6972 6f6e 6d65 6e74 3a0a  te environment:.
+000007b0: 0a60 6060 6261 7368 0a63 6f6e 6461 2065  .```bash.conda e
+000007c0: 6e76 2063 7265 6174 6520 2d66 2063 6f6e  nv create -f con
+000007d0: 6461 2e79 616d 6c0a 6060 600a 0a46 7572  da.yaml.```..Fur
+000007e0: 7468 6572 6d6f 7265 2c20 4d4c 466c 6f77  thermore, MLFlow
+000007f0: 2072 6571 7569 7265 7320 6120 7365 6c65   requires a sele
+00000800: 6374 696f 6e20 6f66 2065 6e76 6972 6f6e  ction of environ
+00000810: 6d65 6e74 2076 6172 6961 626c 6573 2074  ment variables t
+00000820: 6f20 6265 2073 6574 2069 6e20 7468 6520  o be set in the 
+00000830: 656e 7669 726f 6e6d 656e 7420 6265 666f  environment befo
+00000840: 7265 206f 7065 7261 7469 6f6e 3a0a 0a60  re operation:..`
+00000850: 6060 6261 7368 0a63 6f6e 6461 2065 6e76  ``bash.conda env
+00000860: 2063 6f6e 6669 6720 7661 7273 2073 6574   config vars set
+00000870: 204d 4c46 4c4f 575f 5452 4143 4b49 4e47   MLFLOW_TRACKING
+00000880: 5f55 5345 524e 414d 453d 0a63 6f6e 6461  _USERNAME=.conda
+00000890: 2065 6e76 2063 6f6e 6669 6720 7661 7273   env config vars
+000008a0: 2073 6574 204d 4c46 4c4f 575f 5452 4143   set MLFLOW_TRAC
+000008b0: 4b49 4e47 5f50 4153 5357 4f52 443d 0a63  KING_PASSWORD=.c
+000008c0: 6f6e 6461 2065 6e76 2063 6f6e 6669 6720  onda env config 
+000008d0: 7661 7273 2073 6574 204d 4c46 4c4f 575f  vars set MLFLOW_
+000008e0: 5333 5f45 4e44 504f 494e 545f 5552 4c3d  S3_ENDPOINT_URL=
+000008f0: 0a63 6f6e 6461 2065 6e76 2063 6f6e 6669  .conda env confi
+00000900: 6720 7661 7273 2073 6574 2041 5753 5f41  g vars set AWS_A
+00000910: 4343 4553 535f 4b45 595f 4944 3d0a 636f  CCESS_KEY_ID=.co
+00000920: 6e64 6120 656e 7620 636f 6e66 6967 2076  nda env config v
+00000930: 6172 7320 7365 7420 4157 535f 5345 4352  ars set AWS_SECR
+00000940: 4554 5f41 4343 4553 535f 4b45 593d 0a63  ET_ACCESS_KEY=.c
+00000950: 6f6e 6461 2065 6e76 2063 6f6e 6669 6720  onda env config 
+00000960: 7661 7273 2073 6574 204d 4c46 4c4f 575f  vars set MLFLOW_
+00000970: 5452 4143 4b49 4e47 5f55 5249 3d0a 6060  TRACKING_URI=.``
+00000980: 600a 0a23 2320 5275 6e6e 696e 6720 4578  `..## Running Ex
+00000990: 616d 706c 6573 0a0a 416c 6c20 6578 616d  amples..All exam
+000009a0: 706c 6573 2073 686f 756c 6420 7275 6e20  ples should run 
+000009b0: 7669 6120 6072 6164 7420 3c73 6372 6970  via `radt <scrip
+000009c0: 743e 2e70 7960 2075 6e6c 6573 7320 7370  t>.py` unless sp
+000009d0: 6563 6966 6965 642e 0a72 6164 5420 7769  ecified..radT wi
+000009e0: 6c6c 2061 7574 6f6d 6174 6963 616c 6c79  ll automatically
+000009f0: 2073 7570 706c 7920 4d4c 7072 6f6a 6563   supply MLprojec
+00000a00: 7420 6669 6c65 7320 666f 7220 4d4c 466c  t files for MLFl
+00000a10: 6f77 2074 6f20 6675 6e63 7469 6f6e 2063  ow to function c
+00000a20: 6f72 7265 6374 6c79 2e0a 0a2a 2a45 7861  orrectly...**Exa
+00000a30: 6d70 6c65 7320 7368 6f75 6c64 2077 6f72  mples should wor
+00000a40: 6b20 6f75 7420 6f66 2074 6865 2062 6f78  k out of the box
+00000a50: 2075 7369 6e67 2074 6865 2073 7570 706c   using the suppl
+00000a60: 6965 6420 636f 6e64 6120 656e 7669 726f  ied conda enviro
+00000a70: 6e6d 656e 7421 2a2a 0a0a 2323 204f 7468  nment!**..## Oth
+00000a80: 6572 2045 7861 6d70 6c65 730a 0a50 6c65  er Examples..Ple
+00000a90: 6173 6520 6665 656c 2066 7265 6520 746f  ase feel free to
+00000aa0: 2063 6f6e 7472 6962 7574 6520 6578 616d   contribute exam
+00000ab0: 706c 6573 210a                           ples!.
```

### Comparing `radt-0.1.0/radt.py` & `radt-0.1.3/radt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Resource-Aware Data systems Tracker (radT) for automatically tracking and training machine learning software"""
 
-__version__ = "0.1.0"
+__version__ = "0.1.3"
 
 import argparse
 import numpy as np
 import pandas as pd
 import os
 import sys
 import time
```

### Comparing `radt-0.1.0/radtrun/radtrun/listeners/dcgmi_listener.py` & `radt-0.1.3/radtrun/radtrun/listeners/dcgmi_listener.py`

 * *Files identical despite different names*

### Comparing `radt-0.1.0/radtrun/radtrun/listeners/ps_listener.py` & `radt-0.1.3/radtrun/radtrun/listeners/ps_listener.py`

 * *Files identical despite different names*

### Comparing `radt-0.1.0/radtrun/radtrun/listeners/smi_listener.py` & `radt-0.1.3/radtrun/radtrun/listeners/smi_listener.py`

 * *Files identical despite different names*

### Comparing `radt-0.1.0/radtrun/radtrun/listeners/top_listener.py` & `radt-0.1.3/radtrun/radtrun/listeners/top_listener.py`

 * *Files identical despite different names*

### Comparing `radt-0.1.0/radtrun/radtrun/mldgpu.py` & `radt-0.1.3/radtrun/radtrun/mldgpu.py`

 * *Files identical despite different names*

### Comparing `radt-0.1.0/radtrun/radtrun/radtrun.py` & `radt-0.1.3/radtrun/radtrun/radtrun.py`

 * *Files identical despite different names*

