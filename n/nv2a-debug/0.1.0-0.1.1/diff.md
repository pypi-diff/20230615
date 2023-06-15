# Comparing `tmp/nv2a_debug-0.1.0.tar.gz` & `tmp/nv2a_debug-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nv2a_debug-0.1.0.tar", last modified: Tue Jun 13 14:04:35 2023, max compression
+gzip compressed data, was "nv2a_debug-0.1.1.tar", last modified: Thu Jun 15 07:57:05 2023, max compression
```

## Comparing `nv2a_debug-0.1.0.tar` & `nv2a_debug-0.1.1.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/build_cffi.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      252 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.647108 nv2a_debug-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.647108 nv2a_debug-0.1.0/src/nv2a_debug.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-13 14:04:35.000000 nv2a_debug-0.1.0/src/nv2a_debug.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-13 14:04:35.000000 nv2a_debug-0.1.0/src/nv2a_debug.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:04:35.000000 nv2a_debug-0.1.0/src/nv2a_debug.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 14:04:35.000000 nv2a_debug-0.1.0/src/nv2a_debug.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-13 14:04:35.000000 nv2a_debug-0.1.0/src/nv2a_debug.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 14:04:35.000000 nv2a_debug-0.1.0/src/nv2a_debug.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/src/nv2adbg/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23394 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/_code_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/_file_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/_input_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/_output_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/_program_inputs_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/_program_outputs_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/_register_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/_shader_program.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8132 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/py_nv2a_vsh_emu.py
--rw-r--r--   0 runner    (1001) docker     (123)    19482 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/src/nv2adbg/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/tests/test__code_panel_build_ancestor_root_segments.py
--rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-06-13 14:04:29.000000 nv2a_debug-0.1.0/tests/test__code_panel_build_contributing_source_segments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.647108 nv2a_debug-0.1.0/thirdparty/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.647108 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/githooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3097 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/githooks/pre-commit
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.c
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.h
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.c
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.h
--rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.c
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.h
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.c
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.647108 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/disassembler/
--rw-r--r--   0 runner    (1001) docker     (123)    21365 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/disassembler/test_basic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/disassembler/test_main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/emulator/
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/emulator/test_basic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/emulator/test_main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:35.651108 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/operations/
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/operations/test_basic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-13 14:04:30.000000 nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/operations/test_main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.681933 nv2a_debug-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-15 07:57:05.681933 nv2a_debug-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/build_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-15 07:57:05.681933 nv2a_debug-0.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      252 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.673933 nv2a_debug-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.677933 nv2a_debug-0.1.1/src/nv2a_debug.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-15 07:57:05.000000 nv2a_debug-0.1.1/src/nv2a_debug.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-15 07:57:05.000000 nv2a_debug-0.1.1/src/nv2a_debug.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:57:05.000000 nv2a_debug-0.1.1/src/nv2a_debug.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 07:57:05.000000 nv2a_debug-0.1.1/src/nv2a_debug.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 07:57:05.000000 nv2a_debug-0.1.1/src/nv2a_debug.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 07:57:05.000000 nv2a_debug-0.1.1/src/nv2a_debug.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.677933 nv2a_debug-0.1.1/src/nv2adbg/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23394 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_code_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_error_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_file_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_input_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_output_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_program_inputs_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_program_outputs_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_program_vertex_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_register_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/_shader_program.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8002 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/py_nv2a_vsh_emu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19482 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/src/nv2adbg/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.677933 nv2a_debug-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/tests/test__code_panel_build_ancestor_root_segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/tests/test__code_panel_build_contributing_source_segments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.677933 nv2a_debug-0.1.1/thirdparty/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.681933 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.677933 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.681933 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.681933 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/githooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3097 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/githooks/pre-commit
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.681933 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.c
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.h
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.677933 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.681933 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/disassembler/
+-rw-r--r--   0 runner    (1001) docker     (123)    21365 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/disassembler/test_basic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/disassembler/test_main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.681933 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/emulator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/emulator/test_basic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/emulator/test_main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:05.681933 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/operations/test_basic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 07:57:01.000000 nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/operations/test_main.cpp
```

### Comparing `nv2a_debug-0.1.0/LICENSE` & `nv2a_debug-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/PKG-INFO` & `nv2a_debug-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nv2a_debug
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simulator/debugger for the Xbox nv2a vertex shader
 Home-page: https://github.com/abaire/nv2a_vsh_debug
 Author: Erik Abair
 Author-email: erik.abair@bearbrains.work
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/abaire/nv2a_vsh_debug/issues
 Platform: UNKNOWN
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Simulator/debugger for the original Xbox nv2a vertex shader.
 
 # Use
 
-Run with `--help` to see command line options.
+Run `nv2adbg` with `--help` to see command line options.
 
 ## Menus
 
 ### File menu
 
 Allows inputs to be configured.
```

### Comparing `nv2a_debug-0.1.0/README.md` & `nv2a_debug-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Simulator/debugger for the original Xbox nv2a vertex shader.
 
 # Use
 
-Run with `--help` to see command line options.
+Run `nv2adbg` with `--help` to see command line options.
 
 ## Menus
 
 ### File menu
 
 Allows inputs to be configured.
```

### Comparing `nv2a_debug-0.1.0/build_cffi.py` & `nv2a_debug-0.1.1/build_cffi.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/setup.cfg` & `nv2a_debug-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nv2a_debug
-version = 0.1.0
+version = 0.1.1
 author = Erik Abair
 author_email = erik.abair@bearbrains.work
 description = Simulator/debugger for the Xbox nv2a vertex shader
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/abaire/nv2a_vsh_debug
 project_urls =
```

### Comparing `nv2a_debug-0.1.0/src/nv2a_debug.egg-info/PKG-INFO` & `nv2a_debug-0.1.1/src/nv2a_debug.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nv2a-debug
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simulator/debugger for the Xbox nv2a vertex shader
 Home-page: https://github.com/abaire/nv2a_vsh_debug
 Author: Erik Abair
 Author-email: erik.abair@bearbrains.work
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/abaire/nv2a_vsh_debug/issues
 Platform: UNKNOWN
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Simulator/debugger for the original Xbox nv2a vertex shader.
 
 # Use
 
-Run with `--help` to see command line options.
+Run `nv2adbg` with `--help` to see command line options.
 
 ## Menus
 
 ### File menu
 
 Allows inputs to be configured.
```

### Comparing `nv2a_debug-0.1.0/src/nv2a_debug.egg-info/SOURCES.txt` & `nv2a_debug-0.1.1/src/nv2a_debug.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,21 @@
 src/nv2a_debug.egg-info/dependency_links.txt
 src/nv2a_debug.egg-info/entry_points.txt
 src/nv2a_debug.egg-info/requires.txt
 src/nv2a_debug.egg-info/top_level.txt
 src/nv2adbg/__init__.py
 src/nv2adbg/_code_panel.py
 src/nv2adbg/_editor.py
+src/nv2adbg/_error_message.py
 src/nv2adbg/_file_menu.py
 src/nv2adbg/_input_panel.py
 src/nv2adbg/_output_panel.py
 src/nv2adbg/_program_inputs_viewer.py
 src/nv2adbg/_program_outputs_viewer.py
+src/nv2adbg/_program_vertex_viewer.py
 src/nv2adbg/_register_view.py
 src/nv2adbg/_shader_program.py
 src/nv2adbg/debugger.py
 src/nv2adbg/py_nv2a_vsh_emu.py
 src/nv2adbg/simulator.py
 tests/test__code_panel_build_ancestor_root_segments.py
 tests/test__code_panel_build_contributing_source_segments.py
```

### Comparing `nv2a_debug-0.1.0/src/nv2adbg/_code_panel.py` & `nv2a_debug-0.1.1/src/nv2adbg/_code_panel.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/src/nv2adbg/_editor.py` & `nv2a_debug-0.1.1/src/nv2adbg/_editor.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/src/nv2adbg/_file_menu.py` & `nv2a_debug-0.1.1/src/nv2adbg/_file_menu.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/src/nv2adbg/_input_panel.py` & `nv2a_debug-0.1.1/src/nv2adbg/_input_panel.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/src/nv2adbg/_output_panel.py` & `nv2a_debug-0.1.1/src/nv2adbg/_output_panel.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/src/nv2adbg/_program_inputs_viewer.py` & `nv2a_debug-0.1.1/src/nv2adbg/_program_inputs_viewer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Provides functionality to browse the input state."""
 
 from typing import Optional
 
-import textual.css.query
 from textual.app import ComposeResult
-from textual.containers import Center
-from textual.containers import Middle
-from textual.widgets import DataTable
-from textual.widgets import Label
+from textual.containers import Horizontal
+from textual.containers import VerticalScroll
+from textual.css import query
+from textual.reactive import reactive
+from textual.widgets import ContentSwitcher
 from textual.widgets import Static
 
-from nv2adbg import simulator
+from nv2adbg._error_message import _CenteredErrorMessage
+from nv2adbg._register_view import _RegisterSetPanel
+from nv2adbg.simulator import Context
 
 
 class _ProgramInputsViewer(Static):
     """Provides a browsing interface to view input registers and vertices."""
 
     DEFAULT_CSS = """
     _ProgramInputsViewer {
@@ -22,64 +24,74 @@
         width: 1fr;
     }
 
     _ProgramInputsViewer DataTable {
         height: 1fr;
     }
 
-    #center_message {
-        height: 1fr;
-        width: 1fr;
+    #inputs-table .registersetpanel--register {
+        color: $success;
+        text-style: bold;
     }
 
-    #empty_message {
-        border: double $error;
-        padding: 2 4;
-        content-align: center middle;
+    #constants-table .registersetpanel--border {
+        color: $warning;
+    }
+
+    #constants-table .registersetpanel--register {
+        color: $success;
+        text-style: bold;
     }
     """
 
+    _active_content = reactive("no-content", init=False)
+
     def __init__(self):
         super().__init__()
-        self._context: Optional[simulator.Context] = None
+        self._context: Optional[Context] = None
 
-    def set_context(self, context: simulator.Context):
+        self._inputs_table = _RegisterSetPanel("Inputs", id="inputs-table")
+        self._constants_table = _RegisterSetPanel("Constants", id="constants-table")
+
+    def set_context(self, context: Context):
         self._context = context
+        self._populate()
         self.update()
-        self._populate_table()
 
     def on_mount(self) -> None:
-        self._populate_table()
+        self._populate()
 
     def compose(self) -> ComposeResult:
-        if self._context:
-            table = DataTable()
-            table.add_columns("Register", "x", "y", "z", "w")
-            table.cursor_type = "row"
-            table.zebra_stripes = True
-            table.focus()
-            yield table
-        else:
-            yield Middle(
-                Center(
-                    Label(
-                        "No input context available, load data via the File menu.",
-                        id="empty_message",
-                    )
-                ),
-                id="center_message",
+        with ContentSwitcher(initial="no-content"):
+            with Horizontal(id="content"):
+                with VerticalScroll():
+                    yield self._inputs_table
+                with VerticalScroll():
+                    yield self._constants_table
+
+            yield _CenteredErrorMessage(
+                "No input context available, load data via the File menu.",
+                id="no-content",
             )
 
-    def _populate_table(self):
+    def _populate(self):
         try:
-            table = self.query_one(DataTable)
-            table.clear()
-
             if self._context:
-                for register in self._context.constants:
-                    table.add_row(
-                        register.name, register.x, register.y, register.z, register.w
-                    )
+                self._inputs_table.set_registers(self._context.inputs)
+
+                def rename_constant_register(name: str) -> str:
+                    return f"c[{name[1:]}]"
 
-        except textual.css.query.NoMatches:
+                self._constants_table.set_registers(
+                    self._context.constants, rename_constant_register
+                )
+                self._active_content = "content"
+            else:
+                self._active_content = "no-content"
+
+        except query.NoMatches:
             # The table is not loaded yet.
             pass
+
+    def _watch__active_content(self, _old_val: str, new_val: str):
+        del _old_val
+        self.query_one(ContentSwitcher).current = new_val
```

### Comparing `nv2a_debug-0.1.0/src/nv2adbg/_shader_program.py` & `nv2a_debug-0.1.1/src/nv2adbg/_shader_program.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Internal model of an nv2a shader program."""
 
 import csv
 import json
 import re
-from typing import Iterable, Optional
+from typing import Dict
+from typing import Iterable
+from typing import List
+from typing import Optional
 
 from nv2adbg import simulator
 
 # c[123]
 _CONSTANT_NAME_RE = re.compile(r"c\[(\d+)]")
 
 
@@ -29,14 +32,17 @@
             renderdoc_mesh_csv: Optional path to a CSV file containing mesh vertices as exported from RenderDoc.
             renderdoc_constants_csv: Optional path to a CSV file containing the constant register values as exported
                                      from RenderDoc.
         """
         self._shader = None
         self._shader_trace = None
 
+        self._vertex_inputs: List[Dict] = []
+        self._active_vertex: Optional[Dict] = None
+
         self.inputs_file = inputs_json_file
         self.mesh_inputs_file = renderdoc_mesh_csv
         self.constants_file = renderdoc_constants_csv
         self.source_file = source_file
 
         self.build_shader()
 
@@ -81,41 +87,58 @@
     @property
     def mesh_inputs_file(self) -> str:
         return self._renderdoc_mesh_csv
 
     @mesh_inputs_file.setter
     def mesh_inputs_file(self, val: str):
         self._renderdoc_mesh_csv = val
-        self._mesh = []
+        self._vertex_inputs.clear()
+        self._active_vertex = None
         if val:
             with open(val, newline="", encoding="ascii") as csvfile:
-                reader = csv.DictReader(csvfile)
-                row = next(reader)
-                row = {key.strip(): val.strip() for key, val in row.items()}
-                self._mesh.append(row)
+                for row in csv.DictReader(csvfile):
+                    if not row:
+                        break
+                    row = {key.strip(): val.strip() for key, val in row.items()}
+                    self._vertex_inputs.append(row)
+            if self._vertex_inputs:
+                self._active_vertex = self._vertex_inputs[0]
+
+    @property
+    def vertex_inputs(self):
+        return self._vertex_inputs
 
     @property
     def constants_file(self) -> str:
         return self._renderdoc_constants_csv
 
     @constants_file.setter
     def constants_file(self, val: str):
         self._renderdoc_constants_csv = val
         if val:
             with open(val, newline="", encoding="ascii") as csvfile:
                 self._constants = list(csv.DictReader(csvfile))
         else:
             self._constants = []
 
+    def set_active_vertex_index(self, index: int) -> bool:
+        """Selects a new vertex to use as inputs. Returns True if the shader was rebuilt as a result."""
+        active_vertex = self._vertex_inputs[index]
+        if active_vertex == self._active_vertex:
+            return False
+
+        self._active_vertex = active_vertex
+        self.build_shader()
+        return True
+
     def build_shader(self):
         self._shader = simulator.Shader()
         self._shader.set_initial_state(self._inputs)
 
-        for row in self._mesh:
-            _merge_inputs(row, self._shader)
+        _merge_inputs(self._active_vertex, self._shader)
 
         if self._constants:
             _merge_constants(self._constants, self._shader)
 
         errors = self._shader.set_source(self._source_code)
         if errors:
             error_messsage = [f"Assembly failed due to errors in {self._source_code}:"]
```

### Comparing `nv2a_debug-0.1.0/src/nv2adbg/debugger.py` & `nv2a_debug-0.1.1/src/nv2adbg/debugger.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,79 +3,34 @@
 """Assembles nv2a vertex shader machine code."""
 
 import argparse
 import json
 import logging
 import os
 import sys
-from typing import Optional
 
 from textual.app import App
 from textual.app import ComposeResult
-from textual.containers import Grid
-from textual.screen import ModalScreen
+from textual.reactive import reactive
+from textual.widgets import ContentSwitcher
 from textual.widgets import Footer
 from textual.widgets import Header
-from textual.widgets import Label
 from textual.widgets import TabbedContent
 from textual.widgets import TabPane
 
 from nv2adbg import simulator
 from nv2adbg._editor import _Editor
+from nv2adbg._error_message import _CenteredErrorMessage
 from nv2adbg._file_menu import _FileMenu
 from nv2adbg._program_inputs_viewer import _ProgramInputsViewer
 from nv2adbg._program_outputs_viewer import _ProgramOutputsViewer
+from nv2adbg._program_vertex_viewer import _ProgramVertexViewer
 from nv2adbg._shader_program import _ShaderProgram
 
 
-class _NoTraceErrorScreen(ModalScreen):
-    """Screen used to display message when there is no trace."""
-
-    DEFAULT_CSS = """
-    _NoTraceErrorScreen {
-        align: center middle;
-    }
-
-    #dialog {
-        grid-size: 2;
-        grid-gutter: 1 2;
-        grid-rows: 1fr 3;
-        padding: 0 1;
-        min-width: 60;
-        min-height: 11;
-        border: thick $background 80%;
-        background: $surface;
-    }
-
-    #message {
-        column-span: 2;
-        height: 1fr;
-        width: 1fr;
-        content-align: center middle;
-    }
-    """
-
-    BINDINGS = [
-        ("f1", "app.open_file", "File menu"),
-        ("f10", "app.toggle_dark", "Toggle dark mode"),
-        ("escape,q", "app.quit", "Quit"),
-    ]
-
-    def compose(self) -> ComposeResult:
-        yield Header()
-        yield Grid(
-            Label(
-                "No trace available, load a source file via the File menu.",
-                id="message",
-            ),
-            id="dialog",
-        )
-        yield Footer()
-
-
 class _App(App):
     """Main application."""
 
     TITLE = "nv2a Debugger"
     BINDINGS = [
         ("f1", "open_file", "File menu"),
         ("f10", "app.toggle_dark", "Toggle dark mode"),
@@ -85,46 +40,60 @@
     CSS = """
     /* Workaround for Textualize#2408 */
     TabbedContent ContentSwitcher {
         height: 1fr;
     }
     """
 
+    _active_content = reactive("no-content", init=False)
+
     def __init__(self, program: _ShaderProgram):
         super().__init__()
         self._program = program
         self._editor = _Editor()
         self._program_inputs = _ProgramInputsViewer()
         self._program_outputs = _ProgramOutputsViewer()
+        self._program_vertices = _ProgramVertexViewer()
+        self._editor_content_switcher = ContentSwitcher(initial=self._active_content)
 
     def compose(self) -> ComposeResult:
         """Create child widgets for the app."""
         yield Header()
-        with TabbedContent():
-            with TabPane("Editor"):
-                yield self._editor
-            with TabPane("Inputs"):
-                yield self._program_inputs
-            with TabPane("Outputs"):
-                yield self._program_outputs
+
+        with self._editor_content_switcher:
+            yield _CenteredErrorMessage(
+                "No trace available, load a source file via the File menu.",
+                id="no-content",
+            )
+
+            with TabbedContent(id="content"):
+                with TabPane("Editor"):
+                    yield self._editor
+                with TabPane("Inputs"):
+                    yield self._program_inputs
+                with TabPane("Outputs"):
+                    yield self._program_outputs
+                with TabPane("Vertices"):
+                    yield self._program_vertices
+
         yield Footer()
 
     def action_open_file(self) -> None:
         def on_accept(
             source_file: str,
             inputs_file: str,
             mesh_inputs_file: str,
             constants_file: str,
         ):
             self._program.source_file = source_file
             self._program.inputs_file = inputs_file
             self._program.mesh_inputs_file = mesh_inputs_file
             self._program.constants_file = constants_file
-            self.pop_screen()
             self._load_program()
+            self.pop_screen()
 
         def on_cancel():
             self.pop_screen()
 
         self.push_screen(
             _FileMenu(
                 on_accept,
@@ -138,44 +107,56 @@
 
     def on_mount(self) -> None:
         self._load_program()
 
     def _load_program(self):
         if not self._program.loaded:
             self.sub_title = ""
-            if not isinstance(self.screen, _NoTraceErrorScreen):
-                self.push_screen(_NoTraceErrorScreen(id="notraceerror"))
+            self._active_content = "no-content"
+            self._program_vertices.set_program(None)
             return
-        if isinstance(self.screen, _NoTraceErrorScreen):
-            self.pop_screen()
+
         self.sub_title = self._program.source_file
         self._program.build_shader()
         self.set_shader_trace(self._program.shader_trace)
+        self._active_content = "content"
+        self._program_vertices.set_program(self._program)
 
     def set_shader_trace(self, shader_trace: simulator.Trace):
         self._editor.set_shader_trace(shader_trace)
         self._program_inputs.set_context(shader_trace.input_context)
         self._program_outputs.set_context(
             shader_trace.input_context, shader_trace.output_context
         )
 
-    # def _export(self):
-    #     # TODO: Pop a text input dialog and capture a filename.
-    #     filename = ""
-    #     for index in range(1000):
-    #         filename = f"export{index:04}.vsh"
-    #         if not os.path.exists(filename):
-    #             break
-    #     if os.path.exists(filename):
-    #         raise Exception("Failed to find an unused export filename.")
-    #
-    #     def resolve(input):
-    #         return self._program.shader.initial_state.get(input)
-    #
-    #     self._editor.export(filename, resolve)
+    def _watch__active_content(self, _old_val: str, new_val: str):
+        del _old_val
+        self._editor_content_switcher.current = new_val
+
+    def _on__program_vertex_viewer_active_vertex_changed(
+        self, event: _ProgramVertexViewer.ActiveVertexChanged
+    ):
+        del event
+        self.set_shader_trace(self._program.shader_trace)
+
+
+# def _export(self):
+#     # TODO: Pop a text input dialog and capture a filename.
+#     filename = ""
+#     for index in range(1000):
+#         filename = f"export{index:04}.vsh"
+#         if not os.path.exists(filename):
+#             break
+#     if os.path.exists(filename):
+#         raise Exception("Failed to find an unused export filename.")
+#
+#     def resolve(input):
+#         return self._program.shader.initial_state.get(input)
+#
+#     self._editor.export(filename, resolve)
 
 
 def _emit_input_template():
     ctx = simulator.Context()
     values = ctx.to_dict(True)
     json.dump(values, sys.stdout, indent=2, sort_keys=True)
```

### Comparing `nv2a_debug-0.1.0/src/nv2adbg/py_nv2a_vsh_emu.py` & `nv2a_debug-0.1.1/src/nv2adbg/py_nv2a_vsh_emu.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/src/nv2adbg/simulator.py` & `nv2a_debug-0.1.1/src/nv2adbg/simulator.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/tests/test__code_panel_build_ancestor_root_segments.py` & `nv2a_debug-0.1.1/tests/test__code_panel_build_ancestor_root_segments.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/tests/test__code_panel_build_contributing_source_segments.py` & `nv2a_debug-0.1.1/tests/test__code_panel_build_contributing_source_segments.py`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/.github/workflows/build.yml` & `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/CMakeLists.txt` & `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/LICENSE` & `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/LICENSE`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/githooks/pre-commit` & `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/githooks/pre-commit`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.c` & `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.c`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.h` & `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_cpu.h`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.c` & `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.c`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.h` & `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_disassembler.h`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.c` & `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.c`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.h` & `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator.h`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.c` & `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.c`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.h` & `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/src/nv2a_vsh_emulator_execution_state.h`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/disassembler/test_basic.cpp` & `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/disassembler/test_basic.cpp`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/emulator/test_basic.cpp` & `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/emulator/test_basic.cpp`

 * *Files identical despite different names*

### Comparing `nv2a_debug-0.1.0/thirdparty/nv2a_vsh_cpu/test/operations/test_basic.cpp` & `nv2a_debug-0.1.1/thirdparty/nv2a_vsh_cpu/test/operations/test_basic.cpp`

 * *Files identical despite different names*

