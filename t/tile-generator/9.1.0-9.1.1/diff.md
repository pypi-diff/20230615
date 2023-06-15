# Comparing `tmp/tile-generator-9.1.0.tar.gz` & `tmp/tile-generator-9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tile-generator-9.1.0.tar", last modified: Thu Sep 21 17:58:22 2017, max compression
+gzip compressed data, was "dist/tile-generator-9.1.1.tar", last modified: Fri Sep 22 04:06:01 2017, max compression
```

## Comparing `tile-generator-9.1.0.tar` & `tile-generator-9.1.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-21 17:58:22.000000 tile-generator-9.1.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-21 17:58:22.000000 tile-generator-9.1.0/tile_generator/
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-21 17:58:22.000000 tile-generator-9.1.0/tile_generator/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-21 17:58:22.000000 tile-generator-9.1.0/tile_generator/templates/config/
--rw-r--r--   0 root         (0) root         (0)        7 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/templates/config/blobs.yml
--rw-r--r--   0 root         (0) root         (0)      108 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/templates/config/final.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-21 17:58:22.000000 tile-generator-9.1.0/tile_generator/templates/jobs/
--rw-r--r--   0 root         (0) root         (0)     3088 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/templates/jobs/delete-all.sh.erb
--rw-r--r--   0 root         (0) root         (0)    13376 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/templates/jobs/deploy-all.sh.erb
--rw-r--r--   0 root         (0) root         (0)     1057 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/templates/jobs/docker-bosh.sh.erb
--rw-r--r--   0 root         (0) root         (0)      293 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/templates/jobs/monit
--rw-r--r--   0 root         (0) root         (0)     1460 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/templates/jobs/opsmgr.env.erb
--rw-r--r--   0 root         (0) root         (0)     3237 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/templates/jobs/spec
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-21 17:58:22.000000 tile-generator-9.1.0/tile_generator/templates/packages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-21 17:58:22.000000 tile-generator-9.1.0/tile_generator/templates/packages/cf_cli/
--rw-r--r--   0 root         (0) root         (0)      169 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/templates/packages/cf_cli/packaging
--rw-r--r--   0 root         (0) root         (0)       94 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/templates/packages/cf_cli/spec
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-21 17:58:22.000000 tile-generator-9.1.0/tile_generator/templates/packages/common/
--rw-r--r--   0 root         (0) root         (0)       49 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/templates/packages/common/packaging
--rw-r--r--   0 root         (0) root         (0)       61 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/templates/packages/common/spec
--rw-r--r--   0 root         (0) root         (0)      163 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/templates/packages/packaging
--rw-r--r--   0 root         (0) root         (0)      124 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/templates/packages/spec
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-21 17:58:22.000000 tile-generator-9.1.0/tile_generator/templates/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-21 17:58:22.000000 tile-generator-9.1.0/tile_generator/templates/src/common/
--rw-r--r--   0 root         (0) root         (0)     2325 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/templates/src/common/utils.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-21 17:58:22.000000 tile-generator-9.1.0/tile_generator/templates/src/templates/
--rw-r--r--   0 root         (0) root         (0)       80 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/templates/src/templates/all_open.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-21 17:58:22.000000 tile-generator-9.1.0/tile_generator/templates/tile/
--rw-r--r--   0 root         (0) root         (0)    16974 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/templates/tile/metadata.yml
--rw-r--r--   0 root         (0) root         (0)      141 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/templates/tile/migration.js
--rw-r--r--   0 root         (0) root         (0)       18 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/templates/gitignore
--rw-r--r--   0 root         (0) root         (0)     3202 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/templates/tile.yml
--rw-r--r--   0 root         (0) root         (0)        0 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8666 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/bosh.py
--rw-r--r--   0 root         (0) root         (0)     3102 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/bosh_unittest.py
--rw-r--r--   0 root         (0) root         (0)     3342 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/build.py
--rw-r--r--   0 root         (0) root         (0)     1123 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/build_unittest.py
--rw-r--r--   0 root         (0) root         (0)    23573 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/config.py
--rw-r--r--   0 root         (0) root         (0)    13813 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/config_unittest.py
--rw-r--r--   0 root         (0) root         (0)     4713 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/erb.py
--rw-r--r--   0 root         (0) root         (0)    24624 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/opsmgr.py
--rw-r--r--   0 root         (0) root         (0)    18338 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/opsmgr_unittest.py
--rwxr-xr-x   0 root         (0) root         (0)    15332 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/pcf.py
--rw-r--r--   0 root         (0) root         (0)     7584 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/template.py
--rw-r--r--   0 root         (0) root         (0)     1334 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/template_unittest.py
--rwxr-xr-x   0 root         (0) root         (0)     2662 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/tile.py
--rw-r--r--   0 root         (0) root         (0)     1712 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/tile_unittest.py
--rw-r--r--   0 root         (0) root         (0)     4555 2017-09-21 17:58:18.000000 tile-generator-9.1.0/tile_generator/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-21 17:58:22.000000 tile-generator-9.1.0/tile_generator.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3694 2017-09-21 17:58:22.000000 tile-generator-9.1.0/tile_generator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1604 2017-09-21 17:58:22.000000 tile-generator-9.1.0/tile_generator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2017-09-21 17:58:22.000000 tile-generator-9.1.0/tile_generator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2017-09-21 17:58:22.000000 tile-generator-9.1.0/tile_generator.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      104 2017-09-21 17:58:22.000000 tile-generator-9.1.0/tile_generator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2017-09-21 17:58:22.000000 tile-generator-9.1.0/tile_generator.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    11360 2017-09-21 17:58:18.000000 tile-generator-9.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      114 2017-09-21 17:58:18.000000 tile-generator-9.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      610 2017-09-21 17:58:18.000000 tile-generator-9.1.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     2318 2017-09-21 17:58:18.000000 tile-generator-9.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)     2228 2017-09-21 17:58:18.000000 tile-generator-9.1.0/setup.py
--rw-r--r--   0 root         (0) root         (0)        5 2017-09-21 17:58:22.000000 tile-generator-9.1.0/version.txt
--rw-r--r--   0 root         (0) root         (0)     3694 2017-09-21 17:58:22.000000 tile-generator-9.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2017-09-21 17:58:22.000000 tile-generator-9.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-22 04:06:01.000000 tile-generator-9.1.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-22 04:06:01.000000 tile-generator-9.1.1/tile_generator/
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-22 04:06:01.000000 tile-generator-9.1.1/tile_generator/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-22 04:06:01.000000 tile-generator-9.1.1/tile_generator/templates/config/
+-rw-r--r--   0 root         (0) root         (0)        7 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/templates/config/blobs.yml
+-rw-r--r--   0 root         (0) root         (0)      108 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/templates/config/final.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-22 04:06:01.000000 tile-generator-9.1.1/tile_generator/templates/jobs/
+-rw-r--r--   0 root         (0) root         (0)     3088 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/templates/jobs/delete-all.sh.erb
+-rw-r--r--   0 root         (0) root         (0)    13376 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/templates/jobs/deploy-all.sh.erb
+-rw-r--r--   0 root         (0) root         (0)     1057 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/templates/jobs/docker-bosh.sh.erb
+-rw-r--r--   0 root         (0) root         (0)      293 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/templates/jobs/monit
+-rw-r--r--   0 root         (0) root         (0)     1460 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/templates/jobs/opsmgr.env.erb
+-rw-r--r--   0 root         (0) root         (0)     3237 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/templates/jobs/spec
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-22 04:06:01.000000 tile-generator-9.1.1/tile_generator/templates/packages/
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-22 04:06:01.000000 tile-generator-9.1.1/tile_generator/templates/packages/cf_cli/
+-rw-r--r--   0 root         (0) root         (0)      169 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/templates/packages/cf_cli/packaging
+-rw-r--r--   0 root         (0) root         (0)       94 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/templates/packages/cf_cli/spec
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-22 04:06:01.000000 tile-generator-9.1.1/tile_generator/templates/packages/common/
+-rw-r--r--   0 root         (0) root         (0)       49 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/templates/packages/common/packaging
+-rw-r--r--   0 root         (0) root         (0)       61 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/templates/packages/common/spec
+-rw-r--r--   0 root         (0) root         (0)      163 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/templates/packages/packaging
+-rw-r--r--   0 root         (0) root         (0)      124 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/templates/packages/spec
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-22 04:06:01.000000 tile-generator-9.1.1/tile_generator/templates/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-22 04:06:01.000000 tile-generator-9.1.1/tile_generator/templates/src/common/
+-rw-r--r--   0 root         (0) root         (0)     2325 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/templates/src/common/utils.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-22 04:06:01.000000 tile-generator-9.1.1/tile_generator/templates/src/templates/
+-rw-r--r--   0 root         (0) root         (0)       80 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/templates/src/templates/all_open.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-22 04:06:01.000000 tile-generator-9.1.1/tile_generator/templates/tile/
+-rw-r--r--   0 root         (0) root         (0)    16974 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/templates/tile/metadata.yml
+-rw-r--r--   0 root         (0) root         (0)      141 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/templates/tile/migration.js
+-rw-r--r--   0 root         (0) root         (0)       18 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/templates/gitignore
+-rw-r--r--   0 root         (0) root         (0)     3202 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/templates/tile.yml
+-rw-r--r--   0 root         (0) root         (0)        0 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8666 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/bosh.py
+-rw-r--r--   0 root         (0) root         (0)     3102 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/bosh_unittest.py
+-rw-r--r--   0 root         (0) root         (0)     3342 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/build.py
+-rw-r--r--   0 root         (0) root         (0)     1123 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/build_unittest.py
+-rw-r--r--   0 root         (0) root         (0)    23813 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/config.py
+-rw-r--r--   0 root         (0) root         (0)    13813 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/config_unittest.py
+-rw-r--r--   0 root         (0) root         (0)     4713 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/erb.py
+-rw-r--r--   0 root         (0) root         (0)    24624 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/opsmgr.py
+-rw-r--r--   0 root         (0) root         (0)    18338 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/opsmgr_unittest.py
+-rwxr-xr-x   0 root         (0) root         (0)    15332 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/pcf.py
+-rw-r--r--   0 root         (0) root         (0)     7584 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/template.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/template_unittest.py
+-rwxr-xr-x   0 root         (0) root         (0)     2662 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/tile.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/tile_unittest.py
+-rw-r--r--   0 root         (0) root         (0)     4555 2017-09-22 04:05:46.000000 tile-generator-9.1.1/tile_generator/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-09-22 04:06:01.000000 tile-generator-9.1.1/tile_generator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3694 2017-09-22 04:06:00.000000 tile-generator-9.1.1/tile_generator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1604 2017-09-22 04:06:01.000000 tile-generator-9.1.1/tile_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2017-09-22 04:06:01.000000 tile-generator-9.1.1/tile_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2017-09-22 04:06:01.000000 tile-generator-9.1.1/tile_generator.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2017-09-22 04:06:00.000000 tile-generator-9.1.1/tile_generator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2017-09-22 04:06:01.000000 tile-generator-9.1.1/tile_generator.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    11360 2017-09-22 04:05:46.000000 tile-generator-9.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      114 2017-09-22 04:05:46.000000 tile-generator-9.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      610 2017-09-22 04:05:46.000000 tile-generator-9.1.1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     2318 2017-09-22 04:05:46.000000 tile-generator-9.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     2228 2017-09-22 04:05:46.000000 tile-generator-9.1.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)        5 2017-09-22 04:06:00.000000 tile-generator-9.1.1/version.txt
+-rw-r--r--   0 root         (0) root         (0)     3694 2017-09-22 04:06:01.000000 tile-generator-9.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2017-09-22 04:06:01.000000 tile-generator-9.1.1/setup.cfg
```

### Comparing `tile-generator-9.1.0/tile_generator/templates/jobs/delete-all.sh.erb` & `tile-generator-9.1.1/tile_generator/templates/jobs/delete-all.sh.erb`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator/templates/jobs/deploy-all.sh.erb` & `tile-generator-9.1.1/tile_generator/templates/jobs/deploy-all.sh.erb`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator/templates/jobs/docker-bosh.sh.erb` & `tile-generator-9.1.1/tile_generator/templates/jobs/docker-bosh.sh.erb`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator/templates/jobs/opsmgr.env.erb` & `tile-generator-9.1.1/tile_generator/templates/jobs/opsmgr.env.erb`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator/templates/jobs/spec` & `tile-generator-9.1.1/tile_generator/templates/jobs/spec`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator/templates/src/common/utils.sh` & `tile-generator-9.1.1/tile_generator/templates/src/common/utils.sh`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator/templates/tile/metadata.yml` & `tile-generator-9.1.1/tile_generator/templates/tile/metadata.yml`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator/templates/tile.yml` & `tile-generator-9.1.1/tile_generator/templates/tile.yml`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator/bosh.py` & `tile-generator-9.1.1/tile_generator/bosh.py`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator/bosh_unittest.py` & `tile-generator-9.1.1/tile_generator/bosh_unittest.py`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator/build.py` & `tile-generator-9.1.1/tile_generator/build.py`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator/build_unittest.py` & `tile-generator-9.1.1/tile_generator/build_unittest.py`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator/config.py` & `tile-generator-9.1.1/tile_generator/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,14 +206,21 @@
 			'cf': {
 				'admin_user': '(( ..cf.uaa.system_services_credentials.identity ))',
 				'admin_password': '(( ..cf.uaa.system_services_credentials.password ))',
 			},
 			'apply_open_security_group': '(( .properties.apply_open_security_group.value ))',
 			'allow_paid_service_plans': '(( .properties.allow_paid_service_plans.value ))',
 		}
+		if job.get('type') == 'deploy-all':
+			merge_dict(manifest, {
+				'security': {
+					'user': '(( .{}.app_credentials.identity ))'.format(job['name']),
+					'password': '(( .{}.app_credentials.password ))'.format(job['name']),
+				}
+			})
 		merge_dict(manifest, job['properties'])
 		for property in self.get('all_properties', []):
 			merge_dict(manifest, template.render_property(property))
 		for service_plan_form in self.get('service_plan_forms', []):
 			manifest[service_plan_form['name']] = '(( .properties.{}.value ))'.format(service_plan_form['name'])
 		for package in self.get('packages', []):
 			merge_dict(manifest, package['properties'])
```

### Comparing `tile-generator-9.1.0/tile_generator/config_unittest.py` & `tile-generator-9.1.1/tile_generator/config_unittest.py`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator/erb.py` & `tile-generator-9.1.1/tile_generator/erb.py`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator/opsmgr.py` & `tile-generator-9.1.1/tile_generator/opsmgr.py`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator/opsmgr_unittest.py` & `tile-generator-9.1.1/tile_generator/opsmgr_unittest.py`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator/pcf.py` & `tile-generator-9.1.1/tile_generator/pcf.py`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator/template.py` & `tile-generator-9.1.1/tile_generator/template.py`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator/template_unittest.py` & `tile-generator-9.1.1/tile_generator/template_unittest.py`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator/tile.py` & `tile-generator-9.1.1/tile_generator/tile.py`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator/tile_unittest.py` & `tile-generator-9.1.1/tile_generator/tile_unittest.py`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator/util.py` & `tile-generator-9.1.1/tile_generator/util.py`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/tile_generator.egg-info/PKG-INFO` & `tile-generator-9.1.1/tile_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tile-generator
-Version: 9.1.0
+Version: 9.1.1
 Summary: Tools supporting development of Pivotal Cloud Foundry services and add-ons.
 Home-page: https://github.com/cf-platform-eng/tile-generator
 Author: Pivotal Cloud Foundry Platform Engineering
 Author-email: UNKNOWN
 License: Apache 2.0
 Description: PCF Tile Generator
         ==================
```

### Comparing `tile-generator-9.1.0/tile_generator.egg-info/SOURCES.txt` & `tile-generator-9.1.1/tile_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/LICENSE` & `tile-generator-9.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/NOTICE` & `tile-generator-9.1.1/NOTICE`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/README.md` & `tile-generator-9.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/setup.py` & `tile-generator-9.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `tile-generator-9.1.0/PKG-INFO` & `tile-generator-9.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tile-generator
-Version: 9.1.0
+Version: 9.1.1
 Summary: Tools supporting development of Pivotal Cloud Foundry services and add-ons.
 Home-page: https://github.com/cf-platform-eng/tile-generator
 Author: Pivotal Cloud Foundry Platform Engineering
 Author-email: UNKNOWN
 License: Apache 2.0
 Description: PCF Tile Generator
         ==================
```

