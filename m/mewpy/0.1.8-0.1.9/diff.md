# Comparing `tmp/mewpy-0.1.8.tar.gz` & `tmp/mewpy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mewpy-0.1.8.tar", last modified: Tue Jun 22 10:25:09 2021, max compression
+gzip compressed data, was "dist/mewpy-0.1.9.tar", last modified: Mon Jul  5 09:22:30 2021, max compression
```

## Comparing `mewpy-0.1.8.tar` & `mewpy-0.1.9.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    35823 2021-02-17 18:14:33.000000 mewpy-0.1.8/LICENSE
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      223 2021-02-17 18:14:33.000000 mewpy-0.1.8/MANIFEST.in
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1118 2021-06-22 10:25:09.000000 mewpy-0.1.8/PKG-INFO
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     3973 2021-03-08 20:23:07.000000 mewpy-0.1.8/README.md
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      597 2021-02-17 18:14:33.000000 mewpy-0.1.8/README.rst
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/docs/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      633 2021-02-17 18:14:33.000000 mewpy-0.1.8/docs/Makefile
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     2137 2021-02-17 18:14:33.000000 mewpy-0.1.8/docs/conf.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    11852 2021-02-17 18:14:33.000000 mewpy-0.1.8/docs/envelope.png
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      525 2021-02-17 18:14:33.000000 mewpy-0.1.8/docs/index.rst
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      795 2021-02-17 18:14:33.000000 mewpy-0.1.8/docs/make.bat
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    99173 2021-02-17 18:14:33.000000 mewpy-0.1.8/docs/mewpy-2.png
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    55035 2021-02-17 18:14:33.000000 mewpy-0.1.8/docs/mewpy-3.png
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)   149019 2021-02-17 18:14:33.000000 mewpy-0.1.8/docs/mewpy-arch.png
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      708 2021-02-17 18:14:33.000000 mewpy-0.1.8/docs/mewpy.io.rst
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      171 2021-02-17 18:14:33.000000 mewpy-0.1.8/docs/mewpy.model.data.rst
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      541 2021-02-17 18:14:33.000000 mewpy-0.1.8/docs/mewpy.model.rst
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1000 2021-02-17 18:14:33.000000 mewpy-0.1.8/docs/mewpy.optimization.inspyred.rst
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      970 2021-02-17 18:14:33.000000 mewpy-0.1.8/docs/mewpy.optimization.jmetal.rst
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      644 2021-02-17 18:14:33.000000 mewpy-0.1.8/docs/mewpy.optimization.rst
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      802 2021-02-17 18:14:33.000000 mewpy-0.1.8/docs/mewpy.problems.rst
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1768 2021-02-17 18:14:33.000000 mewpy-0.1.8/docs/mewpy.regulation.rst
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      339 2021-02-17 18:14:33.000000 mewpy-0.1.8/docs/mewpy.rst
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      683 2021-02-17 18:14:33.000000 mewpy-0.1.8/docs/mewpy.simulation.rst
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1070 2021-02-17 18:14:33.000000 mewpy-0.1.8/docs/mewpy.utils.rst
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      704 2021-02-17 18:14:33.000000 mewpy-0.1.8/docs/mewpy.visualization.rst
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)       48 2021-02-17 18:14:33.000000 mewpy-0.1.8/docs/modules.rst
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      412 2021-06-22 10:25:09.000000 mewpy-0.1.8/setup.cfg
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1201 2021-06-22 10:01:32.000000 mewpy-0.1.8/setup.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      105 2021-06-22 10:01:32.000000 mewpy-0.1.8/src/mewpy/__init__.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy/algebra/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      750 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/algebra/__init__.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     3864 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/algebra/algebra_constants.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      288 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/algebra/algebra_utils.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     5824 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/algebra/expression.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    17423 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/algebra/parsing.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    15949 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/algebra/symbolic.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy/analysis/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1056 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/analysis/__init__.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      633 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/analysis/analysis_utils.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    20233 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/analysis/fba.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    14925 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/analysis/integrated_analysis.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    12239 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/analysis/metabolic_analysis.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     7353 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/analysis/milp_bool.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     5742 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/analysis/regulatory_analysis.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    20991 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/analysis/rfba.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     3237 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/analysis/sim_bool.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     7957 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/analysis/srfba.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy/io/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    10313 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/io/__init__.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1531 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/io/builder.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     5494 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/io/director.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     6234 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/io/dto.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy/io/engines/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      890 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/io/engines/__init__.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    21611 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/io/engines/cobra.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    29690 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/io/engines/csv.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     5622 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/io/engines/engine.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    10988 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/io/engines/engines_utils.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     2341 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/io/engines/json.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    76091 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/io/engines/sbml.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     5893 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/io/reader.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     4290 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/io/writer.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy/lp/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      281 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/lp/__init__.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     5600 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/lp/linear_containers.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    29683 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/lp/linear_problem.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     7243 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/lp/linear_utils.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    30979 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/lp/linearizer.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      843 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/lp/notification.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy/model/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      180 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/model/__init__.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy/model/data/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-02-17 18:14:33.000000 mewpy-0.1.8/src/mewpy/model/data/__init__.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)  6261715 2021-02-17 18:14:33.000000 mewpy-0.1.8/src/mewpy/model/data/ecYeastGEM_multi-pool.xml
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)  6379721 2021-02-17 18:14:33.000000 mewpy-0.1.8/src/mewpy/model/data/ecYeastGEM_single-pool.xml
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)   183816 2021-02-17 18:14:33.000000 mewpy-0.1.8/src/mewpy/model/data/proteins.txt
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    24009 2021-02-17 18:14:33.000000 mewpy-0.1.8/src/mewpy/model/gecko.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    19864 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/model/metabolic.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    19147 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/model/model.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    14861 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/model/regulatory.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1463 2021-02-17 18:14:33.000000 mewpy-0.1.8/src/mewpy/model/smoment.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy/omics/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)       82 2021-06-17 09:31:29.000000 mewpy-0.1.8/src/mewpy/omics/__init__.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     9871 2021-06-15 14:54:40.000000 mewpy-0.1.8/src/mewpy/omics/expression.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy/omics/integration/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)       51 2021-06-17 09:31:44.000000 mewpy-0.1.8/src/mewpy/omics/integration/__init__.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     2038 2021-06-17 09:40:05.000000 mewpy-0.1.8/src/mewpy/omics/integration/eflux.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     3851 2021-06-17 09:40:03.000000 mewpy-0.1.8/src/mewpy/omics/integration/gimme.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy/optimization/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     4056 2021-06-16 23:26:31.000000 mewpy-0.1.8/src/mewpy/optimization/__init__.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     8933 2021-05-11 10:16:37.000000 mewpy-0.1.8/src/mewpy/optimization/ea.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    22739 2021-06-14 10:34:02.000000 mewpy-0.1.8/src/mewpy/optimization/evaluation.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy/optimization/inspyred/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-02-19 18:22:19.000000 mewpy-0.1.8/src/mewpy/optimization/inspyred/__init__.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     5873 2021-06-16 23:23:47.000000 mewpy-0.1.8/src/mewpy/optimization/inspyred/ea.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     4181 2021-02-20 00:10:42.000000 mewpy-0.1.8/src/mewpy/optimization/inspyred/observers.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    14817 2021-05-11 10:41:44.000000 mewpy-0.1.8/src/mewpy/optimization/inspyred/operators.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1945 2021-02-17 18:14:33.000000 mewpy-0.1.8/src/mewpy/optimization/inspyred/problem.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      832 2021-02-17 18:14:33.000000 mewpy-0.1.8/src/mewpy/optimization/inspyred/settings.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      865 2021-02-17 18:14:33.000000 mewpy-0.1.8/src/mewpy/optimization/inspyred/terminator.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy/optimization/jmetal/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-02-17 18:14:33.000000 mewpy-0.1.8/src/mewpy/optimization/jmetal/__init__.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     6115 2021-06-16 23:24:37.000000 mewpy-0.1.8/src/mewpy/optimization/jmetal/ea.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     4897 2021-02-20 00:30:15.000000 mewpy-0.1.8/src/mewpy/optimization/jmetal/observers.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    14903 2021-06-17 09:48:50.000000 mewpy-0.1.8/src/mewpy/optimization/jmetal/operators.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    10107 2021-05-11 14:00:30.000000 mewpy-0.1.8/src/mewpy/optimization/jmetal/problem.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      138 2021-02-17 18:14:33.000000 mewpy-0.1.8/src/mewpy/optimization/jmetal/settings.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      273 2021-02-17 18:14:33.000000 mewpy-0.1.8/src/mewpy/optimization/settings.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy/problems/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      202 2021-06-16 23:02:53.000000 mewpy-0.1.8/src/mewpy/problems/__init__.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    12319 2021-06-16 10:27:07.000000 mewpy-0.1.8/src/mewpy/problems/etfl.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     7309 2021-02-21 15:06:11.000000 mewpy-0.1.8/src/mewpy/problems/gecko.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     6740 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/problems/genes.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    18625 2021-06-21 16:10:12.000000 mewpy-0.1.8/src/mewpy/problems/problem.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     6388 2021-06-01 11:43:51.000000 mewpy-0.1.8/src/mewpy/problems/reactions.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy/regulation/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      358 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/regulation/__init__.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     5623 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/regulation/optorf.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     7631 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/regulation/optram.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy/simulation/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     7048 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/simulation/__init__.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    23806 2021-06-14 10:55:06.000000 mewpy-0.1.8/src/mewpy/simulation/cobra.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    24391 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/simulation/mew.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    24904 2021-06-14 09:57:45.000000 mewpy-0.1.8/src/mewpy/simulation/reframed.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     7165 2021-03-08 20:14:01.000000 mewpy-0.1.8/src/mewpy/simulation/simulation.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy/solution/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      256 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/solution/__init__.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    14741 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/solution/model_solution.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     4527 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/solution/multi_solution.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1031 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/solution/solution.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy/solvers/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1551 2021-02-21 17:31:09.000000 mewpy-0.1.8/src/mewpy/solvers/__init__.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    18773 2021-03-09 10:50:43.000000 mewpy-0.1.8/src/mewpy/solvers/cplex_solver.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    12582 2021-06-17 09:56:36.000000 mewpy-0.1.8/src/mewpy/solvers/gurobi_solver.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    11031 2021-03-09 11:00:57.000000 mewpy-0.1.8/src/mewpy/solvers/optlang_solver.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     7160 2021-02-23 10:23:16.000000 mewpy-0.1.8/src/mewpy/solvers/solution.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     8036 2021-03-09 10:40:11.000000 mewpy-0.1.8/src/mewpy/solvers/solver.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy/util/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-02-17 18:14:33.000000 mewpy-0.1.8/src/mewpy/util/__init__.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     3675 2021-05-11 10:04:43.000000 mewpy-0.1.8/src/mewpy/util/constants.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     2494 2021-06-18 17:03:07.000000 mewpy-0.1.8/src/mewpy/util/crossmodel.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     7551 2021-02-17 18:14:33.000000 mewpy-0.1.8/src/mewpy/util/graph.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     2967 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/util/history.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    14286 2021-02-21 01:01:07.000000 mewpy-0.1.8/src/mewpy/util/io.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    30952 2021-03-12 17:17:13.000000 mewpy-0.1.8/src/mewpy/util/parsing.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     8647 2021-03-30 14:22:25.000000 mewpy-0.1.8/src/mewpy/util/process.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    21399 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/util/serialization.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     3305 2021-06-14 10:50:35.000000 mewpy-0.1.8/src/mewpy/util/utilities.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy/variables/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      232 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/variables/__init__.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    12609 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/variables/coefficient.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     4852 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/variables/gene.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    16154 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/variables/interaction.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     6541 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/variables/metabolite.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    20621 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/variables/reaction.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     5853 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/variables/regulator.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     5742 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/variables/target.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    20165 2021-03-31 16:03:49.000000 mewpy-0.1.8/src/mewpy/variables/variable.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy/visualization/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-02-17 18:14:33.000000 mewpy-0.1.8/src/mewpy/visualization/__init__.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     4437 2021-02-17 18:14:33.000000 mewpy-0.1.8/src/mewpy/visualization/envelope.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1630 2021-02-17 18:14:33.000000 mewpy-0.1.8/src/mewpy/visualization/escher.py
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    10568 2021-02-20 00:08:15.000000 mewpy-0.1.8/src/mewpy/visualization/plot.py
-drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy.egg-info/
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1118 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy.egg-info/PKG-INFO
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     4434 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy.egg-info/SOURCES.txt
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)        1 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy.egg-info/dependency_links.txt
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)        1 2021-03-30 14:43:59.000000 mewpy-0.1.8/src/mewpy.egg-info/not-zip-safe
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)       93 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy.egg-info/requires.txt
--rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)        6 2021-06-22 10:25:09.000000 mewpy-0.1.8/src/mewpy.egg-info/top_level.txt
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    35823 2021-02-17 18:14:33.000000 mewpy-0.1.9/LICENSE
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      223 2021-02-17 18:14:33.000000 mewpy-0.1.9/MANIFEST.in
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1118 2021-07-05 09:22:30.000000 mewpy-0.1.9/PKG-INFO
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     3973 2021-03-08 20:23:07.000000 mewpy-0.1.9/README.md
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      597 2021-02-17 18:14:33.000000 mewpy-0.1.9/README.rst
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/docs/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      633 2021-02-17 18:14:33.000000 mewpy-0.1.9/docs/Makefile
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     2137 2021-02-17 18:14:33.000000 mewpy-0.1.9/docs/conf.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    11852 2021-02-17 18:14:33.000000 mewpy-0.1.9/docs/envelope.png
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      525 2021-02-17 18:14:33.000000 mewpy-0.1.9/docs/index.rst
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      795 2021-02-17 18:14:33.000000 mewpy-0.1.9/docs/make.bat
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    99173 2021-02-17 18:14:33.000000 mewpy-0.1.9/docs/mewpy-2.png
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    55035 2021-02-17 18:14:33.000000 mewpy-0.1.9/docs/mewpy-3.png
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)   149019 2021-02-17 18:14:33.000000 mewpy-0.1.9/docs/mewpy-arch.png
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      708 2021-02-17 18:14:33.000000 mewpy-0.1.9/docs/mewpy.io.rst
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      171 2021-02-17 18:14:33.000000 mewpy-0.1.9/docs/mewpy.model.data.rst
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      541 2021-02-17 18:14:33.000000 mewpy-0.1.9/docs/mewpy.model.rst
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1000 2021-02-17 18:14:33.000000 mewpy-0.1.9/docs/mewpy.optimization.inspyred.rst
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      970 2021-02-17 18:14:33.000000 mewpy-0.1.9/docs/mewpy.optimization.jmetal.rst
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      644 2021-02-17 18:14:33.000000 mewpy-0.1.9/docs/mewpy.optimization.rst
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      802 2021-02-17 18:14:33.000000 mewpy-0.1.9/docs/mewpy.problems.rst
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1768 2021-02-17 18:14:33.000000 mewpy-0.1.9/docs/mewpy.regulation.rst
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      339 2021-02-17 18:14:33.000000 mewpy-0.1.9/docs/mewpy.rst
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      683 2021-02-17 18:14:33.000000 mewpy-0.1.9/docs/mewpy.simulation.rst
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1070 2021-02-17 18:14:33.000000 mewpy-0.1.9/docs/mewpy.utils.rst
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      704 2021-02-17 18:14:33.000000 mewpy-0.1.9/docs/mewpy.visualization.rst
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)       48 2021-02-17 18:14:33.000000 mewpy-0.1.9/docs/modules.rst
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      412 2021-07-05 09:22:30.000000 mewpy-0.1.9/setup.cfg
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1201 2021-07-05 09:18:30.000000 mewpy-0.1.9/setup.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      105 2021-07-05 09:18:30.000000 mewpy-0.1.9/src/mewpy/__init__.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy/algebra/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      750 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/algebra/__init__.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     3864 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/algebra/algebra_constants.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      288 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/algebra/algebra_utils.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     5824 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/algebra/expression.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    17423 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/algebra/parsing.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    15949 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/algebra/symbolic.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy/analysis/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1056 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/analysis/__init__.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      633 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/analysis/analysis_utils.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    20233 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/analysis/fba.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    14925 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/analysis/integrated_analysis.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    12239 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/analysis/metabolic_analysis.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     7353 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/analysis/milp_bool.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     5742 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/analysis/regulatory_analysis.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    20991 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/analysis/rfba.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     3237 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/analysis/sim_bool.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     7957 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/analysis/srfba.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy/io/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    10313 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/io/__init__.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1531 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/io/builder.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     5494 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/io/director.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     6234 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/io/dto.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy/io/engines/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      890 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/io/engines/__init__.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    21611 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/io/engines/cobra.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    29690 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/io/engines/csv.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     5622 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/io/engines/engine.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    10988 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/io/engines/engines_utils.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     2341 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/io/engines/json.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    76091 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/io/engines/sbml.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     5893 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/io/reader.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     4290 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/io/writer.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy/lp/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      281 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/lp/__init__.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     5600 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/lp/linear_containers.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    29683 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/lp/linear_problem.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     7243 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/lp/linear_utils.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    30979 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/lp/linearizer.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      843 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/lp/notification.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy/model/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      180 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/model/__init__.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy/model/data/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-02-17 18:14:33.000000 mewpy-0.1.9/src/mewpy/model/data/__init__.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)  6261715 2021-02-17 18:14:33.000000 mewpy-0.1.9/src/mewpy/model/data/ecYeastGEM_multi-pool.xml
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)  6379721 2021-02-17 18:14:33.000000 mewpy-0.1.9/src/mewpy/model/data/ecYeastGEM_single-pool.xml
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)   183816 2021-02-17 18:14:33.000000 mewpy-0.1.9/src/mewpy/model/data/proteins.txt
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    24009 2021-02-17 18:14:33.000000 mewpy-0.1.9/src/mewpy/model/gecko.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    19864 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/model/metabolic.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    19147 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/model/model.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    14861 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/model/regulatory.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1463 2021-02-17 18:14:33.000000 mewpy-0.1.9/src/mewpy/model/smoment.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy/omics/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)       82 2021-06-17 09:31:29.000000 mewpy-0.1.9/src/mewpy/omics/__init__.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     9871 2021-06-15 14:54:40.000000 mewpy-0.1.9/src/mewpy/omics/expression.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy/omics/integration/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)       51 2021-06-17 09:31:44.000000 mewpy-0.1.9/src/mewpy/omics/integration/__init__.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     2038 2021-06-17 09:40:05.000000 mewpy-0.1.9/src/mewpy/omics/integration/eflux.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     3851 2021-06-17 09:40:03.000000 mewpy-0.1.9/src/mewpy/omics/integration/gimme.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy/optimization/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     4056 2021-06-16 23:26:31.000000 mewpy-0.1.9/src/mewpy/optimization/__init__.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    10187 2021-07-05 09:06:11.000000 mewpy-0.1.9/src/mewpy/optimization/ea.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    22739 2021-06-14 10:34:02.000000 mewpy-0.1.9/src/mewpy/optimization/evaluation.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy/optimization/inspyred/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-02-19 18:22:19.000000 mewpy-0.1.9/src/mewpy/optimization/inspyred/__init__.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     5873 2021-06-16 23:23:47.000000 mewpy-0.1.9/src/mewpy/optimization/inspyred/ea.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     4181 2021-02-20 00:10:42.000000 mewpy-0.1.9/src/mewpy/optimization/inspyred/observers.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    14817 2021-05-11 10:41:44.000000 mewpy-0.1.9/src/mewpy/optimization/inspyred/operators.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1945 2021-02-17 18:14:33.000000 mewpy-0.1.9/src/mewpy/optimization/inspyred/problem.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      832 2021-02-17 18:14:33.000000 mewpy-0.1.9/src/mewpy/optimization/inspyred/settings.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      865 2021-02-17 18:14:33.000000 mewpy-0.1.9/src/mewpy/optimization/inspyred/terminator.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy/optimization/jmetal/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-02-17 18:14:33.000000 mewpy-0.1.9/src/mewpy/optimization/jmetal/__init__.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     6115 2021-06-16 23:24:37.000000 mewpy-0.1.9/src/mewpy/optimization/jmetal/ea.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     4897 2021-02-20 00:30:15.000000 mewpy-0.1.9/src/mewpy/optimization/jmetal/observers.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    14903 2021-06-17 09:48:50.000000 mewpy-0.1.9/src/mewpy/optimization/jmetal/operators.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    10107 2021-05-11 14:00:30.000000 mewpy-0.1.9/src/mewpy/optimization/jmetal/problem.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      138 2021-02-17 18:14:33.000000 mewpy-0.1.9/src/mewpy/optimization/jmetal/settings.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      273 2021-02-17 18:14:33.000000 mewpy-0.1.9/src/mewpy/optimization/settings.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy/problems/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      202 2021-06-16 23:02:53.000000 mewpy-0.1.9/src/mewpy/problems/__init__.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    12722 2021-07-05 08:56:47.000000 mewpy-0.1.9/src/mewpy/problems/etfl.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     7408 2021-07-05 08:56:47.000000 mewpy-0.1.9/src/mewpy/problems/gecko.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     6132 2021-07-05 08:56:47.000000 mewpy-0.1.9/src/mewpy/problems/genes.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    18558 2021-07-05 08:56:47.000000 mewpy-0.1.9/src/mewpy/problems/problem.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     6528 2021-07-05 08:56:47.000000 mewpy-0.1.9/src/mewpy/problems/reactions.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy/regulation/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      358 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/regulation/__init__.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     5623 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/regulation/optorf.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     7631 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/regulation/optram.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy/simulation/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     7170 2021-07-05 08:56:47.000000 mewpy-0.1.9/src/mewpy/simulation/__init__.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    23837 2021-07-05 08:56:47.000000 mewpy-0.1.9/src/mewpy/simulation/cobra.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    24413 2021-07-05 08:56:47.000000 mewpy-0.1.9/src/mewpy/simulation/mew.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    24950 2021-07-05 08:56:47.000000 mewpy-0.1.9/src/mewpy/simulation/reframed.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     7557 2021-07-05 08:56:47.000000 mewpy-0.1.9/src/mewpy/simulation/simulation.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy/solution/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      256 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/solution/__init__.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    14741 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/solution/model_solution.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     4527 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/solution/multi_solution.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1031 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/solution/solution.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy/solvers/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1551 2021-02-21 17:31:09.000000 mewpy-0.1.9/src/mewpy/solvers/__init__.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    18773 2021-03-09 10:50:43.000000 mewpy-0.1.9/src/mewpy/solvers/cplex_solver.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    12582 2021-06-17 09:56:36.000000 mewpy-0.1.9/src/mewpy/solvers/gurobi_solver.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    11031 2021-03-09 11:00:57.000000 mewpy-0.1.9/src/mewpy/solvers/optlang_solver.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     7160 2021-02-23 10:23:16.000000 mewpy-0.1.9/src/mewpy/solvers/solution.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     8036 2021-03-09 10:40:11.000000 mewpy-0.1.9/src/mewpy/solvers/solver.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy/util/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-02-17 18:14:33.000000 mewpy-0.1.9/src/mewpy/util/__init__.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     3675 2021-05-11 10:04:43.000000 mewpy-0.1.9/src/mewpy/util/constants.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     2494 2021-06-18 17:03:07.000000 mewpy-0.1.9/src/mewpy/util/crossmodel.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     7551 2021-02-17 18:14:33.000000 mewpy-0.1.9/src/mewpy/util/graph.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     2967 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/util/history.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    14286 2021-02-21 01:01:07.000000 mewpy-0.1.9/src/mewpy/util/io.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    30952 2021-03-12 17:17:13.000000 mewpy-0.1.9/src/mewpy/util/parsing.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     8647 2021-03-30 14:22:25.000000 mewpy-0.1.9/src/mewpy/util/process.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    21399 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/util/serialization.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     3305 2021-06-14 10:50:35.000000 mewpy-0.1.9/src/mewpy/util/utilities.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy/variables/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)      232 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/variables/__init__.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    12609 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/variables/coefficient.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     4852 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/variables/gene.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    16154 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/variables/interaction.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     6541 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/variables/metabolite.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    20621 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/variables/reaction.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     5853 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/variables/regulator.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     5742 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/variables/target.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    20165 2021-03-31 16:03:49.000000 mewpy-0.1.9/src/mewpy/variables/variable.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy/visualization/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-02-17 18:14:33.000000 mewpy-0.1.9/src/mewpy/visualization/__init__.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     4437 2021-02-17 18:14:33.000000 mewpy-0.1.9/src/mewpy/visualization/envelope.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1703 2021-07-02 15:48:21.000000 mewpy-0.1.9/src/mewpy/visualization/escher.py
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)    10568 2021-02-20 00:08:15.000000 mewpy-0.1.9/src/mewpy/visualization/plot.py
+drwxrwxr-x   0 vmsapereira  (1000) vmsapereira  (1000)        0 2021-07-05 09:22:30.000000 mewpy-0.1.9/src/mewpy.egg-info/
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     1118 2021-07-05 09:22:29.000000 mewpy-0.1.9/src/mewpy.egg-info/PKG-INFO
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)     4434 2021-07-05 09:22:29.000000 mewpy-0.1.9/src/mewpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)        1 2021-07-05 09:22:29.000000 mewpy-0.1.9/src/mewpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)        1 2021-03-30 14:43:59.000000 mewpy-0.1.9/src/mewpy.egg-info/not-zip-safe
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)       93 2021-07-05 09:22:29.000000 mewpy-0.1.9/src/mewpy.egg-info/requires.txt
+-rw-rw-r--   0 vmsapereira  (1000) vmsapereira  (1000)        6 2021-07-05 09:22:29.000000 mewpy-0.1.9/src/mewpy.egg-info/top_level.txt
```

### Comparing `mewpy-0.1.8/LICENSE` & `mewpy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/PKG-INFO` & `mewpy-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mewpy
-Version: 0.1.8
+Version: 0.1.9
 Summary: mewpy - Metabolic Engineering in Python 
 Home-page: https://github.com/BioSystemsUM/mewpy/
 Author: BiSBII CEB University of Minho
 Author-email: vpereira@ceb.uminho.pt
 License: Apache License Version 2.0
 Description: MEWpy
         ======
```

### Comparing `mewpy-0.1.8/README.md` & `mewpy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/README.rst` & `mewpy-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/docs/Makefile` & `mewpy-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/docs/conf.py` & `mewpy-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/docs/envelope.png` & `mewpy-0.1.9/docs/envelope.png`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/docs/index.rst` & `mewpy-0.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/docs/make.bat` & `mewpy-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/docs/mewpy-2.png` & `mewpy-0.1.9/docs/mewpy-2.png`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/docs/mewpy-3.png` & `mewpy-0.1.9/docs/mewpy-3.png`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/docs/mewpy-arch.png` & `mewpy-0.1.9/docs/mewpy-arch.png`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/docs/mewpy.io.rst` & `mewpy-0.1.9/docs/mewpy.io.rst`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/docs/mewpy.model.rst` & `mewpy-0.1.9/docs/mewpy.model.rst`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/docs/mewpy.optimization.inspyred.rst` & `mewpy-0.1.9/docs/mewpy.optimization.inspyred.rst`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/docs/mewpy.optimization.jmetal.rst` & `mewpy-0.1.9/docs/mewpy.optimization.jmetal.rst`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/docs/mewpy.optimization.rst` & `mewpy-0.1.9/docs/mewpy.optimization.rst`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/docs/mewpy.problems.rst` & `mewpy-0.1.9/docs/mewpy.problems.rst`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/docs/mewpy.regulation.rst` & `mewpy-0.1.9/docs/mewpy.regulation.rst`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/docs/mewpy.simulation.rst` & `mewpy-0.1.9/docs/mewpy.simulation.rst`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/docs/mewpy.utils.rst` & `mewpy-0.1.9/docs/mewpy.utils.rst`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/docs/mewpy.visualization.rst` & `mewpy-0.1.9/docs/mewpy.visualization.rst`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/setup.py` & `mewpy-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 setup_requirements = requirements + ['pytest-runner']
 test_requirements = requirements + ['pytest', 'cplex']
 install_requirements = requirements
 
 setup(
     name='mewpy',
-    version='0.1.8',
+    version='0.1.9',
     python_requires='>=3.6',
     package_dir={'': 'src'},
     packages=find_packages('src'),
     package_data={"": ["*.xml", "*.csv", "*.txt"], 'mewpy': files},
     include_package_data=True,
     zip_safe=False,
     install_requires=install_requirements,
```

### Comparing `mewpy-0.1.8/src/mewpy/algebra/__init__.py` & `mewpy-0.1.9/src/mewpy/algebra/__init__.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/algebra/algebra_constants.py` & `mewpy-0.1.9/src/mewpy/algebra/algebra_constants.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/algebra/expression.py` & `mewpy-0.1.9/src/mewpy/algebra/expression.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/algebra/parsing.py` & `mewpy-0.1.9/src/mewpy/algebra/parsing.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/algebra/symbolic.py` & `mewpy-0.1.9/src/mewpy/algebra/symbolic.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/analysis/__init__.py` & `mewpy-0.1.9/src/mewpy/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/analysis/analysis_utils.py` & `mewpy-0.1.9/src/mewpy/analysis/analysis_utils.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/analysis/fba.py` & `mewpy-0.1.9/src/mewpy/analysis/fba.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/analysis/integrated_analysis.py` & `mewpy-0.1.9/src/mewpy/analysis/integrated_analysis.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/analysis/metabolic_analysis.py` & `mewpy-0.1.9/src/mewpy/analysis/metabolic_analysis.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/analysis/milp_bool.py` & `mewpy-0.1.9/src/mewpy/analysis/milp_bool.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/analysis/regulatory_analysis.py` & `mewpy-0.1.9/src/mewpy/analysis/regulatory_analysis.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/analysis/rfba.py` & `mewpy-0.1.9/src/mewpy/analysis/rfba.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/analysis/sim_bool.py` & `mewpy-0.1.9/src/mewpy/analysis/sim_bool.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/analysis/srfba.py` & `mewpy-0.1.9/src/mewpy/analysis/srfba.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/io/__init__.py` & `mewpy-0.1.9/src/mewpy/io/__init__.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/io/builder.py` & `mewpy-0.1.9/src/mewpy/io/builder.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/io/director.py` & `mewpy-0.1.9/src/mewpy/io/director.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/io/dto.py` & `mewpy-0.1.9/src/mewpy/io/dto.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/io/engines/__init__.py` & `mewpy-0.1.9/src/mewpy/io/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/io/engines/cobra.py` & `mewpy-0.1.9/src/mewpy/io/engines/cobra.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/io/engines/csv.py` & `mewpy-0.1.9/src/mewpy/io/engines/csv.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/io/engines/engine.py` & `mewpy-0.1.9/src/mewpy/io/engines/engine.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/io/engines/engines_utils.py` & `mewpy-0.1.9/src/mewpy/io/engines/engines_utils.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/io/engines/json.py` & `mewpy-0.1.9/src/mewpy/io/engines/json.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/io/engines/sbml.py` & `mewpy-0.1.9/src/mewpy/io/engines/sbml.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/io/reader.py` & `mewpy-0.1.9/src/mewpy/io/reader.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/io/writer.py` & `mewpy-0.1.9/src/mewpy/io/writer.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/lp/linear_containers.py` & `mewpy-0.1.9/src/mewpy/lp/linear_containers.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/lp/linear_problem.py` & `mewpy-0.1.9/src/mewpy/lp/linear_problem.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/lp/linear_utils.py` & `mewpy-0.1.9/src/mewpy/lp/linear_utils.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/lp/linearizer.py` & `mewpy-0.1.9/src/mewpy/lp/linearizer.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/lp/notification.py` & `mewpy-0.1.9/src/mewpy/lp/notification.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/model/data/ecYeastGEM_multi-pool.xml` & `mewpy-0.1.9/src/mewpy/model/data/ecYeastGEM_multi-pool.xml`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/model/data/ecYeastGEM_single-pool.xml` & `mewpy-0.1.9/src/mewpy/model/data/ecYeastGEM_single-pool.xml`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/model/data/proteins.txt` & `mewpy-0.1.9/src/mewpy/model/data/proteins.txt`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/model/gecko.py` & `mewpy-0.1.9/src/mewpy/model/gecko.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/model/metabolic.py` & `mewpy-0.1.9/src/mewpy/model/metabolic.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/model/model.py` & `mewpy-0.1.9/src/mewpy/model/model.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/model/regulatory.py` & `mewpy-0.1.9/src/mewpy/model/regulatory.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/model/smoment.py` & `mewpy-0.1.9/src/mewpy/model/smoment.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/omics/expression.py` & `mewpy-0.1.9/src/mewpy/omics/expression.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/omics/integration/eflux.py` & `mewpy-0.1.9/src/mewpy/omics/integration/eflux.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/omics/integration/gimme.py` & `mewpy-0.1.9/src/mewpy/omics/integration/gimme.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/optimization/__init__.py` & `mewpy-0.1.9/src/mewpy/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/optimization/ea.py` & `mewpy-0.1.9/src/mewpy/optimization/ea.py`

 * *Files 17% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         self.problem = problem
         self.initial_population = initial_population
         self.max_generations = max_generations
         self.visualizer = visualizer
         self.mp = mp
         self.final_population = None
 
-    def run(self):
+    def run(self, simplify=True):
         """ Runs the optimization for the defined problem.
         The number of objectives is defined to be the number of evaluation functions in fevalution.
         """
         # Register signal handler for linux
         signal.signal(signal.SIGINT, self.__signalHandler)
 
         if self.problem.fevaluation is None or len(self.problem.fevaluation) == 0:
@@ -119,18 +119,49 @@
         # builds the target list
         self.problem.pre_process()
 
         if self.problem.number_of_objectives == 1:
             final_pop = self._run_so()
         else:
             final_pop = self._run_mo()
-
-        self.final_population = self._convertPopulation(final_pop)
+        pop = self._convertPopulation(final_pop)
+        pop = filter_duplicates(pop)
+        if simplify:
+            pop = self.problem.simplify_population(pop)
+        self.final_population = pop
         return self.final_population
 
+    def dataframe(self):
+        """Returns a dataframe of the final population.
+
+        :raises Exception: if the final population is empty or None.
+        :return: Returns a dataframe of the final population
+        :rtype: pandas.Dataframe
+        """
+        if not self.final_population:
+            raise Exception("No solutions")
+        table = [[x.values, len(x.values)]+x.fitness for x in self.final_population]
+        import pandas as pd
+        columns = ["Modification", "Size"]
+        columns.extend([obj.short_str() for obj in self.problem.fevaluation])
+        df = pd.DataFrame(table, columns=columns)
+        return df
+
+    def plot(self):
+        """Plots the final population.
+
+        :raises Exception:  if the final population is empty or None.
+        """
+        if not self.final_population:
+            raise Exception("No solutions")
+        from ..visualization.plot import StreamingPlot
+        labels = [obj.short_str() for obj in self.problem.fevaluation]
+        p = StreamingPlot(axis_labels=labels)
+        p.plot(self.final_population)
+
     def __signalHandler(self, signum, frame):
         if EAConstants.KILL_DUMP:
             print("Dumping current population.")
             try:
                 pop = self._get_current_population()
                 data = [s.toDict() for s in pop]
                 import json
```

### Comparing `mewpy-0.1.8/src/mewpy/optimization/evaluation.py` & `mewpy-0.1.9/src/mewpy/optimization/evaluation.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/optimization/inspyred/ea.py` & `mewpy-0.1.9/src/mewpy/optimization/inspyred/ea.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/optimization/inspyred/observers.py` & `mewpy-0.1.9/src/mewpy/optimization/inspyred/observers.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/optimization/inspyred/operators.py` & `mewpy-0.1.9/src/mewpy/optimization/inspyred/operators.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/optimization/inspyred/problem.py` & `mewpy-0.1.9/src/mewpy/optimization/inspyred/problem.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/optimization/inspyred/settings.py` & `mewpy-0.1.9/src/mewpy/optimization/inspyred/settings.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/optimization/inspyred/terminator.py` & `mewpy-0.1.9/src/mewpy/optimization/inspyred/terminator.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/optimization/jmetal/ea.py` & `mewpy-0.1.9/src/mewpy/optimization/jmetal/ea.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/optimization/jmetal/observers.py` & `mewpy-0.1.9/src/mewpy/optimization/jmetal/observers.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/optimization/jmetal/operators.py` & `mewpy-0.1.9/src/mewpy/optimization/jmetal/operators.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/optimization/jmetal/problem.py` & `mewpy-0.1.9/src/mewpy/optimization/jmetal/problem.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/problems/etfl.py` & `mewpy-0.1.9/src/mewpy/problems/etfl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import logging
-import warnings
 import itertools
 
 from .problem import AbstractKOProblem, AbstractOUProblem
 from ..util.parsing import GeneEvaluator, build_tree, Boolean
 
 logger = logging.getLogger(__name__)
 
 
-def gene_has_associated_enzyme(model, gene):
-    if any([gene in x.composition for x in model.enzymes]):
+def gene_has_associated_enzyme(model, gene_id):
+    if any([gene_id in x.composition for x in model.enzymes]):
         try:
             return model._get_translation_name(gene_id)
-        except:
+        except Exception:
             return None
     return None
 
 
 def associated_enzyme(model, gene):
     return [x for x in model.enzymes if gene in x.composition]
 
@@ -61,37 +60,40 @@
             if ee:
                 self.has_enzyme.append(g)
             for e in ee:
                 gene_reaction[g].extend(enzyme_reaction[e.id])
         self.gene_reaction = gene_reaction
 
     def _build_target_list(self):
+        print("Building modification target list.")
         genes = set(self.simulator.genes)
+        # GPR-based
+        print("Computing essential genes.")
         essential = set(self.simulator.essential_genes())
         transport = set(self.simulator.get_transport_genes())
         target = genes - essential - transport
         if self.non_target:
             target = target - set(self.non_target)
         target = list(target)
         self._trg_list = target
 
     def _trans_solution_to_constraints(self, candidate):
         """
         Converts a candidate, dict of genes:0 into a dictionary of constraints.
         """
         genes = list(candidate.keys())
         gr_constraints = dict()
-        no_tans = []
+        no_trans = []
         # Translation
         for g in genes:
             if g in self.has_enzyme:
                 try:
                     rx = self.model._get_translation_name(g)
                     gr_constraints[rx] = 0
-                except:
+                except Exception:
                     no_trans.append(g)
         # GPR based reaction KO
         active_genes = set(self.simulator.genes) - set(genes)
         active_reactions = self.simulator.evaluate_gprs(active_genes)
         catalyzed_reactions = set(itertools.chain.from_iterable(
             [self.gene_reaction[g] for g in genes if g not in no_trans]))
         inactive_reactions = set(self.simulator.reactions) - set(active_reactions) - catalyzed_reactions
@@ -171,15 +173,15 @@
             if ee:
                 self.has_enzyme.append(g)
             for e in ee:
                 gene_reaction[g].extend(enzyme_reaction[e.id])
         self.gene_reaction = gene_reaction
 
     def _build_target_list(self):
-
+        print("Building modification target list.")
         genes = set(self.simulator.genes)
         transport = set(self.simulator.get_transport_genes())
         target = genes - transport
         if self.non_target:
             target = target - set(self.non_target)
         target = list(target)
         self._trg_list = target
@@ -252,15 +254,15 @@
         # translation reactions
         for gene_id, lv in candidate.items():
             if gene_id in self.has_enzyme:
                 try:
                     rx = self.model._get_translation_name(gene_id)
                     gr_constraints.update(
                         self.reaction_constraints(rx, lv))
-                except Exception as ex:
+                except Exception:
                     no_trans.append(gene_id)
         catalyzed_reactions = set(itertools.chain.from_iterable(
             [self.gene_reaction[g] for g in candidate if g not in no_trans]))
         # GPR based reaction
         self.__op()
         # evaluate gpr
         evaluator = GeneEvaluator(
@@ -285,11 +287,18 @@
                         raise ValueError("All UO levels should be positive")
                     else:
                         gr_constraints.update(
                             self.reaction_constraints(rxn_id, lv))
         return gr_constraints
 
     def solution_to_constraints(self, candidate):
+        """Converts a solution, dictionary of modifications, into model constraints.
+
+        :param candidate: The solution
+        :type candidate: dict
+        :return: Dictionary of constraints
+        :rtype: dict
+        """
         if self._only_gpr:
             return self._gpr_solution_to_constraints(candidate)
         else:
             return self._trans_solution_to_constraints(candidate)
```

### Comparing `mewpy-0.1.8/src/mewpy/problems/gecko.py` & `mewpy-0.1.9/src/mewpy/problems/gecko.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,16 +39,18 @@
         self.prot_prefix = kwargs.get('prot_prefix', 'draw_prot_')
         self.simulator.prot_prefix = self.prot_prefix
 
     def _build_target_list(self):
         """
         If not provided, targets are all non essential proteins.
         """
+        print("Building modification target list.")
         proteins = set(self.simulator.proteins)
         # as draw_prot_XXXXXX
+        print("Computing essential proteins.")
         ess = self.simulator.essential_proteins(self.prot_prefix)
         # remove 'draw_prot_'
         n = len(self.prot_prefix)
         essential = set([p[n:] for p in ess])
         target = proteins - essential
         if self.non_target:
             target = target - set(self.non_target)
```

### Comparing `mewpy-0.1.8/src/mewpy/problems/genes.py` & `mewpy-0.1.9/src/mewpy/problems/genes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import logging
-import warnings
-
 from .problem import AbstractKOProblem, AbstractOUProblem
 from ..util.parsing import GeneEvaluator, build_tree, Boolean
 
 logger = logging.getLogger(__name__)
 
 
 class GKOProblem(AbstractKOProblem):
@@ -27,30 +25,23 @@
     """
 
     def __init__(self, model, fevaluation=None, **kwargs):
         super(GKOProblem, self).__init__(
             model, fevaluation=fevaluation, **kwargs)
 
     def _build_target_list(self):
-
+        print("Building modification target list.")
         genes = set(self.simulator.genes)
+        print("Computing essential genes.")
         essential = set(self.simulator.essential_genes())
         transport = set(self.simulator.get_transport_genes())
         target = genes - essential - transport
         if self.non_target:
             target = target - set(self.non_target)
         target = list(target)
-        try:
-            from ..util.constants import EAConstants
-            if EAConstants.PROB_TARGET and self.product:
-                from ..util.graph import probabilistic_gene_targets
-                target = probabilistic_gene_targets(self.model, self.product, target)
-        except Exception as e:
-            warnings.warn(str(e))
-
         self._trg_list = target
 
     def solution_to_constraints(self, candidate):
         """
         Converts a candidate, dict of genes:0 into a dictionary of constraints.
         """
         genes = list(candidate.keys())
@@ -96,22 +87,14 @@
 
         genes = set(self.simulator.genes)
         transport = set(self.simulator.get_transport_genes())
         target = genes - transport
         if self.non_target:
             target = target - set(self.non_target)
         target = list(target)
-        try:
-            from ..util.constants import EAConstants
-            if EAConstants.PROB_TARGET and self.product:
-                from ..util.graph import probabilistic_gene_targets
-                target = probabilistic_gene_targets(self.model, self.product, target)
-        except Exception as e:
-            warnings.warn(str(e))
-
         self._trg_list = target
 
     def __op(self):
         # set default operators as configurable options
         if self._operators:
             pass
         elif not self._temp_op or None in self._temp_op or len(self._temp_op) < 2:
```

### Comparing `mewpy-0.1.8/src/mewpy/problems/problem.py` & `mewpy-0.1.9/src/mewpy/problems/problem.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import copy
 import warnings
 from abc import ABC, abstractmethod
 from enum import Enum
 import numpy as np
-from ..optimization.ea import Solution
+from ..optimization.ea import Solution, filter_duplicates
 from ..simulation import get_simulator
 from ..util.constants import EAConstants, ModelConstants
 
 
 class Strategy(Enum):
     KO = 'KO'
     OU = 'OU'
 
     def __eq__(self, other):
         """Overrides equal to enable string name comparison.
         Allows to seamlessly use:
-            SimulationMethod.FBA = SimulationMethod.FBA
-            SimulationMethod.FBA = 'FBA'
-        without requiring an additional level of comparison (SimulationMethod.FBA.name = 'FBA')
+            Strategy.KO = Strategy.KO
+            Strategy.KO = 'KO'.
         """
         if isinstance(other, Strategy):
             return super().__eq__(other)
         elif isinstance(other, str):
             return self.name == other
         else:
             return False
@@ -203,35 +202,36 @@
         """
         Evaluates a single solution, a list of constraints.
 
         :param solution: The solution to be evaluated.
         :param decode: If the solution needs to be decoded.
         :returns: A list of fitness.
         """
-        p = []
         decoded = {}
         # decoded constraints
         if decode:
             decoded = self.decode(solution)
             constraints = self.solution_to_constraints(decoded)
         else:
             constraints = solution
 
         # pre simulation
         simulation_results = dict()
         try:
+            p = []
             for method in self.methods:
                 simulation_result = self.simulator.simulate(
                     constraints=constraints, method=method, scalefactor=self.scalefactor)
                 simulation_results[method] = simulation_result
             # apply the evaluation function(s)
             for f in self.fevaluation:
-                p.append(f(simulation_results, decoded,
-                           scalefactor=self.scalefactor))
+                v = f(simulation_results, decoded, scalefactor=self.scalefactor)
+                p.append(v)
         except Exception as e:
+            p = []
             for f in self.fevaluation:
                 p.append(f.worst_fitness)
             if EAConstants.DEBUG:
                 warnings.warn(f"Solution couldn't be evaluated [{e}]\n {constraints}")
         return p
 
     @property
@@ -306,15 +306,15 @@
         Returns:
             list: Simplified population
         """
         pop = []
         for solution in population:
             res = self.simplify(solution)
             pop.extend(res)
-        return pop
+        return filter_duplicates(pop)
 
 
 class AbstractKOProblem(AbstractProblem):
     """
     Base class for Knockout optimization problems.
 
     :param model: The constraint metabolic model.
```

### Comparing `mewpy-0.1.8/src/mewpy/problems/reactions.py` & `mewpy-0.1.9/src/mewpy/problems/reactions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import warnings
-from collections import OrderedDict
 import numpy as np
 from .problem import AbstractKOProblem, AbstractOUProblem
 
 
 class RKOProblem(AbstractKOProblem):
     """
     Reaction Knockout Optimization Problem.
@@ -27,15 +25,17 @@
         super(RKOProblem, self).__init__(
             model, fevaluation=fevaluation, **kwargs)
 
     def _build_target_list(self):
         """Default modification target builder.
         Removes drains, transport and essential reactions
         """
+        print("Building modification target list.")
         reactions = set(self.simulator.reactions)
+        print("Computing essential reactions")
         essential = set(self.simulator.essential_reactions())
         drains = set(self.simulator.get_drains())
         transport = set(self.simulator.get_transport_reactions())
         target = reactions - essential - drains - transport
         if self.non_target is not None:
             target = target - set(self.non_target)
         target = list(target)
@@ -64,14 +64,15 @@
     """
 
     def __init__(self, model, fevaluation=None, **kwargs):
         super(ROUProblem, self).__init__(
             model, fevaluation=fevaluation, **kwargs)
 
     def _build_target_list(self):
+        print("Building modification target list.")
         reactions = set(self.simulator.reactions)
         # drains = set(self.simulator.get_drains())
         target = reactions  # - drains
         if self.non_target is not None:
             target = target - set(self.non_target)
         target = list(target)
         self._trg_list = target
@@ -93,16 +94,16 @@
             else:
                 constraints.update(self.reaction_constraints(rxn, lv))
         return constraints
 
 
 class MediumProblem(AbstractOUProblem):
     """
-    Medium Optimization Problem. Try to find an optimized uptake configuration. 
-    By default all uptake reactions are considered. Uptake reactions not included on 
+    Medium Optimization Problem. Try to find an optimized uptake configuration.
+    By default all uptake reactions are considered. Uptake reactions not included in
     a solution candidate are KO.
 
     :param model: The constraint metabolic model.
     :param list fevaluation: A list of callable EvaluationFunctions.
 
     Optional parameters:
 
@@ -117,15 +118,15 @@
     :param list levels: Over/under expression levels (Default [0,0.1,0.2,...,9.9,10.0])
 
     """
 
     def __init__(self, model, fevaluation=None, **kwargs):
         super(ROUProblem, self).__init__(
             model, fevaluation=fevaluation, **kwargs)
-        self.levels = kwargs.get('levels',np.linspace(0,10,101))
+        self.levels = kwargs.get('levels', np.linspace(0, 10, 101))
         self.candidate_max_size = kwargs.get(
             'candidate_max_size', len(self.target))
 
     def _build_target_list(self):
         target = set(self.simulator.get_uptake_reactions())
         if self.non_target is not None:
             target = target - set(self.non_target)
@@ -136,12 +137,13 @@
         """
         Decodes a candidate, a dict {idx:lv} into a dictionary of constraints
         Suposes that reversible reactions have been treated and bounded with positive flux values
         """
         constraints = dict()
         from mewpy.util.constants import ModelConstants
         for rxn in self.target_list:
-            if rxn in candidate.items():
-                constraint[rxn] = (-1*lv, ModelConstants.REACTION_UPPER_BOUND)
+            if rxn in candidate.keys():
+                lv = candidate[rxn]
+                constraints[rxn] = (-1 * lv, ModelConstants.REACTION_UPPER_BOUND)
             else:
-                constraint[rxn] = (0,0)
+                constraints[rxn] = (0, 0)
         return constraints
```

### Comparing `mewpy-0.1.8/src/mewpy/regulation/optorf.py` & `mewpy-0.1.9/src/mewpy/regulation/optorf.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/regulation/optram.py` & `mewpy-0.1.9/src/mewpy/regulation/optram.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/simulation/__init__.py` & `mewpy-0.1.9/src/mewpy/simulation/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,16 @@
         module = __import__(module_name, fromlist=[None])
         class_ = getattr(module, class_name)
         instance = class_(model, envcond=envcond,
                           constraints=constraints, reference=reference, reset_solver=reset_solver)
     elif "etfl" in name:
         try:
             from .cobra import Simulation
+            from etfl.optim.config import standard_solver_config
+            standard_solver_config(model, verbose=False)
             instance = Simulation(
                 model, envcond=envcond, constraints=constraints, reference=reference, reset_solver=reset_solver)
             instance._MAX_STR = 'max'
             instance._MIN_STR = 'min'
         except Exception:
             raise RuntimeError("Could not create simulator for the ETFL model")
     else:
```

### Comparing `mewpy-0.1.8/src/mewpy/simulation/cobra.py` & `mewpy-0.1.9/src/mewpy/simulation/cobra.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from cobra.core.solution import Solution
 from cobra.flux_analysis import pfba, moma, room
 
 from . import get_default_solver, SimulationMethod, SStatus
 from .simulation import Simulator, SimulationResult, ModelContainer
 from ..util.constants import ModelConstants
 from ..util.parsing import evaluate_expression_tree
+from tqdm import tqdm
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 class CobraModelContainer(ModelContainer):
     """ A basic container for COBRApy models.
@@ -63,21 +64,19 @@
         if reaction.gene_reaction_rule:
             return str(reaction.gene_reaction_rule)
         else:
             return None
 
     def get_substrates(self, rxn_id):
         reaction = self.model.reactions.get_by_id(rxn_id)
-        return {k.id: v for k, v in iteritems(reaction.metabolites) if v < 0}
+        return {k.id: v for k, v in reaction.metabolites.items() if v < 0}
 
     def get_products(self, rxn_id):
         reaction = self.model.reactions.get_by_id(rxn_id)
-        return {k.id: v for k, v in iteritems(reaction.metabolites) if v > 0}
-
-
+        return {k.id: v for k, v in reaction.metabolites.items() if v > 0}
 
     def get_drains(self):
         rxns = [r.id for r in self.model.exchanges]
         return rxns
 
 
 class Simulation(CobraModelContainer, Simulator):
@@ -170,15 +169,15 @@
         """
         if self._essential_reactions is not None:
             return self._essential_reactions
         wt_solution = self.simulate()
         wt_growth = wt_solution.objective_value
         reactions = self.reactions
         self._essential_reactions = []
-        for rxn in reactions:
+        for rxn in tqdm(reactions):
             res = self.simulate(constraints={rxn: 0})
             if res:
                 if (res.status == SStatus.OPTIMAL and res.objective_value < wt_growth * min_growth) \
                         or res.status == SStatus.INFEASIBLE:
                     self._essential_reactions.append(rxn)
         return self._essential_reactions
 
@@ -192,15 +191,15 @@
         """
         if self._essential_genes is not None:
             return self._essential_genes
         self._essential_genes = []
         wt_solution = self.simulate()
         wt_growth = wt_solution.objective_value
         genes = self.genes
-        for gene in genes:
+        for gene in tqdm(genes):
             active_genes = set(self.genes) - {gene}
             active_reactions = self.evaluate_gprs(active_genes)
             inactive_reactions = set(self.reactions) - set(active_reactions)
             gr_constraints = {rxn: 0 for rxn in inactive_reactions}
             res = self.simulate(constraints=gr_constraints)
             if res:
                 if (res.status == SStatus.OPTIMAL and res.objective_value < wt_growth * min_growth) \
@@ -316,15 +315,14 @@
                     self._m_r_lookup[m.id][reaction.id] = coeff
 
         return self._m_r_lookup
 
     def metabolite_elements(self, metabolite_id):
         return self.model.metabolites.get_by_id(metabolite_id).elements()
 
-
     def get_reaction_bounds(self, reaction):
         """
         Returns the bounds for a given reaction.
 
         :param reaction: str, reaction ID
         :return: lb(s), ub(s), tuple
 
@@ -522,15 +520,15 @@
     def essential_proteins(self, min_growth=0.01):
         if self._essential_proteins is not None:
             return self._essential_proteins
         wt_solution = self.simulate()
         wt_growth = wt_solution.objective_value
         self._essential_proteins = []
         proteins = self.model.proteins
-        for p in proteins:
+        for p in tqdm(proteins):
             rxn = "{}{}".format(self.protein_prefix, p)
             res = self.simulate(constraints={rxn: 0})
             if res:
                 if (res.status == SStatus.OPTIMAL and res.objective_value < wt_growth * min_growth) or \
                         res.status == SStatus.INFEASIBLE:
                     self._essential_proteins.append(rxn)
         return self._essential_proteins
```

### Comparing `mewpy-0.1.8/src/mewpy/simulation/mew.py` & `mewpy-0.1.9/src/mewpy/simulation/mew.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 from .simulation import Simulator, SimulationResult, ModelContainer
 from mewpy.model import Model, MetabolicModel, RegulatoryModel
 from mewpy.variables import Reaction
 from mewpy.util.constants import ModelConstants
 from mewpy.util.utilities import Dispatcher
 from mewpy.analysis import FBA, pFBA, fva
 from mewpy.solvers.solution import Solution, Status
+from tqdm import tqdm
 
 if TYPE_CHECKING:
     from mewpy.solvers.solver import Solver
     from mewpy.solvers import CplexSolver, GurobiSolver, OptLangSolver
 
 LOGGER = logging.getLogger(__name__)
 
 
 class MewModelContainer(ModelContainer):
 
     def __init__(self, model: Union[Model, MetabolicModel, RegulatoryModel]):
-
         """
         A mew model container. It provides an interface to access mew model containers
 
         :type model: Union[Model, MetabolicModel, RegulatoryModel]
         :param model: A mew Model, MetabolicModel, RegulatoryModel or all together
         """
 
@@ -171,15 +171,14 @@
     def __init__(self,
                  model: Union[Model, MetabolicModel, RegulatoryModel],
                  objective: str = None,
                  envcond: Dict[str, Tuple[Union[int, float], Union[int, float]]] = None,
                  constraints: Dict[str, Tuple[Union[int, float], Union[int, float]]] = None,
                  reference: Dict[str, Union[int, float]] = None,
                  reset_solver=ModelConstants.RESET_SOLVER):
-
         """
         Simulation supports simulation of a mew Model, MetabolicModel, RegulatoryModel or all.
         Additional environmental conditions and constraints can be set using this interface.
         The objective function can be altered too.
         A reference wild type reaction flux values can be provided for convenience.
 
         Simulation offers several methods to retrieve additional information from the model.
@@ -256,15 +255,14 @@
 
         """
         if self._reference is None:
             self._reference = self.simulate(method=SimulationMethod.pFBA).fluxes
         return self._reference
 
     def essential_reactions(self, min_growth=0.01) -> List[str]:
-
         """
         The set of knocked out reactions that impair a minimal growth rate predicted by the model with fba.
         The defined minimal percentage of the wild type growth rate is usually set to 0.01 (1%).
 
         :return: A list of essential reactions.
 
         """
@@ -278,28 +276,27 @@
         wt_solution = self.simulate(method=SimulationMethod.FBA)
         wt_growth = wt_solution.objective_value
 
         self._essential_reactions = []
 
         reactions = self.reactions.copy()
 
-        for rxn in reactions:
+        for rxn in tqdm(reactions):
 
             res = self.simulate(constraints={rxn: 0})
 
             if res:
 
                 if (res.status == SStatus.OPTIMAL and res.objective_value < wt_growth * min_growth) \
                         or res.status == SStatus.INFEASIBLE:
                     self._essential_reactions.append(rxn)
 
         return self._essential_reactions
 
     def essential_genes(self, min_growth=0.01) -> List[str]:
-
         """
         The set of knocked out genes that impair a minimal growth rate predicted by the model with fba.
         The defined minimal percentage of the wild type growth rate is usually set to 0.01 (1%).
 
         :return: A list of essential genes.
 
         """
@@ -313,15 +310,15 @@
         self._essential_genes = []
 
         wt_solution = self.simulate()
         wt_growth = wt_solution.objective_value
 
         values = {gene.id: 1.0 for gene in self.model.yield_genes()}
 
-        for gene in self.model.yield_genes():
+        for gene in tqdm(self.model.yield_genes()):
 
             values[gene.id] = 0.0
 
             constraints = {}
 
             for rxn in gene.yield_reactions():
 
@@ -341,15 +338,14 @@
                 if (res.status == SStatus.OPTIMAL and res.objective_value < wt_growth * min_growth) \
                         or res.status == SStatus.INFEASIBLE:
                     self._essential_genes.append(gene)
 
         return self._essential_genes
 
     def evaluate_gprs(self, active_genes) -> List[str]:
-
         """
         Returns the list of active reactions for a given list of active genes.
 
         :param list active_genes: list of genes identifiers.
         :return: a list of active reaction identifiers.
 
         """
@@ -360,15 +356,14 @@
         values = {gene.id: 1.0 if gene.id in active_genes else 0.0
                   for gene in self.model.yield_genes()}
 
         return [rxn.id for rxn in self.model.yield_reactions()
                 if rxn.gpr.is_none or rxn.gpr.evaluate(values=values)]
 
     def add_reaction(self, reaction: Reaction, replace: bool = True, comprehensive=True):
-
         """
         Adds a reaction to the mew model
 
         :param reaction: Reaction object to be added
         :param replace: Whether to replace the reaction in the model if already exists
         :param comprehensive: Whether to add metabolites and genes associated with the reaction to the model
 
@@ -384,15 +379,14 @@
 
         else:
 
             if reaction.id not in self.model.reactions:
                 self.model.add(reaction, 'reaction', comprehensive=comprehensive, history=False)
 
     def remove_reaction(self, reaction: Reaction, remove_orphans=True):
-
         """
         Removes a reaction from the mew model
 
         :param reaction: Reaction object to be removed
         :param remove_orphans: Whether to remove metabolites and genes orphans associated with the reaction in the model
 
         :return:
@@ -455,15 +449,14 @@
 
             if ext in rxn.compartments and len(rxn.compartments) > 1:
                 genes.update(rxn.genes.keys())
 
         return list(genes)
 
     def reverse_reaction(self, reaction_id: str) -> Union[str, None]:
-
         """
         Identify if a reaction is reversible and returns the reverse reaction if it is the case.
 
         :param reaction_id: a reaction identifier
         :return: a reverse reaction identifier or None
 
         """
@@ -495,15 +488,14 @@
 
                 for met, coef in reaction.stoichiometry.items():
                     self._m_r_lookup[met.id][reaction.id] = coef
 
         return self._m_r_lookup
 
     def get_reaction_bounds(self, reaction: str) -> Tuple[Union[int, float], Union[int, float]]:
-
         """
         Get the bounds for a given reaction.
 
         :param reaction: reaction identifier
 
         :return: a tuple with the reaction bounds
         """
@@ -547,15 +539,14 @@
         if np.isnan(ub):
             LOGGER.warning("Could not identify a median upper bound. Setting the default")
             ub = 1000.0
 
         return lb, ub
 
     def find_unconstrained_reactions(self) -> List[str]:
-
         """
         Finds a list of reactions that are not constrained in the model
 
         :return: list of unconstrained reactions
         """
 
         lb, ub = self.find_bounds()
@@ -646,15 +637,14 @@
                  objective: Dict[str, Union[int, float]] = None,
                  method: SimulationMethod = SimulationMethod.FBA,
                  maximize: bool = True,
                  constraints: Dict[str, Tuple[Union[int, float], Union[int, float]]] = None,
                  reference: Dict[str, Union[int, float]] = None,
                  scalefactor: float = None,
                  solver: Union['Solver', 'CplexSolver', 'GurobiSolver', 'OptLangSolver'] = None) -> SimulationResult:
-
         """
 
         Simulates a phenotype for a given objective and set of constraints using the specified method.
         Reference wild-type conditions are also accepted
 
         :param objective: The simulation objective. If none, the model objective is considered.
         :param method: The SimulationMethod (FBA, pFBA, lMOMA, etc ...).
@@ -704,15 +694,14 @@
             obj_frac: float = 0.9,
             reactions=None,
             constraints=None,
             loopless=False,
             internal=None,
             solver=None,
             format='dict'):
-
         """
 
         It performs a Flux Variability Analysis (FVA).
 
         :param obj_frac: The minimum fraction of the maximum growth rate (default 0.9).
         Requires that the objective value is at least the fraction times maximum objective value.
         A value of 0.85 for instance means that the objective has to be at least at 85% percent of its maximum.
```

### Comparing `mewpy-0.1.8/src/mewpy/simulation/reframed.py` & `mewpy-0.1.9/src/mewpy/simulation/reframed.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,21 @@
 
 from . import SimulationMethod, SStatus, get_default_solver
 from .simulation import Simulator, SimulationResult, ModelContainer
 from ..model.gecko import GeckoModel
 from ..util.constants import ModelConstants
 from ..util.parsing import evaluate_expression_tree
 from ..util.utilities import elements
+from tqdm import tqdm
 
 LOGGER = logging.getLogger(__name__)
 
 solver_map = {'gurobi': 'gurobi', 'cplex': 'cplex', 'glpk': 'optlang'}
 
+
 # TODO: missing proteins and set objective implementations
 class CBModelContainer(ModelContainer):
     """ A basic container for REFRAMED models.
 
     :param model: A metabolic model.
 
     """
@@ -69,19 +71,19 @@
         else:
             return None
 
     def get_drains(self):
         return self.model.get_exchange_reactions()
 
     def get_substrates(self, rxn_id):
-        reaction = self.model.reactions[rxn]
+        reaction = self.model.reactions[rxn_id]
         return {m_id: coeff for m_id, coeff in reaction.stoichiometry.items() if coeff < 0}
 
     def get_products(self, rxn_id):
-        reaction = self.model.reactions[rxn]
+        reaction = self.model.reactions[rxn_id]
         return {m_id: coeff for m_id, coeff in reaction.stoichiometry.items() if coeff > 0}
 
     @property
     def medium(self):
 
         def is_active(rxn):
             """Determine if a boundary reaction permits flux towards creating
@@ -190,15 +192,15 @@
         """
         if self._essential_reactions is not None:
             return self._essential_reactions
         wt_solution = self.simulate()
         wt_growth = wt_solution.objective_value
         reactions = self.model.reactions.keys()
         self._essential_reactions = []
-        for rxn in reactions:
+        for rxn in tqdm(reactions):
             res = self.simulate(constraints={rxn: 0})
             if res:
                 if (res.status == SStatus.OPTIMAL and res.objective_value < wt_growth * min_growth) \
                         or res.status == SStatus.INFEASIBLE:
                     self._essential_reactions.append(rxn)
         return self._essential_reactions
 
@@ -212,15 +214,15 @@
         """
         if self._essential_genes is not None:
             return self._essential_genes
         self._essential_genes = []
         wt_solution = self.simulate()
         wt_growth = wt_solution.objective_value
         genes = self.model.genes
-        for gene in genes:
+        for gene in tqdm(genes):
             active_genes = set(self.model.genes) - {gene}
             active_reactions = self.evaluate_gprs(active_genes)
             inactive_reactions = set(
                 self.model.reactions) - set(active_reactions)
             gr_constraints = {rxn: 0 for rxn in inactive_reactions}
             res = self.simulate(constraints=gr_constraints)
             if res:
@@ -378,15 +380,14 @@
 
         return self._m_r_lookup
 
     def metabolite_elements(self, metabolite_id):
         formula = self.model.metabolites[metabolite_id].metadata['FORMULA']
         return elements(formula)
 
-
     # TODO: this is repeated
     def set_objective(self, reaction):
         self.model.set_objective({reaction: 1})
 
     def get_reaction_bounds(self, reaction):
         """
         Returns the bounds for a given reaction.
@@ -580,15 +581,15 @@
     def essential_proteins(self, min_growth=0.01):
         if self._essential_proteins is not None:
             return self._essential_proteins
         wt_solution = self.simulate()
         wt_growth = wt_solution.objective_value
         self._essential_proteins = []
         proteins = self.model.proteins
-        for p in proteins:
+        for p in tqdm(proteins):
             rxn = "{}{}".format(self.protein_prefix, p)
             res = self.simulate(constraints={rxn: 0})
             if res:
                 if (res.status == SStatus.OPTIMAL and res.objective_value < wt_growth * min_growth) \
                         or res.status == SStatus.INFEASIBLE:
                     self._essential_proteins.append(rxn)
         return self._essential_proteins
```

### Comparing `mewpy-0.1.8/src/mewpy/simulation/simulation.py` & `mewpy-0.1.9/src/mewpy/simulation/simulation.py`

 * *Files 7% similar despite different names*

```diff
@@ -160,38 +160,48 @@
         return (f"objective: {self.objective_value}\nStatus: "
                 f"{self.status}\nConstraints: {self.get_constraints()}\nMethod:{self.method}")
 
     def __str__(self):
         return (f"objective: {self.objective_value}\nStatus: "
                 f"{self.status}\nConstraints: {self.get_constraints()}\nMethod:{self.method}")
 
-    @property
-    def data_frame(self):
+    def find(self, pattern=None, sort=False):
+        values = [(key, value) for key, value in self.fluxes.items()]
+        if pattern:
+            import re
+            re_expr = re.compile(pattern)
+            values = [x for x in values if re_expr.search(x[0]) is not None]
+        if sort:
+            values.sort(key=lambda x: x[1])
         import pandas as pd
-        df = pd.DataFrame(list(self.fluxes.items()), columns=['Reaction ID', 'Flux'])
+        df = pd.DataFrame(values, columns=['Reaction ID', 'Flux rate'])
         return df
 
+    @property
+    def dataframe(self):
+        return self.find()
+
     def get_net_conversion(self, biomassId=None):
         """Returns a string representation of the net conversion.
 
         :params str biosmassId: Biomass identifier (optional)
         :returns: A string representation of the net conversion.
 
         """
 
         left = ""
         right = ""
         firstLeft, firstRight = True, True
-
+        from . import get_simulator
+        sim = get_simulator(self.model)
         ssFluxes = self.fluxes
-        reactions = self.model.reactions
-        for r_id in reactions.keys():
+        for r_id in sim.reactions:
             fluxValue = ssFluxes[r_id]
-            sub = reactions[r_id].get_substrates()
-            prod = reactions[r_id].get_products()
+            sub = list(sim.get_substrates(r_id).keys())
+            prod = list(sim.get_products(r_id).keys())
             # if rId is a drain reaction
             if fluxValue != 0.0 and (len(sub) == 0 or len(prod) == 0):
                 m = sub + prod
                 if fluxValue < 0:
                     if firstLeft:
                         firstLeft = False
                     else:
```

### Comparing `mewpy-0.1.8/src/mewpy/solution/model_solution.py` & `mewpy-0.1.9/src/mewpy/solution/model_solution.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/solution/multi_solution.py` & `mewpy-0.1.9/src/mewpy/solution/multi_solution.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/solution/solution.py` & `mewpy-0.1.9/src/mewpy/solution/solution.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/solvers/__init__.py` & `mewpy-0.1.9/src/mewpy/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/solvers/cplex_solver.py` & `mewpy-0.1.9/src/mewpy/solvers/cplex_solver.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/solvers/gurobi_solver.py` & `mewpy-0.1.9/src/mewpy/solvers/gurobi_solver.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/solvers/optlang_solver.py` & `mewpy-0.1.9/src/mewpy/solvers/optlang_solver.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/solvers/solution.py` & `mewpy-0.1.9/src/mewpy/solvers/solution.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/solvers/solver.py` & `mewpy-0.1.9/src/mewpy/solvers/solver.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/util/constants.py` & `mewpy-0.1.9/src/mewpy/util/constants.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/util/crossmodel.py` & `mewpy-0.1.9/src/mewpy/util/crossmodel.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/util/graph.py` & `mewpy-0.1.9/src/mewpy/util/graph.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/util/history.py` & `mewpy-0.1.9/src/mewpy/util/history.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/util/io.py` & `mewpy-0.1.9/src/mewpy/util/io.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/util/parsing.py` & `mewpy-0.1.9/src/mewpy/util/parsing.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/util/process.py` & `mewpy-0.1.9/src/mewpy/util/process.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/util/serialization.py` & `mewpy-0.1.9/src/mewpy/util/serialization.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/util/utilities.py` & `mewpy-0.1.9/src/mewpy/util/utilities.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/variables/coefficient.py` & `mewpy-0.1.9/src/mewpy/variables/coefficient.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/variables/gene.py` & `mewpy-0.1.9/src/mewpy/variables/gene.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/variables/interaction.py` & `mewpy-0.1.9/src/mewpy/variables/interaction.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/variables/metabolite.py` & `mewpy-0.1.9/src/mewpy/variables/metabolite.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/variables/reaction.py` & `mewpy-0.1.9/src/mewpy/variables/reaction.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/variables/regulator.py` & `mewpy-0.1.9/src/mewpy/variables/regulator.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/variables/target.py` & `mewpy-0.1.9/src/mewpy/variables/target.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/variables/variable.py` & `mewpy-0.1.9/src/mewpy/variables/variable.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/visualization/envelope.py` & `mewpy-0.1.9/src/mewpy/visualization/envelope.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy/visualization/escher.py` & `mewpy-0.1.9/src/mewpy/visualization/escher.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,17 @@
 def build_escher(model=None, fluxes=None, fmt_func=None, **kwargs):
     try:
         import escher
     except ImportError:
         raise RuntimeError("Escher is not installed.")
 
     js = None
-    if isinstance(model, str) and model in escher_maps():
+    if model is None:
+        map_name = 'e_coli_core.Core metabolism'
+    elif isinstance(model, str) and model in escher_maps():
         map_name = model
     else:
         try:
             js = to_json(model)
         except Exception:
             map_name = 'e_coli_core.Core metabolism'
```

### Comparing `mewpy-0.1.8/src/mewpy/visualization/plot.py` & `mewpy-0.1.9/src/mewpy/visualization/plot.py`

 * *Files identical despite different names*

### Comparing `mewpy-0.1.8/src/mewpy.egg-info/PKG-INFO` & `mewpy-0.1.9/src/mewpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mewpy
-Version: 0.1.8
+Version: 0.1.9
 Summary: mewpy - Metabolic Engineering in Python 
 Home-page: https://github.com/BioSystemsUM/mewpy/
 Author: BiSBII CEB University of Minho
 Author-email: vpereira@ceb.uminho.pt
 License: Apache License Version 2.0
 Description: MEWpy
         ======
```

### Comparing `mewpy-0.1.8/src/mewpy.egg-info/SOURCES.txt` & `mewpy-0.1.9/src/mewpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

