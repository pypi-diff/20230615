# Comparing `tmp/PublicDataReader-1.0.8.tar.gz` & `tmp/PublicDataReader-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PublicDataReader-1.0.8.tar", last modified: Mon Jan  2 08:51:22 2023, max compression
+gzip compressed data, was "PublicDataReader-1.0.9.tar", last modified: Tue Jan  3 06:07:00 2023, max compression
```

## Comparing `PublicDataReader-1.0.8.tar` & `PublicDataReader-1.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-01-02 08:51:22.581233 PublicDataReader-1.0.8/
--rw-rw-rw-   0        0        0     1083 2022-11-07 02:02:05.000000 PublicDataReader-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     6202 2023-01-02 08:51:22.581233 PublicDataReader-1.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-01-02 08:51:22.539346 PublicDataReader-1.0.8/PublicDataReader/
-drwxrwxrwx   0        0        0        0 2023-01-02 08:51:22.565276 PublicDataReader-1.0.8/PublicDataReader/PublicDataPortal/
--rw-rw-rw-   0        0        0        0 2022-11-07 02:02:05.000000 PublicDataReader-1.0.8/PublicDataReader/PublicDataPortal/__init__.py
--rw-rw-rw-   0        0        0     9226 2022-12-05 05:25:54.000000 PublicDataReader-1.0.8/PublicDataReader/PublicDataPortal/kamco.py
--rw-rw-rw-   0        0        0    46902 2022-11-07 02:02:05.000000 PublicDataReader-1.0.8/PublicDataReader/PublicDataPortal/molit.py
--rw-rw-rw-   0        0        0     2114 2022-12-16 08:28:53.000000 PublicDataReader-1.0.8/PublicDataReader/PublicDataPortal/nts.py
--rw-rw-rw-   0        0        0    14988 2022-11-07 02:02:05.000000 PublicDataReader-1.0.8/PublicDataReader/PublicDataPortal/semas.py
-drwxrwxrwx   0        0        0        0 2023-01-02 08:51:22.568269 PublicDataReader-1.0.8/PublicDataReader/Seoul/
--rw-rw-rw-   0        0        0        0 2022-11-07 02:02:05.000000 PublicDataReader-1.0.8/PublicDataReader/Seoul/__init__.py
--rw-rw-rw-   0        0        0     5456 2022-11-07 02:02:05.000000 PublicDataReader-1.0.8/PublicDataReader/Seoul/transportation.py
--rw-rw-rw-   0        0        0      463 2023-01-02 00:44:59.000000 PublicDataReader-1.0.8/PublicDataReader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-02 08:51:22.570263 PublicDataReader-1.0.8/PublicDataReader/config/
--rw-rw-rw-   0        0        0        0 2022-11-07 02:02:05.000000 PublicDataReader-1.0.8/PublicDataReader/config/__init__.py
--rw-rw-rw-   0        0        0      158 2023-01-02 08:49:49.000000 PublicDataReader-1.0.8/PublicDataReader/config/info.py
--rw-rw-rw-   0        0        0      926 2023-01-02 00:44:59.000000 PublicDataReader-1.0.8/PublicDataReader/data.py
-drwxrwxrwx   0        0        0        0 2023-01-02 08:51:22.572257 PublicDataReader-1.0.8/PublicDataReader/kbland/
--rw-rw-rw-   0        0        0        0 2023-01-02 00:44:59.000000 PublicDataReader-1.0.8/PublicDataReader/kbland/__init__.py
--rw-rw-rw-   0        0        0    44957 2023-01-02 08:45:56.000000 PublicDataReader-1.0.8/PublicDataReader/kbland/kbland.py
-drwxrwxrwx   0        0        0        0 2023-01-02 08:51:22.574252 PublicDataReader-1.0.8/PublicDataReader/kosis/
--rw-rw-rw-   0        0        0        0 2022-11-07 02:02:05.000000 PublicDataReader-1.0.8/PublicDataReader/kosis/__init__.py
--rw-rw-rw-   0        0        0     3675 2022-11-07 04:05:41.000000 PublicDataReader-1.0.8/PublicDataReader/kosis/kosis.py
-drwxrwxrwx   0        0        0        0 2023-01-02 08:51:22.577244 PublicDataReader-1.0.8/PublicDataReader/utils/
--rw-rw-rw-   0        0        0        0 2022-11-07 02:02:05.000000 PublicDataReader-1.0.8/PublicDataReader/utils/__init__.py
--rw-rw-rw-   0        0        0      928 2022-11-07 02:02:05.000000 PublicDataReader-1.0.8/PublicDataReader/utils/code.py
-drwxrwxrwx   0        0        0        0 2023-01-02 08:51:22.579239 PublicDataReader-1.0.8/PublicDataReader/vworld/
--rw-rw-rw-   0        0        0        0 2022-11-07 02:02:05.000000 PublicDataReader-1.0.8/PublicDataReader/vworld/__init__.py
--rw-rw-rw-   0        0        0     1969 2022-11-07 02:02:05.000000 PublicDataReader-1.0.8/PublicDataReader/vworld/data.py
-drwxrwxrwx   0        0        0        0 2023-01-02 08:51:22.559292 PublicDataReader-1.0.8/PublicDataReader.egg-info/
--rw-rw-rw-   0        0        0     6202 2023-01-02 08:51:22.000000 PublicDataReader-1.0.8/PublicDataReader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      910 2023-01-02 08:51:22.000000 PublicDataReader-1.0.8/PublicDataReader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-02 08:51:22.000000 PublicDataReader-1.0.8/PublicDataReader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-01-02 08:51:22.000000 PublicDataReader-1.0.8/PublicDataReader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-01-02 08:51:22.000000 PublicDataReader-1.0.8/PublicDataReader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5724 2023-01-02 00:44:59.000000 PublicDataReader-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-01-02 08:51:22.581233 PublicDataReader-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      991 2022-12-01 06:36:25.000000 PublicDataReader-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-03 06:07:00.477204 PublicDataReader-1.0.9/
+-rw-rw-rw-   0        0        0     1083 2022-11-07 02:02:05.000000 PublicDataReader-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     6202 2023-01-03 06:07:00.476208 PublicDataReader-1.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-01-03 06:07:00.435346 PublicDataReader-1.0.9/PublicDataReader/
+drwxrwxrwx   0        0        0        0 2023-01-03 06:07:00.461279 PublicDataReader-1.0.9/PublicDataReader/PublicDataPortal/
+-rw-rw-rw-   0        0        0        0 2022-11-07 02:02:05.000000 PublicDataReader-1.0.9/PublicDataReader/PublicDataPortal/__init__.py
+-rw-rw-rw-   0        0        0     9226 2022-12-05 05:25:54.000000 PublicDataReader-1.0.9/PublicDataReader/PublicDataPortal/kamco.py
+-rw-rw-rw-   0        0        0    46902 2022-11-07 02:02:05.000000 PublicDataReader-1.0.9/PublicDataReader/PublicDataPortal/molit.py
+-rw-rw-rw-   0        0        0     2114 2022-12-16 08:28:53.000000 PublicDataReader-1.0.9/PublicDataReader/PublicDataPortal/nts.py
+-rw-rw-rw-   0        0        0    14988 2022-11-07 02:02:05.000000 PublicDataReader-1.0.9/PublicDataReader/PublicDataPortal/semas.py
+drwxrwxrwx   0        0        0        0 2023-01-03 06:07:00.463271 PublicDataReader-1.0.9/PublicDataReader/Seoul/
+-rw-rw-rw-   0        0        0        0 2022-11-07 02:02:05.000000 PublicDataReader-1.0.9/PublicDataReader/Seoul/__init__.py
+-rw-rw-rw-   0        0        0     5456 2022-11-07 02:02:05.000000 PublicDataReader-1.0.9/PublicDataReader/Seoul/transportation.py
+-rw-rw-rw-   0        0        0      494 2023-01-03 05:47:56.000000 PublicDataReader-1.0.9/PublicDataReader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-01-03 06:07:00.466234 PublicDataReader-1.0.9/PublicDataReader/config/
+-rw-rw-rw-   0        0        0        0 2022-11-07 02:02:05.000000 PublicDataReader-1.0.9/PublicDataReader/config/__init__.py
+-rw-rw-rw-   0        0        0      158 2023-01-03 05:49:11.000000 PublicDataReader-1.0.9/PublicDataReader/config/info.py
+-rw-rw-rw-   0        0        0      956 2023-01-03 05:47:40.000000 PublicDataReader-1.0.9/PublicDataReader/data.py
+drwxrwxrwx   0        0        0        0 2023-01-03 06:07:00.468229 PublicDataReader-1.0.9/PublicDataReader/kbland/
+-rw-rw-rw-   0        0        0        0 2023-01-02 00:44:59.000000 PublicDataReader-1.0.9/PublicDataReader/kbland/__init__.py
+-rw-rw-rw-   0        0        0    44957 2023-01-02 08:45:56.000000 PublicDataReader-1.0.9/PublicDataReader/kbland/kbland.py
+drwxrwxrwx   0        0        0        0 2023-01-03 06:07:00.470224 PublicDataReader-1.0.9/PublicDataReader/kosis/
+-rw-rw-rw-   0        0        0        0 2022-11-07 02:02:05.000000 PublicDataReader-1.0.9/PublicDataReader/kosis/__init__.py
+-rw-rw-rw-   0        0        0     3675 2022-11-07 04:05:41.000000 PublicDataReader-1.0.9/PublicDataReader/kosis/kosis.py
+drwxrwxrwx   0        0        0        0 2023-01-03 06:07:00.473215 PublicDataReader-1.0.9/PublicDataReader/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-07 02:02:05.000000 PublicDataReader-1.0.9/PublicDataReader/utils/__init__.py
+-rw-rw-rw-   0        0        0     1471 2023-01-03 06:01:11.000000 PublicDataReader-1.0.9/PublicDataReader/utils/code.py
+drwxrwxrwx   0        0        0        0 2023-01-03 06:07:00.475210 PublicDataReader-1.0.9/PublicDataReader/vworld/
+-rw-rw-rw-   0        0        0        0 2022-11-07 02:02:05.000000 PublicDataReader-1.0.9/PublicDataReader/vworld/__init__.py
+-rw-rw-rw-   0        0        0     1969 2022-11-07 02:02:05.000000 PublicDataReader-1.0.9/PublicDataReader/vworld/data.py
+drwxrwxrwx   0        0        0        0 2023-01-03 06:07:00.455292 PublicDataReader-1.0.9/PublicDataReader.egg-info/
+-rw-rw-rw-   0        0        0     6202 2023-01-03 06:07:00.000000 PublicDataReader-1.0.9/PublicDataReader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      910 2023-01-03 06:07:00.000000 PublicDataReader-1.0.9/PublicDataReader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-03 06:07:00.000000 PublicDataReader-1.0.9/PublicDataReader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-01-03 06:07:00.000000 PublicDataReader-1.0.9/PublicDataReader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-01-03 06:07:00.000000 PublicDataReader-1.0.9/PublicDataReader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5724 2023-01-02 00:44:59.000000 PublicDataReader-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-01-03 06:07:00.477204 PublicDataReader-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      991 2022-12-01 06:36:25.000000 PublicDataReader-1.0.9/setup.py
```

### Comparing `PublicDataReader-1.0.8/LICENSE` & `PublicDataReader-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PublicDataReader-1.0.8/PKG-INFO` & `PublicDataReader-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PublicDataReader
-Version: 1.0.8
+Version: 1.0.9
 Summary: Open Source Public Data Reader
 Home-page: https://github.com/WooilJeong/PublicDataReader
 Author: 정우일(Wooil Jeong)
 Author-email: wooil@kakao.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PublicDataReader-1.0.8/PublicDataReader/PublicDataPortal/kamco.py` & `PublicDataReader-1.0.9/PublicDataReader/PublicDataPortal/kamco.py`

 * *Files identical despite different names*

### Comparing `PublicDataReader-1.0.8/PublicDataReader/PublicDataPortal/molit.py` & `PublicDataReader-1.0.9/PublicDataReader/PublicDataPortal/molit.py`

 * *Files identical despite different names*

### Comparing `PublicDataReader-1.0.8/PublicDataReader/PublicDataPortal/nts.py` & `PublicDataReader-1.0.9/PublicDataReader/PublicDataPortal/nts.py`

 * *Files identical despite different names*

### Comparing `PublicDataReader-1.0.8/PublicDataReader/PublicDataPortal/semas.py` & `PublicDataReader-1.0.9/PublicDataReader/PublicDataPortal/semas.py`

 * *Files identical despite different names*

### Comparing `PublicDataReader-1.0.8/PublicDataReader/Seoul/transportation.py` & `PublicDataReader-1.0.9/PublicDataReader/Seoul/transportation.py`

 * *Files identical despite different names*

### Comparing `PublicDataReader-1.0.8/PublicDataReader/data.py` & `PublicDataReader-1.0.9/PublicDataReader/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 # 국세청 Open API
 from PublicDataReader.PublicDataPortal.nts import Nts
 
 # KB부동산 API
 from PublicDataReader.kbland.kbland import Kbland
 
 # 코드 데이터 조회
-from PublicDataReader.utils.code import code_bdong, get_vworld_data_api_info_by_dataframe, get_vworld_data_api_info_by_dict
+from PublicDataReader.utils.code import code_bdong, code_hdong, code_hdong_bdong, get_vworld_data_api_info_by_dataframe, get_vworld_data_api_info_by_dict
```

### Comparing `PublicDataReader-1.0.8/PublicDataReader/kbland/kbland.py` & `PublicDataReader-1.0.9/PublicDataReader/kbland/kbland.py`

 * *Files identical despite different names*

### Comparing `PublicDataReader-1.0.8/PublicDataReader/kosis/kosis.py` & `PublicDataReader-1.0.9/PublicDataReader/kosis/kosis.py`

 * *Files identical despite different names*

### Comparing `PublicDataReader-1.0.8/PublicDataReader/vworld/data.py` & `PublicDataReader-1.0.9/PublicDataReader/vworld/data.py`

 * *Files identical despite different names*

### Comparing `PublicDataReader-1.0.8/PublicDataReader.egg-info/PKG-INFO` & `PublicDataReader-1.0.9/PublicDataReader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PublicDataReader
-Version: 1.0.8
+Version: 1.0.9
 Summary: Open Source Public Data Reader
 Home-page: https://github.com/WooilJeong/PublicDataReader
 Author: 정우일(Wooil Jeong)
 Author-email: wooil@kakao.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PublicDataReader-1.0.8/PublicDataReader.egg-info/SOURCES.txt` & `PublicDataReader-1.0.9/PublicDataReader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PublicDataReader-1.0.8/README.md` & `PublicDataReader-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `PublicDataReader-1.0.8/setup.py` & `PublicDataReader-1.0.9/setup.py`

 * *Files identical despite different names*

