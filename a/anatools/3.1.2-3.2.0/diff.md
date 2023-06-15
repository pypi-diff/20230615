# Comparing `tmp/anatools-3.1.2.tar.gz` & `tmp/anatools-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anatools-3.1.2.tar", last modified: Fri May  5 22:10:40 2023, max compression
+gzip compressed data, was "anatools-3.2.0.tar", last modified: Thu Jun 15 17:52:45 2023, max compression
```

## Comparing `anatools-3.1.2.tar` & `anatools-3.2.0.tar`

### file list

```diff
@@ -1,102 +1,106 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 22:10:40.560480 anatools-3.1.2/
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-05-05 22:10:16.000000 anatools-3.1.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-05-05 22:10:16.000000 anatools-3.1.2/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     6975 2023-05-05 22:10:40.560480 anatools-3.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6585 2023-05-05 22:10:16.000000 anatools-3.1.2/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 22:10:40.548480 anatools-3.1.2/anatools/
--rw-rw-rw-   0 root         (0) root         (0)      953 2023-05-05 22:10:20.000000 anatools-3.1.2/anatools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 22:10:40.552480 anatools-3.1.2/anatools/anaclient/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11167 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/anaclient.py
--rw-rw-rw-   0 root         (0) root         (0)     3581 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/analytics.py
--rw-rw-rw-   0 root         (0) root         (0)    11005 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/annotations.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 22:10:40.552480 anatools-3.1.2/anatools/anaclient/api/
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2910 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/api/analytics.py
--rw-rw-rw-   0 root         (0) root         (0)     9403 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/api/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)     4454 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/api/api.py
--rw-rw-rw-   0 root         (0) root         (0)    10389 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/api/channels.py
--rw-rw-rw-   0 root         (0) root         (0)     8002 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/api/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)    10116 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/api/gan.py
--rw-rw-rw-   0 root         (0) root         (0)     4206 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/api/graphs.py
--rw-rw-rw-   0 root         (0) root         (0)     1224 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/api/handlers.py
--rw-rw-rw-   0 root         (0) root         (0)     5334 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/api/limits.py
--rw-rw-rw-   0 root         (0) root         (0)     3974 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/api/members.py
--rw-rw-rw-   0 root         (0) root         (0)     1375 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/api/organizations.py
--rw-rw-rw-   0 root         (0) root         (0)     2489 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/api/umap.py
--rw-rw-rw-   0 root         (0) root         (0)     8958 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/api/volumes.py
--rw-rw-rw-   0 root         (0) root         (0)     3202 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/api/workspaces.py
--rw-rw-rw-   0 root         (0) root         (0)    18408 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/channels.py
--rw-rw-rw-   0 root         (0) root         (0)     9203 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)     9573 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/gan.py
--rw-rw-rw-   0 root         (0) root         (0)     6300 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/graphs.py
--rw-rw-rw-   0 root         (0) root         (0)     9386 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/organizations.py
--rw-rw-rw-   0 root         (0) root         (0)     1936 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/umap.py
--rw-rw-rw-   0 root         (0) root         (0)    17861 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/volumes.py
--rw-rw-rw-   0 root         (0) root         (0)     9168 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/anaclient/workspaces.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 22:10:40.556480 anatools-3.1.2/anatools/annotations/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/annotations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7460 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/annotations/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)     3701 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/annotations/convert_coco.py
--rw-rw-rw-   0 root         (0) root         (0)     7173 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/annotations/convert_kitti.py
--rw-rw-rw-   0 root         (0) root         (0)     3381 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/annotations/convert_pascal.py
--rw-rw-rw-   0 root         (0) root         (0)     4641 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/annotations/convert_sagemaker.py
--rw-rw-rw-   0 root         (0) root         (0)     2727 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/annotations/convert_yolo.py
--rw-rw-rw-   0 root         (0) root         (0)     7548 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/annotations/draw.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 22:10:40.556480 anatools-3.1.2/anatools/bin/
--rw-rw-rw-   0 root         (0) root         (0)     4523 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/bin/ana
--rw-rw-rw-   0 root         (0) root         (0)     9659 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/bin/anadeploy
--rw-rw-rw-   0 root         (0) root         (0)     7692 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/bin/anamount
--rw-rw-rw-   0 root         (0) root         (0)     4524 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/bin/anautils
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 22:10:40.556480 anatools-3.1.2/anatools/lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6974 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/lib/ana_object.py
--rw-rw-rw-   0 root         (0) root         (0)     7114 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/lib/bbox.py
--rw-rw-rw-   0 root         (0) root         (0)     2149 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/lib/blender_main.py
--rw-rw-rw-   0 root         (0) root         (0)     4923 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/lib/camera_checks.py
--rw-rw-rw-   0 root         (0) root         (0)    14524 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/lib/channel.py
--rw-rw-rw-   0 root         (0) root         (0)     1777 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/lib/context.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/lib/download.py
--rw-rw-rw-   0 root         (0) root         (0)     2917 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/lib/file_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/lib/file_object.py
--rw-rw-rw-   0 root         (0) root         (0)     9556 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/lib/generator.py
--rw-rw-rw-   0 root         (0) root         (0)     5727 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/lib/interp.py
--rw-rw-rw-   0 root         (0) root         (0)     2244 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/lib/load.py
--rw-rw-rw-   0 root         (0) root         (0)    10556 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/lib/node.py
--rw-rw-rw-   0 root         (0) root         (0)     1430 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/lib/object_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1702 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/lib/package_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/lib/print.py
--rw-rw-rw-   0 root         (0) root         (0)     1918 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/lib/python_main.py
--rw-rw-rw-   0 root         (0) root         (0)     3200 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/lib/rigged_object.py
--rw-rw-rw-   0 root         (0) root         (0)     8111 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/lib/scene.py
--rw-rw-rw-   0 root         (0) root         (0)     3757 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/lib/search_utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 22:10:40.560480 anatools-3.1.2/anatools/nodes/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/nodes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/nodes/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/nodes/constants.yml
--rw-rw-rw-   0 root         (0) root         (0)     2635 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/nodes/generators.py
--rw-rw-rw-   0 root         (0) root         (0)     2183 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/nodes/generators.yml
--rw-rw-rw-   0 root         (0) root         (0)     1592 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/nodes/logic.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/nodes/logic.yml
--rw-rw-rw-   0 root         (0) root         (0)     5381 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/nodes/random_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     8429 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/nodes/random_generator.yml
--rw-rw-rw-   0 root         (0) root         (0)     1321 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/nodes/sweep_arange.py
--rw-rw-rw-   0 root         (0) root         (0)     1509 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/nodes/sweep_arange.yml
--rw-rw-rw-   0 root         (0) root         (0)     1306 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/nodes/sweep_linspace.py
--rw-rw-rw-   0 root         (0) root         (0)     1549 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/nodes/sweep_linspace.yml
--rw-rw-rw-   0 root         (0) root         (0)     1224 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/nodes/vectors.py
--rw-rw-rw-   0 root         (0) root         (0)     1922 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/nodes/vectors.yml
--rw-rw-rw-   0 root         (0) root         (0)      557 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/nodes/volume_file.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-05-05 22:10:16.000000 anatools-3.1.2/anatools/nodes/volume_file.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 22:10:40.548480 anatools-3.1.2/anatools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6975 2023-05-05 22:10:40.000000 anatools-3.1.2/anatools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2583 2023-05-05 22:10:40.000000 anatools-3.1.2/anatools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-05 22:10:40.000000 anatools-3.1.2/anatools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-05 22:10:40.000000 anatools-3.1.2/anatools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-05-05 22:10:40.000000 anatools-3.1.2/anatools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-05-05 22:10:16.000000 anatools-3.1.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-05-05 22:10:16.000000 anatools-3.1.2/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-05 22:10:40.560480 anatools-3.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1110 2023-05-05 22:10:16.000000 anatools-3.1.2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 22:10:40.560480 anatools-3.1.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)      782 2023-05-05 22:10:17.000000 anatools-3.1.2/tests/test_bbox.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 17:52:45.500299 anatools-3.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-15 17:52:22.000000 anatools-3.2.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-15 17:52:22.000000 anatools-3.2.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     6975 2023-06-15 17:52:45.500299 anatools-3.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6585 2023-06-15 17:52:22.000000 anatools-3.2.0/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 17:52:45.484298 anatools-3.2.0/anatools/
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-06-15 17:52:27.000000 anatools-3.2.0/anatools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 17:52:45.488298 anatools-3.2.0/anatools/anaclient/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11167 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/anaclient.py
+-rw-rw-rw-   0 root         (0) root         (0)     3581 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/analytics.py
+-rw-rw-rw-   0 root         (0) root         (0)    11005 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/annotations.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 17:52:45.488298 anatools-3.2.0/anatools/anaclient/api/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2910 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/analytics.py
+-rw-rw-rw-   0 root         (0) root         (0)     9403 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4454 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    10389 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/channels.py
+-rw-rw-rw-   0 root         (0) root         (0)     8002 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)    10116 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/gan.py
+-rw-rw-rw-   0 root         (0) root         (0)     4206 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/graphs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1224 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5334 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/limits.py
+-rw-rw-rw-   0 root         (0) root         (0)     3974 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/members.py
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/organizations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2489 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/umap.py
+-rw-rw-rw-   0 root         (0) root         (0)     8958 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/volumes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/api/workspaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    18408 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/channels.py
+-rw-rw-rw-   0 root         (0) root         (0)     9203 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)     9573 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/gan.py
+-rw-rw-rw-   0 root         (0) root         (0)     6300 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/graphs.py
+-rw-rw-rw-   0 root         (0) root         (0)     9386 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/organizations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/umap.py
+-rw-rw-rw-   0 root         (0) root         (0)    17897 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/volumes.py
+-rw-rw-rw-   0 root         (0) root         (0)     9168 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/anaclient/workspaces.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 17:52:45.492298 anatools-3.2.0/anatools/annotations/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/annotations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7460 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/annotations/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3701 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/annotations/convert_coco.py
+-rw-rw-rw-   0 root         (0) root         (0)     7173 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/annotations/convert_kitti.py
+-rw-rw-rw-   0 root         (0) root         (0)     3381 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/annotations/convert_pascal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4468 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/annotations/convert_sagemaker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2727 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/annotations/convert_yolo.py
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/annotations/draw.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 17:52:45.492298 anatools-3.2.0/anatools/bin/
+-rw-rw-rw-   0 root         (0) root         (0)     4523 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/bin/ana
+-rw-rw-rw-   0 root         (0) root         (0)     9659 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/bin/anadeploy
+-rw-rw-rw-   0 root         (0) root         (0)     7692 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/bin/anamount
+-rw-rw-rw-   0 root         (0) root         (0)     4559 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/bin/anautils
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 17:52:45.496299 anatools-3.2.0/anatools/lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6974 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/ana_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     7114 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/bbox.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/blender_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     4923 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/camera_checks.py
+-rw-rw-rw-   0 root         (0) root         (0)    14524 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/channel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1777 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1490 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/directory_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/download.py
+-rw-rw-rw-   0 root         (0) root         (0)     3806 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/file_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1308 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/file_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/file_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     9556 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5670 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/interp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2244 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/load.py
+-rw-rw-rw-   0 root         (0) root         (0)    10556 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/node.py
+-rw-rw-rw-   0 root         (0) root         (0)     1430 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/object_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1702 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/package_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/print.py
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/python_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3200 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/rigged_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     8111 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/scene.py
+-rw-rw-rw-   0 root         (0) root         (0)     3757 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/lib/search_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 17:52:45.500299 anatools-3.2.0/anatools/nodes/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1228 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/constants.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2635 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2183 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/generators.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1592 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/logic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/logic.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5381 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/random_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     8429 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/random_generator.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/sweep_arange.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/sweep_arange.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1306 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/sweep_linspace.py
+-rw-rw-rw-   0 root         (0) root         (0)     1549 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/sweep_linspace.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1224 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/vectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1922 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/vectors.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1246 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/volume_directory.py
+-rw-rw-rw-   0 root         (0) root         (0)      901 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/volume_directory.yml
+-rw-rw-rw-   0 root         (0) root         (0)      557 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/volume_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-06-15 17:52:22.000000 anatools-3.2.0/anatools/nodes/volume_file.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 17:52:45.484298 anatools-3.2.0/anatools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6975 2023-06-15 17:52:45.000000 anatools-3.2.0/anatools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2717 2023-06-15 17:52:45.000000 anatools-3.2.0/anatools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-15 17:52:45.000000 anatools-3.2.0/anatools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-15 17:52:45.000000 anatools-3.2.0/anatools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-06-15 17:52:45.000000 anatools-3.2.0/anatools.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-15 17:52:22.000000 anatools-3.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-15 17:52:22.000000 anatools-3.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-15 17:52:45.500299 anatools-3.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2023-06-15 17:52:22.000000 anatools-3.2.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 17:52:45.500299 anatools-3.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      782 2023-06-15 17:52:23.000000 anatools-3.2.0/tests/test_bbox.py
```

### Comparing `anatools-3.1.2/LICENSE` & `anatools-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/PKG-INFO` & `anatools-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anatools
-Version: 3.1.2
+Version: 3.2.0
 Summary: Tools for development with the Rendered.ai Platform.
 Home-page: https://rendered.ai
 Author: Rendered AI, Inc
 Author-email: support@rendered.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `anatools-3.1.2/README.md` & `anatools-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/__init__.py` & `anatools-3.2.0/anatools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
         https://support.rendered.ai/gc/Introduction-to-Rendered.ai.1577812005.html
 
 """
 
 from .anaclient.anaclient import client
 from .annotations.annotations import annotations
 
-__version__ = '3.1.2'
+__version__ = '3.2.0'
```

### Comparing `anatools-3.1.2/anatools/anaclient/anaclient.py` & `anatools-3.2.0/anatools/anaclient/anaclient.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/analytics.py` & `anatools-3.2.0/anatools/anaclient/analytics.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/annotations.py` & `anatools-3.2.0/anatools/anaclient/annotations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/api/analytics.py` & `anatools-3.2.0/anatools/anaclient/api/analytics.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/api/annotations.py` & `anatools-3.2.0/anatools/anaclient/api/annotations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/api/api.py` & `anatools-3.2.0/anatools/anaclient/api/api.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/api/channels.py` & `anatools-3.2.0/anatools/anaclient/api/channels.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/api/datasets.py` & `anatools-3.2.0/anatools/anaclient/api/datasets.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/api/gan.py` & `anatools-3.2.0/anatools/anaclient/api/gan.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/api/graphs.py` & `anatools-3.2.0/anatools/anaclient/api/graphs.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/api/handlers.py` & `anatools-3.2.0/anatools/anaclient/api/handlers.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/api/limits.py` & `anatools-3.2.0/anatools/anaclient/api/limits.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/api/members.py` & `anatools-3.2.0/anatools/anaclient/api/members.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/api/organizations.py` & `anatools-3.2.0/anatools/anaclient/api/organizations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/api/umap.py` & `anatools-3.2.0/anatools/anaclient/api/umap.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/api/volumes.py` & `anatools-3.2.0/anatools/anaclient/api/volumes.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/api/workspaces.py` & `anatools-3.2.0/anatools/anaclient/api/workspaces.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/channels.py` & `anatools-3.2.0/anatools/anaclient/channels.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/datasets.py` & `anatools-3.2.0/anatools/anaclient/datasets.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/gan.py` & `anatools-3.2.0/anatools/anaclient/gan.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/graphs.py` & `anatools-3.2.0/anatools/anaclient/graphs.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/organizations.py` & `anatools-3.2.0/anatools/anaclient/organizations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/umap.py` & `anatools-3.2.0/anatools/anaclient/umap.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/anaclient/volumes.py` & `anatools-3.2.0/anatools/anaclient/volumes.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     """
     if self.check_logout(): return
     if organizationId is None: organizationId = self.organization
     return self.ana_api.getManagedVolumes(organizationId=organizationId, volumeId=volumeId)
 
 
 def create_managed_volume(self, name, description=None, organizationId=None):
-    """Creates a new volume with the specified name in the organization and write permission.
+    """Creates a new volume with the specified name in the organization. By default the permission on the volume is set to `write`.
     
     Parameters
     ----------
     name : str
         The name of the new volume. Note: this name needs to be unique per organization.
     description : str
         Description of the volume
@@ -65,15 +65,15 @@
     if self.check_logout(): return
     if organizationId is None: organizationId = self.organization
     if name is None: raise Exception("Name must be specified.")
     return self.ana_api.createManagedVolume(organizationId=organizationId, name=name, description=description)
 
     
 def delete_managed_volume(self, volumeId):
-    """Removes the volumeId from the organization. Note that this will delete any remote data in the volume 
+    """Removes the volume from the organization. Note that this will delete any remote data in the volume 
     and channels that rely on this volume will need to be updated.
     
     Parameters
     ----------
     volumeId : str
         The ID of a specific Volume to delete.
```

### Comparing `anatools-3.1.2/anatools/anaclient/workspaces.py` & `anatools-3.2.0/anatools/anaclient/workspaces.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/annotations/annotations.py` & `anatools-3.2.0/anatools/annotations/annotations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/annotations/convert_coco.py` & `anatools-3.2.0/anatools/annotations/convert_coco.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/annotations/convert_kitti.py` & `anatools-3.2.0/anatools/annotations/convert_kitti.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/annotations/convert_pascal.py` & `anatools-3.2.0/anatools/annotations/convert_pascal.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/annotations/convert_sagemaker.py` & `anatools-3.2.0/anatools/annotations/convert_sagemaker.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,51 +24,52 @@
     metadir = os.path.join(datadir, "metadata")
 
     # Get the image shape
     sample_image_filename = [datadir + '/images/' + imgfilename for imgfilename in os.listdir(datadir + '/images')][0]
     sample_image = Image.open(sample_image_filename)
     imgshape = [sample_image.size[0], sample_image.size[1], 3]
 
-    sodcats = list()
+    # generate categories
+    sodcats = dict()
+    for catnum in mapping['classes'].keys():
+        cat_name = mapping['classes'][catnum][-1]
+        sodcats[cat_name] = catnum
+
     for annsfilename in os.listdir(annsdir):
         with open(os.path.join(annsdir, annsfilename), 'r') as af:
             anns = json.load(af)
         with open(os.path.join(metadir, annsfilename.replace('ana', 'metadata')), 'r') as mf:
             metadata = json.load(mf)
 
         soddata = dict()
         soddata['file'] = anns['filename'].split('.')[0] + '.jpeg'  # Sagemaker requires images be in jpeg format
         soddata['image_size'] = [{'width':imgshape[0],'height':imgshape[1],'depth':imgshape[2]}]
         soddata['annotations'] = list()
         for obj in metadata['objects']:
-            for i, prop in enumerate(mapping['properties']):
+            for prop in mapping['properties']:
                 if eval(prop):
                     for ann in anns['annotations']:
                         if ann['id'] == obj['id']:
                             objann = ann
                             break
-                    else:  # All the objects from the scene are recorded in metadata; only those in the image are annotated
-                        continue
+                    else: continue
 
-                    rai_cat_id = mapping['properties'][prop]
-                    cat = mapping['classes'][rai_cat_id]
-                    cat_name = cat[-1]
-                    if cat_name not in sodcats: sodcats.append(cat_name)              
+                    catid = mapping['properties'][prop]              
                     soddata['annotations'].append({
-                        'class_id': sodcats.index(cat_name),
+                        'class_id': catid,
                         'left':     objann['bbox'][0],
                         'top':      objann['bbox'][1],
                         'width':    objann['bbox'][2],
                         'height':   objann['bbox'][3]
                     })
                     break
 
         soddata['categories'] = list()
-        for cId, cName in enumerate(sodcats):
-            soddata['categories'].append({'class_id':cId, 'name':cName})
+        for cat in sodcats.keys():
+            soddata['categories'].append({'class_id': sodcats[cat], 'name': cat})
     
         outfile = os.path.join(outdir, '{}.json'.format(anns['filename'].split('.')[0]))
         with open(outfile, 'w') as f:
             json.dump(soddata, f)
 
 
 def convert_sagemaker_ss(datadir, outdir, mapping):
```

### Comparing `anatools-3.1.2/anatools/annotations/convert_yolo.py` & `anatools-3.2.0/anatools/annotations/convert_yolo.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/annotations/draw.py` & `anatools-3.2.0/anatools/annotations/draw.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/bin/ana` & `anatools-3.2.0/anatools/bin/ana`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/bin/anadeploy` & `anatools-3.2.0/anatools/bin/anadeploy`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/bin/anamount` & `anatools-3.2.0/anatools/bin/anamount`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/bin/anautils` & `anatools-3.2.0/anatools/bin/anautils`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 channel = Channel(args.channel)
 
 if args.mode == 'schema':
     full_conf = channel.schemas.copy()
     node_list = []
     for item_name in full_conf:
         # don't include VolumeFile node in node_data.yml 
-        if item_name != "VolumeFile":
+        if item_name != "VolumeFile" and item_name != "VolumeDirectory":
             full_conf[item_name]["name"]=item_name
             node_list.append(full_conf[item_name])
 
     # write the schema to the node_data.yml file
     with open(os.path.join(args.output, 'node_data.yml'), 'w') as outfile:
         json.dump(node_list, outfile, indent=2 )
```

### Comparing `anatools-3.1.2/anatools/lib/ana_object.py` & `anatools-3.2.0/anatools/lib/ana_object.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/lib/bbox.py` & `anatools-3.2.0/anatools/lib/bbox.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/lib/blender_main.py` & `anatools-3.2.0/anatools/lib/blender_main.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/lib/camera_checks.py` & `anatools-3.2.0/anatools/lib/camera_checks.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/lib/channel.py` & `anatools-3.2.0/anatools/lib/channel.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/lib/context.py` & `anatools-3.2.0/anatools/lib/context.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/lib/file_handlers.py` & `anatools-3.2.0/anatools/lib/file_handlers.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,71 +10,89 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import sys
 import logging
+from anatools.lib.search_utils import find_root
 from anatools.lib.generator import ObjectGenerator
 from anatools.lib.file_object import FileObject
+from anatools.lib.directory_object import DirectoryObject
 import bpy
 
 logger = logging.getLogger(__name__)
 
 def blender_load(self, **kwargs):
     """
     Load a blender file. Doesn't require a collection name.
     """
 
     if self.loaded:
         # only load the object once
         return
 
     blender_file = kwargs.pop("blender_file")
-    # load the objects
+    # load the collections containing the object
     with bpy.data.libraries.load(filepath="//" + blender_file, link=False) as (df, dt):
-        dt.objects = df.objects
+        dt.collections = df.collections
     
-    name = dt.objects[0].name
-    self.collection = bpy.data.collections.new(name)
-    bpy.data.collections[name].objects.link(dt.objects[0])
+    # find the topmost object and set the ana collection to that object's collection
+    self.root = find_root(dt.collections[0])
+    self.collection = self.root.users_collection[0]
     
+    # link the collection to the scene
     bpy.context.scene.collection.children.link(self.collection)
 
-    self.root = dt.objects[0]
+    # deprecated parameter
     self.loaded = True
-    self.object_type = name
+
+    # get the filename and rename the object and collection for metadata consistency
+    name = os.path.splitext(os.path.basename(blender_file))[0]
+    self.root.name = name
+    self.root.users_collection[0].name = name
+    self.object_type = self.root.name
 
     # save object config if it was provided
     if "config" in kwargs:
         self.config = kwargs.pop("config")
 
+def filename_to_generator(filename, object_class):
+    # create an object generator that uses filename as its source
+
+    # copy the class so we can change the load method
+    new_generator_class = type('DynamicObject', object_class.__bases__, dict(object_class.__dict__))
+    _, ext = os.path.splitext(filename)
+    if ext == ".blend":
+        new_generator_class.load = blender_load
+    else:
+        logger.error(f"File type of '{ext}' not supported")
+        sys.exit(1)
+    wrapped_generator = ObjectGenerator(
+        new_generator_class,
+        None,
+        blender_file=filename)
+    return wrapped_generator
+
 def file_to_objgen(generators, object_class):
     """
-    Process a mixed list of generators and FileObjects.
+    Process a mixed list of generators, FileObjects, and DirectoryObjects
     For any FileObject in the list, wrap it in an ObjectGenerator. The object type returned by the
     generator will be 'object_class'. The loader method will be replaced with one appropriate
-    to the file type specified in the FileObject (currently only Blender is supported)
+    to the file type specified in the FileObject (currently only Blender is supported).
+    For any DirectoryObject in the list, loop through all files in the directory (excluding
+    subdirectories and files ending in .anameta) and make them object generators as above.
     """
 
     # return generators
     wrapped_generators = []
     for generator in generators:
         if isinstance(generator, FileObject):
-            # it's a file object - copy the class so we can change the load method
-            new_generator_class = type('DynamicObject', object_class.__bases__, dict(object_class.__dict__))
-            _, ext = os.path.splitext(generator.filename)
-            if ext == ".blend":
-                new_generator_class.load = blender_load
-            else:
-                logger.error(f"File type of '{ext}' not supported")
-                sys.exit(1)
-            wrapped_generator = ObjectGenerator(
-                new_generator_class,
-                None,
-                blender_file=generator.filename)
+            wrapped_generators.append(filename_to_generator(generator.filename, object_class))
+        elif isinstance(generator, DirectoryObject):
+            files = generator.get_files()
+            for filename in files:
+                wrapped_generators.append(filename_to_generator(filename, object_class))
         else:
-            # it's already a generator
-            wrapped_generator = generator
-        wrapped_generators.append(wrapped_generator)
+            wrapped_generators.append(generator)
 
     return wrapped_generators
```

### Comparing `anatools-3.1.2/anatools/lib/file_object.py` & `anatools-3.2.0/anatools/lib/file_object.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/lib/generator.py` & `anatools-3.2.0/anatools/lib/generator.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/lib/interp.py` & `anatools-3.2.0/anatools/lib/interp.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,14 +102,13 @@
         else:
             # this is either a coding error or a cycle in the graph
             errorString = "Graph execution failed; graph may be cyclic. The following links could not be resolved: "
             linkDescriptions = []
             for name in nodes:
                 for port in nodes[name].inlinks:
                     for inlink in nodes[name].inlinks[port]:
-                        linkDescriptions.append("Node '%s' class '%s' input '%s' link '[%s, %s]'",
-                                                name, nodes[name].__class__.__name__, port, inlink[0], inlink[1])
+                        linkDescriptions.append(f"Node '{name}' class '{nodes[name].__class__.__name__}' input '{port}' link '[{inlink[0]}, {inlink[1]}]'")
             errorString += ', '.join(linkDescriptions)
             logger.error(errorString)
             sys.exit(1)
 
     gc.collect()
```

### Comparing `anatools-3.1.2/anatools/lib/load.py` & `anatools-3.2.0/anatools/lib/load.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/lib/node.py` & `anatools-3.2.0/anatools/lib/node.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/lib/object_utils.py` & `anatools-3.2.0/anatools/lib/object_utils.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/lib/package_utils.py` & `anatools-3.2.0/anatools/lib/package_utils.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/lib/python_main.py` & `anatools-3.2.0/anatools/lib/python_main.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/lib/rigged_object.py` & `anatools-3.2.0/anatools/lib/rigged_object.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/lib/scene.py` & `anatools-3.2.0/anatools/lib/scene.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/lib/search_utils.py` & `anatools-3.2.0/anatools/lib/search_utils.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/nodes/constants.py` & `anatools-3.2.0/anatools/nodes/constants.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/nodes/constants.yml` & `anatools-3.2.0/anatools/nodes/constants.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/nodes/generators.py` & `anatools-3.2.0/anatools/nodes/generators.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/nodes/generators.yml` & `anatools-3.2.0/anatools/nodes/generators.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/nodes/logic.py` & `anatools-3.2.0/anatools/nodes/logic.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/nodes/logic.yml` & `anatools-3.2.0/anatools/nodes/logic.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/nodes/random_generator.py` & `anatools-3.2.0/anatools/nodes/random_generator.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/nodes/random_generator.yml` & `anatools-3.2.0/anatools/nodes/random_generator.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/nodes/sweep_arange.py` & `anatools-3.2.0/anatools/nodes/sweep_arange.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/nodes/sweep_arange.yml` & `anatools-3.2.0/anatools/nodes/sweep_arange.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/nodes/sweep_linspace.py` & `anatools-3.2.0/anatools/nodes/sweep_linspace.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/nodes/sweep_linspace.yml` & `anatools-3.2.0/anatools/nodes/sweep_linspace.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/nodes/vectors.py` & `anatools-3.2.0/anatools/nodes/vectors.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/nodes/vectors.yml` & `anatools-3.2.0/anatools/nodes/vectors.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/nodes/volume_file.py` & `anatools-3.2.0/anatools/nodes/volume_file.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools/nodes/volume_file.yml` & `anatools-3.2.0/anatools/nodes/volume_file.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/anatools.egg-info/PKG-INFO` & `anatools-3.2.0/anatools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anatools
-Version: 3.1.2
+Version: 3.2.0
 Summary: Tools for development with the Rendered.ai Platform.
 Home-page: https://rendered.ai
 Author: Rendered AI, Inc
 Author-email: support@rendered.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `anatools-3.1.2/anatools.egg-info/SOURCES.txt` & `anatools-3.2.0/anatools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -52,16 +52,18 @@
 anatools/lib/__init__.py
 anatools/lib/ana_object.py
 anatools/lib/bbox.py
 anatools/lib/blender_main.py
 anatools/lib/camera_checks.py
 anatools/lib/channel.py
 anatools/lib/context.py
+anatools/lib/directory_object.py
 anatools/lib/download.py
 anatools/lib/file_handlers.py
+anatools/lib/file_metadata.py
 anatools/lib/file_object.py
 anatools/lib/generator.py
 anatools/lib/interp.py
 anatools/lib/load.py
 anatools/lib/node.py
 anatools/lib/object_utils.py
 anatools/lib/package_utils.py
@@ -81,10 +83,12 @@
 anatools/nodes/random_generator.yml
 anatools/nodes/sweep_arange.py
 anatools/nodes/sweep_arange.yml
 anatools/nodes/sweep_linspace.py
 anatools/nodes/sweep_linspace.yml
 anatools/nodes/vectors.py
 anatools/nodes/vectors.yml
+anatools/nodes/volume_directory.py
+anatools/nodes/volume_directory.yml
 anatools/nodes/volume_file.py
 anatools/nodes/volume_file.yml
 tests/test_bbox.py
```

### Comparing `anatools-3.1.2/setup.py` & `anatools-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.2/tests/test_bbox.py` & `anatools-3.2.0/tests/test_bbox.py`

 * *Files identical despite different names*

