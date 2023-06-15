# Comparing `tmp/strangeworks_optimization-0.1.0.tar.gz` & `tmp/strangeworks_optimization-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_optimization-0.1.0.tar", max compression
+gzip compressed data, was "strangeworks_optimization-0.1.1.tar", max compression
```

## Comparing `strangeworks_optimization-0.1.0.tar` & `strangeworks_optimization-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       28 2023-06-13 12:32:36.132765 strangeworks_optimization-0.1.0/README.md
--rw-r--r--   0        0        0      918 2023-06-13 12:32:52.949278 strangeworks_optimization-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      174 2023-06-13 12:32:36.132765 strangeworks_optimization-0.1.0/strangeworks_optimization/__init__.py
--rw-r--r--   0        0        0     1769 2023-06-13 12:32:36.132765 strangeworks_optimization-0.1.0/strangeworks_optimization/optimization.py
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 strangeworks_optimization-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       28 2023-06-15 13:10:29.971670 strangeworks_optimization-0.1.1/README.md
+-rw-r--r--   0        0        0      919 2023-06-15 13:10:45.083640 strangeworks_optimization-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-06-15 13:10:29.971670 strangeworks_optimization-0.1.1/strangeworks_optimization/__init__.py
+-rw-r--r--   0        0        0     1968 2023-06-15 13:10:29.971670 strangeworks_optimization-0.1.1/strangeworks_optimization/optimization.py
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 strangeworks_optimization-0.1.1/PKG-INFO
```

### Comparing `strangeworks_optimization-0.1.0/pyproject.toml` & `strangeworks_optimization-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "strangeworks-optimization"
-version = "0.1.0"
+version = "0.1.1"
 description = "This SDK extends the Strangeworks SDK to provide access to the Strangeworks Optimization API."
 authors = ["James Tricker <james@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_optimization"}]
 
+
 [tool.poetry.dependencies]
 python = "^3.10"
 strangeworks = "^0.4.2"
 dimod = "^0.12.7"
 pytest = "^7.3.1"
 strangeworks-python-core = "^0.1.7"
 python-dotenv = "^1.0.0"
```

### Comparing `strangeworks_optimization-0.1.0/strangeworks_optimization/optimization.py` & `strangeworks_optimization-0.1.1/strangeworks_optimization/optimization.py`

 * *Files 21% similar despite different names*

```diff
@@ -36,27 +36,35 @@
             for rr in range(len(rsc_list)):
                 if rsc_list[rr].product.slug == "optimization":
                     self.rsc = rsc_list[rr]
 
         # self.backend_list = " "
 
     def run(self, qubo_job: OptimizationJob) -> str:
-        job = sw.execute(self.rsc, payload=qubo_job.__dict__, endpoint=path)
-        slug = job["job_slug"]
-        # Get Strangeworks Job from slug
-        return slug
+        return sw.execute(self.rsc, payload=qubo_job.__dict__, endpoint=path)
 
-    def get_results(self, slug: str):
-        result = sw.download_job_files(slug)[1]
+    def get_results(self, sw_job):
+        if type(sw_job) is dict:
+            job_slug = sw_job["job_slug"]
+        else:
+            job_slug = sw_job.slug
+
+        result = sw.download_job_files(job_slug)[1]
         return SampleSet.from_serializable(result)
 
     def upload_model(self, bqm: BinaryQuadraticModel) -> str:
         with tempfile.NamedTemporaryFile(mode="w+") as t:
             json.dump(bqm.to_serializable(), t)
             t.flush()
 
             return sw.upload_file(t.name)
 
-    # def get_status(self, slug: str):
-    # todo: implement this
+    def get_status(self, sw_job, job_slug: str = None):
+        if type(sw_job) is dict:
+            job_slug = sw_job.get("slug")
+        else:
+            job_slug = sw_job.slug
+
+        return sw.jobs(slug=job_slug)[0].status
+
     # def get_backends(self):
     # todo: implement this
```

### Comparing `strangeworks_optimization-0.1.0/PKG-INFO` & `strangeworks_optimization-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-optimization
-Version: 0.1.0
+Version: 0.1.1
 Summary: This SDK extends the Strangeworks SDK to provide access to the Strangeworks Optimization API.
 Author: James Tricker
 Author-email: james@strangeworks.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

