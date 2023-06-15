# Comparing `tmp/sos-0.9.9.8.tar.gz` & `tmp/sos-0.9.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sos-0.9.9.8.tar", last modified: Wed Oct 18 14:11:46 2017, max compression
+gzip compressed data, was "dist/sos-0.9.9.9.tar", last modified: Sat Oct 21 00:34:10 2017, max compression
```

## Comparing `sos-0.9.9.8.tar` & `sos-0.9.9.9.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-18 14:11:46.000000 sos-0.9.9.8/
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    35141 2017-10-06 01:22:25.000000 sos-0.9.9.8/LICENSE
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      337 2017-10-06 01:22:25.000000 sos-0.9.9.8/MANIFEST.in
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-18 14:11:46.000000 sos-0.9.9.8/misc/
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-18 14:11:46.000000 sos-0.9.9.8/misc/celery/
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     3292 2017-10-06 01:22:25.000000 sos-0.9.9.8/misc/celery/sos_task.py
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-18 14:11:46.000000 sos-0.9.9.8/misc/ipython/
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     6768 2017-10-06 01:22:25.000000 sos-0.9.9.8/misc/ipython/ipython_magic.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      596 2017-10-06 01:22:25.000000 sos-0.9.9.8/misc/ipython/sos_ipython_profile.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     4107 2017-10-06 01:22:25.000000 sos-0.9.9.8/misc/ipython/test_ipython.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1932 2017-10-06 01:22:25.000000 sos-0.9.9.8/misc/logo-64x64.png
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      263 2017-10-06 01:22:25.000000 sos-0.9.9.8/misc/sos-detect.vim
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     3244 2017-10-06 01:22:25.000000 sos-0.9.9.8/misc/sos.vim
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-18 14:11:46.000000 sos-0.9.9.8/misc/spyder/
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     8615 2017-10-06 01:22:25.000000 sos-0.9.9.8/misc/spyder/patch_spyder.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     5409 2017-10-06 01:22:25.000000 sos-0.9.9.8/misc/spyder/spyder_kernel.py
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-18 14:11:46.000000 sos-0.9.9.8/misc/vim-ipython/
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     9305 2017-10-06 01:22:25.000000 sos-0.9.9.8/misc/vim-ipython/ipy.vim
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    28254 2017-10-06 01:22:25.000000 sos-0.9.9.8/misc/vim-ipython/vim_ipython.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     2831 2017-10-18 14:11:46.000000 sos-0.9.9.8/PKG-INFO
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1407 2017-10-06 04:13:44.000000 sos-0.9.9.8/README.md
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)       38 2017-10-18 14:11:46.000000 sos-0.9.9.8/setup.cfg
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     6780 2017-10-06 01:22:25.000000 sos-0.9.9.8/setup.py
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-18 14:11:46.000000 sos-0.9.9.8/src/
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-18 14:11:46.000000 sos-0.9.9.8/src/sos/
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      972 2017-10-06 01:22:25.000000 sos-0.9.9.8/src/sos/__init__.py
--rwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)   106840 2017-10-12 20:12:53.000000 sos-0.9.9.8/src/sos/__main__.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1716 2017-10-18 14:11:29.000000 sos-0.9.9.8/src/sos/_version.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    43442 2017-10-06 01:22:25.000000 sos-0.9.9.8/src/sos/actions.py
--rwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    27292 2017-10-06 01:22:25.000000 sos-0.9.9.8/src/sos/converter.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    14672 2017-10-06 01:22:25.000000 sos-0.9.9.8/src/sos/dag.py
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-18 14:11:46.000000 sos-0.9.9.8/src/sos/docker/
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-06 01:22:25.000000 sos-0.9.9.8/src/sos/docker/__init__.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1369 2017-10-06 01:22:25.000000 sos-0.9.9.8/src/sos/docker/actions.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    15867 2017-10-06 01:22:25.000000 sos-0.9.9.8/src/sos/docker/client.py
--rwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    42825 2017-10-07 17:45:20.000000 sos-0.9.9.8/src/sos/hosts.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     7729 2017-10-06 01:22:25.000000 sos-0.9.9.8/src/sos/monitor.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     6170 2017-10-06 01:22:25.000000 sos-0.9.9.8/src/sos/pattern.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     2125 2017-10-06 01:22:25.000000 sos-0.9.9.8/src/sos/runtime.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    22776 2017-10-18 02:33:22.000000 sos-0.9.9.8/src/sos/sos_eval.py
--rwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    57079 2017-10-18 12:33:06.000000 sos-0.9.9.8/src/sos/sos_executor.py
--rwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    58734 2017-10-06 01:22:25.000000 sos-0.9.9.8/src/sos/sos_script.py
--rwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    70084 2017-10-18 13:26:28.000000 sos-0.9.9.8/src/sos/sos_step.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    17307 2017-10-12 20:12:53.000000 sos-0.9.9.8/src/sos/sos_syntax.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    68290 2017-10-18 02:33:22.000000 sos-0.9.9.8/src/sos/sos_task.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    32504 2017-10-06 01:22:25.000000 sos-0.9.9.8/src/sos/target.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    45446 2017-10-06 01:22:25.000000 sos-0.9.9.8/src/sos/utils.py
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-18 14:11:46.000000 sos-0.9.9.8/src/sos.egg-info/
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        1 2017-10-18 14:11:45.000000 sos-0.9.9.8/src/sos.egg-info/dependency_links.txt
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1118 2017-10-18 14:11:45.000000 sos-0.9.9.8/src/sos.egg-info/entry_points.txt
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     2831 2017-10-18 14:11:45.000000 sos-0.9.9.8/src/sos.egg-info/PKG-INFO
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      162 2017-10-18 14:11:45.000000 sos-0.9.9.8/src/sos.egg-info/requires.txt
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1247 2017-10-18 14:11:46.000000 sos-0.9.9.8/src/sos.egg-info/SOURCES.txt
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        4 2017-10-18 14:11:45.000000 sos-0.9.9.8/src/sos.egg-info/top_level.txt
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-18 14:11:46.000000 sos-0.9.9.8/test/
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    16094 2017-10-06 03:25:12.000000 sos-0.9.9.8/test/test_actions.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     2872 2017-10-06 01:22:25.000000 sos-0.9.9.8/test/test_convert.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    23296 2017-10-06 01:22:25.000000 sos-0.9.9.8/test/test_dag.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     6066 2017-10-06 01:22:25.000000 sos-0.9.9.8/test/test_docker_actions.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    35139 2017-10-06 04:10:05.000000 sos-0.9.9.8/test/test_execute.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    17819 2017-10-06 01:22:25.000000 sos-0.9.9.8/test/test_nested.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     5133 2017-10-06 01:22:25.000000 sos-0.9.9.8/test/test_pack.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    30250 2017-10-06 01:22:25.000000 sos-0.9.9.8/test/test_parser.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-06 01:22:25.000000 sos-0.9.9.8/test/test_queue.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     3641 2017-10-06 01:22:25.000000 sos-0.9.9.8/test/test_remote.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     7464 2017-10-06 01:22:25.000000 sos-0.9.9.8/test/test_remove.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    16516 2017-10-07 03:47:35.000000 sos-0.9.9.8/test/test_signature.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     8930 2017-10-06 01:22:25.000000 sos-0.9.9.8/test/test_target.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    21849 2017-10-18 13:50:52.000000 sos-0.9.9.8/test/test_task.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    18992 2017-10-06 01:22:25.000000 sos-0.9.9.8/test/test_utils.py
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-21 00:34:10.000000 sos-0.9.9.9/
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    35141 2017-10-06 20:03:29.000000 sos-0.9.9.9/LICENSE
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      337 2017-10-06 20:03:29.000000 sos-0.9.9.9/MANIFEST.in
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-21 00:34:09.000000 sos-0.9.9.9/misc/
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-21 00:34:09.000000 sos-0.9.9.9/misc/celery/
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     3292 2017-10-06 20:03:29.000000 sos-0.9.9.9/misc/celery/sos_task.py
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-21 00:34:09.000000 sos-0.9.9.9/misc/ipython/
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     6768 2017-10-06 20:03:29.000000 sos-0.9.9.9/misc/ipython/ipython_magic.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      596 2017-10-06 20:03:29.000000 sos-0.9.9.9/misc/ipython/sos_ipython_profile.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     4107 2017-10-06 20:03:29.000000 sos-0.9.9.9/misc/ipython/test_ipython.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1932 2017-10-06 20:03:29.000000 sos-0.9.9.9/misc/logo-64x64.png
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      263 2017-10-06 20:03:29.000000 sos-0.9.9.9/misc/sos-detect.vim
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     3244 2017-10-06 20:03:29.000000 sos-0.9.9.9/misc/sos.vim
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-21 00:34:09.000000 sos-0.9.9.9/misc/spyder/
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     8615 2017-10-06 20:03:29.000000 sos-0.9.9.9/misc/spyder/patch_spyder.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     5409 2017-10-06 20:03:29.000000 sos-0.9.9.9/misc/spyder/spyder_kernel.py
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-21 00:34:09.000000 sos-0.9.9.9/misc/vim-ipython/
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     9305 2017-10-06 20:03:29.000000 sos-0.9.9.9/misc/vim-ipython/ipy.vim
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    28254 2017-10-06 20:03:29.000000 sos-0.9.9.9/misc/vim-ipython/vim_ipython.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     2831 2017-10-21 00:34:10.000000 sos-0.9.9.9/PKG-INFO
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1407 2017-10-06 20:03:29.000000 sos-0.9.9.9/README.md
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)       38 2017-10-21 00:34:10.000000 sos-0.9.9.9/setup.cfg
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     6780 2017-10-06 20:03:29.000000 sos-0.9.9.9/setup.py
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-21 00:34:09.000000 sos-0.9.9.9/src/
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-21 00:34:09.000000 sos-0.9.9.9/src/sos/
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      972 2017-10-06 20:03:29.000000 sos-0.9.9.9/src/sos/__init__.py
+-rwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)   106840 2017-10-10 16:19:00.000000 sos-0.9.9.9/src/sos/__main__.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1716 2017-10-21 00:33:41.000000 sos-0.9.9.9/src/sos/_version.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    43442 2017-10-06 20:03:29.000000 sos-0.9.9.9/src/sos/actions.py
+-rwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    27292 2017-10-06 20:03:29.000000 sos-0.9.9.9/src/sos/converter.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    14672 2017-10-06 20:03:29.000000 sos-0.9.9.9/src/sos/dag.py
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-21 00:34:09.000000 sos-0.9.9.9/src/sos/docker/
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-06 20:03:29.000000 sos-0.9.9.9/src/sos/docker/__init__.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1369 2017-10-06 20:03:29.000000 sos-0.9.9.9/src/sos/docker/actions.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    15867 2017-10-06 20:03:29.000000 sos-0.9.9.9/src/sos/docker/client.py
+-rwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    42825 2017-10-21 00:02:50.000000 sos-0.9.9.9/src/sos/hosts.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     7729 2017-10-06 20:03:29.000000 sos-0.9.9.9/src/sos/monitor.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     6170 2017-10-06 20:03:29.000000 sos-0.9.9.9/src/sos/pattern.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     2125 2017-10-06 20:03:29.000000 sos-0.9.9.9/src/sos/runtime.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    22776 2017-10-17 01:15:17.000000 sos-0.9.9.9/src/sos/sos_eval.py
+-rwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    57270 2017-10-21 00:33:23.000000 sos-0.9.9.9/src/sos/sos_executor.py
+-rwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    58734 2017-10-06 20:03:29.000000 sos-0.9.9.9/src/sos/sos_script.py
+-rwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    70084 2017-10-18 16:09:07.000000 sos-0.9.9.9/src/sos/sos_step.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    17307 2017-10-10 15:23:40.000000 sos-0.9.9.9/src/sos/sos_syntax.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    68290 2017-10-17 02:31:15.000000 sos-0.9.9.9/src/sos/sos_task.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    32504 2017-10-06 20:03:29.000000 sos-0.9.9.9/src/sos/target.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    45446 2017-10-06 20:03:29.000000 sos-0.9.9.9/src/sos/utils.py
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-21 00:34:09.000000 sos-0.9.9.9/src/sos.egg-info/
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        1 2017-10-21 00:34:09.000000 sos-0.9.9.9/src/sos.egg-info/dependency_links.txt
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1118 2017-10-21 00:34:09.000000 sos-0.9.9.9/src/sos.egg-info/entry_points.txt
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     2831 2017-10-21 00:34:09.000000 sos-0.9.9.9/src/sos.egg-info/PKG-INFO
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      162 2017-10-21 00:34:09.000000 sos-0.9.9.9/src/sos.egg-info/requires.txt
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1247 2017-10-21 00:34:09.000000 sos-0.9.9.9/src/sos.egg-info/SOURCES.txt
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        4 2017-10-21 00:34:09.000000 sos-0.9.9.9/src/sos.egg-info/top_level.txt
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-21 00:34:10.000000 sos-0.9.9.9/test/
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    16094 2017-10-06 20:03:29.000000 sos-0.9.9.9/test/test_actions.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     2872 2017-10-06 20:03:29.000000 sos-0.9.9.9/test/test_convert.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    23296 2017-10-06 20:03:29.000000 sos-0.9.9.9/test/test_dag.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     6066 2017-10-06 20:03:29.000000 sos-0.9.9.9/test/test_docker_actions.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    35139 2017-10-06 20:03:29.000000 sos-0.9.9.9/test/test_execute.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    17819 2017-10-06 20:03:29.000000 sos-0.9.9.9/test/test_nested.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     5133 2017-10-06 20:03:29.000000 sos-0.9.9.9/test/test_pack.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    30250 2017-10-06 20:03:29.000000 sos-0.9.9.9/test/test_parser.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-06 20:03:29.000000 sos-0.9.9.9/test/test_queue.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     3641 2017-10-06 20:03:29.000000 sos-0.9.9.9/test/test_remote.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     7464 2017-10-06 20:03:29.000000 sos-0.9.9.9/test/test_remove.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    16516 2017-10-09 14:51:24.000000 sos-0.9.9.9/test/test_signature.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     8930 2017-10-06 20:03:29.000000 sos-0.9.9.9/test/test_target.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    21647 2017-10-18 20:45:39.000000 sos-0.9.9.9/test/test_task.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    18992 2017-10-06 20:03:29.000000 sos-0.9.9.9/test/test_utils.py
```

### Comparing `sos-0.9.9.8/LICENSE` & `sos-0.9.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/misc/celery/sos_task.py` & `sos-0.9.9.9/misc/celery/sos_task.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/misc/ipython/ipython_magic.py` & `sos-0.9.9.9/misc/ipython/ipython_magic.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/misc/ipython/sos_ipython_profile.py` & `sos-0.9.9.9/misc/ipython/sos_ipython_profile.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/misc/ipython/test_ipython.py` & `sos-0.9.9.9/misc/ipython/test_ipython.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/misc/logo-64x64.png` & `sos-0.9.9.9/misc/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/misc/sos.vim` & `sos-0.9.9.9/misc/sos.vim`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/misc/spyder/patch_spyder.py` & `sos-0.9.9.9/misc/spyder/patch_spyder.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/misc/spyder/spyder_kernel.py` & `sos-0.9.9.9/misc/spyder/spyder_kernel.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/misc/vim-ipython/ipy.vim` & `sos-0.9.9.9/misc/vim-ipython/ipy.vim`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/misc/vim-ipython/vim_ipython.py` & `sos-0.9.9.9/misc/vim-ipython/vim_ipython.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/PKG-INFO` & `sos-0.9.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sos
-Version: 0.9.9.8
+Version: 0.9.9.9
 Summary: Script of Scripts (SoS): an interactive, cross-platform, and cross-language workflow system for reproducible data analysis
 Home-page: https://github.com/vatlab/SoS
 Author: Bo Peng
 Author-email: bpeng@mdanderson.org
 License: GPL3
 Description-Content-Type: UNKNOWN
 Description: Computationally intensive disciplines such as computational biology often
```

### Comparing `sos-0.9.9.8/README.md` & `sos-0.9.9.9/README.md`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/setup.py` & `sos-0.9.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/src/sos/__init__.py` & `sos-0.9.9.9/src/sos/__init__.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/src/sos/__main__.py` & `sos-0.9.9.9/src/sos/__main__.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/src/sos/_version.py` & `sos-0.9.9.9/src/sos/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     raise SystemError('SOS requires Python 3.4 or higher. Please upgrade your Python {}.{}.{}.'
         .format(_py_ver.major, _py_ver.minor, _py_ver.micro))
 
 
 # version of the SoS language
 __sos_version__ = '1.0'
 # version of the sos command
-__version__ = '0.9.9.8'
+__version__ = '0.9.9.9'
 __py_version__ = '{}.{}.{}'.format(_py_ver.major, _py_ver.minor, _py_ver.micro)
 
 #
 SOS_FULL_VERSION='{} for Python {}.{}.{}'.format(__version__, _py_ver.major, _py_ver.minor, _py_ver.micro)
 SOS_COPYRIGHT = '''SoS {} : Copyright (c) 2016 Bo Peng'''.format(__version__)
 SOS_CONTACT = '''Please visit http://github.com/vatlab/SOS for more information.'''
```

### Comparing `sos-0.9.9.8/src/sos/actions.py` & `sos-0.9.9.9/src/sos/actions.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/src/sos/converter.py` & `sos-0.9.9.9/src/sos/converter.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/src/sos/dag.py` & `sos-0.9.9.9/src/sos/dag.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/src/sos/docker/actions.py` & `sos-0.9.9.9/src/sos/docker/actions.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/src/sos/docker/client.py` & `sos-0.9.9.9/src/sos/docker/client.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/src/sos/hosts.py` & `sos-0.9.9.9/src/sos/hosts.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/src/sos/monitor.py` & `sos-0.9.9.9/src/sos/monitor.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/src/sos/pattern.py` & `sos-0.9.9.9/src/sos/pattern.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/src/sos/runtime.py` & `sos-0.9.9.9/src/sos/runtime.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/src/sos/sos_eval.py` & `sos-0.9.9.9/src/sos/sos_eval.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/src/sos/sos_executor.py` & `sos-0.9.9.9/src/sos/sos_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -491,18 +491,21 @@
                 # with identical names.
                 dag.add_step(section.uuid, '{} {}'.format(section.step_name(),
                     short_repr(env.sos_dict['__default_output__'])), None, res['step_input'],
                     res['step_depends'], res['step_output'], context=context)
                 added_node += 1
                 resolved += 1
 
-            # for existing targets... we should check if still need to be regenerated
+            # for existing targets... we should check if it actually exists. If
+            # not it would still need to be regenerated
             for target in existing_targets:
                 if target not in dag.dangling(targets)[1]:
                     continue
+                if FileTarget(target).exists('target') if isinstance(target, str) else target.exists('target'):
+                    continue
                 mo = [(x, self.match(target, x)) for x in self.workflow.auxiliary_sections]
                 mo = [x for x in mo if x[1] is not False]
                 if not mo:
                     # this is ok, this is just an existing target, no one is designed to
                     # generate it.
                     continue
                 if len(mo) > 1:
```

### Comparing `sos-0.9.9.8/src/sos/sos_script.py` & `sos-0.9.9.9/src/sos/sos_script.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/src/sos/sos_step.py` & `sos-0.9.9.9/src/sos/sos_step.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/src/sos/sos_syntax.py` & `sos-0.9.9.9/src/sos/sos_syntax.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/src/sos/sos_task.py` & `sos-0.9.9.9/src/sos/sos_task.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/src/sos/target.py` & `sos-0.9.9.9/src/sos/target.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/src/sos/utils.py` & `sos-0.9.9.9/src/sos/utils.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/src/sos.egg-info/entry_points.txt` & `sos-0.9.9.9/src/sos.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/src/sos.egg-info/PKG-INFO` & `sos-0.9.9.9/src/sos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sos
-Version: 0.9.9.8
+Version: 0.9.9.9
 Summary: Script of Scripts (SoS): an interactive, cross-platform, and cross-language workflow system for reproducible data analysis
 Home-page: https://github.com/vatlab/SoS
 Author: Bo Peng
 Author-email: bpeng@mdanderson.org
 License: GPL3
 Description-Content-Type: UNKNOWN
 Description: Computationally intensive disciplines such as computational biology often
```

### Comparing `sos-0.9.9.8/src/sos.egg-info/SOURCES.txt` & `sos-0.9.9.9/src/sos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/test/test_actions.py` & `sos-0.9.9.9/test/test_actions.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/test/test_convert.py` & `sos-0.9.9.9/test/test_convert.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/test/test_dag.py` & `sos-0.9.9.9/test/test_dag.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/test/test_docker_actions.py` & `sos-0.9.9.9/test/test_docker_actions.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/test/test_execute.py` & `sos-0.9.9.9/test/test_execute.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/test/test_nested.py` & `sos-0.9.9.9/test/test_nested.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/test/test_pack.py` & `sos-0.9.9.9/test/test_pack.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/test/test_parser.py` & `sos-0.9.9.9/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/test/test_remote.py` & `sos-0.9.9.9/test/test_remote.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/test/test_remove.py` & `sos-0.9.9.9/test/test_remove.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/test/test_signature.py` & `sos-0.9.9.9/test/test_signature.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/test/test_target.py` & `sos-0.9.9.9/test/test_target.py`

 * *Files identical despite different names*

### Comparing `sos-0.9.9.8/test/test_task.py` & `sos-0.9.9.9/test/test_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,14 @@
     echo "a = ${a}, b = ${b}"
 ''')
         env.config['wait_for_task'] = True
         env.config['max_running_jobs'] = 2
         wf = script.workflow()
         Base_Executor(wf).run()
 
-    @unittest.skipIf('TRAVIS_OS_NAME' in os.environ, 'Test fails on travis for unknown reason #831')
     def testKillAndPurge(self):
         '''Test no wait'''
         subprocess.call(['sos', 'purge'])
         script = SoS_Script(r'''
 [10]
 input: for_each=[{'a': range(2)}]
 
@@ -346,15 +345,14 @@
         subprocess.call(['sos', 'purge', '--status', 'aborted'])
         self.assertFalse('killed' in subprocess.check_output(['sos', 'status', '-v', '3']).decode())
         # test purge by age
         subprocess.call(['sos', 'purge', '--age=-20s'])
         # purge by all is not tested because it is dangerous
 
 
-    @unittest.skipIf('TRAVIS_OS_NAME' in os.environ, 'Test fails on travis for unknown reason #831')
     def testNoWait(self):
         '''Test no wait'''
         script = SoS_Script(r'''
 [10]
 input: for_each=[{'a': range(3)}]
 
 task: concurrent=True
```

### Comparing `sos-0.9.9.8/test/test_utils.py` & `sos-0.9.9.9/test/test_utils.py`

 * *Files identical despite different names*

