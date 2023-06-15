# Comparing `tmp/pymrio-0.4.8.tar.gz` & `tmp/pymrio-0.5.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymrio-0.4.8.tar", last modified: Wed Nov 16 08:44:52 2022, max compression
+gzip compressed data, was "pymrio-0.5.0.dev0.tar", last modified: Thu Jun 15 19:57:48 2023, max compression
```

## Comparing `pymrio-0.4.8.tar` & `pymrio-0.5.0.dev0.tar`

### file list

```diff
@@ -1,142 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:52.641048 pymrio-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (121)    32463 2022-11-16 08:44:31.000000 pymrio-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-11-16 08:44:31.000000 pymrio-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9049 2022-11-16 08:44:52.641048 pymrio-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6423 2022-11-16 08:44:31.000000 pymrio-0.4.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:52.633048 pymrio-0.4.8/pymrio/
--rw-r--r--   0 runner    (1001) docker     (121)     1677 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:52.633048 pymrio-0.4.8/pymrio/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    32548 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/core/fileio.py
--rw-r--r--   0 runner    (1001) docker     (121)    92615 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/core/mriosystem.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:52.633048 pymrio-0.4.8/pymrio/mrio_models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:52.633048 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:52.637048 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/ALL.txt
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/Africa.txt
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/America.txt
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/AsiaPacific.txt
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/BRIC.txt
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/EU.txt
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/Europe.txt
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/ISIC_A.txt
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/ISIC_B.txt
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/ISIC_C.txt
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/ISIC_D.txt
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/ISIC_E.txt
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/ISIC_F.txt
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/ISIC_G_H.txt
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/ISIC_I.txt
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/ISIC_J_K.txt
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/ISIC_L.txt
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/ISIC_M_N_O.txt
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/ISIC_P.txt
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/MiddleEast.txt
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/OECD.txt
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/RoW.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/orig_regions.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_A.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_B.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_C.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_D.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_E.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_F.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_G_H.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_I.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_J_K.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_L.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_M_N_O.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_P.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:52.637048 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/misc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/misc/population.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:52.637048 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:52.641048 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/ALL.txt
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/Africa.txt
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/America.txt
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/AsiaPacific.txt
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/BRIC.txt
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/EU.txt
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/Europe.txt
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/ISIC_A.txt
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/ISIC_B.txt
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/ISIC_C.txt
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/ISIC_D.txt
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/ISIC_E.txt
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/ISIC_F.txt
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/ISIC_G_H.txt
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/ISIC_I.txt
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/ISIC_J_K.txt
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/ISIC_L.txt
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/ISIC_M_N_O.txt
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/ISIC_P.txt
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/MiddleEast.txt
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/OECD.txt
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/RoW.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/orig_regions.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_A.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_B.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_C.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_D.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_E.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_F.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_G_H.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_I.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_J_K.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_L.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_M_N_O.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_P.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:52.641048 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/misc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/misc/population.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:52.641048 pymrio-0.4.8/pymrio/mrio_models/exio3_ixi/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio3_ixi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:52.641048 pymrio-0.4.8/pymrio/mrio_models/exio3_pxp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/exio3_pxp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:52.641048 pymrio-0.4.8/pymrio/mrio_models/test_mrio/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/test_mrio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:52.641048 pymrio-0.4.8/pymrio/mrio_models/test_mrio/concordance/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/test_mrio/concordance/EU.txt
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/test_mrio/concordance/OECD.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/test_mrio/concordance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/test_mrio/concordance/orig_regions.txt
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/test_mrio/concordance/orig_sectors.txt
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/test_mrio/concordance/sector1.txt
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/test_mrio/concordance/sector2.txt
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/test_mrio/concordance/sector3.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/test_mrio/concordance/supreg1.txt
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/test_mrio/concordance/supreg2.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:52.641048 pymrio-0.4.8/pymrio/mrio_models/test_mrio/mrio_data/
--rw-r--r--   0 runner    (1001) docker     (121)     2065 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/test_mrio/mrio_data/FDemissions.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/test_mrio/mrio_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/test_mrio/mrio_data/emissions.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/test_mrio/mrio_data/factor_input.txt
--rw-r--r--   0 runner    (1001) docker     (121)    19990 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/test_mrio/mrio_data/finald_demand_Y.txt
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/test_mrio/mrio_data/metadata.json
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/test_mrio/mrio_data/population.txt
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/test_mrio/mrio_data/readme.txt
--rw-r--r--   0 runner    (1001) docker     (121)    24805 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/mrio_models/test_mrio/mrio_data/trade_flows_Z.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:52.641048 pymrio-0.4.8/pymrio/tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3071 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/tools/ioclass.py
--rw-r--r--   0 runner    (1001) docker     (121)    19225 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/tools/iodownloader.py
--rw-r--r--   0 runner    (1001) docker     (121)    14448 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/tools/iomath.py
--rw-r--r--   0 runner    (1001) docker     (121)    11709 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/tools/iometadata.py
--rw-r--r--   0 runner    (1001) docker     (121)    66586 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/tools/ioparser.py
--rw-r--r--   0 runner    (1001) docker     (121)    19373 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/tools/ioutil.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-16 08:44:31.000000 pymrio-0.4.8/pymrio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:44:52.633048 pymrio-0.4.8/pymrio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9049 2022-11-16 08:44:52.000000 pymrio-0.4.8/pymrio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5822 2022-11-16 08:44:52.000000 pymrio-0.4.8/pymrio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 08:44:52.000000 pymrio-0.4.8/pymrio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-11-16 08:44:52.000000 pymrio-0.4.8/pymrio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-16 08:44:52.000000 pymrio-0.4.8/pymrio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-16 08:44:52.641048 pymrio-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-11-16 08:44:31.000000 pymrio-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.995972 pymrio-0.5.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-06-15 19:57:47.995972 pymrio-0.5.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.983971 pymrio-0.5.0.dev0/pymrio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.983971 pymrio-0.5.0.dev0/pymrio/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22836 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33413 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/core/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92621 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/core/mriosystem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.983971 pymrio-0.5.0.dev0/pymrio/mrio_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.983971 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.987972 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ALL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/Africa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/America.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/AsiaPacific.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/BRIC.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/EU.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/Europe.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_A.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_C.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_D.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_E.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_F.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_G_H.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_J_K.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_L.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_M_N_O.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/ISIC_P.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/MiddleEast.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/OECD.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/RoW.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/orig_regions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_A.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_C.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_D.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_E.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_F.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_G_H.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_J_K.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_L.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_M_N_O.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/concordance/pro_ISIC_P.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.987972 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/misc/population.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.987972 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.991972 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ALL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/Africa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/America.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/AsiaPacific.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/BRIC.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/EU.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/Europe.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_A.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_C.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_D.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_E.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_F.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_G_H.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_J_K.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_L.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_M_N_O.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/ISIC_P.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/MiddleEast.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/OECD.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/RoW.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/orig_regions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_A.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_C.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_D.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_E.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_F.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_G_H.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_J_K.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_L.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_M_N_O.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_P.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.991972 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/misc/population.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.991972 pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_ixi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_ixi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_ixi/finaldemand.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    19783 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_ixi/sectors.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_ixi/valueadded.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.991972 pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_pxp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_pxp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_pxp/finaldemand.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    14758 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_pxp/sectors.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/exio3_pxp/valueadded.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.991972 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.991972 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/EU.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/OECD.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/emissions_charact.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/orig_regions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/orig_sectors.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/sector1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/sector2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/sector3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/supreg1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/concordance/supreg2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/finaldemand.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.995972 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/FDemissions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/emissions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/factor_input.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/finald_demand_Y.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/population.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    24805 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/trade_flows_Z.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/sectors.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.995972 pymrio-0.5.0.dev0/pymrio/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/tools/ioclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24097 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/tools/iodownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/tools/iomath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16201 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/tools/iometadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66586 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/tools/ioparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21204 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/tools/ioutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/pymrio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.983971 pymrio-0.5.0.dev0/pymrio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-06-15 19:57:47.000000 pymrio-0.5.0.dev0/pymrio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-15 19:57:47.000000 pymrio-0.5.0.dev0/pymrio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:57:47.000000 pymrio-0.5.0.dev0/pymrio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-15 19:57:47.000000 pymrio-0.5.0.dev0/pymrio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 19:57:47.000000 pymrio-0.5.0.dev0/pymrio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 19:57:47.995972 pymrio-0.5.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:57:47.995972 pymrio-0.5.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/tests/test_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15544 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18874 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/tests/test_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-06-15 19:57:15.000000 pymrio-0.5.0.dev0/tests/test_util.py
```

### Comparing `pymrio-0.4.8/PKG-INFO` & `pymrio-0.5.0.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 1.2
 Name: pymrio
-Version: 0.4.8
+Version: 0.5.0.dev0
 Summary: A python module for automating input output calculations and generating reports
-Home-page: https://github.com/konstantinstadler/pymrio
+Home-page: https://github.com/IndEcol/pymrio
 Author: Konstantin Stadler
 Author-email: konstantin.stadler@ntnu.no
 License: UNKNOWN
 Description: ############
         Pymrio
         ############
         
         Pymrio: Multi-Regional Input-Output Analysis in Python.
         
         .. image:: https://img.shields.io/pypi/v/pymrio.svg
             :target: https://pypi.python.org/pypi/pymrio/
         .. image:: https://anaconda.org/conda-forge/pymrio/badges/version.svg   
             :target: https://anaconda.org/conda-forge/pymrio
-        .. image:: https://github.com/konstantinstadler/pymrio/workflows/build/badge.svg
-            :target: https://github.com/konstantinstadler/pymrio/actions
-        .. image:: https://coveralls.io/repos/github/konstantinstadler/pymrio/badge.svg?branch=master
-            :target: https://coveralls.io/github/konstantinstadler/pymrio
+        .. image:: https://github.com/IndEcol/pymrio/workflows/build/badge.svg
+            :target: https://github.com/IndEcol/pymrio/actions
+        .. image:: https://coveralls.io/repos/github/IndEcol/pymrio/badge.svg?branch=master
+            :target: https://coveralls.io/github/IndEcol/pymrio
         .. image:: https://readthedocs.org/projects/pymrio/badge/?version=latest
             :target: http://pymrio.readthedocs.io/en/latest/?badge=latest
             :alt: Documentation Status
         .. image:: https://img.shields.io/badge/License-GPL%20v3-blue.svg
             :target: https://www.gnu.org/licenses/gpl-3.0
         .. image:: https://zenodo.org/badge/21688312.svg
             :target: https://zenodo.org/badge/latestdoi/21688312
@@ -48,15 +48,15 @@
         - visualization routines and 
         - automated report generation
           
         
         Where to get it
         ===============
         
-        The full source code is available on Github at: https://github.com/konstantinstadler/pymrio
+        The full source code is available on Github at: https://github.com/IndEcol/pymrio
         
         Pymrio is registered at PyPI and on the Anaconda Cloud. Install it by:
         
         .. code:: bash
         
             pip install pymrio --upgrade
             
@@ -68,22 +68,22 @@
         
         or update to the latest version by
         
         .. code:: bash
         
             conda update -c conda-forge pymrio
         
-        The source-code of Pymrio available at the GitHub repo: https://github.com/konstantinstadler/pymrio  
+        The source-code of Pymrio available at the GitHub repo: https://github.com/IndEcol/pymrio  
         
         The master branch in that repo is supposed to be ready for use and might be 
         ahead of the official releases. To install directly from the master branch use:
         
         .. code:: bash
         
-            pip install git+https://github.com/konstantinstadler/pymrio@master
+            pip install git+https://github.com/IndEcol/pymrio@master
         
         
         
         Quickstart    
         ==========
         
         A small test mrio is included in the package. 
@@ -161,15 +161,15 @@
         
         Contributing
         =============
         
         Want to contribute? Great!
         Please check `CONTRIBUTING.rst`_ if you want to help to improve Pymrio.
           
-        .. _CONTRIBUTING.rst: https://github.com/konstantinstadler/pymrio/blob/master/CONTRIBUTING.rst
+        .. _CONTRIBUTING.rst: https://github.com/IndEcol/pymrio/blob/master/CONTRIBUTING.rst
            
         Communication, issues, bugs and enhancements
         ============================================
         
         Please use the issue tracker for documenting bugs, proposing enhancements and all other communication related to pymrio.
         
         You can follow me on twitter_ to get the latest news about all my open-source and research projects (and occasionally some random retweets).
@@ -203,16 +203,18 @@
         .. _OECD: https://www.oecd.org/sti/ind/inter-country-input-output-tables.htm
         .. _EORA26: http://www.worldmrio.com/simplified/
         
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pymrio-0.4.8/README.rst` & `pymrio-0.5.0.dev0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 Pymrio: Multi-Regional Input-Output Analysis in Python.
 
 .. image:: https://img.shields.io/pypi/v/pymrio.svg
     :target: https://pypi.python.org/pypi/pymrio/
 .. image:: https://anaconda.org/conda-forge/pymrio/badges/version.svg   
     :target: https://anaconda.org/conda-forge/pymrio
-.. image:: https://github.com/konstantinstadler/pymrio/workflows/build/badge.svg
-    :target: https://github.com/konstantinstadler/pymrio/actions
-.. image:: https://coveralls.io/repos/github/konstantinstadler/pymrio/badge.svg?branch=master
-    :target: https://coveralls.io/github/konstantinstadler/pymrio
+.. image:: https://github.com/IndEcol/pymrio/workflows/build/badge.svg
+    :target: https://github.com/IndEcol/pymrio/actions
+.. image:: https://coveralls.io/repos/github/IndEcol/pymrio/badge.svg?branch=master
+    :target: https://coveralls.io/github/IndEcol/pymrio
 .. image:: https://readthedocs.org/projects/pymrio/badge/?version=latest
     :target: http://pymrio.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 .. image:: https://img.shields.io/badge/License-GPL%20v3-blue.svg
     :target: https://www.gnu.org/licenses/gpl-3.0
 .. image:: https://zenodo.org/badge/21688312.svg
     :target: https://zenodo.org/badge/latestdoi/21688312
@@ -40,15 +40,15 @@
 - visualization routines and 
 - automated report generation
   
 
 Where to get it
 ===============
 
-The full source code is available on Github at: https://github.com/konstantinstadler/pymrio
+The full source code is available on Github at: https://github.com/IndEcol/pymrio
 
 Pymrio is registered at PyPI and on the Anaconda Cloud. Install it by:
 
 .. code:: bash
 
     pip install pymrio --upgrade
     
@@ -60,22 +60,22 @@
 
 or update to the latest version by
 
 .. code:: bash
 
     conda update -c conda-forge pymrio
 
-The source-code of Pymrio available at the GitHub repo: https://github.com/konstantinstadler/pymrio  
+The source-code of Pymrio available at the GitHub repo: https://github.com/IndEcol/pymrio  
 
 The master branch in that repo is supposed to be ready for use and might be 
 ahead of the official releases. To install directly from the master branch use:
 
 .. code:: bash
 
-    pip install git+https://github.com/konstantinstadler/pymrio@master
+    pip install git+https://github.com/IndEcol/pymrio@master
 
 
 
 Quickstart    
 ==========
 
 A small test mrio is included in the package. 
@@ -153,15 +153,15 @@
 
 Contributing
 =============
 
 Want to contribute? Great!
 Please check `CONTRIBUTING.rst`_ if you want to help to improve Pymrio.
   
-.. _CONTRIBUTING.rst: https://github.com/konstantinstadler/pymrio/blob/master/CONTRIBUTING.rst
+.. _CONTRIBUTING.rst: https://github.com/IndEcol/pymrio/blob/master/CONTRIBUTING.rst
    
 Communication, issues, bugs and enhancements
 ============================================
 
 Please use the issue tracker for documenting bugs, proposing enhancements and all other communication related to pymrio.
 
 You can follow me on twitter_ to get the latest news about all my open-source and research projects (and occasionally some random retweets).
```

### Comparing `pymrio-0.4.8/pymrio/__init__.py` & `pymrio-0.5.0.dev0/pymrio/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 from pymrio.core.mriosystem import Extension, IOSystem, concate_extension
 from pymrio.tools.ioclass import ClassificationData, get_classification
 from pymrio.tools.iodownloader import (
     download_eora26,
     download_exiobase1,
     download_exiobase2,
     download_exiobase3,
+    download_gloria,
     download_oecd,
     download_wiod2013,
 )
 from pymrio.tools.iomath import (
     calc_A,
     calc_accounts,
     calc_e,
```

### Comparing `pymrio-0.4.8/pymrio/core/fileio.py` & `pymrio-0.5.0.dev0/pymrio/core/fileio.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,27 +11,45 @@
 import re
 import sys
 import zipfile
 from pathlib import Path
 
 import pandas as pd
 
-from pymrio.core.constants import DEFAULT_FILE_NAMES, GENERIC_NAMES, PYMRIO_PATH
+from pymrio.core.constants import (
+    DEFAULT_FILE_NAMES,
+    GENERIC_NAMES,
+    PYMRIO_PATH,
+    STORAGE_FORMAT,
+)
 from pymrio.core.mriosystem import Extension, IOSystem
 from pymrio.tools.iometadata import MRIOMetaData
 from pymrio.tools.ioutil import get_file_para
 
 
 # Exceptions
 class ReadError(Exception):
     """Base class for errors occuring while reading MRIO data"""
 
     pass
 
 
+def _get_file_format(file_name):
+    """Helper function to get the format of a stored file"""
+    # TODO: move to pathlib
+    given_extension = Path(file_name).suffix.lstrip(".")
+    for format_key, format_extension in STORAGE_FORMAT.items():
+        if given_extension.lower() in format_extension:
+            table_format = format_key
+            break
+    else:
+        raise ValueError("Unkown format of stored files")
+    return format_key
+
+
 def load_all(path, include_core=True, subfolders=None, path_in_arc=None):
     """Loads a full IO system with all extension in path
 
     Parameters
     ----------
     path : pathlib.Path or string
         Path or path with para file name for the data to load.
@@ -199,17 +217,17 @@
 
 def load(path, include_core=True, path_in_arc=""):
     """Loads a IOSystem or Extension previously saved with pymrio
 
     This function can be used to load a IOSystem or Extension specified in a
     metadata file (as defined in DEFAULT_FILE_NAMES['filepara']: metadata.json)
 
-    DataFrames (tables) are loaded from text or binary pickle files.
-    For the latter, the extension .pkl or .pickle is assumed, in all other case
-    the tables are assumed to be in .txt format.
+    The format of DataFrames (tables) are determined by the file extension.
+    Avaialble formats are defined in constant.py - STORAGE_FORMAT.
+    If using the save/save_all functionality from the mriosystem it just works.
 
     Parameters
     ----------
     path : pathlib.Path or string
         Path or path with para file name for the data to load. This must
         either point to the directory containing the uncompressed data or
         the location of a compressed zip file with the data. In the
@@ -294,47 +312,54 @@
                 full_file_name = file_para.folder + "/" + file_name
                 full_file_name = full_file_name.replace("//", "/")
             else:
                 full_file_name = file_name
             logging.info("Load data from {}".format(full_file_name))
 
             with zipfile.ZipFile(file=str(path)) as zf:
-                if (
-                    os.path.splitext(str(full_file_name))[1] == ".pkl"
-                    or os.path.splitext(str(full_file_name))[1] == ".pickle"
-                ):
-                    setattr(ret_system, key, pd.read_pickle(zf.open(full_file_name)))
-                else:
+                file_format = _get_file_format(full_file_name)
+                if file_format == "txt":
                     setattr(
                         ret_system,
                         key,
                         pd.read_csv(
                             zf.open(full_file_name),
                             index_col=_index_col,
                             header=_header,
                             sep="\t",
                         ),
                     )
+                elif file_format == "pickle":
+                    setattr(ret_system, key, pd.read_pickle(zf.open(full_file_name)))
+                elif file_format == "parquet":
+                    setattr(ret_system, key, pd.read_parquet(zf.open(full_file_name)))
+                else:
+                    ValueError("Unknown file format")
+
         else:
             full_file_name = path / file_name
             logging.info("Load data from {}".format(full_file_name))
-
-            if (
-                os.path.splitext(str(full_file_name))[1] == ".pkl"
-                or os.path.splitext(str(full_file_name))[1] == ".pickle"
-            ):
-                setattr(ret_system, key, pd.read_pickle(full_file_name))
-            else:
+            file_format = _get_file_format(full_file_name)
+            if file_format == "txt":
                 setattr(
                     ret_system,
                     key,
                     pd.read_csv(
-                        full_file_name, index_col=_index_col, header=_header, sep="\t"
+                        full_file_name,
+                        index_col=_index_col,
+                        header=_header,
+                        sep="\t",
                     ),
                 )
+            elif file_format == "pickle":
+                setattr(ret_system, key, pd.read_pickle(full_file_name))
+            elif file_format == "parquet":
+                setattr(ret_system, key, pd.read_parquet(full_file_name))
+            else:
+                ValueError("Unknown file format")
     return ret_system
 
 
 def archive(
     source,
     archive,
     path_in_arc=None,
```

### Comparing `pymrio-0.4.8/pymrio/core/mriosystem.py` & `pymrio-0.5.0.dev0/pymrio/core/mriosystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,20 @@
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
 import pymrio.tools.ioutil as ioutil
-from pymrio.core.constants import DEFAULT_FILE_NAMES, GENERIC_NAMES, MISSING_AGG_ENTRY
+from pymrio.core.constants import (
+    DEFAULT_FILE_NAMES,
+    GENERIC_NAMES,
+    MISSING_AGG_ENTRY,
+    STORAGE_FORMAT,
+)
 from pymrio.tools.iomath import (
     calc_A,
     calc_accounts,
     calc_F,
     calc_F_Y,
     calc_gross_trade,
     calc_L,
@@ -512,70 +517,62 @@
                 continue
             if type(self.__dict__[key]) is pd.DataFrame:
                 if data:
                     yield getattr(self, key)
                 else:
                     yield key
 
-    def save(
-        self, path, table_format="txt", sep="\t", table_ext=None, float_format="%.12g"
-    ):
+    def save(self, path, table_format="txt", sep="\t", float_format="%.12g"):
         """Saving the system to path
 
 
         Parameters
         ----------
         path : pathlib.Path or string
             path for the saved data (will be created if necessary, data
             within will be overwritten).
 
         table_format : string
             Format to save the DataFrames:
 
                 - 'pkl' : Binary pickle files,
-                          alias: 'pickle', 'bin', 'binary'
-                - 'txt' : Text files (default), alias: 'text', 'csv'
+                          alias: 'pickle'
+                - 'parquet': Parquet format
+                          alias: 'par'
+                - 'txt' : Text files (default), alias: 'text', 'csv', 'tsv'
 
-        table_ext : string, optional
-            File extension,
-            default depends on table_format(.pkl for pickle, .txt for text)
 
         sep : string, optional
             Field delimiter for the output file, only for txt files.
             Default: tab ('\t')
 
         float_format : string, optional
-            Format for saving the DataFrames,
-            default = '%.12g', only for txt files
+            Format for saving the DataFrames, only for txt files.
+            default = '%.12g'
         """
 
-        path = Path(path)
+        for format_key, format_extension in STORAGE_FORMAT.items():
+            if table_format.lower() in format_extension:
+                table_extension = table_format
+                table_format = format_key
+                break
+        else:
+            raise ValueError(
+                'Unknown table format "{}" - '
+                'must be "txt", "pkl", "parquet" or an alias as '
+                "defined in STORAGE_FORMAT".format(table_format)
+            )
 
+        path = Path(path)
         path.mkdir(parents=True, exist_ok=True)
 
         para_file_path = path / DEFAULT_FILE_NAMES["filepara"]
         file_para = dict()
         file_para["files"] = dict()
 
-        if table_format in ["text", "csv", "txt"]:
-            table_format = "txt"
-        elif table_format in ["pickle", "bin", "binary", "pkl"]:
-            table_format = "pkl"
-        else:
-            raise ValueError(
-                'Unknown table format "{}" - '
-                'must be "txt" or "pkl"'.format(table_format)
-            )
-
-        if not table_ext:
-            if table_format == "txt":
-                table_ext = ".txt"
-            if table_format == "pkl":
-                table_ext = ".pkl"
-
         if str(type(self)) == "<class 'pymrio.core.mriosystem.IOSystem'>":
             file_para["systemtype"] = GENERIC_NAMES["iosys"]
         elif str(type(self)) == "<class 'pymrio.core.mriosystem.Extension'>":
             file_para["systemtype"] = GENERIC_NAMES["ext"]
             file_para["name"] = self.name
         else:
             logging.warn(
@@ -590,21 +587,25 @@
                 nr_index_col = 1
 
             if type(df.columns) is pd.MultiIndex:
                 nr_header = len(df.columns.levels)
             else:
                 nr_header = 1
 
-            save_file = df_name + table_ext
+            save_file = df_name + "." + table_extension
             save_file_with_path = path / save_file
             logging.info("Save file {}".format(save_file_with_path))
             if table_format == "txt":
                 df.to_csv(save_file_with_path, sep=sep, float_format=float_format)
-            else:
+            elif table_format == "pickle":
                 df.to_pickle(save_file_with_path)
+            elif table_format == "parquet":
+                df.to_parquet(save_file_with_path)
+            else:
+                raise ValueError("Unknow table format passed through")
 
             file_para["files"][df_name] = dict()
             file_para["files"][df_name]["name"] = save_file
             file_para["files"][df_name]["nr_index_col"] = str(nr_index_col)
             file_para["files"][df_name]["nr_header"] = str(nr_header)
 
         with para_file_path.open(mode="w") as pf:
@@ -988,15 +989,14 @@
             except (AssertionError, KeyError):
                 self.D_exp_reg = self.D_exp.groupby(level=0, axis=1, sort=False).sum()
 
             logging.debug("{} - Accounts D for regions calculated".format(self.name))
 
         # calc accounts per capita if population data is available
         if population is not None:
-
             if (
                 (self.D_cba_cap is None)
                 or (self.D_pba_cap is None)
                 or (self.D_imp_cap is None)
                 or (self.D_exp_cap is None)
             ):
                 self.D_cba_cap = (
@@ -2061,17 +2061,15 @@
 
         """
         self.reset_to_coefficients()
         [ee.reset_to_coefficients() for ee in self.get_extensions(data=True)]
         self.meta._add_modify("Reset full system to coefficients")
         return self
 
-    def save_all(
-        self, path, table_format="txt", sep="\t", table_ext=None, float_format="%.12g"
-    ):
+    def save_all(self, path, table_format="txt", sep="\t", float_format="%.12g"):
         """Saves the system and all extensions
 
         Extensions are saved in separate folders (names based on extension)
 
         Parameters are passed to the .save methods of the IOSystem and
         Extensions. See parameters description there.
         """
@@ -2080,26 +2078,24 @@
 
         path.mkdir(parents=True, exist_ok=True)
 
         self.save(
             path=path,
             table_format=table_format,
             sep=sep,
-            table_ext=table_ext,
             float_format=float_format,
         )
 
         for ext, ext_name in zip(self.get_extensions(data=True), self.get_extensions()):
             ext_path = path / ext_name
 
             ext.save(
                 path=ext_path,
                 table_format=table_format,
                 sep=sep,
-                table_ext=table_ext,
                 float_format=float_format,
             )
         return self
 
     def aggregate_duplicates(self, inplace=True):
         """Aggregate duplicated regions and sectors
 
@@ -2421,15 +2417,14 @@
             self.meta._add_modify("Aggregate extensions...")
             extension.reset_to_flows()
             st_redo_unit = False
             for ik_name, ik_df in zip(
                 extension.get_DataFrame(data=False, with_unit=False),
                 extension.get_DataFrame(data=True, with_unit=False),
             ):
-
                 # Without unit - this is reset aftwards if necessary
                 if ik_df.index.names == ["region", "sector"] == ik_df.columns.names:
                     # Full disaggregated extensions - aggregate both axis
                     # (this is the case if the extions shows the flows from
                     # pda to cba)
                     extension.__dict__[ik_name] = pd.DataFrame(
                         data=conc.dot(ik_df).dot(conc.T)
@@ -2439,15 +2434,14 @@
                     extension.__dict__[ik_name].columns = mi_reg_sec
                     extension.__dict__[ik_name].index = mi_reg_sec
                     st_redo_unit = True
                 elif ik_df.index.names == [
                     "region",
                     "sector",
                 ] and ik_df.columns.names == ["region", "category"]:
-
                     # Full disaggregated finald demand satellite account.
                     # Thats not implemented yet - but aggregation is in place
                     extension.__dict__[ik_name] = pd.DataFrame(
                         data=conc.dot(ik_df).dot(conc_y.T)
                     )
                     # next step must be done afterwards due to unknown reasons
                     extension.__dict__[ik_name].columns = mi_reg_Ycat
```

### Comparing `pymrio-0.4.8/pymrio/mrio_models/exio2_ixi/misc/population.txt` & `pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_ixi/misc/population.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.4.8/pymrio/mrio_models/exio2_pxp/misc/population.txt` & `pymrio-0.5.0.dev0/pymrio/mrio_models/exio2_pxp/misc/population.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.4.8/pymrio/mrio_models/test_mrio/mrio_data/FDemissions.txt` & `pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/FDemissions.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.4.8/pymrio/mrio_models/test_mrio/mrio_data/emissions.txt` & `pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/emissions.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.4.8/pymrio/mrio_models/test_mrio/mrio_data/factor_input.txt` & `pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/factor_input.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.4.8/pymrio/mrio_models/test_mrio/mrio_data/finald_demand_Y.txt` & `pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/finald_demand_Y.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.4.8/pymrio/mrio_models/test_mrio/mrio_data/trade_flows_Z.txt` & `pymrio-0.5.0.dev0/pymrio/mrio_models/test_mrio/mrio_data/trade_flows_Z.txt`

 * *Files identical despite different names*

### Comparing `pymrio-0.4.8/pymrio/tools/ioclass.py` & `pymrio-0.5.0.dev0/pymrio/tools/ioclass.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.4.8/pymrio/tools/iodownloader.py` & `pymrio-0.5.0.dev0/pymrio/tools/iodownloader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 """ Utility functions for automatic downloading of public MRIO databases
 """
 
+import getpass
 import itertools
+import json
 import os
 import re
+import ssl
 import zipfile
 from collections import namedtuple
 
 import requests
+import urllib3
 
+from pymrio.core.constants import __ROOT, GLORIA_URLS
 from pymrio.tools.iometadata import MRIOMetaData
+from pymrio.tools.ioutil import filename_from_url, ssl_fix
 
 WIOD_CONFIG = {
     "url_db_view": "http://www.wiod.org/database/wiots13",
     "url_db_content": "http://www.wiod.org/",
     "mrio_regex": r"protected.*?wiot\d\d.*?xlsx",
     "satellite_urls": [
         "http://www.wiod.org/protected3/data13/SEA/WIOD_SEA_July14.xlsx",
@@ -85,14 +91,16 @@
             "2005-2009": "https://stats.oecd.org/wbos/fileview2.aspx?IDFile=fe218690-0a3b-44aa-a82c-b3e3da6d24db",
             "2010-2014": "https://stats.oecd.org/wbos/fileview2.aspx?IDFile=2c2f499f-5703-4034-9457-2f7518e8f2fc",
             "2015-2018": "https://stats.oecd.org/wbos/fileview2.aspx?IDFile=59a3d7f2-3f23-40d5-95ca-48da84c0f861",
         },
     },
 }
 
+GLORIA_CONFIG = {"datafiles": GLORIA_URLS}
+
 
 def _get_url_datafiles(
     url_db_view,
     url_db_content,
     mrio_regex,
     access_cookie=None,
     requests_func=requests.post,
@@ -131,15 +139,15 @@
     returnvalue = namedtuple("url_content", ["raw_text", "data_urls"])
     url_text = requests_func(url_db_view, cookies=access_cookie).text
     data_urls = [url_db_content + ff for ff in re.findall(mrio_regex, url_text)]
     return returnvalue(raw_text=url_text, data_urls=data_urls)
 
 
 def _download_urls(
-    url_list, storage_folder, overwrite_existing, meta_handler, access_cookie=None
+    url_list, storage_folder, overwrite_existing, downlog_handler, access_cookie=None
 ):
     """Save url from url_list to storage_folder
 
     Parameters
     ----------
     url_list: list of str
         Valid url to download
@@ -150,44 +158,47 @@
         the download depends on the setting in 'overwrite_existing'.
 
     overwrite_existing: boolean, optional
         If False, skip download of file already existing in
         the storage folder (default). Set to True to replace
         files.
 
-    meta_handler: instance of MRIOMetaData
+    downlog_handler: instance of MRIOMetaData
+        Instance of MRIOMetaData to store the download log
 
     access_cookie: cookie, optional
         Cookie to be passed to the requests.post function fetching the data
 
 
     Returns
     -------
 
-    The meta_handler is passed back
+    The downlog_handler is passed back
 
     """
     for url in url_list:
-        filename = os.path.basename(url)
+        filename = filename_from_url(url)
+        if downlog_handler.name == "Eora":
+            filename = filename.split(".zip")[0] + ".zip"
         if not overwrite_existing and filename in os.listdir(storage_folder):
             continue
         storage_file = os.path.join(storage_folder, filename)
 
         # Using requests here - tried with aiohttp but was actually slower
         # Also don’t use shutil.copyfileobj - corrupts zips from Eora
         # req = requests.post(url, stream=True, cookies=access_cookie)
         req = requests.get(url, stream=True, cookies=access_cookie)
         with open(storage_file, "wb") as lf:
             for chunk in req.iter_content(1024 * 5):
                 lf.write(chunk)
 
-        meta_handler._add_fileio("Downloaded {} to {}".format(url, filename))
-        meta_handler.save()
+        downlog_handler._add_fileio("Downloaded {} to {}".format(url, filename))
+        downlog_handler.save()
 
-    return meta_handler
+    return downlog_handler
 
 
 def download_oecd(
     storage_folder, version="v2021", years=None, overwrite_existing=False
 ):
     """Downloads the OECD ICIO tables
 
@@ -237,73 +248,72 @@
     elif "21" in version:
         version = "v2021"
     else:
         raise ValueError("Version not understood")
 
     if type(years) is int or type(years) is str:
         years = [years]
+
     if not years:
         if version == "v2018":
             years = range(2005, 2016)
         elif version == "v2021":
             years = ["1995-1999", "2000-2004", "2005-2009", "2010-2014", "2015-2018"]
 
         else:
             years = range(1995, 2012)
+
     years = [str(yy) for yy in years]
 
-    meta = MRIOMetaData(
+    downlog = MRIOMetaData._make_download_log(
         location=storage_folder,
         description="OECD-ICIO download",
         name="OECD-ICIO",
         system="IxI",
         version=version,
     )
 
-    oecd_webcontent = requests.get(OECD_CONFIG["url_db_view"]).text
     for yy in years:
         if yy not in OECD_CONFIG["datafiles"][version].keys():
             raise ValueError("Datafile for {} not specified or available.".format(yy))
-        if version == "v2016":
-            url_to_check = os.path.basename(OECD_CONFIG["datafiles"][version][yy])
-        elif version == "v2021":
-            url_to_check = os.path.basename(OECD_CONFIG["datafiles"][version][yy])
-        else:
-            url_to_check = OECD_CONFIG["datafiles"][version][yy]
-
-        if url_to_check not in oecd_webcontent:
-            raise ValueError(
-                "Specified datafile for {} () not found in the current"
-                "OECD ICIO webpage.\n"
-                "Perhaps filenames have been changed - update OECD_CONFIG "
-                "to the new filenames".format(yy, url_to_check)
-            )
 
         filename = "ICIO" + version.lstrip("v") + "_" + yy + ".zip"
+
+        if not overwrite_existing:
+            if version == "v2021":
+                filenames = [
+                    f"ICIO{version.lstrip('v')}_{str(yr)}.csv"
+                    for yr in range(int(yy[:4]), int(yy[-4:]) + 1)
+                ]
+                if set(filenames).issubset(os.listdir(storage_folder)):
+                    continue
+            elif filename in os.listdir(storage_folder):
+                continue
+
+        req = ssl_fix(OECD_CONFIG["datafiles"][version][yy], stream=True)
         storage_file = os.path.join(storage_folder, filename)
 
-        req = requests.get(OECD_CONFIG["datafiles"][version][yy], stream=True)
         with open(storage_file, "wb") as lf:
             for chunk in req.iter_content(1024 * 5):
                 lf.write(chunk)
 
         if version == "v2021":
             with zipfile.ZipFile(storage_file, "r") as zip_ref:
                 zip_ref.extractall(storage_folder)
             os.remove(storage_file)
 
-        meta._add_fileio(
+        downlog._add_fileio(
             "Downloaded {} to {}".format(
                 OECD_CONFIG["datafiles"][version][yy], filename
             )
         )
 
-    meta.save()
+    downlog.save()
 
-    return meta
+    return downlog
 
 
 def download_wiod2013(
     storage_folder,
     years=None,
     overwrite_existing=False,
     satellite_urls=WIOD_CONFIG["satellite_urls"],
@@ -363,49 +373,134 @@
 
     restricted_wiod_io_urls = [
         url
         for url in wiod_web_content.data_urls
         if re.search(r"(wiot)(\d\d)", os.path.basename(url)).group(2) in years
     ]
 
-    meta = MRIOMetaData(
+    downlog = MRIOMetaData._make_download_log(
         location=storage_folder,
         description="WIOD metadata file for pymrio",
         name="WIOD",
         system="IxI",
         version="data13",
     )
 
-    meta = _download_urls(
+    downlog = _download_urls(
         url_list=restricted_wiod_io_urls + satellite_urls,
         storage_folder=storage_folder,
         overwrite_existing=overwrite_existing,
-        meta_handler=meta,
+        downlog_handler=downlog,
     )
 
-    meta.save()
-    return meta
+    downlog.save()
+    return downlog
 
 
-def download_eora26():
-    """Downloading eora26 not implemented (registration required)"""
-    raise NotImplementedError(
-        "Eora26 3 requires registration prior to download. "
-        "Please register at http://www.worldmrio.com and download the "
-        "Eora26 files from the subdomain /simplified"
+def download_eora26(
+    storage_folder, email, password, years=None, prices=["bp"], overwrite_existing=False
+):
+    """Downloading eora26 mrios (registration required),
+    To use this function you have to have an Eora account,
+    New account registration can be done through https://worldmrio.com/login.jsp
+
+    Parameters
+    ----------
+    storage_folder: str, valid path
+        Location to store the download, folder will be created if
+        not existing. If the file is already present in the folder,
+        the download of the specific file will be skipped.
+    email: str,
+        Eora account email
+    password: str,
+        Eora account password
+    years: list of int or str, optional
+        If years is given only downloads the specific years. This
+        only applies to the IO tables because extensions are stored
+        by country and not per year.
+        The years can be given in 2 or 4 digits.
+    prices: list of str
+        If bp (default), download basic price tables.
+        If pp, download purchaser prices. ['bp', 'pp'] possible.
+    overwrite_existing: boolean, optional
+        If False, skip download of file already existing in
+        the storage folder (default). Set to True to replace
+        files.
+    """
+
+    try:
+        os.makedirs(storage_folder)
+    except FileExistsError:
+        pass
+
+    false_cred = True
+
+    while false_cred:
+        r = requests.post(
+            "https://worldmrio.com/Register2?submit=login",
+            data={
+                "email": email,
+                "pass": password,
+                "targetURL": "null",
+                "submit": "login",
+            },
+        )
+
+        if "no account found" in r.text:
+            print(
+                """Eora account with this email was not found\n
+            Please try again or register a new user at the following website:\n
+            https://worldmrio.com/login.jsp"""
+            )
+
+            email = input("Enter your Eora account email: ")
+            password = getpass.getpass(prompt="Enter your Eora account password: ")
+
+        elif "Sorry, wrong password provided" in r.text:
+            print(
+                """The password for this email account is incorrect\n
+            Please try again"""
+            )
+
+            password = getpass.getpass(prompt="Enter your Eora account password: ")
+
+        else:
+            false_cred = False
+
+    if type(years) is int or type(years) is str:
+        years = [years]
+    years = years if years else range(1995, 2012)
+    years = [str(yy).zfill(4) for yy in years]
+
+    if type(prices) is str:
+        prices = [prices]
+
+    restricted_eora_urls = [
+        f"https://worldmrio.com/ComputationsM/Phase199/Loop082/simplified/Eora26_{yr}_bp.zip?email={email}&pass={password}"
+        for yr in years
+    ]
+
+    downlog = MRIOMetaData._make_download_log(
+        location=storage_folder,
+        description="Download log for Eora",
+        name="Eora",
+        system="ixi",
+        version="v199.82",
     )
-    return None
 
-    # Development note:
-    # Eora 26 autodownload was implemented before but was
-    # removed since worldmrio does require
-    # a registration now (by summer 2018).
-    # The previous implementation can be found
-    # in the github history (e.g. at 2e61424 2018-10-09
-    # or before)
+    downlog = _download_urls(
+        url_list=restricted_eora_urls,
+        storage_folder=storage_folder,
+        overwrite_existing=overwrite_existing,
+        downlog_handler=downlog,
+    )
+
+    downlog.save()
+
+    return downlog
 
 
 def download_exiobase1():
     """Downloading exiobase not implemented (registration required)"""
     raise NotImplementedError(
         "EXIOBASE 1 requires registration prior to download. "
         "Please register at www.exiobase.eu and download the "
@@ -427,17 +522,14 @@
         "and/or_"
         ">MrIOT_PxP_ita_coefficient_version2.2.2.zip<_"
         "manually (tab Data Download - EXIOBASE 2)."
     )
     return None
 
 
-# def download_exiobase3():
-
-
 def download_exiobase3(
     storage_folder,
     years=None,
     system=None,
     overwrite_existing=False,
     doi="10.5281/zenodo.3583070",
 ):
@@ -505,17 +597,17 @@
         years = [years]
     years = years if years else list(available_years)
 
     system = system if system else ["pxp", "ixi"]
     if type(system) is str:
         system = [system]
 
-    meta = MRIOMetaData(
+    downlog = MRIOMetaData._make_download_log(
         location=storage_folder,
-        description="EXIOBASE3 metadata file for pymrio",
+        description="Download log of EXIOBASE3",
         name="EXIO3",
         system=",".join(system),
         version=doi,
     )
 
     requested_urls = []
     for file_specs in itertools.product(years, system):
@@ -523,26 +615,105 @@
             filter(
                 lambda x: str(file_specs[0]) in x and str(file_specs[1]) in x,
                 available_files,
             )
         )
 
         if not filename:
-            meta._add_fileio(
+            downlog._add_fileio(
                 "Could not find EXIOBASE 3 source file with >{}< and >{}<".format(
                     file_specs[0], file_specs[1]
                 )
             )
             continue
         requested_urls += [
             u for u in exio_web_content.data_urls for f in filename if f in u
         ]
 
-    meta = _download_urls(
+    downlog = _download_urls(
         url_list=requested_urls,
         storage_folder=storage_folder,
         overwrite_existing=overwrite_existing,
-        meta_handler=meta,
+        downlog_handler=downlog,
+    )
+
+    downlog.save()
+    return downlog
+
+
+def download_gloria(
+    storage_folder,
+    urls=GLORIA_CONFIG["datafiles"],
+    year=None,
+    version=57,
+    overwrite_existing=False,
+):
+    """
+    Download Gloria databases files
+
+    Parameters
+    ----------
+
+    urls: dict, optional
+        Dictionary containing the links of gloria databases
+        for different versions, this is already fed to the function,
+        imported from urls.json file
+
+    storage_folder: str, option
+        The path where to download the file(s), if not specified
+        it/they will be downloaded to the current working directory
+
+    year: int, str or list, optional
+        The year(s) of the wanted database, if not specified
+        the databases of all available years will be downloaded
+
+    version: int or str, option
+        The wanted version of Gloria database, if not specified
+        the database of the latest version will be downloaded
+
+    overwrite_existing: boolean, optional
+        If False, skip download of file already existing in
+        the storage folder (default). Set to True to replace
+        files.
+
+    Returns
+    -------
+
+    No returns
+    """
+
+    if f"0{int(version)}" not in urls.keys():
+        raise Exception("Specified version is invalid")
+
+    downlog = MRIOMetaData._make_download_log(
+        location=storage_folder,
+        description="Download log of Gloria",
+        name="GLORIA",
+        system="IxI",
+        version=version,
+    )
+
+    files_to_download = []
+    if type(year) is int or type(year) is str:
+        year = [year]
+
+    if year:
+        for yr in year:
+            files_to_download.extend(
+                [
+                    file
+                    for file in urls[f"0{int(version)}"]
+                    if str(yr) in filename_from_url(file)
+                ]
+            )
+    else:
+        files_to_download = urls[f"0{int(version)}"]
+
+    downlog = _download_urls(
+        url_list=files_to_download,
+        storage_folder=storage_folder,
+        overwrite_existing=overwrite_existing,
+        downlog_handler=downlog,
     )
 
-    meta.save()
-    return meta
+    downlog.save()
+    return downlog
```

### Comparing `pymrio-0.4.8/pymrio/tools/iomath.py` & `pymrio-0.5.0.dev0/pymrio/tools/iomath.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.4.8/pymrio/tools/iometadata.py` & `pymrio-0.5.0.dev0/pymrio/tools/iometadata.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 """ Meta data for provenance and version tracking in pymrio
 """
 
 import datetime
+import getpass
 import json
 import logging
 import os
+import platform
 import zipfile
 from collections import OrderedDict
 from pathlib import Path
 
 from pymrio.core.constants import DEFAULT_FILE_NAMES
+from pymrio.version import __version__ as pymrio_version
 
 
 class MRIOMetaData(object):
     def __init__(
         self,
         location=None,
         description=None,
         name=None,
         system=None,
         version=None,
         path_in_arc="",
         logger_function=logging.info,
     ):
-
         """Organzises the MRIO meta data
 
         The meta data is stored in a json file.
 
         Note
         -----
             The parameters 'description', 'name', 'system', and
@@ -167,14 +169,116 @@
                 system=self.system,
                 ver=self.version,
                 metafile=self._metadata_file,
                 hist=hist,
             )
         )
 
+    def _make_download_log(
+        location,
+        name,
+        description=None,
+        system=None,
+        version=None,
+        logger_function=logging.info,
+    ):
+        """Factory method for making a download log file
+
+        This makes an instance of the metahander suitable for storing download information.
+        During estabishment it also records system information (username, hostname, pymrio version, etc.)
+        as defined in _get_system_meta.
+
+        Parameters
+        -----------
+
+        location: str, valid path
+            Path or filename for the history log file.
+            This can be the full file path or just the
+            storage folder.  In the latter case, the filename defined in
+            DEFAULT_FILE_NAMES['download_log'] (currently 'download_log.json') is
+            assumed.
+
+        name: str
+            Name of the mrio (e.g. wiod, exiobase)
+            Will be set the first time the metadata file gets established;
+            subsequent changes are recorded in 'history'.
+
+        description: str, optional
+            Description of the metadata file purpose and mrio,
+            default set to 'Metadata file for pymrio'.
+            Will be set the first time the metadata file gets established;
+            subsequent changes are recorded in 'history'.
+
+        system: str, optional
+            For example 'industry by industry', 'ixi', ...
+            Will be set the first time the metadata file gets established;
+            subsequent changes are recorded in 'history'.
+
+        version: str, int, float, optional
+            Version number
+            Will be set the first time the metadata file gets established;
+            subsequent changes are recorded in 'history'.
+
+        logger_function: func, optional
+            Function accepting strings.
+            The info string written to the metadata is also
+            passed to this function. By default, the funtion
+            is set to logging.info. Set to None for no output.
+
+        Returns
+        --------
+        MRIOMetaData object
+            setup as a download log
+
+        """
+
+        location = Path(location)
+
+        if location.exists():
+            if location.is_file():
+                full_location = location
+            elif location.is_dir():
+                full_location = location / DEFAULT_FILE_NAMES["download_log"]
+            else:
+                raise ValueError("Location must be a valid file or directory")
+        else:
+            if location.suffix == "":
+                full_location = location / DEFAULT_FILE_NAMES["download_log"]
+            else:
+                full_location = location
+
+        mmd = MRIOMetaData(
+            location=full_location,
+            description=description,
+            name=name,
+            system=system,
+            version=version,
+            logger_function=logger_function,
+        )
+
+        for typ, val in mmd._get_system_meta().items():
+            mmd.note(f"{typ}: {val}")
+
+        mmd.note("Download log created")
+
+        return mmd
+
+    def _read_content(self):
+        """Read the metadata file and store the content in self._content"""
+        if self._metadata_file:
+            if self._path_in_arc:
+                with zipfile.ZipFile(file=str(self._metadata_file)) as zf:
+                    with zf.open(self._path_in_arc) as f:
+                        self._content = json.load(f, object_pairs_hook=OrderedDict)
+            else:
+                with open(str(self._metadata_file), "r") as f:
+                    self._content = json.load(f, object_pairs_hook=OrderedDict)
+
+        return mmd
+
     def note(self, entry):
         """Add the passed string as note to the history
 
         If log is True (default), also log the string by logging.info
         """
         self._add_history(entry_type="NOTE", entry=entry)
 
@@ -271,14 +375,48 @@
                 entry_type="METADATA_CHANGE",
                 entry='Changed parameter "{para}" '
                 'from "{old}" to "{new}"'.format(
                     para=para, old=old_value, new=new_value
                 ),
             )
 
+    def _get_system_meta(self):
+        """Returns a dictionary with user meta data
+
+        with username, computername, os, os version, and python version
+        """
+
+        try:
+            username = getpass.getuser()
+        except:
+            username = "unknown"
+
+        try:
+            hostname = platform.node()
+        except:
+            hostname = "unknown"
+
+        try:
+            os = platform.system()
+        except:
+            os = "unknown"
+
+        try:
+            pyver = platform.python_version()
+        except:
+            pyver = "unknown"
+
+        return {
+            "username": username,
+            "hostname": hostname,
+            "os": os,
+            "pymrio_version": pymrio_version,
+            "python_version": pyver,
+        }
+
     def _time(self):
         return "{:%Y%m%d %H:%M:%S}".format(datetime.datetime.now())
 
     def _read_content(self):
         """Reads metadata from location (and path_in_arc if archive)
 
         This function is called during the init process and
```

### Comparing `pymrio-0.4.8/pymrio/tools/ioparser.py` & `pymrio-0.5.0.dev0/pymrio/tools/ioparser.py`

 * *Files identical despite different names*

### Comparing `pymrio-0.4.8/pymrio/tools/ioutil.py` & `pymrio-0.5.0.dev0/pymrio/tools/ioutil.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 Utility function for pymrio
 
 KST 20140502
 """
 import json
 import logging
 import os
+import re
+import ssl
 import zipfile
 from collections import namedtuple
 from pathlib import Path
 from typing import Union
 
 import numpy as np
 import pandas as pd
+import requests
+import urllib3
 
 from pymrio.core.constants import DEFAULT_FILE_NAMES, PYMRIO_PATH
 
 
 def is_vector(inp):
     """Returns true if the input can be interpreted as a 'true' vector
 
@@ -632,7 +636,72 @@
         nr_index_col = find_first_number(lines_with_sep[-1].split(sep))
         if nr_index_col:
             for nr_header_row, line in enumerate(lines_with_sep):
                 if find_first_number(line.split(sep)) == nr_index_col:
                     break
 
     return dict(sep=sep, nr_header_row=nr_header_row, nr_index_col=nr_index_col)
+
+
+def filename_from_url(url):
+    """
+    Extract a file name from the download link for that file
+
+    Parameters
+    ----------
+
+    url: str,
+        The download link of the file
+
+    Returns
+    -------
+    str,
+        The extracted file name
+
+    """
+    name = re.search("[^/\\&\?]+\.\w{2,7}(?=([\?&].*$|$))", url)
+    return name.group()
+
+
+def ssl_fix(*args, **kwargs):
+    """
+    Tries to use a request connection with Lagacy option
+    when normal connection fails
+
+    Parameters
+    ----------
+    Parameters of a normal requests.get() function
+        url: URL for the new :class:`Request` object.
+        params: (optional) Dictionary, list of tuples or bytes to send
+        in the query string for the class `Request`.
+        **kwargs: Optional arguments that `request` takes.
+
+    Returns
+    -------
+        r: class:`Response <Response>` object
+    """
+
+    class CustomHttpAdapter(requests.adapters.HTTPAdapter):
+        # "Transport adapter" that allows us to use custom ssl_context.
+
+        def __init__(self, ssl_context=None, **kwargs):
+            self.ssl_context = ssl_context
+            super().__init__(**kwargs)
+
+        def init_poolmanager(self, connections, maxsize, block=False):
+            self.poolmanager = urllib3.poolmanager.PoolManager(
+                num_pools=connections,
+                maxsize=maxsize,
+                block=block,
+                ssl_context=self.ssl_context,
+            )
+
+    try:
+        r = requests.get(*args, **kwargs)
+    except:
+        ctx = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)
+        ctx.options |= 0x4  # OP_LEGACY_SERVER_CONNECT
+        session = requests.session()
+        session.mount("https://", CustomHttpAdapter(ctx))
+        r = session.get(*args, **kwargs)
+
+    return r
```

### Comparing `pymrio-0.4.8/pymrio.egg-info/PKG-INFO` & `pymrio-0.5.0.dev0/pymrio.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 1.2
 Name: pymrio
-Version: 0.4.8
+Version: 0.5.0.dev0
 Summary: A python module for automating input output calculations and generating reports
-Home-page: https://github.com/konstantinstadler/pymrio
+Home-page: https://github.com/IndEcol/pymrio
 Author: Konstantin Stadler
 Author-email: konstantin.stadler@ntnu.no
 License: UNKNOWN
 Description: ############
         Pymrio
         ############
         
         Pymrio: Multi-Regional Input-Output Analysis in Python.
         
         .. image:: https://img.shields.io/pypi/v/pymrio.svg
             :target: https://pypi.python.org/pypi/pymrio/
         .. image:: https://anaconda.org/conda-forge/pymrio/badges/version.svg   
             :target: https://anaconda.org/conda-forge/pymrio
-        .. image:: https://github.com/konstantinstadler/pymrio/workflows/build/badge.svg
-            :target: https://github.com/konstantinstadler/pymrio/actions
-        .. image:: https://coveralls.io/repos/github/konstantinstadler/pymrio/badge.svg?branch=master
-            :target: https://coveralls.io/github/konstantinstadler/pymrio
+        .. image:: https://github.com/IndEcol/pymrio/workflows/build/badge.svg
+            :target: https://github.com/IndEcol/pymrio/actions
+        .. image:: https://coveralls.io/repos/github/IndEcol/pymrio/badge.svg?branch=master
+            :target: https://coveralls.io/github/IndEcol/pymrio
         .. image:: https://readthedocs.org/projects/pymrio/badge/?version=latest
             :target: http://pymrio.readthedocs.io/en/latest/?badge=latest
             :alt: Documentation Status
         .. image:: https://img.shields.io/badge/License-GPL%20v3-blue.svg
             :target: https://www.gnu.org/licenses/gpl-3.0
         .. image:: https://zenodo.org/badge/21688312.svg
             :target: https://zenodo.org/badge/latestdoi/21688312
@@ -48,15 +48,15 @@
         - visualization routines and 
         - automated report generation
           
         
         Where to get it
         ===============
         
-        The full source code is available on Github at: https://github.com/konstantinstadler/pymrio
+        The full source code is available on Github at: https://github.com/IndEcol/pymrio
         
         Pymrio is registered at PyPI and on the Anaconda Cloud. Install it by:
         
         .. code:: bash
         
             pip install pymrio --upgrade
             
@@ -68,22 +68,22 @@
         
         or update to the latest version by
         
         .. code:: bash
         
             conda update -c conda-forge pymrio
         
-        The source-code of Pymrio available at the GitHub repo: https://github.com/konstantinstadler/pymrio  
+        The source-code of Pymrio available at the GitHub repo: https://github.com/IndEcol/pymrio  
         
         The master branch in that repo is supposed to be ready for use and might be 
         ahead of the official releases. To install directly from the master branch use:
         
         .. code:: bash
         
-            pip install git+https://github.com/konstantinstadler/pymrio@master
+            pip install git+https://github.com/IndEcol/pymrio@master
         
         
         
         Quickstart    
         ==========
         
         A small test mrio is included in the package. 
@@ -161,15 +161,15 @@
         
         Contributing
         =============
         
         Want to contribute? Great!
         Please check `CONTRIBUTING.rst`_ if you want to help to improve Pymrio.
           
-        .. _CONTRIBUTING.rst: https://github.com/konstantinstadler/pymrio/blob/master/CONTRIBUTING.rst
+        .. _CONTRIBUTING.rst: https://github.com/IndEcol/pymrio/blob/master/CONTRIBUTING.rst
            
         Communication, issues, bugs and enhancements
         ============================================
         
         Please use the issue tracker for documenting bugs, proposing enhancements and all other communication related to pymrio.
         
         You can follow me on twitter_ to get the latest news about all my open-source and research projects (and occasionally some random retweets).
@@ -203,16 +203,18 @@
         .. _OECD: https://www.oecd.org/sti/ind/inter-country-input-output-tables.htm
         .. _EORA26: http://www.worldmrio.com/simplified/
         
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pymrio-0.4.8/pymrio.egg-info/SOURCES.txt` & `pymrio-0.5.0.dev0/pymrio.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -89,19 +89,28 @@
 pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_J_K.txt
 pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_L.txt
 pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_M_N_O.txt
 pymrio/mrio_models/exio2_pxp/concordance/pro_ISIC_P.txt
 pymrio/mrio_models/exio2_pxp/misc/__init__.py
 pymrio/mrio_models/exio2_pxp/misc/population.txt
 pymrio/mrio_models/exio3_ixi/__init__.py
+pymrio/mrio_models/exio3_ixi/finaldemand.tsv
+pymrio/mrio_models/exio3_ixi/sectors.tsv
+pymrio/mrio_models/exio3_ixi/valueadded.tsv
 pymrio/mrio_models/exio3_pxp/__init__.py
+pymrio/mrio_models/exio3_pxp/finaldemand.tsv
+pymrio/mrio_models/exio3_pxp/sectors.tsv
+pymrio/mrio_models/exio3_pxp/valueadded.tsv
 pymrio/mrio_models/test_mrio/__init__.py
+pymrio/mrio_models/test_mrio/finaldemand.tsv
+pymrio/mrio_models/test_mrio/sectors.tsv
 pymrio/mrio_models/test_mrio/concordance/EU.txt
 pymrio/mrio_models/test_mrio/concordance/OECD.txt
 pymrio/mrio_models/test_mrio/concordance/__init__.py
+pymrio/mrio_models/test_mrio/concordance/emissions_charact.tsv
 pymrio/mrio_models/test_mrio/concordance/orig_regions.txt
 pymrio/mrio_models/test_mrio/concordance/orig_sectors.txt
 pymrio/mrio_models/test_mrio/concordance/sector1.txt
 pymrio/mrio_models/test_mrio/concordance/sector2.txt
 pymrio/mrio_models/test_mrio/concordance/sector3.txt
 pymrio/mrio_models/test_mrio/concordance/supreg1.txt
 pymrio/mrio_models/test_mrio/concordance/supreg2.txt
@@ -116,8 +125,15 @@
 pymrio/mrio_models/test_mrio/mrio_data/trade_flows_Z.txt
 pymrio/tools/__init__.py
 pymrio/tools/ioclass.py
 pymrio/tools/iodownloader.py
 pymrio/tools/iomath.py
 pymrio/tools/iometadata.py
 pymrio/tools/ioparser.py
-pymrio/tools/ioutil.py
+pymrio/tools/ioutil.py
+tests/test_aggregation.py
+tests/test_core.py
+tests/test_integration.py
+tests/test_math.py
+tests/test_outputs.py
+tests/test_parsers.py
+tests/test_util.py
```

### Comparing `pymrio-0.4.8/setup.py` & `pymrio-0.5.0.dev0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,39 +5,44 @@
 setup(
     name="pymrio",
     description=(
         "A python module for automating input output "
         "calculations and generating reports"
     ),
     long_description=open("README.rst").read(),
-    url="https://github.com/konstantinstadler/pymrio",
+    url="https://github.com/IndEcol/pymrio",
     author="Konstantin Stadler",
     author_email="konstantin.stadler@ntnu.no",
     version=__version__,  # noqa
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.7.0",
     package_data={
         "": ["*.txt", "*.dat", "*.doc", "*.rst", "*.json", "*.tsv"],
     },
-    # This some needs to be here and in requirments.txt (for conda)
+    # This some needs to be here and in environment.yml (for conda)
     install_requires=[
-        "pandas >= 1.0",
+        "pandas >= 1.5",
+        "pyarrow >= 11.0",
         "numpy >= 1.20",
         "matplotlib >= 2.0.0",
         "requests >= 2.18",
         "xlrd > 1.1.0 ",
-        "openpyxl >= 3.0.6",
+        "openpyxl >= 3.0.6, < 3.1.1",
+        # openpyxl 3.1.1 has a bug that breaks the tests, issue is close, should be fine next release
         "docutils >= 0.14",
+        "faker >= 18.4.0",
     ],
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: End Users/Desktop",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

