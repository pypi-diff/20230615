# Comparing `tmp/mhi-psout-1.0.1.tar.gz` & `tmp/mhi-psout-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mhi-psout-1.0.1.tar", last modified: Thu Jan  5 20:46:58 2023, max compression
+gzip compressed data, was "mhi-psout-1.0.2.tar", last modified: Thu Jun 15 21:15:32 2023, max compression
```

## Comparing `mhi-psout-1.0.1.tar` & `mhi-psout-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-01-05 20:46:58.669935 mhi-psout-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-01-05 20:46:58.573743 mhi-psout-1.0.1/CurveFile/
--rw-rw-rw-   0        0        0    96224 2022-07-05 20:48:20.000000 mhi-psout-1.0.1/CurveFile/Interface.h
--rw-rw-rw-   0        0        0     1731 2022-07-05 20:46:10.000000 mhi-psout-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      116 2022-07-05 20:46:10.000000 mhi-psout-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1433 2023-01-05 20:46:58.669935 mhi-psout-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-01-05 20:46:58.619528 mhi-psout-1.0.1/PSOut/
--rw-rw-rw-   0        0        0    12160 2022-07-05 20:46:10.000000 mhi-psout-1.0.1/PSOut/Call.cpp
--rw-rw-rw-   0        0        0     3594 2022-07-05 20:46:10.000000 mhi-psout-1.0.1/PSOut/Closable.cpp
--rw-rw-rw-   0        0        0    12545 2022-07-05 20:46:10.000000 mhi-psout-1.0.1/PSOut/File.cpp
--rw-rw-rw-   0        0        0     2848 2022-07-05 20:46:10.000000 mhi-psout-1.0.1/PSOut/PSOut.cpp
--rw-rw-rw-   0        0        0    11417 2022-07-05 20:46:10.000000 mhi-psout-1.0.1/PSOut/PSOut.h
--rw-rw-rw-   0        0        0    11344 2022-07-05 20:46:10.000000 mhi-psout-1.0.1/PSOut/Run.cpp
--rw-rw-rw-   0        0        0    16962 2023-01-05 20:41:18.000000 mhi-psout-1.0.1/PSOut/Trace.cpp
--rw-rw-rw-   0        0        0    12410 2022-07-05 20:46:10.000000 mhi-psout-1.0.1/PSOut/VarList.cpp
--rw-rw-rw-   0        0        0      533 2022-07-05 20:46:10.000000 mhi-psout-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-01-05 20:46:58.630950 mhi-psout-1.0.1/Release/
--rw-rw-rw-   0        0        0    95744 2022-07-05 20:48:35.000000 mhi-psout-1.0.1/Release/CurveFile.dll
--rw-rw-rw-   0        0        0    31928 2022-07-05 20:48:32.000000 mhi-psout-1.0.1/Release/CurveFile.lib
--rw-rw-rw-   0        0        0      933 2023-01-05 20:46:58.673383 mhi-psout-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1585 2023-01-05 20:41:18.000000 mhi-psout-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-05 20:46:58.538331 mhi-psout-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-01-05 20:46:58.537334 mhi-psout-1.0.1/src/mhi/
-drwxrwxrwx   0        0        0        0 2023-01-05 20:46:58.642107 mhi-psout-1.0.1/src/mhi/psout/
--rw-rw-rw-   0        0        0    95744 2023-01-05 20:46:58.000000 mhi-psout-1.0.1/src/mhi/psout/CurveFile.dll
--rw-rw-rw-   0        0        0    12182 2023-01-05 20:41:58.000000 mhi-psout-1.0.1/src/mhi/psout/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-05 20:46:58.665549 mhi-psout-1.0.1/src/mhi_psout.egg-info/
--rw-rw-rw-   0        0        0     1433 2023-01-05 20:46:58.000000 mhi-psout-1.0.1/src/mhi_psout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      443 2023-01-05 20:46:58.000000 mhi-psout-1.0.1/src/mhi_psout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-05 20:46:58.000000 mhi-psout-1.0.1/src/mhi_psout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-01-05 20:46:58.000000 mhi-psout-1.0.1/src/mhi_psout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 21:15:32.743473 mhi-psout-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-15 21:15:32.581130 mhi-psout-1.0.2/CurveFile/
+-rw-rw-rw-   0        0        0    96224 2022-07-05 20:48:20.000000 mhi-psout-1.0.2/CurveFile/Interface.h
+-rw-rw-rw-   0        0        0     1731 2023-06-15 21:08:41.000000 mhi-psout-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      116 2022-07-05 20:46:10.000000 mhi-psout-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1433 2023-06-15 21:15:32.744471 mhi-psout-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 21:15:32.643740 mhi-psout-1.0.2/PSOut/
+-rw-rw-rw-   0        0        0    12160 2022-07-05 20:46:10.000000 mhi-psout-1.0.2/PSOut/Call.cpp
+-rw-rw-rw-   0        0        0     3594 2022-07-05 20:46:10.000000 mhi-psout-1.0.2/PSOut/Closable.cpp
+-rw-rw-rw-   0        0        0    12545 2022-07-05 20:46:10.000000 mhi-psout-1.0.2/PSOut/File.cpp
+-rw-rw-rw-   0        0        0     2848 2022-07-05 20:46:10.000000 mhi-psout-1.0.2/PSOut/PSOut.cpp
+-rw-rw-rw-   0        0        0    11417 2022-07-05 20:46:10.000000 mhi-psout-1.0.2/PSOut/PSOut.h
+-rw-rw-rw-   0        0        0    11344 2022-07-05 20:46:10.000000 mhi-psout-1.0.2/PSOut/Run.cpp
+-rw-rw-rw-   0        0        0    16962 2023-01-05 21:24:18.000000 mhi-psout-1.0.2/PSOut/Trace.cpp
+-rw-rw-rw-   0        0        0    12452 2023-06-15 21:08:41.000000 mhi-psout-1.0.2/PSOut/VarList.cpp
+-rw-rw-rw-   0        0        0      533 2022-07-05 20:46:10.000000 mhi-psout-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 21:15:32.659702 mhi-psout-1.0.2/Release/
+-rw-rw-rw-   0        0        0    95744 2023-06-15 20:16:19.000000 mhi-psout-1.0.2/Release/CurveFile.dll
+-rw-rw-rw-   0        0        0    31928 2023-06-15 20:16:13.000000 mhi-psout-1.0.2/Release/CurveFile.lib
+-rw-rw-rw-   0        0        0      933 2023-06-15 21:15:32.749458 mhi-psout-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1557 2023-06-15 21:08:41.000000 mhi-psout-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:15:32.537252 mhi-psout-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-15 21:15:32.536252 mhi-psout-1.0.2/src/mhi/
+drwxrwxrwx   0        0        0        0 2023-06-15 21:15:32.674657 mhi-psout-1.0.2/src/mhi/psout/
+-rw-rw-rw-   0        0        0    95744 2023-06-15 21:15:32.000000 mhi-psout-1.0.2/src/mhi/psout/CurveFile.dll
+-rw-rw-rw-   0        0        0    12182 2023-06-15 21:09:14.000000 mhi-psout-1.0.2/src/mhi/psout/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:15:32.704577 mhi-psout-1.0.2/src/mhi_psout.egg-info/
+-rw-rw-rw-   0        0        0     1433 2023-06-15 21:15:32.000000 mhi-psout-1.0.2/src/mhi_psout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      548 2023-06-15 21:15:32.000000 mhi-psout-1.0.2/src/mhi_psout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 21:15:32.000000 mhi-psout-1.0.2/src/mhi_psout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-15 21:15:32.000000 mhi-psout-1.0.2/src/mhi_psout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 21:15:32.736492 mhi-psout-1.0.2/tests/
+-rw-rw-rw-   0        0        0     2357 2022-07-05 20:46:10.000000 mhi-psout-1.0.2/tests/test_cigre.py
+-rw-rw-rw-   0        0        0     2000 2023-01-05 21:24:18.000000 mhi-psout-1.0.2/tests/test_psout_compliance.py
+-rw-rw-rw-   0        0        0      424 2022-07-05 20:46:10.000000 mhi-psout-1.0.2/tests/test_psout_devel.py
+-rw-rw-rw-   0        0        0     2033 2022-07-05 20:46:10.000000 mhi-psout-1.0.2/tests/test_psout_version.py
```

### Comparing `mhi-psout-1.0.1/CurveFile/Interface.h` & `mhi-psout-1.0.2/CurveFile/Interface.h`

 * *Files identical despite different names*

### Comparing `mhi-psout-1.0.1/LICENSE` & `mhi-psout-1.0.2/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The Clear BSD License
 
-Copyright 2022 Manitoba Hydro International Ltd.
+Copyright 2023 Manitoba Hydro International Ltd.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted (subject to the limitations in the disclaimer
 below) provided that the following conditions are met:
 
      * Redistributions of source code must retain the above copyright notice,
```

### Comparing `mhi-psout-1.0.1/PKG-INFO` & `mhi-psout-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mhi-psout
-Version: 1.0.1
+Version: 1.0.2
 Summary: Manitoba Hydro International: PSOUT File Reader
 Home-page: https://www.pscad.com/webhelp-v5-al/index.html
 Author: Manitoba Hydro International Ltd.
 Author-email: pscad@mhi.ca
 License: BSD-3-Clause-Clear
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mhi-psout-1.0.1/PSOut/Call.cpp` & `mhi-psout-1.0.2/PSOut/Call.cpp`

 * *Files identical despite different names*

### Comparing `mhi-psout-1.0.1/PSOut/Closable.cpp` & `mhi-psout-1.0.2/PSOut/Closable.cpp`

 * *Files identical despite different names*

### Comparing `mhi-psout-1.0.1/PSOut/File.cpp` & `mhi-psout-1.0.2/PSOut/File.cpp`

 * *Files identical despite different names*

### Comparing `mhi-psout-1.0.1/PSOut/PSOut.cpp` & `mhi-psout-1.0.2/PSOut/PSOut.cpp`

 * *Files identical despite different names*

### Comparing `mhi-psout-1.0.1/PSOut/PSOut.h` & `mhi-psout-1.0.2/PSOut/PSOut.h`

 * *Files identical despite different names*

### Comparing `mhi-psout-1.0.1/PSOut/Run.cpp` & `mhi-psout-1.0.2/PSOut/Run.cpp`

 * *Files identical despite different names*

### Comparing `mhi-psout-1.0.1/PSOut/Trace.cpp` & `mhi-psout-1.0.2/PSOut/Trace.cpp`

 * *Files identical despite different names*

### Comparing `mhi-psout-1.0.1/PSOut/VarList.cpp` & `mhi-psout-1.0.2/PSOut/VarList.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -121,27 +121,29 @@
          case RFVT_UInt32: object = PyLong_FromUnsignedLong(*(unsigned int *)p);    break;
          case RFVT_Int64: object = PyLong_FromLongLong(*(signed long long *) p); break;
          case RFVT_UInt64: object = PyLong_FromUnsignedLongLong(*(unsigned long long *) p);  break;
          case RFVT_Real32: object = PyFloat_FromDouble(*(float *)p);    break;
          case RFVT_Real64: object = PyFloat_FromDouble(*(double *)p);  break;
          case RFVT_Charater: object = PyUnicode_FromStringAndSize(p, 1); break;
          case RFVT_WideChar: object = PyUnicode_FromWideChar((wchar_t*)p, 1); break;
-         case RFVT_StringAscii: object = PyUnicode_FromStringAndSize(p, size - 1); break;
+         case RFVT_StringAscii: object = PyUnicode_DecodeUTF8(p, size - 1, "replace"); break;
          case RFVT_StringUnicode: object = PyUnicode_FromWideChar((wchar_t*)p, size / 2 - 1); break;
          case RFVT_Blob: object = PyBytes_FromStringAndSize(p, size); break;
          case RFVT_Complex64: object = PyComplex_FromDoubles(((float*)p)[0], ((float*)p)[1]); break;
          case RFVT_Complex128: object = PyComplex_FromDoubles(((double*)p)[0], ((double*)p)[1]); break;
          default:
             PyErr_Format(PyExc_NotImplementedError, "Variable Type not supported: type=%d size=%lld", type, size);
       }
    }
 
-   //if (type == RFVT_StringAscii) {
-   //   TRACE("      %s\n", p);
-   //}
+//#ifdef TRACE_VARLIST
+//   if (type == RFVT_StringAscii) {
+//      TRACE("      \"%s\"\n", p);
+//   }
+//#endif
 
    if (size > GETVAR_BUF_SIZE)
       free(p);
 
    if (result != RFR_SUCCESS)
       return resultError("VarList", "getVariableW", result);
```

### Comparing `mhi-psout-1.0.1/README.md` & `mhi-psout-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mhi-psout-1.0.1/Release/CurveFile.dll` & `mhi-psout-1.0.2/Release/CurveFile.dll`

 * *Files 1% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018001066c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Jul  5 20:48:35 2022
+Time/Date		Thu Jun 15 20:16:18 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	16
 SizeOfCode		0000000000010a00
 SizeOfInitializedData	0000000000006e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001066c
@@ -3287,15 +3287,15 @@
 	reloc   20 offset  3a8 [173a8] DIR64
 	reloc   21 offset  3d0 [173d0] DIR64
 
 There is a debug directory in .rdata at 0x180013040
 
 Type                Size     Rva      Offset
   2        CodeView 0000004f 00013c9c 00012a9c
-(format RSDS signature 70ffc712c3c6400aaf3ce336050922db age 1 pdb C:\git-projects\Automation\psout\Release\CurveFile.pdb)
+(format RSDS signature fd5e1fefcfbb40c8a81e08a90ac4fbe0 age 1 pdb C:\git-projects\Automation\psout\Release\CurveFile.pdb)
  12         Feature 00000014 00013cec 00012aec
  13         CoffGrp 00000278 00013d00 00012b00
  14           ILTCG 00000000 00000000 00000000
 
 The .rsrc Resource Directory section:
 000  Type Table: Char: 0, Time: 00000000, Ver: 0/0, Num Names: 0, IDs: 1
 010   Entry: ID: 0x000018, Value: 0x80000018
@@ -25610,44 +25610,52 @@
    180013032:	add    %eax,(%rax)
    180013034:	and    %al,(%rax)
    180013036:	add    %al,(%rax)
    180013038:	add    %al,(%rax)
    18001303a:	add    %al,(%rax)
    18001303c:	add    $0x0,%eax
    180013041:	add    %al,(%rax)
-   180013043:	add    %ah,0x62c4a3(%rbx)
+   180013043:	add    %dl,0x648b71(%rdx)
    180013049:	add    %al,(%rax)
    18001304b:	add    %al,(%rdx)
    18001304d:	add    %al,(%rax)
    18001304f:	add    %cl,0x0(%rdi)
    180013052:	add    %al,(%rax)
    180013054:	pushf
    180013055:	cmp    $0x1,%al
    180013057:	add    %bl,0x1(%rdx,%rbp,1)
    18001305e:	add    %al,(%rax)
-   180013060:	movabs %eax,0xc0000000062c4a3
-   180013069:	add    %al,(%rax)
-   18001306b:	add    %dl,(%rax,%rax,1)
+   180013060:	xchg   %eax,%edx
+   180013061:	jno    0x180012fee
+   180013063:	add    %al,%fs:(%rax)
+   180013066:	add    %al,(%rax)
+   180013068:	or     $0x0,%al
+   18001306a:	add    %al,(%rax)
+   18001306c:	adc    $0x0,%al
    18001306e:	add    %al,(%rax)
    180013070:	in     (%dx),%al
    180013071:	cmp    $0x1,%al
    180013073:	add    %ch,%ah
    180013075:	sub    (%rcx),%al
    180013077:	add    %al,(%rax)
    180013079:	add    %al,(%rax)
-   18001307b:	add    %ah,0x62c4a3(%rbx)
+   18001307b:	add    %dl,0x648b71(%rdx)
    180013081:	add    %al,(%rax)
    180013083:	add    %cl,0x78000000(%rip)        # 0x1f8013089
    180013089:	add    (%rax),%al
    18001308b:	add    %al,(%rax)
    18001308d:	cmp    $0x2b000001,%eax
    180013092:	add    %eax,(%rax)
    180013094:	add    %al,(%rax)
    180013096:	add    %al,(%rax)
-   180013098:	movabs %eax,0xe0000000062c4a3
+   180013098:	xchg   %eax,%edx
+   180013099:	jno    0x180013026
+   18001309b:	add    %al,%fs:(%rax)
+   18001309e:	add    %al,(%rax)
+   1800130a0:	(bad)
 	...
    1800130b1:	add    %eax,(%rax)
 	...
    180013107:	add    %cl,(%rax)
    180013109:	jo     0x18001310c
    18001310b:	addb   $0x0,(%rcx)
 	...
@@ -26393,24 +26401,28 @@
    180013c89:	cmp    (%rcx),%eax
    180013c8b:	add    %bh,0x3c(%rax)
    180013c8e:	add    %eax,(%rax)
 	...
    180013c9c:	push   %rdx
    180013c9d:	push   %rbx
    180013c9e:	rex.R push %rbx
-   180013ca0:	adc    %bh,%al
-   180013ca2:	push   -0x3a(%rax)
-   180013ca5:	ret
-   180013ca6:	or     -0x51(%rax),%al
-   180013ca9:	cmp    $0xe3,%al
-   180013cab:	ss add $0x1db2209,%eax
-   180013cb1:	add    %al,(%rax)
-   180013cb3:	add    %al,0x3a(%rbx)
-   180013cb6:	pop    %rsp
-   180013cb7:	imul   $0x656a6f72,0x70(%ebp,%ebp,1),%esi
+   180013ca0:	out    %eax,(%dx)
+   180013ca1:	(bad)
+   180013ca2:	pop    %rsi
+   180013ca3:	std
+   180013ca4:	mov    $0xa840c8cf,%ebx
+   180013ca9:	(bad)
+   180013caa:	or     %ch,-0x1f043bf6(%rcx)
+   180013cb0:	add    %eax,(%rax)
+   180013cb2:	add    %al,(%rax)
+   180013cb4:	cmp    0x69(%r15,%r12,2),%bl
+   180013cb9:	je     0x180013ce8
+   180013cbb:	jo     0x180013d2f
+   180013cbd:	outsl  %ds:(%rsi),(%dx)
+   180013cbe:	push   $0x65
    180013cc0:	movsxd 0x5c(%rbx,%rsi,2),%esi
    180013cc4:	rex.B jne 0x180013d3b
    180013cc7:	outsl  %ds:(%rsi),(%dx)
    180013cc8:	insl   (%dx),%es:(%rdi)
    180013cc9:	(bad)
    180013cca:	je     0x180013d35
    180013ccc:	outsl  %ds:(%rsi),(%dx)
```

### Comparing `mhi-psout-1.0.1/Release/CurveFile.lib` & `mhi-psout-1.0.2/Release/CurveFile.lib`

 * *Files identical despite different names*

### Comparing `mhi-psout-1.0.1/setup.cfg` & `mhi-psout-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `mhi-psout-1.0.1/setup.py` & `mhi-psout-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import codecs, re, site, sys, shutil, os
-import distutils.sysconfig
 from setuptools import setup, Extension
 
 def get_version(version_file):
     with codecs.open(version_file, 'r') as fp:
         contents = fp.read()
     match = re.search(r"^__version__ = '([^']+)'", contents, re.M)
     if match:
```

### Comparing `mhi-psout-1.0.1/src/mhi/psout/CurveFile.dll` & `mhi-psout-1.0.2/src/mhi/psout/CurveFile.dll`

 * *Files 1% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018001066c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Jul  5 20:48:35 2022
+Time/Date		Thu Jun 15 20:16:18 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	16
 SizeOfCode		0000000000010a00
 SizeOfInitializedData	0000000000006e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001066c
@@ -3287,15 +3287,15 @@
 	reloc   20 offset  3a8 [173a8] DIR64
 	reloc   21 offset  3d0 [173d0] DIR64
 
 There is a debug directory in .rdata at 0x180013040
 
 Type                Size     Rva      Offset
   2        CodeView 0000004f 00013c9c 00012a9c
-(format RSDS signature 70ffc712c3c6400aaf3ce336050922db age 1 pdb C:\git-projects\Automation\psout\Release\CurveFile.pdb)
+(format RSDS signature fd5e1fefcfbb40c8a81e08a90ac4fbe0 age 1 pdb C:\git-projects\Automation\psout\Release\CurveFile.pdb)
  12         Feature 00000014 00013cec 00012aec
  13         CoffGrp 00000278 00013d00 00012b00
  14           ILTCG 00000000 00000000 00000000
 
 The .rsrc Resource Directory section:
 000  Type Table: Char: 0, Time: 00000000, Ver: 0/0, Num Names: 0, IDs: 1
 010   Entry: ID: 0x000018, Value: 0x80000018
@@ -25610,44 +25610,52 @@
    180013032:	add    %eax,(%rax)
    180013034:	and    %al,(%rax)
    180013036:	add    %al,(%rax)
    180013038:	add    %al,(%rax)
    18001303a:	add    %al,(%rax)
    18001303c:	add    $0x0,%eax
    180013041:	add    %al,(%rax)
-   180013043:	add    %ah,0x62c4a3(%rbx)
+   180013043:	add    %dl,0x648b71(%rdx)
    180013049:	add    %al,(%rax)
    18001304b:	add    %al,(%rdx)
    18001304d:	add    %al,(%rax)
    18001304f:	add    %cl,0x0(%rdi)
    180013052:	add    %al,(%rax)
    180013054:	pushf
    180013055:	cmp    $0x1,%al
    180013057:	add    %bl,0x1(%rdx,%rbp,1)
    18001305e:	add    %al,(%rax)
-   180013060:	movabs %eax,0xc0000000062c4a3
-   180013069:	add    %al,(%rax)
-   18001306b:	add    %dl,(%rax,%rax,1)
+   180013060:	xchg   %eax,%edx
+   180013061:	jno    0x180012fee
+   180013063:	add    %al,%fs:(%rax)
+   180013066:	add    %al,(%rax)
+   180013068:	or     $0x0,%al
+   18001306a:	add    %al,(%rax)
+   18001306c:	adc    $0x0,%al
    18001306e:	add    %al,(%rax)
    180013070:	in     (%dx),%al
    180013071:	cmp    $0x1,%al
    180013073:	add    %ch,%ah
    180013075:	sub    (%rcx),%al
    180013077:	add    %al,(%rax)
    180013079:	add    %al,(%rax)
-   18001307b:	add    %ah,0x62c4a3(%rbx)
+   18001307b:	add    %dl,0x648b71(%rdx)
    180013081:	add    %al,(%rax)
    180013083:	add    %cl,0x78000000(%rip)        # 0x1f8013089
    180013089:	add    (%rax),%al
    18001308b:	add    %al,(%rax)
    18001308d:	cmp    $0x2b000001,%eax
    180013092:	add    %eax,(%rax)
    180013094:	add    %al,(%rax)
    180013096:	add    %al,(%rax)
-   180013098:	movabs %eax,0xe0000000062c4a3
+   180013098:	xchg   %eax,%edx
+   180013099:	jno    0x180013026
+   18001309b:	add    %al,%fs:(%rax)
+   18001309e:	add    %al,(%rax)
+   1800130a0:	(bad)
 	...
    1800130b1:	add    %eax,(%rax)
 	...
    180013107:	add    %cl,(%rax)
    180013109:	jo     0x18001310c
    18001310b:	addb   $0x0,(%rcx)
 	...
@@ -26393,24 +26401,28 @@
    180013c89:	cmp    (%rcx),%eax
    180013c8b:	add    %bh,0x3c(%rax)
    180013c8e:	add    %eax,(%rax)
 	...
    180013c9c:	push   %rdx
    180013c9d:	push   %rbx
    180013c9e:	rex.R push %rbx
-   180013ca0:	adc    %bh,%al
-   180013ca2:	push   -0x3a(%rax)
-   180013ca5:	ret
-   180013ca6:	or     -0x51(%rax),%al
-   180013ca9:	cmp    $0xe3,%al
-   180013cab:	ss add $0x1db2209,%eax
-   180013cb1:	add    %al,(%rax)
-   180013cb3:	add    %al,0x3a(%rbx)
-   180013cb6:	pop    %rsp
-   180013cb7:	imul   $0x656a6f72,0x70(%ebp,%ebp,1),%esi
+   180013ca0:	out    %eax,(%dx)
+   180013ca1:	(bad)
+   180013ca2:	pop    %rsi
+   180013ca3:	std
+   180013ca4:	mov    $0xa840c8cf,%ebx
+   180013ca9:	(bad)
+   180013caa:	or     %ch,-0x1f043bf6(%rcx)
+   180013cb0:	add    %eax,(%rax)
+   180013cb2:	add    %al,(%rax)
+   180013cb4:	cmp    0x69(%r15,%r12,2),%bl
+   180013cb9:	je     0x180013ce8
+   180013cbb:	jo     0x180013d2f
+   180013cbd:	outsl  %ds:(%rsi),(%dx)
+   180013cbe:	push   $0x65
    180013cc0:	movsxd 0x5c(%rbx,%rsi,2),%esi
    180013cc4:	rex.B jne 0x180013d3b
    180013cc7:	outsl  %ds:(%rsi),(%dx)
    180013cc8:	insl   (%dx),%es:(%rdi)
    180013cc9:	(bad)
    180013cca:	je     0x180013d35
    180013ccc:	outsl  %ds:(%rsi),(%dx)
```

### Comparing `mhi-psout-1.0.1/src/mhi/psout/__init__.py` & `mhi-psout-1.0.2/src/mhi/psout/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
 try:
     import mhi.psout._psout as _psout
 except ModuleNotFoundError:
     import _psout # For debug builds only
 
 __all__ = ['File', 'Call', 'Trace', 'Run']
-__version__ = '1.0.1'
-__version_hex__ = 0x01_00_01_f0
+__version__ = '1.0.2'
+__version_hex__ = 0x01_00_02_f0
 
 
 #==============================================================================
 # Variable List as a Dictionary
 #------------------------------------------------------------------------------
 
 class VarListMixin:
```

### Comparing `mhi-psout-1.0.1/src/mhi_psout.egg-info/PKG-INFO` & `mhi-psout-1.0.2/src/mhi_psout.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mhi-psout
-Version: 1.0.1
+Version: 1.0.2
 Summary: Manitoba Hydro International: PSOUT File Reader
 Home-page: https://www.pscad.com/webhelp-v5-al/index.html
 Author: Manitoba Hydro International Ltd.
 Author-email: pscad@mhi.ca
 License: BSD-3-Clause-Clear
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

