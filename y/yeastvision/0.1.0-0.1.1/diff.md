# Comparing `tmp/yeastvision-0.1.0.tar.gz` & `tmp/yeastvision-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeastvision-0.1.0.tar", last modified: Tue Jun 13 10:42:58 2023, max compression
+gzip compressed data, was "yeastvision-0.1.1.tar", last modified: Thu Jun 15 16:00:10 2023, max compression
```

## Comparing `yeastvision-0.1.0.tar` & `yeastvision-0.1.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-13 10:42:58.026209 yeastvision-0.1.0/
--rw-r--r--   0 berk       (502) staff       (20)     1467 2023-06-13 00:33:13.000000 yeastvision-0.1.0/LICENSE
--rw-r--r--   0 berk       (502) staff       (20)      314 2023-06-13 10:42:58.025644 yeastvision-0.1.0/PKG-INFO
--rw-r--r--   0 berk       (502) staff       (20)       38 2023-06-13 10:42:58.026366 yeastvision-0.1.0/setup.cfg
--rw-r--r--   0 berk       (502) staff       (20)     1357 2023-06-13 10:42:53.000000 yeastvision-0.1.0/setup.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-13 10:42:57.999586 yeastvision-0.1.0/yeastvision/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 01:16:17.000000 yeastvision-0.1.0/yeastvision/__init__.py
--rw-rw-r--   0 berk       (502) staff       (20)    76908 2023-06-13 10:40:13.000000 yeastvision-0.1.0/yeastvision/__main__.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-13 10:42:58.003692 yeastvision-0.1.0/yeastvision/disk/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-01-09 00:08:51.000000 yeastvision-0.1.0/yeastvision/disk/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     1019 2023-06-13 10:01:19.000000 yeastvision-0.1.0/yeastvision/disk/io.py
--rw-rw-r--   0 berk       (502) staff       (20)    10386 2023-06-13 10:01:09.000000 yeastvision-0.1.0/yeastvision/disk/reader.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-13 10:42:58.005041 yeastvision-0.1.0/yeastvision/flou/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-02-23 11:08:01.000000 yeastvision-0.1.0/yeastvision/flou/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     1676 2023-06-13 10:06:19.000000 yeastvision-0.1.0/yeastvision/flou/blob_detect.py
--rw-r--r--   0 berk       (502) staff       (20)     1374 2023-03-29 01:49:55.000000 yeastvision-0.1.0/yeastvision/flou/utils.py
--rw-r--r--   0 berk       (502) staff       (20)     2688 2023-04-13 08:05:01.000000 yeastvision-0.1.0/yeastvision/ims.py
--rw-r--r--   0 berk       (502) staff       (20)     2128 2023-06-13 10:32:44.000000 yeastvision-0.1.0/yeastvision/install_weights.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-13 10:42:58.008763 yeastvision-0.1.0/yeastvision/models/
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-13 10:42:58.010952 yeastvision-0.1.0/yeastvision/models/YeaZ/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:23:10.000000 yeastvision-0.1.0/yeastvision/models/YeaZ/__init__.py
--rw-rw-r--   0 berk       (502) staff       (20)     1919 2023-06-13 09:59:20.000000 yeastvision-0.1.0/yeastvision/models/YeaZ/model.py
--rw-rw-r--   0 berk       (502) staff       (20)     6145 2022-09-09 01:01:50.000000 yeastvision-0.1.0/yeastvision/models/YeaZ/segment.py
--rw-r--r--   0 berk       (502) staff       (20)     3665 2022-10-05 10:22:57.000000 yeastvision-0.1.0/yeastvision/models/YeaZ/unet.py
--rw-rw-r--   0 berk       (502) staff       (20)        0 2023-06-13 07:27:49.000000 yeastvision-0.1.0/yeastvision/models/__init__.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-13 10:42:58.011776 yeastvision-0.1.0/yeastvision/models/artilife/
--rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-07 09:15:32.000000 yeastvision-0.1.0/yeastvision/models/artilife/__init__.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-13 10:42:58.012707 yeastvision-0.1.0/yeastvision/models/artilife/budSeg/
--rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-25 06:42:22.000000 yeastvision-0.1.0/yeastvision/models/artilife/budSeg/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      578 2023-02-23 01:09:49.000000 yeastvision-0.1.0/yeastvision/models/artilife/budSeg/model.py
--rw-r--r--   0 berk       (502) staff       (20)     8907 2023-06-13 09:58:10.000000 yeastvision-0.1.0/yeastvision/models/artilife/model.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-13 10:42:58.013562 yeastvision-0.1.0/yeastvision/models/budNET/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:22:46.000000 yeastvision-0.1.0/yeastvision/models/budNET/__init__.py
--rw-rw-r--   0 berk       (502) staff       (20)     1334 2023-06-13 09:58:28.000000 yeastvision-0.1.0/yeastvision/models/budNET/model.py
--rw-r--r--   0 berk       (502) staff       (20)     3736 2023-06-13 09:59:29.000000 yeastvision-0.1.0/yeastvision/models/cp.py
--rw-r--r--   0 berk       (502) staff       (20)       21 2022-12-28 01:01:29.000000 yeastvision-0.1.0/yeastvision/models/eval.py
--rw-r--r--   0 berk       (502) staff       (20)      381 2023-01-19 00:50:23.000000 yeastvision-0.1.0/yeastvision/models/loss.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-13 10:42:58.014413 yeastvision-0.1.0/yeastvision/models/matSeg/
--rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-17 21:54:19.000000 yeastvision-0.1.0/yeastvision/models/matSeg/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      164 2023-06-13 09:58:37.000000 yeastvision-0.1.0/yeastvision/models/matSeg/model.py
--rw-rw-r--   0 berk       (502) staff       (20)     1649 2023-06-13 10:00:05.000000 yeastvision-0.1.0/yeastvision/models/model.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-13 10:42:58.015210 yeastvision-0.1.0/yeastvision/models/tetradSeg/
--rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-17 21:54:27.000000 yeastvision-0.1.0/yeastvision/models/tetradSeg/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      168 2023-06-13 09:58:44.000000 yeastvision-0.1.0/yeastvision/models/tetradSeg/model.py
--rw-rw-r--   0 berk       (502) staff       (20)    14546 2023-06-04 23:09:45.000000 yeastvision-0.1.0/yeastvision/models/unet.py
--rw-rw-r--   0 berk       (502) staff       (20)     6177 2023-06-13 10:04:25.000000 yeastvision-0.1.0/yeastvision/models/utils.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-13 10:42:58.016282 yeastvision-0.1.0/yeastvision/models/vacNET/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:22:37.000000 yeastvision-0.1.0/yeastvision/models/vacNET/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      468 2023-06-13 09:58:56.000000 yeastvision-0.1.0/yeastvision/models/vacNET/model.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-13 10:42:58.019212 yeastvision-0.1.0/yeastvision/parts/
--rw-rw-r--   0 berk       (502) staff       (20)    12988 2023-06-13 09:57:07.000000 yeastvision-0.1.0/yeastvision/parts/canvas.py
--rw-r--r--   0 berk       (502) staff       (20)    30883 2023-06-13 09:57:15.000000 yeastvision-0.1.0/yeastvision/parts/dialogs.py
--rw-rw-r--   0 berk       (502) staff       (20)    11822 2023-06-13 09:57:21.000000 yeastvision-0.1.0/yeastvision/parts/guiparts.py
--rw-r--r--   0 berk       (502) staff       (20)     3662 2023-06-13 10:02:14.000000 yeastvision-0.1.0/yeastvision/parts/menu.py
--rw-r--r--   0 berk       (502) staff       (20)        5 2023-04-12 05:16:38.000000 yeastvision-0.1.0/yeastvision/parts/utils.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-13 10:42:58.020938 yeastvision-0.1.0/yeastvision/plot/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-03-09 00:45:38.000000 yeastvision-0.1.0/yeastvision/plot/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     3241 2023-06-10 01:30:23.000000 yeastvision-0.1.0/yeastvision/plot/cell_table.py
--rw-r--r--   0 berk       (502) staff       (20)     9224 2023-06-13 09:56:38.000000 yeastvision-0.1.0/yeastvision/plot/plot.py
--rw-r--r--   0 berk       (502) staff       (20)     1149 2023-04-05 22:48:46.000000 yeastvision-0.1.0/yeastvision/plot/types.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-13 10:42:58.024991 yeastvision-0.1.0/yeastvision/track/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-03-09 12:09:09.000000 yeastvision-0.1.0/yeastvision/track/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     5908 2023-06-13 09:55:42.000000 yeastvision-0.1.0/yeastvision/track/cell.py
--rw-r--r--   0 berk       (502) staff       (20)      265 2023-06-07 05:33:05.000000 yeastvision-0.1.0/yeastvision/track/data.py
--rw-r--r--   0 berk       (502) staff       (20)     6820 2023-03-08 23:50:11.000000 yeastvision-0.1.0/yeastvision/track/hungarian_track.py
--rw-rw-r--   0 berk       (502) staff       (20)     5515 2023-06-13 09:56:06.000000 yeastvision-0.1.0/yeastvision/track/lineage.py
--rw-rw-r--   0 berk       (502) staff       (20)    16246 2023-06-13 09:56:22.000000 yeastvision-0.1.0/yeastvision/track/track.py
--rw-r--r--   0 berk       (502) staff       (20)     2529 2023-05-25 03:23:59.000000 yeastvision-0.1.0/yeastvision/track/utils.py
--rw-rw-r--   0 berk       (502) staff       (20)     4648 2023-05-23 07:13:40.000000 yeastvision-0.1.0/yeastvision/utils.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-13 10:42:58.002281 yeastvision-0.1.0/yeastvision.egg-info/
--rw-r--r--   0 berk       (502) staff       (20)      314 2023-06-13 10:42:57.000000 yeastvision-0.1.0/yeastvision.egg-info/PKG-INFO
--rw-r--r--   0 berk       (502) staff       (20)     1761 2023-06-13 10:42:57.000000 yeastvision-0.1.0/yeastvision.egg-info/SOURCES.txt
--rw-r--r--   0 berk       (502) staff       (20)        1 2023-06-13 10:42:57.000000 yeastvision-0.1.0/yeastvision.egg-info/dependency_links.txt
--rw-r--r--   0 berk       (502) staff       (20)      116 2023-06-13 10:42:57.000000 yeastvision-0.1.0/yeastvision.egg-info/entry_points.txt
--rw-r--r--   0 berk       (502) staff       (20)      287 2023-06-13 10:42:57.000000 yeastvision-0.1.0/yeastvision.egg-info/requires.txt
--rw-r--r--   0 berk       (502) staff       (20)       12 2023-06-13 10:42:57.000000 yeastvision-0.1.0/yeastvision.egg-info/top_level.txt
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-15 16:00:10.409095 yeastvision-0.1.1/
+-rw-r--r--   0 berk       (502) staff       (20)     1467 2023-06-13 00:33:13.000000 yeastvision-0.1.1/LICENSE
+-rw-r--r--   0 berk       (502) staff       (20)      314 2023-06-15 16:00:10.408709 yeastvision-0.1.1/PKG-INFO
+-rw-r--r--   0 berk       (502) staff       (20)       38 2023-06-15 16:00:10.409199 yeastvision-0.1.1/setup.cfg
+-rw-r--r--   0 berk       (502) staff       (20)     1357 2023-06-15 15:58:24.000000 yeastvision-0.1.1/setup.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-15 16:00:10.392637 yeastvision-0.1.1/yeastvision/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 01:16:17.000000 yeastvision-0.1.1/yeastvision/__init__.py
+-rw-rw-r--   0 berk       (502) staff       (20)    77207 2023-06-15 15:26:45.000000 yeastvision-0.1.1/yeastvision/__main__.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-15 16:00:10.395864 yeastvision-0.1.1/yeastvision/disk/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-01-09 00:08:51.000000 yeastvision-0.1.1/yeastvision/disk/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     1019 2023-06-13 10:01:19.000000 yeastvision-0.1.1/yeastvision/disk/io.py
+-rw-rw-r--   0 berk       (502) staff       (20)    10386 2023-06-13 10:01:09.000000 yeastvision-0.1.1/yeastvision/disk/reader.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-15 16:00:10.396743 yeastvision-0.1.1/yeastvision/flou/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-02-23 11:08:01.000000 yeastvision-0.1.1/yeastvision/flou/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     1676 2023-06-13 10:06:19.000000 yeastvision-0.1.1/yeastvision/flou/blob_detect.py
+-rw-r--r--   0 berk       (502) staff       (20)     1374 2023-03-29 01:49:55.000000 yeastvision-0.1.1/yeastvision/flou/utils.py
+-rw-r--r--   0 berk       (502) staff       (20)     2688 2023-04-13 08:05:01.000000 yeastvision-0.1.1/yeastvision/ims.py
+-rw-r--r--   0 berk       (502) staff       (20)     2128 2023-06-13 10:32:44.000000 yeastvision-0.1.1/yeastvision/install_weights.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-15 16:00:10.399107 yeastvision-0.1.1/yeastvision/models/
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-15 16:00:10.400312 yeastvision-0.1.1/yeastvision/models/YeaZ/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:23:10.000000 yeastvision-0.1.1/yeastvision/models/YeaZ/__init__.py
+-rw-rw-r--   0 berk       (502) staff       (20)     1919 2023-06-13 09:59:20.000000 yeastvision-0.1.1/yeastvision/models/YeaZ/model.py
+-rw-rw-r--   0 berk       (502) staff       (20)     6145 2022-09-09 01:01:50.000000 yeastvision-0.1.1/yeastvision/models/YeaZ/segment.py
+-rw-r--r--   0 berk       (502) staff       (20)     3665 2022-10-05 10:22:57.000000 yeastvision-0.1.1/yeastvision/models/YeaZ/unet.py
+-rw-rw-r--   0 berk       (502) staff       (20)        0 2023-06-13 07:27:49.000000 yeastvision-0.1.1/yeastvision/models/__init__.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-15 16:00:10.400808 yeastvision-0.1.1/yeastvision/models/artilife/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-07 09:15:32.000000 yeastvision-0.1.1/yeastvision/models/artilife/__init__.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-15 16:00:10.401307 yeastvision-0.1.1/yeastvision/models/artilife/budSeg/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-25 06:42:22.000000 yeastvision-0.1.1/yeastvision/models/artilife/budSeg/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      578 2023-02-23 01:09:49.000000 yeastvision-0.1.1/yeastvision/models/artilife/budSeg/model.py
+-rw-r--r--   0 berk       (502) staff       (20)     8907 2023-06-13 09:58:10.000000 yeastvision-0.1.1/yeastvision/models/artilife/model.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-15 16:00:10.401787 yeastvision-0.1.1/yeastvision/models/budNET/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:22:46.000000 yeastvision-0.1.1/yeastvision/models/budNET/__init__.py
+-rw-rw-r--   0 berk       (502) staff       (20)     1334 2023-06-13 09:58:28.000000 yeastvision-0.1.1/yeastvision/models/budNET/model.py
+-rw-r--r--   0 berk       (502) staff       (20)     3736 2023-06-13 09:59:29.000000 yeastvision-0.1.1/yeastvision/models/cp.py
+-rw-r--r--   0 berk       (502) staff       (20)       21 2022-12-28 01:01:29.000000 yeastvision-0.1.1/yeastvision/models/eval.py
+-rw-r--r--   0 berk       (502) staff       (20)      381 2023-01-19 00:50:23.000000 yeastvision-0.1.1/yeastvision/models/loss.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-15 16:00:10.402266 yeastvision-0.1.1/yeastvision/models/matSeg/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-17 21:54:19.000000 yeastvision-0.1.1/yeastvision/models/matSeg/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      164 2023-06-13 09:58:37.000000 yeastvision-0.1.1/yeastvision/models/matSeg/model.py
+-rw-rw-r--   0 berk       (502) staff       (20)     1649 2023-06-13 10:00:05.000000 yeastvision-0.1.1/yeastvision/models/model.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-15 16:00:10.402712 yeastvision-0.1.1/yeastvision/models/tetradSeg/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2022-10-17 21:54:27.000000 yeastvision-0.1.1/yeastvision/models/tetradSeg/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      168 2023-06-13 09:58:44.000000 yeastvision-0.1.1/yeastvision/models/tetradSeg/model.py
+-rw-rw-r--   0 berk       (502) staff       (20)    14546 2023-06-04 23:09:45.000000 yeastvision-0.1.1/yeastvision/models/unet.py
+-rw-rw-r--   0 berk       (502) staff       (20)     6177 2023-06-13 10:04:25.000000 yeastvision-0.1.1/yeastvision/models/utils.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-15 16:00:10.403190 yeastvision-0.1.1/yeastvision/models/vacNET/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-06-13 10:22:37.000000 yeastvision-0.1.1/yeastvision/models/vacNET/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      468 2023-06-13 09:58:56.000000 yeastvision-0.1.1/yeastvision/models/vacNET/model.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-15 16:00:10.404790 yeastvision-0.1.1/yeastvision/parts/
+-rw-rw-r--   0 berk       (502) staff       (20)    13051 2023-06-13 11:05:47.000000 yeastvision-0.1.1/yeastvision/parts/canvas.py
+-rw-r--r--   0 berk       (502) staff       (20)    30883 2023-06-13 09:57:15.000000 yeastvision-0.1.1/yeastvision/parts/dialogs.py
+-rw-rw-r--   0 berk       (502) staff       (20)    11822 2023-06-13 09:57:21.000000 yeastvision-0.1.1/yeastvision/parts/guiparts.py
+-rw-r--r--   0 berk       (502) staff       (20)     3662 2023-06-13 10:02:14.000000 yeastvision-0.1.1/yeastvision/parts/menu.py
+-rw-r--r--   0 berk       (502) staff       (20)        5 2023-04-12 05:16:38.000000 yeastvision-0.1.1/yeastvision/parts/utils.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-15 16:00:10.405866 yeastvision-0.1.1/yeastvision/plot/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-03-09 00:45:38.000000 yeastvision-0.1.1/yeastvision/plot/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     3442 2023-06-14 19:37:54.000000 yeastvision-0.1.1/yeastvision/plot/cell_table.py
+-rw-r--r--   0 berk       (502) staff       (20)     9224 2023-06-14 19:25:48.000000 yeastvision-0.1.1/yeastvision/plot/plot.py
+-rw-r--r--   0 berk       (502) staff       (20)     1149 2023-04-05 22:48:46.000000 yeastvision-0.1.1/yeastvision/plot/types.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-15 16:00:10.408279 yeastvision-0.1.1/yeastvision/track/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-03-09 12:09:09.000000 yeastvision-0.1.1/yeastvision/track/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     5908 2023-06-13 09:55:42.000000 yeastvision-0.1.1/yeastvision/track/cell.py
+-rw-r--r--   0 berk       (502) staff       (20)      265 2023-06-07 05:33:05.000000 yeastvision-0.1.1/yeastvision/track/data.py
+-rw-r--r--   0 berk       (502) staff       (20)     6820 2023-03-08 23:50:11.000000 yeastvision-0.1.1/yeastvision/track/hungarian_track.py
+-rw-rw-r--   0 berk       (502) staff       (20)     5515 2023-06-13 09:56:06.000000 yeastvision-0.1.1/yeastvision/track/lineage.py
+-rw-rw-r--   0 berk       (502) staff       (20)    16246 2023-06-13 09:56:22.000000 yeastvision-0.1.1/yeastvision/track/track.py
+-rw-r--r--   0 berk       (502) staff       (20)     2529 2023-05-25 03:23:59.000000 yeastvision-0.1.1/yeastvision/track/utils.py
+-rw-rw-r--   0 berk       (502) staff       (20)     4648 2023-05-23 07:13:40.000000 yeastvision-0.1.1/yeastvision/utils.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2023-06-15 16:00:10.394910 yeastvision-0.1.1/yeastvision.egg-info/
+-rw-r--r--   0 berk       (502) staff       (20)      314 2023-06-15 16:00:10.000000 yeastvision-0.1.1/yeastvision.egg-info/PKG-INFO
+-rw-r--r--   0 berk       (502) staff       (20)     1761 2023-06-15 16:00:10.000000 yeastvision-0.1.1/yeastvision.egg-info/SOURCES.txt
+-rw-r--r--   0 berk       (502) staff       (20)        1 2023-06-15 16:00:10.000000 yeastvision-0.1.1/yeastvision.egg-info/dependency_links.txt
+-rw-r--r--   0 berk       (502) staff       (20)      116 2023-06-15 16:00:10.000000 yeastvision-0.1.1/yeastvision.egg-info/entry_points.txt
+-rw-r--r--   0 berk       (502) staff       (20)      287 2023-06-15 16:00:10.000000 yeastvision-0.1.1/yeastvision.egg-info/requires.txt
+-rw-r--r--   0 berk       (502) staff       (20)       12 2023-06-15 16:00:10.000000 yeastvision-0.1.1/yeastvision.egg-info/top_level.txt
```

### Comparing `yeastvision-0.1.0/LICENSE` & `yeastvision-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/setup.py` & `yeastvision-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             "yeastvision.parts", "yeastvision.flou", "yeastvision.disk", 
             "yeastvision.models.artilife", "yeastvision.models.artilife.budSeg",
             "yeastvision.models.matSeg", "yeastvision.models.tetradSeg", "yeastvision.models.budNET", 
             "yeastvision.models.vacNET", "yeastvision.models.YeaZ"]
 
 setup(
     name = "yeastvision",
-    version = "0.1.0",
+    version = "0.1.1",
     description = "Deep learning-enabled image analysis of the yeast full life cycle",
     author = "Berk Yalcinkaya",
     url = "https://github.com/berkyalcinkaya/budNET_gui",
     author_email="berkyalcinkaya55@gmail.com",
     license = "BSD",
     packages = packages,
     install_requires = requires,
```

### Comparing `yeastvision-0.1.0/yeastvision/__main__.py` & `yeastvision-0.1.1/yeastvision/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,14 +203,16 @@
                 self.maskChanged = True
                 self._maskZ = num
         except AttributeError:
             self._maskZ  = num
         if num>=0:
             try:
                 self.checkDataAvailibility()
+                # if self.pWindow:
+                #     self.
             except IndexError:
                 pass
         
     
     @property
     def tIndex(self):
         return self._tIndex
@@ -468,14 +470,15 @@
         self.brushTypeSelect.currentIndexChanged.connect(self.brushTypeChoose)
         self.brushTypeSelect.setStyleSheet(self.dropdowns)
         self.brushTypeSelect.setFont(self.medfont)
         self.brushTypeSelect.setCurrentText("")
         self.brushTypeSelect.setFocusPolicy(QtCore.Qt.NoFocus)
         self.brushTypeSelect.setEnabled(False)
         self.brushTypeSelect.setFixedWidth(90)
+        self.brushTypeSelect.setEnabled(False)
         self.l.addWidget(self.brushTypeSelect, rowspace+1,2,1,1)
 
         
         label = QLabel("Brush Size")
         label.setStyleSheet(self.labelstyle)
         label.setFont(self.medfont)
         self.l.addWidget(label, rowspace+2,0,1,2)
@@ -848,14 +851,20 @@
 
         self.checkDataAvailibility()  
 
         if self.pWindow:
             self.pWindow.setData()
             self.pWindow.updatePlots()
     
+    def updateCellTable(self):
+        if not self.pWindow:
+            return
+        # self.pWindow.table.model.setData(self.getCellDataAbbrev())
+        # self.pWindow.
+    
 
     def hasCellData(self, i = None):
         if type(i) is not int:
             i = self.maskZ
         return (type(self.cellData[i]) is pd.core.frame.DataFrame)
     
     def hasLineageData(self, i = None):
@@ -1555,15 +1564,15 @@
         
     def getModels(self):
         for modelName in self.modelNames:
             if os.path.exists(os.path.join("models",modelName,"model.py")):
                 importlib.import_module(self.getPkgString(modelName))
     
     def getPkgString(self, string):
-        return f"models.{string}.model"
+        return f"yeastvision.models.{string}.model"
 
     def getModelClass(self, modelName):
         module = importlib.import_module(self.getPkgString(modelName))
         modelClass = getattr(module, capitalize(modelName))
         return modelClass
     
     def showTW(self):
```

### Comparing `yeastvision-0.1.0/yeastvision/disk/io.py` & `yeastvision-0.1.1/yeastvision/disk/io.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/disk/reader.py` & `yeastvision-0.1.1/yeastvision/disk/reader.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/flou/blob_detect.py` & `yeastvision-0.1.1/yeastvision/flou/blob_detect.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/flou/utils.py` & `yeastvision-0.1.1/yeastvision/flou/utils.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/ims.py` & `yeastvision-0.1.1/yeastvision/ims.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/install_weights.py` & `yeastvision-0.1.1/yeastvision/install_weights.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/models/YeaZ/model.py` & `yeastvision-0.1.1/yeastvision/models/YeaZ/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/models/YeaZ/segment.py` & `yeastvision-0.1.1/yeastvision/models/YeaZ/segment.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/models/YeaZ/unet.py` & `yeastvision-0.1.1/yeastvision/models/YeaZ/unet.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/models/artilife/budSeg/model.py` & `yeastvision-0.1.1/yeastvision/models/artilife/budSeg/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/models/artilife/model.py` & `yeastvision-0.1.1/yeastvision/models/artilife/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/models/budNET/model.py` & `yeastvision-0.1.1/yeastvision/models/budNET/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/models/cp.py` & `yeastvision-0.1.1/yeastvision/models/cp.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/models/model.py` & `yeastvision-0.1.1/yeastvision/models/model.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/models/unet.py` & `yeastvision-0.1.1/yeastvision/models/unet.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/models/utils.py` & `yeastvision-0.1.1/yeastvision/models/utils.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/parts/canvas.py` & `yeastvision-0.1.1/yeastvision/parts/canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,25 +48,28 @@
         bs = kernel_size
         kernel = np.ones((bs,bs), np.uint8)
         self.drawKernel = kernel
         self.drawKernelCenter = [int(np.floor(kernel.shape[0]/2)),
                                  int(np.floor(kernel.shape[1]/2))]
     
     def mouseClickEvent(self, ev):
+        if not self.parent.imLoaded:
+            return
+        
         cellNum = self.parent.currMask[int(ev.pos().y()), int(ev.pos().x())]
         
         if ev.button() == QtCore.Qt.LeftButton and self.parent.maskOn:
             if cellNum!=0:
                 self.parent.selectCell(ev.pos())
         
         # mask must be on for drawing
         elif ev.button() == QtCore.Qt.RightButton and not self.parent.probOn and self.parent.maskOn:
             
             if self.parent.drawType != "":
-                if self.parent.maskData.isDummy:
+                if not self.parent.maskLoaded:
                     self.parent.loadMasks(self.parent.maskData.channels[self.parent.maskZ][0,:,:,:], 
                                       name = self.parent.channelSelect.currentText() + "-draw")
                 
                 # different brush modes
                 if self.parent.drawType == "Brush":
                     self.colorNum = self.parent.selectedCells[0] if self.parent.selectedCells else self.parent.currMask.max()+1
                     self.drawAt(ev.pos())
```

### Comparing `yeastvision-0.1.0/yeastvision/parts/dialogs.py` & `yeastvision-0.1.1/yeastvision/parts/dialogs.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/parts/guiparts.py` & `yeastvision-0.1.1/yeastvision/parts/guiparts.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/parts/menu.py` & `yeastvision-0.1.1/yeastvision/parts/menu.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/plot/cell_table.py` & `yeastvision-0.1.1/yeastvision/plot/cell_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,9 +74,14 @@
             return
         if (new.column() == self.columns["cell"] or new.column() == self.columns["mother"]) and self.hasLineages:
             value = int(self._data.iloc[new.row(), new.column()])
             mother = self._data.iloc[value-1, self.columns["mother"]]
             birth = int(self._data.iloc[value-1, self.columns["birth"]])
             self.main.showMotherDaughter(mother, value, birth)
         
+        if (new.column() in [self.columns["birth"], self.columns["death"]]):
+            self.parent.tIndex = int(self._data.iloc[new.row(), new.column()])
+            self.parent.drawMask()
+
+
```

### Comparing `yeastvision-0.1.0/yeastvision/plot/plot.py` & `yeastvision-0.1.1/yeastvision/plot/plot.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/plot/types.py` & `yeastvision-0.1.1/yeastvision/plot/types.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/track/cell.py` & `yeastvision-0.1.1/yeastvision/track/cell.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/track/hungarian_track.py` & `yeastvision-0.1.1/yeastvision/track/hungarian_track.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/track/lineage.py` & `yeastvision-0.1.1/yeastvision/track/lineage.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/track/track.py` & `yeastvision-0.1.1/yeastvision/track/track.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/track/utils.py` & `yeastvision-0.1.1/yeastvision/track/utils.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision/utils.py` & `yeastvision-0.1.1/yeastvision/utils.py`

 * *Files identical despite different names*

### Comparing `yeastvision-0.1.0/yeastvision.egg-info/SOURCES.txt` & `yeastvision-0.1.1/yeastvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

