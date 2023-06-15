# Comparing `tmp/cubestat-0.0.2.tar.gz` & `tmp/cubestat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubestat-0.0.2.tar", last modified: Fri Jun  9 19:54:09 2023, max compression
+gzip compressed data, was "cubestat-0.0.3.tar", last modified: Thu Jun 15 02:34:08 2023, max compression
```

## Comparing `cubestat-0.0.2.tar` & `cubestat-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:54:09.980810 cubestat-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-09 19:54:00.000000 cubestat-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-09 19:54:09.980810 cubestat-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-06-09 19:54:00.000000 cubestat-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:54:09.980810 cubestat-0.0.2/cubestat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 19:54:00.000000 cubestat-0.0.2/cubestat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10967 2023-06-09 19:54:00.000000 cubestat-0.0.2/cubestat/cubestat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:54:09.980810 cubestat-0.0.2/cubestat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-09 19:54:09.000000 cubestat-0.0.2/cubestat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-09 19:54:09.000000 cubestat-0.0.2/cubestat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 19:54:09.000000 cubestat-0.0.2/cubestat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 19:54:09.000000 cubestat-0.0.2/cubestat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 19:54:09.000000 cubestat-0.0.2/cubestat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 19:54:09.980810 cubestat-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-09 19:54:00.000000 cubestat-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:34:08.900593 cubestat-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-15 02:33:53.000000 cubestat-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-15 02:34:08.900593 cubestat-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-15 02:33:53.000000 cubestat-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:34:08.900593 cubestat-0.0.3/cubestat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 02:33:53.000000 cubestat-0.0.3/cubestat/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15826 2023-06-15 02:33:53.000000 cubestat-0.0.3/cubestat/cubestat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:34:08.900593 cubestat-0.0.3/cubestat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-15 02:34:08.000000 cubestat-0.0.3/cubestat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-15 02:34:08.000000 cubestat-0.0.3/cubestat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 02:34:08.000000 cubestat-0.0.3/cubestat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 02:34:08.000000 cubestat-0.0.3/cubestat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 02:34:08.000000 cubestat-0.0.3/cubestat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 02:34:08.000000 cubestat-0.0.3/cubestat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 02:34:08.900593 cubestat-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-15 02:33:53.000000 cubestat-0.0.3/setup.py
```

### Comparing `cubestat-0.0.2/LICENSE` & `cubestat-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cubestat-0.0.2/README.md` & `cubestat-0.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Horizon charts for Apple M1/M2 monitoring
 
-Command-line utility to monitor CPU/GPU/NeuralEngine utilization on Apple M1/M2 devices. Requires sudo access as it calls `powermetrics` and parses its output.
-Is useful when connecting to another OS X device remotely over ssh. 
+In progress: also working for linux with nVidia GPUs
+
+Command-line utility to monitor CPU/GPU/NeuralEngine utilization on Apple M1/M2 devices as horizon chart. Unfortunately, it requires sudo access as it calls `powermetrics` and parses its output.
+
+cubestat is particularly useful when connecting to another device remotely over ssh. 
 
 Installation:
 ```
 pip3 install cubestat
 ```
 
 ```
@@ -44,26 +47,24 @@
                         be toggled by pressing d.
   --network             show network io. Can be
                         toggled by pressing n.
 ```
 
 Monitors:
 1. CPU utilization - configurable per core ('expanded'), cluster of cores: Efficiency/Performance ('cluster') or both. Is shown as percentage.
-2. GPU utilization. Is shown in percentage.
+2. GPU utilization per GPU. Is shown in percentage.
 3. ANE power consumption. According to `man powermetrics` it is an estimate, but seems working good enough as a proxy to ANE utilization. Is shown as percentage.
 4. Disk and network IO; Is shown in Kb/s.
+5. Memory usage in %
 
 We could add more data from powermetrics (e.g. frequency), but it was adding too much visual noise.
 
 Example: running [deep RL loop](https://github.com/okuvshynov/rlscout) (self play to generate data, model training, model evaluation) on a single MacBook Air M2:
 
-First chart we have playing games to generate data on CPU only (as there's no trained model yet).
-![Self-play RL horizon chart here](static/started_model_eval.png)
-
-Once we have enough data, we start training the model (on GPU):
-![Self-play + training](static/started_training.png)
-
-After we have first model snapshot, we start model evaluation, which runs model inference (on Neural Engine):
-![Self-play + training + eval](static/selfplay_only.png)
+We can see model training (on GPU), self-play (done on 4 performance CPU cores) and model evaluation, which runs inference on Neural Engine:
+![Self-play + training + eval](static/selfplay.png)
 
 Another example running [GPT inference on ggml](https://github.com/ggerganov/ggml): 
-![GPT inference](static/ggml_gpt.png)
+![GPT inference](static/ggml_gpt.png)
+
+Multi-gpu example - training [nano GPT](https://github.com/karpathy/nanoGPT) on 4 GPU instance:
+![nanoGPT](static/ggml_gpt.png)
```

### Comparing `cubestat-0.0.2/setup.py` & `cubestat-0.0.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cubestat',
-    version='0.0.2',
+    version='0.0.3',
     author='Oleksandr Kuvshynov',
     author_email='okuvshynov@gmail.com',
-    description='Horizon chart in terminal for CPU/GPU/ANE monitoring for Apple M1/M2',
-    long_description='Horizon chart in terminal for CPU/GPU/ANE monitoring for Apple M1/M2',
+    description='Horizon chart in terminal for CPU/GPU/ANE monitoring',
+    long_description='Horizon chart in terminal. Supports CPU/GPU/ANE monitoring for Apple M1/M2, nVidia GPUs',
     packages=find_packages(),
+    install_requires=['psutil>=5.9.5'],
     url='https://github.com/okuvshynov/cubestat',
     entry_points={
         'console_scripts': [
             'cubestat = cubestat.cubestat:main'
         ]
     },
 )
```

