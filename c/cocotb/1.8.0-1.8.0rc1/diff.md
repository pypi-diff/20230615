# Comparing `tmp/cocotb-1.8.0.tar.gz` & `tmp/cocotb-1.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cocotb-1.8.0.tar", last modified: Thu Jun 15 11:03:32 2023, max compression
+gzip compressed data, was "cocotb-1.8.0rc1.tar", last modified: Mon Jun 12 21:37:16 2023, max compression
```

## Comparing `cocotb-1.8.0.tar` & `cocotb-1.8.0rc1.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.539834 cocotb-1.8.0/
--rw-r--r--   0 runner     (501) staff       (20)     1542 2023-06-15 10:42:42.000000 cocotb-1.8.0/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      131 2023-06-15 10:42:42.000000 cocotb-1.8.0/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     6714 2023-06-15 11:03:32.540011 cocotb-1.8.0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     5581 2023-06-15 10:42:42.000000 cocotb-1.8.0/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.498649 cocotb-1.8.0/cocotb/
--rw-r--r--   0 runner     (501) staff       (20)     3366 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/ANSI.py
--rw-r--r--   0 runner     (501) staff       (20)    11296 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1153 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/_deprecation.py
--rw-r--r--   0 runner     (501) staff       (20)     2691 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/_py_compat.py
--rw-r--r--   0 runner     (501) staff       (20)     3544 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/_sim_versions.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.503138 cocotb-1.8.0/cocotb/_vendor/
--rw-r--r--   0 runner     (501) staff       (20)     1166 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/_vendor/README.md
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/_vendor/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    12839 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/_vendor/distutils_version.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.504865 cocotb-1.8.0/cocotb/_vendor/fli/
--rw-r--r--   0 runner     (501) staff       (20)    25349 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/_vendor/fli/acc_user.h
--rw-r--r--   0 runner     (501) staff       (20)    11914 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/_vendor/fli/acc_vhdl.h
--rw-r--r--   0 runner     (501) staff       (20)    32939 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/_vendor/fli/mti.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.507627 cocotb-1.8.0/cocotb/_vendor/tcl/
--rw-r--r--   0 runner     (501) staff       (20)     2255 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/_vendor/tcl/license.terms
--rw-r--r--   0 runner     (501) staff       (20)    94743 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/_vendor/tcl/tcl.h
--rw-r--r--   0 runner     (501) staff       (20)   169681 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/_vendor/tcl/tclDecls.h
--rw-r--r--   0 runner     (501) staff       (20)     3279 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/_vendor/tcl/tclPlatDecls.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.508210 cocotb-1.8.0/cocotb/_vendor/vhpi/
--rw-r--r--   0 runner     (501) staff       (20)    42107 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/_vendor/vhpi/vhpi_user.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.509394 cocotb-1.8.0/cocotb/_vendor/vpi/
--rw-r--r--   0 runner     (501) staff       (20)    25694 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/_vendor/vpi/sv_vpi_user.h
--rw-r--r--   0 runner     (501) staff       (20)    44349 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/_vendor/vpi/vpi_user.h
--rw-r--r--   0 runner     (501) staff       (20)      295 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/_version.py
--rwxr-xr-x   0 runner     (501) staff       (20)    26172 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/binary.py
--rw-r--r--   0 runner     (501) staff       (20)     6560 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/clock.py
--rwxr-xr-x   0 runner     (501) staff       (20)     9847 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/config.py
--rw-r--r--   0 runner     (501) staff       (20)    11476 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/decorators.py
--rwxr-xr-x   0 runner     (501) staff       (20)    41612 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/handle.py
--rw-r--r--   0 runner     (501) staff       (20)     3136 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/ipython_support.py
--rw-r--r--   0 runner     (501) staff       (20)    10443 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/log.py
--rw-r--r--   0 runner     (501) staff       (20)     1853 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/memdebug.py
--rw-r--r--   0 runner     (501) staff       (20)     1299 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/outcomes.py
--rw-r--r--   0 runner     (501) staff       (20)     5159 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/queue.py
--rw-r--r--   0 runner     (501) staff       (20)    32968 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/regression.py
--rw-r--r--   0 runner     (501) staff       (20)     6696 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/result.py
--rw-r--r--   0 runner     (501) staff       (20)    35588 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/runner.py
--rwxr-xr-x   0 runner     (501) staff       (20)    40942 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/scheduler.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.478598 cocotb-1.8.0/cocotb/share/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.512781 cocotb-1.8.0/cocotb/share/def/
--rw-r--r--   0 runner     (501) staff       (20)       44 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/def/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)      376 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/def/README.md
--rw-r--r--   0 runner     (501) staff       (20)      930 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/def/aldec.def
--rw-r--r--   0 runner     (501) staff       (20)      662 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/def/ghdl.def
--rw-r--r--   0 runner     (501) staff       (20)      655 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/def/icarus.def
--rw-r--r--   0 runner     (501) staff       (20)     2252 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/def/modelsim.def
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.517265 cocotb-1.8.0/cocotb/share/include/
--rw-r--r--   0 runner     (501) staff       (20)     3998 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/include/cocotb_utils.h
--rw-r--r--   0 runner     (501) staff       (20)     2453 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/include/embed.h
--rw-r--r--   0 runner     (501) staff       (20)      657 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/include/exports.h
--rw-r--r--   0 runner     (501) staff       (20)     9999 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/include/gpi.h
--rw-r--r--   0 runner     (501) staff       (20)    10341 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/include/gpi_logging.h
--rw-r--r--   0 runner     (501) staff       (20)      642 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/include/py_gpi_logging.h
--rw-r--r--   0 runner     (501) staff       (20)      628 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/include/vhpi_user_ext.h
--rw-r--r--   0 runner     (501) staff       (20)     2456 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/include/vpi_user_ext.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.478377 cocotb-1.8.0/cocotb/share/lib/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.518270 cocotb-1.8.0/cocotb/share/lib/embed/
--rw-r--r--   0 runner     (501) staff       (20)     4377 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/lib/embed/embed.cpp
--rw-r--r--   0 runner     (501) staff       (20)    10476 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/lib/embed/gpi_embed.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.520555 cocotb-1.8.0/cocotb/share/lib/fli/
--rw-r--r--   0 runner     (501) staff       (20)     7754 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/lib/fli/FliCbHdl.cpp
--rw-r--r--   0 runner     (501) staff       (20)    40118 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/lib/fli/FliImpl.cpp
--rw-r--r--   0 runner     (501) staff       (20)    16198 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/lib/fli/FliImpl.h
--rw-r--r--   0 runner     (501) staff       (20)    26850 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/lib/fli/FliObjHdl.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.522151 cocotb-1.8.0/cocotb/share/lib/gpi/
--rw-r--r--   0 runner     (501) staff       (20)     4362 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/lib/gpi/GpiCbHdl.cpp
--rw-r--r--   0 runner     (501) staff       (20)    19643 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/lib/gpi/GpiCommon.cpp
--rw-r--r--   0 runner     (501) staff       (20)    11255 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/lib/gpi/gpi_priv.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.522673 cocotb-1.8.0/cocotb/share/lib/gpi_log/
--rw-r--r--   0 runner     (501) staff       (20)     7056 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/lib/gpi_log/gpi_logging.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.523250 cocotb-1.8.0/cocotb/share/lib/py_gpi_log/
--rw-r--r--   0 runner     (501) staff       (20)     7022 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/lib/py_gpi_log/py_gpi_logging.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.523761 cocotb-1.8.0/cocotb/share/lib/simulator/
--rw-r--r--   0 runner     (501) staff       (20)    41165 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/lib/simulator/simulatormodule.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.524390 cocotb-1.8.0/cocotb/share/lib/utils/
--rw-r--r--   0 runner     (501) staff       (20)     3896 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/lib/utils/cocotb_utils.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.524968 cocotb-1.8.0/cocotb/share/lib/verilator/
--rw-r--r--   0 runner     (501) staff       (20)     4407 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/lib/verilator/verilator.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.526749 cocotb-1.8.0/cocotb/share/lib/vhpi/
--rw-r--r--   0 runner     (501) staff       (20)    38860 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/lib/vhpi/VhpiCbHdl.cpp
--rw-r--r--   0 runner     (501) staff       (20)    36640 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/lib/vhpi/VhpiImpl.cpp
--rw-r--r--   0 runner     (501) staff       (20)    10762 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/lib/vhpi/VhpiImpl.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.528421 cocotb-1.8.0/cocotb/share/lib/vpi/
--rw-r--r--   0 runner     (501) staff       (20)    27347 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/lib/vpi/VpiCbHdl.cpp
--rw-r--r--   0 runner     (501) staff       (20)    22748 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/lib/vpi/VpiImpl.cpp
--rw-r--r--   0 runner     (501) staff       (20)    10441 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/lib/vpi/VpiImpl.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.529988 cocotb-1.8.0/cocotb/share/makefiles/
--rw-r--r--   0 runner     (501) staff       (20)      416 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/makefiles/Makefile.deprecations
--rw-r--r--   0 runner     (501) staff       (20)     7030 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/makefiles/Makefile.inc
--rw-r--r--   0 runner     (501) staff       (20)     5299 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/makefiles/Makefile.sim
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.536128 cocotb-1.8.0/cocotb/share/makefiles/simulators/
--rw-r--r--   0 runner     (501) staff       (20)     2656 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.activehdl
--rw-r--r--   0 runner     (501) staff       (20)     3901 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.cvc
--rw-r--r--   0 runner     (501) staff       (20)     3542 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.ghdl
--rw-r--r--   0 runner     (501) staff       (20)     4374 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.icarus
--rw-r--r--   0 runner     (501) staff       (20)     4965 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.ius
--rw-r--r--   0 runner     (501) staff       (20)     1906 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.modelsim
--rw-r--r--   0 runner     (501) staff       (20)     6427 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.questa
--rw-r--r--   0 runner     (501) staff       (20)     5913 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.riviera
--rw-r--r--   0 runner     (501) staff       (20)     3690 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.vcs
--rw-r--r--   0 runner     (501) staff       (20)     2407 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.verilator
--rw-r--r--   0 runner     (501) staff       (20)     5414 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.xcelium
--rw-r--r--   0 runner     (501) staff       (20)    11035 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/task.py
--rw-r--r--   0 runner     (501) staff       (20)    32228 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/triggers.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.538554 cocotb-1.8.0/cocotb/types/
--rw-r--r--   0 runner     (501) staff       (20)     1803 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/types/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    10899 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/types/array.py
--rw-r--r--   0 runner     (501) staff       (20)     8499 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/types/logic.py
--rw-r--r--   0 runner     (501) staff       (20)     9957 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/types/logic_array.py
--rw-r--r--   0 runner     (501) staff       (20)     6230 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/types/range.py
--rw-r--r--   0 runner     (501) staff       (20)    23064 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     5988 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/wavedrom.py
--rw-r--r--   0 runner     (501) staff       (20)     3552 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb/xunit_reporter.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.501703 cocotb-1.8.0/cocotb.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     6714 2023-06-15 11:03:32.000000 cocotb-1.8.0/cocotb.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3103 2023-06-15 11:03:32.000000 cocotb-1.8.0/cocotb.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-06-15 11:03:32.000000 cocotb-1.8.0/cocotb.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       53 2023-06-15 11:03:32.000000 cocotb-1.8.0/cocotb.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)       33 2023-06-15 11:03:32.000000 cocotb-1.8.0/cocotb.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)      516 2023-06-15 11:03:32.000000 cocotb-1.8.0/cocotb.egg-info/top_level.txt
--rwxr-xr-x   0 runner     (501) staff       (20)    27213 2023-06-15 10:42:42.000000 cocotb-1.8.0/cocotb_build_libs.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-15 11:03:32.539368 cocotb-1.8.0/pygpi/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-15 10:42:42.000000 cocotb-1.8.0/pygpi/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      946 2023-06-15 10:42:42.000000 cocotb-1.8.0/pygpi/entry.py
--rw-r--r--   0 runner     (501) staff       (20)     2089 2023-06-15 10:42:42.000000 cocotb-1.8.0/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)      808 2023-06-15 11:03:32.540835 cocotb-1.8.0/setup.cfg
--rwxr-xr-x   0 runner     (501) staff       (20)     5543 2023-06-15 10:42:42.000000 cocotb-1.8.0/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.508607 cocotb-1.8.0rc1/
+-rw-r--r--   0 runner     (501) staff       (20)     1542 2023-06-12 21:15:17.000000 cocotb-1.8.0rc1/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      131 2023-06-12 21:15:17.000000 cocotb-1.8.0rc1/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     6717 2023-06-12 21:37:16.508825 cocotb-1.8.0rc1/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     5581 2023-06-12 21:15:17.000000 cocotb-1.8.0rc1/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.459431 cocotb-1.8.0rc1/cocotb/
+-rw-r--r--   0 runner     (501) staff       (20)     3366 2023-06-12 21:15:17.000000 cocotb-1.8.0rc1/cocotb/ANSI.py
+-rw-r--r--   0 runner     (501) staff       (20)    11296 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1153 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_deprecation.py
+-rw-r--r--   0 runner     (501) staff       (20)     2691 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_py_compat.py
+-rw-r--r--   0 runner     (501) staff       (20)     3544 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_sim_versions.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.464655 cocotb-1.8.0rc1/cocotb/_vendor/
+-rw-r--r--   0 runner     (501) staff       (20)     1166 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/README.md
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    12839 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/distutils_version.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.466487 cocotb-1.8.0rc1/cocotb/_vendor/fli/
+-rw-r--r--   0 runner     (501) staff       (20)    25349 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/fli/acc_user.h
+-rw-r--r--   0 runner     (501) staff       (20)    11914 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/fli/acc_vhdl.h
+-rw-r--r--   0 runner     (501) staff       (20)    32939 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/fli/mti.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.469758 cocotb-1.8.0rc1/cocotb/_vendor/tcl/
+-rw-r--r--   0 runner     (501) staff       (20)     2255 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/tcl/license.terms
+-rw-r--r--   0 runner     (501) staff       (20)    94743 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/tcl/tcl.h
+-rw-r--r--   0 runner     (501) staff       (20)   169681 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/tcl/tclDecls.h
+-rw-r--r--   0 runner     (501) staff       (20)     3279 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/tcl/tclPlatDecls.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.470460 cocotb-1.8.0rc1/cocotb/_vendor/vhpi/
+-rw-r--r--   0 runner     (501) staff       (20)    42107 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/vhpi/vhpi_user.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.472031 cocotb-1.8.0rc1/cocotb/_vendor/vpi/
+-rw-r--r--   0 runner     (501) staff       (20)    25694 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/vpi/sv_vpi_user.h
+-rw-r--r--   0 runner     (501) staff       (20)    44349 2023-06-12 21:15:18.000000 cocotb-1.8.0rc1/cocotb/_vendor/vpi/vpi_user.h
+-rw-r--r--   0 runner     (501) staff       (20)      298 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/_version.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    26172 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/binary.py
+-rw-r--r--   0 runner     (501) staff       (20)     6560 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/clock.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     9847 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/config.py
+-rw-r--r--   0 runner     (501) staff       (20)    11476 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/decorators.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    41612 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/handle.py
+-rw-r--r--   0 runner     (501) staff       (20)     3136 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/ipython_support.py
+-rw-r--r--   0 runner     (501) staff       (20)    10443 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/log.py
+-rw-r--r--   0 runner     (501) staff       (20)     1853 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/memdebug.py
+-rw-r--r--   0 runner     (501) staff       (20)     1299 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/outcomes.py
+-rw-r--r--   0 runner     (501) staff       (20)     5159 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/queue.py
+-rw-r--r--   0 runner     (501) staff       (20)    32968 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/regression.py
+-rw-r--r--   0 runner     (501) staff       (20)     6696 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/result.py
+-rw-r--r--   0 runner     (501) staff       (20)    35588 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/runner.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    40942 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/scheduler.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.437707 cocotb-1.8.0rc1/cocotb/share/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.476083 cocotb-1.8.0rc1/cocotb/share/def/
+-rw-r--r--   0 runner     (501) staff       (20)       44 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/def/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)      376 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/def/README.md
+-rw-r--r--   0 runner     (501) staff       (20)      930 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/def/aldec.def
+-rw-r--r--   0 runner     (501) staff       (20)      662 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/def/ghdl.def
+-rw-r--r--   0 runner     (501) staff       (20)      655 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/def/icarus.def
+-rw-r--r--   0 runner     (501) staff       (20)     2252 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/def/modelsim.def
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.481112 cocotb-1.8.0rc1/cocotb/share/include/
+-rw-r--r--   0 runner     (501) staff       (20)     3998 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/include/cocotb_utils.h
+-rw-r--r--   0 runner     (501) staff       (20)     2453 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/include/embed.h
+-rw-r--r--   0 runner     (501) staff       (20)      657 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/include/exports.h
+-rw-r--r--   0 runner     (501) staff       (20)     9999 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/include/gpi.h
+-rw-r--r--   0 runner     (501) staff       (20)    10341 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/include/gpi_logging.h
+-rw-r--r--   0 runner     (501) staff       (20)      642 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/include/py_gpi_logging.h
+-rw-r--r--   0 runner     (501) staff       (20)      628 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/include/vhpi_user_ext.h
+-rw-r--r--   0 runner     (501) staff       (20)     2456 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/include/vpi_user_ext.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.437423 cocotb-1.8.0rc1/cocotb/share/lib/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.482299 cocotb-1.8.0rc1/cocotb/share/lib/embed/
+-rw-r--r--   0 runner     (501) staff       (20)     4377 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/embed/embed.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    10476 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/embed/gpi_embed.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.485218 cocotb-1.8.0rc1/cocotb/share/lib/fli/
+-rw-r--r--   0 runner     (501) staff       (20)     7754 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/fli/FliCbHdl.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    40118 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/fli/FliImpl.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    16198 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/fli/FliImpl.h
+-rw-r--r--   0 runner     (501) staff       (20)    26850 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/fli/FliObjHdl.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.487247 cocotb-1.8.0rc1/cocotb/share/lib/gpi/
+-rw-r--r--   0 runner     (501) staff       (20)     4362 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/gpi/GpiCbHdl.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    19643 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/gpi/GpiCommon.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    11255 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/gpi/gpi_priv.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.487877 cocotb-1.8.0rc1/cocotb/share/lib/gpi_log/
+-rw-r--r--   0 runner     (501) staff       (20)     7056 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/gpi_log/gpi_logging.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.488488 cocotb-1.8.0rc1/cocotb/share/lib/py_gpi_log/
+-rw-r--r--   0 runner     (501) staff       (20)     7022 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/py_gpi_log/py_gpi_logging.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.489217 cocotb-1.8.0rc1/cocotb/share/lib/simulator/
+-rw-r--r--   0 runner     (501) staff       (20)    41165 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/simulator/simulatormodule.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.489950 cocotb-1.8.0rc1/cocotb/share/lib/utils/
+-rw-r--r--   0 runner     (501) staff       (20)     3896 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/utils/cocotb_utils.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.490639 cocotb-1.8.0rc1/cocotb/share/lib/verilator/
+-rw-r--r--   0 runner     (501) staff       (20)     4407 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/verilator/verilator.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.492853 cocotb-1.8.0rc1/cocotb/share/lib/vhpi/
+-rw-r--r--   0 runner     (501) staff       (20)    38860 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/vhpi/VhpiCbHdl.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    36640 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/vhpi/VhpiImpl.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    10762 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/vhpi/VhpiImpl.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.495007 cocotb-1.8.0rc1/cocotb/share/lib/vpi/
+-rw-r--r--   0 runner     (501) staff       (20)    27347 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/vpi/VpiCbHdl.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    22748 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/vpi/VpiImpl.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    10441 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/lib/vpi/VpiImpl.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.496844 cocotb-1.8.0rc1/cocotb/share/makefiles/
+-rw-r--r--   0 runner     (501) staff       (20)      416 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/Makefile.deprecations
+-rw-r--r--   0 runner     (501) staff       (20)     7030 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/Makefile.inc
+-rw-r--r--   0 runner     (501) staff       (20)     5299 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/Makefile.sim
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.503902 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/
+-rw-r--r--   0 runner     (501) staff       (20)     2656 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.activehdl
+-rw-r--r--   0 runner     (501) staff       (20)     3901 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.cvc
+-rw-r--r--   0 runner     (501) staff       (20)     3542 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.ghdl
+-rw-r--r--   0 runner     (501) staff       (20)     4374 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.icarus
+-rw-r--r--   0 runner     (501) staff       (20)     4965 2023-06-12 21:15:19.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.ius
+-rw-r--r--   0 runner     (501) staff       (20)     1906 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.modelsim
+-rw-r--r--   0 runner     (501) staff       (20)     6427 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.questa
+-rw-r--r--   0 runner     (501) staff       (20)     5913 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.riviera
+-rw-r--r--   0 runner     (501) staff       (20)     3690 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.vcs
+-rw-r--r--   0 runner     (501) staff       (20)     2407 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.verilator
+-rw-r--r--   0 runner     (501) staff       (20)     5414 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.xcelium
+-rw-r--r--   0 runner     (501) staff       (20)    11035 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/task.py
+-rw-r--r--   0 runner     (501) staff       (20)    32228 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/triggers.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.507084 cocotb-1.8.0rc1/cocotb/types/
+-rw-r--r--   0 runner     (501) staff       (20)     1803 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/types/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    10899 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/types/array.py
+-rw-r--r--   0 runner     (501) staff       (20)     8499 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/types/logic.py
+-rw-r--r--   0 runner     (501) staff       (20)     9957 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/types/logic_array.py
+-rw-r--r--   0 runner     (501) staff       (20)     6230 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/types/range.py
+-rw-r--r--   0 runner     (501) staff       (20)    23064 2023-06-12 21:15:20.000000 cocotb-1.8.0rc1/cocotb/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     5988 2023-06-12 21:15:21.000000 cocotb-1.8.0rc1/cocotb/wavedrom.py
+-rw-r--r--   0 runner     (501) staff       (20)     3552 2023-06-12 21:15:21.000000 cocotb-1.8.0rc1/cocotb/xunit_reporter.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.462964 cocotb-1.8.0rc1/cocotb.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     6717 2023-06-12 21:37:16.000000 cocotb-1.8.0rc1/cocotb.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3103 2023-06-12 21:37:16.000000 cocotb-1.8.0rc1/cocotb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-06-12 21:37:16.000000 cocotb-1.8.0rc1/cocotb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       53 2023-06-12 21:37:16.000000 cocotb-1.8.0rc1/cocotb.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)       33 2023-06-12 21:37:16.000000 cocotb-1.8.0rc1/cocotb.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)      516 2023-06-12 21:37:16.000000 cocotb-1.8.0rc1/cocotb.egg-info/top_level.txt
+-rwxr-xr-x   0 runner     (501) staff       (20)    27213 2023-06-12 21:15:21.000000 cocotb-1.8.0rc1/cocotb_build_libs.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-12 21:37:16.508117 cocotb-1.8.0rc1/pygpi/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-12 21:15:27.000000 cocotb-1.8.0rc1/pygpi/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      946 2023-06-12 21:15:27.000000 cocotb-1.8.0rc1/pygpi/entry.py
+-rw-r--r--   0 runner     (501) staff       (20)     2089 2023-06-12 21:15:27.000000 cocotb-1.8.0rc1/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)      808 2023-06-12 21:37:16.509804 cocotb-1.8.0rc1/setup.cfg
+-rwxr-xr-x   0 runner     (501) staff       (20)     5543 2023-06-12 21:15:27.000000 cocotb-1.8.0rc1/setup.py
```

### Comparing `cocotb-1.8.0/LICENSE` & `cocotb-1.8.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/PKG-INFO` & `cocotb-1.8.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocotb
-Version: 1.8.0
+Version: 1.8.0rc1
 Summary: cocotb is a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
 Home-page: https://www.cocotb.org
 Author: Chris Higgs, Stuart Hodgson
 Maintainer: cocotb contributors
 Maintainer-email: cocotb@lists.librecores.org
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cocotb/cocotb/issues
```

### Comparing `cocotb-1.8.0/README.md` & `cocotb-1.8.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/ANSI.py` & `cocotb-1.8.0rc1/cocotb/ANSI.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/__init__.py` & `cocotb-1.8.0rc1/cocotb/__init__.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/_deprecation.py` & `cocotb-1.8.0rc1/cocotb/_deprecation.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/_py_compat.py` & `cocotb-1.8.0rc1/cocotb/_py_compat.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/_sim_versions.py` & `cocotb-1.8.0rc1/cocotb/_sim_versions.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/_vendor/README.md` & `cocotb-1.8.0rc1/cocotb/_vendor/README.md`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/_vendor/distutils_version.py` & `cocotb-1.8.0rc1/cocotb/_vendor/distutils_version.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/_vendor/fli/acc_user.h` & `cocotb-1.8.0rc1/cocotb/_vendor/fli/acc_user.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/_vendor/fli/acc_vhdl.h` & `cocotb-1.8.0rc1/cocotb/_vendor/fli/acc_vhdl.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/_vendor/fli/mti.h` & `cocotb-1.8.0rc1/cocotb/_vendor/fli/mti.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/_vendor/tcl/license.terms` & `cocotb-1.8.0rc1/cocotb/_vendor/tcl/license.terms`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/_vendor/tcl/tcl.h` & `cocotb-1.8.0rc1/cocotb/_vendor/tcl/tcl.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/_vendor/tcl/tclDecls.h` & `cocotb-1.8.0rc1/cocotb/_vendor/tcl/tclDecls.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/_vendor/tcl/tclPlatDecls.h` & `cocotb-1.8.0rc1/cocotb/_vendor/tcl/tclPlatDecls.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/_vendor/vhpi/vhpi_user.h` & `cocotb-1.8.0rc1/cocotb/_vendor/vhpi/vhpi_user.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/_vendor/vpi/sv_vpi_user.h` & `cocotb-1.8.0rc1/cocotb/_vendor/vpi/sv_vpi_user.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/_vendor/vpi/vpi_user.h` & `cocotb-1.8.0rc1/cocotb/_vendor/vpi/vpi_user.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/binary.py` & `cocotb-1.8.0rc1/cocotb/binary.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/clock.py` & `cocotb-1.8.0rc1/cocotb/clock.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/config.py` & `cocotb-1.8.0rc1/cocotb/config.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/decorators.py` & `cocotb-1.8.0rc1/cocotb/decorators.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/handle.py` & `cocotb-1.8.0rc1/cocotb/handle.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/ipython_support.py` & `cocotb-1.8.0rc1/cocotb/ipython_support.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/log.py` & `cocotb-1.8.0rc1/cocotb/log.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/memdebug.py` & `cocotb-1.8.0rc1/cocotb/memdebug.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/outcomes.py` & `cocotb-1.8.0rc1/cocotb/outcomes.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/queue.py` & `cocotb-1.8.0rc1/cocotb/queue.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/regression.py` & `cocotb-1.8.0rc1/cocotb/regression.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/result.py` & `cocotb-1.8.0rc1/cocotb/result.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/runner.py` & `cocotb-1.8.0rc1/cocotb/runner.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/scheduler.py` & `cocotb-1.8.0rc1/cocotb/scheduler.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/def/aldec.def` & `cocotb-1.8.0rc1/cocotb/share/def/aldec.def`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/def/ghdl.def` & `cocotb-1.8.0rc1/cocotb/share/def/ghdl.def`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/def/icarus.def` & `cocotb-1.8.0rc1/cocotb/share/def/icarus.def`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/def/modelsim.def` & `cocotb-1.8.0rc1/cocotb/share/def/modelsim.def`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/include/cocotb_utils.h` & `cocotb-1.8.0rc1/cocotb/share/include/cocotb_utils.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/include/embed.h` & `cocotb-1.8.0rc1/cocotb/share/include/embed.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/include/exports.h` & `cocotb-1.8.0rc1/cocotb/share/include/exports.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/include/gpi.h` & `cocotb-1.8.0rc1/cocotb/share/include/gpi.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/include/gpi_logging.h` & `cocotb-1.8.0rc1/cocotb/share/include/gpi_logging.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/include/py_gpi_logging.h` & `cocotb-1.8.0rc1/cocotb/share/include/py_gpi_logging.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/include/vhpi_user_ext.h` & `cocotb-1.8.0rc1/cocotb/share/include/vhpi_user_ext.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/include/vpi_user_ext.h` & `cocotb-1.8.0rc1/cocotb/share/include/vpi_user_ext.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/lib/embed/embed.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/embed/embed.cpp`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/lib/embed/gpi_embed.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/embed/gpi_embed.cpp`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/lib/fli/FliCbHdl.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/fli/FliCbHdl.cpp`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/lib/fli/FliImpl.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/fli/FliImpl.cpp`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/lib/fli/FliImpl.h` & `cocotb-1.8.0rc1/cocotb/share/lib/fli/FliImpl.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/lib/fli/FliObjHdl.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/fli/FliObjHdl.cpp`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/lib/gpi/GpiCbHdl.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/gpi/GpiCbHdl.cpp`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/lib/gpi/GpiCommon.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/gpi/GpiCommon.cpp`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/lib/gpi/gpi_priv.h` & `cocotb-1.8.0rc1/cocotb/share/lib/gpi/gpi_priv.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/lib/gpi_log/gpi_logging.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/gpi_log/gpi_logging.cpp`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/lib/py_gpi_log/py_gpi_logging.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/py_gpi_log/py_gpi_logging.cpp`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/lib/simulator/simulatormodule.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/simulator/simulatormodule.cpp`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/lib/utils/cocotb_utils.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/utils/cocotb_utils.cpp`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/lib/verilator/verilator.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/verilator/verilator.cpp`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/lib/vhpi/VhpiCbHdl.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/vhpi/VhpiCbHdl.cpp`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/lib/vhpi/VhpiImpl.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/vhpi/VhpiImpl.cpp`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/lib/vhpi/VhpiImpl.h` & `cocotb-1.8.0rc1/cocotb/share/lib/vhpi/VhpiImpl.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/lib/vpi/VpiCbHdl.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/vpi/VpiCbHdl.cpp`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/lib/vpi/VpiImpl.cpp` & `cocotb-1.8.0rc1/cocotb/share/lib/vpi/VpiImpl.cpp`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/lib/vpi/VpiImpl.h` & `cocotb-1.8.0rc1/cocotb/share/lib/vpi/VpiImpl.h`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/makefiles/Makefile.inc` & `cocotb-1.8.0rc1/cocotb/share/makefiles/Makefile.inc`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/makefiles/Makefile.sim` & `cocotb-1.8.0rc1/cocotb/share/makefiles/Makefile.sim`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.activehdl` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.activehdl`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.cvc` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.cvc`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.ghdl` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.ghdl`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.icarus` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.icarus`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.ius` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.ius`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.modelsim` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.modelsim`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.questa` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.questa`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.riviera` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.riviera`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.vcs` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.vcs`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.verilator` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.verilator`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/share/makefiles/simulators/Makefile.xcelium` & `cocotb-1.8.0rc1/cocotb/share/makefiles/simulators/Makefile.xcelium`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/task.py` & `cocotb-1.8.0rc1/cocotb/task.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/triggers.py` & `cocotb-1.8.0rc1/cocotb/triggers.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/types/__init__.py` & `cocotb-1.8.0rc1/cocotb/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/types/array.py` & `cocotb-1.8.0rc1/cocotb/types/array.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/types/logic.py` & `cocotb-1.8.0rc1/cocotb/types/logic.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/types/logic_array.py` & `cocotb-1.8.0rc1/cocotb/types/logic_array.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/types/range.py` & `cocotb-1.8.0rc1/cocotb/types/range.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/utils.py` & `cocotb-1.8.0rc1/cocotb/utils.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/wavedrom.py` & `cocotb-1.8.0rc1/cocotb/wavedrom.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb/xunit_reporter.py` & `cocotb-1.8.0rc1/cocotb/xunit_reporter.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb.egg-info/PKG-INFO` & `cocotb-1.8.0rc1/cocotb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocotb
-Version: 1.8.0
+Version: 1.8.0rc1
 Summary: cocotb is a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
 Home-page: https://www.cocotb.org
 Author: Chris Higgs, Stuart Hodgson
 Maintainer: cocotb contributors
 Maintainer-email: cocotb@lists.librecores.org
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cocotb/cocotb/issues
```

### Comparing `cocotb-1.8.0/cocotb.egg-info/SOURCES.txt` & `cocotb-1.8.0rc1/cocotb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb.egg-info/top_level.txt` & `cocotb-1.8.0rc1/cocotb.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/cocotb_build_libs.py` & `cocotb-1.8.0rc1/cocotb_build_libs.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/pygpi/entry.py` & `cocotb-1.8.0rc1/pygpi/entry.py`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/pyproject.toml` & `cocotb-1.8.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/setup.cfg` & `cocotb-1.8.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `cocotb-1.8.0/setup.py` & `cocotb-1.8.0rc1/setup.py`

 * *Files identical despite different names*

