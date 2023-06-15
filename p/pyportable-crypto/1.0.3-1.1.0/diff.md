# Comparing `tmp/pyportable-crypto-1.0.3.tar.gz` & `tmp/pyportable_crypto-1.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyportable-crypto-1.0.3.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

## Comparing `pyportable-crypto-1.0.3.tar` & `pyportable_crypto/cipher_gen/site-packages.zip`

 * *Files 26% similar despite different names*

### file list

```diff
@@ -1,18 +1,475 @@
--rw-r--r--   0        0        0     1064 2022-08-01 02:26:30.329172 pyportable-crypto-1.0.3/LICENSE
--rw-r--r--   0        0        0      539 2022-09-13 10:38:01.287332 pyportable-crypto-1.0.3/pyportable_crypto/__init__.py
--rw-r--r--   0        0        0     1192 2022-09-13 10:38:01.278521 pyportable-crypto-1.0.3/pyportable_crypto/__main__.py
--rw-r--r--   0        0        0    54567 2022-08-01 02:26:30.332305 pyportable-crypto-1.0.3/pyportable_crypto/_pyaes_snippet.py
--rw-r--r--   0        0        0       54 2022-08-01 02:26:30.332452 pyportable-crypto-1.0.3/pyportable_crypto/cipher_gen/__init__.py
--rw-r--r--   0        0        0        0 2022-08-01 02:26:30.332656 pyportable-crypto-1.0.3/pyportable_crypto/cipher_gen/cache/.gitkeep
--rw-r--r--   0        0        0    64397 2022-08-01 02:26:30.333114 pyportable-crypto-1.0.3/pyportable_crypto/cipher_gen/cipher_standalone.py
--rw-r--r--   0        0        0      479 2022-08-01 02:26:30.333232 pyportable-crypto-1.0.3/pyportable_crypto/cipher_gen/cythonize.py
--rw-r--r--   0        0        0     4960 2022-08-01 02:26:30.333370 pyportable-crypto-1.0.3/pyportable_crypto/cipher_gen/generator.py
--rw-r--r--   0        0        0  1867638 2022-08-01 02:26:30.340567 pyportable-crypto-1.0.3/pyportable_crypto/cipher_gen/site-packages.zip
--rw-r--r--   0        0        0     2648 2022-09-13 10:38:51.985135 pyportable-crypto-1.0.3/pyportable_crypto/compiler.py
--rw-r--r--   0        0        0     1034 2022-08-01 02:26:30.341214 pyportable-crypto-1.0.3/pyportable_crypto/decrypt.py
--rw-r--r--   0        0        0     1061 2022-08-01 02:26:30.341359 pyportable-crypto-1.0.3/pyportable_crypto/encrypt.py
--rw-r--r--   0        0        0      344 2022-08-01 02:26:30.341494 pyportable-crypto-1.0.3/pyportable_crypto/formatter.py
--rw-r--r--   0        0        0      227 2022-08-01 02:26:30.341633 pyportable-crypto-1.0.3/pyportable_crypto/keygen.py
--rw-r--r--   0        0        0      606 2022-09-14 06:49:34.806505 pyportable-crypto-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      796 2022-09-14 06:49:47.836205 pyportable-crypto-1.0.3/setup.py
--rw-r--r--   0        0        0      642 2022-09-14 06:49:47.836524 pyportable-crypto-1.0.3/PKG-INFO
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:10.000000 _distutils_hack/
+-rw-rw-r--   0        0        0     3688 2021-09-09 02:02:40.000000 _distutils_hack/__init__.py
+-rw-rw-r--   0        0        0       44 2021-09-09 02:02:40.000000 _distutils_hack/override.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:06.000000 Cython-3.0a7.dist-info/
+-rw-rw-r--   0        0        0     1167 2021-05-24 16:39:12.000000 Cython-3.0a7.dist-info/DESCRIPTION.rst
+-rw-rw-r--   0        0        0      140 2021-05-24 16:39:10.000000 Cython-3.0a7.dist-info/entry_points.txt
+-rw-rw-r--   0        0        0     2631 2021-05-24 16:39:12.000000 Cython-3.0a7.dist-info/METADATA
+-rw-rw-r--   0        0        0     1829 2021-05-24 16:39:12.000000 Cython-3.0a7.dist-info/metadata.json
+-rw-rw-r--   0        0        0    24925 2021-05-24 16:39:12.000000 Cython-3.0a7.dist-info/RECORD
+-rw-rw-r--   0        0        0       24 2021-05-24 16:39:10.000000 Cython-3.0a7.dist-info/top_level.txt
+-rw-rw-r--   0        0        0      110 2021-05-24 16:39:12.000000 Cython-3.0a7.dist-info/WHEEL
+-rw-rw-r--   0        0        0      520 2015-06-22 12:53:10.000000 cython.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:06.000000 Cython/
+-rw-rw-r--   0        0        0      358 2016-12-10 15:41:14.000000 Cython/__init__.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:06.000000 Cython/Build/
+-rw-rw-r--   0        0        0       69 2016-12-10 15:41:14.000000 Cython/Build/__init__.py
+-rw-rw-r--   0        0        0     4219 2021-05-24 14:21:44.000000 Cython/Build/BuildExecutable.py
+-rw-rw-r--   0        0        0     8348 2021-05-24 14:21:44.000000 Cython/Build/Cythonize.py
+-rw-rw-r--   0        0        0    51410 2021-05-24 14:21:54.000000 Cython/Build/Dependencies.py
+-rw-rw-r--   0        0        0       49 2016-12-10 15:41:14.000000 Cython/Build/Distutils.py
+-rw-rw-r--   0        0        0    12561 2021-05-24 14:21:44.000000 Cython/Build/Inline.py
+-rw-rw-r--   0        0        0    23063 2021-05-24 14:21:54.000000 Cython/Build/IpythonMagic.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:06.000000 Cython/Build/Tests/
+-rw-rw-r--   0        0        0       13 2015-06-22 12:53:10.000000 Cython/Build/Tests/__init__.py
+-rw-rw-r--   0        0        0     4401 2021-05-24 14:21:44.000000 Cython/Build/Tests/TestCyCache.py
+-rw-rw-r--   0        0        0    20346 2021-05-24 14:21:44.000000 Cython/Build/Tests/TestCythonizeArgsParser.py
+-rw-rw-r--   0        0        0     3477 2021-05-24 14:21:44.000000 Cython/Build/Tests/TestInline.py
+-rw-rw-r--   0        0        0     9687 2021-05-24 14:21:54.000000 Cython/Build/Tests/TestIpythonMagic.py
+-rw-rw-r--   0        0        0     1549 2021-05-24 14:21:44.000000 Cython/Build/Tests/TestStripLiterals.py
+-rw-rw-r--   0        0        0    24470 2021-05-24 14:21:54.000000 Cython/CodeWriter.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:06.000000 Cython/Compiler/
+-rw-rw-r--   0        0        0       13 2015-06-22 12:53:10.000000 Cython/Compiler/__init__.py
+-rw-rw-r--   0        0        0     3834 2021-05-24 14:21:54.000000 Cython/Compiler/AnalysedTreeTransforms.py
+-rw-rw-r--   0        0        0    14139 2021-05-24 14:21:54.000000 Cython/Compiler/Annotate.py
+-rw-rw-r--   0        0        0     9144 2021-05-24 14:21:54.000000 Cython/Compiler/AutoDocTransforms.py
+-rw-rw-r--   0        0        0    29045 2021-05-24 14:21:54.000000 Cython/Compiler/Buffer.py
+-rw-rw-r--   0        0        0    23240 2021-05-24 14:21:54.000000 Cython/Compiler/Builtin.py
+-rw-rw-r--   0        0        0    11353 2021-05-24 14:21:44.000000 Cython/Compiler/CmdLine.py
+-rw-rw-r--   0        0        0     3308 2021-05-24 14:21:54.000000 Cython/Compiler/Code.pxd
+-rw-rw-r--   0        0        0    99154 2021-05-24 14:21:54.000000 Cython/Compiler/Code.py
+-rw-rw-r--   0        0        0     1108 2018-09-22 14:18:56.000000 Cython/Compiler/CodeGeneration.py
+-rw-rw-r--   0        0        0     6425 2021-05-24 14:21:54.000000 Cython/Compiler/CythonScope.py
+-rw-rw-r--   0        0        0      623 2015-06-22 12:53:10.000000 Cython/Compiler/DebugFlags.py
+-rw-rw-r--   0        0        0     7703 2021-05-24 14:21:54.000000 Cython/Compiler/Errors.py
+-rw-rw-r--   0        0        0   563327 2021-05-24 14:21:54.000000 Cython/Compiler/ExprNodes.py
+-rw-rw-r--   0        0        0     2934 2021-05-24 14:21:54.000000 Cython/Compiler/FlowControl.pxd
+-rw-rw-r--   0        0        0    46938 2021-05-24 14:21:54.000000 Cython/Compiler/FlowControl.py
+-rw-rw-r--   0        0        0    40425 2021-05-24 14:21:54.000000 Cython/Compiler/FusedNode.py
+-rw-rw-r--   0        0        0      629 2021-05-24 14:21:44.000000 Cython/Compiler/Future.py
+-rw-rw-r--   0        0        0     2114 2021-05-24 14:21:44.000000 Cython/Compiler/Interpreter.py
+-rw-rw-r--   0        0        0    12144 2021-05-24 14:21:54.000000 Cython/Compiler/Lexicon.py
+-rw-rw-r--   0        0        0    29304 2021-05-24 14:21:54.000000 Cython/Compiler/Main.py
+-rw-rw-r--   0        0        0    30401 2021-05-24 14:21:54.000000 Cython/Compiler/MemoryView.py
+-rw-rw-r--   0        0        0   169572 2021-05-24 14:21:54.000000 Cython/Compiler/ModuleNode.py
+-rw-rw-r--   0        0        0     7143 2021-05-24 14:21:44.000000 Cython/Compiler/Naming.py
+-rw-rw-r--   0        0        0   414789 2021-05-24 14:21:54.000000 Cython/Compiler/Nodes.py
+-rw-rw-r--   0        0        0   221692 2021-05-24 14:21:54.000000 Cython/Compiler/Optimize.py
+-rw-rw-r--   0        0        0    28096 2021-05-24 14:21:44.000000 Cython/Compiler/Options.py
+-rw-rw-r--   0        0        0     2455 2021-05-24 14:21:54.000000 Cython/Compiler/ParseTreeTransforms.pxd
+-rw-rw-r--   0        0        0   145348 2021-05-24 14:21:54.000000 Cython/Compiler/ParseTreeTransforms.py
+-rw-rw-r--   0        0        0     9053 2021-05-24 14:21:54.000000 Cython/Compiler/Parsing.pxd
+-rw-rw-r--   0        0        0   133793 2021-05-24 14:21:54.000000 Cython/Compiler/Parsing.py
+-rw-rw-r--   0        0        0    14869 2021-05-24 14:21:54.000000 Cython/Compiler/Pipeline.py
+-rw-rw-r--   0        0        0   186445 2021-05-24 14:21:54.000000 Cython/Compiler/PyrexTypes.py
+-rw-rw-r--   0        0        0     7267 2020-05-19 07:31:38.000000 Cython/Compiler/Pythran.py
+-rw-rw-r--   0        0        0     2003 2021-05-24 14:21:54.000000 Cython/Compiler/Scanning.pxd
+-rw-rw-r--   0        0        0    18133 2021-05-24 14:21:44.000000 Cython/Compiler/Scanning.py
+-rw-rw-r--   0        0        0    11728 2021-05-24 14:21:44.000000 Cython/Compiler/StringEncoding.py
+-rw-rw-r--   0        0        0   119193 2021-05-24 14:21:54.000000 Cython/Compiler/Symtab.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:06.000000 Cython/Compiler/Tests/
+-rw-rw-r--   0        0        0       13 2015-06-22 12:53:10.000000 Cython/Compiler/Tests/__init__.py
+-rw-rw-r--   0        0        0     4156 2021-05-24 14:21:44.000000 Cython/Compiler/Tests/TestBuffer.py
+-rw-rw-r--   0        0        0    19207 2021-05-24 14:21:44.000000 Cython/Compiler/Tests/TestCmdLine.py
+-rw-rw-r--   0        0        0     1848 2016-12-10 15:41:14.000000 Cython/Compiler/Tests/TestFlowControl.py
+-rw-rw-r--   0        0        0     3977 2021-05-24 14:21:44.000000 Cython/Compiler/Tests/TestGrammar.py
+-rw-rw-r--   0        0        0     2517 2021-05-24 14:21:44.000000 Cython/Compiler/Tests/TestMemView.py
+-rw-rw-r--   0        0        0     8529 2021-05-24 14:21:44.000000 Cython/Compiler/Tests/TestParseTreeTransforms.py
+-rw-rw-r--   0        0        0     3342 2021-05-24 14:21:44.000000 Cython/Compiler/Tests/TestSignatureMatching.py
+-rw-rw-r--   0        0        0     2315 2020-07-31 07:03:12.000000 Cython/Compiler/Tests/TestStringEncoding.py
+-rw-rw-r--   0        0        0     2206 2021-05-24 14:21:44.000000 Cython/Compiler/Tests/TestTreeFragment.py
+-rw-rw-r--   0        0        0     4238 2018-09-22 14:18:56.000000 Cython/Compiler/Tests/TestTreePath.py
+-rw-rw-r--   0        0        0     3295 2021-05-24 14:21:54.000000 Cython/Compiler/Tests/TestTypes.py
+-rw-rw-r--   0        0        0     3119 2021-05-24 14:21:44.000000 Cython/Compiler/Tests/TestUtilityLoad.py
+-rw-rw-r--   0        0        0     2228 2015-06-22 12:53:10.000000 Cython/Compiler/Tests/TestVisitor.py
+-rw-rw-r--   0        0        0     1065 2021-05-24 14:21:44.000000 Cython/Compiler/Tests/Utils.py
+-rw-rw-r--   0        0        0     9334 2021-05-24 14:21:44.000000 Cython/Compiler/TreeFragment.py
+-rw-rw-r--   0        0        0     7641 2021-05-24 14:21:54.000000 Cython/Compiler/TreePath.py
+-rw-rw-r--   0        0        0    22540 2021-05-24 14:21:44.000000 Cython/Compiler/TypeInference.py
+-rw-rw-r--   0        0        0    41634 2021-05-24 14:21:54.000000 Cython/Compiler/TypeSlots.py
+-rw-rw-r--   0        0        0     9392 2021-05-24 14:21:54.000000 Cython/Compiler/UtilityCode.py
+-rw-rw-r--   0        0        0    11817 2021-05-24 14:21:44.000000 Cython/Compiler/UtilNodes.py
+-rw-rw-r--   0        0        0      181 2015-06-22 12:53:10.000000 Cython/Compiler/Version.py
+-rw-rw-r--   0        0        0     1780 2021-05-24 14:21:54.000000 Cython/Compiler/Visitor.pxd
+-rw-rw-r--   0        0        0    30766 2021-05-24 14:21:54.000000 Cython/Compiler/Visitor.py
+-rw-rw-r--   0        0        0    14991 2021-05-24 14:21:54.000000 Cython/Coverage.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:06.000000 Cython/Debugger/
+-rw-rw-r--   0        0        0       13 2015-06-22 12:53:10.000000 Cython/Debugger/__init__.py
+-rw-rw-r--   0        0        0     6150 2021-05-24 14:21:44.000000 Cython/Debugger/Cygdb.py
+-rw-rw-r--   0        0        0     1949 2021-05-24 14:21:44.000000 Cython/Debugger/DebugWriter.py
+-rw-rw-r--   0        0        0    46539 2021-05-24 14:21:54.000000 Cython/Debugger/libcython.py
+-rw-rw-r--   0        0        0    93839 2021-05-24 14:21:54.000000 Cython/Debugger/libpython.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:06.000000 Cython/Debugger/Tests/
+-rw-rw-r--   0        0        0       13 2015-06-22 12:53:10.000000 Cython/Debugger/Tests/__init__.py
+-rw-rw-r--   0        0        0       71 2015-06-22 12:53:10.000000 Cython/Debugger/Tests/cfuncs.c
+-rw-rw-r--   0        0        0      642 2021-05-24 14:21:54.000000 Cython/Debugger/Tests/codefile
+-rw-rw-r--   0        0        0    18048 2021-05-24 14:21:54.000000 Cython/Debugger/Tests/test_libcython_in_gdb.py
+-rw-rw-r--   0        0        0     4079 2018-09-22 14:18:56.000000 Cython/Debugger/Tests/test_libpython_in_gdb.py
+-rw-rw-r--   0        0        0     8327 2021-05-24 14:21:44.000000 Cython/Debugger/Tests/TestLibCython.py
+-rw-rw-r--   0        0        0      552 2015-06-22 12:53:10.000000 Cython/Debugging.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:06.000000 Cython/Distutils/
+-rw-rw-r--   0        0        0       98 2015-06-22 12:53:10.000000 Cython/Distutils/__init__.py
+-rw-rw-r--   0        0        0     1007 2018-09-22 14:18:56.000000 Cython/Distutils/build_ext.py
+-rw-rw-r--   0        0        0     4706 2015-09-10 16:25:36.000000 Cython/Distutils/extension.py
+-rw-rw-r--   0        0        0    13583 2021-05-24 14:21:44.000000 Cython/Distutils/old_build_ext.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:06.000000 Cython/Includes/
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:06.000000 Cython/Includes/cpython/
+-rw-rw-r--   0        0        0     8306 2021-05-24 14:21:54.000000 Cython/Includes/cpython/__init__.pxd
+-rw-rw-r--   0        0        0     6358 2021-05-24 14:21:54.000000 Cython/Includes/cpython/array.pxd
+-rw-rw-r--   0        0        0     1359 2015-06-22 12:53:10.000000 Cython/Includes/cpython/bool.pxd
+-rw-rw-r--   0        0        0     4870 2021-05-24 14:21:54.000000 Cython/Includes/cpython/buffer.pxd
+-rw-rw-r--   0        0        0     1443 2020-04-19 09:26:02.000000 Cython/Includes/cpython/bytearray.pxd
+-rw-rw-r--   0        0        0    10068 2021-05-24 14:21:44.000000 Cython/Includes/cpython/bytes.pxd
+-rw-rw-r--   0        0        0     1390 2021-05-24 14:21:54.000000 Cython/Includes/cpython/cellobject.pxd
+-rw-rw-r--   0        0        0      236 2020-04-19 09:26:02.000000 Cython/Includes/cpython/ceval.pxd
+-rw-rw-r--   0        0        0     1524 2015-06-22 12:53:10.000000 Cython/Includes/cpython/cobject.pxd
+-rw-rw-r--   0        0        0     5084 2021-05-24 14:21:54.000000 Cython/Includes/cpython/codecs.pxd
+-rw-rw-r--   0        0        0     1824 2021-05-24 14:21:44.000000 Cython/Includes/cpython/complex.pxd
+-rw-rw-r--   0        0        0     5637 2021-05-24 14:21:54.000000 Cython/Includes/cpython/contextvars.pxd
+-rw-rw-r--   0        0        0     1696 2021-05-24 14:21:54.000000 Cython/Includes/cpython/conversion.pxd
+-rw-rw-r--   0        0        0    15433 2021-05-24 14:21:54.000000 Cython/Includes/cpython/datetime.pxd
+-rw-rw-r--   0        0        0      728 2021-05-24 14:21:44.000000 Cython/Includes/cpython/descr.pxd
+-rw-rw-r--   0        0        0     7939 2021-05-24 14:21:44.000000 Cython/Includes/cpython/dict.pxd
+-rw-rw-r--   0        0        0    13606 2020-04-19 09:26:02.000000 Cython/Includes/cpython/exc.pxd
+-rw-rw-r--   0        0        0     2889 2021-05-24 14:21:54.000000 Cython/Includes/cpython/fileobject.pxd
+-rw-rw-r--   0        0        0     1424 2015-06-22 12:53:10.000000 Cython/Includes/cpython/float.pxd
+-rw-rw-r--   0        0        0     2671 2015-06-22 12:53:10.000000 Cython/Includes/cpython/function.pxd
+-rw-rw-r--   0        0        0     1052 2020-05-19 07:31:38.000000 Cython/Includes/cpython/genobject.pxd
+-rw-rw-r--   0        0        0      775 2015-06-22 12:53:10.000000 Cython/Includes/cpython/getargs.pxd
+-rw-rw-r--   0        0        0      985 2015-06-22 12:53:10.000000 Cython/Includes/cpython/instance.pxd
+-rw-rw-r--   0        0        0     4131 2015-06-22 12:53:10.000000 Cython/Includes/cpython/int.pxd
+-rw-rw-r--   0        0        0     1319 2015-06-22 12:53:10.000000 Cython/Includes/cpython/iterator.pxd
+-rw-rw-r--   0        0        0     1036 2020-05-19 07:31:38.000000 Cython/Includes/cpython/iterobject.pxd
+-rw-rw-r--   0        0        0     4098 2021-05-24 14:21:44.000000 Cython/Includes/cpython/list.pxd
+-rw-rw-r--   0        0        0     7047 2021-05-24 14:21:54.000000 Cython/Includes/cpython/long.pxd
+-rw-rw-r--   0        0        0      445 2018-11-24 09:20:06.000000 Cython/Includes/cpython/longintrepr.pxd
+-rw-rw-r--   0        0        0     2693 2015-06-22 12:53:10.000000 Cython/Includes/cpython/mapping.pxd
+-rw-rw-r--   0        0        0     2901 2021-05-24 14:21:44.000000 Cython/Includes/cpython/marshal.pxd
+-rw-rw-r--   0        0        0     5386 2020-04-19 09:26:02.000000 Cython/Includes/cpython/mem.pxd
+-rw-rw-r--   0        0        0     2504 2020-05-19 07:31:38.000000 Cython/Includes/cpython/memoryview.pxd
+-rw-rw-r--   0        0        0     2196 2015-06-22 12:53:10.000000 Cython/Includes/cpython/method.pxd
+-rw-rw-r--   0        0        0    10128 2021-05-24 14:21:44.000000 Cython/Includes/cpython/module.pxd
+-rw-rw-r--   0        0        0    11922 2020-05-19 07:31:38.000000 Cython/Includes/cpython/number.pxd
+-rw-rw-r--   0        0        0    19764 2021-05-24 14:21:44.000000 Cython/Includes/cpython/object.pxd
+-rw-rw-r--   0        0        0     2916 2015-06-22 12:53:10.000000 Cython/Includes/cpython/oldbuffer.pxd
+-rw-rw-r--   0        0        0     5692 2021-05-24 14:21:54.000000 Cython/Includes/cpython/pycapsule.pxd
+-rw-rw-r--   0        0        0     2000 2020-05-19 07:31:38.000000 Cython/Includes/cpython/pylifecycle.pxd
+-rw-rw-r--   0        0        0      222 2021-05-24 14:21:44.000000 Cython/Includes/cpython/pyport.pxd
+-rw-rw-r--   0        0        0     3779 2021-05-24 14:21:44.000000 Cython/Includes/cpython/pystate.pxd
+-rw-rw-r--   0        0        0     1946 2018-09-22 14:18:56.000000 Cython/Includes/cpython/pythread.pxd
+-rw-rw-r--   0        0        0     2557 2015-06-22 12:53:10.000000 Cython/Includes/cpython/ref.pxd
+-rw-rw-r--   0        0        0     6008 2015-06-22 12:53:10.000000 Cython/Includes/cpython/sequence.pxd
+-rw-rw-r--   0        0        0     5383 2018-09-22 14:18:56.000000 Cython/Includes/cpython/set.pxd
+-rw-rw-r--   0        0        0     3111 2020-05-19 07:31:38.000000 Cython/Includes/cpython/slice.pxd
+-rw-rw-r--   0        0        0     9944 2015-06-22 12:53:10.000000 Cython/Includes/cpython/string.pxd
+-rw-rw-r--   0        0        0     1356 2021-05-24 14:21:54.000000 Cython/Includes/cpython/time.pxd
+-rw-rw-r--   0        0        0     3220 2021-05-24 14:21:44.000000 Cython/Includes/cpython/tuple.pxd
+-rw-rw-r--   0        0        0     2067 2021-05-24 14:21:44.000000 Cython/Includes/cpython/type.pxd
+-rw-rw-r--   0        0        0    26593 2021-05-24 14:21:44.000000 Cython/Includes/cpython/unicode.pxd
+-rw-rw-r--   0        0        0      847 2015-06-22 12:53:10.000000 Cython/Includes/cpython/version.pxd
+-rw-rw-r--   0        0        0     1984 2018-09-22 14:18:56.000000 Cython/Includes/cpython/weakref.pxd
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:06.000000 Cython/Includes/libc/
+-rw-rw-r--   0        0        0       13 2015-06-22 12:53:10.000000 Cython/Includes/libc/__init__.pxd
+-rw-rw-r--   0        0        0     1224 2021-05-24 14:21:44.000000 Cython/Includes/libc/complex.pxd
+-rw-rw-r--   0        0        0     2050 2016-12-10 15:41:14.000000 Cython/Includes/libc/errno.pxd
+-rw-rw-r--   0        0        0      966 2016-12-10 15:41:14.000000 Cython/Includes/libc/float.pxd
+-rw-rw-r--   0        0        0      621 2018-09-22 14:18:56.000000 Cython/Includes/libc/limits.pxd
+-rw-rw-r--   0        0        0     1140 2016-12-10 15:41:14.000000 Cython/Includes/libc/locale.pxd
+-rw-rw-r--   0        0        0     6581 2021-05-24 14:21:44.000000 Cython/Includes/libc/math.pxd
+-rw-rw-r--   0        0        0      297 2016-12-10 15:41:14.000000 Cython/Includes/libc/setjmp.pxd
+-rw-rw-r--   0        0        0     1170 2018-09-22 14:18:56.000000 Cython/Includes/libc/signal.pxd
+-rw-rw-r--   0        0        0      164 2016-12-10 15:41:14.000000 Cython/Includes/libc/stddef.pxd
+-rw-rw-r--   0        0        0     3449 2016-12-10 15:41:14.000000 Cython/Includes/libc/stdint.pxd
+-rw-rw-r--   0        0        0     2476 2016-12-10 15:41:14.000000 Cython/Includes/libc/stdio.pxd
+-rw-rw-r--   0        0        0     2444 2016-12-10 15:41:14.000000 Cython/Includes/libc/stdlib.pxd
+-rw-rw-r--   0        0        0     2038 2016-12-10 15:41:14.000000 Cython/Includes/libc/string.pxd
+-rw-rw-r--   0        0        0     1354 2021-05-24 14:21:54.000000 Cython/Includes/libc/time.pxd
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:06.000000 Cython/Includes/libcpp/
+-rw-rw-r--   0        0        0       94 2015-09-10 16:25:36.000000 Cython/Includes/libcpp/__init__.pxd
+-rw-rw-r--   0        0        0     8321 2021-05-24 14:21:44.000000 Cython/Includes/libcpp/algorithm.pxd
+-rw-rw-r--   0        0        0     1762 2021-05-24 14:21:44.000000 Cython/Includes/libcpp/atomic.pxd
+-rw-rw-r--   0        0        0      501 2015-06-22 12:53:10.000000 Cython/Includes/libcpp/cast.pxd
+-rw-rw-r--   0        0        0     3012 2015-06-22 12:53:10.000000 Cython/Includes/libcpp/complex.pxd
+-rw-rw-r--   0        0        0     3223 2021-05-24 14:21:54.000000 Cython/Includes/libcpp/deque.pxd
+-rw-rw-r--   0        0        0     2392 2020-04-19 09:26:02.000000 Cython/Includes/libcpp/forward_list.pxd
+-rw-rw-r--   0        0        0      601 2021-05-24 14:21:44.000000 Cython/Includes/libcpp/functional.pxd
+-rw-rw-r--   0        0        0     1512 2021-05-24 14:21:44.000000 Cython/Includes/libcpp/iterator.pxd
+-rw-rw-r--   0        0        0     1661 2017-09-16 07:37:00.000000 Cython/Includes/libcpp/limits.pxd
+-rw-rw-r--   0        0        0     2721 2021-05-24 14:21:54.000000 Cython/Includes/libcpp/list.pxd
+-rw-rw-r--   0        0        0     2551 2020-04-19 09:26:02.000000 Cython/Includes/libcpp/map.pxd
+-rw-rw-r--   0        0        0     3662 2021-05-24 14:21:54.000000 Cython/Includes/libcpp/memory.pxd
+-rw-rw-r--   0        0        0     1411 2021-05-24 14:21:44.000000 Cython/Includes/libcpp/numeric.pxd
+-rw-rw-r--   0        0        0       27 2015-06-22 12:53:10.000000 Cython/Includes/libcpp/pair.pxd
+-rw-rw-r--   0        0        0      649 2020-04-19 09:26:02.000000 Cython/Includes/libcpp/queue.pxd
+-rw-rw-r--   0        0        0     2170 2020-04-19 09:26:02.000000 Cython/Includes/libcpp/set.pxd
+-rw-rw-r--   0        0        0      292 2016-12-10 15:41:14.000000 Cython/Includes/libcpp/stack.pxd
+-rw-rw-r--   0        0        0     6411 2021-05-24 14:21:54.000000 Cython/Includes/libcpp/string.pxd
+-rw-rw-r--   0        0        0      524 2016-12-10 15:41:14.000000 Cython/Includes/libcpp/typeindex.pxd
+-rw-rw-r--   0        0        0      304 2016-12-10 15:41:14.000000 Cython/Includes/libcpp/typeinfo.pxd
+-rw-rw-r--   0        0        0     2867 2020-07-31 07:03:12.000000 Cython/Includes/libcpp/unordered_map.pxd
+-rw-rw-r--   0        0        0     2622 2020-04-19 09:26:02.000000 Cython/Includes/libcpp/unordered_set.pxd
+-rw-rw-r--   0        0        0     1040 2021-05-24 14:21:54.000000 Cython/Includes/libcpp/utility.pxd
+-rw-rw-r--   0        0        0     3368 2021-05-24 14:21:54.000000 Cython/Includes/libcpp/vector.pxd
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:06.000000 Cython/Includes/numpy/
+-rw-rw-r--   0        0        0    36520 2021-05-24 14:21:54.000000 Cython/Includes/numpy/__init__.pxd
+-rw-rw-r--   0        0        0     5807 2016-12-10 15:41:14.000000 Cython/Includes/numpy/math.pxd
+-rw-rw-r--   0        0        0     1713 2016-12-10 15:41:14.000000 Cython/Includes/openmp.pxd
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:06.000000 Cython/Includes/posix/
+-rw-rw-r--   0        0        0       13 2015-06-22 12:53:10.000000 Cython/Includes/posix/__init__.pxd
+-rw-rw-r--   0        0        0      356 2021-05-24 14:21:44.000000 Cython/Includes/posix/dlfcn.pxd
+-rw-rw-r--   0        0        0     1194 2021-05-24 14:21:54.000000 Cython/Includes/posix/fcntl.pxd
+-rw-rw-r--   0        0        0       99 2016-12-10 15:41:14.000000 Cython/Includes/posix/ioctl.pxd
+-rw-rw-r--   0        0        0     3363 2021-05-24 14:21:44.000000 Cython/Includes/posix/mman.pxd
+-rw-rw-r--   0        0        0     1255 2021-05-24 14:21:44.000000 Cython/Includes/posix/resource.pxd
+-rw-rw-r--   0        0        0      546 2016-12-10 15:41:14.000000 Cython/Includes/posix/select.pxd
+-rw-rw-r--   0        0        0     1876 2020-05-19 07:31:38.000000 Cython/Includes/posix/signal.pxd
+-rw-rw-r--   0        0        0     1734 2018-09-22 14:18:56.000000 Cython/Includes/posix/stat.pxd
+-rw-rw-r--   0        0        0     1055 2021-05-24 14:21:44.000000 Cython/Includes/posix/stdio.pxd
+-rw-rw-r--   0        0        0      935 2021-05-24 14:21:44.000000 Cython/Includes/posix/stdlib.pxd
+-rw-rw-r--   0        0        0      374 2016-12-10 15:41:14.000000 Cython/Includes/posix/strings.pxd
+-rw-rw-r--   0        0        0     1981 2021-05-24 14:21:44.000000 Cython/Includes/posix/time.pxd
+-rw-rw-r--   0        0        0     1162 2017-09-16 07:37:00.000000 Cython/Includes/posix/types.pxd
+-rw-rw-r--   0        0        0     8061 2016-12-10 15:41:14.000000 Cython/Includes/posix/unistd.pxd
+-rw-rw-r--   0        0        0     1245 2021-05-24 14:21:44.000000 Cython/Includes/posix/wait.pxd
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:06.000000 Cython/Plex/
+-rw-rw-r--   0        0        0     1155 2021-05-24 14:21:44.000000 Cython/Plex/__init__.py
+-rw-rw-r--   0        0        0      581 2021-05-24 14:21:54.000000 Cython/Plex/Actions.pxd
+-rw-rw-r--   0        0        0     2919 2021-05-24 14:21:54.000000 Cython/Plex/Actions.py
+-rw-rw-r--   0        0        0      776 2021-05-24 14:21:44.000000 Cython/Plex/DFA.pxd
+-rw-rw-r--   0        0        0     5427 2021-05-24 14:21:44.000000 Cython/Plex/DFA.py
+-rw-rw-r--   0        0        0      976 2021-05-24 14:21:44.000000 Cython/Plex/Errors.py
+-rw-rw-r--   0        0        0     5944 2021-05-24 14:21:44.000000 Cython/Plex/Lexicons.py
+-rw-rw-r--   0        0        0      734 2021-05-24 14:21:44.000000 Cython/Plex/Machines.pxd
+-rw-rw-r--   0        0        0     7687 2021-05-24 14:21:54.000000 Cython/Plex/Machines.py
+-rw-rw-r--   0        0        0    14957 2021-05-24 14:21:44.000000 Cython/Plex/Regexps.py
+-rw-rw-r--   0        0        0     1437 2021-05-24 14:21:44.000000 Cython/Plex/Scanners.pxd
+-rw-rw-r--   0        0        0    11960 2021-05-24 14:21:44.000000 Cython/Plex/Scanners.py
+-rw-rw-r--   0        0        0      590 2021-05-24 14:21:44.000000 Cython/Plex/Transitions.pxd
+-rw-rw-r--   0        0        0     6761 2021-05-24 14:21:44.000000 Cython/Plex/Transitions.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:06.000000 Cython/Runtime/
+-rw-rw-r--   0        0        0       13 2015-06-22 12:53:10.000000 Cython/Runtime/__init__.py
+-rw-rw-r--   0        0        0     6599 2021-05-24 14:21:44.000000 Cython/Runtime/refnanny.pyx
+-rw-rw-r--   0        0        0    14898 2021-05-24 14:21:54.000000 Cython/Shadow.py
+-rw-rw-r--   0        0        0     5092 2021-05-24 14:21:54.000000 Cython/StringIOTree.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:06.000000 Cython/Tempita/
+-rw-rw-r--   0        0        0      152 2015-09-10 16:25:36.000000 Cython/Tempita/__init__.py
+-rw-rw-r--   0        0        0     4168 2015-06-22 12:53:10.000000 Cython/Tempita/_looper.py
+-rw-rw-r--   0        0        0    39626 2021-05-24 14:21:44.000000 Cython/Tempita/_tempita.py
+-rw-rw-r--   0        0        0      903 2015-09-10 16:25:36.000000 Cython/Tempita/compat3.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:06.000000 Cython/Tests/
+-rw-rw-r--   0        0        0       13 2015-06-22 12:53:10.000000 Cython/Tests/__init__.py
+-rw-rw-r--   0        0        0     3799 2021-05-24 14:21:54.000000 Cython/Tests/TestCodeWriter.py
+-rw-rw-r--   0        0        0      474 2020-04-19 09:26:02.000000 Cython/Tests/TestCythonUtils.py
+-rw-rw-r--   0        0        0     7021 2021-05-24 14:21:44.000000 Cython/Tests/TestJediTyper.py
+-rw-rw-r--   0        0        0     1946 2015-09-10 16:25:36.000000 Cython/Tests/TestStringIOTree.py
+-rw-rw-r--   0        0        0    14781 2021-05-24 14:21:44.000000 Cython/Tests/xmlrunner.py
+-rw-rw-r--   0        0        0     8672 2021-05-24 14:21:44.000000 Cython/TestUtils.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:06.000000 Cython/Utility/
+-rw-rw-r--   0        0        0     1159 2016-12-10 15:41:14.000000 Cython/Utility/__init__.py
+-rw-rw-r--   0        0        0     4089 2021-05-24 14:21:54.000000 Cython/Utility/arrayarray.h
+-rw-rw-r--   0        0        0    42841 2021-05-24 14:21:54.000000 Cython/Utility/AsyncGen.c
+-rw-rw-r--   0        0        0    29865 2021-05-24 14:21:54.000000 Cython/Utility/Buffer.c
+-rw-rw-r--   0        0        0    16052 2021-05-24 14:21:54.000000 Cython/Utility/Builtins.c
+-rw-rw-r--   0        0        0      363 2021-05-24 14:21:44.000000 Cython/Utility/Capsule.c
+-rw-rw-r--   0        0        0     4419 2021-05-24 14:21:44.000000 Cython/Utility/CConvert.pyx
+-rw-rw-r--   0        0        0     2566 2018-09-22 14:18:56.000000 Cython/Utility/CMath.c
+-rw-rw-r--   0        0        0     4568 2021-05-24 14:21:44.000000 Cython/Utility/CommonStructures.c
+-rw-rw-r--   0        0        0    10043 2020-05-19 07:31:38.000000 Cython/Utility/Complex.c
+-rw-rw-r--   0        0        0    90130 2021-05-24 14:21:54.000000 Cython/Utility/Coroutine.c
+-rw-rw-r--   0        0        0     2634 2021-05-24 14:21:54.000000 Cython/Utility/CpdefEnums.pyx
+-rw-rw-r--   0        0        0     6875 2021-05-24 14:21:54.000000 Cython/Utility/CppConvert.pyx
+-rw-rw-r--   0        0        0     2973 2021-05-24 14:21:54.000000 Cython/Utility/CppSupport.cpp
+-rw-rw-r--   0        0        0    54798 2021-05-24 14:21:54.000000 Cython/Utility/CythonFunction.c
+-rw-rw-r--   0        0        0     6536 2021-05-24 14:21:54.000000 Cython/Utility/Embed.c
+-rw-rw-r--   0        0        0    26997 2021-05-24 14:21:54.000000 Cython/Utility/Exceptions.c
+-rw-rw-r--   0        0        0    16467 2021-05-24 14:21:54.000000 Cython/Utility/ExtensionTypes.c
+-rw-rw-r--   0        0        0    16993 2021-05-24 14:21:44.000000 Cython/Utility/FunctionArguments.c
+-rw-rw-r--   0        0        0    26437 2021-05-24 14:21:54.000000 Cython/Utility/ImportExport.c
+-rw-rw-r--   0        0        0    49969 2021-05-24 14:21:54.000000 Cython/Utility/MemoryView.pyx
+-rw-rw-r--   0        0        0    29690 2021-05-24 14:21:54.000000 Cython/Utility/MemoryView_C.c
+-rw-rw-r--   0        0        0    62713 2021-05-24 14:21:54.000000 Cython/Utility/ModuleSetupCode.c
+-rw-rw-r--   0        0        0      979 2021-05-24 14:21:44.000000 Cython/Utility/NumpyImportArray.c
+-rw-rw-r--   0        0        0   107997 2021-05-24 14:21:54.000000 Cython/Utility/ObjectHandling.c
+-rw-rw-r--   0        0        0    58777 2021-05-24 14:21:54.000000 Cython/Utility/Optimize.c
+-rw-rw-r--   0        0        0    16066 2021-05-24 14:21:44.000000 Cython/Utility/Overflow.c
+-rw-rw-r--   0        0        0     5103 2015-06-22 12:53:10.000000 Cython/Utility/Printing.c
+-rw-rw-r--   0        0        0    17204 2021-05-24 14:21:54.000000 Cython/Utility/Profile.c
+-rw-rw-r--   0        0        0    44719 2021-05-24 14:21:54.000000 Cython/Utility/StringTools.c
+-rw-rw-r--   0        0        0     1795 2021-05-24 14:21:44.000000 Cython/Utility/TestCythonScope.pyx
+-rw-rw-r--   0        0        0      152 2015-06-22 12:53:10.000000 Cython/Utility/TestCyUtilityLoader.pyx
+-rw-rw-r--   0        0        0      279 2015-06-22 12:53:10.000000 Cython/Utility/TestUtilityLoader.c
+-rw-rw-r--   0        0        0    38689 2021-05-24 14:21:54.000000 Cython/Utility/TypeConversion.c
+-rw-rw-r--   0        0        0    15960 2021-05-24 14:21:54.000000 Cython/Utils.py
+-rw-rw-r--   0        0        0      152 2021-09-09 02:03:10.000000 distutils-precedence.pth
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:10.000000 pkg_resources/
+-rw-rw-r--   0        0        0   108202 2021-09-09 02:02:40.000000 pkg_resources/__init__.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:10.000000 pkg_resources/_vendor/
+-rw-rw-r--   0        0        0        0 2021-09-09 02:02:40.000000 pkg_resources/_vendor/__init__.py
+-rw-rw-r--   0        0        0    24701 2021-09-09 02:02:40.000000 pkg_resources/_vendor/appdirs.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:10.000000 pkg_resources/_vendor/packaging/
+-rw-rw-r--   0        0        0      736 2021-09-09 02:02:40.000000 pkg_resources/_vendor/packaging/__about__.py
+-rw-rw-r--   0        0        0      562 2021-09-09 02:02:40.000000 pkg_resources/_vendor/packaging/__init__.py
+-rw-rw-r--   0        0        0     1128 2021-09-09 02:02:40.000000 pkg_resources/_vendor/packaging/_compat.py
+-rw-rw-r--   0        0        0     2022 2021-09-09 02:02:40.000000 pkg_resources/_vendor/packaging/_structures.py
+-rw-rw-r--   0        0        0     1812 2021-09-09 02:02:40.000000 pkg_resources/_vendor/packaging/_typing.py
+-rw-rw-r--   0        0        0     9518 2021-09-09 02:02:40.000000 pkg_resources/_vendor/packaging/markers.py
+-rw-rw-r--   0        0        0     4929 2021-09-09 02:02:40.000000 pkg_resources/_vendor/packaging/requirements.py
+-rw-rw-r--   0        0        0    31944 2021-09-09 02:02:40.000000 pkg_resources/_vendor/packaging/specifiers.py
+-rw-rw-r--   0        0        0    24067 2021-09-09 02:02:40.000000 pkg_resources/_vendor/packaging/tags.py
+-rw-rw-r--   0        0        0     1811 2021-09-09 02:02:40.000000 pkg_resources/_vendor/packaging/utils.py
+-rw-rw-r--   0        0        0    15470 2021-09-09 02:02:40.000000 pkg_resources/_vendor/packaging/version.py
+-rw-rw-r--   0        0        0   232056 2021-09-09 02:02:40.000000 pkg_resources/_vendor/pyparsing.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:10.000000 pkg_resources/extern/
+-rw-rw-r--   0        0        0     2362 2021-09-09 02:02:40.000000 pkg_resources/extern/__init__.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:10.000000 pkg_resources/tests/
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:10.000000 pkg_resources/tests/data/
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:10.000000 pkg_resources/tests/data/my-test-package-source/
+-rw-rw-r--   0        0        0      104 2021-09-09 02:02:40.000000 pkg_resources/tests/data/my-test-package-source/setup.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:06.000000 pyximport/
+-rw-rw-r--   0        0        0       79 2015-09-10 16:25:36.000000 pyximport/__init__.py
+-rw-rw-r--   0        0        0     5707 2021-05-24 14:21:44.000000 pyximport/pyxbuild.py
+-rw-rw-r--   0        0        0    23547 2021-05-24 14:21:44.000000 pyximport/pyximport.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:10.000000 setuptools-58.0.4.dist-info/
+-rw-rw-r--   0        0        0     2636 2021-09-09 02:03:10.000000 setuptools-58.0.4.dist-info/entry_points.txt
+-rw-rw-r--   0        0        0     1050 2021-09-09 02:03:10.000000 setuptools-58.0.4.dist-info/LICENSE
+-rw-rw-r--   0        0        0     4852 2021-09-09 02:03:10.000000 setuptools-58.0.4.dist-info/METADATA
+-rw-rw-r--   0        0        0    13981 2021-09-09 02:03:12.000000 setuptools-58.0.4.dist-info/RECORD
+-rw-rw-r--   0        0        0       41 2021-09-09 02:03:10.000000 setuptools-58.0.4.dist-info/top_level.txt
+-rw-rw-r--   0        0        0       92 2021-09-09 02:03:10.000000 setuptools-58.0.4.dist-info/WHEEL
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:10.000000 setuptools/
+-rw-rw-r--   0        0        0     7448 2021-09-09 02:02:40.000000 setuptools/__init__.py
+-rw-rw-r--   0        0        0      218 2021-09-09 02:02:40.000000 setuptools/_deprecation_warning.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:10.000000 setuptools/_distutils/
+-rw-rw-r--   0        0        0      250 2021-09-09 02:02:40.000000 setuptools/_distutils/__init__.py
+-rw-rw-r--   0        0        0    20813 2021-09-09 02:02:40.000000 setuptools/_distutils/_msvccompiler.py
+-rw-rw-r--   0        0        0     8572 2021-09-09 02:02:40.000000 setuptools/_distutils/archive_util.py
+-rw-rw-r--   0        0        0    14894 2021-09-09 02:02:40.000000 setuptools/_distutils/bcppcompiler.py
+-rw-rw-r--   0        0        0    47607 2021-09-09 02:02:40.000000 setuptools/_distutils/ccompiler.py
+-rw-rw-r--   0        0        0    18079 2021-09-09 02:02:40.000000 setuptools/_distutils/cmd.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:10.000000 setuptools/_distutils/command/
+-rw-rw-r--   0        0        0      799 2021-09-09 02:02:40.000000 setuptools/_distutils/command/__init__.py
+-rw-rw-r--   0        0        0     5562 2021-09-09 02:02:40.000000 setuptools/_distutils/command/bdist.py
+-rw-rw-r--   0        0        0     4913 2021-09-09 02:02:40.000000 setuptools/_distutils/command/bdist_dumb.py
+-rw-rw-r--   0        0        0    35579 2021-09-09 02:02:40.000000 setuptools/_distutils/command/bdist_msi.py
+-rw-rw-r--   0        0        0    21537 2021-09-09 02:02:40.000000 setuptools/_distutils/command/bdist_rpm.py
+-rw-rw-r--   0        0        0    16030 2021-09-09 02:02:40.000000 setuptools/_distutils/command/bdist_wininst.py
+-rw-rw-r--   0        0        0     5773 2021-09-09 02:02:40.000000 setuptools/_distutils/command/build.py
+-rw-rw-r--   0        0        0     8022 2021-09-09 02:02:40.000000 setuptools/_distutils/command/build_clib.py
+-rw-rw-r--   0        0        0    31720 2021-09-09 02:02:40.000000 setuptools/_distutils/command/build_ext.py
+-rw-rw-r--   0        0        0    16495 2021-09-09 02:02:40.000000 setuptools/_distutils/command/build_py.py
+-rw-rw-r--   0        0        0     5963 2021-09-09 02:02:40.000000 setuptools/_distutils/command/build_scripts.py
+-rw-rw-r--   0        0        0     5637 2021-09-09 02:02:40.000000 setuptools/_distutils/command/check.py
+-rw-rw-r--   0        0        0     2776 2021-09-09 02:02:40.000000 setuptools/_distutils/command/clean.py
+-rw-rw-r--   0        0        0    13117 2021-09-09 02:02:40.000000 setuptools/_distutils/command/config.py
+-rw-rw-r--   0        0        0    27488 2021-09-09 02:02:40.000000 setuptools/_distutils/command/install.py
+-rw-rw-r--   0        0        0     2822 2021-09-09 02:02:40.000000 setuptools/_distutils/command/install_data.py
+-rw-rw-r--   0        0        0     2603 2021-09-09 02:02:40.000000 setuptools/_distutils/command/install_egg_info.py
+-rw-rw-r--   0        0        0     1298 2021-09-09 02:02:40.000000 setuptools/_distutils/command/install_headers.py
+-rw-rw-r--   0        0        0     8397 2021-09-09 02:02:40.000000 setuptools/_distutils/command/install_lib.py
+-rw-rw-r--   0        0        0     2017 2021-09-09 02:02:40.000000 setuptools/_distutils/command/install_scripts.py
+-rw-rw-r--   0        0        0      671 2021-09-09 02:02:40.000000 setuptools/_distutils/command/py37compat.py
+-rw-rw-r--   0        0        0    11712 2021-09-09 02:02:40.000000 setuptools/_distutils/command/register.py
+-rw-rw-r--   0        0        0    19005 2021-09-09 02:02:40.000000 setuptools/_distutils/command/sdist.py
+-rw-rw-r--   0        0        0     7597 2021-09-09 02:02:40.000000 setuptools/_distutils/command/upload.py
+-rw-rw-r--   0        0        0     4827 2021-09-09 02:02:40.000000 setuptools/_distutils/config.py
+-rw-rw-r--   0        0        0     8876 2021-09-09 02:02:40.000000 setuptools/_distutils/core.py
+-rw-rw-r--   0        0        0    16938 2021-09-09 02:02:40.000000 setuptools/_distutils/cygwinccompiler.py
+-rw-rw-r--   0        0        0      139 2021-09-09 02:02:40.000000 setuptools/_distutils/debug.py
+-rw-rw-r--   0        0        0     3491 2021-09-09 02:02:40.000000 setuptools/_distutils/dep_util.py
+-rw-rw-r--   0        0        0     7778 2021-09-09 02:02:40.000000 setuptools/_distutils/dir_util.py
+-rw-rw-r--   0        0        0    50421 2021-09-09 02:02:40.000000 setuptools/_distutils/dist.py
+-rw-rw-r--   0        0        0     3577 2021-09-09 02:02:40.000000 setuptools/_distutils/errors.py
+-rw-rw-r--   0        0        0    10515 2021-09-09 02:02:40.000000 setuptools/_distutils/extension.py
+-rw-rw-r--   0        0        0    17784 2021-09-09 02:02:40.000000 setuptools/_distutils/fancy_getopt.py
+-rw-rw-r--   0        0        0     8148 2021-09-09 02:02:40.000000 setuptools/_distutils/file_util.py
+-rw-rw-r--   0        0        0    13407 2021-09-09 02:02:40.000000 setuptools/_distutils/filelist.py
+-rw-rw-r--   0        0        0     1969 2021-09-09 02:02:40.000000 setuptools/_distutils/log.py
+-rw-rw-r--   0        0        0    30453 2021-09-09 02:02:40.000000 setuptools/_distutils/msvc9compiler.py
+-rw-rw-r--   0        0        0    23540 2021-09-09 02:02:40.000000 setuptools/_distutils/msvccompiler.py
+-rw-rw-r--   0        0        0      455 2021-09-09 02:02:40.000000 setuptools/_distutils/py35compat.py
+-rw-rw-r--   0        0        0      212 2021-09-09 02:02:40.000000 setuptools/_distutils/py38compat.py
+-rw-rw-r--   0        0        0     3498 2021-09-09 02:02:40.000000 setuptools/_distutils/spawn.py
+-rw-rw-r--   0        0        0    21349 2021-09-09 02:02:40.000000 setuptools/_distutils/sysconfig.py
+-rw-rw-r--   0        0        0    12483 2021-09-09 02:02:40.000000 setuptools/_distutils/text_file.py
+-rw-rw-r--   0        0        0    14957 2021-09-09 02:02:40.000000 setuptools/_distutils/unixccompiler.py
+-rw-rw-r--   0        0        0    20373 2021-09-09 02:02:40.000000 setuptools/_distutils/util.py
+-rw-rw-r--   0        0        0    12514 2021-09-09 02:02:40.000000 setuptools/_distutils/version.py
+-rw-rw-r--   0        0        0     5133 2021-09-09 02:02:40.000000 setuptools/_distutils/versionpredicate.py
+-rw-rw-r--   0        0        0     2392 2021-09-09 02:02:40.000000 setuptools/_imp.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:10.000000 setuptools/_vendor/
+-rw-rw-r--   0        0        0        0 2021-09-09 02:02:40.000000 setuptools/_vendor/__init__.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:10.000000 setuptools/_vendor/more_itertools/
+-rw-rw-r--   0        0        0       82 2021-09-09 02:02:40.000000 setuptools/_vendor/more_itertools/__init__.py
+-rw-rw-r--   0        0        0   117968 2021-09-09 02:02:40.000000 setuptools/_vendor/more_itertools/more.py
+-rw-rw-r--   0        0        0    16256 2021-09-09 02:02:40.000000 setuptools/_vendor/more_itertools/recipes.py
+-rw-rw-r--   0        0        0    15130 2021-09-09 02:02:40.000000 setuptools/_vendor/ordered_set.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:10.000000 setuptools/_vendor/packaging/
+-rw-rw-r--   0        0        0      736 2021-09-09 02:02:40.000000 setuptools/_vendor/packaging/__about__.py
+-rw-rw-r--   0        0        0      562 2021-09-09 02:02:40.000000 setuptools/_vendor/packaging/__init__.py
+-rw-rw-r--   0        0        0     1128 2021-09-09 02:02:40.000000 setuptools/_vendor/packaging/_compat.py
+-rw-rw-r--   0        0        0     2022 2021-09-09 02:02:40.000000 setuptools/_vendor/packaging/_structures.py
+-rw-rw-r--   0        0        0     1812 2021-09-09 02:02:40.000000 setuptools/_vendor/packaging/_typing.py
+-rw-rw-r--   0        0        0     9509 2021-09-09 02:02:40.000000 setuptools/_vendor/packaging/markers.py
+-rw-rw-r--   0        0        0     4917 2021-09-09 02:02:40.000000 setuptools/_vendor/packaging/requirements.py
+-rw-rw-r--   0        0        0    31944 2021-09-09 02:02:40.000000 setuptools/_vendor/packaging/specifiers.py
+-rw-rw-r--   0        0        0    24067 2021-09-09 02:02:40.000000 setuptools/_vendor/packaging/tags.py
+-rw-rw-r--   0        0        0     1811 2021-09-09 02:02:40.000000 setuptools/_vendor/packaging/utils.py
+-rw-rw-r--   0        0        0    15470 2021-09-09 02:02:40.000000 setuptools/_vendor/packaging/version.py
+-rw-rw-r--   0        0        0   232056 2021-09-09 02:02:40.000000 setuptools/_vendor/pyparsing.py
+-rw-rw-r--   0        0        0     7077 2021-09-09 02:02:40.000000 setuptools/archive_util.py
+-rw-rw-r--   0        0        0    10280 2021-09-09 02:02:40.000000 setuptools/build_meta.py
+-rw-rw-r--   0        0        0    65536 2021-09-09 02:02:40.000000 setuptools/cli-32.exe
+-rw-rw-r--   0        0        0    74752 2021-09-09 02:02:40.000000 setuptools/cli-64.exe
+-rw-rw-r--   0        0        0    65536 2021-09-09 02:02:40.000000 setuptools/cli.exe
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:10.000000 setuptools/command/
+-rw-rw-r--   0        0        0      217 2021-09-09 02:02:40.000000 setuptools/command/__init__.py
+-rw-rw-r--   0        0        0     2381 2021-09-09 02:02:40.000000 setuptools/command/alias.py
+-rw-rw-r--   0        0        0    16604 2021-09-09 02:02:40.000000 setuptools/command/bdist_egg.py
+-rw-rw-r--   0        0        0      900 2021-09-09 02:02:40.000000 setuptools/command/bdist_rpm.py
+-rw-rw-r--   0        0        0     4415 2021-09-09 02:02:40.000000 setuptools/command/build_clib.py
+-rw-rw-r--   0        0        0    13212 2021-09-09 02:02:40.000000 setuptools/command/build_ext.py
+-rw-rw-r--   0        0        0     8276 2021-09-09 02:02:40.000000 setuptools/command/build_py.py
+-rw-rw-r--   0        0        0     7012 2021-09-09 02:02:40.000000 setuptools/command/develop.py
+-rw-rw-r--   0        0        0      960 2021-09-09 02:02:40.000000 setuptools/command/dist_info.py
+-rw-rw-r--   0        0        0    85341 2021-09-09 02:02:40.000000 setuptools/command/easy_install.py
+-rw-rw-r--   0        0        0    25335 2021-09-09 02:02:40.000000 setuptools/command/egg_info.py
+-rw-rw-r--   0        0        0     4705 2021-09-09 02:02:40.000000 setuptools/command/install.py
+-rw-rw-r--   0        0        0     2203 2021-09-09 02:02:40.000000 setuptools/command/install_egg_info.py
+-rw-rw-r--   0        0        0     3875 2021-09-09 02:02:40.000000 setuptools/command/install_lib.py
+-rw-rw-r--   0        0        0     2593 2021-09-09 02:02:40.000000 setuptools/command/install_scripts.py
+-rw-rw-r--   0        0        0      628 2021-09-09 02:02:40.000000 setuptools/command/launcher manifest.xml
+-rw-rw-r--   0        0        0     4946 2021-09-09 02:02:40.000000 setuptools/command/py36compat.py
+-rw-rw-r--   0        0        0      468 2021-09-09 02:02:40.000000 setuptools/command/register.py
+-rw-rw-r--   0        0        0     2128 2021-09-09 02:02:40.000000 setuptools/command/rotate.py
+-rw-rw-r--   0        0        0      658 2021-09-09 02:02:40.000000 setuptools/command/saveopts.py
+-rw-rw-r--   0        0        0     5967 2021-09-09 02:02:40.000000 setuptools/command/sdist.py
+-rw-rw-r--   0        0        0     5086 2021-09-09 02:02:40.000000 setuptools/command/setopt.py
+-rw-rw-r--   0        0        0     8088 2021-09-09 02:02:40.000000 setuptools/command/test.py
+-rw-rw-r--   0        0        0      462 2021-09-09 02:02:40.000000 setuptools/command/upload.py
+-rw-rw-r--   0        0        0     7218 2021-09-09 02:02:40.000000 setuptools/command/upload_docs.py
+-rw-rw-r--   0        0        0    23123 2021-09-09 02:02:40.000000 setuptools/config.py
+-rw-rw-r--   0        0        0      949 2021-09-09 02:02:40.000000 setuptools/dep_util.py
+-rw-rw-r--   0        0        0     5474 2021-09-09 02:02:40.000000 setuptools/depends.py
+-rw-rw-r--   0        0        0    43087 2021-09-09 02:02:40.000000 setuptools/dist.py
+-rw-rw-r--   0        0        0      524 2021-09-09 02:02:40.000000 setuptools/errors.py
+-rw-rw-r--   0        0        0     1684 2021-09-09 02:02:40.000000 setuptools/extension.py
+drwxrwxr-x   0        0        0        0 2021-09-10 16:48:10.000000 setuptools/extern/
+-rw-rw-r--   0        0        0     2407 2021-09-09 02:02:40.000000 setuptools/extern/__init__.py
+-rw-rw-r--   0        0        0     4873 2021-09-09 02:02:40.000000 setuptools/glob.py
+-rw-rw-r--   0        0        0    65536 2021-09-09 02:02:40.000000 setuptools/gui-32.exe
+-rw-rw-r--   0        0        0    75264 2021-09-09 02:02:40.000000 setuptools/gui-64.exe
+-rw-rw-r--   0        0        0    65536 2021-09-09 02:02:40.000000 setuptools/gui.exe
+-rw-rw-r--   0        0        0     3567 2021-09-09 02:02:40.000000 setuptools/installer.py
+-rw-rw-r--   0        0        0      812 2021-09-09 02:02:40.000000 setuptools/launch.py
+-rw-rw-r--   0        0        0     5217 2021-09-09 02:02:40.000000 setuptools/monkey.py
+-rw-rw-r--   0        0        0    50561 2021-09-09 02:02:40.000000 setuptools/msvc.py
+-rw-rw-r--   0        0        0     3093 2021-09-09 02:02:40.000000 setuptools/namespaces.py
+-rw-rw-r--   0        0        0    39886 2021-09-09 02:02:40.000000 setuptools/package_index.py
+-rw-rw-r--   0        0        0      245 2021-09-09 02:02:40.000000 setuptools/py34compat.py
+-rw-rw-r--   0        0        0    14348 2021-09-09 02:02:40.000000 setuptools/sandbox.py
+-rw-rw-r--   0        0        0      218 2021-09-09 02:02:40.000000 setuptools/script (dev).tmpl
+-rw-rw-r--   0        0        0      138 2021-09-09 02:02:40.000000 setuptools/script.tmpl
+-rw-rw-r--   0        0        0      941 2021-09-09 02:02:40.000000 setuptools/unicode_utils.py
+-rw-rw-r--   0        0        0      144 2021-09-09 02:02:40.000000 setuptools/version.py
+-rw-rw-r--   0        0        0     8288 2021-09-09 02:02:40.000000 setuptools/wheel.py
+-rw-rw-r--   0        0        0      714 2021-09-09 02:02:40.000000 setuptools/windows_support.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+Zip archive data, at least v2.0 to extract, compression method=store
```

### filetype from diffoscope

```diff
@@ -1 +1 @@
-TarFile
+ZipFile
```

### Comparing `pyportable-crypto-1.0.3/LICENSE` & `setuptools-58.0.4.dist-info/LICENSE`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-MIT License
-
-Copyright (c) 2021 likianta
+Copyright Jason R. Coombs
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
+of this software and associated documentation files (the "Software"), to
+deal in the Software without restriction, including without limitation the
+rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
+sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
+IN THE SOFTWARE.
```

