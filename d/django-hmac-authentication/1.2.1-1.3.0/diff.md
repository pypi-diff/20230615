# Comparing `tmp/django_hmac_authentication-1.2.1.tar.gz` & `tmp/django_hmac_authentication-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_hmac_authentication-1.2.1.tar", last modified: Tue Jun  6 01:25:01 2023, max compression
+gzip compressed data, was "django_hmac_authentication-1.3.0.tar", last modified: Thu Jun 15 10:14:48 2023, max compression
```

## Comparing `django_hmac_authentication-1.2.1.tar` & `django_hmac_authentication-1.3.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.373198 django_hmac_authentication-1.2.1/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6359 2023-06-06 01:25:01.373198 django_hmac_authentication-1.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5821 2023-06-06 01:20:20.000000 django_hmac_authentication-1.2.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      722 2023-06-06 01:20:20.000000 django_hmac_authentication-1.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 01:25:01.373198 django_hmac_authentication-1.2.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.353197 django_hmac_authentication-1.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.361197 django_hmac_authentication-1.2.1/src/django_hmac_authentication/
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-06-06 01:20:20.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2023-06-06 00:58:59.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/aes.py
--rw-rw-rw-   0 root         (0) root         (0)     4383 2023-06-06 00:34:30.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     2817 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/client_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1375 2023-06-06 00:34:30.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.365198 django_hmac_authentication-1.2.1/src/django_hmac_authentication/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 01:24:20.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.365198 django_hmac_authentication-1.2.1/src/django_hmac_authentication/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 01:24:20.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1282 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/management/commands/create_hmac_for_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.365198 django_hmac_authentication-1.2.1/src/django_hmac_authentication/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      494 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/migrations/0002_apihmackey_failed_attempts.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2023-06-05 22:40:36.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 01:24:20.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1229 2023-06-05 22:40:36.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/models.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/padding.py
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     2546 2023-06-05 23:55:52.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/server_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      813 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.365198 django_hmac_authentication-1.2.1/src/django_hmac_authentication.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6359 2023-06-06 01:25:01.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2283 2023-06-06 01:25:01.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 01:25:01.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-06 01:25:01.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-06-06 01:25:01.000000 django_hmac_authentication-1.2.1/src/django_hmac_authentication.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.365198 django_hmac_authentication-1.2.1/src/example_django_project/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.369198 django_hmac_authentication-1.2.1/src/example_django_project/accounts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 01:24:20.000000 django_hmac_authentication-1.2.1/src/example_django_project/accounts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-05 01:42:47.000000 django_hmac_authentication-1.2.1/src/example_django_project/accounts/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/example_django_project/accounts/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.369198 django_hmac_authentication-1.2.1/src/example_django_project/accounts/migrations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 01:24:20.000000 django_hmac_authentication-1.2.1/src/example_django_project/accounts/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-05 01:42:47.000000 django_hmac_authentication-1.2.1/src/example_django_project/accounts/models.py
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-05 01:42:47.000000 django_hmac_authentication-1.2.1/src/example_django_project/accounts/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/example_django_project/accounts/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      576 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/example_django_project/accounts/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.369198 django_hmac_authentication-1.2.1/src/example_django_project/example_django_project/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 01:24:20.000000 django_hmac_authentication-1.2.1/src/example_django_project/example_django_project/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      421 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/example_django_project/example_django_project/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     3741 2023-06-06 00:58:59.000000 django_hmac_authentication-1.2.1/src/example_django_project/example_django_project/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/example_django_project/example_django_project/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      421 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/example_django_project/example_django_project/wsgi.py
--rw-rw-rw-   0 root         (0) root         (0)     1834 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/example_django_project/example_python_client.py
--rwxrwxrwx   0 root         (0) root         (0)      678 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/example_django_project/manage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 01:25:01.373198 django_hmac_authentication-1.2.1/src/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 01:24:20.000000 django_hmac_authentication-1.2.1/src/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-06-06 00:34:30.000000 django_hmac_authentication-1.2.1/src/tests/factories.py
--rw-rw-rw-   0 root         (0) root         (0)    14831 2023-06-06 00:34:30.000000 django_hmac_authentication-1.2.1/src/tests/test_authentication_api_key_secret.py
--rw-rw-rw-   0 root         (0) root         (0)     1502 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/tests/test_hmac_authorization_header_parsing.py
--rw-rw-rw-   0 root         (0) root         (0)     2356 2023-06-05 23:55:52.000000 django_hmac_authentication-1.2.1/src/tests/test_mgmt_cmd_create_hmac_for_user.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/tests/test_padding.py
--rw-rw-rw-   0 root         (0) root         (0)     3773 2023-06-05 23:55:52.000000 django_hmac_authentication-1.2.1/src/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1836 2023-06-04 10:27:36.000000 django_hmac_authentication-1.2.1/src/tests/test_view_create_api_key_secret.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.174998 django_hmac_authentication-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6348 2023-06-15 10:14:48.174998 django_hmac_authentication-1.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5810 2023-06-13 03:07:01.000000 django_hmac_authentication-1.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-06-15 10:09:43.000000 django_hmac_authentication-1.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 10:14:48.174998 django_hmac_authentication-1.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.154998 django_hmac_authentication-1.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.162998 django_hmac_authentication-1.3.0/src/django_hmac_authentication/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-06-15 10:09:43.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-06-06 00:58:59.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/aes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4485 2023-06-15 10:03:50.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     2817 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/client_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1520 2023-06-15 10:03:50.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.162998 django_hmac_authentication-1.3.0/src/django_hmac_authentication/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 10:14:10.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.162998 django_hmac_authentication-1.3.0/src/django_hmac_authentication/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 10:14:10.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/management/commands/create_hmac_for_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.162998 django_hmac_authentication-1.3.0/src/django_hmac_authentication/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      494 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/migrations/0002_apihmackey_failed_attempts.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-06-05 22:40:36.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 10:14:10.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2023-06-05 22:40:36.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/padding.py
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2546 2023-06-05 23:55:52.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/server_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.162998 django_hmac_authentication-1.3.0/src/django_hmac_authentication.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6348 2023-06-15 10:14:48.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2283 2023-06-15 10:14:48.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 10:14:48.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-15 10:14:48.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-15 10:14:48.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.166998 django_hmac_authentication-1.3.0/src/example_django_project/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.166998 django_hmac_authentication-1.3.0/src/example_django_project/accounts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 10:14:10.000000 django_hmac_authentication-1.3.0/src/example_django_project/accounts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-05 01:42:47.000000 django_hmac_authentication-1.3.0/src/example_django_project/accounts/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/example_django_project/accounts/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.166998 django_hmac_authentication-1.3.0/src/example_django_project/accounts/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 10:14:10.000000 django_hmac_authentication-1.3.0/src/example_django_project/accounts/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-05 01:42:47.000000 django_hmac_authentication-1.3.0/src/example_django_project/accounts/models.py
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-05 01:42:47.000000 django_hmac_authentication-1.3.0/src/example_django_project/accounts/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/example_django_project/accounts/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      576 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/example_django_project/accounts/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.166998 django_hmac_authentication-1.3.0/src/example_django_project/example_django_project/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 10:14:10.000000 django_hmac_authentication-1.3.0/src/example_django_project/example_django_project/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      421 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/example_django_project/example_django_project/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     3741 2023-06-06 00:58:59.000000 django_hmac_authentication-1.3.0/src/example_django_project/example_django_project/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/example_django_project/example_django_project/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      421 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/example_django_project/example_django_project/wsgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     1834 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/example_django_project/example_python_client.py
+-rwxrwxrwx   0 root         (0) root         (0)      678 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/example_django_project/manage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.170998 django_hmac_authentication-1.3.0/src/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 10:14:10.000000 django_hmac_authentication-1.3.0/src/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-06-06 00:34:30.000000 django_hmac_authentication-1.3.0/src/tests/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)    15731 2023-06-15 10:03:50.000000 django_hmac_authentication-1.3.0/src/tests/test_authentication_api_key_secret.py
+-rw-rw-rw-   0 root         (0) root         (0)     1502 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/tests/test_hmac_authorization_header_parsing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2356 2023-06-05 23:55:52.000000 django_hmac_authentication-1.3.0/src/tests/test_mgmt_cmd_create_hmac_for_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/tests/test_padding.py
+-rw-rw-rw-   0 root         (0) root         (0)     3773 2023-06-05 23:55:52.000000 django_hmac_authentication-1.3.0/src/tests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1836 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/tests/test_view_create_api_key_secret.py
```

### Comparing `django_hmac_authentication-1.2.1/LICENSE` & `django_hmac_authentication-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.1/PKG-INFO` & `django_hmac_authentication-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_hmac_authentication
-Version: 1.2.1
+Version: 1.3.0
 Summary: Django HMAC authentication using shared secret
 Author-email: Harisankar Krishna Swamy <harisankar.krishna@outlook.com>
 Project-URL: Homepage, https://github.com/harisankar-krishna-swamy/django_hmac_authentication
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.2
@@ -22,15 +22,15 @@
 * HMAC secret can be created with management command or obtained with a configured url
 * Supports Javascript and Python clients for programmatic access 
 * Optional configuration to auto revoke keys after N failed attempts to authenticate
 
 New feature
 * Optional `HMAC_EXPIRES_IN` configuration. If set HMAC keys will expire after interval.
 
->Built on Debian, KDE and CI/CD on GitLab :rocket:
+>Built on Debian, KDE and CI/CD on GitLab :rocket: :rocket:
 # 1. Install
 `pip install django_hmac_authentication`
 
 # 2. Configuration
 
 ## 2.1 settings.py
 
@@ -69,15 +69,15 @@
         'rest_framework.authentication.SessionAuthentication',
         'django_hmac_authentication.authentication.HMACAuthentication',
     ],
 }
 
 # Optional configurations
 HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD = 10
-HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD = '5m'
+HMAC_EXPIRES_IN = '5m'
 ```
 
 ## 2.2 urls.py
 Add url to obtain HMAC key and secret 
 ```python
 ...
 from django_hmac_authentication.views import CreateApiHMACKey
```

### Comparing `django_hmac_authentication-1.2.1/README.md` & `django_hmac_authentication-1.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 * HMAC secret can be created with management command or obtained with a configured url
 * Supports Javascript and Python clients for programmatic access 
 * Optional configuration to auto revoke keys after N failed attempts to authenticate
 
 New feature
 * Optional `HMAC_EXPIRES_IN` configuration. If set HMAC keys will expire after interval.
 
->Built on Debian, KDE and CI/CD on GitLab :rocket:
+>Built on Debian, KDE and CI/CD on GitLab :rocket: :rocket:
 # 1. Install
 `pip install django_hmac_authentication`
 
 # 2. Configuration
 
 ## 2.1 settings.py
 
@@ -56,15 +56,15 @@
         'rest_framework.authentication.SessionAuthentication',
         'django_hmac_authentication.authentication.HMACAuthentication',
     ],
 }
 
 # Optional configurations
 HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD = 10
-HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD = '5m'
+HMAC_EXPIRES_IN = '5m'
 ```
 
 ## 2.2 urls.py
 Add url to obtain HMAC key and secret 
 ```python
 ...
 from django_hmac_authentication.views import CreateApiHMACKey
```

### Comparing `django_hmac_authentication-1.2.1/pyproject.toml` & `django_hmac_authentication-1.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django_hmac_authentication"
-version = "1.2.1"
+version = "1.3.0"
 authors = [
   { name="Harisankar Krishna Swamy", email="harisankar.krishna@outlook.com" },
 ]
 description = "Django HMAC authentication using shared secret"
 readme = "README.md"
 requires-python = ">=3.9.2"
 dependencies = [
```

### Comparing `django_hmac_authentication-1.2.1/src/django_hmac_authentication/admin.py` & `django_hmac_authentication-1.3.0/src/django_hmac_authentication/admin.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.1/src/django_hmac_authentication/aes.py` & `django_hmac_authentication-1.3.0/src/django_hmac_authentication/aes.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.1/src/django_hmac_authentication/authentication.py` & `django_hmac_authentication-1.3.0/src/django_hmac_authentication/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from rest_framework.exceptions import AuthenticationFailed
 
 from django_hmac_authentication.client_utils import prepare_string_to_sign, sign_string
 from django_hmac_authentication.exceptions import (
     DateFormatException,
     ExpiredKeyException,
     ExpiredRequestException,
+    FutureRequestException,
     KeyDoesNotExistException,
     RevokedKeyException,
     SignatureVerificationException,
     UnsupportedHMACMethodException,
 )
 from django_hmac_authentication.models import ApiHMACKey
 from django_hmac_authentication.server_utils import aes_decrypt_hmac_secret
@@ -72,14 +73,17 @@
         utcnow = datetime.datetime.now(timezone.utc)
 
         try:
             req_utc = datetime.datetime.fromisoformat(date_in)
         except ValueError:
             raise DateFormatException()
 
+        if req_utc >= utcnow:
+            raise FutureRequestException()
+
         delta = utcnow - req_utc
         if delta.total_seconds() > auth_req_timeout:
             raise ExpiredRequestException()
 
         hmac_key = ApiHMACKey.objects.filter(id=key).first()
         if not hmac_key:
             raise KeyDoesNotExistException()
```

### Comparing `django_hmac_authentication-1.2.1/src/django_hmac_authentication/client_utils.py` & `django_hmac_authentication-1.3.0/src/django_hmac_authentication/client_utils.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.1/src/django_hmac_authentication/exceptions.py` & `django_hmac_authentication-1.3.0/src/django_hmac_authentication/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 
 
 class ExpiredRequestException(AuthenticationFailed):
     default_detail = _('Request has expired.')
     default_code = 'expired_request'
 
 
+class FutureRequestException(AuthenticationFailed):
+    default_detail = _('Request cannot be in future.')
+    default_code = 'future_request'
+
+
 class SignatureVerificationException(AuthenticationFailed):
     default_detail = _('Signature verification failed.')
     default_code = 'verification_failed'
 
 
 class DateFormatException(AuthenticationFailed):
     default_detail = _('Invalid date format in Authorization header.')
```

### Comparing `django_hmac_authentication-1.2.1/src/django_hmac_authentication/management/commands/create_hmac_for_user.py` & `django_hmac_authentication-1.3.0/src/django_hmac_authentication/management/commands/create_hmac_for_user.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.1/src/django_hmac_authentication/migrations/0001_initial.py` & `django_hmac_authentication-1.3.0/src/django_hmac_authentication/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.1/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py` & `django_hmac_authentication-1.3.0/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.1/src/django_hmac_authentication/models.py` & `django_hmac_authentication-1.3.0/src/django_hmac_authentication/models.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.1/src/django_hmac_authentication/server_utils.py` & `django_hmac_authentication-1.3.0/src/django_hmac_authentication/server_utils.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.1/src/django_hmac_authentication/views.py` & `django_hmac_authentication-1.3.0/src/django_hmac_authentication/views.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.1/src/django_hmac_authentication.egg-info/PKG-INFO` & `django_hmac_authentication-1.3.0/src/django_hmac_authentication.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-hmac-authentication
-Version: 1.2.1
+Version: 1.3.0
 Summary: Django HMAC authentication using shared secret
 Author-email: Harisankar Krishna Swamy <harisankar.krishna@outlook.com>
 Project-URL: Homepage, https://github.com/harisankar-krishna-swamy/django_hmac_authentication
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.2
@@ -22,15 +22,15 @@
 * HMAC secret can be created with management command or obtained with a configured url
 * Supports Javascript and Python clients for programmatic access 
 * Optional configuration to auto revoke keys after N failed attempts to authenticate
 
 New feature
 * Optional `HMAC_EXPIRES_IN` configuration. If set HMAC keys will expire after interval.
 
->Built on Debian, KDE and CI/CD on GitLab :rocket:
+>Built on Debian, KDE and CI/CD on GitLab :rocket: :rocket:
 # 1. Install
 `pip install django_hmac_authentication`
 
 # 2. Configuration
 
 ## 2.1 settings.py
 
@@ -69,15 +69,15 @@
         'rest_framework.authentication.SessionAuthentication',
         'django_hmac_authentication.authentication.HMACAuthentication',
     ],
 }
 
 # Optional configurations
 HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD = 10
-HMAC_AUTH_FAILED_ATTEMPTS_THRESHOLD = '5m'
+HMAC_EXPIRES_IN = '5m'
 ```
 
 ## 2.2 urls.py
 Add url to obtain HMAC key and secret 
 ```python
 ...
 from django_hmac_authentication.views import CreateApiHMACKey
```

### Comparing `django_hmac_authentication-1.2.1/src/django_hmac_authentication.egg-info/SOURCES.txt` & `django_hmac_authentication-1.3.0/src/django_hmac_authentication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.1/src/example_django_project/accounts/views.py` & `django_hmac_authentication-1.3.0/src/example_django_project/accounts/views.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.1/src/example_django_project/example_django_project/settings.py` & `django_hmac_authentication-1.3.0/src/example_django_project/example_django_project/settings.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.1/src/example_django_project/example_django_project/urls.py` & `django_hmac_authentication-1.3.0/src/example_django_project/example_django_project/urls.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.1/src/example_django_project/example_python_client.py` & `django_hmac_authentication-1.3.0/src/example_django_project/example_python_client.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.1/src/example_django_project/manage.py` & `django_hmac_authentication-1.3.0/src/example_django_project/manage.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.1/src/tests/factories.py` & `django_hmac_authentication-1.3.0/src/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.1/src/tests/test_authentication_api_key_secret.py` & `django_hmac_authentication-1.3.0/src/tests/test_authentication_api_key_secret.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from django_hmac_authentication.authentication import HMACAuthentication
 from django_hmac_authentication.client_utils import prepare_string_to_sign, sign_string
 from django_hmac_authentication.exceptions import (
     DateFormatException,
     ExpiredKeyException,
     ExpiredRequestException,
+    FutureRequestException,
     KeyDoesNotExistException,
     RevokedKeyException,
     SignatureVerificationException,
     UnsupportedHMACMethodException,
 )
 from django_hmac_authentication.server_utils import aes_decrypt_hmac_secret
 from tests.factories import ApiHMACKeyFactory, ApiHMACKeyUserFactory
@@ -234,14 +235,36 @@
         self.assertEqual(
             response.status_code,
             HTTPStatus.FORBIDDEN,
             'Timed out request must fail authentication',
         )
         self._assert_response_error_detail(response.data, ExpiredRequestException())
 
+    def test_hmac_authentication__future_request(self):
+        factory = APIRequestFactory()
+        req_data = ''
+        initial_datetime = datetime.utcnow() + timedelta(seconds=6)
+        with freeze_time(initial_datetime):
+            signature, utc_8601 = self._request_auth_header_fields(
+                req_data, 'HMAC-SHA512'
+            )
+
+        headers = {
+            f'{self.auth_header}': f'HMAC-SHA512 {self.hmac_key.id};{signature};{utc_8601}',
+            'Content-Type': 'application/json',
+        }
+        request = factory.get('/', data=None, **headers)
+        response = self.view(request)
+        self.assertEqual(
+            response.status_code,
+            HTTPStatus.FORBIDDEN,
+            'Future timed request must fail authentication',
+        )
+        self._assert_response_error_detail(response.data, FutureRequestException())
+
     def test_hmac_authentication__unsupported_hmac_method(self):
         factory = APIRequestFactory()
         req_data = ''
         signature, utc_8601 = self._request_auth_header_fields(req_data, 'HMAC-SHA512')
         # Unsupported hmac method
         headers = {
             f'{self.auth_header}': f'HMAC-SHA123 {self.hmac_key.id};{signature};{utc_8601}',
@@ -380,31 +403,33 @@
         self.assertEqual(
             response.status_code,
             HTTPStatus.FORBIDDEN,
             'Authentication must fail on malformed header',
         )
 
     def test_hmac_authentication__expires_in(self):
-        initial_datetime = datetime.now(timezone.utc)
-        test_expires_at = initial_datetime + timedelta(days=1)
+        initial_time = datetime.now(timezone.utc)
+        test_expires_at = initial_time - timedelta(days=1)
+        self.hmac_key.expires_at = test_expires_at
+        self.hmac_key.save()
+        self.hmac_key.refresh_from_db()
         factory = APIRequestFactory()
         req_data = ''
         with mock.patch(
             'django_hmac_authentication.authentication.hmac_expires_in',
             '1d',
         ):
-            with freeze_time(test_expires_at):
-                signature, utc_8601 = self._request_auth_header_fields(
-                    req_data, 'HMAC-SHA512'
-                )
-                headers = {
-                    f'{self.auth_header}': f'HMAC-SHA512 {self.hmac_key.id};{signature};{utc_8601}',
-                    'Content-Type': 'application/json',
-                }
-                request = factory.get('/', data=None, **headers)
-                response = self.view(request)
-                self.assertEqual(
-                    response.status_code,
-                    HTTPStatus.FORBIDDEN,
-                    'Expired key must fail authentication',
-                )
-                self._assert_response_error_detail(response.data, ExpiredKeyException())
+            signature, utc_8601 = self._request_auth_header_fields(
+                req_data, 'HMAC-SHA512'
+            )
+            headers = {
+                f'{self.auth_header}': f'HMAC-SHA512 {self.hmac_key.id};{signature};{utc_8601}',
+                'Content-Type': 'application/json',
+            }
+            request = factory.get('/', data=None, **headers)
+            response = self.view(request)
+            self.assertEqual(
+                response.status_code,
+                HTTPStatus.FORBIDDEN,
+                'Expired key must fail authentication',
+            )
+            self._assert_response_error_detail(response.data, ExpiredKeyException())
```

### Comparing `django_hmac_authentication-1.2.1/src/tests/test_hmac_authorization_header_parsing.py` & `django_hmac_authentication-1.3.0/src/tests/test_hmac_authorization_header_parsing.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.1/src/tests/test_mgmt_cmd_create_hmac_for_user.py` & `django_hmac_authentication-1.3.0/src/tests/test_mgmt_cmd_create_hmac_for_user.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.1/src/tests/test_padding.py` & `django_hmac_authentication-1.3.0/src/tests/test_padding.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.1/src/tests/test_utils.py` & `django_hmac_authentication-1.3.0/src/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.2.1/src/tests/test_view_create_api_key_secret.py` & `django_hmac_authentication-1.3.0/src/tests/test_view_create_api_key_secret.py`

 * *Files identical despite different names*

