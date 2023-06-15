# Comparing `tmp/RobertCommonBasic-0.1.41.tar.gz` & `tmp/RobertCommonBasic-0.1.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonBasic-0.1.41.tar", last modified: Fri Jun  9 09:56:00 2023, max compression
+gzip compressed data, was "RobertCommonBasic-0.1.42.tar", last modified: Thu Jun 15 07:13:23 2023, max compression
```

## Comparing `RobertCommonBasic-0.1.41.tar` & `RobertCommonBasic-0.1.42.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.346027 RobertCommonBasic-0.1.41/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonBasic-0.1.41/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonBasic-0.1.41/MANIFEST.in
--rw-rw-rw-   0        0        0      868 2023-06-09 09:56:00.346027 RobertCommonBasic-0.1.41/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-06-02 07:56:40.000000 RobertCommonBasic-0.1.41/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.211968 RobertCommonBasic-0.1.41/RobertCommonBasic.egg-info/
--rw-rw-rw-   0        0        0      868 2023-06-09 09:56:00.000000 RobertCommonBasic-0.1.41/RobertCommonBasic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4467 2023-06-09 09:56:00.000000 RobertCommonBasic-0.1.41/RobertCommonBasic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 09:56:00.000000 RobertCommonBasic-0.1.41/RobertCommonBasic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2023-06-09 09:56:00.000000 RobertCommonBasic-0.1.41/RobertCommonBasic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-09 09:56:00.000000 RobertCommonBasic-0.1.41/RobertCommonBasic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      187 2023-05-23 06:22:21.000000 RobertCommonBasic-0.1.41/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.212969 RobertCommonBasic-0.1.41/robertcommonbasic/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonBasic-0.1.41/robertcommonbasic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.212969 RobertCommonBasic-0.1.41/robertcommonbasic/basic/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.214972 RobertCommonBasic-0.1.41/robertcommonbasic/basic/base/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:39:20.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/base/__init__.py
--rw-rw-rw-   0        0        0      471 2023-01-04 02:45:25.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/base/constant.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.217409 RobertCommonBasic-0.1.41/robertcommonbasic/basic/cache/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/cache/__init__.py
--rw-rw-rw-   0        0        0      667 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/cache/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.219409 RobertCommonBasic-0.1.41/robertcommonbasic/basic/cls/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/cls/__init__.py
--rw-rw-rw-   0        0        0    12853 2023-06-09 09:28:37.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/cls/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.234174 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/__init__.py
--rw-rw-rw-   0        0        0    13611 2023-01-31 14:01:59.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/conversion.py
--rw-rw-rw-   0        0        0     4537 2022-11-14 07:54:50.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/crc16.py
--rw-rw-rw-   0        0        0     2169 2023-04-28 09:36:20.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/csv.py
--rw-rw-rw-   0        0        0    39297 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/datatuple.py
--rw-rw-rw-   0        0        0     2528 2023-05-25 09:05:54.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/express.py
--rw-rw-rw-   0        0        0     8304 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/frame.py
--rw-rw-rw-   0        0        0     1097 2022-11-14 09:48:07.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/nametuple.py
--rw-rw-rw-   0        0        0       62 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/type.py
--rw-rw-rw-   0        0        0    12943 2023-05-23 08:43:23.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.237181 RobertCommonBasic-0.1.41/robertcommonbasic/basic/decorator/
--rw-rw-rw-   0        0        0        0 2021-12-08 01:56:09.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/decorator/__init__.py
--rw-rw-rw-   0        0        0     1250 2022-12-05 08:07:43.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/decorator/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.241679 RobertCommonBasic-0.1.41/robertcommonbasic/basic/dt/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/dt/__init__.py
--rw-rw-rw-   0        0        0     4474 2022-12-28 02:51:52.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/dt/schedule.py
--rw-rw-rw-   0        0        0    10445 2023-05-18 03:32:13.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/dt/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.249686 RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/__init__.py
--rw-rw-rw-   0        0        0      583 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/aes.py
--rw-rw-rw-   0        0        0     3856 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/dsa.py
--rw-rw-rw-   0        0        0      716 2023-03-09 07:09:06.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/hash.py
--rw-rw-rw-   0        0        0      338 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/md5.py
--rw-rw-rw-   0        0        0     2661 2022-11-14 07:25:08.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/rsa.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.253038 RobertCommonBasic-0.1.41/robertcommonbasic/basic/error/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/error/__init__.py
--rw-rw-rw-   0        0        0     2354 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/error/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.255370 RobertCommonBasic-0.1.41/robertcommonbasic/basic/exector/
--rw-rw-rw-   0        0        0        0 2022-08-31 08:25:14.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/exector/__init__.py
--rw-rw-rw-   0        0        0     3641 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/exector/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.263368 RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/
--rw-rw-rw-   0        0        0        0 2022-11-18 02:39:00.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/__init__.py
--rw-rw-rw-   0        0        0     3053 2023-04-28 09:36:20.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/csv.py
--rw-rw-rw-   0        0        0     4951 2023-05-18 08:56:41.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/ini.py
--rw-rw-rw-   0        0        0     1035 2022-11-18 06:23:07.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/log.py
--rw-rw-rw-   0        0        0     3157 2022-11-24 03:18:18.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/xml.py
--rw-rw-rw-   0        0        0      339 2022-11-18 06:47:46.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/yaml.py
--rw-rw-rw-   0        0        0     3039 2023-03-08 07:31:52.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/zip.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.267867 RobertCommonBasic-0.1.41/robertcommonbasic/basic/log/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/log/__init__.py
--rw-rw-rw-   0        0        0     6582 2023-06-09 09:52:58.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/log/utils.py
--rw-rw-rw-   0        0        0     1366 2022-12-05 08:20:54.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/log/watch.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.270480 RobertCommonBasic-0.1.41/robertcommonbasic/basic/net/
--rw-rw-rw-   0        0        0        0 2022-06-29 12:44:36.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/net/__init__.py
--rw-rw-rw-   0        0        0     8521 2023-05-16 03:07:09.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/net/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.281123 RobertCommonBasic-0.1.41/robertcommonbasic/basic/os/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/os/__init__.py
--rw-rw-rw-   0        0        0      228 2022-12-14 09:03:01.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/os/cmd.py
--rw-rw-rw-   0        0        0      400 2022-06-29 09:34:23.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/os/env.py
--rw-rw-rw-   0        0        0     3446 2023-03-16 09:00:41.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/os/file.py
--rw-rw-rw-   0        0        0      533 2023-02-06 07:51:13.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/os/path.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.284511 RobertCommonBasic-0.1.41/robertcommonbasic/basic/process/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/process/__init__.py
--rw-rw-rw-   0        0        0     8845 2022-12-14 08:53:18.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/process/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.287021 RobertCommonBasic-0.1.41/robertcommonbasic/basic/profile/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/profile/__init__.py
--rw-rw-rw-   0        0        0     1264 2022-11-18 02:27:39.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/profile/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.291642 RobertCommonBasic-0.1.41/robertcommonbasic/basic/re/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/re/__init__.py
--rw-rw-rw-   0        0        0     1876 2023-05-25 09:11:33.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/re/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.295273 RobertCommonBasic-0.1.41/robertcommonbasic/basic/safetext/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/safetext/__init__.py
--rw-rw-rw-   0        0        0       91 2023-02-03 07:26:22.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/safetext/converter.py
--rw-rw-rw-   0        0        0      377 2022-11-18 02:33:07.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/safetext/funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.298338 RobertCommonBasic-0.1.41/robertcommonbasic/basic/sugar/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/sugar/__init__.py
--rw-rw-rw-   0        0        0      377 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/sugar/funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.300756 RobertCommonBasic-0.1.41/robertcommonbasic/basic/validation/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/validation/__init__.py
--rw-rw-rw-   0        0        0    36389 2023-02-21 08:51:30.000000 RobertCommonBasic-0.1.41/robertcommonbasic/basic/validation/input.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.302763 RobertCommonBasic-0.1.41/robertcommonbasic/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.303763 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:18.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.305763 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_cls/
--rw-rw-rw-   0        0        0        0 2022-04-22 02:07:10.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_cls/__init__.py
--rw-rw-rw-   0        0        0     1291 2023-03-02 14:03:08.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_cls/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.317431 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_data/
--rw-rw-rw-   0        0        0        0 2022-01-19 07:38:20.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_data/__init__.py
--rw-rw-rw-   0        0        0      928 2023-05-25 08:51:36.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_data/test_conversion.py
--rw-rw-rw-   0        0        0     5920 2022-04-21 06:58:53.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py
--rw-rw-rw-   0        0        0     2456 2022-01-27 05:56:15.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_data/test_frame.py
--rw-rw-rw-   0        0        0     4649 2023-05-23 08:03:46.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_data/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.320918 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_dt/
--rw-rw-rw-   0        0        0        0 2022-03-08 05:59:28.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_dt/__init__.py
--rw-rw-rw-   0        0        0     2313 2023-05-25 08:43:02.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_dt/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.325971 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_encrypt/
--rw-rw-rw-   0        0        0        0 2021-07-30 08:42:35.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_encrypt/__init__.py
--rw-rw-rw-   0        0        0    32599 2022-07-03 01:41:08.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py
--rw-rw-rw-   0        0        0      270 2022-07-03 01:04:51.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_encrypt/test_md5.py
--rw-rw-rw-   0        0        0     3004 2022-11-22 07:10:43.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.327977 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_exector/
--rw-rw-rw-   0        0        0        0 2022-08-31 08:24:08.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_exector/__init__.py
--rw-rw-rw-   0        0        0     1234 2022-12-05 09:33:27.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_exector/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.333978 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_file/
--rw-rw-rw-   0        0        0        0 2022-11-18 06:48:14.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_file/__init__.py
--rw-rw-rw-   0        0        0     1090 2023-02-03 06:30:00.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_file/test_csv.py
--rw-rw-rw-   0        0        0     4285 2023-02-02 03:00:01.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_file/test_xml.py
--rw-rw-rw-   0        0        0      705 2023-03-08 07:17:17.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_file/test_zip.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.335990 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_net/
--rw-rw-rw-   0        0        0        0 2022-06-29 13:56:13.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_net/__init__.py
--rw-rw-rw-   0        0        0      637 2023-05-16 02:40:06.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_net/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.339996 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_os/
--rw-rw-rw-   0        0        0        0 2022-03-25 04:05:00.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_os/__init__.py
--rw-rw-rw-   0        0        0      258 2022-06-29 09:29:01.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_os/test_env.py
--rw-rw-rw-   0        0        0      449 2022-11-14 02:56:25.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_os/test_file.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.342013 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_re/
--rw-rw-rw-   0        0        0        0 2022-05-18 02:57:45.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_re/__init__.py
--rw-rw-rw-   0        0        0      670 2023-05-23 08:45:26.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_re/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:00.345029 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_validation/
--rw-rw-rw-   0        0        0        0 2021-11-19 07:34:54.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_validation/__init__.py
--rw-rw-rw-   0        0        0      218 2022-05-10 03:46:33.000000 RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_validation/test_input.py
--rw-rw-rw-   0        0        0       42 2023-06-09 09:56:00.347027 RobertCommonBasic-0.1.41/setup.cfg
--rw-rw-rw-   0        0        0     3876 2023-06-09 09:27:49.000000 RobertCommonBasic-0.1.41/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.503600 RobertCommonBasic-0.1.42/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonBasic-0.1.42/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonBasic-0.1.42/MANIFEST.in
+-rw-rw-rw-   0        0        0      868 2023-06-15 07:13:23.503600 RobertCommonBasic-0.1.42/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-06-02 07:56:40.000000 RobertCommonBasic-0.1.42/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.363424 RobertCommonBasic-0.1.42/RobertCommonBasic.egg-info/
+-rw-rw-rw-   0        0        0      868 2023-06-15 07:13:23.000000 RobertCommonBasic-0.1.42/RobertCommonBasic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4467 2023-06-15 07:13:23.000000 RobertCommonBasic-0.1.42/RobertCommonBasic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 07:13:23.000000 RobertCommonBasic-0.1.42/RobertCommonBasic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      169 2023-06-15 07:13:23.000000 RobertCommonBasic-0.1.42/RobertCommonBasic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-15 07:13:23.000000 RobertCommonBasic-0.1.42/RobertCommonBasic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      187 2023-05-23 06:22:21.000000 RobertCommonBasic-0.1.42/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.367016 RobertCommonBasic-0.1.42/robertcommonbasic/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonBasic-0.1.42/robertcommonbasic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.368119 RobertCommonBasic-0.1.42/robertcommonbasic/basic/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.370124 RobertCommonBasic-0.1.42/robertcommonbasic/basic/base/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:39:20.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/base/__init__.py
+-rw-rw-rw-   0        0        0      471 2023-01-04 02:45:25.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/base/constant.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.372125 RobertCommonBasic-0.1.42/robertcommonbasic/basic/cache/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/cache/__init__.py
+-rw-rw-rw-   0        0        0      667 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/cache/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.374124 RobertCommonBasic-0.1.42/robertcommonbasic/basic/cls/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/cls/__init__.py
+-rw-rw-rw-   0        0        0    12853 2023-06-09 09:28:37.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/cls/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.388125 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/__init__.py
+-rw-rw-rw-   0        0        0    13611 2023-01-31 14:01:59.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/conversion.py
+-rw-rw-rw-   0        0        0     4537 2022-11-14 07:54:50.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/crc16.py
+-rw-rw-rw-   0        0        0     2169 2023-04-28 09:36:20.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/csv.py
+-rw-rw-rw-   0        0        0    39297 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/datatuple.py
+-rw-rw-rw-   0        0        0     2528 2023-05-25 09:05:54.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/express.py
+-rw-rw-rw-   0        0        0     8304 2023-06-15 07:11:29.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/frame.py
+-rw-rw-rw-   0        0        0     1097 2022-11-14 09:48:07.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/nametuple.py
+-rw-rw-rw-   0        0        0       62 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/type.py
+-rw-rw-rw-   0        0        0    12943 2023-06-15 07:11:29.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.391127 RobertCommonBasic-0.1.42/robertcommonbasic/basic/decorator/
+-rw-rw-rw-   0        0        0        0 2021-12-08 01:56:09.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/decorator/__init__.py
+-rw-rw-rw-   0        0        0     1250 2022-12-05 08:07:43.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/decorator/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.396124 RobertCommonBasic-0.1.42/robertcommonbasic/basic/dt/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/dt/__init__.py
+-rw-rw-rw-   0        0        0     4474 2022-12-28 02:51:52.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/dt/schedule.py
+-rw-rw-rw-   0        0        0    12394 2023-06-13 02:45:07.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/dt/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.402431 RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/__init__.py
+-rw-rw-rw-   0        0        0      583 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/aes.py
+-rw-rw-rw-   0        0        0     3856 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/dsa.py
+-rw-rw-rw-   0        0        0      716 2023-03-09 07:09:06.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/hash.py
+-rw-rw-rw-   0        0        0      338 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/md5.py
+-rw-rw-rw-   0        0        0     2661 2022-11-14 07:25:08.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/rsa.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.405430 RobertCommonBasic-0.1.42/robertcommonbasic/basic/error/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/error/__init__.py
+-rw-rw-rw-   0        0        0     2354 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/error/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.408498 RobertCommonBasic-0.1.42/robertcommonbasic/basic/exector/
+-rw-rw-rw-   0        0        0        0 2022-08-31 08:25:14.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/exector/__init__.py
+-rw-rw-rw-   0        0        0     3641 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/exector/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.417847 RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/
+-rw-rw-rw-   0        0        0        0 2022-11-18 02:39:00.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/__init__.py
+-rw-rw-rw-   0        0        0     3053 2023-04-28 09:36:20.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/csv.py
+-rw-rw-rw-   0        0        0     4951 2023-05-18 08:56:41.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/ini.py
+-rw-rw-rw-   0        0        0     1035 2022-11-18 06:23:07.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/log.py
+-rw-rw-rw-   0        0        0     3157 2022-11-24 03:18:18.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/xml.py
+-rw-rw-rw-   0        0        0      339 2022-11-18 06:47:46.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/yaml.py
+-rw-rw-rw-   0        0        0     3039 2023-03-08 07:31:52.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/zip.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.425847 RobertCommonBasic-0.1.42/robertcommonbasic/basic/log/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/log/__init__.py
+-rw-rw-rw-   0        0        0     6582 2023-06-09 09:52:58.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/log/utils.py
+-rw-rw-rw-   0        0        0     1366 2022-12-05 08:20:54.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/log/watch.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.428221 RobertCommonBasic-0.1.42/robertcommonbasic/basic/net/
+-rw-rw-rw-   0        0        0        0 2022-06-29 12:44:36.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/net/__init__.py
+-rw-rw-rw-   0        0        0     8521 2023-05-16 03:07:09.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/net/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.440098 RobertCommonBasic-0.1.42/robertcommonbasic/basic/os/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/os/__init__.py
+-rw-rw-rw-   0        0        0      228 2022-12-14 09:03:01.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/os/cmd.py
+-rw-rw-rw-   0        0        0      400 2022-06-29 09:34:23.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/os/env.py
+-rw-rw-rw-   0        0        0     3446 2023-03-16 09:00:41.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/os/file.py
+-rw-rw-rw-   0        0        0      533 2023-02-06 07:51:13.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/os/path.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.442562 RobertCommonBasic-0.1.42/robertcommonbasic/basic/process/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/process/__init__.py
+-rw-rw-rw-   0        0        0     8845 2022-12-14 08:53:18.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/process/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.444568 RobertCommonBasic-0.1.42/robertcommonbasic/basic/profile/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/profile/__init__.py
+-rw-rw-rw-   0        0        0     1264 2022-11-18 02:27:39.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/profile/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.446980 RobertCommonBasic-0.1.42/robertcommonbasic/basic/re/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/re/__init__.py
+-rw-rw-rw-   0        0        0     1876 2023-05-25 09:11:33.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/re/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.451549 RobertCommonBasic-0.1.42/robertcommonbasic/basic/safetext/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/safetext/__init__.py
+-rw-rw-rw-   0        0        0       91 2023-02-03 07:26:22.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/safetext/converter.py
+-rw-rw-rw-   0        0        0      377 2022-11-18 02:33:07.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/safetext/funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.454613 RobertCommonBasic-0.1.42/robertcommonbasic/basic/sugar/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/sugar/__init__.py
+-rw-rw-rw-   0        0        0      377 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/sugar/funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.459878 RobertCommonBasic-0.1.42/robertcommonbasic/basic/validation/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/validation/__init__.py
+-rw-rw-rw-   0        0        0    36389 2023-02-21 08:51:30.000000 RobertCommonBasic-0.1.42/robertcommonbasic/basic/validation/input.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.463911 RobertCommonBasic-0.1.42/robertcommonbasic/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.464914 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:18.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.467252 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_cls/
+-rw-rw-rw-   0        0        0        0 2022-04-22 02:07:10.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_cls/__init__.py
+-rw-rw-rw-   0        0        0     1291 2023-03-02 14:03:08.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_cls/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.474250 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_data/
+-rw-rw-rw-   0        0        0        0 2022-01-19 07:38:20.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_data/__init__.py
+-rw-rw-rw-   0        0        0      928 2023-05-25 08:51:36.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_data/test_conversion.py
+-rw-rw-rw-   0        0        0     5920 2022-04-21 06:58:53.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py
+-rw-rw-rw-   0        0        0     2456 2022-01-27 05:56:15.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_data/test_frame.py
+-rw-rw-rw-   0        0        0     4649 2023-05-23 08:03:46.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_data/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.476250 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_dt/
+-rw-rw-rw-   0        0        0        0 2022-03-08 05:59:28.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_dt/__init__.py
+-rw-rw-rw-   0        0        0     2313 2023-05-25 08:43:02.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_dt/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.481577 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_encrypt/
+-rw-rw-rw-   0        0        0        0 2021-07-30 08:42:35.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_encrypt/__init__.py
+-rw-rw-rw-   0        0        0    32599 2022-07-03 01:41:08.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py
+-rw-rw-rw-   0        0        0      270 2022-07-03 01:04:51.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_encrypt/test_md5.py
+-rw-rw-rw-   0        0        0     3004 2022-11-22 07:10:43.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.484584 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_exector/
+-rw-rw-rw-   0        0        0        0 2022-08-31 08:24:08.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_exector/__init__.py
+-rw-rw-rw-   0        0        0     1234 2022-12-05 09:33:27.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_exector/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.489665 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_file/
+-rw-rw-rw-   0        0        0        0 2022-11-18 06:48:14.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_file/__init__.py
+-rw-rw-rw-   0        0        0     1090 2023-02-03 06:30:00.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_file/test_csv.py
+-rw-rw-rw-   0        0        0     4285 2023-02-02 03:00:01.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_file/test_xml.py
+-rw-rw-rw-   0        0        0      705 2023-03-08 07:17:17.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_file/test_zip.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.492638 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_net/
+-rw-rw-rw-   0        0        0        0 2022-06-29 13:56:13.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_net/__init__.py
+-rw-rw-rw-   0        0        0      637 2023-05-16 02:40:06.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_net/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.495381 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_os/
+-rw-rw-rw-   0        0        0        0 2022-03-25 04:05:00.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_os/__init__.py
+-rw-rw-rw-   0        0        0      258 2022-06-29 09:29:01.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_os/test_env.py
+-rw-rw-rw-   0        0        0      449 2022-11-14 02:56:25.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_os/test_file.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.499258 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_re/
+-rw-rw-rw-   0        0        0        0 2022-05-18 02:57:45.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_re/__init__.py
+-rw-rw-rw-   0        0        0      670 2023-05-23 08:45:26.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_re/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:13:23.502116 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_validation/
+-rw-rw-rw-   0        0        0        0 2021-11-19 07:34:54.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_validation/__init__.py
+-rw-rw-rw-   0        0        0      218 2022-05-10 03:46:33.000000 RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_validation/test_input.py
+-rw-rw-rw-   0        0        0       42 2023-06-15 07:13:23.503600 RobertCommonBasic-0.1.42/setup.cfg
+-rw-rw-rw-   0        0        0     3876 2023-06-15 07:11:29.000000 RobertCommonBasic-0.1.42/setup.py
```

### Comparing `RobertCommonBasic-0.1.41/LICENSE` & `RobertCommonBasic-0.1.42/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/PKG-INFO` & `RobertCommonBasic-0.1.42/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonBasic
-Version: 0.1.41
+Version: 0.1.42
 Summary: Robert Common Basic Library
 Home-page: https://github.com/hun0423/RobertCommonBasic
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonBasic-0.1.41/RobertCommonBasic.egg-info/PKG-INFO` & `RobertCommonBasic-0.1.42/RobertCommonBasic.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonBasic
-Version: 0.1.41
+Version: 0.1.42
 Summary: Robert Common Basic Library
 Home-page: https://github.com/hun0423/RobertCommonBasic
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonBasic-0.1.41/RobertCommonBasic.egg-info/SOURCES.txt` & `RobertCommonBasic-0.1.42/RobertCommonBasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/cache/utils.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/cache/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/cls/utils.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/cls/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/conversion.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/conversion.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/crc16.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/crc16.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/csv.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/csv.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/datatuple.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/datatuple.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/express.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/express.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/frame.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
 # 包头起始长度
 def get_pack_start_length() -> int:
     return int(FRAME.FRAME_TYPE - FRAME.START)
 
 
 def convert_bytes_to_int(data: bytes) -> int:
-    return unpack('L', data[:4])[0]
+    return unpack('I', data[:4])[0]
 
 
 # 组包
 def pack_frame(packs: dict, secret: str = '') -> bytes:
     if isinstance(packs, dict):
         frame_type = packs.get('frame_type')
         if frame_type is None:
@@ -177,30 +177,30 @@
         if length > 0:
             packs = bytearray(length + FRAME.EXTRA_LENGTH)
             packs[FRAME.START: FRAME.START + 2] = FRAMEFLAG.START_FLAG  # 包头
             packs[FRAME.FRAME_TYPE] = frame_type  # 帧类型
             packs[FRAME.PACKAGE_TYPE] = package_type  # 包类型
             packs[FRAME.FRAME_INDEX: FRAME.FRAME_INDEX + 2] = pack('H', package_index)  # 编号
             packs[FRAME.TRANSFER_TYPE] = transfer_type  # 传输方式
-            packs[FRAME.CONTENT_LENGTH: FRAME.CONTENT_LENGTH + 4] = pack('L', length)  # 长度
+            packs[FRAME.CONTENT_LENGTH: FRAME.CONTENT_LENGTH + 4] = pack('I', length)  # 长度
             packs[FRAME.CONTENT: FRAME.CONTENT + length] = data
             packs[FRAME.CONTENT + length] = sum(data) & 0xFF
             packs[FRAME.END:] = FRAMEFLAG.END_FLAG
             return packs
         raise Exception(f"Invalid length({len(data)}<=0)")
     raise Exception(f"Invalid Type")
 
 
 # 解包
 def unpack_frame(data: bytes, secret: str = '') -> dict:
     length = len(data)
     if length > FRAME.EXTRA_LENGTH:
         packs = {}
         if data[FRAME.START: FRAME.START + 2] == FRAMEFLAG.START_FLAG and data[FRAME.END:] == FRAMEFLAG.END_FLAG:
-            content_length = unpack('L', data[FRAME.CONTENT_LENGTH: FRAME.CONTENT_LENGTH + 4])[0]
+            content_length = unpack('I', data[FRAME.CONTENT_LENGTH: FRAME.CONTENT_LENGTH + 4])[0]
             if length == content_length + FRAME.EXTRA_LENGTH:
                 content = data[FRAME.CONTENT: FRAME.CONTENT + content_length]
                 if sum(content) & 0xFF == data[FRAME.CONTENT + content_length]:    # 校验和
                     packs['frame_type'] = data[FRAME.FRAME_TYPE]
                     packs['package_type'] = data[FRAME.PACKAGE_TYPE]
                     packs['package_index'] = unpack('H', data[FRAME.FRAME_INDEX: FRAME.FRAME_INDEX + 2])[0]
                     packs['transfer_type'] = data[FRAME.TRANSFER_TYPE]
```

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/nametuple.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/nametuple.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/data/utils.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/data/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,16 +379,16 @@
         pass
     return value
 
 
 def inverse_long(value):
     try:
         value = int(float(value))
-        vev_value = unpack('HH', pack('L', value))
-        return unpack('L', pack('HH', vev_value[1], vev_value[0]))[0]
+        vev_value = unpack('HH', pack('I', value))
+        return unpack('I', pack('HH', vev_value[1], vev_value[0]))[0]
     except Exception:
         pass
     return value
 
 
 def inverse_float(value):
     try:
```

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/decorator/utils.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/decorator/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/dt/schedule.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/dt/schedule.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/dt/utils.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/dt/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+import math
 import pytz
 import logging
+import pandas as pd
+
 from datetime import datetime, timedelta, tzinfo
 from enum import Enum, unique
-from typing import Union, NamedTuple, Tuple, Optional, Any
+from typing import Union, NamedTuple, Tuple, Optional, Any, List
 from dateutil.relativedelta import relativedelta
 from dateutil.parser import parse
 from ..error.utils import InputDataError
 from ..validation import input
 from ..base.constant import DATETIME_FMT_FULL, DATETIME_FMT_DATE
 
 
@@ -285,7 +288,65 @@
         vs = {}
         for k, v in values.items():
             vs[k] = convert_values_property_time(v, original_tz, target_tz)
         return vs
     elif isinstance(values, datetime):
         return convert_time(values, original_tz, target_tz)
     return values
+
+
+def align_time(input: datetime, interval: str) -> datetime:
+    """时间对齐"""
+    input = input.replace(second=0, microsecond=0)
+    if interval == TimeInterval.m1:
+        return input
+
+    if interval == TimeInterval.m5:
+        minute = int(5 * (math.floor(input.minute / 5)))
+        input = input.replace(minute=minute)
+        return input
+
+    input = input.replace(minute=0)
+    if interval == TimeInterval.h1:
+        return input
+
+    input = input.replace(hour=0)
+    if interval == TimeInterval.d1:
+        return input
+
+    input = input.replace(day=1)
+    if interval == TimeInterval.M1:
+        return input
+
+    raise ValueError(f'Invalid time interval: {interval}')
+
+
+def normalize_dataframe(df: pd.DataFrame, interval: str):
+    # formalize input dataframe time index
+    if not isinstance(df.index, pd.DatetimeIndex):
+        if 'time' in df:
+            df = df.set_index('time')
+            if not isinstance(df.index, pd.DatetimeIndex):
+                df.index = pd.to_datetime(df.index)
+
+    if not isinstance(df.index, pd.DatetimeIndex):
+        raise ValueError(f'Invalid DataFrame index, {type(df.index)}, DatetimeIndex required')
+
+    index_floor = '5T'
+    if interval == TimeInterval.s1:
+        index_floor = 'S'
+    elif interval == TimeInterval.m1:
+        index_floor = 'T'
+
+    changes: List[str] = []
+    idx = df.index.floor(index_floor)
+    diff = df.index != idx
+    if diff.any():
+        change_map = pd.DataFrame(df.index[diff].values, index=idx[diff].values, columns=['t'])
+        changes = [f"{str(t)} <= {', '.join((str(t) for t in g['t']))}" for t, g in change_map.groupby(level=0)]
+        df = df.set_index(idx)
+
+    if df.index.duplicated().any():
+        changes = [f"removed: {str(t)}" for t in df[df.index.duplicated()].index]
+        df = df.groupby(level=0).last()
+
+    return df, changes
```

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/aes.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/aes.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/dsa.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/dsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/hash.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/hash.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/encrypt/rsa.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/encrypt/rsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/error/utils.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/error/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/exector/utils.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/exector/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/csv.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/csv.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/ini.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/ini.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/log.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/log.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/xml.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/xml.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/file/zip.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/file/zip.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/log/utils.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/log/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/log/watch.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/log/watch.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/net/utils.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/net/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/os/file.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/os/file.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/os/path.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/os/path.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/process/utils.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/process/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/profile/utils.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/profile/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/re/utils.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/re/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/basic/validation/input.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/basic/validation/input.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_cls/test_utils.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_cls/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_data/test_conversion.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_data/test_conversion.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_data/test_frame.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_data/test_frame.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_data/test_utils.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_data/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_dt/test_utils.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_dt/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_exector/test_utils.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_exector/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_file/test_csv.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_file/test_csv.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_file/test_xml.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_file/test_xml.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_file/test_zip.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_file/test_zip.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_net/test_utils.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_net/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/robertcommonbasic/tests/test_basic/test_re/test_utils.py` & `RobertCommonBasic-0.1.42/robertcommonbasic/tests/test_basic/test_re/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.41/setup.py` & `RobertCommonBasic-0.1.42/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonBasic'
 DESCRIPTION = 'Robert Common Basic Library'
 URL = 'https://github.com/hun0423/RobertCommonBasic'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.41'
-DATE = '2023-06-09'
+VERSION = '0.1.42'
+DATE = '2023-06-15'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

