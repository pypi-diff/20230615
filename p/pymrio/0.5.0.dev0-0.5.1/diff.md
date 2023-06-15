# Comparing `tmp/pymrio-0.5.0.dev0.tar.gz` & `tmp/pymrio-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymrio-0.5.0.dev0.tar", last modified: Thu Jun 15 19:57:48 2023, max compression
+gzip compressed data, was "pymrio-0.5.1.tar", last modified: Thu Jun 15 20:34:33 2023, max compression
```

## Comparing `pymrio-0.5.0.dev0.tar` & `pymrio-0.5.1.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.995972 pymrio-0.5.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-06-15 19:57:47.995972 pymrio-0.5.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.983971 pymrio-0.5.0.dev0/pymrio/
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.983971 pymrio-0.5.0.dev0/pymrio/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22836 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    33413 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/core/fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)    92621 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/core/mriosystem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.983971 pymrio-0.5.0.dev0/pymrio/mrio_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.983971 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.987972 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ALL.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/Africa.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/America.txt
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/AsiaPacific.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/BRIC.txt
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/EU.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/Europe.txt
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_A.txt
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_B.txt
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_C.txt
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_D.txt
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_E.txt
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_F.txt
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_G_H.txt
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_I.txt
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_J_K.txt
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_L.txt
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_M_N_O.txt
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_P.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/MiddleEast.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/OECD.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/RoW.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/orig_regions.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_A.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_B.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_C.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_D.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_E.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_F.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_G_H.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_I.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_J_K.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_L.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_M_N_O.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_P.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.987972 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/misc/population.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.987972 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.991972 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ALL.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/Africa.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/America.txt
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/AsiaPacific.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/BRIC.txt
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/EU.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/Europe.txt
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_A.txt
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_B.txt
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_C.txt
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_D.txt
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_E.txt
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_F.txt
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_G_H.txt
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_I.txt
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_J_K.txt
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_L.txt
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_M_N_O.txt
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_P.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/MiddleEast.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/OECD.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/RoW.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/orig_regions.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_A.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_B.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_C.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_D.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_E.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_F.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_G_H.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_I.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_J_K.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_L.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_M_N_O.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_P.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.991972 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/misc/population.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.991972 pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_ixi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_ixi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_ixi/finaldemand.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    19783 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_ixi/sectors.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_ixi/valueadded.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.991972 pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_pxp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_pxp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_pxp/finaldemand.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    14758 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_pxp/sectors.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_pxp/valueadded.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.991972 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.991972 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/EU.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/OECD.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/emissions_charact.tsv
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/orig_regions.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/orig_sectors.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/sector1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/sector2.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/sector3.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/supreg1.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/supreg2.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/finaldemand.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.995972 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/FDemissions.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/emissions.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/factor_input.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/finald_demand_Y.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/population.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)    24805 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/trade_flows_Z.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/sectors.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.995972 pymrio-0.5.0.dev0/pymrio/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/tools/ioclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    24097 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/tools/iodownloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/tools/iomath.py
--rw-r--r--   0 runner    (1001) docker     (123)    16201 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/tools/iometadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    66586 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/tools/ioparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    21204 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/tools/ioutil.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.983971 pymrio-0.5.0.dev0/pymrio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-06-15 19:57:47.000000 pymrio-0.5.0.dev0/pymrio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-15 19:57:47.000000 pymrio-0.5.0.dev0/pymrio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:57:47.000000 pymrio-0.5.0.dev0/pymrio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-15 19:57:47.000000 pymrio-0.5.0.dev0/pymrio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 19:57:47.000000 pymrio-0.5.0.dev0/pymrio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 19:57:47.995972 pymrio-0.5.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.995972 pymrio-0.5.0.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/tests/test_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15544 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    18874 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/tests/test_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:33.849322 pymrio-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-15 20:34:03.000000 pymrio-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-15 20:34:03.000000 pymrio-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-06-15 20:34:33.845322 pymrio-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-15 20:34:03.000000 pymrio-0.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:33.833322 pymrio-0.5.1/pymrio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:33.833322 pymrio-0.5.1/pymrio/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22836 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33413 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/core/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92621 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/core/mriosystem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:33.837322 pymrio-0.5.1/pymrio/mrio_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:33.837322 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:33.837322 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/ALL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/Africa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/America.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/AsiaPacific.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/BRIC.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/EU.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/Europe.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/ISIC_A.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/ISIC_B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/ISIC_C.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/ISIC_D.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/ISIC_E.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/ISIC_F.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/ISIC_G_H.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/ISIC_I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/ISIC_J_K.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/ISIC_L.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/ISIC_M_N_O.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/ISIC_P.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/MiddleEast.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/OECD.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/RoW.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/orig_regions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_A.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_C.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_D.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_E.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_F.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_G_H.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_J_K.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_L.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_M_N_O.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_P.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:33.837322 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/misc/population.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:33.837322 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:33.841322 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/ALL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/Africa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/America.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/AsiaPacific.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/BRIC.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/EU.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/Europe.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/ISIC_A.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/ISIC_B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/ISIC_C.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/ISIC_D.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/ISIC_E.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/ISIC_F.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/ISIC_G_H.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/ISIC_I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/ISIC_J_K.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/ISIC_L.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/ISIC_M_N_O.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/ISIC_P.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/MiddleEast.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/OECD.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/RoW.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/orig_regions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_A.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_C.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_D.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_E.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_F.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_G_H.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_J_K.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_L.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_M_N_O.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_P.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:33.841322 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/misc/population.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:33.841322 pymrio-0.5.1/pymrio/mrio_models/exio3_ixi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio3_ixi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio3_ixi/finaldemand.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    19783 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio3_ixi/sectors.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio3_ixi/valueadded.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:33.845322 pymrio-0.5.1/pymrio/mrio_models/exio3_pxp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio3_pxp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio3_pxp/finaldemand.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    14758 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio3_pxp/sectors.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/exio3_pxp/valueadded.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:33.845322 pymrio-0.5.1/pymrio/mrio_models/test_mrio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:33.845322 pymrio-0.5.1/pymrio/mrio_models/test_mrio/concordance/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/concordance/EU.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/concordance/OECD.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/concordance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/concordance/emissions_charact.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/concordance/orig_regions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/concordance/orig_sectors.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/concordance/sector1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/concordance/sector2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/concordance/sector3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/concordance/supreg1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/concordance/supreg2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/finaldemand.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:33.845322 pymrio-0.5.1/pymrio/mrio_models/test_mrio/mrio_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/mrio_data/FDemissions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/mrio_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/mrio_data/emissions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/mrio_data/factor_input.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/mrio_data/finald_demand_Y.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/mrio_data/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/mrio_data/population.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/mrio_data/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    24805 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/mrio_data/trade_flows_Z.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/mrio_models/test_mrio/sectors.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:33.845322 pymrio-0.5.1/pymrio/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/tools/ioclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24097 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/tools/iodownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/tools/iomath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16201 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/tools/iometadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66586 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/tools/ioparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21204 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/tools/ioutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 20:34:03.000000 pymrio-0.5.1/pymrio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:33.833322 pymrio-0.5.1/pymrio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-06-15 20:34:33.000000 pymrio-0.5.1/pymrio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-15 20:34:33.000000 pymrio-0.5.1/pymrio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 20:34:33.000000 pymrio-0.5.1/pymrio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-15 20:34:33.000000 pymrio-0.5.1/pymrio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 20:34:33.000000 pymrio-0.5.1/pymrio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 20:34:33.849322 pymrio-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-15 20:34:03.000000 pymrio-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:34:33.845322 pymrio-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-15 20:34:03.000000 pymrio-0.5.1/tests/test_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15544 2023-06-15 20:34:03.000000 pymrio-0.5.1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-06-15 20:34:03.000000 pymrio-0.5.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18874 2023-06-15 20:34:03.000000 pymrio-0.5.1/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-15 20:34:03.000000 pymrio-0.5.1/tests/test_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-06-15 20:34:03.000000 pymrio-0.5.1/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-06-15 20:34:03.000000 pymrio-0.5.1/tests/test_util.py
```

### Comparing `pymrio-0.5.0.dev0/LICENSE` & `pymrio-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/PKG-INFO` & `pymrio-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pymrio
-Version: 0.5.0.dev0
+Version: 0.5.1
 Summary: A python module for automating input output calculations and generating reports
 Home-page: https://github.com/IndEcol/pymrio
 Author: Konstantin Stadler
 Author-email: konstantin.stadler@ntnu.no
 License: UNKNOWN
 Description: ############
         Pymrio
```

### Comparing `pymrio-0.5.0.dev0/README.rst` & `pymrio-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio/__init__.py` & `pymrio-0.5.1/pymrio/__init__.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio/core/constants.py` & `pymrio-0.5.1/pymrio/core/constants.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio/core/fileio.py` & `pymrio-0.5.1/pymrio/core/fileio.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio/core/mriosystem.py` & `pymrio-0.5.1/pymrio/core/mriosystem.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/misc/population.txt` & `pymrio-0.5.1/pymrio/mrio_models/exio2_ixi/misc/population.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/misc/population.txt` & `pymrio-0.5.1/pymrio/mrio_models/exio2_pxp/misc/population.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_ixi/sectors.tsv` & `pymrio-0.5.1/pymrio/mrio_models/exio3_ixi/sectors.tsv`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_ixi/valueadded.tsv` & `pymrio-0.5.1/pymrio/mrio_models/exio3_ixi/valueadded.tsv`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_pxp/sectors.tsv` & `pymrio-0.5.1/pymrio/mrio_models/exio3_pxp/sectors.tsv`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_pxp/valueadded.tsv` & `pymrio-0.5.1/pymrio/mrio_models/exio3_pxp/valueadded.tsv`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/FDemissions.txt` & `pymrio-0.5.1/pymrio/mrio_models/test_mrio/mrio_data/FDemissions.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/emissions.txt` & `pymrio-0.5.1/pymrio/mrio_models/test_mrio/mrio_data/emissions.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/factor_input.txt` & `pymrio-0.5.1/pymrio/mrio_models/test_mrio/mrio_data/factor_input.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/finald_demand_Y.txt` & `pymrio-0.5.1/pymrio/mrio_models/test_mrio/mrio_data/finald_demand_Y.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/trade_flows_Z.txt` & `pymrio-0.5.1/pymrio/mrio_models/test_mrio/mrio_data/trade_flows_Z.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio/tools/ioclass.py` & `pymrio-0.5.1/pymrio/tools/ioclass.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio/tools/iodownloader.py` & `pymrio-0.5.1/pymrio/tools/iodownloader.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio/tools/iomath.py` & `pymrio-0.5.1/pymrio/tools/iomath.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio/tools/iometadata.py` & `pymrio-0.5.1/pymrio/tools/iometadata.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio/tools/ioparser.py` & `pymrio-0.5.1/pymrio/tools/ioparser.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio/tools/ioutil.py` & `pymrio-0.5.1/pymrio/tools/ioutil.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/pymrio.egg-info/PKG-INFO` & `pymrio-0.5.1/pymrio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pymrio
-Version: 0.5.0.dev0
+Version: 0.5.1
 Summary: A python module for automating input output calculations and generating reports
 Home-page: https://github.com/IndEcol/pymrio
 Author: Konstantin Stadler
 Author-email: konstantin.stadler@ntnu.no
 License: UNKNOWN
 Description: ############
         Pymrio
```

### Comparing `pymrio-0.5.0.dev0/pymrio.egg-info/SOURCES.txt` & `pymrio-0.5.1/pymrio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/setup.py` & `pymrio-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/tests/test_aggregation.py` & `pymrio-0.5.1/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/tests/test_core.py` & `pymrio-0.5.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/tests/test_integration.py` & `pymrio-0.5.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/tests/test_math.py` & `pymrio-0.5.1/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/tests/test_outputs.py` & `pymrio-0.5.1/tests/test_outputs.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/tests/test_parsers.py` & `pymrio-0.5.1/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.5.0.dev0/tests/test_util.py` & `pymrio-0.5.1/tests/test_util.py`

 * *Files identical despite different names*

