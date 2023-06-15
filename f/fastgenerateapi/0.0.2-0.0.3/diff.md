# Comparing `tmp/fastgenerateapi-0.0.2.tar.gz` & `tmp/fastgenerateapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastgenerateapi-0.0.2.tar", last modified: Wed Jun 14 08:53:03 2023, max compression
+gzip compressed data, was "fastgenerateapi-0.0.3.tar", last modified: Thu Jun 15 06:54:42 2023, max compression
```

## Comparing `fastgenerateapi-0.0.2.tar` & `fastgenerateapi-0.0.3.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.579274 fastgenerateapi-0.0.2/
--rw-rw-rw-   0        0        0    35821 2023-06-14 08:27:11.000000 fastgenerateapi-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      885 2023-06-14 08:53:03.579274 fastgenerateapi-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-14 08:27:11.000000 fastgenerateapi-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.375508 fastgenerateapi-0.0.2/fastgenerateapi/
--rw-rw-rw-   0        0        0      756 2023-06-14 01:36:26.000000 fastgenerateapi-0.0.2/fastgenerateapi/__init__.py
--rw-rw-rw-   0        0        0      496 2023-06-14 08:27:11.000000 fastgenerateapi-0.0.2/fastgenerateapi/__version__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.407435 fastgenerateapi-0.0.2/fastgenerateapi/api_view/
--rw-rw-rw-   0        0        0       14 2023-06-09 00:54:08.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/__init__.py
--rw-rw-rw-   0        0        0     1160 2023-06-09 00:54:08.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/api_view.py
--rw-rw-rw-   0        0        0     9133 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/base_view.py
--rw-rw-rw-   0        0        0     4202 2023-06-13 14:48:03.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/create_view.py
--rw-rw-rw-   0        0        0     3075 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/delete_view.py
--rw-rw-rw-   0        0        0     7585 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/get_all_view.py
--rw-rw-rw-   0        0        0     3077 2023-06-13 00:43:06.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/get_one_view.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.438713 fastgenerateapi-0.0.2/fastgenerateapi/api_view/mixin/
--rw-rw-rw-   0        0        0        0 2023-06-09 00:54:08.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/mixin/__init__.py
--rw-rw-rw-   0        0        0     6486 2023-06-12 00:42:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/mixin/base_mixin.py
--rw-rw-rw-   0        0        0      266 2023-06-12 00:42:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/mixin/get_mixin.py
--rw-rw-rw-   0        0        0     2221 2023-06-13 00:43:06.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/mixin/response_mixin.py
--rw-rw-rw-   0        0        0      317 2023-06-13 14:43:14.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/mixin/save_mixin.py
--rw-rw-rw-   0        0        0    13029 2023-06-12 00:42:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/mixin/tool_mixin.py
--rw-rw-rw-   0        0        0     3279 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/switch_view.py
--rw-rw-rw-   0        0        0     4150 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/api_view/update_view.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.469957 fastgenerateapi-0.0.2/fastgenerateapi/controller/
--rw-rw-rw-   0        0        0      316 2023-06-09 00:54:08.000000 fastgenerateapi-0.0.2/fastgenerateapi/controller/__init__.py
--rw-rw-rw-   0        0        0     3391 2023-06-13 10:04:30.000000 fastgenerateapi-0.0.2/fastgenerateapi/controller/filter_controller.py
--rw-rw-rw-   0        0        0     2385 2023-06-09 00:54:08.000000 fastgenerateapi-0.0.2/fastgenerateapi/controller/router_controller.py
--rw-rw-rw-   0        0        0     2298 2023-06-09 00:54:08.000000 fastgenerateapi-0.0.2/fastgenerateapi/controller/rpc_controller.py
--rw-rw-rw-   0        0        0      873 2023-06-09 00:54:08.000000 fastgenerateapi-0.0.2/fastgenerateapi/controller/search_controller.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.469957 fastgenerateapi-0.0.2/fastgenerateapi/data_type/
--rw-rw-rw-   0        0        0        0 2023-06-09 00:54:08.000000 fastgenerateapi-0.0.2/fastgenerateapi/data_type/__init__.py
--rw-rw-rw-   0        0        0      727 2023-06-09 00:54:08.000000 fastgenerateapi-0.0.2/fastgenerateapi/data_type/data_type.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.501166 fastgenerateapi-0.0.2/fastgenerateapi/deps/
--rw-rw-rw-   0        0        0      160 2023-06-09 00:54:08.000000 fastgenerateapi-0.0.2/fastgenerateapi/deps/__init__.py
--rw-rw-rw-   0        0        0     1573 2023-06-13 01:42:38.000000 fastgenerateapi-0.0.2/fastgenerateapi/deps/filter_params_deps.py
--rw-rw-rw-   0        0        0     3171 2023-06-13 01:42:38.000000 fastgenerateapi-0.0.2/fastgenerateapi/deps/paginator_deps.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.501166 fastgenerateapi-0.0.2/fastgenerateapi/pydantic_utils/
--rw-rw-rw-   0        0        0        0 2023-06-09 00:54:09.000000 fastgenerateapi-0.0.2/fastgenerateapi/pydantic_utils/__init__.py
--rw-rw-rw-   0        0        0      648 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/pydantic_utils/base_model.py
--rw-rw-rw-   0        0        0     2814 2023-06-12 00:42:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/pydantic_utils/json_encoders.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.548030 fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/
--rw-rw-rw-   0        0        0      472 2023-06-12 00:42:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/__init__.py
--rw-rw-rw-   0        0        0     4296 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/common_function.py
--rw-rw-rw-   0        0        0     1856 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/create_schema_factory.py
--rw-rw-rw-   0        0        0     3102 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/get_all_schema_factory.py
--rw-rw-rw-   0        0        0     1763 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/get_one_schema_factory.py
--rw-rw-rw-   0        0        0     1251 2023-06-12 00:42:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/response_factory.py
--rw-rw-rw-   0        0        0     1856 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/update_schema_factory.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.563683 fastgenerateapi-0.0.2/fastgenerateapi/settings/
--rw-rw-rw-   0        0        0        6 2023-06-09 00:54:09.000000 fastgenerateapi-0.0.2/fastgenerateapi/settings/__init__.py
--rw-rw-rw-   0        0        0      232 2023-06-09 00:54:09.000000 fastgenerateapi-0.0.2/fastgenerateapi/settings/register_settings.py
--rw-rw-rw-   0        0        0     2955 2023-06-14 01:34:53.000000 fastgenerateapi-0.0.2/fastgenerateapi/settings/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.563683 fastgenerateapi-0.0.2/fastgenerateapi/utils/
--rw-rw-rw-   0        0        0        0 2023-06-09 00:54:09.000000 fastgenerateapi-0.0.2/fastgenerateapi/utils/__init__.py
--rw-rw-rw-   0        0        0      121 2023-06-09 00:54:09.000000 fastgenerateapi-0.0.2/fastgenerateapi/utils/exception.py
--rw-rw-rw-   0        0        0      670 2023-06-09 00:54:09.000000 fastgenerateapi-0.0.2/fastgenerateapi/utils/parse_str.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:53:03.391129 fastgenerateapi-0.0.2/fastgenerateapi.egg-info/
--rw-rw-rw-   0        0        0      885 2023-06-14 08:53:03.000000 fastgenerateapi-0.0.2/fastgenerateapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2023 2023-06-14 08:53:03.000000 fastgenerateapi-0.0.2/fastgenerateapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 08:53:03.000000 fastgenerateapi-0.0.2/fastgenerateapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-14 08:53:03.000000 fastgenerateapi-0.0.2/fastgenerateapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 08:53:03.579274 fastgenerateapi-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     3832 2023-06-14 08:51:43.000000 fastgenerateapi-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.401717 fastgenerateapi-0.0.3/
+-rw-rw-rw-   0        0        0    35821 2023-06-15 06:34:41.000000 fastgenerateapi-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      664 2023-06-15 06:54:42.401717 fastgenerateapi-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.339232 fastgenerateapi-0.0.3/fastgenerateapi/
+-rw-rw-rw-   0        0        0      826 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/__init__.py
+-rw-rw-rw-   0        0        0      496 2023-06-15 06:54:39.000000 fastgenerateapi-0.0.3/fastgenerateapi/__version__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.370474 fastgenerateapi-0.0.3/fastgenerateapi/api_view/
+-rw-rw-rw-   0        0        0       14 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/__init__.py
+-rw-rw-rw-   0        0        0     1160 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/api_view.py
+-rw-rw-rw-   0        0        0     9311 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/base_view.py
+-rw-rw-rw-   0        0        0     4192 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/create_view.py
+-rw-rw-rw-   0        0        0     3829 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/delete_tree_view.py
+-rw-rw-rw-   0        0        0     3225 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/delete_view.py
+-rw-rw-rw-   0        0        0     7585 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/get_all_view.py
+-rw-rw-rw-   0        0        0     3077 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/get_one_view.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.370474 fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/
+-rw-rw-rw-   0        0        0        0 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/__init__.py
+-rw-rw-rw-   0        0        0     3529 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/base_mixin.py
+-rw-rw-rw-   0        0        0     3826 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/dbmodel_mixin.py
+-rw-rw-rw-   0        0        0      266 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/get_mixin.py
+-rw-rw-rw-   0        0        0     2221 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/response_mixin.py
+-rw-rw-rw-   0        0        0      317 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/save_mixin.py
+-rw-rw-rw-   0        0        0    13029 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/tool_mixin.py
+-rw-rw-rw-   0        0        0     3279 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/switch_view.py
+-rw-rw-rw-   0        0        0     4152 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/update_view.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.370474 fastgenerateapi-0.0.3/fastgenerateapi/controller/
+-rw-rw-rw-   0        0        0      316 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/controller/__init__.py
+-rw-rw-rw-   0        0        0     3391 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/controller/filter_controller.py
+-rw-rw-rw-   0        0        0     2385 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/controller/router_controller.py
+-rw-rw-rw-   0        0        0     2298 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/controller/rpc_controller.py
+-rw-rw-rw-   0        0        0      873 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/controller/search_controller.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.386096 fastgenerateapi-0.0.3/fastgenerateapi/data_type/
+-rw-rw-rw-   0        0        0        0 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/data_type/__init__.py
+-rw-rw-rw-   0        0        0      727 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/data_type/data_type.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.386096 fastgenerateapi-0.0.3/fastgenerateapi/deps/
+-rw-rw-rw-   0        0        0      160 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/deps/__init__.py
+-rw-rw-rw-   0        0        0     1581 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/deps/filter_params_deps.py
+-rw-rw-rw-   0        0        0     3171 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/deps/paginator_deps.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.386096 fastgenerateapi-0.0.3/fastgenerateapi/pydantic_utils/
+-rw-rw-rw-   0        0        0        0 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/pydantic_utils/__init__.py
+-rw-rw-rw-   0        0        0      648 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/pydantic_utils/base_model.py
+-rw-rw-rw-   0        0        0     2814 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/pydantic_utils/json_encoders.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.386096 fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/
+-rw-rw-rw-   0        0        0      472 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/__init__.py
+-rw-rw-rw-   0        0        0     4305 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/common_function.py
+-rw-rw-rw-   0        0        0     1856 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/create_schema_factory.py
+-rw-rw-rw-   0        0        0     3102 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/get_all_schema_factory.py
+-rw-rw-rw-   0        0        0     1763 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/get_one_schema_factory.py
+-rw-rw-rw-   0        0        0     1251 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/response_factory.py
+-rw-rw-rw-   0        0        0     1856 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/update_schema_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.401717 fastgenerateapi-0.0.3/fastgenerateapi/settings/
+-rw-rw-rw-   0        0        0        6 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/settings/__init__.py
+-rw-rw-rw-   0        0        0      232 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/settings/register_settings.py
+-rw-rw-rw-   0        0        0     3083 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/settings/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.401717 fastgenerateapi-0.0.3/fastgenerateapi/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      121 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/utils/exception.py
+-rw-rw-rw-   0        0        0      670 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/utils/parse_str.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.354853 fastgenerateapi-0.0.3/fastgenerateapi.egg-info/
+-rw-rw-rw-   0        0        0      664 2023-06-15 06:54:42.000000 fastgenerateapi-0.0.3/fastgenerateapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2106 2023-06-15 06:54:42.000000 fastgenerateapi-0.0.3/fastgenerateapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 06:54:42.000000 fastgenerateapi-0.0.3/fastgenerateapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-15 06:54:42.000000 fastgenerateapi-0.0.3/fastgenerateapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 06:54:42.401717 fastgenerateapi-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2023-06-15 06:34:41.000000 fastgenerateapi-0.0.3/setup.py
```

### Comparing `fastgenerateapi-0.0.2/LICENSE` & `fastgenerateapi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.2/PKG-INFO` & `fastgenerateapi-0.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,18 @@
 Metadata-Version: 2.1
 Name: fastgenerateapi
-Version: 0.0.2
+Version: 0.0.3
 Summary: FastAPIView Class View
 Author: ShiLiang
 Author-email: 2509144896@qq.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-
-[联系作者](Wait To be improved)
-
-This is a simple example package. You can use
-
-[Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
-
-to write your content.
-
-
-from fastapiview import APIView
-
-
-
-
+FastAPIView Class View
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/__init__.py` & `fastgenerateapi-0.0.3/fastgenerateapi/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,12 +6,13 @@
 #  `88888P' dP    dP dP   dP dP `88888P8 dP    dP `8888P88
 #                                                      .88
 #                                                  d8888P
 
 
 from fastgenerateapi.api_view.api_view import APIView, CreateView, GetOneView, GetAllView, UpdateView, DeleteView, \
     SwitchView
+from fastgenerateapi.api_view.delete_tree_view import DeleteTreeView
 from fastgenerateapi.api_view.base_view import BaseView
 from fastgenerateapi.settings.settings import SettingsModel
 from fastgenerateapi.settings.register_settings import register_settings
```

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/api_view/api_view.py` & `fastgenerateapi-0.0.3/fastgenerateapi/api_view/api_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/api_view/base_view.py` & `fastgenerateapi-0.0.3/fastgenerateapi/api_view/base_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 from fastapi import params
 from pydantic import create_model
 from starlette.requests import Request
 from tortoise import Model
 
 from fastgenerateapi.api_view.mixin.base_mixin import BaseMixin
+from fastgenerateapi.api_view.mixin.dbmodel_mixin import DBModelMixin
 from fastgenerateapi.api_view.mixin.response_mixin import ResponseMixin
 from fastgenerateapi.api_view.mixin.tool_mixin import ToolMixin
 from fastgenerateapi.controller import RouterController
-from fastgenerateapi.data_type.data_type import RESPONSE_WRAPPER
 from fastgenerateapi.pydantic_utils.base_model import BaseModel
 from fastgenerateapi.settings.register_settings import settings
 from fastgenerateapi.utils.exception import NOT_FOUND
 
 
-class BaseView(BaseMixin, ResponseMixin, ToolMixin):
+class BaseView(BaseMixin, ResponseMixin, ToolMixin, DBModelMixin):
 
     prefix: Optional[str] = None  # 路由追加后缀
     model_class: Optional[Type[Model]] = None  # 数据库模型
     prefetch_related_fields: Union[None, dict] = None
     schema: Optional[Type[BaseModel]] = None  # 返回序列化
     dependencies: Optional[Sequence[params.Depends]] = None
     tags: Optional[List[str]] = None  # swagger标签
@@ -43,18 +43,21 @@
         #("函数名", "默认POST方法", "路由[默认_替换为-]", "[依赖函数]", "swagger备注,默认函数名")
         ("update_avatar", "PATCH", "update-avatar", [依赖函数], "修改头像"),
     ]
     """
 
     def __init__(self, **kwargs):
         self.prefetch_related_fields: dict = self.prefetch_related_fields or {}
+        try:
+            prefix = self.prefix or self.get_model_strike_name(self.model_class)
+            prefix = "/" + prefix.strip("/")
+        except:
+            prefix = ""
 
-        prefix = str(self.prefix or self.model_class.__name__).lower()
-        prefix = "/" + prefix.strip("/")
-        tags = self.tags or [prefix.strip("/").capitalize()]
+        tags = self.tags or [self.get_model_description(self.model_class) or prefix.strip("/").capitalize()]
         super().__init__(prefix=prefix, tags=tags, dependencies=self.dependencies, **kwargs)
 
         self.router_summary = RouterController(self, self._get_cls_func())
         for router in self.router_summary.router_data:
             self._add_api_route(
                 f"/{router.prefix}",
                 getattr(self, router.func_name),
@@ -125,22 +128,22 @@
 
     async def check_unique_field(
             self,
             request_data: BaseModel,  # 创建或修改的参数数据
             model_class: Type[Model],       # 数据库模型
             model: Union[Model, None] = None
     ):
-        check_unique_fields = self._get_unique_fields(model_class=model_class)
-        check_unique_together_fields = self._get_unique_together_fields()
+        check_unique_fields = self._get_unique_fields(model_class) + self._get_foreign_key_fields(model_class)
+        check_unique_together_fields = self._get_unique_together_fields(model_class)
         for unique_field in check_unique_fields:
             if hasattr(request_data, unique_field):
                 if model and getattr(request_data, unique_field) == getattr(model, unique_field):
                     continue
                 if await model_class.filter(**{unique_field: getattr(request_data, unique_field)}).first():
-                    self.fail(message=f"{self._get_field_description(model_class, unique_field)}已存在相同值：{getattr(request_data, unique_field)}")
+                    self.fail(message=f"{self.get_field_description(model_class, unique_field)}已存在相同值：{getattr(request_data, unique_field)}")
         for unique_together_fields in check_unique_together_fields:
             filter_fields = {}
             is_equal = True
             description_fields = []
             for unique_together_field in unique_together_fields:
                 if model:
                     if hasattr(request_data, unique_together_field):
@@ -156,15 +159,15 @@
                         description_fields.append(unique_together_field)
                         filter_fields[unique_together_field] = getattr(request_data, unique_together_field)
             if is_equal:
                 continue
 
             if await model_class.filter(**filter_fields).first():
                 self.fail(
-                    message=f"{self._get_field_description(model_class, description_fields)}已存在相同值：{[filter_fields.get(field) for field in description_fields]}"
+                    message=f"{self.get_field_description(model_class, description_fields)}已存在相同值：{[filter_fields.get(field) for field in description_fields]}"
                 )
 
     # @staticmethod
     # async def setattr_model_rpc(
     #         rpc_class,
     #         model: Model,
     #         rpc_param: Union[Dict[str, Dict[str, List[Union[str, tuple]]]], Type[RPCParam]],
```

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/api_view/create_view.py` & `fastgenerateapi-0.0.3/fastgenerateapi/api_view/create_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     @atomic()
     async def create(self, request_data, *args, **kwargs):
         try:
             model = await self.set_create_fields(request_data=request_data, *args, **kwargs)
         except ValueError as e:
             error_field = str(e).split(" ")[0]
             if getattr(request_data, error_field):
-                raise self.fail(msg=f"{self.model_class._meta.fields_map.get(error_field).description}格式不正确")
-            raise self.fail(msg=f"{self.model_class._meta.fields_map.get(error_field).description}不能为空")
+                raise self.fail(msg=f"{self.get_field_description(self.model_class, error_field)}格式不正确")
+            raise self.fail(msg=f"{self.get_field_description(self.model_class, error_field)}不能为空")
 
         model = await self.set_save_model(model=model, request_data=request_data, *args, **kwargs)
 
         model = await self.set_create_model(model=model, request_data=request_data, *args, **kwargs)
 
         await self.check_unique_field(request_data, model_class=self.model_class)
```

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/api_view/delete_view.py` & `fastgenerateapi-0.0.3/fastgenerateapi/api_view/delete_view.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import time
 from typing import Optional, Type, Any, Union
 
 from fastapi.types import DecoratedCallable
 from starlette.requests import Request
 from starlette.responses import JSONResponse
-from tortoise import Model
 from tortoise.transactions import atomic
 
 from fastgenerateapi.api_view.base_view import BaseView
 from fastgenerateapi.data_type.data_type import CALLABLE, DEPENDENCIES
 from fastgenerateapi.pydantic_utils.base_model import BaseModel, IDList
 from fastgenerateapi.schemas_factory import response_factory
 from fastgenerateapi.settings.register_settings import settings
@@ -23,29 +22,31 @@
     delete_schema: 删除请求模型
     """
 
     @atomic()
     async def destroy(self, request_data, request, *args, **kwargs):
         queryset = await self.get_del_queryset(request_data=request_data, request=request, *args, **kwargs)
 
-        if self.check_unique_fields:
+        if unique_fields := self._get_unique_fields(self.model_class):
             for model in await queryset:
                 model.is_active = False
-                for field in self.check_unique_fields:
+                for field in unique_fields:
                     try:
                         setattr(model, field, getattr(model, field) + f"__{int(time.time() * 1000)}")
                     except Exception as e:
                         setattr(model, field, getattr(model, field) + f"__{int(time.time() * 1000)}")
                 await model.save()
         else:
             await queryset.update(is_active=False)
         return
 
     async def get_del_queryset(self, request_data, *args, **kwargs):
-        queryset = self.model_class.filter(id__in=request_data.id_list)
+        queryset = self.model_class.filter(
+            eval(f"Q({settings.app_settings.WHETHER_DELETE_FIELD}='{settings.app_settings.ACTIVE_DEFAULT_VALUE}')"))
+        queryset = queryset.filter(id__in=request_data.id_list)
         return queryset
 
     def _delete_decorator(self, *args: Any, **kwargs: Any) -> DecoratedCallable:
         async def route(
                 request_data: self.delete_schema,  # type: ignore
                 request: Request,
         ) -> JSONResponse:
```

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/api_view/get_all_view.py` & `fastgenerateapi-0.0.3/fastgenerateapi/api_view/get_all_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/api_view/get_one_view.py` & `fastgenerateapi-0.0.3/fastgenerateapi/api_view/get_one_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/api_view/mixin/response_mixin.py` & `fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/response_mixin.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/api_view/mixin/tool_mixin.py` & `fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/tool_mixin.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/api_view/switch_view.py` & `fastgenerateapi-0.0.3/fastgenerateapi/api_view/switch_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/api_view/update_view.py` & `fastgenerateapi-0.0.3/fastgenerateapi/api_view/update_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
         model = await self.set_update_model(model=model, request_data=request_data, *args, **kwargs)
 
         await model.update_from_dict(request_data.dict(exclude_none=True)).save()
 
         await self.setattr_model(model, prefetch_related_fields=self.prefetch_related_fields, *args, **kwargs)
 
-        await self.setattr_model_rpc(self.rpc_class, model, self.rpc_param)
+        # await self.setattr_model_rpc(self.rpc_class, model, self.rpc_param)
 
         return await self.schema.from_tortoise_orm(model)
 
     @staticmethod
     async def set_update_fields(request_data, *args, **kwargs):
         """
         修改属性: request_data.user_id = current_user.id
```

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/controller/filter_controller.py` & `fastgenerateapi-0.0.3/fastgenerateapi/controller/filter_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/controller/router_controller.py` & `fastgenerateapi-0.0.3/fastgenerateapi/controller/router_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/controller/rpc_controller.py` & `fastgenerateapi-0.0.3/fastgenerateapi/controller/rpc_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/controller/search_controller.py` & `fastgenerateapi-0.0.3/fastgenerateapi/controller/search_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/data_type/data_type.py` & `fastgenerateapi-0.0.3/fastgenerateapi/data_type/data_type.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/deps/filter_params_deps.py` & `fastgenerateapi-0.0.3/fastgenerateapi/deps/filter_params_deps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Type, Union, Any
 
 from fastapi import Query, Depends
 from pydantic import create_model
 from pydantic.fields import FieldInfo
 from tortoise import Model
 
-from fastgenerateapi.api_view.mixin.base_mixin import BaseMixin
+from fastgenerateapi.api_view.mixin.dbmodel_mixin import DBModelMixin
 from fastgenerateapi.controller.filter_controller import BaseFilter
 from fastgenerateapi.pydantic_utils.base_model import BaseModel, QueryConfig
 
 
 def filter_params_deps(model_class: Type[Model], fields: list[str, tuple[str, Type], BaseFilter] = None):
     """
         生成filter依赖
@@ -24,15 +24,15 @@
 
         model_fields.update({
             f: (
                 Union[t, str],
                 FieldInfo(
                     title=f"{f}",
                     default=Query(""),
-                    description=f"{BaseMixin._get_field_description(model_class, field_info.model_field)}"
+                    description=f"{DBModelMixin.get_field_description(model_class, field_info.model_field)}"
                 ))
         })
 
     filter_params_model: Type[BaseModel] = create_model(__model_name="CommonFilterParams", **model_fields, __config__=QueryConfig)
 
     def filter_query(filter_params: filter_params_model = Depends(filter_params_model)) -> dict[str, Any]:
         """
```

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/deps/paginator_deps.py` & `fastgenerateapi-0.0.3/fastgenerateapi/deps/paginator_deps.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/pydantic_utils/base_model.py` & `fastgenerateapi-0.0.3/fastgenerateapi/pydantic_utils/base_model.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/pydantic_utils/json_encoders.py` & `fastgenerateapi-0.0.3/fastgenerateapi/pydantic_utils/json_encoders.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/common_function.py` & `fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/common_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Type, Optional, Union
 
 from pydantic.fields import FieldInfo
 from tortoise import Model
 
-from fastgenerateapi.api_view.mixin.base_mixin import BaseMixin
+from fastgenerateapi.api_view.mixin.dbmodel_mixin import DBModelMixin
 from fastgenerateapi.settings.register_settings import settings
 
 
 def get_field_info(value, description="") -> (Type, FieldInfo):
     if value.field_type is None:
         field_type = Optional[str]
     else:
@@ -55,15 +55,15 @@
         if not value:
             return Optional[str], FieldInfo(default=None, description=f"{field}")
         return get_field_info(value, description=description)
 
     if field_info := model_class._meta.fields_map.get(field.split("__", maxsplit=1)[0]):
         description += field_info.description or ""
 
-    model_class = BaseMixin._get_foreign_key_relation_class(model_class, field.split("__", maxsplit=1)[0])
+    model_class = DBModelMixin._get_foreign_key_relation_class(model_class, field.split("__", maxsplit=1)[0])
 
     return get_field_info_from_model_class(model_class, field.split("__", maxsplit=1)[1], description)
 
 
 def get_dict_from_pydanticmeta(model_class: Type[Model], data: Union[list, tuple, set]):
     fields_info = {}
     if not data:
```

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/create_schema_factory.py` & `fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/create_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/get_all_schema_factory.py` & `fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/get_all_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/get_one_schema_factory.py` & `fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/get_one_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/response_factory.py` & `fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/response_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/schemas_factory/update_schema_factory.py` & `fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/update_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/settings/settings.py` & `fastgenerateapi-0.0.3/fastgenerateapi/settings/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     # 路由后缀字段是否添加以及配置默认值
     ROUTER_WHETHER_ADD_SUFFIX: Optional[bool] = Field(default=True, description="增删改查路由是否添加后缀")
     ROUTER_CREATE_SUFFIX_FIELD: Optional[str] = Field(default='create', description="创建后缀字段")
     ROUTER_GET_ONE_SUFFIX_FIELD: Optional[str] = Field(default='get-one', description="获取一个后缀字段")
     ROUTER_GET_ALL_SUFFIX_FIELD: Optional[str] = Field(default='get-all', description="获取列表后缀字段")
     ROUTER_UPDATE_SUFFIX_FIELD: Optional[str] = Field(default='update', description="修改后缀字段")
     ROUTER_DELETE_SUFFIX_FIELD: Optional[str] = Field(default='delete', description="删除后缀字段")
+    ROUTER_RECURSION_DELETE_SUFFIX_FIELD: Optional[str] = Field(default='delete-tree', description="递归删除后缀字段")
 
     # 数据库字段默认值
     WHETHER_DELETE_FIELD: Optional[str] = Field(default="is_active", description="是否删除字段")
     ACTIVE_DEFAULT_VALUE: Optional[bool] = Field(default=True, description="有效的默认值值")
 
     # 返回格式字段配置默认值
     CODE_RESPONSE_FIELD: Optional[bool] = Field(default=True, description="code返回字段")
```

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi/utils/parse_str.py` & `fastgenerateapi-0.0.3/fastgenerateapi/utils/parse_str.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi.egg-info/PKG-INFO` & `fastgenerateapi-0.0.3/fastgenerateapi.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,18 @@
 Metadata-Version: 2.1
 Name: fastgenerateapi
-Version: 0.0.2
+Version: 0.0.3
 Summary: FastAPIView Class View
 Author: ShiLiang
 Author-email: 2509144896@qq.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-
-[联系作者](Wait To be improved)
-
-This is a simple example package. You can use
-
-[Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
-
-to write your content.
-
-
-from fastapiview import APIView
-
-
-
-
+FastAPIView Class View
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fastgenerateapi-0.0.2/fastgenerateapi.egg-info/SOURCES.txt` & `fastgenerateapi-0.0.3/fastgenerateapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 LICENSE
-README.md
 setup.py
 fastgenerateapi/__init__.py
 fastgenerateapi/__version__.py
 fastgenerateapi.egg-info/PKG-INFO
 fastgenerateapi.egg-info/SOURCES.txt
 fastgenerateapi.egg-info/dependency_links.txt
 fastgenerateapi.egg-info/top_level.txt
 fastgenerateapi/api_view/__init__.py
 fastgenerateapi/api_view/api_view.py
 fastgenerateapi/api_view/base_view.py
 fastgenerateapi/api_view/create_view.py
+fastgenerateapi/api_view/delete_tree_view.py
 fastgenerateapi/api_view/delete_view.py
 fastgenerateapi/api_view/get_all_view.py
 fastgenerateapi/api_view/get_one_view.py
 fastgenerateapi/api_view/switch_view.py
 fastgenerateapi/api_view/update_view.py
 fastgenerateapi/api_view/mixin/__init__.py
 fastgenerateapi/api_view/mixin/base_mixin.py
+fastgenerateapi/api_view/mixin/dbmodel_mixin.py
 fastgenerateapi/api_view/mixin/get_mixin.py
 fastgenerateapi/api_view/mixin/response_mixin.py
 fastgenerateapi/api_view/mixin/save_mixin.py
 fastgenerateapi/api_view/mixin/tool_mixin.py
 fastgenerateapi/controller/__init__.py
 fastgenerateapi/controller/filter_controller.py
 fastgenerateapi/controller/router_controller.py
```

### Comparing `fastgenerateapi-0.0.2/setup.py` & `fastgenerateapi-0.0.3/setup.py`

 * *Files identical despite different names*

