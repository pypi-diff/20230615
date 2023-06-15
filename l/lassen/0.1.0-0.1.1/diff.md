# Comparing `tmp/lassen-0.1.0.tar.gz` & `tmp/lassen-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lassen-0.1.0.tar", max compression
+gzip compressed data, was "lassen-0.1.1.tar", max compression
```

## Comparing `lassen-0.1.0.tar` & `lassen-0.1.1.tar`

### file list

```diff
@@ -1,46 +1,52 @@
--rw-r--r--   0        0        0     1071 2023-06-06 18:13:43.336753 lassen-0.1.0/LICENSE
--rw-r--r--   0        0        0     1307 2023-06-06 23:14:20.986381 lassen-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.986429 lassen-0.1.0/lassen/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.986933 lassen-0.1.0/lassen/alembic/__init__.py
--rw-r--r--   0        0        0     3685 2023-06-06 23:14:20.987092 lassen-0.1.0/lassen/alembic/cli.py
--rw-r--r--   0        0        0     3601 2023-06-06 23:14:20.987203 lassen-0.1.0/lassen/alembic/io.py
--rw-r--r--   0        0        0     1043 2023-06-06 23:14:20.987305 lassen-0.1.0/lassen/alembic/runner.py
--rw-r--r--   0        0        0      174 2023-06-06 23:14:20.987414 lassen-0.1.0/lassen/assets/__init__.py
--rw-r--r--   0        0        0     1592 2023-06-06 23:14:20.987525 lassen-0.1.0/lassen/assets/alembic.ini
--rw-r--r--   0        0        0      494 2023-06-06 23:14:20.987634 lassen-0.1.0/lassen/assets/script.py.mako
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.987697 lassen-0.1.0/lassen/core/__init__.py
--rw-r--r--   0        0        0      153 2023-06-06 23:14:20.988104 lassen-0.1.0/lassen/core/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2487 2023-06-06 23:14:20.988340 lassen-0.1.0/lassen/core/__pycache__/config.cpython-310.pyc
--rw-r--r--   0        0        0     1862 2023-06-06 23:14:20.988497 lassen-0.1.0/lassen/core/config.py
--rw-r--r--   0        0        0      240 2023-06-06 23:14:20.988685 lassen-0.1.0/lassen/db/__init__.py
--rw-r--r--   0        0        0      396 2023-06-06 23:14:20.988967 lassen-0.1.0/lassen/db/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      139 2023-06-06 23:14:20.989157 lassen-0.1.0/lassen/db/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      147 2023-06-06 23:14:20.989285 lassen-0.1.0/lassen/db/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0      293 2023-06-06 23:14:20.989436 lassen-0.1.0/lassen/db/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     1931 2023-06-06 23:14:20.989563 lassen-0.1.0/lassen/db/__pycache__/base_class.cpython-310.pyc
--rw-r--r--   0        0        0     2727 2023-06-06 23:14:20.989823 lassen-0.1.0/lassen/db/__pycache__/base_class.cpython-311.pyc
--rw-r--r--   0        0        0      839 2023-06-06 23:14:20.990021 lassen-0.1.0/lassen/db/__pycache__/session.cpython-310.pyc
--rw-r--r--   0        0        0     1271 2023-06-06 23:14:20.990178 lassen-0.1.0/lassen/db/__pycache__/session.cpython-311.pyc
--rw-r--r--   0        0        0     1909 2023-06-06 23:14:20.990303 lassen-0.1.0/lassen/db/base_class.py
--rw-r--r--   0        0        0      627 2023-06-06 23:14:20.990409 lassen-0.1.0/lassen/db/session.py
--rw-r--r--   0        0        0      210 2023-06-06 23:14:20.990522 lassen-0.1.0/lassen/schema.py
--rw-r--r--   0        0        0     9983 2023-06-06 23:14:20.990676 lassen-0.1.0/lassen/store.py
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.990727 lassen-0.1.0/lassen/tests/__init__.py
--rw-r--r--   0        0        0      154 2023-06-06 23:14:20.991017 lassen-0.1.0/lassen/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1754 2023-06-06 23:14:20.991221 lassen-0.1.0/lassen/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1220 2023-06-06 23:14:20.991368 lassen-0.1.0/lassen/tests/__pycache__/fixtures.cpython-310.pyc
--rw-r--r--   0        0        0     5734 2023-06-06 23:14:20.991533 lassen-0.1.0/lassen/tests/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1762 2023-06-06 23:14:20.991674 lassen-0.1.0/lassen/tests/conftest.py
--rw-r--r--   0        0        0      176 2023-06-06 23:14:20.991801 lassen-0.1.0/lassen/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      463 2023-06-06 23:14:20.991923 lassen-0.1.0/lassen/tests/fixtures/test_harness/README.md
--rw-r--r--   0        0        0      311 2023-06-06 23:14:20.992056 lassen-0.1.0/lassen/tests/fixtures/test_harness/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.992112 lassen-0.1.0/lassen/tests/fixtures/test_harness/test_harness/__init__.py
--rw-r--r--   0        0        0      691 2023-06-06 23:14:20.992321 lassen-0.1.0/lassen/tests/fixtures/test_harness/test_harness/migrations/62bf8def9fb1_new_migration.py
--rw-r--r--   0        0        0      653 2023-06-06 23:14:20.992456 lassen-0.1.0/lassen/tests/fixtures/test_harness/test_harness/migrations/96dbf6f6d068_add_name.py
--rw-r--r--   0        0        0      217 2023-06-06 23:14:20.992593 lassen-0.1.0/lassen/tests/fixtures/test_harness/test_harness/models.py
--rw-r--r--   0        0        0      461 2023-06-06 23:14:20.992727 lassen-0.1.0/lassen/tests/model_fixtures.py
--rw-r--r--   0        0        0     2252 2023-06-06 23:14:20.992858 lassen-0.1.0/lassen/tests/test_alembic.py
--rw-r--r--   0        0        0     2799 2023-06-06 23:14:20.992986 lassen-0.1.0/lassen/tests/test_store.py
--rw-r--r--   0        0        0      825 2023-06-06 23:14:20.993596 lassen-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2592 1970-01-01 00:00:00.000000 lassen-0.1.0/setup.py
--rw-r--r--   0        0        0     2014 1970-01-01 00:00:00.000000 lassen-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-06 18:13:43.336753 lassen-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2781 2023-06-15 20:32:39.925939 lassen-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.986429 lassen-0.1.1/lassen/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.986933 lassen-0.1.1/lassen/alembic/__init__.py
+-rw-r--r--   0        0        0     3685 2023-06-06 23:14:20.987092 lassen-0.1.1/lassen/alembic/cli.py
+-rw-r--r--   0        0        0     3601 2023-06-06 23:14:20.987203 lassen-0.1.1/lassen/alembic/io.py
+-rw-r--r--   0        0        0     1043 2023-06-06 23:14:20.987305 lassen-0.1.1/lassen/alembic/runner.py
+-rw-r--r--   0        0        0      174 2023-06-06 23:14:20.987414 lassen-0.1.1/lassen/assets/__init__.py
+-rw-r--r--   0        0        0     1592 2023-06-06 23:14:20.987525 lassen-0.1.1/lassen/assets/alembic.ini
+-rw-r--r--   0        0        0      494 2023-06-06 23:14:20.987634 lassen-0.1.1/lassen/assets/script.py.mako
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.987697 lassen-0.1.1/lassen/core/__init__.py
+-rw-r--r--   0        0        0      153 2023-06-15 18:56:14.388483 lassen-0.1.1/lassen/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2487 2023-06-15 18:56:14.389047 lassen-0.1.1/lassen/core/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0        0        0     1862 2023-06-06 23:14:20.988497 lassen-0.1.1/lassen/core/config.py
+-rw-r--r--   0        0        0        0 2023-06-15 18:37:01.994869 lassen-0.1.1/lassen/datasets/__init__.py
+-rw-r--r--   0        0        0     2178 2023-06-15 20:51:56.247602 lassen-0.1.1/lassen/datasets/dataset_helpers.py
+-rw-r--r--   0        0        0     3354 2023-06-15 20:44:26.345816 lassen-0.1.1/lassen/datasets/pyarrow_schemas.py
+-rw-r--r--   0        0        0      240 2023-06-06 23:14:20.988685 lassen-0.1.1/lassen/db/__init__.py
+-rw-r--r--   0        0        0      396 2023-06-15 18:56:14.757958 lassen-0.1.1/lassen/db/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      139 2023-06-06 23:14:20.989157 lassen-0.1.1/lassen/db/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      147 2023-06-06 23:14:20.989285 lassen-0.1.1/lassen/db/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0      293 2023-06-06 23:14:20.989436 lassen-0.1.1/lassen/db/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     1931 2023-06-15 18:56:14.890788 lassen-0.1.1/lassen/db/__pycache__/base_class.cpython-310.pyc
+-rw-r--r--   0        0        0     2727 2023-06-06 23:14:20.989823 lassen-0.1.1/lassen/db/__pycache__/base_class.cpython-311.pyc
+-rw-r--r--   0        0        0      839 2023-06-15 18:56:14.758390 lassen-0.1.1/lassen/db/__pycache__/session.cpython-310.pyc
+-rw-r--r--   0        0        0     1271 2023-06-06 23:14:20.990178 lassen-0.1.1/lassen/db/__pycache__/session.cpython-311.pyc
+-rw-r--r--   0        0        0     1909 2023-06-06 23:14:20.990303 lassen-0.1.1/lassen/db/base_class.py
+-rw-r--r--   0        0        0      627 2023-06-06 23:14:20.990409 lassen-0.1.1/lassen/db/session.py
+-rw-r--r--   0        0        0      210 2023-06-06 23:14:20.990522 lassen-0.1.1/lassen/schema.py
+-rw-r--r--   0        0        0      227 2023-06-15 20:59:44.481932 lassen-0.1.1/lassen/shared.py
+-rw-r--r--   0        0        0     9983 2023-06-06 23:14:20.990676 lassen-0.1.1/lassen/store.py
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.990727 lassen-0.1.1/lassen/tests/__init__.py
+-rw-r--r--   0        0        0      154 2023-06-15 18:56:14.194644 lassen-0.1.1/lassen/tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1973 2023-06-15 20:58:19.623882 lassen-0.1.1/lassen/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1220 2023-06-06 23:14:20.991368 lassen-0.1.1/lassen/tests/__pycache__/fixtures.cpython-310.pyc
+-rw-r--r--   0        0        0     5734 2023-06-15 18:56:14.924433 lassen-0.1.1/lassen/tests/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1901 2023-06-15 20:31:44.029614 lassen-0.1.1/lassen/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-15 18:44:54.915233 lassen-0.1.1/lassen/tests/datasets/__init__.py
+-rw-r--r--   0        0        0     1693 2023-06-15 21:00:27.169417 lassen-0.1.1/lassen/tests/datasets/test_dataset_helpers.py
+-rw-r--r--   0        0        0      176 2023-06-06 23:14:20.991801 lassen-0.1.1/lassen/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      463 2023-06-06 23:14:20.991923 lassen-0.1.1/lassen/tests/fixtures/test_harness/README.md
+-rw-r--r--   0        0        0      311 2023-06-06 23:14:20.992056 lassen-0.1.1/lassen/tests/fixtures/test_harness/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.992112 lassen-0.1.1/lassen/tests/fixtures/test_harness/test_harness/__init__.py
+-rw-r--r--   0        0        0      691 2023-06-06 23:14:20.992321 lassen-0.1.1/lassen/tests/fixtures/test_harness/test_harness/migrations/62bf8def9fb1_new_migration.py
+-rw-r--r--   0        0        0      653 2023-06-06 23:14:20.992456 lassen-0.1.1/lassen/tests/fixtures/test_harness/test_harness/migrations/96dbf6f6d068_add_name.py
+-rw-r--r--   0        0        0      217 2023-06-06 23:14:20.992593 lassen-0.1.1/lassen/tests/fixtures/test_harness/test_harness/models.py
+-rw-r--r--   0        0        0      461 2023-06-06 23:14:20.992727 lassen-0.1.1/lassen/tests/model_fixtures.py
+-rw-r--r--   0        0        0     2252 2023-06-06 23:14:20.992858 lassen-0.1.1/lassen/tests/test_alembic.py
+-rw-r--r--   0        0        0     2799 2023-06-06 23:14:20.992986 lassen-0.1.1/lassen/tests/test_store.py
+-rw-r--r--   0        0        0     1224 2023-06-15 21:09:05.405287 lassen-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4334 1970-01-01 00:00:00.000000 lassen-0.1.1/setup.py
+-rw-r--r--   0        0        0     3696 1970-01-01 00:00:00.000000 lassen-0.1.1/PKG-INFO
```

### Comparing `lassen-0.1.0/LICENSE` & `lassen-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lassen-0.1.0/lassen/alembic/cli.py` & `lassen-0.1.1/lassen/alembic/cli.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.0/lassen/alembic/io.py` & `lassen-0.1.1/lassen/alembic/io.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.0/lassen/alembic/runner.py` & `lassen-0.1.1/lassen/alembic/runner.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.0/lassen/assets/alembic.ini` & `lassen-0.1.1/lassen/assets/alembic.ini`

 * *Files identical despite different names*

### Comparing `lassen-0.1.0/lassen/core/__pycache__/config.cpython-310.pyc` & `lassen-0.1.1/lassen/core/__pycache__/config.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun  6 18:58:44 2023 UTC, .py size: 1862 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e481 7f64 4607 0000  o..........dF...
+00000000: 6f0d 0d0a 0000 0000 ccbd 7f64 4607 0000  o..........dF...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 0100 6400 6402 6c06  m.Z.m.Z...d.d.l.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 4700 6403 6404 8400 6404 6508 8303  ..G.d.d...d.e...
 00000070: 5a0b 6405 610c 6406 650b 6602 6407 6408  Z.d.a.d.e.f.d.d.
@@ -29,44 +29,44 @@
 000001c0: 0865 1066 0664 1264 1384 0483 015a 1147  .e.f.d.d.....Z.G
 000001d0: 0064 1464 1584 0064 1583 025a 1264 0f53  .d.d...d...Z.d.S
 000001e0: 0029 16da 0c43 6f72 6553 6574 7469 6e67  .)...CoreSetting
 000001f0: 737a 450a 2020 2020 436f 6d6d 6f6e 2063  szE.    Common c
 00000200: 6f6c 6c65 6374 696f 6e20 6f66 2073 6574  ollection of set
 00000210: 7469 6e67 732c 206b 6570 7420 6173 2073  tings, kept as s
 00000220: 696d 706c 6520 6173 2070 6f73 7369 626c  imple as possibl
-00000230: 652e 0a0a 2020 2020 5a0b 5345 5256 4552  e...    Z.SERVER
-00000240: 5f4e 414d 455a 0b53 4552 5645 525f 484f  _NAMEZ.SERVER_HO
+00000230: 652e 0a0a 2020 2020 da0b 5345 5256 4552  e...    ..SERVER
+00000240: 5f4e 414d 45da 0b53 4552 5645 525f 484f  _NAME..SERVER_HO
 00000250: 5354 da14 4241 434b 454e 445f 434f 5253  ST..BACKEND_CORS
 00000260: 5f4f 5249 4749 4e53 5429 01da 0370 7265  _ORIGINST)...pre
 00000270: da01 76da 0672 6574 7572 6e63 0200 0000  ..v..returnc....
 00000280: 0000 0000 0000 0000 0200 0000 0400 0000  ................
 00000290: 4300 0000 7342 0000 0074 007c 0174 0183  C...sB...t.|.t..
 000002a0: 0272 147c 01a0 0264 01a1 0173 1464 0264  .r.|...d...s.d.d
 000002b0: 0384 007c 01a0 0364 04a1 0144 0083 0153  ...|...d...D...S
 000002c0: 0074 007c 0174 0474 0166 0283 0272 1d7c  .t.|.t.t.f...r.|
 000002d0: 0153 0074 057c 0183 0182 0129 054e fa01  .S.t.|.....).N..
 000002e0: 5b63 0100 0000 0000 0000 0000 0000 0200  [c..............
 000002f0: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
 00000300: 007c 005d 067d 017c 01a0 00a1 0091 0271  .|.].}.|.......q
 00000310: 0253 00a9 0029 01da 0573 7472 6970 2902  .S...)...strip).
-00000320: da02 2e30 da01 6972 1100 0000 7211 0000  ...0..ir....r...
+00000320: da02 2e30 da01 6972 1300 0000 7213 0000  ...0..ir....r...
 00000330: 00fa 3a2f 5573 6572 732f 7069 6572 6365  ..:/Users/pierce
 00000340: 6672 6565 6d61 6e2f 7072 6f6a 6563 7473  freeman/projects
 00000350: 2f6c 6173 7365 6e2f 6c61 7373 656e 2f63  /lassen/lassen/c
 00000360: 6f72 652f 636f 6e66 6967 2e70 79da 0a3c  ore/config.py..<
 00000370: 6c69 7374 636f 6d70 3e13 0000 0073 0200  listcomp>....s..
 00000380: 0000 1400 7a36 436f 7265 5365 7474 696e  ....z6CoreSettin
 00000390: 6773 2e61 7373 656d 626c 655f 636f 7273  gs.assemble_cors
 000003a0: 5f6f 7269 6769 6e73 2e3c 6c6f 6361 6c73  _origins.<locals
 000003b0: 3e2e 3c6c 6973 7463 6f6d 703e fa01 2c29  >.<listcomp>..,)
 000003c0: 06da 0a69 7369 6e73 7461 6e63 65da 0373  ...isinstance..s
 000003d0: 7472 da0a 7374 6172 7473 7769 7468 da05  tr..startswith..
 000003e0: 7370 6c69 74da 046c 6973 74da 0a56 616c  split..list..Val
-000003f0: 7565 4572 726f 7229 02da 0363 6c73 720e  ueError)...clsr.
-00000400: 0000 0072 1100 0000 7211 0000 0072 1500  ...r....r....r..
+000003f0: 7565 4572 726f 7229 02da 0363 6c73 7210  ueError)...clsr.
+00000400: 0000 0072 1300 0000 7213 0000 0072 1700  ...r....r....r..
 00000410: 0000 da15 6173 7365 6d62 6c65 5f63 6f72  ....assemble_cor
 00000420: 735f 6f72 6967 696e 7310 0000 0073 0a00  s_origins....s..
 00000430: 0000 1402 1401 0e01 0401 0801 7a22 436f  ............z"Co
 00000440: 7265 5365 7474 696e 6773 2e61 7373 656d  reSettings.assem
 00000450: 626c 655f 636f 7273 5f6f 7269 6769 6e73  ble_cors_origins
 00000460: da0f 504f 5354 4752 4553 5f53 4552 5645  ..POSTGRES_SERVE
 00000470: 52da 0d50 4f53 5447 5245 535f 5553 4552  R..POSTGRES_USER
@@ -77,80 +77,80 @@
 000004c0: 6573 6303 0000 0000 0000 0000 0000 0003  esc.............
 000004d0: 0000 0009 0000 0043 0000 0073 4400 0000  .......C...sD...
 000004e0: 7400 7c01 7401 8302 7207 7c01 5300 7402  t.|.t...r.|.S.t.
 000004f0: 6a03 6401 7c02 a004 6402 a101 7c02 a004  j.d.|...d...|...
 00000500: 6403 a101 7c02 a004 6404 a101 6405 7c02  d...|...d...d.|.
 00000510: a004 6406 a101 701d 6407 9b00 9d02 6408  ..d...p.d.....d.
 00000520: 8d05 5300 2909 4eda 0a70 6f73 7467 7265  ..S.).N..postgre
-00000530: 7371 6c72 2100 0000 7222 0000 0072 2000  sqlr!...r"...r .
-00000540: 0000 fa01 2f72 2300 0000 da00 2905 da06  ..../r#.....)...
+00000530: 7371 6c72 2300 0000 7224 0000 0072 2200  sqlr#...r$...r".
+00000540: 0000 fa01 2f72 2500 0000 da00 2905 da06  ..../r%.....)...
 00000550: 7363 6865 6d65 da04 7573 6572 da08 7061  scheme..user..pa
 00000560: 7373 776f 7264 da04 686f 7374 da04 7061  ssword..host..pa
-00000570: 7468 2905 7218 0000 0072 1900 0000 7209  th).r....r....r.
+00000570: 7468 2905 721a 0000 0072 1b00 0000 7209  th).r....r....r.
 00000580: 0000 00da 0562 7569 6c64 da03 6765 7429  .....build..get)
-00000590: 0372 1e00 0000 720e 0000 0072 2500 0000  .r....r....r%...
-000005a0: 7211 0000 0072 1100 0000 7215 0000 00da  r....r....r.....
+00000590: 0372 2000 0000 7210 0000 0072 2700 0000  .r ...r....r'...
+000005a0: 7213 0000 0072 1300 0000 7217 0000 00da  r....r....r.....
 000005b0: 1661 7373 656d 626c 655f 6462 5f63 6f6e  .assemble_db_con
 000005c0: 6e65 6374 696f 6e1e 0000 0073 1200 0000  nection....s....
 000005d0: 0a02 0401 0401 0201 0801 0801 0801 1201  ................
 000005e0: 06fb 7a23 436f 7265 5365 7474 696e 6773  ..z#CoreSettings
 000005f0: 2e61 7373 656d 626c 655f 6462 5f63 6f6e  .assemble_db_con
 00000600: 6e65 6374 696f 6e63 0000 0000 0000 0000  nectionc........
 00000610: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
 00000620: 7310 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
 00000630: 0364 0253 0029 037a 1343 6f72 6553 6574  .d.S.).z.CoreSet
 00000640: 7469 6e67 732e 436f 6e66 6967 544e 2904  tings.ConfigTN).
 00000650: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
 00000660: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000670: 6d65 5f5f da0e 6361 7365 5f73 656e 7369  me__..case_sensi
-00000680: 7469 7665 7211 0000 0072 1100 0000 7211  tiver....r....r.
-00000690: 0000 0072 1500 0000 da06 436f 6e66 6967  ...r......Config
-000006a0: 2a00 0000 7304 0000 0008 0008 0172 3500  *...s........r5.
-000006b0: 0000 2913 7231 0000 0072 3200 0000 7233  ..).r1...r2...r3
-000006c0: 0000 00da 075f 5f64 6f63 5f5f 7219 0000  .....__doc__r...
+00000670: 6d65 5f5f 5a0e 6361 7365 5f73 656e 7369  me__Z.case_sensi
+00000680: 7469 7665 7213 0000 0072 1300 0000 7213  tiver....r....r.
+00000690: 0000 0072 1700 0000 da06 436f 6e66 6967  ...r......Config
+000006a0: 2a00 0000 7304 0000 0008 0008 0172 3600  *...s........r6.
+000006b0: 0000 2913 7233 0000 0072 3400 0000 7235  ..).r3...r4...r5
+000006c0: 0000 00da 075f 5f64 6f63 5f5f 721b 0000  .....__doc__r...
 000006d0: 00da 0f5f 5f61 6e6e 6f74 6174 696f 6e73  ...__annotations
-000006e0: 5f5f 7207 0000 0072 0c00 0000 7204 0000  __r....r....r...
-000006f0: 0072 0a00 0000 7206 0000 0072 1f00 0000  .r....r....r....
-00000700: 7224 0000 0072 0500 0000 7209 0000 0072  r$...r....r....r
-00000710: 0300 0000 7202 0000 0072 3000 0000 7235  ....r....r0...r5
-00000720: 0000 0072 1100 0000 7211 0000 0072 1100  ...r....r....r..
-00000730: 0000 7215 0000 0072 0b00 0000 0600 0000  ..r....r........
+000006e0: 5f5f 7207 0000 0072 0e00 0000 7204 0000  __r....r....r...
+000006f0: 0072 0a00 0000 7206 0000 0072 2100 0000  .r....r....r!...
+00000700: 7226 0000 0072 0500 0000 7209 0000 0072  r&...r....r....r
+00000710: 0300 0000 7202 0000 0072 3200 0000 7236  ....r....r2...r6
+00000720: 0000 0072 1300 0000 7213 0000 0072 1300  ...r....r....r..
+00000730: 0000 7217 0000 0072 0b00 0000 0600 0000  ..r....r........
 00000740: 731e 0000 000a 0004 0108 0508 0110 010a  s...............
 00000750: 022c 0108 0708 0108 0108 0110 010a 0224  .,.............$
 00000760: 0112 0b72 0b00 0000 4eda 0873 6574 7469  ...r....N..setti
 00000770: 6e67 7363 0100 0000 0000 0000 0000 0000  ngsc............
 00000780: 0100 0000 0100 0000 4300 0000 7308 0000  ........C...s...
 00000790: 007c 0061 0064 0153 0029 027a 490a 2020  .|.a.d.S.).zI.  
 000007a0: 2020 5265 6769 7374 6572 2061 2063 6c69    Register a cli
 000007b0: 656e 7420 7365 7474 696e 6773 206f 626a  ent settings obj
 000007c0: 6563 7420 7769 7468 2074 6865 206c 6173  ect with the las
 000007d0: 7365 6e20 6170 706c 6963 6174 696f 6e2e  sen application.
 000007e0: 0a0a 2020 2020 4e29 01da 0f5f 7365 7474  ..    N)..._sett
-000007f0: 696e 6773 5f63 6c61 7373 2901 7238 0000  ings_class).r8..
-00000800: 0072 1100 0000 7211 0000 0072 1500 0000  .r....r....r....
+000007f0: 696e 6773 5f63 6c61 7373 2901 7239 0000  ings_class).r9..
+00000800: 0072 1300 0000 7213 0000 0072 1700 0000  .r....r....r....
 00000810: da11 7265 6769 7374 6572 5f73 6574 7469  ..register_setti
-00000820: 6e67 7331 0000 0073 0200 0000 0806 723a  ngs1...s......r:
+00000820: 6e67 7331 0000 0073 0200 0000 0806 723b  ngs1...s......r;
 00000830: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
 00000840: 0000 0000 0200 0000 4300 0000 7316 0000  ........C...s...
 00000850: 0074 0064 0075 0072 0874 0164 0183 0182  .t.d.u.r.t.d....
 00000860: 0174 0083 0053 0029 024e 7a7d 4e6f 2073  .t...S.).Nz}No s
 00000870: 6574 7469 6e67 7320 7265 6769 7374 6572  ettings register
 00000880: 6564 2061 7420 7275 6e74 696d 6520 6279  ed at runtime by
 00000890: 2063 6c69 656e 7420 6170 706c 6963 6174   client applicat
 000008a0: 696f 6e2e 0a54 6f20 7265 6769 7374 6572  ion..To register
 000008b0: 2c20 7772 6170 2079 6f75 7220 436f 7265  , wrap your Core
 000008c0: 5365 7474 696e 6773 2073 7562 636c 6173  Settings subclas
 000008d0: 7320 7769 7468 2040 7265 6769 7374 6572  s with @register
-000008e0: 5f73 6574 7469 6e67 7329 0272 3900 0000  _settings).r9...
-000008f0: 721d 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-00000900: 1100 0000 7215 0000 00da 0c67 6574 5f73  ....r......get_s
+000008e0: 5f73 6574 7469 6e67 7329 0272 3a00 0000  _settings).r:...
+000008f0: 721f 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
+00000900: 1300 0000 7217 0000 00da 0c67 6574 5f73  ....r......get_s
 00000910: 6574 7469 6e67 733a 0000 0073 0a00 0000  ettings:...s....
-00000920: 0802 0201 0201 04ff 0604 723b 0000 0029  ..........r;...)
+00000920: 0802 0201 0201 04ff 0604 723c 0000 0029  ..........r<...)
 00000930: 0fda 0674 7970 696e 6772 0200 0000 7203  ...typingr....r.
 00000940: 0000 0072 0400 0000 7205 0000 0072 0600  ...r....r....r..
-00000950: 0000 da08 7079 6461 6e74 6963 7207 0000  ....pydanticr...
+00000950: 0000 5a08 7079 6461 6e74 6963 7207 0000  ..Z.pydanticr...
 00000960: 0072 0800 0000 7209 0000 0072 0a00 0000  .r....r....r....
-00000970: 720b 0000 0072 3900 0000 723a 0000 0072  r....r9...r:...r
-00000980: 3b00 0000 7211 0000 0072 1100 0000 7211  ;...r....r....r.
-00000990: 0000 0072 1500 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000970: 720b 0000 0072 3a00 0000 723b 0000 0072  r....r:...r;...r
+00000980: 3c00 0000 7213 0000 0072 1300 0000 7213  <...r....r....r.
+00000990: 0000 0072 1700 0000 da08 3c6d 6f64 756c  ...r......<modul
 000009a0: 653e 0100 0000 730c 0000 001c 0018 0210  e>....s.........
 000009b0: 0304 280e 030c 09                        ..(....
```

### Comparing `lassen-0.1.0/lassen/core/config.py` & `lassen-0.1.1/lassen/core/config.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.0/lassen/db/__pycache__/base_class.cpython-310.pyc` & `lassen-0.1.1/lassen/db/__pycache__/base_class.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun  6 19:22:11 2023 UTC, .py size: 1909 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6387 7f64 7507 0000  o.......c..du...
+00000000: 6f0d 0d0a 0000 0000 ccbd 7f64 7507 0000  o..........du...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6400  m.Z.m.Z.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 0100 650d  m.Z.m.Z.m.Z...e.
@@ -53,15 +53,15 @@
 00000340: 04da 0d41 7263 6869 7665 644d 6978 696e  ...ArchivedMixin
 00000350: 4629 02da 0764 6566 6175 6c74 da08 6e75  F)...default..nu
 00000360: 6c6c 6162 6c65 4e29 0672 1000 0000 7218  llableN).r....r.
 00000370: 0000 0072 1900 0000 7205 0000 0072 0400  ...r....r....r..
 00000380: 0000 da08 6172 6368 6976 6564 7215 0000  ....archivedr...
 00000390: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
 000003a0: 721c 0000 001b 0000 0073 0400 0000 0800  r........s......
-000003b0: 1201 721c 0000 005a 0e64 6f5f 6f72 6d5f  ..r....Z.do_orm_
+000003b0: 1201 721c 0000 00da 0e64 6f5f 6f72 6d5f  ..r......do_orm_
 000003c0: 6578 6563 7574 6563 0100 0000 0000 0000  executec........
 000003d0: 0000 0000 0100 0000 0700 0000 4300 0000  ............C...
 000003e0: 7346 0000 007c 006a 0073 1d7c 006a 0173  sF...|.j.s.|.j.s
 000003f0: 1f7c 006a 02a0 0364 0164 02a1 0273 217c  .|.j...d.d...s!|
 00000400: 006a 04a0 0574 0674 0764 0364 0484 0064  .j...t.t.d.d...d
 00000410: 0564 068d 03a1 017c 005f 0464 0753 0064  .d.....|._.d.S.d
 00000420: 0753 0064 0753 0064 0753 0029 0861 1501  .S.d.S.d.S.).a..
@@ -90,32 +90,32 @@
 00000590: 7207 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
 000005a0: 1500 0000 7216 0000 00da 083c 6c61 6d62  ....r......<lamb
 000005b0: 6461 3e3c 0000 0073 0200 0000 0c00 7a29  da><...s......z)
 000005c0: 5f61 6464 5f66 696c 7465 7269 6e67 5f63  _add_filtering_c
 000005d0: 7269 7465 7269 612e 3c6c 6f63 616c 733e  riteria.<locals>
 000005e0: 2e3c 6c61 6d62 6461 3e54 2901 da0f 696e  .<lambda>T)...in
 000005f0: 636c 7564 655f 616c 6961 7365 734e 2908  clude_aliasesN).
-00000600: 5a0e 6973 5f63 6f6c 756d 6e5f 6c6f 6164  Z.is_column_load
-00000610: 5a14 6973 5f72 656c 6174 696f 6e73 6869  Z.is_relationshi
+00000600: da0e 6973 5f63 6f6c 756d 6e5f 6c6f 6164  ..is_column_load
+00000610: da14 6973 5f72 656c 6174 696f 6e73 6869  ..is_relationshi
 00000620: 705f 6c6f 6164 da11 6578 6563 7574 696f  p_load..executio
 00000630: 6e5f 6f70 7469 6f6e 73da 0367 6574 da09  n_options..get..
 00000640: 7374 6174 656d 656e 74da 076f 7074 696f  statement..optio
 00000650: 6e73 720d 0000 0072 1c00 0000 2901 5a0d  nsr....r....).Z.
 00000660: 6578 6563 7574 655f 7374 6174 6572 1500  execute_stater..
 00000670: 0000 7215 0000 0072 1600 0000 da17 5f61  ..r....r......_a
 00000680: 6464 5f66 696c 7465 7269 6e67 5f63 7269  dd_filtering_cri
 00000690: 7465 7269 6123 0000 0073 1c00 0000 0411  teria#...s......
 000006a0: 02ff 0402 02fe 0c03 02fd 0606 0201 0201  ................
-000006b0: 0601 0201 04fd 0aff 0cfa 7226 0000 004e  ..........r&...N
+000006b0: 0601 0201 04fd 0aff 0cfa 7229 0000 004e  ..........r)...N
 000006c0: 2915 da06 7479 7069 6e67 7202 0000 005a  )...typingr....Z
 000006d0: 0a69 6e66 6c65 6374 696f 6e72 0300 0000  .inflectionr....
 000006e0: da0a 7371 6c61 6c63 6865 6d79 7204 0000  ..sqlalchemyr...
 000006f0: 0072 0500 0000 7206 0000 0072 0700 0000  .r....r....r....
-00000700: 5a0e 7371 6c61 6c63 6865 6d79 2e6f 726d  Z.sqlalchemy.orm
+00000700: da0e 7371 6c61 6c63 6865 6d79 2e6f 726d  ..sqlalchemy.orm
 00000710: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
 00000720: 0b00 0000 720c 0000 0072 0d00 0000 720e  ....r....r....r.
 00000730: 0000 0072 1c00 0000 da04 4261 7365 da0b  ...r......Base..
-00000740: 6c69 7374 656e 735f 666f 7272 2600 0000  listens_forr&...
+00000740: 6c69 7374 656e 735f 666f 7272 2900 0000  listens_forr)...
 00000750: 7215 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
 00000760: 1600 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
 00000770: 0000 7314 0000 000c 000c 0218 0120 0102  ..s.......... ..
 00000780: 0a10 010e 0b06 040a 040e 01              ...........
```

### Comparing `lassen-0.1.0/lassen/db/__pycache__/base_class.cpython-311.pyc` & `lassen-0.1.1/lassen/db/__pycache__/base_class.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.1.0/lassen/db/__pycache__/session.cpython-310.pyc` & `lassen-0.1.1/lassen/db/__pycache__/session.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun  6 18:44:55 2023 UTC, .py size: 627 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a77e 7f64 7302 0000  o........~.ds...
+00000000: 6f0d 0d0a 0000 0000 ccbd 7f64 7302 0000  o..........ds...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6108 6406 6407 8400 5a09 6501 6408 6409  a.d.d...Z.e.d.d.
 00000070: 8400 8301 5a0a 6405 5300 290a e900 0000  ....Z.d.S.).....
@@ -12,17 +12,17 @@
 000000b0: 616b 6572 2901 da0c 6765 745f 7365 7474  aker)...get_sett
 000000c0: 696e 6773 4e63 0000 0000 0000 0000 0000  ingsNc..........
 000000d0: 0000 0200 0000 0500 0000 4300 0000 7326  ..........C...s&
 000000e0: 0000 0074 0083 007d 0074 017c 006a 0264  ...t...}.t.|.j.d
 000000f0: 0164 028d 027d 0174 0364 0364 037c 0164  .d...}.t.d.d.|.d
 00000100: 048d 0361 0474 0453 0029 054e 5429 01da  ...a.t.S.).NT)..
 00000110: 0d70 6f6f 6c5f 7072 655f 7069 6e67 4629  .pool_pre_pingF)
-00000120: 03da 0a61 7574 6f63 6f6d 6d69 74da 0961  ...autocommit..a
+00000120: 03da 0a61 7574 6f63 6f6d 6d69 745a 0961  ...autocommitZ.a
 00000130: 7574 6f66 6c75 7368 da04 6269 6e64 2905  utoflush..bind).
-00000140: 7205 0000 0072 0300 0000 5a17 5351 4c41  r....r....Z.SQLA
+00000140: 7205 0000 0072 0300 0000 da17 5351 4c41  r....r......SQLA
 00000150: 4c43 4845 4d59 5f44 4154 4142 4153 455f  LCHEMY_DATABASE_
 00000160: 5552 4972 0400 0000 da0c 5365 7373 696f  URIr......Sessio
 00000170: 6e4c 6f63 616c 2902 da08 7365 7474 696e  nLocal)...settin
 00000180: 6773 da06 656e 6769 6e65 a900 720d 0000  gs..engine..r...
 00000190: 00fa 392f 5573 6572 732f 7069 6572 6365  ..9/Users/pierce
 000001a0: 6672 6565 6d61 6e2f 7072 6f6a 6563 7473  freeman/projects
 000001b0: 2f6c 6173 7365 6e2f 6c61 7373 656e 2f64  /lassen/lassen/d
@@ -39,15 +39,15 @@
 00000260: 00da 0563 6c6f 7365 2901 da02 6462 720d  ...close)...dbr.
 00000270: 0000 0072 0d00 0000 720e 0000 00da 0e67  ...r....r......g
 00000280: 6574 5f64 625f 636f 6e74 6578 7414 0000  et_db_context...
 00000290: 0073 1400 0000 0280 0402 0201 0801 0801  .s..............
 000002a0: 0802 0c01 0cff 0a01 02ff 7212 0000 0029  ..........r....)
 000002b0: 0bda 0a63 6f6e 7465 7874 6c69 6272 0200  ...contextlibr..
 000002c0: 0000 da0a 7371 6c61 6c63 6865 6d79 7203  ....sqlalchemyr.
-000002d0: 0000 00da 0e73 716c 616c 6368 656d 792e  .....sqlalchemy.
+000002d0: 0000 005a 0e73 716c 616c 6368 656d 792e  ...Z.sqlalchemy.
 000002e0: 6f72 6d72 0400 0000 da12 6c61 7373 656e  ormr......lassen
 000002f0: 2e63 6f72 652e 636f 6e66 6967 7205 0000  .core.configr...
 00000300: 0072 0a00 0000 720f 0000 0072 1200 0000  .r....r....r....
 00000310: 720d 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
 00000320: 0e00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
 00000330: 0000 7310 0000 000c 000c 020c 010c 0204  ..s.............
 00000340: 0208 0302 090e 01                        .......
```

### Comparing `lassen-0.1.0/lassen/db/__pycache__/session.cpython-311.pyc` & `lassen-0.1.1/lassen/db/__pycache__/session.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.1.0/lassen/db/base_class.py` & `lassen-0.1.1/lassen/db/base_class.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.0/lassen/db/session.py` & `lassen-0.1.1/lassen/db/session.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.0/lassen/store.py` & `lassen-0.1.1/lassen/store.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.0/lassen/tests/__pycache__/fixtures.cpython-310.pyc` & `lassen-0.1.1/lassen/tests/__pycache__/fixtures.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.1.0/lassen/tests/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc` & `lassen-0.1.1/lassen/tests/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun  6 23:00:26 2023 UTC, .py size: 2797 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-00000000: 6f0d 0d0a 0000 0000 8aba 7f64 ed0a 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 ccbd 7f64 ef0a 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
-00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
-00000050: 5a07 0100 6400 6403 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
-00000060: 6400 6404 6c0a 6d0b 5a0b 6d0c 5a0c 6d0d  d.d.l.m.Z.m.Z.m.
-00000070: 5a0d 6d0e 5a0e 0100 6400 6401 6c0f 5a0f  Z.m.Z...d.d.l.Z.
-00000080: 650f 6a10 6405 6507 6602 6406 6407 8404  e.j.d.e.f.d.d...
-00000090: 8301 5a11 6414 6405 6507 6409 6512 6604  ..Z.d.d.e.d.e.f.
-000000a0: 640a 640b 8405 5a13 6405 6507 6602 640c  d.d...Z.d.e.f.d.
-000000b0: 640d 8404 5a14 6405 6507 6602 640e 640f  d...Z.d.e.f.d.d.
-000000c0: 8404 5a15 6405 6507 6602 6410 6411 8404  ..Z.d.e.f.d.d...
-000000d0: 5a16 6405 6507 6602 6412 6413 8404 5a17  Z.d.e.f.d.d...Z.
+00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
+00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
+00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
+00000070: 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 0100  Z.m.Z.m.Z.m.Z...
+00000080: 6506 6a10 6405 6508 6602 6406 6407 8404  e.j.d.e.f.d.d...
+00000090: 8301 5a11 6414 6405 6508 6409 6512 6604  ..Z.d.d.e.d.e.f.
+000000a0: 640a 640b 8405 5a13 6405 6508 6602 640c  d.d...Z.d.e.f.d.
+000000b0: 640d 8404 5a14 6405 6508 6602 640e 640f  d...Z.d.e.f.d.d.
+000000c0: 8404 5a15 6405 6508 6602 6410 6411 8404  ..Z.d.e.f.d.d...
+000000d0: 5a16 6405 6508 6602 6412 6413 8404 5a17  Z.d.e.f.d.d...Z.
 000000e0: 6401 5300 2915 e900 0000 004e 2901 da07  d.S.)......N)...
 000000f0: 5365 7373 696f 6e29 01da 0953 746f 7265  Session)...Store
 00000100: 4261 7365 2904 da09 5465 7374 4d6f 6465  Base)...TestMode
 00000110: 6cda 0a54 6573 7453 6368 656d 61da 1054  l..TestSchema..T
 00000120: 6573 7453 6368 656d 6143 7265 6174 65da  estSchemaCreate.
 00000130: 1054 6573 7453 6368 656d 6155 7064 6174  .TestSchemaUpdat
 00000140: 65da 0a64 625f 7365 7373 696f 6e63 0100  e..db_sessionc..
@@ -30,15 +30,15 @@
 000001d0: 7465 5f61 6c6c 720a 0000 0029 0272 0800  te_allr....).r..
 000001e0: 0000 7209 0000 00a9 0072 0e00 0000 fa3f  ..r......r.....?
 000001f0: 2f55 7365 7273 2f70 6965 7263 6566 7265  /Users/piercefre
 00000200: 656d 616e 2f70 726f 6a65 6374 732f 6c61  eman/projects/la
 00000210: 7373 656e 2f6c 6173 7365 6e2f 7465 7374  ssen/lassen/test
 00000220: 732f 7465 7374 5f73 746f 7265 2e70 79da  s/test_store.py.
 00000230: 1275 7365 5f66 6978 7475 7265 5f6d 6f64  .use_fixture_mod
-00000240: 656c 730c 0000 0073 0400 0000 0c02 1401  els....s........
+00000240: 656c 730d 0000 0073 0400 0000 0c02 1402  els....s........
 00000250: 7210 0000 00e9 0100 0000 da08 7175 616e  r...........quan
 00000260: 7469 7479 6302 0000 0000 0000 0000 0000  tityc...........
 00000270: 0005 0000 0004 0000 0043 0000 0073 4e00  .........C...sN.
 00000280: 0000 6700 7d02 7400 7c01 8301 4400 5d1e  ..g.}.t.|...D.].
 00000290: 7d03 7401 6401 7c03 9b00 9d02 6402 8d01  }.t.d.|.....d...
 000002a0: 7d04 7c00 a002 7c04 a101 0100 7c00 a003  }.|...|.....|...
 000002b0: a100 0100 7c00 a004 7c04 a101 0100 7c02  ....|...|.....|.
@@ -48,15 +48,15 @@
 000002f0: 6572 0400 0000 da03 6164 64da 0566 6c75  er......add..flu
 00000300: 7368 da07 7265 6672 6573 68da 0661 7070  sh..refresh..app
 00000310: 656e 64da 0269 6429 0572 0800 0000 7212  end..id).r....r.
 00000320: 0000 005a 1263 7265 6174 655f 6964 656e  ...Z.create_iden
 00000330: 7469 6669 6572 73da 0169 5a0a 7465 7374  tifiers..iZ.test
 00000340: 5f6d 6f64 656c 720e 0000 0072 0e00 0000  _modelr....r....
 00000350: 720f 0000 00da 0c63 7265 6174 655f 6261  r......create_ba
-00000360: 7463 6812 0000 0073 1000 0000 0401 0c01  tch....s........
+00000360: 7463 6814 0000 0073 1000 0000 0401 0c01  tch....s........
 00000370: 1001 0a01 0801 0a01 0e01 0401 721b 0000  ............r...
 00000380: 0063 0200 0000 0000 0000 0000 0000 1300  .c..............
 00000390: 0000 0900 0000 4300 0000 73b0 0200 0074  ......C...s....t
 000003a0: 007c 0064 0164 028d 0264 0319 007d 0274  .|.d.d...d...}.t
 000003b0: 0174 0274 0374 0466 0319 0074 0583 017d  .t.t.t.f...t...}
 000003c0: 037c 036a 067c 007c 0264 048d 027d 0464  .|.j.|.|.d...}.d
 000003d0: 007d 057c 047c 0575 017d 067c 0673 5074  .}.|.|.u.}.|.sPt
@@ -150,15 +150,15 @@
 00000950: 4070 795f 6173 7365 7274 34da 0b40 7079  @py_assert4..@py
 00000960: 5f66 6f72 6d61 7438 da0b 4070 795f 6173  _format8..@py_as
 00000970: 7365 7274 36da 0b40 7079 5f61 7373 6572  sert6..@py_asser
 00000980: 7439 da0b 4070 795f 6173 7365 7274 38da  t9..@py_assert8.
 00000990: 0c40 7079 5f66 6f72 6d61 7431 31da 0c40  .@py_format11..@
 000009a0: 7079 5f66 6f72 6d61 7431 3372 0e00 0000  py_format13r....
 000009b0: 720e 0000 0072 0f00 0000 da13 7465 7374  r....r......test
-000009c0: 5f73 746f 7265 5f62 6173 655f 6765 741d  _store_base_get.
+000009c0: 5f73 746f 7265 5f62 6173 655f 6765 741f  _store_base_get.
 000009d0: 0000 0073 0e00 0000 1001 1202 0e02 7801  ...s..........x.
 000009e0: 9c01 8a01 e203 724e 0000 0063 0200 0000  ......rN...c....
 000009f0: 0000 0000 0000 0000 0900 0000 0700 0000  ................
 00000a00: 4300 0000 7320 0300 0074 007c 0064 0164  C...s ...t.|.d.d
 00000a10: 028d 0201 0074 0174 0274 0374 0466 0319  .....t.t.t.t.f..
 00000a20: 0074 0583 017d 027c 02a0 067c 00a1 017d  .t...}.|...|...}
 00000a30: 0374 077c 0383 017d 0464 017d 057c 047c  .t.|...}.d.}.|.|
@@ -227,15 +227,15 @@
 00000e20: 0000 0072 3f00 0000 2909 7208 0000 0072  ...r?...).r....r
 00000e30: 1000 0000 7234 0000 0072 2100 0000 7240  ....r4...r!...r@
 00000e40: 0000 00da 0b40 7079 5f61 7373 6572 7435  .....@py_assert5
 00000e50: 7247 0000 0072 4600 0000 5a0b 4070 795f  rG...rF...Z.@py_
 00000e60: 666f 726d 6174 3972 0e00 0000 720e 0000  format9r....r...
 00000e70: 0072 0f00 0000 da19 7465 7374 5f73 746f  .r......test_sto
 00000e80: 7265 5f62 6173 655f 6765 745f 6d75 6c74  re_base_get_mult
-00000e90: 692b 0000 0073 1400 0000 0c01 1202 0a02  i+...s..........
+00000e90: 692d 0000 0073 1400 0000 0c01 1202 0a02  i-...s..........
 00000ea0: ae01 0e03 ae01 0e03 b401 1003 bc01 7258  ..............rX
 00000eb0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
 00000ec0: 1000 0000 0700 0000 4300 0000 73f6 0100  ........C...s...
 00000ed0: 0074 007c 0064 0164 028d 0264 0319 007d  .t.|.d.d...d...}
 00000ee0: 0274 0174 0274 0374 0466 0319 0074 0583  .t.t.t.t.f...t..
 00000ef0: 017d 0374 047c 0264 0464 058d 027d 047c  .}.t.|.d.d...}.|
 00000f00: 036a 067c 007c 0264 068d 027d 0564 007d  .j.|.|.d...}.d.}
@@ -286,15 +286,15 @@
 000011d0: 0072 1000 0000 722a 0000 0072 3400 0000  .r....r*...r4...
 000011e0: 5a0d 7570 6461 7465 5f73 6368 656d 6172  Z.update_schemar
 000011f0: 5900 0000 7240 0000 0072 4100 0000 7242  Y...r@...rA...rB
 00001200: 0000 0072 4300 0000 725a 0000 0072 4400  ...rC...rZ...rD.
 00001210: 0000 7245 0000 0072 4600 0000 7247 0000  ..rE...rF...rG..
 00001220: 0072 4800 0000 720e 0000 0072 0e00 0000  .rH...r....r....
 00001230: 720f 0000 00da 1674 6573 745f 7374 6f72  r......test_stor
-00001240: 655f 6261 7365 5f75 7064 6174 6540 0000  e_base_update@..
+00001240: 655f 6261 7365 5f75 7064 6174 6542 0000  e_base_updateB..
 00001250: 0073 1200 0000 1001 1202 0c01 0e01 7801  .s............x.
 00001260: 1002 0801 9c01 8e01 725d 0000 0063 0200  ........r]...c..
 00001270: 0000 0000 0000 0000 0000 0a00 0000 0900  ................
 00001280: 0000 4300 0000 7322 0100 0074 007c 0064  ..C...s"...t.|.d
 00001290: 0164 028d 0264 0319 007d 0274 0174 0274  .d...d...}.t.t.t
 000012a0: 0374 0466 0319 0074 0583 017d 037c 036a  .t.f...t...}.|.j
 000012b0: 067c 007c 0264 048d 0201 007c 00a0 07a1  .|.|.d.....|....
@@ -333,27 +333,27 @@
 000014c0: 0000 0029 0a72 0800 0000 7210 0000 0072  ...).r....r....r
 000014d0: 2a00 0000 7234 0000 0072 4100 0000 7257  *...r4...rA...rW
 000014e0: 0000 0072 4b00 0000 da0b 4070 795f 6173  ...rK.....@py_as
 000014f0: 7365 7274 37da 0c40 7079 5f66 6f72 6d61  sert7..@py_forma
 00001500: 7431 305a 0c40 7079 5f66 6f72 6d61 7431  t10Z.@py_format1
 00001510: 3272 0e00 0000 720e 0000 0072 0f00 0000  2r....r....r....
 00001520: da16 7465 7374 5f73 746f 7265 5f62 6173  ..test_store_bas
-00001530: 655f 7265 6d6f 7665 4e00 0000 730a 0000  e_removeN...s...
+00001530: 655f 7265 6d6f 7665 5000 0000 730a 0000  e_removeP...s...
 00001540: 0010 0112 020e 0108 01ea 0372 6300 0000  ...........rc...
 00001550: 2901 7211 0000 0029 18da 0862 7569 6c74  ).r....)...built
 00001560: 696e 7372 3a00 0000 da19 5f70 7974 6573  insr:....._pytes
 00001570: 742e 6173 7365 7274 696f 6e2e 7265 7772  t.assertion.rewr
 00001580: 6974 65da 0961 7373 6572 7469 6f6e da07  ite..assertion..
-00001590: 7265 7772 6974 6572 3800 0000 da0e 7371  rewriter8.....sq
-000015a0: 6c61 6c63 6865 6d79 2e6f 726d 7202 0000  lalchemy.ormr...
-000015b0: 005a 0c6c 6173 7365 6e2e 7374 6f72 6572  .Z.lassen.storer
-000015c0: 0300 0000 5a1b 6c61 7373 656e 2e74 6573  ....Z.lassen.tes
-000015d0: 7473 2e6d 6f64 656c 5f66 6978 7475 7265  ts.model_fixture
-000015e0: 7372 0400 0000 7205 0000 0072 0600 0000  sr....r....r....
-000015f0: 7207 0000 00da 0670 7974 6573 74da 0766  r......pytest..f
+00001590: 7265 7772 6974 6572 3800 0000 da06 7079  rewriter8.....py
+000015a0: 7465 7374 da0e 7371 6c61 6c63 6865 6d79  test..sqlalchemy
+000015b0: 2e6f 726d 7202 0000 005a 0c6c 6173 7365  .ormr....Z.lasse
+000015c0: 6e2e 7374 6f72 6572 0300 0000 da1b 6c61  n.storer......la
+000015d0: 7373 656e 2e74 6573 7473 2e6d 6f64 656c  ssen.tests.model
+000015e0: 5f66 6978 7475 7265 7372 0400 0000 7205  _fixturesr....r.
+000015f0: 0000 0072 0600 0000 7207 0000 00da 0766  ...r....r......f
 00001600: 6978 7475 7265 7210 0000 00da 0369 6e74  ixturer......int
 00001610: 721b 0000 0072 4e00 0000 7258 0000 0072  r....rN...rX...r
 00001620: 5d00 0000 7263 0000 0072 0e00 0000 720e  ]...rc...r....r.
 00001630: 0000 0072 0e00 0000 720f 0000 00da 083c  ...r....r......<
 00001640: 6d6f 6475 6c65 3e01 0000 0073 1600 0000  module>....s....
-00001650: 2600 0c02 1801 0806 0402 1001 1405 0e0b  &...............
+00001650: 2200 0c01 0c02 1801 0408 1001 1406 0e0b  "...............
 00001660: 0e0e 0e15 120e                           ......
```

### Comparing `lassen-0.1.0/lassen/tests/conftest.py` & `lassen-0.1.1/lassen/tests/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from json import dumps as json_dumps
 from os import environ
+from tempfile import TemporaryDirectory
 
 import pytest
 from sqlalchemy import text
 
 from lassen.core.config import CoreSettings, register_settings
 from lassen.db.session import get_db_context
 
@@ -55,7 +56,13 @@
 
         # Make sure each test has a fresh context
         from lassen.db.base_class import Base
 
         Base.metadata.drop_all(bind=db.bind)
 
         yield db
+
+
+@pytest.fixture()
+def tempdir():
+    with TemporaryDirectory() as tempdir:
+        yield tempdir
```

### Comparing `lassen-0.1.0/lassen/tests/fixtures/test_harness/test_harness/migrations/62bf8def9fb1_new_migration.py` & `lassen-0.1.1/lassen/tests/fixtures/test_harness/test_harness/migrations/62bf8def9fb1_new_migration.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.0/lassen/tests/fixtures/test_harness/test_harness/migrations/96dbf6f6d068_add_name.py` & `lassen-0.1.1/lassen/tests/fixtures/test_harness/test_harness/migrations/96dbf6f6d068_add_name.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.0/lassen/tests/test_alembic.py` & `lassen-0.1.1/lassen/tests/test_alembic.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.0/lassen/tests/test_store.py` & `lassen-0.1.1/lassen/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.0/pyproject.toml` & `lassen-0.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lassen"
-version = "0.1.0"
+version = "0.1.1"
 description = "Common webapp scaffolding."
 authors = ["Pierce Freeman <pierce@freeman.vc>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 fastapi = "^0.96.0"
@@ -13,28 +13,43 @@
 inflection = "^0.5.1"
 psycopg2 = "^2.9.6"
 click = "^8.1.3"
 alembic = "^1.11.1"
 alembic-autogenerate-enums = "^0.1.1"
 python-dotenv = "^1.0.0"
 
+datasets = { version = "^2.13.0", optional = true }
+numpy = { version = "^1.24.3", optional = true }
+pandas = { version = "^2.0.2", optional = true }
+
+[tool.poetry.extras]
+datasets = ["datasets", "numpy", "pandas"]
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 black = "^23.3.0"
 mypy = "^1.3.0"
 autoflake = "^2.1.1"
 types-setuptools = "^67.8.0.0"
+pandas-stubs = "^2.0.2.230605"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 migrate = "lassen.alembic.cli:main"
 
 [tool.isort]
 profile = "black"
 known_first_party = "lassen"
 multi_line_output=3
+
+[[tool.mypy.overrides]]
+module = "pyarrow.*"
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = "datasets.*"
+ignore_missing_imports = true
```

