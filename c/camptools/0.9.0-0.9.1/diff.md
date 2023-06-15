# Comparing `tmp/camptools-0.9.0.tar.gz` & `tmp/camptools-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camptools-0.9.0.tar", last modified: Mon Mar 13 14:08:41 2023, max compression
+gzip compressed data, was "camptools-0.9.1.tar", last modified: Thu Jun 15 18:59:58 2023, max compression
```

## Comparing `camptools-0.9.0.tar` & `camptools-0.9.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 14:08:41.892255 camptools-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-13 14:08:31.000000 camptools-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-03-13 14:08:41.892255 camptools-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-03-13 14:08:31.000000 camptools-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 14:08:41.888255 camptools-0.9.0/camptools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/cmdjob.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/conversion_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/create_vdist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/extent_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/filesync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 14:08:41.888255 camptools-0.9.0/camptools/grand/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/grand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/grand/pjsub_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/job_history.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 14:08:41.888255 camptools-0.9.0/camptools/job_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/job_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/job_scheduler/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/job_scheduler/laurel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/job_scheduler/sbatch_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/job_scheduler/throw_job_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/job_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/mymkdir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/qsub_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 14:08:41.892255 camptools-0.9.0/camptools/simmanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/simmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/simmanager/copylist.py
--rw-r--r--   0 runner    (1001) docker     (123)    12942 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/simmanager/simmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/simmanager/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-13 14:08:31.000000 camptools-0.9.0/camptools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 14:08:41.888255 camptools-0.9.0/camptools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-03-13 14:08:41.000000 camptools-0.9.0/camptools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-13 14:08:41.000000 camptools-0.9.0/camptools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 14:08:41.000000 camptools-0.9.0/camptools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-03-13 14:08:41.000000 camptools-0.9.0/camptools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-13 14:08:41.000000 camptools-0.9.0/camptools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-13 14:08:41.000000 camptools-0.9.0/camptools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 14:08:41.892255 camptools-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-03-13 14:08:31.000000 camptools-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:59:58.124682 camptools-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-15 18:59:48.000000 camptools-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-06-15 18:59:58.124682 camptools-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-15 18:59:48.000000 camptools-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:59:58.120682 camptools-0.9.1/camptools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/cmdjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/conversion_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/create_vdist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/extent_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/filesync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:59:58.120682 camptools-0.9.1/camptools/grand/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/grand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/grand/mypjsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/grand/pjsub_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/job_history.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:59:58.124682 camptools-0.9.1/camptools/job_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/job_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/job_scheduler/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/job_scheduler/laurel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/job_scheduler/sbatch_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/job_scheduler/throw_job_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/job_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/mymkdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/qsub_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:59:58.124682 camptools-0.9.1/camptools/simmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/simmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/simmanager/copylist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12942 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/simmanager/simmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/simmanager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-15 18:59:48.000000 camptools-0.9.1/camptools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:59:58.120682 camptools-0.9.1/camptools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-06-15 18:59:58.000000 camptools-0.9.1/camptools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-15 18:59:58.000000 camptools-0.9.1/camptools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 18:59:58.000000 camptools-0.9.1/camptools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-15 18:59:58.000000 camptools-0.9.1/camptools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 18:59:58.000000 camptools-0.9.1/camptools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 18:59:58.000000 camptools-0.9.1/camptools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 18:59:58.124682 camptools-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-15 18:59:48.000000 camptools-0.9.1/setup.py
```

### Comparing `camptools-0.9.0/LICENSE` & `camptools-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `camptools-0.9.0/PKG-INFO` & `camptools-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camptools
-Version: 0.9.0
+Version: 0.9.1
 Summary: Tools for camphor
 Home-page: https://github.com/Nkzono99/camptools
 Author: Nkzono
 Author-email: 71783375+Nkzono99@users.noreply.github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `camptools-0.9.0/README.md` & `camptools-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `camptools-0.9.0/camptools/checkpoint.py` & `camptools-0.9.1/camptools/checkpoint.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.0/camptools/cmdjob.py` & `camptools-0.9.1/camptools/cmdjob.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.0/camptools/conversion_unit.py` & `camptools-0.9.1/camptools/conversion_unit.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.0/camptools/create_vdist.py` & `camptools-0.9.1/camptools/create_vdist.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.0/camptools/extent_sim.py` & `camptools-0.9.1/camptools/extent_sim.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.0/camptools/filesync.py` & `camptools-0.9.1/camptools/filesync.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.0/camptools/grand/pjsub_wrapper.py` & `camptools-0.9.1/camptools/grand/pjsub_wrapper.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.0/camptools/job_history.py` & `camptools-0.9.1/camptools/job_history.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.0/camptools/job_scheduler/core.py` & `camptools-0.9.1/camptools/job_scheduler/core.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.0/camptools/job_scheduler/laurel.py` & `camptools-0.9.1/camptools/job_scheduler/laurel.py`

 * *Files 25% similar despite different names*

```diff
@@ -49,19 +49,16 @@
             if m:
                 return int(m.group(1))
         return None
 
     @nprocs.setter
     def nprocs(self, nprocs: int):
         p = re.compile(r'#SBATCH --rsc p=(\d+)')
-        p_srun = re.compile(r'srun\s+-n\s+(\d+)\s+--ntasks-per-node')
         for i in range(len(self.lines)):
             self.lines[i] = p.sub(f'#SBATCH --rsc p={nprocs}', self.lines[i])
-            self.lines[i] = p_srun.sub(
-                f'srun -n {nprocs} --ntasks-per-node', self.lines[i])
 
     @property
     def exec_time_hour(self):
         p = re.compile(r'#SBATCH -t (\d+):(\d+):(\d+)')
         for line in self.lines:
             m = p.match(line)
             if m:
@@ -90,16 +87,7 @@
 
     @queue_name.setter
     def queue_name(self, queue_name):
         p = re.compile(r'#SBATCH -p (\S+)')
         for i in range(len(self.lines)):
             self.lines[i] = p.sub(f'#SBATCH -p {queue_name}', self.lines[i])
 
-    def finalize_with_nprocs_per_node(self, nprocs_per_node: int = 32):
-        nprocs = self.nprocs
-        self.nprocs = nprocs//nprocs_per_node*40 if nprocs > 40 else nprocs
-
-        p = re.compile(r'--ntasks-per-node=(\d+)')
-        p_srun = re.compile(r'srun\s+-n\s+(\d+)\s+--ntasks-per-node=(\d+)')
-        for i in range(len(self.lines)):
-            self.lines[i] = p_srun.sub(
-                f'srun -n {nprocs} --ntasks-per-node={min(nprocs, nprocs_per_node)}', self.lines[i])
```

### Comparing `camptools-0.9.0/camptools/job_scheduler/sbatch_wrapper.py` & `camptools-0.9.1/camptools/job_scheduler/sbatch_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
         jobfile.queue_name = queue_name
     else:
         queue_limit: QueueLimit = jobqueue.queue_limit_dict[jobfile.queue_name]
         if not queue_limit.can_accept(jobfile.nprocs, jobfile.exec_time_hour):
             jobfile.queue_name = jobqueue.minimum_queue_name(jobfile.nprocs, 
                                                                   jobfile.exec_time_hour)
 
-    jobfile.finalize_with_nprocs_per_node()
     jobfile.save(tmpjob_filepath)
 
 
 def nmysbatch():
     
     args = parse_args()
```

### Comparing `camptools-0.9.0/camptools/job_scheduler/throw_job_wrapper.py` & `camptools-0.9.1/camptools/job_scheduler/throw_job_wrapper.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.0/camptools/job_status.py` & `camptools-0.9.1/camptools/job_status.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.0/camptools/jobs.py` & `camptools-0.9.1/camptools/jobs.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.0/camptools/mymkdir.py` & `camptools-0.9.1/camptools/mymkdir.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.0/camptools/qsub_wrapper.py` & `camptools-0.9.1/camptools/qsub_wrapper.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.0/camptools/settings.py` & `camptools-0.9.1/camptools/settings.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.0/camptools/simmanager/simmanager.py` & `camptools-0.9.1/camptools/simmanager/simmanager.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.0/camptools/simmanager/utils.py` & `camptools-0.9.1/camptools/simmanager/utils.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.0/camptools/utils.py` & `camptools-0.9.1/camptools/utils.py`

 * *Files identical despite different names*

### Comparing `camptools-0.9.0/camptools.egg-info/PKG-INFO` & `camptools-0.9.1/camptools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camptools
-Version: 0.9.0
+Version: 0.9.1
 Summary: Tools for camphor
 Home-page: https://github.com/Nkzono99/camptools
 Author: Nkzono
 Author-email: 71783375+Nkzono99@users.noreply.github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `camptools-0.9.0/camptools.egg-info/SOURCES.txt` & `camptools-0.9.1/camptools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 camptools.egg-info/PKG-INFO
 camptools.egg-info/SOURCES.txt
 camptools.egg-info/dependency_links.txt
 camptools.egg-info/entry_points.txt
 camptools.egg-info/requires.txt
 camptools.egg-info/top_level.txt
 camptools/grand/__init__.py
+camptools/grand/mypjsub.py
 camptools/grand/pjsub_wrapper.py
 camptools/job_scheduler/__init__.py
 camptools/job_scheduler/core.py
 camptools/job_scheduler/laurel.py
 camptools/job_scheduler/sbatch_wrapper.py
 camptools/job_scheduler/throw_job_wrapper.py
 camptools/simmanager/__init__.py
```

### Comparing `camptools-0.9.0/camptools.egg-info/entry_points.txt` & `camptools-0.9.1/camptools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `camptools-0.9.0/setup.py` & `camptools-0.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 
 long_description = open('README.md', 'r', encoding='utf-8').read()
 
 setup(
     name="camptools",
-    version="0.9.0",
+    version="0.9.1",
     install_requires=[
         'f90nml',
     ],
     entry_points={
         'console_scripts': [
             'nmyqsub = camptools.qsub_wrapper:nmyqsub',
             'myqsub = camptools.qsub_wrapper:myqsub',
```

