# Comparing `tmp/dushyanth-1.0.3.tar.gz` & `tmp/dushyanth-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dushyanth-1.0.3.tar", last modified: Thu Jun 15 15:20:48 2023, max compression
+gzip compressed data, was "dushyanth-1.0.4.tar", last modified: Thu Jun 15 15:28:26 2023, max compression
```

## Comparing `dushyanth-1.0.3.tar` & `dushyanth-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 dboppidi   (501) staff       (20)        0 2023-06-15 15:20:48.377268 dushyanth-1.0.3/
--rw-r--r--   0 dboppidi   (501) staff       (20)      304 2023-06-15 15:20:48.377142 dushyanth-1.0.3/PKG-INFO
-drwxr-xr-x   0 dboppidi   (501) staff       (20)        0 2023-06-15 15:20:48.376661 dushyanth-1.0.3/dushyanth.egg-info/
--rw-r--r--   0 dboppidi   (501) staff       (20)      304 2023-06-15 15:20:48.000000 dushyanth-1.0.3/dushyanth.egg-info/PKG-INFO
--rw-r--r--   0 dboppidi   (501) staff       (20)      229 2023-06-15 15:20:48.000000 dushyanth-1.0.3/dushyanth.egg-info/SOURCES.txt
--rw-r--r--   0 dboppidi   (501) staff       (20)        1 2023-06-15 15:20:48.000000 dushyanth-1.0.3/dushyanth.egg-info/dependency_links.txt
--rw-r--r--   0 dboppidi   (501) staff       (20)       24 2023-06-15 15:20:48.000000 dushyanth-1.0.3/dushyanth.egg-info/requires.txt
--rw-r--r--   0 dboppidi   (501) staff       (20)       14 2023-06-15 15:20:48.000000 dushyanth-1.0.3/dushyanth.egg-info/top_level.txt
-drwxr-xr-x   0 dboppidi   (501) staff       (20)        0 2023-06-15 15:20:48.376861 dushyanth-1.0.3/find_ip_to_db/
--rw-r--r--   0 dboppidi   (501) staff       (20)        0 2023-06-15 05:22:49.000000 dushyanth-1.0.3/find_ip_to_db/__init__.py
--rw-r--r--   0 dboppidi   (501) staff       (20)     1937 2023-06-15 15:19:03.000000 dushyanth-1.0.3/find_ip_to_db/find_ip_to_db.py
--rw-r--r--   0 dboppidi   (501) staff       (20)       38 2023-06-15 15:20:48.377315 dushyanth-1.0.3/setup.cfg
--rw-r--r--   0 dboppidi   (501) staff       (20)      340 2023-06-15 15:20:45.000000 dushyanth-1.0.3/setup.py
+drwxr-xr-x   0 dboppidi   (501) staff       (20)        0 2023-06-15 15:28:26.449175 dushyanth-1.0.4/
+-rw-r--r--   0 dboppidi   (501) staff       (20)      304 2023-06-15 15:28:26.448991 dushyanth-1.0.4/PKG-INFO
+drwxr-xr-x   0 dboppidi   (501) staff       (20)        0 2023-06-15 15:28:26.448413 dushyanth-1.0.4/dushyanth.egg-info/
+-rw-r--r--   0 dboppidi   (501) staff       (20)      304 2023-06-15 15:28:26.000000 dushyanth-1.0.4/dushyanth.egg-info/PKG-INFO
+-rw-r--r--   0 dboppidi   (501) staff       (20)      229 2023-06-15 15:28:26.000000 dushyanth-1.0.4/dushyanth.egg-info/SOURCES.txt
+-rw-r--r--   0 dboppidi   (501) staff       (20)        1 2023-06-15 15:28:26.000000 dushyanth-1.0.4/dushyanth.egg-info/dependency_links.txt
+-rw-r--r--   0 dboppidi   (501) staff       (20)       16 2023-06-15 15:28:26.000000 dushyanth-1.0.4/dushyanth.egg-info/requires.txt
+-rw-r--r--   0 dboppidi   (501) staff       (20)       14 2023-06-15 15:28:26.000000 dushyanth-1.0.4/dushyanth.egg-info/top_level.txt
+drwxr-xr-x   0 dboppidi   (501) staff       (20)        0 2023-06-15 15:28:26.448635 dushyanth-1.0.4/find_ip_to_db/
+-rw-r--r--   0 dboppidi   (501) staff       (20)        0 2023-06-15 05:22:49.000000 dushyanth-1.0.4/find_ip_to_db/__init__.py
+-rw-r--r--   0 dboppidi   (501) staff       (20)     1937 2023-06-15 15:26:37.000000 dushyanth-1.0.4/find_ip_to_db/find_ip_to_db.py
+-rw-r--r--   0 dboppidi   (501) staff       (20)       38 2023-06-15 15:28:26.449231 dushyanth-1.0.4/setup.cfg
+-rw-r--r--   0 dboppidi   (501) staff       (20)      329 2023-06-15 15:28:02.000000 dushyanth-1.0.4/setup.py
```

### Comparing `dushyanth-1.0.3/find_ip_to_db/find_ip_to_db.py` & `dushyanth-1.0.4/find_ip_to_db/find_ip_to_db.py`

 * *Files identical despite different names*

