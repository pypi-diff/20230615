# Comparing `tmp/dask-jobqueue-0.8.1.tar.gz` & `tmp/dask-jobqueue-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-jobqueue-0.8.1.tar", last modified: Tue Oct  4 17:17:06 2022, max compression
+gzip compressed data, was "dask-jobqueue-0.8.2.tar", last modified: Thu Jun 15 04:23:42 2023, max compression
```

## Comparing `dask-jobqueue-0.8.1.tar` & `dask-jobqueue-0.8.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2022-10-04 17:17:06.651677 dask-jobqueue-0.8.1/
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     1483 2022-08-02 17:50:42.000000 dask-jobqueue-0.8.1/LICENSE.txt
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)      260 2022-08-02 17:50:42.000000 dask-jobqueue-0.8.1/MANIFEST.in
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     1363 2022-10-04 17:17:06.651677 dask-jobqueue-0.8.1/PKG-INFO
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     1104 2022-08-02 17:50:42.000000 dask-jobqueue-0.8.1/README.rst
-drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2022-10-04 17:17:06.651677 dask-jobqueue-0.8.1/dask_jobqueue/
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)      376 2022-08-02 17:50:42.000000 dask-jobqueue-0.8.1/dask_jobqueue/__init__.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)      497 2022-10-04 17:17:06.651677 dask-jobqueue-0.8.1/dask_jobqueue/_version.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)      282 2022-08-07 18:06:52.000000 dask-jobqueue-0.8.1/dask_jobqueue/config.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)    31513 2022-10-04 16:31:30.000000 dask-jobqueue-0.8.1/dask_jobqueue/core.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     8682 2022-09-05 16:33:40.000000 dask-jobqueue-0.8.1/dask_jobqueue/htcondor.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     9377 2022-09-06 06:50:50.000000 dask-jobqueue-0.8.1/dask_jobqueue/jobqueue.yaml
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     2918 2022-08-29 11:06:01.000000 dask-jobqueue-0.8.1/dask_jobqueue/local.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     8986 2022-09-06 06:50:50.000000 dask-jobqueue-0.8.1/dask_jobqueue/lsf.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)      272 2022-08-02 17:50:42.000000 dask-jobqueue-0.8.1/dask_jobqueue/moab.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     5294 2022-09-06 06:50:50.000000 dask-jobqueue-0.8.1/dask_jobqueue/oar.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     5658 2022-09-06 06:50:50.000000 dask-jobqueue-0.8.1/dask_jobqueue/pbs.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     3981 2022-09-06 06:50:50.000000 dask-jobqueue-0.8.1/dask_jobqueue/sge.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     5962 2022-09-06 06:50:50.000000 dask-jobqueue-0.8.1/dask_jobqueue/slurm.py
-drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2022-10-04 17:17:06.651677 dask-jobqueue-0.8.1/dask_jobqueue/tests/
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       27 2022-08-02 17:50:42.000000 dask-jobqueue-0.8.1/dask_jobqueue/tests/__init__.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     5236 2022-08-29 11:06:01.000000 dask-jobqueue-0.8.1/dask_jobqueue/tests/test_htcondor.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)    14488 2022-09-12 09:22:31.000000 dask-jobqueue-0.8.1/dask_jobqueue/tests/test_job.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)    16914 2022-09-12 17:22:59.000000 dask-jobqueue-0.8.1/dask_jobqueue/tests/test_jobqueue_core.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)    12583 2022-08-29 11:06:01.000000 dask-jobqueue-0.8.1/dask_jobqueue/tests/test_lsf.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     4269 2022-08-29 11:06:01.000000 dask-jobqueue-0.8.1/dask_jobqueue/tests/test_oar.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)    13797 2022-09-06 06:50:50.000000 dask-jobqueue-0.8.1/dask_jobqueue/tests/test_pbs.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     3871 2022-08-29 11:06:01.000000 dask-jobqueue-0.8.1/dask_jobqueue/tests/test_sge.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     9848 2022-09-06 06:50:50.000000 dask-jobqueue-0.8.1/dask_jobqueue/tests/test_slurm.py
-drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2022-10-04 17:17:06.651677 dask-jobqueue-0.8.1/dask_jobqueue.egg-info/
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     1363 2022-10-04 17:17:06.000000 dask-jobqueue-0.8.1/dask_jobqueue.egg-info/PKG-INFO
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)      913 2022-10-04 17:17:06.000000 dask-jobqueue-0.8.1/dask_jobqueue.egg-info/SOURCES.txt
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)        1 2022-10-04 17:17:06.000000 dask-jobqueue-0.8.1/dask_jobqueue.egg-info/dependency_links.txt
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)        1 2022-10-04 17:17:06.000000 dask-jobqueue-0.8.1/dask_jobqueue.egg-info/not-zip-safe
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       82 2022-10-04 17:17:06.000000 dask-jobqueue-0.8.1/dask_jobqueue.egg-info/requires.txt
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       14 2022-10-04 17:17:06.000000 dask-jobqueue-0.8.1/dask_jobqueue.egg-info/top_level.txt
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       39 2022-08-07 19:31:48.000000 dask-jobqueue-0.8.1/requirements.txt
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)      457 2022-10-04 17:17:06.651677 dask-jobqueue-0.8.1/setup.cfg
--rwxrwxr-x   0 guillaume  (1000) guillaume  (1000)      947 2022-08-07 18:06:52.000000 dask-jobqueue-0.8.1/setup.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)    68748 2022-08-07 18:06:52.000000 dask-jobqueue-0.8.1/versioneer.py
+drwxr-xr-x   0 lesteve   (1000) lesteve   (1000)        0 2023-06-15 04:23:42.939140 dask-jobqueue-0.8.2/
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)     1483 2023-06-15 04:12:38.000000 dask-jobqueue-0.8.2/LICENSE.txt
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)      260 2023-06-15 04:12:38.000000 dask-jobqueue-0.8.2/MANIFEST.in
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)     1363 2023-06-15 04:23:42.939140 dask-jobqueue-0.8.2/PKG-INFO
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)     1104 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/README.rst
+drwxr-xr-x   0 lesteve   (1000) lesteve   (1000)        0 2023-06-15 04:23:42.939140 dask-jobqueue-0.8.2/dask_jobqueue/
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)      376 2023-06-15 04:12:38.000000 dask-jobqueue-0.8.2/dask_jobqueue/__init__.py
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)      497 2023-06-15 04:23:42.939140 dask-jobqueue-0.8.2/dask_jobqueue/_version.py
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)      282 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/dask_jobqueue/config.py
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)    31513 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/dask_jobqueue/core.py
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)     8682 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/dask_jobqueue/htcondor.py
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)     9385 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/dask_jobqueue/jobqueue.yaml
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)     2918 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/dask_jobqueue/local.py
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)     8986 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/dask_jobqueue/lsf.py
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)      272 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/dask_jobqueue/moab.py
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)     8277 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/dask_jobqueue/oar.py
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)     5658 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/dask_jobqueue/pbs.py
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)     3981 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/dask_jobqueue/sge.py
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)     5962 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/dask_jobqueue/slurm.py
+drwxr-xr-x   0 lesteve   (1000) lesteve   (1000)        0 2023-06-15 04:23:42.939140 dask-jobqueue-0.8.2/dask_jobqueue/tests/
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)       27 2023-06-15 04:12:38.000000 dask-jobqueue-0.8.2/dask_jobqueue/tests/__init__.py
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)     5236 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/dask_jobqueue/tests/test_htcondor.py
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)    14632 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/dask_jobqueue/tests/test_job.py
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)    16914 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/dask_jobqueue/tests/test_jobqueue_core.py
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)    12583 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/dask_jobqueue/tests/test_lsf.py
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)     6669 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/dask_jobqueue/tests/test_oar.py
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)    13797 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/dask_jobqueue/tests/test_pbs.py
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)     3871 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/dask_jobqueue/tests/test_sge.py
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)     9848 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/dask_jobqueue/tests/test_slurm.py
+drwxr-xr-x   0 lesteve   (1000) lesteve   (1000)        0 2023-06-15 04:23:42.939140 dask-jobqueue-0.8.2/dask_jobqueue.egg-info/
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)     1363 2023-06-15 04:23:42.000000 dask-jobqueue-0.8.2/dask_jobqueue.egg-info/PKG-INFO
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)      913 2023-06-15 04:23:42.000000 dask-jobqueue-0.8.2/dask_jobqueue.egg-info/SOURCES.txt
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)        1 2023-06-15 04:23:42.000000 dask-jobqueue-0.8.2/dask_jobqueue.egg-info/dependency_links.txt
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)        1 2023-06-15 04:23:42.000000 dask-jobqueue-0.8.2/dask_jobqueue.egg-info/not-zip-safe
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)       82 2023-06-15 04:23:42.000000 dask-jobqueue-0.8.2/dask_jobqueue.egg-info/requires.txt
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)       14 2023-06-15 04:23:42.000000 dask-jobqueue-0.8.2/dask_jobqueue.egg-info/top_level.txt
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)       39 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/requirements.txt
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)      457 2023-06-15 04:23:42.939140 dask-jobqueue-0.8.2/setup.cfg
+-rwxr-xr-x   0 lesteve   (1000) lesteve   (1000)      947 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/setup.py
+-rw-r--r--   0 lesteve   (1000) lesteve   (1000)    68748 2023-06-15 04:17:51.000000 dask-jobqueue-0.8.2/versioneer.py
```

### Comparing `dask-jobqueue-0.8.1/LICENSE.txt` & `dask-jobqueue-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask-jobqueue-0.8.1/PKG-INFO` & `dask-jobqueue-0.8.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-jobqueue
-Version: 0.8.1
+Version: 0.8.2
 Summary: Deploy Dask on job queuing systems like PBS, Slurm, SGE or LSF
 Home-page: https://jobqueue.dask.org
 License: BSD 3-Clause
 Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE.txt
```

### Comparing `dask-jobqueue-0.8.1/README.rst` & `dask-jobqueue-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `dask-jobqueue-0.8.1/dask_jobqueue/core.py` & `dask-jobqueue-0.8.2/dask_jobqueue/core.py`

 * *Files identical despite different names*

### Comparing `dask-jobqueue-0.8.1/dask_jobqueue/htcondor.py` & `dask-jobqueue-0.8.2/dask_jobqueue/htcondor.py`

 * *Files identical despite different names*

### Comparing `dask-jobqueue-0.8.1/dask_jobqueue/jobqueue.yaml` & `dask-jobqueue-0.8.2/dask_jobqueue/jobqueue.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,16 @@
     env-extra: null
     job-script-prologue: []
     resource-spec: null
     job-extra: null
     job-extra-directives: []
     job-directives-skip: []
     log-directory: null
-    
+    memory-per-core-property-name: null
+
     # Scheduler options
     scheduler-options: {}
 
   pbs:
     name: dask-worker
 
     # Dask worker options
@@ -53,15 +54,15 @@
     env-extra: null
     job-script-prologue: []
     resource-spec: null
     job-extra: null
     job-extra-directives: []
     job-directives-skip: []
     log-directory: null
-    
+
     # Scheduler options
     scheduler-options: {}
 
   sge:
     name: dask-worker
 
     # Dask worker options
@@ -84,15 +85,15 @@
     env-extra: null
     job-script-prologue: []
     job-extra: null
     job-extra-directives: []
     job-directives-skip: []
     log-directory: null
     resource-spec: null
-    
+
     # Scheduler options
     scheduler-options: {}
 
   slurm:
     name: dask-worker
 
     # Dask worker options
@@ -116,15 +117,15 @@
     job-script-prologue: []
     job-cpu: null
     job-mem: null
     job-extra: null
     job-extra-directives: []
     job-directives-skip: []
     log-directory: null
-    
+
     # Scheduler options
     scheduler-options: {}
 
   moab:
     name: dask-worker
 
     # Dask worker options
@@ -147,15 +148,15 @@
     env-extra: null
     job-script-prologue: []
     resource-spec: null
     job-extra: null
     job-extra-directives: []
     job-directives-skip: []
     log-directory: null
-    
+
     # Scheduler options
     scheduler-options: {}
 
   lsf:
     name: dask-worker
 
     # Dask worker options
@@ -181,15 +182,15 @@
     mem: null
     job-extra: null
     job-extra-directives: []
     job-directives-skip: []
     log-directory: null
     lsf-units: null
     use-stdin: True             # (bool) How jobs are launched, i.e. 'bsub jobscript.sh' or 'bsub < jobscript.sh'
-    
+
     # Scheduler options
     scheduler-options: {}
 
   htcondor:
     name: dask-worker
 
     # Dask worker options
@@ -211,15 +212,15 @@
     job-extra: null             # Extra submit attributes
     job-extra-directives: {}    # Extra submit attributes
     job-directives-skip: []
     submit-command-extra: []    # Extra condor_submit arguments
     cancel-command-extra: []    # Extra condor_rm arguments
     log-directory: null
     shebang: "#!/usr/bin/env condor_submit"
-    
+
     # Scheduler options
     scheduler-options: {}
 
   local:
     name: dask-worker
     # Dask worker options
     cores: null                 # Total number of cores per job
@@ -235,10 +236,10 @@
 
     env-extra: null
     job-script-prologue: []
     job-extra: null
     job-extra-directives: []
     job-directives-skip: []
     log-directory: null
-    
+
     # Scheduler options
     scheduler-options: {}
```

### Comparing `dask-jobqueue-0.8.1/dask_jobqueue/local.py` & `dask-jobqueue-0.8.2/dask_jobqueue/local.py`

 * *Files identical despite different names*

### Comparing `dask-jobqueue-0.8.1/dask_jobqueue/lsf.py` & `dask-jobqueue-0.8.2/dask_jobqueue/lsf.py`

 * *Files identical despite different names*

### Comparing `dask-jobqueue-0.8.1/dask_jobqueue/oar.py` & `dask-jobqueue-0.8.2/dask_jobqueue/pbs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,142 +1,166 @@
 import logging
-import shlex
+import math
+import os
+import warnings
 
 import dask
 
-from .core import JobQueueCluster, Job, job_parameters, cluster_parameters
+from .core import Job, JobQueueCluster, job_parameters, cluster_parameters
 
 logger = logging.getLogger(__name__)
 
 
-class OARJob(Job):
+def pbs_format_bytes_ceil(n):
+    """Format bytes as text.
 
-    # Override class variables
-    submit_command = "oarsub"
-    cancel_command = "oardel"
-    job_id_regexp = r"OAR_JOB_ID=(?P<job_id>\d+)"
-    config_name = "oar"
+    PBS expects KiB, MiB or Gib, but names it KB, MB, GB whereas Dask makes the difference between KB and KiB.
+
+    >>> pbs_format_bytes_ceil(1)
+    '1B'
+    >>> pbs_format_bytes_ceil(1234)
+    '1234B'
+    >>> pbs_format_bytes_ceil(12345678)
+    '13MB'
+    >>> pbs_format_bytes_ceil(1234567890)
+    '1177MB'
+    >>> pbs_format_bytes_ceil(15000000000)
+    '14GB'
+    """
+    if n >= 10 * (1024**3):
+        return "%dGB" % math.ceil(n / (1024**3))
+    if n >= 10 * (1024**2):
+        return "%dMB" % math.ceil(n / (1024**2))
+    if n >= 10 * 1024:
+        return "%dkB" % math.ceil(n / 1024)
+    return "%dB" % n
+
+
+class PBSJob(Job):
+    submit_command = "qsub"
+    cancel_command = "qdel"
+    config_name = "pbs"
 
     def __init__(
         self,
         scheduler=None,
         name=None,
         queue=None,
         project=None,
+        account=None,
         resource_spec=None,
         walltime=None,
         config_name=None,
         **base_class_kwargs
     ):
         super().__init__(
             scheduler=scheduler, name=name, config_name=config_name, **base_class_kwargs
         )
 
         if queue is None:
             queue = dask.config.get("jobqueue.%s.queue" % self.config_name)
-        if project is None:
-            project = dask.config.get("jobqueue.%s.project" % self.config_name)
         if resource_spec is None:
             resource_spec = dask.config.get(
                 "jobqueue.%s.resource-spec" % self.config_name
             )
         if walltime is None:
             walltime = dask.config.get("jobqueue.%s.walltime" % self.config_name)
 
+        if account is None:
+            account = dask.config.get(
+                "jobqueue.%s.account" % self.config_name
+            ) or os.environ.get("PBS_ACCOUNT")
+        if project is None:
+            project = dask.config.get("jobqueue.%s.project" % self.config_name, None)
+        if project is not None:
+            warn = (
+                "project has been renamed to account as this kwarg was used wit -A option. "
+                "You are still using it (please also check config files). "
+                "If you did not set account yet, project will be respected for now, "
+                "but it will be removed in a future release. "
+                "If you already set account, project is ignored and you can remove it."
+            )
+            warnings.warn(warn, FutureWarning)
+            if not account:
+                account = project
+
         header_lines = []
+        # PBS header build
         if self.job_name is not None:
-            header_lines.append("#OAR -n %s" % self.job_name)
+            header_lines.append("#PBS -N %s" % self.job_name)
         if queue is not None:
-            header_lines.append("#OAR -q %s" % queue)
-        if project is not None:
-            header_lines.append("#OAR --project %s" % project)
-
-        # OAR needs to have the resource on a single line otherwise it is
-        # considered as a "moldable job" (i.e. the scheduler can chose between
-        # multiple sets of resources constraints)
-        resource_spec_list = []
+            header_lines.append("#PBS -q %s" % queue)
+        if account is not None:
+            header_lines.append("#PBS -A %s" % account)
         if resource_spec is None:
-            # default resource_spec if not specified. Crucial to specify
-            # nodes=1 to make sure the cores allocated are on the same node.
-            resource_spec = "/nodes=1/core=%d" % self.worker_cores
-        resource_spec_list.append(resource_spec)
+            # Compute default resources specifications
+            resource_spec = "select=1:ncpus=%d" % self.worker_cores
+            memory_string = pbs_format_bytes_ceil(self.worker_memory)
+            resource_spec += ":mem=" + memory_string
+            logger.info(
+                "Resource specification for PBS not set, initializing it to %s"
+                % resource_spec
+            )
+        if resource_spec is not None:
+            header_lines.append("#PBS -l %s" % resource_spec)
         if walltime is not None:
-            resource_spec_list.append("walltime=%s" % walltime)
-
-        full_resource_spec = ",".join(resource_spec_list)
-        header_lines.append("#OAR -l %s" % full_resource_spec)
+            header_lines.append("#PBS -l walltime=%s" % walltime)
+        if self.log_directory is not None:
+            header_lines.append("#PBS -e %s/" % self.log_directory)
+            header_lines.append("#PBS -o %s/" % self.log_directory)
 
         # Skip requested header directives
         header_lines = list(
             filter(
                 lambda line: not any(skip in line for skip in self.job_directives_skip),
                 header_lines,
             )
         )
 
         # Add extra header directives
-        header_lines.extend(["#OAR %s" % arg for arg in self.job_extra_directives])
+        header_lines.extend(["#PBS %s" % arg for arg in self.job_extra_directives])
 
+        # Declare class attribute that shall be overridden
         self.job_header = "\n".join(header_lines)
 
         logger.debug("Job script: \n %s" % self.job_script())
 
-    async def _submit_job(self, fn):
-        # OAR specificity: the submission script needs to exist on the worker
-        # when the job starts on the worker. This is different from other
-        # schedulers that only need the script on the submission node at
-        # submission time. That means that we can not use the same strategy as
-        # in JobQueueCluster: create a temporary submission file, submit the
-        # script, delete the submission file. In order to reuse the code in
-        # the base JobQueueCluster class, we read from the temporary file and
-        # reconstruct the command line where the script is passed in as a
-        # string (inline script in OAR jargon) rather than as a filename.
-        with open(fn) as f:
-            content_lines = f.readlines()
-
-        oar_lines = [line for line in content_lines if line.startswith("#OAR ")]
-        oarsub_options = [line.replace("#OAR ", "").strip() for line in oar_lines]
-        inline_script_lines = [
-            line for line in content_lines if not line.startswith("#")
-        ]
-        inline_script = "".join(inline_script_lines)
-        oarsub_command = " ".join([self.submit_command] + oarsub_options)
-        oarsub_command_split = shlex.split(oarsub_command) + [inline_script]
-        return self._call(oarsub_command_split)
-
 
-class OARCluster(JobQueueCluster):
-    __doc__ = """ Launch Dask on an OAR cluster
+class PBSCluster(JobQueueCluster):
+    __doc__ = """ Launch Dask on a PBS cluster
 
     Parameters
     ----------
     queue : str
-        Destination queue for each worker job. Passed to `#OAR -q` option.
+        Destination queue for each worker job. Passed to `#PBS -q` option.
     project : str
-        Project associated with each worker job. Passed to `#OAR --project` option.
+        Deprecated: use ``account`` instead. This parameter will be removed in a future version.
+    account : str
+        Accounting string associated with each worker job. Passed to `#PBS -A` option.
     {job}
     {cluster}
     resource_spec : str
-        Request resources and specify job placement. Passed to `#OAR -l` option.
+        Request resources and specify job placement. Passed to `#PBS -l` option.
     walltime : str
         Walltime for each worker job.
     job_extra : list
         Deprecated: use ``job_extra_directives`` instead. This parameter will be removed in a future version.
     job_extra_directives : list
-        List of other OAR options, for example `-t besteffort`. Each option will be prepended with the #OAR prefix.
+        List of other PBS options. Each option will be prepended with the #PBS prefix.
 
     Examples
     --------
-    >>> from dask_jobqueue import OARCluster
-    >>> cluster = OARCluster(queue='regular')
+    >>> from dask_jobqueue import PBSCluster
+    >>> cluster = PBSCluster(queue='regular', account="myaccountingstring", cores=24,
+    ...     memory="500 GB")
     >>> cluster.scale(jobs=10)  # ask for 10 jobs
 
     >>> from dask.distributed import Client
     >>> client = Client(cluster)
 
     This also works with adaptive clusters.  This automatically launches and kill workers based on load.
 
     >>> cluster.adapt(maximum_jobs=20)
     """.format(
         job=job_parameters, cluster=cluster_parameters
     )
-    job_cls = OARJob
+    job_cls = PBSJob
```

### Comparing `dask-jobqueue-0.8.1/dask_jobqueue/pbs.py` & `dask-jobqueue-0.8.2/dask_jobqueue/slurm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,166 +1,179 @@
 import logging
 import math
-import os
 import warnings
 
 import dask
 
 from .core import Job, JobQueueCluster, job_parameters, cluster_parameters
 
 logger = logging.getLogger(__name__)
 
 
-def pbs_format_bytes_ceil(n):
-    """Format bytes as text.
-
-    PBS expects KiB, MiB or Gib, but names it KB, MB, GB whereas Dask makes the difference between KB and KiB.
-
-    >>> pbs_format_bytes_ceil(1)
-    '1B'
-    >>> pbs_format_bytes_ceil(1234)
-    '1234B'
-    >>> pbs_format_bytes_ceil(12345678)
-    '13MB'
-    >>> pbs_format_bytes_ceil(1234567890)
-    '1177MB'
-    >>> pbs_format_bytes_ceil(15000000000)
-    '14GB'
-    """
-    if n >= 10 * (1024**3):
-        return "%dGB" % math.ceil(n / (1024**3))
-    if n >= 10 * (1024**2):
-        return "%dMB" % math.ceil(n / (1024**2))
-    if n >= 10 * 1024:
-        return "%dkB" % math.ceil(n / 1024)
-    return "%dB" % n
-
-
-class PBSJob(Job):
-    submit_command = "qsub"
-    cancel_command = "qdel"
-    config_name = "pbs"
+class SLURMJob(Job):
+    # Override class variables
+    submit_command = "sbatch"
+    cancel_command = "scancel"
+    config_name = "slurm"
 
     def __init__(
         self,
         scheduler=None,
         name=None,
         queue=None,
         project=None,
         account=None,
-        resource_spec=None,
         walltime=None,
+        job_cpu=None,
+        job_mem=None,
         config_name=None,
         **base_class_kwargs
     ):
         super().__init__(
             scheduler=scheduler, name=name, config_name=config_name, **base_class_kwargs
         )
 
         if queue is None:
             queue = dask.config.get("jobqueue.%s.queue" % self.config_name)
-        if resource_spec is None:
-            resource_spec = dask.config.get(
-                "jobqueue.%s.resource-spec" % self.config_name
-            )
-        if walltime is None:
-            walltime = dask.config.get("jobqueue.%s.walltime" % self.config_name)
-
         if account is None:
-            account = dask.config.get(
-                "jobqueue.%s.account" % self.config_name
-            ) or os.environ.get("PBS_ACCOUNT")
+            account = dask.config.get("jobqueue.%s.account" % self.config_name)
         if project is None:
             project = dask.config.get("jobqueue.%s.project" % self.config_name, None)
         if project is not None:
             warn = (
                 "project has been renamed to account as this kwarg was used wit -A option. "
                 "You are still using it (please also check config files). "
                 "If you did not set account yet, project will be respected for now, "
                 "but it will be removed in a future release. "
                 "If you already set account, project is ignored and you can remove it."
             )
             warnings.warn(warn, FutureWarning)
             if not account:
                 account = project
 
+        if walltime is None:
+            walltime = dask.config.get("jobqueue.%s.walltime" % self.config_name)
+        if job_cpu is None:
+            job_cpu = dask.config.get("jobqueue.%s.job-cpu" % self.config_name)
+        if job_mem is None:
+            job_mem = dask.config.get("jobqueue.%s.job-mem" % self.config_name)
+
         header_lines = []
-        # PBS header build
+        # SLURM header build
         if self.job_name is not None:
-            header_lines.append("#PBS -N %s" % self.job_name)
+            header_lines.append("#SBATCH -J %s" % self.job_name)
+        if self.log_directory is not None:
+            header_lines.append(
+                "#SBATCH -e %s/%s-%%J.err"
+                % (self.log_directory, self.job_name or "worker")
+            )
+            header_lines.append(
+                "#SBATCH -o %s/%s-%%J.out"
+                % (self.log_directory, self.job_name or "worker")
+            )
         if queue is not None:
-            header_lines.append("#PBS -q %s" % queue)
+            header_lines.append("#SBATCH -p %s" % queue)
         if account is not None:
-            header_lines.append("#PBS -A %s" % account)
-        if resource_spec is None:
-            # Compute default resources specifications
-            resource_spec = "select=1:ncpus=%d" % self.worker_cores
-            memory_string = pbs_format_bytes_ceil(self.worker_memory)
-            resource_spec += ":mem=" + memory_string
-            logger.info(
-                "Resource specification for PBS not set, initializing it to %s"
-                % resource_spec
-            )
-        if resource_spec is not None:
-            header_lines.append("#PBS -l %s" % resource_spec)
+            header_lines.append("#SBATCH -A %s" % account)
+
+        # Init resources, always 1 task,
+        # and then number of cpu is processes * threads if not set
+        header_lines.append("#SBATCH -n 1")
+        header_lines.append(
+            "#SBATCH --cpus-per-task=%d" % (job_cpu or self.worker_cores)
+        )
+        # Memory
+        memory = job_mem
+        if job_mem is None:
+            memory = slurm_format_bytes_ceil(self.worker_memory)
+        if memory is not None:
+            header_lines.append("#SBATCH --mem=%s" % memory)
+
         if walltime is not None:
-            header_lines.append("#PBS -l walltime=%s" % walltime)
-        if self.log_directory is not None:
-            header_lines.append("#PBS -e %s/" % self.log_directory)
-            header_lines.append("#PBS -o %s/" % self.log_directory)
+            header_lines.append("#SBATCH -t %s" % walltime)
 
         # Skip requested header directives
         header_lines = list(
             filter(
                 lambda line: not any(skip in line for skip in self.job_directives_skip),
                 header_lines,
             )
         )
 
         # Add extra header directives
-        header_lines.extend(["#PBS %s" % arg for arg in self.job_extra_directives])
+        header_lines.extend(["#SBATCH %s" % arg for arg in self.job_extra_directives])
 
         # Declare class attribute that shall be overridden
         self.job_header = "\n".join(header_lines)
 
-        logger.debug("Job script: \n %s" % self.job_script())
+
+def slurm_format_bytes_ceil(n):
+    """Format bytes as text.
+
+    SLURM expects KiB, MiB or Gib, but names it KB, MB, GB. SLURM does not handle Bytes, only starts at KB.
+
+    >>> slurm_format_bytes_ceil(1)
+    '1K'
+    >>> slurm_format_bytes_ceil(1234)
+    '2K'
+    >>> slurm_format_bytes_ceil(12345678)
+    '13M'
+    >>> slurm_format_bytes_ceil(1234567890)
+    '2G'
+    >>> slurm_format_bytes_ceil(15000000000)
+    '14G'
+    """
+    if n >= (1024**3):
+        return "%dG" % math.ceil(n / (1024**3))
+    if n >= (1024**2):
+        return "%dM" % math.ceil(n / (1024**2))
+    if n >= 1024:
+        return "%dK" % math.ceil(n / 1024)
+    return "1K" % n
 
 
-class PBSCluster(JobQueueCluster):
-    __doc__ = """ Launch Dask on a PBS cluster
+class SLURMCluster(JobQueueCluster):
+    __doc__ = """ Launch Dask on a SLURM cluster
 
     Parameters
     ----------
     queue : str
-        Destination queue for each worker job. Passed to `#PBS -q` option.
+        Destination queue for each worker job. Passed to `#SBATCH -p` option.
     project : str
         Deprecated: use ``account`` instead. This parameter will be removed in a future version.
     account : str
         Accounting string associated with each worker job. Passed to `#PBS -A` option.
     {job}
     {cluster}
-    resource_spec : str
-        Request resources and specify job placement. Passed to `#PBS -l` option.
     walltime : str
         Walltime for each worker job.
+    job_cpu : int
+        Number of cpu to book in SLURM, if None, defaults to worker `threads * processes`
+    job_mem : str
+        Amount of memory to request in SLURM. If None, defaults to worker
+        processes * memory
     job_extra : list
         Deprecated: use ``job_extra_directives`` instead. This parameter will be removed in a future version.
     job_extra_directives : list
-        List of other PBS options. Each option will be prepended with the #PBS prefix.
+        List of other Slurm options, for example -j oe. Each option will be prepended with the #SBATCH prefix.
 
     Examples
     --------
-    >>> from dask_jobqueue import PBSCluster
-    >>> cluster = PBSCluster(queue='regular', account="myaccountingstring", cores=24,
-    ...     memory="500 GB")
+    >>> from dask_jobqueue import SLURMCluster
+    >>> cluster = SLURMCluster(
+    ...     queue='regular',
+    ...     account="myaccount",
+    ...     cores=24,
+    ...     memory="500 GB"
+    ... )
     >>> cluster.scale(jobs=10)  # ask for 10 jobs
 
     >>> from dask.distributed import Client
     >>> client = Client(cluster)
 
     This also works with adaptive clusters.  This automatically launches and kill workers based on load.
 
     >>> cluster.adapt(maximum_jobs=20)
     """.format(
         job=job_parameters, cluster=cluster_parameters
     )
-    job_cls = PBSJob
+    job_cls = SLURMJob
```

### Comparing `dask-jobqueue-0.8.1/dask_jobqueue/sge.py` & `dask-jobqueue-0.8.2/dask_jobqueue/sge.py`

 * *Files identical despite different names*

### Comparing `dask-jobqueue-0.8.1/dask_jobqueue/tests/test_htcondor.py` & `dask-jobqueue-0.8.2/dask_jobqueue/tests/test_htcondor.py`

 * *Files identical despite different names*

### Comparing `dask-jobqueue-0.8.1/dask_jobqueue/tests/test_job.py` & `dask-jobqueue-0.8.2/dask_jobqueue/tests/test_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,16 +138,16 @@
 # Test only header_skip for the cluster implementation that uses job_name.
 
 
 @pytest.mark.parametrize("Cluster", [PBSCluster, SLURMCluster, SGECluster, OARCluster])
 def test_deprecation_header_skip(Cluster):
     import warnings
 
-    # test issuing of warning
-    warnings.simplefilter("always")
+    # test issuing of warning but ignore UserWarning
+    warnings.simplefilter("ignore", UserWarning)
 
     job_cls = Cluster.job_cls
     with warnings.catch_warnings(record=True) as w:
         # should give a warning
         job = job_cls(cores=1, memory="1 GB", header_skip=["old_param"])
         assert len(w) == 1
         assert issubclass(w[0].category, FutureWarning)
@@ -236,16 +236,16 @@
     assert "cores :" in Cluster.__doc__
     assert Cluster.__name__[: -len("Cluster")] in Cluster.__doc__
 
 
 def test_deprecation_env_extra(Cluster):
     import warnings
 
-    # test issuing of warning
-    warnings.simplefilter("always")
+    # test issuing of warning but ignore UserWarning
+    warnings.simplefilter("ignore", UserWarning)
 
     job_cls = Cluster.job_cls
     with warnings.catch_warnings(record=True) as w:
         # should give a warning
         job = job_cls(cores=1, memory="1 GB", env_extra=["env_extra is used"])
         assert len(w) == 1
         assert issubclass(w[0].category, FutureWarning)
@@ -300,16 +300,16 @@
     job_script = job.job_script()
     assert "env_extra" in job_script
 
 
 def test_deprecation_extra(Cluster):
     import warnings
 
-    # test issuing of warning
-    warnings.simplefilter("always")
+    # test issuing of warning but ignore UserWarning
+    warnings.simplefilter("ignore", UserWarning)
 
     job_cls = Cluster.job_cls
     with warnings.catch_warnings(record=True) as w:
         # should give a warning
         job = job_cls(cores=1, memory="1 GB", extra=["old_param"])
         assert len(w) == 1
         assert issubclass(w[0].category, FutureWarning)
@@ -367,16 +367,16 @@
 
 def test_deprecation_job_extra(Cluster):
     if issubclass(Cluster, LocalCluster):
         return  # nothing to test in this implentation, really
 
     import warnings
 
-    # test issuing of warning
-    warnings.simplefilter("always")
+    # test issuing of warning but ignore UserWarning
+    warnings.simplefilter("ignore", UserWarning)
 
     job_cls = Cluster.job_cls
     with warnings.catch_warnings(record=True) as w:
         # should give a warning
         job = job_cls(cores=1, memory="1 GB", job_extra={"old_param": "1"})
         assert len(w) == 1
         assert issubclass(w[0].category, FutureWarning)
```

### Comparing `dask-jobqueue-0.8.1/dask_jobqueue/tests/test_jobqueue_core.py` & `dask-jobqueue-0.8.2/dask_jobqueue/tests/test_jobqueue_core.py`

 * *Files identical despite different names*

### Comparing `dask-jobqueue-0.8.1/dask_jobqueue/tests/test_lsf.py` & `dask-jobqueue-0.8.2/dask_jobqueue/tests/test_lsf.py`

 * *Files identical despite different names*

### Comparing `dask-jobqueue-0.8.1/dask_jobqueue/tests/test_pbs.py` & `dask-jobqueue-0.8.2/dask_jobqueue/tests/test_pbs.py`

 * *Files identical despite different names*

### Comparing `dask-jobqueue-0.8.1/dask_jobqueue/tests/test_sge.py` & `dask-jobqueue-0.8.2/dask_jobqueue/tests/test_sge.py`

 * *Files identical despite different names*

### Comparing `dask-jobqueue-0.8.1/dask_jobqueue/tests/test_slurm.py` & `dask-jobqueue-0.8.2/dask_jobqueue/tests/test_slurm.py`

 * *Files identical despite different names*

### Comparing `dask-jobqueue-0.8.1/dask_jobqueue.egg-info/PKG-INFO` & `dask-jobqueue-0.8.2/dask_jobqueue.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-jobqueue
-Version: 0.8.1
+Version: 0.8.2
 Summary: Deploy Dask on job queuing systems like PBS, Slurm, SGE or LSF
 Home-page: https://jobqueue.dask.org
 License: BSD 3-Clause
 Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE.txt
```

### Comparing `dask-jobqueue-0.8.1/dask_jobqueue.egg-info/SOURCES.txt` & `dask-jobqueue-0.8.2/dask_jobqueue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-jobqueue-0.8.1/setup.py` & `dask-jobqueue-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `dask-jobqueue-0.8.1/versioneer.py` & `dask-jobqueue-0.8.2/versioneer.py`

 * *Files identical despite different names*

