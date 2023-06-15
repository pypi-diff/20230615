# Comparing `tmp/pynter-defects-1.0.0.tar.gz` & `tmp/pynter-defects-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynter-defects-1.0.0.tar", last modified: Mon Jun  5 16:16:17 2023, max compression
+gzip compressed data, was "pynter-defects-1.0.1.tar", last modified: Thu Jun 15 16:31:06 2023, max compression
```

## Comparing `pynter-defects-1.0.0.tar` & `pynter-defects-1.0.1.tar`

### file list

```diff
@@ -1,82 +1,91 @@
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-05 16:16:17.454446 pynter-defects-1.0.0/
--rw-rw-r--   0 villa     (1123) villa     (1123)      122 2023-06-05 16:16:17.454446 pynter-defects-1.0.0/PKG-INFO
--rwxrwxr-x   0 villa     (1123) villa     (1123)      299 2022-01-18 18:41:16.000000 pynter-defects-1.0.0/README.md
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-05 16:16:17.126453 pynter-defects-1.0.0/pynter/
--rwxrwxr-x   0 villa     (1123) villa     (1123)     1714 2023-06-05 15:25:10.000000 pynter-defects-1.0.0/pynter/__init__.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-05 16:16:17.146453 pynter-defects-1.0.0/pynter/automations/
--rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.0/pynter/automations/__init__.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     6625 2023-05-30 14:13:48.000000 pynter-defects-1.0.0/pynter/automations/core.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    20887 2023-05-30 14:17:51.000000 pynter-defects-1.0.0/pynter/automations/vasp.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-05 16:16:17.206451 pynter-defects-1.0.0/pynter/cli/
--rw-rw-r--   0 villa     (1123) villa     (1123)     3428 2023-06-01 12:15:01.000000 pynter-defects-1.0.0/pynter/cli/analysis.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     3410 2023-05-31 09:10:02.000000 pynter-defects-1.0.0/pynter/cli/automations.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     5879 2023-06-05 14:30:42.000000 pynter-defects-1.0.0/pynter/cli/config.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    17274 2023-06-05 13:29:31.000000 pynter-defects-1.0.0/pynter/cli/defects.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     3785 2023-06-05 15:33:00.000000 pynter-defects-1.0.0/pynter/cli/hpc.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     6378 2023-06-05 13:18:55.000000 pynter-defects-1.0.0/pynter/cli/inputs.py
--rwxrwxr--   0 villa     (1123) villa     (1123)     1493 2023-06-05 15:11:39.000000 pynter-defects-1.0.0/pynter/cli/main.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     1734 2023-06-02 09:46:40.000000 pynter-defects-1.0.0/pynter/cli/materials_project.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     4058 2023-06-02 14:29:01.000000 pynter-defects-1.0.0/pynter/cli/phase_diagram.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     7896 2023-05-31 09:33:54.000000 pynter-defects-1.0.0/pynter/cli/plotter.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     3782 2023-06-02 14:17:35.000000 pynter-defects-1.0.0/pynter/cli/slurm.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     1452 2023-06-05 09:25:02.000000 pynter-defects-1.0.0/pynter/cli/utils.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-05 16:16:17.214451 pynter-defects-1.0.0/pynter/data/
--rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.0/pynter/data/__init__.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-05 16:16:17.230451 pynter-defects-1.0.0/pynter/data/database/
--rwxrwxr-x   0 villa     (1123) villa     (1123)        3 2020-11-13 14:36:46.000000 pynter-defects-1.0.0/pynter/data/database/__init__.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     2179 2023-05-23 12:43:01.000000 pynter-defects-1.0.0/pynter/data/database/creator.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     5713 2022-01-18 18:41:16.000000 pynter-defects-1.0.0/pynter/data/database/query.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    30031 2023-05-31 16:31:50.000000 pynter-defects-1.0.0/pynter/data/datasets.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     9713 2023-05-31 09:26:11.000000 pynter-defects-1.0.0/pynter/data/jobs.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-05 16:16:17.274450 pynter-defects-1.0.0/pynter/defects/
--rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.0/pynter/defects/__init__.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    45917 2023-06-02 12:11:11.000000 pynter-defects-1.0.0/pynter/defects/analysis.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    10821 2023-05-03 16:47:07.000000 pynter-defects-1.0.0/pynter/defects/corrections.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    35277 2023-05-23 12:43:01.000000 pynter-defects-1.0.0/pynter/defects/defects.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     6471 2023-05-23 12:43:01.000000 pynter-defects-1.0.0/pynter/defects/elasticity.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    11914 2023-05-31 16:46:23.000000 pynter-defects-1.0.0/pynter/defects/entries.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    15353 2023-05-23 12:43:01.000000 pynter-defects-1.0.0/pynter/defects/plotter.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-05 16:16:17.294449 pynter-defects-1.0.0/pynter/defects/pmg/
--rwxrwxr-x   0 villa     (1123) villa     (1123)    24611 2023-04-18 08:58:38.000000 pynter-defects-1.0.0/pynter/defects/pmg/pmg_defects_core.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    39163 2023-04-18 08:58:38.000000 pynter-defects-1.0.0/pynter/defects/pmg/pmg_defects_corrections.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    60074 2023-04-18 08:58:38.000000 pynter-defects-1.0.0/pynter/defects/pmg/pmg_defects_utils.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    39933 2023-04-18 08:58:38.000000 pynter-defects-1.0.0/pynter/defects/pmg/pmg_dos.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    12053 2023-05-23 12:43:01.000000 pynter-defects-1.0.0/pynter/defects/structure.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    19876 2023-05-23 12:43:02.000000 pynter-defects-1.0.0/pynter/defects/thermodynamics.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)      994 2023-04-18 08:58:38.000000 pynter-defects-1.0.0/pynter/defects/utils.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-05 16:16:17.310449 pynter-defects-1.0.0/pynter/phase_diagram/
--rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.0/pynter/phase_diagram/__init__.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    32436 2023-05-23 12:43:02.000000 pynter-defects-1.0.0/pynter/phase_diagram/chempots.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     7430 2023-04-18 08:58:38.000000 pynter-defects-1.0.0/pynter/phase_diagram/plotter.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    10260 2023-05-23 12:43:02.000000 pynter-defects-1.0.0/pynter/phase_diagram/thermodynamics.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-05 16:16:17.358448 pynter-defects-1.0.0/pynter/slurm/
--rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.0/pynter/slurm/__init__.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     9047 2023-06-05 14:47:11.000000 pynter-defects-1.0.0/pynter/slurm/interface.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    10393 2023-05-30 13:23:32.000000 pynter-defects-1.0.0/pynter/slurm/job_script.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     1486 2023-05-23 12:43:02.000000 pynter-defects-1.0.0/pynter/slurm/job_status.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-05 16:16:17.390447 pynter-defects-1.0.0/pynter/tools/
--rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.0/pynter/tools/__init__.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     1038 2020-10-12 14:14:35.000000 pynter-defects-1.0.0/pynter/tools/format.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     7422 2023-06-02 12:18:36.000000 pynter-defects-1.0.0/pynter/tools/materials_project.py
--rw-rw-r--   0 villa     (1123) villa     (1123)      251 2022-01-18 18:41:18.000000 pynter-defects-1.0.0/pynter/tools/plotter.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     9866 2023-05-23 12:43:02.000000 pynter-defects-1.0.0/pynter/tools/structure.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     8433 2023-05-31 15:51:51.000000 pynter-defects-1.0.0/pynter/tools/utils.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-05 16:16:17.422446 pynter-defects-1.0.0/pynter/vasp/
--rwxrwxr-x   0 villa     (1123) villa     (1123)      857 2023-05-23 12:43:02.000000 pynter-defects-1.0.0/pynter/vasp/__init__.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     9438 2022-01-18 18:41:18.000000 pynter-defects-1.0.0/pynter/vasp/analysis.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    10352 2023-05-23 12:43:02.000000 pynter-defects-1.0.0/pynter/vasp/default_inputs.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    36311 2023-05-23 12:43:02.000000 pynter-defects-1.0.0/pynter/vasp/jobs.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     6192 2023-04-18 08:58:38.000000 pynter-defects-1.0.0/pynter/vasp/plotter.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-05 16:16:17.422446 pynter-defects-1.0.0/pynter/vasp/pmg/
--rw-rw-r--   0 villa     (1123) villa     (1123)   183623 2023-04-18 08:58:38.000000 pynter-defects-1.0.0/pynter/vasp/pmg/pmg_electronic_structure_plotter.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    51500 2023-06-05 12:14:41.000000 pynter-defects-1.0.0/pynter/vasp/schemes.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     3845 2020-10-12 14:14:35.000000 pynter-defects-1.0.0/pynter/vasp/utils.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-05 16:16:17.450446 pynter-defects-1.0.0/pynter_defects.egg-info/
--rw-rw-r--   0 villa     (1123) villa     (1123)      122 2023-06-05 16:16:16.000000 pynter-defects-1.0.0/pynter_defects.egg-info/PKG-INFO
--rw-rw-r--   0 villa     (1123) villa     (1123)     1831 2023-06-05 16:16:17.000000 pynter-defects-1.0.0/pynter_defects.egg-info/SOURCES.txt
--rw-rw-r--   0 villa     (1123) villa     (1123)        1 2023-06-05 16:16:16.000000 pynter-defects-1.0.0/pynter_defects.egg-info/dependency_links.txt
--rw-rw-r--   0 villa     (1123) villa     (1123)       48 2023-06-05 16:16:16.000000 pynter-defects-1.0.0/pynter_defects.egg-info/entry_points.txt
--rw-rw-r--   0 villa     (1123) villa     (1123)       89 2023-06-05 16:16:16.000000 pynter-defects-1.0.0/pynter_defects.egg-info/requires.txt
--rw-rw-r--   0 villa     (1123) villa     (1123)       23 2023-06-05 16:16:16.000000 pynter-defects-1.0.0/pynter_defects.egg-info/top_level.txt
--rw-rw-r--   0 villa     (1123) villa     (1123)       38 2023-06-05 16:16:17.454446 pynter-defects-1.0.0/setup.cfg
--rw-rw-r--   0 villa     (1123) villa     (1123)      903 2023-06-05 16:15:48.000000 pynter-defects-1.0.0/setup.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:06.096874 pynter-defects-1.0.1/
+-rw-rw-r--   0 villa     (1123) villa     (1123)      122 2023-06-15 16:31:06.088874 pynter-defects-1.0.1/PKG-INFO
+-rwxrwxr-x   0 villa     (1123) villa     (1123)      299 2022-01-18 18:41:16.000000 pynter-defects-1.0.1/README.md
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:03.884925 pynter-defects-1.0.1/pynter/
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     1793 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/__init__.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:03.992923 pynter-defects-1.0.1/pynter/automations/
+-rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.1/pynter/automations/__init__.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     6625 2023-05-30 14:13:48.000000 pynter-defects-1.0.1/pynter/automations/core.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    20887 2023-05-30 14:17:51.000000 pynter-defects-1.0.1/pynter/automations/vasp.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:04.352914 pynter-defects-1.0.1/pynter/cli/
+-rw-rw-r--   0 villa     (1123) villa     (1123)     3416 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/cli/analysis.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     3410 2023-05-31 09:10:02.000000 pynter-defects-1.0.1/pynter/cli/automations.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     6876 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/cli/config.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)    17275 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/cli/defects.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     5371 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/cli/hpc.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     6375 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/cli/inputs.py
+-rwxrwxr--   0 villa     (1123) villa     (1123)     1493 2023-06-05 15:11:39.000000 pynter-defects-1.0.1/pynter/cli/main.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     1732 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/cli/materials_project.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     4062 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/cli/phase_diagram.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     7896 2023-05-31 09:33:54.000000 pynter-defects-1.0.1/pynter/cli/plotter.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     3782 2023-06-02 14:17:35.000000 pynter-defects-1.0.1/pynter/cli/slurm.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     1452 2023-06-05 09:25:02.000000 pynter-defects-1.0.1/pynter/cli/utils.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:04.424913 pynter-defects-1.0.1/pynter/data/
+-rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.1/pynter/data/__init__.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:04.512911 pynter-defects-1.0.1/pynter/data/database/
+-rwxrwxr-x   0 villa     (1123) villa     (1123)        3 2020-11-13 14:36:46.000000 pynter-defects-1.0.1/pynter/data/database/__init__.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     2179 2023-05-23 12:43:01.000000 pynter-defects-1.0.1/pynter/data/database/creator.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     5713 2022-01-18 18:41:16.000000 pynter-defects-1.0.1/pynter/data/database/query.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    29512 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/data/datasets.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    11765 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/data/jobs.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:04.980900 pynter-defects-1.0.1/pynter/defects/
+-rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.1/pynter/defects/__init__.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    45917 2023-06-02 12:11:11.000000 pynter-defects-1.0.1/pynter/defects/analysis.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)    10821 2023-05-03 16:47:07.000000 pynter-defects-1.0.1/pynter/defects/corrections.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)    35277 2023-05-23 12:43:01.000000 pynter-defects-1.0.1/pynter/defects/defects.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     6471 2023-05-23 12:43:01.000000 pynter-defects-1.0.1/pynter/defects/elasticity.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    11914 2023-05-31 16:46:23.000000 pynter-defects-1.0.1/pynter/defects/entries.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    15353 2023-05-23 12:43:01.000000 pynter-defects-1.0.1/pynter/defects/plotter.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:05.112897 pynter-defects-1.0.1/pynter/defects/pmg/
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    24611 2023-04-18 08:58:38.000000 pynter-defects-1.0.1/pynter/defects/pmg/pmg_defects_core.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)    39163 2023-04-18 08:58:38.000000 pynter-defects-1.0.1/pynter/defects/pmg/pmg_defects_corrections.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)    60074 2023-04-18 08:58:38.000000 pynter-defects-1.0.1/pynter/defects/pmg/pmg_defects_utils.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    39933 2023-04-18 08:58:38.000000 pynter-defects-1.0.1/pynter/defects/pmg/pmg_dos.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)    12053 2023-05-23 12:43:01.000000 pynter-defects-1.0.1/pynter/defects/structure.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    19876 2023-05-23 12:43:02.000000 pynter-defects-1.0.1/pynter/defects/thermodynamics.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)      994 2023-04-18 08:58:38.000000 pynter-defects-1.0.1/pynter/defects/utils.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:05.212895 pynter-defects-1.0.1/pynter/phase_diagram/
+-rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.1/pynter/phase_diagram/__init__.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    32436 2023-05-23 12:43:02.000000 pynter-defects-1.0.1/pynter/phase_diagram/chempots.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     7430 2023-04-18 08:58:38.000000 pynter-defects-1.0.1/pynter/phase_diagram/plotter.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    10388 2023-06-15 16:23:42.000000 pynter-defects-1.0.1/pynter/phase_diagram/thermodynamics.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:05.312892 pynter-defects-1.0.1/pynter/slurm/
+-rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.1/pynter/slurm/__init__.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     9065 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/slurm/interface.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    10416 2023-06-12 14:42:45.000000 pynter-defects-1.0.1/pynter/slurm/job_script.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     1486 2023-05-23 12:43:02.000000 pynter-defects-1.0.1/pynter/slurm/job_status.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:05.528887 pynter-defects-1.0.1/pynter/testing/
+-rw-rw-r--   0 villa     (1123) villa     (1123)     2363 2023-06-15 16:23:42.000000 pynter-defects-1.0.1/pynter/testing/__init__.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     6067 2023-06-15 16:23:42.000000 pynter-defects-1.0.1/pynter/testing/core.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     2574 2023-06-15 16:23:43.000000 pynter-defects-1.0.1/pynter/testing/data.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     1285 2023-06-15 16:23:43.000000 pynter-defects-1.0.1/pynter/testing/defects.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     1493 2023-06-15 16:23:43.000000 pynter-defects-1.0.1/pynter/testing/phase_diagram.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)      988 2023-06-15 16:23:43.000000 pynter-defects-1.0.1/pynter/testing/slurm.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)      916 2023-06-15 16:23:43.000000 pynter-defects-1.0.1/pynter/testing/structure.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)     4923 2023-06-15 16:23:43.000000 pynter-defects-1.0.1/pynter/testing/vasp.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:05.680884 pynter-defects-1.0.1/pynter/tools/
+-rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.1/pynter/tools/__init__.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     1038 2020-10-12 14:14:35.000000 pynter-defects-1.0.1/pynter/tools/format.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     7422 2023-06-02 12:18:36.000000 pynter-defects-1.0.1/pynter/tools/materials_project.py
+-rw-rw-r--   0 villa     (1123) villa     (1123)      251 2022-01-18 18:41:18.000000 pynter-defects-1.0.1/pynter/tools/plotter.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     9866 2023-05-23 12:43:02.000000 pynter-defects-1.0.1/pynter/tools/structure.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     8433 2023-05-31 15:51:51.000000 pynter-defects-1.0.1/pynter/tools/utils.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:05.884879 pynter-defects-1.0.1/pynter/vasp/
+-rwxrwxr-x   0 villa     (1123) villa     (1123)      872 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/vasp/__init__.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     9438 2022-01-18 18:41:18.000000 pynter-defects-1.0.1/pynter/vasp/analysis.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    10352 2023-05-23 12:43:02.000000 pynter-defects-1.0.1/pynter/vasp/default_inputs.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    36627 2023-06-07 14:47:05.000000 pynter-defects-1.0.1/pynter/vasp/jobs.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     6192 2023-04-18 08:58:38.000000 pynter-defects-1.0.1/pynter/vasp/plotter.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:05.904878 pynter-defects-1.0.1/pynter/vasp/pmg/
+-rw-rw-r--   0 villa     (1123) villa     (1123)   183623 2023-04-18 08:58:38.000000 pynter-defects-1.0.1/pynter/vasp/pmg/pmg_electronic_structure_plotter.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)    51500 2023-06-05 12:14:41.000000 pynter-defects-1.0.1/pynter/vasp/schemes.py
+-rwxrwxr-x   0 villa     (1123) villa     (1123)     3845 2020-10-12 14:14:35.000000 pynter-defects-1.0.1/pynter/vasp/utils.py
+drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-15 16:31:06.072875 pynter-defects-1.0.1/pynter_defects.egg-info/
+-rw-rw-r--   0 villa     (1123) villa     (1123)      122 2023-06-15 16:31:02.000000 pynter-defects-1.0.1/pynter_defects.egg-info/PKG-INFO
+-rw-rw-r--   0 villa     (1123) villa     (1123)     2037 2023-06-15 16:31:03.000000 pynter-defects-1.0.1/pynter_defects.egg-info/SOURCES.txt
+-rw-rw-r--   0 villa     (1123) villa     (1123)        1 2023-06-15 16:31:02.000000 pynter-defects-1.0.1/pynter_defects.egg-info/dependency_links.txt
+-rw-rw-r--   0 villa     (1123) villa     (1123)       48 2023-06-15 16:31:02.000000 pynter-defects-1.0.1/pynter_defects.egg-info/entry_points.txt
+-rw-rw-r--   0 villa     (1123) villa     (1123)       89 2023-06-15 16:31:02.000000 pynter-defects-1.0.1/pynter_defects.egg-info/requires.txt
+-rw-rw-r--   0 villa     (1123) villa     (1123)       23 2023-06-15 16:31:02.000000 pynter-defects-1.0.1/pynter_defects.egg-info/top_level.txt
+-rw-rw-r--   0 villa     (1123) villa     (1123)       38 2023-06-15 16:31:06.100874 pynter-defects-1.0.1/setup.cfg
+-rw-rw-r--   0 villa     (1123) villa     (1123)      703 2023-06-15 16:30:04.000000 pynter-defects-1.0.1/setup.py
```

### Comparing `pynter-defects-1.0.0/pynter/__init__.py` & `pynter-defects-1.0.1/pynter/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,42 +25,44 @@
     (dict)
         Configuration dictionary.
     """
     if os.path.exists(cfgfile):
         with open(cfgfile,"r") as ymlfile:
             return yaml.load(ymlfile,Loader=yaml.FullLoader) # add Loader to not get warning
     else:
-        raise FileNotFoundError('%s does not exist. Run the setup.py script to create it.'%cfgfile)
+        raise FileNotFoundError('%s does not exist. Run "pynter configure" in the terminal to create it.'%cfgfile)
         return
 
 
 def run_local(cmd,printout=True,dry_run=False,**kwargs):
     """
     Run a command locally with subprocess package.
 
     Parameters
     ----------
     cmd : (str)
         Command to run.
     printout : (bool), optional
-        Print output and error. The default is True.
+        Print command, output and error. The default is True.
     dry_run : (bool), optional
         Return back the command, without executing it. The default is False.
     **kwargs : (dict)
         Kwargs to pass to subprocess.run().
 
     Returns
     -------
     stdout
     stderr
     """
     if dry_run:
         if printout:
             print(cmd)
         return cmd, ''
+    if printout:
+        print("Run command: %s" %cmd)
     command = cmd.split()
     proc = subprocess.run(command, capture_output=True, shell=False, text=True,**kwargs)
     stdout = proc.stdout
     stderr = proc.stderr
     if printout:
         print(stdout)
         if stderr:
```

### Comparing `pynter-defects-1.0.0/pynter/automations/core.py` & `pynter-defects-1.0.1/pynter/automations/core.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/automations/vasp.py` & `pynter-defects-1.0.1/pynter/automations/vasp.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/cli/analysis.py` & `pynter-defects-1.0.1/pynter/cli/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 Created on Tue May 30 14:07:47 2023
 
 @author: villa
 """
 
 import os
-import json
 import warnings
 import numpy as np
 
 from pymatgen.io.vasp.outputs import Vasprun
 
 
 def setup_analysis(subparsers):
```

### Comparing `pynter-defects-1.0.0/pynter/cli/automations.py` & `pynter-defects-1.0.1/pynter/cli/automations.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/cli/config.py` & `pynter-defects-1.0.1/pynter/cli/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,103 +2,121 @@
 # -*- coding: utf-8 -*-
 """
 Created on Mon Jun  5 16:24:40 2023
 
 @author: villa
 """
 
+import os
+import yaml
+
+
 def setup_config(subparsers):
     parser_configure = subparsers.add_parser('configure',help='Set up pynter configuration files')
-    parser_configure.set_defaults(func=run_config)
-    return
     
-
-def run_config(args):
-
-    import os
-    import yaml
+    parser_configure.add_argument('-e','--exclude',help='Exclude file ("config.yml" or "vasp.yml")',
+                               default=None,metavar='',dest='exclude')
+    parser_configure.add_argument('-i','--info',action='store_true',help='Print configuration files paths',
+                               default=False,dest='info')
+    parser_configure.set_defaults(func=create_config)
     
-    print('Set up configuration file for pynter...\n\n')
+    return
+  
+    
+def create_config(args):
     
+    filename_config = 'config.yml'
+    filename_vasp = 'vasp.yml'
     filepath = os.path.join(os.getenv("HOME"),'.pynter')
-    print('Path of configuration file is: %s' %filepath)
-    if not os.path.exists(filepath):
-        os.makedirs(filepath)
-    
-    filename = input('Choose file name (default: config.yml): ')
-    filename = filename if filename else 'config.yml' 
-    
-    print('Begin setup\n')
-    print('HPC setup:')
-    hostname = input('Hostname: ')
-    localdir = input('Local calculation directory: ')
-    localdir = os.path.abspath(localdir)
-    workdir = input('Remote calculation directory: ')
-    localdir = os.path.normpath(workdir)
-    
-    print('\nDefault settings for job script setup: ')
-    project_id = input('Project ID: ')
-    email = input('email address (Default None): ')
-    path_exe = input('Path of default executable: ')
-    job_script_filename = input('Job script filename (default job.sh): ')
-    
-    print('\nDatabase configuration:')
-    host = input('Host (default: 127.0.0.1 ): ')
-    port = input('Port (default: 27017): ')
-    database = input('Database (default: pynter): ')
-    collection = input('Collection (default vasp): ')
-    
-    
-    job_script_filename = job_script_filename if job_script_filename else 'job.sh'
-    host = host if host else '127.0.0.1'
-    port = port if port else 27017
-    database = database if database else 'pynter'
-    collection = collection if collection else 'vasp'
-    
-    config = {
-        
-        'HPC': 
-              {'hostname': hostname,
-              'localdir': localdir,
-              'workdir': workdir},
-        'API_KEY': 'DSR45TfHVuyuB1WvP1',
-        'job_settings': 
-              {'project_id': project_id,
-              'name': 'no_name',
-              'array_size': None,
-              'email': email,
-              'nodes': 4,
-              'cores_per_node': 96,
-              'output_filename': 'out.%j',
-              'error_filename': 'err.%j',
-              'timelimit': '24:00:00',
-              'memory_per_cpu': 3500,
-              'partition': None,
-              'processor': None,
-              'modules': ['intel/2020.2','intelmpi/2020.2','fftw/3.3.8'],
-              'path_exe': path_exe,
-              'add_stop_array': True,
-              'add_automation': None,
-              'add_lines_header': ['I_MPI_PMI_LIBRARY=/opt/slurm/current/lib/libpmi2.so'],
-              'add_lines_body': None,
-              'filename': job_script_filename},
-        'dbconfig': 
-              {'vasp': 
-                   {'collection': collection,
-                   'database': database,
-                   'host': host,
-                   'password': None,
-                   'port': port,
-                   'user': None}}}
     
+    # print configuration files path
+    if args.info:
+        print('Path of general configuration file: %s' %(os.path.join(filepath,filename_config)))
+        print('Path of vasp configuration file: %s' %(os.path.join(filepath,filename_vasp)))
+        return
+
+    # Set config.yml
+    if args.exclude != filename_config:
+        print('Set up configuration file for pynter...\n\n')
+        print('Path of configuration file is: %s' %filepath)
+        if not os.path.exists(filepath):
+            os.makedirs(filepath)
+        
+        filename = filename_config
+        
+        print('Begin setup\n')
+        print('HPC setup:')
+        hostname = input('Hostname: ')
+        localdir = input('Local calculation directory: ')
+        localdir = os.path.abspath(localdir)
+        workdir = input('Remote calculation directory: ')
+        workdir = os.path.normpath(workdir)
         
-    with open(os.path.join(filepath,filename),'w+') as f:
-        yaml.dump(config,f) 
+        print('\nDefault settings for job script setup: ')
+        project_id = input('Project ID: ')
+        email = input('email address (Default None): ')
+        path_exe = input('Path of default executable: ')
+        job_script_filename = input('Job script filename (default job.sh): ')
         
-    print(f'Configuration file {filename} written in {filepath}\n')    
+        API_KEY = input('\nMaterials Project API_KEY (default None):')
+        
+        print('\nDatabase configuration:')
+        host = input('Host (default: 127.0.0.1 ): ')
+        port = input('Port (default: 27017): ')
+        database = input('Database (default: pynter): ')
+        collection = input('Collection (default vasp): ')
+        
+        
+        job_script_filename = job_script_filename if job_script_filename else 'job.sh'
+        host = host if host else '127.0.0.1'
+        port = port if port else 27017
+        database = database if database else 'pynter'
+        collection = collection if collection else 'vasp'
+        
+        config = {
+            
+            'HPC': 
+                  {'hostname': hostname,
+                  'localdir': localdir,
+                  'workdir': workdir},
+            'API_KEY': API_KEY,
+            'job_settings': 
+                  {'project_id': project_id,
+                  'name': 'no_name',
+                  'array_size': None,
+                  'email': email,
+                  'nodes': 4,
+                  'cores_per_node': 96,
+                  'output_filename': 'out.%j',
+                  'error_filename': 'err.%j',
+                  'timelimit': '24:00:00',
+                  'memory_per_cpu': 3500,
+                  'partition': None,
+                  'processor': None,
+                  'modules': ['intel/2020.2','intelmpi/2020.2','fftw/3.3.8'],
+                  'path_exe': path_exe,
+                  'add_stop_array': True,
+                  'add_automation': None,
+                  'add_lines_header': ['I_MPI_PMI_LIBRARY=/opt/slurm/current/lib/libpmi2.so'],
+                  'add_lines_body': None,
+                  'filename': job_script_filename},
+            'dbconfig': 
+                  {'vasp': 
+                       {'collection': collection,
+                       'database': database,
+                       'host': host,
+                       'password': None,
+                       'port': port,
+                       'user': None}}}
+        
+        
+        with open(os.path.join(filepath,filename),'w+') as f:
+            yaml.dump(config,f) 
+            
+        print(f'Configuration file {filename} written in {filepath}\n')    
         
     
     vasp_default = {
       'incar_default': {'ALGO': 'Normal',
       'AMIX': 0.2,
       'EDIFF': 1e-06,
       'EDIFFG': -0.05,
@@ -112,15 +130,15 @@
       'LREAL': '.FALSE.',
       'LWAVE': '.TRUE.',
       'NELM': 200,
       'NSW': 0,
       'SIGMA': 0.05},
      
      'computed_entry_default': ['final_energy','structures','eigenvalue_band_properties',
-                                'parameters','actual_kpoints'],
+                                'parameters','actual_kpoints','ionic_steps'],
      
      'default_potcar_symbols': {'Ac': 'Ac',
       'Ag': 'Ag',
       'Al': 'Al',
       'Ar': 'Ar',
       'As': 'As',
       'Au': 'Au',
@@ -204,21 +222,23 @@
       'W': 'W_pv',
       'Xe': 'Xe',
       'Y': 'Y_sv',
       'Yb': 'Yb_2',
       'Zn': 'Zn',
       'Zr': 'Zr_sv'}}
     
-    filename = input('Choose file name for vasp default parameters(default: vasp.yml): ')
-    filename = filename if filename else 'vasp.yml' 
-    
-    with open(os.path.join(filepath,filename),'w+') as f:
-        yaml.dump(vasp_default,f) 
+    # set vasp.yml
+    if args.exclude != filename_vasp:
     
-    print(f'Vasp default file {filename} written in {filepath}')  
+        filename = filename_vasp
+        
+        with open(os.path.join(filepath,filename),'w+') as f:
+            yaml.dump(vasp_default,f) 
+        
+        print(f'Vasp default file {filename} written in {filepath}')
```

### Comparing `pynter-defects-1.0.0/pynter/cli/defects.py` & `pynter-defects-1.0.1/pynter/cli/defects.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,21 +13,19 @@
 import warnings
 from pprint import pprint
 
 from pymatgen.electronic_structure.dos import FermiDos
 
 from pynter.data.datasets import Dataset
 from pynter.vasp.jobs import VaspJob
-from pynter.vasp.schemes import AdvancedSchemes
 from pynter.slurm.job_script import ScriptHandler
 from pynter.defects.entries import DefectEntry
 from pynter.defects.analysis import DefectsAnalysis
 from pynter.defects.corrections import get_kumagai_correction_from_jobs
 from pynter.phase_diagram.chempots import Chempots, Reservoirs
-from pynter.tools.materials_project import MPDatabase
 from pynter.tools.utils import save_object_as_json, get_object_from_json
 from pynter.cli import inputs
 from pynter.cli.utils import get_dict_from_line_string, round_floats
 
 
 
 def setup_defects(subparsers):
@@ -75,27 +73,29 @@
                         default=None,metavar='',dest='vacancies')
     
     parser_vasp.set_defaults(func=create_vasp_inputs)
     return
 
 
 def create_vasp_inputs(args):
+    jobs = []
     schemes = inputs.get_schemes(args)
     if args.substitutions:
         elements_to_replace_with_charges = json.loads(args.substitutions)
         jobs_sub = schemes.substitutions_pbe_relaxation(elements_to_replace_with_charges=elements_to_replace_with_charges,
                                                     supercell_size=args.supercell_size,automation=args.automation,
                                                     locpot=True,rel_scheme=args.relaxation_scheme)
+        jobs = jobs + jobs_sub
     if args.vacancies:
         elements_with_charges = json.loads(args.vacancies)
         jobs_vac = schemes.vacancies_pbe_relaxation(elements_with_charges=elements_with_charges,
                                                     supercell_size=args.supercell_size,automation=args.automation,
                                                     locpot=True,rel_scheme=args.relaxation_scheme)
-    
-    jobs = jobs_sub + jobs_vac
+        jobs = jobs + jobs_vac
+
     ds = Dataset(jobs)
     ds.write_jobs_input()
     return
 
 
 def setup_import(parser):
     job_script_filename = ScriptHandler().filename
@@ -213,14 +213,15 @@
         raise ValueError('DefectsAnalysis object must be provided as json file')
     return da
         
 def get_chempots(args):
     if args.chempots:
         chempots_dict = get_dict_from_line_string(args.chempots)
     else:
+        from pynter.tools.materials_project import MPDatabase
         mpd = MPDatabase()
         compositions = args.da.elements
         entries_dict = mpd.get_entries_from_compositions(compositions,lowest_e_above_hull=True)
         chempots_dict = {el:entry.energy_per_atom for el,entry in entries_dict.items()} #get elemental chempots from MP
         warnings.warn('Chemical potentials have not been provided, elemental chemical potentials taken ' \
                       'from the Materials Project database. Use with care.')
         print('Chemical potentials:')
```

### Comparing `pynter-defects-1.0.0/pynter/cli/inputs.py` & `pynter-defects-1.0.1/pynter/cli/inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 # -*- coding: utf-8 -*-
 """
 Created on Fri Jun  2 15:05:08 2023
 
 @author: villa
 """
 import os
-import importlib
 
 from pymatgen.io.vasp.inputs import Incar,Kpoints,Poscar,Potcar
 
 from pynter.data.datasets import Dataset
 from pynter.slurm.job_script import ScriptHandler
-from pynter.tools.materials_project import MPDatabase
-from pynter.vasp.schemes import InputSets,AdvancedSchemes
+from pynter.vasp.schemes import AdvancedSchemes
 
 
 def setup_inputs(subparsers):
     
     parser_schemes = subparsers.add_parser('inputs',help='Create inputs for several calculation schemes')
     subparsers_schemes = parser_schemes.add_subparsers()
 
@@ -28,15 +26,15 @@
 
 
 def setup_inputs_vasp(parser):
     parser = parse_common_args(parser)
     parser = parse_vasp_args(parser)
     
     parser.add_argument('-cs','--charge-states',action='append',help='Charged states. Provide a list of integer charge states',required=False,
-                        type=int,default=None,dest='charge_states')
+                        type=int,default=None,metavar='',dest='charge_states')
     
     parser.add_argument('-dp','--dielectric-properties',action='store_true',help='Electronic and ionic parts of the dielectric tensor',required=False,
                         default=False,dest='dielectric_properties')
 
     parser.add_argument('-ec','--encut-convergence',action='store_true',help='Energy cutoff convergence',required=False,
                         default=False,dest='encut_convergence')
     
@@ -97,41 +95,42 @@
         
 
 def get_schemes(args):    
     if args.poscar:
         poscar = Poscar.from_file(os.path.abspath(args.poscar))
         structure = poscar.structure
     elif args.mp_id:
+        from pynter.tools.materials_project import MPDatabase
         structure = MPDatabase(args.mp_id).get_structure()
     else:
         raise ValueError('Either POSCAR or Materials Project ID needs to be provided')
 
     incar = Incar.from_file(os.path.abspath(args.incar)) if args.incar else None
-    kpoints = Incar.from_file(os.path.abspath(args.kpoints)) if args.kpoints else None
+    kpoints = Kpoints.from_file(os.path.abspath(args.kpoints)) if args.kpoints else None
     potcar = Potcar.from_file(os.path.abspath(args.potcar)) if args.potcar else None
     if args.job_script:
         script_path = os.path.abspath(os.path.dirname(args.job_script))
         job_settings = ScriptHandler.from_file(path=script_path,filename=os.path.basename(args.job_script)).settings
     else:
         job_settings = None
     
     schemes = AdvancedSchemes(path=args.path,structure=structure,incar_settings=incar,
                                kpoints=kpoints,potcar=potcar,job_settings=job_settings,
                                name=args.name,add_parent_folder=True)
     return schemes
 
 
 def parse_common_args(parser):
-    parser.add_argument('-id','--materials-project-id',help='Materials project ID containing the structure, in case the POSCAR is not provided (default %(default)s)',
+    parser.add_argument('-id','--materials-project-id',help='Materials project ID containing the structure, in case the POSCAR is not provided (default: %(default)s)',
                         required=False,type=str,default=None,metavar='',dest='mp_id')
 
-    parser.add_argument('-n','--name',help='Name of the folder containing input files (default %(default)s)',required=False,type=str,
+    parser.add_argument('-n','--name',help='Name of the folder containing input files (default: %(default)s)',required=False,type=str,
                         default='inputs',metavar='',dest='name')
     
-    parser.add_argument('-p','--path',help='Path for input files (default %(default)s)',required=False,type=str,
+    parser.add_argument('-p','--path',help='Path for input files (default: %(default)s)',required=False,type=str,
                         default=os.getcwd(),metavar='',dest='path')
     
     return parser
 
 
 def parse_vasp_args(parser):
```

### Comparing `pynter-defects-1.0.0/pynter/cli/main.py` & `pynter-defects-1.0.1/pynter/cli/main.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/cli/materials_project.py` & `pynter-defects-1.0.1/pynter/cli/materials_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 Created on Fri Jun  2 11:27:24 2023
 
 @author: villa
 """
 
 from pymatgen.io.vasp.inputs import Poscar
 
-from pynter.tools.materials_project import MPDatabase
-
 
 def setup_mp_database(subparsers):
     
     parser_sub = subparsers.add_parser('MP',help='Interface with Materials Project database')
     
     parser_sub.add_argument('-id','--mp-id',help='Materials project ID',required=True,type=str,metavar='',dest='mp_id')
     parser_sub.add_argument('-s','--structure',help='print Structure',action='store_true',required=False,default=False,dest='print_structure')
@@ -26,15 +24,15 @@
                         default='POSCAR',type=str,metavar='',dest='filename')
     
     parser_sub.set_defaults(func=run_mp_database)
     return
     
 
 def run_mp_database(args):
-    
+    from pynter.tools.materials_project import MPDatabase
     mp = MPDatabase(mp_id=args.mp_id)
     structure = mp.get_structure(final=args.get_final,conventional_unit_cell=args.get_conventional)
     
     if args.print_structure:
         print(structure)
     if args.write_poscar:
         Poscar(structure).write_file(args.filename)
```

### Comparing `pynter-defects-1.0.0/pynter/cli/phase_diagram.py` & `pynter-defects-1.0.1/pynter/cli/phase_diagram.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 Created on Wed May 31 14:50:11 2023
 
 @author: villa
 """
 import os
 
 from pymatgen.core.composition import Composition
-from pymatgen.ext.matproj import MPRester
 from pymatgen.entries.compatibility import MaterialsProjectCompatibility
 from pymatgen.analysis.phase_diagram import PhaseDiagram
 
 from pynter.__init__ import load_config
 from pynter.phase_diagram.chempots import PDHandler, Reservoirs
 from pynter.tools.utils import save_object_as_json
 
@@ -71,14 +70,15 @@
     return
 
 
 def get_chempots(pd,composition):
     return PDHandler(pd).get_all_boundaries_chempots(composition)
     
 def get_phase_diagram(elements):  
+    from pymatgen.ext.matproj import MPRester
     with MPRester(load_config()['API_KEY']) as mpr:
         compat = MaterialsProjectCompatibility()  # sets energy corrections and +U/pseudopotential choice
         unprocessed_entries = mpr.get_entries_in_chemsys(elements,inc_structure=True)
     processed_entries = compat.process_entries(unprocessed_entries)  # filter and add energy corrections    
     return PhaseDiagram(processed_entries)
 
 def plot_pd(pd):
```

### Comparing `pynter-defects-1.0.0/pynter/cli/plotter.py` & `pynter-defects-1.0.1/pynter/cli/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/cli/slurm.py` & `pynter-defects-1.0.1/pynter/cli/slurm.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/cli/utils.py` & `pynter-defects-1.0.1/pynter/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/data/database/creator.py` & `pynter-defects-1.0.1/pynter/data/database/creator.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/data/database/query.py` & `pynter-defects-1.0.1/pynter/data/database/query.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/data/datasets.py` & `pynter-defects-1.0.1/pynter/data/datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 
 import os
 import os.path as op
 from pynter.vasp.jobs import VaspJob, VaspNEBJob
+from pynter.data.jobs import get_job_from_directory
 from pynter.slurm.interface import HPCInterface
 import pandas as pd
 import json
 from monty.json import MontyDecoder
 from pynter.tools.utils import get_object_feature, sort_objects
 
 def _check_job_script(job_script_filenames,files):
-    """ Check if job script names are in a list of files. Can be either a str or list of str"""
+    """
+    Check if job script names are in a list of files. Can be either a str or list of str
+    """
     check = False
     if isinstance(job_script_filenames,str):    
         if job_script_filenames in files:
             check= True
             job_script_filename = job_script_filenames
         else:
             job_script_filename = None
@@ -40,43 +43,34 @@
     path : (str)
         Parent directory.
     job_script_filenames : (str or list), optional
         Filename of job bash script. The default is 'job.sh'. Can also be a list of strings if multiple 
         file names are present. The default is 'job.sh'.
     sort : (str or list), optional
         Sort list of jobs by features. If False or None jobs are not sorted. The default is 'name'.
+    load_outputs : (bool)
+        Load job outputs. The default is True.
     jobs_kwargs : (dict), optional
-        Dictionay with job class name as keys and kwargs as values. Kwargs to be used when importing job 
+        Dictionary with job class name as keys and kwargs as values. Kwargs to be used when importing job 
         from directory for each job class.
 
     Returns
     -------
     jobs : (list)
         List of Job objects.
 
     """
     jobs = []    
     for root , dirs, files in os.walk(path):
         if files != []:
             check_job_script, job_script_filename = _check_job_script(job_script_filenames,files)
             if check_job_script:
-                if all(f in files for f in ['INCAR','KPOINTS','POSCAR','POTCAR']):
-                    path = op.abspath(root)
-                    if jobs_kwargs:
-                        kwargs = jobs_kwargs['VaspJob'] if 'VaspJob' in jobs_kwargs.keys() else {}
-                    else:
-                        kwargs = {}
-                    j = VaspJob.from_directory(path,job_script_filename=job_script_filename,load_outputs=load_outputs,**kwargs)
-                    j.job_script_filename = job_script_filename
-                    jobs.append(j)
-                elif all(f in files for f in ['INCAR','KPOINTS','POTCAR']) and 'POSCAR' not in files:
-                    path = op.abspath(root)
-                    j = VaspNEBJob.from_directory(path,job_script_filename=job_script_filename,load_outputs=load_outputs)
-                    j.job_script_filename = job_script_filename
-                    jobs.append(j)
+                j = get_job_from_directory(path=root,job_script_filename=job_script_filename,
+                                           load_outputs=load_outputs,jobs_kwargs=jobs_kwargs)
+                jobs.append(j)
     if sort:
         jobs = Dataset().sort_jobs(jobs_to_sort=jobs,features=sort)
                 
     return jobs
 
 
 
@@ -221,21 +215,23 @@
         path : (str)
             Parent directory of the dataset. If None the current wdir is used.
        job_script_filenames : (str or list), optional
             Filename of job bash script. The default is 'job.sh'. Can also be a list of strings if multiple 
             file names are present. The default is 'job.sh'.
         sort : (str or list), optional
             Sort list of jobs by feature. If False or None jobs are not sorted. The default is 'name'.
+        load_outputs : (bool)
+            Load job outputs. The default is True.
         jobs_kwargs : (dict), optional
-            Dictionay with job class name as keys and kwargs as values. Kwargs to be used when importing job 
+            Dictionary with job class name as keys and kwargs as values. Kwargs to be used when importing job 
             from directory for each job class.
         """
         path = path if path else os.getcwd()
         jobs = find_jobs(path,job_script_filenames=job_script_filenames,sort='name',
-                         load_outputs=load_outputs,jobs_kwargs=jobs_kwargs) # names are sorted in __init__ method
+                         load_outputs=load_outputs,jobs_kwargs=jobs_kwargs) 
         
         return  Dataset(path=path,jobs=jobs,sort=sort)
     
     
     @property
     def groups(self):
         """Directory names of the first subdirectories in the dataset path."""
```

### Comparing `pynter-defects-1.0.0/pynter/data/jobs.py` & `pynter-defects-1.0.1/pynter/data/jobs.py`

 * *Files 15% similar despite different names*

```diff
@@ -314,8 +314,52 @@
         return status
  
            
     @abstractmethod
     def write_input():
         pass
         
-            
+
+
+def get_job_from_directory(path=None,job_script_filename=None,load_outputs=True,jobs_kwargs=None):   
+    """
+    Get Job object froma directory. The job type is selected based on the content of the folder.
+    - If ("INCAR","KPOINTS","POSCAR","POTCAR") files are present, VaspJob is initialized.
+    - If ("INCAR","KPOINTS","POTCAR") files are present and "POSCAR" is not present, VaspNEBJob is initialized.
+
+    Parameters
+    ----------
+    path : (str)
+        Directory containing job.
+    job_script_filename : (str), optional
+        Filename of job script. The default is taken from the key 'filename' in the job_settings in the config file.
+    sort : (str or list), optional
+        Sort list of jobs by features. If False or None jobs are not sorted. The default is 'name'.
+    load_outputs : (bool)
+        Load job outputs. The default is True.
+    jobs_kwargs : (dict), optional
+        Dictionary with job class name as keys and kwargs as values. Kwargs to be used when importing job 
+        from directory for each job class.
+
+    Returns
+    -------
+    jobs : (list)
+        List of Job objects.
+    """    
+    from pynter.vasp.jobs import VaspJob, VaspNEBJob
+    
+    path = path if path else os.getcwd()
+    job_script_filename = job_script_filename if job_script_filename else ScriptHandler().filename
+        
+    for root,dirs,files in os.walk(path):      
+        if all(f in files for f in ['INCAR','KPOINTS','POSCAR','POTCAR']):
+            path = op.abspath(root)
+            if jobs_kwargs:
+                kwargs = jobs_kwargs['VaspJob'] if 'VaspJob' in jobs_kwargs.keys() else {}
+            else:
+                kwargs = {}
+            j = VaspJob.from_directory(path,job_script_filename=job_script_filename,load_outputs=load_outputs,**kwargs)
+            return j
+        elif all(f in files for f in ['INCAR','KPOINTS','POTCAR']) and 'POSCAR' not in files:
+            path = op.abspath(root)
+            j = VaspNEBJob.from_directory(path,job_script_filename=job_script_filename,load_outputs=load_outputs)
+            return j
```

### Comparing `pynter-defects-1.0.0/pynter/defects/analysis.py` & `pynter-defects-1.0.1/pynter/defects/analysis.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/defects/corrections.py` & `pynter-defects-1.0.1/pynter/defects/corrections.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/defects/defects.py` & `pynter-defects-1.0.1/pynter/defects/defects.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/defects/elasticity.py` & `pynter-defects-1.0.1/pynter/defects/elasticity.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/defects/entries.py` & `pynter-defects-1.0.1/pynter/defects/entries.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/defects/plotter.py` & `pynter-defects-1.0.1/pynter/defects/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/defects/pmg/pmg_defects_core.py` & `pynter-defects-1.0.1/pynter/defects/pmg/pmg_defects_core.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/defects/pmg/pmg_defects_corrections.py` & `pynter-defects-1.0.1/pynter/defects/pmg/pmg_defects_corrections.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/defects/pmg/pmg_defects_utils.py` & `pynter-defects-1.0.1/pynter/defects/pmg/pmg_defects_utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/defects/pmg/pmg_dos.py` & `pynter-defects-1.0.1/pynter/defects/pmg/pmg_dos.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/defects/structure.py` & `pynter-defects-1.0.1/pynter/defects/structure.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/defects/thermodynamics.py` & `pynter-defects-1.0.1/pynter/defects/thermodynamics.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/defects/utils.py` & `pynter-defects-1.0.1/pynter/defects/utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/phase_diagram/chempots.py` & `pynter-defects-1.0.1/pynter/phase_diagram/chempots.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/phase_diagram/plotter.py` & `pynter-defects-1.0.1/pynter/phase_diagram/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/phase_diagram/thermodynamics.py` & `pynter-defects-1.0.1/pynter/phase_diagram/thermodynamics.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,16 @@
                 for el in extrinsic_chempots_range:
                     mu_el_O_poor,mu_el_O_rich = extrinsic_chempots_range[el][0], extrinsic_chempots_range[el][1]
                     chempots_abs[el] = mu_el_O_poor + ((mu_el_O_rich - mu_el_O_poor)/npoints)*i 
                         
             if get_pressures_as_strings:
                 p = "%.1g" % p
                 p = str(p)
+            else:
+                p = float("{:.3e}".format(p))
             reservoirs[p] = chempots_abs
     
             
         return PressureReservoirs(reservoirs,temperature,phase_diagram=pd,are_chempots_delta=False)
                                 
 
     def get_oxygen_pressure_reservoirs(self,oxygen_ref,temperature=None,pressure_range=(-20,10),npoints=50,get_pressures_as_strings=False):
@@ -192,14 +194,16 @@
         for p in partial_pressures:
             mu = {}
             muO = self.chempot_ideal_gas(mu_standard,temperature=temperature,partial_pressure=p)
             mu.update({'O':oxygen_ref + muO})
             if get_pressures_as_strings:
                 p = "%.1g" % p
                 p = str(p)
+            else:
+                p = float("{:.3e}".format(p))
             reservoirs[p] = Chempots(mu)
         
         return PressureReservoirs(reservoirs,temperature,phase_diagram=None,
                                   mu_refs=mu_refs,are_chempots_delta=False)
     
     
     def oxygen_standard_chempot(self,temperature=None):
```

### Comparing `pynter-defects-1.0.0/pynter/slurm/interface.py` & `pynter-defects-1.0.1/pynter/slurm/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         if dry_run:
             cmd += "--dry-run "
         if exclude:
             for s in exclude:
                 cmd += f'--exclude={s} ' 
         cmd += f"-e ssh {self.hostname}:{remotedir} {localdir} "
 
-        stdout,stderr = run_local(cmd,printout,dry_run=False,**kwargs)
+        stdout,stderr = run_local(cmd,printout=printout,dry_run=False,**kwargs)
         return stdout,stderr
 
 
     def rsync_to_hpc(self,localdir=None,remotedir=None,exclude=None,printout=True,dry_run=False,**kwargs):
         """
         Sync folders from local machine to HPC. The command "rsync" is used. With this function all
         the folders contained in the local dir are synched to the remote dir.
@@ -226,15 +226,15 @@
         if dry_run:
             cmd += "--dry-run "
         if exclude:
             for s in exclude:
                 cmd += f'--exclude={s} '
         cmd += f"-e ssh  {localdir} {self.hostname}:{remotedir} "
         
-        stdout,stderr = run_local(cmd,printout,dry_run=False,**kwargs)
+        stdout,stderr = run_local(cmd,printout=printout,dry_run=False,**kwargs)
 
         return stdout,stderr
     
           
     def sbatch(self,path='',job_script_filename='job.sh',printout=True,dry_run=False,**kwargs):
         """
         Execute "sbatch" command on HPC to run job.
```

### Comparing `pynter-defects-1.0.0/pynter/slurm/job_script.py` & `pynter-defects-1.0.1/pynter/slurm/job_script.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         f.append('\n')
         f.append('srun %s\n' %self.path_exe)
 
         automation_written = False
         if self.array_size:
             if self.add_stop_array:
                 f.append('\n')
-                f.append('convergence.py > convergence.txt\n')
+                f.append('pynter analysis vasprun --convergence > convergence.txt\n')
                 f.append("if  grep -q 'Electronic convergence: True' convergence.txt  = true  && grep -q 'Ionic convergence: True' convergence.txt  = true; then\n")
                 if self.add_automation:
                     f.append('    %s\n' %self.add_automation) # KEEP THE TAB!
                     automation_written = True
                 f.append('    scancel ${SLURM_ARRAY_JOB_ID}_*\n') #KEEP THE TAB!
                 f.append('fi\n')
         if self.add_automation and automation_written is False:
```

### Comparing `pynter-defects-1.0.0/pynter/slurm/job_status.py` & `pynter-defects-1.0.1/pynter/slurm/job_status.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/tools/format.py` & `pynter-defects-1.0.1/pynter/tools/format.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/tools/materials_project.py` & `pynter-defects-1.0.1/pynter/tools/materials_project.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/tools/structure.py` & `pynter-defects-1.0.1/pynter/tools/structure.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/tools/utils.py` & `pynter-defects-1.0.1/pynter/tools/utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/vasp/__init__.py` & `pynter-defects-1.0.1/pynter/vasp/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,9 +24,9 @@
     (dict)
         Configuration dictionary.
     """
     if os.path.exists(cfgfile):
         with open(cfgfile,"r") as ymlfile:
             return yaml.load(ymlfile,Loader=yaml.FullLoader) # add Loader to not get warning
     else:
-        raise FileNotFoundError('%s does not exist. Run the setup.py script to create it.'%cfgfile)
+        raise FileNotFoundError('%s does not exist. Run "pynter configure" in the terminal to create it.'%cfgfile)
         return
```

### Comparing `pynter-defects-1.0.0/pynter/vasp/analysis.py` & `pynter-defects-1.0.1/pynter/vasp/analysis.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/vasp/default_inputs.py` & `pynter-defects-1.0.1/pynter/vasp/default_inputs.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/vasp/jobs.py` & `pynter-defects-1.0.1/pynter/vasp/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,16 @@
 
         Parameters
         ----------
         path : (str)
             Path were job data is stored. If None the current wdir is used. The default is None.
         job_script_filename : (str), optional
             Filename of job script. The default is set in the config file.
+        load_outputs : (bool)
+            Load job outputs. The default is True.
         kwargs : (dict)
             Arguments to pass to Vasprun parser.
         Returns
         -------
         VaspJob object.
         
         """
@@ -152,15 +154,16 @@
                     warnings.warn('Reading of vasprun.xml in "%s" failed'%path)
                     outputs['Vasprun'] = None
         
         job_script_filename = job_script_filename if job_script_filename else ScriptHandler().filename
         s = ScriptHandler.from_file(path,filename=job_script_filename)
         job_settings =  s.settings
         
-        return VaspJob(path,inputs,job_settings,outputs,job_script_filename)
+        return VaspJob(path=path,inputs=inputs,job_settings=job_settings,
+                       outputs=outputs,job_script_filename=job_script_filename)
 
 
     @staticmethod
     def from_json(path_or_string):
         """
         Build VaspJob object from json file or string.
 
@@ -671,14 +674,16 @@
 
         Parameters
         ----------
         path : (str)
             Path were job data is stored. If None the current wdir is used. The default is None.
         job_script_filename : (str), optional
             Filename of job script. The default is set in the config file.
+        load_outputs : (bool)
+            Load job outputs. The default is True.
 
         Returns
         -------
         VaspNEBJob object.
         
         """                
         inputs = {}
@@ -706,15 +711,16 @@
                 warnings.warn('NEB output reading with NEBAnalysis in "%s" failed'%path)
                 outputs['NEBAnalysis'] = None
         
         job_script_filename = job_script_filename if job_script_filename else ScriptHandler().filename
         s = ScriptHandler.from_file(path,filename=job_script_filename)
         job_settings =  s.settings
         
-        return VaspNEBJob(path,inputs,job_settings,outputs,job_script_filename)
+        return VaspNEBJob(path=path,inputs=inputs,job_settings=job_settings,
+                       outputs=outputs,job_script_filename=job_script_filename)
 
 
     @staticmethod
     def from_json(path_or_string):
         """
         Build VaspJob object from json file or string.
         Parameters
```

### Comparing `pynter-defects-1.0.0/pynter/vasp/plotter.py` & `pynter-defects-1.0.1/pynter/vasp/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/vasp/pmg/pmg_electronic_structure_plotter.py` & `pynter-defects-1.0.1/pynter/vasp/pmg/pmg_electronic_structure_plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/vasp/schemes.py` & `pynter-defects-1.0.1/pynter/vasp/schemes.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter/vasp/utils.py` & `pynter-defects-1.0.1/pynter/vasp/utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.0/pynter_defects.egg-info/SOURCES.txt` & `pynter-defects-1.0.1/pynter_defects.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -40,14 +40,22 @@
 pynter/phase_diagram/chempots.py
 pynter/phase_diagram/plotter.py
 pynter/phase_diagram/thermodynamics.py
 pynter/slurm/__init__.py
 pynter/slurm/interface.py
 pynter/slurm/job_script.py
 pynter/slurm/job_status.py
+pynter/testing/__init__.py
+pynter/testing/core.py
+pynter/testing/data.py
+pynter/testing/defects.py
+pynter/testing/phase_diagram.py
+pynter/testing/slurm.py
+pynter/testing/structure.py
+pynter/testing/vasp.py
 pynter/tools/__init__.py
 pynter/tools/format.py
 pynter/tools/materials_project.py
 pynter/tools/plotter.py
 pynter/tools/structure.py
 pynter/tools/utils.py
 pynter/vasp/__init__.py
```

### Comparing `pynter-defects-1.0.0/setup.py` & `pynter-defects-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,37 +3,28 @@
 """
 Created on Thu May 25 14:39:37 2023
 
 @author: villa
 """
 
 from setuptools import setup, find_namespace_packages
-import atexit
-
-from pynter.cli.config import run_config
-
-def post_install():
-    print("\nRunning configuration setup\n")
-    run_config(None)
-    return
 
 setup(
     name='pynter-defects',
-    version='1.0.0',
+    version='1.0.1',
     author='Lorenzo Villa',
     description='Tools for atomistic calculations',
-    packages=find_namespace_packages(exclude=["pynter.tests","pynter.*.tests", "pynter.*.*.tests"]),
+    packages=find_namespace_packages(exclude=["pynter.*.tests", "pynter.*.*.tests"]),
     install_requires=[
         'ase',
         'pymatgen>=2023.3.23',
         'pymatgen-analysis-defects>=2023.3.25',
         'pymatgen-db',
         'PyYAML',
         'schedule'        
     ],
     extra_requires={'test':'pytest'},
     entry_points={
     "console_scripts": [
         "pynter = pynter.cli.main:main"]}
 )
 
-#atexit.register(post_install)
```

