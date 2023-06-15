# Comparing `tmp/tencentcloud-sdk-python-postgres-3.0.914.tar.gz` & `tmp/tencentcloud-sdk-python-postgres-3.0.915.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.914.tar", last modified: Wed Jun 14 00:31:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.915.tar", last modified: Thu Jun 15 00:31:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-postgres-3.0.914.tar` & `tencentcloud-sdk-python-postgres-3.0.915.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/postgres/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/postgres/v20170312/
--rw-r--r--   0 root         (0) root         (0)    85728 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/postgres/v20170312/postgres_client.py
--rw-r--r--   0 root         (0) root         (0)    20657 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/postgres/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/postgres/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   277922 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/postgres/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud_sdk_python_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:31:02.000000 tencentcloud-sdk-python-postgres-3.0.915/
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-15 00:31:02.000000 tencentcloud-sdk-python-postgres-3.0.915/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:31:02.000000 tencentcloud-sdk-python-postgres-3.0.915/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:31:02.000000 tencentcloud-sdk-python-postgres-3.0.915/tencentcloud/postgres/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:31:02.000000 tencentcloud-sdk-python-postgres-3.0.915/tencentcloud/postgres/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    85773 2023-06-15 00:31:02.000000 tencentcloud-sdk-python-postgres-3.0.915/tencentcloud/postgres/v20170312/postgres_client.py
+-rw-r--r--   0 root         (0) root         (0)    20657 2023-06-15 00:31:02.000000 tencentcloud-sdk-python-postgres-3.0.915/tencentcloud/postgres/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:31:02.000000 tencentcloud-sdk-python-postgres-3.0.915/tencentcloud/postgres/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   277941 2023-06-15 00:31:02.000000 tencentcloud-sdk-python-postgres-3.0.915/tencentcloud/postgres/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:31:02.000000 tencentcloud-sdk-python-postgres-3.0.915/tencentcloud/postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-15 00:31:02.000000 tencentcloud-sdk-python-postgres-3.0.915/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-15 00:31:02.000000 tencentcloud-sdk-python-postgres-3.0.915/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-06-15 00:31:02.000000 tencentcloud-sdk-python-postgres-3.0.915/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-15 00:31:02.000000 tencentcloud-sdk-python-postgres-3.0.915/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:31:02.000000 tencentcloud-sdk-python-postgres-3.0.915/tencentcloud_sdk_python_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 00:31:02.000000 tencentcloud-sdk-python-postgres-3.0.915/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-06-15 00:31:02.000000 tencentcloud-sdk-python-postgres-3.0.915/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-15 00:31:02.000000 tencentcloud-sdk-python-postgres-3.0.915/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-15 00:31:02.000000 tencentcloud-sdk-python-postgres-3.0.915/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.914/README.rst` & `tencentcloud-sdk-python-postgres-3.0.915/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/postgres/v20170312/postgres_client.py` & `tencentcloud-sdk-python-postgres-3.0.915/tencentcloud/postgres/v20170312/postgres_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -782,15 +782,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeDBInstanceParameters(self, request):
-        """获取实例可修改参数列表
+        """本接口（DescribeDBInstanceAttribute）用于查询实例的参数信息。
 
         :param request: Request instance for DescribeDBInstanceParameters.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeDBInstanceParametersRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.DescribeDBInstanceParametersResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/postgres/v20170312/errorcodes.py` & `tencentcloud-sdk-python-postgres-3.0.915/tencentcloud/postgres/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/postgres/v20170312/models.py` & `tencentcloud-sdk-python-postgres-3.0.915/tencentcloud/postgres/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -961,15 +961,18 @@
 1、mssql_compatible引擎：
 migrationMode：数据库模式，可选参数，可取值：single-db（单数据库模式），multi-db（多数据库模式）。默认为single-db。
 defaultLocale：排序区域规则，可选参数，在初始化后不可修改，默认为en_US，可选值如下：
 "af_ZA", "sq_AL", "ar_DZ", "ar_BH", "ar_EG", "ar_IQ", "ar_JO", "ar_KW", "ar_LB", "ar_LY", "ar_MA", "ar_OM", "ar_QA", "ar_SA", "ar_SY", "ar_TN", "ar_AE", "ar_YE", "hy_AM", "az_Cyrl_AZ", "az_Latn_AZ", "eu_ES", "be_BY", "bg_BG", "ca_ES", "zh_HK", "zh_MO", "zh_CN", "zh_SG", "zh_TW", "hr_HR", "cs_CZ", "da_DK", "nl_BE", "nl_NL", "en_AU", "en_BZ", "en_CA", "en_IE", "en_JM", "en_NZ", "en_PH", "en_ZA", "en_TT", "en_GB", "en_US", "en_ZW", "et_EE", "fo_FO", "fa_IR", "fi_FI", "fr_BE", "fr_CA", "fr_FR", "fr_LU", "fr_MC", "fr_CH", "mk_MK", "ka_GE", "de_AT", "de_DE", "de_LI", "de_LU", "de_CH", "el_GR", "gu_IN", "he_IL", "hi_IN", "hu_HU", "is_IS", "id_ID", "it_IT", "it_CH", "ja_JP", "kn_IN", "kok_IN", "ko_KR", "ky_KG", "lv_LV", "lt_LT", "ms_BN", "ms_MY", "mr_IN", "mn_MN", "nb_NO", "nn_NO", "pl_PL", "pt_BR", "pt_PT", "pa_IN", "ro_RO", "ru_RU", "sa_IN", "sr_Cyrl_RS", "sr_Latn_RS", "sk_SK", "sl_SI", "es_AR", "es_BO", "es_CL", "es_CO", "es_CR", "es_DO", "es_EC", "es_SV", "es_GT", "es_HN", "es_MX", "es_NI", "es_PA", "es_PY","es_PE", "es_PR", "es_ES", "es_TRADITIONAL", "es_UY", "es_VE", "sw_KE", "sv_FI", "sv_SE", "tt_RU", "te_IN", "th_TH", "tr_TR", "uk_UA", "ur_IN", "ur_PK", "uz_Cyrl_UZ", "uz_Latn_UZ", "vi_VN"。
 serverCollationName：排序规则名称，可选参数，在初始化后不可修改，默认为sql_latin1_general_cp1_ci_as，可选值如下：
 "bbf_unicode_general_ci_as", "bbf_unicode_cp1_ci_as", "bbf_unicode_CP1250_ci_as", "bbf_unicode_CP1251_ci_as", "bbf_unicode_cp1253_ci_as", "bbf_unicode_cp1254_ci_as", "bbf_unicode_cp1255_ci_as", "bbf_unicode_cp1256_ci_as", "bbf_unicode_cp1257_ci_as", "bbf_unicode_cp1258_ci_as", "bbf_unicode_cp874_ci_as", "sql_latin1_general_cp1250_ci_as", "sql_latin1_general_cp1251_ci_as", "sql_latin1_general_cp1_ci_as", "sql_latin1_general_cp1253_ci_as", "sql_latin1_general_cp1254_ci_as", "sql_latin1_general_cp1255_ci_as","sql_latin1_general_cp1256_ci_as", "sql_latin1_general_cp1257_ci_as", "sql_latin1_general_cp1258_ci_as", "chinese_prc_ci_as", "cyrillic_general_ci_as", "finnish_swedish_ci_as", "french_ci_as", "japanese_ci_as", "korean_wansung_ci_as", "latin1_general_ci_as", "modern_spanish_ci_as", "polish_ci_as", "thai_ci_as", "traditional_spanish_ci_as", "turkish_ci_as", "ukrainian_ci_as", "vietnamese_ci_as"。
         :type DBEngineConfig: str
-        :param SyncMode: 主从同步方式，取值： 1)Semi-sync：半同步 2)Async：异步 默认为Async
+        :param SyncMode: 主从同步方式，可取值： 
+1、Semi-sync：半同步
+2、Async：异步 
+当前只支持Semi-sync
         :type SyncMode: str
         """
         self.SpecCode = None
         self.Storage = None
         self.InstanceCount = None
         self.Period = None
         self.Zone = None
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/__init__.py` & `tencentcloud-sdk-python-postgres-3.0.915/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.914'
+__version__ = '3.0.915'
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.914/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.915/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.914
+Version: 3.0.915
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.914/setup.py` & `tencentcloud-sdk-python-postgres-3.0.915/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.914/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.915/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.914
+Version: 3.0.915
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

