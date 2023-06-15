# Comparing `tmp/sphinx-subprojecttoctree-0.5.2.tar.gz` & `tmp/sphinx-subprojecttoctree-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-subprojecttoctree-0.5.2.tar", last modified: Sat Nov 12 16:30:14 2022, max compression
+gzip compressed data, was "sphinx-subprojecttoctree-0.5.3.tar", last modified: Thu Jun 15 20:29:58 2023, max compression
```

## Comparing `sphinx-subprojecttoctree-0.5.2.tar` & `sphinx-subprojecttoctree-0.5.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 dries     (1000) dries     (1000)        0 2022-11-12 16:30:14.303975 sphinx-subprojecttoctree-0.5.2/
-drwxrwxr-x   0 dries     (1000) dries     (1000)        0 2022-11-12 16:30:14.287979 sphinx-subprojecttoctree-0.5.2/.github/
--rw-rw-r--   0 dries     (1000) dries     (1000)      203 2022-11-06 12:11:13.000000 sphinx-subprojecttoctree-0.5.2/.github/dependabot.yml
-drwxrwxr-x   0 dries     (1000) dries     (1000)        0 2022-11-12 16:30:14.287979 sphinx-subprojecttoctree-0.5.2/.github/workflows/
--rw-rw-r--   0 dries     (1000) dries     (1000)     1687 2022-11-11 12:20:43.000000 sphinx-subprojecttoctree-0.5.2/.github/workflows/ci.yml
--rw-rw-r--   0 dries     (1000) dries     (1000)      132 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/.gitignore
--rw-rw-r--   0 dries     (1000) dries     (1000)      216 2022-11-09 21:13:10.000000 sphinx-subprojecttoctree-0.5.2/.pre-commit-config.yaml
--rw-rw-r--   0 dries     (1000) dries     (1000)      118 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/.readthedocs.yml
--rw-rw-r--   0 dries     (1000) dries     (1000)     2322 2022-11-12 16:14:36.000000 sphinx-subprojecttoctree-0.5.2/CHANGELOG.rst
--rw-rw-r--   0 dries     (1000) dries     (1000)     1072 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/LICENSE
--rw-rw-r--   0 dries     (1000) dries     (1000)     2466 2022-11-12 16:30:14.303975 sphinx-subprojecttoctree-0.5.2/PKG-INFO
--rw-rw-r--   0 dries     (1000) dries     (1000)     1581 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/README.md
-drwxrwxr-x   0 dries     (1000) dries     (1000)        0 2022-11-12 16:30:14.287979 sphinx-subprojecttoctree-0.5.2/docs/
--rw-rw-r--   0 dries     (1000) dries     (1000)      638 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/docs/Makefile
--rw-rw-r--   0 dries     (1000) dries     (1000)      804 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/docs/make.bat
-drwxrwxr-x   0 dries     (1000) dries     (1000)        0 2022-11-12 16:30:14.291978 sphinx-subprojecttoctree-0.5.2/docs/source/
--rw-rw-r--   0 dries     (1000) dries     (1000)       32 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/docs/source/changelog.rst
--rw-rw-r--   0 dries     (1000) dries     (1000)     2443 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/docs/source/conf.py
-drwxrwxr-x   0 dries     (1000) dries     (1000)        0 2022-11-12 16:30:14.291978 sphinx-subprojecttoctree-0.5.2/docs/source/images/
--rwxrwxr-x   0 dries     (1000) dries     (1000)   197925 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/docs/source/images/subprojects.png
--rw-rw-r--   0 dries     (1000) dries     (1000)      789 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/docs/source/index.rst
--rw-rw-r--   0 dries     (1000) dries     (1000)     1006 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/docs/source/installation.rst
--rw-rw-r--   0 dries     (1000) dries     (1000)     7518 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/docs/source/userguide.rst
--rw-rw-r--   0 dries     (1000) dries     (1000)      354 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/pyproject.toml
--rw-rw-r--   0 dries     (1000) dries     (1000)     1282 2022-11-12 16:30:14.303975 sphinx-subprojecttoctree-0.5.2/setup.cfg
-drwxrwxr-x   0 dries     (1000) dries     (1000)        0 2022-11-12 16:30:14.295977 sphinx-subprojecttoctree-0.5.2/sphinx_subprojecttoctree.egg-info/
--rw-rw-r--   0 dries     (1000) dries     (1000)     2466 2022-11-12 16:30:14.000000 sphinx-subprojecttoctree-0.5.2/sphinx_subprojecttoctree.egg-info/PKG-INFO
--rw-rw-r--   0 dries     (1000) dries     (1000)     2376 2022-11-12 16:30:14.000000 sphinx-subprojecttoctree-0.5.2/sphinx_subprojecttoctree.egg-info/SOURCES.txt
--rw-rw-r--   0 dries     (1000) dries     (1000)        1 2022-11-12 16:30:14.000000 sphinx-subprojecttoctree-0.5.2/sphinx_subprojecttoctree.egg-info/dependency_links.txt
--rw-rw-r--   0 dries     (1000) dries     (1000)      114 2022-11-12 16:30:14.000000 sphinx-subprojecttoctree-0.5.2/sphinx_subprojecttoctree.egg-info/requires.txt
--rw-rw-r--   0 dries     (1000) dries     (1000)       18 2022-11-12 16:30:14.000000 sphinx-subprojecttoctree-0.5.2/sphinx_subprojecttoctree.egg-info/top_level.txt
-drwxrwxr-x   0 dries     (1000) dries     (1000)        0 2022-11-12 16:30:14.295977 sphinx-subprojecttoctree-0.5.2/subprojecttoctree/
--rw-rw-r--   0 dries     (1000) dries     (1000)     6105 2022-11-09 21:13:10.000000 sphinx-subprojecttoctree-0.5.2/subprojecttoctree/__init__.py
--rw-rw-r--   0 dries     (1000) dries     (1000)      176 2022-11-12 16:30:14.000000 sphinx-subprojecttoctree-0.5.2/subprojecttoctree/__version__.py
--rw-rw-r--   0 dries     (1000) dries     (1000)      875 2022-11-12 15:43:56.000000 sphinx-subprojecttoctree-0.5.2/subprojecttoctree/builders.py
--rw-rw-r--   0 dries     (1000) dries     (1000)     3901 2022-11-09 21:13:10.000000 sphinx-subprojecttoctree-0.5.2/subprojecttoctree/toctree.py
--rw-rw-r--   0 dries     (1000) dries     (1000)      979 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/subprojecttoctree/utils.py
-drwxrwxr-x   0 dries     (1000) dries     (1000)        0 2022-11-12 16:30:14.299976 sphinx-subprojecttoctree-0.5.2/test/
--rw-rw-r--   0 dries     (1000) dries     (1000)     2621 2022-11-12 16:06:52.000000 sphinx-subprojecttoctree-0.5.2/test/conftest.py
-drwxrwxr-x   0 dries     (1000) dries     (1000)        0 2022-11-12 16:30:14.279982 sphinx-subprojecttoctree-0.5.2/test/roots/
-drwxrwxr-x   0 dries     (1000) dries     (1000)        0 2022-11-12 16:30:14.299976 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-master/
--rw-rw-r--   0 dries     (1000) dries     (1000)        7 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-master/bar.rst
--rw-rw-r--   0 dries     (1000) dries     (1000)      117 2022-11-12 15:47:58.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-master/conf.py
--rw-rw-r--   0 dries     (1000) dries     (1000)        7 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-master/foo.rst
--rw-rw-r--   0 dries     (1000) dries     (1000)      136 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-master/index.rst
-drwxrwxr-x   0 dries     (1000) dries     (1000)        0 2022-11-12 16:30:14.299976 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-master-entry-after-subproject/
--rw-rw-r--   0 dries     (1000) dries     (1000)        7 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-master-entry-after-subproject/bar.rst
--rw-rw-r--   0 dries     (1000) dries     (1000)      117 2022-11-12 15:45:05.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-master-entry-after-subproject/conf.py
--rw-rw-r--   0 dries     (1000) dries     (1000)        7 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-master-entry-after-subproject/foo.rst
--rw-rw-r--   0 dries     (1000) dries     (1000)      147 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-master-entry-after-subproject/index.rst
--rw-rw-r--   0 dries     (1000) dries     (1000)       11 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-master-entry-after-subproject/ipsum.rst
-drwxrwxr-x   0 dries     (1000) dries     (1000)        0 2022-11-12 16:30:14.299976 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-master-with-regular-http-url/
--rw-rw-r--   0 dries     (1000) dries     (1000)        7 2022-11-09 21:13:10.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-master-with-regular-http-url/bar.rst
--rw-rw-r--   0 dries     (1000) dries     (1000)      117 2022-11-12 15:45:20.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-master-with-regular-http-url/conf.py
--rw-rw-r--   0 dries     (1000) dries     (1000)        7 2022-11-09 21:13:10.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-master-with-regular-http-url/foo.rst
--rw-rw-r--   0 dries     (1000) dries     (1000)      170 2022-11-09 21:13:10.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-master-with-regular-http-url/index.rst
-drwxrwxr-x   0 dries     (1000) dries     (1000)        0 2022-11-12 16:30:14.303975 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-subproject/
--rw-rw-r--   0 dries     (1000) dries     (1000)        7 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-subproject/bar.rst
--rw-rw-r--   0 dries     (1000) dries     (1000)      116 2022-11-12 15:47:42.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-subproject/conf.py
--rw-rw-r--   0 dries     (1000) dries     (1000)        7 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-subproject/foo.rst
--rw-rw-r--   0 dries     (1000) dries     (1000)      101 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-subproject/index.rst
-drwxrwxr-x   0 dries     (1000) dries     (1000)        0 2022-11-12 16:30:14.303975 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-subproject-multiple-toctrees/
--rw-rw-r--   0 dries     (1000) dries     (1000)        7 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-subproject-multiple-toctrees/bar.rst
--rw-rw-r--   0 dries     (1000) dries     (1000)      116 2022-11-12 15:47:49.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-subproject-multiple-toctrees/conf.py
--rw-rw-r--   0 dries     (1000) dries     (1000)        7 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-subproject-multiple-toctrees/foo.rst
--rw-rw-r--   0 dries     (1000) dries     (1000)       92 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-subproject-multiple-toctrees/index.rst
-drwxrwxr-x   0 dries     (1000) dries     (1000)        0 2022-11-12 16:30:14.303975 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-subproject-nested/
--rw-rw-r--   0 dries     (1000) dries     (1000)        7 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-subproject-nested/bar.rst
--rw-rw-r--   0 dries     (1000) dries     (1000)      116 2022-11-12 15:45:11.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-subproject-nested/conf.py
--rw-rw-r--   0 dries     (1000) dries     (1000)        7 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-subproject-nested/foo.rst
--rw-rw-r--   0 dries     (1000) dries     (1000)      144 2022-08-29 18:52:47.000000 sphinx-subprojecttoctree-0.5.2/test/roots/test-subprojecttoctree-subproject-nested/index.rst
--rw-rw-r--   0 dries     (1000) dries     (1000)    20000 2022-11-11 23:17:00.000000 sphinx-subprojecttoctree-0.5.2/test/test_subprojecttoctree.py
--rw-rw-r--   0 dries     (1000) dries     (1000)     1268 2022-11-11 12:26:49.000000 sphinx-subprojecttoctree-0.5.2/tox.ini
+drwxr-xr-x   0 driesschaumont   (501) staff       (20)        0 2023-06-15 20:29:58.916883 sphinx-subprojecttoctree-0.5.3/
+drwxr-xr-x   0 driesschaumont   (501) staff       (20)        0 2023-06-15 20:29:58.907432 sphinx-subprojecttoctree-0.5.3/.github/
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      203 2022-11-07 07:57:05.000000 sphinx-subprojecttoctree-0.5.3/.github/dependabot.yml
+drwxr-xr-x   0 driesschaumont   (501) staff       (20)        0 2023-06-15 20:29:58.907699 sphinx-subprojecttoctree-0.5.3/.github/workflows/
+-rw-r--r--   0 driesschaumont   (501) staff       (20)     1695 2022-11-17 17:07:32.000000 sphinx-subprojecttoctree-0.5.3/.github/workflows/ci.yml
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      132 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/.gitignore
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      216 2022-11-10 08:16:46.000000 sphinx-subprojecttoctree-0.5.3/.pre-commit-config.yaml
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      118 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/.readthedocs.yml
+-rw-r--r--   0 driesschaumont   (501) staff       (20)     2473 2023-06-15 20:24:02.000000 sphinx-subprojecttoctree-0.5.3/CHANGELOG.rst
+-rw-r--r--   0 driesschaumont   (501) staff       (20)     1072 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/LICENSE
+-rw-r--r--   0 driesschaumont   (501) staff       (20)     2466 2023-06-15 20:29:58.916981 sphinx-subprojecttoctree-0.5.3/PKG-INFO
+-rw-r--r--   0 driesschaumont   (501) staff       (20)     1581 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/README.md
+drwxr-xr-x   0 driesschaumont   (501) staff       (20)        0 2023-06-15 20:29:58.908126 sphinx-subprojecttoctree-0.5.3/docs/
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      638 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/docs/Makefile
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      804 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/docs/make.bat
+drwxr-xr-x   0 driesschaumont   (501) staff       (20)        0 2023-06-15 20:29:58.909122 sphinx-subprojecttoctree-0.5.3/docs/source/
+-rw-r--r--   0 driesschaumont   (501) staff       (20)       32 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/docs/source/changelog.rst
+-rw-r--r--   0 driesschaumont   (501) staff       (20)     2443 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/docs/source/conf.py
+drwxr-xr-x   0 driesschaumont   (501) staff       (20)        0 2023-06-15 20:29:58.909325 sphinx-subprojecttoctree-0.5.3/docs/source/images/
+-rwxr-xr-x   0 driesschaumont   (501) staff       (20)   197925 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/docs/source/images/subprojects.png
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      789 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/docs/source/index.rst
+-rw-r--r--   0 driesschaumont   (501) staff       (20)     1006 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/docs/source/installation.rst
+-rw-r--r--   0 driesschaumont   (501) staff       (20)     7518 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/docs/source/userguide.rst
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      363 2022-11-17 17:07:32.000000 sphinx-subprojecttoctree-0.5.3/pyproject.toml
+-rw-r--r--   0 driesschaumont   (501) staff       (20)     1277 2023-06-15 20:29:58.917348 sphinx-subprojecttoctree-0.5.3/setup.cfg
+drwxr-xr-x   0 driesschaumont   (501) staff       (20)        0 2023-06-15 20:29:58.910204 sphinx-subprojecttoctree-0.5.3/sphinx_subprojecttoctree.egg-info/
+-rw-r--r--   0 driesschaumont   (501) staff       (20)     2466 2023-06-15 20:29:58.000000 sphinx-subprojecttoctree-0.5.3/sphinx_subprojecttoctree.egg-info/PKG-INFO
+-rw-r--r--   0 driesschaumont   (501) staff       (20)     2376 2023-06-15 20:29:58.000000 sphinx-subprojecttoctree-0.5.3/sphinx_subprojecttoctree.egg-info/SOURCES.txt
+-rw-r--r--   0 driesschaumont   (501) staff       (20)        1 2023-06-15 20:29:58.000000 sphinx-subprojecttoctree-0.5.3/sphinx_subprojecttoctree.egg-info/dependency_links.txt
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      110 2023-06-15 20:29:58.000000 sphinx-subprojecttoctree-0.5.3/sphinx_subprojecttoctree.egg-info/requires.txt
+-rw-r--r--   0 driesschaumont   (501) staff       (20)       18 2023-06-15 20:29:58.000000 sphinx-subprojecttoctree-0.5.3/sphinx_subprojecttoctree.egg-info/top_level.txt
+drwxr-xr-x   0 driesschaumont   (501) staff       (20)        0 2023-06-15 20:29:58.911163 sphinx-subprojecttoctree-0.5.3/subprojecttoctree/
+-rw-r--r--   0 driesschaumont   (501) staff       (20)     6105 2022-11-10 08:16:46.000000 sphinx-subprojecttoctree-0.5.3/subprojecttoctree/__init__.py
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      160 2023-06-15 20:29:58.000000 sphinx-subprojecttoctree-0.5.3/subprojecttoctree/__version__.py
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      875 2022-11-17 17:07:32.000000 sphinx-subprojecttoctree-0.5.3/subprojecttoctree/builders.py
+-rw-r--r--   0 driesschaumont   (501) staff       (20)     3901 2022-11-10 08:16:46.000000 sphinx-subprojecttoctree-0.5.3/subprojecttoctree/toctree.py
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      979 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/subprojecttoctree/utils.py
+drwxr-xr-x   0 driesschaumont   (501) staff       (20)        0 2023-06-15 20:29:58.911625 sphinx-subprojecttoctree-0.5.3/test/
+-rw-r--r--   0 driesschaumont   (501) staff       (20)     2621 2023-06-15 19:56:27.000000 sphinx-subprojecttoctree-0.5.3/test/conftest.py
+drwxr-xr-x   0 driesschaumont   (501) staff       (20)        0 2023-06-15 20:29:58.905202 sphinx-subprojecttoctree-0.5.3/test/roots/
+drwxr-xr-x   0 driesschaumont   (501) staff       (20)        0 2023-06-15 20:29:58.912541 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-master/
+-rw-r--r--   0 driesschaumont   (501) staff       (20)        7 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-master/bar.rst
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      117 2022-11-10 08:16:46.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-master/conf.py
+-rw-r--r--   0 driesschaumont   (501) staff       (20)        7 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-master/foo.rst
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      136 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-master/index.rst
+drwxr-xr-x   0 driesschaumont   (501) staff       (20)        0 2023-06-15 20:29:58.913584 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-master-entry-after-subproject/
+-rw-r--r--   0 driesschaumont   (501) staff       (20)        7 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-master-entry-after-subproject/bar.rst
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      117 2022-11-10 08:16:46.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-master-entry-after-subproject/conf.py
+-rw-r--r--   0 driesschaumont   (501) staff       (20)        7 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-master-entry-after-subproject/foo.rst
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      147 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-master-entry-after-subproject/index.rst
+-rw-r--r--   0 driesschaumont   (501) staff       (20)       11 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-master-entry-after-subproject/ipsum.rst
+drwxr-xr-x   0 driesschaumont   (501) staff       (20)        0 2023-06-15 20:29:58.914449 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-master-with-regular-http-url/
+-rw-r--r--   0 driesschaumont   (501) staff       (20)        7 2022-11-10 08:16:46.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-master-with-regular-http-url/bar.rst
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      117 2022-11-10 08:16:46.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-master-with-regular-http-url/conf.py
+-rw-r--r--   0 driesschaumont   (501) staff       (20)        7 2022-11-10 08:16:46.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-master-with-regular-http-url/foo.rst
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      170 2022-11-10 08:16:46.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-master-with-regular-http-url/index.rst
+drwxr-xr-x   0 driesschaumont   (501) staff       (20)        0 2023-06-15 20:29:58.915221 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-subproject/
+-rw-r--r--   0 driesschaumont   (501) staff       (20)        7 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-subproject/bar.rst
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      116 2022-11-10 08:16:46.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-subproject/conf.py
+-rw-r--r--   0 driesschaumont   (501) staff       (20)        7 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-subproject/foo.rst
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      101 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-subproject/index.rst
+drwxr-xr-x   0 driesschaumont   (501) staff       (20)        0 2023-06-15 20:29:58.915950 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-subproject-multiple-toctrees/
+-rw-r--r--   0 driesschaumont   (501) staff       (20)        7 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-subproject-multiple-toctrees/bar.rst
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      116 2022-11-10 08:16:46.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-subproject-multiple-toctrees/conf.py
+-rw-r--r--   0 driesschaumont   (501) staff       (20)        7 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-subproject-multiple-toctrees/foo.rst
+-rw-r--r--   0 driesschaumont   (501) staff       (20)       92 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-subproject-multiple-toctrees/index.rst
+drwxr-xr-x   0 driesschaumont   (501) staff       (20)        0 2023-06-15 20:29:58.916710 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-subproject-nested/
+-rw-r--r--   0 driesschaumont   (501) staff       (20)        7 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-subproject-nested/bar.rst
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      116 2022-11-10 08:16:46.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-subproject-nested/conf.py
+-rw-r--r--   0 driesschaumont   (501) staff       (20)        7 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-subproject-nested/foo.rst
+-rw-r--r--   0 driesschaumont   (501) staff       (20)      144 2022-08-23 10:00:39.000000 sphinx-subprojecttoctree-0.5.3/test/roots/test-subprojecttoctree-subproject-nested/index.rst
+-rw-r--r--   0 driesschaumont   (501) staff       (20)    20000 2022-11-10 08:16:46.000000 sphinx-subprojecttoctree-0.5.3/test/test_subprojecttoctree.py
+-rw-r--r--   0 driesschaumont   (501) staff       (20)     1489 2023-06-15 20:22:34.000000 sphinx-subprojecttoctree-0.5.3/tox.ini
```

### Comparing `sphinx-subprojecttoctree-0.5.2/.github/workflows/ci.yml` & `sphinx-subprojecttoctree-0.5.3/.github/workflows/ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     - name: Run tox env ${{ matrix.tox-env }}
       run: tox -e ${{ matrix.tox-env }}
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest]
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
         sphinx-version: ["sphinx44", "sphinx45", "sphinx50", "sphinx51", "sphinx52", "sphinx53"]
         readthedocs-theme-version: [ "theme100", "theme110"]
         sphinxextension: ["on", "off"]
         include:
         - os: macos-latest
           python-version: 3.8
           sphinx-version: sphinx44
```

### Comparing `sphinx-subprojecttoctree-0.5.2/CHANGELOG.rst` & `sphinx-subprojecttoctree-0.5.3/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 
 Changelog
 *********
 
-0.5.3 (in development)
+0.5.4 (in development)
 ----------------------
 
+0.5.3 (15/06/2023)
+------------------
+* Officially support python 3.11 (by adding it to the tests) (:pr:`59`)
+* Add support for sphinx 6.0 (:pr:`63`)
+
 0.5.2 (12/11/2022)
 ------------------
 * Next and previous link now work when the sphinx readthedocs extension (readthedocs-sphinx-ext) is installed (which is the case with online builds) (:issue:`57`)
 
 0.5.1 (11/11/2022)
 ------------------
 * Fixed an issue where the HTML builder was not compatible with the builder from readthedocs-sphinx-ext, causing `AttributeError` when building subprojects on readthedocs (:issue:`55`)
```

### Comparing `sphinx-subprojecttoctree-0.5.2/LICENSE` & `sphinx-subprojecttoctree-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-subprojecttoctree-0.5.2/PKG-INFO` & `sphinx-subprojecttoctree-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-subprojecttoctree
-Version: 0.5.2
+Version: 0.5.3
 Summary: Subprojecttoctrees is a Sphinx extension that aims to facilitate the integration of several documentation sources into a single Read the Docs webpage.
 Home-page: https://sphinx-subprojecttoctree.readthedocs.io
 Author: Dries Schaumont
 Author-email: dries.schaumont@ilvo.vlaanderen.be
 License: MIT
 Project-URL: Changelog, https://sphinx-subprojecttoctree.readthedocs.io/en/latest/changelog.html
 Classifier: Operating System :: OS Independent
```

### Comparing `sphinx-subprojecttoctree-0.5.2/README.md` & `sphinx-subprojecttoctree-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `sphinx-subprojecttoctree-0.5.2/docs/Makefile` & `sphinx-subprojecttoctree-0.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx-subprojecttoctree-0.5.2/docs/make.bat` & `sphinx-subprojecttoctree-0.5.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sphinx-subprojecttoctree-0.5.2/docs/source/conf.py` & `sphinx-subprojecttoctree-0.5.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-subprojecttoctree-0.5.2/docs/source/images/subprojects.png` & `sphinx-subprojecttoctree-0.5.3/docs/source/images/subprojects.png`

 * *Files identical despite different names*

### Comparing `sphinx-subprojecttoctree-0.5.2/docs/source/index.rst` & `sphinx-subprojecttoctree-0.5.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-subprojecttoctree-0.5.2/docs/source/installation.rst` & `sphinx-subprojecttoctree-0.5.3/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `sphinx-subprojecttoctree-0.5.2/docs/source/userguide.rst` & `sphinx-subprojecttoctree-0.5.3/docs/source/userguide.rst`

 * *Files identical despite different names*

### Comparing `sphinx-subprojecttoctree-0.5.2/setup.cfg` & `sphinx-subprojecttoctree-0.5.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -34,22 +34,22 @@
 
 [options]
 python_requires = >=3.8
 setup_requires = 
 	setuptools-scm
 	setuptools_scm_git_archive
 install_requires = 
-	sphinx >= 4.4.0, < 5.4.0
+	sphinx >= 4.4.0,< 7
 	requests ~= 2.27
 packages = 
 	subprojecttoctree
 
 [options.extras_require]
 docs = 
-	sphinx_rtd_theme>=1.0,<1.2
+	sphinx_rtd_theme>=1.0,<1.3
 	sphinx-issues~=3.0.0
 dev = 
 	tox
 	pre-commit
 
 [egg_info]
 tag_build =
```

### Comparing `sphinx-subprojecttoctree-0.5.2/sphinx_subprojecttoctree.egg-info/PKG-INFO` & `sphinx-subprojecttoctree-0.5.3/sphinx_subprojecttoctree.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-subprojecttoctree
-Version: 0.5.2
+Version: 0.5.3
 Summary: Subprojecttoctrees is a Sphinx extension that aims to facilitate the integration of several documentation sources into a single Read the Docs webpage.
 Home-page: https://sphinx-subprojecttoctree.readthedocs.io
 Author: Dries Schaumont
 Author-email: dries.schaumont@ilvo.vlaanderen.be
 License: MIT
 Project-URL: Changelog, https://sphinx-subprojecttoctree.readthedocs.io/en/latest/changelog.html
 Classifier: Operating System :: OS Independent
```

### Comparing `sphinx-subprojecttoctree-0.5.2/sphinx_subprojecttoctree.egg-info/SOURCES.txt` & `sphinx-subprojecttoctree-0.5.3/sphinx_subprojecttoctree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinx-subprojecttoctree-0.5.2/subprojecttoctree/__init__.py` & `sphinx-subprojecttoctree-0.5.3/subprojecttoctree/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-subprojecttoctree-0.5.2/subprojecttoctree/builders.py` & `sphinx-subprojecttoctree-0.5.3/subprojecttoctree/builders.py`

 * *Files identical despite different names*

### Comparing `sphinx-subprojecttoctree-0.5.2/subprojecttoctree/toctree.py` & `sphinx-subprojecttoctree-0.5.3/subprojecttoctree/toctree.py`

 * *Files identical despite different names*

### Comparing `sphinx-subprojecttoctree-0.5.2/subprojecttoctree/utils.py` & `sphinx-subprojecttoctree-0.5.3/subprojecttoctree/utils.py`

 * *Files identical despite different names*

### Comparing `sphinx-subprojecttoctree-0.5.2/test/conftest.py` & `sphinx-subprojecttoctree-0.5.3/test/conftest.py`

 * *Files identical despite different names*

### Comparing `sphinx-subprojecttoctree-0.5.2/test/test_subprojecttoctree.py` & `sphinx-subprojecttoctree-0.5.3/test/test_subprojecttoctree.py`

 * *Files identical despite different names*

### Comparing `sphinx-subprojecttoctree-0.5.2/tox.ini` & `sphinx-subprojecttoctree-0.5.3/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 [tox]
 minversion = 3.24.5
 isolated_build = True
-envlist = py{3.8,3.9,3.10}-sphinx{44,45,50,51,52,53}-theme{100,110}-sphinxextension{off,on},docs,flake8
-
+envlist = 
+    py{3.8,3.9,3.10,3.11}-sphinx{44,45,50,51,52,53}-theme{100,110,120}-sphinxextension{off,on}
+    py{3.8,3.9,3.10,3.11}-sphinx{60,61,62}-theme{120}-sphinxextension{off,on}
+    docs
+    flake8
 
 [testenv]
 deps = 
     sphinx44: sphinx~=4.4.0
     sphinx45: sphinx~=4.5.0
     sphinx50: sphinx~=5.0.0
     sphinx51: sphinx~=5.1.0
     sphinx52: sphinx~=5.2.0
     sphinx53: sphinx~=5.3.0
+    sphinx60: sphinx~=6.0.0
+    sphinx61: sphinx~=6.1.0
+    sphinx62: sphinx~=6.2.0
     theme100: sphinx_rtd_theme~=1.0.0
     theme110: sphinx_rtd_theme~=1.1.0
+    theme120: sphinx_rtd_theme~=1.2.0
     sphinxextensionon: readthedocs-sphinx-ext
     pytest
     pytest-mock
     coverage
 commands =
     coverage run -m pytest --pyargs     
     coverage report
```

