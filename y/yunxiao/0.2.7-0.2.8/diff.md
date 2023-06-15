# Comparing `tmp/yunxiao-0.2.7.tar.gz` & `tmp/yunxiao-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.2.7.tar", last modified: Wed Jun 14 17:49:56 2023, max compression
+gzip compressed data, was "yunxiao-0.2.8.tar", last modified: Thu Jun 15 05:57:02 2023, max compression
```

## Comparing `yunxiao-0.2.7.tar` & `yunxiao-0.2.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 17:49:56.603193 yunxiao-0.2.7/
--rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.2.7/LICENSE
--rw-rw-rw-   0        0        0    12954 2023-06-14 17:49:56.602184 yunxiao-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0    12463 2023-06-12 14:40:15.000000 yunxiao-0.2.7/README.md
--rw-rw-rw-   0        0        0     1250 2023-06-14 17:49:40.000000 yunxiao-0.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 17:49:56.603193 yunxiao-0.2.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-14 17:49:56.591036 yunxiao-0.2.7/test/
--rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.2.7/test/test.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:49:56.596099 yunxiao-0.2.7/yunxiao/
--rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.2.7/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    21527 2023-06-12 09:49:14.000000 yunxiao-0.2.7/yunxiao/app.py
--rw-rw-rw-   0        0        0    18555 2023-06-14 17:49:30.000000 yunxiao-0.2.7/yunxiao/v2.py
--rw-rw-rw-   0        0        0    10142 2023-06-10 13:46:06.000000 yunxiao-0.2.7/yunxiao/web.py
--rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.2.7/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:49:56.601157 yunxiao-0.2.7/yunxiao.egg-info/
--rw-rw-rw-   0        0        0    12954 2023-06-14 17:49:56.000000 yunxiao-0.2.7/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-06-14 17:49:56.000000 yunxiao-0.2.7/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 17:49:56.000000 yunxiao-0.2.7/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 17:49:56.000000 yunxiao-0.2.7/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-14 17:49:56.000000 yunxiao-0.2.7/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 05:57:02.733653 yunxiao-0.2.8/
+-rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0    12954 2023-06-15 05:57:02.732643 yunxiao-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0    12463 2023-06-12 14:40:15.000000 yunxiao-0.2.8/README.md
+-rw-rw-rw-   0        0        0     1250 2023-06-15 05:56:45.000000 yunxiao-0.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-15 05:57:02.733653 yunxiao-0.2.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-15 05:57:02.720496 yunxiao-0.2.8/test/
+-rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.2.8/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:57:02.725569 yunxiao-0.2.8/yunxiao/
+-rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.2.8/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    21527 2023-06-12 09:49:14.000000 yunxiao-0.2.8/yunxiao/app.py
+-rw-rw-rw-   0        0        0    20799 2023-06-15 05:56:37.000000 yunxiao-0.2.8/yunxiao/v2.py
+-rw-rw-rw-   0        0        0    10142 2023-06-10 13:46:06.000000 yunxiao-0.2.8/yunxiao/web.py
+-rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.2.8/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:57:02.731632 yunxiao-0.2.8/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0    12954 2023-06-15 05:57:02.000000 yunxiao-0.2.8/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-06-15 05:57:02.000000 yunxiao-0.2.8/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 05:57:02.000000 yunxiao-0.2.8/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 05:57:02.000000 yunxiao-0.2.8/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-15 05:57:02.000000 yunxiao-0.2.8/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.2.7/LICENSE` & `yunxiao-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.7/PKG-INFO` & `yunxiao-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.2.7
+Version: 0.2.8
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `yunxiao-0.2.7/README.md` & `yunxiao-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.7/pyproject.toml` & `yunxiao-0.2.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.2.7"
+version = "0.2.8"
 description = "An API SDK tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "YiZixuan", email = "admin@sqkkyzx.com"},
 ]
 license.text = "GPL-3.0-only"
 classifiers = [
```

### Comparing `yunxiao-0.2.7/yunxiao/app.py` & `yunxiao-0.2.8/yunxiao/app.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.7/yunxiao/v2.py` & `yunxiao-0.2.8/yunxiao/v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,22 @@
             self.renew_cookie()
             self.renew_token()
             response = requests.request(
                 method=kwargs.get("method"),
                 url=kwargs.get("url"),
                 json=kwargs.get("json"),
                 params=kwargs.get("params"),
-                headers={"x3-authentication": self.token, "Cookie": self.cookie}
+                headers={
+                    "x3-authentication": self.token,
+                    "Cookie": self.cookie,
+                    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) "
+                                  "Chrome/114.0.0.0 Safari/537.36 Edg/114.0.1823.43",
+                    "Origin": "https://yunxiao.xiaogj.com",
+                    "Referer": "https://yunxiao.xiaogj.com/app/teacher/"
+                }
             )
 
         return response.json()
 
     # 循环装饰器
     @staticmethod
     def loop(KEY):
@@ -56,22 +63,22 @@
             def wrapper(*args, **kwargs):
                 result = []
                 count = 1
                 page = kwargs.get("page")
                 size = kwargs.get("size")
                 while (now := len(result)) != count:
                     page += 1
+                    kwargs["page"] = page
                     res = func(*args, **kwargs)
                     data = res["data"][KEY] if KEY else res["data"]
                     result.extend(data)
                     count = res["page"]["totalCount"]
                     print(f"size: {size}, page: {page}, {now}/{count}")
                     size = size if (count - len(result)) > size else (count - len(result))
                     kwargs["size"] = size
-                    kwargs["page"] = page
                 print(f"size: {size}, page: {page}, {now}/{count}")
                 return result
 
             return wrapper
 
         return wrapper_func
 
@@ -212,26 +219,27 @@
     # 列出指定日期范围全部排课
     @loop("")
     def arrange_list_daterange(self, page, size, before_today: int, after_today: int):
         """
         列出全部排课
         :return:
         """
-        return self.request(
+        res = self.request(
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-edu/arrange/page",
             json={
                 "_t_": UsedTime.stamp,
                 "campusIds": self.campus,
                 "startDate": time.strftime('%Y-%m-%d', time.localtime(time.time() - 86400 * before_today)),
                 "endDate": time.strftime('%Y-%m-%d', time.localtime(time.time() + 86400 * after_today)),
                 "displayCompletedClass": True,
                 "page": {"pageNum": page, "pageSize": size}
             }
         )
+        return res
 
     # 列出指定日期全部排课[最大999条]
     def arrange_list_date(self, date: str = UsedTime.today) -> list:
         """
         列出日期范围全部排课[最大9999条]
         :param date:
         :return:
@@ -248,15 +256,15 @@
                     "pageSize": 999
                 }
             }
         )["data"]
 
     # 查询指定日期范围排课
     def arrange_query_daterange(self, starttime: str = None, endtime: str = None,
-                                displayCompletedClass=False, size: int = 99999) -> list:
+                                displayCompletedClass=False, size: int = 9999) -> list:
         """
         排课管理。
         :param displayCompletedClass: 显示已结班排课
         :param size:
         :param starttime: 查询起始时间
         :param endtime: 查询截止时间
         :return:
@@ -399,15 +407,15 @@
                 "courseStartTime": startdate,
                 "curriculumIds": [],
                 "studentIds": [],
                 "teacherIds": []
             }
         )
 
-    # 列出指定操作日期范围的所有订单记录
+    # 列出指定操作日期范围的所有订单项目记录
     @loop("orderItemAllList")
     def order_item_list_all(self, page, size, startdate: str = "", enddate: str = ""):
         """
         列出指定操作日期范围的所有订单记录
         :param size: 每次取数据的分片量
         :param page: 从第几页开始取数据。应设为 0
         :param enddate: YY-MM-DD
@@ -422,14 +430,61 @@
                 "page": {"pageNum": page, "pageSize": size},
                 "campusIds": self.campus,
                 "startTime": startdate,
                 "endTime": enddate
             }
         )
 
+    # 列出指定操作日期范围的所有收入/转课订单组记录
+    @loop("")
+    def order_list_all(self, page, size, startdate: str = "", enddate: str = ""):
+        """
+        列出指定操作日期范围的所有订单记录
+        :param size: 每次取数据的分片量
+        :param page: 从第几页开始取数据。应设为 0
+        :param enddate: YY-MM-DD
+        :param startdate: YY-MM-DD
+        :return:
+        """
+        return self.request(
+            method="post",
+            url="https://yunxiao.xiaogj.com/api/cs-edu/orderInfo/pageAdbOrder",
+            json={
+                "_t_": UsedTime.stamp,
+                "page": {"pageNum": page, "pageSize": size},
+                "campusIds": self.campus,
+                "startTime": startdate,
+                "endTime": enddate
+            }
+        )
+
+    # 列出指定操作日期范围的所有退费订单组记录
+    @loop("")
+    def order_refund_list_all(self, page, size, startdate: str = "", enddate: str = ""):
+        """
+        列出指定操作日期范围的所有订单记录
+        :param size: 每次取数据的分片量
+        :param page: 从第几页开始取数据。应设为 0
+        :param enddate: YY-MM-DD
+        :param startdate: YY-MM-DD
+        :return:
+        """
+        return self.request(
+            method="post",
+            url="https://yunxiao.xiaogj.com/api/cs-edu/orderRefund/adbRefundOrderInfoPage",
+            json={
+                "_t_": UsedTime.stamp,
+                "page": {"pageNum": page, "pageSize": size},
+                "campusIds": self.campus,
+                "orderType": 2,
+                "startTime": startdate,
+                "endTime": enddate
+            }
+        )
+
     # 列出指定操作日期范围的所有退费详情
     def payment_refund_list_all(self, startdate: str = "", enddate: str = "") -> list:
         """
         列出指定操作日期范围的所有订单记录
         :param enddate: YY-MM-DD
         :param startdate: YY-MM-DD
         :return:
@@ -442,33 +497,34 @@
                 "page": {"pageNum": 1, "pageSize": 10000},
                 "campusIds": self.campus,
                 "refundFinishStartTime": startdate,
                 "refundFinishEndTime": enddate
             }
         )["data"]
 
-    # 列出指定操作日期范围的所有支出详情
-    def payment_item_list_all(self, startdate: str = "", enddate: str = "") -> list:
+    # 列出指定操作日期范围的所有收入详情
+    @loop("paymentDetailDtos")
+    def payment_item_list_all(self, page, size, startdate: str = "", enddate: str = ""):
         """
         列出指定操作日期范围的所有订单记录
         :param enddate: YY-MM-DD
         :param startdate: YY-MM-DD
         :return:
         """
         return self.request(
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-pc-report/cs-report/reports/findPaymentList",
             json={
                 "_t_": UsedTime.stamp,
-                "page": {"pageNum": 1, "pageSize": 10000},
+                "page": {"pageNum": page, "pageSize": size},
                 "campusIds": self.campus,
                 "payStartTime": startdate,
                 "payEndTime": enddate
             }
-        )["data"]
+        )
 
     # 列出指定操作日期范围的所有账户收支记录
     def payment_record_list_all(self, startdate: str = "", enddate: str = "") -> list:
         """
         列出指定操作日期范围的所有订单记录
         :param enddate: YY-MM-DD
         :param startdate: YY-MM-DD
```

### Comparing `yunxiao-0.2.7/yunxiao/web.py` & `yunxiao-0.2.8/yunxiao/web.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.7/yunxiao/yunxiao.py` & `yunxiao-0.2.8/yunxiao/yunxiao.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.7/yunxiao.egg-info/PKG-INFO` & `yunxiao-0.2.8/yunxiao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.2.7
+Version: 0.2.8
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

