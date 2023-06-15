# Comparing `tmp/deeplearningoptimized-1.1.0.tar.gz` & `tmp/deeplearningoptimized-1.1.1.tar.gz`

## Comparing `deeplearningoptimized-1.1.0.tar` & `deeplearningoptimized-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.0/src/Pipfile
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.0/src/Pipfile.lock
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.0/src/DeepLearningOptimized/Data_DL.py
--rw-r--r--   0        0        0    18577 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.0/src/DeepLearningOptimized/Model_DL.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.0/src/DeepLearningOptimized/__init__.py
--rw-r--r--   0        0        0   255251 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.0/src/DeepLearningOptimized/deepC.dll
--rw-r--r--   0        0        0    17888 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.0/src/DeepLearningOptimized/deepC.so
--rw-r--r--   0        0        0   380928 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.0/src/DeepLearningOptimized/deepCUDA.dll
--rw-r--r--   0        0        0    18080 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.0/src/DeepLearningOptimized/interface.c
--rw-r--r--   0        0        0    18925 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.0/src/DeepLearningOptimized/interface.cu
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.0/src/DeepLearningOptimized/interface.cuh
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.0/src/DeepLearningOptimized/interface.h
--rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.0/LICENSE.lic
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.0/README.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.1/src/Pipfile
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.1/src/Pipfile.lock
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.1/src/DeepLearningOptimized/Data_DL.py
+-rw-r--r--   0        0        0    18575 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.1/src/DeepLearningOptimized/Model_DL.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.1/src/DeepLearningOptimized/__init__.py
+-rw-r--r--   0        0        0   255251 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.1/src/DeepLearningOptimized/deepC.dll
+-rw-r--r--   0        0        0    17888 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.1/src/DeepLearningOptimized/deepC.so
+-rw-r--r--   0        0        0   380928 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.1/src/DeepLearningOptimized/deepCUDA.dll
+-rw-r--r--   0        0        0    18080 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.1/src/DeepLearningOptimized/interface.c
+-rw-r--r--   0        0        0    18925 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.1/src/DeepLearningOptimized/interface.cu
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.1/src/DeepLearningOptimized/interface.cuh
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.1/src/DeepLearningOptimized/interface.h
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.1/LICENSE.lic
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.1/README.md
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 deeplearningoptimized-1.1.1/PKG-INFO
```

### Comparing `deeplearningoptimized-1.1.0/src/Pipfile.lock` & `deeplearningoptimized-1.1.1/src/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.0/src/DeepLearningOptimized/Data_DL.py` & `deeplearningoptimized-1.1.1/src/DeepLearningOptimized/Data_DL.py`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.0/src/DeepLearningOptimized/Model_DL.py` & `deeplearningoptimized-1.1.1/src/DeepLearningOptimized/Model_DL.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,30 +273,30 @@
                     self.learning_rate -= Decimal(1)/Decimal(2)**(i+1)
                 else:
                     self.learning_rate += Decimal(1)/Decimal(2)**(i+1)
 
                 self.c_learning_rate = c_double(self.learning_rate)
 
                 backup_weights_values = self.weights_values.copy()
-                clib.train(temp_c_min_diff, self.c_learning_rate, temp_c_cycles, self._c_ignore_minimum, Data_train.c_batch_count, Data_train.c_stream, Data_train.c_shift_count, Data_train.c_line_count, Data_train.c_input_values, Data_train.c_target_values, Data_validate.c_stream, Data_validate.c_shift_count, Data_validate.c_line_count, Data_validate.c_input_values, Data_validate.c_target_values, self.c_activation_values, self.c_hidden_sizes_values, self.c_layer_count, self.c_bias_count, self.c_hidden_count, self.c_weight_count, self.c_weights_values)
+                clib.train(temp_c_min_diff, self.c_learning_rate, temp_c_cycles, self.c_ignore_minimum, Data_train.c_batch_count, Data_train.c_stream, Data_train.c_shift_count, Data_train.c_line_count, Data_train.c_input_values, Data_train.c_target_values, Data_validate.c_stream, Data_validate.c_shift_count, Data_validate.c_line_count, Data_validate.c_input_values, Data_validate.c_target_values, self.c_activation_values, self.c_hidden_sizes_values, self.c_layer_count, self.c_bias_count, self.c_hidden_count, self.c_weight_count, self.c_weights_values)
                 self.weights_values = [Decimal(value) for value in self.c_weights_values]
 
                 if "nan" in [str(value).lower() for value in self.weights_values] or self.weights_values == backup_weights_values:
                     fault = True
                 else:
                     fault = False
 
                 self.weights_values = backup_weights_values.copy()
                 weights_values_seq = c_type*len(self.weights_values)
                 self.c_weights_values = weights_values_seq(*self.weights_values)
             
             self.learning_rate *= Decimal("0." + 16*"9")
             self.c_learning_rate = c_double(self.learning_rate)
             
-        clib.train(self.c_min_diff, self.c_learning_rate, self.c_cycles, self._c_ignore_minimum, Data_train.c_batch_count, Data_train.c_stream, Data_train.c_shift_count, Data_train.c_line_count, Data_train.c_input_values, Data_train.c_target_values, Data_validate.c_stream, Data_validate.c_shift_count, Data_validate.c_line_count, Data_validate.c_input_values, Data_validate.c_target_values, self.c_activation_values, self.c_hidden_sizes_values, self.c_layer_count, self.c_bias_count, self.c_hidden_count, self.c_weight_count, self.c_weights_values)
+        clib.train(self.c_min_diff, self.c_learning_rate, self.c_cycles, self.c_ignore_minimum, Data_train.c_batch_count, Data_train.c_stream, Data_train.c_shift_count, Data_train.c_line_count, Data_train.c_input_values, Data_train.c_target_values, Data_validate.c_stream, Data_validate.c_shift_count, Data_validate.c_line_count, Data_validate.c_input_values, Data_validate.c_target_values, self.c_activation_values, self.c_hidden_sizes_values, self.c_layer_count, self.c_bias_count, self.c_hidden_count, self.c_weight_count, self.c_weights_values)
         self.weights_values = [Decimal(value) for value in self.c_weights_values]
 
         if self.normaliser_depth > 0:
             self.test(Data_validate, test_mode=False)
 
             self.NData_train.load(self.output_values, Data_validate.target_values, 0, Data_validate.output_count)
             self.NData_train.prepare(self.output_count, self.output_count, False)
```

### Comparing `deeplearningoptimized-1.1.0/src/DeepLearningOptimized/deepC.dll` & `deeplearningoptimized-1.1.1/src/DeepLearningOptimized/deepC.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -5,15 +5,15 @@
 
 Characteristics 0x2026
 	executable
 	line numbers stripped
 	large address aware
 	DLL
 
-Time/Date		Thu Jun 15 18:34:50 2023
+Time/Date		Thu Jun 15 18:37:10 2023
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
-CheckSum		0004e141
+CheckSum		0004e259
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
-Time/Date stamp 		648b59ca
+Time/Date stamp 		648b5a56
 Major/Minor 			0/0
 Name 				000000000001014a deepC.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		0000001d
 	[Name Pointer/Ordinal] Table	0000001d
 Table Addresses
@@ -20025,16 +20025,17 @@
 	...
 
 Disassembly of section .edata:
 
 000000035c020000 <.edata>:
    35c020000:	add    %al,(%rax)
    35c020002:	add    %al,(%rax)
-   35c020004:	lret   $0x8b59
-   35c020007:	add    %al,%fs:(%rax)
+   35c020004:	push   %rsi
+   35c020005:	pop    %rdx
+   35c020006:	mov    0x0(%rax,%rax,1),%esp
    35c02000a:	add    %al,(%rax)
    35c02000c:	rex.WX add %rax,(%rcx)
    35c02000f:	add    %al,(%rcx)
    35c020011:	add    %al,(%rax)
    35c020013:	add    %bl,0x1d000000(%rip)        # 379020019 <.debug_rnglists+0x1cfcca99>
    35c020019:	add    %al,(%rax)
    35c02001b:	add    %ch,(%rax)
```

### Comparing `deeplearningoptimized-1.1.0/src/DeepLearningOptimized/deepC.so` & `deeplearningoptimized-1.1.1/src/DeepLearningOptimized/deepC.so`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.0/src/DeepLearningOptimized/deepCUDA.dll` & `deeplearningoptimized-1.1.1/src/DeepLearningOptimized/deepCUDA.dll`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.0/src/DeepLearningOptimized/interface.c` & `deeplearningoptimized-1.1.1/src/DeepLearningOptimized/interface.c`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.0/src/DeepLearningOptimized/interface.cu` & `deeplearningoptimized-1.1.1/src/DeepLearningOptimized/interface.cu`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.0/src/DeepLearningOptimized/interface.cuh` & `deeplearningoptimized-1.1.1/src/DeepLearningOptimized/interface.cuh`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.0/src/DeepLearningOptimized/interface.h` & `deeplearningoptimized-1.1.1/src/DeepLearningOptimized/interface.h`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.0/LICENSE.lic` & `deeplearningoptimized-1.1.1/LICENSE.lic`

 * *Files identical despite different names*

### Comparing `deeplearningoptimized-1.1.0/pyproject.toml` & `deeplearningoptimized-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "DeepLearningOptimized"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Liam Roan Watson", email="lrwatson@uwaterloo.ca" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

