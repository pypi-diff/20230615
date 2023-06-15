# Comparing `tmp/fnattr-0.2.7.tar.gz` & `tmp/fnattr-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnattr-0.2.7.tar", last modified: Mon Jun  5 21:53:09 2023, max compression
+gzip compressed data, was "fnattr-0.2.8.tar", last modified: Thu Jun 15 14:54:49 2023, max compression
```

## Comparing `fnattr-0.2.7.tar` & `fnattr-0.2.8.tar`

### file list

```diff
@@ -1,83 +1,88 @@
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1057 2023-05-06 18:55:15.000000 fnattr-0.2.7/LICENSE
--rw-rw-r--   0 kevin     (1001) dialout     (20)       31 2023-05-07 00:42:08.000000 fnattr-0.2.7/MANIFEST.in
--rw-rw-r--   0 kevin     (1001) dialout     (20)     5174 2023-06-05 21:53:09.000000 fnattr-0.2.7/PKG-INFO
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4523 2023-06-03 16:51:05.000000 fnattr-0.2.7/README.md
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:08.000000 fnattr-0.2.7/config/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1638 2023-05-27 20:42:39.000000 fnattr-0.2.7/config/vlju.toml
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:08.000000 fnattr-0.2.7/doc/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2976 2023-05-31 13:53:09.000000 fnattr-0.2.7/doc/configuration.md
--rw-rw-r--   0 kevin     (1001) dialout     (20)    10407 2023-05-25 00:54:41.000000 fnattr-0.2.7/doc/fna.md
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4501 2023-05-30 12:57:29.000000 fnattr-0.2.7/doc/keys.md
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4647 2023-06-05 20:11:45.000000 fnattr-0.2.7/pyproject.toml
--rw-rw-r--   0 kevin     (1001) dialout     (20)       38 2023-06-05 21:53:09.000000 fnattr-0.2.7/setup.cfg
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:08.000000 fnattr-0.2.7/src/
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:08.000000 fnattr-0.2.7/src/fnattr/
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:08.000000 fnattr-0.2.7/src/fnattr/extra/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     5193 2023-06-03 16:43:56.000000 fnattr-0.2.7/src/fnattr/extra/fnaffle.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4547 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/extra/make_isbn_ranges.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:08.000000 fnattr-0.2.7/src/fnattr/fna/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3961 2023-06-03 16:43:56.000000 fnattr-0.2.7/src/fnattr/fna/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/util/
--rw-rw-r--   0 kevin     (1001) dialout     (20)       23 2023-05-30 23:01:42.000000 fnattr-0.2.7/src/fnattr/util/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      778 2023-05-30 23:01:42.000000 fnattr-0.2.7/src/fnattr/util/checksum.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3735 2023-06-03 16:45:07.000000 fnattr-0.2.7/src/fnattr/util/config.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      625 2023-05-30 23:01:42.000000 fnattr-0.2.7/src/fnattr/util/docsplit.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     9200 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/util/duration.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      102 2023-05-30 23:01:43.000000 fnattr-0.2.7/src/fnattr/util/error.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2181 2023-05-30 23:01:43.000000 fnattr-0.2.7/src/fnattr/util/escape.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1082 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/util/fearmat.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1857 2023-05-30 23:01:43.000000 fnattr-0.2.7/src/fnattr/util/io.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3535 2023-05-30 23:01:43.000000 fnattr-0.2.7/src/fnattr/util/multimap.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1063 2023-05-30 23:01:43.000000 fnattr-0.2.7/src/fnattr/util/pytestutil.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1738 2023-05-30 23:01:43.000000 fnattr-0.2.7/src/fnattr/util/registry.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1099 2023-05-30 23:01:43.000000 fnattr-0.2.7/src/fnattr/util/repr.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     8107 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/util/sqlite.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      438 2023-05-30 23:01:44.000000 fnattr-0.2.7/src/fnattr/util/typecheck.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1797 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      401 2023-05-30 23:01:44.000000 fnattr-0.2.7/src/fnattr/vlju/testutil.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/
--rw-rw-r--   0 kevin     (1001) dialout     (20)       23 2023-05-30 23:01:44.000000 fnattr-0.2.7/src/fnattr/vlju/types/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      920 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/all.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/doi/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4175 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/doi/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)  1136932 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/doi/org.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/ean/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1687 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/ean/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3214 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/ean/isbn.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)    40480 2023-05-30 23:01:45.000000 fnattr-0.2.7/src/fnattr/vlju/types/ean/isbn_ranges.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      666 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/ean/ismn.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1307 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/ean/issn.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/file/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1998 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/file/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/info/
--rw-rw-r--   0 kevin     (1001) dialout     (20)      983 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/info/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2870 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/info/kinds.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/lccn/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1282 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/lccn/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/site/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3990 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/site/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/timestamp/
--rw-rw-r--   0 kevin     (1001) dialout     (20)      888 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/timestamp/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/uri/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     8655 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/uri/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/url/
--rw-rw-r--   0 kevin     (1001) dialout     (20)      772 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/url/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vlju/types/urn/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1372 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/urn/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4046 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vlju/types/urn/kinds.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vljum/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     8666 2023-06-05 17:44:49.000000 fnattr-0.2.7/src/fnattr/vljum/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3007 2023-06-03 16:43:56.000000 fnattr-0.2.7/src/fnattr/vljum/m.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)    10570 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vljum/runner.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:09.000000 fnattr-0.2.7/src/fnattr/vljumap/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1218 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vljumap/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)    22971 2023-06-05 15:10:26.000000 fnattr-0.2.7/src/fnattr/vljumap/enc.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1357 2023-05-30 23:01:46.000000 fnattr-0.2.7/src/fnattr/vljumap/factory.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-05 21:53:08.000000 fnattr-0.2.7/src/fnattr.egg-info/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     5174 2023-06-05 21:53:08.000000 fnattr-0.2.7/src/fnattr.egg-info/PKG-INFO
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1694 2023-06-05 21:53:08.000000 fnattr-0.2.7/src/fnattr.egg-info/SOURCES.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)        1 2023-06-05 21:53:08.000000 fnattr-0.2.7/src/fnattr.egg-info/dependency_links.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)       76 2023-06-05 21:53:08.000000 fnattr-0.2.7/src/fnattr.egg-info/entry_points.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)        7 2023-06-05 21:53:08.000000 fnattr-0.2.7/src/fnattr.egg-info/top_level.txt
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1057 2023-05-06 18:55:15.000000 fnattr-0.2.8/LICENSE
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       31 2023-05-07 00:42:08.000000 fnattr-0.2.8/MANIFEST.in
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5174 2023-06-15 14:54:49.000000 fnattr-0.2.8/PKG-INFO
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4523 2023-06-03 16:51:05.000000 fnattr-0.2.8/README.md
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/config/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1638 2023-05-27 20:42:39.000000 fnattr-0.2.8/config/vlju.toml
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/doc/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2976 2023-05-31 13:53:09.000000 fnattr-0.2.8/doc/configuration.md
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    10407 2023-05-25 00:54:41.000000 fnattr-0.2.8/doc/fna.md
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4501 2023-05-30 12:57:29.000000 fnattr-0.2.8/doc/keys.md
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4685 2023-06-15 14:44:48.000000 fnattr-0.2.8/pyproject.toml
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       38 2023-06-15 14:54:49.000000 fnattr-0.2.8/setup.cfg
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/extra/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/extra/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     6253 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/extra/danname.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     8832 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/extra/fnaffle.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4547 2023-06-08 03:14:19.000000 fnattr-0.2.8/src/fnattr/extra/make_isbn_ranges.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     9356 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/extra/tellico_sqlite3_rename.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/fna/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3788 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/fna/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/util/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       23 2023-05-30 23:01:42.000000 fnattr-0.2.8/src/fnattr/util/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      778 2023-05-30 23:01:42.000000 fnattr-0.2.8/src/fnattr/util/checksum.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4693 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/util/config.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      625 2023-05-30 23:01:42.000000 fnattr-0.2.8/src/fnattr/util/docsplit.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     9200 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/util/duration.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      102 2023-05-30 23:01:43.000000 fnattr-0.2.8/src/fnattr/util/error.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2181 2023-05-30 23:01:43.000000 fnattr-0.2.8/src/fnattr/util/escape.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1243 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/util/fearmat.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1857 2023-05-30 23:01:43.000000 fnattr-0.2.8/src/fnattr/util/io.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      560 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/util/log.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3535 2023-05-30 23:01:43.000000 fnattr-0.2.8/src/fnattr/util/multimap.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2157 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/util/nested.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1063 2023-05-30 23:01:43.000000 fnattr-0.2.8/src/fnattr/util/pytestutil.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1738 2023-05-30 23:01:43.000000 fnattr-0.2.8/src/fnattr/util/registry.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1099 2023-05-30 23:01:43.000000 fnattr-0.2.8/src/fnattr/util/repr.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     8362 2023-06-12 19:21:48.000000 fnattr-0.2.8/src/fnattr/util/sqlite.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      472 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/util/typecheck.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1797 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      401 2023-05-30 23:01:44.000000 fnattr-0.2.8/src/fnattr/vlju/testutil.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       23 2023-05-30 23:01:44.000000 fnattr-0.2.8/src/fnattr/vlju/types/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      920 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/all.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/doi/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4175 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/doi/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)  1136932 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/doi/org.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/ean/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1687 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/ean/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3214 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/ean/isbn.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    40480 2023-05-30 23:01:45.000000 fnattr-0.2.8/src/fnattr/vlju/types/ean/isbn_ranges.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      666 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/ean/ismn.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1307 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/ean/issn.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/file/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1998 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/file/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/info/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      983 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/info/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2870 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/info/kinds.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/lccn/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1282 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/lccn/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/site/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3990 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/site/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/timestamp/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      888 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/timestamp/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/uri/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     8655 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/uri/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/url/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      772 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/url/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/urn/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1372 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/urn/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4046 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/urn/kinds.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vljum/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     9288 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/vljum/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3136 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/vljum/m.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    10570 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vljum/runner.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vljumap/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1218 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vljumap/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    23350 2023-06-12 19:21:48.000000 fnattr-0.2.8/src/fnattr/vljumap/enc.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1357 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vljumap/factory.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr.egg-info/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5174 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr.egg-info/PKG-INFO
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1843 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr.egg-info/SOURCES.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)        1 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr.egg-info/dependency_links.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       76 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr.egg-info/entry_points.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)        7 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr.egg-info/top_level.txt
```

### Comparing `fnattr-0.2.7/LICENSE` & `fnattr-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/PKG-INFO` & `fnattr-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnattr
-Version: 0.2.7
+Version: 0.2.8
 Summary: Manage key/value metadata in file names.
 License: MIT License
 Project-URL: repository, https://codeberg.org/datatravelandexperiments/fna
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fnattr-0.2.7/README.md` & `fnattr-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/config/vlju.toml` & `fnattr-0.2.8/config/vlju.toml`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/doc/configuration.md` & `fnattr-0.2.8/doc/configuration.md`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/doc/fna.md` & `fnattr-0.2.8/doc/fna.md`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/doc/keys.md` & `fnattr-0.2.8/doc/keys.md`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/pyproject.toml` & `fnattr-0.2.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fnattr"
-version = "0.2.7"
+version = "0.2.8"
 description = "Manage key/value metadata in file names."
 license.text = "MIT License"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
@@ -104,14 +104,17 @@
     "C901",     # complex-structure: Be direct.
     "D102",     # undocumented-public-method: Plan to fix eventually.
     "D103",     # undocumented-public-function: Plan to fix eventually.
     "D105",     # undocumented-magic-method: We know what they're for.
     "D107",     # undocumented-public-init: We know what it's for.
     "D203",     # one-blank-line-before-class: Conflicts with D211.
     "D212",     # multi-line-summary-first-line: Conflicts with D213.
+    "PD",       # pandas-vet: Not using Pandas.
+    "PLR0911",  # too-many-return-statements: Be direct.
+    "PLR0912",  # too-many-branches: Be direct.
     "PLR0912",  # too-many-branches: Be direct.
     "PLR0913",  # too-many-arguments: Be direct.
     "PLR2004",  # magic-value-comparison: Be direct.
     "S314", 	# suspicious-xml-element-tree-usage: defusedxml is not builtin.
     "T20",      # flake8-print: I like having output.
     "TRY400",   # error-instead-of-exception: Don't dump traces on end users.
 ]
@@ -149,17 +152,14 @@
 column_limit = 80
 dedent_closing_brackets = false
 each_dict_entry_on_separate_line = true
 indent_dictionary_value = true
 join_multiple_lines = false
 spaces_around_default_or_named_assign = false
 spaces_around_subscript_colon = true
-spaces_before_comment = [
-    13, 17, 21, 25, 29, 33, 37, 41, 45, 49, 53, 57, 61, 65, 69
-]
-split_all_top_level_comma_separated_values = true
+spaces_before_comment = 2
 split_before_bitwise_operator = true
 split_before_arithmetic_operator = true
 split_before_dot = true
 split_before_expression_after_opening_paren = true
 split_before_logical_operator = true
 split_complex_comprehension = true
```

### Comparing `fnattr-0.2.7/src/fnattr/extra/fnaffle.py` & `fnattr-0.2.8/src/fnattr/util/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,180 +1,136 @@
 # SPDX-License-Identifier: MIT
-"""Move files to directories based on matching attributes."""
+"""Configuration-file related utilities."""
 
 import argparse
+import contextlib
 import logging
-import sys
+import os
+import tomllib
 
-from collections.abc import Iterable
+from collections.abc import Iterable, Mapping
 from pathlib import Path
+from typing import Any, Self
 
-from fnattr.util.config import read_cmd_configs, xdg_config
-from fnattr.vljum.m import M
-from fnattr.vljumap import enc
-
-def find_map_files(cmd: str) -> list[Path]:
-    return [
-        f for f in (xdg_config('vlju/fnaffle.map'),
-                    xdg_config(f'{cmd}/fnaffle.map'),
-                    Path('fnaffle.map'),
-                    Path('.fnaffle')) if f is not None and f.exists()
-    ]
+from fnattr.util import nested
 
-Maps = list[tuple[Path, str, dict]]
+class Dirs(list[Path]):
+    """Maintain a list of directories."""
 
-def read_map_files(files: Iterable[Path | str]) -> Maps:
-    maps: Maps = []
-    for file in files:
-        maps += read_map_file(file)
-    return maps
-
-def read_map_file(file: Path | str) -> Maps:
-    maps = []
-    with Path(file).open(encoding='utf-8') as f:
-        while line := f.readline():
-            dst, op, encoding = line.strip().split(None, 2)
-            m = M().decode(encoding, 'v3')
-            target = sorted_strings(m)
-            maps.append((Path(dst), op, target))
-    return maps
-
-StringListDict = dict[str, list[str]]
-
-def sorted_strings(m: M) -> StringListDict:
-    d = {}
-    for k in sorted(m.keys()):
-        d[k] = sorted(str(v) for v in m[k])
+    def add_env_dir(self, evar: str, default: Path | None = None) -> Self:
+        """
+        Add an environment-variable-based or default directory.
+
+        Based on XDG conventions. If the environment variable named `evar`
+        exists and contains a directory path, add it; otherwise, if the
+        `default` exists, add that.
+        """
+        if evar in os.environ:
+            p = Path(os.environ[evar])
+            if p.is_dir():
+                self.append(p)
+        elif default and default.is_dir():
+            self.append(default)
+        return self
+
+    def add_env_dirs(self, env: str, default: list[Path]) -> Self:
+        """
+        Add a list of environment-variable-based or default directories.
+
+        Based on XDG conventions. If the environment variable named `evar`
+        exists, treat it as a `:`-separated path and add any existing absolute
+        directory. Otherwise, add any existing directory in `default`.
+        """
+        if env in os.environ:
+            for d in os.environ[env].split(':'):
+                p = Path(d)
+                if p.is_dir() and p.is_absolute():
+                    self.append(p)
+        else:
+            for p in default:
+                if p.is_dir():
+                    self.append(p)
+        return self
+
+    def find_first(self, p: Path | str) -> Path | None:
+        """Return the first matching file in the directory list."""
+        for i in self:
+            d = i / p
+            if d.exists():
+                return d
+        return None
+
+def xdg_dirs(name: str,
+             default_dir: str,
+             default_paths: list[Path],
+             home: Path | None = None) -> Dirs:
+    """Obtain a list of XDG directories of the given kind."""
+    if home is None:
+        with contextlib.suppress(RuntimeError):
+            home = Path.home()
+
+    default_path = None if home is None else home / default_dir
+    d = Dirs()
+    d.add_env_dir(f'XDG_{name}_HOME', default_path)
+    d.add_env_dirs(f'XDG_{name}_DIRS', default_paths)
     return d
 
-def compare_sorted_lists(a: list, b: list) -> str:
-    r = 3
-    an = len(a)
-    bn = len(b)
-    ai = 0
-    bi = 0
-    while ai < an and bi < bn and r:
-        if a[ai] < b[bi]:
-            r &= ~1
-            ai += 1
-            continue
-        if a[ai] > b[bi]:
-            r &= ~2
-            bi += 1
-            continue
-        ai += 1
-        bi += 1
-    if (r & 1) and ai < an:
-        r &= ~1
-    if (r & 2) and bi < bn:
-        r &= ~2
-    return ['≠', '⊂', '⊃', '='][r]
-
-def match_map(op: str, source: StringListDict, target: StringListDict) -> bool:
-    ok = {
-        '⊆': ('⊂', '='),
-        '⊇': ('⊃', '='),
-    }.get(op, (op, ))
-    for k, v in target.items():
-        if not (s := source.get(k)):
-            return False
-        r = compare_sorted_lists(s, v)
-        if r not in ok:
-            return False
-    return True
-
-def match_maps(maps: Maps, m: M) -> Path | None:
-    source = sorted_strings(m)
-    for dst, op, target in maps:
-        if match_map(op, source, target):
-            return dst
-    return None
-
-def main(argv: list[str] | None = None) -> int:
-    if argv is None:
-        argv = sys.argv
-    cmd = Path(argv[0]).stem
-    parser = argparse.ArgumentParser(
-        prog=cmd, description='Move files according to file name attributes')
-    parser.add_argument(
-        '--config',
-        '-c',
-        metavar='FILE',
-        type=str,
-        action='append',
-        help='Configuration file.')
-    parser.add_argument(
-        '--decoder',
-        '-d',
-        metavar='DECODER',
-        type=str,
-        choices=enc.decoder.keys(),
-        help='Default string decoder.')
-    parser.add_argument(
-        '--dryrun',
-        '-n',
-        default=False,
-        action='store_true',
-        help='Do not actually rename.')
-    parser.add_argument(
-        '--map',
-        '-m',
-        metavar='FILE',
-        type=str,
-        action='append',
-        help='Renaming map file.')
-    parser.add_argument(
-        '--log-level',
-        '-L',
-        metavar='LEVEL',
-        type=str,
-        choices=[c for c in logging.getLevelNamesMapping() if c != 'NOTSET'],
-        default='INFO')
-    parser.add_argument(
-        'file',
-        metavar='FILENAME',
-        type=str,
-        nargs=argparse.REMAINDER,
-        default=[],
-        help='File name(s).')
-    args = parser.parse_args(argv[1 :])
-    logging.basicConfig(level=getattr(logging, args.log_level.upper()),
-                        format=f'{cmd}: %(levelname)s: %(message)s')
-
-    config = read_cmd_configs(cmd, args.config)
-    options = config.get('option', {})
-    if args.decoder:
-        options['decoder'] = args.decoder
-    M.configure_options(options)
-    M.configure_sites(config.get('site', {}))
-
-    try:
-        if not args.map:
-            args.map = find_map_files(cmd)
-        if not args.map:
-            logging.error('%s: no map file', cmd)
-            return 1
-        maps = read_map_files(args.map)
-        for file in args.file:
-            m = M().file(file)
-            if dst := match_maps(maps, m):
-                if not dst.exists():
-                    if not args.dryrun:
-                        dst.mkdir(parents=True)
-                    logging.info('%s: created', dst)
-                if not args.dryrun:
-                    try:
-                        m.with_dir(dst).rename()
-                    except FileExistsError:
-                        logging.error('file exists: %s', file)
-                if args.dryrun or args.verbose:
-                    print(f'{dst}: {file}')
-            elif args.verbose:
-                print(f'no match for {file}')
-    except Exception as e:
-        logging.error('Unhandled exception: %s%s', type(e).__name__, e.args)
-        if logging.getLogger().getEffectiveLevel() < logging.INFO:
-            raise
-    return 0
+def xdg_config_dirs() -> Dirs:
+    return xdg_dirs('CONFIG', '.config', [Path('/etc/xdg')])
+
+def xdg_config(filename: Path | str) -> Path | None:
+    return xdg_config_dirs().find_first(filename)
 
-if __name__ == '__main__':
-    sys.exit(main())
+def read_toml_config(file: Path | str) -> dict | None:
+    with Path(file).open('rb') as f:
+        try:
+            return tomllib.load(f)
+        except tomllib.TOMLDecodeError as e:
+            logging.error('%s: %s', file, str(e))
+            return None
+
+def read_configs(args: Iterable[Path | str]) -> dict:
+    config: dict[str, Any] = {}
+    for p in args:
+        if c := read_toml_config(p):
+            nested.nupdate(config, c)
+    return config
+
+def read_xdg_configs(files: Iterable[Path]) -> dict:
+    config: dict[str, Any] = {}
+    for file in files:
+        if (cf := xdg_config(file)) and (c := read_toml_config(cf)):
+            nested.nupdate(config, c)
+    return config
+
+def read_cmd_configs(cmds: str | Iterable[str],
+                     config_files: Iterable[Path | str]) -> dict:
+    paths = []
+    names = ['vlju', cmds] if isinstance(cmds, str) else ['vlju', *cmds]
+    for i in names:
+        paths.append(Path(f'{i}.toml'))
+        paths.append(Path(f'fnattr/{i}.toml'))
+    config = read_xdg_configs(paths)
+    if config_files:
+        nested.nupdate(config, read_configs(config_files))
+    return config
+
+def merge_options(options: dict[str, Any] | None, args: argparse.Namespace,
+                  **kwargs) -> dict[str, Any]:
+    if options is None:
+        options = {}
+    for k, d in kwargs.items():
+        option = d.get('option', k) if isinstance(d, Mapping) else k
+        default = d.get('default') if isinstance(d, Mapping) else d
+        if (a := getattr(args, k)) is not None:
+            nested.dset(options, option, a)
+        elif k not in options and default is not None:
+            nested.dset(options, option, default)
+    return options
+
+def read_cmd_configs_and_merge_options(cmds: str | Iterable[str],
+                                       config_files: Iterable[Path | str],
+                                       args: argparse.Namespace,
+                                       **kwargs) -> tuple[dict, dict]:
+    config = read_cmd_configs(cmds, config_files)
+    options = merge_options(config.get('option'), args, **kwargs)
+    return config, options
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fnattr-0.2.7/src/fnattr/extra/make_isbn_ranges.py` & `fnattr-0.2.8/src/fnattr/extra/make_isbn_ranges.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/fna/__init__.py` & `fnattr-0.2.8/src/fnattr/fna/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import argparse
 import logging
 import pathlib
 import sys
 
 import fnattr.util.config
 import fnattr.util.io
+import fnattr.util.log
 import fnattr.vljum.m
 import fnattr.vljum.runner
 import fnattr.vljumap.enc
 
 def main(argv: list[str] | None = None) -> int:
     if argv is None:
         argv = sys.argv
@@ -44,16 +45,16 @@
         choices=fnattr.vljumap.enc.encoder.keys(),
         help='Default string encoder.')
     parser.add_argument(
         '--log-level',
         '-L',
         metavar='LEVEL',
         type=str,
-        choices=[c for c in logging.getLevelNamesMapping() if c != 'NOTSET'],
-        default='INFO')
+        choices=fnattr.util.log.CHOICES,
+        default='WARNING')
     mode = parser.add_mutually_exclusive_group()
     mode.add_argument(
         '--dsl',
         '-D',
         dest='mode',
         default='dsl',
         const='dsl',
@@ -85,23 +86,23 @@
         metavar='ARGUMENT',
         type=str,
         nargs=argparse.REMAINDER,
         default=[],
         help='Part of a subcommand, or an expression or statement.')
     args = parser.parse_args(argv[1 :])
 
-    logging.basicConfig(level=getattr(logging, args.log_level.upper()),
-                        format=f'{cmd}: %(levelname)s: %(message)s')
+    log.level(cmd, args.log_level)
 
-    config = fnattr.util.config.read_cmd_configs(cmd, args.config)
-    options = config.get('option', {})
-    if args.decoder:
-        options['decoder'] = args.decoder
-    if args.encoder:
-        options['encoder'] = args.encoder
+    config, options = fnattr.util.config.read_cmd_configs_and_merge_options(
+        cmd,
+        args.config,
+        args,
+        decoder='v3',
+        encoder='v3',
+    )
     fnattr.vljum.m.M.configure_options(options)
     fnattr.vljum.m.M.configure_sites(config.get('site', {}))
 
     try:
         match args.mode:
             case 'dsl':
                 fnattr.vljum.runner.Runner().run(args.argument)
@@ -119,11 +120,12 @@
                         fnattr.vljum.m.M.execute(f.read())
             case _:
                 logging.error('Unknown mode: %s', args.mode)
     except Exception as e:
         logging.error('Unhandled exception: %s%s', type(e).__name__, e.args)
         if logging.getLogger().getEffectiveLevel() < logging.INFO:
             raise
+
     return 0
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `fnattr-0.2.7/src/fnattr/util/checksum.py` & `fnattr-0.2.8/src/fnattr/util/checksum.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/util/docsplit.py` & `fnattr-0.2.8/src/fnattr/util/docsplit.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/util/duration.py` & `fnattr-0.2.8/src/fnattr/util/duration.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/util/escape.py` & `fnattr-0.2.8/src/fnattr/util/escape.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/util/fearmat.py` & `fnattr-0.2.8/src/fnattr/util/fearmat.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-License-Identifier: MIT
 """Like format, but scary."""
 
+import builtins
 import operator
 
 from collections.abc import Mapping
 from typing import Any
 
 from fnattr.util.error import Error
 
@@ -34,15 +35,15 @@
 )
 ALLOWED_OPERATORS = (
     'add',
     'sub',
 )
 
 BUILTINS = {
-    k: globals()['__builtins__'][k]
+    k: getattr(builtins, k)
     for k in ALLOWED_BUILTINS
 } | {
     k: getattr(operator, k)
     for k in ALLOWED_OPERATORS
 }
 
 def fearmat(template: str,
@@ -50,9 +51,14 @@
             builtins: Mapping[str, Any] | None = None) -> str:
     if '"""' in template:
         msg = '‘"""’ in ‘template’'
         raise Error(msg)
     template = 'f"""' + template + '"""'
     if builtins is None:
         builtins = BUILTINS
+    return str(evaluate(template, values, builtins))
+
+def evaluate(s: str,
+             values: Mapping[str, Any],
+             builtins: Mapping[str, Any]) -> Any:
     g = dict(values) | {'__builtins__': builtins}
-    return str(eval(template, g))   # noqa: PGH001, eval-used
+    return eval(s, g)   # noqa: PGH001, eval-used
```

### Comparing `fnattr-0.2.7/src/fnattr/util/io.py` & `fnattr-0.2.8/src/fnattr/util/io.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/util/multimap.py` & `fnattr-0.2.8/src/fnattr/util/multimap.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/util/pytestutil.py` & `fnattr-0.2.8/src/fnattr/util/pytestutil.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/util/registry.py` & `fnattr-0.2.8/src/fnattr/util/registry.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/util/repr.py` & `fnattr-0.2.8/src/fnattr/util/repr.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/util/sqlite.py` & `fnattr-0.2.8/src/fnattr/util/sqlite.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 class SQLite:
     """Wrapper including context manager for sqlite3."""
 
     # These are intended for subclasses to provide initialization for all
     # instances of the subclasses. The model is that a subclass defines a
     # database including a schema definition as its `on_create`.
-    on_connect: Iterable[str] | None = None
     on_create: Iterable[str] | None = None
+    on_connect: Iterable[str] | None = None
+    foreign_keys: bool | None = True
 
     def __init__(self,
                  filename: PathLike = '',
                  mode: str = '',
                  **kwargs) -> None:
         if not mode:
             mode = 'ro' if filename else 'rw'
@@ -46,14 +47,17 @@
     def __enter__(self) -> Self:
         return self.connect()
 
     def connect(self) -> Self:
         """Open and initialize the database connection."""
         if not self._connection:
             self._connection, created = self._open()
+            if self.foreign_keys is not None:
+                self._connection.execute(
+                    f'PRAGMA foreign_keys = {int(self.foreign_keys)};')
             if self.on_connect:
                 for i in self.on_connect:
                     self._connection.execute(i)
             if created and self.on_create:
                 for i in self.on_create:
                     self._connection.execute(i)
         return self
@@ -195,21 +199,23 @@
             if c not in table_columns:
                 message = f'column {c!r} does not exist in {table!r}'
                 raise sqlite3.ProgrammingError(message)
 
     def _init_table_column_cache(self) -> None:
         c = self.connection().execute(
             'SELECT name FROM sqlite_master WHERE type == "table"')
+        c.row_factory = None
         while (row := c.fetchone()):
             table = row[0]
             self._table_columns[table] = None
 
     def _load_table_column_cache(self, table: str) -> list[str]:
         r = []
         c = self.connection().execute(f'PRAGMA TABLE_INFO({quote_id(table)})')
+        c.row_factory = None
         while (row := c.fetchone()):
             column = row[1]
             r.append(column)
         self._table_columns[table] = r
         return r
 
     def clear_table_column_cache(self) -> None:
```

### Comparing `fnattr-0.2.7/src/fnattr/vlju/__init__.py` & `fnattr-0.2.8/src/fnattr/vlju/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/vlju/types/all.py` & `fnattr-0.2.8/src/fnattr/vlju/types/all.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/vlju/types/doi/__init__.py` & `fnattr-0.2.8/src/fnattr/vlju/types/doi/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/vlju/types/doi/org.py` & `fnattr-0.2.8/src/fnattr/vlju/types/doi/org.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/vlju/types/ean/__init__.py` & `fnattr-0.2.8/src/fnattr/vlju/types/ean/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/vlju/types/ean/isbn.py` & `fnattr-0.2.8/src/fnattr/vlju/types/ean/isbn.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/vlju/types/ean/isbn_ranges.py` & `fnattr-0.2.8/src/fnattr/vlju/types/ean/isbn_ranges.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/vlju/types/ean/ismn.py` & `fnattr-0.2.8/src/fnattr/vlju/types/ean/ismn.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/vlju/types/ean/issn.py` & `fnattr-0.2.8/src/fnattr/vlju/types/ean/issn.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/vlju/types/file/__init__.py` & `fnattr-0.2.8/src/fnattr/vlju/types/file/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/vlju/types/info/__init__.py` & `fnattr-0.2.8/src/fnattr/vlju/types/info/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/vlju/types/info/kinds.py` & `fnattr-0.2.8/src/fnattr/vlju/types/info/kinds.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/vlju/types/lccn/__init__.py` & `fnattr-0.2.8/src/fnattr/vlju/types/lccn/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/vlju/types/site/__init__.py` & `fnattr-0.2.8/src/fnattr/vlju/types/site/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/vlju/types/timestamp/__init__.py` & `fnattr-0.2.8/src/fnattr/vlju/types/timestamp/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/vlju/types/uri/__init__.py` & `fnattr-0.2.8/src/fnattr/vlju/types/uri/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/vlju/types/url/__init__.py` & `fnattr-0.2.8/src/fnattr/vlju/types/url/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/vlju/types/urn/__init__.py` & `fnattr-0.2.8/src/fnattr/vlju/types/urn/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/vlju/types/urn/kinds.py` & `fnattr-0.2.8/src/fnattr/vlju/types/urn/kinds.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/vljum/__init__.py` & `fnattr-0.2.8/src/fnattr/vljum/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # SPDX-License-Identifier: MIT
 """VljuMap operations."""
 
 import copy
+import filecmp
+import logging
 import re
 import sys
 
 from collections import defaultdict
 from collections.abc import Mapping, MutableMapping
 from pathlib import Path
 from typing import Any, Self, TextIO
@@ -81,53 +83,69 @@
         return self.submap(args)
 
     def file(self,
              s: str | Path,
              decoder: EncoderArg = None,
              factory: FactoryArg = None) -> Self:
         self.set_path(s)
-        r = self.decoder.get(decoder).decode_file(self,
-                                                  self._original_path,
+        r = self.decoder.get(decoder).decode_file(self, self._original_path,
                                                   self.factory.get(factory))
         self._current_dir = r.directory
         self._current_suffix = r.suffix
         return self
 
     def order(self, *args: str) -> Self:
         return self.sortkeys(args or None)
 
     def read(self,
              file: PathLike = '-',
              decoder: EncoderArg = None,
              factory: FactoryArg = None) -> Self:
         with open_input(file, sys.stdin) as f:
-            self.decoder.get(decoder).decode(self,
-                                             f.read(),
+            self.decoder.get(decoder).decode(self, f.read(),
                                              self.factory.get(factory))
         return self
 
     def remove(self,
                k: str,
                v: VljuArg = None,
                factory: FactoryArg = None) -> Self:
         if v is None:
             del self[k]
             return self
         super().remove(k, self._vlju(k, v, factory))
         return self
 
-    def rename(self, encoder: EncoderArg = None, mode: ModeArg = None) -> Self:
+    def rename(self,
+               encoder: EncoderArg = None,
+               mode: ModeArg = None,
+               *,
+               mkdir: bool = True,
+               dedup: bool = False,
+               dryrun: bool = False) -> Self:
         if self._original_path == Path():
             message = 'no file to rename'
             raise Error(message)
         modified_path = self.filename(encoder, self.mode.get(mode))
+        logging.info('rename: %s', self._original_path)
+        logging.info('    to: %s', modified_path)
+        if dryrun:
+            return self
         if modified_path.exists():
             if modified_path.samefile(self._original_path):
+                logging.info('same file')
+                return self
+            if dedup and filecmp.cmp(
+                    self._original_path, modified_path, shallow=False):
+                logging.info('removing duplicate')
+                self._original_path.unlink()
                 return self
             raise FileExistsError(modified_path)
+        if mkdir and not modified_path.parent.exists():
+            modified_path.parent.mkdir(parents=True)
         self._original_path.rename(modified_path)
         self.set_path(modified_path)
         return self
 
     def reset(self,
               k: str,
               v: VljuArg = None,
@@ -153,15 +171,15 @@
               file: PathLike = '-',
               encoder: EncoderArg = None,
               mode: ModeArg = None) -> Self:
         with open_output(file, sys.stdout) as f:
             f.write(self.encoder.get(encoder).encode(self, self.mode.get(mode)))
         return self
 
-    def z(self, file: TextIO = sys.stderr) -> Self:     # pragma: no coverage
+    def z(self, file: TextIO = sys.stderr) -> Self:  # pragma: no coverage
         print(repr(self), file=file)
         return self
 
     # String reductions.
 
     def __str__(self) -> str:
         return str(self.filename())
```

### Comparing `fnattr-0.2.7/src/fnattr/vljum/m.py` & `fnattr-0.2.8/src/fnattr/vljum/m.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,25 +66,29 @@
             x[k] = v
             x[v.__name__] = v
         return x
 
     @classmethod
     def evaluate(cls,
                  s: str,
-                 g: dict[str, Any] | None = None) -> Any:   # noqa: any-type
-        if g is None:
-            g = cls.exports()
-        return eval(s, g)                                   # noqa: eval
+                 glo: dict[str, Any] | None = None,
+                 loc: dict[str, Any] | None = None) -> Any:  # noqa: any-type
+        if glo is None:
+            glo = cls.exports()
+        return eval(s, glo, loc)  # noqa: eval
 
     @classmethod
-    def execute(cls, s: str, g: dict[str, Any] | None = None) -> dict[str, Any]:
-        if g is None:
-            g = cls.exports()
-        exec(s, g)  # noqa: exec-builtin
-        return g
+    def execute(cls,
+                s: str,
+                glo: dict[str, Any] | None = None,
+                loc: dict[str, Any] | None = None) -> dict[str, Any]:
+        if glo is None:
+            glo = cls.exports()
+        exec(s, glo, loc)  # noqa: exec-builtin
+        return glo
 
 def _make_free_function(cls: type, name: str) -> Callable:
     method = getattr(cls, name)
 
     def f(*args, **kwargs) -> Any:  # noqa: ANN401
         return method(cls(), *args, **kwargs)
```

### Comparing `fnattr-0.2.7/src/fnattr/vljum/runner.py` & `fnattr-0.2.8/src/fnattr/vljum/runner.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/vljumap/__init__.py` & `fnattr-0.2.8/src/fnattr/vljumap/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr/vljumap/enc.py` & `fnattr-0.2.8/src/fnattr/vljumap/enc.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """Encode and decode VljuMap."""
 
 import csv as py_csv
 import io
 import json as py_json
 import re
 import shlex
+import urllib.parse
 import warnings
 
 from collections.abc import Callable, Generator, Iterable
 from dataclasses import dataclass
 from pathlib import Path
 from typing import NamedTuple
 
@@ -121,15 +122,18 @@
     attr_join: str = '; '
     attr_kv: str = '='
     title_join: str = ' - '
     seq_start: str = ''
     seq_end: str = '.'
     seq_join: str = '.'
 
-V3_CONFIG = V3Config(quote=escape.unixfile)
+V3_CONFIG = V3Config(
+    quote=escape.Escape(
+        escape.mkencode_urlish(escape.UNSAFE_ON_UNIX
+                               + '[];='), urllib.parse.unquote))
 
 def v3_encode(n: VljuMap, mode: str | None = None) -> str:
     return _v3_enc(V3_CONFIG, n, mode)
 
 def v3_decode(n: VljuMap, s: str, factory: VljuFactory) -> VljuMap:
     return _v3_dec(V3_CONFIG, n, s, factory)
 
@@ -153,16 +157,17 @@
     sequence = sequence and f'{config.seq_start}{sequence}{config.seq_end}'
     title_qjoin = config.title_join.translate(
         escape.mktrans_urlish(config.title_join.strip()))
     title = config.title_join.join(
         config.quote.encode(i).replace(config.title_join, title_qjoin)
         for i in m['title'])
     attrs = config.attr_join.join(
-        kv_fmt(k, v, config.attr_kv, config.quote) for k,
-        v in m.pairs() if k not in ('title', 'n'))
+        kv_fmt(k, v, config.attr_kv, config.quote)
+        for k, v in m.pairs()
+        if k not in ('title', 'n'))
     attrs = attrs and f'{config.attr_start}{attrs}{config.attr_end}'
     return join_non_empty(' ', sequence, title, attrs)
 
 def _v3_dec_file(config: V3Config, n: VljuMap, p: Path,
                  factory: VljuFactory) -> DecodeFileResult:
     bad_suffix = (
         config.attr_end in p.suffix
@@ -245,15 +250,18 @@
 
 WIN_DESC = 'Like v3, but escape Windows forbidden characters.'
 WIN_DESCRIPTION = """
   This is the same as v3 encoding format, except that additional characters
   are URL-escaped to comply with Windows file name limitations.
 """
 
-WIN_CONFIG = V3Config(quote=escape.winfile)
+WIN_CONFIG = V3Config(
+    quote=escape.Escape(
+        escape.mkencode_urlish(escape.UNSAFE_ON_WINDOWS
+                               + '[];='), urllib.parse.unquote))
 
 def win_encode(n: VljuMap, mode: str | None = None) -> str:
     return _v3_enc(WIN_CONFIG, n, mode)
 
 def win_decode(n: VljuMap, s: str, factory: VljuFactory) -> VljuMap:
     return _v3_dec(WIN_CONFIG, n, s, factory)
 
@@ -294,15 +302,20 @@
   Encoder format v2 is similar to v3, except that attributes are surrounded
   by ‘{ … }' rather than ‘[ … ]’, and separated by semicolons with no space.
 
   This is supported only to covert old file names.
 """ + V2_GRAMMAR
 
 V2_CONFIG = V3Config(
-    quote=escape.unixfile, attr_start='{', attr_join=';', attr_end='}')
+    quote=escape.Escape(
+        escape.mkencode_urlish(escape.UNSAFE_ON_UNIX + '{};='),
+        urllib.parse.unquote),
+    attr_start='{',
+    attr_join=';',
+    attr_end='}')
 
 def v2_encode(n: VljuMap, mode: str | None = None) -> str:
     return _v3_enc(V2_CONFIG, n, mode)
 
 def v2_decode(n: VljuMap, s: str, factory: VljuFactory) -> VljuMap:
     return _v3_dec(V2_CONFIG, n, s, factory)
 
@@ -353,16 +366,17 @@
 V1_CONFIG = V3Config(
     escape.unixfile, attr_start='[', attr_end=']', attr_join=',')
 
 def v1_encode(n: VljuMap, mode: str | None = None) -> str:
     m = n.to_strings(mode)
     r = _v1_enc_author_title(m)
     attrs = ','.join(
-        kv_fmt(k, v, '=', escape.unixfile) for k,
-        v in m.pairs() if k not in ('title', 'a'))
+        kv_fmt(k, v, '=', escape.unixfile)
+        for k, v in m.pairs()
+        if k not in ('title', 'a'))
     return spj(r, f'[{attrs}]') if attrs else r
 
 def v1_decode(n: VljuMap, s: str, factory: VljuFactory) -> VljuMap:
     return n.add_pairs(_v1_dec_iter(V1_CONFIG, s), factory)
 
 v1 = _register_encoder(
     Encoder(
@@ -431,16 +445,15 @@
 V0_RE = re.compile(
     r"""
         (?P<rest>.*)
         \b(?:
             (?P<isbn> (?: [0-9]{13} | [0-9]{9}[0-9xX] ) )
         | lccn=(?P<lccn> \S+ )
         )$
-        """,
-    re.VERBOSE)
+        """, re.VERBOSE)
 
 def _v0_dec_iter(s: str) -> Generator[tuple[str, str], None, None]:
     if m := V0_RE.fullmatch(s):
         s = m.group('rest')
     yield from _v1_dec_author_title(s)
     if m:
         if isbn := m.group('isbn'):
@@ -508,16 +521,15 @@
 SFC_TAIL_RE = re.compile(
     r"""
         (?P<prefix> .*)
         (?:
             (?P<date> [12]\d\d\d ) |
             (?: (?P<edition> \d+ ) \w*\s+edition )
         )$
-        """,
-    re.X)
+        """, re.X)
 
 def _sfc_dec_iter(s: str) -> Generator[tuple[str, str], None, None]:
     while True:
         if m := SFC_TAIL_RE.fullmatch(s):
             for k in ('date', 'edition'):
                 if v := m.group(k):
                     yield (k, v)
```

### Comparing `fnattr-0.2.7/src/fnattr/vljumap/factory.py` & `fnattr-0.2.8/src/fnattr/vljumap/factory.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.7/src/fnattr.egg-info/PKG-INFO` & `fnattr-0.2.8/src/fnattr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnattr
-Version: 0.2.7
+Version: 0.2.8
 Summary: Manage key/value metadata in file names.
 License: MIT License
 Project-URL: repository, https://codeberg.org/datatravelandexperiments/fna
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fnattr-0.2.7/src/fnattr.egg-info/SOURCES.txt` & `fnattr-0.2.8/src/fnattr.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,27 +7,32 @@
 doc/fna.md
 doc/keys.md
 src/fnattr.egg-info/PKG-INFO
 src/fnattr.egg-info/SOURCES.txt
 src/fnattr.egg-info/dependency_links.txt
 src/fnattr.egg-info/entry_points.txt
 src/fnattr.egg-info/top_level.txt
+src/fnattr/extra/__init__.py
+src/fnattr/extra/danname.py
 src/fnattr/extra/fnaffle.py
 src/fnattr/extra/make_isbn_ranges.py
+src/fnattr/extra/tellico_sqlite3_rename.py
 src/fnattr/fna/__init__.py
 src/fnattr/util/__init__.py
 src/fnattr/util/checksum.py
 src/fnattr/util/config.py
 src/fnattr/util/docsplit.py
 src/fnattr/util/duration.py
 src/fnattr/util/error.py
 src/fnattr/util/escape.py
 src/fnattr/util/fearmat.py
 src/fnattr/util/io.py
+src/fnattr/util/log.py
 src/fnattr/util/multimap.py
+src/fnattr/util/nested.py
 src/fnattr/util/pytestutil.py
 src/fnattr/util/registry.py
 src/fnattr/util/repr.py
 src/fnattr/util/sqlite.py
 src/fnattr/util/typecheck.py
 src/fnattr/vlju/__init__.py
 src/fnattr/vlju/testutil.py
```

