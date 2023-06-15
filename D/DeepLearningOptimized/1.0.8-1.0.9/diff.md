# Comparing `tmp/deeplearningoptimized-1.0.8.tar.gz` & `tmp/deeplearningoptimized-1.0.9.tar.gz`

## Comparing `deeplearningoptimized-1.0.8.tar` & `deeplearningoptimized-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.8/src/Pipfile
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.8/src/Pipfile.lock
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.8/src/DeepLearningOptimized/Data_DL.py
--rw-r--r--   0        0        0    18455 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.8/src/DeepLearningOptimized/Model_DL.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.8/src/DeepLearningOptimized/__init__.py
--rw-r--r--   0        0        0   255251 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.8/src/DeepLearningOptimized/deepC.dll
--rw-r--r--   0        0        0    17888 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.8/src/DeepLearningOptimized/deepC.so
--rw-r--r--   0        0        0   380928 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.8/src/DeepLearningOptimized/deepCUDA.dll
--rw-r--r--   0        0        0    18033 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.8/src/DeepLearningOptimized/interface.c
--rw-r--r--   0        0        0    18925 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.8/src/DeepLearningOptimized/interface.cu
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.8/src/DeepLearningOptimized/interface.cuh
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.8/src/DeepLearningOptimized/interface.h
--rw-r--r--   0        0        0    14431 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.8/src/DeepLearningOptimized/interface.o
--rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.8/LICENSE.lic
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.8/README.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.9/src/Pipfile
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.9/src/Pipfile.lock
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.9/src/DeepLearningOptimized/Data_DL.py
+-rw-r--r--   0        0        0    18455 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.9/src/DeepLearningOptimized/Model_DL.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.9/src/DeepLearningOptimized/__init__.py
+-rw-r--r--   0        0        0   255251 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.9/src/DeepLearningOptimized/deepC.dll
+-rw-r--r--   0        0        0    17888 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.9/src/DeepLearningOptimized/deepC.so
+-rw-r--r--   0        0        0   380928 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.9/src/DeepLearningOptimized/deepCUDA.dll
+-rw-r--r--   0        0        0    18034 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.9/src/DeepLearningOptimized/interface.c
+-rw-r--r--   0        0        0    18925 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.9/src/DeepLearningOptimized/interface.cu
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.9/src/DeepLearningOptimized/interface.cuh
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.9/src/DeepLearningOptimized/interface.h
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.9/LICENSE.lic
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.9/README.md
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 deeplearningoptimized-1.0.9/PKG-INFO
```

### Comparing `deeplearningoptimized-1.0.8/src/Pipfile.lock` & `deeplearningoptimized-1.0.9/src/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.0.8/src/DeepLearningOptimized/Data_DL.py` & `deeplearningoptimized-1.0.9/src/DeepLearningOptimized/Data_DL.py`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.0.8/src/DeepLearningOptimized/Model_DL.py` & `deeplearningoptimized-1.0.9/src/DeepLearningOptimized/Model_DL.py`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.0.8/src/DeepLearningOptimized/deepC.dll` & `deeplearningoptimized-1.0.9/src/DeepLearningOptimized/deepC.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -5,15 +5,15 @@
 
 Characteristics 0x2026
 	executable
 	line numbers stripped
 	large address aware
 	DLL
 
-Time/Date		Thu Jun 15 18:16:10 2023
+Time/Date		Thu Jun 15 18:23:26 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	38
 SizeOfCode		0000000000009a00
 SizeOfInitializedData	000000000000c800
 SizeOfUninitializedData	0000000000000c00
 AddressOfEntryPoint	0000000000001320
@@ -26,15 +26,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		00044000
 SizeOfHeaders		00000600
-CheckSum		00042ed5
+CheckSum		00044e65
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000200000
 SizeOfStackCommit	0000000000001000
@@ -115,15 +115,15 @@
  00011028	00000000 00000000 00000000 00000000 00000000
 
 There is an export table in .edata at 0x35c020000
 
 The Export Tables (interpreted .edata section contents)
 
 Export Flags 			0
-Time/Date stamp 		648b556a
+Time/Date stamp 		648b571e
 Major/Minor 			0/0
 Name 				000000000001014a deepC.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		0000001d
 	[Name Pointer/Ordinal] Table	0000001d
 Table Addresses
@@ -4541,16 +4541,16 @@
    35c012817:	movsd  %xmm0,0xf8(%rbp)
    35c01281f:	movsd  0xc7f9(%rip),%xmm0        # 35c01f020 <zero>
    35c012827:	movsd  %xmm0,0xf0(%rbp)
    35c01282f:	movsd  0xc7e9(%rip),%xmm0        # 35c01f020 <zero>
    35c012837:	movsd  %xmm0,0xe8(%rbp)
    35c01283f:	movsd  0xc7d9(%rip),%xmm0        # 35c01f020 <zero>
    35c012847:	movsd  %xmm0,0xe0(%rbp)
-   35c01284f:	movl   $0xa,0x4c(%rbp)
-   35c012856:	movl   $0x2,0x48(%rbp)
+   35c01284f:	movl   $0x32,0x4c(%rbp)
+   35c012856:	movl   $0x1e,0x48(%rbp)
    35c01285d:	mov    0x87ad(%rip),%eax        # 35c01b010 <size_of_double>
    35c012863:	imul   0x4c(%rbp),%eax
    35c012867:	cltq
    35c012869:	mov    %rax,%rcx
    35c01286c:	call   35c01a770 <malloc>
    35c012871:	mov    %rax,0x40(%rbp)
    35c012875:	mov    0x8795(%rip),%eax        # 35c01b010 <size_of_double>
@@ -19926,15 +19926,16 @@
 	...
 
 Disassembly of section .edata:
 
 000000035c020000 <.edata>:
    35c020000:	add    %al,(%rax)
    35c020002:	add    %al,(%rax)
-   35c020004:	push   $0x55
+   35c020004:	(bad)
+   35c020005:	push   %rdi
    35c020006:	mov    0x0(%rax,%rax,1),%esp
    35c02000a:	add    %al,(%rax)
    35c02000c:	rex.WX add %rax,(%rcx)
    35c02000f:	add    %al,(%rcx)
    35c020011:	add    %al,(%rax)
    35c020013:	add    %bl,0x1d000000(%rip)        # 379020019 <.debug_rnglists+0x1cfcca99>
    35c020019:	add    %al,(%rax)
```

### Comparing `deeplearningoptimized-1.0.8/src/DeepLearningOptimized/deepC.so` & `deeplearningoptimized-1.0.9/src/DeepLearningOptimized/deepC.so`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.0.8/src/DeepLearningOptimized/deepCUDA.dll` & `deeplearningoptimized-1.0.9/src/DeepLearningOptimized/deepCUDA.dll`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.0.8/src/DeepLearningOptimized/interface.c` & `deeplearningoptimized-1.0.9/src/DeepLearningOptimized/interface.c`

 * *Files 0% similar despite different names*

```diff
@@ -311,16 +311,16 @@
   double change_coefficient, cycles_remaining_current;
   
   double cycles_remaining_sum1 = zero;
   double cycles_remaining_average1 = zero;
   double cycles_remaining_sum2 = zero;
   double cycles_remaining_average2 = zero;
 
-  int average_size1 = 10;
-  int average_size2 = 2;
+  int average_size1 = 50;
+  int average_size2 = 30;
 
   double* prev_cycles_remaining1 = (double*) malloc(average_size1 * size_of_double);
   double* prev_cycles_remaining2 = (double*) malloc(average_size2 * size_of_double);
 
   int minimum_reached = zero;
 
   int cycle = zero;
```

### Comparing `deeplearningoptimized-1.0.8/src/DeepLearningOptimized/interface.cu` & `deeplearningoptimized-1.0.9/src/DeepLearningOptimized/interface.cu`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.0.8/src/DeepLearningOptimized/interface.cuh` & `deeplearningoptimized-1.0.9/src/DeepLearningOptimized/interface.cuh`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.0.8/src/DeepLearningOptimized/interface.h` & `deeplearningoptimized-1.0.9/src/DeepLearningOptimized/interface.h`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.0.8/LICENSE.lic` & `deeplearningoptimized-1.0.9/LICENSE.lic`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.0.8/pyproject.toml` & `deeplearningoptimized-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "DeepLearningOptimized"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Liam Roan Watson", email="lrwatson@uwaterloo.ca" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

