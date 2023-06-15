# Comparing `tmp/openlrc-0.0.6.tar.gz` & `tmp/openlrc-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlrc-0.0.6.tar", max compression
+gzip compressed data, was "openlrc-0.1.0.tar", max compression
```

## Comparing `openlrc-0.0.6.tar` & `openlrc-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
--rw-r--r--   0        0        0     1083 2023-05-10 10:20:06.659160 openlrc-0.0.6/LICENSE
--rw-r--r--   0        0        0      106 2023-06-09 13:01:57.605311 openlrc-0.0.6/openlrc/__init__.py
--rw-r--r--   0        0        0      257 2023-06-09 13:43:55.157439 openlrc-0.0.6/openlrc/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3799 2023-06-10 15:06:50.217240 openlrc-0.0.6/openlrc/__pycache__/chatbot.cpython-310.pyc
--rw-r--r--   0        0        0     1031 2023-06-09 20:00:35.708506 openlrc-0.0.6/openlrc/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0      340 2023-06-08 23:05:47.950899 openlrc-0.0.6/openlrc/__pycache__/logger.cpython-310.pyc
--rw-r--r--   0        0        0     9283 2023-06-11 16:23:25.091195 openlrc-0.0.6/openlrc/__pycache__/lrc.cpython-310.pyc
--rw-r--r--   0        0        0     2926 2023-06-11 19:51:57.480862 openlrc-0.0.6/openlrc/__pycache__/openlrc.cpython-310.pyc
--rw-r--r--   0        0        0     2941 2023-06-09 20:52:00.624913 openlrc-0.0.6/openlrc/__pycache__/prompter.cpython-310.pyc
--rw-r--r--   0        0        0     3475 2023-06-11 19:51:59.408921 openlrc-0.0.6/openlrc/__pycache__/transcribe.cpython-310.pyc
--rw-r--r--   0        0        0     4592 2023-06-11 16:23:25.372735 openlrc-0.0.6/openlrc/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0     4301 2023-06-09 22:40:37.156767 openlrc-0.0.6/openlrc/chatbot.py
--rw-r--r--   0        0        0      532 2023-06-09 19:56:29.876606 openlrc-0.0.6/openlrc/exceptions.py
--rw-r--r--   0        0        0      195 2023-06-08 23:05:32.606247 openlrc-0.0.6/openlrc/logger.py
--rw-r--r--   0        0        0    10255 2023-06-11 20:26:56.200428 openlrc-0.0.6/openlrc/lrc.py
--rw-r--r--   0        0        0     3674 2023-06-11 20:24:01.584313 openlrc-0.0.6/openlrc/openlrc.py
--rw-r--r--   0        0        0     2168 2023-06-09 20:51:58.921408 openlrc-0.0.6/openlrc/prompter.py
--rw-r--r--   0        0        0     3924 2023-06-11 20:26:31.160612 openlrc-0.0.6/openlrc/transcribe.py
--rw-r--r--   0        0        0     4610 2023-06-11 16:23:10.962796 openlrc-0.0.6/openlrc/utils.py
--rw-r--r--   0        0        0     1112 2023-06-11 20:34:13.115312 openlrc-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1911 2023-06-11 20:33:03.084818 openlrc-0.0.6/README.md
--rw-r--r--   0        0        0     3092 1970-01-01 00:00:00.000000 openlrc-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-10 10:20:06.659160 openlrc-0.1.0/LICENSE
+-rw-r--r--   0        0        0      106 2023-06-09 13:01:57.605311 openlrc-0.1.0/openlrc/__init__.py
+-rw-r--r--   0        0        0      257 2023-06-09 13:43:55.157439 openlrc-0.1.0/openlrc/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5287 2023-06-15 10:23:25.757313 openlrc-0.1.0/openlrc/__pycache__/chatbot.cpython-310.pyc
+-rw-r--r--   0        0        0     1031 2023-06-09 20:00:35.708506 openlrc-0.1.0/openlrc/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0      340 2023-06-12 12:38:01.595807 openlrc-0.1.0/openlrc/__pycache__/logger.cpython-310.pyc
+-rw-r--r--   0        0        0     3725 2023-06-15 08:09:05.872049 openlrc-0.1.0/openlrc/__pycache__/openlrc.cpython-310.pyc
+-rw-r--r--   0        0        0     4618 2023-06-14 15:51:24.457572 openlrc-0.1.0/openlrc/__pycache__/opt.cpython-310.pyc
+-rw-r--r--   0        0        0     6760 2023-06-15 08:09:13.804807 openlrc-0.1.0/openlrc/__pycache__/prompter.cpython-310.pyc
+-rw-r--r--   0        0        0     3340 2023-06-15 08:09:06.043276 openlrc-0.1.0/openlrc/__pycache__/subtitle.cpython-310.pyc
+-rw-r--r--   0        0        0     4064 2023-06-15 08:52:50.310738 openlrc-0.1.0/openlrc/__pycache__/transcribe.cpython-310.pyc
+-rw-r--r--   0        0        0     4497 2023-06-15 08:09:13.606018 openlrc-0.1.0/openlrc/__pycache__/translate.cpython-310.pyc
+-rw-r--r--   0        0        0     3558 2023-06-15 08:09:06.045276 openlrc-0.1.0/openlrc/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     5906 2023-06-15 10:23:11.726062 openlrc-0.1.0/openlrc/chatbot.py
+-rw-r--r--   0        0        0      532 2023-06-09 19:56:29.876606 openlrc-0.1.0/openlrc/exceptions.py
+-rw-r--r--   0        0        0      197 2023-06-12 10:09:17.659287 openlrc-0.1.0/openlrc/logger.py
+-rw-r--r--   0        0        0     5103 2023-06-15 08:09:05.053025 openlrc-0.1.0/openlrc/openlrc.py
+-rw-r--r--   0        0        0     4435 2023-06-14 15:50:59.059792 openlrc-0.1.0/openlrc/opt.py
+-rw-r--r--   0        0        0     6863 2023-06-15 10:45:04.241536 openlrc-0.1.0/openlrc/prompter.py
+-rw-r--r--   0        0        0     2523 2023-06-15 08:09:05.047514 openlrc-0.1.0/openlrc/subtitle.py
+-rw-r--r--   0        0        0     5676 2023-06-15 08:52:38.231073 openlrc-0.1.0/openlrc/transcribe.py
+-rw-r--r--   0        0        0     5404 2023-06-15 08:09:05.050068 openlrc-0.1.0/openlrc/translate.py
+-rw-r--r--   0        0        0     2488 2023-06-15 08:08:08.742912 openlrc-0.1.0/openlrc/utils.py
+-rw-r--r--   0        0        0     1113 2023-06-15 10:50:01.537808 openlrc-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2046 2023-06-15 07:10:10.168150 openlrc-0.1.0/README.md
+-rw-r--r--   0        0        0     3225 1970-01-01 00:00:00.000000 openlrc-0.1.0/PKG-INFO
```

### Comparing `openlrc-0.0.6/LICENSE` & `openlrc-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openlrc-0.0.6/openlrc/__pycache__/exceptions.cpython-310.pyc` & `openlrc-0.1.0/openlrc/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `openlrc-0.0.6/openlrc/__pycache__/openlrc.cpython-310.pyc` & `openlrc-0.1.0/openlrc/__pycache__/openlrc.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jun 11 19:26:28 2023 UTC, .py size: 3686 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,183 +1,233 @@
-00000000: 6f0d 0d0a 0000 0000 e41f 8664 660e 0000  o..........df...
+00000000: 6f0d 0d0a 0000 0000 21c7 8a64 ef13 0000  o.......!..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
+00000020: 0003 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
-00000050: 6d05 5a05 6d06 5a06 0100 6400 6404 6c07  m.Z.m.Z...d.d.l.
-00000060: 6d08 5a08 0100 6400 6405 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
-00000070: 0100 6400 6406 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
-00000080: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 0100 4700  m.Z.m.Z.m.Z...G.
-00000090: 6407 6408 8400 6408 8302 5a11 6401 5300  d.d...d...Z.d.S.
-000000a0: 2909 e900 0000 004e 2901 da06 6c6f 6767  )......N)...logg
-000000b0: 6572 2902 da03 4c52 43da 0c4c 5243 4f70  er)...LRC..LRCOp
-000000c0: 7469 6d69 7a65 7229 01da 0c70 726f 6d70  timizer)...promp
-000000d0: 7465 725f 6d61 7029 01da 0b54 7261 6e73  ter_map)...Trans
-000000e0: 6372 6962 6572 2905 da05 5469 6d65 72da  criber)...Timer.
-000000f0: 0a63 6861 6e67 655f 6578 74da 0f65 7874  .change_ext..ext
-00000100: 656e 645f 6669 6c65 6e61 6d65 da12 6765  end_filename..ge
-00000110: 745f 6175 6469 6f5f 6475 7261 7469 6f6e  t_audio_duration
-00000120: da10 666f 726d 6174 5f74 696d 6573 7461  ..format_timesta
-00000130: 6d70 6300 0000 0000 0000 0000 0000 0000  mpc.............
-00000140: 0000 0004 0000 0040 0000 0073 3a00 0000  .......@...s:...
-00000150: 6500 5a01 6400 5a02 640e 6402 6403 8401  e.Z.d.Z.d.d.d...
-00000160: 5a03 640f 6406 6407 8401 5a04 6505 6408  Z.d.d.d...Z.e.d.
-00000170: 6409 8400 8301 5a06 6505 6410 640c 640d  d.....Z.e.d.d.d.
-00000180: 8401 8301 5a07 640a 5300 2911 da05 4c52  ....Z.d.S.)...LR
-00000190: 4365 72fa 086c 6172 6765 2d76 3263 0200  Cer..large-v2c..
-000001a0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-000001b0: 0000 4300 0000 7310 0000 0074 007c 0164  ..C...s....t.|.d
-000001c0: 018d 017c 005f 0164 0053 0029 024e 2901  ...|._.d.S.).N).
-000001d0: da0a 6d6f 6465 6c5f 6e61 6d65 2902 7206  ..model_name).r.
-000001e0: 0000 00da 0b74 7261 6e73 6372 6962 6572  .....transcriber
-000001f0: 2902 da04 7365 6c66 720e 0000 00a9 0072  )...selfr......r
-00000200: 1100 0000 fa32 463a 5c57 6f72 6b73 7061  .....2F:\Workspa
-00000210: 6365 5c70 7974 686f 6e5c 4f70 656e 2d4c  ce\python\Open-L
-00000220: 7972 6963 735c 6f70 656e 6c72 635c 6f70  yrics\openlrc\op
-00000230: 656e 6c72 632e 7079 da08 5f5f 696e 6974  enlrc.py..__init
-00000240: 5f5f 0d00 0000 7302 0000 0010 017a 0e4c  __....s......z.L
-00000250: 5243 6572 2e5f 5f69 6e69 745f 5ffa 057a  RCer.__init__..z
-00000260: 682d 636e da0a 6261 7365 5f74 7261 6e73  h-cn..base_trans
-00000270: 6304 0000 0000 0000 0000 0000 000b 0000  c...............
-00000280: 0008 0000 0043 0000 0073 5e01 0000 7c03  .....C...s^...|.
-00000290: 7400 7601 720c 7401 6401 7c03 9b00 6402  t.v.r.t.d.|...d.
-000002a0: 9d03 8301 8201 7400 7c03 1900 8300 7d03  ......t.|.....}.
-000002b0: 7402 7403 7c01 6403 8302 6404 8302 7d04  t.t.|.d...d...}.
-000002c0: 7404 6a05 a006 7c04 a101 7371 7407 a008  t.j...|...sqt...
-000002d0: 6405 7c04 9b00 9d02 a101 0100 7409 6406  d.|.........t.d.
-000002e0: 8301 8f34 0100 7407 a008 6407 7c01 9b00  ...4..t...d.|...
-000002f0: 6408 740a 7c01 8301 9b00 9d04 a101 0100  d.t.|...........
-00000300: 7c00 6a0b 6a0c 7c01 6409 640a 8d02 5c02  |.j.j.|.d.d...\.
-00000310: 7d05 7d06 7407 a008 640b 7c06 6a0d 9b00  }.}.t...d.|.j...
-00000320: 9d02 a101 0100 7c05 640c 1900 7d07 7407  ......|.d...}.t.
-00000330: a00e 640d 7c07 9b00 9d02 a101 0100 5700  ..d.|.........W.
-00000340: 6400 0400 0400 8303 0100 6e08 3100 7362  d.........n.1.sb
-00000350: 7701 0100 0100 0100 5900 0100 7c00 6a0f  w.......Y...|.j.
-00000360: 7c07 7c04 7c06 6a0d 640e 8d03 0100 6e08  |.|.|.j.d.....n.
-00000370: 7407 a008 640f 7c04 9b00 9d02 a101 0100  t...d.|.........
-00000380: 7c00 a010 7c04 a101 7d08 7411 7c08 8301  |...|...}.t.|...
-00000390: 7d09 7409 6410 8301 8f0f 0100 7c09 6a12  }.t.d.......|.j.
-000003a0: 7c03 7c02 6411 8d02 7d0a 5700 6400 0400  |.|.d...}.W.d...
-000003b0: 0400 8303 0100 6e08 3100 7398 7701 0100  ......n.1.s.w...
-000003c0: 0100 0100 5900 0100 7c00 6a10 7c0a 7402  ....Y...|.j.|.t.
-000003d0: 7c01 6404 8302 7c02 6412 6b02 7c08 7c0a  |.d...|.d.k.|.|.
-000003e0: 6702 6413 8d04 0100 6400 5300 2914 4e7a  g.d.....d.S.).Nz
-000003f0: 0950 726f 6d70 7465 7220 7a0b 206e 6f74  .Prompter z. not
-00000400: 2066 6f75 6e64 2e5a 0c5f 7472 616e 7363   found.Z._transc
-00000410: 7269 6265 64da 036c 7263 7a20 4e6f 7420  ribed..lrcz Not 
-00000420: 666f 756e 6420 7472 616e 7363 7269 6265  found transcribe
-00000430: 6420 6c72 6320 6669 6c65 3a20 7a0f 5472  d lrc file: z.Tr
-00000440: 616e 7363 7269 6269 6e67 2e2e 2e7a 0e41  anscribing...z.A
-00000450: 7564 696f 206c 656e 6774 683a 207a 023a  udio length: z.:
-00000460: 20e9 0200 0000 2901 5a0a 6261 7463 685f   .....).Z.batch_
-00000470: 7369 7a65 7a13 4465 7465 6374 6564 206c  sizez.Detected l
-00000480: 616e 6775 6167 653a 205a 0973 656e 7465  anguage: Z.sente
-00000490: 6e63 6573 7a23 5472 616e 7363 7269 6265  ncesz#Transcribe
-000004a0: 6420 6661 7374 2d77 6869 7370 6572 2053  d fast-whisper S
-000004b0: 6567 6d65 6e74 733a 2029 02da 046e 616d  egments: )...nam
-000004c0: 65da 046c 616e 677a 1c46 6f75 6e64 2074  e..langz.Found t
-000004d0: 7261 6e73 6372 6962 6564 206c 7263 2066  ranscribed lrc f
-000004e0: 696c 653a 207a 0e54 7261 6e73 6c61 7469  ile: z.Translati
-000004f0: 6e67 2e2e 2e29 02da 0870 726f 6d70 7465  ng...)...prompte
-00000500: 72da 0b74 6172 6765 745f 6c61 6e67 7214  r..target_langr.
-00000510: 0000 0029 03da 0f6f 7574 7075 745f 6c72  ...)...output_lr
-00000520: 635f 6e61 6d65 da03 7432 6dda 0c72 656d  c_name..t2m..rem
-00000530: 6f76 655f 6669 6c65 7329 1372 0500 0000  ove_files).r....
-00000540: da0a 5661 6c75 6545 7272 6f72 7208 0000  ..ValueErrorr...
-00000550: 0072 0900 0000 da02 6f73 da04 7061 7468  .r......os..path
-00000560: da06 6578 6973 7473 7202 0000 00da 0469  ..existsr......i
-00000570: 6e66 6f72 0700 0000 720a 0000 0072 0f00  nfor....r....r..
-00000580: 0000 5a0a 7472 616e 7363 7269 6265 da08  ..Z.transcribe..
-00000590: 6c61 6e67 7561 6765 da05 6465 6275 67da  language..debug.
-000005a0: 0674 6f5f 6c72 63da 0c70 6f73 745f 7072  .to_lrc..post_pr
-000005b0: 6f63 6573 7372 0300 0000 da09 7472 616e  ocessr......tran
-000005c0: 736c 6174 6529 0b72 1000 0000 5a0a 6175  slate).r....Z.au
-000005d0: 6469 6f5f 7061 7468 721b 0000 0072 1a00  dio_pathr....r..
-000005e0: 0000 5a14 7472 616e 7363 7269 6265 645f  ..Z.transcribed_
-000005f0: 6c72 635f 7061 7468 da08 7365 676d 656e  lrc_path..segmen
-00000600: 7473 7223 0000 005a 0873 6567 5f6c 6973  tsr#...Z.seg_lis
-00000610: 745a 1a74 7261 6e73 6372 6962 6564 5f6f  tZ.transcribed_o
-00000620: 7074 696d 697a 6564 5f70 6174 685a 1974  ptimized_pathZ.t
-00000630: 7261 6e73 6372 6962 6564 5f6f 7074 696d  ranscribed_optim
-00000640: 697a 6564 5f6c 7263 da08 6c72 635f 6e61  ized_lrc..lrc_na
-00000650: 6d65 7211 0000 0072 1100 0000 7212 0000  mer....r....r...
-00000660: 00da 085f 5f63 616c 6c5f 5f10 0000 0073  ...__call__....s
-00000670: 3600 0000 0801 1001 0a01 1002 0c01 1001  6...............
-00000680: 0a01 1a01 1401 1201 0803 1201 1cf9 140a  ................
-00000690: 1002 0a02 0803 0a02 0401 0401 08ff 1cff  ................
-000006a0: 1405 0202 0201 02fe 0aff 7a0e 4c52 4365  ..........z.LRCe
-000006b0: 722e 5f5f 6361 6c6c 5f5f 6303 0000 0000  r.__call__c.....
-000006c0: 0000 0000 0000 0006 0000 0008 0000 0043  ...............C
-000006d0: 0000 0073 b400 0000 7400 7c01 6401 6402  ...s....t.|.d.d.
-000006e0: 6403 8d03 8f41 7d03 7401 6404 7c02 9b00  d....A}.t.d.|...
-000006f0: 9d02 7c03 6405 6406 8d03 0100 7402 7c00  ..|.d.d.....t.|.
-00000700: 8301 4400 5d2a 5c02 7d04 7d05 7401 6407  ..D.]*\.}.}.t.d.
-00000710: 7403 7c05 6408 1900 6409 1900 8301 9b00  t.|.d...d.......
-00000720: 640a 7c05 640b 1900 9b00 9d04 7c03 6405  d.|.d.......|.d.
-00000730: 6406 8d03 0100 7401 6407 7403 7c05 640c  d.....t.d.t.|.d.
-00000740: 1900 640d 1900 8301 9b00 640e 9d03 7c03  ..d.......d...|.
-00000750: 6405 6406 8d03 0100 7116 5700 640f 0400  d.d.....q.W.d...
-00000760: 0400 8303 0100 6e08 3100 734b 7701 0100  ......n.1.sKw...
-00000770: 0100 0100 5900 0100 7404 a005 6410 7c01  ....Y...t...d.|.
-00000780: 9b00 9d02 a101 0100 640f 5300 2911 7a37  ........d.S.).z7
-00000790: 0a20 2020 2020 2020 2043 6f6e 7665 7274  .        Convert
-000007a0: 2074 6865 2073 6567 6d65 6e74 7320 696e   the segments in
-000007b0: 746f 206c 7263 2066 6f72 6d61 742e 0a20  to lrc format.. 
-000007c0: 2020 2020 2020 20da 0177 7a05 7574 662d         ..wz.utf-
-000007d0: 3829 01da 0865 6e63 6f64 696e 677a 3e4c  8)...encodingz>L
-000007e0: 5243 2067 656e 6572 6174 6564 2062 7920  RC generated by 
-000007f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000800: 6f6d 2f7a 682d 706c 7573 2f4f 7065 6e2d  om/zh-plus/Open-
-00000810: 4c79 7269 6373 2c20 6c61 6e67 3d54 2902  Lyrics, lang=T).
-00000820: da04 6669 6c65 da05 666c 7573 68fa 015b  ..file..flush..[
-00000830: 5a0a 7374 6172 745f 776f 7264 da05 7374  Z.start_word..st
-00000840: 6172 747a 025d 20da 0474 6578 745a 0865  artz.] ..textZ.e
-00000850: 6e64 5f77 6f72 64da 0365 6e64 fa01 5d4e  nd_word..end..]N
-00000860: 7a0e 4669 6c65 2073 6176 6564 2074 6f20  z.File saved to 
-00000870: 2906 da04 6f70 656e da05 7072 696e 74da  )...open..print.
-00000880: 0965 6e75 6d65 7261 7465 720b 0000 0072  .enumerater....r
-00000890: 0200 0000 7223 0000 0029 0672 2900 0000  ....r#...).r)...
-000008a0: 7218 0000 0072 1900 0000 da01 66da 0169  r....r......f..i
-000008b0: da07 7365 676d 656e 7472 1100 0000 7211  ..segmentr....r.
-000008c0: 0000 0072 1200 0000 7226 0000 0036 0000  ...r....r&...6..
-000008d0: 0073 1800 0000 1005 1401 1001 0201 1e01  .s..............
-000008e0: 0201 0201 06fd 2406 02f9 1cfe 140b 7a0c  ......$.......z.
-000008f0: 4c52 4365 722e 746f 5f6c 7263 4e46 6304  LRCer.to_lrcNFc.
-00000900: 0000 0000 0000 0000 0000 0007 0000 0004  ................
-00000910: 0000 0043 0000 0073 3c00 0000 7400 7c00  ...C...s<...t.|.
-00000920: 8301 7d04 7c04 6a01 7c03 6401 8d01 0100  ..}.|.j.|.d.....
-00000930: 7c04 6a02 7c01 6402 8d01 7d05 7c02 721c  |.j.|.d...}.|.r.
-00000940: 7c02 4400 5d07 7d06 7403 a004 7c06 a101  |.D.].}.t...|...
-00000950: 0100 7114 7c05 5300 2903 4e29 0172 1d00  ..q.|.S.).N).r..
-00000960: 0000 2901 721c 0000 0029 0572 0400 0000  ..).r....).r....
-00000970: 5a0b 7065 7266 6f72 6d5f 616c 6cda 0473  Z.perform_all..s
-00000980: 6176 6572 2000 0000 da06 7265 6d6f 7665  aver .....remove
-00000990: 2907 722a 0000 0072 1c00 0000 721e 0000  ).r*...r....r...
-000009a0: 0072 1d00 0000 5a0d 6c72 635f 6f70 7469  .r....Z.lrc_opti
-000009b0: 6d69 7a65 725a 0e6f 7074 696d 697a 6564  mizerZ.optimized
-000009c0: 5f6e 616d 6572 2e00 0000 7211 0000 0072  _namer....r....r
-000009d0: 1100 0000 7212 0000 0072 2700 0000 4800  ....r....r'...H.
-000009e0: 0000 730e 0000 0008 020c 010c 0104 0308  ..s.............
-000009f0: 010c 0104 027a 124c 5243 6572 2e70 6f73  .....z.LRCer.pos
-00000a00: 745f 7072 6f63 6573 7329 0172 0d00 0000  t_process).r....
-00000a10: 2902 7214 0000 0072 1500 0000 2903 4e4e  ).r....r....).NN
-00000a20: 4629 08da 085f 5f6e 616d 655f 5fda 0a5f  F)...__name__.._
-00000a30: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00000a40: 6c6e 616d 655f 5f72 1300 0000 722b 0000  lname__r....r+..
-00000a50: 00da 0c73 7461 7469 636d 6574 686f 6472  ...staticmethodr
-00000a60: 2600 0000 7227 0000 0072 1100 0000 7211  &...r'...r....r.
-00000a70: 0000 0072 1100 0000 7212 0000 0072 0c00  ...r....r....r..
-00000a80: 0000 0c00 0000 730e 0000 0008 000a 010a  ......s.........
-00000a90: 0302 260a 0102 1110 0172 0c00 0000 2912  ..&......r....).
-00000aa0: 7220 0000 005a 076c 6962 726f 7361 da0e  r ...Z.librosa..
-00000ab0: 6f70 656e 6c72 632e 6c6f 6767 6572 7202  openlrc.loggerr.
-00000ac0: 0000 005a 0b6f 7065 6e6c 7263 2e6c 7263  ...Z.openlrc.lrc
-00000ad0: 7203 0000 0072 0400 0000 5a10 6f70 656e  r....r....Z.open
-00000ae0: 6c72 632e 7072 6f6d 7074 6572 7205 0000  lrc.prompterr...
-00000af0: 005a 126f 7065 6e6c 7263 2e74 7261 6e73  .Z.openlrc.trans
-00000b00: 6372 6962 6572 0600 0000 da0d 6f70 656e  criber......open
-00000b10: 6c72 632e 7574 696c 7372 0700 0000 7208  lrc.utilsr....r.
-00000b20: 0000 0072 0900 0000 720a 0000 0072 0b00  ...r....r....r..
-00000b30: 0000 720c 0000 0072 1100 0000 7211 0000  ..r....r....r...
-00000b40: 0072 1100 0000 7212 0000 00da 083c 6d6f  .r....r......<mo
-00000b50: 6475 6c65 3e01 0000 0073 1000 0000 0800  dule>....s......
-00000b60: 0802 0c02 1001 0c01 0c01 1c01 1203       ..............
+00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
+00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
+00000070: 6406 6c0a 6d0b 5a0b 0100 6400 6407 6c0c  d.l.m.Z...d.d.l.
+00000080: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10  m.Z.m.Z.m.Z.m.Z.
+00000090: 0100 4700 6408 6409 8400 6409 8302 5a11  ..G.d.d...d...Z.
+000000a0: 6401 5300 290a e900 0000 004e 2901 da06  d.S.)......N)...
+000000b0: 6c6f 6767 6572 2901 da11 5375 6274 6974  logger)...Subtit
+000000c0: 6c65 4f70 7469 6d69 7a65 7229 01da 0853  leOptimizer)...S
+000000d0: 7562 7469 746c 6529 01da 0b54 7261 6e73  ubtitle)...Trans
+000000e0: 6372 6962 6572 2901 da0a 5472 616e 736c  criber)...Transl
+000000f0: 6174 6f72 2904 da05 5469 6d65 72da 0a63  ator)...Timer..c
+00000100: 6861 6e67 655f 6578 74da 0f65 7874 656e  hange_ext..exten
+00000110: 645f 6669 6c65 6e61 6d65 da12 6765 745f  d_filename..get_
+00000120: 6175 6469 6f5f 6475 7261 7469 6f6e 6300  audio_durationc.
+00000130: 0000 0000 0000 0000 0000 0000 0000 0004  ................
+00000140: 0000 0040 0000 0073 3e00 0000 6500 5a01  ...@...s>...e.Z.
+00000150: 6400 5a02 6401 5a03 6411 6404 6405 8401  d.Z.d.Z.d.d.d...
+00000160: 5a04 6412 6409 640a 8401 5a05 6506 640b  Z.d.d.d...Z.e.d.
+00000170: 640c 8400 8301 5a07 6506 6413 640f 6410  d.....Z.e.d.d.d.
+00000180: 8401 8301 5a08 640d 5300 2914 da05 4c52  ....Z.d.S.)...LR
+00000190: 4365 7261 9301 0000 0a20 2020 203a 6976  Cera.....    :iv
+000001a0: 6172 206d 6f64 656c 5f6e 616d 653a 204e  ar model_name: N
+000001b0: 616d 6520 6f66 2077 6869 7370 6572 206d  ame of whisper m
+000001c0: 6f64 656c 2028 7469 6e79 2c20 7469 6e79  odel (tiny, tiny
+000001d0: 2e65 6e2c 2062 6173 652c 2062 6173 652e  .en, base, base.
+000001e0: 656e 2c20 736d 616c 6c2c 2073 6d61 6c6c  en, small, small
+000001f0: 2e65 6e2c 206d 6564 6975 6d2c 0a20 2020  .en, medium,.   
+00000200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000210: 206d 6564 6975 6d2e 656e 2c20 6c61 7267   medium.en, larg
+00000220: 652d 7631 2c20 6f72 206c 6172 6765 2d76  e-v1, or large-v
+00000230: 3229 2057 6865 6e20 6120 7369 7a65 2069  2) When a size i
+00000240: 7320 636f 6e66 6967 7572 6564 2c20 7468  s configured, th
+00000250: 6520 636f 6e76 6572 7465 6420 6d6f 6465  e converted mode
+00000260: 6c20 6973 2064 6f77 6e6c 6f61 6465 640a  l is downloaded.
+00000270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000280: 2020 2020 6672 6f6d 2074 6865 2048 7567      from the Hug
+00000290: 6769 6e67 2046 6163 6520 4875 622e 0a20  ging Face Hub.. 
+000002a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002b0: 2020 2044 6566 6175 6c74 3a20 6060 6c61     Default: ``la
+000002c0: 7267 652d 7632 6060 0a20 2020 203a 6976  rge-v2``.    :iv
+000002d0: 6172 2066 6565 5f6c 696d 6974 3a20 5468  ar fee_limit: Th
+000002e0: 6520 6d61 7869 6d75 6d20 6665 6520 796f  e maximum fee yo
+000002f0: 7520 6172 6520 7769 6c6c 696e 6720 746f  u are willing to
+00000300: 2070 6179 2066 6f72 2074 7261 6e73 6c61   pay for transla
+00000310: 7469 6f6e 2e20 4465 6661 756c 743a 2060  tion. Default: `
+00000320: 6030 2e31 6060 0a20 2020 20fa 086c 6172  `0.1``.    ..lar
+00000330: 6765 2d76 32e7 9a99 9999 9999 b93f 6303  ge-v2........?c.
+00000340: 0000 0000 0000 0000 0000 0003 0000 0003  ................
+00000350: 0000 0043 0000 0073 1600 0000 7400 7c01  ...C...s....t.|.
+00000360: 6401 8d01 7c00 5f01 7c02 7c00 5f02 6400  d...|._.|.|._.d.
+00000370: 5300 2902 4e29 01da 0a6d 6f64 656c 5f6e  S.).N)...model_n
+00000380: 616d 6529 0372 0500 0000 da0b 7472 616e  ame).r......tran
+00000390: 7363 7269 6265 72da 0966 6565 5f6c 696d  scriber..fee_lim
+000003a0: 6974 2903 da04 7365 6c66 720e 0000 0072  it)...selfr....r
+000003b0: 1000 0000 a900 7212 0000 00fa 3246 3a5c  ......r.....2F:\
+000003c0: 576f 726b 7370 6163 655c 7079 7468 6f6e  Workspace\python
+000003d0: 5c4f 7065 6e2d 4c79 7269 6373 5c6f 7065  \Open-Lyrics\ope
+000003e0: 6e6c 7263 5c6f 7065 6e6c 7263 2e70 79da  nlrc\openlrc.py.
+000003f0: 085f 5f69 6e69 745f 5f15 0000 0073 0400  .__init__....s..
+00000400: 0000 0c01 0a01 7a0e 4c52 4365 722e 5f5f  ......z.LRCer.__
+00000410: 696e 6974 5f5f fa05 7a68 2d63 6eda 0a62  init__..zh-cn..b
+00000420: 6173 655f 7472 616e 73da 0541 6e69 6d65  ase_trans..Anime
+00000430: 6305 0000 0000 0000 0000 0000 0012 0000  c...............
+00000440: 000b 0000 0043 0000 0073 ee01 0000 7400  .....C...s....t.
+00000450: 7401 7c01 6401 8302 6402 8302 7d05 7402  t.|.d...d...}.t.
+00000460: 6a03 a004 7c05 a101 7358 7405 6403 8301  j...|...sXt.d...
+00000470: 8f34 0100 7406 a007 6404 7c01 9b00 6405  .4..t...d.|...d.
+00000480: 7408 7c01 8301 9b00 9d04 a101 0100 7c00  t.|...........|.
+00000490: 6a09 6a0a 7c01 6406 6407 8d02 5c02 7d06  j.j.|.d.d...\.}.
+000004a0: 7d07 7406 a007 6408 7c07 6a0b 9b00 9d02  }.t...d.|.j.....
+000004b0: a101 0100 7c06 6409 1900 7d08 7406 a00c  ....|.d...}.t...
+000004c0: 640a 7c08 9b00 9d02 a101 0100 5700 6400  d.|.........W.d.
+000004d0: 0400 0400 8303 0100 6e08 3100 7349 7701  ........n.1.sIw.
+000004e0: 0100 0100 0100 5900 0100 7c00 6a0d 7c08  ......Y...|.j.|.
+000004f0: 7c05 7c07 6a0b 640b 8d03 0100 6e08 7406  |.|.j.d.....n.t.
+00000500: a007 640c 7c05 9b00 9d02 a101 0100 740e  ..d.|.........t.
+00000510: 7c05 8301 7d09 7c00 6a0f 7c09 640d 640e  |...}.|.j.|.d.d.
+00000520: 8d02 7d0a 7401 7c0a 6a10 640f 8302 7d0b  ..}.t.|.j.d...}.
+00000530: 7402 6a03 a004 7c0b a101 73c4 7411 7c03  t.j...|...s.t.|.
+00000540: 7c00 6a12 6410 8d02 7d0c 7405 6411 8301  |.j.d...}.t.d...
+00000550: 8f39 0100 7a0e 7c0c 6a13 7c0a a014 a100  .9..z.|.j.|.....
+00000560: 7c0a 6a15 7c02 7c04 6412 8d04 7d0d 5700  |.j.|.|.d...}.W.
+00000570: 6e16 0400 7416 79a7 0100 7d0e 0100 7a0a  n...t.y...}...z.
+00000580: 7406 a017 6413 7c0a 9b00 9d02 a101 0100  t...d.|.........
+00000590: 7c0e 8201 6400 7d0e 7e0e 7701 7700 7c0a  |...d.}.~.w.w.|.
+000005a0: a018 7c0d a101 0100 7c0a 6a19 7c0b 640d  ..|.....|.j.|.d.
+000005b0: 640e 8d02 0100 5700 6400 0400 0400 8303  d.....W.d.......
+000005c0: 0100 6e08 3100 73be 7701 0100 0100 0100  ..n.1.s.w.......
+000005d0: 5900 0100 6e08 7406 a007 640c 7c0b 9b00  Y...n.t...d.|...
+000005e0: 9d02 a101 0100 740e 7c0b 8301 7d0f 7c03  ......t.|...}.|.
+000005f0: a01a 6414 a101 72de 7400 7401 7c01 6415  ..d...r.t.t.|.d.
+00000600: 8302 6402 8302 7d10 6e05 7400 7c01 6402  ..d...}.n.t.|.d.
+00000610: 8302 7d10 7c00 6a0f 7c0f 7c10 7c02 6416  ..}.|.j.|.|.|.d.
+00000620: 6b02 7c0a 6a10 6701 640d 6417 8d05 7d11  k.|.j.g.d.d...}.
+00000630: 7c11 a01b a100 0100 6400 5300 2918 4e5a  |.......d.S.).NZ
+00000640: 0c5f 7472 616e 7363 7269 6265 64da 046a  ._transcribed..j
+00000650: 736f 6e7a 1554 7261 6e73 6372 6970 7469  sonz.Transcripti
+00000660: 6f6e 2070 726f 6365 7373 7a0e 4175 6469  on processz.Audi
+00000670: 6f20 6c65 6e67 7468 3a20 7a02 3a20 e904  o length: z.: ..
+00000680: 0000 0029 01da 0a62 6174 6368 5f73 697a  ...)...batch_siz
+00000690: 657a 1344 6574 6563 7465 6420 6c61 6e67  ez.Detected lang
+000006a0: 7561 6765 3a20 5a09 7365 6e74 656e 6365  uage: Z.sentence
+000006b0: 737a 2354 7261 6e73 6372 6962 6564 2066  sz#Transcribed f
+000006c0: 6173 742d 7768 6973 7065 7220 5365 676d  ast-whisper Segm
+000006d0: 656e 7473 3a20 2902 da04 6e61 6d65 da04  ents: )...name..
+000006e0: 6c61 6e67 7a1d 466f 756e 6420 7472 616e  langz.Found tran
+000006f0: 7363 7269 6265 6420 6a73 6f6e 2066 696c  scribed json fil
+00000700: 653a 2054 a901 da0b 7570 6461 7465 5f6e  e: T....update_n
+00000710: 616d 655a 0b5f 7472 616e 736c 6174 6564  ameZ._translated
+00000720: 2902 da08 7072 6f6d 7074 6572 7210 0000  )...prompterr...
+00000730: 007a 0e54 7261 6e73 6c61 7469 6e67 2e2e  .z.Translating..
+00000740: 2e29 035a 0873 7263 5f6c 616e 67da 0b74  .).Z.src_lang..t
+00000750: 6172 6765 745f 6c61 6e67 da0a 6175 6469  arget_lang..audi
+00000760: 6f5f 7479 7065 7a15 4661 696c 6564 2074  o_typez.Failed t
+00000770: 6f20 7472 616e 736c 6174 653a 20da 0276  o translate: ..v
+00000780: 325a 035f 7632 7215 0000 0029 04da 0b6f  2Z._v2r....)...o
+00000790: 7574 7075 745f 6e61 6d65 da03 7432 6dda  utput_name..t2m.
+000007a0: 0c72 656d 6f76 655f 6669 6c65 7372 1e00  .remove_filesr..
+000007b0: 0000 291c 7208 0000 0072 0900 0000 da02  ..).r....r......
+000007c0: 6f73 da04 7061 7468 da06 6578 6973 7473  os..path..exists
+000007d0: 7207 0000 0072 0200 0000 da04 696e 666f  r....r......info
+000007e0: 720a 0000 0072 0f00 0000 5a0a 7472 616e  r....r....Z.tran
+000007f0: 7363 7269 6265 da08 6c61 6e67 7561 6765  scribe..language
+00000800: da05 6465 6275 67da 0774 6f5f 6a73 6f6e  ..debug..to_json
+00000810: 7204 0000 00da 0c70 6f73 745f 7072 6f63  r......post_proc
+00000820: 6573 73da 0866 696c 656e 616d 6572 0600  ess..filenamer..
+00000830: 0000 7210 0000 00da 0974 7261 6e73 6c61  ..r......transla
+00000840: 7465 5a09 6765 745f 7465 7874 7372 1c00  teZ.get_textsr..
+00000850: 0000 da09 4578 6365 7074 696f 6eda 0565  ....Exception..e
+00000860: 7272 6f72 5a09 7365 745f 7465 7874 73da  rrorZ.set_texts.
+00000870: 0473 6176 65da 0865 6e64 7377 6974 685a  .save..endswithZ
+00000880: 0674 6f5f 6c72 6329 1272 1100 0000 5a0a  .to_lrc).r....Z.
+00000890: 6175 6469 6f5f 7061 7468 7220 0000 0072  audio_pathr ...r
+000008a0: 1f00 0000 7221 0000 005a 1074 7261 6e73  ....r!...Z.trans
+000008b0: 6372 6962 6564 5f70 6174 68da 0873 6567  cribed_path..seg
+000008c0: 6d65 6e74 7372 2900 0000 5a08 7365 675f  mentsr)...Z.seg_
+000008d0: 6c69 7374 da0f 7472 616e 7363 7269 6265  list..transcribe
+000008e0: 645f 7375 625a 1374 7261 6e73 6372 6962  d_subZ.transcrib
+000008f0: 6564 5f6f 7074 5f73 7562 5a0f 7472 616e  ed_opt_subZ.tran
+00000900: 736c 6174 6564 5f70 6174 685a 0a74 7261  slated_pathZ.tra
+00000910: 6e73 6c61 746f 725a 0c74 6172 6765 745f  nslatorZ.target_
+00000920: 7465 7874 73da 0165 5a0e 7472 616e 736c  texts..eZ.transl
+00000930: 6174 6564 5f73 7562 5a0f 6f75 7470 7574  ated_subZ.output
+00000940: 5f66 696c 656e 616d 655a 0e66 696e 616c  _filenameZ.final
+00000950: 5f73 7562 7469 746c 6572 1200 0000 7212  _subtitler....r.
+00000960: 0000 0072 1300 0000 da08 5f5f 6361 6c6c  ...r......__call
+00000970: 5f5f 1900 0000 7356 0000 0010 010c 010a  __....sV........
+00000980: 011a 0114 0112 0108 0312 011c f914 0a10  ................
+00000990: 0208 020e 010c 030c 010e 020a 0202 010a  ................
+000009a0: 0104 0102 0102 010a fd0e 0410 0104 0108  ................
+000009b0: 8002 fe0a 0410 031c f302 8010 0f08 020a  ................
+000009c0: 0212 010a 020e 0204 0202 ff02 0206 fd0c  ................
+000009d0: 047a 0e4c 5243 6572 2e5f 5f63 616c 6c5f  .z.LRCer.__call_
+000009e0: 5f63 0300 0000 0000 0000 0000 0000 0600  _c..............
+000009f0: 0000 0800 0000 4300 0000 7394 0000 0064  ......C...s....d
+00000a00: 017c 0267 0064 029c 037d 037c 0044 005d  .|.g.d...}.|.D.]
+00000a10: 177d 047c 0364 0319 00a0 007c 0464 0419  .}.|.d.....|.d..
+00000a20: 0064 0519 007c 0464 0619 0064 0719 007c  .d...|.d...d...|
+00000a30: 0464 0819 0064 099c 03a1 0101 0071 0874  .d...d.......q.t
+00000a40: 017c 0164 0a64 0b64 0c8d 038f 117d 0574  .|.d.d.d.....}.t
+00000a50: 026a 037c 037c 0564 0d64 0e64 0f8d 0401  .j.|.|.d.d.d....
+00000a60: 0057 0064 0004 0004 0083 0301 006e 0831  .W.d.........n.1
+00000a70: 0073 3b77 0101 0001 0001 0059 0001 0074  .s;w.......Y...t
+00000a80: 04a0 0564 107c 019b 009d 02a1 0101 007c  ...d.|.........|
+00000a90: 0353 0029 114e 7a37 4c52 4320 6765 6e65  .S.).Nz7LRC gene
+00000aa0: 7261 7465 6420 6279 2068 7474 7073 3a2f  rated by https:/
+00000ab0: 2f67 6974 6875 622e 636f 6d2f 7a68 2d70  /github.com/zh-p
+00000ac0: 6c75 732f 4f70 656e 2d4c 7972 6963 7329  lus/Open-Lyrics)
+00000ad0: 03da 0967 656e 6572 6174 6f72 722a 0000  ...generatorr*..
+00000ae0: 0072 3400 0000 7234 0000 005a 0a73 7461  .r4...r4...Z.sta
+00000af0: 7274 5f77 6f72 64da 0573 7461 7274 5a08  rt_word..startZ.
+00000b00: 656e 645f 776f 7264 da03 656e 64da 0474  end_word..end..t
+00000b10: 6578 7429 0372 3900 0000 723a 0000 0072  ext).r9...r:...r
+00000b20: 3b00 0000 da01 777a 0575 7466 2d38 2901  ;.....wz.utf-8).
+00000b30: da08 656e 636f 6469 6e67 4672 1900 0000  ..encodingFr....
+00000b40: 2902 da0c 656e 7375 7265 5f61 7363 6969  )...ensure_ascii
+00000b50: da06 696e 6465 6e74 7a0e 4669 6c65 2073  ..indentz.File s
+00000b60: 6176 6564 2074 6f20 2906 da06 6170 7065  aved to )...appe
+00000b70: 6e64 da04 6f70 656e 7218 0000 00da 0464  nd..openr......d
+00000b80: 756d 7072 0200 0000 7229 0000 0029 0672  umpr....r)...).r
+00000b90: 3400 0000 721b 0000 0072 1c00 0000 da06  4...r....r......
+00000ba0: 7265 7375 6c74 da07 7365 676d 656e 74da  result..segment.
+00000bb0: 0166 7212 0000 0072 1200 0000 7213 0000  .fr....r....r...
+00000bc0: 0072 2c00 0000 5100 0000 731e 0000 0002  .r,...Q...s.....
+00000bd0: 0302 0102 0106 fd08 0608 010a 010a 0106  ................
+00000be0: 010a fd10 0614 011c ff10 0304 027a 0d4c  .............z.L
+00000bf0: 5243 6572 2e74 6f5f 6a73 6f6e 4e46 6305  RCer.to_jsonNFc.
+00000c00: 0000 0000 0000 0000 0000 0007 0000 0004  ................
+00000c10: 0000 0043 0000 0073 4000 0000 7400 7c00  ...C...s@...t.|.
+00000c20: 8301 7d05 7c05 6a01 7c03 6401 8d01 0100  ..}.|.j.|.d.....
+00000c30: 7c05 6a02 7c01 7c04 6402 8d02 0100 7c02  |.j.|.|.d.....|.
+00000c40: 721d 7c02 4400 5d07 7d06 7403 a004 7c06  r.|.D.].}.t...|.
+00000c50: a101 0100 7115 7c05 6a05 5300 2903 4e29  ....q.|.j.S.).N)
+00000c60: 0172 2400 0000 721d 0000 0029 0672 0300  .r$...r....).r..
+00000c70: 0000 5a0b 7065 7266 6f72 6d5f 616c 6c72  ..Z.perform_allr
+00000c80: 3200 0000 7226 0000 00da 0672 656d 6f76  2...r&.....remov
+00000c90: 655a 0873 7562 7469 746c 6529 0772 3500  eZ.subtitle).r5.
+00000ca0: 0000 7223 0000 0072 2500 0000 7224 0000  ..r#...r%...r$..
+00000cb0: 0072 1e00 0000 5a09 6f70 7469 6d69 7a65  .r....Z.optimize
+00000cc0: 72da 0466 696c 6572 1200 0000 7212 0000  r..filer....r...
+00000cd0: 0072 1300 0000 722d 0000 0067 0000 0073  .r....r-...g...s
+00000ce0: 0e00 0000 0802 0c01 0e01 0403 0801 0c01  ................
+00000cf0: 0602 7a12 4c52 4365 722e 706f 7374 5f70  ..z.LRCer.post_p
+00000d00: 726f 6365 7373 2902 720c 0000 0072 0d00  rocess).r....r..
+00000d10: 0000 2903 7215 0000 0072 1600 0000 7217  ..).r....r....r.
+00000d20: 0000 0029 044e 4e46 4629 09da 085f 5f6e  ...).NNFF)...__n
+00000d30: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000d40: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
+00000d50: 075f 5f64 6f63 5f5f 7214 0000 0072 3700  .__doc__r....r7.
+00000d60: 0000 da0c 7374 6174 6963 6d65 7468 6f64  ....staticmethod
+00000d70: 722c 0000 0072 2d00 0000 7212 0000 0072  r,...r-...r....r
+00000d80: 1200 0000 7212 0000 0072 1300 0000 720b  ....r....r....r.
+00000d90: 0000 000c 0000 0073 1000 0000 0800 0401  .......s........
+00000da0: 0a08 0a04 0238 0a01 0215 1001 720b 0000  .....8......r...
+00000db0: 0029 1272 1800 0000 7226 0000 00da 0e6f  .).r....r&.....o
+00000dc0: 7065 6e6c 7263 2e6c 6f67 6765 7272 0200  penlrc.loggerr..
+00000dd0: 0000 5a0b 6f70 656e 6c72 632e 6f70 7472  ..Z.openlrc.optr
+00000de0: 0300 0000 5a10 6f70 656e 6c72 632e 7375  ....Z.openlrc.su
+00000df0: 6274 6974 6c65 7204 0000 005a 126f 7065  btitler....Z.ope
+00000e00: 6e6c 7263 2e74 7261 6e73 6372 6962 6572  nlrc.transcriber
+00000e10: 0500 0000 5a11 6f70 656e 6c72 632e 7472  ....Z.openlrc.tr
+00000e20: 616e 736c 6174 6572 0600 0000 da0d 6f70  anslater......op
+00000e30: 656e 6c72 632e 7574 696c 7372 0700 0000  enlrc.utilsr....
+00000e40: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+00000e50: 0b00 0000 7212 0000 0072 1200 0000 7212  ....r....r....r.
+00000e60: 0000 0072 1300 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000e70: 653e 0100 0000 7312 0000 0008 0008 010c  e>....s.........
+00000e80: 020c 010c 010c 010c 0118 0112 03         .............
```

### Comparing `openlrc-0.0.6/openlrc/exceptions.py` & `openlrc-0.1.0/openlrc/exceptions.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.0.6/pyproject.toml` & `openlrc-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [virtualenvs]
 create = true
 in-project = true
 
 [tool.poetry]
 name = "openlrc"
-version = "0.0.6"
+version = "0.1.0"
 description = "Transcribe (whisper) and translate (gpt) voice into LRC file."
 license = "MIT"
 authors = [
     "Hao Zheng <zhenghaosustc@gmail.com>"
 ]
 readme = "README.md"
 homepage = "https://github.com/zh-plus/Open-Lyrics"
@@ -38,12 +38,12 @@
 openai = "^0.27.6"
 faster-whisper = "^0.6.0"
 tiktoken = "^0.3.1"
 langcodes = "^3.3.0"
 language-data = "^1.1"
 rich = "^12.6.0"
 tqdm = "^4.65.0"
-librosa = "^0.10.0"
+audioread = "^3.0.0"
 opencc = "^1.1.1"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/zh-plus/Open-Lyrics/issues"
```

### Comparing `openlrc-0.0.6/README.md` & `openlrc-0.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -42,16 +42,18 @@
 ```
 
 ## Todo
 
 - [x] Batched translate/polish for GPT request (enable contextual ability).
 - [x] Concurrent support for GPT request.
 - [x] Use [whisperx](https://github.com/m-bain/whisperX) for transcription.
-- [ ] Automatically fix json encoder error using GPT.
-- [ ] Make translate prompt more robust.
+- [x] Make translate prompt more robust according to https://github.com/openai/openai-cookbook.
+- [x] Automatically fix json encoder error using GPT.
+- [ ] Multiple output format support.
+- [ ] Add Azure OpenAI Service support.
 - [ ] Add local LLM support.
 - [ ] Add transcribed examples.
     - [ ] Song
     - [ ] Podcast
     - [ ] Audiobook
 
 ## Credits
```

### Comparing `openlrc-0.0.6/PKG-INFO` & `openlrc-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlrc
-Version: 0.0.6
+Version: 0.1.0
 Summary: Transcribe (whisper) and translate (gpt) voice into LRC file.
 Home-page: https://github.com/zh-plus/Open-Lyrics
 License: MIT
 Keywords: openai-gpt3,whisper,voice transcribe,lrc
 Author: Hao Zheng
 Author-email: zhenghaosustc@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -13,18 +13,18 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
+Requires-Dist: audioread (>=3.0.0,<4.0.0)
 Requires-Dist: faster-whisper (>=0.6.0,<0.7.0)
 Requires-Dist: langcodes (>=3.3.0,<4.0.0)
 Requires-Dist: language-data (>=1.1,<2.0)
-Requires-Dist: librosa (>=0.10.0,<0.11.0)
 Requires-Dist: openai (>=0.27.6,<0.28.0)
 Requires-Dist: opencc (>=1.1.1,<2.0.0)
 Requires-Dist: rich (>=12.6.0,<13.0.0)
 Requires-Dist: tiktoken (>=0.3.1,<0.4.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/zh-plus/Open-Lyrics/issues
 Description-Content-Type: text/markdown
@@ -73,16 +73,18 @@
 ```
 
 ## Todo
 
 - [x] Batched translate/polish for GPT request (enable contextual ability).
 - [x] Concurrent support for GPT request.
 - [x] Use [whisperx](https://github.com/m-bain/whisperX) for transcription.
-- [ ] Automatically fix json encoder error using GPT.
-- [ ] Make translate prompt more robust.
+- [x] Make translate prompt more robust according to https://github.com/openai/openai-cookbook.
+- [x] Automatically fix json encoder error using GPT.
+- [ ] Multiple output format support.
+- [ ] Add Azure OpenAI Service support.
 - [ ] Add local LLM support.
 - [ ] Add transcribed examples.
     - [ ] Song
     - [ ] Podcast
     - [ ] Audiobook
 
 ## Credits
```

