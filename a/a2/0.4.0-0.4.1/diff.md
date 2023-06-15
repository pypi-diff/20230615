# Comparing `tmp/a2-0.4.0.tar.gz` & `tmp/a2-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a2-0.4.0.tar", max compression
+gzip compressed data, was "a2-0.4.1.tar", max compression
```

## Comparing `a2-0.4.0.tar` & `a2-0.4.1.tar`

### file list

```diff
@@ -1,1967 +1,1970 @@
--rw-r--r--   0        0        0     4419 2023-06-15 10:27:31.283733 a2-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 15:29:54.345253 a2-0.4.0/src/a2/__init__.py
--rw-r--r--   0        0        0       45 2023-01-13 09:43:31.404482 a2-0.4.0/src/a2/cli/__init__.py
--rw-r--r--   0        0        0      200 2023-01-13 09:53:11.940626 a2-0.4.0/src/a2/cli/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      297 2023-01-13 09:40:55.677429 a2-0.4.0/src/a2/cli/__pycache__/main.cpython-310.pyc
--rw-r--r--   0        0        0       39 2023-01-13 09:45:19.522669 a2-0.4.0/src/a2/cli/cli_plotting/__init__.py
--rw-r--r--   0        0        0      203 2023-01-13 09:53:11.952627 a2-0.4.0/src/a2/cli/cli_plotting/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      359 2023-01-13 09:53:14.892690 a2-0.4.0/src/a2/cli/cli_plotting/__pycache__/plot.cpython-310.pyc
--rw-r--r--   0        0        0     2094 2023-06-13 15:13:22.154868 a2-0.4.0/src/a2/cli/cli_plotting/__pycache__/single_plots.cpython-310.pyc
--rw-r--r--   0        0        0      107 2023-01-13 09:46:23.599985 a2-0.4.0/src/a2/cli/cli_plotting/plot.py
--rw-r--r--   0        0        0     2049 2023-06-13 14:49:56.664626 a2-0.4.0/src/a2/cli/cli_plotting/single_plots.py
--rw-r--r--   0        0        0       66 2023-01-13 09:36:10.235731 a2-0.4.0/src/a2/cli/main.py
--rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.4.0/src/a2/data/__init__.py
--rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.4.0/src/a2/data/emoji/__init__.py
--rw-r--r--   0        0        0   379747 2022-11-01 14:44:14.724032 a2-0.4.0/src/a2/data/emoji/emoji_df.csv
--rw-r--r--   0        0        0     1117 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/0023_fe0f_20e3.png
--rw-r--r--   0        0        0     1221 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/002a_fe0f_20e3.png
--rw-r--r--   0        0        0     1065 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/0030_fe0f_20e3.png
--rw-r--r--   0        0        0      989 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/0031_fe0f_20e3.png
--rw-r--r--   0        0        0     1043 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/0032_fe0f_20e3.png
--rw-r--r--   0        0        0     1133 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/0033_fe0f_20e3.png
--rw-r--r--   0        0        0     1077 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/0034_fe0f_20e3.png
--rw-r--r--   0        0        0     1204 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/0035_fe0f_20e3.png
--rw-r--r--   0        0        0     1142 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/0036_fe0f_20e3.png
--rw-r--r--   0        0        0      985 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/0037_fe0f_20e3.png
--rw-r--r--   0        0        0     1120 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/0038_fe0f_20e3.png
--rw-r--r--   0        0        0     1157 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/0039_fe0f_20e3.png
--rw-r--r--   0        0        0     1096 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/00a9.png
--rw-r--r--   0        0        0     1091 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/00ae.png
--rw-r--r--   0        0        0     1250 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f004.png
--rw-r--r--   0        0        0     1141 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f0cf.png
--rw-r--r--   0        0        0     1236 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f170.png
--rw-r--r--   0        0        0     1186 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f171.png
--rw-r--r--   0        0        0     1363 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f17e.png
--rw-r--r--   0        0        0     1075 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f17f.png
--rw-r--r--   0        0        0     1342 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f18e.png
--rw-r--r--   0        0        0     1352 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f191.png
--rw-r--r--   0        0        0     1192 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f192.png
--rw-r--r--   0        0        0     1133 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f193.png
--rw-r--r--   0        0        0     1150 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f194.png
--rw-r--r--   0        0        0     1202 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f195.png
--rw-r--r--   0        0        0     1194 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f196.png
--rw-r--r--   0        0        0     1264 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f197.png
--rw-r--r--   0        0        0     1471 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f198.png
--rw-r--r--   0        0        0     1260 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f199.png
--rw-r--r--   0        0        0     1361 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f19a.png
--rw-r--r--   0        0        0     1893 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1e8.png
--rw-r--r--   0        0        0     1526 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1e9.png
--rw-r--r--   0        0        0     1245 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1ea.png
--rw-r--r--   0        0        0     1346 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1eb.png
--rw-r--r--   0        0        0     1555 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1ec.png
--rw-r--r--   0        0        0     2029 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1ee.png
--rw-r--r--   0        0        0     1206 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1f1.png
--rw-r--r--   0        0        0     1444 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1f2.png
--rw-r--r--   0        0        0     1314 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1f4.png
--rw-r--r--   0        0        0     1016 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1f6.png
--rw-r--r--   0        0        0     1193 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1f7.png
--rw-r--r--   0        0        0     1597 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1f8.png
--rw-r--r--   0        0        0     1252 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1f9.png
--rw-r--r--   0        0        0     1890 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1fa.png
--rw-r--r--   0        0        0     1379 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1fc.png
--rw-r--r--   0        0        0     1637 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1fd.png
--rw-r--r--   0        0        0     1592 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1ff.png
--rw-r--r--   0        0        0     1362 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1e6.png
--rw-r--r--   0        0        0     1135 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1e7.png
--rw-r--r--   0        0        0      935 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1e9.png
--rw-r--r--   0        0        0      998 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1ea.png
--rw-r--r--   0        0        0     1253 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1eb.png
--rw-r--r--   0        0        0     1348 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1ec.png
--rw-r--r--   0        0        0     1129 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1ed.png
--rw-r--r--   0        0        0     1766 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1ee.png
--rw-r--r--   0        0        0     1173 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1ef.png
--rw-r--r--   0        0        0     1638 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1f1.png
--rw-r--r--   0        0        0     2553 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1f2.png
--rw-r--r--   0        0        0     2134 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1f3.png
--rw-r--r--   0        0        0     1662 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1f4.png
--rw-r--r--   0        0        0     1467 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1f6.png
--rw-r--r--   0        0        0     1477 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1f7.png
--rw-r--r--   0        0        0     1323 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1f8.png
--rw-r--r--   0        0        0     1794 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1f9.png
--rw-r--r--   0        0        0     1658 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1fb.png
--rw-r--r--   0        0        0     1278 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1fc.png
--rw-r--r--   0        0        0     1417 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1fe.png
--rw-r--r--   0        0        0     2195 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1ff.png
--rw-r--r--   0        0        0     1263 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1e6.png
--rw-r--r--   0        0        0     1241 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1e8.png
--rw-r--r--   0        0        0     2050 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1e9.png
--rw-r--r--   0        0        0     1831 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1eb.png
--rw-r--r--   0        0        0     1460 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1ec.png
--rw-r--r--   0        0        0      879 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1ed.png
--rw-r--r--   0        0        0     1053 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1ee.png
--rw-r--r--   0        0        0     1735 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1f0.png
--rw-r--r--   0        0        0     1317 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1f1.png
--rw-r--r--   0        0        0     1118 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1f2.png
--rw-r--r--   0        0        0     1055 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1f3.png
--rw-r--r--   0        0        0     1372 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1f4.png
--rw-r--r--   0        0        0     1073 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1f5.png
--rw-r--r--   0        0        0     1521 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1f7.png
--rw-r--r--   0        0        0     1609 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1fa.png
--rw-r--r--   0        0        0     1711 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1fb.png
--rw-r--r--   0        0        0     1215 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1fc.png
--rw-r--r--   0        0        0     1511 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1fd.png
--rw-r--r--   0        0        0     1224 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1fe.png
--rw-r--r--   0        0        0     1236 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1ff.png
--rw-r--r--   0        0        0     1280 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e9_1f1ea.png
--rw-r--r--   0        0        0     2888 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e9_1f1ec.png
--rw-r--r--   0        0        0     1331 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e9_1f1ef.png
--rw-r--r--   0        0        0     1257 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e9_1f1f0.png
--rw-r--r--   0        0        0     2283 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e9_1f1f2.png
--rw-r--r--   0        0        0     1737 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e9_1f1f4.png
--rw-r--r--   0        0        0     1324 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e9_1f1ff.png
--rw-r--r--   0        0        0     1513 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ea_1f1e6.png
--rw-r--r--   0        0        0     1976 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ea_1f1e8.png
--rw-r--r--   0        0        0     1138 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ea_1f1ea.png
--rw-r--r--   0        0        0     1301 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ea_1f1ec.png
--rw-r--r--   0        0        0     1270 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ea_1f1ed.png
--rw-r--r--   0        0        0     1719 2022-11-18 15:36:28.436585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ea_1f1f7.png
--rw-r--r--   0        0        0     1513 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ea_1f1f8.png
--rw-r--r--   0        0        0     1477 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ea_1f1f9.png
--rw-r--r--   0        0        0      969 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ea_1f1fa.png
--rw-r--r--   0        0        0     1213 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1eb_1f1ee.png
--rw-r--r--   0        0        0     2421 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1eb_1f1ef.png
--rw-r--r--   0        0        0     2067 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1eb_1f1f0.png
--rw-r--r--   0        0        0     1005 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1eb_1f1f2.png
--rw-r--r--   0        0        0     1837 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1eb_1f1f4.png
--rw-r--r--   0        0        0     1073 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1eb_1f1f7.png
--rw-r--r--   0        0        0     1362 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1e6.png
--rw-r--r--   0        0        0     2314 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1e7.png
--rw-r--r--   0        0        0     1749 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1e9.png
--rw-r--r--   0        0        0     1583 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1ea.png
--rw-r--r--   0        0        0     1274 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1eb.png
--rw-r--r--   0        0        0     1488 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1ec.png
--rw-r--r--   0        0        0     1425 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1ed.png
--rw-r--r--   0        0        0     1678 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1ee.png
--rw-r--r--   0        0        0     1202 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1f1.png
--rw-r--r--   0        0        0     1570 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1f2.png
--rw-r--r--   0        0        0     1023 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1f3.png
--rw-r--r--   0        0        0     1442 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1f5.png
--rw-r--r--   0        0        0     1641 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1f6.png
--rw-r--r--   0        0        0     1677 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1f7.png
--rw-r--r--   0        0        0     2181 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1f8.png
--rw-r--r--   0        0        0     1224 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1f9.png
--rw-r--r--   0        0        0     1354 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1fa.png
--rw-r--r--   0        0        0     1314 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1fc.png
--rw-r--r--   0        0        0     1857 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1fe.png
--rw-r--r--   0        0        0     1138 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ed_1f1f0.png
--rw-r--r--   0        0        0     1890 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ed_1f1f2.png
--rw-r--r--   0        0        0     1250 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ed_1f1f3.png
--rw-r--r--   0        0        0     1843 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ed_1f1f7.png
--rw-r--r--   0        0        0     1394 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ed_1f1f9.png
--rw-r--r--   0        0        0     1317 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ed_1f1fa.png
--rw-r--r--   0        0        0     1300 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1e8.png
--rw-r--r--   0        0        0     1131 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1e9.png
--rw-r--r--   0        0        0     1070 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1ea.png
--rw-r--r--   0        0        0     1453 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1f1.png
--rw-r--r--   0        0        0     1135 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1f2.png
--rw-r--r--   0        0        0     1507 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1f3.png
--rw-r--r--   0        0        0     2888 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1f4.png
--rw-r--r--   0        0        0     1295 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1f6.png
--rw-r--r--   0        0        0     1566 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1f7.png
--rw-r--r--   0        0        0     1577 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1f8.png
--rw-r--r--   0        0        0      995 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1f9.png
--rw-r--r--   0        0        0     1711 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ef_1f1ea.png
--rw-r--r--   0        0        0     1536 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ef_1f1f2.png
--rw-r--r--   0        0        0     1361 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ef_1f1f4.png
--rw-r--r--   0        0        0     1019 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ef_1f1f5.png
--rw-r--r--   0        0        0     1778 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1ea.png
--rw-r--r--   0        0        0     1133 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1ec.png
--rw-r--r--   0        0        0     1600 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1ed.png
--rw-r--r--   0        0        0     1897 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1ee.png
--rw-r--r--   0        0        0     1884 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1f2.png
--rw-r--r--   0        0        0     1760 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1f3.png
--rw-r--r--   0        0        0     1552 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1f5.png
--rw-r--r--   0        0        0     1531 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1f7.png
--rw-r--r--   0        0        0     1291 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1fc.png
--rw-r--r--   0        0        0     2144 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1fe.png
--rw-r--r--   0        0        0     1473 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1ff.png
--rw-r--r--   0        0        0     1229 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1e6.png
--rw-r--r--   0        0        0     1510 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1e7.png
--rw-r--r--   0        0        0     1336 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1e8.png
--rw-r--r--   0        0        0     1314 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1ee.png
--rw-r--r--   0        0        0     1483 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1f0.png
--rw-r--r--   0        0        0     1995 2022-11-18 15:36:28.440585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1f7.png
--rw-r--r--   0        0        0     1480 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1f8.png
--rw-r--r--   0        0        0     1333 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1f9.png
--rw-r--r--   0        0        0     1363 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1fa.png
--rw-r--r--   0        0        0     1056 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1fb.png
--rw-r--r--   0        0        0     1336 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1fe.png
--rw-r--r--   0        0        0     1158 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1e6.png
--rw-r--r--   0        0        0     1071 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1e8.png
--rw-r--r--   0        0        0     1548 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1e9.png
--rw-r--r--   0        0        0     1112 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1ea.png
--rw-r--r--   0        0        0     1073 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1eb.png
--rw-r--r--   0        0        0     1189 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1ec.png
--rw-r--r--   0        0        0     1577 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1ed.png
--rw-r--r--   0        0        0     1957 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1f0.png
--rw-r--r--   0        0        0     1046 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1f1.png
--rw-r--r--   0        0        0     1574 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1f2.png
--rw-r--r--   0        0        0     1204 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1f3.png
--rw-r--r--   0        0        0     1165 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1f4.png
--rw-r--r--   0        0        0     1791 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1f5.png
--rw-r--r--   0        0        0     1505 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1f6.png
--rw-r--r--   0        0        0     1373 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1f7.png
--rw-r--r--   0        0        0     2172 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1f8.png
--rw-r--r--   0        0        0     1035 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1f9.png
--rw-r--r--   0        0        0     1488 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1fa.png
--rw-r--r--   0        0        0     1163 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1fb.png
--rw-r--r--   0        0        0     1364 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1fc.png
--rw-r--r--   0        0        0     1311 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1fd.png
--rw-r--r--   0        0        0     2364 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1fe.png
--rw-r--r--   0        0        0     1802 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1ff.png
--rw-r--r--   0        0        0     1835 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1e6.png
--rw-r--r--   0        0        0     1794 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1e8.png
--rw-r--r--   0        0        0     1423 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1ea.png
--rw-r--r--   0        0        0     1149 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1eb.png
--rw-r--r--   0        0        0      881 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1ec.png
--rw-r--r--   0        0        0     1377 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1ee.png
--rw-r--r--   0        0        0     1234 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1f1.png
--rw-r--r--   0        0        0     1658 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1f4.png
--rw-r--r--   0        0        0      999 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1f5.png
--rw-r--r--   0        0        0     1148 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1f7.png
--rw-r--r--   0        0        0     2200 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1fa.png
--rw-r--r--   0        0        0     1683 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1ff.png
--rw-r--r--   0        0        0     1419 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f4_1f1f2.png
--rw-r--r--   0        0        0     1550 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1e6.png
--rw-r--r--   0        0        0      977 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1ea.png
--rw-r--r--   0        0        0     1502 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1eb.png
--rw-r--r--   0        0        0     1432 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1ec.png
--rw-r--r--   0        0        0     1695 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1ed.png
--rw-r--r--   0        0        0     1098 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1f0.png
--rw-r--r--   0        0        0     1040 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1f1.png
--rw-r--r--   0        0        0     3113 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1f2.png
--rw-r--r--   0        0        0     2228 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1f3.png
--rw-r--r--   0        0        0     1622 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1f7.png
--rw-r--r--   0        0        0     1211 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1f8.png
--rw-r--r--   0        0        0     1590 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1f9.png
--rw-r--r--   0        0        0     1022 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1fc.png
--rw-r--r--   0        0        0     1607 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1fe.png
--rw-r--r--   0        0        0      959 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f6_1f1e6.png
--rw-r--r--   0        0        0     1792 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f7_1f1ea.png
--rw-r--r--   0        0        0      954 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f7_1f1f4.png
--rw-r--r--   0        0        0     1872 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f7_1f1f8.png
--rw-r--r--   0        0        0     1298 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f7_1f1fa.png
--rw-r--r--   0        0        0     1632 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f7_1f1fc.png
--rw-r--r--   0        0        0     1134 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1e6.png
--rw-r--r--   0        0        0     1729 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1e7.png
--rw-r--r--   0        0        0     1725 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1e8.png
--rw-r--r--   0        0        0     1203 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1e9.png
--rw-r--r--   0        0        0     1307 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1ea.png
--rw-r--r--   0        0        0     1261 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1ec.png
--rw-r--r--   0        0        0     1893 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1ed.png
--rw-r--r--   0        0        0     1613 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1ee.png
--rw-r--r--   0        0        0     1658 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1ef.png
--rw-r--r--   0        0        0     1656 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1f0.png
--rw-r--r--   0        0        0     1411 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1f1.png
--rw-r--r--   0        0        0     1662 2022-11-18 15:36:28.444585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1f2.png
--rw-r--r--   0        0        0     1228 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1f3.png
--rw-r--r--   0        0        0      884 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1f4.png
--rw-r--r--   0        0        0     1557 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1f7.png
--rw-r--r--   0        0        0     1630 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1f8.png
--rw-r--r--   0        0        0     1600 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1f9.png
--rw-r--r--   0        0        0     1424 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1fb.png
--rw-r--r--   0        0        0     1684 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1fd.png
--rw-r--r--   0        0        0     1373 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1fe.png
--rw-r--r--   0        0        0     2344 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1ff.png
--rw-r--r--   0        0        0     1893 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1e6.png
--rw-r--r--   0        0        0     2139 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1e8.png
--rw-r--r--   0        0        0      968 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1e9.png
--rw-r--r--   0        0        0     1213 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1eb.png
--rw-r--r--   0        0        0     1780 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1ec.png
--rw-r--r--   0        0        0     1646 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1ed.png
--rw-r--r--   0        0        0     1440 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1ef.png
--rw-r--r--   0        0        0     1176 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1f0.png
--rw-r--r--   0        0        0     1409 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1f1.png
--rw-r--r--   0        0        0     1338 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1f2.png
--rw-r--r--   0        0        0     1118 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1f3.png
--rw-r--r--   0        0        0     1163 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1f4.png
--rw-r--r--   0        0        0     1213 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1f7.png
--rw-r--r--   0        0        0     1448 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1f9.png
--rw-r--r--   0        0        0     2227 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1fb.png
--rw-r--r--   0        0        0     1350 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1fc.png
--rw-r--r--   0        0        0     1690 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1ff.png
--rw-r--r--   0        0        0     1105 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fa_1f1e6.png
--rw-r--r--   0        0        0     1967 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fa_1f1ec.png
--rw-r--r--   0        0        0     2435 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fa_1f1f2.png
--rw-r--r--   0        0        0     1129 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fa_1f1f3.png
--rw-r--r--   0        0        0     2435 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fa_1f1f8.png
--rw-r--r--   0        0        0     2010 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fa_1f1fe.png
--rw-r--r--   0        0        0     1743 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fa_1f1ff.png
--rw-r--r--   0        0        0     1197 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fb_1f1e6.png
--rw-r--r--   0        0        0     1337 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fb_1f1e8.png
--rw-r--r--   0        0        0     1580 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fb_1f1ea.png
--rw-r--r--   0        0        0     1974 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fb_1f1ec.png
--rw-r--r--   0        0        0     2635 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fb_1f1ee.png
--rw-r--r--   0        0        0     1046 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fb_1f1f3.png
--rw-r--r--   0        0        0     1594 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fb_1f1fa.png
--rw-r--r--   0        0        0     1319 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fc_1f1eb.png
--rw-r--r--   0        0        0     1134 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fc_1f1f8.png
--rw-r--r--   0        0        0     1128 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fd_1f1f0.png
--rw-r--r--   0        0        0     1184 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fe_1f1ea.png
--rw-r--r--   0        0        0     1649 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fe_1f1f9.png
--rw-r--r--   0        0        0     2075 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ff_1f1e6.png
--rw-r--r--   0        0        0     1071 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ff_1f1f2.png
--rw-r--r--   0        0        0     2394 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ff_1f1fc.png
--rw-r--r--   0        0        0     1081 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f201.png
--rw-r--r--   0        0        0     1165 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f202.png
--rw-r--r--   0        0        0     1478 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f21a.png
--rw-r--r--   0        0        0     1514 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f22f.png
--rw-r--r--   0        0        0     1682 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f232.png
--rw-r--r--   0        0        0     1372 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f233.png
--rw-r--r--   0        0        0     1450 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f234.png
--rw-r--r--   0        0        0     1667 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f235.png
--rw-r--r--   0        0        0     1243 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f236.png
--rw-r--r--   0        0        0     1127 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f237.png
--rw-r--r--   0        0        0     1207 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f238.png
--rw-r--r--   0        0        0     1517 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f239.png
--rw-r--r--   0        0        0     1349 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f23a.png
--rw-r--r--   0        0        0     1457 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f250.png
--rw-r--r--   0        0        0     1181 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f251.png
--rw-r--r--   0        0        0     1345 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f300.png
--rw-r--r--   0        0        0     1493 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f301.png
--rw-r--r--   0        0        0     1753 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f302.png
--rw-r--r--   0        0        0     2162 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f303.png
--rw-r--r--   0        0        0     1959 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f304.png
--rw-r--r--   0        0        0     1748 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f305.png
--rw-r--r--   0        0        0     2046 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f306.png
--rw-r--r--   0        0        0     2397 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f307.png
--rw-r--r--   0        0        0     3358 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f308.png
--rw-r--r--   0        0        0     1972 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f309.png
--rw-r--r--   0        0        0     2761 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f30a.png
--rw-r--r--   0        0        0     3524 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f30b.png
--rw-r--r--   0        0        0     1639 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f30c.png
--rw-r--r--   0        0        0     3984 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f30d.png
--rw-r--r--   0        0        0     3347 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f30e.png
--rw-r--r--   0        0        0     3956 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f30f.png
--rw-r--r--   0        0        0     2985 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f310.png
--rw-r--r--   0        0        0     1274 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f311.png
--rw-r--r--   0        0        0     2102 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f312.png
--rw-r--r--   0        0        0     2416 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f313.png
--rw-r--r--   0        0        0     2310 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f314.png
--rw-r--r--   0        0        0     1897 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f315.png
--rw-r--r--   0        0        0     2545 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f316.png
--rw-r--r--   0        0        0     2489 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f317.png
--rw-r--r--   0        0        0     1857 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f318.png
--rw-r--r--   0        0        0     1394 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f319.png
--rw-r--r--   0        0        0     1551 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f31a.png
--rw-r--r--   0        0        0     1589 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f31b.png
--rw-r--r--   0        0        0     1662 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f31c.png
--rw-r--r--   0        0        0     2808 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f31d.png
--rw-r--r--   0        0        0     3537 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f31e.png
--rw-r--r--   0        0        0     1898 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f31f.png
--rw-r--r--   0        0        0     2160 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f320.png
--rw-r--r--   0        0        0     1925 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f321.png
--rw-r--r--   0        0        0     1971 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f324.png
--rw-r--r--   0        0        0     1326 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f325.png
--rw-r--r--   0        0        0     2070 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f326.png
--rw-r--r--   0        0        0     1721 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f327.png
--rw-r--r--   0        0        0     1666 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f328.png
--rw-r--r--   0        0        0     1323 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f329.png
--rw-r--r--   0        0        0     2338 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f32a.png
--rw-r--r--   0        0        0     1345 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f32b.png
--rw-r--r--   0        0        0     1482 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f32c.png
--rw-r--r--   0        0        0     2143 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f32d.png
--rw-r--r--   0        0        0     3164 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f32e.png
--rw-r--r--   0        0        0     2846 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f32f.png
--rw-r--r--   0        0        0     2278 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f330.png
--rw-r--r--   0        0        0     1332 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f331.png
--rw-r--r--   0        0        0     2597 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f332.png
--rw-r--r--   0        0        0     2484 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f333.png
--rw-r--r--   0        0        0     3072 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f334.png
--rw-r--r--   0        0        0     2572 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f335.png
--rw-r--r--   0        0        0     1845 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f336.png
--rw-r--r--   0        0        0     3135 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f337.png
--rw-r--r--   0        0        0     3604 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f338.png
--rw-r--r--   0        0        0     2576 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f339.png
--rw-r--r--   0        0        0     3826 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f33a.png
--rw-r--r--   0        0        0     2868 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f33b.png
--rw-r--r--   0        0        0     2956 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f33c.png
--rw-r--r--   0        0        0     3578 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f33d.png
--rw-r--r--   0        0        0     3449 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f33e.png
--rw-r--r--   0        0        0     2049 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f33f.png
--rw-r--r--   0        0        0     3051 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f340.png
--rw-r--r--   0        0        0     2961 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f341.png
--rw-r--r--   0        0        0     2139 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f342.png
--rw-r--r--   0        0        0     2318 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f343.png
--rw-r--r--   0        0        0     2132 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f344.png
--rw-r--r--   0        0        0     2412 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f345.png
--rw-r--r--   0        0        0     1652 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f346.png
--rw-r--r--   0        0        0     3397 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f347.png
--rw-r--r--   0        0        0     2312 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f348.png
--rw-r--r--   0        0        0     1901 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f349.png
--rw-r--r--   0        0        0     2540 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f34a.png
--rw-r--r--   0        0        0     2346 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f34b.png
--rw-r--r--   0        0        0     2330 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f34c.png
--rw-r--r--   0        0        0     3133 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f34d.png
--rw-r--r--   0        0        0     2045 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f34e.png
--rw-r--r--   0        0        0     1960 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f34f.png
--rw-r--r--   0        0        0     1295 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f350.png
--rw-r--r--   0        0        0     2750 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f351.png
--rw-r--r--   0        0        0     2440 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f352.png
--rw-r--r--   0        0        0     3080 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f353.png
--rw-r--r--   0        0        0     3804 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f354.png
--rw-r--r--   0        0        0     2094 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f355.png
--rw-r--r--   0        0        0     2512 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f356.png
--rw-r--r--   0        0        0     1660 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f357.png
--rw-r--r--   0        0        0     2273 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f358.png
--rw-r--r--   0        0        0     2050 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f359.png
--rw-r--r--   0        0        0     1857 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f35a.png
--rw-r--r--   0        0        0     2172 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f35b.png
--rw-r--r--   0        0        0     3130 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f35c.png
--rw-r--r--   0        0        0     2982 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f35d.png
--rw-r--r--   0        0        0     1849 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f35e.png
--rw-r--r--   0        0        0     2730 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f35f.png
--rw-r--r--   0        0        0     1949 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f360.png
--rw-r--r--   0        0        0     2058 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f361.png
--rw-r--r--   0        0        0     1834 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f362.png
--rw-r--r--   0        0        0     2825 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f363.png
--rw-r--r--   0        0        0     3028 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f364.png
--rw-r--r--   0        0        0     1761 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f365.png
--rw-r--r--   0        0        0     1748 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f366.png
--rw-r--r--   0        0        0     2335 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f367.png
--rw-r--r--   0        0        0     2337 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f368.png
--rw-r--r--   0        0        0     4358 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f369.png
--rw-r--r--   0        0        0     2375 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f36a.png
--rw-r--r--   0        0        0     1498 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f36b.png
--rw-r--r--   0        0        0     2528 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f36c.png
--rw-r--r--   0        0        0     2993 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f36d.png
--rw-r--r--   0        0        0     1876 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f36e.png
--rw-r--r--   0        0        0     3145 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f36f.png
--rw-r--r--   0        0        0     2091 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f370.png
--rw-r--r--   0        0        0     4187 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f371.png
--rw-r--r--   0        0        0     2229 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f372.png
--rw-r--r--   0        0        0     2053 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f373.png
--rw-r--r--   0        0        0     1571 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f374.png
--rw-r--r--   0        0        0     2237 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f375.png
--rw-r--r--   0        0        0     1653 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f376.png
--rw-r--r--   0        0        0     1820 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f377.png
--rw-r--r--   0        0        0     2130 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f378.png
--rw-r--r--   0        0        0     2815 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f379.png
--rw-r--r--   0        0        0     3064 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f37a.png
--rw-r--r--   0        0        0     3070 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f37b.png
--rw-r--r--   0        0        0     1840 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f37c.png
--rw-r--r--   0        0        0     2200 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f37d.png
--rw-r--r--   0        0        0     2490 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f37e.png
--rw-r--r--   0        0        0     3063 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f37f.png
--rw-r--r--   0        0        0     2216 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f380.png
--rw-r--r--   0        0        0     2290 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f381.png
--rw-r--r--   0        0        0     2452 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f382.png
--rw-r--r--   0        0        0     1957 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f383.png
--rw-r--r--   0        0        0     3064 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f384.png
--rw-r--r--   0        0        0     3193 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f385.png
--rw-r--r--   0        0        0     2478 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f386.png
--rw-r--r--   0        0        0     2644 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f387.png
--rw-r--r--   0        0        0     1412 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f388.png
--rw-r--r--   0        0        0     3725 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f389.png
--rw-r--r--   0        0        0     3748 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f38a.png
--rw-r--r--   0        0        0     2909 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f38b.png
--rw-r--r--   0        0        0     2120 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f38c.png
--rw-r--r--   0        0        0     2268 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f38d.png
--rw-r--r--   0        0        0     3885 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f38e.png
--rw-r--r--   0        0        0    13409 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f38f.png
--rw-r--r--   0        0        0     2158 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f390.png
--rw-r--r--   0        0        0     3030 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f391.png
--rw-r--r--   0        0        0     2593 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f392.png
--rw-r--r--   0        0        0     1595 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f393.png
--rw-r--r--   0        0        0     1673 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f396.png
--rw-r--r--   0        0        0     1273 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f397.png
--rw-r--r--   0        0        0     2738 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f399.png
--rw-r--r--   0        0        0     1254 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f39a.png
--rw-r--r--   0        0        0     2214 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f39b.png
--rw-r--r--   0        0        0     2621 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f39e.png
--rw-r--r--   0        0        0     1459 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f39f.png
--rw-r--r--   0        0        0     3774 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3a0.png
--rw-r--r--   0        0        0     3756 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3a1.png
--rw-r--r--   0        0        0     2888 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3a2.png
--rw-r--r--   0        0        0     3092 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3a3.png
--rw-r--r--   0        0        0     1510 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3a4.png
--rw-r--r--   0        0        0     2437 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3a5.png
--rw-r--r--   0        0        0     1101 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3a6.png
--rw-r--r--   0        0        0     2400 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3a7.png
--rw-r--r--   0        0        0     3744 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3a8.png
--rw-r--r--   0        0        0     1380 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3a9.png
--rw-r--r--   0        0        0     3014 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3aa.png
--rw-r--r--   0        0        0     1519 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ab.png
--rw-r--r--   0        0        0     1679 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ac.png
--rw-r--r--   0        0        0     3610 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ad.png
--rw-r--r--   0        0        0     2008 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ae.png
--rw-r--r--   0        0        0     2799 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3af.png
--rw-r--r--   0        0        0     2850 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3b0.png
--rw-r--r--   0        0        0     1685 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3b1.png
--rw-r--r--   0        0        0     1690 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3b2.png
--rw-r--r--   0        0        0     2574 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3b3.png
--rw-r--r--   0        0        0     1297 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3b4.png
--rw-r--r--   0        0        0      989 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3b5.png
--rw-r--r--   0        0        0     1731 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3b6.png
--rw-r--r--   0        0        0     2673 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3b7.png
--rw-r--r--   0        0        0     2595 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3b8.png
--rw-r--r--   0        0        0     1147 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3b9.png
--rw-r--r--   0        0        0     3202 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ba.png
--rw-r--r--   0        0        0     3440 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3bb.png
--rw-r--r--   0        0        0     1461 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3bc.png
--rw-r--r--   0        0        0     1974 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3bd.png
--rw-r--r--   0        0        0     2114 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3be.png
--rw-r--r--   0        0        0     3507 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3bf.png
--rw-r--r--   0        0        0     3092 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c0.png
--rw-r--r--   0        0        0     1384 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c1.png
--rw-r--r--   0        0        0     3205 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c2.png
--rw-r--r--   0        0        0     2226 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c3.png
--rw-r--r--   0        0        0     2518 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c3_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2449 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c3_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3228 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c4.png
--rw-r--r--   0        0        0     3265 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c4_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3181 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c4_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2901 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c5.png
--rw-r--r--   0        0        0     2765 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c6.png
--rw-r--r--   0        0        0     2834 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c7.png
--rw-r--r--   0        0        0     2681 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c8.png
--rw-r--r--   0        0        0     2430 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c9.png
--rw-r--r--   0        0        0     2697 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ca.png
--rw-r--r--   0        0        0     3074 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ca_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2879 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ca_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3446 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3cb.png
--rw-r--r--   0        0        0     3400 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3cb_fe0f_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3505 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3cb_fe0f_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2121 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3cc.png
--rw-r--r--   0        0        0     2502 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3cc_fe0f_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2612 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3cc_fe0f_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2485 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3cd.png
--rw-r--r--   0        0        0     2826 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ce.png
--rw-r--r--   0        0        0     1908 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3cf.png
--rw-r--r--   0        0        0     1724 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3d0.png
--rw-r--r--   0        0        0     1866 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3d1.png
--rw-r--r--   0        0        0     1758 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3d2.png
--rw-r--r--   0        0        0     2481 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3d3.png
--rw-r--r--   0        0        0     3018 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3d4.png
--rw-r--r--   0        0        0     2698 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3d5.png
--rw-r--r--   0        0        0     3183 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3d6.png
--rw-r--r--   0        0        0     3121 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3d7.png
--rw-r--r--   0        0        0     3021 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3d8.png
--rw-r--r--   0        0        0     1628 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3d9.png
--rw-r--r--   0        0        0     2752 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3da.png
--rw-r--r--   0        0        0     2060 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3db.png
--rw-r--r--   0        0        0     3123 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3dc.png
--rw-r--r--   0        0        0     3133 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3dd.png
--rw-r--r--   0        0        0     2371 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3de.png
--rw-r--r--   0        0        0     4049 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3df.png
--rw-r--r--   0        0        0     2364 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3e0.png
--rw-r--r--   0        0        0     2954 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3e1.png
--rw-r--r--   0        0        0     2241 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3e2.png
--rw-r--r--   0        0        0     2318 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3e3.png
--rw-r--r--   0        0        0     2654 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3e4.png
--rw-r--r--   0        0        0     1880 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3e5.png
--rw-r--r--   0        0        0     2564 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3e6.png
--rw-r--r--   0        0        0     1142 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3e7.png
--rw-r--r--   0        0        0     2990 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3e8.png
--rw-r--r--   0        0        0     3226 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3e9.png
--rw-r--r--   0        0        0     2202 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ea.png
--rw-r--r--   0        0        0     2239 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3eb.png
--rw-r--r--   0        0        0     2206 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ec.png
--rw-r--r--   0        0        0     2448 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ed.png
--rw-r--r--   0        0        0     1482 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ee.png
--rw-r--r--   0        0        0     2396 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ef.png
--rw-r--r--   0        0        0     3103 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f0.png
--rw-r--r--   0        0        0      848 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f3.png
--rw-r--r--   0        0        0     1471 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f3_fe0f_200d_1f308.png
--rw-r--r--   0        0        0     1389 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f3_fe0f_200d_26a7_fe0f.png
--rw-r--r--   0        0        0      761 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f4.png
--rw-r--r--   0        0        0     1096 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f4_200d_2620_fe0f.png
--rw-r--r--   0        0        0     1283 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f4_e0067_e0062_e0065_e006e_e0067_e007f.png
--rw-r--r--   0        0        0     1451 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f4_e0067_e0062_e0073_e0063_e0074_e007f.png
--rw-r--r--   0        0        0     2115 2022-11-18 15:36:28.448585 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f4_e0067_e0062_e0077_e006c_e0073_e007f.png
--rw-r--r--   0        0        0     4095 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f5.png
--rw-r--r--   0        0        0      495 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f7.png
--rw-r--r--   0        0        0     3310 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f8.png
--rw-r--r--   0        0        0     2605 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f9.png
--rw-r--r--   0        0        0     2936 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f3fa.png
--rw-r--r--   0        0        0     1698 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f400.png
--rw-r--r--   0        0        0     2505 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f401.png
--rw-r--r--   0        0        0     1710 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f402.png
--rw-r--r--   0        0        0     1549 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f403.png
--rw-r--r--   0        0        0     2271 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f404.png
--rw-r--r--   0        0        0     3086 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f405.png
--rw-r--r--   0        0        0     2863 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f406.png
--rw-r--r--   0        0        0     1741 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f407.png
--rw-r--r--   0        0        0     2893 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f408.png
--rw-r--r--   0        0        0     1511 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f408_200d_2b1b.png
--rw-r--r--   0        0        0     4191 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f409.png
--rw-r--r--   0        0        0     2749 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f40a.png
--rw-r--r--   0        0        0     2014 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f40b.png
--rw-r--r--   0        0        0     3036 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f40c.png
--rw-r--r--   0        0        0     2917 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f40d.png
--rw-r--r--   0        0        0     2236 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f40e.png
--rw-r--r--   0        0        0     2169 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f40f.png
--rw-r--r--   0        0        0     1862 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f410.png
--rw-r--r--   0        0        0     1931 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f411.png
--rw-r--r--   0        0        0     2556 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f412.png
--rw-r--r--   0        0        0     2453 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f413.png
--rw-r--r--   0        0        0     2304 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f414.png
--rw-r--r--   0        0        0     2328 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f415.png
--rw-r--r--   0        0        0     2326 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f415_200d_1f9ba.png
--rw-r--r--   0        0        0     1591 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f416.png
--rw-r--r--   0        0        0     1773 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f417.png
--rw-r--r--   0        0        0     1699 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f418.png
--rw-r--r--   0        0        0     2151 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f419.png
--rw-r--r--   0        0        0     1983 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f41a.png
--rw-r--r--   0        0        0     3478 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f41b.png
--rw-r--r--   0        0        0     2245 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f41c.png
--rw-r--r--   0        0        0     3566 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f41d.png
--rw-r--r--   0        0        0     3427 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f41e.png
--rw-r--r--   0        0        0     1868 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f41f.png
--rw-r--r--   0        0        0     3171 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f420.png
--rw-r--r--   0        0        0     3511 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f421.png
--rw-r--r--   0        0        0     2029 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f422.png
--rw-r--r--   0        0        0     2750 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f423.png
--rw-r--r--   0        0        0     1385 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f424.png
--rw-r--r--   0        0        0     2506 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f425.png
--rw-r--r--   0        0        0     1535 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f426.png
--rw-r--r--   0        0        0     1612 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f427.png
--rw-r--r--   0        0        0     1805 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f428.png
--rw-r--r--   0        0        0     2137 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f429.png
--rw-r--r--   0        0        0     1655 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f42a.png
--rw-r--r--   0        0        0     2229 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f42b.png
--rw-r--r--   0        0        0     2182 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f42c.png
--rw-r--r--   0        0        0     2063 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f42d.png
--rw-r--r--   0        0        0     2011 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f42e.png
--rw-r--r--   0        0        0     3152 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f42f.png
--rw-r--r--   0        0        0     1994 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f430.png
--rw-r--r--   0        0        0     2193 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f431.png
--rw-r--r--   0        0        0     4538 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f432.png
--rw-r--r--   0        0        0     2468 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f433.png
--rw-r--r--   0        0        0     2249 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f434.png
--rw-r--r--   0        0        0     2358 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f435.png
--rw-r--r--   0        0        0     2210 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f436.png
--rw-r--r--   0        0        0     2307 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f437.png
--rw-r--r--   0        0        0     3023 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f438.png
--rw-r--r--   0        0        0     2911 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f439.png
--rw-r--r--   0        0        0     1848 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f43a.png
--rw-r--r--   0        0        0     1870 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f43b.png
--rw-r--r--   0        0        0     1802 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f43b_200d_2744_fe0f.png
--rw-r--r--   0        0        0     1740 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f43c.png
--rw-r--r--   0        0        0     1528 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f43d.png
--rw-r--r--   0        0        0      771 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f43e.png
--rw-r--r--   0        0        0     3248 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f43f.png
--rw-r--r--   0        0        0     1237 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f440.png
--rw-r--r--   0        0        0     2158 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f441.png
--rw-r--r--   0        0        0     1409 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f441_fe0f_200d_1f5e8_fe0f.png
--rw-r--r--   0        0        0     1291 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f442.png
--rw-r--r--   0        0        0     1094 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f443.png
--rw-r--r--   0        0        0     1491 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f444.png
--rw-r--r--   0        0        0     1666 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f445.png
--rw-r--r--   0        0        0     1054 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f446.png
--rw-r--r--   0        0        0     1039 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f447.png
--rw-r--r--   0        0        0      972 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f448.png
--rw-r--r--   0        0        0      959 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f449.png
--rw-r--r--   0        0        0     1180 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f44a.png
--rw-r--r--   0        0        0     1977 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f44b.png
--rw-r--r--   0        0        0     1488 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f44c.png
--rw-r--r--   0        0        0     1454 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f44d.png
--rw-r--r--   0        0        0     1423 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f44e.png
--rw-r--r--   0        0        0     1748 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f44f.png
--rw-r--r--   0        0        0     1459 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f450.png
--rw-r--r--   0        0        0     3262 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f451.png
--rw-r--r--   0        0        0     2519 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f452.png
--rw-r--r--   0        0        0     1157 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f453.png
--rw-r--r--   0        0        0     2735 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f454.png
--rw-r--r--   0        0        0     1489 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f455.png
--rw-r--r--   0        0        0     2568 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f456.png
--rw-r--r--   0        0        0     1811 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f457.png
--rw-r--r--   0        0        0     3086 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f458.png
--rw-r--r--   0        0        0     2700 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f459.png
--rw-r--r--   0        0        0     1671 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f45a.png
--rw-r--r--   0        0        0     1638 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f45b.png
--rw-r--r--   0        0        0     2326 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f45c.png
--rw-r--r--   0        0        0     1758 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f45d.png
--rw-r--r--   0        0        0     2073 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f45e.png
--rw-r--r--   0        0        0     1529 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f45f.png
--rw-r--r--   0        0        0     2329 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f460.png
--rw-r--r--   0        0        0     1465 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f461.png
--rw-r--r--   0        0        0     1526 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f462.png
--rw-r--r--   0        0        0      806 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f463.png
--rw-r--r--   0        0        0      905 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f464.png
--rw-r--r--   0        0        0     1012 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f465.png
--rw-r--r--   0        0        0     2126 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f466.png
--rw-r--r--   0        0        0     2215 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f467.png
--rw-r--r--   0        0        0     2023 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468.png
--rw-r--r--   0        0        0     4097 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f33e.png
--rw-r--r--   0        0        0     2906 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f373.png
--rw-r--r--   0        0        0     2948 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f37c.png
--rw-r--r--   0        0        0     2403 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f393.png
--rw-r--r--   0        0        0     3325 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f3a4.png
--rw-r--r--   0        0        0     3552 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f3a8.png
--rw-r--r--   0        0        0     2669 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f3eb.png
--rw-r--r--   0        0        0     3239 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f3ed.png
--rw-r--r--   0        0        0     2498 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f466.png
--rw-r--r--   0        0        0     2694 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f466_200d_1f466.png
--rw-r--r--   0        0        0     2644 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f467.png
--rw-r--r--   0        0        0     3625 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f467_200d_1f466.png
--rw-r--r--   0        0        0     3062 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f467_200d_1f467.png
--rw-r--r--   0        0        0     3524 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f466.png
--rw-r--r--   0        0        0     4079 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f466_200d_1f466.png
--rw-r--r--   0        0        0     3727 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f467.png
--rw-r--r--   0        0        0     4567 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f467_200d_1f466.png
--rw-r--r--   0        0        0     4614 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f467_200d_1f467.png
--rw-r--r--   0        0        0     3437 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f466.png
--rw-r--r--   0        0        0     4310 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f466_200d_1f466.png
--rw-r--r--   0        0        0     3696 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f467.png
--rw-r--r--   0        0        0     4734 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f467_200d_1f466.png
--rw-r--r--   0        0        0     4600 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f467_200d_1f467.png
--rw-r--r--   0        0        0     1895 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f4bb.png
--rw-r--r--   0        0        0     2409 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f4bc.png
--rw-r--r--   0        0        0     3178 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f527.png
--rw-r--r--   0        0        0     3350 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f52c.png
--rw-r--r--   0        0        0     3231 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f680.png
--rw-r--r--   0        0        0     3740 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f692.png
--rw-r--r--   0        0        0     2564 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f9af.png
--rw-r--r--   0        0        0     2081 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f9b0.png
--rw-r--r--   0        0        0     2301 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f9b1.png
--rw-r--r--   0        0        0     1717 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f9b2.png
--rw-r--r--   0        0        0     1968 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f9b3.png
--rw-r--r--   0        0        0     3029 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f9bc.png
--rw-r--r--   0        0        0     2477 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f9bd.png
--rw-r--r--   0        0        0     2561 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_2695_fe0f.png
--rw-r--r--   0        0        0     2680 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_2696_fe0f.png
--rw-r--r--   0        0        0     2660 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_2708_fe0f.png
--rw-r--r--   0        0        0     3289 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_2764_fe0f_200d_1f468.png
--rw-r--r--   0        0        0     2437 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_2764_fe0f_200d_1f48b_200d_1f468.png
--rw-r--r--   0        0        0     2497 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469.png
--rw-r--r--   0        0        0     4126 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f33e.png
--rw-r--r--   0        0        0     3312 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f373.png
--rw-r--r--   0        0        0     2951 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f37c.png
--rw-r--r--   0        0        0     2659 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f393.png
--rw-r--r--   0        0        0     3648 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f3a4.png
--rw-r--r--   0        0        0     3778 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f3a8.png
--rw-r--r--   0        0        0     2988 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f3eb.png
--rw-r--r--   0        0        0     3394 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f3ed.png
--rw-r--r--   0        0        0     2519 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f466.png
--rw-r--r--   0        0        0     2793 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f466_200d_1f466.png
--rw-r--r--   0        0        0     2718 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f467.png
--rw-r--r--   0        0        0     3700 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f467_200d_1f466.png
--rw-r--r--   0        0        0     3174 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f467_200d_1f467.png
--rw-r--r--   0        0        0     3363 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f466.png
--rw-r--r--   0        0        0     3984 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f466_200d_1f466.png
--rw-r--r--   0        0        0     3860 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f467.png
--rw-r--r--   0        0        0     4626 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f467_200d_1f466.png
--rw-r--r--   0        0        0     4582 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f467_200d_1f467.png
--rw-r--r--   0        0        0     2002 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f4bb.png
--rw-r--r--   0        0        0     2411 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f4bc.png
--rw-r--r--   0        0        0     3131 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f527.png
--rw-r--r--   0        0        0     3659 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f52c.png
--rw-r--r--   0        0        0     3150 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f680.png
--rw-r--r--   0        0        0     3773 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f692.png
--rw-r--r--   0        0        0     2532 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f9af.png
--rw-r--r--   0        0        0     2294 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f9b0.png
--rw-r--r--   0        0        0     2744 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f9b1.png
--rw-r--r--   0        0        0     1749 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f9b2.png
--rw-r--r--   0        0        0     2475 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f9b3.png
--rw-r--r--   0        0        0     3044 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f9bc.png
--rw-r--r--   0        0        0     2575 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f9bd.png
--rw-r--r--   0        0        0     2722 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_2695_fe0f.png
--rw-r--r--   0        0        0     2543 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_2696_fe0f.png
--rw-r--r--   0        0        0     2931 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_2708_fe0f.png
--rw-r--r--   0        0        0     3634 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f468.png
--rw-r--r--   0        0        0     3993 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f469.png
--rw-r--r--   0        0        0     2908 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f48b_200d_1f468.png
--rw-r--r--   0        0        0     2986 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f48b_200d_1f469.png
--rw-r--r--   0        0        0     3110 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f46a.png
--rw-r--r--   0        0        0     3563 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f46b.png
--rw-r--r--   0        0        0     3481 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f46c.png
--rw-r--r--   0        0        0     3729 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f46d.png
--rw-r--r--   0        0        0     3074 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f46e.png
--rw-r--r--   0        0        0     3026 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f46e_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3184 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f46e_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2773 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f46f.png
--rw-r--r--   0        0        0     3282 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f46f_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2849 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f46f_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2859 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f470.png
--rw-r--r--   0        0        0     2914 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f470_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2994 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f470_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2408 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f471.png
--rw-r--r--   0        0        0     2558 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f471_200d_2640_fe0f.png
--rw-r--r--   0        0        0     1962 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f471_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2225 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f472.png
--rw-r--r--   0        0        0     2279 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f473.png
--rw-r--r--   0        0        0     2127 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f473_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2497 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f473_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2160 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f474.png
--rw-r--r--   0        0        0     2445 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f475.png
--rw-r--r--   0        0        0     2198 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f476.png
--rw-r--r--   0        0        0     3221 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f477.png
--rw-r--r--   0        0        0     3455 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f477_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3157 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f477_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2492 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f478.png
--rw-r--r--   0        0        0     3442 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f479.png
--rw-r--r--   0        0        0     2863 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f47a.png
--rw-r--r--   0        0        0     2131 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f47b.png
--rw-r--r--   0        0        0     2657 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f47c.png
--rw-r--r--   0        0        0     1689 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f47d.png
--rw-r--r--   0        0        0     1189 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f47e.png
--rw-r--r--   0        0        0     2312 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f47f.png
--rw-r--r--   0        0        0     1705 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f480.png
--rw-r--r--   0        0        0     2539 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f481.png
--rw-r--r--   0        0        0     2759 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f481_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2232 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f481_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2667 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f482.png
--rw-r--r--   0        0        0     2451 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f482_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2572 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f482_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3554 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f483.png
--rw-r--r--   0        0        0     1511 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f484.png
--rw-r--r--   0        0        0     2498 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f485.png
--rw-r--r--   0        0        0     2577 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f486.png
--rw-r--r--   0        0        0     2578 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f486_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2291 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f486_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2902 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f487.png
--rw-r--r--   0        0        0     3136 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f487_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2768 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f487_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2127 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f488.png
--rw-r--r--   0        0        0     1689 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f489.png
--rw-r--r--   0        0        0     2073 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f48a.png
--rw-r--r--   0        0        0     2182 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f48b.png
--rw-r--r--   0        0        0     1041 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f48c.png
--rw-r--r--   0        0        0     2384 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f48d.png
--rw-r--r--   0        0        0     2358 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f48e.png
--rw-r--r--   0        0        0     2590 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f48f.png
--rw-r--r--   0        0        0    13813 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f490.png
--rw-r--r--   0        0        0     3493 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f491.png
--rw-r--r--   0        0        0     2163 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f492.png
--rw-r--r--   0        0        0     1344 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f493.png
--rw-r--r--   0        0        0     1561 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f494.png
--rw-r--r--   0        0        0     1153 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f495.png
--rw-r--r--   0        0        0     2111 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f496.png
--rw-r--r--   0        0        0     1760 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f497.png
--rw-r--r--   0        0        0     1985 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f498.png
--rw-r--r--   0        0        0     1130 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f499.png
--rw-r--r--   0        0        0     1209 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f49a.png
--rw-r--r--   0        0        0     1168 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f49b.png
--rw-r--r--   0        0        0     1112 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f49c.png
--rw-r--r--   0        0        0     2849 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f49d.png
--rw-r--r--   0        0        0     1678 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f49e.png
--rw-r--r--   0        0        0     1082 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f49f.png
--rw-r--r--   0        0        0     2790 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4a0.png
--rw-r--r--   0        0        0     1218 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4a1.png
--rw-r--r--   0        0        0     1301 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4a2.png
--rw-r--r--   0        0        0     2163 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4a3.png
--rw-r--r--   0        0        0      663 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4a4.png
--rw-r--r--   0        0        0     2101 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4a5.png
--rw-r--r--   0        0        0     1905 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4a6.png
--rw-r--r--   0        0        0     1268 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4a7.png
--rw-r--r--   0        0        0     1661 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4a8.png
--rw-r--r--   0        0        0     1782 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4a9.png
--rw-r--r--   0        0        0     1393 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4aa.png
--rw-r--r--   0        0        0     1890 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ab.png
--rw-r--r--   0        0        0     1244 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ac.png
--rw-r--r--   0        0        0     1370 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ad.png
--rw-r--r--   0        0        0     1790 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ae.png
--rw-r--r--   0        0        0     1447 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4af.png
--rw-r--r--   0        0        0     2079 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4b0.png
--rw-r--r--   0        0        0      996 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4b1.png
--rw-r--r--   0        0        0      731 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4b2.png
--rw-r--r--   0        0        0     1261 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4b3.png
--rw-r--r--   0        0        0     2017 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4b4.png
--rw-r--r--   0        0        0     2022 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4b5.png
--rw-r--r--   0        0        0     2210 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4b6.png
--rw-r--r--   0        0        0     1974 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4b7.png
--rw-r--r--   0        0        0     3067 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4b8.png
--rw-r--r--   0        0        0     1480 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4b9.png
--rw-r--r--   0        0        0     2448 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ba.png
--rw-r--r--   0        0        0     1176 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4bb.png
--rw-r--r--   0        0        0     1748 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4bc.png
--rw-r--r--   0        0        0     2198 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4bd.png
--rw-r--r--   0        0        0      907 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4be.png
--rw-r--r--   0        0        0     2244 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4bf.png
--rw-r--r--   0        0        0     2307 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4c0.png
--rw-r--r--   0        0        0     1335 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4c1.png
--rw-r--r--   0        0        0     1241 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4c2.png
--rw-r--r--   0        0        0     1241 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4c3.png
--rw-r--r--   0        0        0     1257 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4c4.png
--rw-r--r--   0        0        0     1046 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4c5.png
--rw-r--r--   0        0        0     1568 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4c6.png
--rw-r--r--   0        0        0     2054 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4c7.png
--rw-r--r--   0        0        0     1861 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4c8.png
--rw-r--r--   0        0        0     1762 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4c9.png
--rw-r--r--   0        0        0     1723 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ca.png
--rw-r--r--   0        0        0     1189 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4cb.png
--rw-r--r--   0        0        0     2156 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4cc.png
--rw-r--r--   0        0        0     1466 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4cd.png
--rw-r--r--   0        0        0     2382 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ce.png
--rw-r--r--   0        0        0      803 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4cf.png
--rw-r--r--   0        0        0      935 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4d0.png
--rw-r--r--   0        0        0     1723 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4d1.png
--rw-r--r--   0        0        0     2351 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4d2.png
--rw-r--r--   0        0        0     2386 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4d3.png
--rw-r--r--   0        0        0     1766 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4d4.png
--rw-r--r--   0        0        0     1593 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4d5.png
--rw-r--r--   0        0        0     2091 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4d6.png
--rw-r--r--   0        0        0     1470 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4d7.png
--rw-r--r--   0        0        0     1661 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4d8.png
--rw-r--r--   0        0        0     1807 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4d9.png
--rw-r--r--   0        0        0     2567 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4da.png
--rw-r--r--   0        0        0     1381 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4db.png
--rw-r--r--   0        0        0     2294 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4dc.png
--rw-r--r--   0        0        0     2169 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4dd.png
--rw-r--r--   0        0        0     1086 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4de.png
--rw-r--r--   0        0        0     1650 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4df.png
--rw-r--r--   0        0        0     1045 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4e0.png
--rw-r--r--   0        0        0     2446 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4e1.png
--rw-r--r--   0        0        0     1759 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4e2.png
--rw-r--r--   0        0        0     2230 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4e3.png
--rw-r--r--   0        0        0     1412 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4e4.png
--rw-r--r--   0        0        0     1396 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4e5.png
--rw-r--r--   0        0        0     1493 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4e6.png
--rw-r--r--   0        0        0     1113 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4e7.png
--rw-r--r--   0        0        0     1712 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4e8.png
--rw-r--r--   0        0        0     1223 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4e9.png
--rw-r--r--   0        0        0     1854 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ea.png
--rw-r--r--   0        0        0     2096 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4eb.png
--rw-r--r--   0        0        0     2146 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ec.png
--rw-r--r--   0        0        0     1703 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ed.png
--rw-r--r--   0        0        0     1507 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ee.png
--rw-r--r--   0        0        0     2827 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ef.png
--rw-r--r--   0        0        0     2109 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4f0.png
--rw-r--r--   0        0        0     1517 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4f1.png
--rw-r--r--   0        0        0     1869 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4f2.png
--rw-r--r--   0        0        0     1436 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4f3.png
--rw-r--r--   0        0        0     1432 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4f4.png
--rw-r--r--   0        0        0     1809 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4f5.png
--rw-r--r--   0        0        0     1014 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4f6.png
--rw-r--r--   0        0        0     1722 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4f7.png
--rw-r--r--   0        0        0     2671 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4f8.png
--rw-r--r--   0        0        0     1917 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4f9.png
--rw-r--r--   0        0        0     2416 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4fa.png
--rw-r--r--   0        0        0     1837 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4fb.png
--rw-r--r--   0        0        0     1155 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4fc.png
--rw-r--r--   0        0        0     2361 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4fd.png
--rw-r--r--   0        0        0     2542 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ff.png
--rw-r--r--   0        0        0     1165 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f500.png
--rw-r--r--   0        0        0     1196 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f501.png
--rw-r--r--   0        0        0     1260 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f502.png
--rw-r--r--   0        0        0     1258 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f503.png
--rw-r--r--   0        0        0     1313 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f504.png
--rw-r--r--   0        0        0     1209 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f505.png
--rw-r--r--   0        0        0     1611 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f506.png
--rw-r--r--   0        0        0     2099 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f507.png
--rw-r--r--   0        0        0     1884 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f508.png
--rw-r--r--   0        0        0     2513 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f509.png
--rw-r--r--   0        0        0     3375 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f50a.png
--rw-r--r--   0        0        0     2030 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f50b.png
--rw-r--r--   0        0        0     1447 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f50c.png
--rw-r--r--   0        0        0     1931 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f50d.png
--rw-r--r--   0        0        0     2090 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f50e.png
--rw-r--r--   0        0        0     2493 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f50f.png
--rw-r--r--   0        0        0     2190 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f510.png
--rw-r--r--   0        0        0     1672 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f511.png
--rw-r--r--   0        0        0     1356 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f512.png
--rw-r--r--   0        0        0     1472 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f513.png
--rw-r--r--   0        0        0     1922 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f514.png
--rw-r--r--   0        0        0     2107 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f515.png
--rw-r--r--   0        0        0     1450 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f516.png
--rw-r--r--   0        0        0     2545 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f517.png
--rw-r--r--   0        0        0     1393 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f518.png
--rw-r--r--   0        0        0     1003 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f519.png
--rw-r--r--   0        0        0      723 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f51a.png
--rw-r--r--   0        0        0      949 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f51b.png
--rw-r--r--   0        0        0     1086 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f51c.png
--rw-r--r--   0        0        0      731 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f51d.png
--rw-r--r--   0        0        0     2019 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f51e.png
--rw-r--r--   0        0        0     1156 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f51f.png
--rw-r--r--   0        0        0     1441 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f520.png
--rw-r--r--   0        0        0     1340 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f521.png
--rw-r--r--   0        0        0     1353 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f522.png
--rw-r--r--   0        0        0     1398 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f523.png
--rw-r--r--   0        0        0     1160 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f524.png
--rw-r--r--   0        0        0     2128 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f525.png
--rw-r--r--   0        0        0     1502 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f526.png
--rw-r--r--   0        0        0     1216 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f527.png
--rw-r--r--   0        0        0     1276 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f528.png
--rw-r--r--   0        0        0     1853 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f529.png
--rw-r--r--   0        0        0     1165 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f52a.png
--rw-r--r--   0        0        0     2371 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f52b.png
--rw-r--r--   0        0        0     2364 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f52c.png
--rw-r--r--   0        0        0     2039 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f52d.png
--rw-r--r--   0        0        0     3144 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f52e.png
--rw-r--r--   0        0        0     1358 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f52f.png
--rw-r--r--   0        0        0     1252 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f530.png
--rw-r--r--   0        0        0     2726 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f531.png
--rw-r--r--   0        0        0      733 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f532.png
--rw-r--r--   0        0        0      531 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f533.png
--rw-r--r--   0        0        0      961 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f534.png
--rw-r--r--   0        0        0      952 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f535.png
--rw-r--r--   0        0        0      780 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f536.png
--rw-r--r--   0        0        0      847 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f537.png
--rw-r--r--   0        0        0      668 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f538.png
--rw-r--r--   0        0        0      719 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f539.png
--rw-r--r--   0        0        0      566 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f53a.png
--rw-r--r--   0        0        0      654 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f53b.png
--rw-r--r--   0        0        0     1044 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f53c.png
--rw-r--r--   0        0        0      972 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f53d.png
--rw-r--r--   0        0        0     1553 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f549.png
--rw-r--r--   0        0        0     1919 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f54a.png
--rw-r--r--   0        0        0     1294 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f54b.png
--rw-r--r--   0        0        0     2786 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f54c.png
--rw-r--r--   0        0        0     2481 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f54d.png
--rw-r--r--   0        0        0     1663 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f54e.png
--rw-r--r--   0        0        0     1700 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f550.png
--rw-r--r--   0        0        0     1660 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f551.png
--rw-r--r--   0        0        0     1705 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f552.png
--rw-r--r--   0        0        0     1748 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f553.png
--rw-r--r--   0        0        0     1749 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f554.png
--rw-r--r--   0        0        0     1687 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f555.png
--rw-r--r--   0        0        0     1750 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f556.png
--rw-r--r--   0        0        0     1767 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f557.png
--rw-r--r--   0        0        0     1635 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f558.png
--rw-r--r--   0        0        0     1645 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f559.png
--rw-r--r--   0        0        0     1720 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f55a.png
--rw-r--r--   0        0        0     1669 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f55b.png
--rw-r--r--   0        0        0     1778 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f55c.png
--rw-r--r--   0        0        0     1707 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f55d.png
--rw-r--r--   0        0        0     1648 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f55e.png
--rw-r--r--   0        0        0     1689 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f55f.png
--rw-r--r--   0        0        0     1722 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f560.png
--rw-r--r--   0        0        0     1694 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f561.png
--rw-r--r--   0        0        0     1679 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f562.png
--rw-r--r--   0        0        0     1717 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f563.png
--rw-r--r--   0        0        0     1637 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f564.png
--rw-r--r--   0        0        0     1619 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f565.png
--rw-r--r--   0        0        0     1725 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f566.png
--rw-r--r--   0        0        0     1678 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f567.png
--rw-r--r--   0        0        0     2185 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f56f.png
--rw-r--r--   0        0        0     2228 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f570.png
--rw-r--r--   0        0        0      714 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f573.png
--rw-r--r--   0        0        0     1301 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f574.png
--rw-r--r--   0        0        0     3208 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f575.png
--rw-r--r--   0        0        0     3188 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f575_fe0f_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3174 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f575_fe0f_200d_2642_fe0f.png
--rw-r--r--   0        0        0      841 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f576.png
--rw-r--r--   0        0        0     1848 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f577.png
--rw-r--r--   0        0        0     2208 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f578.png
--rw-r--r--   0        0        0     1401 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f579.png
--rw-r--r--   0        0        0     2299 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f57a.png
--rw-r--r--   0        0        0     3424 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f587.png
--rw-r--r--   0        0        0     1232 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f58a.png
--rw-r--r--   0        0        0     1662 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f58b.png
--rw-r--r--   0        0        0     1928 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f58c.png
--rw-r--r--   0        0        0     1260 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f58d.png
--rw-r--r--   0        0        0     1529 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f590.png
--rw-r--r--   0        0        0      871 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f595.png
--rw-r--r--   0        0        0     1489 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f596.png
--rw-r--r--   0        0        0     1165 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5a4.png
--rw-r--r--   0        0        0      973 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5a5.png
--rw-r--r--   0        0        0     1403 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5a8.png
--rw-r--r--   0        0        0      761 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5b1.png
--rw-r--r--   0        0        0     1783 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5b2.png
--rw-r--r--   0        0        0     2515 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5bc.png
--rw-r--r--   0        0        0      831 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5c2.png
--rw-r--r--   0        0        0     1401 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5c3.png
--rw-r--r--   0        0        0     1035 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5c4.png
--rw-r--r--   0        0        0     4755 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5d1.png
--rw-r--r--   0        0        0     1897 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5d2.png
--rw-r--r--   0        0        0     2281 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5d3.png
--rw-r--r--   0        0        0     2007 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5dc.png
--rw-r--r--   0        0        0     1484 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5dd.png
--rw-r--r--   0        0        0     2030 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5de.png
--rw-r--r--   0        0        0     1129 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5e1.png
--rw-r--r--   0        0        0     1137 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5e3.png
--rw-r--r--   0        0        0      839 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5e8.png
--rw-r--r--   0        0        0     1569 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5ef.png
--rw-r--r--   0        0        0     1656 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5f3.png
--rw-r--r--   0        0        0     4392 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5fa.png
--rw-r--r--   0        0        0     1425 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5fb.png
--rw-r--r--   0        0        0     2590 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5fc.png
--rw-r--r--   0        0        0     2201 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5fd.png
--rw-r--r--   0        0        0     1010 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5fe.png
--rw-r--r--   0        0        0     1759 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f5ff.png
--rw-r--r--   0        0        0     2044 2022-11-18 15:36:28.336582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f600.png
--rw-r--r--   0        0        0     2219 2022-11-18 15:36:28.336582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f601.png
--rw-r--r--   0        0        0     2808 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f602.png
--rw-r--r--   0        0        0     2198 2022-11-18 15:36:28.336582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f603.png
--rw-r--r--   0        0        0     2129 2022-11-18 15:36:28.336582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f604.png
--rw-r--r--   0        0        0     2690 2022-11-18 15:36:28.336582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f605.png
--rw-r--r--   0        0        0     2241 2022-11-18 15:36:28.336582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f606.png
--rw-r--r--   0        0        0     3349 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f607.png
--rw-r--r--   0        0        0     2347 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f608.png
--rw-r--r--   0        0        0     1949 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f609.png
--rw-r--r--   0        0        0     1964 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f60a.png
--rw-r--r--   0        0        0     2305 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f60b.png
--rw-r--r--   0        0        0     1922 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f60c.png
--rw-r--r--   0        0        0     2417 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f60d.png
--rw-r--r--   0        0        0     2129 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f60e.png
--rw-r--r--   0        0        0     1855 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f60f.png
--rw-r--r--   0        0        0     1777 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f610.png
--rw-r--r--   0        0        0     1645 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f611.png
--rw-r--r--   0        0        0     1865 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f612.png
--rw-r--r--   0        0        0     2480 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f613.png
--rw-r--r--   0        0        0     1794 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f614.png
--rw-r--r--   0        0        0     1847 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f615.png
--rw-r--r--   0        0        0     1950 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f616.png
--rw-r--r--   0        0        0     1878 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f617.png
--rw-r--r--   0        0        0     2543 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f618.png
--rw-r--r--   0        0        0     2010 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f619.png
--rw-r--r--   0        0        0     2040 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f61a.png
--rw-r--r--   0        0        0     2093 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f61b.png
--rw-r--r--   0        0        0     2563 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f61c.png
--rw-r--r--   0        0        0     2292 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f61d.png
--rw-r--r--   0        0        0     1764 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f61e.png
--rw-r--r--   0        0        0     1962 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f61f.png
--rw-r--r--   0        0        0     1809 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f620.png
--rw-r--r--   0        0        0     1398 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f621.png
--rw-r--r--   0        0        0     2477 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f622.png
--rw-r--r--   0        0        0     1947 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f623.png
--rw-r--r--   0        0        0     3109 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f624.png
--rw-r--r--   0        0        0     2491 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f625.png
--rw-r--r--   0        0        0     1691 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f626.png
--rw-r--r--   0        0        0     1967 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f627.png
--rw-r--r--   0        0        0     2236 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f628.png
--rw-r--r--   0        0        0     2300 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f629.png
--rw-r--r--   0        0        0     2659 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f62a.png
--rw-r--r--   0        0        0     2376 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f62b.png
--rw-r--r--   0        0        0     1959 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f62c.png
--rw-r--r--   0        0        0     2464 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f62d.png
--rw-r--r--   0        0        0     1681 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f62e.png
--rw-r--r--   0        0        0     3413 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f62e_200d_1f4a8.png
--rw-r--r--   0        0        0     1895 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f62f.png
--rw-r--r--   0        0        0     2915 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f630.png
--rw-r--r--   0        0        0     2986 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f631.png
--rw-r--r--   0        0        0     2122 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f632.png
--rw-r--r--   0        0        0     2367 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f633.png
--rw-r--r--   0        0        0     2695 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f634.png
--rw-r--r--   0        0        0     2059 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f635.png
--rw-r--r--   0        0        0     3751 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f635_200d_1f4ab.png
--rw-r--r--   0        0        0     1711 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f636.png
--rw-r--r--   0        0        0     4477 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f636_200d_1f32b_fe0f.png
--rw-r--r--   0        0        0     2431 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f637.png
--rw-r--r--   0        0        0     2358 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f638.png
--rw-r--r--   0        0        0     3507 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f639.png
--rw-r--r--   0        0        0     2628 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f63a.png
--rw-r--r--   0        0        0     2917 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f63b.png
--rw-r--r--   0        0        0     2509 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f63c.png
--rw-r--r--   0        0        0     2625 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f63d.png
--rw-r--r--   0        0        0     2423 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f63e.png
--rw-r--r--   0        0        0     2830 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f63f.png
--rw-r--r--   0        0        0     3113 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f640.png
--rw-r--r--   0        0        0     1784 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f641.png
--rw-r--r--   0        0        0     1841 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f642.png
--rw-r--r--   0        0        0     1804 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f643.png
--rw-r--r--   0        0        0     2149 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f644.png
--rw-r--r--   0        0        0     2762 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f645.png
--rw-r--r--   0        0        0     2860 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f645_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3058 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f645_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3132 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f646.png
--rw-r--r--   0        0        0     3051 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f646_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3260 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f646_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2497 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f647.png
--rw-r--r--   0        0        0     2862 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f647_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2829 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f647_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2542 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f648.png
--rw-r--r--   0        0        0     2640 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f649.png
--rw-r--r--   0        0        0     2350 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f64a.png
--rw-r--r--   0        0        0     2576 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f64b.png
--rw-r--r--   0        0        0     2762 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f64b_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2406 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f64b_200d_2642_fe0f.png
--rw-r--r--   0        0        0     1918 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f64c.png
--rw-r--r--   0        0        0     2133 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f64d.png
--rw-r--r--   0        0        0     2384 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f64d_200d_2640_fe0f.png
--rw-r--r--   0        0        0     1984 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f64d_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2123 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f64e.png
--rw-r--r--   0        0        0     2383 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f64e_200d_2640_fe0f.png
--rw-r--r--   0        0        0     1936 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f64e_200d_2642_fe0f.png
--rw-r--r--   0        0        0     1910 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f64f.png
--rw-r--r--   0        0        0     3216 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f680.png
--rw-r--r--   0        0        0     3045 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f681.png
--rw-r--r--   0        0        0     3402 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f682.png
--rw-r--r--   0        0        0     2144 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f683.png
--rw-r--r--   0        0        0     2088 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f684.png
--rw-r--r--   0        0        0     2044 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f685.png
--rw-r--r--   0        0        0     2384 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f686.png
--rw-r--r--   0        0        0     2168 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f687.png
--rw-r--r--   0        0        0     1819 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f688.png
--rw-r--r--   0        0        0     2106 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f689.png
--rw-r--r--   0        0        0     1964 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f68a.png
--rw-r--r--   0        0        0     1812 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f68b.png
--rw-r--r--   0        0        0     2469 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f68c.png
--rw-r--r--   0        0        0     2164 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f68d.png
--rw-r--r--   0        0        0     3075 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f68e.png
--rw-r--r--   0        0        0     1852 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f68f.png
--rw-r--r--   0        0        0     2315 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f690.png
--rw-r--r--   0        0        0     2769 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f691.png
--rw-r--r--   0        0        0     2906 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f692.png
--rw-r--r--   0        0        0     2109 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f693.png
--rw-r--r--   0        0        0     2206 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f694.png
--rw-r--r--   0        0        0     3166 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f695.png
--rw-r--r--   0        0        0     2435 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f696.png
--rw-r--r--   0        0        0     2501 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f697.png
--rw-r--r--   0        0        0     2412 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f698.png
--rw-r--r--   0        0        0     2429 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f699.png
--rw-r--r--   0        0        0     2291 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f69a.png
--rw-r--r--   0        0        0     2309 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f69b.png
--rw-r--r--   0        0        0     2980 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f69c.png
--rw-r--r--   0        0        0     1988 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f69d.png
--rw-r--r--   0        0        0     3138 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f69e.png
--rw-r--r--   0        0        0     2456 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f69f.png
--rw-r--r--   0        0        0     2526 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a0.png
--rw-r--r--   0        0        0     1735 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a1.png
--rw-r--r--   0        0        0     2413 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a2.png
--rw-r--r--   0        0        0     1966 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a3.png
--rw-r--r--   0        0        0     2262 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a3_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2156 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a3_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2041 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a4.png
--rw-r--r--   0        0        0     1795 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a5.png
--rw-r--r--   0        0        0     2019 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a6.png
--rw-r--r--   0        0        0     2554 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a7.png
--rw-r--r--   0        0        0     2975 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a8.png
--rw-r--r--   0        0        0      917 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a9.png
--rw-r--r--   0        0        0      951 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6aa.png
--rw-r--r--   0        0        0     2250 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6ab.png
--rw-r--r--   0        0        0     1543 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6ac.png
--rw-r--r--   0        0        0     1875 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6ad.png
--rw-r--r--   0        0        0     1258 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6ae.png
--rw-r--r--   0        0        0     1929 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6af.png
--rw-r--r--   0        0        0     2641 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b0.png
--rw-r--r--   0        0        0     1950 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b1.png
--rw-r--r--   0        0        0     2702 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b2.png
--rw-r--r--   0        0        0     2181 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b3.png
--rw-r--r--   0        0        0     3994 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b4.png
--rw-r--r--   0        0        0     3960 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b4_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3931 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b4_200d_2642_fe0f.png
--rw-r--r--   0        0        0     4126 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b5.png
--rw-r--r--   0        0        0     4684 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b5_200d_2640_fe0f.png
--rw-r--r--   0        0        0     4495 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b5_200d_2642_fe0f.png
--rw-r--r--   0        0        0     1893 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b6.png
--rw-r--r--   0        0        0     2212 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b6_200d_2640_fe0f.png
--rw-r--r--   0        0        0     1986 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b6_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2018 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b7.png
--rw-r--r--   0        0        0     1190 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b8.png
--rw-r--r--   0        0        0     1142 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b9.png
--rw-r--r--   0        0        0     1170 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6ba.png
--rw-r--r--   0        0        0     1251 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6bb.png
--rw-r--r--   0        0        0     1188 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6bc.png
--rw-r--r--   0        0        0     1173 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6bd.png
--rw-r--r--   0        0        0     1457 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6be.png
--rw-r--r--   0        0        0     2007 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6bf.png
--rw-r--r--   0        0        0     2399 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6c0.png
--rw-r--r--   0        0        0     2784 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6c1.png
--rw-r--r--   0        0        0     1350 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6c2.png
--rw-r--r--   0        0        0     1244 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6c3.png
--rw-r--r--   0        0        0     1089 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6c4.png
--rw-r--r--   0        0        0     1292 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6c5.png
--rw-r--r--   0        0        0     1881 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6cb.png
--rw-r--r--   0        0        0     1564 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6cc.png
--rw-r--r--   0        0        0     4037 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6cd.png
--rw-r--r--   0        0        0     2362 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6ce.png
--rw-r--r--   0        0        0     1192 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6cf.png
--rw-r--r--   0        0        0     1220 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6d0.png
--rw-r--r--   0        0        0      875 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6d1.png
--rw-r--r--   0        0        0     2699 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6d2.png
--rw-r--r--   0        0        0     1632 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6d5.png
--rw-r--r--   0        0        0     1632 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6d6.png
--rw-r--r--   0        0        0     1243 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6d7.png
--rw-r--r--   0        0        0     8111 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6dd.png
--rw-r--r--   0        0        0     4305 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6de.png
--rw-r--r--   0        0        0     3886 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6df.png
--rw-r--r--   0        0        0     2317 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6e0.png
--rw-r--r--   0        0        0     1601 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6e1.png
--rw-r--r--   0        0        0     2017 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6e2.png
--rw-r--r--   0        0        0     2352 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6e3.png
--rw-r--r--   0        0        0     3595 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6e4.png
--rw-r--r--   0        0        0     2267 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6e5.png
--rw-r--r--   0        0        0     2443 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6e9.png
--rw-r--r--   0        0        0     1908 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6eb.png
--rw-r--r--   0        0        0     2282 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6ec.png
--rw-r--r--   0        0        0     3617 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6f0.png
--rw-r--r--   0        0        0     2329 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6f3.png
--rw-r--r--   0        0        0     1741 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6f4.png
--rw-r--r--   0        0        0     3308 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6f5.png
--rw-r--r--   0        0        0     1926 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6f6.png
--rw-r--r--   0        0        0     2647 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6f7.png
--rw-r--r--   0        0        0     1416 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6f8.png
--rw-r--r--   0        0        0     1452 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6f9.png
--rw-r--r--   0        0        0     3549 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6fa.png
--rw-r--r--   0        0        0     1981 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6fb.png
--rw-r--r--   0        0        0     3566 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f6fc.png
--rw-r--r--   0        0        0      911 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f7e0.png
--rw-r--r--   0        0        0      949 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f7e1.png
--rw-r--r--   0        0        0      857 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f7e2.png
--rw-r--r--   0        0        0      959 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f7e3.png
--rw-r--r--   0        0        0     1016 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f7e4.png
--rw-r--r--   0        0        0      630 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f7e5.png
--rw-r--r--   0        0        0      544 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f7e6.png
--rw-r--r--   0        0        0      486 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f7e7.png
--rw-r--r--   0        0        0      695 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f7e8.png
--rw-r--r--   0        0        0      568 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f7e9.png
--rw-r--r--   0        0        0      537 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f7ea.png
--rw-r--r--   0        0        0      534 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f7eb.png
--rw-r--r--   0        0        0      335 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f7f0.png
--rw-r--r--   0        0        0     1468 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f90c.png
--rw-r--r--   0        0        0      959 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f90d.png
--rw-r--r--   0        0        0     1168 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f90e.png
--rw-r--r--   0        0        0     1031 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f90f.png
--rw-r--r--   0        0        0     2728 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f910.png
--rw-r--r--   0        0        0     2691 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f911.png
--rw-r--r--   0        0        0     2684 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f912.png
--rw-r--r--   0        0        0     2539 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f913.png
--rw-r--r--   0        0        0     2157 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f914.png
--rw-r--r--   0        0        0     2019 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f915.png
--rw-r--r--   0        0        0     2767 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f916.png
--rw-r--r--   0        0        0     2530 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f917.png
--rw-r--r--   0        0        0     1300 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f918.png
--rw-r--r--   0        0        0     1397 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f919.png
--rw-r--r--   0        0        0     1383 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f91a.png
--rw-r--r--   0        0        0     1239 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f91b.png
--rw-r--r--   0        0        0     1276 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f91c.png
--rw-r--r--   0        0        0     1399 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f91d.png
--rw-r--r--   0        0        0     1371 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f91e.png
--rw-r--r--   0        0        0     1250 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f91f.png
--rw-r--r--   0        0        0     2550 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f920.png
--rw-r--r--   0        0        0     3526 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f921.png
--rw-r--r--   0        0        0     1684 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f922.png
--rw-r--r--   0        0        0     2752 2022-11-18 15:36:28.336582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f923.png
--rw-r--r--   0        0        0     2405 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f924.png
--rw-r--r--   0        0        0     2241 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f925.png
--rw-r--r--   0        0        0     2211 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f926.png
--rw-r--r--   0        0        0     2487 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f926_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2222 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f926_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2604 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f927.png
--rw-r--r--   0        0        0     1957 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f928.png
--rw-r--r--   0        0        0     3007 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f929.png
--rw-r--r--   0        0        0     2941 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f92a.png
--rw-r--r--   0        0        0     2316 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f92b.png
--rw-r--r--   0        0        0     2135 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f92c.png
--rw-r--r--   0        0        0     2253 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f92d.png
--rw-r--r--   0        0        0     3481 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f92e.png
--rw-r--r--   0        0        0     3562 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f92f.png
--rw-r--r--   0        0        0     2250 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f930.png
--rw-r--r--   0        0        0     2852 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f931.png
--rw-r--r--   0        0        0     1656 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f932.png
--rw-r--r--   0        0        0     1585 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f933.png
--rw-r--r--   0        0        0     3154 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f934.png
--rw-r--r--   0        0        0     2265 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f935.png
--rw-r--r--   0        0        0     2536 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f935_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2112 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f935_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2791 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f936.png
--rw-r--r--   0        0        0     2649 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f937.png
--rw-r--r--   0        0        0     2917 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f937_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2398 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f937_200d_2642_fe0f.png
--rw-r--r--   0        0        0     1942 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f938.png
--rw-r--r--   0        0        0     2235 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f938_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2155 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f938_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3423 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f939.png
--rw-r--r--   0        0        0     3506 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f939_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3465 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f939_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2695 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f93a.png
--rw-r--r--   0        0        0     3981 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f93c.png
--rw-r--r--   0        0        0     3878 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f93c_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3927 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f93c_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3013 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f93d.png
--rw-r--r--   0        0        0     3287 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f93d_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2618 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f93d_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2954 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f93e.png
--rw-r--r--   0        0        0     3042 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f93e_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3126 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f93e_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2827 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f93f.png
--rw-r--r--   0        0        0     2393 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f940.png
--rw-r--r--   0        0        0     2710 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f941.png
--rw-r--r--   0        0        0     2319 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f942.png
--rw-r--r--   0        0        0     2060 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f943.png
--rw-r--r--   0        0        0     1133 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f944.png
--rw-r--r--   0        0        0     2674 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f945.png
--rw-r--r--   0        0        0     2078 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f947.png
--rw-r--r--   0        0        0     1808 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f948.png
--rw-r--r--   0        0        0     2087 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f949.png
--rw-r--r--   0        0        0     2046 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f94a.png
--rw-r--r--   0        0        0     2194 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f94b.png
--rw-r--r--   0        0        0     2270 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f94c.png
--rw-r--r--   0        0        0     2214 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f94d.png
--rw-r--r--   0        0        0     2622 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f94e.png
--rw-r--r--   0        0        0     1705 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f94f.png
--rw-r--r--   0        0        0     2311 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f950.png
--rw-r--r--   0        0        0     2485 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f951.png
--rw-r--r--   0        0        0     2890 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f952.png
--rw-r--r--   0        0        0     2832 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f953.png
--rw-r--r--   0        0        0     1741 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f954.png
--rw-r--r--   0        0        0     2090 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f955.png
--rw-r--r--   0        0        0     1414 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f956.png
--rw-r--r--   0        0        0     4262 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f957.png
--rw-r--r--   0        0        0     3316 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f958.png
--rw-r--r--   0        0        0     2853 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f959.png
--rw-r--r--   0        0        0     1015 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f95a.png
--rw-r--r--   0        0        0     1727 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f95b.png
--rw-r--r--   0        0        0     3624 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f95c.png
--rw-r--r--   0        0        0     2337 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f95d.png
--rw-r--r--   0        0        0     2837 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f95e.png
--rw-r--r--   0        0        0     2009 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f95f.png
--rw-r--r--   0        0        0     1509 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f960.png
--rw-r--r--   0        0        0     1724 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f961.png
--rw-r--r--   0        0        0     1278 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f962.png
--rw-r--r--   0        0        0     1504 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f963.png
--rw-r--r--   0        0        0     1548 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f964.png
--rw-r--r--   0        0        0     2092 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f965.png
--rw-r--r--   0        0        0     2813 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f966.png
--rw-r--r--   0        0        0     2219 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f967.png
--rw-r--r--   0        0        0     2790 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f968.png
--rw-r--r--   0        0        0     2651 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f969.png
--rw-r--r--   0        0        0     2666 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f96a.png
--rw-r--r--   0        0        0     1859 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f96b.png
--rw-r--r--   0        0        0     3117 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f96c.png
--rw-r--r--   0        0        0     2602 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f96d.png
--rw-r--r--   0        0        0     2615 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f96e.png
--rw-r--r--   0        0        0     3023 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f96f.png
--rw-r--r--   0        0        0     2696 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f970.png
--rw-r--r--   0        0        0     2412 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f971.png
--rw-r--r--   0        0        0     2349 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f972.png
--rw-r--r--   0        0        0     3929 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f973.png
--rw-r--r--   0        0        0     2106 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f974.png
--rw-r--r--   0        0        0     2491 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f975.png
--rw-r--r--   0        0        0     2947 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f976.png
--rw-r--r--   0        0        0     2065 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f977.png
--rw-r--r--   0        0        0     2697 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f978.png
--rw-r--r--   0        0        0     3326 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f979.png
--rw-r--r--   0        0        0     2404 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f97a.png
--rw-r--r--   0        0        0     1975 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f97b.png
--rw-r--r--   0        0        0     1541 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f97c.png
--rw-r--r--   0        0        0     2260 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f97d.png
--rw-r--r--   0        0        0     2291 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f97e.png
--rw-r--r--   0        0        0      996 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f97f.png
--rw-r--r--   0        0        0     3907 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f980.png
--rw-r--r--   0        0        0     3404 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f981.png
--rw-r--r--   0        0        0     2013 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f982.png
--rw-r--r--   0        0        0     3489 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f983.png
--rw-r--r--   0        0        0     3552 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f984.png
--rw-r--r--   0        0        0     2600 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f985.png
--rw-r--r--   0        0        0     2282 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f986.png
--rw-r--r--   0        0        0     1855 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f987.png
--rw-r--r--   0        0        0     2029 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f988.png
--rw-r--r--   0        0        0     2574 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f989.png
--rw-r--r--   0        0        0     2522 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f98a.png
--rw-r--r--   0        0        0     2937 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f98b.png
--rw-r--r--   0        0        0     2432 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f98c.png
--rw-r--r--   0        0        0     1950 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f98d.png
--rw-r--r--   0        0        0     3110 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f98e.png
--rw-r--r--   0        0        0     1713 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f98f.png
--rw-r--r--   0        0        0     4212 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f990.png
--rw-r--r--   0        0        0     4058 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f991.png
--rw-r--r--   0        0        0     2540 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f992.png
--rw-r--r--   0        0        0     2060 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f993.png
--rw-r--r--   0        0        0     2587 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f994.png
--rw-r--r--   0        0        0     1802 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f995.png
--rw-r--r--   0        0        0     2149 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f996.png
--rw-r--r--   0        0        0     2046 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f997.png
--rw-r--r--   0        0        0     1932 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f998.png
--rw-r--r--   0        0        0     1793 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f999.png
--rw-r--r--   0        0        0     4253 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f99a.png
--rw-r--r--   0        0        0     1338 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f99b.png
--rw-r--r--   0        0        0     2652 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f99c.png
--rw-r--r--   0        0        0     1442 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f99d.png
--rw-r--r--   0        0        0     3170 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f99e.png
--rw-r--r--   0        0        0     3035 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f99f.png
--rw-r--r--   0        0        0     3160 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9a0.png
--rw-r--r--   0        0        0     1386 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9a1.png
--rw-r--r--   0        0        0     1745 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9a2.png
--rw-r--r--   0        0        0     1946 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9a3.png
--rw-r--r--   0        0        0     2772 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9a4.png
--rw-r--r--   0        0        0     2641 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9a5.png
--rw-r--r--   0        0        0     2185 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9a6.png
--rw-r--r--   0        0        0     2603 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9a7.png
--rw-r--r--   0        0        0     1870 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9a8.png
--rw-r--r--   0        0        0     1782 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9a9.png
--rw-r--r--   0        0        0     1986 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9aa.png
--rw-r--r--   0        0        0     1721 2022-11-18 15:36:28.372583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ab.png
--rw-r--r--   0        0        0     1659 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ac.png
--rw-r--r--   0        0        0     1328 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ad.png
--rw-r--r--   0        0        0     3191 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ae.png
--rw-r--r--   0        0        0      801 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9af.png
--rw-r--r--   0        0        0     1127 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b0.png
--rw-r--r--   0        0        0     1559 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b1.png
--rw-r--r--   0        0        0      833 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b2.png
--rw-r--r--   0        0        0     1131 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b3.png
--rw-r--r--   0        0        0     1101 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b4.png
--rw-r--r--   0        0        0      921 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b5.png
--rw-r--r--   0        0        0     1240 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b6.png
--rw-r--r--   0        0        0     1290 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b7.png
--rw-r--r--   0        0        0     3429 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b8.png
--rw-r--r--   0        0        0     3693 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b8_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3512 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b8_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3996 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b9.png
--rw-r--r--   0        0        0     4529 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b9_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3957 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b9_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2908 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ba.png
--rw-r--r--   0        0        0     1819 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9bb.png
--rw-r--r--   0        0        0     1750 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9bc.png
--rw-r--r--   0        0        0     1499 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9bd.png
--rw-r--r--   0        0        0     1854 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9be.png
--rw-r--r--   0        0        0     1429 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9bf.png
--rw-r--r--   0        0        0     1368 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9c0.png
--rw-r--r--   0        0        0     3498 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9c1.png
--rw-r--r--   0        0        0     1692 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9c2.png
--rw-r--r--   0        0        0     1825 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9c3.png
--rw-r--r--   0        0        0     1754 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9c4.png
--rw-r--r--   0        0        0     2237 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9c5.png
--rw-r--r--   0        0        0     2313 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9c6.png
--rw-r--r--   0        0        0     1936 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9c7.png
--rw-r--r--   0        0        0     1223 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9c8.png
--rw-r--r--   0        0        0     1859 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9c9.png
--rw-r--r--   0        0        0     2521 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ca.png
--rw-r--r--   0        0        0     2091 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9cb.png
--rw-r--r--   0        0        0     3993 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9cc.png
--rw-r--r--   0        0        0     1802 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9cd.png
--rw-r--r--   0        0        0     2194 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9cd_200d_2640_fe0f.png
--rw-r--r--   0        0        0     1803 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9cd_200d_2642_fe0f.png
--rw-r--r--   0        0        0     1355 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ce.png
--rw-r--r--   0        0        0     1672 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ce_200d_2640_fe0f.png
--rw-r--r--   0        0        0     1371 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ce_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2635 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9cf.png
--rw-r--r--   0        0        0     2699 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9cf_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2712 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9cf_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2484 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d0.png
--rw-r--r--   0        0        0     2148 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1.png
--rw-r--r--   0        0        0     4085 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f33e.png
--rw-r--r--   0        0        0     3096 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f373.png
--rw-r--r--   0        0        0     2947 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f37c.png
--rw-r--r--   0        0        0     3304 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f384.png
--rw-r--r--   0        0        0     2602 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f393.png
--rw-r--r--   0        0        0     3162 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3a4.png
--rw-r--r--   0        0        0     3507 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3a8.png
--rw-r--r--   0        0        0     2985 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3eb.png
--rw-r--r--   0        0        0     3277 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3ed.png
--rw-r--r--   0        0        0     1983 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f4bb.png
--rw-r--r--   0        0        0     2284 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f4bc.png
--rw-r--r--   0        0        0     3264 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f527.png
--rw-r--r--   0        0        0     3470 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f52c.png
--rw-r--r--   0        0        0     3285 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f680.png
--rw-r--r--   0        0        0     3739 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f692.png
--rw-r--r--   0        0        0     3138 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f91d_200d_1f9d1.png
--rw-r--r--   0        0        0     2547 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9af.png
--rw-r--r--   0        0        0     2030 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b0.png
--rw-r--r--   0        0        0     2393 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b1.png
--rw-r--r--   0        0        0     1800 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b2.png
--rw-r--r--   0        0        0     2200 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b3.png
--rw-r--r--   0        0        0     2927 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9bc.png
--rw-r--r--   0        0        0     2244 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9bd.png
--rw-r--r--   0        0        0     2529 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_2695_fe0f.png
--rw-r--r--   0        0        0     2671 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_2696_fe0f.png
--rw-r--r--   0        0        0     2718 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_2708_fe0f.png
--rw-r--r--   0        0        0     2366 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d2.png
--rw-r--r--   0        0        0     2801 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d3.png
--rw-r--r--   0        0        0     2178 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d4.png
--rw-r--r--   0        0        0     4333 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d4_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3689 2022-11-18 15:36:28.352583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d4_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2258 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d5.png
--rw-r--r--   0        0        0     3176 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d6.png
--rw-r--r--   0        0        0     3180 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d6_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3220 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d6_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3412 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d7.png
--rw-r--r--   0        0        0     3963 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d7_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3608 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d7_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2201 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d8.png
--rw-r--r--   0        0        0     2189 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d8_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2314 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d8_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3401 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d9.png
--rw-r--r--   0        0        0     3318 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d9_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3327 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d9_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2627 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9da.png
--rw-r--r--   0        0        0     3146 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9da_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2586 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9da_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2949 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9db.png
--rw-r--r--   0        0        0     3078 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9db_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3077 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9db_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3533 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9dc.png
--rw-r--r--   0        0        0     3786 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9dc_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3488 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9dc_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3089 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9dd.png
--rw-r--r--   0        0        0     3289 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9dd_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3449 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9dd_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2735 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9de.png
--rw-r--r--   0        0        0     2996 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9de_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2841 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9de_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2737 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9df.png
--rw-r--r--   0        0        0     2739 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9df_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2760 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9df_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2467 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9e0.png
--rw-r--r--   0        0        0     1175 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9e1.png
--rw-r--r--   0        0        0     1084 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9e2.png
--rw-r--r--   0        0        0     1803 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9e3.png
--rw-r--r--   0        0        0     1581 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9e4.png
--rw-r--r--   0        0        0     1812 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9e5.png
--rw-r--r--   0        0        0     1914 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9e6.png
--rw-r--r--   0        0        0     1351 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9e7.png
--rw-r--r--   0        0        0     2523 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9e8.png
--rw-r--r--   0        0        0     1911 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9e9.png
--rw-r--r--   0        0        0     2524 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ea.png
--rw-r--r--   0        0        0     1718 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9eb.png
--rw-r--r--   0        0        0     3148 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ec.png
--rw-r--r--   0        0        0     2612 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ed.png
--rw-r--r--   0        0        0     3580 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ee.png
--rw-r--r--   0        0        0     3068 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ef.png
--rw-r--r--   0        0        0     1488 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9f0.png
--rw-r--r--   0        0        0     1688 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9f1.png
--rw-r--r--   0        0        0     1816 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9f2.png
--rw-r--r--   0        0        0     2325 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9f3.png
--rw-r--r--   0        0        0     1117 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9f4.png
--rw-r--r--   0        0        0     2571 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9f5.png
--rw-r--r--   0        0        0     2874 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9f6.png
--rw-r--r--   0        0        0     1924 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9f7.png
--rw-r--r--   0        0        0     2489 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9f8.png
--rw-r--r--   0        0        0     1047 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9f9.png
--rw-r--r--   0        0        0     2773 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9fa.png
--rw-r--r--   0        0        0     1623 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9fb.png
--rw-r--r--   0        0        0     2401 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9fc.png
--rw-r--r--   0        0        0     2080 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9fd.png
--rw-r--r--   0        0        0     1461 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9fe.png
--rw-r--r--   0        0        0     2710 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ff.png
--rw-r--r--   0        0        0     2121 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa70.png
--rw-r--r--   0        0        0     1499 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa71.png
--rw-r--r--   0        0        0     1002 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa72.png
--rw-r--r--   0        0        0     2386 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa73.png
--rw-r--r--   0        0        0     1526 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa74.png
--rw-r--r--   0        0        0     1146 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa78.png
--rw-r--r--   0        0        0     1312 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa79.png
--rw-r--r--   0        0        0     1968 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa7a.png
--rw-r--r--   0        0        0     4290 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa7b.png
--rw-r--r--   0        0        0     2091 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa7c.png
--rw-r--r--   0        0        0     2378 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa80.png
--rw-r--r--   0        0        0     1942 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa81.png
--rw-r--r--   0        0        0     3182 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa82.png
--rw-r--r--   0        0        0     1651 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa83.png
--rw-r--r--   0        0        0     1076 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa84.png
--rw-r--r--   0        0        0     9582 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa85.png
--rw-r--r--   0        0        0     3331 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa86.png
--rw-r--r--   0        0        0     2815 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa90.png
--rw-r--r--   0        0        0     1145 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa91.png
--rw-r--r--   0        0        0     1548 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa92.png
--rw-r--r--   0        0        0     1251 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa93.png
--rw-r--r--   0        0        0     2078 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa94.png
--rw-r--r--   0        0        0     1644 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa95.png
--rw-r--r--   0        0        0     1803 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa96.png
--rw-r--r--   0        0        0     2194 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa97.png
--rw-r--r--   0        0        0     1906 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa98.png
--rw-r--r--   0        0        0     2641 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa99.png
--rw-r--r--   0        0        0     1455 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa9a.png
--rw-r--r--   0        0        0     1387 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa9b.png
--rw-r--r--   0        0        0     2654 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa9c.png
--rw-r--r--   0        0        0     1534 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa9d.png
--rw-r--r--   0        0        0     1070 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa9e.png
--rw-r--r--   0        0        0      844 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fa9f.png
--rw-r--r--   0        0        0     1214 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1faa0.png
--rw-r--r--   0        0        0     1646 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1faa1.png
--rw-r--r--   0        0        0     3421 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1faa2.png
--rw-r--r--   0        0        0     2517 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1faa3.png
--rw-r--r--   0        0        0     2137 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/1faa4.png
--rw-r--r--   0        0        0     1078 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1faa5.png
--rw-r--r--   0        0        0     1357 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1faa6.png
--rw-r--r--   0        0        0      739 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1faa7.png
--rw-r--r--   0        0        0     1398 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1faa8.png
--rw-r--r--   0        0        0     4069 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/1faa9.png
--rw-r--r--   0        0        0     3116 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1faaa.png
--rw-r--r--   0        0        0     2959 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/1faab.png
--rw-r--r--   0        0        0     3385 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1faac.png
--rw-r--r--   0        0        0     3390 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fab0.png
--rw-r--r--   0        0        0     2544 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fab1.png
--rw-r--r--   0        0        0     2712 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fab2.png
--rw-r--r--   0        0        0     2220 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fab3.png
--rw-r--r--   0        0        0     2337 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fab4.png
--rw-r--r--   0        0        0     1796 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fab5.png
--rw-r--r--   0        0        0     1694 2022-11-18 15:36:28.376583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fab6.png
--rw-r--r--   0        0        0     3028 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fab7.png
--rw-r--r--   0        0        0     8701 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fab8.png
--rw-r--r--   0        0        0     3220 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fab9.png
--rw-r--r--   0        0        0     3143 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1faba.png
--rw-r--r--   0        0        0     3145 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1fac0.png
--rw-r--r--   0        0        0     2355 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1fac1.png
--rw-r--r--   0        0        0     1207 2022-11-18 15:36:28.368583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fac2.png
--rw-r--r--   0        0        0     2880 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fac3.png
--rw-r--r--   0        0        0     2915 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fac4.png
--rw-r--r--   0        0        0     3239 2022-11-18 15:36:28.356583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fac5.png
--rw-r--r--   0        0        0     2208 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fad0.png
--rw-r--r--   0        0        0     2166 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fad1.png
--rw-r--r--   0        0        0     1780 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fad2.png
--rw-r--r--   0        0        0     1470 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fad3.png
--rw-r--r--   0        0        0     1942 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fad4.png
--rw-r--r--   0        0        0     2275 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fad5.png
--rw-r--r--   0        0        0     1506 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fad6.png
--rw-r--r--   0        0        0     2456 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fad7.png
--rw-r--r--   0        0        0     3231 2022-11-18 15:36:28.384583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fad8.png
--rw-r--r--   0        0        0     2883 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/1fad9.png
--rw-r--r--   0        0        0     3754 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1fae0.png
--rw-r--r--   0        0        0     2667 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1fae1.png
--rw-r--r--   0        0        0     3645 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1fae2.png
--rw-r--r--   0        0        0     3805 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1fae3.png
--rw-r--r--   0        0        0     3362 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/1fae4.png
--rw-r--r--   0        0        0     2324 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/1fae5.png
--rw-r--r--   0        0        0     2612 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1fae6.png
--rw-r--r--   0        0        0     8233 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/1fae7.png
--rw-r--r--   0        0        0     3094 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1faf0.png
--rw-r--r--   0        0        0     3119 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1faf1.png
--rw-r--r--   0        0        0     3274 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1faf2.png
--rw-r--r--   0        0        0     2474 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1faf3.png
--rw-r--r--   0        0        0     2475 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1faf4.png
--rw-r--r--   0        0        0     4017 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1faf5.png
--rw-r--r--   0        0        0     2903 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/1faf6.png
--rw-r--r--   0        0        0      979 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/203c.png
--rw-r--r--   0        0        0     1134 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2049.png
--rw-r--r--   0        0        0      574 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/2122.png
--rw-r--r--   0        0        0     1078 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/2139.png
--rw-r--r--   0        0        0     1083 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/2194.png
--rw-r--r--   0        0        0     1027 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/2195.png
--rw-r--r--   0        0        0     1046 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/2196.png
--rw-r--r--   0        0        0     1044 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/2197.png
--rw-r--r--   0        0        0     1041 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/2198.png
--rw-r--r--   0        0        0     1000 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/2199.png
--rw-r--r--   0        0        0     1098 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/21a9.png
--rw-r--r--   0        0        0     1061 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/21aa.png
--rw-r--r--   0        0        0     1401 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/231a.png
--rw-r--r--   0        0        0     2614 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/231b.png
--rw-r--r--   0        0        0      983 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/2328.png
--rw-r--r--   0        0        0     1078 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/23cf.png
--rw-r--r--   0        0        0     1028 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/23e9.png
--rw-r--r--   0        0        0     1097 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/23ea.png
--rw-r--r--   0        0        0     1069 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/23eb.png
--rw-r--r--   0        0        0     1086 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/23ec.png
--rw-r--r--   0        0        0     1085 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/23ed.png
--rw-r--r--   0        0        0     1153 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/23ee.png
--rw-r--r--   0        0        0     1009 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/23ef.png
--rw-r--r--   0        0        0     3657 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/23f0.png
--rw-r--r--   0        0        0     2800 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/23f1.png
--rw-r--r--   0        0        0     2100 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/23f2.png
--rw-r--r--   0        0        0     2759 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/23f3.png
--rw-r--r--   0        0        0     1053 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/23f8.png
--rw-r--r--   0        0        0      952 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/23f9.png
--rw-r--r--   0        0        0     1014 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/23fa.png
--rw-r--r--   0        0        0     1295 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/24c2.png
--rw-r--r--   0        0        0      408 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/25aa.png
--rw-r--r--   0        0        0      194 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/25ab.png
--rw-r--r--   0        0        0     1011 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/25b6.png
--rw-r--r--   0        0        0     1028 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/25c0.png
--rw-r--r--   0        0        0      196 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/25fb.png
--rw-r--r--   0        0        0      291 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/25fc.png
--rw-r--r--   0        0        0      175 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/25fd.png
--rw-r--r--   0        0        0      283 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/25fe.png
--rw-r--r--   0        0        0     1597 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/2600.png
--rw-r--r--   0        0        0      934 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/2601.png
--rw-r--r--   0        0        0     1630 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/2602.png
--rw-r--r--   0        0        0     3102 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/2603.png
--rw-r--r--   0        0        0     2996 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/2604.png
--rw-r--r--   0        0        0     2616 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/260e.png
--rw-r--r--   0        0        0     1309 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2611.png
--rw-r--r--   0        0        0     2749 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/2614.png
--rw-r--r--   0        0        0     1869 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/2615.png
--rw-r--r--   0        0        0     2927 2022-11-18 15:36:28.380583 a2-0.4.0/src/a2/data/emoji/emoji_images/2618.png
--rw-r--r--   0        0        0     1186 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/261d.png
--rw-r--r--   0        0        0     1956 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/2620.png
--rw-r--r--   0        0        0     1258 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/2622.png
--rw-r--r--   0        0        0     1740 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/2623.png
--rw-r--r--   0        0        0     1113 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2626.png
--rw-r--r--   0        0        0     1243 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/262a.png
--rw-r--r--   0        0        0     1349 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/262e.png
--rw-r--r--   0        0        0     1307 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/262f.png
--rw-r--r--   0        0        0     1621 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/2638.png
--rw-r--r--   0        0        0     1931 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/2639.png
--rw-r--r--   0        0        0     1931 2022-11-18 15:36:28.340582 a2-0.4.0/src/a2/data/emoji/emoji_images/263a.png
--rw-r--r--   0        0        0     1373 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2640.png
--rw-r--r--   0        0        0     1449 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2642.png
--rw-r--r--   0        0        0     1307 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2648.png
--rw-r--r--   0        0        0     1302 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2649.png
--rw-r--r--   0        0        0     1204 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/264a.png
--rw-r--r--   0        0        0     1498 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/264b.png
--rw-r--r--   0        0        0     1435 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/264c.png
--rw-r--r--   0        0        0     1437 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/264d.png
--rw-r--r--   0        0        0     1217 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/264e.png
--rw-r--r--   0        0        0     1252 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/264f.png
--rw-r--r--   0        0        0     1250 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2650.png
--rw-r--r--   0        0        0     1424 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2651.png
--rw-r--r--   0        0        0     1355 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2652.png
--rw-r--r--   0        0        0     1223 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2653.png
--rw-r--r--   0        0        0     1041 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/265f.png
--rw-r--r--   0        0        0      990 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/2660.png
--rw-r--r--   0        0        0     1105 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/2663.png
--rw-r--r--   0        0        0     1024 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/2665.png
--rw-r--r--   0        0        0      819 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/2666.png
--rw-r--r--   0        0        0     1476 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/2668.png
--rw-r--r--   0        0        0     1547 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/267b.png
--rw-r--r--   0        0        0      902 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/267e.png
--rw-r--r--   0        0        0     1487 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/267f.png
--rw-r--r--   0        0        0     1688 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/2692.png
--rw-r--r--   0        0        0     1587 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/2693.png
--rw-r--r--   0        0        0     1924 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/2694.png
--rw-r--r--   0        0        0     1600 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2695.png
--rw-r--r--   0        0        0     2360 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/2696.png
--rw-r--r--   0        0        0     2664 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/2697.png
--rw-r--r--   0        0        0     2767 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/2699.png
--rw-r--r--   0        0        0     1680 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/269b.png
--rw-r--r--   0        0        0     2332 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/269c.png
--rw-r--r--   0        0        0      862 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/26a0.png
--rw-r--r--   0        0        0      822 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/26a1.png
--rw-r--r--   0        0        0     1297 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/26a7.png
--rw-r--r--   0        0        0      833 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/26aa.png
--rw-r--r--   0        0        0     1038 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/26ab.png
--rw-r--r--   0        0        0     1809 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/26b0.png
--rw-r--r--   0        0        0     1967 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/26b1.png
--rw-r--r--   0        0        0     1834 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/26bd.png
--rw-r--r--   0        0        0     2594 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/26be.png
--rw-r--r--   0        0        0     2364 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/26c4.png
--rw-r--r--   0        0        0     1471 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/26c5.png
--rw-r--r--   0        0        0     2224 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/26c8.png
--rw-r--r--   0        0        0     1288 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/26ce.png
--rw-r--r--   0        0        0     1106 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/26cf.png
--rw-r--r--   0        0        0     2363 2022-11-18 15:36:28.408584 a2-0.4.0/src/a2/data/emoji/emoji_images/26d1.png
--rw-r--r--   0        0        0     3241 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/26d3.png
--rw-r--r--   0        0        0     1286 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/26d4.png
--rw-r--r--   0        0        0     1219 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/26e9.png
--rw-r--r--   0        0        0     2405 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/26ea.png
--rw-r--r--   0        0        0     2999 2022-11-18 15:36:28.388583 a2-0.4.0/src/a2/data/emoji/emoji_images/26f0.png
--rw-r--r--   0        0        0     1902 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/26f1.png
--rw-r--r--   0        0        0     3153 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/26f2.png
--rw-r--r--   0        0        0     1712 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/26f3.png
--rw-r--r--   0        0        0     2385 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/26f4.png
--rw-r--r--   0        0        0     2439 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/26f5.png
--rw-r--r--   0        0        0     3013 2022-11-18 15:36:28.360583 a2-0.4.0/src/a2/data/emoji/emoji_images/26f7.png
--rw-r--r--   0        0        0     1886 2022-11-18 15:36:28.404584 a2-0.4.0/src/a2/data/emoji/emoji_images/26f8.png
--rw-r--r--   0        0        0     3213 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/26f9.png
--rw-r--r--   0        0        0     3294 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/26f9_fe0f_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3168 2022-11-18 15:36:28.364583 a2-0.4.0/src/a2/data/emoji/emoji_images/26f9_fe0f_200d_2642_fe0f.png
--rw-r--r--   0        0        0     1854 2022-11-18 15:36:28.392583 a2-0.4.0/src/a2/data/emoji/emoji_images/26fa.png
--rw-r--r--   0        0        0     2366 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/26fd.png
--rw-r--r--   0        0        0     3030 2022-11-18 15:36:28.416584 a2-0.4.0/src/a2/data/emoji/emoji_images/2702.png
--rw-r--r--   0        0        0     1137 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2705.png
--rw-r--r--   0        0        0     2700 2022-11-18 15:36:28.396584 a2-0.4.0/src/a2/data/emoji/emoji_images/2708.png
--rw-r--r--   0        0        0      871 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/2709.png
--rw-r--r--   0        0        0     1669 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/270a.png
--rw-r--r--   0        0        0     1464 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/270b.png
--rw-r--r--   0        0        0     1407 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/270c.png
--rw-r--r--   0        0        0     1751 2022-11-18 15:36:28.348582 a2-0.4.0/src/a2/data/emoji/emoji_images/270d.png
--rw-r--r--   0        0        0     1587 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/270f.png
--rw-r--r--   0        0        0     1526 2022-11-18 15:36:28.412584 a2-0.4.0/src/a2/data/emoji/emoji_images/2712.png
--rw-r--r--   0        0        0      631 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2714.png
--rw-r--r--   0        0        0      518 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2716.png
--rw-r--r--   0        0        0      890 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/271d.png
--rw-r--r--   0        0        0     1315 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/2721.png
--rw-r--r--   0        0        0     1385 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/2728.png
--rw-r--r--   0        0        0     1187 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/2733.png
--rw-r--r--   0        0        0     1432 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/2734.png
--rw-r--r--   0        0        0     3717 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/2744.png
--rw-r--r--   0        0        0     1179 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/2747.png
--rw-r--r--   0        0        0      782 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/274c.png
--rw-r--r--   0        0        0     1100 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/274e.png
--rw-r--r--   0        0        0      685 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2753.png
--rw-r--r--   0        0        0      624 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2754.png
--rw-r--r--   0        0        0      690 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2755.png
--rw-r--r--   0        0        0      568 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2757.png
--rw-r--r--   0        0        0     1038 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/2763.png
--rw-r--r--   0        0        0     1358 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/2764.png
--rw-r--r--   0        0        0     3565 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/2764_fe0f_200d_1f525.png
--rw-r--r--   0        0        0     3181 2022-11-18 15:36:28.344582 a2-0.4.0/src/a2/data/emoji/emoji_images/2764_fe0f_200d_1fa79.png
--rw-r--r--   0        0        0      251 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2795.png
--rw-r--r--   0        0        0      200 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2796.png
--rw-r--r--   0        0        0      249 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2797.png
--rw-r--r--   0        0        0     1047 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/27a1.png
--rw-r--r--   0        0        0      858 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/27b0.png
--rw-r--r--   0        0        0      686 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/27bf.png
--rw-r--r--   0        0        0     1083 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/2934.png
--rw-r--r--   0        0        0     1076 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/2935.png
--rw-r--r--   0        0        0     1044 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/2b05.png
--rw-r--r--   0        0        0     1034 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/2b06.png
--rw-r--r--   0        0        0     1054 2022-11-18 15:36:28.420584 a2-0.4.0/src/a2/data/emoji/emoji_images/2b07.png
--rw-r--r--   0        0        0      700 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/2b1b.png
--rw-r--r--   0        0        0      203 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/2b1c.png
--rw-r--r--   0        0        0     1704 2022-11-18 15:36:28.400584 a2-0.4.0/src/a2/data/emoji/emoji_images/2b50.png
--rw-r--r--   0        0        0     1025 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/2b55.png
--rw-r--r--   0        0        0      614 2022-11-18 15:36:28.424584 a2-0.4.0/src/a2/data/emoji/emoji_images/3030.png
--rw-r--r--   0        0        0      791 2022-11-18 15:36:28.428584 a2-0.4.0/src/a2/data/emoji/emoji_images/303d.png
--rw-r--r--   0        0        0     1614 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/3297.png
--rw-r--r--   0        0        0     1733 2022-11-18 15:36:28.432584 a2-0.4.0/src/a2/data/emoji/emoji_images/3299.png
--rw-r--r--   0        0        0  2152796 2022-07-06 14:12:42.663962 a2-0.4.0/src/a2/data/font/Symbola.ttf
--rw-r--r--   0        0        0  3727644 2022-07-06 14:12:42.683963 a2-0.4.0/src/a2/data/font/Symbola_hint.ttf
--rw-r--r--   0        0        0       44 2022-07-06 14:12:42.683963 a2-0.4.0/src/a2/data/font/sharefonts.net.txt
--rw-r--r--   0        0        0        0 2022-11-01 14:44:14.724032 a2-0.4.0/src/a2/data/vocabularies/__init__.py
--rw-r--r--   0        0        0     2789 2023-02-21 08:27:21.563839 a2-0.4.0/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt
--rw-r--r--   0        0        0      236 2023-02-21 08:27:21.563869 a2-0.4.0/src/a2/data/vocabularies/weather_vocab_enchanted_precipitation.txt
--rw-r--r--   0        0        0      188 2023-02-21 14:04:17.568649 a2-0.4.0/src/a2/dataset/__init__.py
--rw-r--r--   0        0        0      366 2023-02-21 14:04:45.557653 a2-0.4.0/src/a2/dataset/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      645 2023-01-30 15:08:36.152054 a2-0.4.0/src/a2/dataset/__pycache__/emojis.cpython-310.pyc
--rw-r--r--   0        0        0     8877 2023-06-07 07:51:53.099831 a2-0.4.0/src/a2/dataset/__pycache__/load_dataset.cpython-310.pyc
--rw-r--r--   0        0        0      434 2022-08-02 15:37:53.112570 a2-0.4.0/src/a2/dataset/__pycache__/manipulate_datasets.cpython-310.pyc
--rw-r--r--   0        0        0    39422 2023-01-30 15:08:36.940073 a2-0.4.0/src/a2/dataset/__pycache__/radar.cpython-310.pyc
--rw-r--r--   0        0        0     8738 2023-01-30 15:08:36.944073 a2-0.4.0/src/a2/dataset/__pycache__/stations.cpython-310.pyc
--rw-r--r--   0        0        0     1040 2023-02-20 13:59:16.193086 a2-0.4.0/src/a2/dataset/__pycache__/tweets.cpython-310.pyc
--rw-r--r--   0        0        0     2155 2022-12-14 09:39:28.258310 a2-0.4.0/src/a2/dataset/__pycache__/units.cpython-310.pyc
--rw-r--r--   0        0        0    15533 2023-06-06 13:09:57.413845 a2-0.4.0/src/a2/dataset/__pycache__/utils_dataset.cpython-310.pyc
--rw-r--r--   0        0        0      556 2023-01-30 14:59:51.635141 a2-0.4.0/src/a2/dataset/emojis.py
--rw-r--r--   0        0        0     8227 2023-06-06 16:23:55.890263 a2-0.4.0/src/a2/dataset/load_dataset.py
--rw-r--r--   0        0        0    50068 2023-01-30 14:59:51.635141 a2-0.4.0/src/a2/dataset/radar.py
--rw-r--r--   0        0        0    10354 2023-01-30 14:59:51.635141 a2-0.4.0/src/a2/dataset/stations.py
--rw-r--r--   0        0        0      699 2023-02-20 13:53:30.152744 a2-0.4.0/src/a2/dataset/tweets.py
--rw-r--r--   0        0        0     1464 2022-12-14 09:36:33.150856 a2-0.4.0/src/a2/dataset/units.py
--rw-r--r--   0        0        0    17623 2023-06-06 13:09:51.493718 a2-0.4.0/src/a2/dataset/utils_dataset.py
--rw-r--r--   0        0        0      218 2023-06-13 14:57:04.764349 a2-0.4.0/src/a2/plotting/__init__.py
--rw-r--r--   0        0        0      397 2023-06-13 15:02:53.558067 a2-0.4.0/src/a2/plotting/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7285 2023-06-15 09:40:17.553725 a2-0.4.0/src/a2/plotting/__pycache__/analysis.cpython-310.pyc
--rw-r--r--   0        0        0     2275 2023-06-13 15:02:53.558067 a2-0.4.0/src/a2/plotting/__pycache__/axes_utils.cpython-310.pyc
--rw-r--r--   0        0        0     1082 2023-06-12 14:35:35.933045 a2-0.4.0/src/a2/plotting/__pycache__/colormesh.cpython-310.pyc
--rw-r--r--   0        0        0      754 2023-06-13 14:21:36.116890 a2-0.4.0/src/a2/plotting/__pycache__/figures.cpython-310.pyc
--rw-r--r--   0        0        0     5981 2023-06-13 14:21:36.104889 a2-0.4.0/src/a2/plotting/__pycache__/histogram_2d_utils.cpython-310.pyc
--rw-r--r--   0        0        0    24893 2023-06-13 15:16:41.952119 a2-0.4.0/src/a2/plotting/__pycache__/histograms.cpython-310.pyc
--rw-r--r--   0        0        0     3126 2023-06-12 14:30:40.201208 a2-0.4.0/src/a2/plotting/__pycache__/parallel_plotting.cpython-310.pyc
--rw-r--r--   0        0        0     2721 2023-06-13 14:05:47.932777 a2-0.4.0/src/a2/plotting/__pycache__/timeseries.cpython-310.pyc
--rw-r--r--   0        0        0    16725 2023-06-14 10:00:39.495890 a2-0.4.0/src/a2/plotting/__pycache__/utils_plotting.cpython-310.pyc
--rw-r--r--   0        0        0    29262 2023-06-13 15:02:53.834075 a2-0.4.0/src/a2/plotting/__pycache__/weather_maps.cpython-310.pyc
--rw-r--r--   0        0        0     8299 2023-06-14 10:05:04.619166 a2-0.4.0/src/a2/plotting/analysis.py
--rw-r--r--   0        0        0     2266 2023-06-13 14:57:04.764349 a2-0.4.0/src/a2/plotting/axes_utils.py
--rw-r--r--   0        0        0      910 2023-06-12 14:35:07.100288 a2-0.4.0/src/a2/plotting/colormesh.py
--rw-r--r--   0        0        0      505 2023-06-13 14:18:41.948324 a2-0.4.0/src/a2/plotting/figures.py
--rw-r--r--   0        0        0     8363 2023-06-13 14:21:30.496741 a2-0.4.0/src/a2/plotting/histogram_2d_utils.py
--rw-r--r--   0        0        0    35236 2023-06-13 15:16:40.584083 a2-0.4.0/src/a2/plotting/histograms.py
--rw-r--r--   0        0        0     3010 2023-06-12 14:30:35.341077 a2-0.4.0/src/a2/plotting/parallel_plotting.py
--rw-r--r--   0        0        0     2814 2023-06-13 14:05:14.219928 a2-0.4.0/src/a2/plotting/timeseries.py
--rw-r--r--   0        0        0    19695 2023-06-14 10:00:38.439840 a2-0.4.0/src/a2/plotting/utils_plotting.py
--rw-r--r--   0        0        0    34761 2023-06-13 14:57:04.760349 a2-0.4.0/src/a2/plotting/weather_maps.py
--rw-r--r--   0        0        0       67 2022-11-01 14:44:14.724032 a2-0.4.0/src/a2/preprocess/__init__.py
--rw-r--r--   0        0        0      228 2022-11-10 09:21:06.475180 a2-0.4.0/src/a2/preprocess/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3659 2022-12-06 08:50:28.056225 a2-0.4.0/src/a2/preprocess/__pycache__/embedding.cpython-310.pyc
--rw-r--r--   0        0        0    26114 2023-05-23 13:01:09.722463 a2-0.4.0/src/a2/preprocess/__pycache__/normalize_text.cpython-310.pyc
--rw-r--r--   0        0        0     3645 2022-12-06 08:38:01.708129 a2-0.4.0/src/a2/preprocess/embedding.py
--rw-r--r--   0        0        0    30389 2023-05-12 12:06:33.277030 a2-0.4.0/src/a2/preprocess/normalize_text.py
--rw-r--r--   0        0        0      172 2023-05-12 12:06:13.512505 a2-0.4.0/src/a2/training/__init__.py
--rw-r--r--   0        0        0      343 2023-05-16 09:06:59.916315 a2-0.4.0/src/a2/training/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4800 2023-05-16 09:07:02.808385 a2-0.4.0/src/a2/training/__pycache__/benchmarks.cpython-310.pyc
--rw-r--r--   0        0        0     3145 2023-06-08 14:11:17.917178 a2-0.4.0/src/a2/training/__pycache__/dataset_hugging.cpython-310.pyc
--rw-r--r--   0        0        0     4071 2023-06-08 09:56:22.659014 a2-0.4.0/src/a2/training/__pycache__/evaluate_hugging.cpython-310.pyc
--rw-r--r--   0        0        0     5245 2023-06-12 13:59:16.034461 a2-0.4.0/src/a2/training/__pycache__/tracking.cpython-310.pyc
--rw-r--r--   0        0        0     2217 2023-05-16 09:07:02.804385 a2-0.4.0/src/a2/training/__pycache__/tracking_hugging.cpython-310.pyc
--rw-r--r--   0        0        0     6945 2023-06-14 09:47:23.282569 a2-0.4.0/src/a2/training/__pycache__/training_deep500.cpython-310.pyc
--rw-r--r--   0        0        0     9552 2023-06-09 13:11:55.102911 a2-0.4.0/src/a2/training/__pycache__/training_hugging.cpython-310.pyc
--rw-r--r--   0        0        0     6756 2023-04-18 13:46:32.335340 a2-0.4.0/src/a2/training/__pycache__/training_performance.cpython-310.pyc
--rw-r--r--   0        0        0      306 2023-01-30 15:08:44.672258 a2-0.4.0/src/a2/training/__pycache__/utils_training.cpython-310.pyc
--rw-r--r--   0        0        0     3889 2023-05-12 12:12:57.271066 a2-0.4.0/src/a2/training/benchmarks.py
--rw-r--r--   0        0        0     3252 2023-06-08 10:49:52.048837 a2-0.4.0/src/a2/training/dataset_hugging.py
--rw-r--r--   0        0        0     4295 2023-06-08 08:43:16.088673 a2-0.4.0/src/a2/training/evaluate_hugging.py
--rw-r--r--   0        0        0     4846 2023-06-12 13:56:25.094228 a2-0.4.0/src/a2/training/tracking.py
--rw-r--r--   0        0        0     1780 2023-05-12 12:06:13.512505 a2-0.4.0/src/a2/training/tracking_hugging.py
--rw-r--r--   0        0        0     6757 2023-06-14 09:47:14.434154 a2-0.4.0/src/a2/training/training_deep500.py
--rw-r--r--   0        0        0    12776 2023-06-09 13:11:33.538318 a2-0.4.0/src/a2/training/training_hugging.py
--rw-r--r--   0        0        0     6821 2023-05-12 12:06:33.277030 a2-0.4.0/src/a2/training/training_performance.py
--rw-r--r--   0        0        0       73 2023-01-30 14:59:51.639141 a2-0.4.0/src/a2/training/utils_training.py
--rw-r--r--   0        0        0       87 2022-11-01 14:44:14.728032 a2-0.4.0/src/a2/twitter/__init__.py
--rw-r--r--   0        0        0      249 2022-11-10 09:22:53.001431 a2-0.4.0/src/a2/twitter/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4896 2023-02-20 13:59:24.705291 a2-0.4.0/src/a2/twitter/__pycache__/downloader.cpython-310.pyc
--rw-r--r--   0        0        0     9148 2023-05-23 13:01:12.894332 a2-0.4.0/src/a2/twitter/__pycache__/locations.cpython-310.pyc
--rw-r--r--   0        0        0     8339 2022-08-01 13:51:16.422462 a2-0.4.0/src/a2/twitter/__pycache__/manipulate_tweets.cpython-310.pyc
--rw-r--r--   0        0        0     5836 2023-02-20 13:59:24.705291 a2-0.4.0/src/a2/twitter/__pycache__/twitter_api.cpython-310.pyc
--rw-r--r--   0        0        0     4570 2023-02-20 13:53:30.156744 a2-0.4.0/src/a2/twitter/downloader.py
--rw-r--r--   0        0        0    11489 2023-06-06 13:55:59.732319 a2-0.4.0/src/a2/twitter/locations.py
--rw-r--r--   0        0        0     6765 2023-02-20 13:53:30.156744 a2-0.4.0/src/a2/twitter/twitter_api.py
--rw-r--r--   0        0        0      196 2023-06-06 12:24:26.982480 a2-0.4.0/src/a2/utils/__init__.py
--rw-r--r--   0        0        0      376 2023-06-06 12:42:23.443076 a2-0.4.0/src/a2/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     9436 2023-06-12 09:48:54.002620 a2-0.4.0/src/a2/utils/__pycache__/argparse.cpython-310.pyc
--rw-r--r--   0        0        0      787 2023-05-16 09:06:59.920315 a2-0.4.0/src/a2/utils/__pycache__/checks.cpython-310.pyc
--rw-r--r--   0        0        0     1037 2023-06-13 15:02:52.894049 a2-0.4.0/src/a2/utils/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0     9546 2023-06-06 15:04:04.548994 a2-0.4.0/src/a2/utils/__pycache__/file_handling.cpython-310.pyc
--rw-r--r--   0        0        0      445 2023-05-16 09:07:00.248323 a2-0.4.0/src/a2/utils/__pycache__/strings.cpython-310.pyc
--rw-r--r--   0        0        0     6104 2023-05-16 09:07:00.248323 a2-0.4.0/src/a2/utils/__pycache__/testing.cpython-310.pyc
--rw-r--r--   0        0        0      545 2022-12-14 09:39:28.222309 a2-0.4.0/src/a2/utils/__pycache__/times.cpython-310.pyc
--rw-r--r--   0        0        0     7600 2023-06-13 15:02:53.402063 a2-0.4.0/src/a2/utils/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0    10625 2023-06-12 09:48:51.558565 a2-0.4.0/src/a2/utils/argparse.py
--rw-r--r--   0        0        0      518 2023-05-11 10:46:59.965258 a2-0.4.0/src/a2/utils/checks.py
--rw-r--r--   0        0        0      731 2023-06-13 14:57:04.760349 a2-0.4.0/src/a2/utils/constants.py
--rw-r--r--   0        0        0     9361 2023-06-06 14:01:17.485564 a2-0.4.0/src/a2/utils/file_handling.py
--rw-r--r--   0        0        0       90 2023-05-12 12:06:33.277030 a2-0.4.0/src/a2/utils/strings.py
--rw-r--r--   0        0        0     5327 2023-05-12 12:06:33.277030 a2-0.4.0/src/a2/utils/testing.py
--rw-r--r--   0        0        0      394 2022-12-14 09:36:33.154856 a2-0.4.0/src/a2/utils/times.py
--rw-r--r--   0        0        0     7061 2023-06-13 14:57:08.084443 a2-0.4.0/src/a2/utils/utils.py
--rw-r--r--   0        0        0     1947 1970-01-01 00:00:00.000000 a2-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     4419 2023-06-15 16:17:28.212046 a2-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-20 15:29:54.345253 a2-0.4.1/src/a2/__init__.py
+-rw-r--r--   0        0        0       45 2023-01-13 09:43:31.404482 a2-0.4.1/src/a2/cli/__init__.py
+-rw-r--r--   0        0        0      200 2023-01-13 09:53:11.940626 a2-0.4.1/src/a2/cli/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      297 2023-01-13 09:40:55.677429 a2-0.4.1/src/a2/cli/__pycache__/main.cpython-310.pyc
+-rw-r--r--   0        0        0       39 2023-01-13 09:45:19.522669 a2-0.4.1/src/a2/cli/cli_plotting/__init__.py
+-rw-r--r--   0        0        0      203 2023-01-13 09:53:11.952627 a2-0.4.1/src/a2/cli/cli_plotting/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      359 2023-01-13 09:53:14.892690 a2-0.4.1/src/a2/cli/cli_plotting/__pycache__/plot.cpython-310.pyc
+-rw-r--r--   0        0        0     2094 2023-06-13 15:13:22.154868 a2-0.4.1/src/a2/cli/cli_plotting/__pycache__/single_plots.cpython-310.pyc
+-rw-r--r--   0        0        0      107 2023-01-13 09:46:23.599985 a2-0.4.1/src/a2/cli/cli_plotting/plot.py
+-rw-r--r--   0        0        0     2049 2023-06-13 14:49:56.664626 a2-0.4.1/src/a2/cli/cli_plotting/single_plots.py
+-rw-r--r--   0        0        0       66 2023-01-13 09:36:10.235731 a2-0.4.1/src/a2/cli/main.py
+-rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.4.1/src/a2/data/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.4.1/src/a2/data/emoji/__init__.py
+-rw-r--r--   0        0        0   379747 2022-11-01 14:44:14.724032 a2-0.4.1/src/a2/data/emoji/emoji_df.csv
+-rw-r--r--   0        0        0     1117 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/0023_fe0f_20e3.png
+-rw-r--r--   0        0        0     1221 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/002a_fe0f_20e3.png
+-rw-r--r--   0        0        0     1065 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/0030_fe0f_20e3.png
+-rw-r--r--   0        0        0      989 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/0031_fe0f_20e3.png
+-rw-r--r--   0        0        0     1043 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/0032_fe0f_20e3.png
+-rw-r--r--   0        0        0     1133 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/0033_fe0f_20e3.png
+-rw-r--r--   0        0        0     1077 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/0034_fe0f_20e3.png
+-rw-r--r--   0        0        0     1204 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/0035_fe0f_20e3.png
+-rw-r--r--   0        0        0     1142 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/0036_fe0f_20e3.png
+-rw-r--r--   0        0        0      985 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/0037_fe0f_20e3.png
+-rw-r--r--   0        0        0     1120 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/0038_fe0f_20e3.png
+-rw-r--r--   0        0        0     1157 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/0039_fe0f_20e3.png
+-rw-r--r--   0        0        0     1096 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/00a9.png
+-rw-r--r--   0        0        0     1091 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/00ae.png
+-rw-r--r--   0        0        0     1250 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f004.png
+-rw-r--r--   0        0        0     1141 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f0cf.png
+-rw-r--r--   0        0        0     1236 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f170.png
+-rw-r--r--   0        0        0     1186 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f171.png
+-rw-r--r--   0        0        0     1363 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f17e.png
+-rw-r--r--   0        0        0     1075 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f17f.png
+-rw-r--r--   0        0        0     1342 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f18e.png
+-rw-r--r--   0        0        0     1352 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f191.png
+-rw-r--r--   0        0        0     1192 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f192.png
+-rw-r--r--   0        0        0     1133 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f193.png
+-rw-r--r--   0        0        0     1150 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f194.png
+-rw-r--r--   0        0        0     1202 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f195.png
+-rw-r--r--   0        0        0     1194 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f196.png
+-rw-r--r--   0        0        0     1264 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f197.png
+-rw-r--r--   0        0        0     1471 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f198.png
+-rw-r--r--   0        0        0     1260 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f199.png
+-rw-r--r--   0        0        0     1361 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f19a.png
+-rw-r--r--   0        0        0     1893 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1e8.png
+-rw-r--r--   0        0        0     1526 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1e9.png
+-rw-r--r--   0        0        0     1245 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1ea.png
+-rw-r--r--   0        0        0     1346 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1eb.png
+-rw-r--r--   0        0        0     1555 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1ec.png
+-rw-r--r--   0        0        0     2029 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1ee.png
+-rw-r--r--   0        0        0     1206 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1f1.png
+-rw-r--r--   0        0        0     1444 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1f2.png
+-rw-r--r--   0        0        0     1314 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1f4.png
+-rw-r--r--   0        0        0     1016 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1f6.png
+-rw-r--r--   0        0        0     1193 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1f7.png
+-rw-r--r--   0        0        0     1597 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1f8.png
+-rw-r--r--   0        0        0     1252 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1f9.png
+-rw-r--r--   0        0        0     1890 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1fa.png
+-rw-r--r--   0        0        0     1379 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1fc.png
+-rw-r--r--   0        0        0     1637 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1fd.png
+-rw-r--r--   0        0        0     1592 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1ff.png
+-rw-r--r--   0        0        0     1362 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1e6.png
+-rw-r--r--   0        0        0     1135 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1e7.png
+-rw-r--r--   0        0        0      935 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1e9.png
+-rw-r--r--   0        0        0      998 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1ea.png
+-rw-r--r--   0        0        0     1253 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1eb.png
+-rw-r--r--   0        0        0     1348 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1ec.png
+-rw-r--r--   0        0        0     1129 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1ed.png
+-rw-r--r--   0        0        0     1766 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1ee.png
+-rw-r--r--   0        0        0     1173 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1ef.png
+-rw-r--r--   0        0        0     1638 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1f1.png
+-rw-r--r--   0        0        0     2553 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1f2.png
+-rw-r--r--   0        0        0     2134 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1f3.png
+-rw-r--r--   0        0        0     1662 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1f4.png
+-rw-r--r--   0        0        0     1467 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1f6.png
+-rw-r--r--   0        0        0     1477 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1f7.png
+-rw-r--r--   0        0        0     1323 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1f8.png
+-rw-r--r--   0        0        0     1794 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1f9.png
+-rw-r--r--   0        0        0     1658 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1fb.png
+-rw-r--r--   0        0        0     1278 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1fc.png
+-rw-r--r--   0        0        0     1417 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1fe.png
+-rw-r--r--   0        0        0     2195 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1ff.png
+-rw-r--r--   0        0        0     1263 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1e6.png
+-rw-r--r--   0        0        0     1241 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1e8.png
+-rw-r--r--   0        0        0     2050 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1e9.png
+-rw-r--r--   0        0        0     1831 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1eb.png
+-rw-r--r--   0        0        0     1460 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1ec.png
+-rw-r--r--   0        0        0      879 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1ed.png
+-rw-r--r--   0        0        0     1053 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1ee.png
+-rw-r--r--   0        0        0     1735 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1f0.png
+-rw-r--r--   0        0        0     1317 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1f1.png
+-rw-r--r--   0        0        0     1118 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1f2.png
+-rw-r--r--   0        0        0     1055 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1f3.png
+-rw-r--r--   0        0        0     1372 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1f4.png
+-rw-r--r--   0        0        0     1073 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1f5.png
+-rw-r--r--   0        0        0     1521 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1f7.png
+-rw-r--r--   0        0        0     1609 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1fa.png
+-rw-r--r--   0        0        0     1711 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1fb.png
+-rw-r--r--   0        0        0     1215 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1fc.png
+-rw-r--r--   0        0        0     1511 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1fd.png
+-rw-r--r--   0        0        0     1224 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1fe.png
+-rw-r--r--   0        0        0     1236 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1ff.png
+-rw-r--r--   0        0        0     1280 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e9_1f1ea.png
+-rw-r--r--   0        0        0     2888 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e9_1f1ec.png
+-rw-r--r--   0        0        0     1331 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e9_1f1ef.png
+-rw-r--r--   0        0        0     1257 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e9_1f1f0.png
+-rw-r--r--   0        0        0     2283 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e9_1f1f2.png
+-rw-r--r--   0        0        0     1737 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e9_1f1f4.png
+-rw-r--r--   0        0        0     1324 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e9_1f1ff.png
+-rw-r--r--   0        0        0     1513 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ea_1f1e6.png
+-rw-r--r--   0        0        0     1976 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ea_1f1e8.png
+-rw-r--r--   0        0        0     1138 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ea_1f1ea.png
+-rw-r--r--   0        0        0     1301 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ea_1f1ec.png
+-rw-r--r--   0        0        0     1270 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ea_1f1ed.png
+-rw-r--r--   0        0        0     1719 2022-11-18 15:36:28.436585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ea_1f1f7.png
+-rw-r--r--   0        0        0     1513 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ea_1f1f8.png
+-rw-r--r--   0        0        0     1477 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ea_1f1f9.png
+-rw-r--r--   0        0        0      969 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ea_1f1fa.png
+-rw-r--r--   0        0        0     1213 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1eb_1f1ee.png
+-rw-r--r--   0        0        0     2421 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1eb_1f1ef.png
+-rw-r--r--   0        0        0     2067 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1eb_1f1f0.png
+-rw-r--r--   0        0        0     1005 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1eb_1f1f2.png
+-rw-r--r--   0        0        0     1837 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1eb_1f1f4.png
+-rw-r--r--   0        0        0     1073 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1eb_1f1f7.png
+-rw-r--r--   0        0        0     1362 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1e6.png
+-rw-r--r--   0        0        0     2314 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1e7.png
+-rw-r--r--   0        0        0     1749 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1e9.png
+-rw-r--r--   0        0        0     1583 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1ea.png
+-rw-r--r--   0        0        0     1274 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1eb.png
+-rw-r--r--   0        0        0     1488 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1ec.png
+-rw-r--r--   0        0        0     1425 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1ed.png
+-rw-r--r--   0        0        0     1678 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1ee.png
+-rw-r--r--   0        0        0     1202 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1f1.png
+-rw-r--r--   0        0        0     1570 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1f2.png
+-rw-r--r--   0        0        0     1023 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1f3.png
+-rw-r--r--   0        0        0     1442 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1f5.png
+-rw-r--r--   0        0        0     1641 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1f6.png
+-rw-r--r--   0        0        0     1677 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1f7.png
+-rw-r--r--   0        0        0     2181 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1f8.png
+-rw-r--r--   0        0        0     1224 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1f9.png
+-rw-r--r--   0        0        0     1354 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1fa.png
+-rw-r--r--   0        0        0     1314 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1fc.png
+-rw-r--r--   0        0        0     1857 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1fe.png
+-rw-r--r--   0        0        0     1138 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ed_1f1f0.png
+-rw-r--r--   0        0        0     1890 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ed_1f1f2.png
+-rw-r--r--   0        0        0     1250 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ed_1f1f3.png
+-rw-r--r--   0        0        0     1843 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ed_1f1f7.png
+-rw-r--r--   0        0        0     1394 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ed_1f1f9.png
+-rw-r--r--   0        0        0     1317 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ed_1f1fa.png
+-rw-r--r--   0        0        0     1300 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1e8.png
+-rw-r--r--   0        0        0     1131 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1e9.png
+-rw-r--r--   0        0        0     1070 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1ea.png
+-rw-r--r--   0        0        0     1453 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1f1.png
+-rw-r--r--   0        0        0     1135 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1f2.png
+-rw-r--r--   0        0        0     1507 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1f3.png
+-rw-r--r--   0        0        0     2888 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1f4.png
+-rw-r--r--   0        0        0     1295 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1f6.png
+-rw-r--r--   0        0        0     1566 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1f7.png
+-rw-r--r--   0        0        0     1577 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1f8.png
+-rw-r--r--   0        0        0      995 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1f9.png
+-rw-r--r--   0        0        0     1711 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ef_1f1ea.png
+-rw-r--r--   0        0        0     1536 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ef_1f1f2.png
+-rw-r--r--   0        0        0     1361 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ef_1f1f4.png
+-rw-r--r--   0        0        0     1019 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ef_1f1f5.png
+-rw-r--r--   0        0        0     1778 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1ea.png
+-rw-r--r--   0        0        0     1133 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1ec.png
+-rw-r--r--   0        0        0     1600 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1ed.png
+-rw-r--r--   0        0        0     1897 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1ee.png
+-rw-r--r--   0        0        0     1884 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1f2.png
+-rw-r--r--   0        0        0     1760 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1f3.png
+-rw-r--r--   0        0        0     1552 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1f5.png
+-rw-r--r--   0        0        0     1531 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1f7.png
+-rw-r--r--   0        0        0     1291 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1fc.png
+-rw-r--r--   0        0        0     2144 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1fe.png
+-rw-r--r--   0        0        0     1473 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1ff.png
+-rw-r--r--   0        0        0     1229 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1e6.png
+-rw-r--r--   0        0        0     1510 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1e7.png
+-rw-r--r--   0        0        0     1336 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1e8.png
+-rw-r--r--   0        0        0     1314 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1ee.png
+-rw-r--r--   0        0        0     1483 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1f0.png
+-rw-r--r--   0        0        0     1995 2022-11-18 15:36:28.440585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1f7.png
+-rw-r--r--   0        0        0     1480 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1f8.png
+-rw-r--r--   0        0        0     1333 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1f9.png
+-rw-r--r--   0        0        0     1363 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1fa.png
+-rw-r--r--   0        0        0     1056 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1fb.png
+-rw-r--r--   0        0        0     1336 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1fe.png
+-rw-r--r--   0        0        0     1158 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1e6.png
+-rw-r--r--   0        0        0     1071 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1e8.png
+-rw-r--r--   0        0        0     1548 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1e9.png
+-rw-r--r--   0        0        0     1112 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1ea.png
+-rw-r--r--   0        0        0     1073 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1eb.png
+-rw-r--r--   0        0        0     1189 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1ec.png
+-rw-r--r--   0        0        0     1577 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1ed.png
+-rw-r--r--   0        0        0     1957 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1f0.png
+-rw-r--r--   0        0        0     1046 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1f1.png
+-rw-r--r--   0        0        0     1574 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1f2.png
+-rw-r--r--   0        0        0     1204 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1f3.png
+-rw-r--r--   0        0        0     1165 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1f4.png
+-rw-r--r--   0        0        0     1791 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1f5.png
+-rw-r--r--   0        0        0     1505 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1f6.png
+-rw-r--r--   0        0        0     1373 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1f7.png
+-rw-r--r--   0        0        0     2172 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1f8.png
+-rw-r--r--   0        0        0     1035 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1f9.png
+-rw-r--r--   0        0        0     1488 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1fa.png
+-rw-r--r--   0        0        0     1163 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1fb.png
+-rw-r--r--   0        0        0     1364 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1fc.png
+-rw-r--r--   0        0        0     1311 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1fd.png
+-rw-r--r--   0        0        0     2364 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1fe.png
+-rw-r--r--   0        0        0     1802 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1ff.png
+-rw-r--r--   0        0        0     1835 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1e6.png
+-rw-r--r--   0        0        0     1794 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1e8.png
+-rw-r--r--   0        0        0     1423 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1ea.png
+-rw-r--r--   0        0        0     1149 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1eb.png
+-rw-r--r--   0        0        0      881 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1ec.png
+-rw-r--r--   0        0        0     1377 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1ee.png
+-rw-r--r--   0        0        0     1234 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1f1.png
+-rw-r--r--   0        0        0     1658 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1f4.png
+-rw-r--r--   0        0        0      999 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1f5.png
+-rw-r--r--   0        0        0     1148 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1f7.png
+-rw-r--r--   0        0        0     2200 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1fa.png
+-rw-r--r--   0        0        0     1683 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1ff.png
+-rw-r--r--   0        0        0     1419 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f4_1f1f2.png
+-rw-r--r--   0        0        0     1550 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1e6.png
+-rw-r--r--   0        0        0      977 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1ea.png
+-rw-r--r--   0        0        0     1502 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1eb.png
+-rw-r--r--   0        0        0     1432 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1ec.png
+-rw-r--r--   0        0        0     1695 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1ed.png
+-rw-r--r--   0        0        0     1098 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1f0.png
+-rw-r--r--   0        0        0     1040 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1f1.png
+-rw-r--r--   0        0        0     3113 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1f2.png
+-rw-r--r--   0        0        0     2228 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1f3.png
+-rw-r--r--   0        0        0     1622 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1f7.png
+-rw-r--r--   0        0        0     1211 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1f8.png
+-rw-r--r--   0        0        0     1590 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1f9.png
+-rw-r--r--   0        0        0     1022 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1fc.png
+-rw-r--r--   0        0        0     1607 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1fe.png
+-rw-r--r--   0        0        0      959 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f6_1f1e6.png
+-rw-r--r--   0        0        0     1792 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f7_1f1ea.png
+-rw-r--r--   0        0        0      954 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f7_1f1f4.png
+-rw-r--r--   0        0        0     1872 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f7_1f1f8.png
+-rw-r--r--   0        0        0     1298 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f7_1f1fa.png
+-rw-r--r--   0        0        0     1632 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f7_1f1fc.png
+-rw-r--r--   0        0        0     1134 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1e6.png
+-rw-r--r--   0        0        0     1729 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1e7.png
+-rw-r--r--   0        0        0     1725 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1e8.png
+-rw-r--r--   0        0        0     1203 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1e9.png
+-rw-r--r--   0        0        0     1307 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1ea.png
+-rw-r--r--   0        0        0     1261 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1ec.png
+-rw-r--r--   0        0        0     1893 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1ed.png
+-rw-r--r--   0        0        0     1613 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1ee.png
+-rw-r--r--   0        0        0     1658 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1ef.png
+-rw-r--r--   0        0        0     1656 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1f0.png
+-rw-r--r--   0        0        0     1411 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1f1.png
+-rw-r--r--   0        0        0     1662 2022-11-18 15:36:28.444585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1f2.png
+-rw-r--r--   0        0        0     1228 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1f3.png
+-rw-r--r--   0        0        0      884 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1f4.png
+-rw-r--r--   0        0        0     1557 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1f7.png
+-rw-r--r--   0        0        0     1630 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1f8.png
+-rw-r--r--   0        0        0     1600 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1f9.png
+-rw-r--r--   0        0        0     1424 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1fb.png
+-rw-r--r--   0        0        0     1684 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1fd.png
+-rw-r--r--   0        0        0     1373 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1fe.png
+-rw-r--r--   0        0        0     2344 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1ff.png
+-rw-r--r--   0        0        0     1893 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1e6.png
+-rw-r--r--   0        0        0     2139 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1e8.png
+-rw-r--r--   0        0        0      968 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1e9.png
+-rw-r--r--   0        0        0     1213 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1eb.png
+-rw-r--r--   0        0        0     1780 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1ec.png
+-rw-r--r--   0        0        0     1646 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1ed.png
+-rw-r--r--   0        0        0     1440 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1ef.png
+-rw-r--r--   0        0        0     1176 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1f0.png
+-rw-r--r--   0        0        0     1409 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1f1.png
+-rw-r--r--   0        0        0     1338 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1f2.png
+-rw-r--r--   0        0        0     1118 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1f3.png
+-rw-r--r--   0        0        0     1163 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1f4.png
+-rw-r--r--   0        0        0     1213 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1f7.png
+-rw-r--r--   0        0        0     1448 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1f9.png
+-rw-r--r--   0        0        0     2227 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1fb.png
+-rw-r--r--   0        0        0     1350 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1fc.png
+-rw-r--r--   0        0        0     1690 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1ff.png
+-rw-r--r--   0        0        0     1105 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fa_1f1e6.png
+-rw-r--r--   0        0        0     1967 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fa_1f1ec.png
+-rw-r--r--   0        0        0     2435 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fa_1f1f2.png
+-rw-r--r--   0        0        0     1129 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fa_1f1f3.png
+-rw-r--r--   0        0        0     2435 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fa_1f1f8.png
+-rw-r--r--   0        0        0     2010 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fa_1f1fe.png
+-rw-r--r--   0        0        0     1743 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fa_1f1ff.png
+-rw-r--r--   0        0        0     1197 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fb_1f1e6.png
+-rw-r--r--   0        0        0     1337 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fb_1f1e8.png
+-rw-r--r--   0        0        0     1580 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fb_1f1ea.png
+-rw-r--r--   0        0        0     1974 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fb_1f1ec.png
+-rw-r--r--   0        0        0     2635 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fb_1f1ee.png
+-rw-r--r--   0        0        0     1046 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fb_1f1f3.png
+-rw-r--r--   0        0        0     1594 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fb_1f1fa.png
+-rw-r--r--   0        0        0     1319 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fc_1f1eb.png
+-rw-r--r--   0        0        0     1134 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fc_1f1f8.png
+-rw-r--r--   0        0        0     1128 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fd_1f1f0.png
+-rw-r--r--   0        0        0     1184 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fe_1f1ea.png
+-rw-r--r--   0        0        0     1649 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fe_1f1f9.png
+-rw-r--r--   0        0        0     2075 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ff_1f1e6.png
+-rw-r--r--   0        0        0     1071 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ff_1f1f2.png
+-rw-r--r--   0        0        0     2394 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ff_1f1fc.png
+-rw-r--r--   0        0        0     1081 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f201.png
+-rw-r--r--   0        0        0     1165 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f202.png
+-rw-r--r--   0        0        0     1478 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f21a.png
+-rw-r--r--   0        0        0     1514 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f22f.png
+-rw-r--r--   0        0        0     1682 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f232.png
+-rw-r--r--   0        0        0     1372 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f233.png
+-rw-r--r--   0        0        0     1450 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f234.png
+-rw-r--r--   0        0        0     1667 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f235.png
+-rw-r--r--   0        0        0     1243 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f236.png
+-rw-r--r--   0        0        0     1127 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f237.png
+-rw-r--r--   0        0        0     1207 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f238.png
+-rw-r--r--   0        0        0     1517 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f239.png
+-rw-r--r--   0        0        0     1349 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f23a.png
+-rw-r--r--   0        0        0     1457 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f250.png
+-rw-r--r--   0        0        0     1181 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f251.png
+-rw-r--r--   0        0        0     1345 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f300.png
+-rw-r--r--   0        0        0     1493 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f301.png
+-rw-r--r--   0        0        0     1753 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f302.png
+-rw-r--r--   0        0        0     2162 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f303.png
+-rw-r--r--   0        0        0     1959 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f304.png
+-rw-r--r--   0        0        0     1748 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f305.png
+-rw-r--r--   0        0        0     2046 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f306.png
+-rw-r--r--   0        0        0     2397 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f307.png
+-rw-r--r--   0        0        0     3358 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f308.png
+-rw-r--r--   0        0        0     1972 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f309.png
+-rw-r--r--   0        0        0     2761 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f30a.png
+-rw-r--r--   0        0        0     3524 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f30b.png
+-rw-r--r--   0        0        0     1639 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f30c.png
+-rw-r--r--   0        0        0     3984 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f30d.png
+-rw-r--r--   0        0        0     3347 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f30e.png
+-rw-r--r--   0        0        0     3956 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f30f.png
+-rw-r--r--   0        0        0     2985 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f310.png
+-rw-r--r--   0        0        0     1274 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f311.png
+-rw-r--r--   0        0        0     2102 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f312.png
+-rw-r--r--   0        0        0     2416 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f313.png
+-rw-r--r--   0        0        0     2310 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f314.png
+-rw-r--r--   0        0        0     1897 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f315.png
+-rw-r--r--   0        0        0     2545 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f316.png
+-rw-r--r--   0        0        0     2489 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f317.png
+-rw-r--r--   0        0        0     1857 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f318.png
+-rw-r--r--   0        0        0     1394 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f319.png
+-rw-r--r--   0        0        0     1551 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f31a.png
+-rw-r--r--   0        0        0     1589 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f31b.png
+-rw-r--r--   0        0        0     1662 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f31c.png
+-rw-r--r--   0        0        0     2808 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f31d.png
+-rw-r--r--   0        0        0     3537 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f31e.png
+-rw-r--r--   0        0        0     1898 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f31f.png
+-rw-r--r--   0        0        0     2160 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f320.png
+-rw-r--r--   0        0        0     1925 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f321.png
+-rw-r--r--   0        0        0     1971 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f324.png
+-rw-r--r--   0        0        0     1326 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f325.png
+-rw-r--r--   0        0        0     2070 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f326.png
+-rw-r--r--   0        0        0     1721 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f327.png
+-rw-r--r--   0        0        0     1666 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f328.png
+-rw-r--r--   0        0        0     1323 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f329.png
+-rw-r--r--   0        0        0     2338 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f32a.png
+-rw-r--r--   0        0        0     1345 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f32b.png
+-rw-r--r--   0        0        0     1482 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f32c.png
+-rw-r--r--   0        0        0     2143 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f32d.png
+-rw-r--r--   0        0        0     3164 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f32e.png
+-rw-r--r--   0        0        0     2846 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f32f.png
+-rw-r--r--   0        0        0     2278 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f330.png
+-rw-r--r--   0        0        0     1332 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f331.png
+-rw-r--r--   0        0        0     2597 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f332.png
+-rw-r--r--   0        0        0     2484 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f333.png
+-rw-r--r--   0        0        0     3072 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f334.png
+-rw-r--r--   0        0        0     2572 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f335.png
+-rw-r--r--   0        0        0     1845 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f336.png
+-rw-r--r--   0        0        0     3135 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f337.png
+-rw-r--r--   0        0        0     3604 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f338.png
+-rw-r--r--   0        0        0     2576 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f339.png
+-rw-r--r--   0        0        0     3826 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f33a.png
+-rw-r--r--   0        0        0     2868 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f33b.png
+-rw-r--r--   0        0        0     2956 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f33c.png
+-rw-r--r--   0        0        0     3578 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f33d.png
+-rw-r--r--   0        0        0     3449 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f33e.png
+-rw-r--r--   0        0        0     2049 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f33f.png
+-rw-r--r--   0        0        0     3051 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f340.png
+-rw-r--r--   0        0        0     2961 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f341.png
+-rw-r--r--   0        0        0     2139 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f342.png
+-rw-r--r--   0        0        0     2318 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f343.png
+-rw-r--r--   0        0        0     2132 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f344.png
+-rw-r--r--   0        0        0     2412 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f345.png
+-rw-r--r--   0        0        0     1652 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f346.png
+-rw-r--r--   0        0        0     3397 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f347.png
+-rw-r--r--   0        0        0     2312 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f348.png
+-rw-r--r--   0        0        0     1901 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f349.png
+-rw-r--r--   0        0        0     2540 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f34a.png
+-rw-r--r--   0        0        0     2346 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f34b.png
+-rw-r--r--   0        0        0     2330 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f34c.png
+-rw-r--r--   0        0        0     3133 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f34d.png
+-rw-r--r--   0        0        0     2045 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f34e.png
+-rw-r--r--   0        0        0     1960 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f34f.png
+-rw-r--r--   0        0        0     1295 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f350.png
+-rw-r--r--   0        0        0     2750 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f351.png
+-rw-r--r--   0        0        0     2440 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f352.png
+-rw-r--r--   0        0        0     3080 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f353.png
+-rw-r--r--   0        0        0     3804 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f354.png
+-rw-r--r--   0        0        0     2094 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f355.png
+-rw-r--r--   0        0        0     2512 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f356.png
+-rw-r--r--   0        0        0     1660 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f357.png
+-rw-r--r--   0        0        0     2273 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f358.png
+-rw-r--r--   0        0        0     2050 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f359.png
+-rw-r--r--   0        0        0     1857 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f35a.png
+-rw-r--r--   0        0        0     2172 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f35b.png
+-rw-r--r--   0        0        0     3130 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f35c.png
+-rw-r--r--   0        0        0     2982 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f35d.png
+-rw-r--r--   0        0        0     1849 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f35e.png
+-rw-r--r--   0        0        0     2730 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f35f.png
+-rw-r--r--   0        0        0     1949 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f360.png
+-rw-r--r--   0        0        0     2058 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f361.png
+-rw-r--r--   0        0        0     1834 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f362.png
+-rw-r--r--   0        0        0     2825 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f363.png
+-rw-r--r--   0        0        0     3028 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f364.png
+-rw-r--r--   0        0        0     1761 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f365.png
+-rw-r--r--   0        0        0     1748 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f366.png
+-rw-r--r--   0        0        0     2335 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f367.png
+-rw-r--r--   0        0        0     2337 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f368.png
+-rw-r--r--   0        0        0     4358 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f369.png
+-rw-r--r--   0        0        0     2375 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f36a.png
+-rw-r--r--   0        0        0     1498 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f36b.png
+-rw-r--r--   0        0        0     2528 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f36c.png
+-rw-r--r--   0        0        0     2993 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f36d.png
+-rw-r--r--   0        0        0     1876 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f36e.png
+-rw-r--r--   0        0        0     3145 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f36f.png
+-rw-r--r--   0        0        0     2091 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f370.png
+-rw-r--r--   0        0        0     4187 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f371.png
+-rw-r--r--   0        0        0     2229 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f372.png
+-rw-r--r--   0        0        0     2053 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f373.png
+-rw-r--r--   0        0        0     1571 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f374.png
+-rw-r--r--   0        0        0     2237 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f375.png
+-rw-r--r--   0        0        0     1653 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f376.png
+-rw-r--r--   0        0        0     1820 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f377.png
+-rw-r--r--   0        0        0     2130 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f378.png
+-rw-r--r--   0        0        0     2815 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f379.png
+-rw-r--r--   0        0        0     3064 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f37a.png
+-rw-r--r--   0        0        0     3070 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f37b.png
+-rw-r--r--   0        0        0     1840 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f37c.png
+-rw-r--r--   0        0        0     2200 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f37d.png
+-rw-r--r--   0        0        0     2490 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f37e.png
+-rw-r--r--   0        0        0     3063 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f37f.png
+-rw-r--r--   0        0        0     2216 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f380.png
+-rw-r--r--   0        0        0     2290 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f381.png
+-rw-r--r--   0        0        0     2452 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f382.png
+-rw-r--r--   0        0        0     1957 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f383.png
+-rw-r--r--   0        0        0     3064 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f384.png
+-rw-r--r--   0        0        0     3193 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f385.png
+-rw-r--r--   0        0        0     2478 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f386.png
+-rw-r--r--   0        0        0     2644 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f387.png
+-rw-r--r--   0        0        0     1412 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f388.png
+-rw-r--r--   0        0        0     3725 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f389.png
+-rw-r--r--   0        0        0     3748 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f38a.png
+-rw-r--r--   0        0        0     2909 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f38b.png
+-rw-r--r--   0        0        0     2120 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f38c.png
+-rw-r--r--   0        0        0     2268 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f38d.png
+-rw-r--r--   0        0        0     3885 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f38e.png
+-rw-r--r--   0        0        0    13409 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f38f.png
+-rw-r--r--   0        0        0     2158 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f390.png
+-rw-r--r--   0        0        0     3030 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f391.png
+-rw-r--r--   0        0        0     2593 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f392.png
+-rw-r--r--   0        0        0     1595 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f393.png
+-rw-r--r--   0        0        0     1673 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f396.png
+-rw-r--r--   0        0        0     1273 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f397.png
+-rw-r--r--   0        0        0     2738 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f399.png
+-rw-r--r--   0        0        0     1254 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f39a.png
+-rw-r--r--   0        0        0     2214 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f39b.png
+-rw-r--r--   0        0        0     2621 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f39e.png
+-rw-r--r--   0        0        0     1459 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f39f.png
+-rw-r--r--   0        0        0     3774 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3a0.png
+-rw-r--r--   0        0        0     3756 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3a1.png
+-rw-r--r--   0        0        0     2888 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3a2.png
+-rw-r--r--   0        0        0     3092 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3a3.png
+-rw-r--r--   0        0        0     1510 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3a4.png
+-rw-r--r--   0        0        0     2437 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3a5.png
+-rw-r--r--   0        0        0     1101 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3a6.png
+-rw-r--r--   0        0        0     2400 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3a7.png
+-rw-r--r--   0        0        0     3744 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3a8.png
+-rw-r--r--   0        0        0     1380 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3a9.png
+-rw-r--r--   0        0        0     3014 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3aa.png
+-rw-r--r--   0        0        0     1519 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ab.png
+-rw-r--r--   0        0        0     1679 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ac.png
+-rw-r--r--   0        0        0     3610 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ad.png
+-rw-r--r--   0        0        0     2008 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ae.png
+-rw-r--r--   0        0        0     2799 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3af.png
+-rw-r--r--   0        0        0     2850 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3b0.png
+-rw-r--r--   0        0        0     1685 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3b1.png
+-rw-r--r--   0        0        0     1690 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3b2.png
+-rw-r--r--   0        0        0     2574 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3b3.png
+-rw-r--r--   0        0        0     1297 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3b4.png
+-rw-r--r--   0        0        0      989 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3b5.png
+-rw-r--r--   0        0        0     1731 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3b6.png
+-rw-r--r--   0        0        0     2673 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3b7.png
+-rw-r--r--   0        0        0     2595 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3b8.png
+-rw-r--r--   0        0        0     1147 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3b9.png
+-rw-r--r--   0        0        0     3202 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ba.png
+-rw-r--r--   0        0        0     3440 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3bb.png
+-rw-r--r--   0        0        0     1461 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3bc.png
+-rw-r--r--   0        0        0     1974 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3bd.png
+-rw-r--r--   0        0        0     2114 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3be.png
+-rw-r--r--   0        0        0     3507 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3bf.png
+-rw-r--r--   0        0        0     3092 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c0.png
+-rw-r--r--   0        0        0     1384 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c1.png
+-rw-r--r--   0        0        0     3205 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c2.png
+-rw-r--r--   0        0        0     2226 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c3.png
+-rw-r--r--   0        0        0     2518 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c3_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2449 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c3_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3228 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c4.png
+-rw-r--r--   0        0        0     3265 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c4_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3181 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c4_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2901 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c5.png
+-rw-r--r--   0        0        0     2765 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c6.png
+-rw-r--r--   0        0        0     2834 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c7.png
+-rw-r--r--   0        0        0     2681 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c8.png
+-rw-r--r--   0        0        0     2430 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c9.png
+-rw-r--r--   0        0        0     2697 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ca.png
+-rw-r--r--   0        0        0     3074 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ca_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2879 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ca_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3446 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3cb.png
+-rw-r--r--   0        0        0     3400 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3cb_fe0f_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3505 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3cb_fe0f_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2121 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3cc.png
+-rw-r--r--   0        0        0     2502 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3cc_fe0f_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2612 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3cc_fe0f_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2485 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3cd.png
+-rw-r--r--   0        0        0     2826 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ce.png
+-rw-r--r--   0        0        0     1908 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3cf.png
+-rw-r--r--   0        0        0     1724 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3d0.png
+-rw-r--r--   0        0        0     1866 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3d1.png
+-rw-r--r--   0        0        0     1758 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3d2.png
+-rw-r--r--   0        0        0     2481 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3d3.png
+-rw-r--r--   0        0        0     3018 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3d4.png
+-rw-r--r--   0        0        0     2698 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3d5.png
+-rw-r--r--   0        0        0     3183 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3d6.png
+-rw-r--r--   0        0        0     3121 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3d7.png
+-rw-r--r--   0        0        0     3021 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3d8.png
+-rw-r--r--   0        0        0     1628 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3d9.png
+-rw-r--r--   0        0        0     2752 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3da.png
+-rw-r--r--   0        0        0     2060 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3db.png
+-rw-r--r--   0        0        0     3123 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3dc.png
+-rw-r--r--   0        0        0     3133 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3dd.png
+-rw-r--r--   0        0        0     2371 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3de.png
+-rw-r--r--   0        0        0     4049 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3df.png
+-rw-r--r--   0        0        0     2364 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3e0.png
+-rw-r--r--   0        0        0     2954 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3e1.png
+-rw-r--r--   0        0        0     2241 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3e2.png
+-rw-r--r--   0        0        0     2318 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3e3.png
+-rw-r--r--   0        0        0     2654 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3e4.png
+-rw-r--r--   0        0        0     1880 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3e5.png
+-rw-r--r--   0        0        0     2564 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3e6.png
+-rw-r--r--   0        0        0     1142 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3e7.png
+-rw-r--r--   0        0        0     2990 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3e8.png
+-rw-r--r--   0        0        0     3226 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3e9.png
+-rw-r--r--   0        0        0     2202 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ea.png
+-rw-r--r--   0        0        0     2239 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3eb.png
+-rw-r--r--   0        0        0     2206 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ec.png
+-rw-r--r--   0        0        0     2448 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ed.png
+-rw-r--r--   0        0        0     1482 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ee.png
+-rw-r--r--   0        0        0     2396 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ef.png
+-rw-r--r--   0        0        0     3103 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f0.png
+-rw-r--r--   0        0        0      848 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f3.png
+-rw-r--r--   0        0        0     1471 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f3_fe0f_200d_1f308.png
+-rw-r--r--   0        0        0     1389 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f3_fe0f_200d_26a7_fe0f.png
+-rw-r--r--   0        0        0      761 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f4.png
+-rw-r--r--   0        0        0     1096 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f4_200d_2620_fe0f.png
+-rw-r--r--   0        0        0     1283 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f4_e0067_e0062_e0065_e006e_e0067_e007f.png
+-rw-r--r--   0        0        0     1451 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f4_e0067_e0062_e0073_e0063_e0074_e007f.png
+-rw-r--r--   0        0        0     2115 2022-11-18 15:36:28.448585 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f4_e0067_e0062_e0077_e006c_e0073_e007f.png
+-rw-r--r--   0        0        0     4095 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f5.png
+-rw-r--r--   0        0        0      495 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f7.png
+-rw-r--r--   0        0        0     3310 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f8.png
+-rw-r--r--   0        0        0     2605 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f9.png
+-rw-r--r--   0        0        0     2936 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f3fa.png
+-rw-r--r--   0        0        0     1698 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f400.png
+-rw-r--r--   0        0        0     2505 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f401.png
+-rw-r--r--   0        0        0     1710 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f402.png
+-rw-r--r--   0        0        0     1549 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f403.png
+-rw-r--r--   0        0        0     2271 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f404.png
+-rw-r--r--   0        0        0     3086 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f405.png
+-rw-r--r--   0        0        0     2863 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f406.png
+-rw-r--r--   0        0        0     1741 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f407.png
+-rw-r--r--   0        0        0     2893 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f408.png
+-rw-r--r--   0        0        0     1511 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f408_200d_2b1b.png
+-rw-r--r--   0        0        0     4191 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f409.png
+-rw-r--r--   0        0        0     2749 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f40a.png
+-rw-r--r--   0        0        0     2014 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f40b.png
+-rw-r--r--   0        0        0     3036 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f40c.png
+-rw-r--r--   0        0        0     2917 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f40d.png
+-rw-r--r--   0        0        0     2236 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f40e.png
+-rw-r--r--   0        0        0     2169 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f40f.png
+-rw-r--r--   0        0        0     1862 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f410.png
+-rw-r--r--   0        0        0     1931 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f411.png
+-rw-r--r--   0        0        0     2556 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f412.png
+-rw-r--r--   0        0        0     2453 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f413.png
+-rw-r--r--   0        0        0     2304 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f414.png
+-rw-r--r--   0        0        0     2328 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f415.png
+-rw-r--r--   0        0        0     2326 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f415_200d_1f9ba.png
+-rw-r--r--   0        0        0     1591 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f416.png
+-rw-r--r--   0        0        0     1773 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f417.png
+-rw-r--r--   0        0        0     1699 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f418.png
+-rw-r--r--   0        0        0     2151 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f419.png
+-rw-r--r--   0        0        0     1983 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f41a.png
+-rw-r--r--   0        0        0     3478 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f41b.png
+-rw-r--r--   0        0        0     2245 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f41c.png
+-rw-r--r--   0        0        0     3566 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f41d.png
+-rw-r--r--   0        0        0     3427 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f41e.png
+-rw-r--r--   0        0        0     1868 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f41f.png
+-rw-r--r--   0        0        0     3171 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f420.png
+-rw-r--r--   0        0        0     3511 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f421.png
+-rw-r--r--   0        0        0     2029 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f422.png
+-rw-r--r--   0        0        0     2750 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f423.png
+-rw-r--r--   0        0        0     1385 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f424.png
+-rw-r--r--   0        0        0     2506 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f425.png
+-rw-r--r--   0        0        0     1535 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f426.png
+-rw-r--r--   0        0        0     1612 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f427.png
+-rw-r--r--   0        0        0     1805 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f428.png
+-rw-r--r--   0        0        0     2137 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f429.png
+-rw-r--r--   0        0        0     1655 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f42a.png
+-rw-r--r--   0        0        0     2229 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f42b.png
+-rw-r--r--   0        0        0     2182 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f42c.png
+-rw-r--r--   0        0        0     2063 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f42d.png
+-rw-r--r--   0        0        0     2011 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f42e.png
+-rw-r--r--   0        0        0     3152 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f42f.png
+-rw-r--r--   0        0        0     1994 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f430.png
+-rw-r--r--   0        0        0     2193 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f431.png
+-rw-r--r--   0        0        0     4538 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f432.png
+-rw-r--r--   0        0        0     2468 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f433.png
+-rw-r--r--   0        0        0     2249 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f434.png
+-rw-r--r--   0        0        0     2358 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f435.png
+-rw-r--r--   0        0        0     2210 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f436.png
+-rw-r--r--   0        0        0     2307 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f437.png
+-rw-r--r--   0        0        0     3023 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f438.png
+-rw-r--r--   0        0        0     2911 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f439.png
+-rw-r--r--   0        0        0     1848 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f43a.png
+-rw-r--r--   0        0        0     1870 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f43b.png
+-rw-r--r--   0        0        0     1802 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f43b_200d_2744_fe0f.png
+-rw-r--r--   0        0        0     1740 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f43c.png
+-rw-r--r--   0        0        0     1528 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f43d.png
+-rw-r--r--   0        0        0      771 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f43e.png
+-rw-r--r--   0        0        0     3248 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f43f.png
+-rw-r--r--   0        0        0     1237 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f440.png
+-rw-r--r--   0        0        0     2158 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f441.png
+-rw-r--r--   0        0        0     1409 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f441_fe0f_200d_1f5e8_fe0f.png
+-rw-r--r--   0        0        0     1291 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f442.png
+-rw-r--r--   0        0        0     1094 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f443.png
+-rw-r--r--   0        0        0     1491 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f444.png
+-rw-r--r--   0        0        0     1666 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f445.png
+-rw-r--r--   0        0        0     1054 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f446.png
+-rw-r--r--   0        0        0     1039 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f447.png
+-rw-r--r--   0        0        0      972 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f448.png
+-rw-r--r--   0        0        0      959 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f449.png
+-rw-r--r--   0        0        0     1180 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f44a.png
+-rw-r--r--   0        0        0     1977 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f44b.png
+-rw-r--r--   0        0        0     1488 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f44c.png
+-rw-r--r--   0        0        0     1454 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f44d.png
+-rw-r--r--   0        0        0     1423 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f44e.png
+-rw-r--r--   0        0        0     1748 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f44f.png
+-rw-r--r--   0        0        0     1459 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f450.png
+-rw-r--r--   0        0        0     3262 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f451.png
+-rw-r--r--   0        0        0     2519 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f452.png
+-rw-r--r--   0        0        0     1157 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f453.png
+-rw-r--r--   0        0        0     2735 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f454.png
+-rw-r--r--   0        0        0     1489 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f455.png
+-rw-r--r--   0        0        0     2568 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f456.png
+-rw-r--r--   0        0        0     1811 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f457.png
+-rw-r--r--   0        0        0     3086 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f458.png
+-rw-r--r--   0        0        0     2700 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f459.png
+-rw-r--r--   0        0        0     1671 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f45a.png
+-rw-r--r--   0        0        0     1638 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f45b.png
+-rw-r--r--   0        0        0     2326 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f45c.png
+-rw-r--r--   0        0        0     1758 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f45d.png
+-rw-r--r--   0        0        0     2073 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f45e.png
+-rw-r--r--   0        0        0     1529 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f45f.png
+-rw-r--r--   0        0        0     2329 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f460.png
+-rw-r--r--   0        0        0     1465 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f461.png
+-rw-r--r--   0        0        0     1526 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f462.png
+-rw-r--r--   0        0        0      806 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f463.png
+-rw-r--r--   0        0        0      905 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f464.png
+-rw-r--r--   0        0        0     1012 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f465.png
+-rw-r--r--   0        0        0     2126 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f466.png
+-rw-r--r--   0        0        0     2215 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f467.png
+-rw-r--r--   0        0        0     2023 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468.png
+-rw-r--r--   0        0        0     4097 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f33e.png
+-rw-r--r--   0        0        0     2906 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f373.png
+-rw-r--r--   0        0        0     2948 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f37c.png
+-rw-r--r--   0        0        0     2403 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f393.png
+-rw-r--r--   0        0        0     3325 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f3a4.png
+-rw-r--r--   0        0        0     3552 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f3a8.png
+-rw-r--r--   0        0        0     2669 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f3eb.png
+-rw-r--r--   0        0        0     3239 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f3ed.png
+-rw-r--r--   0        0        0     2498 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f466.png
+-rw-r--r--   0        0        0     2694 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f466_200d_1f466.png
+-rw-r--r--   0        0        0     2644 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f467.png
+-rw-r--r--   0        0        0     3625 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f467_200d_1f466.png
+-rw-r--r--   0        0        0     3062 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f467_200d_1f467.png
+-rw-r--r--   0        0        0     3524 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f466.png
+-rw-r--r--   0        0        0     4079 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f466_200d_1f466.png
+-rw-r--r--   0        0        0     3727 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f467.png
+-rw-r--r--   0        0        0     4567 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f467_200d_1f466.png
+-rw-r--r--   0        0        0     4614 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f467_200d_1f467.png
+-rw-r--r--   0        0        0     3437 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f466.png
+-rw-r--r--   0        0        0     4310 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f466_200d_1f466.png
+-rw-r--r--   0        0        0     3696 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f467.png
+-rw-r--r--   0        0        0     4734 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f467_200d_1f466.png
+-rw-r--r--   0        0        0     4600 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f467_200d_1f467.png
+-rw-r--r--   0        0        0     1895 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f4bb.png
+-rw-r--r--   0        0        0     2409 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f4bc.png
+-rw-r--r--   0        0        0     3178 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f527.png
+-rw-r--r--   0        0        0     3350 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f52c.png
+-rw-r--r--   0        0        0     3231 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f680.png
+-rw-r--r--   0        0        0     3740 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f692.png
+-rw-r--r--   0        0        0     2564 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f9af.png
+-rw-r--r--   0        0        0     2081 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f9b0.png
+-rw-r--r--   0        0        0     2301 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f9b1.png
+-rw-r--r--   0        0        0     1717 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f9b2.png
+-rw-r--r--   0        0        0     1968 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f9b3.png
+-rw-r--r--   0        0        0     3029 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f9bc.png
+-rw-r--r--   0        0        0     2477 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f9bd.png
+-rw-r--r--   0        0        0     2561 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_2695_fe0f.png
+-rw-r--r--   0        0        0     2680 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_2696_fe0f.png
+-rw-r--r--   0        0        0     2660 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_2708_fe0f.png
+-rw-r--r--   0        0        0     3289 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_2764_fe0f_200d_1f468.png
+-rw-r--r--   0        0        0     2437 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_2764_fe0f_200d_1f48b_200d_1f468.png
+-rw-r--r--   0        0        0     2497 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469.png
+-rw-r--r--   0        0        0     4126 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f33e.png
+-rw-r--r--   0        0        0     3312 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f373.png
+-rw-r--r--   0        0        0     2951 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f37c.png
+-rw-r--r--   0        0        0     2659 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f393.png
+-rw-r--r--   0        0        0     3648 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f3a4.png
+-rw-r--r--   0        0        0     3778 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f3a8.png
+-rw-r--r--   0        0        0     2988 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f3eb.png
+-rw-r--r--   0        0        0     3394 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f3ed.png
+-rw-r--r--   0        0        0     2519 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f466.png
+-rw-r--r--   0        0        0     2793 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f466_200d_1f466.png
+-rw-r--r--   0        0        0     2718 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f467.png
+-rw-r--r--   0        0        0     3700 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f467_200d_1f466.png
+-rw-r--r--   0        0        0     3174 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f467_200d_1f467.png
+-rw-r--r--   0        0        0     3363 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f466.png
+-rw-r--r--   0        0        0     3984 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f466_200d_1f466.png
+-rw-r--r--   0        0        0     3860 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f467.png
+-rw-r--r--   0        0        0     4626 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f467_200d_1f466.png
+-rw-r--r--   0        0        0     4582 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f467_200d_1f467.png
+-rw-r--r--   0        0        0     2002 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f4bb.png
+-rw-r--r--   0        0        0     2411 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f4bc.png
+-rw-r--r--   0        0        0     3131 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f527.png
+-rw-r--r--   0        0        0     3659 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f52c.png
+-rw-r--r--   0        0        0     3150 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f680.png
+-rw-r--r--   0        0        0     3773 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f692.png
+-rw-r--r--   0        0        0     2532 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f9af.png
+-rw-r--r--   0        0        0     2294 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f9b0.png
+-rw-r--r--   0        0        0     2744 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f9b1.png
+-rw-r--r--   0        0        0     1749 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f9b2.png
+-rw-r--r--   0        0        0     2475 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f9b3.png
+-rw-r--r--   0        0        0     3044 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f9bc.png
+-rw-r--r--   0        0        0     2575 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f9bd.png
+-rw-r--r--   0        0        0     2722 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_2695_fe0f.png
+-rw-r--r--   0        0        0     2543 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_2696_fe0f.png
+-rw-r--r--   0        0        0     2931 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_2708_fe0f.png
+-rw-r--r--   0        0        0     3634 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f468.png
+-rw-r--r--   0        0        0     3993 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f469.png
+-rw-r--r--   0        0        0     2908 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f48b_200d_1f468.png
+-rw-r--r--   0        0        0     2986 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f48b_200d_1f469.png
+-rw-r--r--   0        0        0     3110 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f46a.png
+-rw-r--r--   0        0        0     3563 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f46b.png
+-rw-r--r--   0        0        0     3481 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f46c.png
+-rw-r--r--   0        0        0     3729 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f46d.png
+-rw-r--r--   0        0        0     3074 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f46e.png
+-rw-r--r--   0        0        0     3026 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f46e_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3184 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f46e_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2773 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f46f.png
+-rw-r--r--   0        0        0     3282 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f46f_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2849 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f46f_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2859 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f470.png
+-rw-r--r--   0        0        0     2914 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f470_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2994 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f470_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2408 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f471.png
+-rw-r--r--   0        0        0     2558 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f471_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     1962 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f471_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2225 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f472.png
+-rw-r--r--   0        0        0     2279 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f473.png
+-rw-r--r--   0        0        0     2127 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f473_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2497 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f473_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2160 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f474.png
+-rw-r--r--   0        0        0     2445 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f475.png
+-rw-r--r--   0        0        0     2198 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f476.png
+-rw-r--r--   0        0        0     3221 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f477.png
+-rw-r--r--   0        0        0     3455 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f477_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3157 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f477_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2492 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f478.png
+-rw-r--r--   0        0        0     3442 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f479.png
+-rw-r--r--   0        0        0     2863 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f47a.png
+-rw-r--r--   0        0        0     2131 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f47b.png
+-rw-r--r--   0        0        0     2657 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f47c.png
+-rw-r--r--   0        0        0     1689 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f47d.png
+-rw-r--r--   0        0        0     1189 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f47e.png
+-rw-r--r--   0        0        0     2312 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f47f.png
+-rw-r--r--   0        0        0     1705 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f480.png
+-rw-r--r--   0        0        0     2539 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f481.png
+-rw-r--r--   0        0        0     2759 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f481_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2232 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f481_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2667 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f482.png
+-rw-r--r--   0        0        0     2451 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f482_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2572 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f482_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3554 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f483.png
+-rw-r--r--   0        0        0     1511 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f484.png
+-rw-r--r--   0        0        0     2498 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f485.png
+-rw-r--r--   0        0        0     2577 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f486.png
+-rw-r--r--   0        0        0     2578 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f486_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2291 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f486_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2902 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f487.png
+-rw-r--r--   0        0        0     3136 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f487_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2768 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f487_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2127 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f488.png
+-rw-r--r--   0        0        0     1689 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f489.png
+-rw-r--r--   0        0        0     2073 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f48a.png
+-rw-r--r--   0        0        0     2182 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f48b.png
+-rw-r--r--   0        0        0     1041 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f48c.png
+-rw-r--r--   0        0        0     2384 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f48d.png
+-rw-r--r--   0        0        0     2358 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f48e.png
+-rw-r--r--   0        0        0     2590 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f48f.png
+-rw-r--r--   0        0        0    13813 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f490.png
+-rw-r--r--   0        0        0     3493 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f491.png
+-rw-r--r--   0        0        0     2163 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f492.png
+-rw-r--r--   0        0        0     1344 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f493.png
+-rw-r--r--   0        0        0     1561 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f494.png
+-rw-r--r--   0        0        0     1153 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f495.png
+-rw-r--r--   0        0        0     2111 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f496.png
+-rw-r--r--   0        0        0     1760 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f497.png
+-rw-r--r--   0        0        0     1985 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f498.png
+-rw-r--r--   0        0        0     1130 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f499.png
+-rw-r--r--   0        0        0     1209 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f49a.png
+-rw-r--r--   0        0        0     1168 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f49b.png
+-rw-r--r--   0        0        0     1112 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f49c.png
+-rw-r--r--   0        0        0     2849 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f49d.png
+-rw-r--r--   0        0        0     1678 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f49e.png
+-rw-r--r--   0        0        0     1082 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f49f.png
+-rw-r--r--   0        0        0     2790 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4a0.png
+-rw-r--r--   0        0        0     1218 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4a1.png
+-rw-r--r--   0        0        0     1301 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4a2.png
+-rw-r--r--   0        0        0     2163 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4a3.png
+-rw-r--r--   0        0        0      663 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4a4.png
+-rw-r--r--   0        0        0     2101 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4a5.png
+-rw-r--r--   0        0        0     1905 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4a6.png
+-rw-r--r--   0        0        0     1268 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4a7.png
+-rw-r--r--   0        0        0     1661 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4a8.png
+-rw-r--r--   0        0        0     1782 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4a9.png
+-rw-r--r--   0        0        0     1393 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4aa.png
+-rw-r--r--   0        0        0     1890 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ab.png
+-rw-r--r--   0        0        0     1244 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ac.png
+-rw-r--r--   0        0        0     1370 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ad.png
+-rw-r--r--   0        0        0     1790 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ae.png
+-rw-r--r--   0        0        0     1447 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4af.png
+-rw-r--r--   0        0        0     2079 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4b0.png
+-rw-r--r--   0        0        0      996 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4b1.png
+-rw-r--r--   0        0        0      731 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4b2.png
+-rw-r--r--   0        0        0     1261 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4b3.png
+-rw-r--r--   0        0        0     2017 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4b4.png
+-rw-r--r--   0        0        0     2022 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4b5.png
+-rw-r--r--   0        0        0     2210 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4b6.png
+-rw-r--r--   0        0        0     1974 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4b7.png
+-rw-r--r--   0        0        0     3067 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4b8.png
+-rw-r--r--   0        0        0     1480 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4b9.png
+-rw-r--r--   0        0        0     2448 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ba.png
+-rw-r--r--   0        0        0     1176 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4bb.png
+-rw-r--r--   0        0        0     1748 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4bc.png
+-rw-r--r--   0        0        0     2198 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4bd.png
+-rw-r--r--   0        0        0      907 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4be.png
+-rw-r--r--   0        0        0     2244 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4bf.png
+-rw-r--r--   0        0        0     2307 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4c0.png
+-rw-r--r--   0        0        0     1335 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4c1.png
+-rw-r--r--   0        0        0     1241 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4c2.png
+-rw-r--r--   0        0        0     1241 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4c3.png
+-rw-r--r--   0        0        0     1257 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4c4.png
+-rw-r--r--   0        0        0     1046 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4c5.png
+-rw-r--r--   0        0        0     1568 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4c6.png
+-rw-r--r--   0        0        0     2054 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4c7.png
+-rw-r--r--   0        0        0     1861 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4c8.png
+-rw-r--r--   0        0        0     1762 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4c9.png
+-rw-r--r--   0        0        0     1723 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ca.png
+-rw-r--r--   0        0        0     1189 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4cb.png
+-rw-r--r--   0        0        0     2156 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4cc.png
+-rw-r--r--   0        0        0     1466 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4cd.png
+-rw-r--r--   0        0        0     2382 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ce.png
+-rw-r--r--   0        0        0      803 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4cf.png
+-rw-r--r--   0        0        0      935 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4d0.png
+-rw-r--r--   0        0        0     1723 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4d1.png
+-rw-r--r--   0        0        0     2351 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4d2.png
+-rw-r--r--   0        0        0     2386 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4d3.png
+-rw-r--r--   0        0        0     1766 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4d4.png
+-rw-r--r--   0        0        0     1593 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4d5.png
+-rw-r--r--   0        0        0     2091 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4d6.png
+-rw-r--r--   0        0        0     1470 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4d7.png
+-rw-r--r--   0        0        0     1661 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4d8.png
+-rw-r--r--   0        0        0     1807 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4d9.png
+-rw-r--r--   0        0        0     2567 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4da.png
+-rw-r--r--   0        0        0     1381 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4db.png
+-rw-r--r--   0        0        0     2294 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4dc.png
+-rw-r--r--   0        0        0     2169 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4dd.png
+-rw-r--r--   0        0        0     1086 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4de.png
+-rw-r--r--   0        0        0     1650 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4df.png
+-rw-r--r--   0        0        0     1045 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4e0.png
+-rw-r--r--   0        0        0     2446 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4e1.png
+-rw-r--r--   0        0        0     1759 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4e2.png
+-rw-r--r--   0        0        0     2230 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4e3.png
+-rw-r--r--   0        0        0     1412 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4e4.png
+-rw-r--r--   0        0        0     1396 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4e5.png
+-rw-r--r--   0        0        0     1493 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4e6.png
+-rw-r--r--   0        0        0     1113 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4e7.png
+-rw-r--r--   0        0        0     1712 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4e8.png
+-rw-r--r--   0        0        0     1223 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4e9.png
+-rw-r--r--   0        0        0     1854 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ea.png
+-rw-r--r--   0        0        0     2096 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4eb.png
+-rw-r--r--   0        0        0     2146 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ec.png
+-rw-r--r--   0        0        0     1703 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ed.png
+-rw-r--r--   0        0        0     1507 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ee.png
+-rw-r--r--   0        0        0     2827 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ef.png
+-rw-r--r--   0        0        0     2109 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4f0.png
+-rw-r--r--   0        0        0     1517 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4f1.png
+-rw-r--r--   0        0        0     1869 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4f2.png
+-rw-r--r--   0        0        0     1436 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4f3.png
+-rw-r--r--   0        0        0     1432 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4f4.png
+-rw-r--r--   0        0        0     1809 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4f5.png
+-rw-r--r--   0        0        0     1014 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4f6.png
+-rw-r--r--   0        0        0     1722 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4f7.png
+-rw-r--r--   0        0        0     2671 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4f8.png
+-rw-r--r--   0        0        0     1917 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4f9.png
+-rw-r--r--   0        0        0     2416 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4fa.png
+-rw-r--r--   0        0        0     1837 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4fb.png
+-rw-r--r--   0        0        0     1155 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4fc.png
+-rw-r--r--   0        0        0     2361 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4fd.png
+-rw-r--r--   0        0        0     2542 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ff.png
+-rw-r--r--   0        0        0     1165 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f500.png
+-rw-r--r--   0        0        0     1196 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f501.png
+-rw-r--r--   0        0        0     1260 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f502.png
+-rw-r--r--   0        0        0     1258 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f503.png
+-rw-r--r--   0        0        0     1313 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f504.png
+-rw-r--r--   0        0        0     1209 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f505.png
+-rw-r--r--   0        0        0     1611 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f506.png
+-rw-r--r--   0        0        0     2099 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f507.png
+-rw-r--r--   0        0        0     1884 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f508.png
+-rw-r--r--   0        0        0     2513 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f509.png
+-rw-r--r--   0        0        0     3375 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f50a.png
+-rw-r--r--   0        0        0     2030 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f50b.png
+-rw-r--r--   0        0        0     1447 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f50c.png
+-rw-r--r--   0        0        0     1931 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f50d.png
+-rw-r--r--   0        0        0     2090 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f50e.png
+-rw-r--r--   0        0        0     2493 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f50f.png
+-rw-r--r--   0        0        0     2190 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f510.png
+-rw-r--r--   0        0        0     1672 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f511.png
+-rw-r--r--   0        0        0     1356 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f512.png
+-rw-r--r--   0        0        0     1472 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f513.png
+-rw-r--r--   0        0        0     1922 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f514.png
+-rw-r--r--   0        0        0     2107 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f515.png
+-rw-r--r--   0        0        0     1450 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f516.png
+-rw-r--r--   0        0        0     2545 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f517.png
+-rw-r--r--   0        0        0     1393 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f518.png
+-rw-r--r--   0        0        0     1003 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f519.png
+-rw-r--r--   0        0        0      723 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f51a.png
+-rw-r--r--   0        0        0      949 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f51b.png
+-rw-r--r--   0        0        0     1086 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f51c.png
+-rw-r--r--   0        0        0      731 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f51d.png
+-rw-r--r--   0        0        0     2019 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f51e.png
+-rw-r--r--   0        0        0     1156 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f51f.png
+-rw-r--r--   0        0        0     1441 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f520.png
+-rw-r--r--   0        0        0     1340 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f521.png
+-rw-r--r--   0        0        0     1353 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f522.png
+-rw-r--r--   0        0        0     1398 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f523.png
+-rw-r--r--   0        0        0     1160 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f524.png
+-rw-r--r--   0        0        0     2128 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f525.png
+-rw-r--r--   0        0        0     1502 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f526.png
+-rw-r--r--   0        0        0     1216 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f527.png
+-rw-r--r--   0        0        0     1276 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f528.png
+-rw-r--r--   0        0        0     1853 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f529.png
+-rw-r--r--   0        0        0     1165 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f52a.png
+-rw-r--r--   0        0        0     2371 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f52b.png
+-rw-r--r--   0        0        0     2364 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f52c.png
+-rw-r--r--   0        0        0     2039 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f52d.png
+-rw-r--r--   0        0        0     3144 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f52e.png
+-rw-r--r--   0        0        0     1358 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f52f.png
+-rw-r--r--   0        0        0     1252 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f530.png
+-rw-r--r--   0        0        0     2726 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f531.png
+-rw-r--r--   0        0        0      733 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f532.png
+-rw-r--r--   0        0        0      531 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f533.png
+-rw-r--r--   0        0        0      961 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f534.png
+-rw-r--r--   0        0        0      952 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f535.png
+-rw-r--r--   0        0        0      780 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f536.png
+-rw-r--r--   0        0        0      847 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f537.png
+-rw-r--r--   0        0        0      668 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f538.png
+-rw-r--r--   0        0        0      719 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f539.png
+-rw-r--r--   0        0        0      566 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f53a.png
+-rw-r--r--   0        0        0      654 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f53b.png
+-rw-r--r--   0        0        0     1044 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f53c.png
+-rw-r--r--   0        0        0      972 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f53d.png
+-rw-r--r--   0        0        0     1553 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f549.png
+-rw-r--r--   0        0        0     1919 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f54a.png
+-rw-r--r--   0        0        0     1294 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f54b.png
+-rw-r--r--   0        0        0     2786 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f54c.png
+-rw-r--r--   0        0        0     2481 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f54d.png
+-rw-r--r--   0        0        0     1663 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f54e.png
+-rw-r--r--   0        0        0     1700 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f550.png
+-rw-r--r--   0        0        0     1660 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f551.png
+-rw-r--r--   0        0        0     1705 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f552.png
+-rw-r--r--   0        0        0     1748 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f553.png
+-rw-r--r--   0        0        0     1749 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f554.png
+-rw-r--r--   0        0        0     1687 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f555.png
+-rw-r--r--   0        0        0     1750 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f556.png
+-rw-r--r--   0        0        0     1767 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f557.png
+-rw-r--r--   0        0        0     1635 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f558.png
+-rw-r--r--   0        0        0     1645 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f559.png
+-rw-r--r--   0        0        0     1720 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f55a.png
+-rw-r--r--   0        0        0     1669 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f55b.png
+-rw-r--r--   0        0        0     1778 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f55c.png
+-rw-r--r--   0        0        0     1707 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f55d.png
+-rw-r--r--   0        0        0     1648 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f55e.png
+-rw-r--r--   0        0        0     1689 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f55f.png
+-rw-r--r--   0        0        0     1722 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f560.png
+-rw-r--r--   0        0        0     1694 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f561.png
+-rw-r--r--   0        0        0     1679 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f562.png
+-rw-r--r--   0        0        0     1717 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f563.png
+-rw-r--r--   0        0        0     1637 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f564.png
+-rw-r--r--   0        0        0     1619 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f565.png
+-rw-r--r--   0        0        0     1725 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f566.png
+-rw-r--r--   0        0        0     1678 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f567.png
+-rw-r--r--   0        0        0     2185 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f56f.png
+-rw-r--r--   0        0        0     2228 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f570.png
+-rw-r--r--   0        0        0      714 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f573.png
+-rw-r--r--   0        0        0     1301 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f574.png
+-rw-r--r--   0        0        0     3208 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f575.png
+-rw-r--r--   0        0        0     3188 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f575_fe0f_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3174 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f575_fe0f_200d_2642_fe0f.png
+-rw-r--r--   0        0        0      841 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f576.png
+-rw-r--r--   0        0        0     1848 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f577.png
+-rw-r--r--   0        0        0     2208 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f578.png
+-rw-r--r--   0        0        0     1401 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f579.png
+-rw-r--r--   0        0        0     2299 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f57a.png
+-rw-r--r--   0        0        0     3424 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f587.png
+-rw-r--r--   0        0        0     1232 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f58a.png
+-rw-r--r--   0        0        0     1662 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f58b.png
+-rw-r--r--   0        0        0     1928 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f58c.png
+-rw-r--r--   0        0        0     1260 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f58d.png
+-rw-r--r--   0        0        0     1529 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f590.png
+-rw-r--r--   0        0        0      871 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f595.png
+-rw-r--r--   0        0        0     1489 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f596.png
+-rw-r--r--   0        0        0     1165 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5a4.png
+-rw-r--r--   0        0        0      973 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5a5.png
+-rw-r--r--   0        0        0     1403 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5a8.png
+-rw-r--r--   0        0        0      761 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5b1.png
+-rw-r--r--   0        0        0     1783 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5b2.png
+-rw-r--r--   0        0        0     2515 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5bc.png
+-rw-r--r--   0        0        0      831 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5c2.png
+-rw-r--r--   0        0        0     1401 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5c3.png
+-rw-r--r--   0        0        0     1035 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5c4.png
+-rw-r--r--   0        0        0     4755 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5d1.png
+-rw-r--r--   0        0        0     1897 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5d2.png
+-rw-r--r--   0        0        0     2281 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5d3.png
+-rw-r--r--   0        0        0     2007 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5dc.png
+-rw-r--r--   0        0        0     1484 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5dd.png
+-rw-r--r--   0        0        0     2030 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5de.png
+-rw-r--r--   0        0        0     1129 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5e1.png
+-rw-r--r--   0        0        0     1137 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5e3.png
+-rw-r--r--   0        0        0      839 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5e8.png
+-rw-r--r--   0        0        0     1569 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5ef.png
+-rw-r--r--   0        0        0     1656 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5f3.png
+-rw-r--r--   0        0        0     4392 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5fa.png
+-rw-r--r--   0        0        0     1425 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5fb.png
+-rw-r--r--   0        0        0     2590 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5fc.png
+-rw-r--r--   0        0        0     2201 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5fd.png
+-rw-r--r--   0        0        0     1010 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5fe.png
+-rw-r--r--   0        0        0     1759 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f5ff.png
+-rw-r--r--   0        0        0     2044 2022-11-18 15:36:28.336582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f600.png
+-rw-r--r--   0        0        0     2219 2022-11-18 15:36:28.336582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f601.png
+-rw-r--r--   0        0        0     2808 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f602.png
+-rw-r--r--   0        0        0     2198 2022-11-18 15:36:28.336582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f603.png
+-rw-r--r--   0        0        0     2129 2022-11-18 15:36:28.336582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f604.png
+-rw-r--r--   0        0        0     2690 2022-11-18 15:36:28.336582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f605.png
+-rw-r--r--   0        0        0     2241 2022-11-18 15:36:28.336582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f606.png
+-rw-r--r--   0        0        0     3349 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f607.png
+-rw-r--r--   0        0        0     2347 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f608.png
+-rw-r--r--   0        0        0     1949 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f609.png
+-rw-r--r--   0        0        0     1964 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f60a.png
+-rw-r--r--   0        0        0     2305 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f60b.png
+-rw-r--r--   0        0        0     1922 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f60c.png
+-rw-r--r--   0        0        0     2417 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f60d.png
+-rw-r--r--   0        0        0     2129 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f60e.png
+-rw-r--r--   0        0        0     1855 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f60f.png
+-rw-r--r--   0        0        0     1777 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f610.png
+-rw-r--r--   0        0        0     1645 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f611.png
+-rw-r--r--   0        0        0     1865 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f612.png
+-rw-r--r--   0        0        0     2480 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f613.png
+-rw-r--r--   0        0        0     1794 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f614.png
+-rw-r--r--   0        0        0     1847 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f615.png
+-rw-r--r--   0        0        0     1950 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f616.png
+-rw-r--r--   0        0        0     1878 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f617.png
+-rw-r--r--   0        0        0     2543 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f618.png
+-rw-r--r--   0        0        0     2010 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f619.png
+-rw-r--r--   0        0        0     2040 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f61a.png
+-rw-r--r--   0        0        0     2093 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f61b.png
+-rw-r--r--   0        0        0     2563 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f61c.png
+-rw-r--r--   0        0        0     2292 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f61d.png
+-rw-r--r--   0        0        0     1764 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f61e.png
+-rw-r--r--   0        0        0     1962 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f61f.png
+-rw-r--r--   0        0        0     1809 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f620.png
+-rw-r--r--   0        0        0     1398 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f621.png
+-rw-r--r--   0        0        0     2477 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f622.png
+-rw-r--r--   0        0        0     1947 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f623.png
+-rw-r--r--   0        0        0     3109 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f624.png
+-rw-r--r--   0        0        0     2491 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f625.png
+-rw-r--r--   0        0        0     1691 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f626.png
+-rw-r--r--   0        0        0     1967 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f627.png
+-rw-r--r--   0        0        0     2236 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f628.png
+-rw-r--r--   0        0        0     2300 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f629.png
+-rw-r--r--   0        0        0     2659 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f62a.png
+-rw-r--r--   0        0        0     2376 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f62b.png
+-rw-r--r--   0        0        0     1959 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f62c.png
+-rw-r--r--   0        0        0     2464 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f62d.png
+-rw-r--r--   0        0        0     1681 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f62e.png
+-rw-r--r--   0        0        0     3413 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f62e_200d_1f4a8.png
+-rw-r--r--   0        0        0     1895 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f62f.png
+-rw-r--r--   0        0        0     2915 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f630.png
+-rw-r--r--   0        0        0     2986 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f631.png
+-rw-r--r--   0        0        0     2122 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f632.png
+-rw-r--r--   0        0        0     2367 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f633.png
+-rw-r--r--   0        0        0     2695 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f634.png
+-rw-r--r--   0        0        0     2059 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f635.png
+-rw-r--r--   0        0        0     3751 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f635_200d_1f4ab.png
+-rw-r--r--   0        0        0     1711 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f636.png
+-rw-r--r--   0        0        0     4477 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f636_200d_1f32b_fe0f.png
+-rw-r--r--   0        0        0     2431 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f637.png
+-rw-r--r--   0        0        0     2358 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f638.png
+-rw-r--r--   0        0        0     3507 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f639.png
+-rw-r--r--   0        0        0     2628 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f63a.png
+-rw-r--r--   0        0        0     2917 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f63b.png
+-rw-r--r--   0        0        0     2509 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f63c.png
+-rw-r--r--   0        0        0     2625 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f63d.png
+-rw-r--r--   0        0        0     2423 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f63e.png
+-rw-r--r--   0        0        0     2830 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f63f.png
+-rw-r--r--   0        0        0     3113 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f640.png
+-rw-r--r--   0        0        0     1784 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f641.png
+-rw-r--r--   0        0        0     1841 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f642.png
+-rw-r--r--   0        0        0     1804 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f643.png
+-rw-r--r--   0        0        0     2149 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f644.png
+-rw-r--r--   0        0        0     2762 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f645.png
+-rw-r--r--   0        0        0     2860 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f645_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3058 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f645_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3132 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f646.png
+-rw-r--r--   0        0        0     3051 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f646_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3260 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f646_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2497 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f647.png
+-rw-r--r--   0        0        0     2862 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f647_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2829 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f647_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2542 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f648.png
+-rw-r--r--   0        0        0     2640 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f649.png
+-rw-r--r--   0        0        0     2350 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f64a.png
+-rw-r--r--   0        0        0     2576 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f64b.png
+-rw-r--r--   0        0        0     2762 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f64b_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2406 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f64b_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     1918 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f64c.png
+-rw-r--r--   0        0        0     2133 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f64d.png
+-rw-r--r--   0        0        0     2384 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f64d_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     1984 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f64d_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2123 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f64e.png
+-rw-r--r--   0        0        0     2383 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f64e_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     1936 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f64e_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     1910 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f64f.png
+-rw-r--r--   0        0        0     3216 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f680.png
+-rw-r--r--   0        0        0     3045 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f681.png
+-rw-r--r--   0        0        0     3402 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f682.png
+-rw-r--r--   0        0        0     2144 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f683.png
+-rw-r--r--   0        0        0     2088 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f684.png
+-rw-r--r--   0        0        0     2044 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f685.png
+-rw-r--r--   0        0        0     2384 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f686.png
+-rw-r--r--   0        0        0     2168 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f687.png
+-rw-r--r--   0        0        0     1819 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f688.png
+-rw-r--r--   0        0        0     2106 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f689.png
+-rw-r--r--   0        0        0     1964 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f68a.png
+-rw-r--r--   0        0        0     1812 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f68b.png
+-rw-r--r--   0        0        0     2469 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f68c.png
+-rw-r--r--   0        0        0     2164 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f68d.png
+-rw-r--r--   0        0        0     3075 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f68e.png
+-rw-r--r--   0        0        0     1852 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f68f.png
+-rw-r--r--   0        0        0     2315 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f690.png
+-rw-r--r--   0        0        0     2769 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f691.png
+-rw-r--r--   0        0        0     2906 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f692.png
+-rw-r--r--   0        0        0     2109 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f693.png
+-rw-r--r--   0        0        0     2206 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f694.png
+-rw-r--r--   0        0        0     3166 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f695.png
+-rw-r--r--   0        0        0     2435 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f696.png
+-rw-r--r--   0        0        0     2501 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f697.png
+-rw-r--r--   0        0        0     2412 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f698.png
+-rw-r--r--   0        0        0     2429 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f699.png
+-rw-r--r--   0        0        0     2291 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f69a.png
+-rw-r--r--   0        0        0     2309 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f69b.png
+-rw-r--r--   0        0        0     2980 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f69c.png
+-rw-r--r--   0        0        0     1988 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f69d.png
+-rw-r--r--   0        0        0     3138 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f69e.png
+-rw-r--r--   0        0        0     2456 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f69f.png
+-rw-r--r--   0        0        0     2526 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a0.png
+-rw-r--r--   0        0        0     1735 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a1.png
+-rw-r--r--   0        0        0     2413 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a2.png
+-rw-r--r--   0        0        0     1966 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a3.png
+-rw-r--r--   0        0        0     2262 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a3_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2156 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a3_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2041 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a4.png
+-rw-r--r--   0        0        0     1795 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a5.png
+-rw-r--r--   0        0        0     2019 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a6.png
+-rw-r--r--   0        0        0     2554 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a7.png
+-rw-r--r--   0        0        0     2975 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a8.png
+-rw-r--r--   0        0        0      917 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a9.png
+-rw-r--r--   0        0        0      951 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6aa.png
+-rw-r--r--   0        0        0     2250 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6ab.png
+-rw-r--r--   0        0        0     1543 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6ac.png
+-rw-r--r--   0        0        0     1875 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6ad.png
+-rw-r--r--   0        0        0     1258 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6ae.png
+-rw-r--r--   0        0        0     1929 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6af.png
+-rw-r--r--   0        0        0     2641 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b0.png
+-rw-r--r--   0        0        0     1950 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b1.png
+-rw-r--r--   0        0        0     2702 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b2.png
+-rw-r--r--   0        0        0     2181 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b3.png
+-rw-r--r--   0        0        0     3994 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b4.png
+-rw-r--r--   0        0        0     3960 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b4_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3931 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b4_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     4126 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b5.png
+-rw-r--r--   0        0        0     4684 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b5_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     4495 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b5_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     1893 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b6.png
+-rw-r--r--   0        0        0     2212 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b6_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     1986 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b6_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2018 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b7.png
+-rw-r--r--   0        0        0     1190 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b8.png
+-rw-r--r--   0        0        0     1142 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b9.png
+-rw-r--r--   0        0        0     1170 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6ba.png
+-rw-r--r--   0        0        0     1251 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6bb.png
+-rw-r--r--   0        0        0     1188 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6bc.png
+-rw-r--r--   0        0        0     1173 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6bd.png
+-rw-r--r--   0        0        0     1457 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6be.png
+-rw-r--r--   0        0        0     2007 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6bf.png
+-rw-r--r--   0        0        0     2399 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6c0.png
+-rw-r--r--   0        0        0     2784 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6c1.png
+-rw-r--r--   0        0        0     1350 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6c2.png
+-rw-r--r--   0        0        0     1244 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6c3.png
+-rw-r--r--   0        0        0     1089 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6c4.png
+-rw-r--r--   0        0        0     1292 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6c5.png
+-rw-r--r--   0        0        0     1881 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6cb.png
+-rw-r--r--   0        0        0     1564 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6cc.png
+-rw-r--r--   0        0        0     4037 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6cd.png
+-rw-r--r--   0        0        0     2362 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6ce.png
+-rw-r--r--   0        0        0     1192 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6cf.png
+-rw-r--r--   0        0        0     1220 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6d0.png
+-rw-r--r--   0        0        0      875 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6d1.png
+-rw-r--r--   0        0        0     2699 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6d2.png
+-rw-r--r--   0        0        0     1632 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6d5.png
+-rw-r--r--   0        0        0     1632 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6d6.png
+-rw-r--r--   0        0        0     1243 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6d7.png
+-rw-r--r--   0        0        0     8111 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6dd.png
+-rw-r--r--   0        0        0     4305 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6de.png
+-rw-r--r--   0        0        0     3886 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6df.png
+-rw-r--r--   0        0        0     2317 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6e0.png
+-rw-r--r--   0        0        0     1601 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6e1.png
+-rw-r--r--   0        0        0     2017 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6e2.png
+-rw-r--r--   0        0        0     2352 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6e3.png
+-rw-r--r--   0        0        0     3595 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6e4.png
+-rw-r--r--   0        0        0     2267 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6e5.png
+-rw-r--r--   0        0        0     2443 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6e9.png
+-rw-r--r--   0        0        0     1908 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6eb.png
+-rw-r--r--   0        0        0     2282 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6ec.png
+-rw-r--r--   0        0        0     3617 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6f0.png
+-rw-r--r--   0        0        0     2329 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6f3.png
+-rw-r--r--   0        0        0     1741 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6f4.png
+-rw-r--r--   0        0        0     3308 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6f5.png
+-rw-r--r--   0        0        0     1926 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6f6.png
+-rw-r--r--   0        0        0     2647 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6f7.png
+-rw-r--r--   0        0        0     1416 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6f8.png
+-rw-r--r--   0        0        0     1452 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6f9.png
+-rw-r--r--   0        0        0     3549 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6fa.png
+-rw-r--r--   0        0        0     1981 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6fb.png
+-rw-r--r--   0        0        0     3566 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f6fc.png
+-rw-r--r--   0        0        0      911 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f7e0.png
+-rw-r--r--   0        0        0      949 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f7e1.png
+-rw-r--r--   0        0        0      857 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f7e2.png
+-rw-r--r--   0        0        0      959 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f7e3.png
+-rw-r--r--   0        0        0     1016 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f7e4.png
+-rw-r--r--   0        0        0      630 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f7e5.png
+-rw-r--r--   0        0        0      544 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f7e6.png
+-rw-r--r--   0        0        0      486 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f7e7.png
+-rw-r--r--   0        0        0      695 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f7e8.png
+-rw-r--r--   0        0        0      568 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f7e9.png
+-rw-r--r--   0        0        0      537 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f7ea.png
+-rw-r--r--   0        0        0      534 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f7eb.png
+-rw-r--r--   0        0        0      335 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f7f0.png
+-rw-r--r--   0        0        0     1468 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f90c.png
+-rw-r--r--   0        0        0      959 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f90d.png
+-rw-r--r--   0        0        0     1168 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f90e.png
+-rw-r--r--   0        0        0     1031 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f90f.png
+-rw-r--r--   0        0        0     2728 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f910.png
+-rw-r--r--   0        0        0     2691 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f911.png
+-rw-r--r--   0        0        0     2684 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f912.png
+-rw-r--r--   0        0        0     2539 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f913.png
+-rw-r--r--   0        0        0     2157 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f914.png
+-rw-r--r--   0        0        0     2019 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f915.png
+-rw-r--r--   0        0        0     2767 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f916.png
+-rw-r--r--   0        0        0     2530 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f917.png
+-rw-r--r--   0        0        0     1300 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f918.png
+-rw-r--r--   0        0        0     1397 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f919.png
+-rw-r--r--   0        0        0     1383 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f91a.png
+-rw-r--r--   0        0        0     1239 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f91b.png
+-rw-r--r--   0        0        0     1276 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f91c.png
+-rw-r--r--   0        0        0     1399 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f91d.png
+-rw-r--r--   0        0        0     1371 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f91e.png
+-rw-r--r--   0        0        0     1250 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f91f.png
+-rw-r--r--   0        0        0     2550 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f920.png
+-rw-r--r--   0        0        0     3526 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f921.png
+-rw-r--r--   0        0        0     1684 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f922.png
+-rw-r--r--   0        0        0     2752 2022-11-18 15:36:28.336582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f923.png
+-rw-r--r--   0        0        0     2405 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f924.png
+-rw-r--r--   0        0        0     2241 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f925.png
+-rw-r--r--   0        0        0     2211 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f926.png
+-rw-r--r--   0        0        0     2487 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f926_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2222 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f926_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2604 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f927.png
+-rw-r--r--   0        0        0     1957 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f928.png
+-rw-r--r--   0        0        0     3007 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f929.png
+-rw-r--r--   0        0        0     2941 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f92a.png
+-rw-r--r--   0        0        0     2316 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f92b.png
+-rw-r--r--   0        0        0     2135 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f92c.png
+-rw-r--r--   0        0        0     2253 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f92d.png
+-rw-r--r--   0        0        0     3481 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f92e.png
+-rw-r--r--   0        0        0     3562 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f92f.png
+-rw-r--r--   0        0        0     2250 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f930.png
+-rw-r--r--   0        0        0     2852 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f931.png
+-rw-r--r--   0        0        0     1656 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f932.png
+-rw-r--r--   0        0        0     1585 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f933.png
+-rw-r--r--   0        0        0     3154 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f934.png
+-rw-r--r--   0        0        0     2265 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f935.png
+-rw-r--r--   0        0        0     2536 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f935_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2112 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f935_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2791 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f936.png
+-rw-r--r--   0        0        0     2649 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f937.png
+-rw-r--r--   0        0        0     2917 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f937_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2398 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f937_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     1942 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f938.png
+-rw-r--r--   0        0        0     2235 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f938_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2155 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f938_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3423 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f939.png
+-rw-r--r--   0        0        0     3506 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f939_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3465 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f939_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2695 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f93a.png
+-rw-r--r--   0        0        0     3981 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f93c.png
+-rw-r--r--   0        0        0     3878 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f93c_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3927 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f93c_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3013 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f93d.png
+-rw-r--r--   0        0        0     3287 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f93d_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2618 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f93d_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2954 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f93e.png
+-rw-r--r--   0        0        0     3042 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f93e_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3126 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f93e_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2827 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f93f.png
+-rw-r--r--   0        0        0     2393 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f940.png
+-rw-r--r--   0        0        0     2710 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f941.png
+-rw-r--r--   0        0        0     2319 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f942.png
+-rw-r--r--   0        0        0     2060 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f943.png
+-rw-r--r--   0        0        0     1133 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f944.png
+-rw-r--r--   0        0        0     2674 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f945.png
+-rw-r--r--   0        0        0     2078 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f947.png
+-rw-r--r--   0        0        0     1808 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f948.png
+-rw-r--r--   0        0        0     2087 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f949.png
+-rw-r--r--   0        0        0     2046 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f94a.png
+-rw-r--r--   0        0        0     2194 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f94b.png
+-rw-r--r--   0        0        0     2270 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f94c.png
+-rw-r--r--   0        0        0     2214 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f94d.png
+-rw-r--r--   0        0        0     2622 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f94e.png
+-rw-r--r--   0        0        0     1705 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f94f.png
+-rw-r--r--   0        0        0     2311 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f950.png
+-rw-r--r--   0        0        0     2485 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f951.png
+-rw-r--r--   0        0        0     2890 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f952.png
+-rw-r--r--   0        0        0     2832 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f953.png
+-rw-r--r--   0        0        0     1741 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f954.png
+-rw-r--r--   0        0        0     2090 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f955.png
+-rw-r--r--   0        0        0     1414 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f956.png
+-rw-r--r--   0        0        0     4262 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f957.png
+-rw-r--r--   0        0        0     3316 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f958.png
+-rw-r--r--   0        0        0     2853 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f959.png
+-rw-r--r--   0        0        0     1015 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f95a.png
+-rw-r--r--   0        0        0     1727 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f95b.png
+-rw-r--r--   0        0        0     3624 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f95c.png
+-rw-r--r--   0        0        0     2337 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f95d.png
+-rw-r--r--   0        0        0     2837 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f95e.png
+-rw-r--r--   0        0        0     2009 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f95f.png
+-rw-r--r--   0        0        0     1509 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f960.png
+-rw-r--r--   0        0        0     1724 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f961.png
+-rw-r--r--   0        0        0     1278 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f962.png
+-rw-r--r--   0        0        0     1504 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f963.png
+-rw-r--r--   0        0        0     1548 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f964.png
+-rw-r--r--   0        0        0     2092 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f965.png
+-rw-r--r--   0        0        0     2813 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f966.png
+-rw-r--r--   0        0        0     2219 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f967.png
+-rw-r--r--   0        0        0     2790 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f968.png
+-rw-r--r--   0        0        0     2651 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f969.png
+-rw-r--r--   0        0        0     2666 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f96a.png
+-rw-r--r--   0        0        0     1859 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f96b.png
+-rw-r--r--   0        0        0     3117 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f96c.png
+-rw-r--r--   0        0        0     2602 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f96d.png
+-rw-r--r--   0        0        0     2615 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f96e.png
+-rw-r--r--   0        0        0     3023 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f96f.png
+-rw-r--r--   0        0        0     2696 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f970.png
+-rw-r--r--   0        0        0     2412 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f971.png
+-rw-r--r--   0        0        0     2349 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f972.png
+-rw-r--r--   0        0        0     3929 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f973.png
+-rw-r--r--   0        0        0     2106 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f974.png
+-rw-r--r--   0        0        0     2491 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f975.png
+-rw-r--r--   0        0        0     2947 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f976.png
+-rw-r--r--   0        0        0     2065 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f977.png
+-rw-r--r--   0        0        0     2697 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f978.png
+-rw-r--r--   0        0        0     3326 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f979.png
+-rw-r--r--   0        0        0     2404 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f97a.png
+-rw-r--r--   0        0        0     1975 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f97b.png
+-rw-r--r--   0        0        0     1541 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f97c.png
+-rw-r--r--   0        0        0     2260 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f97d.png
+-rw-r--r--   0        0        0     2291 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f97e.png
+-rw-r--r--   0        0        0      996 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f97f.png
+-rw-r--r--   0        0        0     3907 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f980.png
+-rw-r--r--   0        0        0     3404 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f981.png
+-rw-r--r--   0        0        0     2013 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f982.png
+-rw-r--r--   0        0        0     3489 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f983.png
+-rw-r--r--   0        0        0     3552 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f984.png
+-rw-r--r--   0        0        0     2600 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f985.png
+-rw-r--r--   0        0        0     2282 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f986.png
+-rw-r--r--   0        0        0     1855 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f987.png
+-rw-r--r--   0        0        0     2029 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f988.png
+-rw-r--r--   0        0        0     2574 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f989.png
+-rw-r--r--   0        0        0     2522 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f98a.png
+-rw-r--r--   0        0        0     2937 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f98b.png
+-rw-r--r--   0        0        0     2432 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f98c.png
+-rw-r--r--   0        0        0     1950 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f98d.png
+-rw-r--r--   0        0        0     3110 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f98e.png
+-rw-r--r--   0        0        0     1713 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f98f.png
+-rw-r--r--   0        0        0     4212 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f990.png
+-rw-r--r--   0        0        0     4058 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f991.png
+-rw-r--r--   0        0        0     2540 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f992.png
+-rw-r--r--   0        0        0     2060 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f993.png
+-rw-r--r--   0        0        0     2587 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f994.png
+-rw-r--r--   0        0        0     1802 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f995.png
+-rw-r--r--   0        0        0     2149 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f996.png
+-rw-r--r--   0        0        0     2046 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f997.png
+-rw-r--r--   0        0        0     1932 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f998.png
+-rw-r--r--   0        0        0     1793 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f999.png
+-rw-r--r--   0        0        0     4253 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f99a.png
+-rw-r--r--   0        0        0     1338 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f99b.png
+-rw-r--r--   0        0        0     2652 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f99c.png
+-rw-r--r--   0        0        0     1442 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f99d.png
+-rw-r--r--   0        0        0     3170 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f99e.png
+-rw-r--r--   0        0        0     3035 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f99f.png
+-rw-r--r--   0        0        0     3160 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9a0.png
+-rw-r--r--   0        0        0     1386 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9a1.png
+-rw-r--r--   0        0        0     1745 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9a2.png
+-rw-r--r--   0        0        0     1946 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9a3.png
+-rw-r--r--   0        0        0     2772 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9a4.png
+-rw-r--r--   0        0        0     2641 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9a5.png
+-rw-r--r--   0        0        0     2185 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9a6.png
+-rw-r--r--   0        0        0     2603 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9a7.png
+-rw-r--r--   0        0        0     1870 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9a8.png
+-rw-r--r--   0        0        0     1782 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9a9.png
+-rw-r--r--   0        0        0     1986 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9aa.png
+-rw-r--r--   0        0        0     1721 2022-11-18 15:36:28.372583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ab.png
+-rw-r--r--   0        0        0     1659 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ac.png
+-rw-r--r--   0        0        0     1328 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ad.png
+-rw-r--r--   0        0        0     3191 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ae.png
+-rw-r--r--   0        0        0      801 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9af.png
+-rw-r--r--   0        0        0     1127 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b0.png
+-rw-r--r--   0        0        0     1559 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b1.png
+-rw-r--r--   0        0        0      833 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b2.png
+-rw-r--r--   0        0        0     1131 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b3.png
+-rw-r--r--   0        0        0     1101 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b4.png
+-rw-r--r--   0        0        0      921 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b5.png
+-rw-r--r--   0        0        0     1240 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b6.png
+-rw-r--r--   0        0        0     1290 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b7.png
+-rw-r--r--   0        0        0     3429 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b8.png
+-rw-r--r--   0        0        0     3693 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b8_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3512 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b8_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3996 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b9.png
+-rw-r--r--   0        0        0     4529 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b9_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3957 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b9_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2908 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ba.png
+-rw-r--r--   0        0        0     1819 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9bb.png
+-rw-r--r--   0        0        0     1750 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9bc.png
+-rw-r--r--   0        0        0     1499 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9bd.png
+-rw-r--r--   0        0        0     1854 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9be.png
+-rw-r--r--   0        0        0     1429 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9bf.png
+-rw-r--r--   0        0        0     1368 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9c0.png
+-rw-r--r--   0        0        0     3498 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9c1.png
+-rw-r--r--   0        0        0     1692 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9c2.png
+-rw-r--r--   0        0        0     1825 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9c3.png
+-rw-r--r--   0        0        0     1754 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9c4.png
+-rw-r--r--   0        0        0     2237 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9c5.png
+-rw-r--r--   0        0        0     2313 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9c6.png
+-rw-r--r--   0        0        0     1936 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9c7.png
+-rw-r--r--   0        0        0     1223 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9c8.png
+-rw-r--r--   0        0        0     1859 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9c9.png
+-rw-r--r--   0        0        0     2521 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ca.png
+-rw-r--r--   0        0        0     2091 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9cb.png
+-rw-r--r--   0        0        0     3993 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9cc.png
+-rw-r--r--   0        0        0     1802 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9cd.png
+-rw-r--r--   0        0        0     2194 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9cd_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     1803 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9cd_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     1355 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ce.png
+-rw-r--r--   0        0        0     1672 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ce_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     1371 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ce_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2635 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9cf.png
+-rw-r--r--   0        0        0     2699 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9cf_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2712 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9cf_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2484 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d0.png
+-rw-r--r--   0        0        0     2148 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1.png
+-rw-r--r--   0        0        0     4085 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f33e.png
+-rw-r--r--   0        0        0     3096 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f373.png
+-rw-r--r--   0        0        0     2947 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f37c.png
+-rw-r--r--   0        0        0     3304 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f384.png
+-rw-r--r--   0        0        0     2602 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f393.png
+-rw-r--r--   0        0        0     3162 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3a4.png
+-rw-r--r--   0        0        0     3507 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3a8.png
+-rw-r--r--   0        0        0     2985 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3eb.png
+-rw-r--r--   0        0        0     3277 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3ed.png
+-rw-r--r--   0        0        0     1983 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f4bb.png
+-rw-r--r--   0        0        0     2284 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f4bc.png
+-rw-r--r--   0        0        0     3264 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f527.png
+-rw-r--r--   0        0        0     3470 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f52c.png
+-rw-r--r--   0        0        0     3285 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f680.png
+-rw-r--r--   0        0        0     3739 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f692.png
+-rw-r--r--   0        0        0     3138 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f91d_200d_1f9d1.png
+-rw-r--r--   0        0        0     2547 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9af.png
+-rw-r--r--   0        0        0     2030 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b0.png
+-rw-r--r--   0        0        0     2393 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b1.png
+-rw-r--r--   0        0        0     1800 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b2.png
+-rw-r--r--   0        0        0     2200 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b3.png
+-rw-r--r--   0        0        0     2927 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9bc.png
+-rw-r--r--   0        0        0     2244 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9bd.png
+-rw-r--r--   0        0        0     2529 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_2695_fe0f.png
+-rw-r--r--   0        0        0     2671 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_2696_fe0f.png
+-rw-r--r--   0        0        0     2718 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_2708_fe0f.png
+-rw-r--r--   0        0        0     2366 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d2.png
+-rw-r--r--   0        0        0     2801 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d3.png
+-rw-r--r--   0        0        0     2178 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d4.png
+-rw-r--r--   0        0        0     4333 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d4_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3689 2022-11-18 15:36:28.352583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d4_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2258 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d5.png
+-rw-r--r--   0        0        0     3176 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d6.png
+-rw-r--r--   0        0        0     3180 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d6_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3220 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d6_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3412 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d7.png
+-rw-r--r--   0        0        0     3963 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d7_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3608 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d7_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2201 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d8.png
+-rw-r--r--   0        0        0     2189 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d8_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2314 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d8_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3401 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d9.png
+-rw-r--r--   0        0        0     3318 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d9_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3327 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d9_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2627 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9da.png
+-rw-r--r--   0        0        0     3146 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9da_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2586 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9da_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2949 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9db.png
+-rw-r--r--   0        0        0     3078 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9db_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3077 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9db_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3533 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9dc.png
+-rw-r--r--   0        0        0     3786 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9dc_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3488 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9dc_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     3089 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9dd.png
+-rw-r--r--   0        0        0     3289 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9dd_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3449 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9dd_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2735 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9de.png
+-rw-r--r--   0        0        0     2996 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9de_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2841 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9de_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2737 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9df.png
+-rw-r--r--   0        0        0     2739 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9df_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     2760 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9df_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     2467 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9e0.png
+-rw-r--r--   0        0        0     1175 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9e1.png
+-rw-r--r--   0        0        0     1084 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9e2.png
+-rw-r--r--   0        0        0     1803 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9e3.png
+-rw-r--r--   0        0        0     1581 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9e4.png
+-rw-r--r--   0        0        0     1812 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9e5.png
+-rw-r--r--   0        0        0     1914 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9e6.png
+-rw-r--r--   0        0        0     1351 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9e7.png
+-rw-r--r--   0        0        0     2523 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9e8.png
+-rw-r--r--   0        0        0     1911 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9e9.png
+-rw-r--r--   0        0        0     2524 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ea.png
+-rw-r--r--   0        0        0     1718 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9eb.png
+-rw-r--r--   0        0        0     3148 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ec.png
+-rw-r--r--   0        0        0     2612 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ed.png
+-rw-r--r--   0        0        0     3580 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ee.png
+-rw-r--r--   0        0        0     3068 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ef.png
+-rw-r--r--   0        0        0     1488 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9f0.png
+-rw-r--r--   0        0        0     1688 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9f1.png
+-rw-r--r--   0        0        0     1816 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9f2.png
+-rw-r--r--   0        0        0     2325 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9f3.png
+-rw-r--r--   0        0        0     1117 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9f4.png
+-rw-r--r--   0        0        0     2571 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9f5.png
+-rw-r--r--   0        0        0     2874 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9f6.png
+-rw-r--r--   0        0        0     1924 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9f7.png
+-rw-r--r--   0        0        0     2489 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9f8.png
+-rw-r--r--   0        0        0     1047 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9f9.png
+-rw-r--r--   0        0        0     2773 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9fa.png
+-rw-r--r--   0        0        0     1623 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9fb.png
+-rw-r--r--   0        0        0     2401 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9fc.png
+-rw-r--r--   0        0        0     2080 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9fd.png
+-rw-r--r--   0        0        0     1461 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9fe.png
+-rw-r--r--   0        0        0     2710 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ff.png
+-rw-r--r--   0        0        0     2121 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa70.png
+-rw-r--r--   0        0        0     1499 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa71.png
+-rw-r--r--   0        0        0     1002 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa72.png
+-rw-r--r--   0        0        0     2386 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa73.png
+-rw-r--r--   0        0        0     1526 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa74.png
+-rw-r--r--   0        0        0     1146 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa78.png
+-rw-r--r--   0        0        0     1312 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa79.png
+-rw-r--r--   0        0        0     1968 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa7a.png
+-rw-r--r--   0        0        0     4290 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa7b.png
+-rw-r--r--   0        0        0     2091 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa7c.png
+-rw-r--r--   0        0        0     2378 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa80.png
+-rw-r--r--   0        0        0     1942 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa81.png
+-rw-r--r--   0        0        0     3182 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa82.png
+-rw-r--r--   0        0        0     1651 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa83.png
+-rw-r--r--   0        0        0     1076 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa84.png
+-rw-r--r--   0        0        0     9582 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa85.png
+-rw-r--r--   0        0        0     3331 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa86.png
+-rw-r--r--   0        0        0     2815 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa90.png
+-rw-r--r--   0        0        0     1145 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa91.png
+-rw-r--r--   0        0        0     1548 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa92.png
+-rw-r--r--   0        0        0     1251 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa93.png
+-rw-r--r--   0        0        0     2078 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa94.png
+-rw-r--r--   0        0        0     1644 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa95.png
+-rw-r--r--   0        0        0     1803 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa96.png
+-rw-r--r--   0        0        0     2194 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa97.png
+-rw-r--r--   0        0        0     1906 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa98.png
+-rw-r--r--   0        0        0     2641 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa99.png
+-rw-r--r--   0        0        0     1455 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa9a.png
+-rw-r--r--   0        0        0     1387 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa9b.png
+-rw-r--r--   0        0        0     2654 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa9c.png
+-rw-r--r--   0        0        0     1534 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa9d.png
+-rw-r--r--   0        0        0     1070 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa9e.png
+-rw-r--r--   0        0        0      844 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fa9f.png
+-rw-r--r--   0        0        0     1214 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1faa0.png
+-rw-r--r--   0        0        0     1646 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1faa1.png
+-rw-r--r--   0        0        0     3421 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1faa2.png
+-rw-r--r--   0        0        0     2517 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1faa3.png
+-rw-r--r--   0        0        0     2137 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/1faa4.png
+-rw-r--r--   0        0        0     1078 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1faa5.png
+-rw-r--r--   0        0        0     1357 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1faa6.png
+-rw-r--r--   0        0        0      739 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1faa7.png
+-rw-r--r--   0        0        0     1398 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1faa8.png
+-rw-r--r--   0        0        0     4069 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/1faa9.png
+-rw-r--r--   0        0        0     3116 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1faaa.png
+-rw-r--r--   0        0        0     2959 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/1faab.png
+-rw-r--r--   0        0        0     3385 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1faac.png
+-rw-r--r--   0        0        0     3390 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fab0.png
+-rw-r--r--   0        0        0     2544 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fab1.png
+-rw-r--r--   0        0        0     2712 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fab2.png
+-rw-r--r--   0        0        0     2220 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fab3.png
+-rw-r--r--   0        0        0     2337 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fab4.png
+-rw-r--r--   0        0        0     1796 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fab5.png
+-rw-r--r--   0        0        0     1694 2022-11-18 15:36:28.376583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fab6.png
+-rw-r--r--   0        0        0     3028 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fab7.png
+-rw-r--r--   0        0        0     8701 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fab8.png
+-rw-r--r--   0        0        0     3220 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fab9.png
+-rw-r--r--   0        0        0     3143 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1faba.png
+-rw-r--r--   0        0        0     3145 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1fac0.png
+-rw-r--r--   0        0        0     2355 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1fac1.png
+-rw-r--r--   0        0        0     1207 2022-11-18 15:36:28.368583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fac2.png
+-rw-r--r--   0        0        0     2880 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fac3.png
+-rw-r--r--   0        0        0     2915 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fac4.png
+-rw-r--r--   0        0        0     3239 2022-11-18 15:36:28.356583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fac5.png
+-rw-r--r--   0        0        0     2208 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fad0.png
+-rw-r--r--   0        0        0     2166 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fad1.png
+-rw-r--r--   0        0        0     1780 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fad2.png
+-rw-r--r--   0        0        0     1470 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fad3.png
+-rw-r--r--   0        0        0     1942 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fad4.png
+-rw-r--r--   0        0        0     2275 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fad5.png
+-rw-r--r--   0        0        0     1506 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fad6.png
+-rw-r--r--   0        0        0     2456 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fad7.png
+-rw-r--r--   0        0        0     3231 2022-11-18 15:36:28.384583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fad8.png
+-rw-r--r--   0        0        0     2883 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/1fad9.png
+-rw-r--r--   0        0        0     3754 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1fae0.png
+-rw-r--r--   0        0        0     2667 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1fae1.png
+-rw-r--r--   0        0        0     3645 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1fae2.png
+-rw-r--r--   0        0        0     3805 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1fae3.png
+-rw-r--r--   0        0        0     3362 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/1fae4.png
+-rw-r--r--   0        0        0     2324 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/1fae5.png
+-rw-r--r--   0        0        0     2612 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1fae6.png
+-rw-r--r--   0        0        0     8233 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/1fae7.png
+-rw-r--r--   0        0        0     3094 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1faf0.png
+-rw-r--r--   0        0        0     3119 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1faf1.png
+-rw-r--r--   0        0        0     3274 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1faf2.png
+-rw-r--r--   0        0        0     2474 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1faf3.png
+-rw-r--r--   0        0        0     2475 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1faf4.png
+-rw-r--r--   0        0        0     4017 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1faf5.png
+-rw-r--r--   0        0        0     2903 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/1faf6.png
+-rw-r--r--   0        0        0      979 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/203c.png
+-rw-r--r--   0        0        0     1134 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2049.png
+-rw-r--r--   0        0        0      574 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/2122.png
+-rw-r--r--   0        0        0     1078 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/2139.png
+-rw-r--r--   0        0        0     1083 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/2194.png
+-rw-r--r--   0        0        0     1027 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/2195.png
+-rw-r--r--   0        0        0     1046 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/2196.png
+-rw-r--r--   0        0        0     1044 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/2197.png
+-rw-r--r--   0        0        0     1041 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/2198.png
+-rw-r--r--   0        0        0     1000 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/2199.png
+-rw-r--r--   0        0        0     1098 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/21a9.png
+-rw-r--r--   0        0        0     1061 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/21aa.png
+-rw-r--r--   0        0        0     1401 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/231a.png
+-rw-r--r--   0        0        0     2614 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/231b.png
+-rw-r--r--   0        0        0      983 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/2328.png
+-rw-r--r--   0        0        0     1078 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/23cf.png
+-rw-r--r--   0        0        0     1028 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/23e9.png
+-rw-r--r--   0        0        0     1097 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/23ea.png
+-rw-r--r--   0        0        0     1069 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/23eb.png
+-rw-r--r--   0        0        0     1086 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/23ec.png
+-rw-r--r--   0        0        0     1085 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/23ed.png
+-rw-r--r--   0        0        0     1153 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/23ee.png
+-rw-r--r--   0        0        0     1009 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/23ef.png
+-rw-r--r--   0        0        0     3657 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/23f0.png
+-rw-r--r--   0        0        0     2800 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/23f1.png
+-rw-r--r--   0        0        0     2100 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/23f2.png
+-rw-r--r--   0        0        0     2759 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/23f3.png
+-rw-r--r--   0        0        0     1053 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/23f8.png
+-rw-r--r--   0        0        0      952 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/23f9.png
+-rw-r--r--   0        0        0     1014 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/23fa.png
+-rw-r--r--   0        0        0     1295 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/24c2.png
+-rw-r--r--   0        0        0      408 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/25aa.png
+-rw-r--r--   0        0        0      194 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/25ab.png
+-rw-r--r--   0        0        0     1011 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/25b6.png
+-rw-r--r--   0        0        0     1028 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/25c0.png
+-rw-r--r--   0        0        0      196 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/25fb.png
+-rw-r--r--   0        0        0      291 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/25fc.png
+-rw-r--r--   0        0        0      175 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/25fd.png
+-rw-r--r--   0        0        0      283 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/25fe.png
+-rw-r--r--   0        0        0     1597 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/2600.png
+-rw-r--r--   0        0        0      934 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/2601.png
+-rw-r--r--   0        0        0     1630 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/2602.png
+-rw-r--r--   0        0        0     3102 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/2603.png
+-rw-r--r--   0        0        0     2996 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/2604.png
+-rw-r--r--   0        0        0     2616 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/260e.png
+-rw-r--r--   0        0        0     1309 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2611.png
+-rw-r--r--   0        0        0     2749 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/2614.png
+-rw-r--r--   0        0        0     1869 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/2615.png
+-rw-r--r--   0        0        0     2927 2022-11-18 15:36:28.380583 a2-0.4.1/src/a2/data/emoji/emoji_images/2618.png
+-rw-r--r--   0        0        0     1186 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/261d.png
+-rw-r--r--   0        0        0     1956 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/2620.png
+-rw-r--r--   0        0        0     1258 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/2622.png
+-rw-r--r--   0        0        0     1740 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/2623.png
+-rw-r--r--   0        0        0     1113 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2626.png
+-rw-r--r--   0        0        0     1243 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/262a.png
+-rw-r--r--   0        0        0     1349 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/262e.png
+-rw-r--r--   0        0        0     1307 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/262f.png
+-rw-r--r--   0        0        0     1621 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/2638.png
+-rw-r--r--   0        0        0     1931 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/2639.png
+-rw-r--r--   0        0        0     1931 2022-11-18 15:36:28.340582 a2-0.4.1/src/a2/data/emoji/emoji_images/263a.png
+-rw-r--r--   0        0        0     1373 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2640.png
+-rw-r--r--   0        0        0     1449 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2642.png
+-rw-r--r--   0        0        0     1307 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2648.png
+-rw-r--r--   0        0        0     1302 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2649.png
+-rw-r--r--   0        0        0     1204 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/264a.png
+-rw-r--r--   0        0        0     1498 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/264b.png
+-rw-r--r--   0        0        0     1435 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/264c.png
+-rw-r--r--   0        0        0     1437 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/264d.png
+-rw-r--r--   0        0        0     1217 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/264e.png
+-rw-r--r--   0        0        0     1252 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/264f.png
+-rw-r--r--   0        0        0     1250 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2650.png
+-rw-r--r--   0        0        0     1424 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2651.png
+-rw-r--r--   0        0        0     1355 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2652.png
+-rw-r--r--   0        0        0     1223 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2653.png
+-rw-r--r--   0        0        0     1041 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/265f.png
+-rw-r--r--   0        0        0      990 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/2660.png
+-rw-r--r--   0        0        0     1105 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/2663.png
+-rw-r--r--   0        0        0     1024 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/2665.png
+-rw-r--r--   0        0        0      819 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/2666.png
+-rw-r--r--   0        0        0     1476 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/2668.png
+-rw-r--r--   0        0        0     1547 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/267b.png
+-rw-r--r--   0        0        0      902 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/267e.png
+-rw-r--r--   0        0        0     1487 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/267f.png
+-rw-r--r--   0        0        0     1688 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/2692.png
+-rw-r--r--   0        0        0     1587 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/2693.png
+-rw-r--r--   0        0        0     1924 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/2694.png
+-rw-r--r--   0        0        0     1600 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2695.png
+-rw-r--r--   0        0        0     2360 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/2696.png
+-rw-r--r--   0        0        0     2664 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/2697.png
+-rw-r--r--   0        0        0     2767 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/2699.png
+-rw-r--r--   0        0        0     1680 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/269b.png
+-rw-r--r--   0        0        0     2332 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/269c.png
+-rw-r--r--   0        0        0      862 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/26a0.png
+-rw-r--r--   0        0        0      822 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/26a1.png
+-rw-r--r--   0        0        0     1297 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/26a7.png
+-rw-r--r--   0        0        0      833 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/26aa.png
+-rw-r--r--   0        0        0     1038 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/26ab.png
+-rw-r--r--   0        0        0     1809 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/26b0.png
+-rw-r--r--   0        0        0     1967 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/26b1.png
+-rw-r--r--   0        0        0     1834 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/26bd.png
+-rw-r--r--   0        0        0     2594 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/26be.png
+-rw-r--r--   0        0        0     2364 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/26c4.png
+-rw-r--r--   0        0        0     1471 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/26c5.png
+-rw-r--r--   0        0        0     2224 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/26c8.png
+-rw-r--r--   0        0        0     1288 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/26ce.png
+-rw-r--r--   0        0        0     1106 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/26cf.png
+-rw-r--r--   0        0        0     2363 2022-11-18 15:36:28.408584 a2-0.4.1/src/a2/data/emoji/emoji_images/26d1.png
+-rw-r--r--   0        0        0     3241 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/26d3.png
+-rw-r--r--   0        0        0     1286 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/26d4.png
+-rw-r--r--   0        0        0     1219 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/26e9.png
+-rw-r--r--   0        0        0     2405 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/26ea.png
+-rw-r--r--   0        0        0     2999 2022-11-18 15:36:28.388583 a2-0.4.1/src/a2/data/emoji/emoji_images/26f0.png
+-rw-r--r--   0        0        0     1902 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/26f1.png
+-rw-r--r--   0        0        0     3153 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/26f2.png
+-rw-r--r--   0        0        0     1712 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/26f3.png
+-rw-r--r--   0        0        0     2385 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/26f4.png
+-rw-r--r--   0        0        0     2439 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/26f5.png
+-rw-r--r--   0        0        0     3013 2022-11-18 15:36:28.360583 a2-0.4.1/src/a2/data/emoji/emoji_images/26f7.png
+-rw-r--r--   0        0        0     1886 2022-11-18 15:36:28.404584 a2-0.4.1/src/a2/data/emoji/emoji_images/26f8.png
+-rw-r--r--   0        0        0     3213 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/26f9.png
+-rw-r--r--   0        0        0     3294 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/26f9_fe0f_200d_2640_fe0f.png
+-rw-r--r--   0        0        0     3168 2022-11-18 15:36:28.364583 a2-0.4.1/src/a2/data/emoji/emoji_images/26f9_fe0f_200d_2642_fe0f.png
+-rw-r--r--   0        0        0     1854 2022-11-18 15:36:28.392583 a2-0.4.1/src/a2/data/emoji/emoji_images/26fa.png
+-rw-r--r--   0        0        0     2366 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/26fd.png
+-rw-r--r--   0        0        0     3030 2022-11-18 15:36:28.416584 a2-0.4.1/src/a2/data/emoji/emoji_images/2702.png
+-rw-r--r--   0        0        0     1137 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2705.png
+-rw-r--r--   0        0        0     2700 2022-11-18 15:36:28.396584 a2-0.4.1/src/a2/data/emoji/emoji_images/2708.png
+-rw-r--r--   0        0        0      871 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/2709.png
+-rw-r--r--   0        0        0     1669 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/270a.png
+-rw-r--r--   0        0        0     1464 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/270b.png
+-rw-r--r--   0        0        0     1407 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/270c.png
+-rw-r--r--   0        0        0     1751 2022-11-18 15:36:28.348582 a2-0.4.1/src/a2/data/emoji/emoji_images/270d.png
+-rw-r--r--   0        0        0     1587 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/270f.png
+-rw-r--r--   0        0        0     1526 2022-11-18 15:36:28.412584 a2-0.4.1/src/a2/data/emoji/emoji_images/2712.png
+-rw-r--r--   0        0        0      631 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2714.png
+-rw-r--r--   0        0        0      518 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2716.png
+-rw-r--r--   0        0        0      890 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/271d.png
+-rw-r--r--   0        0        0     1315 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/2721.png
+-rw-r--r--   0        0        0     1385 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/2728.png
+-rw-r--r--   0        0        0     1187 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/2733.png
+-rw-r--r--   0        0        0     1432 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/2734.png
+-rw-r--r--   0        0        0     3717 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/2744.png
+-rw-r--r--   0        0        0     1179 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/2747.png
+-rw-r--r--   0        0        0      782 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/274c.png
+-rw-r--r--   0        0        0     1100 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/274e.png
+-rw-r--r--   0        0        0      685 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2753.png
+-rw-r--r--   0        0        0      624 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2754.png
+-rw-r--r--   0        0        0      690 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2755.png
+-rw-r--r--   0        0        0      568 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2757.png
+-rw-r--r--   0        0        0     1038 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/2763.png
+-rw-r--r--   0        0        0     1358 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/2764.png
+-rw-r--r--   0        0        0     3565 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/2764_fe0f_200d_1f525.png
+-rw-r--r--   0        0        0     3181 2022-11-18 15:36:28.344582 a2-0.4.1/src/a2/data/emoji/emoji_images/2764_fe0f_200d_1fa79.png
+-rw-r--r--   0        0        0      251 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2795.png
+-rw-r--r--   0        0        0      200 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2796.png
+-rw-r--r--   0        0        0      249 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2797.png
+-rw-r--r--   0        0        0     1047 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/27a1.png
+-rw-r--r--   0        0        0      858 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/27b0.png
+-rw-r--r--   0        0        0      686 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/27bf.png
+-rw-r--r--   0        0        0     1083 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/2934.png
+-rw-r--r--   0        0        0     1076 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/2935.png
+-rw-r--r--   0        0        0     1044 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/2b05.png
+-rw-r--r--   0        0        0     1034 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/2b06.png
+-rw-r--r--   0        0        0     1054 2022-11-18 15:36:28.420584 a2-0.4.1/src/a2/data/emoji/emoji_images/2b07.png
+-rw-r--r--   0        0        0      700 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/2b1b.png
+-rw-r--r--   0        0        0      203 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/2b1c.png
+-rw-r--r--   0        0        0     1704 2022-11-18 15:36:28.400584 a2-0.4.1/src/a2/data/emoji/emoji_images/2b50.png
+-rw-r--r--   0        0        0     1025 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/2b55.png
+-rw-r--r--   0        0        0      614 2022-11-18 15:36:28.424584 a2-0.4.1/src/a2/data/emoji/emoji_images/3030.png
+-rw-r--r--   0        0        0      791 2022-11-18 15:36:28.428584 a2-0.4.1/src/a2/data/emoji/emoji_images/303d.png
+-rw-r--r--   0        0        0     1614 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/3297.png
+-rw-r--r--   0        0        0     1733 2022-11-18 15:36:28.432584 a2-0.4.1/src/a2/data/emoji/emoji_images/3299.png
+-rw-r--r--   0        0        0  2152796 2022-07-06 14:12:42.663962 a2-0.4.1/src/a2/data/font/Symbola.ttf
+-rw-r--r--   0        0        0  3727644 2022-07-06 14:12:42.683963 a2-0.4.1/src/a2/data/font/Symbola_hint.ttf
+-rw-r--r--   0        0        0       44 2022-07-06 14:12:42.683963 a2-0.4.1/src/a2/data/font/sharefonts.net.txt
+-rw-r--r--   0        0        0        0 2022-11-01 14:44:14.724032 a2-0.4.1/src/a2/data/vocabularies/__init__.py
+-rw-r--r--   0        0        0     2789 2023-02-21 08:27:21.563839 a2-0.4.1/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt
+-rw-r--r--   0        0        0      236 2023-02-21 08:27:21.563869 a2-0.4.1/src/a2/data/vocabularies/weather_vocab_enchanted_precipitation.txt
+-rw-r--r--   0        0        0      188 2023-02-21 14:04:17.568649 a2-0.4.1/src/a2/dataset/__init__.py
+-rw-r--r--   0        0        0      366 2023-02-21 14:04:45.557653 a2-0.4.1/src/a2/dataset/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      645 2023-01-30 15:08:36.152054 a2-0.4.1/src/a2/dataset/__pycache__/emojis.cpython-310.pyc
+-rw-r--r--   0        0        0     8877 2023-06-07 07:51:53.099831 a2-0.4.1/src/a2/dataset/__pycache__/load_dataset.cpython-310.pyc
+-rw-r--r--   0        0        0      434 2022-08-02 15:37:53.112570 a2-0.4.1/src/a2/dataset/__pycache__/manipulate_datasets.cpython-310.pyc
+-rw-r--r--   0        0        0    39422 2023-01-30 15:08:36.940073 a2-0.4.1/src/a2/dataset/__pycache__/radar.cpython-310.pyc
+-rw-r--r--   0        0        0     8738 2023-01-30 15:08:36.944073 a2-0.4.1/src/a2/dataset/__pycache__/stations.cpython-310.pyc
+-rw-r--r--   0        0        0     1040 2023-02-20 13:59:16.193086 a2-0.4.1/src/a2/dataset/__pycache__/tweets.cpython-310.pyc
+-rw-r--r--   0        0        0     2155 2022-12-14 09:39:28.258310 a2-0.4.1/src/a2/dataset/__pycache__/units.cpython-310.pyc
+-rw-r--r--   0        0        0    15533 2023-06-06 13:09:57.413845 a2-0.4.1/src/a2/dataset/__pycache__/utils_dataset.cpython-310.pyc
+-rw-r--r--   0        0        0      556 2023-01-30 14:59:51.635141 a2-0.4.1/src/a2/dataset/emojis.py
+-rw-r--r--   0        0        0     8227 2023-06-06 16:23:55.890263 a2-0.4.1/src/a2/dataset/load_dataset.py
+-rw-r--r--   0        0        0    50068 2023-01-30 14:59:51.635141 a2-0.4.1/src/a2/dataset/radar.py
+-rw-r--r--   0        0        0    10354 2023-01-30 14:59:51.635141 a2-0.4.1/src/a2/dataset/stations.py
+-rw-r--r--   0        0        0      699 2023-02-20 13:53:30.152744 a2-0.4.1/src/a2/dataset/tweets.py
+-rw-r--r--   0        0        0     1464 2022-12-14 09:36:33.150856 a2-0.4.1/src/a2/dataset/units.py
+-rw-r--r--   0        0        0    17623 2023-06-06 13:09:51.493718 a2-0.4.1/src/a2/dataset/utils_dataset.py
+-rw-r--r--   0        0        0      218 2023-06-13 14:57:04.764349 a2-0.4.1/src/a2/plotting/__init__.py
+-rw-r--r--   0        0        0      397 2023-06-13 15:02:53.558067 a2-0.4.1/src/a2/plotting/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7285 2023-06-15 09:40:17.553725 a2-0.4.1/src/a2/plotting/__pycache__/analysis.cpython-310.pyc
+-rw-r--r--   0        0        0     2275 2023-06-13 15:02:53.558067 a2-0.4.1/src/a2/plotting/__pycache__/axes_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     1082 2023-06-12 14:35:35.933045 a2-0.4.1/src/a2/plotting/__pycache__/colormesh.cpython-310.pyc
+-rw-r--r--   0        0        0      754 2023-06-13 14:21:36.116890 a2-0.4.1/src/a2/plotting/__pycache__/figures.cpython-310.pyc
+-rw-r--r--   0        0        0     5981 2023-06-13 14:21:36.104889 a2-0.4.1/src/a2/plotting/__pycache__/histogram_2d_utils.cpython-310.pyc
+-rw-r--r--   0        0        0    24893 2023-06-13 15:16:41.952119 a2-0.4.1/src/a2/plotting/__pycache__/histograms.cpython-310.pyc
+-rw-r--r--   0        0        0     3126 2023-06-12 14:30:40.201208 a2-0.4.1/src/a2/plotting/__pycache__/parallel_plotting.cpython-310.pyc
+-rw-r--r--   0        0        0     2721 2023-06-13 14:05:47.932777 a2-0.4.1/src/a2/plotting/__pycache__/timeseries.cpython-310.pyc
+-rw-r--r--   0        0        0    16725 2023-06-14 10:00:39.495890 a2-0.4.1/src/a2/plotting/__pycache__/utils_plotting.cpython-310.pyc
+-rw-r--r--   0        0        0    29262 2023-06-13 15:02:53.834075 a2-0.4.1/src/a2/plotting/__pycache__/weather_maps.cpython-310.pyc
+-rw-r--r--   0        0        0     8299 2023-06-14 10:05:04.619166 a2-0.4.1/src/a2/plotting/analysis.py
+-rw-r--r--   0        0        0     2266 2023-06-13 14:57:04.764349 a2-0.4.1/src/a2/plotting/axes_utils.py
+-rw-r--r--   0        0        0      910 2023-06-12 14:35:07.100288 a2-0.4.1/src/a2/plotting/colormesh.py
+-rw-r--r--   0        0        0      505 2023-06-13 14:18:41.948324 a2-0.4.1/src/a2/plotting/figures.py
+-rw-r--r--   0        0        0     8363 2023-06-13 14:21:30.496741 a2-0.4.1/src/a2/plotting/histogram_2d_utils.py
+-rw-r--r--   0        0        0    35236 2023-06-13 15:16:40.584083 a2-0.4.1/src/a2/plotting/histograms.py
+-rw-r--r--   0        0        0     3010 2023-06-12 14:30:35.341077 a2-0.4.1/src/a2/plotting/parallel_plotting.py
+-rw-r--r--   0        0        0     2814 2023-06-13 14:05:14.219928 a2-0.4.1/src/a2/plotting/timeseries.py
+-rw-r--r--   0        0        0    19695 2023-06-14 10:00:38.439840 a2-0.4.1/src/a2/plotting/utils_plotting.py
+-rw-r--r--   0        0        0    34761 2023-06-13 14:57:04.760349 a2-0.4.1/src/a2/plotting/weather_maps.py
+-rw-r--r--   0        0        0       67 2022-11-01 14:44:14.724032 a2-0.4.1/src/a2/preprocess/__init__.py
+-rw-r--r--   0        0        0      228 2022-11-10 09:21:06.475180 a2-0.4.1/src/a2/preprocess/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3659 2022-12-06 08:50:28.056225 a2-0.4.1/src/a2/preprocess/__pycache__/embedding.cpython-310.pyc
+-rw-r--r--   0        0        0    26114 2023-05-23 13:01:09.722463 a2-0.4.1/src/a2/preprocess/__pycache__/normalize_text.cpython-310.pyc
+-rw-r--r--   0        0        0     3645 2022-12-06 08:38:01.708129 a2-0.4.1/src/a2/preprocess/embedding.py
+-rw-r--r--   0        0        0    30389 2023-05-12 12:06:33.277030 a2-0.4.1/src/a2/preprocess/normalize_text.py
+-rw-r--r--   0        0        0      205 2023-06-15 15:57:05.208733 a2-0.4.1/src/a2/training/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-15 15:37:57.896991 a2-0.4.1/src/a2/training/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4800 2023-05-16 09:07:02.808385 a2-0.4.1/src/a2/training/__pycache__/benchmarks.cpython-310.pyc
+-rw-r--r--   0        0        0     3145 2023-06-08 14:11:17.917178 a2-0.4.1/src/a2/training/__pycache__/dataset_hugging.cpython-310.pyc
+-rw-r--r--   0        0        0     4071 2023-06-08 09:56:22.659014 a2-0.4.1/src/a2/training/__pycache__/evaluate_hugging.cpython-310.pyc
+-rw-r--r--   0        0        0      662 2023-06-15 15:36:21.742808 a2-0.4.1/src/a2/training/__pycache__/model_config.cpython-310.pyc
+-rw-r--r--   0        0        0      757 2023-06-15 15:43:21.180573 a2-0.4.1/src/a2/training/__pycache__/model_configs.cpython-310.pyc
+-rw-r--r--   0        0        0     5245 2023-06-12 13:59:16.034461 a2-0.4.1/src/a2/training/__pycache__/tracking.cpython-310.pyc
+-rw-r--r--   0        0        0     2217 2023-05-16 09:07:02.804385 a2-0.4.1/src/a2/training/__pycache__/tracking_hugging.cpython-310.pyc
+-rw-r--r--   0        0        0     6945 2023-06-14 09:47:23.282569 a2-0.4.1/src/a2/training/__pycache__/training_deep500.cpython-310.pyc
+-rw-r--r--   0        0        0     9942 2023-06-15 15:33:07.345902 a2-0.4.1/src/a2/training/__pycache__/training_hugging.cpython-310.pyc
+-rw-r--r--   0        0        0     6756 2023-04-18 13:46:32.335340 a2-0.4.1/src/a2/training/__pycache__/training_performance.cpython-310.pyc
+-rw-r--r--   0        0        0      306 2023-01-30 15:08:44.672258 a2-0.4.1/src/a2/training/__pycache__/utils_training.cpython-310.pyc
+-rw-r--r--   0        0        0     3889 2023-05-12 12:12:57.271066 a2-0.4.1/src/a2/training/benchmarks.py
+-rw-r--r--   0        0        0     3252 2023-06-08 10:49:52.048837 a2-0.4.1/src/a2/training/dataset_hugging.py
+-rw-r--r--   0        0        0     4295 2023-06-08 08:43:16.088673 a2-0.4.1/src/a2/training/evaluate_hugging.py
+-rw-r--r--   0        0        0      605 2023-06-15 15:43:04.208168 a2-0.4.1/src/a2/training/model_configs.py
+-rw-r--r--   0        0        0     4846 2023-06-12 13:56:25.094228 a2-0.4.1/src/a2/training/tracking.py
+-rw-r--r--   0        0        0     1780 2023-05-12 12:06:13.512505 a2-0.4.1/src/a2/training/tracking_hugging.py
+-rw-r--r--   0        0        0     6757 2023-06-14 09:47:14.434154 a2-0.4.1/src/a2/training/training_deep500.py
+-rw-r--r--   0        0        0    13209 2023-06-15 15:57:05.640744 a2-0.4.1/src/a2/training/training_hugging.py
+-rw-r--r--   0        0        0     6821 2023-05-12 12:06:33.277030 a2-0.4.1/src/a2/training/training_performance.py
+-rw-r--r--   0        0        0       73 2023-01-30 14:59:51.639141 a2-0.4.1/src/a2/training/utils_training.py
+-rw-r--r--   0        0        0       87 2022-11-01 14:44:14.728032 a2-0.4.1/src/a2/twitter/__init__.py
+-rw-r--r--   0        0        0      249 2022-11-10 09:22:53.001431 a2-0.4.1/src/a2/twitter/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4896 2023-02-20 13:59:24.705291 a2-0.4.1/src/a2/twitter/__pycache__/downloader.cpython-310.pyc
+-rw-r--r--   0        0        0     9148 2023-05-23 13:01:12.894332 a2-0.4.1/src/a2/twitter/__pycache__/locations.cpython-310.pyc
+-rw-r--r--   0        0        0     8339 2022-08-01 13:51:16.422462 a2-0.4.1/src/a2/twitter/__pycache__/manipulate_tweets.cpython-310.pyc
+-rw-r--r--   0        0        0     5836 2023-02-20 13:59:24.705291 a2-0.4.1/src/a2/twitter/__pycache__/twitter_api.cpython-310.pyc
+-rw-r--r--   0        0        0     4570 2023-02-20 13:53:30.156744 a2-0.4.1/src/a2/twitter/downloader.py
+-rw-r--r--   0        0        0    11489 2023-06-06 13:55:59.732319 a2-0.4.1/src/a2/twitter/locations.py
+-rw-r--r--   0        0        0     6765 2023-02-20 13:53:30.156744 a2-0.4.1/src/a2/twitter/twitter_api.py
+-rw-r--r--   0        0        0      198 2023-06-15 15:38:44.098053 a2-0.4.1/src/a2/utils/__init__.py
+-rw-r--r--   0        0        0      347 2023-06-15 15:38:47.770138 a2-0.4.1/src/a2/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     9640 2023-06-15 15:39:49.767577 a2-0.4.1/src/a2/utils/__pycache__/argparse.cpython-310.pyc
+-rw-r--r--   0        0        0      787 2023-05-16 09:06:59.920315 a2-0.4.1/src/a2/utils/__pycache__/checks.cpython-310.pyc
+-rw-r--r--   0        0        0     1037 2023-06-13 15:02:52.894049 a2-0.4.1/src/a2/utils/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0     9546 2023-06-06 15:04:04.548994 a2-0.4.1/src/a2/utils/__pycache__/file_handling.cpython-310.pyc
+-rw-r--r--   0        0        0      445 2023-05-16 09:07:00.248323 a2-0.4.1/src/a2/utils/__pycache__/strings.cpython-310.pyc
+-rw-r--r--   0        0        0     6104 2023-05-16 09:07:00.248323 a2-0.4.1/src/a2/utils/__pycache__/testing.cpython-310.pyc
+-rw-r--r--   0        0        0      545 2022-12-14 09:39:28.222309 a2-0.4.1/src/a2/utils/__pycache__/times.cpython-310.pyc
+-rw-r--r--   0        0        0     7600 2023-06-13 15:02:53.402063 a2-0.4.1/src/a2/utils/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0    10872 2023-06-15 15:57:05.632744 a2-0.4.1/src/a2/utils/argparse.py
+-rw-r--r--   0        0        0      518 2023-05-11 10:46:59.965258 a2-0.4.1/src/a2/utils/checks.py
+-rw-r--r--   0        0        0      731 2023-06-13 14:57:04.760349 a2-0.4.1/src/a2/utils/constants.py
+-rw-r--r--   0        0        0     9361 2023-06-06 14:01:17.485564 a2-0.4.1/src/a2/utils/file_handling.py
+-rw-r--r--   0        0        0       90 2023-05-12 12:06:33.277030 a2-0.4.1/src/a2/utils/strings.py
+-rw-r--r--   0        0        0     5327 2023-05-12 12:06:33.277030 a2-0.4.1/src/a2/utils/testing.py
+-rw-r--r--   0        0        0      394 2022-12-14 09:36:33.154856 a2-0.4.1/src/a2/utils/times.py
+-rw-r--r--   0        0        0     7061 2023-06-13 14:57:08.084443 a2-0.4.1/src/a2/utils/utils.py
+-rw-r--r--   0        0        0     1947 1970-01-01 00:00:00.000000 a2-0.4.1/PKG-INFO
```

### Comparing `a2-0.4.0/pyproject.toml` & `a2-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "a2"
-version = "0.4.0"
+version = "0.4.1"
 description = "Package for predicting information about the weather from social media data as application 2 for maelstrom project"
 authors = ["Kristian Ehlert <kristian.ehlert@4-cast.de>"]
 packages = [{ include = "a2", from = "src"}]
 
 [tool.poetry.dependencies]
 # torch = {url = "https://download.pytorch.org/whl/cpu/torch-2.0.1%2Bcpu-cp310-cp310-linux_x86_64.whl", optional = true} # cannot upload this to package
 python = ">=3.10,<3.12"
```

### Comparing `a2-0.4.0/src/a2/cli/cli_plotting/__pycache__/single_plots.cpython-310.pyc` & `a2-0.4.1/src/a2/cli/cli_plotting/__pycache__/single_plots.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/cli/cli_plotting/single_plots.py` & `a2-0.4.1/src/a2/cli/cli_plotting/single_plots.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_df.csv` & `a2-0.4.1/src/a2/data/emoji/emoji_df.csv`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/0023_fe0f_20e3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/0023_fe0f_20e3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/002a_fe0f_20e3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/002a_fe0f_20e3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/0030_fe0f_20e3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/0030_fe0f_20e3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/0031_fe0f_20e3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/0031_fe0f_20e3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/0032_fe0f_20e3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/0032_fe0f_20e3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/0033_fe0f_20e3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/0033_fe0f_20e3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/0034_fe0f_20e3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/0034_fe0f_20e3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/0035_fe0f_20e3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/0035_fe0f_20e3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/0036_fe0f_20e3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/0036_fe0f_20e3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/0037_fe0f_20e3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/0037_fe0f_20e3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/0038_fe0f_20e3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/0038_fe0f_20e3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/0039_fe0f_20e3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/0039_fe0f_20e3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/00a9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/00a9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/00ae.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/00ae.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f004.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f004.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f0cf.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f0cf.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f170.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f170.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f171.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f171.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f17e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f17e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f17f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f17f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f18e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f18e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f191.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f191.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f192.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f192.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f193.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f193.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f194.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f194.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f195.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f195.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f196.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f196.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f197.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f197.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f198.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f198.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f199.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f199.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f19a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f19a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1e8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1e8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1e9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1e9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1ea.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1ea.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1eb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1eb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1ec.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1ec.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1ee.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1ee.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1f1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1f1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1f2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1f2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1f4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1f4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1f6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1f6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1f7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1f7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1f8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1f8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1f9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1f9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1fa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1fa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1fc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1fc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1fd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1fd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e6_1f1ff.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e6_1f1ff.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1e6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1e6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1e7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1e7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1e9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1e9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1ea.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1ea.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1eb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1eb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1ec.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1ec.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1ed.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1ed.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1ee.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1ee.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1ef.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1ef.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1f1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1f1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1f2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1f2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1f3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1f3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1f4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1f4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1f6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1f6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1f7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1f7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1f8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1f8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1f9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1f9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1fb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1fb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1fc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1fc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1fe.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1fe.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e7_1f1ff.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e7_1f1ff.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1e6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1e6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1e8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1e8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1e9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1e9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1eb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1eb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1ec.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1ec.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1ed.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1ed.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1ee.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1ee.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1f0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1f0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1f1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1f1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1f2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1f2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1f3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1f3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1f4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1f4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1f5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1f5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1f7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1f7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1fa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1fa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1fb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1fb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1fc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1fc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1fd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1fd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1fe.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1fe.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e8_1f1ff.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e8_1f1ff.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e9_1f1ea.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e9_1f1ea.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e9_1f1ec.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e9_1f1ec.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e9_1f1ef.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e9_1f1ef.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e9_1f1f0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e9_1f1f0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e9_1f1f2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e9_1f1f2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e9_1f1f4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e9_1f1f4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1e9_1f1ff.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1e9_1f1ff.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ea_1f1e6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ea_1f1e6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ea_1f1e8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ea_1f1e8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ea_1f1ea.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ea_1f1ea.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ea_1f1ec.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ea_1f1ec.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ea_1f1ed.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ea_1f1ed.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ea_1f1f7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ea_1f1f7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ea_1f1f8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ea_1f1f8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ea_1f1f9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ea_1f1f9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ea_1f1fa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ea_1f1fa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1eb_1f1ee.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1eb_1f1ee.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1eb_1f1ef.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1eb_1f1ef.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1eb_1f1f0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1eb_1f1f0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1eb_1f1f2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1eb_1f1f2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1eb_1f1f4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1eb_1f1f4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1eb_1f1f7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1eb_1f1f7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1e6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1e6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1e7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1e7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1e9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1e9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1ea.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1ea.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1eb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1eb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1ec.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1ec.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1ed.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1ed.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1ee.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1ee.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1f1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1f1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1f2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1f2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1f3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1f3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1f5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1f5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1f6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1f6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1f7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1f7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1f8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1f8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1f9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1f9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1fa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1fa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1fc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1fc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ec_1f1fe.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ec_1f1fe.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ed_1f1f0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ed_1f1f0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ed_1f1f2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ed_1f1f2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ed_1f1f3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ed_1f1f3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ed_1f1f7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ed_1f1f7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ed_1f1f9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ed_1f1f9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ed_1f1fa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ed_1f1fa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1e8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1e8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1e9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1e9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1ea.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1ea.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1f1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1f1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1f2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1f2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1f3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1f3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1f4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1f4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1f6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1f6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1f7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1f7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1f8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1f8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ee_1f1f9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ee_1f1f9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ef_1f1ea.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ef_1f1ea.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ef_1f1f2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ef_1f1f2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ef_1f1f4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ef_1f1f4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ef_1f1f5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ef_1f1f5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1ea.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1ea.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1ec.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1ec.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1ed.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1ed.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1ee.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1ee.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1f2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1f2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1f3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1f3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1f5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1f5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1f7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1f7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1fc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1fc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1fe.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1fe.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f0_1f1ff.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f0_1f1ff.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1e6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1e6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1e7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1e7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1e8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1e8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1ee.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1ee.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1f0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1f0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1f7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1f7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1f8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1f8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1f9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1f9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1fa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1fa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1fb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1fb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f1_1f1fe.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f1_1f1fe.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1e6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1e6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1e8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1e8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1e9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1e9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1ea.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1ea.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1eb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1eb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1ec.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1ec.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1ed.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1ed.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1f0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1f0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1f1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1f1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1f2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1f2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1f3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1f3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1f4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1f4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1f5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1f5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1f6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1f6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1f7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1f7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1f8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1f8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1f9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1f9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1fa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1fa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1fb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1fb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1fc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1fc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1fd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1fd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1fe.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1fe.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f2_1f1ff.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f2_1f1ff.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1e6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1e6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1e8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1e8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1ea.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1ea.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1eb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1eb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1ec.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1ec.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1ee.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1ee.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1f1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1f1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1f4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1f4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1f5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1f5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1f7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1f7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1fa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1fa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f3_1f1ff.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f3_1f1ff.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f4_1f1f2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f4_1f1f2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1e6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1e6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1ea.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1ea.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1eb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1eb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1ec.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1ec.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1ed.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1ed.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1f0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1f0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1f1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1f1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1f2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1f2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1f3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1f3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1f7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1f7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1f8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1f8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1f9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1f9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1fc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1fc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f5_1f1fe.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f5_1f1fe.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f6_1f1e6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f6_1f1e6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f7_1f1ea.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f7_1f1ea.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f7_1f1f4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f7_1f1f4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f7_1f1f8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f7_1f1f8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f7_1f1fa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f7_1f1fa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f7_1f1fc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f7_1f1fc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1e6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1e6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1e7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1e7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1e8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1e8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1e9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1e9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1ea.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1ea.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1ec.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1ec.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1ed.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1ed.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1ee.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1ee.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1ef.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1ef.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1f0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1f0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1f1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1f1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1f2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1f2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1f3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1f3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1f4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1f4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1f7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1f7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1f8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1f8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1f9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1f9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1fb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1fb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1fd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1fd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1fe.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1fe.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f8_1f1ff.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f8_1f1ff.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1e6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1e6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1e8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1e8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1e9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1e9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1eb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1eb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1ec.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1ec.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1ed.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1ed.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1ef.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1ef.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1f0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1f0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1f1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1f1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1f2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1f2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1f3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1f3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1f4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1f4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1f7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1f7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1f9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1f9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1fb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1fb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1fc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1fc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1f9_1f1ff.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1f9_1f1ff.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fa_1f1e6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fa_1f1e6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fa_1f1ec.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fa_1f1ec.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fa_1f1f2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fa_1f1f2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fa_1f1f3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fa_1f1f3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fa_1f1f8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fa_1f1f8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fa_1f1fe.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fa_1f1fe.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fa_1f1ff.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fa_1f1ff.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fb_1f1e6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fb_1f1e6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fb_1f1e8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fb_1f1e8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fb_1f1ea.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fb_1f1ea.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fb_1f1ec.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fb_1f1ec.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fb_1f1ee.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fb_1f1ee.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fb_1f1f3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fb_1f1f3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fb_1f1fa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fb_1f1fa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fc_1f1eb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fc_1f1eb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fc_1f1f8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fc_1f1f8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fd_1f1f0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fd_1f1f0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fe_1f1ea.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fe_1f1ea.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1fe_1f1f9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1fe_1f1f9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ff_1f1e6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ff_1f1e6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ff_1f1f2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ff_1f1f2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f1ff_1f1fc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f1ff_1f1fc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f201.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f201.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f202.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f202.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f21a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f21a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f22f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f22f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f232.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f232.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f233.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f233.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f234.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f234.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f235.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f235.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f236.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f236.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f237.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f237.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f238.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f238.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f239.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f239.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f23a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f23a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f250.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f250.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f251.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f251.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f300.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f300.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f301.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f301.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f302.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f302.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f303.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f303.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f304.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f304.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f305.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f305.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f306.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f306.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f307.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f307.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f308.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f308.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f309.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f309.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f30a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f30a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f30b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f30b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f30c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f30c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f30d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f30d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f30e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f30e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f30f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f30f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f310.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f310.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f311.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f311.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f312.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f312.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f313.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f313.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f314.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f314.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f315.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f315.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f316.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f316.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f317.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f317.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f318.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f318.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f319.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f319.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f31a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f31a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f31b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f31b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f31c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f31c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f31d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f31d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f31e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f31e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f31f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f31f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f320.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f320.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f321.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f321.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f324.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f324.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f325.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f325.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f326.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f326.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f327.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f327.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f328.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f328.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f329.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f329.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f32a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f32a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f32b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f32b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f32c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f32c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f32d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f32d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f32e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f32e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f32f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f32f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f330.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f330.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f331.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f331.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f332.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f332.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f333.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f333.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f334.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f334.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f335.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f335.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f336.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f336.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f337.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f337.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f338.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f338.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f339.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f339.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f33a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f33a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f33b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f33b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f33c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f33c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f33d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f33d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f33e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f33e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f33f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f33f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f340.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f340.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f341.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f341.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f342.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f342.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f343.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f343.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f344.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f344.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f345.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f345.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f346.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f346.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f347.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f347.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f348.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f348.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f349.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f349.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f34a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f34a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f34b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f34b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f34c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f34c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f34d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f34d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f34e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f34e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f34f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f34f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f350.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f350.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f351.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f351.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f352.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f352.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f353.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f353.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f354.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f354.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f355.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f355.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f356.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f356.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f357.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f357.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f358.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f358.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f359.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f359.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f35a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f35a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f35b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f35b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f35c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f35c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f35d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f35d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f35e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f35e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f35f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f35f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f360.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f360.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f361.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f361.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f362.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f362.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f363.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f363.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f364.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f364.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f365.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f365.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f366.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f366.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f367.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f367.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f368.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f368.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f369.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f369.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f36a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f36a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f36b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f36b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f36c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f36c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f36d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f36d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f36e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f36e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f36f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f36f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f370.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f370.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f371.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f371.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f372.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f372.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f373.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f373.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f374.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f374.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f375.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f375.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f376.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f376.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f377.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f377.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f378.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f378.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f379.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f379.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f37a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f37a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f37b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f37b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f37c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f37c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f37d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f37d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f37e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f37e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f37f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f37f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f380.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f380.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f381.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f381.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f382.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f382.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f383.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f383.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f384.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f384.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f385.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f385.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f386.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f386.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f387.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f387.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f388.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f388.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f389.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f389.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f38a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f38a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f38b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f38b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f38c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f38c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f38d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f38d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f38e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f38e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f38f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f38f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f390.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f390.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f391.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f391.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f392.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f392.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f393.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f393.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f396.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f396.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f397.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f397.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f399.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f399.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f39a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f39a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f39b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f39b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f39e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f39e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f39f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f39f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3a0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3a0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3a1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3a1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3a2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3a2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3a3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3a3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3a4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3a4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3a5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3a5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3a6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3a6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3a7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3a7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3a8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3a8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3a9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3a9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3aa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3aa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ab.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ab.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ac.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ac.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ad.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ad.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ae.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ae.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3af.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3af.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3b0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3b0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3b1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3b1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3b2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3b2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3b3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3b3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3b4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3b4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3b5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3b5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3b6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3b6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3b7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3b7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3b8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3b8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3b9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3b9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ba.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ba.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3bb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3bb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3bc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3bc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3bd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3bd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3be.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3be.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3bf.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3bf.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c3_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c3_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c3_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c3_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c4_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c4_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c4_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c4_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3c9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3c9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ca.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ca.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ca_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ca_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ca_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ca_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3cb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3cb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3cb_fe0f_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3cb_fe0f_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3cb_fe0f_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3cb_fe0f_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3cc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3cc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3cc_fe0f_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3cc_fe0f_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3cc_fe0f_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3cc_fe0f_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3cd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3cd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ce.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ce.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3cf.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3cf.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3d0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3d0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3d1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3d1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3d2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3d2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3d3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3d3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3d4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3d4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3d5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3d5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3d6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3d6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3d7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3d7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3d8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3d8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3d9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3d9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3da.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3da.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3db.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3db.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3dc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3dc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3dd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3dd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3de.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3de.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3df.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3df.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3e0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3e0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3e1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3e1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3e2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3e2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3e3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3e3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3e4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3e4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3e5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3e5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3e6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3e6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3e7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3e7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3e8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3e8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3e9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3e9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ea.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ea.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3eb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3eb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ec.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ec.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ed.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ed.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ee.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ee.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3ef.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3ef.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f3_fe0f_200d_1f308.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f3_fe0f_200d_1f308.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f3_fe0f_200d_26a7_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f3_fe0f_200d_26a7_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f4_200d_2620_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f4_200d_2620_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f4_e0067_e0062_e0065_e006e_e0067_e007f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f4_e0067_e0062_e0065_e006e_e0067_e007f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f4_e0067_e0062_e0073_e0063_e0074_e007f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f4_e0067_e0062_e0073_e0063_e0074_e007f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f4_e0067_e0062_e0077_e006c_e0073_e007f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f4_e0067_e0062_e0077_e006c_e0073_e007f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3f9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3f9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f3fa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f3fa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f400.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f400.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f401.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f401.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f402.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f402.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f403.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f403.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f404.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f404.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f405.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f405.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f406.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f406.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f407.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f407.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f408.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f408.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f408_200d_2b1b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f408_200d_2b1b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f409.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f409.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f40a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f40a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f40b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f40b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f40c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f40c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f40d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f40d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f40e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f40e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f40f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f40f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f410.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f410.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f411.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f411.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f412.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f412.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f413.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f413.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f414.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f414.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f415.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f415.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f415_200d_1f9ba.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f415_200d_1f9ba.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f416.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f416.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f417.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f417.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f418.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f418.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f419.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f419.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f41a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f41a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f41b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f41b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f41c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f41c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f41d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f41d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f41e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f41e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f41f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f41f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f420.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f420.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f421.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f421.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f422.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f422.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f423.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f423.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f424.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f424.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f425.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f425.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f426.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f426.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f427.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f427.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f428.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f428.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f429.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f429.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f42a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f42a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f42b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f42b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f42c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f42c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f42d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f42d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f42e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f42e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f42f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f42f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f430.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f430.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f431.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f431.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f432.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f432.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f433.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f433.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f434.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f434.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f435.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f435.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f436.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f436.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f437.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f437.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f438.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f438.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f439.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f439.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f43a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f43a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f43b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f43b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f43b_200d_2744_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f43b_200d_2744_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f43c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f43c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f43d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f43d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f43e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f43e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f43f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f43f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f440.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f440.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f441.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f441.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f441_fe0f_200d_1f5e8_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f441_fe0f_200d_1f5e8_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f442.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f442.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f443.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f443.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f444.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f444.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f445.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f445.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f446.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f446.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f447.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f447.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f448.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f448.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f449.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f449.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f44a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f44a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f44b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f44b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f44c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f44c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f44d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f44d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f44e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f44e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f44f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f44f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f450.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f450.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f451.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f451.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f452.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f452.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f453.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f453.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f454.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f454.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f455.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f455.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f456.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f456.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f457.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f457.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f458.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f458.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f459.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f459.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f45a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f45a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f45b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f45b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f45c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f45c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f45d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f45d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f45e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f45e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f45f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f45f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f460.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f460.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f461.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f461.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f462.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f462.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f463.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f463.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f464.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f464.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f465.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f465.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f466.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f466.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f467.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f467.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f33e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f33e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f373.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f373.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f37c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f37c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f393.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f393.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f3a4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f3a4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f3a8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f3a8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f3eb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f3eb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f3ed.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f3ed.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f466.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f466.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f466_200d_1f466.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f466_200d_1f466.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f467.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f467.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f467_200d_1f466.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f467_200d_1f466.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f467_200d_1f467.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f467_200d_1f467.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f466.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f466.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f466_200d_1f466.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f466_200d_1f466.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f467.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f467.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f467_200d_1f466.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f467_200d_1f466.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f467_200d_1f467.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f467_200d_1f467.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f466.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f466.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f466_200d_1f466.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f466_200d_1f466.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f467.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f467.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f467_200d_1f466.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f467_200d_1f466.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f467_200d_1f467.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f467_200d_1f467.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f4bb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f4bb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f4bc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f4bc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f527.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f527.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f52c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f52c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f680.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f680.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f692.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f692.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f9af.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f9af.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f9b0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f9b0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f9b1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f9b1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f9b2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f9b2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f9b3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f9b3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f9bc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f9bc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_1f9bd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_1f9bd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_2695_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_2695_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_2696_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_2696_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_2708_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_2708_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_2764_fe0f_200d_1f468.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_2764_fe0f_200d_1f468.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f468_200d_2764_fe0f_200d_1f48b_200d_1f468.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f468_200d_2764_fe0f_200d_1f48b_200d_1f468.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f33e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f33e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f373.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f373.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f37c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f37c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f393.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f393.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f3a4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f3a4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f3a8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f3a8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f3eb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f3eb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f3ed.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f3ed.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f466.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f466.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f466_200d_1f466.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f466_200d_1f466.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f467.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f467.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f467_200d_1f466.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f467_200d_1f466.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f467_200d_1f467.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f467_200d_1f467.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f466.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f466.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f466_200d_1f466.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f466_200d_1f466.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f467.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f467.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f467_200d_1f466.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f467_200d_1f466.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f467_200d_1f467.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f467_200d_1f467.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f4bb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f4bb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f4bc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f4bc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f527.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f527.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f52c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f52c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f680.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f680.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f692.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f692.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f9af.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f9af.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f9b0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f9b0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f9b1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f9b1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f9b2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f9b2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f9b3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f9b3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f9bc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f9bc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_1f9bd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_1f9bd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_2695_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_2695_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_2696_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_2696_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_2708_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_2708_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f468.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f468.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f469.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f469.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f48b_200d_1f468.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f48b_200d_1f468.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f48b_200d_1f469.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f48b_200d_1f469.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f46a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f46a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f46b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f46b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f46c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f46c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f46d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f46d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f46e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f46e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f46e_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f46e_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f46e_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f46e_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f46f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f46f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f46f_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f46f_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f46f_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f46f_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f470.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f470.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f470_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f470_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f470_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f470_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f471.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f471.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f471_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f471_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f471_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f471_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f472.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f472.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f473.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f473.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f473_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f473_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f473_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f473_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f474.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f474.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f475.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f475.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f476.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f476.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f477.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f477.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f477_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f477_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f477_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f477_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f478.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f478.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f479.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f479.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f47a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f47a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f47b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f47b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f47c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f47c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f47d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f47d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f47e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f47e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f47f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f47f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f480.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f480.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f481.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f481.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f481_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f481_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f481_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f481_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f482.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f482.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f482_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f482_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f482_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f482_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f483.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f483.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f484.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f484.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f485.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f485.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f486.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f486.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f486_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f486_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f486_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f486_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f487.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f487.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f487_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f487_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f487_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f487_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f488.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f488.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f489.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f489.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f48a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f48a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f48b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f48b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f48c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f48c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f48d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f48d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f48e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f48e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f48f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f48f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f490.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f490.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f491.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f491.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f492.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f492.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f493.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f493.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f494.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f494.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f495.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f495.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f496.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f496.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f497.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f497.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f498.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f498.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f499.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f499.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f49a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f49a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f49b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f49b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f49c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f49c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f49d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f49d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f49e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f49e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f49f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f49f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4a0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4a0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4a1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4a1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4a2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4a2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4a3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4a3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4a4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4a4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4a5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4a5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4a6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4a6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4a7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4a7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4a8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4a8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4a9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4a9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4aa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4aa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ab.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ab.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ac.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ac.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ad.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ad.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ae.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ae.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4af.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4af.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4b0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4b0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4b1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4b1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4b2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4b2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4b3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4b3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4b4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4b4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4b5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4b5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4b6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4b6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4b7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4b7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4b8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4b8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4b9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4b9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ba.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ba.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4bb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4bb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4bc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4bc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4bd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4bd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4be.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4be.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4bf.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4bf.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4c0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4c0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4c1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4c1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4c2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4c2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4c3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4c3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4c4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4c4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4c5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4c5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4c6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4c6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4c7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4c7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4c8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4c8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4c9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4c9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ca.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ca.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4cb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4cb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4cc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4cc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4cd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4cd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ce.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ce.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4cf.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4cf.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4d0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4d0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4d1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4d1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4d2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4d2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4d3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4d3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4d4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4d4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4d5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4d5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4d6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4d6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4d7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4d7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4d8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4d8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4d9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4d9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4da.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4da.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4db.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4db.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4dc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4dc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4dd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4dd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4de.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4de.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4df.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4df.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4e0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4e0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4e1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4e1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4e2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4e2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4e3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4e3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4e4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4e4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4e5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4e5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4e6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4e6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4e7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4e7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4e8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4e8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4e9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4e9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ea.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ea.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4eb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4eb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ec.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ec.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ed.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ed.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ee.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ee.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ef.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ef.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4f0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4f0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4f1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4f1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4f2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4f2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4f3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4f3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4f4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4f4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4f5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4f5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4f6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4f6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4f7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4f7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4f8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4f8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4f9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4f9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4fa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4fa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4fb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4fb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4fc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4fc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4fd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4fd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f4ff.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f4ff.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f500.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f500.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f501.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f501.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f502.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f502.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f503.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f503.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f504.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f504.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f505.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f505.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f506.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f506.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f507.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f507.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f508.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f508.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f509.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f509.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f50a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f50a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f50b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f50b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f50c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f50c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f50d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f50d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f50e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f50e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f50f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f50f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f510.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f510.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f511.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f511.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f512.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f512.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f513.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f513.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f514.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f514.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f515.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f515.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f516.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f516.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f517.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f517.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f518.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f518.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f519.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f519.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f51a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f51a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f51b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f51b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f51c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f51c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f51d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f51d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f51e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f51e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f51f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f51f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f520.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f520.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f521.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f521.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f522.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f522.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f523.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f523.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f524.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f524.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f525.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f525.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f526.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f526.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f527.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f527.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f528.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f528.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f529.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f529.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f52a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f52a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f52b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f52b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f52c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f52c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f52d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f52d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f52e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f52e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f52f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f52f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f530.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f530.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f531.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f531.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f532.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f532.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f533.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f533.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f534.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f534.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f535.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f535.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f536.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f536.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f537.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f537.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f538.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f538.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f539.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f539.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f53a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f53a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f53b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f53b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f53c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f53c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f53d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f53d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f549.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f549.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f54a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f54a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f54b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f54b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f54c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f54c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f54d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f54d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f54e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f54e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f550.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f550.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f551.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f551.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f552.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f552.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f553.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f553.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f554.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f554.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f555.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f555.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f556.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f556.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f557.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f557.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f558.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f558.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f559.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f559.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f55a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f55a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f55b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f55b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f55c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f55c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f55d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f55d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f55e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f55e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f55f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f55f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f560.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f560.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f561.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f561.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f562.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f562.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f563.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f563.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f564.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f564.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f565.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f565.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f566.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f566.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f567.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f567.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f56f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f56f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f570.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f570.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f573.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f573.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f574.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f574.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f575.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f575.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f575_fe0f_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f575_fe0f_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f575_fe0f_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f575_fe0f_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f576.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f576.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f577.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f577.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f578.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f578.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f579.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f579.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f57a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f57a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f587.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f587.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f58a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f58a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f58b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f58b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f58c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f58c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f58d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f58d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f590.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f590.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f595.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f595.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f596.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f596.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5a4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5a4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5a5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5a5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5a8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5a8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5b1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5b1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5b2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5b2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5bc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5bc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5c2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5c2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5c3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5c3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5c4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5c4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5d1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5d1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5d2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5d2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5d3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5d3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5dc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5dc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5dd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5dd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5de.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5de.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5e1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5e1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5e3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5e3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5e8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5e8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5ef.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5ef.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5f3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5f3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5fa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5fa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5fb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5fb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5fc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5fc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5fd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5fd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5fe.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5fe.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f5ff.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f5ff.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f600.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f600.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f601.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f601.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f602.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f602.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f603.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f603.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f604.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f604.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f605.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f605.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f606.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f606.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f607.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f607.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f608.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f608.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f609.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f609.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f60a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f60a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f60b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f60b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f60c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f60c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f60d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f60d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f60e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f60e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f60f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f60f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f610.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f610.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f611.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f611.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f612.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f612.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f613.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f613.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f614.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f614.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f615.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f615.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f616.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f616.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f617.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f617.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f618.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f618.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f619.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f619.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f61a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f61a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f61b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f61b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f61c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f61c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f61d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f61d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f61e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f61e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f61f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f61f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f620.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f620.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f621.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f621.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f622.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f622.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f623.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f623.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f624.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f624.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f625.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f625.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f626.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f626.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f627.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f627.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f628.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f628.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f629.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f629.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f62a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f62a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f62b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f62b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f62c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f62c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f62d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f62d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f62e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f62e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f62e_200d_1f4a8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f62e_200d_1f4a8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f62f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f62f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f630.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f630.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f631.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f631.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f632.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f632.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f633.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f633.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f634.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f634.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f635.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f635.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f635_200d_1f4ab.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f635_200d_1f4ab.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f636.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f636.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f636_200d_1f32b_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f636_200d_1f32b_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f637.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f637.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f638.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f638.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f639.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f639.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f63a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f63a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f63b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f63b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f63c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f63c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f63d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f63d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f63e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f63e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f63f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f63f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f640.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f640.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f641.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f641.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f642.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f642.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f643.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f643.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f644.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f644.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f645.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f645.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f645_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f645_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f645_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f645_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f646.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f646.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f646_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f646_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f646_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f646_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f647.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f647.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f647_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f647_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f647_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f647_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f648.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f648.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f649.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f649.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f64a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f64a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f64b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f64b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f64b_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f64b_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f64b_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f64b_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f64c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f64c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f64d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f64d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f64d_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f64d_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f64d_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f64d_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f64e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f64e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f64e_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f64e_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f64e_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f64e_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f64f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f64f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f680.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f680.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f681.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f681.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f682.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f682.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f683.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f683.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f684.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f684.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f685.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f685.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f686.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f686.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f687.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f687.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f688.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f688.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f689.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f689.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f68a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f68a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f68b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f68b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f68c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f68c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f68d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f68d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f68e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f68e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f68f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f68f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f690.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f690.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f691.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f691.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f692.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f692.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f693.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f693.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f694.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f694.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f695.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f695.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f696.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f696.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f697.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f697.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f698.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f698.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f699.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f699.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f69a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f69a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f69b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f69b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f69c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f69c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f69d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f69d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f69e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f69e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f69f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f69f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a3_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a3_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a3_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a3_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6a9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6a9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6aa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6aa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6ab.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6ab.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6ac.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6ac.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6ad.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6ad.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6ae.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6ae.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6af.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6af.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b4_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b4_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b4_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b4_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b5_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b5_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b5_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b5_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b6_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b6_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b6_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b6_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6b9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6b9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6ba.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6ba.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6bb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6bb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6bc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6bc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6bd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6bd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6be.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6be.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6bf.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6bf.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6c0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6c0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6c1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6c1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6c2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6c2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6c3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6c3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6c4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6c4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6c5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6c5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6cb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6cb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6cc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6cc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6cd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6cd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6ce.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6ce.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6cf.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6cf.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6d0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6d0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6d1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6d1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6d2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6d2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6d5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6d5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6d6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6d6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6d7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6d7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6dd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6dd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6de.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6de.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6df.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6df.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6e0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6e0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6e1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6e1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6e2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6e2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6e3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6e3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6e4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6e4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6e5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6e5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6e9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6e9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6eb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6eb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6ec.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6ec.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6f0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6f0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6f3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6f3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6f4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6f4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6f5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6f5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6f6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6f6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6f7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6f7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6f8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6f8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6f9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6f9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6fa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6fa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6fb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6fb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f6fc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f6fc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f7e0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f7e0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f7e1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f7e1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f7e2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f7e2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f7e3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f7e3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f7e4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f7e4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f7e5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f7e5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f7e6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f7e6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f7e8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f7e8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f7e9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f7e9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f7ea.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f7ea.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f7eb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f7eb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f90c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f90c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f90d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f90d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f90e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f90e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f90f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f90f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f910.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f910.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f911.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f911.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f912.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f912.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f913.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f913.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f914.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f914.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f915.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f915.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f916.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f916.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f917.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f917.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f918.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f918.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f919.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f919.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f91a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f91a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f91b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f91b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f91c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f91c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f91d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f91d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f91e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f91e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f91f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f91f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f920.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f920.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f921.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f921.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f922.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f922.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f923.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f923.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f924.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f924.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f925.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f925.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f926.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f926.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f926_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f926_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f926_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f926_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f927.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f927.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f928.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f928.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f929.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f929.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f92a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f92a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f92b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f92b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f92c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f92c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f92d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f92d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f92e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f92e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f92f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f92f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f930.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f930.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f931.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f931.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f932.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f932.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f933.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f933.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f934.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f934.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f935.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f935.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f935_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f935_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f935_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f935_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f936.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f936.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f937.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f937.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f937_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f937_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f937_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f937_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f938.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f938.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f938_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f938_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f938_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f938_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f939.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f939.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f939_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f939_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f939_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f939_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f93a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f93a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f93c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f93c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f93c_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f93c_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f93c_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f93c_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f93d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f93d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f93d_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f93d_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f93d_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f93d_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f93e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f93e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f93e_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f93e_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f93e_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f93e_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f93f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f93f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f940.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f940.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f941.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f941.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f942.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f942.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f943.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f943.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f944.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f944.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f945.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f945.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f947.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f947.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f948.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f948.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f949.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f949.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f94a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f94a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f94b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f94b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f94c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f94c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f94d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f94d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f94e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f94e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f94f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f94f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f950.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f950.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f951.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f951.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f952.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f952.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f953.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f953.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f954.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f954.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f955.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f955.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f956.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f956.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f957.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f957.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f958.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f958.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f959.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f959.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f95a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f95a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f95b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f95b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f95c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f95c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f95d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f95d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f95e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f95e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f95f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f95f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f960.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f960.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f961.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f961.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f962.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f962.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f963.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f963.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f964.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f964.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f965.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f965.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f966.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f966.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f967.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f967.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f968.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f968.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f969.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f969.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f96a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f96a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f96b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f96b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f96c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f96c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f96d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f96d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f96e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f96e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f96f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f96f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f970.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f970.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f971.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f971.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f972.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f972.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f973.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f973.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f974.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f974.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f975.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f975.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f976.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f976.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f977.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f977.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f978.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f978.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f979.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f979.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f97a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f97a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f97b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f97b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f97c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f97c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f97d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f97d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f97e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f97e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f97f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f97f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f980.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f980.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f981.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f981.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f982.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f982.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f983.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f983.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f984.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f984.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f985.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f985.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f986.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f986.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f987.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f987.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f988.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f988.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f989.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f989.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f98a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f98a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f98b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f98b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f98c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f98c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f98d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f98d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f98e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f98e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f98f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f98f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f990.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f990.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f991.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f991.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f992.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f992.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f993.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f993.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f994.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f994.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f995.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f995.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f996.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f996.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f997.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f997.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f998.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f998.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f999.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f999.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f99a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f99a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f99b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f99b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f99c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f99c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f99d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f99d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f99e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f99e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f99f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f99f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9a0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9a0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9a1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9a1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9a2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9a2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9a3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9a3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9a4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9a4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9a5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9a5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9a6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9a6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9a7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9a7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9a8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9a8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9a9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9a9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9aa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9aa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ab.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ab.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ac.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ac.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ad.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ad.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ae.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ae.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9af.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9af.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b8_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b8_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b8_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b8_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b9_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b9_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9b9_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9b9_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ba.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ba.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9bb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9bb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9bc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9bc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9bd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9bd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9be.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9be.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9bf.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9bf.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9c0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9c0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9c1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9c1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9c2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9c2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9c3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9c3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9c4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9c4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9c5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9c5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9c6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9c6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9c7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9c7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9c8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9c8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9c9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9c9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ca.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ca.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9cb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9cb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9cc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9cc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9cd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9cd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9cd_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9cd_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9cd_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9cd_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ce.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ce.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ce_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ce_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ce_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ce_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9cf.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9cf.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9cf_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9cf_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9cf_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9cf_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f33e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f33e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f373.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f373.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f37c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f37c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f384.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f384.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f393.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f393.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3a4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3a4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3a8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3a8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3eb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3eb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3ed.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3ed.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f4bb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f4bb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f4bc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f4bc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f527.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f527.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f52c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f52c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f680.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f680.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f692.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f692.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f91d_200d_1f9d1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f91d_200d_1f9d1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9af.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9af.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9bc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9bc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9bd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9bd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_2695_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_2695_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_2696_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_2696_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d1_200d_2708_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d1_200d_2708_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d4_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d4_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d4_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d4_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d6_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d6_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d6_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d6_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d7_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d7_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d7_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d7_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d8_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d8_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d8_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d8_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d9_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d9_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9d9_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9d9_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9da.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9da.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9da_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9da_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9da_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9da_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9db.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9db.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9db_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9db_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9db_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9db_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9dc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9dc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9dc_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9dc_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9dc_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9dc_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9dd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9dd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9dd_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9dd_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9dd_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9dd_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9de.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9de.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9de_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9de_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9de_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9de_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9df.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9df.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9df_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9df_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9df_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9df_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9e0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9e0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9e1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9e1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9e2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9e2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9e3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9e3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9e4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9e4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9e5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9e5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9e6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9e6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9e7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9e7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9e8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9e8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9e9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9e9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ea.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ea.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9eb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9eb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ec.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ec.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ed.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ed.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ee.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ee.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ef.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ef.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9f0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9f0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9f1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9f1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9f2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9f2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9f3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9f3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9f4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9f4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9f5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9f5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9f6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9f6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9f7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9f7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9f8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9f8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9f9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9f9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9fa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9fa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9fb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9fb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9fc.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9fc.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9fd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9fd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9fe.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9fe.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1f9ff.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1f9ff.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa70.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa70.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa71.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa71.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa72.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa72.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa73.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa73.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa74.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa74.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa78.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa78.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa79.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa79.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa7a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa7a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa7b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa7b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa7c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa7c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa80.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa80.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa81.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa81.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa82.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa82.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa83.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa83.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa84.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa84.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa85.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa85.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa86.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa86.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa90.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa90.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa91.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa91.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa92.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa92.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa93.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa93.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa94.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa94.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa95.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa95.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa96.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa96.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa97.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa97.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa98.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa98.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa99.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa99.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa9a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa9a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa9b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa9b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa9c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa9c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa9d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa9d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa9e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa9e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fa9f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fa9f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1faa0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1faa0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1faa1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1faa1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1faa2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1faa2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1faa3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1faa3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1faa4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1faa4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1faa5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1faa5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1faa6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1faa6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1faa7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1faa7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1faa8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1faa8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1faa9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1faa9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1faaa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1faaa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1faab.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1faab.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1faac.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1faac.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fab0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fab0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fab1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fab1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fab2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fab2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fab3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fab3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fab4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fab4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fab5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fab5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fab6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fab6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fab7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fab7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fab8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fab8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fab9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fab9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1faba.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1faba.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fac0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fac0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fac1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fac1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fac2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fac2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fac3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fac3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fac4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fac4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fac5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fac5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fad0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fad0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fad1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fad1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fad2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fad2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fad3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fad3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fad4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fad4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fad5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fad5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fad6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fad6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fad7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fad7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fad8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fad8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fad9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fad9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fae0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fae0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fae1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fae1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fae2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fae2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fae3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fae3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fae4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fae4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fae5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fae5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fae6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fae6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1fae7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1fae7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1faf0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1faf0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1faf1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1faf1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1faf2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1faf2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1faf3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1faf3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1faf4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1faf4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1faf5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1faf5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/1faf6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/1faf6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/203c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/203c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2049.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2049.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2122.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2122.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2139.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2139.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2194.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2194.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2195.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2195.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2196.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2196.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2197.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2197.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2198.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2198.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2199.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2199.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/21a9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/21a9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/21aa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/21aa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/231a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/231a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/231b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/231b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2328.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2328.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/23cf.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/23cf.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/23e9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/23e9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/23ea.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/23ea.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/23eb.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/23eb.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/23ec.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/23ec.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/23ed.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/23ed.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/23ee.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/23ee.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/23ef.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/23ef.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/23f0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/23f0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/23f1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/23f1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/23f2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/23f2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/23f3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/23f3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/23f8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/23f8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/23f9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/23f9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/23fa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/23fa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/24c2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/24c2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/25b6.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/25b6.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/25c0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/25c0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2600.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2600.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2601.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2601.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2602.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2602.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2603.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2603.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2604.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2604.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/260e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/260e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2611.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2611.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2614.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2614.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2615.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2615.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2618.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2618.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/261d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/261d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2620.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2620.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2622.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2622.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2623.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2623.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2626.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2626.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/262a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/262a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/262e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/262e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/262f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/262f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2638.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2638.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2639.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2639.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/263a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/263a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2640.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2640.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2642.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2642.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2648.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2648.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2649.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2649.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/264a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/264a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/264b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/264b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/264c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/264c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/264d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/264d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/264e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/264e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/264f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/264f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2650.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2650.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2651.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2651.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2652.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2652.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2653.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2653.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/265f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/265f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2660.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2660.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2663.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2663.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2665.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2665.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2666.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2666.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2668.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2668.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/267b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/267b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/267e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/267e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/267f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/267f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2692.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2692.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2693.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2693.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2694.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2694.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2695.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2695.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2696.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2696.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2697.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2697.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2699.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2699.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/269b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/269b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/269c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/269c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26a0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26a0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26a1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26a1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26a7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26a7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26aa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26aa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26ab.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26ab.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26b0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26b0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26b1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26b1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26bd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26bd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26be.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26be.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26c4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26c4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26c5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26c5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26c8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26c8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26ce.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26ce.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26cf.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26cf.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26d1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26d1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26d3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26d3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26d4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26d4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26e9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26e9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26ea.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26ea.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26f0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26f0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26f1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26f1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26f2.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26f2.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26f3.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26f3.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26f4.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26f4.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26f5.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26f5.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26f7.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26f7.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26f8.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26f8.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26f9.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26f9.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26f9_fe0f_200d_2640_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26f9_fe0f_200d_2640_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26f9_fe0f_200d_2642_fe0f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26f9_fe0f_200d_2642_fe0f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26fa.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26fa.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/26fd.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/26fd.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2702.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2702.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2705.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2705.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2708.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2708.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2709.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2709.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/270a.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/270a.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/270b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/270b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/270c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/270c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/270d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/270d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/270f.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/270f.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2712.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2712.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2714.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2714.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2716.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2716.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/271d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/271d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2721.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2721.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2728.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2728.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2733.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2733.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2734.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2734.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2744.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2744.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2747.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2747.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/274c.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/274c.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/274e.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/274e.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2753.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2753.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2754.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2754.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2755.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2755.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2757.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2757.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2763.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2763.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2764.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2764.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2764_fe0f_200d_1f525.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2764_fe0f_200d_1f525.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2764_fe0f_200d_1fa79.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2764_fe0f_200d_1fa79.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/27a1.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/27a1.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/27b0.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/27b0.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/27bf.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/27bf.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2934.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2934.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2935.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2935.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2b05.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2b05.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2b06.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2b06.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2b07.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2b07.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2b1b.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2b1b.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2b50.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2b50.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/2b55.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/2b55.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/3030.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/3030.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/303d.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/303d.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/3297.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/3297.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/emoji/emoji_images/3299.png` & `a2-0.4.1/src/a2/data/emoji/emoji_images/3299.png`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/font/Symbola.ttf` & `a2-0.4.1/src/a2/data/font/Symbola.ttf`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/font/Symbola_hint.ttf` & `a2-0.4.1/src/a2/data/font/Symbola_hint.ttf`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt` & `a2-0.4.1/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/dataset/__pycache__/emojis.cpython-310.pyc` & `a2-0.4.1/src/a2/dataset/__pycache__/emojis.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/dataset/__pycache__/load_dataset.cpython-310.pyc` & `a2-0.4.1/src/a2/dataset/__pycache__/load_dataset.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/dataset/__pycache__/radar.cpython-310.pyc` & `a2-0.4.1/src/a2/dataset/__pycache__/radar.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/dataset/__pycache__/stations.cpython-310.pyc` & `a2-0.4.1/src/a2/dataset/__pycache__/stations.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/dataset/__pycache__/tweets.cpython-310.pyc` & `a2-0.4.1/src/a2/dataset/__pycache__/tweets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/dataset/__pycache__/units.cpython-310.pyc` & `a2-0.4.1/src/a2/dataset/__pycache__/units.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/dataset/__pycache__/utils_dataset.cpython-310.pyc` & `a2-0.4.1/src/a2/dataset/__pycache__/utils_dataset.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/dataset/emojis.py` & `a2-0.4.1/src/a2/dataset/emojis.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/dataset/load_dataset.py` & `a2-0.4.1/src/a2/dataset/load_dataset.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/dataset/radar.py` & `a2-0.4.1/src/a2/dataset/radar.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/dataset/stations.py` & `a2-0.4.1/src/a2/dataset/stations.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/dataset/tweets.py` & `a2-0.4.1/src/a2/dataset/tweets.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/dataset/units.py` & `a2-0.4.1/src/a2/dataset/units.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/dataset/utils_dataset.py` & `a2-0.4.1/src/a2/dataset/utils_dataset.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/plotting/__pycache__/analysis.cpython-310.pyc` & `a2-0.4.1/src/a2/plotting/__pycache__/analysis.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/plotting/__pycache__/axes_utils.cpython-310.pyc` & `a2-0.4.1/src/a2/plotting/__pycache__/axes_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/plotting/__pycache__/colormesh.cpython-310.pyc` & `a2-0.4.1/src/a2/plotting/__pycache__/colormesh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/plotting/__pycache__/figures.cpython-310.pyc` & `a2-0.4.1/src/a2/plotting/__pycache__/figures.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/plotting/__pycache__/histogram_2d_utils.cpython-310.pyc` & `a2-0.4.1/src/a2/plotting/__pycache__/histogram_2d_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/plotting/__pycache__/histograms.cpython-310.pyc` & `a2-0.4.1/src/a2/plotting/__pycache__/histograms.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/plotting/__pycache__/parallel_plotting.cpython-310.pyc` & `a2-0.4.1/src/a2/plotting/__pycache__/parallel_plotting.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/plotting/__pycache__/timeseries.cpython-310.pyc` & `a2-0.4.1/src/a2/plotting/__pycache__/timeseries.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/plotting/__pycache__/utils_plotting.cpython-310.pyc` & `a2-0.4.1/src/a2/plotting/__pycache__/utils_plotting.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/plotting/__pycache__/weather_maps.cpython-310.pyc` & `a2-0.4.1/src/a2/plotting/__pycache__/weather_maps.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/plotting/analysis.py` & `a2-0.4.1/src/a2/plotting/analysis.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/plotting/axes_utils.py` & `a2-0.4.1/src/a2/plotting/axes_utils.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/plotting/colormesh.py` & `a2-0.4.1/src/a2/plotting/colormesh.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/plotting/histogram_2d_utils.py` & `a2-0.4.1/src/a2/plotting/histogram_2d_utils.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/plotting/histograms.py` & `a2-0.4.1/src/a2/plotting/histograms.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/plotting/parallel_plotting.py` & `a2-0.4.1/src/a2/plotting/parallel_plotting.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/plotting/timeseries.py` & `a2-0.4.1/src/a2/plotting/timeseries.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/plotting/utils_plotting.py` & `a2-0.4.1/src/a2/plotting/utils_plotting.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/plotting/weather_maps.py` & `a2-0.4.1/src/a2/plotting/weather_maps.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/preprocess/__pycache__/embedding.cpython-310.pyc` & `a2-0.4.1/src/a2/preprocess/__pycache__/embedding.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/preprocess/__pycache__/normalize_text.cpython-310.pyc` & `a2-0.4.1/src/a2/preprocess/__pycache__/normalize_text.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/preprocess/embedding.py` & `a2-0.4.1/src/a2/preprocess/embedding.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/preprocess/normalize_text.py` & `a2-0.4.1/src/a2/preprocess/normalize_text.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/training/__pycache__/benchmarks.cpython-310.pyc` & `a2-0.4.1/src/a2/training/__pycache__/benchmarks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/training/__pycache__/dataset_hugging.cpython-310.pyc` & `a2-0.4.1/src/a2/training/__pycache__/dataset_hugging.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/training/__pycache__/evaluate_hugging.cpython-310.pyc` & `a2-0.4.1/src/a2/training/__pycache__/evaluate_hugging.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/training/__pycache__/tracking.cpython-310.pyc` & `a2-0.4.1/src/a2/training/__pycache__/tracking.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/training/__pycache__/tracking_hugging.cpython-310.pyc` & `a2-0.4.1/src/a2/training/__pycache__/tracking_hugging.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/training/__pycache__/training_deep500.cpython-310.pyc` & `a2-0.4.1/src/a2/training/__pycache__/training_deep500.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/training/__pycache__/training_hugging.cpython-310.pyc` & `a2-0.4.1/src/a2/training/__pycache__/training_hugging.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  9 13:11:33 2023 UTC, .py size: 12776 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,597 +1,622 @@
-00000000: 6f0d 0d0a 0000 0000 0525 8364 e831 0000  o........%.d.1..
+00000000: 6f0d 0d0a 0000 0000 022c 8b64 9633 0000  o........,.d.3..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000d 0000 0040 0000 0073 2401 0000 6400  .....@...s$...d.
+00000020: 000d 0000 0040 0000 0073 5001 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c05 5a06 6400 6401 6c07 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c08 5a06 6400 6401 6c09 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6401 6c0a 5a0a 6400 6401 6c0b 5a0c 6400  d.l.Z.d.d.l.Z.d.
 00000080: 6401 6c0d 5a0e 6400 6401 6c0f 5a0f 6400  d.l.Z.d.d.l.Z.d.
 00000090: 6401 6c10 5a10 6500 6a11 4700 6402 6403  d.l.Z.e.j.G.d.d.
-000000a0: 8400 6403 8302 8301 5a12 641f 6405 6406  ..d.....Z.d.d.d.
-000000b0: 8401 5a13 4700 6407 6408 8400 6408 8302  ..Z.G.d.d...d...
-000000c0: 5a14 6409 640a 8400 5a15 0904 090b 090c  Z.d.d...Z.......
-000000d0: 090d 6420 640e 6510 6a16 640f 6517 6410  ..d d.e.j.d.e.d.
-000000e0: 6518 6411 6519 6412 651a 660a 6413 6414  e.d.e.d.e.f.d.d.
-000000f0: 8405 5a1b 0904 0901 090b 090c 090d 6421  ..Z...........d!
-00000100: 640e 6510 6a16 640f 6517 6415 6518 6401  d.e.j.d.e.d.e.d.
-00000110: 4200 6410 6518 6411 6519 6412 651a 660c  B.d.e.d.e.d.e.f.
-00000120: 6416 6417 8405 5a1c 0901 6422 6419 6517  d.d...Z...d"d.e.
-00000130: 641a 6519 641b 6401 6519 4200 641c 6401  d.e.d.d.e.B.d.d.
-00000140: 6519 4200 6608 641d 641e 8405 5a1d 6401  e.B.f.d.d...Z.d.
-00000150: 5300 2923 e900 0000 004e 6300 0000 0000  S.)#.....Nc.....
-00000160: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-00000170: 0000 0073 8a00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00000180: 5500 6401 5a03 6402 5a04 6505 6506 6403  U.d.Z.d.Z.e.e.d.
-00000190: 3c00 6404 5a07 6508 6506 6405 3c00 6406  <.d.Z.e.e.d.<.d.
-000001a0: 5a09 6505 6506 6407 3c00 6408 5a0a 6508  Z.e.e.d.<.d.Z.e.
-000001b0: 6506 6409 3c00 640a 5a0b 6505 6506 640b  e.d.<.d.Z.e.e.d.
-000001c0: 3c00 640c 5a0c 6505 6506 640d 3c00 640e  <.d.Z.e.e.d.<.d.
-000001d0: 5a0d 6505 6506 640f 3c00 640e 5a0e 6505  Z.e.e.d.<.d.Z.e.
-000001e0: 6506 6410 3c00 640e 5a0f 6505 6506 6411  e.d.<.d.Z.e.e.d.
-000001f0: 3c00 6412 5a10 6511 6506 6413 3c00 6414  <.d.Z.e.e.d.<.d.
-00000200: 5300 2915 da20 4879 7065 7250 6172 616d  S.).. HyperParam
-00000210: 6574 6572 7344 6562 6572 7461 436c 6173  etersDebertaClas
-00000220: 7369 6669 6572 7a43 0a20 2020 2048 6f6c  sifierzC.    Hol
-00000230: 6420 6879 7065 7220 7061 7261 6d65 7465  d hyper paramete
-00000240: 7273 2066 6f72 2048 7567 6769 6e67 2046  rs for Hugging F
-00000250: 6163 6520 4465 4245 5254 6120 636c 6173  ace DeBERTa clas
-00000260: 7369 6669 6572 0a20 2020 2067 691d 554d  sifier.    gi.UM
-00000270: 1075 ff3e da0d 6c65 6172 6e69 6e67 5f72  .u.>..learning_r
-00000280: 6174 65e9 2000 0000 da0a 6261 7463 685f  ate. .....batch_
-00000290: 7369 7a65 677b 14ae 47e1 7a84 3fda 0c77  sizeg{..G.z.?..w
-000002a0: 6569 6768 745f 6465 6361 79e9 0100 0000  eight_decay.....
-000002b0: da06 6570 6f63 6873 7201 0000 00da 0c77  ..epochsr......w
-000002c0: 6172 6d75 705f 7261 7469 6fe9 f401 0000  armup_ratio.....
-000002d0: da0c 7761 726d 7570 5f73 7465 7073 679a  ..warmup_stepsg.
-000002e0: 9999 9999 99b9 3fda 1368 6964 6465 6e5f  ......?..hidden_
-000002f0: 6472 6f70 6f75 745f 7072 6f62 da1c 6174  dropout_prob..at
-00000300: 7465 6e74 696f 6e5f 7072 6f62 735f 6472  tention_probs_dr
-00000310: 6f70 6f75 745f 7072 6f62 da0b 636c 735f  opout_prob..cls_
-00000320: 6472 6f70 6f75 74da 066c 696e 6561 72da  dropout..linear.
-00000330: 116c 725f 7363 6865 6475 6c65 725f 7479  .lr_scheduler_ty
-00000340: 7065 4e29 12da 085f 5f6e 616d 655f 5fda  peN)...__name__.
-00000350: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000360: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
-00000370: 5f5f 7203 0000 00da 0566 6c6f 6174 da0f  __r......float..
-00000380: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5f72  __annotations__r
-00000390: 0500 0000 da03 696e 7472 0600 0000 7208  ......intr....r.
-000003a0: 0000 0072 0900 0000 720b 0000 0072 0c00  ...r....r....r..
-000003b0: 0000 720d 0000 0072 0e00 0000 7210 0000  ..r....r....r...
-000003c0: 00da 0373 7472 a900 7219 0000 0072 1900  ...str..r....r..
-000003d0: 0000 fa3e 2f68 6f6d 652f 6b72 6973 7469  ...>/home/kristi
-000003e0: 616e 2f50 726f 6a65 6374 732f 6132 2f73  an/Projects/a2/s
-000003f0: 7263 2f61 322f 7472 6169 6e69 6e67 2f74  rc/a2/training/t
-00000400: 7261 696e 696e 675f 6875 6767 696e 672e  raining_hugging.
-00000410: 7079 7202 0000 0011 0000 0073 1800 0000  pyr........s....
-00000420: 0a00 0402 0c04 0c01 0c01 0c01 0c01 0c01  ................
-00000430: 0c01 0c01 0c01 1001 7202 0000 00da 0772  ........r......r
-00000440: 6169 6e69 6e67 6302 0000 0000 0000 0000  ainingc.........
-00000450: 0000 0009 0000 0008 0000 0043 0000 0073  ...........C...s
-00000460: 8000 0000 7c00 5c02 7d02 7d03 7c02 6a00  ....|.\.}.}.|.j.
-00000470: 6401 6402 8d01 7d02 7401 6a02 6a03 6a04  d.d...}.t.j.j.j.
-00000480: 7c03 7c02 7c01 6403 6404 8d04 7d04 7c04  |.|.|.d.d...}.|.
-00000490: 6405 1900 6406 1900 7d05 7c04 6407 1900  d...d...}.|.d...
-000004a0: 6406 1900 7d06 7c04 6408 7c01 9b00 9d02  d...}.|.d.|.....
-000004b0: 1900 6406 1900 7d07 7c04 7c01 1900 6406  ..d...}.|.|...d.
-000004c0: 1900 7d08 6409 7c01 9b00 9d02 7c07 640a  ..}.d.|.....|.d.
-000004d0: 7c01 9b00 9d02 7c08 640b 7c05 640c 7c06  |.....|.d.|.d.|.
-000004e0: 6904 5300 290d 6127 0100 000a 2020 2020  i.S.).a'....    
-000004f0: 4164 6f70 7420 4875 6767 696e 6720 4661  Adopt Hugging Fa
-00000500: 6365 206d 6574 7269 6320 6f75 7470 7574  ce metric output
-00000510: 2074 6f20 7072 6566 6572 6564 206d 6574   to prefered met
-00000520: 7269 630a 2020 2020 2866 312d 7363 6f72  ric.    (f1-scor
-00000530: 6529 2066 6f72 2074 6869 7320 7072 6f6a  e) for this proj
-00000540: 6563 740a 0a20 2020 2050 6172 616d 6574  ect..    Paramet
-00000550: 6572 733a 0a20 2020 202d 2d2d 2d2d 2d2d  ers:.    -------
-00000560: 2d2d 2d0a 2020 2020 6576 616c 5f70 7265  ---.    eval_pre
-00000570: 643a 2050 7265 6469 6374 696f 6e73 2061  d: Predictions a
-00000580: 6e64 206c 6162 656c 7320 6f66 2048 7567  nd labels of Hug
-00000590: 6769 6e67 2046 6163 6520 6d6f 6465 6c20  ging Face model 
-000005a0: 7768 696c 6520 7472 6169 6e69 6e67 0a20  while training. 
-000005b0: 2020 206c 6162 656c 3a20 4c61 6265 6c20     label: Label 
-000005c0: 6e61 6d65 206f 6620 7468 6520 636c 6173  name of the clas
-000005d0: 7369 6669 6361 7469 6f6e 0a0a 2020 2020  sification..    
-000005e0: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
-000005f0: 2d2d 2d0a 2020 2020 6469 6374 696f 6e61  ---.    dictiona
-00000600: 7279 206f 6620 6d65 7472 6963 730a 2020  ry of metrics.  
-00000610: 2020 e9ff ffff ff29 01da 0461 7869 7354    .....)...axisT
-00000620: 2902 da05 6c61 6265 6cda 0b6f 7574 7075  )...label..outpu
-00000630: 745f 6469 6374 7a0c 7765 6967 6874 6564  t_dictz.weighted
-00000640: 2061 7667 7a08 6631 2d73 636f 7265 7a09   avgz.f1-scorez.
-00000650: 6d61 6372 6f20 6176 677a 046e 6f74 20da  macro avgz.not .
-00000660: 0766 315f 6e6f 745f da03 6631 5fda 1366  .f1_not_..f1_..f
-00000670: 315f 7765 6967 6874 6564 5f61 7665 7261  1_weighted_avera
-00000680: 6765 da10 6631 5f6d 6163 726f 5f61 7665  ge..f1_macro_ave
-00000690: 7261 6765 2905 da06 6172 676d 6178 da02  rage)...argmax..
-000006a0: 6132 da08 706c 6f74 7469 6e67 da08 616e  a2..plotting..an
-000006b0: 616c 7973 6973 da15 636c 6173 7369 6669  alysis..classifi
-000006c0: 6361 7469 6f6e 5f72 6570 6f72 7429 09da  cation_report)..
-000006d0: 0965 7661 6c5f 7072 6564 721e 0000 00da  .eval_predr.....
-000006e0: 0b70 7265 6469 6374 696f 6e73 da06 6c61  .predictions..la
-000006f0: 6265 6c73 7228 0000 0072 2200 0000 7223  belsr(...r"...r#
-00000700: 0000 00da 0666 315f 6e6f 74da 0266 3172  .....f1_not..f1r
-00000710: 1900 0000 7219 0000 0072 1a00 0000 da10  ....r....r......
-00000720: 5f63 6f6d 7075 7465 5f6d 6574 7269 6373  _compute_metrics
-00000730: 2300 0000 7322 0000 0008 0e0c 0108 0102  #...s"..........
-00000740: 0102 0102 0102 0106 fc0c 060c 0112 010c  ................
-00000750: 010a 020a 0104 0104 0104 fc72 2e00 0000  ...........r....
-00000760: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000770: 0025 0000 0040 0000 0073 ee00 0000 6500  .%...@...s....e.
-00000780: 5a01 6400 5a02 6401 5a03 0902 0903 6428  Z.d.Z.d.Z.....d(
-00000790: 6404 6504 6405 6505 6406 6506 6a07 6506  d.e.d.e.d.e.j.e.
-000007a0: 6a08 1900 6606 6407 6408 8405 5a09 6429  j...f.d.d...Z.d)
-000007b0: 640a 6506 6a08 640b 650a 640c 650a 6606  d.e.j.d.e.d.e.f.
-000007c0: 640d 640e 8405 5a0b 6403 6403 640f 6410  d.d...Z.d.d.d.d.
-000007d0: 6409 6410 6409 6410 6403 6409 650c 6a0d  d.d.d.d.d.d.e.j.
-000007e0: 6411 6411 6412 6413 6414 6409 6415 6612  d.d.d.d.d.d.d.f.
-000007f0: 6416 6506 6a0e 650f 6a10 650f 6a11 6602  d.e.j.e.j.e.j.f.
-00000800: 1900 6417 6512 6403 4200 6418 6506 6a07  ..d.e.d.B.d.e.j.
-00000810: 650c 6a13 1900 6403 4200 6419 6504 641a  e.j...d.B.d.e.d.
-00000820: 650a 641b 650a 641c 650a 640b 650a 641d  e.d.e.d.e.d.e.d.
-00000830: 650a 641e 6514 6403 4200 640c 650a 641f  e.d.e.d.B.d.e.d.
-00000840: 6505 6420 6505 6421 6504 6422 6505 6403  e.d e.d!e.d"e.d.
-00000850: 4200 6423 6504 6424 650a 6425 6504 6624  B.d#e.d$e.d%e.f$
-00000860: 6426 6427 8405 5a15 6403 5300 292a da17  d&d'..Z.d.S.)*..
-00000870: 4875 6767 696e 6746 6163 6554 7261 696e  HuggingFaceTrain
-00000880: 6572 436c 6173 737a 2b0a 2020 2020 5573  erClassz+.    Us
-00000890: 6564 2074 6f20 7472 6169 6e20 4875 6767  ed to train Hugg
-000008a0: 696e 6720 4661 6365 206d 6f64 656c 730a  ing Face models.
-000008b0: 2020 2020 e902 0000 004e da0c 6d6f 6465      .....N..mode
-000008c0: 6c5f 666f 6c64 6572 da0a 6e75 6d5f 6c61  l_folder..num_la
-000008d0: 6265 6c73 da06 636f 6e66 6967 6304 0000  bels..configc...
-000008e0: 0000 0000 0000 0000 0004 0000 0004 0000  ................
-000008f0: 0043 0000 0073 3a00 0000 7c01 7c00 5f00  .C...s:...|.|._.
-00000900: 7c02 7c00 5f01 7c03 6400 7500 7214 7402  |.|._.|.d.u.r.t.
-00000910: 6a03 6a04 7c01 7c02 6401 8d02 7c00 5f05  j.j.|.|.d...|._.
-00000920: 6e03 7c03 7c00 5f05 7406 8300 7c00 5f07  n.|.|._.t...|._.
-00000930: 6400 5300 2902 4e29 0172 3200 0000 2908  d.S.).N).r2...).
-00000940: 7231 0000 0072 3200 0000 da0c 7472 616e  r1...r2.....tran
-00000950: 7366 6f72 6d65 7273 da0a 4175 746f 436f  sformers..AutoCo
-00000960: 6e66 6967 da0f 6672 6f6d 5f70 7265 7472  nfig..from_pretr
-00000970: 6169 6e65 64da 0e64 625f 636f 6e66 6967  ained..db_config
-00000980: 5f62 6173 6572 0200 0000 da10 6879 7065  _baser......hype
-00000990: 725f 7061 7261 6d65 7465 7273 2904 da04  r_parameters)...
-000009a0: 7365 6c66 7231 0000 0072 3200 0000 7233  selfr1...r2...r3
-000009b0: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-000009c0: 0000 da08 5f5f 696e 6974 5f5f 4a00 0000  ....__init__J...
-000009d0: 730c 0000 0006 0606 0108 0114 0106 020c  s...............
-000009e0: 017a 2048 7567 6769 6e67 4661 6365 5472  .z HuggingFaceTr
-000009f0: 6169 6e65 7243 6c61 7373 2e5f 5f69 6e69  ainerClass.__ini
-00000a00: 745f 5f54 da06 7061 7261 6d73 da06 6d61  t__T..params..ma
-00000a10: 6e74 696b da14 6261 7365 5f6d 6f64 656c  ntik..base_model
-00000a20: 5f74 7261 696e 6162 6c65 6304 0000 0000  _trainablec.....
-00000a30: 0000 0000 0000 0007 0000 0005 0000 0043  ...............C
-00000a40: 0000 0073 7000 0000 7c00 6a00 7d04 7c01  ...sp...|.j.}.|.
-00000a50: 6400 7501 7210 7c04 a001 6401 7c01 6401  d.u.r.|...d.|.d.
-00000a60: 1900 6901 a101 0100 7c04 a001 6402 7c00  ..i.....|...d.|.
-00000a70: 6a02 6901 a101 0100 7403 6a04 6a05 7c00  j.i.....t.j.j.|.
-00000a80: 6a06 7c04 6403 8d02 7d05 7c03 732e 7c05  j.|.d...}.|.s.|.
-00000a90: 6a07 a008 a100 4400 5d05 7d06 6404 7c06  j.....D.].}.d.|.
-00000aa0: 5f09 7128 7c02 7236 740a 6a0b 6a0c a00d  _.q(|.r6t.j.j...
-00000ab0: a100 0100 7c05 5300 2905 4e72 0e00 0000  ....|.S.).Nr....
-00000ac0: 7232 0000 0029 0172 3300 0000 4629 0e72  r2...).r3...F).r
-00000ad0: 3700 0000 da06 7570 6461 7465 7232 0000  7.....updater2..
-00000ae0: 0072 3400 0000 da22 4175 746f 4d6f 6465  .r4...."AutoMode
-00000af0: 6c46 6f72 5365 7175 656e 6365 436c 6173  lForSequenceClas
-00000b00: 7369 6669 6361 7469 6f6e 7236 0000 0072  sificationr6...r
-00000b10: 3100 0000 da0a 6261 7365 5f6d 6f64 656c  1.....base_model
-00000b20: da0a 7061 7261 6d65 7465 7273 da0d 7265  ..parameters..re
-00000b30: 7175 6972 6573 5f67 7261 6472 2500 0000  quires_gradr%...
-00000b40: da08 7472 6169 6e69 6e67 da08 7472 6163  ..training..trac
-00000b50: 6b69 6e67 da11 696e 6974 6961 6c69 7a65  king..initialize
-00000b60: 5f6d 616e 7469 6b29 0772 3900 0000 723b  _mantik).r9...r;
-00000b70: 0000 0072 3c00 0000 723d 0000 00da 0964  ...r<...r=.....d
-00000b80: 625f 636f 6e66 6967 da05 6d6f 6465 6cda  b_config..model.
-00000b90: 0570 6172 616d 7219 0000 0072 1900 0000  .paramr....r....
-00000ba0: 721a 0000 00da 0967 6574 5f6d 6f64 656c  r......get_model
-00000bb0: 5800 0000 7316 0000 0006 0108 0112 0110  X...s...........
-00000bc0: 0112 0104 010e 0108 0104 010c 0104 017a  ...............z
-00000bd0: 2148 7567 6769 6e67 4661 6365 5472 6169  !HuggingFaceTrai
-00000be0: 6e65 7243 6c61 7373 2e67 6574 5f6d 6f64  nerClass.get_mod
-00000bf0: 656c 7a07 6f75 7470 7574 2f46 720a 0000  elz.output/Fr...
-00000c00: 00da 0573 7465 7073 e964 0000 00da 0565  ...steps.d.....e
-00000c10: 706f 6368 721b 0000 00da 0764 6174 6173  pochr......datas
-00000c20: 6574 7238 0000 00da 0974 6f6b 656e 697a  etr8.....tokeniz
-00000c30: 6572 da0d 666f 6c64 6572 5f6f 7574 7075  er..folder_outpu
-00000c40: 74da 0c68 7970 6572 5f74 756e 696e 67da  t..hyper_tuning.
-00000c50: 0466 7031 36da 0865 7661 6c75 6174 65da  .fp16..evaluate.
-00000c60: 0c64 6973 6162 6c65 5f74 7164 6dda 0963  .disable_tqdm..c
-00000c70: 616c 6c62 6163 6b73 da0d 6c6f 6767 696e  allbacks..loggin
-00000c80: 675f 7374 6570 73da 0a73 6176 655f 7374  g_steps..save_st
-00000c90: 6570 73da 1365 7661 6c75 6174 696f 6e5f  eps..evaluation_
-00000ca0: 7374 7261 7465 6779 da0a 6576 616c 5f73  strategy..eval_s
-00000cb0: 7465 7073 da0d 7361 7665 5f73 7472 6174  teps..save_strat
-00000cc0: 6567 79da 166c 6f61 645f 6265 7374 5f6d  egy..load_best_m
-00000cd0: 6f64 656c 5f61 745f 656e 6472 1e00 0000  odel_at_endr....
-00000ce0: 6314 0000 0000 0000 0000 0000 0019 0000  c...............
-00000cf0: 0009 0000 0043 0000 0073 7801 0000 7400  .....C...sx...t.
-00000d00: 6a01 6a02 a003 a100 7308 6401 7d06 7c02  j.j.....s.d.}.|.
-00000d10: 6402 7500 720f 7404 8300 7d02 7c02 7c00  d.u.r.t...}.|.|.
-00000d20: 5f05 7c03 6402 7500 721d 7406 6a07 a008  _.|.d.u.r.t.j...
-00000d30: 7c00 6a09 a101 7d03 7c12 723f 7c11 7c0f  |.j...}.|.r?|.|.
-00000d40: 6b03 723f 740a a00b 6403 7c11 9b02 6404  k.r?t...d.|...d.
-00000d50: 7c0f 9b02 6405 7c12 9b02 6406 9d07 a101  |...d.|...d.....
-00000d60: 0100 7c0f 7d11 740c 7c0f 7c10 7c0d 7c0e  ..|.}.t.|.|.|.|.
-00000d70: 6407 8d04 5c03 7d10 7d0e 7d0d 7c05 7384  d...\.}.}.}.|.s.
-00000d80: 7406 6a0d 7c04 6601 6900 6408 7c02 6a0e  t.j.|.f.i.d.|.j.
-00000d90: 9301 6409 7c02 6a0f 9301 640a 7c02 6a10  ..d.|.j...d.|.j.
-00000da0: 9301 640b 7c02 6a11 9301 640c 7c09 9301  ..d.|.j...d.|...
-00000db0: 640d 7c06 9301 640e 7c0f 9301 640f 7c02  d.|...d.|...d.|.
-00000dc0: 6a12 9301 6410 7c02 6a12 9301 6411 7c02  j...d.|.j...d.|.
-00000dd0: 6a13 9301 6412 7c02 6a14 9301 6413 6402  j...d.|.j...d.d.
-00000de0: 9301 6414 7c10 9301 6415 7c0e 9301 6416  ..d.|...d.|...d.
-00000df0: 7c11 9301 6417 7c0d 9301 6418 7c12 9301  |...d.|...d.|...
-00000e00: 8e01 7d14 6e0c 7406 6a0d 7c04 6419 7c06  ..}.n.t.j.|.d.|.
-00000e10: 7c0f 6402 7c11 7c12 641a 8d07 7d14 7415  |.d.|.|.d...}.t.
-00000e20: 6a16 7c00 6a17 7c08 7c0b 641b 8d03 7d15  j.|.j.|.|.d...}.
-00000e30: 7415 6a16 7418 7c13 641c 8d02 7d16 7c07  t.j.t.|.d...}.|.
-00000e40: 72ab 7c0c 7c15 7c14 7c03 7c16 7c0a 641d  r.|.|.|.|.|.|.d.
-00000e50: 8d05 5300 7419 7c01 8301 5c02 7d17 7d18  ..S.t.|...\.}.}.
-00000e60: 7c0c 7c15 7c14 7c17 7c18 7c03 7c16 7c0a  |.|.|.|.|.|.|.|.
-00000e70: 641e 8d07 5300 291f 617f 0500 000a 2020  d...S.).a.....  
-00000e80: 2020 2020 2020 5265 7475 726e 7320 4875        Returns Hu
-00000e90: 6767 696e 6720 4661 6365 2074 7261 696e  gging Face train
-00000ea0: 6572 206f 626a 6563 740a 0a20 2020 2020  er object..     
-00000eb0: 2020 2050 6172 616d 6574 6572 733a 0a20     Parameters:. 
-00000ec0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-00000ed0: 2d0a 2020 2020 2020 2020 6461 7461 7365  -.        datase
-00000ee0: 743a 2044 6174 6173 6574 2069 6e20 4875  t: Dataset in Hu
-00000ef0: 6767 696e 6720 4661 6365 2066 6f72 6d61  gging Face forma
-00000f00: 740a 2020 2020 2020 2020 6879 7065 725f  t.        hyper_
-00000f10: 7061 7261 6d65 7465 7273 3a20 6879 7065  parameters: hype
-00000f20: 7220 7061 7261 6d65 7465 7273 2069 6e20  r parameters in 
-00000f30: 7468 6520 666f 726d 206f 6620 6461 7461  the form of data
-00000f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000f50: 2020 2020 2020 2020 2020 2063 6c61 7373             class
-00000f60: 2060 4879 7065 7250 6172 616d 6574 6572   `HyperParameter
-00000f70: 7344 6562 6572 7461 436c 6173 7369 6669  sDebertaClassifi
-00000f80: 6572 600a 2020 2020 2020 2020 746f 6b65  er`.        toke
-00000f90: 6e69 7a65 723a 2048 7567 6769 6e67 2046  nizer: Hugging F
-00000fa0: 6163 6520 746f 6b65 6e69 7a65 720a 2020  ace tokenizer.  
-00000fb0: 2020 2020 2020 666f 6c64 6572 5f6f 7574        folder_out
-00000fc0: 7075 743a 2046 6f6c 6465 7220 746f 2073  put: Folder to s
-00000fd0: 6176 6520 7472 6169 6e69 6e67 206f 7574  ave training out
-00000fe0: 7075 7473 0a20 2020 2020 2020 2068 7970  puts.        hyp
-00000ff0: 6572 5f74 756e 696e 673a 2057 6865 7468  er_tuning: Wheth
-00001000: 6572 2074 7261 696e 6572 2075 7365 6420  er trainer used 
-00001010: 666f 7220 6879 7065 7220 7475 6e69 6e67  for hyper tuning
-00001020: 0a20 2020 2020 2020 2066 7031 363a 2057  .        fp16: W
-00001030: 6865 7468 6572 2074 6f20 7573 6520 6670  hether to use fp
-00001040: 3136 2031 362d 6269 7420 286d 6978 6564  16 16-bit (mixed
-00001050: 2920 7072 6563 6973 696f 6e20 7472 6169  ) precision trai
-00001060: 6e69 6e67 0a20 2020 2020 2020 2020 2020  ning.           
-00001070: 2020 2069 6e73 7465 6164 206f 6620 3332     instead of 32
-00001080: 2d62 6974 2074 7261 696e 696e 672e 0a20  -bit training.. 
-00001090: 2020 2020 2020 2065 7661 6c75 6174 653a         evaluate:
-000010a0: 2057 6865 7468 6572 2074 7261 696e 6572   Whether trainer
-000010b0: 206f 6e6c 7920 7573 6564 2066 6f72 2065   only used for e
-000010c0: 7661 6c75 6174 696f 6e0a 2020 2020 2020  valuation.      
-000010d0: 2020 6d61 6e74 696b 3a20 5768 6574 6865    mantik: Whethe
-000010e0: 7220 7573 696e 6720 6d61 6e74 696b 2066  r using mantik f
-000010f0: 6f72 2074 7261 636b 696e 670a 2020 2020  or tracking.    
-00001100: 2020 2020 6469 7361 626c 655f 7471 646d      disable_tqdm
-00001110: 3a20 5768 6574 6865 7220 746f 2064 6973  : Whether to dis
-00001120: 6162 6c65 2070 726f 6772 6573 7320 6261  able progress ba
-00001130: 7220 7573 6564 2062 7920 6054 7261 6e73  r used by `Trans
-00001140: 666f 726d 6572 600a 2020 2020 2020 2020  former`.        
-00001150: 6361 6c6c 6261 636b 733a 2043 616c 6c62  callbacks: Callb
-00001160: 6163 6b73 2064 7572 696e 6720 7472 6169  acks during trai
-00001170: 6e69 6e67 0a20 2020 2020 2020 2062 6173  ning.        bas
-00001180: 655f 6d6f 6465 6c5f 7472 6169 6e61 626c  e_model_trainabl
-00001190: 653a 2057 6865 7468 6572 2062 6173 6520  e: Whether base 
-000011a0: 6d6f 6465 6c20 7765 6967 6874 7320 6172  model weights ar
-000011b0: 6520 7472 6169 6e61 626c 6520 286e 6f74  e trainable (not
-000011c0: 2066 6978 6564 290a 2020 2020 2020 2020   fixed).        
-000011d0: 7472 6169 6e65 725f 636c 6173 733a 2054  trainer_class: T
-000011e0: 7261 696e 6572 2063 6c61 7373 2063 6f6d  rainer class com
-000011f0: 7061 7469 626c 6520 7769 7468 2060 7472  patible with `tr
-00001200: 616e 7366 6f72 6d65 722e 5472 6169 6e65  ansformer.Traine
-00001210: 7260 0a20 2020 2020 2020 206c 6f67 6769  r`.        loggi
-00001220: 6e67 5f73 7465 7073 3a20 4e75 6d62 6572  ng_steps: Number
-00001230: 206f 6620 7374 6570 7320 6265 666f 7265   of steps before
-00001240: 2068 7567 6769 6e67 2066 6163 6520 7072   hugging face pr
-00001250: 696e 7473 0a20 2020 2020 2020 2065 7661  ints.        eva
-00001260: 6c75 6174 696f 6e5f 7374 7261 7465 6779  luation_strategy
-00001270: 3a20 5768 656e 2074 6f20 6576 616c 7561  : When to evalua
-00001280: 7465 2c20 6166 7465 7220 2273 7465 7073  te, after "steps
-00001290: 2220 6f72 2022 6570 6f63 6822 0a20 2020  " or "epoch".   
-000012a0: 2020 2020 2065 7661 6c5f 7374 6570 733a       eval_steps:
-000012b0: 204e 756d 6265 7220 6f66 2073 7465 7073   Number of steps
-000012c0: 2062 6574 7765 656e 2065 7661 6c75 6174   between evaluat
-000012d0: 696f 6e20 286f 6e6c 7920 7573 6564 2069  ion (only used i
-000012e0: 6620 6065 7661 6c75 6174 696f 6e5f 7374  f `evaluation_st
-000012f0: 7261 7465 6779 603d 2273 7465 7073 2229  rategy`="steps")
-00001300: 0a20 2020 2020 2020 2073 6176 655f 7374  .        save_st
-00001310: 7261 7465 6779 3a20 5768 656e 2074 6f20  rategy: When to 
-00001320: 7361 7665 2062 6573 7420 6d6f 6465 6c20  save best model 
-00001330: 2273 7465 7073 2220 6f72 2022 6570 6f63  "steps" or "epoc
-00001340: 6822 0a20 2020 2020 2020 206c 6f61 645f  h".        load_
-00001350: 6265 7374 5f6d 6f64 656c 5f61 745f 656e  best_model_at_en
-00001360: 643a 204c 6f61 6420 6265 7374 206d 6f64  d: Load best mod
-00001370: 656c 2061 7420 656e 6420 6f66 2074 7261  el at end of tra
-00001380: 696e 696e 670a 2020 2020 2020 2020 6c61  ining.        la
-00001390: 6265 6c3a 204c 6162 656c 206e 616d 6520  bel: Label name 
-000013a0: 6f66 2074 6865 2063 6c61 7373 6966 6963  of the classific
-000013b0: 6174 696f 6e0a 0a20 2020 2020 2020 2052  ation..        R
-000013c0: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-000013d0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2048  ------.        H
-000013e0: 7567 6769 6e67 2046 6163 6520 5472 6169  ugging Face Trai
-000013f0: 6e65 720a 2020 2020 2020 2020 464e 7a16  ner.        FNz.
-00001400: 5365 7474 696e 6720 7361 7665 5f73 7472  Setting save_str
-00001410: 6174 6567 793d 7a1e 2065 7175 616c 2074  ategy=z. equal t
-00001420: 6f20 6576 616c 7561 7469 6f6e 5f73 7472  o evaluation_str
-00001430: 6174 6567 793d 7a27 2028 7265 7175 6972  ategy=z' (requir
-00001440: 6564 2077 6865 6e20 6c6f 6164 5f62 6573  ed when load_bes
-00001450: 745f 6d6f 6465 6c5f 6174 5f65 6e64 3d7a  t_model_at_end=z
-00001460: 0820 3d20 5472 7565 29a9 0472 5700 0000  . = True)..rW...
-00001470: 7258 0000 0072 5500 0000 7256 0000 0072  rX...rU...rV...r
-00001480: 0300 0000 7209 0000 0072 0b00 0000 7210  ....r....r....r.
-00001490: 0000 0072 5300 0000 7251 0000 0072 5700  ...rS...rQ...rW.
-000014a0: 0000 da1b 7065 725f 6465 7669 6365 5f74  ....per_device_t
-000014b0: 7261 696e 5f62 6174 6368 5f73 697a 65da  rain_batch_size.
-000014c0: 1a70 6572 5f64 6576 6963 655f 6576 616c  .per_device_eval
-000014d0: 5f62 6174 6368 5f73 697a 65da 106e 756d  _batch_size..num
-000014e0: 5f74 7261 696e 5f65 706f 6368 7372 0600  _train_epochsr..
-000014f0: 0000 da09 7265 706f 7274 5f74 6f72 5800  ....report_torX.
-00001500: 0000 7256 0000 0072 5900 0000 7255 0000  ..rV...rY...rU..
-00001510: 0072 5a00 0000 5429 0672 5300 0000 7251  .rZ...T).rS...rQ
-00001520: 0000 0072 5700 0000 725f 0000 0072 5900  ...rW...r_...rY.
-00001530: 0000 725a 0000 0029 0272 3c00 0000 723d  ..rZ...).r<...r=
-00001540: 0000 0029 0172 1e00 0000 2905 da0a 6d6f  ...).r....)...mo
-00001550: 6465 6c5f 696e 6974 da04 6172 6773 724e  del_init..argsrN
-00001560: 0000 00da 0f63 6f6d 7075 7465 5f6d 6574  .....compute_met
-00001570: 7269 6373 7254 0000 0029 0772 6000 0000  ricsrT...).r`...
-00001580: 7261 0000 00da 0d74 7261 696e 5f64 6174  ra.....train_dat
-00001590: 6173 6574 da0c 6576 616c 5f64 6174 6173  aset..eval_datas
-000015a0: 6574 724e 0000 0072 6200 0000 7254 0000  etrN...rb...rT..
-000015b0: 0029 1a72 2500 0000 7243 0000 00da 0e75  .).r%...rC.....u
-000015c0: 7469 6c73 5f74 7261 696e 696e 67da 0d67  tils_training..g
-000015d0: 7075 5f61 7661 696c 6162 6c65 7202 0000  pu_availabler...
-000015e0: 0072 3800 0000 7234 0000 00da 0d41 7574  .r8...r4.....Aut
-000015f0: 6f54 6f6b 656e 697a 6572 7236 0000 0072  oTokenizerr6...r
-00001600: 3100 0000 da07 6c6f 6767 696e 67da 0469  1.....logging..i
-00001610: 6e66 6fda 2173 6574 5f65 7661 6c75 6174  nfo.!set_evaluat
-00001620: 696f 6e5f 7361 7665 5f6c 6f67 6769 6e67  ion_save_logging
-00001630: 5f73 7465 7073 da11 5472 6169 6e69 6e67  _steps..Training
-00001640: 4172 6775 6d65 6e74 7372 0300 0000 7209  Argumentsr....r.
-00001650: 0000 0072 0b00 0000 7210 0000 0072 0500  ...r....r....r..
-00001660: 0000 7208 0000 0072 0600 0000 da09 6675  ..r....r......fu
-00001670: 6e63 746f 6f6c 73da 0770 6172 7469 616c  nctools..partial
-00001680: 7249 0000 0072 2e00 0000 da21 5f67 6574  rI...r.....!_get
-00001690: 5f74 7261 696e 696e 675f 6576 616c 7561  _training_evalua
-000016a0: 7469 6f6e 5f64 6174 6173 6574 7329 1972  tion_datasets).r
-000016b0: 3900 0000 724d 0000 0072 3800 0000 724e  9...rM...r8...rN
-000016c0: 0000 0072 4f00 0000 7250 0000 0072 5100  ...rO...rP...rQ.
-000016d0: 0000 7252 0000 0072 3c00 0000 7253 0000  ..rR...r<...rS..
-000016e0: 0072 5400 0000 723d 0000 00da 0d74 7261  .rT...r=.....tra
-000016f0: 696e 6572 5f63 6c61 7373 7255 0000 0072  iner_classrU...r
-00001700: 5600 0000 7257 0000 0072 5800 0000 7259  V...rW...rX...rY
-00001710: 0000 0072 5a00 0000 721e 0000 0072 6100  ...rZ...r....ra.
-00001720: 0000 7260 0000 00da 185f 7061 7274 6961  ..r`....._partia
-00001730: 6c5f 636f 6d70 7574 655f 6d65 7472 6963  l_compute_metric
-00001740: 7372 6300 0000 7264 0000 0072 1900 0000  src...rd...r....
-00001750: 7219 0000 0072 1a00 0000 da0b 6765 745f  r....r......get_
-00001760: 7472 6169 6e65 7265 0000 0073 ae00 0000  trainere...s....
-00001770: 0c34 0401 0801 0601 0601 0801 0e01 0c01  .4..............
-00001780: 0401 0e01 0201 06ff 04ff 0404 0201 0201  ................
-00001790: 0201 0201 0201 0cfc 0406 0401 0201 06ff  ................
-000017a0: 0602 02fe 0603 02fd 0604 02fc 0605 02fb  ................
-000017b0: 0406 02fa 0407 02f9 0408 02f8 0609 02f7  ................
-000017c0: 060a 02f6 060b 02f5 060c 02f4 040d 02f3  ................
-000017d0: 040e 02f2 040f 02f1 0410 02f0 0411 02ef  ................
-000017e0: 0412 06ee 0415 0201 0201 0201 0201 0201  ................
-000017f0: 0201 0201 06f9 1209 0e01 0401 0201 0201  ................
-00001800: 0201 0201 0201 0201 06fb 0c07 0201 0201  ................
-00001810: 0201 0201 0201 0201 0201 0201 06f9 7a23  ..............z#
-00001820: 4875 6767 696e 6746 6163 6554 7261 696e  HuggingFaceTrain
-00001830: 6572 436c 6173 732e 6765 745f 7472 6169  erClass.get_trai
-00001840: 6e65 7229 0272 3000 0000 4e29 0254 5429  ner).r0...N).TT)
-00001850: 1672 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
-00001860: 7214 0000 0072 1800 0000 7217 0000 00da  r....r....r.....
-00001870: 0174 da08 4f70 7469 6f6e 616c da04 4469  .t..Optional..Di
-00001880: 6374 723a 0000 00da 0462 6f6f 6c72 4900  ctr:.....boolrI.
-00001890: 0000 7234 0000 00da 0754 7261 696e 6572  ..r4.....Trainer
-000018a0: da05 556e 696f 6eda 0864 6174 6173 6574  ..Union..dataset
-000018b0: 73da 0744 6174 6173 6574 da0b 4461 7461  s..Dataset..Data
-000018c0: 7365 7444 6963 7472 0200 0000 da10 4465  setDictr......De
-000018d0: 6265 7274 6154 6f6b 656e 697a 6572 da04  bertaTokenizer..
-000018e0: 6c69 7374 7271 0000 0072 1900 0000 7219  listrq...r....r.
-000018f0: 0000 0072 1900 0000 721a 0000 0072 2f00  ...r....r....r/.
-00001900: 0000 4500 0000 7386 0000 0008 0004 0102  ..E...s.........
-00001910: 0702 0104 fc02 0202 fe02 0302 fd0a 040a  ................
-00001920: fc1a 0e02 1002 0102 0102 0102 0102 0102  ................
-00001930: 0102 0102 0102 0104 0102 0102 0102 0102  ................
-00001940: 0102 0102 0102 0104 ec10 0202 fe06 0302  ................
-00001950: fd0e 0402 fc02 0502 fb02 0602 fa02 0702  ................
-00001960: f902 0802 f802 0902 f702 0a02 f606 0b02  ................
-00001970: f502 0c02 f402 0e02 f202 0f02 f102 1002  ................
-00001980: f006 1102 ef02 1202 ee02 1302 ed02 140e  ................
-00001990: ec72 2f00 0000 6301 0000 0000 0000 0000  .r/...c.........
-000019a0: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
-000019b0: 6200 0000 7400 7c00 7401 6a02 8302 7212  b...t.|.t.j...r.
-000019c0: 7c00 6401 1900 7d01 7c00 6402 1900 7d02  |.d...}.|.d...}.
-000019d0: 7c01 7c02 6602 5300 7400 7c00 7403 8302  |.|.f.S.t.|.t...
-000019e0: 7229 7404 7c00 8301 6403 6b02 7229 7c00  r)t.|...d.k.r)|.
-000019f0: 6404 1900 7d01 7c00 6405 1900 7d02 7c01  d...}.|.d...}.|.
-00001a00: 7c02 6602 5300 7405 6406 7c00 9b02 6407  |.f.S.t.d.|...d.
-00001a10: 9d03 8301 8201 2908 4eda 0574 7261 696e  ......).N..train
-00001a20: da04 7465 7374 7230 0000 0072 0100 0000  ..testr0...r....
-00001a30: 7207 0000 007a 1743 6f75 6c64 6e27 7420  r....z.Couldn't 
-00001a40: 7061 7273 6520 6461 7461 7365 743d fa01  parse dataset=..
-00001a50: 2129 06da 0a69 7369 6e73 7461 6e63 6572  !)...isinstancer
-00001a60: 7800 0000 727a 0000 00da 0574 7570 6c65  x...rz.....tuple
-00001a70: da03 6c65 6eda 0954 7970 6545 7272 6f72  ..len..TypeError
-00001a80: 2903 724d 0000 0072 6300 0000 7264 0000  ).rM...rc...rd..
-00001a90: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00001aa0: 726e 0000 00e1 0000 0073 1200 0000 0c01  rn.......s......
-00001ab0: 0801 0801 0806 16fb 0801 0801 0803 10ff  ................
-00001ac0: 726e 0000 00e7 9a99 9999 9999 c93f e92a  rn...........?.*
-00001ad0: 0000 0054 da02 6473 da0c 6b65 795f 7374  ...T..ds..key_st
-00001ae0: 7261 7469 6679 da09 7465 7374 5f73 697a  ratify..test_siz
-00001af0: 65da 0c72 616e 646f 6d5f 7374 6174 65da  e..random_state.
-00001b00: 0773 6875 6666 6c65 6305 0000 0000 0000  .shufflec.......
-00001b10: 0000 0000 0008 0000 0007 0000 0043 0000  .............C..
-00001b20: 0073 5400 0000 7c01 6401 7501 720a 7c00  .sT...|.d.u.r.|.
-00001b30: 7c01 1900 6a00 7d05 6e02 6401 7d05 7401  |...j.}.n.d.}.t.
-00001b40: 6a02 6a03 7404 a005 7c00 7406 6a07 6a08  j.j.t...|.t.j.j.
-00001b50: a009 7c00 a101 1900 6a0a 6402 1900 a101  ..|.....j.d.....
-00001b60: 7c02 7c03 7c04 7c05 6403 8d05 5c02 7d06  |.|.|.|.d...\.}.
-00001b70: 7d07 7c06 7c07 6602 5300 2904 e150 0200  }.|.|.f.S.)..P..
-00001b80: 000a 2020 2020 5265 7475 726e 7320 696e  ..    Returns in
-00001b90: 6469 6365 7320 6f66 2074 7261 696e 696e  dices of trainin
-00001ba0: 6720 616e 6420 7661 6c69 6461 7469 6f6e  g and validation
-00001bb0: 2073 6574 0a0a 2020 2020 5061 7261 6d65   set..    Parame
-00001bc0: 7465 7273 3a0a 2020 2020 2d2d 2d2d 2d2d  ters:.    ------
-00001bd0: 2d2d 2d2d 0a20 2020 2064 733a 2058 6172  ----.    ds: Xar
-00001be0: 7261 7920 6461 7461 7365 740a 2020 2020  ray dataset.    
-00001bf0: 6b65 795f 7374 7261 7469 6679 3a20 5374  key_stratify: St
-00001c00: 7261 7469 6669 6564 2062 6173 6564 206f  ratified based o
-00001c10: 6e20 7468 6973 206b 6579 2c20 604e 6f6e  n this key, `Non
-00001c20: 6560 2069 6620 6e6f 7420 7265 7175 6972  e` if not requir
-00001c30: 6564 0a20 2020 2076 616c 6964 6174 696f  ed.    validatio
-00001c40: 6e5f 7369 7a65 3a20 4672 6163 7469 6f6e  n_size: Fraction
-00001c50: 206f 6620 7661 6c69 6461 7469 6f6e 2073   of validation s
-00001c60: 6574 3b20 3120 2d20 7661 6c69 6461 7469  et; 1 - validati
-00001c70: 6f6e 5f73 697a 6520 2d20 7465 7374 5f73  on_size - test_s
-00001c80: 697a 6520 3e20 300a 2020 2020 7465 7374  ize > 0.    test
-00001c90: 5f73 697a 653a 2046 7261 6374 696f 6e20  _size: Fraction 
-00001ca0: 6f66 2074 6573 7420 7365 743b 2031 202d  of test set; 1 -
-00001cb0: 2076 616c 6964 6174 696f 6e5f 7369 7a65   validation_size
-00001cc0: 202d 2074 6573 745f 7369 7a65 203e 2030   - test_size > 0
-00001cd0: 0a20 2020 2072 616e 646f 6d5f 7374 6174  .    random_stat
-00001ce0: 653a 2052 616e 646f 6d20 7365 6564 2074  e: Random seed t
-00001cf0: 6f20 696e 6974 6961 6c69 7a65 2073 656c  o initialize sel
-00001d00: 6563 7469 6f6e 0a20 2020 2073 6875 6666  ection.    shuff
-00001d10: 6c65 3a20 5768 6574 6865 7220 6f72 206e  le: Whether or n
-00001d20: 6f74 2074 6f20 7368 7566 666c 6520 7468  ot to shuffle th
-00001d30: 6520 6461 7461 2062 6566 6f72 6520 7370  e data before sp
-00001d40: 6c69 7474 696e 672e 0a20 2020 2020 2020  litting..       
-00001d50: 2020 2020 2020 4966 2073 6875 6666 6c65        If shuffle
-00001d60: 3d46 616c 7365 2074 6865 6e20 7374 7261  =False then stra
-00001d70: 7469 6679 206d 7573 7420 6265 204e 6f6e  tify must be Non
-00001d80: 652e 0a0a 2020 2020 5265 7475 726e 730a  e...    Returns.
-00001d90: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00001da0: 496e 6469 6365 7320 6f66 2074 7261 696e  Indices of train
-00001db0: 696e 672c 2076 616c 6964 6174 696f 6e20  ing, validation 
-00001dc0: 616e 6420 7465 7374 2073 6574 0a20 2020  and test set.   
-00001dd0: 204e 7201 0000 0029 0472 8800 0000 7289   Nr....).r....r.
-00001de0: 0000 0072 8a00 0000 da08 7374 7261 7469  ...r......strati
-00001df0: 6679 290b da06 7661 6c75 6573 da07 736b  fy)...values..sk
-00001e00: 6c65 6172 6eda 0f6d 6f64 656c 5f73 656c  learn..model_sel
-00001e10: 6563 7469 6f6e da10 7472 6169 6e5f 7465  ection..train_te
-00001e20: 7374 5f73 706c 6974 da02 6e70 da06 6172  st_split..np..ar
-00001e30: 616e 6765 7225 0000 0072 4d00 0000 da0d  anger%...rM.....
-00001e40: 7574 696c 735f 6461 7461 7365 74da 1767  utils_dataset..g
-00001e50: 6574 5f76 6172 6961 626c 655f 6e61 6d65  et_variable_name
-00001e60: 5f66 6972 7374 da05 7368 6170 6529 0872  _first..shape).r
-00001e70: 8600 0000 7287 0000 0072 8800 0000 7289  ....r....r....r.
-00001e80: 0000 0072 8a00 0000 728c 0000 00da 0d69  ...r....r......i
-00001e90: 6e64 6963 6573 5f74 7261 696e da0c 696e  ndices_train..in
-00001ea0: 6469 6365 735f 7465 7374 7219 0000 0072  dices_testr....r
-00001eb0: 1900 0000 721a 0000 00da 1273 706c 6974  ....r......split
-00001ec0: 5f74 7261 696e 696e 675f 7365 74ed 0000  _training_set...
-00001ed0: 0073 1600 0000 0818 0c01 0402 0601 1c01  .s..............
-00001ee0: 0201 0201 0201 0201 0afb 0807 7298 0000  ............r...
-00001ef0: 00da 0f76 616c 6964 6174 696f 6e5f 7369  ...validation_si
-00001f00: 7a65 6306 0000 0000 0000 0000 0000 000a  zec.............
-00001f10: 0000 0008 0000 0043 0000 0073 aa00 0000  .......C...s....
-00001f20: 7400 6a01 6a02 a003 7c00 a004 a100 a101  t.j.j...|.......
-00001f30: 7d00 6401 7c03 1800 7d06 7c02 6402 7501  }.d.|...}.|.d.u.
-00001f40: 7215 7c06 7c02 3800 7d06 7c06 6403 6b00  r.|.|.8.}.|.d.k.
-00001f50: 7227 7405 6404 7c06 9b02 6405 7c02 9b02  r't.d.|...d.|...
-00001f60: 6406 7c03 9b02 6407 9d07 8301 8201 7406  d.|...d.......t.
-00001f70: 7c00 7c01 7c03 7c04 7c05 6408 8d05 5c02  |.|.|.|.|.d...\.
-00001f80: 7d07 7d08 7407 6a08 6700 7409 6409 8d02  }.}.t.j.g.t.d...
-00001f90: 7d09 7c02 6402 7501 7250 7406 7c00 6a0a  }.|.d.u.rPt.|.j.
-00001fa0: 7c07 640a 8d01 7c01 7c02 6401 7c03 1800  |.d...|.|.d.|...
-00001fb0: 1b00 7c04 7c05 6408 8d05 5c02 7d07 7d09  ..|.|.d...\.}.}.
-00001fc0: 7c07 7c09 7c08 6603 5300 290b 728b 0000  |.|.|.f.S.).r...
-00001fd0: 0072 0700 0000 4e72 0100 0000 7a0b 7472  .r....Nr....z.tr
-00001fe0: 6169 6e5f 7369 7a65 3d7a 2a20 6973 2062  ain_size=z* is b
-00001ff0: 656c 6f77 207a 6572 6f21 2028 4465 6372  elow zero! (Decr
-00002000: 6561 7365 2076 616c 6964 6174 696f 6e5f  ease validation_
-00002010: 7369 7a65 3d7a 1220 616e 642f 6f72 2074  size=z. and/or t
-00002020: 6573 745f 7369 7a65 3dfa 0129 2905 7286  est_size=..)).r.
-00002030: 0000 0072 8700 0000 7288 0000 0072 8900  ...r....r....r..
-00002040: 0000 728a 0000 0029 01da 0564 7479 7065  ..r....)...dtype
-00002050: 2901 da05 696e 6465 7829 0b72 2500 0000  )...index).r%...
-00002060: 724d 0000 00da 0c6c 6f61 645f 6461 7461  rM.....load_data
-00002070: 7365 74da 1672 6573 6574 5f69 6e64 6578  set..reset_index
-00002080: 5f63 6f6f 7264 696e 6174 65da 0463 6f70  _coordinate..cop
-00002090: 79da 0a56 616c 7565 4572 726f 7272 9800  y..ValueErrorr..
-000020a0: 0000 7291 0000 00da 0561 7272 6179 7217  ..r......arrayr.
-000020b0: 0000 00da 0373 656c 290a 7286 0000 0072  .....sel).r....r
-000020c0: 8700 0000 7299 0000 0072 8800 0000 7289  ....r....r....r.
-000020d0: 0000 0072 8a00 0000 da0a 7472 6169 6e5f  ...r......train_
-000020e0: 7369 7a65 7296 0000 0072 9700 0000 da10  sizer....r......
-000020f0: 696e 6469 6365 735f 7661 6c69 6461 7465  indices_validate
-00002100: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
-00002110: 1a73 706c 6974 5f74 7261 696e 696e 675f  .split_training_
-00002120: 7365 745f 7472 6970 706c 6513 0100 0073  set_tripple....s
-00002130: 2e00 0000 1219 0801 0801 0801 0801 1c01  ................
-00002140: 0201 0201 0201 0201 0201 0201 0afb 0e07  ................
-00002150: 0801 0201 0a01 0201 0a01 0201 0201 0afb  ................
-00002160: 0a07 72a5 0000 0072 0a00 0000 7257 0000  ..r....r....rW..
-00002170: 0072 5800 0000 7255 0000 0072 5600 0000  .rX...rU...rV...
-00002180: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
-00002190: 000b 0000 0043 0000 0073 bc00 0000 7400  .....C...s....t.
-000021a0: a001 6401 7c01 9b02 6402 7c02 9b02 6403  ..d.|...d.|...d.
-000021b0: 7c03 9b02 6404 7c00 9b02 6405 9d09 a101  |...d.|...d.....
-000021c0: 0100 7c01 6400 7500 721e 7402 6406 7c01  ..|.d.u.r.t.d.|.
-000021d0: 9b02 6407 9d03 8301 8201 7c00 6408 6b02  ..d.......|.d.k.
-000021e0: 7223 6e18 7c00 6409 6b02 722e 7c01 6400  r#n.|.d.k.r.|.d.
-000021f0: 7501 722d 7c01 7d03 6e0d 7c00 640a 6b02  u.r-|.}.n.|.d.k.
-00002200: 7233 6e08 7402 640b 7c00 9b02 640c 9d03  r3n.t.d.|...d...
-00002210: 8301 8201 7c02 6400 7500 7241 7c01 7d02  ....|.d.u.rA|.}.
-00002220: 7c03 6400 7500 7247 7c01 7d03 7400 a001  |.d.u.rG|.}.t...
-00002230: 640d 7c01 9b02 6402 7c02 9b02 6403 7c03  d.|...d.|...d.|.
-00002240: 9b02 6404 7c00 9b02 6405 9d09 a101 0100  ..d.|...d.......
-00002250: 7c01 7c03 7c02 6603 5300 290e 4e7a 1855  |.|.|.f.S.).Nz.U
-00002260: 7365 7220 6368 6f69 6365 3a20 6576 616c  ser choice: eval
-00002270: 5f73 7465 7073 3d7a 0f20 6c6f 6767 696e  _steps=z. loggin
-00002280: 675f 7374 6570 733d 7a0c 2073 6176 655f  g_steps=z. save_
-00002290: 7374 6570 733d 7a17 2c20 2865 7661 6c75  steps=z., (evalu
-000022a0: 6174 696f 6e5f 7374 7261 7465 6779 3d72  ation_strategy=r
-000022b0: 9a00 0000 7a0b 6576 616c 5f73 7465 7073  ....z.eval_steps
-000022c0: 3d7a 1020 6361 6e6e 6f74 2062 6520 4e6f  =z. cannot be No
-000022d0: 6e65 2172 4c00 0000 724a 0000 00da 026e  ne!rL...rJ.....n
-000022e0: 6f7a 1465 7661 6c75 6174 696f 6e5f 7374  oz.evaluation_st
-000022f0: 7261 7465 6779 3d7a 0b20 6e6f 7420 6b6e  rategy=z. not kn
-00002300: 6f77 6e21 7a14 5365 7474 696e 673a 2065  own!z.Setting: e
-00002310: 7661 6c5f 7374 6570 733d 2903 7268 0000  val_steps=).rh..
-00002320: 0072 6900 0000 72a0 0000 0072 5b00 0000  .ri...r....r[...
-00002330: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-00002340: 6a00 0000 4501 0000 7324 0000 0024 0308  j...E...s$...$..
-00002350: 0110 0108 0102 0208 0108 0104 0102 8008  ................
-00002360: 0102 0110 0208 0104 0108 0104 0124 010a  .............$..
-00002370: 0172 6a00 0000 2901 721b 0000 0029 0472  .rj...).r....).r
-00002380: 1b00 0000 7284 0000 0072 8500 0000 5429  ....r....r....T)
-00002390: 0572 1b00 0000 4e72 8400 0000 7285 0000  .r....Nr....r...
-000023a0: 0054 2903 720a 0000 004e 4e29 1eda 0b64  .T).r....NN)...d
-000023b0: 6174 6163 6c61 7373 6573 726c 0000 0072  ataclassesrl...r
-000023c0: 6800 0000 da06 7479 7069 6e67 7272 0000  h.....typingrr..
-000023d0: 00da 0a61 322e 6461 7461 7365 7472 2500  ...a2.datasetr%.
-000023e0: 0000 da14 6132 2e70 6c6f 7474 696e 672e  ....a2.plotting.
-000023f0: 616e 616c 7973 6973 da14 6132 2e74 7261  analysis..a2.tra
-00002400: 696e 696e 672e 7472 6163 6b69 6e67 da1a  ining.tracking..
-00002410: 6132 2e74 7261 696e 696e 672e 7574 696c  a2.training.util
-00002420: 735f 7472 6169 6e69 6e67 7278 0000 00da  s_trainingrx....
-00002430: 056e 756d 7079 7291 0000 00da 1773 6b6c  .numpyr......skl
-00002440: 6561 726e 2e6d 6f64 656c 5f73 656c 6563  earn.model_selec
-00002450: 7469 6f6e 728e 0000 0072 3400 0000 da06  tionr....r4.....
-00002460: 7861 7272 6179 da09 6461 7461 636c 6173  xarray..dataclas
-00002470: 7372 0200 0000 722e 0000 0072 2f00 0000  sr....r....r/...
-00002480: 726e 0000 0072 7900 0000 7218 0000 0072  rn...ry...r....r
-00002490: 1500 0000 7217 0000 0072 7500 0000 7298  ....r....ru...r.
-000024a0: 0000 0072 a500 0000 726a 0000 0072 1900  ...r....rj...r..
-000024b0: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-000024c0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000024d0: 7c00 0000 0800 0801 0801 0801 0802 0801  |...............
-000024e0: 0801 0801 0801 0801 0801 0801 0801 0403  ................
-000024f0: 1001 0a11 0e22 007f 081d 020e 0201 0201  ....."..........
-00002500: 0201 04fb 0401 02ff 0202 02fe 0203 02fd  ................
-00002510: 0204 02fc 0205 0afb 0228 0201 0201 0201  .........(......
-00002520: 0201 04fa 0401 02ff 0202 02fe 0603 02fd  ................
-00002530: 0204 02fc 0205 02fb 0206 0afa 0233 04ff  .............3..
-00002540: 0201 02ff 0201 02ff 0601 02ff 0601 0eff  ................
+000000a0: 8400 6403 8302 8301 5a12 6500 6a11 4700  ..d.....Z.e.j.G.
+000000b0: 6404 6405 8400 6405 6512 8303 8301 5a13  d.d...d.e.....Z.
+000000c0: 6500 6a11 4700 6406 6407 8400 6407 6512  e.j.G.d.d...d.e.
+000000d0: 8303 8301 5a14 6423 6409 640a 8401 5a15  ....Z.d#d.d...Z.
+000000e0: 4700 640b 640c 8400 640c 8302 5a16 640d  G.d.d...d...Z.d.
+000000f0: 640e 8400 5a17 0908 090f 0910 0911 6424  d...Z.........d$
+00000100: 6412 6510 6a18 6413 6519 6414 651a 6415  d.e.j.d.e.d.e.d.
+00000110: 651b 6416 651c 660a 6417 6418 8405 5a1d  e.d.e.f.d.d...Z.
+00000120: 0908 0901 090f 0910 0911 6425 6412 6510  ..........d%d.e.
+00000130: 6a18 6413 6519 6419 651a 6401 4200 6414  j.d.e.d.e.d.B.d.
+00000140: 651a 6415 651b 6416 651c 660c 641a 641b  e.d.e.d.e.f.d.d.
+00000150: 8405 5a1e 0901 6426 641d 6519 641e 651b  ..Z...d&d.e.d.e.
+00000160: 641f 6401 651b 4200 6420 6401 651b 4200  d.d.e.B.d d.e.B.
+00000170: 6608 6421 6422 8405 5a1f 6401 5300 2927  f.d!d"..Z.d.S.)'
+00000180: e900 0000 004e 6300 0000 0000 0000 0000  .....Nc.........
+00000190: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
+000001a0: 8a00 0000 6500 5a01 6400 5a02 5500 6401  ....e.Z.d.Z.U.d.
+000001b0: 5a03 6402 5a04 6505 6506 6403 3c00 6404  Z.d.Z.e.e.d.<.d.
+000001c0: 5a07 6508 6506 6405 3c00 6406 5a09 6505  Z.e.e.d.<.d.Z.e.
+000001d0: 6506 6407 3c00 6408 5a0a 6508 6506 6409  e.d.<.d.Z.e.e.d.
+000001e0: 3c00 640a 5a0b 6505 6506 640b 3c00 640c  <.d.Z.e.e.d.<.d.
+000001f0: 5a0c 6505 6506 640d 3c00 640e 5a0d 6505  Z.e.e.d.<.d.Z.e.
+00000200: 6506 640f 3c00 640e 5a0e 6505 6506 6410  e.d.<.d.Z.e.e.d.
+00000210: 3c00 640e 5a0f 6505 6506 6411 3c00 6412  <.d.Z.e.e.d.<.d.
+00000220: 5a10 6511 6506 6413 3c00 6414 5300 2915  Z.e.e.d.<.d.S.).
+00000230: da24 4879 7065 7250 6172 616d 6574 6572  .$HyperParameter
+00000240: 7348 7567 6769 6e67 4661 6365 436c 6173  sHuggingFaceClas
+00000250: 7369 6669 6572 fa43 0a20 2020 2048 6f6c  sifier.C.    Hol
+00000260: 6420 6879 7065 7220 7061 7261 6d65 7465  d hyper paramete
+00000270: 7273 2066 6f72 2048 7567 6769 6e67 2046  rs for Hugging F
+00000280: 6163 6520 4465 4245 5254 6120 636c 6173  ace DeBERTa clas
+00000290: 7369 6669 6572 0a20 2020 20e7 691d 554d  sifier.    .i.UM
+000002a0: 1075 ff3e da0d 6c65 6172 6e69 6e67 5f72  .u.>..learning_r
+000002b0: 6174 65e9 2000 0000 da0a 6261 7463 685f  ate. .....batch_
+000002c0: 7369 7a65 677b 14ae 47e1 7a84 3fda 0c77  sizeg{..G.z.?..w
+000002d0: 6569 6768 745f 6465 6361 79e9 0100 0000  eight_decay.....
+000002e0: da06 6570 6f63 6873 7201 0000 00da 0c77  ..epochsr......w
+000002f0: 6172 6d75 705f 7261 7469 6fe9 f401 0000  armup_ratio.....
+00000300: da0c 7761 726d 7570 5f73 7465 7073 679a  ..warmup_stepsg.
+00000310: 9999 9999 99b9 3fda 1368 6964 6465 6e5f  ......?..hidden_
+00000320: 6472 6f70 6f75 745f 7072 6f62 da1c 6174  dropout_prob..at
+00000330: 7465 6e74 696f 6e5f 7072 6f62 735f 6472  tention_probs_dr
+00000340: 6f70 6f75 745f 7072 6f62 da0b 636c 735f  opout_prob..cls_
+00000350: 6472 6f70 6f75 74da 066c 696e 6561 72da  dropout..linear.
+00000360: 116c 725f 7363 6865 6475 6c65 725f 7479  .lr_scheduler_ty
+00000370: 7065 4e29 12da 085f 5f6e 616d 655f 5fda  peN)...__name__.
+00000380: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000390: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
+000003a0: 5f5f 7205 0000 00da 0566 6c6f 6174 da0f  __r......float..
+000003b0: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5f72  __annotations__r
+000003c0: 0700 0000 da03 696e 7472 0800 0000 720a  ......intr....r.
+000003d0: 0000 0072 0b00 0000 720d 0000 0072 0e00  ...r....r....r..
+000003e0: 0000 720f 0000 0072 1000 0000 7212 0000  ..r....r....r...
+000003f0: 00da 0373 7472 a900 721b 0000 0072 1b00  ...str..r....r..
+00000400: 0000 fa3e 2f68 6f6d 652f 6b72 6973 7469  ...>/home/kristi
+00000410: 616e 2f50 726f 6a65 6374 732f 6132 2f73  an/Projects/a2/s
+00000420: 7263 2f61 322f 7472 6169 6e69 6e67 2f74  rc/a2/training/t
+00000430: 7261 696e 696e 675f 6875 6767 696e 672e  raining_hugging.
+00000440: 7079 7202 0000 0011 0000 0073 1800 0000  pyr........s....
+00000450: 0a00 0402 0c03 0c01 0c01 0c01 0c01 0c01  ................
+00000460: 0c01 0c01 0c01 1001 7202 0000 0063 0000  ........r....c..
+00000470: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+00000480: 0000 4000 0000 f31e 0000 0065 005a 0164  ..@........e.Z.d
+00000490: 005a 0255 0064 015a 0364 025a 0465 0565  .Z.U.d.Z.d.Z.e.e
+000004a0: 0664 033c 0064 0453 0029 05da 2048 7970  .d.<.d.S.).. Hyp
+000004b0: 6572 5061 7261 6d65 7465 7273 4465 6265  erParametersDebe
+000004c0: 7274 6143 6c61 7373 6966 6965 7272 0300  rtaClassifierr..
+000004d0: 0000 7204 0000 0072 0500 0000 4ea9 0772  ..r....r....N..r
+000004e0: 1300 0000 7214 0000 0072 1500 0000 7216  ....r....r....r.
+000004f0: 0000 0072 0500 0000 7217 0000 0072 1800  ...r....r....r..
+00000500: 0000 721b 0000 0072 1b00 0000 721b 0000  ..r....r....r...
+00000510: 0072 1c00 0000 721e 0000 0022 0000 00f3  .r....r...."....
+00000520: 0600 0000 0a00 0402 1003 721e 0000 0063  ..........r....c
+00000530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000540: 0300 0000 4000 0000 721d 0000 0029 05da  ....@...r....)..
+00000550: 2048 7970 6572 5061 7261 6d65 7465 7273   HyperParameters
+00000560: 456c 6563 7472 6143 6c61 7373 6966 6965  ElectraClassifie
+00000570: 7272 0300 0000 67f1 68e3 88b5 f8f4 3e72  rr....g.h.....>r
+00000580: 0500 0000 4e72 1f00 0000 721b 0000 0072  ....Nr....r....r
+00000590: 1b00 0000 721b 0000 0072 1c00 0000 7221  ....r....r....r!
+000005a0: 0000 002a 0000 0072 2000 0000 7221 0000  ...*...r ...r!..
+000005b0: 00da 0772 6169 6e69 6e67 6302 0000 0000  ...rainingc.....
+000005c0: 0000 0000 0000 0009 0000 0008 0000 0043  ...............C
+000005d0: 0000 0073 8000 0000 7c00 5c02 7d02 7d03  ...s....|.\.}.}.
+000005e0: 7c02 6a00 6401 6402 8d01 7d02 7401 6a02  |.j.d.d...}.t.j.
+000005f0: 6a03 6a04 7c03 7c02 7c01 6403 6404 8d04  j.j.|.|.|.d.d...
+00000600: 7d04 7c04 6405 1900 6406 1900 7d05 7c04  }.|.d...d...}.|.
+00000610: 6407 1900 6406 1900 7d06 7c04 6408 7c01  d...d...}.|.d.|.
+00000620: 9b00 9d02 1900 6406 1900 7d07 7c04 7c01  ......d...}.|.|.
+00000630: 1900 6406 1900 7d08 6409 7c01 9b00 9d02  ..d...}.d.|.....
+00000640: 7c07 640a 7c01 9b00 9d02 7c08 640b 7c05  |.d.|.....|.d.|.
+00000650: 640c 7c06 6904 5300 290d 6127 0100 000a  d.|.i.S.).a'....
+00000660: 2020 2020 4164 6f70 7420 4875 6767 696e      Adopt Huggin
+00000670: 6720 4661 6365 206d 6574 7269 6320 6f75  g Face metric ou
+00000680: 7470 7574 2074 6f20 7072 6566 6572 6564  tput to prefered
+00000690: 206d 6574 7269 630a 2020 2020 2866 312d   metric.    (f1-
+000006a0: 7363 6f72 6529 2066 6f72 2074 6869 7320  score) for this 
+000006b0: 7072 6f6a 6563 740a 0a20 2020 2050 6172  project..    Par
+000006c0: 616d 6574 6572 733a 0a20 2020 202d 2d2d  ameters:.    ---
+000006d0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6576 616c  -------.    eval
+000006e0: 5f70 7265 643a 2050 7265 6469 6374 696f  _pred: Predictio
+000006f0: 6e73 2061 6e64 206c 6162 656c 7320 6f66  ns and labels of
+00000700: 2048 7567 6769 6e67 2046 6163 6520 6d6f   Hugging Face mo
+00000710: 6465 6c20 7768 696c 6520 7472 6169 6e69  del while traini
+00000720: 6e67 0a20 2020 206c 6162 656c 3a20 4c61  ng.    label: La
+00000730: 6265 6c20 6e61 6d65 206f 6620 7468 6520  bel name of the 
+00000740: 636c 6173 7369 6669 6361 7469 6f6e 0a0a  classification..
+00000750: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00000760: 2d2d 2d2d 2d2d 2d0a 2020 2020 6469 6374  -------.    dict
+00000770: 696f 6e61 7279 206f 6620 6d65 7472 6963  ionary of metric
+00000780: 730a 2020 2020 e9ff ffff ff29 01da 0461  s.    .....)...a
+00000790: 7869 7354 2902 da05 6c61 6265 6cda 0b6f  xisT)...label..o
+000007a0: 7574 7075 745f 6469 6374 7a0c 7765 6967  utput_dictz.weig
+000007b0: 6874 6564 2061 7667 7a08 6631 2d73 636f  hted avgz.f1-sco
+000007c0: 7265 7a09 6d61 6372 6f20 6176 677a 046e  rez.macro avgz.n
+000007d0: 6f74 20da 0766 315f 6e6f 745f da03 6631  ot ..f1_not_..f1
+000007e0: 5fda 1366 315f 7765 6967 6874 6564 5f61  _..f1_weighted_a
+000007f0: 7665 7261 6765 da10 6631 5f6d 6163 726f  verage..f1_macro
+00000800: 5f61 7665 7261 6765 2905 da06 6172 676d  _average)...argm
+00000810: 6178 da02 6132 da08 706c 6f74 7469 6e67  ax..a2..plotting
+00000820: da08 616e 616c 7973 6973 da15 636c 6173  ..analysis..clas
+00000830: 7369 6669 6361 7469 6f6e 5f72 6570 6f72  sification_repor
+00000840: 7429 09da 0965 7661 6c5f 7072 6564 7225  t)...eval_predr%
+00000850: 0000 00da 0b70 7265 6469 6374 696f 6e73  .....predictions
+00000860: da06 6c61 6265 6c73 722f 0000 0072 2900  ..labelsr/...r).
+00000870: 0000 722a 0000 00da 0666 315f 6e6f 74da  ..r*.....f1_not.
+00000880: 0266 3172 1b00 0000 721b 0000 0072 1c00  .f1r....r....r..
+00000890: 0000 da10 5f63 6f6d 7075 7465 5f6d 6574  ...._compute_met
+000008a0: 7269 6373 3200 0000 7322 0000 0008 0e0c  rics2...s"......
+000008b0: 0108 0102 0102 0102 0102 0106 fc0c 060c  ................
+000008c0: 0112 010c 010a 020a 0104 0104 0104 fc72  ...............r
+000008d0: 3500 0000 6300 0000 0000 0000 0000 0000  5...c...........
+000008e0: 0000 0000 0025 0000 0040 0000 0073 ee00  .....%...@...s..
+000008f0: 0000 6500 5a01 6400 5a02 6401 5a03 0902  ..e.Z.d.Z.d.Z...
+00000900: 0903 6428 6404 6504 6405 6505 6406 6506  ..d(d.e.d.e.d.e.
+00000910: 6a07 6506 6a08 1900 6606 6407 6408 8405  j.e.j...f.d.d...
+00000920: 5a09 6429 640a 6506 6a08 640b 650a 640c  Z.d)d.e.j.d.e.d.
+00000930: 650a 6606 640d 640e 8405 5a0b 6403 6403  e.f.d.d...Z.d.d.
+00000940: 640f 6410 6409 6410 6409 6410 6403 6409  d.d.d.d.d.d.d.d.
+00000950: 650c 6a0d 6411 6411 6412 6413 6414 6409  e.j.d.d.d.d.d.d.
+00000960: 6415 6612 6416 6506 6a0e 650f 6a10 650f  d.f.d.e.j.e.j.e.
+00000970: 6a11 6602 1900 6417 6512 6403 4200 6418  j.f...d.e.d.B.d.
+00000980: 6506 6a07 650c 6a13 1900 6403 4200 6419  e.j.e.j...d.B.d.
+00000990: 6504 641a 650a 641b 650a 641c 650a 640b  e.d.e.d.e.d.e.d.
+000009a0: 650a 641d 650a 641e 6514 6403 4200 640c  e.d.e.d.e.d.B.d.
+000009b0: 650a 641f 6505 6420 6505 6421 6504 6422  e.d.e.d e.d!e.d"
+000009c0: 6505 6403 4200 6423 6504 6424 650a 6425  e.d.B.d#e.d$e.d%
+000009d0: 6504 6624 6426 6427 8405 5a15 6403 5300  e.f$d&d'..Z.d.S.
+000009e0: 292a da17 4875 6767 696e 6746 6163 6554  )*..HuggingFaceT
+000009f0: 7261 696e 6572 436c 6173 737a 2b0a 2020  rainerClassz+.  
+00000a00: 2020 5573 6564 2074 6f20 7472 6169 6e20    Used to train 
+00000a10: 4875 6767 696e 6720 4661 6365 206d 6f64  Hugging Face mod
+00000a20: 656c 730a 2020 2020 e902 0000 004e da0c  els.    .....N..
+00000a30: 6d6f 6465 6c5f 666f 6c64 6572 da0a 6e75  model_folder..nu
+00000a40: 6d5f 6c61 6265 6c73 da06 636f 6e66 6967  m_labels..config
+00000a50: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
+00000a60: 0004 0000 0043 0000 0073 3a00 0000 7c01  .....C...s:...|.
+00000a70: 7c00 5f00 7c02 7c00 5f01 7c03 6400 7500  |._.|.|._.|.d.u.
+00000a80: 7214 7402 6a03 6a04 7c01 7c02 6401 8d02  r.t.j.j.|.|.d...
+00000a90: 7c00 5f05 6e03 7c03 7c00 5f05 7406 8300  |._.n.|.|._.t...
+00000aa0: 7c00 5f07 6400 5300 2902 4e29 0172 3900  |._.d.S.).N).r9.
+00000ab0: 0000 2908 7238 0000 0072 3900 0000 da0c  ..).r8...r9.....
+00000ac0: 7472 616e 7366 6f72 6d65 7273 da0a 4175  transformers..Au
+00000ad0: 746f 436f 6e66 6967 da0f 6672 6f6d 5f70  toConfig..from_p
+00000ae0: 7265 7472 6169 6e65 64da 0e64 625f 636f  retrained..db_co
+00000af0: 6e66 6967 5f62 6173 6572 1e00 0000 da10  nfig_baser......
+00000b00: 6879 7065 725f 7061 7261 6d65 7465 7273  hyper_parameters
+00000b10: 2904 da04 7365 6c66 7238 0000 0072 3900  )...selfr8...r9.
+00000b20: 0000 723a 0000 0072 1b00 0000 721b 0000  ..r:...r....r...
+00000b30: 0072 1c00 0000 da08 5f5f 696e 6974 5f5f  .r......__init__
+00000b40: 5900 0000 730c 0000 0006 0606 0108 0114  Y...s...........
+00000b50: 0106 020c 017a 2048 7567 6769 6e67 4661  .....z HuggingFa
+00000b60: 6365 5472 6169 6e65 7243 6c61 7373 2e5f  ceTrainerClass._
+00000b70: 5f69 6e69 745f 5f54 da06 7061 7261 6d73  _init__T..params
+00000b80: da06 6d61 6e74 696b da14 6261 7365 5f6d  ..mantik..base_m
+00000b90: 6f64 656c 5f74 7261 696e 6162 6c65 6304  odel_trainablec.
+00000ba0: 0000 0000 0000 0000 0000 0007 0000 0005  ................
+00000bb0: 0000 0043 0000 0073 7000 0000 7c00 6a00  ...C...sp...|.j.
+00000bc0: 7d04 7c01 6400 7501 7210 7c04 a001 6401  }.|.d.u.r.|...d.
+00000bd0: 7c01 6401 1900 6901 a101 0100 7c04 a001  |.d...i.....|...
+00000be0: 6402 7c00 6a02 6901 a101 0100 7403 6a04  d.|.j.i.....t.j.
+00000bf0: 6a05 7c00 6a06 7c04 6403 8d02 7d05 7c03  j.|.j.|.d...}.|.
+00000c00: 732e 7c05 6a07 a008 a100 4400 5d05 7d06  s.|.j.....D.].}.
+00000c10: 6404 7c06 5f09 7128 7c02 7236 740a 6a0b  d.|._.q(|.r6t.j.
+00000c20: 6a0c a00d a100 0100 7c05 5300 2905 4e72  j.......|.S.).Nr
+00000c30: 1000 0000 7239 0000 0029 0172 3a00 0000  ....r9...).r:...
+00000c40: 4629 0e72 3e00 0000 da06 7570 6461 7465  F).r>.....update
+00000c50: 7239 0000 0072 3b00 0000 da22 4175 746f  r9...r;...."Auto
+00000c60: 4d6f 6465 6c46 6f72 5365 7175 656e 6365  ModelForSequence
+00000c70: 436c 6173 7369 6669 6361 7469 6f6e 723d  Classificationr=
+00000c80: 0000 0072 3800 0000 da0a 6261 7365 5f6d  ...r8.....base_m
+00000c90: 6f64 656c da0a 7061 7261 6d65 7465 7273  odel..parameters
+00000ca0: da0d 7265 7175 6972 6573 5f67 7261 6472  ..requires_gradr
+00000cb0: 2c00 0000 da08 7472 6169 6e69 6e67 da08  ,.....training..
+00000cc0: 7472 6163 6b69 6e67 da11 696e 6974 6961  tracking..initia
+00000cd0: 6c69 7a65 5f6d 616e 7469 6b29 0772 4000  lize_mantik).r@.
+00000ce0: 0000 7242 0000 0072 4300 0000 7244 0000  ..rB...rC...rD..
+00000cf0: 00da 0964 625f 636f 6e66 6967 da05 6d6f  ...db_config..mo
+00000d00: 6465 6cda 0570 6172 616d 721b 0000 0072  del..paramr....r
+00000d10: 1b00 0000 721c 0000 00da 0967 6574 5f6d  ....r......get_m
+00000d20: 6f64 656c 6700 0000 7316 0000 0006 0108  odelg...s.......
+00000d30: 0112 0110 0112 0104 010e 0108 0104 010c  ................
+00000d40: 0104 017a 2148 7567 6769 6e67 4661 6365  ...z!HuggingFace
+00000d50: 5472 6169 6e65 7243 6c61 7373 2e67 6574  TrainerClass.get
+00000d60: 5f6d 6f64 656c 7a07 6f75 7470 7574 2f46  _modelz.output/F
+00000d70: 720c 0000 00da 0573 7465 7073 e964 0000  r......steps.d..
+00000d80: 00da 0565 706f 6368 7222 0000 00da 0764  ...epochr".....d
+00000d90: 6174 6173 6574 723f 0000 00da 0974 6f6b  atasetr?.....tok
+00000da0: 656e 697a 6572 da0d 666f 6c64 6572 5f6f  enizer..folder_o
+00000db0: 7574 7075 74da 0c68 7970 6572 5f74 756e  utput..hyper_tun
+00000dc0: 696e 67da 0466 7031 36da 0865 7661 6c75  ing..fp16..evalu
+00000dd0: 6174 65da 0c64 6973 6162 6c65 5f74 7164  ate..disable_tqd
+00000de0: 6dda 0963 616c 6c62 6163 6b73 da0d 6c6f  m..callbacks..lo
+00000df0: 6767 696e 675f 7374 6570 73da 0a73 6176  gging_steps..sav
+00000e00: 655f 7374 6570 73da 1365 7661 6c75 6174  e_steps..evaluat
+00000e10: 696f 6e5f 7374 7261 7465 6779 da0a 6576  ion_strategy..ev
+00000e20: 616c 5f73 7465 7073 da0d 7361 7665 5f73  al_steps..save_s
+00000e30: 7472 6174 6567 79da 166c 6f61 645f 6265  trategy..load_be
+00000e40: 7374 5f6d 6f64 656c 5f61 745f 656e 6472  st_model_at_endr
+00000e50: 2500 0000 6314 0000 0000 0000 0000 0000  %...c...........
+00000e60: 0019 0000 0009 0000 0043 0000 0073 7801  .........C...sx.
+00000e70: 0000 7400 6a01 6a02 a003 a100 7308 6401  ..t.j.j.....s.d.
+00000e80: 7d06 7c02 6402 7500 720f 7404 8300 7d02  }.|.d.u.r.t...}.
+00000e90: 7c02 7c00 5f05 7c03 6402 7500 721d 7406  |.|._.|.d.u.r.t.
+00000ea0: 6a07 a008 7c00 6a09 a101 7d03 7c12 723f  j...|.j...}.|.r?
+00000eb0: 7c11 7c0f 6b03 723f 740a a00b 6403 7c11  |.|.k.r?t...d.|.
+00000ec0: 9b02 6404 7c0f 9b02 6405 7c12 9b02 6406  ..d.|...d.|...d.
+00000ed0: 9d07 a101 0100 7c0f 7d11 740c 7c0f 7c10  ......|.}.t.|.|.
+00000ee0: 7c0d 7c0e 6407 8d04 5c03 7d10 7d0e 7d0d  |.|.d...\.}.}.}.
+00000ef0: 7c05 7384 7406 6a0d 7c04 6601 6900 6408  |.s.t.j.|.f.i.d.
+00000f00: 7c02 6a0e 9301 6409 7c02 6a0f 9301 640a  |.j...d.|.j...d.
+00000f10: 7c02 6a10 9301 640b 7c02 6a11 9301 640c  |.j...d.|.j...d.
+00000f20: 7c09 9301 640d 7c06 9301 640e 7c0f 9301  |...d.|...d.|...
+00000f30: 640f 7c02 6a12 9301 6410 7c02 6a12 9301  d.|.j...d.|.j...
+00000f40: 6411 7c02 6a13 9301 6412 7c02 6a14 9301  d.|.j...d.|.j...
+00000f50: 6413 6402 9301 6414 7c10 9301 6415 7c0e  d.d...d.|...d.|.
+00000f60: 9301 6416 7c11 9301 6417 7c0d 9301 6418  ..d.|...d.|...d.
+00000f70: 7c12 9301 8e01 7d14 6e0c 7406 6a0d 7c04  |.....}.n.t.j.|.
+00000f80: 6419 7c06 7c0f 6402 7c11 7c12 641a 8d07  d.|.|.d.|.|.d...
+00000f90: 7d14 7415 6a16 7c00 6a17 7c08 7c0b 641b  }.t.j.|.j.|.|.d.
+00000fa0: 8d03 7d15 7415 6a16 7418 7c13 641c 8d02  ..}.t.j.t.|.d...
+00000fb0: 7d16 7c07 72ab 7c0c 7c15 7c14 7c03 7c16  }.|.r.|.|.|.|.|.
+00000fc0: 7c0a 641d 8d05 5300 7419 7c01 8301 5c02  |.d...S.t.|...\.
+00000fd0: 7d17 7d18 7c0c 7c15 7c14 7c17 7c18 7c03  }.}.|.|.|.|.|.|.
+00000fe0: 7c16 7c0a 641e 8d07 5300 291f 617f 0500  |.|.d...S.).a...
+00000ff0: 000a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00001000: 7320 4875 6767 696e 6720 4661 6365 2074  s Hugging Face t
+00001010: 7261 696e 6572 206f 626a 6563 740a 0a20  rainer object.. 
+00001020: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00001030: 733a 0a20 2020 2020 2020 202d 2d2d 2d2d  s:.        -----
+00001040: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6461  -----.        da
+00001050: 7461 7365 743a 2044 6174 6173 6574 2069  taset: Dataset i
+00001060: 6e20 4875 6767 696e 6720 4661 6365 2066  n Hugging Face f
+00001070: 6f72 6d61 740a 2020 2020 2020 2020 6879  ormat.        hy
+00001080: 7065 725f 7061 7261 6d65 7465 7273 3a20  per_parameters: 
+00001090: 6879 7065 7220 7061 7261 6d65 7465 7273  hyper parameters
+000010a0: 2069 6e20 7468 6520 666f 726d 206f 6620   in the form of 
+000010b0: 6461 7461 0a20 2020 2020 2020 2020 2020  data.           
+000010c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000010d0: 6c61 7373 2060 4879 7065 7250 6172 616d  lass `HyperParam
+000010e0: 6574 6572 7344 6562 6572 7461 436c 6173  etersDebertaClas
+000010f0: 7369 6669 6572 600a 2020 2020 2020 2020  sifier`.        
+00001100: 746f 6b65 6e69 7a65 723a 2048 7567 6769  tokenizer: Huggi
+00001110: 6e67 2046 6163 6520 746f 6b65 6e69 7a65  ng Face tokenize
+00001120: 720a 2020 2020 2020 2020 666f 6c64 6572  r.        folder
+00001130: 5f6f 7574 7075 743a 2046 6f6c 6465 7220  _output: Folder 
+00001140: 746f 2073 6176 6520 7472 6169 6e69 6e67  to save training
+00001150: 206f 7574 7075 7473 0a20 2020 2020 2020   outputs.       
+00001160: 2068 7970 6572 5f74 756e 696e 673a 2057   hyper_tuning: W
+00001170: 6865 7468 6572 2074 7261 696e 6572 2075  hether trainer u
+00001180: 7365 6420 666f 7220 6879 7065 7220 7475  sed for hyper tu
+00001190: 6e69 6e67 0a20 2020 2020 2020 2066 7031  ning.        fp1
+000011a0: 363a 2057 6865 7468 6572 2074 6f20 7573  6: Whether to us
+000011b0: 6520 6670 3136 2031 362d 6269 7420 286d  e fp16 16-bit (m
+000011c0: 6978 6564 2920 7072 6563 6973 696f 6e20  ixed) precision 
+000011d0: 7472 6169 6e69 6e67 0a20 2020 2020 2020  training.       
+000011e0: 2020 2020 2020 2069 6e73 7465 6164 206f         instead o
+000011f0: 6620 3332 2d62 6974 2074 7261 696e 696e  f 32-bit trainin
+00001200: 672e 0a20 2020 2020 2020 2065 7661 6c75  g..        evalu
+00001210: 6174 653a 2057 6865 7468 6572 2074 7261  ate: Whether tra
+00001220: 696e 6572 206f 6e6c 7920 7573 6564 2066  iner only used f
+00001230: 6f72 2065 7661 6c75 6174 696f 6e0a 2020  or evaluation.  
+00001240: 2020 2020 2020 6d61 6e74 696b 3a20 5768        mantik: Wh
+00001250: 6574 6865 7220 7573 696e 6720 6d61 6e74  ether using mant
+00001260: 696b 2066 6f72 2074 7261 636b 696e 670a  ik for tracking.
+00001270: 2020 2020 2020 2020 6469 7361 626c 655f          disable_
+00001280: 7471 646d 3a20 5768 6574 6865 7220 746f  tqdm: Whether to
+00001290: 2064 6973 6162 6c65 2070 726f 6772 6573   disable progres
+000012a0: 7320 6261 7220 7573 6564 2062 7920 6054  s bar used by `T
+000012b0: 7261 6e73 666f 726d 6572 600a 2020 2020  ransformer`.    
+000012c0: 2020 2020 6361 6c6c 6261 636b 733a 2043      callbacks: C
+000012d0: 616c 6c62 6163 6b73 2064 7572 696e 6720  allbacks during 
+000012e0: 7472 6169 6e69 6e67 0a20 2020 2020 2020  training.       
+000012f0: 2062 6173 655f 6d6f 6465 6c5f 7472 6169   base_model_trai
+00001300: 6e61 626c 653a 2057 6865 7468 6572 2062  nable: Whether b
+00001310: 6173 6520 6d6f 6465 6c20 7765 6967 6874  ase model weight
+00001320: 7320 6172 6520 7472 6169 6e61 626c 6520  s are trainable 
+00001330: 286e 6f74 2066 6978 6564 290a 2020 2020  (not fixed).    
+00001340: 2020 2020 7472 6169 6e65 725f 636c 6173      trainer_clas
+00001350: 733a 2054 7261 696e 6572 2063 6c61 7373  s: Trainer class
+00001360: 2063 6f6d 7061 7469 626c 6520 7769 7468   compatible with
+00001370: 2060 7472 616e 7366 6f72 6d65 722e 5472   `transformer.Tr
+00001380: 6169 6e65 7260 0a20 2020 2020 2020 206c  ainer`.        l
+00001390: 6f67 6769 6e67 5f73 7465 7073 3a20 4e75  ogging_steps: Nu
+000013a0: 6d62 6572 206f 6620 7374 6570 7320 6265  mber of steps be
+000013b0: 666f 7265 2068 7567 6769 6e67 2066 6163  fore hugging fac
+000013c0: 6520 7072 696e 7473 0a20 2020 2020 2020  e prints.       
+000013d0: 2065 7661 6c75 6174 696f 6e5f 7374 7261   evaluation_stra
+000013e0: 7465 6779 3a20 5768 656e 2074 6f20 6576  tegy: When to ev
+000013f0: 616c 7561 7465 2c20 6166 7465 7220 2273  aluate, after "s
+00001400: 7465 7073 2220 6f72 2022 6570 6f63 6822  teps" or "epoch"
+00001410: 0a20 2020 2020 2020 2065 7661 6c5f 7374  .        eval_st
+00001420: 6570 733a 204e 756d 6265 7220 6f66 2073  eps: Number of s
+00001430: 7465 7073 2062 6574 7765 656e 2065 7661  teps between eva
+00001440: 6c75 6174 696f 6e20 286f 6e6c 7920 7573  luation (only us
+00001450: 6564 2069 6620 6065 7661 6c75 6174 696f  ed if `evaluatio
+00001460: 6e5f 7374 7261 7465 6779 603d 2273 7465  n_strategy`="ste
+00001470: 7073 2229 0a20 2020 2020 2020 2073 6176  ps").        sav
+00001480: 655f 7374 7261 7465 6779 3a20 5768 656e  e_strategy: When
+00001490: 2074 6f20 7361 7665 2062 6573 7420 6d6f   to save best mo
+000014a0: 6465 6c20 2273 7465 7073 2220 6f72 2022  del "steps" or "
+000014b0: 6570 6f63 6822 0a20 2020 2020 2020 206c  epoch".        l
+000014c0: 6f61 645f 6265 7374 5f6d 6f64 656c 5f61  oad_best_model_a
+000014d0: 745f 656e 643a 204c 6f61 6420 6265 7374  t_end: Load best
+000014e0: 206d 6f64 656c 2061 7420 656e 6420 6f66   model at end of
+000014f0: 2074 7261 696e 696e 670a 2020 2020 2020   training.      
+00001500: 2020 6c61 6265 6c3a 204c 6162 656c 206e    label: Label n
+00001510: 616d 6520 6f66 2074 6865 2063 6c61 7373  ame of the class
+00001520: 6966 6963 6174 696f 6e0a 0a20 2020 2020  ification..     
+00001530: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00001540: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00001550: 2020 2048 7567 6769 6e67 2046 6163 6520     Hugging Face 
+00001560: 5472 6169 6e65 720a 2020 2020 2020 2020  Trainer.        
+00001570: 464e 7a16 5365 7474 696e 6720 7361 7665  FNz.Setting save
+00001580: 5f73 7472 6174 6567 793d 7a1e 2065 7175  _strategy=z. equ
+00001590: 616c 2074 6f20 6576 616c 7561 7469 6f6e  al to evaluation
+000015a0: 5f73 7472 6174 6567 793d 7a27 2028 7265  _strategy=z' (re
+000015b0: 7175 6972 6564 2077 6865 6e20 6c6f 6164  quired when load
+000015c0: 5f62 6573 745f 6d6f 6465 6c5f 6174 5f65  _best_model_at_e
+000015d0: 6e64 3d7a 0820 3d20 5472 7565 29a9 0472  nd=z. = True)..r
+000015e0: 5e00 0000 725f 0000 0072 5c00 0000 725d  ^...r_...r\...r]
+000015f0: 0000 0072 0500 0000 720b 0000 0072 0d00  ...r....r....r..
+00001600: 0000 7212 0000 0072 5a00 0000 7258 0000  ..r....rZ...rX..
+00001610: 0072 5e00 0000 da1b 7065 725f 6465 7669  .r^.....per_devi
+00001620: 6365 5f74 7261 696e 5f62 6174 6368 5f73  ce_train_batch_s
+00001630: 697a 65da 1a70 6572 5f64 6576 6963 655f  ize..per_device_
+00001640: 6576 616c 5f62 6174 6368 5f73 697a 65da  eval_batch_size.
+00001650: 106e 756d 5f74 7261 696e 5f65 706f 6368  .num_train_epoch
+00001660: 7372 0800 0000 da09 7265 706f 7274 5f74  sr......report_t
+00001670: 6f72 5f00 0000 725d 0000 0072 6000 0000  or_...r]...r`...
+00001680: 725c 0000 0072 6100 0000 5429 0672 5a00  r\...ra...T).rZ.
+00001690: 0000 7258 0000 0072 5e00 0000 7266 0000  ..rX...r^...rf..
+000016a0: 0072 6000 0000 7261 0000 0029 0272 4300  .r`...ra...).rC.
+000016b0: 0000 7244 0000 0029 0172 2500 0000 2905  ..rD...).r%...).
+000016c0: da0a 6d6f 6465 6c5f 696e 6974 da04 6172  ..model_init..ar
+000016d0: 6773 7255 0000 00da 0f63 6f6d 7075 7465  gsrU.....compute
+000016e0: 5f6d 6574 7269 6373 725b 0000 0029 0772  _metricsr[...).r
+000016f0: 6700 0000 7268 0000 00da 0d74 7261 696e  g...rh.....train
+00001700: 5f64 6174 6173 6574 da0c 6576 616c 5f64  _dataset..eval_d
+00001710: 6174 6173 6574 7255 0000 0072 6900 0000  atasetrU...ri...
+00001720: 725b 0000 0029 1a72 2c00 0000 724a 0000  r[...).r,...rJ..
+00001730: 00da 0e75 7469 6c73 5f74 7261 696e 696e  ...utils_trainin
+00001740: 67da 0d67 7075 5f61 7661 696c 6162 6c65  g..gpu_available
+00001750: 721e 0000 0072 3f00 0000 723b 0000 00da  r....r?...r;....
+00001760: 0d41 7574 6f54 6f6b 656e 697a 6572 723d  .AutoTokenizerr=
+00001770: 0000 0072 3800 0000 da07 6c6f 6767 696e  ...r8.....loggin
+00001780: 67da 0469 6e66 6fda 2173 6574 5f65 7661  g..info.!set_eva
+00001790: 6c75 6174 696f 6e5f 7361 7665 5f6c 6f67  luation_save_log
+000017a0: 6769 6e67 5f73 7465 7073 da11 5472 6169  ging_steps..Trai
+000017b0: 6e69 6e67 4172 6775 6d65 6e74 7372 0500  ningArgumentsr..
+000017c0: 0000 720b 0000 0072 0d00 0000 7212 0000  ..r....r....r...
+000017d0: 0072 0700 0000 720a 0000 0072 0800 0000  .r....r....r....
+000017e0: da09 6675 6e63 746f 6f6c 73da 0770 6172  ..functools..par
+000017f0: 7469 616c 7250 0000 0072 3500 0000 da21  tialrP...r5....!
+00001800: 5f67 6574 5f74 7261 696e 696e 675f 6576  _get_training_ev
+00001810: 616c 7561 7469 6f6e 5f64 6174 6173 6574  aluation_dataset
+00001820: 7329 1972 4000 0000 7254 0000 0072 3f00  s).r@...rT...r?.
+00001830: 0000 7255 0000 0072 5600 0000 7257 0000  ..rU...rV...rW..
+00001840: 0072 5800 0000 7259 0000 0072 4300 0000  .rX...rY...rC...
+00001850: 725a 0000 0072 5b00 0000 7244 0000 00da  rZ...r[...rD....
+00001860: 0d74 7261 696e 6572 5f63 6c61 7373 725c  .trainer_classr\
+00001870: 0000 0072 5d00 0000 725e 0000 0072 5f00  ...r]...r^...r_.
+00001880: 0000 7260 0000 0072 6100 0000 7225 0000  ..r`...ra...r%..
+00001890: 0072 6800 0000 7267 0000 00da 185f 7061  .rh...rg....._pa
+000018a0: 7274 6961 6c5f 636f 6d70 7574 655f 6d65  rtial_compute_me
+000018b0: 7472 6963 7372 6a00 0000 726b 0000 0072  tricsrj...rk...r
+000018c0: 1b00 0000 721b 0000 0072 1c00 0000 da0b  ....r....r......
+000018d0: 6765 745f 7472 6169 6e65 7274 0000 0073  get_trainert...s
+000018e0: ae00 0000 0c34 0401 0801 0601 0601 0801  .....4..........
+000018f0: 0e01 0c01 0401 0e01 0201 06ff 04ff 0404  ................
+00001900: 0201 0201 0201 0201 0201 0cfc 0406 0401  ................
+00001910: 0201 06ff 0602 02fe 0603 02fd 0604 02fc  ................
+00001920: 0605 02fb 0406 02fa 0407 02f9 0408 02f8  ................
+00001930: 0609 02f7 060a 02f6 060b 02f5 060c 02f4  ................
+00001940: 040d 02f3 040e 02f2 040f 02f1 0410 02f0  ................
+00001950: 0411 02ef 0412 06ee 0415 0201 0201 0201  ................
+00001960: 0201 0201 0201 0201 06f9 1209 0e01 0401  ................
+00001970: 0201 0201 0201 0201 0201 0201 06fb 0c07  ................
+00001980: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001990: 06f9 7a23 4875 6767 696e 6746 6163 6554  ..z#HuggingFaceT
+000019a0: 7261 696e 6572 436c 6173 732e 6765 745f  rainerClass.get_
+000019b0: 7472 6169 6e65 7229 0272 3700 0000 4e29  trainer).r7...N)
+000019c0: 0254 5429 1672 1300 0000 7214 0000 0072  .TT).r....r....r
+000019d0: 1500 0000 7216 0000 0072 1a00 0000 7219  ....r....r....r.
+000019e0: 0000 00da 0174 da08 4f70 7469 6f6e 616c  .....t..Optional
+000019f0: da04 4469 6374 7241 0000 00da 0462 6f6f  ..DictrA.....boo
+00001a00: 6c72 5000 0000 723b 0000 00da 0754 7261  lrP...r;.....Tra
+00001a10: 696e 6572 da05 556e 696f 6eda 0864 6174  iner..Union..dat
+00001a20: 6173 6574 73da 0744 6174 6173 6574 da0b  asets..Dataset..
+00001a30: 4461 7461 7365 7444 6963 7472 1e00 0000  DatasetDictr....
+00001a40: da10 4465 6265 7274 6154 6f6b 656e 697a  ..DebertaTokeniz
+00001a50: 6572 da04 6c69 7374 7278 0000 0072 1b00  er..listrx...r..
+00001a60: 0000 721b 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+00001a70: 0072 3600 0000 5400 0000 7386 0000 0008  .r6...T...s.....
+00001a80: 0004 0102 0702 0104 fc02 0202 fe02 0302  ................
+00001a90: fd0a 040a fc1a 0e02 1002 0102 0102 0102  ................
+00001aa0: 0102 0102 0102 0102 0102 0104 0102 0102  ................
+00001ab0: 0102 0102 0102 0102 0102 0104 ec10 0202  ................
+00001ac0: fe06 0302 fd0e 0402 fc02 0502 fb02 0602  ................
+00001ad0: fa02 0702 f902 0802 f802 0902 f702 0a02  ................
+00001ae0: f606 0b02 f502 0c02 f402 0e02 f202 0f02  ................
+00001af0: f102 1002 f006 1102 ef02 1202 ee02 1302  ................
+00001b00: ed02 140e ec72 3600 0000 6301 0000 0000  .....r6...c.....
+00001b10: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
+00001b20: 0000 0073 6200 0000 7400 7c00 7401 6a02  ...sb...t.|.t.j.
+00001b30: 8302 7212 7c00 6401 1900 7d01 7c00 6402  ..r.|.d...}.|.d.
+00001b40: 1900 7d02 7c01 7c02 6602 5300 7400 7c00  ..}.|.|.f.S.t.|.
+00001b50: 7403 8302 7229 7404 7c00 8301 6403 6b02  t...r)t.|...d.k.
+00001b60: 7229 7c00 6404 1900 7d01 7c00 6405 1900  r)|.d...}.|.d...
+00001b70: 7d02 7c01 7c02 6602 5300 7405 6406 7c00  }.|.|.f.S.t.d.|.
+00001b80: 9b02 6407 9d03 8301 8201 2908 4eda 0574  ..d.......).N..t
+00001b90: 7261 696e da04 7465 7374 7237 0000 0072  rain..testr7...r
+00001ba0: 0100 0000 7209 0000 007a 1743 6f75 6c64  ....r....z.Could
+00001bb0: 6e27 7420 7061 7273 6520 6461 7461 7365  n't parse datase
+00001bc0: 743d fa01 2129 06da 0a69 7369 6e73 7461  t=..!)...isinsta
+00001bd0: 6e63 6572 7f00 0000 7281 0000 00da 0574  ncer....r......t
+00001be0: 7570 6c65 da03 6c65 6eda 0954 7970 6545  uple..len..TypeE
+00001bf0: 7272 6f72 2903 7254 0000 0072 6a00 0000  rror).rT...rj...
+00001c00: 726b 0000 0072 1b00 0000 721b 0000 0072  rk...r....r....r
+00001c10: 1c00 0000 7275 0000 00f0 0000 0073 1200  ....ru.......s..
+00001c20: 0000 0c01 0801 0801 0806 16fb 0801 0801  ................
+00001c30: 0803 10ff 7275 0000 00e7 9a99 9999 9999  ....ru..........
+00001c40: c93f e92a 0000 0054 da02 6473 da0c 6b65  .?.*...T..ds..ke
+00001c50: 795f 7374 7261 7469 6679 da09 7465 7374  y_stratify..test
+00001c60: 5f73 697a 65da 0c72 616e 646f 6d5f 7374  _size..random_st
+00001c70: 6174 65da 0773 6875 6666 6c65 6305 0000  ate..shufflec...
+00001c80: 0000 0000 0000 0000 0008 0000 0007 0000  ................
+00001c90: 0043 0000 0073 5400 0000 7c01 6401 7501  .C...sT...|.d.u.
+00001ca0: 720a 7c00 7c01 1900 6a00 7d05 6e02 6401  r.|.|...j.}.n.d.
+00001cb0: 7d05 7401 6a02 6a03 7404 a005 7c00 7406  }.t.j.j.t...|.t.
+00001cc0: 6a07 6a08 a009 7c00 a101 1900 6a0a 6402  j.j...|.....j.d.
+00001cd0: 1900 a101 7c02 7c03 7c04 7c05 6403 8d05  ....|.|.|.|.d...
+00001ce0: 5c02 7d06 7d07 7c06 7c07 6602 5300 2904  \.}.}.|.|.f.S.).
+00001cf0: e150 0200 000a 2020 2020 5265 7475 726e  .P....    Return
+00001d00: 7320 696e 6469 6365 7320 6f66 2074 7261  s indices of tra
+00001d10: 696e 696e 6720 616e 6420 7661 6c69 6461  ining and valida
+00001d20: 7469 6f6e 2073 6574 0a0a 2020 2020 5061  tion set..    Pa
+00001d30: 7261 6d65 7465 7273 3a0a 2020 2020 2d2d  rameters:.    --
+00001d40: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 733a  --------.    ds:
+00001d50: 2058 6172 7261 7920 6461 7461 7365 740a   Xarray dataset.
+00001d60: 2020 2020 6b65 795f 7374 7261 7469 6679      key_stratify
+00001d70: 3a20 5374 7261 7469 6669 6564 2062 6173  : Stratified bas
+00001d80: 6564 206f 6e20 7468 6973 206b 6579 2c20  ed on this key, 
+00001d90: 604e 6f6e 6560 2069 6620 6e6f 7420 7265  `None` if not re
+00001da0: 7175 6972 6564 0a20 2020 2076 616c 6964  quired.    valid
+00001db0: 6174 696f 6e5f 7369 7a65 3a20 4672 6163  ation_size: Frac
+00001dc0: 7469 6f6e 206f 6620 7661 6c69 6461 7469  tion of validati
+00001dd0: 6f6e 2073 6574 3b20 3120 2d20 7661 6c69  on set; 1 - vali
+00001de0: 6461 7469 6f6e 5f73 697a 6520 2d20 7465  dation_size - te
+00001df0: 7374 5f73 697a 6520 3e20 300a 2020 2020  st_size > 0.    
+00001e00: 7465 7374 5f73 697a 653a 2046 7261 6374  test_size: Fract
+00001e10: 696f 6e20 6f66 2074 6573 7420 7365 743b  ion of test set;
+00001e20: 2031 202d 2076 616c 6964 6174 696f 6e5f   1 - validation_
+00001e30: 7369 7a65 202d 2074 6573 745f 7369 7a65  size - test_size
+00001e40: 203e 2030 0a20 2020 2072 616e 646f 6d5f   > 0.    random_
+00001e50: 7374 6174 653a 2052 616e 646f 6d20 7365  state: Random se
+00001e60: 6564 2074 6f20 696e 6974 6961 6c69 7a65  ed to initialize
+00001e70: 2073 656c 6563 7469 6f6e 0a20 2020 2073   selection.    s
+00001e80: 6875 6666 6c65 3a20 5768 6574 6865 7220  huffle: Whether 
+00001e90: 6f72 206e 6f74 2074 6f20 7368 7566 666c  or not to shuffl
+00001ea0: 6520 7468 6520 6461 7461 2062 6566 6f72  e the data befor
+00001eb0: 6520 7370 6c69 7474 696e 672e 0a20 2020  e splitting..   
+00001ec0: 2020 2020 2020 2020 2020 4966 2073 6875            If shu
+00001ed0: 6666 6c65 3d46 616c 7365 2074 6865 6e20  ffle=False then 
+00001ee0: 7374 7261 7469 6679 206d 7573 7420 6265  stratify must be
+00001ef0: 204e 6f6e 652e 0a0a 2020 2020 5265 7475   None...    Retu
+00001f00: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
+00001f10: 2020 2020 496e 6469 6365 7320 6f66 2074      Indices of t
+00001f20: 7261 696e 696e 672c 2076 616c 6964 6174  raining, validat
+00001f30: 696f 6e20 616e 6420 7465 7374 2073 6574  ion and test set
+00001f40: 0a20 2020 204e 7201 0000 0029 0472 8f00  .    Nr....).r..
+00001f50: 0000 7290 0000 0072 9100 0000 da08 7374  ..r....r......st
+00001f60: 7261 7469 6679 290b da06 7661 6c75 6573  ratify)...values
+00001f70: da07 736b 6c65 6172 6eda 0f6d 6f64 656c  ..sklearn..model
+00001f80: 5f73 656c 6563 7469 6f6e da10 7472 6169  _selection..trai
+00001f90: 6e5f 7465 7374 5f73 706c 6974 da02 6e70  n_test_split..np
+00001fa0: da06 6172 616e 6765 722c 0000 0072 5400  ..aranger,...rT.
+00001fb0: 0000 da0d 7574 696c 735f 6461 7461 7365  ....utils_datase
+00001fc0: 74da 1767 6574 5f76 6172 6961 626c 655f  t..get_variable_
+00001fd0: 6e61 6d65 5f66 6972 7374 da05 7368 6170  name_first..shap
+00001fe0: 6529 0872 8d00 0000 728e 0000 0072 8f00  e).r....r....r..
+00001ff0: 0000 7290 0000 0072 9100 0000 7293 0000  ..r....r....r...
+00002000: 00da 0d69 6e64 6963 6573 5f74 7261 696e  ...indices_train
+00002010: da0c 696e 6469 6365 735f 7465 7374 721b  ..indices_testr.
+00002020: 0000 0072 1b00 0000 721c 0000 00da 1273  ...r....r......s
+00002030: 706c 6974 5f74 7261 696e 696e 675f 7365  plit_training_se
+00002040: 74fc 0000 0073 1600 0000 0818 0c01 0402  t....s..........
+00002050: 0601 1c01 0201 0201 0201 0201 0afb 0807  ................
+00002060: 729f 0000 00da 0f76 616c 6964 6174 696f  r......validatio
+00002070: 6e5f 7369 7a65 6306 0000 0000 0000 0000  n_sizec.........
+00002080: 0000 000a 0000 0008 0000 0043 0000 0073  ...........C...s
+00002090: aa00 0000 7400 6a01 6a02 a003 7c00 a004  ....t.j.j...|...
+000020a0: a100 a101 7d00 6401 7c03 1800 7d06 7c02  ....}.d.|...}.|.
+000020b0: 6402 7501 7215 7c06 7c02 3800 7d06 7c06  d.u.r.|.|.8.}.|.
+000020c0: 6403 6b00 7227 7405 6404 7c06 9b02 6405  d.k.r't.d.|...d.
+000020d0: 7c02 9b02 6406 7c03 9b02 6407 9d07 8301  |...d.|...d.....
+000020e0: 8201 7406 7c00 7c01 7c03 7c04 7c05 6408  ..t.|.|.|.|.|.d.
+000020f0: 8d05 5c02 7d07 7d08 7407 6a08 6700 7409  ..\.}.}.t.j.g.t.
+00002100: 6409 8d02 7d09 7c02 6402 7501 7250 7406  d...}.|.d.u.rPt.
+00002110: 7c00 6a0a 7c07 640a 8d01 7c01 7c02 6401  |.j.|.d...|.|.d.
+00002120: 7c03 1800 1b00 7c04 7c05 6408 8d05 5c02  |.....|.|.d...\.
+00002130: 7d07 7d09 7c07 7c09 7c08 6603 5300 290b  }.}.|.|.|.f.S.).
+00002140: 7292 0000 0072 0900 0000 4e72 0100 0000  r....r....Nr....
+00002150: 7a0b 7472 6169 6e5f 7369 7a65 3d7a 2a20  z.train_size=z* 
+00002160: 6973 2062 656c 6f77 207a 6572 6f21 2028  is below zero! (
+00002170: 4465 6372 6561 7365 2076 616c 6964 6174  Decrease validat
+00002180: 696f 6e5f 7369 7a65 3d7a 1220 616e 642f  ion_size=z. and/
+00002190: 6f72 2074 6573 745f 7369 7a65 3dfa 0129  or test_size=..)
+000021a0: 2905 728d 0000 0072 8e00 0000 728f 0000  ).r....r....r...
+000021b0: 0072 9000 0000 7291 0000 0029 01da 0564  .r....r....)...d
+000021c0: 7479 7065 2901 da05 696e 6465 7829 0b72  type)...index).r
+000021d0: 2c00 0000 7254 0000 00da 0c6c 6f61 645f  ,...rT.....load_
+000021e0: 6461 7461 7365 74da 1672 6573 6574 5f69  dataset..reset_i
+000021f0: 6e64 6578 5f63 6f6f 7264 696e 6174 65da  ndex_coordinate.
+00002200: 0463 6f70 79da 0a56 616c 7565 4572 726f  .copy..ValueErro
+00002210: 7272 9f00 0000 7298 0000 00da 0561 7272  rr....r......arr
+00002220: 6179 7219 0000 00da 0373 656c 290a 728d  ayr......sel).r.
+00002230: 0000 0072 8e00 0000 72a0 0000 0072 8f00  ...r....r....r..
+00002240: 0000 7290 0000 0072 9100 0000 da0a 7472  ..r....r......tr
+00002250: 6169 6e5f 7369 7a65 729d 0000 0072 9e00  ain_sizer....r..
+00002260: 0000 da10 696e 6469 6365 735f 7661 6c69  ....indices_vali
+00002270: 6461 7465 721b 0000 0072 1b00 0000 721c  dater....r....r.
+00002280: 0000 00da 1a73 706c 6974 5f74 7261 696e  .....split_train
+00002290: 696e 675f 7365 745f 7472 6970 706c 6522  ing_set_tripple"
+000022a0: 0100 0073 2e00 0000 1219 0801 0801 0801  ...s............
+000022b0: 0801 1c01 0201 0201 0201 0201 0201 0201  ................
+000022c0: 0afb 0e07 0801 0201 0a01 0201 0a01 0201  ................
+000022d0: 0201 0afb 0a07 72ac 0000 0072 0c00 0000  ......r....r....
+000022e0: 725e 0000 0072 5f00 0000 725c 0000 0072  r^...r_...r\...r
+000022f0: 5d00 0000 6304 0000 0000 0000 0000 0000  ]...c...........
+00002300: 0004 0000 000b 0000 0043 0000 0073 bc00  .........C...s..
+00002310: 0000 7400 a001 6401 7c01 9b02 6402 7c02  ..t...d.|...d.|.
+00002320: 9b02 6403 7c03 9b02 6404 7c00 9b02 6405  ..d.|...d.|...d.
+00002330: 9d09 a101 0100 7c01 6400 7500 721e 7402  ......|.d.u.r.t.
+00002340: 6406 7c01 9b02 6407 9d03 8301 8201 7c00  d.|...d.......|.
+00002350: 6408 6b02 7223 6e18 7c00 6409 6b02 722e  d.k.r#n.|.d.k.r.
+00002360: 7c01 6400 7501 722d 7c01 7d03 6e0d 7c00  |.d.u.r-|.}.n.|.
+00002370: 640a 6b02 7233 6e08 7402 640b 7c00 9b02  d.k.r3n.t.d.|...
+00002380: 640c 9d03 8301 8201 7c02 6400 7500 7241  d.......|.d.u.rA
+00002390: 7c01 7d02 7c03 6400 7500 7247 7c01 7d03  |.}.|.d.u.rG|.}.
+000023a0: 7400 a001 640d 7c01 9b02 6402 7c02 9b02  t...d.|...d.|...
+000023b0: 6403 7c03 9b02 6404 7c00 9b02 6405 9d09  d.|...d.|...d...
+000023c0: a101 0100 7c01 7c03 7c02 6603 5300 290e  ....|.|.|.f.S.).
+000023d0: 4e7a 1855 7365 7220 6368 6f69 6365 3a20  Nz.User choice: 
+000023e0: 6576 616c 5f73 7465 7073 3d7a 0f20 6c6f  eval_steps=z. lo
+000023f0: 6767 696e 675f 7374 6570 733d 7a0c 2073  gging_steps=z. s
+00002400: 6176 655f 7374 6570 733d 7a17 2c20 2865  ave_steps=z., (e
+00002410: 7661 6c75 6174 696f 6e5f 7374 7261 7465  valuation_strate
+00002420: 6779 3d72 a100 0000 7a0b 6576 616c 5f73  gy=r....z.eval_s
+00002430: 7465 7073 3d7a 1020 6361 6e6e 6f74 2062  teps=z. cannot b
+00002440: 6520 4e6f 6e65 2172 5300 0000 7251 0000  e None!rS...rQ..
+00002450: 00da 026e 6f7a 1465 7661 6c75 6174 696f  ...noz.evaluatio
+00002460: 6e5f 7374 7261 7465 6779 3d7a 0b20 6e6f  n_strategy=z. no
+00002470: 7420 6b6e 6f77 6e21 7a14 5365 7474 696e  t known!z.Settin
+00002480: 673a 2065 7661 6c5f 7374 6570 733d 2903  g: eval_steps=).
+00002490: 726f 0000 0072 7000 0000 72a7 0000 0072  ro...rp...r....r
+000024a0: 6200 0000 721b 0000 0072 1b00 0000 721c  b...r....r....r.
+000024b0: 0000 0072 7100 0000 5401 0000 7324 0000  ...rq...T...s$..
+000024c0: 0024 0308 0110 0108 0102 0208 0108 0104  .$..............
+000024d0: 0102 8008 0102 0110 0208 0104 0108 0104  ................
+000024e0: 0124 010a 0172 7100 0000 2901 7222 0000  .$...rq...).r"..
+000024f0: 0029 0472 2200 0000 728b 0000 0072 8c00  .).r"...r....r..
+00002500: 0000 5429 0572 2200 0000 4e72 8b00 0000  ..T).r"...Nr....
+00002510: 728c 0000 0054 2903 720c 0000 004e 4e29  r....T).r....NN)
+00002520: 20da 0b64 6174 6163 6c61 7373 6573 7273   ..dataclassesrs
+00002530: 0000 0072 6f00 0000 da06 7479 7069 6e67  ...ro.....typing
+00002540: 7279 0000 00da 0a61 322e 6461 7461 7365  ry.....a2.datase
+00002550: 7472 2c00 0000 da14 6132 2e70 6c6f 7474  tr,.....a2.plott
+00002560: 696e 672e 616e 616c 7973 6973 da14 6132  ing.analysis..a2
+00002570: 2e74 7261 696e 696e 672e 7472 6163 6b69  .training.tracki
+00002580: 6e67 da1a 6132 2e74 7261 696e 696e 672e  ng..a2.training.
+00002590: 7574 696c 735f 7472 6169 6e69 6e67 727f  utils_trainingr.
+000025a0: 0000 00da 056e 756d 7079 7298 0000 00da  .....numpyr.....
+000025b0: 1773 6b6c 6561 726e 2e6d 6f64 656c 5f73  .sklearn.model_s
+000025c0: 656c 6563 7469 6f6e 7295 0000 0072 3b00  electionr....r;.
+000025d0: 0000 da06 7861 7272 6179 da09 6461 7461  ....xarray..data
+000025e0: 636c 6173 7372 0200 0000 721e 0000 0072  classr....r....r
+000025f0: 2100 0000 7235 0000 0072 3600 0000 7275  !...r5...r6...ru
+00002600: 0000 0072 8000 0000 721a 0000 0072 1700  ...r....r....r..
+00002610: 0000 7219 0000 0072 7c00 0000 729f 0000  ..r....r|...r...
+00002620: 0072 ac00 0000 7271 0000 0072 1b00 0000  .r....rq...r....
+00002630: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
+00002640: 083c 6d6f 6475 6c65 3e01 0000 0073 8400  .<module>....s..
+00002650: 0000 0800 0801 0801 0801 0802 0801 0801  ................
+00002660: 0801 0801 0801 0801 0801 0801 0403 1001  ................
+00002670: 0410 1201 0407 1201 0a07 0e22 007f 081d  ..........."....
+00002680: 020e 0201 0201 0201 04fb 0401 02ff 0202  ................
+00002690: 02fe 0203 02fd 0204 02fc 0205 0afb 0228  ...............(
+000026a0: 0201 0201 0201 0201 04fa 0401 02ff 0202  ................
+000026b0: 02fe 0603 02fd 0204 02fc 0205 02fb 0206  ................
+000026c0: 0afa 0233 04ff 0201 02ff 0201 02ff 0601  ...3............
+000026d0: 02ff 0601 0eff                           ......
```

### Comparing `a2-0.4.0/src/a2/training/__pycache__/training_performance.cpython-310.pyc` & `a2-0.4.1/src/a2/training/__pycache__/training_performance.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/training/benchmarks.py` & `a2-0.4.1/src/a2/training/benchmarks.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/training/dataset_hugging.py` & `a2-0.4.1/src/a2/training/dataset_hugging.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/training/evaluate_hugging.py` & `a2-0.4.1/src/a2/training/evaluate_hugging.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/training/tracking.py` & `a2-0.4.1/src/a2/training/tracking.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/training/tracking_hugging.py` & `a2-0.4.1/src/a2/training/tracking_hugging.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/training/training_deep500.py` & `a2-0.4.1/src/a2/training/training_deep500.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/training/training_hugging.py` & `a2-0.4.1/src/a2/training/training_hugging.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import numpy as np
 import sklearn.model_selection
 import transformers
 import xarray
 
 
 @dataclasses.dataclass
-class HyperParametersDebertaClassifier:
+class HyperParametersHuggingFaceClassifier:
     """
     Hold hyper parameters for Hugging Face DeBERTa classifier
     """
 
     learning_rate: float = 3e-05
     batch_size: int = 32
     weight_decay: float = 0.01
@@ -28,14 +28,32 @@
     warmup_steps: float = 500  # 0
     hidden_dropout_prob: float = 0.1
     attention_probs_dropout_prob: float = 0.1
     cls_dropout: float = 0.1
     lr_scheduler_type: str = "linear"
 
 
+@dataclasses.dataclass
+class HyperParametersDebertaClassifier(HyperParametersHuggingFaceClassifier):
+    """
+    Hold hyper parameters for Hugging Face DeBERTa classifier
+    """
+
+    learning_rate: float = 3e-05
+
+
+@dataclasses.dataclass
+class HyperParametersElectraClassifier(HyperParametersHuggingFaceClassifier):
+    """
+    Hold hyper parameters for Hugging Face DeBERTa classifier
+    """
+
+    learning_rate: float = 2e-5
+
+
 def _compute_metrics(eval_pred, label="raining"):
     """
     Adopt Hugging Face metric output to prefered metric
     (f1-score) for this project
 
     Parameters:
     ----------
```

### Comparing `a2-0.4.0/src/a2/training/training_performance.py` & `a2-0.4.1/src/a2/training/training_performance.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/twitter/__pycache__/downloader.cpython-310.pyc` & `a2-0.4.1/src/a2/twitter/__pycache__/downloader.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/twitter/__pycache__/locations.cpython-310.pyc` & `a2-0.4.1/src/a2/twitter/__pycache__/locations.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/twitter/__pycache__/manipulate_tweets.cpython-310.pyc` & `a2-0.4.1/src/a2/twitter/__pycache__/manipulate_tweets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/twitter/__pycache__/twitter_api.cpython-310.pyc` & `a2-0.4.1/src/a2/twitter/__pycache__/twitter_api.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/twitter/downloader.py` & `a2-0.4.1/src/a2/twitter/downloader.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/twitter/locations.py` & `a2-0.4.1/src/a2/twitter/locations.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/twitter/twitter_api.py` & `a2-0.4.1/src/a2/twitter/twitter_api.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/utils/__pycache__/argparse.cpython-310.pyc` & `a2-0.4.1/src/a2/utils/__pycache__/argparse.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 09:48:51 2023 UTC, .py size: 10625 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,590 +1,603 @@
-00000000: 6f0d 0d0a 0000 0000 03ea 8664 8129 0000  o..........d.)..
+00000000: 6f0d 0d0a 0000 0000 c130 8b64 772a 0000  o........0.dw*..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 e400 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 ec00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c02 5a03 6500 6a04 6601 6402 6403  d.l.Z.e.j.f.d.d.
-00000050: 8401 5a05 6404 6405 8400 5a06 6406 6407  ..Z.d.d...Z.d.d.
-00000060: 8400 5a07 6408 6409 8400 5a08 640a 640b  ..Z.d.d...Z.d.d.
-00000070: 8400 5a09 640c 640d 8400 5a0a 640e 640f  ..Z.d.d...Z.d.d.
-00000080: 8400 5a0b 6410 6411 8400 5a0c 6412 6413  ..Z.d.d...Z.d.d.
-00000090: 8400 5a0d 6414 6415 8400 5a0e 6416 6417  ..Z.d.d...Z.d.d.
-000000a0: 8400 5a0f 6418 6419 8400 5a10 641a 641b  ..Z.d.d...Z.d.d.
-000000b0: 8400 5a11 641c 641d 8400 5a12 641e 641f  ..Z.d.d...Z.d.d.
-000000c0: 8400 5a13 6420 6421 8400 5a14 6422 6423  ..Z.d d!..Z.d"d#
-000000d0: 8400 5a15 6424 6425 8400 5a16 6426 6427  ..Z.d$d%..Z.d&d'
-000000e0: 8400 5a17 6428 6429 8400 5a18 642a 642b  ..Z.d(d)..Z.d*d+
-000000f0: 8400 5a19 642c 642d 8400 5a1a 642e 651b  ..Z.d,d-..Z.d.e.
-00000100: 642f 651c 6604 6430 6431 8404 5a1d 6401  d/e.f.d0d1..Z.d.
-00000110: 5300 2932 e900 0000 004e 6301 0000 0000  S.)2.....Nc.....
-00000120: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
-00000130: 0000 0073 1000 0000 7400 6a01 7c00 6401  ...s....t.j.|.d.
-00000140: 8d01 7d01 7c01 5300 2902 4e29 01da 0f66  ..}.|.S.).N)...f
-00000150: 6f72 6d61 7474 6572 5f63 6c61 7373 2902  ormatter_class).
-00000160: da08 6172 6770 6172 7365 da0e 4172 6775  ..argparse..Argu
-00000170: 6d65 6e74 5061 7273 6572 2902 7202 0000  mentParser).r...
-00000180: 00da 0670 6172 7365 72a9 0072 0600 0000  ...parser..r....
-00000190: fa33 2f68 6f6d 652f 6b72 6973 7469 616e  .3/home/kristian
-000001a0: 2f50 726f 6a65 6374 732f 6132 2f73 7263  /Projects/a2/src
-000001b0: 2f61 322f 7574 696c 732f 6172 6770 6172  /a2/utils/argpar
-000001c0: 7365 2e70 79da 0a67 6574 5f70 6172 7365  se.py..get_parse
-000001d0: 7207 0000 0073 0400 0000 0c01 0401 7208  r....s........r.
-000001e0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-000001f0: 0100 0000 0700 0000 4300 0000 7324 0000  ........C...s$..
-00000200: 007c 006a 0064 0164 0274 0174 026a 036a  .|.j.d.d.t.t.j.j
-00000210: 04a0 05a1 0064 031b 0064 0464 058d 0501  .....d...d.d....
-00000220: 0064 0053 0029 064e 7a0c 2d2d 7477 6565  .d.S.).Nz.--twee
-00000230: 7473 5f64 6972 7a07 2d69 6e70 6174 687a  ts_dirz.-inpathz
-00000240: 0774 7765 6574 732f fa2e 4469 7265 6374  .tweets/..Direct
-00000250: 6f72 7920 7768 6572 6520 696e 7075 7420  ory where input 
-00000260: 6e65 7443 4446 2d66 696c 6573 2061 7265  netCDF-files are
-00000270: 2073 746f 7265 642e a903 da04 7479 7065   stored.....type
-00000280: da07 6465 6661 756c 74da 0468 656c 7029  ..default..help)
-00000290: 06da 0c61 6464 5f61 7267 756d 656e 74da  ...add_argument.
-000002a0: 0373 7472 da02 6132 da05 7574 696c 73da  .str..a2..utils.
-000002b0: 0d66 696c 655f 6861 6e64 6c69 6e67 da0f  .file_handling..
-000002c0: 6765 745f 666f 6c64 6572 5f64 6174 61a9  get_folder_data.
-000002d0: 0172 0500 0000 7206 0000 0072 0600 0000  .r....r....r....
-000002e0: 7207 0000 00da 0e64 6174 6173 6574 5f74  r......dataset_t
-000002f0: 7765 6574 730c 0000 0073 0e00 0000 0401  weets....s......
-00000300: 0201 0201 0201 0e01 0201 0afb 7215 0000  ............r...
-00000310: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-00000320: 0000 0700 0000 4300 0000 732a 0000 007c  ......C...s*...|
-00000330: 006a 0064 0174 0164 0264 0364 048d 0401  .j.d.t.d.d.d....
-00000340: 007c 006a 0064 0564 0674 0164 0764 0864  .|.j.d.d.t.d.d.d
-00000350: 048d 0501 0064 0053 0029 094e 7a10 2d2d  .....d.S.).Nz.--
-00000360: 6461 7461 7365 745f 7072 6566 6978 da86  dataset_prefix..
-00000370: 3230 3230 5f74 7765 6574 735f 7261 696e  2020_tweets_rain
-00000380: 5f73 756e 5f76 6f63 6162 5f65 6d6f 6a69  _sun_vocab_emoji
-00000390: 735f 6c6f 6361 7469 6f6e 735f 6262 615f  s_locations_bba_
-000003a0: 5470 5f65 7261 355f 6e6f 5f62 6f74 735f  Tp_era5_no_bots_
-000003b0: 6e6f 726d 616c 697a 6564 5f66 696c 7465  normalized_filte
-000003c0: 7265 645f 7765 6174 6865 725f 7374 6174  red_weather_stat
-000003d0: 696f 6e73 5f66 6978 5f70 7265 6469 6374  ions_fix_predict
-000003e0: 6564 5f73 696d 706c 6564 6562 6572 7461  ed_simpledeberta
-000003f0: 5f72 6164 6172 7a32 4461 7461 7365 7420  _radarz2Dataset 
-00000400: 7072 6566 6978 2064 6574 6572 6d69 6e65  prefix determine
-00000410: 6420 6475 7269 6e67 2073 706c 6974 206f  d during split o
-00000420: 6620 6461 7461 7365 742e 720a 0000 007a  f dataset.r....z
-00000430: 122d 2d64 6174 615f 6465 7363 7269 7074  .--data_descript
-00000440: 696f 6e7a 062d 6461 7461 647a 3f74 7765  ionz.-datadz?twe
-00000450: 6574 7320 3230 3137 2d32 3032 302c 206b  ets 2017-2020, k
-00000460: 6579 776f 7264 7320 656d 6f6a 6973 2061  eywords emojis a
-00000470: 7320 6465 7363 7269 7074 696f 6e2c 206b  s description, k
-00000480: 6579 776f 7264 7320 6f6e 6c79 7a29 4461  eywords onlyz)Da
-00000490: 7461 2064 6573 6372 6970 7469 6f6e 2070  ta description p
-000004a0: 7572 656c 7920 7573 6564 2066 6f72 206c  urely used for l
-000004b0: 6f67 6769 6e67 2ea9 0272 0e00 0000 720f  ogging...r....r.
-000004c0: 0000 0072 1400 0000 7206 0000 0072 0600  ...r....r....r..
-000004d0: 0000 7207 0000 00da 0764 6174 6173 6574  ..r......dataset
-000004e0: 1600 0000 731a 0000 0004 0102 0102 0102  ....s...........
-000004f0: 0102 0106 fc04 0602 0102 0102 0102 0102  ................
-00000500: 010a fb72 1800 0000 6301 0000 0000 0000  ...r....c.......
-00000510: 0000 0000 0001 0000 0007 0000 0043 0000  .............C..
-00000520: 0073 2c00 0000 7c00 6a00 6401 6402 7401  .s,...|.j.d.d.t.
-00000530: 6403 6404 6405 8d05 0100 7c00 6a00 6406  d.d.d.....|.j.d.
-00000540: 6407 7402 6400 6408 6405 8d05 0100 6400  d.t.d.d.d.....d.
-00000550: 5300 2909 4e7a 152d 2d65 7661 6c75 6174  S.).Nz.--evaluat
-00000560: 696f 6e5f 7374 7261 7465 6779 7a07 2d65  ion_strategyz.-e
-00000570: 7374 7261 74da 0565 706f 6368 7a1f 5768  strat..epochz.Wh
-00000580: 656e 2074 6f20 6576 616c 7561 7465 2073  en to evaluate s
-00000590: 7465 7073 2f65 706f 6368 2f6e 6f72 0a00  teps/epoch/nor..
-000005a0: 0000 7a0c 2d2d 6576 616c 5f73 7465 7073  ..z.--eval_steps
-000005b0: 7a07 2d65 7374 6570 737a 4b4e 756d 6265  z.-estepszKNumbe
-000005c0: 7220 6f66 2073 7465 7073 2062 6574 7765  r of steps betwe
-000005d0: 656e 2065 7661 6c75 6174 696f 6e73 2069  en evaluations i
-000005e0: 6620 6576 616c 7561 7469 6f6e 2073 7472  f evaluation str
-000005f0: 6174 6567 7920 6973 2073 6574 2074 6f20  ategy is set to 
-00000600: 7374 6570 732e 2903 720e 0000 0072 0f00  steps.).r....r..
-00000610: 0000 da03 696e 7472 1400 0000 7206 0000  ....intr....r...
-00000620: 0072 0600 0000 7207 0000 00da 0a65 7661  .r....r......eva
-00000630: 6c75 6174 696f 6e26 0000 0073 1400 0000  luation&...s....
-00000640: 0401 0a01 06ff 0403 0201 0201 0201 0201  ................
-00000650: 0201 0afb 721b 0000 0063 0100 0000 0000  ....r....c......
-00000660: 0000 0000 0000 0100 0000 0700 0000 4300  ..............C.
-00000670: 0000 735c 0000 007c 006a 0064 0174 0164  ..s\...|.j.d.t.d
-00000680: 0264 0364 048d 0401 007c 006a 0064 0564  .d.d.....|.j.d.d
-00000690: 0664 0767 0274 0164 0864 0964 0a8d 0501  .d.g.t.d.d.d....
-000006a0: 007c 006a 0064 0b74 0164 0c64 0c67 0164  .|.j.d.t.d.d.g.d
-000006b0: 0d64 0e8d 0501 007c 006a 0064 0f74 0164  .d.....|.j.d.t.d
-000006c0: 1067 0064 11a2 0164 1264 0e8d 0501 0064  .g.d...d.d.....d
-000006d0: 0053 0029 134e 7a0a 2d2d 6b65 795f 7465  .S.).Nz.--key_te
-000006e0: 7874 da0f 7465 7874 5f6e 6f72 6d61 6c69  xt..text_normali
-000006f0: 7a65 647a 1b4b 6579 2066 6f72 2074 6578  zedz.Key for tex
-00000700: 7420 696e 2069 6e70 7574 2066 696c 652e  t in input file.
-00000710: 720a 0000 007a 132d 2d63 6c61 7373 6966  r....z.--classif
-00000720: 6965 725f 646f 6d61 696e da04 7261 696e  ier_domain..rain
-00000730: da09 7265 6c65 7661 6e63 6554 7a14 446f  ..relevanceTz.Do
-00000740: 6d61 696e 206f 6620 636c 6173 7369 6669  main of classifi
-00000750: 6572 2904 da07 6368 6f69 6365 7372 0b00  er)...choicesr..
-00000760: 0000 da08 7265 7175 6972 6564 720d 0000  ....requiredr...
-00000770: 007a 0b2d 2d6b 6579 5f69 6e70 7574 da04  .z.--key_input..
-00000780: 7465 7874 7a3f 436f 6c75 6d6e 206e 616d  textz?Column nam
-00000790: 6520 6f66 2064 6174 6173 6574 2074 6861  e of dataset tha
-000007a0: 7420 636f 7272 6573 706f 6e64 7320 746f  t corresponds to
-000007b0: 2069 6e70 7574 206f 6620 636c 6173 7369   input of classi
-000007c0: 6669 6572 2e29 0472 0b00 0000 720c 0000  fier.).r....r...
-000007d0: 0072 1f00 0000 720d 0000 007a 0c2d 2d6b  .r....r....z.--k
-000007e0: 6579 5f6f 7574 7075 74da 0772 6169 6e69  ey_output..raini
-000007f0: 6e67 2903 7222 0000 00da 0872 656c 6576  ng).r".....relev
-00000800: 616e 74da 0f72 6169 6e69 6e67 5f73 7461  ant..raining_sta
-00000810: 7469 6f6e 7a40 436f 6c75 6d6e 206e 616d  tionz@Column nam
-00000820: 6520 6f66 2064 6174 6173 6574 2074 6861  e of dataset tha
-00000830: 7420 636f 7272 6573 706f 6e64 7320 746f  t corresponds to
-00000840: 206f 7574 7075 7420 6f66 2063 6c61 7373   output of class
-00000850: 6966 6965 722e 7217 0000 0072 1400 0000  ifier.r....r....
-00000860: 7206 0000 0072 0600 0000 7207 0000 00da  r....r....r.....
-00000870: 0a63 6c61 7373 6966 6965 7233 0000 0073  .classifier3...s
-00000880: 2400 0000 1201 0401 0e01 06ff 0403 0201  $...............
-00000890: 0201 0201 0401 0201 06fb 0407 0201 0201  ................
-000008a0: 0201 0601 0201 0afb 7225 0000 0063 0100  ........r%...c..
-000008b0: 0000 0000 0000 0000 0000 0100 0000 0600  ................
-000008c0: 0000 4300 0000 733a 0000 007c 006a 0064  ..C...s:...|.j.d
-000008d0: 0164 0274 0164 0364 048d 0401 007c 006a  .d.t.d.d.....|.j
-000008e0: 0064 0564 0274 0164 0664 048d 0401 007c  .d.d.t.d.d.....|
-000008f0: 006a 0064 0764 0274 0164 0864 048d 0401  .j.d.d.t.d.d....
-00000900: 0064 0053 0029 094e 7a18 2d2d 6669 6c65  .d.S.).Nz.--file
-00000910: 6e61 6d65 5f64 6174 6173 6574 5f74 7261  name_dataset_tra
-00000920: 696e 547a 2646 696c 656e 616d 6520 6f66  inTz&Filename of
-00000930: 2064 6174 6173 6574 2075 7365 6420 666f   dataset used fo
-00000940: 7220 7472 6169 6e69 6e67 2ea9 0372 2000  r training...r .
-00000950: 0000 720b 0000 0072 0d00 0000 7a1b 2d2d  ..r....r....z.--
-00000960: 6669 6c65 6e61 6d65 5f64 6174 6173 6574  filename_dataset
-00000970: 5f76 616c 6964 6174 657a 2846 696c 656e  _validatez(Filen
-00000980: 616d 6520 6f66 2064 6174 6173 6574 2075  ame of dataset u
-00000990: 7365 6420 666f 7220 7661 6c69 6461 7469  sed for validati
-000009a0: 6f6e 2e7a 172d 2d66 696c 656e 616d 655f  on.z.--filename_
-000009b0: 6461 7461 7365 745f 7465 7374 7a25 4669  dataset_testz%Fi
-000009c0: 6c65 6e61 6d65 206f 6620 6461 7461 7365  lename of datase
-000009d0: 7420 7573 6564 2066 6f72 2074 6573 7469  t used for testi
-000009e0: 6e67 2e72 1700 0000 7214 0000 0072 0600  ng.r....r....r..
-000009f0: 0000 7206 0000 0072 0700 0000 da10 6461  ..r....r......da
-00000a00: 7461 7365 745f 7472 6169 6e69 6e67 4800  taset_trainingH.
-00000a10: 0000 7312 0000 0004 0108 0106 ff04 0308  ..s.............
-00000a20: 0106 ff04 0308 010a ff72 2700 0000 6301  .........r'...c.
-00000a30: 0000 0000 0000 0000 0000 0001 0000 0006  ................
-00000a40: 0000 0043 0000 0073 2800 0000 7c00 6a00  ...C...s(...|.j.
-00000a50: 6401 7401 6402 6403 6404 8d04 0100 7c00  d.t.d.d.d.....|.
-00000a60: 6a00 6405 7401 6406 6407 6408 8d04 0100  j.d.t.d.d.d.....
-00000a70: 6400 5300 2909 4e7a 0c2d 2d6f 7574 7075  d.S.).Nz.--outpu
-00000a80: 745f 6469 727a 076f 7574 7075 742f 7a17  t_dirz.output/z.
-00000a90: 466f 6c64 6572 2074 6f20 7361 7665 2072  Folder to save r
-00000aa0: 6573 756c 7473 2e72 0a00 0000 7a0b 2d2d  esults.r....z.--
-00000ab0: 7461 736b 5f6e 616d 6554 7a43 4e61 6d65  task_nameTzCName
-00000ac0: 206f 6620 7461 736b 2c20 7265 7375 6c74   of task, result
-00000ad0: 7320 7769 6c6c 2062 6520 7361 7665 6420  s will be saved 
-00000ae0: 696e 2074 6869 7320 7375 6264 6972 6563  in this subdirec
-00000af0: 746f 7279 206f 6620 6f75 7470 7574 2ea9  tory of output..
-00000b00: 0372 0b00 0000 7220 0000 0072 0d00 0000  .r....r ...r....
-00000b10: 7217 0000 0072 1400 0000 7206 0000 0072  r....r....r....r
-00000b20: 0600 0000 7207 0000 00da 066f 7574 7075  ....r......outpu
-00000b30: 7454 0000 0073 1800 0000 0401 0201 0201  tT...s..........
-00000b40: 0201 0201 06fc 0406 0201 0201 0201 0201  ................
-00000b50: 0afc 7229 0000 0063 0100 0000 0000 0000  ..r)...c........
-00000b60: 0000 0000 0100 0000 0600 0000 4300 0000  ............C...
-00000b70: 7328 0000 007c 006a 0064 0174 0164 0264  s(...|.j.d.t.d.d
-00000b80: 0364 048d 0401 007c 006a 0064 0574 0264  .d.....|.j.d.t.d
-00000b90: 0664 0764 048d 0401 0064 0053 0029 084e  .d.d.....d.S.).N
-00000ba0: 7a0a 2d2d 6b65 795f 7261 696e da04 7470  z.--key_rain..tp
-00000bb0: 5f68 7a20 4b65 7920 666f 7220 7261 696e  _hz Key for rain
-00000bc0: 2064 6174 6120 696e 2069 6e70 7574 2066   data in input f
-00000bd0: 696c 652e 720a 0000 007a 102d 2d74 6872  ile.r....z.--thr
-00000be0: 6573 686f 6c64 5f72 6169 6e67 3a8c 30e2  eshold_raing:.0.
-00000bf0: 8e79 453e 7a48 5468 7265 7368 6f6c 6420  .yE>zHThreshold 
-00000c00: 6162 6f76 6520 7768 6963 6820 7072 6563  above which prec
-00000c10: 6970 6974 6174 696f 6e20 6973 2063 6f6e  ipitation is con
-00000c20: 7369 6465 7265 6420 7261 696e 696e 6720  sidered raining 
-00000c30: 696e 2069 6e70 7574 2066 696c 652e 2903  in input file.).
-00000c40: 720e 0000 0072 0f00 0000 da05 666c 6f61  r....r......floa
-00000c50: 7472 1400 0000 7206 0000 0072 0600 0000  tr....r....r....
-00000c60: 7207 0000 00da 0c64 6174 6173 6574 5f72  r......dataset_r
-00000c70: 6169 6e63 0000 0073 0e00 0000 1201 0401  ainc...s........
-00000c80: 0201 0201 0201 0201 0afc 722c 0000 0063  ..........r,...c
-00000c90: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000ca0: 0600 0000 4300 0000 f316 0000 007c 006a  ....C........|.j
-00000cb0: 0064 0174 0164 0264 0364 048d 0401 0064  .d.t.d.d.d.....d
-00000cc0: 0053 0029 054e 7a0f 2d2d 6b65 795f 7265  .S.).Nz.--key_re
-00000cd0: 6c65 7661 6e63 6572 2300 0000 7a30 5661  levancer#...z0Va
-00000ce0: 7269 6162 6c65 206e 616d 6520 7468 6174  riable name that
-00000cf0: 2073 7065 6369 6669 6573 2072 656c 6576   specifies relev
-00000d00: 616e 6365 206f 6620 5477 6565 742e 720a  ance of Tweet.r.
-00000d10: 0000 0072 1700 0000 7214 0000 0072 0600  ...r....r....r..
-00000d20: 0000 7206 0000 0072 0700 0000 da11 6461  ..r....r......da
-00000d30: 7461 7365 745f 7265 6c65 7661 6e63 656d  taset_relevancem
-00000d40: 0000 00f3 0c00 0000 0401 0201 0201 0201  ................
-00000d50: 0201 0afc 722e 0000 0063 0100 0000 0000  ....r....c......
-00000d60: 0000 0000 0000 0100 0000 0700 0000 4300  ..............C.
-00000d70: 0000 73a8 0000 007c 006a 0064 0174 0164  ..s....|.j.d.t.d
-00000d80: 0264 0364 048d 0401 007c 006a 0064 0574  .d.d.....|.j.d.t
-00000d90: 0164 0264 0364 048d 0401 007c 006a 0064  .d.d.d.....|.j.d
-00000da0: 0674 0264 0764 0864 048d 0401 007c 006a  .t.d.d.d.....|.j
-00000db0: 0064 0974 0164 0a64 0b64 048d 0401 007c  .d.t.d.d.d.....|
-00000dc0: 006a 0064 0c64 0d74 0364 0e64 0f64 048d  .j.d.d.t.d.d.d..
-00000dd0: 0501 007c 006a 0064 1074 0164 1164 1264  ...|.j.d.t.d.d.d
-00000de0: 048d 0401 007c 006a 0064 1374 0164 1464  .....|.j.d.t.d.d
-00000df0: 1564 048d 0401 007c 006a 0064 1674 0164  .d.....|.j.d.t.d
-00000e00: 1764 1864 048d 0401 007c 006a 0064 1974  .d.d.....|.j.d.t
-00000e10: 0164 1a64 1b64 048d 0401 0064 0053 0029  .d.d.d.....d.S.)
-00000e20: 1c4e 7a1f 2d2d 6669 6c65 6e61 6d65 5f74  .Nz.--filename_t
-00000e30: 7765 6574 735f 7769 7468 5f6b 6579 776f  weets_with_keywo
-00000e40: 7264 737a 5b32 3031 375f 3230 3230 5f74  rdsz[2017_2020_t
-00000e50: 7765 6574 735f 7261 696e 5f73 756e 5f76  weets_rain_sun_v
-00000e60: 6f63 6162 5f65 6d6f 6a69 735f 6c6f 6361  ocab_emojis_loca
-00000e70: 7469 6f6e 735f 6262 615f 5470 5f65 7261  tions_bba_Tp_era
-00000e80: 355f 6e6f 5f62 6f74 735f 6e6f 726d 616c  5_no_bots_normal
-00000e90: 697a 6564 5f66 696c 7465 7265 642e 6e63  ized_filtered.nc
-00000ea0: 7a1a 4669 6c65 6e61 6d65 206f 6620 7472  z.Filename of tr
-00000eb0: 6169 6e69 6e67 2064 6174 612e 720a 0000  aining data.r...
-00000ec0: 007a 1a2d 2d64 6174 615f 6669 6c65 6e61  .z.--data_filena
-00000ed0: 6d65 5f69 7272 656c 6576 616e 747a 152d  me_irrelevantz.-
-00000ee0: 2d6e 5f74 7765 6574 735f 6972 7265 6c65  -n_tweets_irrele
-00000ef0: 7661 6e74 e9ff ffff ff7a 744e 756d 6265  vant.....ztNumbe
-00000f00: 7220 6f66 2069 7272 656c 6576 616e 7420  r of irrelevant 
-00000f10: 7477 6565 7473 2075 7365 6420 746f 2063  tweets used to c
-00000f20: 7265 6174 6520 6461 7461 7365 742c 2075  reate dataset, u
-00000f30: 7365 2061 6c6c 2069 7272 656c 6576 616e  se all irrelevan
-00000f40: 7420 7477 6565 7473 2062 7920 6465 6661  t tweets by defa
-00000f50: 756c 7420 2860 6e5f 7477 6565 7473 5f69  ult (`n_tweets_i
-00000f60: 7272 656c 6576 616e 743d 2d31 6029 2e7a  rrelevant=-1`).z
-00000f70: 0b2d 2d73 706c 6974 5f64 6972 da0f 7370  .--split_dir..sp
-00000f80: 6c69 745f 7265 6c65 7661 6e63 657a 1e46  lit_relevancez.F
-00000f90: 6f6c 6465 7220 746f 2073 6176 6520 7370  older to save sp
-00000fa0: 6c69 7420 6461 7461 7365 7473 2e7a 142d  lit datasets.z.-
-00000fb0: 2d6b 6d73 5f77 6974 6869 6e5f 7374 6174  -kms_within_stat
-00000fc0: 696f 6e7a 042d 6b6d 73e9 0100 0000 7a44  ionz.-kms.....zD
-00000fd0: 4469 7374 616e 6365 2074 6f20 7765 6174  Distance to weat
-00000fe0: 6865 7220 7374 6174 696f 6e2e 2055 7365  her station. Use
-00000ff0: 6420 746f 2063 7265 6174 6520 7765 6174  d to create weat
-00001000: 6865 7220 7374 6174 696f 6e20 6461 7461  her station data
-00001010: 7365 742e 7a1e 2d2d 6b65 795f 6469 7374  set.z.--key_dist
-00001020: 616e 6365 5f77 6561 7468 6572 5f73 7461  ance_weather_sta
-00001030: 7469 6f6e da13 7374 6174 696f 6e5f 6469  tion..station_di
-00001040: 7374 616e 6365 5f6b 6d7a 5e4b 6579 2069  stance_kmz^Key i
-00001050: 6e20 6461 7461 7365 7420 7468 6174 2073  n dataset that s
-00001060: 686f 7773 2064 6973 7461 6e63 6520 746f  hows distance to
-00001070: 2077 6561 7468 6572 2073 7461 7469 6f6e   weather station
-00001080: 2e20 5573 6564 2074 6f20 6372 6561 7465  . Used to create
-00001090: 2077 6561 7468 6572 2073 7461 7469 6f6e   weather station
-000010a0: 2064 6174 6173 6574 2e7a 202d 2d77 6561   dataset.z --wea
-000010b0: 7468 6572 5f73 7461 7469 6f6e 5f64 6174  ther_station_dat
-000010c0: 6173 6574 5f70 7265 6669 78da 1557 6561  aset_prefix..Wea
-000010d0: 7468 6572 5374 6174 696f 6e44 6174 6173  therStationDatas
-000010e0: 6574 7a22 5072 6566 6978 206f 6620 7765  etz"Prefix of we
-000010f0: 6174 6865 7220 7374 6174 696f 6e20 6461  ather station da
-00001100: 7461 7365 742e 7a23 2d2d 7261 696e 696e  taset.z#--rainin
-00001110: 675f 636c 6173 7369 6669 6572 5f64 6174  g_classifier_dat
-00001120: 6173 6574 5f70 7265 6669 78da 1852 6169  aset_prefix..Rai
-00001130: 6e69 6e67 436c 6173 7369 6669 6572 4461  ningClassifierDa
-00001140: 7461 7365 747a 2550 7265 6669 7820 6f66  tasetz%Prefix of
-00001150: 2072 6169 6e69 6e67 2063 6c61 7373 6966   raining classif
-00001160: 6965 7220 6461 7461 7365 742e 7a25 2d2d  ier dataset.z%--
-00001170: 7265 6c65 7661 6e63 655f 636c 6173 7369  relevance_classi
-00001180: 6669 6572 5f64 6174 6173 6574 5f70 7265  fier_dataset_pre
-00001190: 6669 78da 1a52 656c 6576 616e 6365 436c  fix..RelevanceCl
-000011a0: 6173 7369 6669 6572 4461 7461 7365 747a  assifierDatasetz
-000011b0: 2750 7265 6669 7820 6f66 2072 656c 6576  'Prefix of relev
-000011c0: 616e 6365 2063 6c61 7373 6966 6965 7220  ance classifier 
-000011d0: 6461 7461 7365 742e 2904 720e 0000 0072  dataset.).r....r
-000011e0: 0f00 0000 721a 0000 0072 2b00 0000 7214  ....r....r+...r.
-000011f0: 0000 0072 0600 0000 7206 0000 0072 0700  ...r....r....r..
-00001200: 0000 da17 6461 7461 7365 745f 7265 6c65  ....dataset_rele
-00001210: 7661 6e63 655f 7370 6c69 7476 0000 0073  vance_splitv...s
-00001220: 6e00 0000 0401 0201 0201 0201 0201 06fc  n...............
-00001230: 0406 0201 0201 0201 0201 06fc 0406 0201  ................
-00001240: 0201 0201 0201 06fc 0407 0201 0201 0201  ................
-00001250: 0201 06fc 0406 0201 0201 0201 0201 0201  ................
-00001260: 06fb 0407 0201 0201 0201 0201 06fc 0406  ................
-00001270: 0201 0201 0201 0201 06fc 0406 0201 0201  ................
-00001280: 0201 0201 06fc 0406 0201 0201 0201 0201  ................
-00001290: 0afc 7237 0000 0063 0100 0000 0000 0000  ..r7...c........
-000012a0: 0000 0000 0100 0000 0700 0000 4300 0000  ............C...
-000012b0: 732c 0000 007c 006a 0064 0164 0274 0164  s,...|.j.d.d.t.d
-000012c0: 0364 0464 058d 0501 007c 006a 0064 0664  .d.d.....|.j.d.d
-000012d0: 0774 0164 0364 0864 058d 0501 0064 0053  .t.d.d.d.....d.S
-000012e0: 0029 094e 7a0b 2d2d 7465 7374 5f73 697a  .).Nz.--test_siz
-000012f0: 657a 032d 7473 679a 9999 9999 99c9 3f7a  ez.-tsg.......?z
-00001300: 1546 7261 6374 696f 6e20 6f66 2074 6573  .Fraction of tes
-00001310: 7420 7365 742e 720a 0000 007a 112d 2d76  t set.r....z.--v
-00001320: 616c 6964 6174 696f 6e5f 7369 7a65 7a03  alidation_sizez.
-00001330: 2d76 737a 1b46 7261 6374 696f 6e20 6f66  -vsz.Fraction of
-00001340: 2076 616c 6964 6174 696f 6e20 7365 742e   validation set.
-00001350: 2902 720e 0000 0072 2b00 0000 7214 0000  ).r....r+...r...
-00001360: 0072 0600 0000 7206 0000 0072 0700 0000  .r....r....r....
-00001370: da13 6461 7461 7365 745f 7370 6c69 745f  ..dataset_split_
-00001380: 7369 7a65 73b1 0000 0073 0400 0000 1401  sizes....s......
-00001390: 1801 7238 0000 0063 0100 0000 0000 0000  ..r8...c........
-000013a0: 0000 0000 0100 0000 0600 0000 4300 0000  ............C...
-000013b0: 7332 0000 0074 007c 0083 0101 007c 006a  s2...t.|.....|.j
-000013c0: 0164 0164 0274 026a 0364 0364 048d 0401  .d.d.t.j.d.d....
-000013d0: 007c 006a 0164 0574 0464 0064 0664 078d  .|.j.d.t.d.d.d..
-000013e0: 0401 0064 0053 0029 084e 7a1b 2d2d 6669  ...d.S.).Nz.--fi
-000013f0: 6c65 6e61 6d65 5f64 6174 6173 6574 5f74  lename_dataset_t
-00001400: 6f5f 7370 6c69 7454 7a27 4669 6c65 6e61  o_splitTz'Filena
-00001410: 6d65 206f 6620 6461 7461 7365 7420 7468  me of dataset th
-00001420: 6174 2077 696c 6c20 6265 2073 706c 6974  at will be split
-00001430: 2e72 2600 0000 7a0e 2d2d 6b65 795f 7374  .r&...z.--key_st
-00001440: 7261 7469 6679 7a23 4b65 7920 7573 6564  ratifyz#Key used
-00001450: 2074 6f20 7374 7261 7469 6679 2064 6174   to stratify dat
-00001460: 6173 6574 2073 706c 6974 2e72 0a00 0000  aset split.r....
-00001470: 2905 7238 0000 0072 0e00 0000 da07 7061  ).r8...r......pa
-00001480: 7468 6c69 62da 0450 6174 6872 0f00 0000  thlib..Pathr....
-00001490: 7214 0000 0072 0600 0000 7206 0000 0072  r....r....r....r
-000014a0: 0700 0000 da0d 6461 7461 7365 745f 7370  ......dataset_sp
-000014b0: 6c69 74b6 0000 0073 1a00 0000 0801 0401  lit....s........
-000014c0: 0201 0201 0401 0201 06fc 0406 0201 0201  ................
-000014d0: 0201 0201 0afc 723b 0000 0063 0100 0000  ......r;...c....
-000014e0: 0000 0000 0000 0000 0100 0000 0600 0000  ................
-000014f0: 4300 0000 722d 0000 0029 054e 7a11 2d2d  C...r-...).Nz.--
-00001500: 7365 6c65 6374 5f72 656c 6576 616e 7454  select_relevantT
-00001510: 7a47 5768 6574 6865 7220 746f 206f 6e6c  zGWhether to onl
-00001520: 7920 7365 6c65 6374 2054 7765 6574 7320  y select Tweets 
-00001530: 6173 2072 6576 656c 616e 7420 2860 6172  as revelant (`ar
-00001540: 6773 2e6b 6579 5f72 656c 6576 616e 6365  gs.key_relevance
-00001550: 603d 3d54 7275 6529 2e72 0a00 0000 2902  `==True).r....).
-00001560: 720e 0000 00da 0e63 7573 746f 6d5f 626f  r......custom_bo
-00001570: 6f6c 6561 6e72 1400 0000 7206 0000 0072  oleanr....r....r
-00001580: 0600 0000 7207 0000 00da 0e64 6174 6173  ....r......datas
-00001590: 6574 5f73 656c 6563 74c6 0000 0072 2f00  et_select....r/.
-000015a0: 0000 723d 0000 0063 0100 0000 0000 0000  ..r=...c........
-000015b0: 0000 0000 0100 0000 0600 0000 4300 0000  ............C...
-000015c0: 733c 0000 007c 006a 0064 0164 0274 016a  s<...|.j.d.d.t.j
-000015d0: 0264 0364 048d 0401 007c 006a 0064 0574  .d.d.....|.j.d.t
-000015e0: 0364 0264 0664 078d 0401 007c 006a 0064  .d.d.d.....|.j.d
-000015f0: 0874 0364 0264 0964 078d 0401 0064 0053  .t.d.d.d.....d.S
-00001600: 0029 0a4e 7a1a 2d2d 6669 6c65 6e61 6d65  .).Nz.--filename
-00001610: 5f64 6174 6173 6574 5f70 7265 6469 6374  _dataset_predict
-00001620: 547a 3646 696c 656e 616d 6520 6f66 2064  Tz6Filename of d
-00001630: 6174 6173 6574 2074 6861 7420 7072 6564  ataset that pred
-00001640: 6963 7469 6f6e 7320 7769 6c6c 2062 6520  ictions will be 
-00001650: 6d61 6465 2066 6f72 2e72 2600 0000 7a10  made for.r&...z.
-00001660: 2d2d 7061 7468 5f72 6177 5f6d 6f64 656c  --path_raw_model
-00001670: 7a26 4469 7265 6374 6f72 7920 7768 6572  z&Directory wher
-00001680: 6520 756e 7472 6169 6e65 6420 6d6f 6465  e untrained mode
-00001690: 6c20 7361 7665 642e 7228 0000 007a 142d  l saved.r(...z.-
-000016a0: 2d70 6174 685f 7472 6169 6e65 645f 6d6f  -path_trained_mo
-000016b0: 6465 6c7a 2444 6972 6563 746f 7279 2077  delz$Directory w
-000016c0: 6865 7265 2074 7261 696e 6564 206d 6f64  here trained mod
-000016d0: 656c 2073 6176 6564 2e29 0472 0e00 0000  el saved.).r....
-000016e0: 7239 0000 0072 3a00 0000 720f 0000 0072  r9...r:...r....r
-000016f0: 1400 0000 7206 0000 0072 0600 0000 7207  ....r....r....r.
-00001700: 0000 00da 0d70 7265 6469 6374 5f6d 6f64  .....predict_mod
-00001710: 656c cf00 0000 7324 0000 0004 0102 0102  el....s$........
-00001720: 0104 0102 0106 fc04 0602 0102 0102 0102  ................
-00001730: 0106 fc04 0602 0102 0102 0102 010a fc72  ...............r
-00001740: 3e00 0000 6301 0000 0000 0000 0000 0000  >...c...........
-00001750: 0001 0000 0007 0000 0043 0000 0073 3400  .........C...s4.
-00001760: 0000 7c00 6a00 6401 6402 7401 6403 6404  ..|.j.d.d.t.d.d.
-00001770: 6405 8d05 0100 7c00 6a00 6406 6407 7401  d.....|.j.d.d.t.
-00001780: 7402 6a03 6a04 a005 a100 6408 6405 8d05  t.j.j.....d.d...
-00001790: 0100 6400 5300 2909 4e7a 0c2d 2d6d 6f64  ..d.S.).Nz.--mod
-000017a0: 656c 5f70 6174 687a 032d 696e 7a36 2f70  el_pathz.-inz6/p
-000017b0: 2f70 726f 6a65 6374 2f64 6565 7061 6366  /project/deepacf
-000017c0: 2f6d 6165 6c73 7472 6f6d 2f65 686c 6572  /maelstrom/ehler
-000017d0: 7431 2f64 6562 6572 7461 2d76 332d 736d  t1/deberta-v3-sm
-000017e0: 616c 6c2f 7209 0000 0072 0a00 0000 7a12  all/r....r....z.
-000017f0: 2d2d 6f75 7470 7574 5f64 6972 5f6d 6f64  --output_dir_mod
-00001800: 656c 7a07 2d6f 7574 6469 727a 264f 7574  elz.-outdirz&Out
-00001810: 7075 7420 6469 7265 6374 6f72 7920 7768  put directory wh
-00001820: 6572 6520 6d6f 6465 6c20 6973 2073 6176  ere model is sav
-00001830: 6564 2e29 0672 0e00 0000 720f 0000 0072  ed.).r....r....r
-00001840: 1000 0000 7211 0000 0072 1200 0000 da11  ....r....r......
-00001850: 6765 745f 666f 6c64 6572 5f6d 6f64 656c  get_folder_model
-00001860: 7372 1400 0000 7206 0000 0072 0600 0000  sr....r....r....
-00001870: 7207 0000 00da 056d 6f64 656c e400 0000  r......model....
-00001880: 731c 0000 0004 0102 0102 0102 0102 0102  s...............
-00001890: 0106 fb04 0702 0102 0102 010a 0102 010a  ................
-000018a0: fb72 4000 0000 6301 0000 0000 0000 0000  .r@...c.........
-000018b0: 0000 0001 0000 0006 0000 0043 0000 0072  ...........C...r
-000018c0: 2d00 0000 2905 4e7a 0c2d 2d72 756e 5f66  -...).Nz.--run_f
-000018d0: 6f6c 6465 7254 7a33 4f75 7470 7574 2066  olderTz3Output f
-000018e0: 6f6c 6465 7220 7768 6572 6520 6d6f 6465  older where mode
-000018f0: 6c20 6973 2073 6176 6564 2069 6e20 606f  l is saved in `o
-00001900: 7574 7075 745f 6469 7260 2e72 2800 0000  utput_dir`.r(...
-00001910: 7217 0000 0072 1400 0000 7206 0000 0072  r....r....r....r
-00001920: 0600 0000 7207 0000 00da 0372 756e f500  ....r......run..
-00001930: 0000 f306 0000 0004 0108 010a ff72 4100  .............rA.
-00001940: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-00001950: 0000 0006 0000 0043 0000 0073 3000 0000  .......C...s0...
-00001960: 7400 7c00 8301 0100 7c00 6a01 6401 7402  t.|.....|.j.d.t.
-00001970: 6402 6403 6404 8d04 0100 7c00 6a01 6405  d.d.d.....|.j.d.
-00001980: 7402 6406 6407 6404 8d04 0100 6400 5300  t.d.d.d.....d.S.
-00001990: 2908 4e7a 0a2d 2d72 756e 5f6e 616d 657a  ).Nz.--run_namez
-000019a0: 1265 7261 3520 7768 6f6c 6520 6461 7461  .era5 whole data
-000019b0: 7365 747a 224e 616d 6520 6f66 2072 756e  setz"Name of run
-000019c0: 2075 7365 6420 666f 7220 6c6f 6767 696e   used for loggin
-000019d0: 6720 6f6e 6c79 2e72 0a00 0000 7a18 2d2d  g only.r....z.--
-000019e0: 6d6c 666c 6f77 5f65 7870 6572 696d 656e  mlflow_experimen
-000019f0: 745f 6e61 6d65 7a12 6d61 656c 7374 726f  t_namez.maelstro
-00001a00: 6d2d 6132 2d74 7261 696e 7a30 4e61 6d65  m-a2-trainz0Name
-00001a10: 204d 4c66 6c6f 7720 6578 7065 7269 6d65   MLflow experime
-00001a20: 6e74 2077 6865 7265 2072 6573 756c 7473  nt where results
-00001a30: 2061 7265 206c 6f67 6765 642e 2903 da07   are logged.)...
-00001a40: 6669 6775 7265 7372 0e00 0000 720f 0000  figuresr....r...
-00001a50: 0072 1400 0000 7206 0000 0072 0600 0000  .r....r....r....
-00001a60: 7207 0000 00da 066d 6c66 6c6f 77fb 0000  r......mlflow...
-00001a70: 0073 1000 0000 0801 1201 0401 0201 0201  .s..............
-00001a80: 0201 0201 0afc 7244 0000 0063 0100 0000  ......rD...c....
-00001a90: 0000 0000 0000 0000 0100 0000 0600 0000  ................
-00001aa0: 4300 0000 722d 0000 0029 054e 7a0f 2d2d  C...r-...).Nz.--
-00001ab0: 6669 6775 7265 5f66 6f6c 6465 727a 0866  figure_folderz.f
-00001ac0: 6967 7572 6573 2f72 0900 0000 720a 0000  igures/r....r...
-00001ad0: 0072 1700 0000 7214 0000 0072 0600 0000  .r....r....r....
-00001ae0: 7206 0000 0072 0700 0000 7243 0000 0006  r....r....rC....
-00001af0: 0100 0072 4200 0000 7243 0000 0063 0100  ...rB...rC...c..
-00001b00: 0000 0000 0000 0000 0000 0100 0000 0700  ................
-00001b10: 0000 4300 0000 7340 0000 007c 006a 0064  ..C...s@...|.j.d
-00001b20: 0164 0274 0164 0364 0464 058d 0501 007c  .d.t.d.d.d.....|
-00001b30: 006a 0064 0664 0774 0164 0064 0864 058d  .j.d.d.t.d.d.d..
-00001b40: 0501 007c 006a 0064 0964 0a74 0164 0b64  ...|.j.d.d.t.d.d
-00001b50: 0c64 058d 0501 0064 0053 0029 0d4e 7a0d  .d.....d.S.).Nz.
-00001b60: 2d2d 7261 6e64 6f6d 5f73 6565 647a 032d  --random_seedz.-
-00001b70: 7273 e92a 0000 007a 1252 616e 646f 6d20  rs.*...z.Random 
-00001b80: 7365 6564 2076 616c 7565 2e72 0a00 0000  seed value.r....
-00001b90: 7a08 2d2d 6a6f 625f 6964 7a04 2d6a 6964  z.--job_idz.-jid
-00001ba0: 7a1b 4a6f 6220 6964 2077 6865 6e20 7275  z.Job id when ru
-00001bb0: 6e6e 696e 6720 6f6e 2068 7063 2e7a 0b2d  nning on hpc.z.-
-00001bc0: 2d69 7465 7261 7469 6f6e 7a02 2d69 7201  -iterationz.-ir.
-00001bd0: 0000 007a 2949 7465 7261 7469 6f6e 206e  ...z)Iteration n
-00001be0: 756d 6265 7220 7768 656e 2072 756e 6e69  umber when runni
-00001bf0: 6e67 2062 656e 6368 6d61 726b 732e 2902  ng benchmarks.).
-00001c00: 720e 0000 0072 1a00 0000 7214 0000 0072  r....r....r....r
-00001c10: 0600 0000 7206 0000 0072 0700 0000 da14  ....r....r......
-00001c20: 6879 7065 7270 6172 616d 6574 6572 5f62  hyperparameter_b
-00001c30: 6173 6963 0c01 0000 7306 0000 0014 0114  asic....s.......
-00001c40: 0118 0172 4600 0000 6301 0000 0000 0000  ...rF...c.......
-00001c50: 0000 0000 0001 0000 0007 0000 0043 0000  .............C..
-00001c60: 0073 f600 0000 7400 7c00 8301 0100 7c00  .s....t.|.....|.
-00001c70: 6a01 6401 6402 7402 6403 6404 6405 8d05  j.d.d.t.d.d.d...
-00001c80: 0100 7c00 6a01 6406 6407 7402 6408 6409  ..|.j.d.d.t.d.d.
-00001c90: 6405 8d05 0100 7c00 6a01 640a 640b 7403  d.....|.j.d.d.t.
-00001ca0: 640c 640d 6405 8d05 0100 7c00 6a01 640e  d.d.d.....|.j.d.
-00001cb0: 640f 7403 6410 6411 6405 8d05 0100 7c00  d.t.d.d.d.....|.
-00001cc0: 6a01 6412 6413 7403 6410 6414 6405 8d05  j.d.d.t.d.d.d...
-00001cd0: 0100 7c00 6a01 6415 6416 7403 6417 6418  ..|.j.d.d.t.d.d.
-00001ce0: 6405 8d05 0100 7c00 6a01 6419 641a 7403  d.....|.j.d.d.t.
-00001cf0: 641b 641c 6405 8d05 0100 7c00 6a01 641d  d.d.d.....|.j.d.
-00001d00: 641e 7403 641b 641f 6405 8d05 0100 7c00  d.t.d.d.d.....|.
-00001d10: 6a01 6420 6421 7404 6422 6423 6405 8d05  j.d d!t.d"d#d...
-00001d20: 0100 7c00 6a01 6424 6425 6426 6427 6428  ..|.j.d$d%d&d'd(
-00001d30: 8d04 0100 7c00 6a01 6429 7402 6417 642a  ....|.j.d)t.d.d*
-00001d40: 6405 8d04 0100 7c00 6a01 642b 7402 6403  d.....|.j.d+t.d.
-00001d50: 642c 6405 8d04 0100 6400 5300 292d 4e7a  d,d.....d.S.)-Nz
-00001d60: 0f2d 2d6e 756d 6265 725f 6570 6f63 6873  .--number_epochs
-00001d70: 7a08 2d6e 6570 6f63 6873 7232 0000 007a  z.-nepochsr2...z
-00001d80: 194e 756d 6572 206f 6620 6570 6f63 6873  .Numer of epochs
-00001d90: 2074 6f20 7472 6169 6e2e 720a 0000 007a   to train.r....z
-00001da0: 0c2d 2d62 6174 6368 5f73 697a 657a 032d  .--batch_sizez.-
-00001db0: 6273 e920 0000 007a 214e 756d 6265 7220  bs. ...z!Number 
-00001dc0: 6f66 2073 616d 706c 6573 2070 6572 206d  of samples per m
-00001dd0: 696e 692d 6261 7463 682e 7a0f 2d2d 6c65  ini-batch.z.--le
-00001de0: 6172 6e69 6e67 5f72 6174 657a 032d 6c72  arning_ratez.-lr
-00001df0: 6769 1d55 4d10 75ff 3e7a 1d4c 6561 726e  gi.UM.u.>z.Learn
-00001e00: 696e 6720 7261 7465 2074 6f20 7472 6169  ing rate to trai
-00001e10: 6e20 6d6f 6465 6c2e 7a0e 2d2d 7765 6967  n model.z.--weig
-00001e20: 6874 5f64 6563 6179 7a03 2d77 6472 0100  ht_decayz.-wdr..
-00001e30: 0000 7a21 5765 6967 6874 2064 6563 6179  ..z!Weight decay
-00001e40: 2072 6174 6520 746f 2074 7261 696e 206d   rate to train m
-00001e50: 6f64 656c 2e7a 0e2d 2d77 6172 6d75 705f  odel.z.--warmup_
-00001e60: 7261 7469 6f7a 032d 7772 7a1c 5761 726d  ratioz.-wrz.Warm
-00001e70: 7570 2072 6174 696f 2074 6f20 7472 6169  up ratio to trai
-00001e80: 6e20 6d6f 6465 6c2e 7a0e 2d2d 7761 726d  n model.z.--warm
-00001e90: 7570 5f73 7465 7073 7a03 2d77 7369 f401  up_stepsz.-wsi..
-00001ea0: 0000 7a1c 5761 726d 7570 2073 7465 7073  ..z.Warmup steps
-00001eb0: 2074 6f20 7472 6169 6e20 6d6f 6465 6c2e   to train model.
-00001ec0: 7a15 2d2d 6869 6464 656e 5f64 726f 706f  z.--hidden_dropo
-00001ed0: 7574 5f70 726f 627a 042d 6864 7067 9a99  ut_probz.-hdpg..
-00001ee0: 9999 9999 b93f 7a26 5072 6f62 6162 696c  .....?z&Probabil
-00001ef0: 6974 7920 6f66 2068 6964 6465 6e20 6472  ity of hidden dr
-00001f00: 6f75 7020 6f75 7420 6c61 7965 722e 7a0d  oup out layer.z.
-00001f10: 2d2d 636c 735f 6472 6f70 6f75 747a 032d  --cls_dropoutz.-
-00001f20: 6364 7a27 4472 6f70 6f75 7420 7072 6f62  cdz'Dropout prob
-00001f30: 6162 696c 6974 7920 696e 2063 6c61 7373  ability in class
-00001f40: 6966 6965 7220 6865 6164 2e7a 132d 2d6c  ifier head.z.--l
-00001f50: 725f 7363 6865 6475 6c65 725f 7479 7065  r_scheduler_type
-00001f60: 7a04 2d6c 7374 da06 6c69 6e65 6172 7a1d  z.-lst..linearz.
-00001f70: 4c65 6172 6e69 6e67 2072 6174 6520 7363  Learning rate sc
-00001f80: 6865 6475 6c65 7220 7479 7065 2e7a 1a2d  heduler type.z.-
-00001f90: 2d62 6173 655f 6d6f 6465 6c5f 7765 6967  -base_model_weig
-00001fa0: 6874 735f 6669 7865 647a 0d2d 7765 6967  hts_fixedz.-weig
-00001fb0: 6874 7366 6978 6564 da0a 7374 6f72 655f  htsfixed..store_
-00001fc0: 7472 7565 7a4e 5765 6967 6874 7320 6f66  truezNWeights of
-00001fd0: 2062 6173 6520 6d6f 6465 6c20 2877 6974   base model (wit
-00001fe0: 686f 7574 2063 6c61 7373 6966 6963 6174  hout classificat
-00001ff0: 696f 6e20 6865 6164 2920 6172 6520 6669  ion head) are fi
-00002000: 7865 6420 286e 6f74 2074 7261 696e 6162  xed (not trainab
-00002010: 6c65 292e a902 da06 6163 7469 6f6e 720d  le).....actionr.
-00002020: 0000 007a 0c2d 2d73 6176 655f 7374 6570  ...z.--save_step
-00002030: 737a 2153 7465 7073 2061 6674 6572 2077  sz!Steps after w
-00002040: 6869 6368 206d 6f64 656c 2069 7320 7361  hich model is sa
-00002050: 7665 642e 7a0f 2d2d 6c6f 6767 696e 675f  ved.z.--logging_
-00002060: 7374 6570 737a 2953 7465 7073 2061 6674  stepsz)Steps aft
-00002070: 6572 2077 6869 6368 206d 6f64 656c 206c  er which model l
-00002080: 6f67 7320 6172 6520 7772 6974 7465 6e2e  ogs are written.
-00002090: 2905 7246 0000 0072 0e00 0000 721a 0000  ).rF...r....r...
-000020a0: 0072 2b00 0000 720f 0000 0072 1400 0000  .r+...r....r....
-000020b0: 7206 0000 0072 0600 0000 7207 0000 00da  r....r....r.....
-000020c0: 0e68 7970 6572 7061 7261 6d65 7465 7212  .hyperparameter.
-000020d0: 0100 0073 2800 0000 0801 1401 1401 1401  ...s(...........
-000020e0: 1401 1401 1401 0401 0a01 06ff 1403 1401  ................
-000020f0: 0402 0201 0201 0201 0201 06fc 1206 1601  ................
-00002100: 724c 0000 0063 0100 0000 0000 0000 0000  rL...c..........
-00002110: 0000 0100 0000 0500 0000 4300 0000 7324  ..........C...s$
-00002120: 0000 007c 006a 0064 0164 0264 0364 048d  ...|.j.d.d.d.d..
-00002130: 0301 007c 006a 0064 0564 0264 0664 048d  ...|.j.d.d.d.d..
-00002140: 0301 0064 0053 0029 074e 7a10 2d2d 6c6f  ...d.S.).Nz.--lo
-00002150: 675f 6770 755f 6d65 6d6f 7279 7249 0000  g_gpu_memoryrI..
-00002160: 007a 1a4d 6f6e 6974 6f72 2043 7564 6120  .z.Monitor Cuda 
-00002170: 6d65 6d6f 7279 2075 7361 6765 2e72 4a00  memory usage.rJ.
-00002180: 0000 7a11 2d2d 6967 6e6f 7265 5f74 7261  ..z.--ignore_tra
-00002190: 636b 696e 677a 1455 7365 206d 616e 7469  ckingz.Use manti
-000021a0: 6b20 7472 6163 6b69 6e67 2ea9 0172 0e00  k tracking...r..
-000021b0: 0000 7214 0000 0072 0600 0000 7206 0000  ..r....r....r...
-000021c0: 0072 0700 0000 da0a 6265 6e63 686d 6172  .r......benchmar
-000021d0: 6b73 2a01 0000 7314 0000 0004 0102 0102  ks*...s.........
-000021e0: 0102 0106 fd04 0502 0102 0102 010a fd72  ...............r
-000021f0: 4e00 0000 6301 0000 0000 0000 0000 0000  N...c...........
-00002200: 0001 0000 0005 0000 0043 0000 0073 1400  .........C...s..
-00002210: 0000 7c00 6a00 6401 6402 6403 6404 8d03  ..|.j.d.d.d.d...
-00002220: 0100 6400 5300 2905 4e7a 072d 2d64 6562  ..d.S.).Nz.--deb
-00002230: 7567 7249 0000 007a 1d57 6865 7468 6572  ugrI...z.Whether
-00002240: 2074 6f20 746f 6767 6c65 2064 6562 7567   to toggle debug
-00002250: 206d 6f64 652e 724a 0000 0072 4d00 0000   mode.rJ...rM...
-00002260: 7214 0000 0072 0600 0000 7206 0000 0072  r....r....r....r
-00002270: 0700 0000 da05 6465 6275 6737 0100 0073  ......debug7...s
-00002280: 0a00 0000 0401 0201 0201 0201 0afd 724f  ..............rO
-00002290: 0000 00da 0762 6f6f 6c65 616e da06 7265  .....boolean..re
-000022a0: 7475 726e 6301 0000 0000 0000 0000 0000  turnc...........
-000022b0: 0001 0000 0005 0000 0043 0000 0073 4a00  .........C...sJ.
-000022c0: 0000 7c00 6401 6b02 730c 7c00 6402 6b02  ..|.d.k.s.|.d.k.
-000022d0: 730c 7c00 6403 6b02 720e 6404 5300 7c00  s.|.d.k.r.d.S.|.
-000022e0: 6405 6b02 731a 7c00 6406 6b02 731a 7c00  d.k.s.|.d.k.s.|.
-000022f0: 6407 6b02 721c 6408 5300 7400 a001 6409  d.k.r.d.S.t...d.
-00002300: 7c00 9b02 640a 9d03 a101 8201 290b 7a21  |...d.......).z!
-00002310: 4375 7374 6f6d 2061 7267 7061 7273 6520  Custom argparse 
-00002320: 7479 7065 2066 6f72 2062 6f6f 6c65 616e  type for boolean
-00002330: 73da 0546 616c 7365 da05 6661 6c73 65da  s..False..false.
-00002340: 0130 46da 0454 7275 65da 0474 7275 65da  .0F..True..true.
-00002350: 0131 547a 1943 6f75 6c64 6e27 7420 636f  .1Tz.Couldn't co
-00002360: 6e76 6572 7420 626f 6f6c 6561 6e3d 7a0c  nvert boolean=z.
-00002370: 2074 6f20 626f 6f6c 6561 6e21 2902 7203   to boolean!).r.
-00002380: 0000 00da 1141 7267 756d 656e 7454 7970  .....ArgumentTyp
-00002390: 6545 7272 6f72 2901 7250 0000 0072 0600  eError).rP...r..
-000023a0: 0000 7206 0000 0072 0700 0000 723c 0000  ..r....r....r<..
-000023b0: 003f 0100 0073 0a00 0000 1802 0401 1801  .?...s..........
-000023c0: 0401 1202 723c 0000 0029 1e72 0300 0000  ....r<...).r....
-000023d0: 7239 0000 00da 0861 322e 7574 696c 7372  r9.....a2.utilsr
-000023e0: 1000 0000 da1d 4172 6775 6d65 6e74 4465  ......ArgumentDe
-000023f0: 6661 756c 7473 4865 6c70 466f 726d 6174  faultsHelpFormat
-00002400: 7465 7272 0800 0000 7215 0000 0072 1800  terr....r....r..
-00002410: 0000 721b 0000 0072 2500 0000 7227 0000  ..r....r%...r'..
-00002420: 0072 2900 0000 722c 0000 0072 2e00 0000  .r)...r,...r....
-00002430: 7237 0000 0072 3800 0000 723b 0000 0072  r7...r8...r;...r
-00002440: 3d00 0000 723e 0000 0072 4000 0000 7241  =...r>...r@...rA
-00002450: 0000 0072 4400 0000 7243 0000 0072 4600  ...rD...rC...rF.
-00002460: 0000 724c 0000 0072 4e00 0000 724f 0000  ..rL...rN...rO..
-00002470: 0072 0f00 0000 da04 626f 6f6c 723c 0000  .r......boolr<..
-00002480: 0072 0600 0000 7206 0000 0072 0600 0000  .r....r....r....
-00002490: 7207 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-000024a0: 0000 0073 3400 0000 0800 0801 0802 0e03  ...s4...........
-000024b0: 0805 080a 0810 080d 0815 080c 080f 080a  ................
-000024c0: 0809 083b 0805 0810 0809 0815 0811 0806  ...;............
-000024d0: 080b 0806 0806 0818 080d 1608            ............
+00000040: 6401 6c02 5a03 6400 6401 6c04 5a03 6500  d.l.Z.d.d.l.Z.e.
+00000050: 6a05 6601 6402 6403 8401 5a06 6404 6405  j.f.d.d...Z.d.d.
+00000060: 8400 5a07 6406 6407 8400 5a08 6408 6409  ..Z.d.d...Z.d.d.
+00000070: 8400 5a09 640a 640b 8400 5a0a 640c 640d  ..Z.d.d...Z.d.d.
+00000080: 8400 5a0b 640e 640f 8400 5a0c 6410 6411  ..Z.d.d...Z.d.d.
+00000090: 8400 5a0d 6412 6413 8400 5a0e 6414 6415  ..Z.d.d...Z.d.d.
+000000a0: 8400 5a0f 6416 6417 8400 5a10 6418 6419  ..Z.d.d...Z.d.d.
+000000b0: 8400 5a11 641a 641b 8400 5a12 641c 641d  ..Z.d.d...Z.d.d.
+000000c0: 8400 5a13 641e 641f 8400 5a14 6420 6421  ..Z.d.d...Z.d d!
+000000d0: 8400 5a15 6422 6423 8400 5a16 6424 6425  ..Z.d"d#..Z.d$d%
+000000e0: 8400 5a17 6426 6427 8400 5a18 6428 6429  ..Z.d&d'..Z.d(d)
+000000f0: 8400 5a19 642a 642b 8400 5a1a 642c 642d  ..Z.d*d+..Z.d,d-
+00000100: 8400 5a1b 642e 651c 642f 651d 6604 6430  ..Z.d.e.d/e.f.d0
+00000110: 6431 8404 5a1e 6401 5300 2932 e900 0000  d1..Z.d.S.)2....
+00000120: 004e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
+00000130: 0000 0003 0000 0043 0000 0073 1000 0000  .......C...s....
+00000140: 7400 6a01 7c00 6401 8d01 7d01 7c01 5300  t.j.|.d...}.|.S.
+00000150: 2902 4e29 01da 0f66 6f72 6d61 7474 6572  ).N)...formatter
+00000160: 5f63 6c61 7373 2902 da08 6172 6770 6172  _class)...argpar
+00000170: 7365 da0e 4172 6775 6d65 6e74 5061 7273  se..ArgumentPars
+00000180: 6572 2902 7202 0000 00da 0670 6172 7365  er).r......parse
+00000190: 72a9 0072 0600 0000 fa33 2f68 6f6d 652f  r..r.....3/home/
+000001a0: 6b72 6973 7469 616e 2f50 726f 6a65 6374  kristian/Project
+000001b0: 732f 6132 2f73 7263 2f61 322f 7574 696c  s/a2/src/a2/util
+000001c0: 732f 6172 6770 6172 7365 2e70 79da 0a67  s/argparse.py..g
+000001d0: 6574 5f70 6172 7365 7207 0000 0073 0400  et_parser....s..
+000001e0: 0000 0c01 0401 7208 0000 0063 0100 0000  ......r....c....
+000001f0: 0000 0000 0000 0000 0100 0000 0700 0000  ................
+00000200: 4300 0000 7324 0000 007c 006a 0064 0164  C...s$...|.j.d.d
+00000210: 0274 0174 026a 036a 04a0 05a1 0064 031b  .t.t.j.j.....d..
+00000220: 0064 0464 058d 0501 0064 0053 0029 064e  .d.d.....d.S.).N
+00000230: 7a0c 2d2d 7477 6565 7473 5f64 6972 7a07  z.--tweets_dirz.
+00000240: 2d69 6e70 6174 687a 0774 7765 6574 732f  -inpathz.tweets/
+00000250: fa2e 4469 7265 6374 6f72 7920 7768 6572  ..Directory wher
+00000260: 6520 696e 7075 7420 6e65 7443 4446 2d66  e input netCDF-f
+00000270: 696c 6573 2061 7265 2073 746f 7265 642e  iles are stored.
+00000280: a903 da04 7479 7065 da07 6465 6661 756c  ....type..defaul
+00000290: 74da 0468 656c 7029 06da 0c61 6464 5f61  t..help)...add_a
+000002a0: 7267 756d 656e 74da 0373 7472 da02 6132  rgument..str..a2
+000002b0: da05 7574 696c 73da 0d66 696c 655f 6861  ..utils..file_ha
+000002c0: 6e64 6c69 6e67 da0f 6765 745f 666f 6c64  ndling..get_fold
+000002d0: 6572 5f64 6174 61a9 0172 0500 0000 7206  er_data..r....r.
+000002e0: 0000 0072 0600 0000 7207 0000 00da 0e64  ...r....r......d
+000002f0: 6174 6173 6574 5f74 7765 6574 730c 0000  ataset_tweets...
+00000300: 0073 0e00 0000 0401 0201 0201 0201 0e01  .s..............
+00000310: 0201 0afb 7215 0000 0063 0100 0000 0000  ....r....c......
+00000320: 0000 0000 0000 0100 0000 0700 0000 4300  ..............C.
+00000330: 0000 732a 0000 007c 006a 0064 0174 0164  ..s*...|.j.d.t.d
+00000340: 0264 0364 048d 0401 007c 006a 0064 0564  .d.d.....|.j.d.d
+00000350: 0674 0164 0764 0864 048d 0501 0064 0053  .t.d.d.d.....d.S
+00000360: 0029 094e 7a10 2d2d 6461 7461 7365 745f  .).Nz.--dataset_
+00000370: 7072 6566 6978 da86 3230 3230 5f74 7765  prefix..2020_twe
+00000380: 6574 735f 7261 696e 5f73 756e 5f76 6f63  ets_rain_sun_voc
+00000390: 6162 5f65 6d6f 6a69 735f 6c6f 6361 7469  ab_emojis_locati
+000003a0: 6f6e 735f 6262 615f 5470 5f65 7261 355f  ons_bba_Tp_era5_
+000003b0: 6e6f 5f62 6f74 735f 6e6f 726d 616c 697a  no_bots_normaliz
+000003c0: 6564 5f66 696c 7465 7265 645f 7765 6174  ed_filtered_weat
+000003d0: 6865 725f 7374 6174 696f 6e73 5f66 6978  her_stations_fix
+000003e0: 5f70 7265 6469 6374 6564 5f73 696d 706c  _predicted_simpl
+000003f0: 6564 6562 6572 7461 5f72 6164 6172 7a32  edeberta_radarz2
+00000400: 4461 7461 7365 7420 7072 6566 6978 2064  Dataset prefix d
+00000410: 6574 6572 6d69 6e65 6420 6475 7269 6e67  etermined during
+00000420: 2073 706c 6974 206f 6620 6461 7461 7365   split of datase
+00000430: 742e 720a 0000 007a 122d 2d64 6174 615f  t.r....z.--data_
+00000440: 6465 7363 7269 7074 696f 6e7a 062d 6461  descriptionz.-da
+00000450: 7461 647a 3f74 7765 6574 7320 3230 3137  tadz?tweets 2017
+00000460: 2d32 3032 302c 206b 6579 776f 7264 7320  -2020, keywords 
+00000470: 656d 6f6a 6973 2061 7320 6465 7363 7269  emojis as descri
+00000480: 7074 696f 6e2c 206b 6579 776f 7264 7320  ption, keywords 
+00000490: 6f6e 6c79 7a29 4461 7461 2064 6573 6372  onlyz)Data descr
+000004a0: 6970 7469 6f6e 2070 7572 656c 7920 7573  iption purely us
+000004b0: 6564 2066 6f72 206c 6f67 6769 6e67 2ea9  ed for logging..
+000004c0: 0272 0e00 0000 720f 0000 0072 1400 0000  .r....r....r....
+000004d0: 7206 0000 0072 0600 0000 7207 0000 00da  r....r....r.....
+000004e0: 0764 6174 6173 6574 1600 0000 731a 0000  .dataset....s...
+000004f0: 0004 0102 0102 0102 0102 0106 fc04 0602  ................
+00000500: 0102 0102 0102 0102 010a fb72 1800 0000  ...........r....
+00000510: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000520: 0007 0000 0043 0000 0073 2c00 0000 7c00  .....C...s,...|.
+00000530: 6a00 6401 6402 7401 6403 6404 6405 8d05  j.d.d.t.d.d.d...
+00000540: 0100 7c00 6a00 6406 6407 7402 6400 6408  ..|.j.d.d.t.d.d.
+00000550: 6405 8d05 0100 6400 5300 2909 4e7a 152d  d.....d.S.).Nz.-
+00000560: 2d65 7661 6c75 6174 696f 6e5f 7374 7261  -evaluation_stra
+00000570: 7465 6779 7a07 2d65 7374 7261 74da 0565  tegyz.-estrat..e
+00000580: 706f 6368 7a1f 5768 656e 2074 6f20 6576  pochz.When to ev
+00000590: 616c 7561 7465 2073 7465 7073 2f65 706f  aluate steps/epo
+000005a0: 6368 2f6e 6f72 0a00 0000 7a0c 2d2d 6576  ch/nor....z.--ev
+000005b0: 616c 5f73 7465 7073 7a07 2d65 7374 6570  al_stepsz.-estep
+000005c0: 737a 4b4e 756d 6265 7220 6f66 2073 7465  szKNumber of ste
+000005d0: 7073 2062 6574 7765 656e 2065 7661 6c75  ps between evalu
+000005e0: 6174 696f 6e73 2069 6620 6576 616c 7561  ations if evalua
+000005f0: 7469 6f6e 2073 7472 6174 6567 7920 6973  tion strategy is
+00000600: 2073 6574 2074 6f20 7374 6570 732e 2903   set to steps.).
+00000610: 720e 0000 0072 0f00 0000 da03 696e 7472  r....r......intr
+00000620: 1400 0000 7206 0000 0072 0600 0000 7207  ....r....r....r.
+00000630: 0000 00da 0a65 7661 6c75 6174 696f 6e26  .....evaluation&
+00000640: 0000 0073 1400 0000 0401 0a01 06ff 0403  ...s............
+00000650: 0201 0201 0201 0201 0201 0afb 721b 0000  ............r...
+00000660: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00000670: 0000 0700 0000 4300 0000 735c 0000 007c  ......C...s\...|
+00000680: 006a 0064 0174 0164 0264 0364 048d 0401  .j.d.t.d.d.d....
+00000690: 007c 006a 0064 0564 0664 0767 0274 0164  .|.j.d.d.d.g.t.d
+000006a0: 0864 0964 0a8d 0501 007c 006a 0064 0b74  .d.d.....|.j.d.t
+000006b0: 0164 0c64 0c67 0164 0d64 0e8d 0501 007c  .d.d.g.d.d.....|
+000006c0: 006a 0064 0f74 0164 1067 0064 11a2 0164  .j.d.t.d.g.d...d
+000006d0: 1264 0e8d 0501 0064 0053 0029 134e 7a0a  .d.....d.S.).Nz.
+000006e0: 2d2d 6b65 795f 7465 7874 da0f 7465 7874  --key_text..text
+000006f0: 5f6e 6f72 6d61 6c69 7a65 647a 1b4b 6579  _normalizedz.Key
+00000700: 2066 6f72 2074 6578 7420 696e 2069 6e70   for text in inp
+00000710: 7574 2066 696c 652e 720a 0000 007a 132d  ut file.r....z.-
+00000720: 2d63 6c61 7373 6966 6965 725f 646f 6d61  -classifier_doma
+00000730: 696e da04 7261 696e da09 7265 6c65 7661  in..rain..releva
+00000740: 6e63 6554 7a14 446f 6d61 696e 206f 6620  nceTz.Domain of 
+00000750: 636c 6173 7369 6669 6572 2904 da07 6368  classifier)...ch
+00000760: 6f69 6365 7372 0b00 0000 da08 7265 7175  oicesr......requ
+00000770: 6972 6564 720d 0000 007a 0b2d 2d6b 6579  iredr....z.--key
+00000780: 5f69 6e70 7574 da04 7465 7874 7a3f 436f  _input..textz?Co
+00000790: 6c75 6d6e 206e 616d 6520 6f66 2064 6174  lumn name of dat
+000007a0: 6173 6574 2074 6861 7420 636f 7272 6573  aset that corres
+000007b0: 706f 6e64 7320 746f 2069 6e70 7574 206f  ponds to input o
+000007c0: 6620 636c 6173 7369 6669 6572 2e29 0472  f classifier.).r
+000007d0: 0b00 0000 720c 0000 0072 1f00 0000 720d  ....r....r....r.
+000007e0: 0000 007a 0c2d 2d6b 6579 5f6f 7574 7075  ...z.--key_outpu
+000007f0: 74da 0772 6169 6e69 6e67 2903 7222 0000  t..raining).r"..
+00000800: 00da 0872 656c 6576 616e 74da 0f72 6169  ...relevant..rai
+00000810: 6e69 6e67 5f73 7461 7469 6f6e 7a40 436f  ning_stationz@Co
+00000820: 6c75 6d6e 206e 616d 6520 6f66 2064 6174  lumn name of dat
+00000830: 6173 6574 2074 6861 7420 636f 7272 6573  aset that corres
+00000840: 706f 6e64 7320 746f 206f 7574 7075 7420  ponds to output 
+00000850: 6f66 2063 6c61 7373 6966 6965 722e 7217  of classifier.r.
+00000860: 0000 0072 1400 0000 7206 0000 0072 0600  ...r....r....r..
+00000870: 0000 7207 0000 00da 0a63 6c61 7373 6966  ..r......classif
+00000880: 6965 7233 0000 0073 2400 0000 1201 0401  ier3...s$.......
+00000890: 0e01 06ff 0403 0201 0201 0201 0401 0201  ................
+000008a0: 06fb 0407 0201 0201 0201 0601 0201 0afb  ................
+000008b0: 7225 0000 0063 0100 0000 0000 0000 0000  r%...c..........
+000008c0: 0000 0100 0000 0600 0000 4300 0000 733a  ..........C...s:
+000008d0: 0000 007c 006a 0064 0164 0274 0164 0364  ...|.j.d.d.t.d.d
+000008e0: 048d 0401 007c 006a 0064 0564 0274 0164  .....|.j.d.d.t.d
+000008f0: 0664 048d 0401 007c 006a 0064 0764 0274  .d.....|.j.d.d.t
+00000900: 0164 0864 048d 0401 0064 0053 0029 094e  .d.d.....d.S.).N
+00000910: 7a18 2d2d 6669 6c65 6e61 6d65 5f64 6174  z.--filename_dat
+00000920: 6173 6574 5f74 7261 696e 547a 2646 696c  aset_trainTz&Fil
+00000930: 656e 616d 6520 6f66 2064 6174 6173 6574  ename of dataset
+00000940: 2075 7365 6420 666f 7220 7472 6169 6e69   used for traini
+00000950: 6e67 2ea9 0372 2000 0000 720b 0000 0072  ng...r ...r....r
+00000960: 0d00 0000 7a1b 2d2d 6669 6c65 6e61 6d65  ....z.--filename
+00000970: 5f64 6174 6173 6574 5f76 616c 6964 6174  _dataset_validat
+00000980: 657a 2846 696c 656e 616d 6520 6f66 2064  ez(Filename of d
+00000990: 6174 6173 6574 2075 7365 6420 666f 7220  ataset used for 
+000009a0: 7661 6c69 6461 7469 6f6e 2e7a 172d 2d66  validation.z.--f
+000009b0: 696c 656e 616d 655f 6461 7461 7365 745f  ilename_dataset_
+000009c0: 7465 7374 7a25 4669 6c65 6e61 6d65 206f  testz%Filename o
+000009d0: 6620 6461 7461 7365 7420 7573 6564 2066  f dataset used f
+000009e0: 6f72 2074 6573 7469 6e67 2e72 1700 0000  or testing.r....
+000009f0: 7214 0000 0072 0600 0000 7206 0000 0072  r....r....r....r
+00000a00: 0700 0000 da10 6461 7461 7365 745f 7472  ......dataset_tr
+00000a10: 6169 6e69 6e67 4800 0000 7312 0000 0004  ainingH...s.....
+00000a20: 0108 0106 ff04 0308 0106 ff04 0308 010a  ................
+00000a30: ff72 2700 0000 6301 0000 0000 0000 0000  .r'...c.........
+00000a40: 0000 0001 0000 0006 0000 0043 0000 0073  ...........C...s
+00000a50: 2800 0000 7c00 6a00 6401 7401 6402 6403  (...|.j.d.t.d.d.
+00000a60: 6404 8d04 0100 7c00 6a00 6405 7401 6406  d.....|.j.d.t.d.
+00000a70: 6407 6408 8d04 0100 6400 5300 2909 4e7a  d.d.....d.S.).Nz
+00000a80: 0c2d 2d6f 7574 7075 745f 6469 727a 076f  .--output_dirz.o
+00000a90: 7574 7075 742f 7a17 466f 6c64 6572 2074  utput/z.Folder t
+00000aa0: 6f20 7361 7665 2072 6573 756c 7473 2e72  o save results.r
+00000ab0: 0a00 0000 7a0b 2d2d 7461 736b 5f6e 616d  ....z.--task_nam
+00000ac0: 6554 7a43 4e61 6d65 206f 6620 7461 736b  eTzCName of task
+00000ad0: 2c20 7265 7375 6c74 7320 7769 6c6c 2062  , results will b
+00000ae0: 6520 7361 7665 6420 696e 2074 6869 7320  e saved in this 
+00000af0: 7375 6264 6972 6563 746f 7279 206f 6620  subdirectory of 
+00000b00: 6f75 7470 7574 2ea9 0372 0b00 0000 7220  output...r....r 
+00000b10: 0000 0072 0d00 0000 7217 0000 0072 1400  ...r....r....r..
+00000b20: 0000 7206 0000 0072 0600 0000 7207 0000  ..r....r....r...
+00000b30: 00da 066f 7574 7075 7454 0000 0073 1800  ...outputT...s..
+00000b40: 0000 0401 0201 0201 0201 0201 06fc 0406  ................
+00000b50: 0201 0201 0201 0201 0afc 7229 0000 0063  ..........r)...c
+00000b60: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000b70: 0600 0000 4300 0000 7328 0000 007c 006a  ....C...s(...|.j
+00000b80: 0064 0174 0164 0264 0364 048d 0401 007c  .d.t.d.d.d.....|
+00000b90: 006a 0064 0574 0264 0664 0764 048d 0401  .j.d.t.d.d.d....
+00000ba0: 0064 0053 0029 084e 7a0a 2d2d 6b65 795f  .d.S.).Nz.--key_
+00000bb0: 7261 696e da04 7470 5f68 7a20 4b65 7920  rain..tp_hz Key 
+00000bc0: 666f 7220 7261 696e 2064 6174 6120 696e  for rain data in
+00000bd0: 2069 6e70 7574 2066 696c 652e 720a 0000   input file.r...
+00000be0: 007a 102d 2d74 6872 6573 686f 6c64 5f72  .z.--threshold_r
+00000bf0: 6169 6e67 3a8c 30e2 8e79 453e 7a48 5468  aing:.0..yE>zHTh
+00000c00: 7265 7368 6f6c 6420 6162 6f76 6520 7768  reshold above wh
+00000c10: 6963 6820 7072 6563 6970 6974 6174 696f  ich precipitatio
+00000c20: 6e20 6973 2063 6f6e 7369 6465 7265 6420  n is considered 
+00000c30: 7261 696e 696e 6720 696e 2069 6e70 7574  raining in input
+00000c40: 2066 696c 652e 2903 720e 0000 0072 0f00   file.).r....r..
+00000c50: 0000 da05 666c 6f61 7472 1400 0000 7206  ....floatr....r.
+00000c60: 0000 0072 0600 0000 7207 0000 00da 0c64  ...r....r......d
+00000c70: 6174 6173 6574 5f72 6169 6e63 0000 0073  ataset_rainc...s
+00000c80: 0e00 0000 1201 0401 0201 0201 0201 0201  ................
+00000c90: 0afc 722c 0000 0063 0100 0000 0000 0000  ..r,...c........
+00000ca0: 0000 0000 0100 0000 0600 0000 4300 0000  ............C...
+00000cb0: f316 0000 007c 006a 0064 0174 0164 0264  .....|.j.d.t.d.d
+00000cc0: 0364 048d 0401 0064 0053 0029 054e 7a0f  .d.....d.S.).Nz.
+00000cd0: 2d2d 6b65 795f 7265 6c65 7661 6e63 6572  --key_relevancer
+00000ce0: 2300 0000 7a30 5661 7269 6162 6c65 206e  #...z0Variable n
+00000cf0: 616d 6520 7468 6174 2073 7065 6369 6669  ame that specifi
+00000d00: 6573 2072 656c 6576 616e 6365 206f 6620  es relevance of 
+00000d10: 5477 6565 742e 720a 0000 0072 1700 0000  Tweet.r....r....
+00000d20: 7214 0000 0072 0600 0000 7206 0000 0072  r....r....r....r
+00000d30: 0700 0000 da11 6461 7461 7365 745f 7265  ......dataset_re
+00000d40: 6c65 7661 6e63 656d 0000 00f3 0c00 0000  levancem........
+00000d50: 0401 0201 0201 0201 0201 0afc 722e 0000  ............r...
+00000d60: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00000d70: 0000 0700 0000 4300 0000 73a8 0000 007c  ......C...s....|
+00000d80: 006a 0064 0174 0164 0264 0364 048d 0401  .j.d.t.d.d.d....
+00000d90: 007c 006a 0064 0574 0164 0264 0364 048d  .|.j.d.t.d.d.d..
+00000da0: 0401 007c 006a 0064 0674 0264 0764 0864  ...|.j.d.t.d.d.d
+00000db0: 048d 0401 007c 006a 0064 0974 0164 0a64  .....|.j.d.t.d.d
+00000dc0: 0b64 048d 0401 007c 006a 0064 0c64 0d74  .d.....|.j.d.d.t
+00000dd0: 0364 0e64 0f64 048d 0501 007c 006a 0064  .d.d.d.....|.j.d
+00000de0: 1074 0164 1164 1264 048d 0401 007c 006a  .t.d.d.d.....|.j
+00000df0: 0064 1374 0164 1464 1564 048d 0401 007c  .d.t.d.d.d.....|
+00000e00: 006a 0064 1674 0164 1764 1864 048d 0401  .j.d.t.d.d.d....
+00000e10: 007c 006a 0064 1974 0164 1a64 1b64 048d  .|.j.d.t.d.d.d..
+00000e20: 0401 0064 0053 0029 1c4e 7a1f 2d2d 6669  ...d.S.).Nz.--fi
+00000e30: 6c65 6e61 6d65 5f74 7765 6574 735f 7769  lename_tweets_wi
+00000e40: 7468 5f6b 6579 776f 7264 737a 5b32 3031  th_keywordsz[201
+00000e50: 375f 3230 3230 5f74 7765 6574 735f 7261  7_2020_tweets_ra
+00000e60: 696e 5f73 756e 5f76 6f63 6162 5f65 6d6f  in_sun_vocab_emo
+00000e70: 6a69 735f 6c6f 6361 7469 6f6e 735f 6262  jis_locations_bb
+00000e80: 615f 5470 5f65 7261 355f 6e6f 5f62 6f74  a_Tp_era5_no_bot
+00000e90: 735f 6e6f 726d 616c 697a 6564 5f66 696c  s_normalized_fil
+00000ea0: 7465 7265 642e 6e63 7a1a 4669 6c65 6e61  tered.ncz.Filena
+00000eb0: 6d65 206f 6620 7472 6169 6e69 6e67 2064  me of training d
+00000ec0: 6174 612e 720a 0000 007a 1a2d 2d64 6174  ata.r....z.--dat
+00000ed0: 615f 6669 6c65 6e61 6d65 5f69 7272 656c  a_filename_irrel
+00000ee0: 6576 616e 747a 152d 2d6e 5f74 7765 6574  evantz.--n_tweet
+00000ef0: 735f 6972 7265 6c65 7661 6e74 e9ff ffff  s_irrelevant....
+00000f00: ff7a 744e 756d 6265 7220 6f66 2069 7272  .ztNumber of irr
+00000f10: 656c 6576 616e 7420 7477 6565 7473 2075  elevant tweets u
+00000f20: 7365 6420 746f 2063 7265 6174 6520 6461  sed to create da
+00000f30: 7461 7365 742c 2075 7365 2061 6c6c 2069  taset, use all i
+00000f40: 7272 656c 6576 616e 7420 7477 6565 7473  rrelevant tweets
+00000f50: 2062 7920 6465 6661 756c 7420 2860 6e5f   by default (`n_
+00000f60: 7477 6565 7473 5f69 7272 656c 6576 616e  tweets_irrelevan
+00000f70: 743d 2d31 6029 2e7a 0b2d 2d73 706c 6974  t=-1`).z.--split
+00000f80: 5f64 6972 da0f 7370 6c69 745f 7265 6c65  _dir..split_rele
+00000f90: 7661 6e63 657a 1e46 6f6c 6465 7220 746f  vancez.Folder to
+00000fa0: 2073 6176 6520 7370 6c69 7420 6461 7461   save split data
+00000fb0: 7365 7473 2e7a 142d 2d6b 6d73 5f77 6974  sets.z.--kms_wit
+00000fc0: 6869 6e5f 7374 6174 696f 6e7a 042d 6b6d  hin_stationz.-km
+00000fd0: 73e9 0100 0000 7a44 4469 7374 616e 6365  s.....zDDistance
+00000fe0: 2074 6f20 7765 6174 6865 7220 7374 6174   to weather stat
+00000ff0: 696f 6e2e 2055 7365 6420 746f 2063 7265  ion. Used to cre
+00001000: 6174 6520 7765 6174 6865 7220 7374 6174  ate weather stat
+00001010: 696f 6e20 6461 7461 7365 742e 7a1e 2d2d  ion dataset.z.--
+00001020: 6b65 795f 6469 7374 616e 6365 5f77 6561  key_distance_wea
+00001030: 7468 6572 5f73 7461 7469 6f6e da13 7374  ther_station..st
+00001040: 6174 696f 6e5f 6469 7374 616e 6365 5f6b  ation_distance_k
+00001050: 6d7a 5e4b 6579 2069 6e20 6461 7461 7365  mz^Key in datase
+00001060: 7420 7468 6174 2073 686f 7773 2064 6973  t that shows dis
+00001070: 7461 6e63 6520 746f 2077 6561 7468 6572  tance to weather
+00001080: 2073 7461 7469 6f6e 2e20 5573 6564 2074   station. Used t
+00001090: 6f20 6372 6561 7465 2077 6561 7468 6572  o create weather
+000010a0: 2073 7461 7469 6f6e 2064 6174 6173 6574   station dataset
+000010b0: 2e7a 202d 2d77 6561 7468 6572 5f73 7461  .z --weather_sta
+000010c0: 7469 6f6e 5f64 6174 6173 6574 5f70 7265  tion_dataset_pre
+000010d0: 6669 78da 1557 6561 7468 6572 5374 6174  fix..WeatherStat
+000010e0: 696f 6e44 6174 6173 6574 7a22 5072 6566  ionDatasetz"Pref
+000010f0: 6978 206f 6620 7765 6174 6865 7220 7374  ix of weather st
+00001100: 6174 696f 6e20 6461 7461 7365 742e 7a23  ation dataset.z#
+00001110: 2d2d 7261 696e 696e 675f 636c 6173 7369  --raining_classi
+00001120: 6669 6572 5f64 6174 6173 6574 5f70 7265  fier_dataset_pre
+00001130: 6669 78da 1852 6169 6e69 6e67 436c 6173  fix..RainingClas
+00001140: 7369 6669 6572 4461 7461 7365 747a 2550  sifierDatasetz%P
+00001150: 7265 6669 7820 6f66 2072 6169 6e69 6e67  refix of raining
+00001160: 2063 6c61 7373 6966 6965 7220 6461 7461   classifier data
+00001170: 7365 742e 7a25 2d2d 7265 6c65 7661 6e63  set.z%--relevanc
+00001180: 655f 636c 6173 7369 6669 6572 5f64 6174  e_classifier_dat
+00001190: 6173 6574 5f70 7265 6669 78da 1a52 656c  aset_prefix..Rel
+000011a0: 6576 616e 6365 436c 6173 7369 6669 6572  evanceClassifier
+000011b0: 4461 7461 7365 747a 2750 7265 6669 7820  Datasetz'Prefix 
+000011c0: 6f66 2072 656c 6576 616e 6365 2063 6c61  of relevance cla
+000011d0: 7373 6966 6965 7220 6461 7461 7365 742e  ssifier dataset.
+000011e0: 2904 720e 0000 0072 0f00 0000 721a 0000  ).r....r....r...
+000011f0: 0072 2b00 0000 7214 0000 0072 0600 0000  .r+...r....r....
+00001200: 7206 0000 0072 0700 0000 da17 6461 7461  r....r......data
+00001210: 7365 745f 7265 6c65 7661 6e63 655f 7370  set_relevance_sp
+00001220: 6c69 7476 0000 0073 6e00 0000 0401 0201  litv...sn.......
+00001230: 0201 0201 0201 06fc 0406 0201 0201 0201  ................
+00001240: 0201 06fc 0406 0201 0201 0201 0201 06fc  ................
+00001250: 0407 0201 0201 0201 0201 06fc 0406 0201  ................
+00001260: 0201 0201 0201 0201 06fb 0407 0201 0201  ................
+00001270: 0201 0201 06fc 0406 0201 0201 0201 0201  ................
+00001280: 06fc 0406 0201 0201 0201 0201 06fc 0406  ................
+00001290: 0201 0201 0201 0201 0afc 7237 0000 0063  ..........r7...c
+000012a0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000012b0: 0700 0000 4300 0000 732c 0000 007c 006a  ....C...s,...|.j
+000012c0: 0064 0164 0274 0164 0364 0464 058d 0501  .d.d.t.d.d.d....
+000012d0: 007c 006a 0064 0664 0774 0164 0364 0864  .|.j.d.d.t.d.d.d
+000012e0: 058d 0501 0064 0053 0029 094e 7a0b 2d2d  .....d.S.).Nz.--
+000012f0: 7465 7374 5f73 697a 657a 032d 7473 679a  test_sizez.-tsg.
+00001300: 9999 9999 99c9 3f7a 1546 7261 6374 696f  ......?z.Fractio
+00001310: 6e20 6f66 2074 6573 7420 7365 742e 720a  n of test set.r.
+00001320: 0000 007a 112d 2d76 616c 6964 6174 696f  ...z.--validatio
+00001330: 6e5f 7369 7a65 7a03 2d76 737a 1b46 7261  n_sizez.-vsz.Fra
+00001340: 6374 696f 6e20 6f66 2076 616c 6964 6174  ction of validat
+00001350: 696f 6e20 7365 742e 2902 720e 0000 0072  ion set.).r....r
+00001360: 2b00 0000 7214 0000 0072 0600 0000 7206  +...r....r....r.
+00001370: 0000 0072 0700 0000 da13 6461 7461 7365  ...r......datase
+00001380: 745f 7370 6c69 745f 7369 7a65 73b1 0000  t_split_sizes...
+00001390: 0073 0400 0000 1401 1801 7238 0000 0063  .s........r8...c
+000013a0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000013b0: 0600 0000 4300 0000 7332 0000 0074 007c  ....C...s2...t.|
+000013c0: 0083 0101 007c 006a 0164 0164 0274 026a  .....|.j.d.d.t.j
+000013d0: 0364 0364 048d 0401 007c 006a 0164 0574  .d.d.....|.j.d.t
+000013e0: 0464 0064 0664 078d 0401 0064 0053 0029  .d.d.d.....d.S.)
+000013f0: 084e 7a1b 2d2d 6669 6c65 6e61 6d65 5f64  .Nz.--filename_d
+00001400: 6174 6173 6574 5f74 6f5f 7370 6c69 7454  ataset_to_splitT
+00001410: 7a27 4669 6c65 6e61 6d65 206f 6620 6461  z'Filename of da
+00001420: 7461 7365 7420 7468 6174 2077 696c 6c20  taset that will 
+00001430: 6265 2073 706c 6974 2e72 2600 0000 7a0e  be split.r&...z.
+00001440: 2d2d 6b65 795f 7374 7261 7469 6679 7a23  --key_stratifyz#
+00001450: 4b65 7920 7573 6564 2074 6f20 7374 7261  Key used to stra
+00001460: 7469 6679 2064 6174 6173 6574 2073 706c  tify dataset spl
+00001470: 6974 2e72 0a00 0000 2905 7238 0000 0072  it.r....).r8...r
+00001480: 0e00 0000 da07 7061 7468 6c69 62da 0450  ......pathlib..P
+00001490: 6174 6872 0f00 0000 7214 0000 0072 0600  athr....r....r..
+000014a0: 0000 7206 0000 0072 0700 0000 da0d 6461  ..r....r......da
+000014b0: 7461 7365 745f 7370 6c69 74b6 0000 0073  taset_split....s
+000014c0: 1a00 0000 0801 0401 0201 0201 0401 0201  ................
+000014d0: 06fc 0406 0201 0201 0201 0201 0afc 723b  ..............r;
+000014e0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+000014f0: 0100 0000 0600 0000 4300 0000 722d 0000  ........C...r-..
+00001500: 0029 054e 7a11 2d2d 7365 6c65 6374 5f72  .).Nz.--select_r
+00001510: 656c 6576 616e 7454 7a47 5768 6574 6865  elevantTzGWhethe
+00001520: 7220 746f 206f 6e6c 7920 7365 6c65 6374  r to only select
+00001530: 2054 7765 6574 7320 6173 2072 6576 656c   Tweets as revel
+00001540: 616e 7420 2860 6172 6773 2e6b 6579 5f72  ant (`args.key_r
+00001550: 656c 6576 616e 6365 603d 3d54 7275 6529  elevance`==True)
+00001560: 2e72 0a00 0000 2902 720e 0000 00da 0e63  .r....).r......c
+00001570: 7573 746f 6d5f 626f 6f6c 6561 6e72 1400  ustom_booleanr..
+00001580: 0000 7206 0000 0072 0600 0000 7207 0000  ..r....r....r...
+00001590: 00da 0e64 6174 6173 6574 5f73 656c 6563  ...dataset_selec
+000015a0: 74c6 0000 0072 2f00 0000 723d 0000 0063  t....r/...r=...c
+000015b0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000015c0: 0600 0000 4300 0000 733c 0000 007c 006a  ....C...s<...|.j
+000015d0: 0064 0164 0274 016a 0264 0364 048d 0401  .d.d.t.j.d.d....
+000015e0: 007c 006a 0064 0574 0364 0264 0664 078d  .|.j.d.t.d.d.d..
+000015f0: 0401 007c 006a 0064 0874 0364 0264 0964  ...|.j.d.t.d.d.d
+00001600: 078d 0401 0064 0053 0029 0a4e 7a1a 2d2d  .....d.S.).Nz.--
+00001610: 6669 6c65 6e61 6d65 5f64 6174 6173 6574  filename_dataset
+00001620: 5f70 7265 6469 6374 547a 3646 696c 656e  _predictTz6Filen
+00001630: 616d 6520 6f66 2064 6174 6173 6574 2074  ame of dataset t
+00001640: 6861 7420 7072 6564 6963 7469 6f6e 7320  hat predictions 
+00001650: 7769 6c6c 2062 6520 6d61 6465 2066 6f72  will be made for
+00001660: 2e72 2600 0000 7a10 2d2d 7061 7468 5f72  .r&...z.--path_r
+00001670: 6177 5f6d 6f64 656c 7a26 4469 7265 6374  aw_modelz&Direct
+00001680: 6f72 7920 7768 6572 6520 756e 7472 6169  ory where untrai
+00001690: 6e65 6420 6d6f 6465 6c20 7361 7665 642e  ned model saved.
+000016a0: 7228 0000 007a 142d 2d70 6174 685f 7472  r(...z.--path_tr
+000016b0: 6169 6e65 645f 6d6f 6465 6c7a 2444 6972  ained_modelz$Dir
+000016c0: 6563 746f 7279 2077 6865 7265 2074 7261  ectory where tra
+000016d0: 696e 6564 206d 6f64 656c 2073 6176 6564  ined model saved
+000016e0: 2e29 0472 0e00 0000 7239 0000 0072 3a00  .).r....r9...r:.
+000016f0: 0000 720f 0000 0072 1400 0000 7206 0000  ..r....r....r...
+00001700: 0072 0600 0000 7207 0000 00da 0d70 7265  .r....r......pre
+00001710: 6469 6374 5f6d 6f64 656c cf00 0000 7324  dict_model....s$
+00001720: 0000 0004 0102 0102 0104 0102 0106 fc04  ................
+00001730: 0602 0102 0102 0102 0106 fc04 0602 0102  ................
+00001740: 0102 0102 010a fc72 3e00 0000 6301 0000  .......r>...c...
+00001750: 0000 0000 0000 0000 0001 0000 0007 0000  ................
+00001760: 0043 0000 0073 4e00 0000 7c00 6a00 6401  .C...sN...|.j.d.
+00001770: 6402 7401 6403 6404 6405 8d05 0100 7c00  d.t.d.d.d.....|.
+00001780: 6a00 6406 7401 7402 6a03 6a04 6a05 6407  j.d.t.t.j.j.j.d.
+00001790: 6408 6409 8d05 0100 7c00 6a00 640a 640b  d.d.....|.j.d.d.
+000017a0: 7401 7402 6a06 6a07 a008 a100 640c 6405  t.t.j.j.....d.d.
+000017b0: 8d05 0100 6400 5300 290d 4e7a 0c2d 2d6d  ....d.S.).Nz.--m
+000017c0: 6f64 656c 5f70 6174 687a 032d 696e 7a36  odel_pathz.-inz6
+000017d0: 2f70 2f70 726f 6a65 6374 2f64 6565 7061  /p/project/deepa
+000017e0: 6366 2f6d 6165 6c73 7472 6f6d 2f65 686c  cf/maelstrom/ehl
+000017f0: 6572 7431 2f64 6562 6572 7461 2d76 332d  ert1/deberta-v3-
+00001800: 736d 616c 6c2f 7209 0000 0072 0a00 0000  small/r....r....
+00001810: 7a0c 2d2d 6d6f 6465 6c5f 6e61 6d65 da0d  z.--model_name..
+00001820: 6465 6265 7274 615f 736d 616c 6c7a 2d4e  deberta_smallz-N
+00001830: 616d 6520 6f66 206d 6f64 656c 2c20 7365  ame of model, se
+00001840: 7473 2064 6566 6175 6c74 2068 7970 6572  ts default hyper
+00001850: 2070 6172 616d 6574 6572 732e 2904 720b   parameters.).r.
+00001860: 0000 0072 1f00 0000 720c 0000 0072 0d00  ...r....r....r..
+00001870: 0000 7a12 2d2d 6f75 7470 7574 5f64 6972  ..z.--output_dir
+00001880: 5f6d 6f64 656c 7a07 2d6f 7574 6469 727a  _modelz.-outdirz
+00001890: 264f 7574 7075 7420 6469 7265 6374 6f72  &Output director
+000018a0: 7920 7768 6572 6520 6d6f 6465 6c20 6973  y where model is
+000018b0: 2073 6176 6564 2e29 0972 0e00 0000 720f   saved.).r....r.
+000018c0: 0000 0072 1000 0000 da08 7472 6169 6e69  ...r......traini
+000018d0: 6e67 da0d 6d6f 6465 6c5f 636f 6e66 6967  ng..model_config
+000018e0: 73da 1053 5550 504f 5254 4544 5f4d 4f44  s..SUPPORTED_MOD
+000018f0: 454c 5372 1100 0000 7212 0000 00da 1167  ELSr....r......g
+00001900: 6574 5f66 6f6c 6465 725f 6d6f 6465 6c73  et_folder_models
+00001910: 7214 0000 0072 0600 0000 7206 0000 0072  r....r....r....r
+00001920: 0700 0000 da05 6d6f 6465 6ce4 0000 0073  ......model....s
+00001930: 2a00 0000 0401 0201 0201 0201 0201 0201  *...............
+00001940: 06fb 0407 0201 0201 0801 0201 0201 06fb  ................
+00001950: 0407 0201 0201 0201 0a01 0201 0afb 7244  ..............rD
+00001960: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00001970: 0100 0000 0600 0000 4300 0000 722d 0000  ........C...r-..
+00001980: 0029 054e 7a0c 2d2d 7275 6e5f 666f 6c64  .).Nz.--run_fold
+00001990: 6572 547a 334f 7574 7075 7420 666f 6c64  erTz3Output fold
+000019a0: 6572 2077 6865 7265 206d 6f64 656c 2069  er where model i
+000019b0: 7320 7361 7665 6420 696e 2060 6f75 7470  s saved in `outp
+000019c0: 7574 5f64 6972 602e 7228 0000 0072 1700  ut_dir`.r(...r..
+000019d0: 0000 7214 0000 0072 0600 0000 7206 0000  ..r....r....r...
+000019e0: 0072 0700 0000 da03 7275 6efc 0000 00f3  .r......run.....
+000019f0: 0600 0000 0401 0801 0aff 7245 0000 0063  ..........rE...c
+00001a00: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001a10: 0600 0000 4300 0000 7330 0000 0074 007c  ....C...s0...t.|
+00001a20: 0083 0101 007c 006a 0164 0174 0264 0264  .....|.j.d.t.d.d
+00001a30: 0364 048d 0401 007c 006a 0164 0574 0264  .d.....|.j.d.t.d
+00001a40: 0664 0764 048d 0401 0064 0053 0029 084e  .d.d.....d.S.).N
+00001a50: 7a0a 2d2d 7275 6e5f 6e61 6d65 7a12 6572  z.--run_namez.er
+00001a60: 6135 2077 686f 6c65 2064 6174 6173 6574  a5 whole dataset
+00001a70: 7a22 4e61 6d65 206f 6620 7275 6e20 7573  z"Name of run us
+00001a80: 6564 2066 6f72 206c 6f67 6769 6e67 206f  ed for logging o
+00001a90: 6e6c 792e 720a 0000 007a 182d 2d6d 6c66  nly.r....z.--mlf
+00001aa0: 6c6f 775f 6578 7065 7269 6d65 6e74 5f6e  low_experiment_n
+00001ab0: 616d 657a 126d 6165 6c73 7472 6f6d 2d61  amez.maelstrom-a
+00001ac0: 322d 7472 6169 6e7a 304e 616d 6520 4d4c  2-trainz0Name ML
+00001ad0: 666c 6f77 2065 7870 6572 696d 656e 7420  flow experiment 
+00001ae0: 7768 6572 6520 7265 7375 6c74 7320 6172  where results ar
+00001af0: 6520 6c6f 6767 6564 2e29 03da 0766 6967  e logged.)...fig
+00001b00: 7572 6573 720e 0000 0072 0f00 0000 7214  uresr....r....r.
+00001b10: 0000 0072 0600 0000 7206 0000 0072 0700  ...r....r....r..
+00001b20: 0000 da06 6d6c 666c 6f77 0201 0000 7310  ....mlflow....s.
+00001b30: 0000 0008 0112 0104 0102 0102 0102 0102  ................
+00001b40: 010a fc72 4800 0000 6301 0000 0000 0000  ...rH...c.......
+00001b50: 0000 0000 0001 0000 0006 0000 0043 0000  .............C..
+00001b60: 0072 2d00 0000 2905 4e7a 0f2d 2d66 6967  .r-...).Nz.--fig
+00001b70: 7572 655f 666f 6c64 6572 7a08 6669 6775  ure_folderz.figu
+00001b80: 7265 732f 7209 0000 0072 0a00 0000 7217  res/r....r....r.
+00001b90: 0000 0072 1400 0000 7206 0000 0072 0600  ...r....r....r..
+00001ba0: 0000 7207 0000 0072 4700 0000 0d01 0000  ..r....rG.......
+00001bb0: 7246 0000 0072 4700 0000 6301 0000 0000  rF...rG...c.....
+00001bc0: 0000 0000 0000 0001 0000 0007 0000 0043  ...............C
+00001bd0: 0000 0073 4000 0000 7c00 6a00 6401 6402  ...s@...|.j.d.d.
+00001be0: 7401 6403 6404 6405 8d05 0100 7c00 6a00  t.d.d.d.....|.j.
+00001bf0: 6406 6407 7401 6400 6408 6405 8d05 0100  d.d.t.d.d.d.....
+00001c00: 7c00 6a00 6409 640a 7401 640b 640c 6405  |.j.d.d.t.d.d.d.
+00001c10: 8d05 0100 6400 5300 290d 4e7a 0d2d 2d72  ....d.S.).Nz.--r
+00001c20: 616e 646f 6d5f 7365 6564 7a03 2d72 73e9  andom_seedz.-rs.
+00001c30: 2a00 0000 7a12 5261 6e64 6f6d 2073 6565  *...z.Random see
+00001c40: 6420 7661 6c75 652e 720a 0000 007a 082d  d value.r....z.-
+00001c50: 2d6a 6f62 5f69 647a 042d 6a69 647a 1b4a  -job_idz.-jidz.J
+00001c60: 6f62 2069 6420 7768 656e 2072 756e 6e69  ob id when runni
+00001c70: 6e67 206f 6e20 6870 632e 7a0b 2d2d 6974  ng on hpc.z.--it
+00001c80: 6572 6174 696f 6e7a 022d 6972 0100 0000  erationz.-ir....
+00001c90: 7a29 4974 6572 6174 696f 6e20 6e75 6d62  z)Iteration numb
+00001ca0: 6572 2077 6865 6e20 7275 6e6e 696e 6720  er when running 
+00001cb0: 6265 6e63 686d 6172 6b73 2e29 0272 0e00  benchmarks.).r..
+00001cc0: 0000 721a 0000 0072 1400 0000 7206 0000  ..r....r....r...
+00001cd0: 0072 0600 0000 7207 0000 00da 1468 7970  .r....r......hyp
+00001ce0: 6572 7061 7261 6d65 7465 725f 6261 7369  erparameter_basi
+00001cf0: 6313 0100 0073 0600 0000 1401 1401 1801  c....s..........
+00001d00: 724a 0000 0063 0100 0000 0000 0000 0000  rJ...c..........
+00001d10: 0000 0100 0000 0700 0000 4300 0000 73f6  ..........C...s.
+00001d20: 0000 0074 007c 0083 0101 007c 006a 0164  ...t.|.....|.j.d
+00001d30: 0164 0274 0264 0364 0464 058d 0501 007c  .d.t.d.d.d.....|
+00001d40: 006a 0164 0664 0774 0264 0864 0964 058d  .j.d.d.t.d.d.d..
+00001d50: 0501 007c 006a 0164 0a64 0b74 0364 0c64  ...|.j.d.d.t.d.d
+00001d60: 0d64 058d 0501 007c 006a 0164 0e64 0f74  .d.....|.j.d.d.t
+00001d70: 0364 1064 1164 058d 0501 007c 006a 0164  .d.d.d.....|.j.d
+00001d80: 1264 1374 0364 1064 1464 058d 0501 007c  .d.t.d.d.d.....|
+00001d90: 006a 0164 1564 1674 0364 1764 1864 058d  .j.d.d.t.d.d.d..
+00001da0: 0501 007c 006a 0164 1964 1a74 0364 1b64  ...|.j.d.d.t.d.d
+00001db0: 1c64 058d 0501 007c 006a 0164 1d64 1e74  .d.....|.j.d.d.t
+00001dc0: 0364 1b64 1f64 058d 0501 007c 006a 0164  .d.d.d.....|.j.d
+00001dd0: 2064 2174 0464 2264 2364 058d 0501 007c   d!t.d"d#d.....|
+00001de0: 006a 0164 2464 2564 2664 2764 288d 0401  .j.d$d%d&d'd(...
+00001df0: 007c 006a 0164 2974 0264 1764 2a64 058d  .|.j.d)t.d.d*d..
+00001e00: 0401 007c 006a 0164 2b74 0264 0364 2c64  ...|.j.d+t.d.d,d
+00001e10: 058d 0401 0064 0053 0029 2d4e 7a0f 2d2d  .....d.S.)-Nz.--
+00001e20: 6e75 6d62 6572 5f65 706f 6368 737a 082d  number_epochsz.-
+00001e30: 6e65 706f 6368 7372 3200 0000 7a19 4e75  nepochsr2...z.Nu
+00001e40: 6d65 7220 6f66 2065 706f 6368 7320 746f  mer of epochs to
+00001e50: 2074 7261 696e 2e72 0a00 0000 7a0c 2d2d   train.r....z.--
+00001e60: 6261 7463 685f 7369 7a65 7a03 2d62 73e9  batch_sizez.-bs.
+00001e70: 2000 0000 7a21 4e75 6d62 6572 206f 6620   ...z!Number of 
+00001e80: 7361 6d70 6c65 7320 7065 7220 6d69 6e69  samples per mini
+00001e90: 2d62 6174 6368 2e7a 0f2d 2d6c 6561 726e  -batch.z.--learn
+00001ea0: 696e 675f 7261 7465 7a03 2d6c 7267 691d  ing_ratez.-lrgi.
+00001eb0: 554d 1075 ff3e 7a1d 4c65 6172 6e69 6e67  UM.u.>z.Learning
+00001ec0: 2072 6174 6520 746f 2074 7261 696e 206d   rate to train m
+00001ed0: 6f64 656c 2e7a 0e2d 2d77 6569 6768 745f  odel.z.--weight_
+00001ee0: 6465 6361 797a 032d 7764 7201 0000 007a  decayz.-wdr....z
+00001ef0: 2157 6569 6768 7420 6465 6361 7920 7261  !Weight decay ra
+00001f00: 7465 2074 6f20 7472 6169 6e20 6d6f 6465  te to train mode
+00001f10: 6c2e 7a0e 2d2d 7761 726d 7570 5f72 6174  l.z.--warmup_rat
+00001f20: 696f 7a03 2d77 727a 1c57 6172 6d75 7020  ioz.-wrz.Warmup 
+00001f30: 7261 7469 6f20 746f 2074 7261 696e 206d  ratio to train m
+00001f40: 6f64 656c 2e7a 0e2d 2d77 6172 6d75 705f  odel.z.--warmup_
+00001f50: 7374 6570 737a 032d 7773 69f4 0100 007a  stepsz.-wsi....z
+00001f60: 1c57 6172 6d75 7020 7374 6570 7320 746f  .Warmup steps to
+00001f70: 2074 7261 696e 206d 6f64 656c 2e7a 152d   train model.z.-
+00001f80: 2d68 6964 6465 6e5f 6472 6f70 6f75 745f  -hidden_dropout_
+00001f90: 7072 6f62 7a04 2d68 6470 679a 9999 9999  probz.-hdpg.....
+00001fa0: 99b9 3f7a 2650 726f 6261 6269 6c69 7479  ..?z&Probability
+00001fb0: 206f 6620 6869 6464 656e 2064 726f 7570   of hidden droup
+00001fc0: 206f 7574 206c 6179 6572 2e7a 0d2d 2d63   out layer.z.--c
+00001fd0: 6c73 5f64 726f 706f 7574 7a03 2d63 647a  ls_dropoutz.-cdz
+00001fe0: 2744 726f 706f 7574 2070 726f 6261 6269  'Dropout probabi
+00001ff0: 6c69 7479 2069 6e20 636c 6173 7369 6669  lity in classifi
+00002000: 6572 2068 6561 642e 7a13 2d2d 6c72 5f73  er head.z.--lr_s
+00002010: 6368 6564 756c 6572 5f74 7970 657a 042d  cheduler_typez.-
+00002020: 6c73 74da 066c 696e 6561 727a 1d4c 6561  lst..linearz.Lea
+00002030: 726e 696e 6720 7261 7465 2073 6368 6564  rning rate sched
+00002040: 756c 6572 2074 7970 652e 7a1a 2d2d 6261  uler type.z.--ba
+00002050: 7365 5f6d 6f64 656c 5f77 6569 6768 7473  se_model_weights
+00002060: 5f66 6978 6564 7a0d 2d77 6569 6768 7473  _fixedz.-weights
+00002070: 6669 7865 64da 0a73 746f 7265 5f74 7275  fixed..store_tru
+00002080: 657a 4e57 6569 6768 7473 206f 6620 6261  ezNWeights of ba
+00002090: 7365 206d 6f64 656c 2028 7769 7468 6f75  se model (withou
+000020a0: 7420 636c 6173 7369 6669 6361 7469 6f6e  t classification
+000020b0: 2068 6561 6429 2061 7265 2066 6978 6564   head) are fixed
+000020c0: 2028 6e6f 7420 7472 6169 6e61 626c 6529   (not trainable)
+000020d0: 2ea9 02da 0661 6374 696f 6e72 0d00 0000  .....actionr....
+000020e0: 7a0c 2d2d 7361 7665 5f73 7465 7073 7a21  z.--save_stepsz!
+000020f0: 5374 6570 7320 6166 7465 7220 7768 6963  Steps after whic
+00002100: 6820 6d6f 6465 6c20 6973 2073 6176 6564  h model is saved
+00002110: 2e7a 0f2d 2d6c 6f67 6769 6e67 5f73 7465  .z.--logging_ste
+00002120: 7073 7a29 5374 6570 7320 6166 7465 7220  psz)Steps after 
+00002130: 7768 6963 6820 6d6f 6465 6c20 6c6f 6773  which model logs
+00002140: 2061 7265 2077 7269 7474 656e 2e29 0572   are written.).r
+00002150: 4a00 0000 720e 0000 0072 1a00 0000 722b  J...r....r....r+
+00002160: 0000 0072 0f00 0000 7214 0000 0072 0600  ...r....r....r..
+00002170: 0000 7206 0000 0072 0700 0000 da0e 6879  ..r....r......hy
+00002180: 7065 7270 6172 616d 6574 6572 1901 0000  perparameter....
+00002190: 7328 0000 0008 0114 0114 0114 0114 0114  s(..............
+000021a0: 0114 0104 010a 0106 ff14 0314 0104 0202  ................
+000021b0: 0102 0102 0102 0106 fc12 0616 0172 5000  .............rP.
+000021c0: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
+000021d0: 0000 0005 0000 0043 0000 0073 2400 0000  .......C...s$...
+000021e0: 7c00 6a00 6401 6402 6403 6404 8d03 0100  |.j.d.d.d.d.....
+000021f0: 7c00 6a00 6405 6402 6406 6404 8d03 0100  |.j.d.d.d.d.....
+00002200: 6400 5300 2907 4e7a 102d 2d6c 6f67 5f67  d.S.).Nz.--log_g
+00002210: 7075 5f6d 656d 6f72 7972 4d00 0000 7a1a  pu_memoryrM...z.
+00002220: 4d6f 6e69 746f 7220 4375 6461 206d 656d  Monitor Cuda mem
+00002230: 6f72 7920 7573 6167 652e 724e 0000 007a  ory usage.rN...z
+00002240: 112d 2d69 676e 6f72 655f 7472 6163 6b69  .--ignore_tracki
+00002250: 6e67 7a14 5573 6520 6d61 6e74 696b 2074  ngz.Use mantik t
+00002260: 7261 636b 696e 672e a901 720e 0000 0072  racking...r....r
+00002270: 1400 0000 7206 0000 0072 0600 0000 7207  ....r....r....r.
+00002280: 0000 00da 0a62 656e 6368 6d61 726b 7331  .....benchmarks1
+00002290: 0100 0073 1400 0000 0401 0201 0201 0201  ...s............
+000022a0: 06fd 0405 0201 0201 0201 0afd 7252 0000  ............rR..
+000022b0: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+000022c0: 0000 0500 0000 4300 0000 7314 0000 007c  ......C...s....|
+000022d0: 006a 0064 0164 0264 0364 048d 0301 0064  .j.d.d.d.d.....d
+000022e0: 0053 0029 054e 7a07 2d2d 6465 6275 6772  .S.).Nz.--debugr
+000022f0: 4d00 0000 7a1d 5768 6574 6865 7220 746f  M...z.Whether to
+00002300: 2074 6f67 676c 6520 6465 6275 6720 6d6f   toggle debug mo
+00002310: 6465 2e72 4e00 0000 7251 0000 0072 1400  de.rN...rQ...r..
+00002320: 0000 7206 0000 0072 0600 0000 7207 0000  ..r....r....r...
+00002330: 00da 0564 6562 7567 3e01 0000 730a 0000  ...debug>...s...
+00002340: 0004 0102 0102 0102 010a fd72 5300 0000  ...........rS...
+00002350: da07 626f 6f6c 6561 6eda 0672 6574 7572  ..boolean..retur
+00002360: 6e63 0100 0000 0000 0000 0000 0000 0100  nc..............
+00002370: 0000 0500 0000 4300 0000 734a 0000 007c  ......C...sJ...|
+00002380: 0064 016b 0273 0c7c 0064 026b 0273 0c7c  .d.k.s.|.d.k.s.|
+00002390: 0064 036b 0272 0e64 0453 007c 0064 056b  .d.k.r.d.S.|.d.k
+000023a0: 0273 1a7c 0064 066b 0273 1a7c 0064 076b  .s.|.d.k.s.|.d.k
+000023b0: 0272 1c64 0853 0074 00a0 0164 097c 009b  .r.d.S.t...d.|..
+000023c0: 0264 0a9d 03a1 0182 0129 0b7a 2143 7573  .d.......).z!Cus
+000023d0: 746f 6d20 6172 6770 6172 7365 2074 7970  tom argparse typ
+000023e0: 6520 666f 7220 626f 6f6c 6561 6e73 da05  e for booleans..
+000023f0: 4661 6c73 65da 0566 616c 7365 da01 3046  False..false..0F
+00002400: da04 5472 7565 da04 7472 7565 da01 3154  ..True..true..1T
+00002410: 7a19 436f 756c 646e 2774 2063 6f6e 7665  z.Couldn't conve
+00002420: 7274 2062 6f6f 6c65 616e 3d7a 0c20 746f  rt boolean=z. to
+00002430: 2062 6f6f 6c65 616e 2129 0272 0300 0000   boolean!).r....
+00002440: da11 4172 6775 6d65 6e74 5479 7065 4572  ..ArgumentTypeEr
+00002450: 726f 7229 0172 5400 0000 7206 0000 0072  ror).rT...r....r
+00002460: 0600 0000 7207 0000 0072 3c00 0000 4601  ....r....r<...F.
+00002470: 0000 730a 0000 0018 0204 0118 0104 0112  ..s.............
+00002480: 0272 3c00 0000 291f 7203 0000 0072 3900  .r<...).r....r9.
+00002490: 0000 da08 6132 2e75 7469 6c73 7210 0000  ....a2.utilsr...
+000024a0: 00da 0b61 322e 7472 6169 6e69 6e67 da1d  ...a2.training..
+000024b0: 4172 6775 6d65 6e74 4465 6661 756c 7473  ArgumentDefaults
+000024c0: 4865 6c70 466f 726d 6174 7465 7272 0800  HelpFormatterr..
+000024d0: 0000 7215 0000 0072 1800 0000 721b 0000  ..r....r....r...
+000024e0: 0072 2500 0000 7227 0000 0072 2900 0000  .r%...r'...r)...
+000024f0: 722c 0000 0072 2e00 0000 7237 0000 0072  r,...r....r7...r
+00002500: 3800 0000 723b 0000 0072 3d00 0000 723e  8...r;...r=...r>
+00002510: 0000 0072 4400 0000 7245 0000 0072 4800  ...rD...rE...rH.
+00002520: 0000 7247 0000 0072 4a00 0000 7250 0000  ..rG...rJ...rP..
+00002530: 0072 5200 0000 7253 0000 0072 0f00 0000  .rR...rS...r....
+00002540: da04 626f 6f6c 723c 0000 0072 0600 0000  ..boolr<...r....
+00002550: 7206 0000 0072 0600 0000 7207 0000 00da  r....r....r.....
+00002560: 083c 6d6f 6475 6c65 3e01 0000 0073 3600  .<module>....s6.
+00002570: 0000 0800 0801 0802 0801 0e02 0805 080a  ................
+00002580: 0810 080d 0815 080c 080f 080a 0809 083b  ...............;
+00002590: 0805 0810 0809 0815 0818 0806 080b 0806  ................
+000025a0: 0806 0818 080d 1608                      ........
```

### Comparing `a2-0.4.0/src/a2/utils/__pycache__/checks.cpython-310.pyc` & `a2-0.4.1/src/a2/utils/__pycache__/checks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/utils/__pycache__/constants.cpython-310.pyc` & `a2-0.4.1/src/a2/utils/__pycache__/constants.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/utils/__pycache__/file_handling.cpython-310.pyc` & `a2-0.4.1/src/a2/utils/__pycache__/file_handling.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/utils/__pycache__/testing.cpython-310.pyc` & `a2-0.4.1/src/a2/utils/__pycache__/testing.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/utils/__pycache__/times.cpython-310.pyc` & `a2-0.4.1/src/a2/utils/__pycache__/times.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/utils/__pycache__/utils.cpython-310.pyc` & `a2-0.4.1/src/a2/utils/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/utils/argparse.py` & `a2-0.4.1/src/a2/utils/argparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import pathlib
 
+import a2.training
 import a2.utils
 
 
 def get_parser(formatter_class=argparse.ArgumentDefaultsHelpFormatter):
     parser = argparse.ArgumentParser(formatter_class=formatter_class)
     return parser
 
@@ -230,14 +231,21 @@
         "--model_path",
         "-in",
         type=str,
         default="/p/project/deepacf/maelstrom/ehlert1/deberta-v3-small/",
         help="Directory where input netCDF-files are stored.",
     )
     parser.add_argument(
+        "--model_name",
+        type=str,
+        choices=a2.training.model_configs.SUPPORTED_MODELS,
+        default="deberta_small",
+        help="Name of model, sets default hyper parameters.",
+    )
+    parser.add_argument(
         "--output_dir_model",
         "-outdir",
         type=str,
         default=a2.utils.file_handling.get_folder_models(),
         help="Output directory where model is saved.",
     )
```

### Comparing `a2-0.4.0/src/a2/utils/checks.py` & `a2-0.4.1/src/a2/utils/checks.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/utils/constants.py` & `a2-0.4.1/src/a2/utils/constants.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/utils/file_handling.py` & `a2-0.4.1/src/a2/utils/file_handling.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/utils/testing.py` & `a2-0.4.1/src/a2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/src/a2/utils/utils.py` & `a2-0.4.1/src/a2/utils/utils.py`

 * *Files identical despite different names*

### Comparing `a2-0.4.0/PKG-INFO` & `a2-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a2
-Version: 0.4.0
+Version: 0.4.1
 Summary: Package for predicting information about the weather from social media data as application 2 for maelstrom project
 Author: Kristian Ehlert
 Author-email: kristian.ehlert@4-cast.de
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

