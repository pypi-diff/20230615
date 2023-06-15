# Comparing `tmp/m_scheduler_partitioning-0.1.8.tar.gz` & `tmp/m_scheduler_partitioning-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m_scheduler_partitioning-0.1.8.tar", last modified: Mon May  8 04:59:24 2023, max compression
+gzip compressed data, was "m_scheduler_partitioning-0.1.9.tar", last modified: Thu Jun 15 08:01:51 2023, max compression
```

## Comparing `m_scheduler_partitioning-0.1.8.tar` & `m_scheduler_partitioning-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:59:24.074867 m_scheduler_partitioning-0.1.8/
--rw-r--r--   0 root         (0) root         (0)     3441 2023-05-08 04:59:24.073867 m_scheduler_partitioning-0.1.8/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     2122 2023-05-08 04:43:40.000000 m_scheduler_partitioning-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:59:24.066867 m_scheduler_partitioning-0.1.8/m_scheduler_partitioning.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3441 2023-05-08 04:59:23.000000 m_scheduler_partitioning-0.1.8/m_scheduler_partitioning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      728 2023-05-08 04:59:23.000000 m_scheduler_partitioning-0.1.8/m_scheduler_partitioning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 04:59:23.000000 m_scheduler_partitioning-0.1.8/m_scheduler_partitioning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-08 04:59:23.000000 m_scheduler_partitioning-0.1.8/m_scheduler_partitioning.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-08 04:59:23.000000 m_scheduler_partitioning-0.1.8/m_scheduler_partitioning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-08 04:59:23.000000 m_scheduler_partitioning-0.1.8/m_scheduler_partitioning.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:59:24.059867 m_scheduler_partitioning-0.1.8/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:59:24.067867 m_scheduler_partitioning-0.1.8/mobio/libs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:43:40.000000 m_scheduler_partitioning-0.1.8/mobio/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:59:24.069867 m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/
--rw-r--r--   0 root         (0) root         (0)      142 2023-05-08 04:43:40.000000 m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10956 2023-05-08 04:43:40.000000 m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/m_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:59:24.072867 m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/scheduler_models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:43:40.000000 m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/scheduler_models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-05-08 04:43:40.000000 m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/scheduler_models/base_model.py
--rw-r--r--   0 root         (0) root         (0)      887 2023-05-08 04:43:40.000000 m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/scheduler_models/db_manager.py
--rw-r--r--   0 root         (0) root         (0)     3081 2023-05-08 04:43:40.000000 m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/scheduler_models/scheduler_state_model.py
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-08 04:43:40.000000 m_scheduler_partitioning-0.1.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 04:59:24.074867 m_scheduler_partitioning-0.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9269 2023-05-08 04:59:23.000000 m_scheduler_partitioning-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:01:51.766714 m_scheduler_partitioning-0.1.9/
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-06-15 08:01:51.765715 m_scheduler_partitioning-0.1.9/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     2252 2023-06-15 07:53:51.000000 m_scheduler_partitioning-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:01:51.466706 m_scheduler_partitioning-0.1.9/m_scheduler_partitioning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-06-15 08:01:51.000000 m_scheduler_partitioning-0.1.9/m_scheduler_partitioning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      728 2023-06-15 08:01:51.000000 m_scheduler_partitioning-0.1.9/m_scheduler_partitioning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 08:01:51.000000 m_scheduler_partitioning-0.1.9/m_scheduler_partitioning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-15 08:01:51.000000 m_scheduler_partitioning-0.1.9/m_scheduler_partitioning.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-15 08:01:51.000000 m_scheduler_partitioning-0.1.9/m_scheduler_partitioning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-15 08:01:51.000000 m_scheduler_partitioning-0.1.9/m_scheduler_partitioning.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:01:51.457706 m_scheduler_partitioning-0.1.9/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:01:51.467707 m_scheduler_partitioning-0.1.9/mobio/libs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 07:53:51.000000 m_scheduler_partitioning-0.1.9/mobio/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:01:51.485707 m_scheduler_partitioning-0.1.9/mobio/libs/m_scheduler_partitioning/
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-15 07:53:51.000000 m_scheduler_partitioning-0.1.9/mobio/libs/m_scheduler_partitioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12224 2023-06-15 07:53:51.000000 m_scheduler_partitioning-0.1.9/mobio/libs/m_scheduler_partitioning/m_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:01:51.736714 m_scheduler_partitioning-0.1.9/mobio/libs/m_scheduler_partitioning/scheduler_models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 07:53:51.000000 m_scheduler_partitioning-0.1.9/mobio/libs/m_scheduler_partitioning/scheduler_models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-06-15 07:53:51.000000 m_scheduler_partitioning-0.1.9/mobio/libs/m_scheduler_partitioning/scheduler_models/base_model.py
+-rw-r--r--   0 root         (0) root         (0)      887 2023-06-15 07:53:51.000000 m_scheduler_partitioning-0.1.9/mobio/libs/m_scheduler_partitioning/scheduler_models/db_manager.py
+-rw-r--r--   0 root         (0) root         (0)     3851 2023-06-15 07:53:51.000000 m_scheduler_partitioning-0.1.9/mobio/libs/m_scheduler_partitioning/scheduler_models/scheduler_state_model.py
+-rw-r--r--   0 root         (0) root         (0)      103 2023-06-15 07:53:51.000000 m_scheduler_partitioning-0.1.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 08:01:51.767714 m_scheduler_partitioning-0.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9269 2023-06-15 08:01:48.000000 m_scheduler_partitioning-0.1.9/setup.py
```

### Comparing `m_scheduler_partitioning-0.1.8/PKG-INFO` & `m_scheduler_partitioning-0.1.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 Metadata-Version: 2.1
 Name: m_scheduler_partitioning
-Version: 0.1.8
+Version: 0.1.9
 Summary: Mobio scheduler partitioning libs
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
-Description: Thư viện scheduler multiple partitions của Profiling
-        
-        <b>nop</b>: maximum partitions now support is 1000 
-        <br>
-        <b>delays</b>: maximum time delays now support is 3600 seconds (1 hour)
-        
-        sample code:
-        
-        ```python
-        from mobio.libs.m_scheduler_partitioning.m_scheduler import MobioScheduler
-        from mobio.libs.m_scheduler_partitioning.scheduler_models.scheduler_state_model import SchedulerStateModel
-        
-        
-        class SampleScheduler(MobioScheduler):
-            def process(self):
-                if self.url_connection:
-                    SchedulerStateModel(self.url_connection).set_busy(
-                        worker_id=self.node_id
-                    )
-                print("Hi there ! :)")
-        
-        
-        if __name__ == "__main__":
-            SampleScheduler(root_node="test-scheduler", nop=100, delays=1, url_connection="mongodb://test_user:test_password@0.0.0.0:27017/test_db", zookeeper_uri="127.0.0.1:2181")
-        
-        ```
-        # Change logs
-        * 0.1.2
-          * log state of worker
-          * get free worker
-          * Để không bị mất 50k cho anh Lợi, thêm 2 index này:
-        
-                    * db.scheduler_state.createIndex({"expiry_time": 1}, {expireAfterSeconds: 5, name: "expiry_time_1"})
-                    * db.scheduler_state.createIndex({"root_node": 1, "state":1}, {name: "root_node_1_state_1"})
-            
-        * 0.1.3
-          * fix issue khi worker rebalance không tự động cập nhật danh sách partitions.
-            
-        * 0.1.4
-          * fix issue register worker
-          * cơ chế đảm bảo việc register worker với hệ thống csdl
-        * 0.1.5
-          * Refix issue register worker
-          * Thử nghiệm cơ chế đảm bảo 1 partition chỉ nằm trên 1 worker. 
-          * *NOTE*: phần này chưa đảm bảo được việc đủ partitions trên các workers
-        
-        * 0.1.6
-          * missing version do nâng cấp CICD
-        
-        * 0.1.7
-          * Sử dụng threading để quản lý heart_beat và expiry_time
-          * Kiểm tra trạng thái subscribe của worker mỗi khi chuẩn bị process data (Đảm bảo rằng việc subscribe phải diễn ra thành công tránh 2 worker cùng xử lý 1 partition)
-        
-        * 0.1.8
-          * Cho phép truyền zookeeper_uri vào param khi khởi tạo Schedule, nếu không truyền thì lấy mặc định từ ENV: ZOOKEEPER_CLUSTER
 Keywords: mobio,scheduler,partitioning
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+
+Thư viện scheduler multiple partitions của Profiling
+
+<b>nop</b>: maximum partitions now support is 1000 
+<br>
+<b>delays</b>: maximum time delays now support is 3600 seconds (1 hour)
+
+sample code:
+
+```python
+from mobio.libs.m_scheduler_partitioning.m_scheduler import MobioScheduler
+from mobio.libs.m_scheduler_partitioning.scheduler_models.scheduler_state_model import SchedulerStateModel
+
+
+class SampleScheduler(MobioScheduler):
+    def process(self):
+        if self.url_connection:
+            SchedulerStateModel(self.url_connection).set_busy(
+                worker_id=self.node_id
+            )
+        print("Hi there ! :)")
+
+
+if __name__ == "__main__":
+    SampleScheduler(root_node="test-scheduler", nop=100, delays=1, url_connection="mongodb://test_user:test_password@0.0.0.0:27017/test_db", zookeeper_uri="127.0.0.1:2181")
+
+```
+# Change logs
+* 0.1.2
+  * log state of worker
+  * get free worker
+  * Để không bị mất 50k cho anh Lợi, thêm 2 index này:
+
+            * db.scheduler_state.createIndex({"expiry_time": 1}, {expireAfterSeconds: 5, name: "expiry_time_1"})
+            * db.scheduler_state.createIndex({"root_node": 1, "state":1}, {name: "root_node_1_state_1"})
+    
+* 0.1.3
+  * fix issue khi worker rebalance không tự động cập nhật danh sách partitions.
+    
+* 0.1.4
+  * fix issue register worker
+  * cơ chế đảm bảo việc register worker với hệ thống csdl
+* 0.1.5
+  * Refix issue register worker
+  * Thử nghiệm cơ chế đảm bảo 1 partition chỉ nằm trên 1 worker. 
+  * *NOTE*: phần này chưa đảm bảo được việc đủ partitions trên các workers
+
+* 0.1.6
+  * missing version do nâng cấp CICD
+
+* 0.1.7
+  * Sử dụng threading để quản lý heart_beat và expiry_time
+  * Kiểm tra trạng thái subscribe của worker mỗi khi chuẩn bị process data (Đảm bảo rằng việc subscribe phải diễn ra thành công tránh 2 worker cùng xử lý 1 partition)
+
+* 0.1.8
+  * Cho phép truyền zookeeper_uri vào param khi khởi tạo Schedule, nếu không truyền thì lấy mặc định từ ENV: ZOOKEEPER_CLUSTER
+
+* 0.1.9
+  * Tự động quản lý và cập nhật state cho worker.
+  * fix lỗi tự động release worker ở bản 0.1.8
```

### Comparing `m_scheduler_partitioning-0.1.8/README.md` & `m_scheduler_partitioning-0.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -48,8 +48,12 @@
   * missing version do nâng cấp CICD
 
 * 0.1.7
   * Sử dụng threading để quản lý heart_beat và expiry_time
   * Kiểm tra trạng thái subscribe của worker mỗi khi chuẩn bị process data (Đảm bảo rằng việc subscribe phải diễn ra thành công tránh 2 worker cùng xử lý 1 partition)
 
 * 0.1.8
-  * Cho phép truyền zookeeper_uri vào param khi khởi tạo Schedule, nếu không truyền thì lấy mặc định từ ENV: ZOOKEEPER_CLUSTER
+  * Cho phép truyền zookeeper_uri vào param khi khởi tạo Schedule, nếu không truyền thì lấy mặc định từ ENV: ZOOKEEPER_CLUSTER
+
+* 0.1.9
+  * Tự động quản lý và cập nhật state cho worker.
+  * fix lỗi tự động release worker ở bản 0.1.8
```

### Comparing `m_scheduler_partitioning-0.1.8/m_scheduler_partitioning.egg-info/PKG-INFO` & `m_scheduler_partitioning-0.1.9/m_scheduler_partitioning.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 Metadata-Version: 2.1
 Name: m-scheduler-partitioning
-Version: 0.1.8
+Version: 0.1.9
 Summary: Mobio scheduler partitioning libs
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
-Description: Thư viện scheduler multiple partitions của Profiling
-        
-        <b>nop</b>: maximum partitions now support is 1000 
-        <br>
-        <b>delays</b>: maximum time delays now support is 3600 seconds (1 hour)
-        
-        sample code:
-        
-        ```python
-        from mobio.libs.m_scheduler_partitioning.m_scheduler import MobioScheduler
-        from mobio.libs.m_scheduler_partitioning.scheduler_models.scheduler_state_model import SchedulerStateModel
-        
-        
-        class SampleScheduler(MobioScheduler):
-            def process(self):
-                if self.url_connection:
-                    SchedulerStateModel(self.url_connection).set_busy(
-                        worker_id=self.node_id
-                    )
-                print("Hi there ! :)")
-        
-        
-        if __name__ == "__main__":
-            SampleScheduler(root_node="test-scheduler", nop=100, delays=1, url_connection="mongodb://test_user:test_password@0.0.0.0:27017/test_db", zookeeper_uri="127.0.0.1:2181")
-        
-        ```
-        # Change logs
-        * 0.1.2
-          * log state of worker
-          * get free worker
-          * Để không bị mất 50k cho anh Lợi, thêm 2 index này:
-        
-                    * db.scheduler_state.createIndex({"expiry_time": 1}, {expireAfterSeconds: 5, name: "expiry_time_1"})
-                    * db.scheduler_state.createIndex({"root_node": 1, "state":1}, {name: "root_node_1_state_1"})
-            
-        * 0.1.3
-          * fix issue khi worker rebalance không tự động cập nhật danh sách partitions.
-            
-        * 0.1.4
-          * fix issue register worker
-          * cơ chế đảm bảo việc register worker với hệ thống csdl
-        * 0.1.5
-          * Refix issue register worker
-          * Thử nghiệm cơ chế đảm bảo 1 partition chỉ nằm trên 1 worker. 
-          * *NOTE*: phần này chưa đảm bảo được việc đủ partitions trên các workers
-        
-        * 0.1.6
-          * missing version do nâng cấp CICD
-        
-        * 0.1.7
-          * Sử dụng threading để quản lý heart_beat và expiry_time
-          * Kiểm tra trạng thái subscribe của worker mỗi khi chuẩn bị process data (Đảm bảo rằng việc subscribe phải diễn ra thành công tránh 2 worker cùng xử lý 1 partition)
-        
-        * 0.1.8
-          * Cho phép truyền zookeeper_uri vào param khi khởi tạo Schedule, nếu không truyền thì lấy mặc định từ ENV: ZOOKEEPER_CLUSTER
 Keywords: mobio,scheduler,partitioning
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+
+Thư viện scheduler multiple partitions của Profiling
+
+<b>nop</b>: maximum partitions now support is 1000 
+<br>
+<b>delays</b>: maximum time delays now support is 3600 seconds (1 hour)
+
+sample code:
+
+```python
+from mobio.libs.m_scheduler_partitioning.m_scheduler import MobioScheduler
+from mobio.libs.m_scheduler_partitioning.scheduler_models.scheduler_state_model import SchedulerStateModel
+
+
+class SampleScheduler(MobioScheduler):
+    def process(self):
+        if self.url_connection:
+            SchedulerStateModel(self.url_connection).set_busy(
+                worker_id=self.node_id
+            )
+        print("Hi there ! :)")
+
+
+if __name__ == "__main__":
+    SampleScheduler(root_node="test-scheduler", nop=100, delays=1, url_connection="mongodb://test_user:test_password@0.0.0.0:27017/test_db", zookeeper_uri="127.0.0.1:2181")
+
+```
+# Change logs
+* 0.1.2
+  * log state of worker
+  * get free worker
+  * Để không bị mất 50k cho anh Lợi, thêm 2 index này:
+
+            * db.scheduler_state.createIndex({"expiry_time": 1}, {expireAfterSeconds: 5, name: "expiry_time_1"})
+            * db.scheduler_state.createIndex({"root_node": 1, "state":1}, {name: "root_node_1_state_1"})
+    
+* 0.1.3
+  * fix issue khi worker rebalance không tự động cập nhật danh sách partitions.
+    
+* 0.1.4
+  * fix issue register worker
+  * cơ chế đảm bảo việc register worker với hệ thống csdl
+* 0.1.5
+  * Refix issue register worker
+  * Thử nghiệm cơ chế đảm bảo 1 partition chỉ nằm trên 1 worker. 
+  * *NOTE*: phần này chưa đảm bảo được việc đủ partitions trên các workers
+
+* 0.1.6
+  * missing version do nâng cấp CICD
+
+* 0.1.7
+  * Sử dụng threading để quản lý heart_beat và expiry_time
+  * Kiểm tra trạng thái subscribe của worker mỗi khi chuẩn bị process data (Đảm bảo rằng việc subscribe phải diễn ra thành công tránh 2 worker cùng xử lý 1 partition)
+
+* 0.1.8
+  * Cho phép truyền zookeeper_uri vào param khi khởi tạo Schedule, nếu không truyền thì lấy mặc định từ ENV: ZOOKEEPER_CLUSTER
+
+* 0.1.9
+  * Tự động quản lý và cập nhật state cho worker.
+  * fix lỗi tự động release worker ở bản 0.1.8
```

### Comparing `m_scheduler_partitioning-0.1.8/m_scheduler_partitioning.egg-info/SOURCES.txt` & `m_scheduler_partitioning-0.1.9/m_scheduler_partitioning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/m_scheduler.py` & `m_scheduler_partitioning-0.1.9/mobio/libs/m_scheduler_partitioning/m_scheduler.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,33 +5,36 @@
 from time import sleep
 from kazoo.client import KazooClient
 from kazoo.recipe.watchers import DataWatch, ChildrenWatch
 from kazoo.exceptions import NodeExistsError
 import ast
 from mobio.libs.m_scheduler_partitioning import generate_nano_id
 from mobio.libs.m_scheduler_partitioning.scheduler_models.scheduler_state_model import (
-    SchedulerStateModel,
+    SchedulerStateModel, SchedulerState
 )
 
 
 class MobioScheduler:
     rebalancing = False
     lst_partitions = []
     zk_client = None
+    last_set_state = datetime.utcnow()
+    current_state = SchedulerState.FREE
+    state_in_db = SchedulerState.FREE
 
     def register_worker(self):
         result_register_worker = None
         count_try = 0
         sleep_time = 3
         while not result_register_worker:
             if count_try >= 10:
                 sleep_time = 10
             try:
                 print(datetime.utcnow(), " waiting for register worker with partitions:", self.lst_partitions)
-                result_register_worker = SchedulerStateModel(self.url_connection).register_worker(
+                result_register_worker = SchedulerStateModel(url_connection=self.url_connection).register_worker(
                     worker_id=self.node_id,
                     partitions=self.lst_partitions,
                     delay_time=self.delays,
                     root_node=self.root_node,
                 )
             except Exception as ex:
                 print(datetime.utcnow(), " register_worker ERROR: {}".format(ex))
@@ -43,23 +46,30 @@
             else:
                 break
         return result_register_worker
 
     def __send_heart_beat(self):
         while True:
             result_increase_expiry_time = None
-            while not result_increase_expiry_time:
-                result_increase_expiry_time = SchedulerStateModel(self.url_connection).increase_expiry_time(
+            while not result_increase_expiry_time and datetime.utcnow().second % 5 == 0:
+                result_increase_expiry_time = SchedulerStateModel(url_connection=self.url_connection).increase_expiry_time(
                     worker_id=self.node_id, delay_time=self.delays
                 )
                 print(datetime.utcnow(), " result_increase_expiry_time: {}".format(result_increase_expiry_time))
                 if not result_increase_expiry_time:
                     result_register_worker = self.register_worker()
                     print(datetime.utcnow(), " register worker success: {}".format(result_register_worker))
-            sleep(10)
+            if (datetime.utcnow() - self.last_set_state).seconds >= 15 and self.state_in_db != self.current_state:
+                result = SchedulerStateModel(url_connection=self.url_connection).set_state(self.node_id,
+                                                                                           state=self.current_state)
+                if result:
+                    print(datetime.utcnow(), "result update state: {} old_state: {}, new_state: {}".format(result, self.state_in_db, self.current_state))
+                    self.state_in_db = str(self.current_state)
+                    self.last_set_state = datetime.utcnow()
+            sleep(1)
 
     def __init__(
         self,
         root_node="test-scheduler",
         node_id=None,
         nop=100,
         delays=1,
@@ -104,19 +114,26 @@
         data_watch_child = DataWatch(
             client=self.zk_client, path=self.my_node_path, func=self.watch_data_children
         )
         if self.url_connection:
             t = Thread(target=self.__send_heart_beat)
             t.daemon = True
             t.start()
+
         try:
             while True:
                 if self.check_is_subscribed():
+                    if self.url_connection:
+                        self.current_state = str(SchedulerState.BUSY)
+                        self.last_set_state = datetime.utcnow()
                     self.process()
                     print(datetime.utcnow(), " still alive after: {} seconds".format(self.delays))
+                    if self.url_connection:
+                        self.current_state = str(SchedulerState.FREE)
+                        self.last_set_state = datetime.utcnow()
                 else:
                     print(datetime.utcnow(), " worker: {} is not subscribed".format(self.node_id))
                     self.subscribe_to_node()
                 sleep(self.delays)
         except RuntimeError as e:
             print(datetime.utcnow(), " something unexpected happened: {}: {}".format(self.my_node_path, e))
         finally:
@@ -240,18 +257,19 @@
                 result_check_partition_in_parent = self.check_partition_in_parent(partition=p)
                 if result_check_partition_in_parent:
                     self.lst_partitions.append(p)
         print(datetime.utcnow(), " current partition: {}".format(self.lst_partitions))
         if self.url_connection:
             result = None
             while not result:
-                result = SchedulerStateModel(self.url_connection).rebalance_partitions(
-                    worker_id=self.node_id, partitions=self.lst_partitions
-                )
-                print(datetime.utcnow(), " result rebalance: {}".format(result))
+                if self.url_connection:
+                    result = SchedulerStateModel(url_connection=self.url_connection).rebalance_partitions(
+                        worker_id=self.node_id, partitions=self.lst_partitions
+                    )
+                    print(datetime.utcnow(), " result rebalance: {}".format(result))
                 if not result:
                     result_register_worker = self.register_worker()
                     print(datetime.utcnow(), " register worker success: {}".format(result_register_worker))
 
     # function reset số lượng partitions cúa worker này.
     def rebalance_current_node(self):
         self.zk_client.set(path=self.my_node_path, value=bytes("", "utf-8"))
```

### Comparing `m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/scheduler_models/base_model.py` & `m_scheduler_partitioning-0.1.9/mobio/libs/m_scheduler_partitioning/scheduler_models/base_model.py`

 * *Files identical despite different names*

### Comparing `m_scheduler_partitioning-0.1.8/mobio/libs/m_scheduler_partitioning/scheduler_models/db_manager.py` & `m_scheduler_partitioning-0.1.9/mobio/libs/m_scheduler_partitioning/scheduler_models/db_manager.py`

 * *Files identical despite different names*

### Comparing `m_scheduler_partitioning-0.1.8/setup.py` & `m_scheduler_partitioning-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         :return:
         """
         requirements = ["nanoid==2.0.0", "kazoo==2.8.0"]
         return requirements
 
 
 version_dev='0.1.7'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
-version_prod='0.1.8'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
+version_prod='0.1.9'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
 
 run_mode = ''
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
@@ -48,15 +48,15 @@
     name="m_scheduler_partitioning" + run_mode,  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.1.8',  # Required, Phần này cũng không được format file.
+    version='0.1.9',  # Required, Phần này cũng không được format file.
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Mobio scheduler partitioning libs",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

