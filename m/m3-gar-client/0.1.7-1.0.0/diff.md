# Comparing `tmp/m3-gar-client-0.1.7.tar.gz` & `tmp/m3-gar-client-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3-gar-client-0.1.7.tar", last modified: Thu Jun 15 12:09:12 2023, max compression
+gzip compressed data, was "m3-gar-client-1.0.0.tar", last modified: Wed Oct 12 04:05:41 2022, max compression
```

## Comparing `m3-gar-client-0.1.7.tar` & `m3-gar-client-1.0.0.tar`

### file list

```diff
@@ -1,40 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:09:12.794577 m3-gar-client-0.1.7/
--rw-r--r--   0 root         (0) root         (0)      565 2021-10-28 11:22:58.000000 m3-gar-client-0.1.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      153 2021-10-28 11:22:58.000000 m3-gar-client-0.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3624 2023-06-15 12:09:12.793577 m3-gar-client-0.1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2869 2023-06-15 12:09:01.000000 m3-gar-client-0.1.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:09:12.785577 m3-gar-client-0.1.7/requirements/
--rw-r--r--   0 root         (0) root         (0)      584 2023-06-15 12:09:01.000000 m3-gar-client-0.1.7/requirements/_base.txt
--rw-r--r--   0 root         (0) root         (0)       13 2021-10-28 11:22:58.000000 m3-gar-client-0.1.7/requirements/prod.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 12:09:12.794577 m3-gar-client-0.1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2170 2023-06-15 12:09:01.000000 m3-gar-client-0.1.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:09:12.782577 m3-gar-client-0.1.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:09:12.786577 m3-gar-client-0.1.7/src/m3_gar_client/
--rw-r--r--   0 root         (0) root         (0)     1222 2023-06-15 12:09:01.000000 m3-gar-client-0.1.7/src/m3_gar_client/__init__.py
--rw-r--r--   0 root         (0) root         (0)      402 2023-06-15 12:09:01.000000 m3-gar-client-0.1.7/src/m3_gar_client/app_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:09:12.788577 m3-gar-client-0.1.7/src/m3_gar_client/backends/
--rw-r--r--   0 root         (0) root         (0)       70 2021-10-28 11:22:58.000000 m3-gar-client-0.1.7/src/m3_gar_client/backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4714 2023-06-15 12:09:01.000000 m3-gar-client-0.1.7/src/m3_gar_client/backends/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:09:12.789577 m3-gar-client-0.1.7/src/m3_gar_client/backends/m3_rest_gar/
--rw-r--r--   0 root         (0) root         (0)      127 2021-10-28 11:22:58.000000 m3-gar-client-0.1.7/src/m3_gar_client/backends/m3_rest_gar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:09:12.792577 m3-gar-client-0.1.7/src/m3_gar_client/backends/m3_rest_gar/proxy/
--rw-r--r--   0 root         (0) root         (0)     6880 2023-06-15 12:09:01.000000 m3-gar-client-0.1.7/src/m3_gar_client/backends/m3_rest_gar/proxy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4602 2023-06-15 12:09:01.000000 m3-gar-client-0.1.7/src/m3_gar_client/backends/m3_rest_gar/proxy/actions.py
--rw-r--r--   0 root         (0) root         (0)     9873 2023-06-15 12:09:01.000000 m3-gar-client-0.1.7/src/m3_gar_client/backends/m3_rest_gar/proxy/server.py
--rw-r--r--   0 root         (0) root         (0)    32692 2023-06-15 12:09:01.000000 m3-gar-client-0.1.7/src/m3_gar_client/backends/m3_rest_gar/proxy/utils.py
--rw-r--r--   0 root         (0) root         (0)    24929 2023-06-15 12:09:01.000000 m3-gar-client-0.1.7/src/m3_gar_client/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:09:12.782577 m3-gar-client-0.1.7/src/m3_gar_client/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:09:12.783577 m3-gar-client-0.1.7/src/m3_gar_client/static/m3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:09:12.783577 m3-gar-client-0.1.7/src/m3_gar_client/static/m3/js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:09:12.793577 m3-gar-client-0.1.7/src/m3_gar_client/static/m3/js/gar/
--rw-r--r--   0 root         (0) root         (0)    36929 2023-06-15 12:09:01.000000 m3-gar-client-0.1.7/src/m3_gar_client/static/m3/js/gar/AddressPanel.js
--rw-r--r--   0 root         (0) root         (0)     6455 2023-06-15 12:09:01.000000 m3-gar-client-0.1.7/src/m3_gar_client/static/m3/js/gar/AddressPanelPatch.js
--rw-r--r--   0 root         (0) root         (0)    27727 2023-06-15 12:09:01.000000 m3-gar-client-0.1.7/src/m3_gar_client/ui.py
--rw-r--r--   0 root         (0) root         (0)    11531 2023-06-15 12:09:01.000000 m3-gar-client-0.1.7/src/m3_gar_client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:09:12.787577 m3-gar-client-0.1.7/src/m3_gar_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3624 2023-06-15 12:09:12.000000 m3-gar-client-0.1.7/src/m3_gar_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      892 2023-06-15 12:09:12.000000 m3-gar-client-0.1.7/src/m3_gar_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-15 12:09:12.000000 m3-gar-client-0.1.7/src/m3_gar_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-06-15 12:09:12.000000 m3-gar-client-0.1.7/src/m3_gar_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-15 12:09:12.000000 m3-gar-client-0.1.7/src/m3_gar_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      448 2023-06-15 12:09:12.000000 m3-gar-client-0.1.7/version.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 04:05:41.673380 m3-gar-client-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)      565 2021-10-28 11:22:58.000000 m3-gar-client-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      153 2021-10-28 11:22:58.000000 m3-gar-client-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4910 2022-10-12 04:05:41.673380 m3-gar-client-1.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4056 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 04:05:41.660380 m3-gar-client-1.0.0/requirements/
+-rw-r--r--   0 root         (0) root         (0)      536 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/requirements/_base.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2021-10-28 11:22:58.000000 m3-gar-client-1.0.0/requirements/prod.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-10-12 04:05:41.674380 m3-gar-client-1.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2412 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 04:05:41.659380 m3-gar-client-1.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 04:05:41.661380 m3-gar-client-1.0.0/src/m3_gar_client/
+-rw-r--r--   0 root         (0) root         (0)     1163 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/m3_gar_client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      453 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/m3_gar_client/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 04:05:41.663380 m3-gar-client-1.0.0/src/m3_gar_client/backends/
+-rw-r--r--   0 root         (0) root         (0)       70 2021-10-28 11:22:58.000000 m3-gar-client-1.0.0/src/m3_gar_client/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3847 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/m3_gar_client/backends/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 04:05:41.664380 m3-gar-client-1.0.0/src/m3_gar_client/backends/m3_rest_gar/
+-rw-r--r--   0 root         (0) root         (0)      127 2021-10-28 11:22:58.000000 m3-gar-client-1.0.0/src/m3_gar_client/backends/m3_rest_gar/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3091 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/m3_gar_client/backends/m3_rest_gar/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 04:05:41.664380 m3-gar-client-1.0.0/src/m3_gar_client/backends/m3_rest_gar/proxy/
+-rw-r--r--   0 root         (0) root         (0)     2162 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/m3_gar_client/backends/m3_rest_gar/proxy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4290 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/m3_gar_client/backends/m3_rest_gar/proxy/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 04:05:41.665380 m3-gar-client-1.0.0/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/
+-rw-r--r--   0 root         (0) root         (0)     1760 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      496 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/authentication.py
+-rw-r--r--   0 root         (0) root         (0)      177 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/const.py
+-rw-r--r--   0 root         (0) root         (0)      590 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/urls.py
+-rw-r--r--   0 root         (0) root         (0)     3150 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/views.py
+-rw-r--r--   0 root         (0) root         (0)     9847 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/m3_gar_client/backends/m3_rest_gar/server.py
+-rw-r--r--   0 root         (0) root         (0)    30087 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/m3_gar_client/backends/m3_rest_gar/utils.py
+-rw-r--r--   0 root         (0) root         (0)    18063 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/m3_gar_client/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 04:05:41.658380 m3-gar-client-1.0.0/src/m3_gar_client/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 04:05:41.658380 m3-gar-client-1.0.0/src/m3_gar_client/static/m3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 04:05:41.658380 m3-gar-client-1.0.0/src/m3_gar_client/static/m3/js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 04:05:41.670380 m3-gar-client-1.0.0/src/m3_gar_client/static/m3/js/gar/
+-rw-r--r--   0 root         (0) root         (0)    36932 2022-05-18 19:58:53.000000 m3-gar-client-1.0.0/src/m3_gar_client/static/m3/js/gar/AddressPanel.js
+-rw-r--r--   0 root         (0) root         (0)     6368 2022-05-18 19:58:53.000000 m3-gar-client-1.0.0/src/m3_gar_client/static/m3/js/gar/AddressPanelPatch.js
+-rw-r--r--   0 root         (0) root         (0)    27440 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/m3_gar_client/ui.py
+-rw-r--r--   0 root         (0) root         (0)     9997 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/m3_gar_client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 04:05:41.662380 m3-gar-client-1.0.0/src/m3_gar_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4910 2022-10-12 04:05:41.000000 m3-gar-client-1.0.0/src/m3_gar_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1488 2022-10-12 04:05:41.000000 m3-gar-client-1.0.0/src/m3_gar_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2022-10-12 04:05:41.000000 m3-gar-client-1.0.0/src/m3_gar_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      193 2022-10-12 04:05:41.000000 m3-gar-client-1.0.0/src/m3_gar_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2022-10-12 04:05:41.000000 m3-gar-client-1.0.0/src/m3_gar_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 04:05:41.672380 m3-gar-client-1.0.0/src/testapp/
+-rw-r--r--   0 root         (0) root         (0)       50 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/testapp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      407 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/testapp/apps.py
+-rw-r--r--   0 root         (0) root         (0)      400 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/testapp/asgi.py
+-rwxr-xr-x   0 root         (0) root         (0)      687 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/testapp/manage.py
+-rw-r--r--   0 root         (0) root         (0)     3497 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/testapp/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 04:05:41.673380 m3-gar-client-1.0.0/src/testapp/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/testapp/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/testapp/tests/test_backend_responses.py
+-rw-r--r--   0 root         (0) root         (0)      999 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/testapp/tests/test_defaults.py
+-rw-r--r--   0 root         (0) root         (0)      766 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/testapp/urls.py
+-rw-r--r--   0 root         (0) root         (0)      400 2022-10-12 04:05:28.000000 m3-gar-client-1.0.0/src/testapp/wsgi.py
+-rw-r--r--   0 root         (0) root         (0)      450 2022-10-12 04:05:41.000000 m3-gar-client-1.0.0/version.conf
```

### Comparing `m3-gar-client-0.1.7/LICENSE` & `m3-gar-client-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `m3-gar-client-0.1.7/PKG-INFO` & `m3-gar-client-1.0.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: m3-gar-client
-Version: 0.1.7
-Summary: UI клиент для сервера ГАР m3-rest-gar
-Home-page: https://stash.bars-open.ru/projects/M3/repos/m3-gar-client
-Author: BARS Group
-Author-email: bars@bars-open.ru
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Web Environment
-Classifier: Natural Language :: Russian
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.2
-Provides-Extra: oauth2
-License-File: LICENSE
-
 Пакет ``m3-gar-client`` предоставляет панель для ввода адресов Российской Федерации с
 использованием `ГАР <https://fias.nalog.ru/>`_ (Государственного адресного реестра),
 готовую к использованию в проектах на базе платформы
 `M3 <http://m3.bars-open.ru/>`_ компании `БАРС Груп <http://bars.group>`_.
 
 Возможности
 -----------
@@ -31,25 +10,86 @@
 * Встраивание в интерфейс веб-приложений на базе ExtJS.
 * Поиск адресов в ГАР по мере ввода наименований адресных объектов (субъектов
   Федерации, населенных пунктов, улиц, зданий).
 
 Системные требования
 --------------------
 
-* `Python <http://www.python.org/>`_ 2.7
-* `Django <http://djangoproject.com/>`_ 1.4 --- 1.11
+* `Python <http://www.python.org/>`_ 3.6+
+* `Django <http://djangoproject.com/>`_ 2.2 - 4.0
 * `m3-core <https://pypi.python.org/pypi/m3-core>`_ 2.2
 * `m3-ui <https://pypi.python.org/pypi/m3-ui>`_ 2.2
 
-Установка
----------
 
-..
+Подключение в варианте M3
+-------------------------
+
+Установка:
+
+.. code-block:: bash
+
+  $ pip install m3-gar-client[m3]
+
+
+Настройка:
+
+.. code-block:: python
+
+  INSTALLED_APPS += [
+      'testapp',
+      'rest_framework',
+      'm3_gar_client',
+  ]
+
+  GAR_API_URL = 'http://gar.bars.group/gar/v1/'
+
+  GAR = dict(
+      BACKEND='m3_gar_client.backends.m3_rest_gar.proxy',  # <---
+      URL=GAR_API_URL,
+      USE_CACHE=True,
+      USE_SIMPLE_SERVER=True,
+  )
 
-  pip install m3-gar-client
+
+Подключение в варианте REST
+---------------------------
+
+Установка:
+
+.. code-block:: bash
+
+  $ pip install m3-gar-client[rest]
+
+
+Настройка:
+
+.. code-block:: python
+
+  INSTALLED_APPS += [
+      'testapp',
+      'rest_framework',
+      'm3_gar_client',
+  ]
+
+  GAR_API_URL = 'http://gar.bars.group/gar/v1/'
+
+  GAR = dict(
+      BACKEND='m3_gar_client.backends.m3_rest_gar.proxy_rest',  # <---
+      URL=GAR_API_URL,
+      USE_CACHE=True,
+      USE_SIMPLE_SERVER=True,
+      REST=dict(
+          AUTHENTICATION_CLASSES=[
+              'oidc_auth.authentication.JSONWebTokenAuthentication'
+          ],
+          PERMISSION_CLASSES=[
+              'rest_framework.permissions.IsAuthenticated'
+          ]
+      )
+  )
 
 
 Настройки
 ---------
 - ``URL`` --- URL API сервера ГАР.
 - ``TIMEOUT`` --- timeout запроса к серверу ГАР в секундах.
 - ``PAGE_LIMIT`` --- количество страниц запрашиваемых у m3-rest-gar, по умолчанию 1. При большом количестве можно заддосить ГАР
@@ -60,7 +100,8 @@
 - ``OAUTH2`` --- параметры OAuth2: необходиы если не указано использовать простой сервер
 
   - ``TOKEN_URL`` --- URL для получения токена, должен использоваться HTTPS.
   - ``CLIENT_ID`` --- id клиента - создается на стороне РЕСТ сервера
   - ``CLIENT_SECRET`` --- Секретный ключ клиента - генерируется на стороне РЕСТ сервера
   - ``USERNAME`` --- username пользователя для получения токена
   - ``PASSWORD`` --- password пользователя для получения токена
+
```

### Comparing `m3-gar-client-0.1.7/setup.py` & `m3-gar-client-1.0.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 # coding: utf-8
-from os.path import abspath
-from os.path import dirname
-from os.path import join
+from os.path import (
+    abspath,
+    dirname,
+    join
+)
 import re
 
-from pkg_resources import Requirement
-from setuptools import find_packages
-from setuptools import setup
+from pkg_resources import (
+    Requirement
+)
+from setuptools import (
+    find_packages,
+    setup
+)
 
 
 _COMMENT_RE = re.compile(r'(^|\s)+#.*$')
 
 
 def _get_requirements(file_path):
     with open(file_path, 'r') as file:
@@ -41,37 +47,46 @@
     name='m3-gar-client',
     url='https://stash.bars-open.ru/projects/M3/repos/m3-gar-client',
     license='MIT',
     author='BARS Group',
     description=u'UI клиент для сервера ГАР m3-rest-gar',
     author_email='bars@bars-open.ru',
     package_dir={'': 'src'},
-    packages=find_packages('src'),
-    install_requires=tuple(_get_requirements('requirements/prod.txt')),
+    packages=find_packages('src', exclude=('testapp', 'testapp.*',)),
     long_description=_read('README.rst'),
+    long_description_content_type='text/x-rst',
     include_package_data=True,
     classifiers=[
         'Intended Audience :: Developers',
         'Environment :: Web Environment',
         'Natural Language :: Russian',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.9',
         'Development Status :: 5 - Production/Stable',
         'Framework :: Django :: 2.2',
         'Framework :: Django :: 3.2',
     ],
+    install_requires=tuple(_get_requirements('requirements/prod.txt')),
     extras_require={
         'oauth2': (
             'oauthlib>=2,<3',
             'requests-oauthlib<1',
         ),
+        'm3': (
+            'm3-core>=2.2.16,<4',
+            'm3-ui>=2.0.8,<3'
+        ),
+        'rest': (
+            'djangorestframework',
+        )
     },
     dependency_links=(
         'http://pypi.bars-open.ru/simple/m3-builder',
     ),
     setup_requires=(
         'm3-builder>=1.2,<2',
     ),
+    python_requires='>=3.6',
     set_build_info=dirname(__file__),
 )
```

### Comparing `m3-gar-client-0.1.7/src/m3_gar_client/__init__.py` & `m3-gar-client-1.0.0/src/m3_gar_client/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 # coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
 
-from importlib import import_module
+from importlib import (
+    import_module
+)
 import abc
 
-from django.conf import settings
-from six import with_metaclass
-
+from django.conf import (
+    settings
+)
 # нужно для импорта констант отсюда в barsdoc
 from m3_gar_constants import *
-from m3_gar_client.utils import cached_property
+
+from m3_gar_client.utils import (
+    cached_property
+)
+
+
+default_app_config = f'{__package__}.apps.AppConfig'
 
 
-class Config(with_metaclass(abc.ABCMeta, object)):
+class Config(abc.ABC):
 
     """Базовый класс для конфигурации пакета."""
 
     @cached_property
     def backend(self):
         """Бэкенд для доступа к данным ГАР.
```

### Comparing `m3-gar-client-0.1.7/src/m3_gar_client/backends/base.py` & `m3-gar-client-1.0.0/src/m3_gar_client/backends/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
+from abc import (
+    ABC,
+    abstractmethod,
+    abstractproperty
+)
 
-from abc import ABCMeta
-from abc import abstractmethod
-from abc import abstractproperty
 
-from six import with_metaclass
-
-
-class BackendBase(with_metaclass(ABCMeta, object)):
+class BackendBase(ABC):
 
     """Базовый класс для бэкендов."""
 
+    def init(self):
+        """Метод инициализации бекенда и бутстреппинга пакета."""
+
     @abstractproperty
     def place_search_url(self):
         """URL для поиска населенных пунктов.
 
         :rtype: str
         """
 
@@ -112,29 +112,7 @@
         Args:
             stead_id: ID земельного участка.
             timeout: Timeout запросов к серверу ГАР в секундах.
 
         Returns:
             Объект m3_gar_client.data.House
         """
-
-    @abstractmethod
-    def find_apartment(self, number, parent_id, timeout=None):
-        """Возвращает информацию о помещении по его номеру.
-
-        Args:
-            number: Номер квартиры.
-            parent_id: ID родительского объекта.
-            timeout: Timeout запросов к серверу ГАР в секундах.
-        """
-
-    @abstractmethod
-    def get_apartment(self, apartment_id, timeout=None):
-        """Возвращает информацию о помещении по его ID в ГАР.
-
-        Args:
-            apartment_id: ID помещения.
-            timeout: Timeout запросов к серверу ГАР в секундах.
-
-        Returns:
-            Объект m3_gar_client.data.Apartment
-        """
```

### Comparing `m3-gar-client-0.1.7/src/m3_gar_client/backends/m3_rest_gar/proxy/actions.py` & `m3-gar-client-1.0.0/src/m3_gar_client/backends/m3_rest_gar/proxy/actions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 # coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
+from abc import (
+    ABCMeta,
+    abstractmethod
+)
+
+from django.http.response import (
+    JsonResponse
+)
+from m3.actions import (
+    Action,
+    ActionPack
+)
+
+from m3_gar_client.backends.m3_rest_gar.utils import (
+    PlaceLoader,
+    StreetLoader,
+    UIHouseLoader,
+    UISteadLoader
+)
+from m3_gar_client.utils import (
+    correct_keyboard_layout
+)
 
-from abc import ABCMeta
-from abc import abstractmethod
 
-from django.http.response import JsonResponse
-from m3.actions import Action
-from m3.actions import ActionPack
-from six import text_type
-from six import with_metaclass
-
-from m3_gar_client.backends.m3_rest_gar.proxy.utils import PlaceLoader
-from m3_gar_client.backends.m3_rest_gar.proxy.utils import StreetLoader
-from m3_gar_client.backends.m3_rest_gar.proxy.utils import UIHouseLoader
-from m3_gar_client.backends.m3_rest_gar.proxy.utils import UISteadLoader
-from m3_gar_client.utils import correct_keyboard_layout
-
-
-class ActionBase(with_metaclass(ABCMeta, Action)):
+class ActionBase(Action, metaclass=ABCMeta):
     """
     Базовый класс для обработчиков запросов на поиск данных в ГАР.
     """
 
     # Признак того, что необходимо корректировать пользовательский ввод
     correct_keyboard_input = True
 
     @abstractmethod
     def _get_loader(self, context):
         """Возвращает загрузчик данных.
 
-        :rtype: m3_gar_client.backends.m3_rest_gar.proxy.utils.LoaderBase
+        :rtype: m3_gar_client.backends.m3_rest_gar.utils.LoaderBase
         """
 
     def context_declaration(self):
         return {
             'filter': {
                 'type': 'unicode',
                 'default': '',
@@ -85,15 +90,15 @@
     Обработчик запросов на поиск улиц в населенном пункте.
     """
 
     url = '/search/street'
 
     def _get_loader(self, context):
         # pylint: disable=abstract-class-instantiated
-        return StreetLoader(context.filter, parent_id=text_type(context.parent))
+        return StreetLoader(context.filter, parent_id=str(context.parent))
 
 
 class HouseSearchAction(ParentMixin, ActionBase):
     """
     Обработчик запросов на поиск домов.
     """
```

### Comparing `m3-gar-client-0.1.7/src/m3_gar_client/backends/m3_rest_gar/proxy/server.py` & `m3-gar-client-1.0.0/src/m3_gar_client/backends/m3_rest_gar/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 # coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-from abc import ABCMeta
-from abc import abstractmethod
+from abc import (
+    ABC,
+    abstractmethod
+)
 import hashlib
+import http.client as http_client
 import json
 
-from django.utils.functional import SimpleLazyObject
-from requests import Session
-from six import with_metaclass
-from six.moves import http_client
-
-from m3_gar_constants import DEFAULT_CACHE_TIMEOUT
-from m3_gar_client.utils import cached_property
+from django.utils.functional import (
+    SimpleLazyObject
+)
+from m3_gar_constants import (
+    DEFAULT_CACHE_TIMEOUT
+)
+from requests import (
+    Session
+)
+
+from m3_gar_client.utils import (
+    cached_property
+)
 
 
-class ServerBase(with_metaclass(ABCMeta, object)):
+class ServerBase(ABC):
     """
     Базовый класс для серверов ГАР.
     """
 
     def __init__(self, **kwargs):
         self._base_url = kwargs['url']
         self._timeout = kwargs.get('timeout')
@@ -149,16 +155,20 @@
         self.client_id = kwargs['client_id']
         self.client_secret = kwargs['client_secret']
         self.username = kwargs['username']
         self.password = kwargs['password']
 
     @cached_property
     def _session(self):
-        from oauthlib.oauth2 import LegacyApplicationClient
-        from requests_oauthlib import OAuth2Session
+        from oauthlib.oauth2 import (
+            LegacyApplicationClient
+        )
+        from requests_oauthlib import (
+            OAuth2Session
+        )
 
         result = OAuth2Session(
             client=LegacyApplicationClient(self.client_id)
         )
         result.trust_env = True
         result.fetch_token(
             token_url=self.token_url,
@@ -212,18 +222,22 @@
           - ``CLIENT_ID``
           - ``CLIENT_SECRET``
           - ``USERNAME``
           - ``PASSWORD``
 
     :rtype: m3_gar_client.backends.m3_rest_gar.ServerBase
     """
-    from django.conf import settings
+    from django.conf import (
+        settings
+    )
 
     if settings.GAR.get('USE_CACHE', False):
-        from django.core.cache import cache
+        from django.core.cache import (
+            cache
+        )
 
         cache_timeout = settings.GAR.get(
             'CACHE_TIMEOUT', DEFAULT_CACHE_TIMEOUT)
 
         if not isinstance(cache_timeout, int):
             raise ValueError(
                 'Устанавливаемое значение для настройки CACHE_TIMEOUT должно '
```

### Comparing `m3-gar-client-0.1.7/src/m3_gar_client/backends/m3_rest_gar/proxy/utils.py` & `m3-gar-client-1.0.0/src/m3_gar_client/backends/m3_rest_gar/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,47 @@
 # coding: utf-8
 from abc import (
-    ABCMeta,
-    abstractmethod,
+    ABC,
+    abstractmethod
 )
 from itertools import (
     chain,
-    count,
-)
-
-from six import (
-    with_metaclass,
-    text_type,
-    iteritems,
-)
-from six.moves import (
-    http_client,
-    map,
-    range,
+    count
 )
+import http.client as http_client
 
 from m3_gar_constants import (
     DEFAULT_PAGE_LIMIT,
     GAR_HIERARCHY_MUN,
     GAR_LEVELS_PLACE,
-    GAR_LEVELS_STREET,
+    GAR_LEVELS_STREET
 )
 
-
-from m3_gar_client.backends.m3_rest_gar.proxy.server import (
-    server,
+from m3_gar_client.backends.m3_rest_gar.server import (
+    server
 )
 from m3_gar_client.data import (
     AddressObject,
-    Apartment,
     House,
-    ObjectMapper,
-    Stead,
+    ObjectMapper
 )
 from m3_gar_client.utils import (
-    cached_property,
+    cached_property
 )
 
 
 # -----------------------------------------------------------------------------
 # Обёртки над данными, поступающими с сервера m3-rest-gar.
 
 class AddressObjectMapper(ObjectMapper):
-    """Обертка над данными сервера m3-rest-gar об адресных объектах.
+    """
+    Обертка над данными сервера m3-rest-gar об адресных объектах.
 
-    Предназначена для использования при создании экземпляров.
+    Предназначена для использования при создании экземпляров
+    :class:`m3_gar_client.data.AddressObject`.
     """
 
     fields_map = {
         'id': 'id',
         'guid': 'objectguid',
         'obj_id': 'objectid',
         'previous_id': 'previd',
@@ -85,15 +74,16 @@
 
     assert set(fields_map) == set(AddressObject.fields)
 
 
 class HouseMapper(ObjectMapper):
     """Обертка над данными сервера m3-rest-gar об адресных объектах.
 
-    Предназначена для использования при создании экземпляров.
+    Предназначена для использования при создании экземпляров
+    :class:`m3_gar_client.data.House`.
     """
 
     fields_map = {
         'id': 'id',
         'guid': 'objectguid',
         'obj_id': 'objectid',
         'ifns_fl_code': 'params__IFNSFL__value',
@@ -110,29 +100,27 @@
         'date_of_creation': 'startdate',
         'date_of_end': 'enddate',
         'region_code': 'region_code',
         'adm_parent_obj_id': 'hierarchy__adm__parentobjid__objectid',
         'adm_parent_guid': 'hierarchy__adm__parentobjid__objectguid',
         'mun_parent_obj_id': 'hierarchy__mun__parentobjid__objectid',
         'mun_parent_guid': 'hierarchy__mun__parentobjid__objectguid',
-        'level': 'hierarchy__mun__objectid__levelid',
         'number': 'number',
         'house_type': 'housetype__shortname',
-        'house_type_full': 'housetype__name',
         'building_type': 'addtype1__shortname',
-        'building_type_full': 'addtype1__name',
         'structure_type': 'addtype2__shortname',
-        'structure_type_full': 'addtype2__name',
     }
 
     assert set(fields_map) == set(House.fields)
 
 
 class SteadMapper(ObjectMapper):
-    """Обертка над данными сервера m3-rest-gar об адресных объектах."""
+    """
+    Обертка над данными сервера m3-rest-gar об адресных объектах.
+    """
 
     fields_map = {
         'id': 'id',
         'guid': 'objectguid',
         'obj_id': 'objectid',
         'ifns_fl_code': 'params__IFNSFL__value',
         'ifns_fl_territorial_district_code': 'params__territorialifnsflcode__value',
@@ -146,40 +134,21 @@
         'date_of_creation': 'startdate',
         'date_of_end': 'enddate',
         'region_code': 'region_code',
         'adm_parent_obj_id': 'hierarchy__adm__parentobjid__objectid',
         'adm_parent_guid': 'hierarchy__adm__parentobjid__objectguid',
         'mun_parent_obj_id': 'hierarchy__mun__parentobjid__objectid',
         'mun_parent_guid': 'hierarchy__mun__parentobjid__objectguid',
-        'level': 'hierarchy__mun__objectid__levelid',
         'number': 'number',
     }
 
 
-class ApartmentMapper(ObjectMapper):
-    """Обертка над данными сервера m3-rest-gar о помещениях."""
-
-    fields_map = {
-        'id': 'id',
-        'guid': 'objectguid',
-        'obj_id': 'objectid',
-        'number': 'number',
-        'apart_type_full': 'aparttype__name',
-        'apart_type': 'aparttype__shortname',
-        'adm_parent_obj_id': 'hierarchy__adm__parentobjid__objectid',
-        'adm_parent_guid': 'hierarchy__adm__parentobjid__objectguid',
-        'mun_parent_obj_id': 'hierarchy__mun__parentobjid__objectid',
-        'mun_parent_guid': 'hierarchy__mun__parentobjid__objectguid',
-        'level': 'hierarchy__mun__objectid__levelid',
-    }
-
-
 class UIAddressObjectMapper(ObjectMapper):
-    """Обертка над данными сервера m3-rest-gar об адресных объектах.
-
+    """
+    Обертка над данными сервера m3-rest-gar об адресных объектах.
     Предназначена для использования в UI.
     """
 
     fields_map = {
         'objectId': 'objectguid',
         'level': 'level',
         'shortName': 'typename',
@@ -188,16 +157,16 @@
         'postalCode': 'params__PostIndex__value',
         'fullName': 'hierarchy__mun__name_with_parents',
         'hasChildren': 'hierarchy__mun__has_children',
     }
 
 
 class UIHouseMapper(ObjectMapper):
-    """Обертка над данными сервера m3-rest-gar о зданиях.
-
+    """
+    Обертка над данными сервера m3-rest-gar о зданиях.
     Предназначена для использования в UI.
     """
 
     fields_map = {
         'objectId': 'objectguid',
         'houseNumber': 'housenum',
         'buildingNumber': 'addnum1',
@@ -206,62 +175,74 @@
         'houseType': 'housetype__shortname',
         'buildingType': 'addtype1__shortname',
         'structureType': 'addtype2__shortname',
     }
 
 
 class UISteadMapper(ObjectMapper):
-    """Обертка над данными сервера m3-rest-gar о земельных участках.
-
+    """
+    Обертка над данными сервера m3-rest-gar о земельных участках.
     Предназначена для использования в UI.
     """
 
     fields_map = {
         'objectId': 'objectguid',
         'steadNumber': 'number',
         'postalCode': 'params__PostIndex__value',
     }
 
 # -----------------------------------------------------------------------------
 # Загрузчики данных с сервера m3-rest-gar.
 
 
-class LoaderBase(with_metaclass(ABCMeta, object)):
-    """Базовый класс для загрузчиков объектов ГАР.
-
-    Attributes:
-        filter_string: Строка для фильтрации объектов.
-        timeout: Timeout запросов к серверу ГАР в секундах.
+class LoaderBase(ABC):
+    """
+    Базовый класс для загрузчиков объектов ГАР.
     """
 
     def __init__(self, filter_string, **kwargs):
+        """Инициализация экземпляра класса.
+
+        :param unicode filter_string: Строка для фильтрации объектов.
+        :param float timeout: Timeout запросов к серверу ГАР в секундах.
+        """
         self.filter_string = filter_string
         self.timeout = kwargs.get('timeout')
         self.exact = kwargs.get('exact', False)
 
     @property
     @abstractmethod
     def _path(self):
-        """Путь к ресурсу API сервера ГАР."""
+        """Путь к ресурсу API сервера ГАР.
+
+        :rtype: str
+        """
 
     @cached_property
     def _fields(self):
-        """Имена полей, подлежащих загрузке."""
+        """Имена полей, подлежащих загрузке.
 
+        :rtype: tuple
+        """
         return list(self._mapper_class.fields_map.keys())
 
     @property
     @abstractmethod
     def _mapper_class(self):
-        """Класс, преобразующий имена полей."""
+        """Класс, преобразующий имена полей.
+
+        ::rtype: m3_gar_client.data.ObjectMapper
+        """
 
     @property
     def _filter_param(self):
-        """Query-параметр для фильтрации."""
+        """Query-параметр для фильтрации.
 
+        :rtype: str
+        """
         return 'name'
 
     def _load_page(self, params, page):
         params = params.copy()
         params['page'] = page
 
         drf_response = server.get(self._path, params, timeout=self.timeout)
@@ -271,58 +252,66 @@
             result = None
 
         return result
 
     def _process_object_data(self, drf_object_data):
         """Выполняет дополнительную обработку данных объекта ГАР.
 
-        Args:
-            drf_object_data: Данные объекта ГАР, полученные с сервера m3-rest-gar.
+        :param dict drf_object_data: Данные объекта ГАР, полученные с сервера m3-rest-gar.
         """
         return map_object_data(self._mapper_class, drf_object_data)
 
     def _build_result(self, object_data):
         """Формирует данные результирующего объекта ГАР.
 
         Полученные данные включаются в результат загрузки.
 
-        Args:
-            object_data: Данные объекта, полученные с сервера ГАР и прошедшие обработку в методе
-                         ``_process_object_data``.
-        """
+        :param dict object_data: Данные объекта, полученные с сервера ГАР и
+            прошедшие обработку в методе ``_process_object_data``.
 
-        return {field: object_data[field] for field in self._fields}
+        :rtype: dict
+        """
+        return {
+            field: object_data[field]
+            for field in self._fields
+        }
 
     @abstractmethod
     def _filter(self, object_data):
-        """Возвращает True, если объект ГАР должен попасть в загрузку."""
+        """Возвращает True, если объект ГАР должен попасть в загрузку.
+
+        :rtype: bool
+        """
 
     def _get_params(self):
-        """Возвращает параметры запроса к серверу ГАР."""
+        """Возвращает параметры запроса к серверу ГАР.
 
+        :rtype: dict
+        """
         filter_param = self._filter_param
 
         if self.exact:
             filter_param += '__exact'
 
         result = {
             filter_param: self.filter_string,
         }
 
         return result
 
     def load_raw(self, page=None):
         """Возвращает данные адресных объектов в исходном виде.
 
-        Args:
-            page: Номера страницы для загрузки данных. ``None`` указывает на необходимость загрузки всех страниц.
-        """
+        :param int page: Номера страницы для загрузки данных. Значение ``None``
+            указывает на необходимость загрузки всех страниц.
 
+        :rtype: generator
+        """
         from django.conf import (
-            settings,
+            settings
         )
 
         # Значение PAGE_LIMIT по умолчанию 5. С большим PAGE_LIMIT можно заддосить ГАР
         page_limit = settings.GAR.get('PAGE_LIMIT', DEFAULT_PAGE_LIMIT)
 
         if page is None:
             pages = count(start=1)
@@ -343,69 +332,70 @@
                     break
             else:
                 break
 
     def load_results(self, page=None):
         """Возвращает данные в соответствии с параметрами загрузчика.
 
-        Args:
-            page: Номера страницы для загрузки данных. ``None`` указывает на необходимость загрузки всех страниц.
-        """
+        :param int page: Номера страницы для загрузки данных. Значение ``None``
+            указывает на необходимость загрузки всех страниц.
 
+        :rtype: map
+        """
         return map(self._build_result, self.load_raw(page))
 
     @abstractmethod
     def _sort_key(self, object_data):
         """Возвращает значение ключа для сортировки результатов загрузки.
 
-        Args:
-            object_data: Данные загруженного объекта ГАР.
+        :param dict object_data: Данные загруженного объекта ГАР.
         """
 
     def _process_result(self, data):
         """Обработка полученных после загрузки данных.
 
-        Args:
-            data: Кортеж словарей с данными загруженных объектов ГАР.
+        :param tuple data: Кортеж словарей с данными загруженных объектов ГАР.
         """
-
         return sorted(data, key=self._sort_key)
 
     def load(self, page=None):
         """Загружает данные с сервера ГАР.
 
-        Args:
-            page: Номера страницы для загрузки данных. ``None`` указывает на необходимость загрузки всех страниц.
-        """
+        :param int page: Номера страницы для загрузки данных. Значение ``None``
+            указывает на необходимость загрузки всех страниц.
 
+        :rtype: collections.Iterable
+        """
         data = tuple(self.load_results(page))
         result = self._process_result(data)
 
         return result
 
 
 class ParentFilterMixin(object):
-    """Миксин для загрузчиков, которые используют id родительского объекта в запросах к серверу ГАР."""
+    """
+    Миксин для загрузчиков, которые используют id родительского объекта в запросах к серверу ГАР
+    """
 
     @property
     @abstractmethod
     def _default_hierarchy(self):
-        """Вид иерархии, используемый по умолчанию."""
+        """Вид иерархии, используемый по умолчанию"""
 
     def __init__(self, *args, **kwargs):
         super(ParentFilterMixin, self).__init__(*args, **kwargs)
 
         self._hierarchy = kwargs.get('hierarchy') or self._default_hierarchy
         self._parent_id = kwargs.get('parent_id')
 
     def _get_params(self):
         result = super(ParentFilterMixin, self)._get_params()
 
         if self._parent_id:
-            result['parent'] = text_type('{}:{}'.format(self._hierarchy, self._parent_id))
+            result['parent'] = str('{}:{}'.format(self._hierarchy, self._parent_id))
 
         return result
 
 
 class AddressObjectLoaderBase(ParentFilterMixin, LoaderBase):
     """Базовый класс для загрузчиков адресных объектов ГАР.
 
@@ -425,19 +415,24 @@
     @property
     def _path(self):
         return '/addrobj/'
 
     @property
     @abstractmethod
     def _levels(self):
-        """Уровни адресных объектов, для которых нужно искать данные в ГАР."""
+        """Уровни адресных объектов, для которых нужно искать данные в ГАР.
+
+        :rtype: tuple
+        """
 
     def _get_params(self):
-        """Возвращает параметры запроса к серверу ГАР."""
+        """Возвращает параметры запроса к серверу ГАР.
 
+        :rtype: dict
+        """
         result = super(AddressObjectLoaderBase, self)._get_params()
 
         if self._levels:
             result['level'] = ','.join(map(str, self._levels))
 
         return result
 
@@ -459,19 +454,17 @@
     _levels = None
 
     _mapper_class = AddressObjectMapper
 
     def __init__(self, filter_string, levels=None, typenames=None, **kwargs):
         """Инициализация экземпляра класса.
 
-        Args:
-            filter_string: Строка для фильтрации объектов.
-            levels: Уровни адресных объектов.
+        :param unicode filter_string: Строка для фильтрации объектов.
+        :param levels: Уровни адресных объектов.
         """
-
         super(AddressObjectLoader, self).__init__(filter_string, **kwargs)
 
         self._levels = levels
         self._typenames = typenames
 
     def _get_params(self):
         result = super(AddressObjectLoader, self)._get_params()
@@ -479,29 +472,35 @@
         if self._typenames:
             result['typename'] = ','.join(map(str, self._typenames))
 
         return result
 
 
 class PlaceLoader(AddressObjectLoaderBase):
-    """Загрузчик сведений о населенных пунктах."""
+    """
+    Загрузчик сведений о населенных пунктах
+    """
 
     _levels = GAR_LEVELS_PLACE
 
     _mapper_class = UIAddressObjectMapper
 
     @property
     def _filter_param(self):
-        """Query-параметр для фильтрации."""
+        """Query-параметр для фильтрации.
 
+        :rtype: str
+        """
         return 'name_with_parents'
 
     def _get_params(self):
-        """Возвращает параметры запроса к серверу ГАР."""
+        """Возвращает параметры запроса к серверу ГАР.
 
+        :rtype: dict
+        """
         filter_param = self._filter_param
 
         if self.exact:
             filter_param += '__exact'
 
         result = {
             filter_param: f'{self._default_hierarchy}:{self.filter_string}',
@@ -513,29 +512,35 @@
         return bool(object_data['fullName'])
 
     def _sort_key(self, object_data):
         return object_data['level'], object_data['fullName'] or ''
 
 
 class StreetLoader(AddressObjectLoaderBase):
-    """Загрузчик сведений об улицах."""
+    """
+    Загрузчик сведений об улицах.
+    """
 
     _levels = GAR_LEVELS_STREET
 
     _mapper_class = UIAddressObjectMapper
 
     @property
     def _filter_param(self):
-        """Query-параметр для фильтрации."""
+        """Query-параметр для фильтрации.
 
+        :rtype: str
+        """
         return 'name_with_typename'
 
 
 class HouseLoader(ParentFilterMixin, LoaderBase):
-    """Загрузчик сведений о зданиях."""
+    """
+    Загрузчик сведений о зданиях.
+    """
 
     _default_hierarchy = GAR_HIERARCHY_MUN
 
     _mapper_class = HouseMapper
 
     @property
     def _path(self):
@@ -551,86 +556,52 @@
     def _sort_key(self, object_data):
         return object_data['house_number'] or ''
 
     @staticmethod
     def _split_number(number):
         """Разделяет номер на целочисленную и буквенную части.
 
-        Args:
-            number: Номер дома/корпуса/строения.
-        """
+        :param unicode number: Номер дома/корпуса/строения.
 
+        :rtype: tuple
+        """
         int_part = ''.join(ch for ch in number if ch.isdigit())
         str_part = number[len(int_part):]
 
         return int(int_part) if int_part else -1, str_part
 
 
 class SteadLoader(ParentFilterMixin, LoaderBase):
-    """Загрузчик сведений о земельных участках."""
+    """
+    Загрузчик сведений о земельных участках.
+    """
 
     _default_hierarchy = GAR_HIERARCHY_MUN
 
-    _mapper_class = SteadMapper
-
     @property
     def _path(self):
         return '/steads/'
 
     @property
     def _filter_param(self):
         return 'number'
 
     def _filter(self, object_data):
         return True
 
     def _sort_key(self, object_data):
-        return object_data.get('stead_number', object_data.get('number')) or ''
+        return object_data['stead_number'] or ''
 
     @staticmethod
     def _split_number(number):
         """Разделяет номер на целочисленную и буквенную части.
 
-        Args:
-            number: Номер земельного участка.
-        """
-
-        int_part = ''.join(ch for ch in number if ch.isdigit())
-        str_part = number[len(int_part):]
-
-        return int(int_part) if int_part else -1, str_part
-
-
-class ApartmentLoader(ParentFilterMixin, LoaderBase):
-    """Загрузчик сведений о помещениях."""
-
-    _default_hierarchy = GAR_HIERARCHY_MUN
-
-    _mapper_class = ApartmentMapper
-
-    @property
-    def _path(self):
-        return '/apartments/'
-
-    @property
-    def _filter_param(self):
-        return 'number'
-
-    def _filter(self, object_data):
-        return True
-
-    def _sort_key(self, object_data):
-        return object_data['number'] or ''
-
-    @staticmethod
-    def _split_number(number):
-        """Разделяет номер на целочисленную и буквенную части.
+        :param unicode number: Номер земельного участка.
 
-        Args:
-            number: Номер земельного участка.
+        :rtype: tuple
         """
 
         int_part = ''.join(ch for ch in number if ch.isdigit())
         str_part = number[len(int_part):]
 
         return int(int_part) if int_part else -1, str_part
 
@@ -653,14 +624,16 @@
             * номер дома (если есть) в записи **начинается со строки**,
               указанной в аргументе ``filter_string``;
             * номер корпуса или строения (если номер дома отсутствует) в записи
               **начинается со строки**, указанной в аргументе
               ``filter_string``;
             * в аргументе ``filter_string`` конструктора класса было передано
               значение ``None``.
+
+        :rtype: bool
         """
         filter_string_lower = self.filter_string.lower()
 
         if self.filter_string is None:
             result = True
         else:
             house = (object_data.get('houseNumber') or '').lower()
@@ -702,14 +675,16 @@
         Запись считается соответствующей указанным при инициализации загрузчика
         параметрам поиска, если:
 
             * номер участка в записи **начинается со строки**,
               указанной в аргументе ``filter_string``;
             * в аргументе ``filter_string`` конструктора класса было передано
               значение ``None``.
+
+        :rtype: bool
         """
 
         filter_string_lower = self.filter_string.lower()
 
         if self.filter_string is None:
             result = True
         else:
@@ -721,31 +696,43 @@
     def _process_object_data(self, drf_object_data):
         stead_data = super(UISteadLoader, self)._process_object_data(drf_object_data)
 
         stead_data['steadNumber'] = stead_data['steadNumber'] or ''
 
         return stead_data
 
+
+class UIHouseOrSteadLoader:
+
+    """Фасад для загрузки домов и участков."""
+
+    def __init__(self, *args, **kwargs):
+        self._house_loader = UIHouseLoader(*args, **kwargs)
+        self._stead_loader = UISteadLoader(*args, **kwargs)
+
+    def load(self, page=None):
+        return list((
+            *self._house_loader.load(page=page),
+            *self._stead_loader.load(page=page)
+        ))
+
+
 # -----------------------------------------------------------------------------
 # Функции для создания объектов m3-gar-client на основе данных m3-rest-gar.
-
 def get_address_object(obj_id, timeout=None):
     """Возвращает адресный объект, загруженный с сервера ГАР.
 
     Если адресный объект не найден, возвращает ``None``.
 
-    Args:
-        obj_id: ObjectID/GUID адресного объекта ГАР.
-        timeout: timeout запроса к серверу ГАР в секундах.
+    :param obj_id: ObjectID/GUID адресного объекта ГАР.
+    :param float timeout: timeout запроса к серверу ГАР в секундах.
 
-    Returns:
-        Адресный объект
+    :rtype: m3_gar_client.data.AddressObject or NoneType
 
-    Exceptions:
-        requests.ConnectionError: если не удалось соединиться с сервером ГАР
+    :raises requests.ConnectionError: если не удалось соединиться с сервером ГАР
     """
     result = None
 
     if obj_id:
         response = server.get('/addrobj/{}/'.format(obj_id), timeout=timeout)
 
         if response and response.status_code == http_client.OK:
@@ -761,21 +748,21 @@
     levels=None,
     typenames=None,
     parent_id=None,
     timeout=None,
 ):
     """Возвращает адресные объекты, соответствующие параметрам поиска.
 
-    Args:
-        filter_string: Строка поиска.
-        levels: Уровни адресных объектов, среди которых нужно осуществлять поиск.
-        parent_id: ID родительского объекта.
-        timeout: Timeout запросов к серверу ГАР в секундах.
-    """
+    :param unicode filter_string: Строка поиска.
+    :param levels: Уровни адресных объектов, среди которых нужно осуществлять поиск.
+    :param parent_id: ID родительского объекта.
+    :param float timeout: Timeout запросов к серверу ГАР в секундах.
 
+    :rtype: generator
+    """
     return AddressObjectLoader(
         filter_string,
         levels=levels,
         typenames=typenames,
         parent_id=parent_id,
         timeout=timeout,
     ).load_results()
@@ -788,15 +775,14 @@
     Args:
         stead_id: ID земельного участка.
         timeout: Timeout запросов к серверу ГАР в секундах.
 
     Returns:
         Объект m3_gar_client.data.House
     """
-
     assert stead_id is not None
 
     response = server.get('/steads/{}/'.format(stead_id), timeout=timeout)
 
     if response and response.status_code == http_client.OK:
         response_data = response.json()
         mapped_data = map_object_data(SteadMapper, response_data)
@@ -806,19 +792,19 @@
 
     return result
 
 
 def get_house(house_id, timeout=None):
     """Возвращает информацию о здании по его ID в ГАР.
 
-    Args:
-        house_id: ID здания.
-        timeout: Timeout запросов к серверу ГАР в секундах.
-    """
+    :param house_id: ID здания.
+    :param float timeout: Timeout запросов к серверу ГАР в секундах.
 
+    :rtype: m3_gar_client.data.House
+    """
     assert house_id is not None
 
     response = server.get('/houses/{}/'.format(house_id), timeout=timeout)
 
     if response and response.status_code == http_client.OK:
         response_data = response.json()
         mapped_data = map_object_data(HouseMapper, response_data)
@@ -828,22 +814,22 @@
 
     return result
 
 
 def find_house(house_number='', parent_id=None, building_number=None, structure_number=None, timeout=None):
     """Возвращает информацию о здании по его номеру.
 
-    Args:
-        house_number: Номер дома.
-        parent_id: ID родительского объекта.
-        building_number: Номер корпуса.
-        structure_number: Номер строения.
-        timeout: Timeout запросов к серверу ГАР в секундах.
-    """
+    :param unicode house_number: Номер дома.
+    :param parent_id: ID родительского объекта.
+    :param unicode building_number: Номер корпуса.
+    :param unicode structure_number: Номер строения.
+    :param float timeout: Timeout запросов к серверу ГАР в секундах.
 
+    :rtype: m3_gar_client.data.House or NoneType
+    """
     houses = HouseLoader(
         house_number,
         parent_id=parent_id,
         exact=True,
         timeout=timeout,
     ).load()
 
@@ -858,119 +844,47 @@
         result = House(**houses[0])
     else:
         result = None
 
     return result
 
 
-def find_stead(number='', parent_id=None, timeout=None):
-    """Возвращает информацию об участке по его номеру.
-
-    :param unicode number: Номер участка.
-    :param parent_id: ID родительского объекта.
-    :param float timeout: Timeout запросов к серверу ГАР в секундах.
-
-    :rtype: m3_gar_client.data.Stead or NoneType
-    """
-    steads = SteadLoader(
-        number,
-        parent_id=parent_id,
-        timeout=timeout,
-    ).load()
-
-    if len(steads) == 1:
-        result = Stead(**steads[0])
-    else:
-        result = None
-
-    return result
-
-
-def get_apartment(apartment_id, timeout=None):
-    """Возвращает информацию о помещении по его ID в ГАР.
-
-    Args:
-        apartment_id: ID помещения.
-        timeout: Timeout запросов к серверу ГАР в секундах.
-    """
-    assert apartment_id is not None
-
-    response = server.get('/apartments/{}/'.format(apartment_id), timeout=timeout)
-
-    if response and response.status_code == http_client.OK:
-        response_data = response.json()
-        mapped_data = map_object_data(ApartmentMapper, response_data)
-        result = Apartment(**mapped_data)
-    else:
-        result = None
-
-    return result
-
-
-def find_apartment(number='', parent_id=None, timeout=None):
-    """Возвращает информацию о помещении по его номеру.
-
-    Args:
-        number: Номер квартиры.
-        parent_id: ID родительского объекта.
-        timeout: Timeout запросов к серверу ГАР в секундах.
-    """
-
-    apartments = ApartmentLoader(
-        number,
-        parent_id=parent_id,
-        exact=True,
-        timeout=timeout,
-    ).load()
-
-    if len(apartments) == 1:
-        result = Apartment(**apartments[0])
-    else:
-        result = None
-
-    return result
-
-
 def flatten_object_data(raw_object_data):
-    """Преобразует данные объекта ГАР к "плоскому" виду.
+    """Преобразует данные объекта ГАР к "плоскому" виду
 
-    Args:
-        raw_object_data: Необработанные данные объекта ГАР, полученные с сервера m3-rest-gar.
+    :param dict raw_object_data: Необработанные данные объекта ГАР, полученные с сервера m3-rest-gar.
     """
-
     flat_data = {}
 
-    for key, value in iteritems(raw_object_data):
+    for key, value in raw_object_data.items():
         if type(value) is dict:
-            for inner_key, inner_value in iteritems(flatten_object_data(value)):
+            for inner_key, inner_value in flatten_object_data(value).items():
                 flat_data['{}__{}'.format(key, inner_key)] = inner_value
 
         elif type(value) is list and key == 'params':
             for param_dict in value:
                 if type(param_dict) is not dict:
                     continue
 
                 code = param_dict.get('typeid', {}).get('code')
                 if code is None:
                     continue
 
-                for inner_key, inner_value in iteritems(flatten_object_data(param_dict)):
+                for inner_key, inner_value in flatten_object_data(param_dict).items():
                     flat_data['params__{}__{}'.format(code, inner_key)] = inner_value
 
         else:
             flat_data[key] = value
 
     return flat_data
 
 
 def map_object_data(mapper_class, raw_object_data):
-    """Выполняет маппинг сырых данных, полученных с сервера m3-rest-gar.
+    """Выполняет маппинг сырых данных, полученных с сервера m3-rest-gar
 
-    Args:
-        mapper_class: Класс-маппер.
-        raw_object_data: Необработанные данные объекта ГАР, полученные с сервера m3-rest-gar.
+    :param dict raw_object_data: Необработанные данные объекта ГАР, полученные с сервера m3-rest-gar.
+    :param class ObjectMapper mapper_class: класс-маппер.
     """
-
     flat_data = flatten_object_data(raw_object_data)
     mapped_data = mapper_class(flat_data)
 
     return mapped_data
```

### Comparing `m3-gar-client-0.1.7/src/m3_gar_client/static/m3/js/gar/AddressPanel.js` & `m3-gar-client-1.0.0/src/m3_gar_client/static/m3/js/gar/AddressPanel.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -353,15 +353,15 @@
             return !this.houseIDField.getValue();
         } else {
             return (
                 !this.houseNumberField.getValue() &&
                 !this.buildingNumberField.getValue() &&
                 !this.structureNumberField.getValue() &&
                 !this.houseIDField.getValue() &&
-                !this.houseTypeField.getValue()
+                !this.hasHouseTypeField.getValue()
             );
         }
     },
 
     isBuildingEmpty: function() {
         return !this.buildingNumberField.getValue();
     },
```

### Comparing `m3-gar-client-0.1.7/src/m3_gar_client/static/m3/js/gar/AddressPanelPatch.js` & `m3-gar-client-1.0.0/src/m3_gar_client/static/m3/js/gar/AddressPanelPatch.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -7,27 +7,23 @@
  * для таких населенных пунктов
  */
 
 var originalOnPlaceChange = Ext.m3.gar.AddressFields.prototype.onPlaceSelect;
 
 Ext.override(Ext.m3.gar.AddressFields, {
     onPlaceSelect: function(field, newValue, oldValue) {
-        var record;
+        var record = this.placeNameField.store.getAt(
+            this.placeNameField.selectedIndex);
 
-        if (this.streetNameField) {
-            record = this.placeNameField.store.getAt(
-                this.placeNameField.selectedIndex);
-
-            if (record && 'hasChildren' in record.json) {
-                this.streetNameField.setDisabled(!record.json['hasChildren']);
-            }
-
-            this.streetNameField.validate();
+        if (record && 'hasChildren' in record.json) {
+            this.streetNameField.setDisabled(!record.json['hasChildren']);
         }
 
+        this.streetNameField.validate();
+
         originalOnPlaceChange.apply(this, [field, newValue, oldValue]);
     },
     // функция построения полного адреса, с учетом необязательности улиц
     getFullAddress: function() {
         var addressParts = [];
 
         if (!this.isZipCodeEmpty()) {
```

### Comparing `m3-gar-client-0.1.7/src/m3_gar_client/ui.py` & `m3-gar-client-1.0.0/src/m3_gar_client/ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 # coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
 import json
 import warnings
 
-from m3_ext.ui.base import BaseExtComponent
-from m3_ext.ui.containers.containers import ExtContainer
-from m3_ext.ui.fields.simple import ExtComboBox
-from m3_ext.ui.fields.simple import ExtHiddenField
-from m3_ext.ui.fields.simple import ExtStringField
-from m3_ext.ui.fields.simple import ExtTextArea
-from m3_ext.ui.misc.store import ExtJsonStore
-
-from m3_gar_constants import UI_LEVEL_FLAT
-from m3_gar_constants import UI_LEVEL_HOUSE
-from m3_gar_constants import UI_LEVEL_PLACE
-from m3_gar_constants import UI_LEVEL_STREET
-from m3_gar_constants import UI_LEVELS
-from m3_gar_client.data import ObjectDictAdapter
-from m3_gar_client.data import ObjectMapper
-from m3_gar_client.utils import cached_property
-from m3_gar_client.utils import get_address_object
-from m3_gar_client.utils import get_house
+from m3_ext.ui.base import (
+    BaseExtComponent
+)
+from m3_ext.ui.containers.containers import (
+    ExtContainer
+)
+from m3_ext.ui.fields.simple import (
+    ExtComboBox,
+    ExtHiddenField,
+    ExtStringField,
+    ExtTextArea
+)
+from m3_ext.ui.misc.store import (
+    ExtJsonStore
+)
+from m3_gar_constants import (
+    UI_LEVEL_FLAT,
+    UI_LEVEL_HOUSE,
+    UI_LEVEL_PLACE,
+    UI_LEVEL_STREET,
+    UI_LEVELS
+)
+
+from m3_gar_client.data import (
+    ObjectDictAdapter,
+    ObjectMapper
+)
+from m3_gar_client.utils import (
+    cached_property,
+    get_address_object,
+    get_house
+)
 import m3_gar_client
 
 
 class UIAddressObjectMapper(ObjectMapper):
     """Обертка над адресным объектом для передачи данных в UI.
 
     Преобразует наименования полей адресного объекта в наименования полей в
@@ -349,15 +360,15 @@
         :rtype: m3_ext.ui.fields.simple.ExtHiddenField
         """
         return ExtHiddenField(
             type=ExtHiddenField.STRING,
             name=self._names_of_fields['house_id'],
         )
 
-#TODO BOBUH-20190 возможно, от этого стоит отказаться или, наоборот, сделать более общим
+    # TODO: BOBUH-20190 возможно, от этого стоит отказаться или, наоборот, сделать более общим
     @cached_property
     def field__house_type(self):
         """
         Поле для хранения типа дома
 
         :rtype: m3_ext.ui.fields.simple.ExtHiddenField
         """
```

### Comparing `m3-gar-client-0.1.7/src/m3_gar_client/utils.py` & `m3-gar-client-1.0.0/src/m3_gar_client/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 # coding: utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
+from importlib import (
+    reload
+)
+import sys
 
+from django.conf import (
+    settings
+)
+from django.urls.base import (
+    clear_url_caches
+)
 from m3_gar_constants import (
     GAR_HIERARCHIES,
-    GAR_HIERARCHY_MUN,
+    GAR_HIERARCHY_MUN
 )
 
 from m3_gar_client.data import (
     AddressObject,
-    Apartment,
-    House,
-    Stead,
+    House
 )
 
 
 class cached_property(property):
     """Кешируемое свойство.
 
     В отличие от :class:`django.utils.functional.cached_property`, наследуется
@@ -91,30 +97,30 @@
     :param levels: Уровни адресных объектов, среди которых нужно осуществлять поиск.
     :param parent_id: ID родительского объекта.
     :param float timeout: Timeout запросов к серверу ГАР в секундах.
 
     :rtype: generator
     """
     from m3_gar_client import (
-        config,
+        config
     )
 
     return config.backend.find_address_objects(filter_string, levels, typenames, parent_id, timeout)
 
 
 def get_address_object(obj_id, timeout=None):
     """Возвращает адресный объект ГАР по его ID.
 
     :param obj_id: ID адресного объекта ГАР.
     :param float timeout: Timeout запросов к серверу ГАР в секундах.
 
     :rtype: m3_gar_client.data.AddressObject or NoneType
     """
     from m3_gar_client import (
-        config,
+        config
     )
 
     return config.backend.get_address_object(obj_id, timeout)
 
 
 def find_house(house_number='', parent_id=None, building_number=None, structure_number=None, timeout=None):
     """Возвращает информацию о здании по его номеру.
@@ -125,15 +131,15 @@
     :param unicode structure_number: Номер строения.
     :param parent_id: ID родительского объекта.
     :param float timeout: Timeout запросов к серверу ГАР в секундах.
 
     :rtype: m3_gar_client.data.House or NoneType
     """
     from m3_gar_client import (
-        config,
+        config
     )
 
     return config.backend.find_house(house_number, parent_id, building_number, structure_number, timeout)
 
 
 def get_house(house_id, timeout=None):
     """Возвращает информацию о здании по его ID в ГАР.
@@ -146,15 +152,15 @@
 
     :param house_id: ID здания.
     :param float timeout: Timeout запросов к серверу ГАР в секундах.
 
     :rtype: m3_gar_client.data.House
     """
     from m3_gar_client import (
-        config,
+        config
     )
 
     return config.backend.get_house(house_id, timeout)
 
 
 def get_stead(stead_id, timeout=None):
     """Возвращает информацию о земельном участке по его ID в ГАР.
@@ -163,53 +169,20 @@
         stead_id: ID земельного участка.
         timeout: Timeout запросов к серверу ГАР в секундах.
 
     Returns:
         Объект m3_gar_client.data.House
     """
     from m3_gar_client import (
-        config,
+        config
     )
 
     return config.backend.get_stead(stead_id, timeout)
 
 
-def find_apartment(number='', parent_id=None, timeout=None):
-    """Возвращает информацию о помещении по его номеру.
-
-    Args:
-        number: Номер квартиры.
-        parent_id: ID родительского объекта.
-        timeout: Timeout запросов к серверу ГАР в секундах.
-    """
-
-    from m3_gar_client import (
-        config,
-    )
-
-    return config.backend.find_apartment(number, parent_id, timeout)
-
-
-def get_apartment(apartment_id, timeout=None):
-    """Возвращает информацию о помещении по его ID в ГАР.
-
-    Args:
-        apartment_id: ID помещения.
-        timeout: Timeout запросов к серверу ГАР в секундах.
-
-    Returns:
-        Объект m3_gar_client.data.Apartment
-    """
-    from m3_gar_client import (
-        config,
-    )
-
-    return config.backend.get_apartment(apartment_id, timeout)
-
-
 def get_address_object_name(address_object):
     """Возвращает наименование объекта с кратким наименованием его типа.
 
     Примеры:
 
       * Забайкальский край
       * ул. Ленина
@@ -221,15 +194,15 @@
     """
     if address_object.guid == 'd66e5325-3a25-4d29-ba86-4ca351d9704b':
         # Ханты-Мансийский Автономный округ - Югра
         result = address_object.formal_name
     elif address_object.short_name in ('край', 'АО', 'Аобл', 'обл'):
         result = '{} {}'.format(address_object.formal_name, address_object.short_name)
     else:
-        result = '{}. {}'.format(address_object.short_name.rstrip('.'), address_object.formal_name)
+        result = '{}. {}'.format(address_object.short_name, address_object.formal_name)
 
     return result
 
 
 def get_house_name(house):
     """Возвращает полное наименование здания.
 
@@ -255,35 +228,14 @@
         names.append('корп. ' + house.building_number)
     if house.structure_number:
         names.append('стр. ' + house.structure_number)
 
     return ', '.join(names)
 
 
-def get_apartment_name(apartment):
-    """Возвращает полное наименование помещения.
-
-    Примеры:
-
-        * кв. 13
-
-    :rtype apartment: m3_gar_client.data.Apartment
-
-    :rtype: unicode
-    """
-    assert isinstance(apartment, Apartment), type(apartment)
-
-    if apartment.apart_type:
-        name = '{} {}'.format(apartment.apart_type, apartment.number)
-    else:
-        name = apartment.number
-
-    return name
-
-
 def get_full_name(obj, hierarchy=GAR_HIERARCHY_MUN, with_postal_code=True, timeout=None):
     """Возвращает полное наименование адресного объекта или здания.
 
     Примеры:
 
       * Забайкальский край, г. Чита
       * Новосибирская обл., г. Новосибирск, ул. Вокзальная магистраль, д. 1/1
@@ -293,60 +245,50 @@
     :param float timeout: Timeout запросов к серверу ГАР в секундах.
 
     :rtype: unicode
     """
     postal_code = None
     names = []
 
-    if not isinstance(obj, (Apartment, House, AddressObject)):
+    if not isinstance(obj, (House, AddressObject)):
         raise TypeError(obj)
 
     for addrobj in get_full_details(obj, hierarchy=hierarchy):
-        if with_postal_code and postal_code is None:
-            postal_code = getattr(addrobj, 'postal_code', None)
+        if postal_code is None and addrobj.postal_code:
+            postal_code = addrobj.postal_code
 
-        if isinstance(addrobj, AddressObject):
-            names.append(get_address_object_name(addrobj))
-
-        elif isinstance(addrobj, House):
+        if isinstance(addrobj, House):
             names.append(get_house_name(addrobj))
 
-        elif isinstance(addrobj, Apartment):
-            names.append(get_apartment_name(addrobj))
+        elif isinstance(addrobj, AddressObject):
+            names.append(get_address_object_name(addrobj))
 
     if with_postal_code and postal_code is not None:
-        names.append(postal_code)
+        names.insert(0, postal_code)
 
     full_name = ', '.join(reversed(names))
 
     return full_name
 
 
 def get_full_details(obj, hierarchy=GAR_HIERARCHY_MUN, timeout=None):
     """
     Возвращает полный список объектов, снизу вверх из иерархии.
     """
-    if not isinstance(obj, (Apartment, Stead, House, AddressObject)):
+    if not isinstance(obj, (House, AddressObject)):
         raise TypeError(obj)
 
     if hierarchy not in GAR_HIERARCHIES:
         raise ValueError(hierarchy)
 
     parent_attr = f'{hierarchy}_parent_obj_id'
 
     objects = []
 
-    if isinstance(obj, Apartment):
-        objects.append(obj)
-
-        parent_id = getattr(obj, parent_attr)
-        if parent_id:
-            obj = get_house(parent_id, timeout)
-
-    if isinstance(obj, (House, Stead)):
+    if isinstance(obj, House):
         objects.append(obj)
 
         parent_id = getattr(obj, parent_attr)
         if parent_id:
             obj = get_address_object(parent_id, timeout)
 
     if isinstance(obj, AddressObject):
@@ -366,7 +308,17 @@
     """
     Возвращает список наименований и сокращений узла, снизу вверх из иерархии.
     Не включая верхний уровень "Субъект РФ"
     """
     result = get_full_details(obj, timeout=timeout)
 
     return result[1:] if len(result) > 1 else result
+
+
+def reload_urlconf(urlconf=None):
+    """Перезагрузка Django urlconf."""
+
+    urlconf = urlconf or settings.ROOT_URLCONF
+    assert urlconf is not None
+
+    if urlconf in sys.modules:
+        clear_url_caches()
```

