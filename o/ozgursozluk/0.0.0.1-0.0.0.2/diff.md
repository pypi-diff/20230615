# Comparing `tmp/ozgursozluk-0.0.0.1.tar.gz` & `tmp/ozgursozluk-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ozgursozluk-0.0.0.1.tar", last modified: Thu Jun 15 11:02:48 2023, max compression
+gzip compressed data, was "ozgursozluk-0.0.0.2.tar", last modified: Thu Jun 15 11:11:11 2023, max compression
```

## Comparing `ozgursozluk-0.0.0.1.tar` & `ozgursozluk-0.0.0.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 beucismis  (1000) beucismis  (1000)        0 2023-06-15 11:02:48.581786 ozgursozluk-0.0.0.1/
-drwxr-xr-x   0 beucismis  (1000) beucismis  (1000)        0 2023-06-15 11:02:48.553786 ozgursozluk-0.0.0.1/.github/
-drwxr-xr-x   0 beucismis  (1000) beucismis  (1000)        0 2023-06-15 11:02:48.557786 ozgursozluk-0.0.0.1/.github/workflows/
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      607 2023-06-14 21:34:47.000000 ozgursozluk-0.0.0.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      582 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/.github/workflows/tests.yml
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)     3087 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/.gitignore
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      175 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/Dockerfile
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      488 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/LICENSE
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      723 2023-06-15 11:02:48.577786 ozgursozluk-0.0.0.1/PKG-INFO
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)     2322 2023-06-14 21:34:43.000000 ozgursozluk-0.0.0.1/README.md
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      366 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/TODO.md
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)       55 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/gunicorn.conf.py
-drwxr-xr-x   0 beucismis  (1000) beucismis  (1000)        0 2023-06-15 11:02:48.561786 ozgursozluk-0.0.0.1/ozgursozluk/
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      308 2023-06-15 11:02:24.000000 ozgursozluk-0.0.0.1/ozgursozluk/__init__.py
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)     5307 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/ozgursozluk/api.py
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      886 2023-06-12 10:53:49.000000 ozgursozluk-0.0.0.1/ozgursozluk/configs.py
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      890 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/ozgursozluk/models.py
-drwxr-xr-x   0 beucismis  (1000) beucismis  (1000)        0 2023-06-15 11:02:48.573786 ozgursozluk-0.0.0.1/ozgursozluk/static/
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      211 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/ozgursozluk/static/amoled.css
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      211 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/ozgursozluk/static/dark.css
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      213 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/ozgursozluk/static/discord.css
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)     1702 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/ozgursozluk/static/favicon.png
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      220 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/ozgursozluk/static/gruvbox.css
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      212 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/ozgursozluk/static/gruvboxlight.css
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      212 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/ozgursozluk/static/light.css
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      213 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/ozgursozluk/static/startpage.css
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)     2995 2023-06-12 10:50:17.000000 ozgursozluk-0.0.0.1/ozgursozluk/static/style.css
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      211 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/ozgursozluk/static/violet.css
-drwxr-xr-x   0 beucismis  (1000) beucismis  (1000)        0 2023-06-15 11:02:48.577786 ozgursozluk-0.0.0.1/ozgursozluk/templates/
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      612 2023-06-15 10:54:36.000000 ozgursozluk-0.0.0.1/ozgursozluk/templates/404.html
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)     1370 2023-06-15 10:54:32.000000 ozgursozluk-0.0.0.1/ozgursozluk/templates/author.html
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)     1392 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/ozgursozluk/templates/base.html
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      766 2023-06-12 10:45:11.000000 ozgursozluk-0.0.0.1/ozgursozluk/templates/debe.html
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      867 2023-06-15 09:37:16.000000 ozgursozluk-0.0.0.1/ozgursozluk/templates/entry.html
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)     1910 2023-06-12 10:41:29.000000 ozgursozluk-0.0.0.1/ozgursozluk/templates/index.html
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)     1610 2023-06-12 10:42:46.000000 ozgursozluk-0.0.0.1/ozgursozluk/templates/macros.html
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      205 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/ozgursozluk/templates/navigation.html
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)     1044 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/ozgursozluk/templates/paginate.html
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)     3818 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/ozgursozluk/templates/settings.html
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)     1234 2023-06-15 10:52:24.000000 ozgursozluk-0.0.0.1/ozgursozluk/templates/topic.html
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      677 2023-06-13 19:45:07.000000 ozgursozluk-0.0.0.1/ozgursozluk/utils.py
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)     2855 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/ozgursozluk/views.py
-drwxr-xr-x   0 beucismis  (1000) beucismis  (1000)        0 2023-06-15 11:02:48.565786 ozgursozluk-0.0.0.1/ozgursozluk.egg-info/
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      723 2023-06-15 11:02:48.000000 ozgursozluk-0.0.0.1/ozgursozluk.egg-info/PKG-INFO
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)     1176 2023-06-15 11:02:48.000000 ozgursozluk-0.0.0.1/ozgursozluk.egg-info/SOURCES.txt
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)        1 2023-06-15 11:02:48.000000 ozgursozluk-0.0.0.1/ozgursozluk.egg-info/dependency_links.txt
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)       92 2023-06-15 11:02:48.000000 ozgursozluk-0.0.0.1/ozgursozluk.egg-info/requires.txt
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)       12 2023-06-15 11:02:48.000000 ozgursozluk-0.0.0.1/ozgursozluk.egg-info/top_level.txt
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)     1153 2023-06-15 10:58:50.000000 ozgursozluk-0.0.0.1/pyproject.toml
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)       17 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/requirements-dev.txt
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)       92 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/requirements.txt
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)       38 2023-06-15 11:02:48.581786 ozgursozluk-0.0.0.1/setup.cfg
--rw-r--r--   0 beucismis  (1000) beucismis  (1000)      917 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.1/tests.py
+drwxr-xr-x   0 beucismis  (1000) beucismis  (1000)        0 2023-06-15 11:11:11.976282 ozgursozluk-0.0.0.2/
+drwxr-xr-x   0 beucismis  (1000) beucismis  (1000)        0 2023-06-15 11:11:11.944282 ozgursozluk-0.0.0.2/.github/
+drwxr-xr-x   0 beucismis  (1000) beucismis  (1000)        0 2023-06-15 11:11:11.956282 ozgursozluk-0.0.0.2/.github/workflows/
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      607 2023-06-14 21:34:47.000000 ozgursozluk-0.0.0.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      582 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/.github/workflows/tests.yml
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)     3087 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/.gitignore
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      175 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/Dockerfile
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      488 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/LICENSE
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)     1325 2023-06-15 11:11:11.976282 ozgursozluk-0.0.0.2/PKG-INFO
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)     2322 2023-06-14 21:34:43.000000 ozgursozluk-0.0.0.2/README.md
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      366 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/TODO.md
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)       55 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/gunicorn.conf.py
+drwxr-xr-x   0 beucismis  (1000) beucismis  (1000)        0 2023-06-15 11:11:11.956282 ozgursozluk-0.0.0.2/ozgursozluk/
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      308 2023-06-15 11:09:50.000000 ozgursozluk-0.0.0.2/ozgursozluk/__init__.py
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)     5307 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/ozgursozluk/api.py
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      886 2023-06-12 10:53:49.000000 ozgursozluk-0.0.0.2/ozgursozluk/configs.py
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      890 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/ozgursozluk/models.py
+drwxr-xr-x   0 beucismis  (1000) beucismis  (1000)        0 2023-06-15 11:11:11.964282 ozgursozluk-0.0.0.2/ozgursozluk/static/
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      211 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/ozgursozluk/static/amoled.css
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      211 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/ozgursozluk/static/dark.css
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      213 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/ozgursozluk/static/discord.css
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)     1702 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/ozgursozluk/static/favicon.png
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      220 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/ozgursozluk/static/gruvbox.css
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      212 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/ozgursozluk/static/gruvboxlight.css
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      212 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/ozgursozluk/static/light.css
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      213 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/ozgursozluk/static/startpage.css
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)     2995 2023-06-12 10:50:17.000000 ozgursozluk-0.0.0.2/ozgursozluk/static/style.css
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      211 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/ozgursozluk/static/violet.css
+drwxr-xr-x   0 beucismis  (1000) beucismis  (1000)        0 2023-06-15 11:11:11.976282 ozgursozluk-0.0.0.2/ozgursozluk/templates/
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      612 2023-06-15 10:54:36.000000 ozgursozluk-0.0.0.2/ozgursozluk/templates/404.html
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)     1370 2023-06-15 10:54:32.000000 ozgursozluk-0.0.0.2/ozgursozluk/templates/author.html
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)     1392 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/ozgursozluk/templates/base.html
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      766 2023-06-12 10:45:11.000000 ozgursozluk-0.0.0.2/ozgursozluk/templates/debe.html
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      867 2023-06-15 09:37:16.000000 ozgursozluk-0.0.0.2/ozgursozluk/templates/entry.html
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)     1910 2023-06-12 10:41:29.000000 ozgursozluk-0.0.0.2/ozgursozluk/templates/index.html
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)     1610 2023-06-12 10:42:46.000000 ozgursozluk-0.0.0.2/ozgursozluk/templates/macros.html
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      205 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/ozgursozluk/templates/navigation.html
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)     1044 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/ozgursozluk/templates/paginate.html
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)     3818 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/ozgursozluk/templates/settings.html
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)     1234 2023-06-15 10:52:24.000000 ozgursozluk-0.0.0.2/ozgursozluk/templates/topic.html
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      677 2023-06-13 19:45:07.000000 ozgursozluk-0.0.0.2/ozgursozluk/utils.py
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)     2855 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/ozgursozluk/views.py
+drwxr-xr-x   0 beucismis  (1000) beucismis  (1000)        0 2023-06-15 11:11:11.960282 ozgursozluk-0.0.0.2/ozgursozluk.egg-info/
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)     1325 2023-06-15 11:11:11.000000 ozgursozluk-0.0.0.2/ozgursozluk.egg-info/PKG-INFO
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)     1176 2023-06-15 11:11:11.000000 ozgursozluk-0.0.0.2/ozgursozluk.egg-info/SOURCES.txt
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)        1 2023-06-15 11:11:11.000000 ozgursozluk-0.0.0.2/ozgursozluk.egg-info/dependency_links.txt
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)       92 2023-06-15 11:11:11.000000 ozgursozluk-0.0.0.2/ozgursozluk.egg-info/requires.txt
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)       12 2023-06-15 11:11:11.000000 ozgursozluk-0.0.0.2/ozgursozluk.egg-info/top_level.txt
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)     1124 2023-06-15 11:10:42.000000 ozgursozluk-0.0.0.2/pyproject.toml
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)       17 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/requirements-dev.txt
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)       92 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/requirements.txt
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)       38 2023-06-15 11:11:11.980283 ozgursozluk-0.0.0.2/setup.cfg
+-rw-r--r--   0 beucismis  (1000) beucismis  (1000)      917 2023-06-11 13:48:49.000000 ozgursozluk-0.0.0.2/tests.py
```

### Comparing `ozgursozluk-0.0.0.1/.github/workflows/publish-to-pypi.yml` & `ozgursozluk-0.0.0.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/.github/workflows/tests.yml` & `ozgursozluk-0.0.0.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/.gitignore` & `ozgursozluk-0.0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/README.md` & `ozgursozluk-0.0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/ozgursozluk/api.py` & `ozgursozluk-0.0.0.2/ozgursozluk/api.py`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/ozgursozluk/configs.py` & `ozgursozluk-0.0.0.2/ozgursozluk/configs.py`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/ozgursozluk/models.py` & `ozgursozluk-0.0.0.2/ozgursozluk/models.py`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/ozgursozluk/static/favicon.png` & `ozgursozluk-0.0.0.2/ozgursozluk/static/favicon.png`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/ozgursozluk/static/style.css` & `ozgursozluk-0.0.0.2/ozgursozluk/static/style.css`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/ozgursozluk/templates/404.html` & `ozgursozluk-0.0.0.2/ozgursozluk/templates/404.html`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/ozgursozluk/templates/author.html` & `ozgursozluk-0.0.0.2/ozgursozluk/templates/author.html`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/ozgursozluk/templates/base.html` & `ozgursozluk-0.0.0.2/ozgursozluk/templates/base.html`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/ozgursozluk/templates/debe.html` & `ozgursozluk-0.0.0.2/ozgursozluk/templates/debe.html`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/ozgursozluk/templates/entry.html` & `ozgursozluk-0.0.0.2/ozgursozluk/templates/entry.html`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/ozgursozluk/templates/index.html` & `ozgursozluk-0.0.0.2/ozgursozluk/templates/index.html`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/ozgursozluk/templates/macros.html` & `ozgursozluk-0.0.0.2/ozgursozluk/templates/macros.html`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/ozgursozluk/templates/paginate.html` & `ozgursozluk-0.0.0.2/ozgursozluk/templates/paginate.html`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/ozgursozluk/templates/settings.html` & `ozgursozluk-0.0.0.2/ozgursozluk/templates/settings.html`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/ozgursozluk/templates/topic.html` & `ozgursozluk-0.0.0.2/ozgursozluk/templates/topic.html`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/ozgursozluk/utils.py` & `ozgursozluk-0.0.0.2/ozgursozluk/utils.py`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/ozgursozluk/views.py` & `ozgursozluk-0.0.0.2/ozgursozluk/views.py`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/ozgursozluk.egg-info/SOURCES.txt` & `ozgursozluk-0.0.0.2/ozgursozluk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.0.0.1/pyproject.toml` & `ozgursozluk-0.0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 ]
 description = "A free and open source alternative ekşi sözlük front-end"
 requires-python = ">=3.8"
 keywords = [
     "alternative", "flask", "front-end", "eksisozluk", "self-hosted",
     "beautifulsoup", "eksi", "sozluk", "debe", "gundem", "sukela",
 ]
+license = {file = "LICENSE"}
 classifiers = [
     "Topic :: Internet",
     "Framework :: Flask",
     "Programming Language :: Python",
 ]
 dynamic = ["version", "dependencies"]
 
 [tool.poetry]
-long_description = "README.md"
-long_description_content_type = "text/markdown"
+readme = "README.md"
 include = [
     "ozgursozluk/static/*", "ozgursozluk/templates/*",
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "ozgursozluk.__version__"}
 dependencies = {file = ["requirements.txt"]}
```

### Comparing `ozgursozluk-0.0.0.1/tests.py` & `ozgursozluk-0.0.0.2/tests.py`

 * *Files identical despite different names*

