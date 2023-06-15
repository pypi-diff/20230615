# Comparing `tmp/ratingcurve-0.3.4.tar.gz` & `tmp/ratingcurve-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratingcurve-0.3.4.tar", last modified: Tue Feb 28 04:39:24 2023, max compression
+gzip compressed data, was "ratingcurve-0.3.5.tar", last modified: Thu Jun 15 15:28:57 2023, max compression
```

## Comparing `ratingcurve-0.3.4.tar` & `ratingcurve-0.3.5.tar`

### file list

```diff
@@ -1,55 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 04:39:24.478833 ratingcurve-0.3.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 04:39:24.474833 ratingcurve-0.3.4/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/.devcontainer/noop.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 04:39:24.470833 ratingcurve-0.3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 04:39:24.474833 ratingcurve-0.3.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/.github/ISSUE_TEMPLATE/review-checklist.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 04:39:24.474833 ratingcurve-0.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/DISCLAIMER.md
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-02-28 04:39:24.478833 ratingcurve-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/code.json
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 04:39:24.474833 ratingcurve-0.3.4/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    55033 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/notebooks/model-evaluation-demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   135158 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/notebooks/segmented-power-law-demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    92747 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/notebooks/spline-demo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 04:39:24.474833 ratingcurve-0.3.4/paper/
--rw-r--r--   0 runner    (1001) docker     (123)    22818 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/paper/green_example.png
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 04:39:24.474833 ratingcurve-0.3.4/ratingcurve/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/ratingcurve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-28 04:39:24.000000 ratingcurve-0.3.4/ratingcurve/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 04:39:24.474833 ratingcurve-0.3.4/ratingcurve/data/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/ratingcurve/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/ratingcurve/data/chalk_artificial.csv
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/ratingcurve/data/co_channel.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/ratingcurve/data/green_channel.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/ratingcurve/data/provo_natural.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/ratingcurve/data/simulated_rating.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/ratingcurve/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/ratingcurve/ratingmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 04:39:24.478833 ratingcurve-0.3.4/ratingcurve/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/ratingcurve/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/ratingcurve/tests/test_ratingmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/ratingcurve/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/ratingcurve/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 04:39:24.474833 ratingcurve-0.3.4/ratingcurve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-02-28 04:39:24.000000 ratingcurve-0.3.4/ratingcurve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-02-28 04:39:24.000000 ratingcurve-0.3.4/ratingcurve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 04:39:24.000000 ratingcurve-0.3.4/ratingcurve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-28 04:39:24.000000 ratingcurve-0.3.4/ratingcurve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-28 04:39:24.000000 ratingcurve-0.3.4/ratingcurve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 04:39:24.478833 ratingcurve-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-28 04:39:08.000000 ratingcurve-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:28:57.678301 ratingcurve-0.3.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:28:57.670300 ratingcurve-0.3.5/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/.devcontainer/noop.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:28:57.666300 ratingcurve-0.3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:28:57.670300 ratingcurve-0.3.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/.github/ISSUE_TEMPLATE/review-checklist.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:28:57.670300 ratingcurve-0.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/.github/workflows/deploy-book.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/DISCLAIMER.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-06-15 15:28:57.678301 ratingcurve-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/code.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:28:57.670300 ratingcurve-0.3.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/docs/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/docs/_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/docs/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:28:57.670300 ratingcurve-0.3.5/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    29183 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/docs/assets/green-channel-rating-plot.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:28:57.674301 ratingcurve-0.3.5/docs/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/docs/meta/background.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/docs/meta/implementation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/docs/meta/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/docs/meta/intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/docs/meta/troubleshooting.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/docs/meta/tutorials.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:28:57.674301 ratingcurve-0.3.5/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/docs/notebooks/getting-started-tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/docs/notebooks/model-selection-tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    94061 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/docs/notebooks/segmented-power-law-tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/docs/notebooks/spline-tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/docs/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/docs/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:28:57.674301 ratingcurve-0.3.5/ratingcurve/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/ratingcurve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-15 15:28:57.000000 ratingcurve-0.3.5/ratingcurve/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:28:57.678301 ratingcurve-0.3.5/ratingcurve/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/ratingcurve/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/ratingcurve/data/chalk_artificial.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/ratingcurve/data/chalk_artificial.md
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/ratingcurve/data/co_channel.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/ratingcurve/data/co_channel.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/ratingcurve/data/green_channel.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/ratingcurve/data/green_channel.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/ratingcurve/data/provo_natural.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/ratingcurve/data/provo_natural.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/ratingcurve/data/simulated_rating.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/ratingcurve/data/simulated_rating.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/ratingcurve/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/ratingcurve/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16305 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/ratingcurve/ratingmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/ratingcurve/sklearn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:28:57.678301 ratingcurve-0.3.5/ratingcurve/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/ratingcurve/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/ratingcurve/tests/test_ratingmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/ratingcurve/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/ratingcurve/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:28:57.674301 ratingcurve-0.3.5/ratingcurve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-06-15 15:28:57.000000 ratingcurve-0.3.5/ratingcurve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-15 15:28:57.000000 ratingcurve-0.3.5/ratingcurve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:28:57.000000 ratingcurve-0.3.5/ratingcurve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-15 15:28:57.000000 ratingcurve-0.3.5/ratingcurve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 15:28:57.000000 ratingcurve-0.3.5/ratingcurve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 15:28:57.678301 ratingcurve-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 15:28:35.000000 ratingcurve-0.3.5/setup.py
```

### Comparing `ratingcurve-0.3.4/.devcontainer/Dockerfile` & `ratingcurve-0.3.5/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `ratingcurve-0.3.4/.devcontainer/devcontainer.json` & `ratingcurve-0.3.5/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ratingcurve-0.3.4/.github/ISSUE_TEMPLATE/feature_request.md` & `ratingcurve-0.3.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-0.3.4/.github/ISSUE_TEMPLATE/review-checklist.md` & `ratingcurve-0.3.5/.github/ISSUE_TEMPLATE/review-checklist.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-0.3.4/.github/workflows/python-package.yml` & `ratingcurve-0.3.5/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `ratingcurve-0.3.4/.github/workflows/python-publish.yml` & `ratingcurve-0.3.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ratingcurve-0.3.4/.gitignore` & `ratingcurve-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ratingcurve-0.3.4/CONTRIBUTING.md` & `ratingcurve-0.3.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-0.3.4/DISCLAIMER.md` & `ratingcurve-0.3.5/DISCLAIMER.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-0.3.4/LICENSE.md` & `ratingcurve-0.3.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-0.3.4/PKG-INFO` & `ratingcurve-0.3.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratingcurve
-Version: 0.3.4
+Version: 0.3.5
 Summary: A library for fitting multi-segment stage-discharge rating curves.
 Maintainer-email: Timothy Hodson <thodson@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, this project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -56,75 +56,63 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
 
 # ratingcurve
-*A Python library for fitting stage-discharge rating curves.*
+*A Python library for fitting hydrologic rating curves.*
 
-Use `ratingcurve` to fit streamflow ratings with a segmented power law,
-which is the the most common model used by USGS.
-
-At this time, the library is for research and is not ready for operation. 
+In hydrology, a rating curve is a mathematical relationship between streamflow and water surface elevation (stage).
+Because stage is much easier to measure than streamflow, almost all streamflow timeseries are generated from rating curves.
+Historically, those ratings were fitted by hand, which can be time consuming and error prone.
+`ratingcurve` provides an easy-to-use algorithm for fitting the standard form of rating curve, the segmented power law.
 
 ## Installation
 Install using pip
 ```sh
 pip install ratingcurve
 ```
 or conda
 ```sh
-# acreate a new environment
-conda create -n ratingcurve
-conda activate ratingcurve
 conda install -c conda-forge ratingcurve
-# add environment to jupyter
-python -m ipykernel install --user --name=ratingcurve
 ```
 
 ## Getting Started
-The [`segmented-power-law-demo.ipynb`](https://github.com/thodson-usgs/ratingcurve/blob/main/notebooks/segmented-power-law-demo.ipynb)
-notebook demonstrates basic use of the package.
-You can try it out in Google Colab
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/thodson-usgs/ratingcurve/blob/master/notebooks/segmented-power-law-demo.ipynb)
-
-or locally using the environment created in the previous step
-```sh
-conda activate base # or your prefered jupyter lab environment
-jupyter lab
-```
-then open the notebook and select the `ratingcurve` kernel that was installed earlier.
-
-A simple example is given below.
+This [`tutorial`](https://github.com/thodson-usgs/ratingcurve/blob/main/docs/notebooks/segmented-power-law-tutorial.ipynb)
+notebook demonstrates basic usage of the package.
+Try it locally or in Colab.
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/thodson-usgs/ratingcurve/blob/main/docs/notebooks/segmented-power-law-tutorial.ipynb)
 
 ```python
 from ratingcurve.ratingmodel import PowerLawRating
 from ratingcurve import data
 
 # load tutorial data
 df = data.load('green channel')
 
-# setup model
-segments = 2
+# initialize the model
 powerrating = PowerLawRating(q=df['q'],
                              h=df['stage'], 
                              q_sigma=df['q_sigma'],
-                             segments=segments)
+                             segments=2)
                                    
-# fit model, then simulate the rating
-with powerrating:
-    mean_field = pm.fit(n=150_000)
-    trace = mean_field.sample(5000)
-    
+# fit the model
+trace = powerrating.fit()
 powerrating.plot(trace)
 ```
-![example plot](https://github.com/thodson-usgs/ratingcurve/blob/main/paper/green_example.png?raw=true)
+![example plot](https://github.com/thodson-usgs/ratingcurve/blob/main/docs/assets/green-channel-rating-plot.png?raw=true)
+
+
+Generate a rating table that can be imported into other applications.
+```python
+powerating.table(trace)
+```
 
-See the [notebooks](https://github.com/thodson-usgs/ratingcurve/tree/main/notebooks) for more examples.
+For more, see the [documentation](https://thodson-usgs.github.io/ratingcurve/meta/intro.html).
 
 ## Disclaimer
 
 This software is preliminary or provisional and is subject to revision. 
 It is being provided to meet the need for timely best science.
 The software has not received final approval by the U.S. Geological Survey (USGS).
 No warranty, expressed or implied, is made by the USGS or the U.S. Government as to the functionality of the software and related material nor shall the fact of release constitute any such warranty.
```

### Comparing `ratingcurve-0.3.4/README.md` & `ratingcurve-0.3.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,57 @@
 # ratingcurve
-*A Python library for fitting stage-discharge rating curves.*
+*A Python library for fitting hydrologic rating curves.*
 
-Use `ratingcurve` to fit streamflow ratings with a segmented power law,
-which is the the most common model used by USGS.
-
-At this time, the library is for research and is not ready for operation. 
+In hydrology, a rating curve is a mathematical relationship between streamflow and water surface elevation (stage).
+Because stage is much easier to measure than streamflow, almost all streamflow timeseries are generated from rating curves.
+Historically, those ratings were fitted by hand, which can be time consuming and error prone.
+`ratingcurve` provides an easy-to-use algorithm for fitting the standard form of rating curve, the segmented power law.
 
 ## Installation
 Install using pip
 ```sh
 pip install ratingcurve
 ```
 or conda
 ```sh
-# acreate a new environment
-conda create -n ratingcurve
-conda activate ratingcurve
 conda install -c conda-forge ratingcurve
-# add environment to jupyter
-python -m ipykernel install --user --name=ratingcurve
 ```
 
 ## Getting Started
-The [`segmented-power-law-demo.ipynb`](https://github.com/thodson-usgs/ratingcurve/blob/main/notebooks/segmented-power-law-demo.ipynb)
-notebook demonstrates basic use of the package.
-You can try it out in Google Colab
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/thodson-usgs/ratingcurve/blob/master/notebooks/segmented-power-law-demo.ipynb)
-
-or locally using the environment created in the previous step
-```sh
-conda activate base # or your prefered jupyter lab environment
-jupyter lab
-```
-then open the notebook and select the `ratingcurve` kernel that was installed earlier.
-
-A simple example is given below.
+This [`tutorial`](https://github.com/thodson-usgs/ratingcurve/blob/main/docs/notebooks/segmented-power-law-tutorial.ipynb)
+notebook demonstrates basic usage of the package.
+Try it locally or in Colab.
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/thodson-usgs/ratingcurve/blob/main/docs/notebooks/segmented-power-law-tutorial.ipynb)
 
 ```python
 from ratingcurve.ratingmodel import PowerLawRating
 from ratingcurve import data
 
 # load tutorial data
 df = data.load('green channel')
 
-# setup model
-segments = 2
+# initialize the model
 powerrating = PowerLawRating(q=df['q'],
                              h=df['stage'], 
                              q_sigma=df['q_sigma'],
-                             segments=segments)
+                             segments=2)
                                    
-# fit model, then simulate the rating
-with powerrating:
-    mean_field = pm.fit(n=150_000)
-    trace = mean_field.sample(5000)
-    
+# fit the model
+trace = powerrating.fit()
 powerrating.plot(trace)
 ```
-![example plot](https://github.com/thodson-usgs/ratingcurve/blob/main/paper/green_example.png?raw=true)
+![example plot](https://github.com/thodson-usgs/ratingcurve/blob/main/docs/assets/green-channel-rating-plot.png?raw=true)
+
+
+Generate a rating table that can be imported into other applications.
+```python
+powerating.table(trace)
+```
 
-See the [notebooks](https://github.com/thodson-usgs/ratingcurve/tree/main/notebooks) for more examples.
+For more, see the [documentation](https://thodson-usgs.github.io/ratingcurve/meta/intro.html).
 
 ## Disclaimer
 
 This software is preliminary or provisional and is subject to revision. 
 It is being provided to meet the need for timely best science.
 The software has not received final approval by the U.S. Geological Survey (USGS).
 No warranty, expressed or implied, is made by the USGS or the U.S. Government as to the functionality of the software and related material nor shall the fact of release constitute any such warranty.
```

### Comparing `ratingcurve-0.3.4/code.json` & `ratingcurve-0.3.5/code.json`

 * *Files identical despite different names*

### Comparing `ratingcurve-0.3.4/notebooks/segmented-power-law-demo.ipynb` & `ratingcurve-0.3.5/docs/notebooks/segmented-power-law-tutorial.ipynb`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7609515477740576%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Segmented Power Law\\n'), (1, '[![Open In "*

 * *            'Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/thodson-usgs/ratingcurve/blob/main/docs/notebooks/segmented-power-law-demo.ipynb)  '*

 * *            "\\n'), (4, 'This notebook demonstrates an simple way to approximate the classic "*

 * *            "approach, \\n'), (5, 'which uses a segmented power law.')], delete: [5, 4, 1, 0]}, "*

 * *            "delete: ['id […]*

```diff
@@ -1,109 +1,65 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "6383be96-4086-48dd-bad4-6a59e5b1398d",
             "metadata": {},
             "source": [
-                "# Fitting a Stage-Discharge Rating using a Segmented\n",
-                "[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/thodson-usgs/ratingcurve/blob/master/notebooks/segmented-power-law-demo.ipynb)  \n",
+                "# Segmented Power Law\n",
+                "[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/thodson-usgs/ratingcurve/blob/main/docs/notebooks/segmented-power-law-demo.ipynb)  \n",
                 "\n",
                 "There are several approaches to fitting a stage-discharge rating curve. \n",
-                "The first section of this notebook demonstrates the classic approach, \n",
-                "which is to use a segmented power law."
+                "This notebook demonstrates an simple way to approximate the classic approach, \n",
+                "which uses a segmented power law."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
-            "id": "d23da995-0d8c-4df5-bceb-f9ea29c5034d",
             "metadata": {
                 "id": "d23da995-0d8c-4df5-bceb-f9ea29c5034d"
             },
             "outputs": [],
             "source": [
-                "# # Only run this cell to setup Google Colab. It will take a minute.\n",
+                "# Uncomment below to setup Google Colab. It will take a minute or so.\n",
                 "# %%capture\n",
-                "# # Specific repo version used in this notebook\n",
-                "# !pip install pymc==5.0.2\n",
-                "#\n",
-                "# # Colab needs this\n",
+                "# !pip install pymc==5.1.2\n",
                 "# %env MKL_THREADING_LAYER=GNU\n",
-                "#\n",
-                "# # install ratingcurve library\n",
                 "# !pip install git+https://github.com/thodson-usgs/ratingcurve.git"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
-            "id": "806409d6-616f-4ecf-a2a7-e5e42744c686",
             "metadata": {
                 "id": "806409d6-616f-4ecf-a2a7-e5e42744c686"
             },
             "outputs": [],
             "source": [
                 "%load_ext autoreload\n",
                 "%autoreload 2\n",
                 "\n",
                 "import pymc as pm\n",
                 "import arviz as az\n",
-                "from ratingcurve.ratingmodel import PowerLawRating, SplineRating"
+                "from ratingcurve.ratingmodel import PowerLawRating"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "20cebce1-1a16-4367-ab86-2d42147a0437",
             "metadata": {
                 "id": "68990119-0f7d-4033-8968-0361b655647a"
             },
             "source": [
-                "## Load Data"
+                "## Load Data\n",
+                "Begin by loading the Green Channel dataset"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
-            "id": "5d481ab2-d42c-4fb3-baeb-460a20ee19fd",
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "['chalk artificial',\n",
-                            " 'co channel',\n",
-                            " 'green channel',\n",
-                            " 'provo natural',\n",
-                            " '3-segment simulated']"
-                        ]
-                    },
-                    "execution_count": 3,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "# load tutorial data\n",
-                "from ratingcurve import data\n",
-                "data.list()"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "96106967-41ff-4189-a751-47b34966147b",
-            "metadata": {},
-            "source": [
-                "and load a specific dataset."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 4,
-            "id": "9a75a0ac-877b-4b19-8b33-236b1a629875",
             "metadata": {
                 "id": "9a75a0ac-877b-4b19-8b33-236b1a629875"
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
@@ -176,73 +132,78 @@
                             "0  2020-05-21 14:13:41 [UTC-07:00]   7.04  12199.342  199.172931\n",
                             "1  2020-04-16 14:55:31 [UTC-07:00]   4.43   4921.953   95.425619\n",
                             "2  2020-03-04 13:54:10 [UTC-07:00]   2.99   2331.665   61.860500\n",
                             "3  2020-03-04 13:16:51 [UTC-07:00]   2.94   2289.220   47.886745\n",
                             "4  2020-01-23 11:04:32 [UTC-07:00]   2.96   2408.210   99.522964"
                         ]
                     },
-                    "execution_count": 4,
+                    "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
+                "from ratingcurve import data\n",
                 "df = data.load('green channel')\n",
                 "df.head()"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "and plotting the observations"
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": 5,
-            "id": "4a60c122-9214-4100-a2f2-aae7d89d7dc3",
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "Text(0, 0.5, 'Stage (ft)')"
                         ]
                     },
-                    "execution_count": 5,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAjgAAAGwCAYAAACkfh/eAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy88F64QAAAACXBIWXMAAA9hAAAPYQGoP6dpAAAzQElEQVR4nO3deXhV1b3/8c8hhIRMBzIRIoEEE0EN0kAAkRrECVAGr0MVaQvVOrRCtOitpNpHrlO011ILWr2iBakl2l5EaZWqLUMYKxJyAdEQzAAiKZlDCCaQrN8f/jjlSBLOIckZdt6v5znPw1l77XO+Wd31fJ6919rbZowxAgAAsJAe3i4AAACgsxFwAACA5RBwAACA5RBwAACA5RBwAACA5RBwAACA5RBwAACA5fT0dgFdraWlRV999ZXCw8Nls9m8XQ4AAHCBMUZHjx5VfHy8evRw/3yM5QPOV199pYSEBG+XAQAAzsHBgwc1YMAAt/ezfMAJDw+X9M0ARUREeLkaAADgirq6OiUkJDh+x91l+YBz6rJUREQEAQcAAD9zrtNLmGQMAAAsh4ADAAAsh4ADAAAsh4ADAAAsh4ADAAAsh4ADAAAsh4ADAAAsh4ADAAAsh4ADAAAsh4ADAAAsx/KPagAAAF2jqLxepVUNSowKVVJ0qLfLcULAAQAAbqlpaFJmTr5yC8sdbRkpMVo8I032kEAvVvZvXKICAABuyczJ1+b9FU5tm/dXaG7OTi9VdCYCDgAAcFlReb1yC8vVbIxTe7Mxyi0sV3HFMS9V5oyAAwAAXFZa1dDu9pJKAg4AAPAzgyJD2t2eGOUbk40JOAAAwGWDY8KUkRKjAJvNqT3AZlNGSozPrKYi4AAAALcsnpGmccnRTm3jkqO1eEaalyo6E8vEAQCAW+whgVp+52gVVxxTSeUx7oMDAACsIyna94LNKVyiAgAAluPVgJObm6upU6cqPj5eNptN77zzjmPbiRMn9PDDD2vYsGEKDQ1VfHy8fvjDH+qrr77yXsEAAMAveDXgHDt2TMOHD9cLL7xwxraGhgbl5eXpl7/8pfLy8vT2229r3759mjZtmhcqBQAA/sRmzLduReglNptNq1at0g033NBmn+3bt2v06NEqLS3VwIEDXfrcuro62e121dbWKiIiopOqBQAAXamjv99+Ncm4trZWNptNffr0abNPY2OjGhsbHe/r6uo8UBkAAPAlfjPJ+Ouvv9b8+fN1++23t5vksrOzZbfbHa+EhAQPVgkAAHyBXwScEydO6LbbblNLS4t+97vftds3KytLtbW1jtfBgwc9VCUAAPAVPn+J6sSJE/re976n4uJirV279qzX4YKCghQUFOSh6gAAgC/y6YBzKtwUFhZq3bp1ioqK8nZJAADAD3g14NTX12v//v2O98XFxcrPz1dkZKTi4+N18803Ky8vT3/961/V3NyssrIySVJkZKR69erlrbIBAICP8+oy8fXr12vChAlntM+aNUsLFixQUlJSq/utW7dOV1xxhUvfwTJxAAD8j18vE7/iiivUXr7ykVv0AAAAP+MXq6gAAADcQcABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACWQ8ABAACW49WAk5ubq6lTpyo+Pl42m03vvPOO03ZjjBYsWKD4+Hj17t1bV1xxhT799FPvFAsAAPyGVwPOsWPHNHz4cL3wwgutbv/Vr36lhQsX6oUXXtD27dsVFxena665RkePHvVwpQAAwJ/09OaXT548WZMnT251mzFGzz//vB555BHdeOONkqTXX39d/fr104oVK3TPPfd4slQAAOBHfHYOTnFxscrKynTttdc62oKCgjR+/Hht2bKlzf0aGxtVV1fn9AIAAN2LzwacsrIySVK/fv2c2vv16+fY1prs7GzZ7XbHKyEhoUvrBAAAvsdnA84pNpvN6b0x5oy202VlZam2ttbxOnjwYFeXCAAAfIxX5+C0Jy4uTtI3Z3L69+/vaD9y5MgZZ3VOFxQUpKCgoC6vDwAA+C6fPYOTlJSkuLg4ffTRR462pqYmbdiwQZdddpkXKwMAAL7Oq2dw6uvrtX//fsf74uJi5efnKzIyUgMHDtQDDzygp59+WikpKUpJSdHTTz+tkJAQ3X777V6sGgAA+DqvBpxPPvlEEyZMcLyfN2+eJGnWrFlatmyZfv7zn+v48eP66U9/qurqao0ZM0YffvihwsPDvVUyAADwAzZjjPF2EV2prq5OdrtdtbW1ioiI8HY5AADABR39/fbZOTgAAADnioADAAAsx2eXiQMAOkdReb1KqxqUGBWqpOhQb5cDeAQBBwAsqqahSZk5+cotLHe0ZaTEaPGMNNlDAr1YGdD1uEQFABaVmZOvzfsrnNo276/Q3JydXqoI8BwCDgBYUFF5vXILy9X8rYWyzcYot7BcxRXHvFQZ4BkEHACwoNKqhna3l1QScGBtBBwAsKBBkSHtbk+MYrIxrI2AAwAWNDgmTBkpMQqw2ZzaA2w2ZaTEsJoKlkfAAQCLWjwjTeOSo53axiVHa/GMNC9VBHgOy8QBwKLsIYFafudoFVccU0nlMe6Dg26FgAMAFpcUTbBB98MlKgAAYDkEHAAAYDkEHAAAYDkEHAAAYDkEHAAAYDkEHAAAYDkEHAAAYDkEHAAAYDkEHAAAYDkEHAAAYDkEHAAAYDk8iwoAvKSovF6lVQ08BBPoAgQcAPCwmoYmZebkK7ew3NGWkRKjxTPSZA8J9GJlgHVwiQoAPCwzJ1+b91c4tW3eX6G5OTu9VBFgPQQcAPCgovJ65RaWq9kYp/ZmY5RbWK7iimNeqgywFgIOAHhQaVVDu9tLKgk4QGcg4ACABw2KDGl3e2IUk42BzkDAAQAPGhwTpoyUGAXYbE7tATabMlJiWE0FdBICDgB42OIZaRqXHO3UNi45WotnpHmpIsB6WCYOAB5mDwnU8jtHq7jimEoqj3EfHKALEHAAwEuSogk2QFfhEhUAALAcAg4AALAcAg4AALAcAg4AALAcAg4AALAcAg4AALAcAg4AALAcAg4AALAcAg4AALAcAg4AALAcAg4AALAcAg4AALAcAg4AALAcAg4AALAcAg4AALAcAg4AALAcAg4AALAcAg4AALAcAg4AALAcAg4AALAcAg4AALCcnu7uUFJSoo0bN6qkpEQNDQ2KiYlRWlqaxo4dq+Dg4K6oEQAAwC0uB5wVK1Zo0aJF+vjjjxUbG6vzzjtPvXv3VlVVlb744gsFBwdr5syZevjhhzVo0KCurBkAAKBdLl2iGjFihBYuXKjvf//7KikpUVlZmXbs2KFNmzZp7969qqur07vvvquWlhalp6frz3/+c6cUd/LkST366KNKSkpS7969NXjwYD3++ONqaWnplM8HAADW5NIZnCeeeELXX399m9uDgoJ0xRVX6IorrtCTTz6p4uLiTinu2Wef1csvv6zXX39dF198sT755BP96Ec/kt1u1/33398p3wEAAKzHpYDTXrj5tujoaEVHR59zQafbunWrpk+f7vj+xMRE5eTk6JNPPmlzn8bGRjU2Njre19XVdUotAADAf7i9iiogIEBHjhw5o72yslIBAQGdUtQp3/3ud/WPf/xD+/btkyT93//9nzZt2qTrrruuzX2ys7Nlt9sdr4SEhE6tCQAA+D63V1EZY1ptb2xsVK9evTpc0Okefvhh1dbWaujQoQoICFBzc7OeeuopzZgxo819srKyNG/ePMf7uro6Qg4AAN2MywFn0aJFkiSbzaZXX31VYWFhjm3Nzc3Kzc3V0KFDO7W4t956S2+88YZWrFihiy++WPn5+XrggQcUHx+vWbNmtbpPUFCQgoKCOrUOAADgX2ymrVMy35KUlCRJKi0t1YABA5wuR/Xq1UuJiYl6/PHHNWbMmE4rLiEhQfPnz9d9993naHvyySf1xhtv6PPPP3fpM+rq6mS321VbW6uIiIhOqw0AAHSdjv5+u3QGZ/Xq1SooKFCvXr00YcIEvf322+rbt6/bX+auhoYG9ejhPE0oICCAZeIAAKBdLgWc//iP/1BZWZliYmKUm5urEydOdHVdkqSpU6fqqaee0sCBA3XxxRdr586dWrhwoe644w6PfD8AAPBPLq2iiomJ0bZt2yR9M8nYZrN1aVGnLF68WDfffLN++tOf6sILL9RDDz2ke+65R0888YRHvh8AAPgnl+bgLFiwQI8//rhLwaa5ublTCusszMEBAMD/eGQOzoIFC3Tbbbdp//79mjZtmpYuXao+ffq4/WUAAACe4PIy8aFDh2ro0KF67LHHdMsttygkJKQr6wIAADhnLi8T91dcogIAwP909PfbpUnGkyZN0pYtW87a7+jRo3r22Wf14osvul0IAABAZ3HpEtUtt9yi733vewoPD9e0adOUnp6u+Ph4BQcHq7q6Wnv3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L5vNpnfeecdpuyfH68CBA5o6dapCQ0MVHR2tzMxMNTU1dcWf3WnONn6zZ88+43i89NJLnfp05/HLzs7WqFGjFB4ertjYWN1www0qKChw6sMx2DpXxo7jr20vvfSSLrnkEsdN+caOHas1a9Y4tvvlcWcs6s033zSBgYFmyZIlZu/eveb+++83oaGhprS01NuledRjjz1mLr74YnP48GHH68iRI47tzzzzjAkPDzcrV640u3fvNrfeeqvp37+/qaurc/S59957zXnnnWc++ugjk5eXZyZMmGCGDx9uTp486egzadIkk5qaarZs2WK2bNliUlNTzZQpUzz6t3aG999/3zzyyCNm5cqVRpJZtWqV03ZPjdfJkydNamqqmTBhgsnLyzMfffSRiY+PN3PmzOnyMeiIs43frFmzzKRJk5yOx8rKSqc+3Xn8Jk6caJYuXWr27Nlj8vPzzfXXX28GDhxo6uvrHX04Blvnythx/LVt9erV5r333jMFBQWmoKDA/OIXvzCBgYFmz549xhj/PO4sG3BGjx5t7r33Xqe2oUOHmvnz53upIu947LHHzPDhw1vd1tLSYuLi4swzzzzjaPv666+N3W43L7/8sjHGmJqaGhMYGGjefPNNR59Dhw6ZHj16mL/97W/GGGP27t1rJJlt27Y5+mzdutVIMp9//nkX/FWe8e0faE+O1/vvv2969OhhDh065OiTk5NjgoKCTG1tbZf8vZ2trYAzffr0Nvdh/JwdOXLESDIbNmwwxnAMuuPbY2cMx5+7+vbta1599VW/Pe4seYmqqalJO3bs0LXXXuvUfu2112rLli1eqsp7CgsLFR8fr6SkJN12220qKiqSJBUXF6usrMxpnIKCgjR+/HjHOO3YsUMnTpxw6hMfH6/U1FRHn61bt8put2vMmDGOPpdeeqnsdrulxtuT47V161alpqY6PWRu4sSJamxs1I4dO7r07+xq69evV2xsrC644ALdddddOnLkiGMb4+estrZW0r8fGswx6Lpvj90pHH9n19zcrDfffFPHjh3T2LFj/fa4s2TAqaioUHNzs/r16+fU3q9fP5WVlXmpKu8YM2aMli9frg8++EBLlixRWVmZLrvsMlVWVjrGor1xKisrU69evdS3b992+8TGxp7x3bGxsZYab0+OV1lZ2Rnf07dvX/Xq1cuvx3Ty5Mn64x//qLVr1+rXv/61tm/friuvvFKNjY2SGL/TGWM0b948ffe731VqaqokjkFXtTZ2Esff2ezevVthYWEKCgrSvffeq1WrVumiiy7y2+PO0k8Tt9lsTu+NMWe0Wd3kyZMd/x42bJjGjh2r888/X6+//rpjct25jNO3+7TW36rj7anxsuKY3nrrrY5/p6amKj09XYMGDdJ7772nG2+8sc39uuP4zZkzR7t27dKmTZvO2MYx2L62xo7jr31DhgxRfn6+ampqtHLlSs2aNUsbNmxwbPe3486SZ3Cio6MVEBBwRto7cuTIGcmwuwkNDdWwYcNUWFjoWE3V3jjFxcWpqalJ1dXV7fb517/+dcZ3lZeXW2q8PTlecXFxZ3xPdXW1Tpw4Yakx7d+/vwYNGqTCwkJJjN8pc+fO1erVq7Vu3ToNGDDA0c4xeHZtjV1rOP6c9erVS8nJyUpPT1d2draGDx+u3/72t3573Fky4PTq1UsjR47URx995NT+0Ucf6bLLLvNSVb6hsbFRn332mfr376+kpCTFxcU5jVNTU5M2bNjgGKeRI0cqMDDQqc/hw4e1Z88eR5+xY8eqtrZWH3/8saPPP//5T9XW1lpqvD05XmPHjtWePXt0+PBhR58PP/xQQUFBGjlyZJf+nZ5UWVmpgwcPqn///pIYP2OM5syZo7fffltr165VUlKS03aOwbadbexaw/HXPmOMGhsb/fe4c2tKsh85tUz8tddeM3v37jUPPPCACQ0NNSUlJd4uzaMefPBBs379elNUVGS2bdtmpkyZYsLDwx3j8Mwzzxi73W7efvtts3v3bjNjxoxWl/4NGDDA/P3vfzd5eXnmyiuvbHXp3yWXXGK2bt1qtm7daoYNG+aXy8SPHj1qdu7caXbu3GkkmYULF5qdO3c6bi/gqfE6tVTyqquuMnl5eebvf/+7GTBggE8vMzWm/fE7evSoefDBB82WLVtMcXGxWbdunRk7dqw577zzGL//7yc/+Ymx2+1m/fr1TkuZGxoaHH04Blt3trHj+GtfVlaWyc3NNcXFxWbXrl3mF7/4henRo4f58MMPjTH+edxZNuAYY8yLL75oBg0aZHr16mVGjBjhtFywuzh1r4LAwEATHx9vbrzxRvPpp586tre0tJjHHnvMxMXFmaCgIJORkWF2797t9BnHjx83c+bMMZGRkaZ3795mypQp5sCBA059KisrzcyZM014eLgJDw83M2fONNXV1Z74EzvVunXrjKQzXrNmzTLGeHa8SktLzfXXX2969+5tIiMjzZw5c8zXX3/dlX9+h7U3fg0NDebaa681MTExJjAw0AwcONDMmjXrjLHpzuPX2thJMkuXLnX04Rhs3dnGjuOvfXfccYfj9zImJsZcddVVjnBjjH8edzZjjHHvnA8AAIBvs+QcHAAA0L0RcAAAgOUQcAAAgOUQcAAAgOUQcAAAgOUQcAAAgOUQcAAAgOUQcAAAgOUQcAC0y2az6Z133unw5yxbtkx9+vTp8Od4WmVlpWJjY1VSUuLyPgsWLFC/fv1cGrsXXnhB06ZN61iRAM5AwAG6odmzZ8tms8lmsykwMFD9+vXTNddco9///vdqaWlx6nv48GFNnjzZS5V6X3Z2tqZOnarExESX+n/22Wf6r//6L/3P//yPS2N31113afv27dq0aVMnVAvgFAIO0E1NmjRJhw8fVklJidasWaMJEybo/vvv15QpU3Ty5ElHv7i4OAUFBXmx0vadOHGiyz77+PHjeu211/TjH//Y5X2++OILSdL06dNdGrugoCDdfvvtWrx4cYdqBeCMgAN0U0FBQYqLi9N5552nESNG6Be/+IXeffddrVmzRsuWLXP0O/0yS1NTk+bMmaP+/fsrODhYiYmJys7OdvStqanR3XffrX79+ik4OFipqan661//6vS9H3zwgS688EKFhYU5QtYp27dv1zXXXKPo6GjZ7XaNHz9eeXl5TvvbbDa9/PLLmj59ukJDQ/Xkk09Kkp588knFxsYqPDxcP/7xjzV//nx95zvfcdp36dKluvDCCxUcHKyhQ4fqd7/7XbtjtGbNGvXs2VNjx451av/00091/fXXKyIiQuHh4br88sv1xRdfaMGCBZo6daokqUePHrLZbJKk9evXa/To0QoNDVWfPn00btw4lZaWOj5v2rRpeuedd3T8+PF26wHgOgIOAIcrr7xSw4cP19tvv93q9kWLFmn16tX605/+pIKCAr3xxhuOSzctLS2aPHmytmzZojfeeEN79+7VM888o4CAAMf+DQ0Neu655/SHP/xBubm5OnDggB566CHH9qNHj2rWrFnauHGjtm3bppSUFF133XU6evSoUx2PPfaYpk+frt27d+uOO+7QH//4Rz311FN69tlntWPHDg0cOFAvvfSS0z5LlizRI488oqeeekqfffaZnn76af3yl7/U66+/3uZ45ObmKj093ant0KFDysjIUHBwsNauXasdO3bojjvu0MmTJ/XQQw9p6dKlkr65tHf48GGdPHlSN9xwg8aPH69du3Zp69atuvvuux3hR5LS09N14sQJffzxx+38rwPALW4/fxyA35s1a5aZPn16q9tuvfVWc+GFFzreSzKrVq0yxhgzd+5cc+WVV5qWlpYz9vvggw9Mjx49TEFBQaufu3TpUiPJ7N+/39H24osvmn79+rVZ58mTJ014eLj5y1/+4lTPAw884NRvzJgx5r777nNqGzdunBk+fLjjfUJCglmxYoVTnyeeeMKMHTu2ze+fPn26ueOOO5zasrKyTFJSkmlqamp1n1WrVpnT/9NaWVlpJJn169e3+T3GGNO3b1+zbNmydvsAcB1ncAA4McY4nV043ezZs5Wfn68hQ4YoMzNTH374oWNbfn6+BgwYoAsuuKDNzw4JCdH555/veN+/f38dOXLE8f7IkSO69957dcEFF8hut8tut6u+vl4HDhxw+pxvn1UpKCjQ6NGjndpOf19eXq6DBw/qzjvvVFhYmOP15JNPOubMtOb48eMKDg52asvPz9fll1+uwMDANvc7XWRkpGbPnq2JEydq6tSp+u1vf+t0We6U3r17q6GhwaXPBHB2BBwATj777DMlJSW1um3EiBEqLi7WE088oePHj+t73/uebr75Zknf/ECfzbdDgc1mkzHG8X727NnasWOHnn/+eW3ZskX5+fmKiopSU1OT036hoaFnfPa3Q9npn3tqZdiSJUuUn5/veO3Zs0fbtm1rs97o6GhVV1c7tbnyd37b0qVLtXXrVl122WV66623dMEFF5zxvVVVVYqJiXH7swG0joADwGHt2rXavXu3brrppjb7RERE6NZbb9WSJUv01ltvaeXKlaqqqtIll1yiL7/8Uvv27Tvn79+4caMyMzN13XXX6eKLL1ZQUJAqKirOut+QIUPOmL/yySefOP7dr18/nXfeeSoqKlJycrLTq60wJ0lpaWnau3evU9sll1yijRs3ur16Ky0tTVlZWdqyZYtSU1O1YsUKx7YvvvhCX3/9tdLS0tz6TABt6+ntAgB4R2Njo8rKytTc3Kx//etf+tvf/qbs7GxNmTJFP/zhD1vd5ze/+Y369++v73znO+rRo4f+/Oc/Ky4uTn369NH48eOVkZGhm266SQsXLlRycrI+//xz2Ww2TZo0yaWakpOT9Yc//EHp6emqq6vTf/7nf7p0xmTu3Lm66667lJ6e7jhLsmvXLg0ePNjRZ8GCBcrMzFRERIQmT56sxsZGffLJJ6qurta8efNa/dyJEycqKytL1dXV6tu3ryRpzpw5Wrx4sW677TZlZWXJbrdr27ZtGj16tIYMGXLGZxQXF+uVV17RtGnTFB8fr4KCAu3bt89pjDdu3KjBgwc7Xb4D0DGcwQG6qb/97W/q37+/EhMTNWnSJK1bt06LFi3Su+++67Ty6XRhYWF69tlnlZ6erlGjRqmkpETvv/++evT45j8lK1eu1KhRozRjxgxddNFF+vnPf67m5maXa/r973+v6upqpaWl6Qc/+IEyMzMVGxt71v1mzpyprKwsPfTQQ47LaLNnz3aaP/PjH/9Yr776qpYtW6Zhw4Zp/PjxWrZsWbtncIYNG6b09HT96U9/crRFRUVp7dq1qq+v1/jx4zVy5EgtWbKkzTk5ISEh+vzzz3XTTTfpggsu0N133605c+bonnvucfTJycnRXXfd5coQAXCRzZx+oRoALOKaa65RXFyc/vCHP3Toc95//3099NBD2rNnjyPIdaY9e/boqquu0r59+2S32zv984HuiktUAPxeQ0ODXn75ZU2cOFEBAQHKycnR3//+d3300Ucd/uzrrrtOhYWFOnTokBISEjqhWmdfffWVli9fTrgBOhlncAD4vePHj2vq1KnKy8tTY2OjhgwZokcffVQ33nijt0sD4CUEHAAAYDlMMgYAAJZDwAEAAJZDwAEAAJZDwAEAAJZDwAEAAJZDwAEAAJZDwAEAAJZDwAEAAJbz/wAOhPt2fh280wAAAABJRU5ErkJggg==\n",
+                        "image/png": "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jxUbG6vzzjtPvXv3VlVVlb744gsFBwdr5syZevjhhzVo0KCurBkAAKBdLl2iGjFihBYuXKjvf//7KikpUVlZmXbs2KFNmzZp7969qqur07vvvquWlhalp6frz3/+c6cUd/LkST366KNKSkpS7969NXjwYD3++ONqaWnplM8HAADW5NIZnCeeeELXX399m9uDgoJ0xRVX6IorrtCTTz6p4uLiTinu2Wef1csvv6zXX39dF198sT755BP96Ec/kt1u1/33398p3wEAAKzHpYDTXrj5tujoaEVHR59zQafbunWrpk+f7vj+xMRE5eTk6JNPPmlzn8bGRjU2Njre19XVdUotAADAf7i9iiogIEBHjhw5o72yslIBAQGdUtQp3/3ud/WPf/xD+/btkyT93//9nzZt2qTrrruuzX2ys7Nlt9sdr4SEhE6tCQAA+D63V1EZY1ptb2xsVK9evTpc0Okefvhh1dbWaujQoQoICFBzc7OeeuopzZgxo819srKyNG/ePMf7uro6Qg4AAN2MywFn0aJFkiSbzaZXX31VYWFhjm3Nzc3Kzc3V0KFDO7W4t956S2+88YZWrFihiy++WPn5+XrggQcUHx+vWbNmtbpPUFCQgoKCOrUOAADgX2ymrVMy35KUlCRJKi0t1YABA5wuR/Xq1UuJiYl6/PHHNWbMmE4rLiEhQfPnz9d9993naHvyySf1xhtv6PPPP3fpM+rq6mS321VbW6uIiIhOqw0AAHSdjv5+u3QGZ/Xq1SooKFCvXr00YcIEvf322+rbt6/bX+auhoYG9ejhPE0oICCAZeIAAKBdLgWc//iP/1BZWZliYmKUm5urEydOdHVdkqSpU6fqqaee0sCBA3XxxRdr586dWrhwoe644w6PfD8AAPBPLq2iiomJ0bZt2yR9M8nYZrN1aVGnLF68WDfffLN++tOf6sILL9RDDz2ke+65R0888YRHvh8AAPgnl+bgLFiwQI8//rhLwaa5ublTCusszMEBAMD/eGQOzoIFC3Tbbbdp//79mjZtmpYuXao+ffq4/WUAAACe4PIy8aFDh2ro0KF67LHHdMsttygkJKQr6wIAADhnLi8T91dcogIAwP909PfbpUnGkyZN0pYtW87a7+jRo3r22Wf14osvul0IAABAZ3HpEtUtt9yi733vewoPD9e0adOUnp6u+Ph4BQcHq7q6Wnv3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L5vNpnfeecdpuyfH68CBA5o6dapCQ0MVHR2tzMxMNTU1dcWf3WnONn6zZ88+43i89NJLnfp05/HLzs7WqFGjFB4ertjYWN1www0qKChw6sMx2DpXxo7jr20vvfSSLrnkEsdN+caOHas1a9Y4tvvlcWcs6s033zSBgYFmyZIlZu/eveb+++83oaGhprS01NuledRjjz1mLr74YnP48GHH68iRI47tzzzzjAkPDzcrV640u3fvNrfeeqvp37+/qaurc/S59957zXnnnWc++ugjk5eXZyZMmGCGDx9uTp486egzadIkk5qaarZs2WK2bNliUlNTzZQpUzz6t3aG999/3zzyyCNm5cqVRpJZtWqV03ZPjdfJkydNamqqmTBhgsnLyzMfffSRiY+PN3PmzOnyMeiIs43frFmzzKRJk5yOx8rKSqc+3Xn8Jk6caJYuXWr27Nlj8vPzzfXXX28GDhxo6uvrHX04Blvnythx/LVt9erV5r333jMFBQWmoKDA/OIXvzCBgYFmz549xhj/PO4sG3BGjx5t7r33Xqe2oUOHmvnz53upIu947LHHzPDhw1vd1tLSYuLi4swzzzzjaPv666+N3W43L7/8sjHGmJqaGhMYGGjefPNNR59Dhw6ZHj16mL/97W/GGGP27t1rJJlt27Y5+mzdutVIMp9//nkX/FWe8e0faE+O1/vvv2969OhhDh065OiTk5NjgoKCTG1tbZf8vZ2trYAzffr0Nvdh/JwdOXLESDIbNmwwxnAMuuPbY2cMx5+7+vbta1599VW/Pe4seYmqqalJO3bs0LXXXuvUfu2112rLli1eqsp7CgsLFR8fr6SkJN12220qKiqSJBUXF6usrMxpnIKCgjR+/HjHOO3YsUMnTpxw6hMfH6/U1FRHn61bt8put2vMmDGOPpdeeqnsdrulxtuT47V161alpqY6PWRu4sSJamxs1I4dO7r07+xq69evV2xsrC644ALdddddOnLkiGMb4+estrZW0r8fGswx6Lpvj90pHH9n19zcrDfffFPHjh3T2LFj/fa4s2TAqaioUHNzs/r16+fU3q9fP5WVlXmpKu8YM2aMli9frg8++EBLlixRWVmZLrvsMlVWVjrGor1xKisrU69evdS3b992+8TGxp7x3bGxsZYab0+OV1lZ2Rnf07dvX/Xq1cuvx3Ty5Mn64x//qLVr1+rXv/61tm/friuvvFKNjY2SGL/TGWM0b948ffe731VqaqokjkFXtTZ2Esff2ezevVthYWEKCgrSvffeq1WrVumiiy7y2+PO0k8Tt9lsTu+NMWe0Wd3kyZMd/x42bJjGjh2r888/X6+//rpjct25jNO3+7TW36rj7anxsuKY3nrrrY5/p6amKj09XYMGDdJ7772nG2+8sc39uuP4zZkzR7t27dKmTZvO2MYx2L62xo7jr31DhgxRfn6+ampqtHLlSs2aNUsbNmxwbPe3486SZ3Cio6MVEBBwRto7cuTIGcmwuwkNDdWwYcNUWFjoWE3V3jjFxcWpqalJ1dXV7fb517/+dcZ3lZeXW2q8PTlecXFxZ3xPdXW1Tpw4Yakx7d+/vwYNGqTCwkJJjN8pc+fO1erVq7Vu3ToNGDDA0c4xeHZtjV1rOP6c9erVS8nJyUpPT1d2draGDx+u3/72t3573Fky4PTq1UsjR47URx995NT+0Ucf6bLLLvNSVb6hsbFRn332mfr376+kpCTFxcU5jVNTU5M2bNjgGKeRI0cqMDDQqc/hw4e1Z88eR5+xY8eqtrZWH3/8saPPP//5T9XW1lpqvD05XmPHjtWePXt0+PBhR58PP/xQQUFBGjlyZJf+nZ5UWVmpgwcPqn///pIYP2OM5syZo7fffltr165VUlKS03aOwbadbexaw/HXPmOMGhsb/fe4c2tKsh85tUz8tddeM3v37jUPPPCACQ0NNSUlJd4uzaMefPBBs379elNUVGS2bdtmpkyZYsLDwx3j8Mwzzxi73W7efvtts3v3bjNjxoxWl/4NGDDA/P3vfzd5eXnmyiuvbHXp3yWXXGK2bt1qtm7daoYNG+aXy8SPHj1qdu7caXbu3GkkmYULF5qdO3c6bi/gqfE6tVTyqquuMnl5eebvf/+7GTBggE8vMzWm/fE7evSoefDBB82WLVtMcXGxWbdunRk7dqw577zzGL//7yc/+Ymx2+1m/fr1TkuZGxoaHH04Blt3trHj+GtfVlaWyc3NNcXFxWbXrl3mF7/4henRo4f58MMPjTH+edxZNuAYY8yLL75oBg0aZHr16mVGjBjhtFywuzh1r4LAwEATHx9vbrzxRvPpp586tre0tJjHHnvMxMXFmaCgIJORkWF2797t9BnHjx83c+bMMZGRkaZ3795mypQp5sCBA059KisrzcyZM014eLgJDw83M2fONNXV1Z74EzvVunXrjKQzXrNmzTLGeHa8SktLzfXXX2969+5tIiMjzZw5c8zXX3/dlX9+h7U3fg0NDebaa681MTExJjAw0AwcONDMmjXrjLHpzuPX2thJMkuXLnX04Rhs3dnGjuOvfXfccYfj9zImJsZcddVVjnBjjH8edzZjjHHvnA8AAIBvs+QcHAAA0L0RcAAAgOUQcAAAgOUQcAAAgOUQcAAAgOUQcAAAgOUQcAAAgOUQcAAAgOUQcAC0y2az6Z133unw5yxbtkx9+vTp8Od4WmVlpWJjY1VSUuLyPgsWLFC/fv1cGrsXXnhB06ZN61iRAM5AwAG6odmzZ8tms8lmsykwMFD9+vXTNddco9///vdqaWlx6nv48GFNnjzZS5V6X3Z2tqZOnarExESX+n/22Wf6r//6L/3P//yPS2N31113afv27dq0aVMnVAvgFAIO0E1NmjRJhw8fVklJidasWaMJEybo/vvv15QpU3Ty5ElHv7i4OAUFBXmx0vadOHGiyz77+PHjeu211/TjH//Y5X2++OILSdL06dNdGrugoCDdfvvtWrx4cYdqBeCMgAN0U0FBQYqLi9N5552nESNG6Be/+IXeffddrVmzRsuWLXP0O/0yS1NTk+bMmaP+/fsrODhYiYmJys7OdvStqanR3XffrX79+ik4OFipqan661//6vS9H3zwgS688EKFhYU5QtYp27dv1zXXXKPo6GjZ7XaNHz9eeXl5TvvbbDa9/PLLmj59ukJDQ/Xkk09Kkp588knFxsYqPDxcP/7xjzV//nx95zvfcdp36dKluvDCCxUcHKyhQ4fqd7/7XbtjtGbNGvXs2VNjx451av/00091/fXXKyIiQuHh4br88sv1xRdfaMGCBZo6daokqUePHrLZbJKk9evXa/To0QoNDVWfPn00btw4lZaWOj5v2rRpeuedd3T8+PF26wHgOgIOAIcrr7xSw4cP19tvv93q9kWLFmn16tX605/+pIKCAr3xxhuOSzctLS2aPHmytmzZojfeeEN79+7VM888o4CAAMf+DQ0Neu655/SHP/xBubm5OnDggB566CHH9qNHj2rWrFnauHGjtm3bppSUFF133XU6evSoUx2PPfaYpk+frt27d+uOO+7QH//4Rz311FN69tlntWPHDg0cOFAvvfSS0z5LlizRI488oqeeekqfffaZnn76af3yl7/U66+/3uZ45ObmKj093ant0KFDysjIUHBwsNauXasdO3bojjvu0MmTJ/XQQw9p6dKlkr65tHf48GGdPHlSN9xwg8aPH69du3Zp69atuvvuux3hR5LS09N14sQJffzxx+38rwPALW4/fxyA35s1a5aZPn16q9tuvfVWc+GFFzreSzKrVq0yxhgzd+5cc+WVV5qWlpYz9vvggw9Mjx49TEFBQaufu3TpUiPJ7N+/39H24osvmn79+rVZ58mTJ014eLj5y1/+4lTPAw884NRvzJgx5r777nNqGzdunBk+fLjjfUJCglmxYoVTnyeeeMKMHTu2ze+fPn26ueOOO5zasrKyTFJSkmlqamp1n1WrVpnT/9NaWVlpJJn169e3+T3GGNO3b1+zbNmydvsAcB1ncAA4McY4nV043ezZs5Wfn68hQ4YoMzNTH374oWNbfn6+BgwYoAsuuKDNzw4JCdH555/veN+/f38dOXLE8f7IkSO69957dcEFF8hut8tut6u+vl4HDhxw+pxvn1UpKCjQ6NGjndpOf19eXq6DBw/qzjvvVFhYmOP15JNPOubMtOb48eMKDg52asvPz9fll1+uwMDANvc7XWRkpGbPnq2JEydq6tSp+u1vf+t0We6U3r17q6GhwaXPBHB2BBwATj777DMlJSW1um3EiBEqLi7WE088oePHj+t73/uebr75Zknf/ECfzbdDgc1mkzHG8X727NnasWOHnn/+eW3ZskX5+fmKiopSU1OT036hoaFnfPa3Q9npn3tqZdiSJUuUn5/veO3Zs0fbtm1rs97o6GhVV1c7tbnyd37b0qVLtXXrVl122WV66623dMEFF5zxvVVVVYqJiXH7swG0joADwGHt2rXavXu3brrppjb7RERE6NZbb9WSJUv01ltvaeXKlaqqqtIll1yiL7/8Uvv27Tvn79+4caMyMzN13XXX6eKLL1ZQUJAqKirOut+QIUPOmL/yySefOP7dr18/nXfeeSoqKlJycrLTq60wJ0lpaWnau3evU9sll1yijRs3ur16Ky0tTVlZWdqyZYtSU1O1YsUKx7YvvvhCX3/9tdLS0tz6TABt6+ntAgB4R2Njo8rKytTc3Kx//etf+tvf/qbs7GxNmTJFP/zhD1vd5ze/+Y369++v73znO+rRo4f+/Oc/Ky4uTn369NH48eOVkZGhm266SQsXLlRycrI+//xz2Ww2TZo0yaWakpOT9Yc//EHp6emqq6vTf/7nf7p0xmTu3Lm66667lJ6e7jhLsmvXLg0ePNjRZ8GCBcrMzFRERIQmT56sxsZGffLJJ6qurta8efNa/dyJEycqKytL1dXV6tu3ryRpzpw5Wrx4sW677TZlZWXJbrdr27ZtGj16tIYMGXLGZxQXF+uVV17RtGnTFB8fr4KCAu3bt89pjDdu3KjBgwc7Xb4D0DGcwQG6qb/97W/q37+/EhMTNWnSJK1bt06LFi3Su+++67Ty6XRhYWF69tlnlZ6erlGjRqmkpETvv/++evT45j8lK1eu1KhRozRjxgxddNFF+vnPf67m5maXa/r973+v6upqpaWl6Qc/+IEyMzMVGxt71v1mzpyprKwsPfTQQ47LaLNnz3aaP/PjH/9Yr776qpYtW6Zhw4Zp/PjxWrZsWbtncIYNG6b09HT96U9/crRFRUVp7dq1qq+v1/jx4zVy5EgtWbKkzTk5ISEh+vzzz3XTTTfpggsu0N133605c+bonnvucfTJycnRXXfd5coQAXCRzZx+oRoALOKaa65RXFyc/vCHP3Toc95//3099NBD2rNnjyPIdaY9e/boqquu0r59+2S32zv984HuiktUAPxeQ0ODXn75ZU2cOFEBAQHKycnR3//+d3300Ucd/uzrrrtOhYWFOnTokBISEjqhWmdfffWVli9fTrgBOhlncAD4vePHj2vq1KnKy8tTY2OjhgwZokcffVQ33nijt0sD4CUEHAAAYDlMMgYAAJZDwAEAAJZDwAEAAJZDwAEAAJZDwAEAAJZDwAEAAJZDwAEAAJZDwAEAAJbz/wAOhPt2fh280wAAAABJRU5ErkJggg==",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "# plot the data\n",
                 "ax = df.plot.scatter(x='q', y='stage', marker='o')\n",
                 "ax.set_xlabel(\"Discharge (cfs)\")\n",
                 "ax.set_ylabel(\"Stage (ft)\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "0e1ccef0-0d5e-4677-a0bb-6eb257a6be62",
             "metadata": {
                 "id": "0e1ccef0-0d5e-4677-a0bb-6eb257a6be62"
             },
             "source": [
                 "## Setup model\n",
-                "Setup a rating model. This make take a minute while the model compiles."
+                "Now, setup the rating model.\n",
+                "This make take a minute the first time while the model compiles but will be faster on subsequent runs."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
-            "id": "c26b75e4-d127-43e3-adec-2ee57a5aba7e",
+            "execution_count": 16,
             "metadata": {
                 "id": "c26b75e4-d127-43e3-adec-2ee57a5aba7e"
             },
             "outputs": [],
             "source": [
                 "segments = 2\n",
                 "powerrating = PowerLawRating(q=df['q'],\n",
@@ -250,24 +211,25 @@
                 "                             q_sigma=df['q_sigma'],\n",
                 "                             segments=segments,\n",
                 "                             prior={'distribution':'uniform'})"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "a45904c6-aa62-449c-8830-babce7667767",
             "metadata": {},
             "source": [
-                "then fit the model using variational inference (this will be slower on the first run). Set the number of iterations `n` such that the model stops after the loss stops decreasing."
+                "There are of variety of ways to adjust the optimization.\n",
+                "Here we'll use the defaults,\n",
+                "which uses ADVI and runs for 200,000 iterations,\n",
+                "though the model should coverge well before that."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
-            "id": "95bf05c6-b219-45c6-bb83-9eb225d45860",
+            "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "<style>\n",
@@ -294,89 +256,75 @@
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "    <div>\n",
-                            "      <progress value='120000' class='' max='120000' style='width:300px; height:20px; vertical-align: middle;'></progress>\n",
-                            "      100.00% [120000/120000 00:10&lt;00:00 Average Loss = -49.281]\n",
+                            "      <progress value='200000' class='' max='200000' style='width:300px; height:20px; vertical-align: middle;'></progress>\n",
+                            "      100.00% [200000/200000 00:21&lt;00:00 Average Loss = -44.318]\n",
                             "    </div>\n",
                             "    "
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Finished [100%]: Average Loss = -49.273\n"
+                        "Finished [100%]: Average Loss = -44.314\n"
                     ]
                 }
             ],
             "source": [
-                "with powerrating:\n",
-                "    mean_field = pm.fit(method='advi', n=120_000)\n",
-                "    trace = mean_field.sample(5000)"
+                "trace = powerrating.fit()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "669f1afa-43a5-45c1-b36b-d33ba119a5ac",
             "metadata": {},
             "source": [
-                "Once fit, we can evaluate the model by plotting the rating curve."
+                "Once fit, we can plot the rating curve."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
-            "id": "a809fb07-e56d-4878-ae3d-a391705c4e8e",
+            "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/mnt/c/Users/thodson/OneDrive - DOI/Desktop/Projects/software-release/ratingcurve/ratingcurve/ratingmodel.py:318: RuntimeWarning: invalid value encountered in log\n",
-                        "  b1 = np.where(h_tile <= hs, clips, np.log(h_tile-h0))\n"
-                    ]
-                },
-                {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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ops3b8brr7+Onj17Gu+Z02q1GDBgADZv3gwA8PLywvLly63XU6JGeuutt9CnTx+UlJQAAHJycjBlyhTodDro9Xp0794d3bt3x9dff42SkhK89957ePzxx03u/wwJCbFV94nIgVj0najBlStXcPXqVQiCgM6dO6NTp07W7JtV8DtR5yIIAnJycowBevnyZYwbNw56vR75+fm44447UFRUhJycHOj1eowaNQofffQRJJIm3TJNRA7Abr4TNejcuTM6d+5slY4QNZVer0d2djbKysoAAD///DOmTZuG6OhorF27FufPn0dCQgJUKhU6d+6MiRMn4rXXXuMFRERkMYtD9NatW/jmm2+QlpaGyspKk+dWrFjR5I4RmcMwkHxFRQUAIDExER988AEeeughLF26FB4eHhg4cKBxaEpOoE1E1mBRiP7vf//D008/jejoaCQlJaFbt25ITU2FIAi45557rN1HonoZBpKvrKyEIAhYt24dPvnkE7z44ouYNWuWyalakUiEoKAgeHp62rDHRNRaWHQea9asWZg2bRr+/vtvuLm5Yd++fUhPT0ffvn3xwgsvWLuPRHXSarVQKBSorKyERqPB+++/j08++QTvvvsu3n//fZMAFYvFCAsLY4ASkdVYFKKXL1/GiBEjANwe2aW8vBxeXl744IMPsGTJEqt2kKguGo0GCoUCWq0WxcXFGDduHL7//nssXrwYb7/9tsmpWplMhvDwcLi6utqwx0TU2lgUop6enlCr1QBuD6pw48YN43O5ubnW6RlRPdRqNRQKBXQ6HXJycvDmm2/i0qVL+OSTT/DEE0+YtPXw8EBYWBivwCUiq7PoU+X+++/HL7/8gq5du+KJJ57AtGnTcPHiRSQmJuL++++3dh+JjA4cOIAlS5bg6tWriIqKwrPPPovt27dDo9Fg27ZtNWZh8fX1RZs2bXgBERE1C4uORFesWIH77rsPADB//nw8+uij2Lt3L9q1a2ccbIHI2g4cOIDhw4fD09MT48ePh0QiQXx8PDQaDXbu3FkjQAMDA+Hn58cAJaJmY9GRaExMjPH/Hh4eWL9+vdU6RFSdYSzcefPmoXv37pg0aRL++usvJCUlwcPDA+7u7igoKIBEIkFgYCBEIhFCQkLg7u5u664TUStn0ZFoTEwM8vLyajxeWFhoErBE1vDZZ5/hoYcewrVr13DhwgW8/PLLiI+PR2VlJcrKynDz5k289NJL+PLLL41TmDFAiaglWBSiqamp0Ol0NR43XOxBZE0vvPAC9u7di+joaOPMKo888gh27dqF7t27IyYmBnv37sWrr76K8PBwkzFwiYiak1mnc7/55hvj/w8ePAi5XG78WafT4X//+x+ioqKs1jkiw2nazp07o23btjh+/DjCw8PRs2dPrF27FhcuXMCqVatw7733Gk/lEhG1FLMGoDeMMSoSiVB9MalUiqioKCxfvhxPPvmkdXvZBByA3jEJgoCCggIUFhYaB1H44Ycf8Nxzz+HKlStISUlBdHQ03nnnHQwbNoxX4BJRg2w+AL1erwcAREdH4/Tp0wgICLBKJ4iqEgQBeXl5UKlUKC0txZQpU3DmzBksW7YMjz32mEnbwMBAeHt726inROTszPpO9Pfff8cPP/yAlJQUY4Bu374d0dHRCAoKwjvvvGMchIHIEoapzFQqFfLy8vDWW2/h4sWL2Lhxo0mAikQihIaGMkCJyKbMOhKdN28eHnnkEQwZMgQAcPHiRfznP//ByJEj0aVLFyxbtgxhYWGYP39+c/S1Sdzc3ODm5mbrblA9BEHArVu3UFJSglu3bmH06NEoKyvDli1bTKbck0gkaNu2Ld9PIjJL9RnHrMGsEP3rr7+wcOFC48979uzBfffdh4SEBABAZGQk5s2bZ5ch6uLiwnkj7Zher0d6ejpKSkpw7do1jB49Gu7u7tixYwciIiKM7VxdXREVFcUrcInIbM2RAWatsaCgAMHBwcafjx8/jsGDBxt/7t27N9LT063XO3IKer0eqampKCkpwV9//YWRI0fC398f27ZtMwlQT09PxMTEMECJyG6YFaLBwcFISUkBcPuw+Ny5c3jggQeMzxcXF/MDjsyi0+mQkpKCsrIynDp1CqNGjUKHDh2wefNmkwvXfH19ERUVBbFYbMPeEhGZMitEBw8ejJkzZ+LkyZOYNWsWPDw88O9//9v4/IULF9C+fXurd5JaJ61Wi5SUFJSXl+Onn37C+PHj0bNnT2zcuNHk8vOgoCCEh4fzFhYisjtmhejChQshFovRt29fJCQkICEhATKZzPj8Z599hkGDBlm9k9T6GAK0oqICiYmJmD59Oh599FGsXr3aZMi+sLAwBAUFMUCJyC6ZNdiCQVFREby8vGqcWsvPz4eXl5dJsNqaYbAFa95cS02j0WiQkpKCyspKbN26FcuXL8dLL72E2bNnmwzo0bZtW97CQkRW0xx5YNGlSnK5vNbvpvz8/KweoAqFAq+99hr8/f3h4eGBu+++G2fPnrXqa1DLqaysRHJyMtRqNT7++GMsX74c77zzDubMmWMMUBcXF0RHRzNAicjuWTQVWkspKChAnz598Mgjj+CHH35AUFAQbty4AV9fX1t3jSxQNUAXLVqEL7/8Eu+99x7eeOMNYxuJRILo6Gi4urrasKdERI1j1yG6ZMkSREZGYsuWLcbHOMC9Y1Kr1caLiGbNmoWffvoJH374IZ599lljG94DSkSOxq5HH/jmm2/Qq1cvvPDCCwgKCsK//vUv48AOdVGr1VCpVCb/yLbUajWSk5NRXFyMiRMn4siRI1ixYoVJgHp4ePAeUCJyOHYdosnJydiwYQM6duyIgwcPYsyYMZg0aRK2b99e5zLx8fGQy+XGf5GRkS3YY6quoqICycnJUKlUGDt2LM6dO4f169djwIABxjY+Pj68B5SIHJJFV+e2FJlMhl69euHUqVPGxyZNmoTTp0/j119/rXUZtVptMgi+SqVCZGQkr861AUOAFhQUYNy4ccY/iu6++25jmzZt2iAsLIy3sBBRs2uOq3Pt+jvR0NBQdO3a1eSxLl26YN++fXUu4+rqyotS7EB5eTlSUlKQm5uL0aNHIzMzE5s2bcKdd95pbBMUFMSJtInIodl1iPbp0wdJSUkmj129ehXt2rWzUY+oMcrKypCamgqlUolRo0ahqKgIW7ZsQceOHY1tQkND4e/vb8NeEhE1nV1/JzplyhT89ttviIuLw/Xr17F79258+umnGD9+vK27RnUoKytDSkoKbt26hZEjR6K0tBRbt241CdCIiAgGKBG1CnYdor1798b+/fvx+eefo1u3bvjwww+xatUqvPrqq7buGtXCEKC7d+/GE088gVu3bsHb2xvXr18HcHsUonbt2vE+XyJqNez6wiJr4LB/LcMQoNu3b8fSpUvh7u6OESNG4MKFCzh16hRWrVqFt99+G56enrbuKhE5qebIA4YoNZkhQH/++WeMGzcOMpkMH3/8MXx9fSEIAuLi4qDX63Hx4kVbd5WInJjTXZ1L9q+0tBSpqan4888/MWnSJOj1elRUVGD06NEm7TiIAhG1RgxRstju3buxaNEiXL9+HRqNBpGRkRCJRJDL5Zg9ezZkMhnCwsLw7rvvory83NbdJSKyOru+sIjs1+eff45XX30VIpEIer0e3t7eSEtLQ//+/XHhwgWsWbMG169fx9y5c/H7779j/vz5tu4yEZHVMUTJbGVlZZg3bx5iYmJw7do1dOnSBWvWrEH37t3xyy+/YN26daioqMD8+fORn5+PxMREPPfcc7buNhGR1fHCIjKL4SKiHj16QKfT1XheIpFArVYb5wYlIrIXvLCIbMowEtEvv/wCvV4PLy8vbNiwATKZDIIgYPHixdDr9QxQInIaDFFqlPLycqSmpuLEiRN499130blzZ1y+fBnr169Hnz598Pvvv+P8+fNITEy0dVeJiFoMDxmoQYbB5I8dO4ZJkybhwQcfxM6dO7Fy5UoUFRVh3bp1KCsr43efROR0+J0o1cswndnRo0cxZcoUPPTQQ1i+fLnxvk9fX1+Eh4dzJhYisnvNkQc8EqU6VVRUICUlBYcPH8bkyZPx8MMPmwSon58fA5SInBpDlGqlVquRkpKCQ4cOYdq0aXjkkUewbNkyY4D6+/sjNDSUAUpETo0hSjVUVlYaj0CnT5+OAQMGYMmSJcYADQgIQEhICAOUiJwer84lE5WVlUhOTsaRI0cwdepUPPLII1i8eDEkktu7SmBgIIKCghigRERgiFIVGo0GKSkpOHHiBKZMmYJ///vfWLJkiTFAg4KCEBQUZONeEhHZD57OJQCAVqs1Tmc2adIk3Hffffjoo4+Mp3AZoERENTFEyRigp06dwsSJE9GzZ0+sXLkSMpkMAAOUiKguDFEnp9PpkJqait9//x3jxo1D9+7d8fHHH8PV1RUAA5SIqD4MUSdmCNDTp09jzJgx6Nq1K1avXg03NzcADFAiooYwRJ2UXq9HWloazp49i9GjR6Njx45Yt24dPDw8ADBAiYgagyHqhARBQFpaGs6dO4d33nkHUVFR2LBhAzw9PQH8320sRERUP4aokxEEAenp6bhw4QJGjRqFsLAwbNy4EV5eXgAYoERE5mCIOhFBEKBQKPDPP/9g1KhR8Pf3x6effmociDkgIIADKRARmYEh6iQEQYBSqURSUhLefvttuLm5ISEhAb6+vgBuj4UbHBzMACUiMgNHLHISOTk5uH79Ot555x3odDp89tlnCAgIAAC0adOGY+ESEVmAIeoE8vLycOPGDYwePRqFhYXYtm0bwsLCANyeDzQsLIwBSkRkAYZoK1dQUIAbN25g/PjxuHXrFrZs2YKoqCgAgI+PD+cDJSJqAoZoK6ZSqZCSkoLJkyfjypUr2LRpEzp16gQA8Pb2RmRkJAOUiKgJnCZE9Xo99Hq9rbvRYkpLS5GSkoL33nsPZ8+exYYNG9C9e3cAgKenJ8LDwyEIAgRBsHFPiYhaRnNkgNOEaEVFhXFA9dZOrVbj1q1bmDt3Lk6cOIFVq1bh3nvvBQC4uroiMDAQlZWVNu4lEVHLqqiosPo6nSZEnYVWq0VGRgaWLl2Kb7/9FkuXLkXfvn0BADKZDKGhoXBx4Z1NRETWwE/TVkSn0yEjIwObNm3Czp07MXv2bAwePBgAIJVKGaBERFbGT9RWQq/XQ6lU4ssvv8SqVaswevRovPzyywAAiUSCsLAwiMViG/eSiKh1YYi2AoIgICcnB4cOHcKCBQvw/PPPY/z48QAYoEREzYkh2goUFBTgl19+wfTp09GvXz+8//77EIlEEIvFCA0NhUTCr76JiJoDP10d2IEDB7B48WIkJSVBo9EgKioKS5YsgVgshouLC8LCwiCVSm3dTSKiVotHog7qwIEDGD58OGQyGWQyGdzc3JCcnIyTJ08yQImIWghD1EEtXboU99xzD/Ly8iCRSLBs2TL07NkTCQkJCA0NdZp7YomIbIkh6oAEQUBSUhJSU1ORkpKCgoICjB8/Hq6urkhNTYWrq6utu0hE5BT4nagDys/Ph7u7O/Lz8xEbG4uePXtCEAR8/PHHxrFxiYio+TFEHUxpaSkSEhKQn58PADh58iT0ej1Onz6NX3/9FZ9//rmNe0hE5Dyc5nRu1bFiKysrodVqAdwepECtVhsHJtZqtVCr1SZtNRoNgNunUau21el0Jm01Gk2NtjqdzqStYcB3S9pqNBocOHAAcXFxGD58OFauXImioiKsW7cOKpUKn3/+OYYMGWKyrWq1ut5tNacuTamhoW31Gjam3tXr0tR6G+pSX9vqNTS0NWyroW31uth7vavX0F7rXX1b7b3e9vIZUVu9q9ewMfW2p33W2p8R1uY0IZqVlWX8f3Z2NgoLCwHcLrpCoTAWt6SkBJmZmca2OTk5NdoaBjEuKSmBQqEwts3NzTUeIQqCAIVCgfLycgBAWVmZSdu8vDzk5eUZf1YoFCgrKwMAlJeXQ6FQGHf6/Px85OTk4MyZM5g+fTruv/9+xMbGYuDAgfj+++/xxx9/4NixY3j66adRWFiInJwc43ozMzNRUlIC4PYvi0KhMO5whYWFyM7ONmmrUqkA3N5RFQqFcQdUqVRQKpUm9SwqKgJweydXKBTGX6Di4mKTtlXrbWhbtYYZGRkm9S4oKABw+xevatvS0tIm1Ts3N9ek3qWlpQBuD0qtUCiMv7QFBQUmbTMyMow1NLQ11LCgoKBGvYuLi01qaPhwKCoqMtkPlUqlsd4ajaZJ9a6+zxpqWNs+W7Xeubm5ZtXbnH3WnHpXrWFt9TbUsPo+q1Qqm1RvQw1VKpVJDR3xM6J6vevaZ535M6Lq+2YtIqGVz4WlUqkgl8tx8+ZNBAQEALj95ru4uEAikUCv10Oj0UAqlcLFxQVarRY6nc54cU5lZSVEIhGkUikEQUBlZaWxrU6ng1arNbY17ExV20okEojFYmNbmUwGkUhkdluFQoHnnnsO5eXl+PzzzyGXy+Hr6wtfX19oNBqTtoIgGK/OVavVEIvFdW6rXq83tm2oLua0rV5DQ9vqNWxMvavXpan1NtSlvrbVa2hoa9hWQ9vqdbH3elevob3Wu3oN7b3e9vAZUVe9q9fQmT8jcnNzERUVhaKiIvj4+MAanCZEMzMzrVa0llZaWorXX38dJ06cwK5du9CxY0d4e3sjICCAk2oTETWSSqVCaGioVUOUFxbZOa1Wi8WLF+PgwYNYvnw5OnbsCHd3dwYoEZEdcKjvROPj4yESiTB58mRbd6VFCIKA/fv3Y9WqVXj77bcxaNAgSKVSBAcHM0CJiOyAw4To6dOn8emnn6J79+627kqLSUpKwtSpU3H//fdjwoQJcHFx4ZygRER2xCE+jUtKSvDqq68iISEBbdq0sXV3WkRpaSlGjx4NiUSCuLg4iMVihISEcEYWIiI74hAhOn78eDzxxBMYOHBgg23VajVUKpXJP0dx4MAB9OnTB4GBgejatSvOnj2LJUuWwN/fH4GBgXBzc7N1F4mIqAq7D9E9e/bg3LlziI+Pb1T7+Ph4yOVy47/IyMhm7qF1GGZl8ff3xzPPPIPc3FwIgoDCwkL4+PjA29vb1l0kIqJq7PoWl/T0dPTq1QuHDh1Cjx49AAD9+vXD3XffjVWrVtW6jFqtNhmVQqVSITIy0u5vcenTpw+8vLwwfvx4jB49Gh07doRUKkVJSQl+++03XkhERNREzXGLi10fiZ49exbZ2dno2bMnJBIJJBIJjh8/jtWrV0MikRhH1ajK1dUVPj4+Jv8cwdWrVyGVSvHKK69ApVKhW7du+Pe//43k5GQGKBGRnbLrq1QGDBiAixcvmjz25ptvonPnzpgxYwbEYrGNemZ9d9xxB5KSkgAA8+bNw8MPP4wPP/yQs7IQEdkxuw5Rb29vdOvWzeQxT09P+Pv713jcUR04cABLly7FpUuXoNFo4O/vj9LSUsyfPx8nT57krCxERHbMrk/ntnZz5szB8OHDceHCBeh0OshkMuTl5WH16tUoKSnB559/jqefftrW3SQiojrY9ZFobY4dO2bRcm5ubnZ1i0hiYiJWrVplHCDaMJBy+/btIZfLcfr0aVt3kYioVak6VZu1OFyIWsrFxcWuRvqJjY0FAPj6+taY7igzM9Ou+kpE1Bo0x+cqP6ltJDU11Xj6FgAef/xxhIeHo6KiAl26dLFx74iIqDEYojYiEomMkxIDtyeaNUweO2fOHFt1i4iIzMAQbWGJiYno2bMn9Ho9tFot2rRpA39/f5w5cwbl5eUIDg7Gc889Z+tuEhFRIzjNd6J6vd7kyK+lJSYmIjY2FikpKXB3dzc+XlBQALFYDC8vLxQXF2PdunU27ScRUWvVHJ+tThOiFRUVkMlkNnltw7i43t7eiImJwa1btwAAL7zwAn744QeUlZWhQ4cOiI2NxZAhQ1BRUWGTfhIRtWbN8dnK07ktYOnSpRgwYAA0Gg1kMhk0Gg2A27frzJ49G25ubvj55595TygRkYNxmhCten9QZWUltFotgNuH92q12niYr9VqTQawr6ysNIaeIAgmbXU6nUlbjUZTo61Op8PVq1cxYMAAuLu748qVK+jZsydef/11FBcX4/Dhw+jUqZOxbdX1GuYGqLpeACZtDf2v2rbqtqrV6nq31Zy6NKWGhrbVa9iYelevS0P1NreGtbWtXsO66l29LvZe7+o1tNd6V99We693Uz8jGqphU+rNzwjTttbmNCGalZVl/H92djYKCwsB3C66QqEwFrekpASZmZnGtjk5OTXaGk4JlJSUQKFQGNvm5uYar7AVBAEKhQLl5eW44447cPDgQeNgD3q9HidPnoREIsGRI0fw3nvvQaFQoKysDABQXl4OhUJh3Onz8/ORm5trfB2FQoGSkhIAt09PKBQK405UWFiInJwcY9vMzExjW7VaXaNtdna2SVvD/KuVlZVQKBTGHVClUkGpVJrUs6ioCMDtnVyhUBh/gYqLi03aVq23oW3VGmZkZJjUu6CgwFinqm1LS0sbVW8AKCsrM2mbl5dXo4alpaUmNTT80hYUFJi0zcjIqLPeBQUFNepdXFxsUkPDh0NRUZHJfqhUKo311mg0Tap39X3WUMPa9tmq9c7NzTWr3tXvaTZnn62v3lVrWFu9DTWsvs8qlcom1dtQQ5VKZVLDlv6MAGrfZ5tSb35G1Kx31ffNWux6KjRrUKlUkMvluHnzJgICAgDcfvNdXFwgkUig1+uh0WgglUrh4uICrVYLnU4HV1dXY1uRSASpVGocVcjQVqfTQavVGtsadqaqbSUSCb799lsMHz4cwO0pz86fP4/S0lJERUUhPj4eTz31lLGtWCw2rlcmk0EkEpmsF7i9oxvaGvpfta0gCMbvf9VqNcRicZ3bqtfrjW0bqos5bavX0NC2eg0bU+/qdWmo3ubWsLa21WtYV72r18Xe6129hvZa7+o1tPd6N/UzoqEaNqXe/Iz4vxrm5uYiKirKqlOhOU2I2mo+0QMHDmDJkiX466+/jDtJ165dMWPGDH4HSkTUgpxuPlFHZ7gq13CqoXv37qisrERsbCwDlIioFXCaI9GCgoIWPxLt3bs3/Pz88Pfff6Ndu3aIi4tDXFwcCgsL8ccff7RoX4iInJ1KpUKbNm2seiTqNPeJtvQA9ImJiTh//jxEIhF0Oh2USiW+++47PP7445g7dy4HmCciamEcgN5BJCYmYtiwYfD09IRIJIJcLgcAdOzYET/++CMHmCciaiWc5nSuNQ/fG9KzZ0/jZeVFRUVwc3ODXC5HWVkZiouLkZiYyPFxiYhaWHPkgdOczm0piYmJOHfunMljGo0GWVlZEIlEDFAiolaEIWpFhtO41el0Onh5eUGv1zNAiYhaEX4nakXjxo2r87mSkhLjKCBERNQ6MEStJDEx0WSIsepEIhG6devWgj0iIqLmxhC1kunTp9f7vCAImDNnTgv1hoiIWgJD1EpSUlLqfT42NpbfhxIRtTIMUStITExssM2SJUtaoCdERNSSGKJNVNcVuVXFxMS0UG+IiKglMUSbaNGiRRg0aFC9bT766KMW6g0REbUkhmgTXblyBY899hjCw8Nrff7ee+/ld6FERK0UQ7SJOnfujIMHDyIsLAzu7u4QiUTG55599ln8/vvvNuwdERE1J45Y1ERz5swxfif69NNPo7CwECdOnODwfkREToBHohZKTExEz5498frrr8Pd3R0SiQSHDh1CSUkJA5SIyEkwRC1guCI3ICAA48aNQ3l5ObRaLdasWYOzZ88yQImInARD1AKGK3J//PFHXLlyBQEBAbj//vuxYcMGW3eNiIhaEEPUAleuXEFoaCjuuusufPvttygvL0dkZCSuXLli664REVEL4oVFFvD29sa2bdsA3B5YPjAwEF9++SXat29v454REVFL4pGomWJjY2vM1pKamgrg9iDzRETkPBiiZkhMTMSyZctMHjMEp5eXF5RKpS26RURENsIQNYNhujORSASRSARXV1cAgEQiQUlJCbp06WLL7hERUQtjiJrBcNpWIpFAEASo1Wq4ublBq9UCAOcLJSJyMrywyAwikQhisRgajQYA4ObmhoqKCgBAcHAw7w8lInIyPBI1Q1RUlPGoUywWGwMUAO8RJSJyQgxRMxguKhKJRNDpdMbHY2NjeRRKROSEGKJmCAkJAQBERETAw8MDPXv2RGJiIpYsWWLjnhERkS0wRBvBMNj8ww8/DJlMhsmTJ6O4uBhnzpzhESgRkRNjiDbAMNi8h4cHdDodIiIiMG3aNHz99de27hoREdkYQ7QBhsHm77zzTvj6+mLt2rUYOHAg4uLibN01IiKyMYZoA65cuYLHHnsM3bt3R/fu3XH48GEMGTIEly9ftnXXiIjIxuw6ROPj49G7d294e3sjKCgIzz77LJKSklq0D507d8bBgwcxduxY7Nq1C1OnTsWPP/7I0YmIiMi+Q/T48eMYP348fvvtN/z000/QarUYNGgQSktLW6wPc+bMwaFDh/DYY4/hiy++wJtvvomffvqJoxMRERFEggNNPZKTk4OgoCAcP34cDz/8cKOWUalUkMvlKCoqgo+Pj0Wvm5iYiLi4OFy+fBldunTBnDlzeFUuEZGDsUYeVOdQw/4VFRUBAPz8/Fr0dYcOHYqhQ4e26GsSEZH9c5gQFQQBU6dOxUMPPYRu3brV2U6tVkOtVht/VqlULdE9IiJyQnb9nWhVEyZMwIULF/D555/X2y4+Ph5yudz4LzIysoV6SEREzsYhvhOdOHEivv76a5w4cQLR0dH1tq3tSDQyMtKq58CJiMjxON13ooIgYOLEidi/fz+OHTvWYIACgKurq3GybCIiouZk1yE6fvx47N69GwcOHIC3tzeUSiUAQC6Xw93d3ca9IyIiZ2fXp3NFIlGtj2/ZsgUjR45s1Dqa4/CdiIgcj1OeziUiIrJXDnN1LhERkb1hiBIREVmIIUpERGQhhigREZGFGKJEREQWYogSERFZiCFKRERkIYYoERGRhRiiREREFmKIEhERWYghSkREZCGGKBERkYUYokRERBZiiBIREVmIIUpERGQhhigREZGFGKJEREQWYogSERFZiCFKRERkIYYoERGRhRiiREREFmKIEhERWYghSkREZCGGKBERkYUYokRERBZiiBIREVmIIUpERGQhia070FL0ej30er2tu0FERDbSHBngNCGqUqkgk8kAAJWVlXBxcYFEIoFer4dGo4FUKoWLiwu0Wi10Oh1cXV2NbUUiEaRSKQRBQGVlpbGtTqeDVqs1ttVoNABg0lYikUAsFhvbymQyiEQii9sCgFqtNrY19L9qW0EQjNuqVqshFovr3Fa9Xt/oupjTtnoNDW2r17Ax9a5el6bWu3oNa2tbvYZ11bt6Xey93tVraK/1rl5De683PyMc4zOiqKgI1uY0p3OzsrKM/8/OzkZhYSEAQKfTQaFQQK1WAwBKSkqQmZlpbJuTk1OjbUVFhbGtQqEwts3NzUV+fj4AQBAEKBQKlJeXAwDKyspM2ubl5SEvL8/4s0KhQFlZGQCgvLwcCoUCgiAAAPLz85Gbm2vStqSkBABQUVEBhUIBnU4HACgsLEROTo6xbWZmprGtWq2u0TY7O9ukrUqlAnB7R1UoFMadUKVSQalUmtTTsENqtVooFApUVlYCAIqLi03aVq23oW3VGmZkZJjUu6CgAMDtvxqrti0tLW1SvavXsLS01KSGhr9SCwoKTNpmZGTUWe+CgoIa9S4uLjapoVarBQAUFRWZ7IdKpdJYb41G06R6V99nDTWsbZ+tWu/c3Fyz6t2Ufba+eletYW31NtSw+j6rVCqbVG9DDVUqlUkN+RnROj8jqr5v1iISDO9CK6VSqSCXy5GZmYmgoCAAt3cUFxcXSKVS6PV6qNVqyGQyiMViaLVaaLVauLm5GduKRCLIZDIIgoCKigqTthqNBu7u7o1u6+bmBpFIZNyZqraVSqWQSCTQ6XSorKw0aSsIgvGvq/Ly8ka3raiogEQiMWnr6uoKFxcXaDQa6PV6k7ZisdikLlXb6nQ6Y13MaWuLetdWF0O9rVFDQ9vaamhoW1tdLK13bTU0tK2thoa2tdXQ0nrXts/WV2/us/yMsLd6Z2dnIywsDEVFRfDx8ak9NMzkNCFqzaIREZHjaY48cJrTuURERNbGECUiIrIQQ5SIiMhCDFEiIiILMUSJiIgsxBAlIiKyEEOUiIjIQgxRIiIiCzFEiYiILMQQJSIishBDlIiIyEIMUSIiIgsxRImIiCzEECUiIrKQxNYdaG6Gmd4ME8kSEZFzMuSANWcAbfUhapj1PjIy0sY9ISIie1BcXAy5XG6VdbX6Sbn1ej0yMjLg7e2N4uJiREZGIj09vdVM0K1SqbhNDoDb5Bi4TY7B0m0SBAHFxcUICwuDi4t1vs1s9UeiLi4uiIiIAACIRCIAgI+PT6vZmQy4TY6B2+QYuE2OwZJtstYRqAEvLCIiIrIQQ5SIiMhCThWirq6umDdvHlxdXW3dFavhNjkGbpNj4DY5BnvaplZ/YREREVFzcaojUSIiImtiiBIREVmIIUpERGQhhigREZGFnCpE169fj+joaLi5uaFnz544efKkTfszf/58iEQik38hISH1LnP8+HH07NkTbm5uiImJwcaNG2u02bdvH7p27QpXV1d07doV+/fvr9HGGrU4ceIEnnrqKYSFhUEkEuHrr782eV4QBMyfPx9hYWFwd3dHv379cOnSpQbXa43+W/raDW3TyJEja7xn999/v11vU3x8PHr37g1vb28EBQXh2WefRVJSklXWbavtasw2Odp7tWHDBnTv3t04gMADDzyAH374oUnrtOX2NGabHO09qpXgJPbs2SNIpVIhISFB+Oeff4R3331X8PT0FG7evGmzPs2bN0+48847hczMTOO/7OzsOtsnJycLHh4ewrvvviv8888/QkJCgiCVSoWvvvrK2ObUqVOCWCwW4uLihMuXLwtxcXGCRCIRfvvtN2Mba9Xi+++/F+bMmSPs27dPACDs37/f5PnFixcL3t7ewr59+4SLFy8KL730khAaGiqoVKo612mt/lvy2o3ZphEjRgiDBw82ec/y8vLqXaett+mxxx4TtmzZIvz999/C+fPnhSeeeEJo27atUFJS0qR123K7GrNNjvZeffPNN8J3330nJCUlCUlJScLs2bMFqVQq/P333xav09b7XkPb5GjvUW2cJkTvvfde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",
                         "text/plain": [
                             "<Figure size 500x500 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "powerrating.plot(trace)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "5f39d6e1-8145-44d3-b126-dd05e2c67808",
             "metadata": {},
             "source": [
                 "or as a table of stage-discharge values."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
-            "id": "cdef01af-eb57-450e-9479-5c5e9174a1fa",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "/mnt/c/Users/thodson/OneDrive - DOI/Desktop/Projects/software-release/ratingcurve/ratingcurve/ratingmodel.py:318: RuntimeWarning: invalid value encountered in log\n",
@@ -461,43 +409,40 @@
             "source": [
                 "table = powerrating.table(trace)\n",
                 "table.head()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "44150e09-69f1-49e4-819c-ff12f9ac3ced",
             "metadata": {
                 "id": "ad003463-d23b-4292-8863-1dc52315fe5c"
             },
             "source": [
                 "## Exercise\n",
                 "What happens if we choose the wrong number of segments? \n",
                 "Increase the number of segments by one and rerun the model.\n",
-                "We can use this approach to select the correct number of segments;\n",
-                "more on this topic in the [model evaluation notebook]()(https://github/thodson-usgs/ratingcurve/blob/master/notebooks/model-evaluation-demo.ipynb) "
+                "In fact, we can use this to select the correct number of segments,\n",
+                "which is demonstrated in the [model evaluation notebook](https://github.com/thodson-usgs/ratingcurve/blob/main/docs/notebooks/model-selection-tutorial.ipynb) "
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "84cc1872-6e76-4e32-83bc-f3e50e42eef5",
             "metadata": {
                 "id": "84cc1872-6e76-4e32-83bc-f3e50e42eef5"
             },
             "source": [
                 "## Simulated Example\n",
-                "This example uses a simulated rating curve, which allows you to test how different sampling schemes affect the rating curve fit.\n",
+                "This example uses a simulated rating curve, which allows you to test how\n",
                 "\n",
-                "First, open the `simulated_rating` tutorial dataset."
+                "First, load the '3-segment simulated' tutorial dataset."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
-            "id": "0160c825-a7ba-47f1-995c-a6695e968a2c",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "The simulated rating contains 763 observations\n"
@@ -507,25 +452,23 @@
             "source": [
                 "sim_df = data.load('3-segment simulated')\n",
                 "print('The simulated rating contains {} observations'.format(len(sim_df)))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "8e721b15-4ada-48a8-b778-692ce9eb9e08",
             "metadata": {},
             "source": [
                 "This rating contains observations of every 0.01 inch. increment in stage, which is much more than we'd have for a natural rating.\n",
                 "Try sampling to `n=15` or `n=30` and see how that affects the model fit."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
-            "id": "bc06f4ff-7855-42db-bc15-2726dc99da7b",
             "metadata": {
                 "id": "bc06f4ff-7855-42db-bc15-2726dc99da7b",
                 "outputId": "f4413937-f75c-4043-f1c7-236d3544d611"
             },
             "outputs": [
                 {
                     "data": {
@@ -551,30 +494,28 @@
             "source": [
                 "# subsample the simulated rating curve\n",
                 "n = 30\n",
                 "df = sim_df.sample(n, random_state=12345)\n",
                 "\n",
                 "ax = sim_df.plot(x='q', y='stage', color='grey', ls='-', legend=False)\n",
                 "df.plot.scatter(x='q', y='stage', marker='o', color='blue', ax=ax)\n",
-                "ax.set_xlabel(\"Discharge (cfs)\")\n",
-                "ax.set_ylabel(\"Stage (ft)\")"
+                "ax.set_xlabel(\"Discharge (cfs)\");\n",
+                "ax.set_ylabel(\"Stage (ft)\");"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "1a66d197-4fe3-4d5b-b4cd-46a36497a760",
             "metadata": {},
             "source": [
                 "Setup a rating model with 3 segments"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
-            "id": "980abb5a-e2a5-46fe-9015-8c613d825957",
+            "execution_count": null,
             "metadata": {
                 "id": "980abb5a-e2a5-46fe-9015-8c613d825957"
             },
             "outputs": [],
             "source": [
                 "segments = 3\n",
                 "powerrating = PowerLawRating(q=df['q'],\n",
@@ -583,387 +524,100 @@
                 "                             segments=segments,\n",
                 "                             prior={'distribution':'uniform'})\n",
                 "                             #prior={'distribution':'normal', 'mu':[5, 8, 11], 'sigma':[1, 1, 0.2]})"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "3c61bf36-5bb7-4597-a1c0-dd7a491be454",
             "metadata": {},
             "source": [
                 "now fit the model using ADVI"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
-            "id": "d40dfddd-8de6-4ba4-b380-f26e4b85594f",
+            "execution_count": null,
             "metadata": {
                 "id": "d40dfddd-8de6-4ba4-b380-f26e4b85594f",
                 "outputId": "abc72ca4-8052-476f-9532-40ee902831d3"
             },
-            "outputs": [
-                {
-                    "data": {
-                        "text/html": [
-                            "\n",
-                            "<style>\n",
-                            "    /* Turns off some styling */\n",
-                            "    progress {\n",
-                            "        /* gets rid of default border in Firefox and Opera. */\n",
-                            "        border: none;\n",
-                            "        /* Needs to be in here for Safari polyfill so background images work as expected. */\n",
-                            "        background-size: auto;\n",
-                            "    }\n",
-                            "    progress:not([value]), progress:not([value])::-webkit-progress-bar {\n",
-                            "        background: repeating-linear-gradient(45deg, #7e7e7e, #7e7e7e 10px, #5c5c5c 10px, #5c5c5c 20px);\n",
-                            "    }\n",
-                            "    .progress-bar-interrupted, .progress-bar-interrupted::-webkit-progress-bar {\n",
-                            "        background: #F44336;\n",
-                            "    }\n",
-                            "</style>\n"
-                        ],
-                        "text/plain": [
-                            "<IPython.core.display.HTML object>"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "data": {
-                        "text/html": [
-                            "\n",
-                            "    <div>\n",
-                            "      <progress value='150000' class='' max='150000' style='width:300px; height:20px; vertical-align: middle;'></progress>\n",
-                            "      100.00% [150000/150000 00:14&lt;00:00 Average Loss = -55.532]\n",
-                            "    </div>\n",
-                            "    "
-                        ],
-                        "text/plain": [
-                            "<IPython.core.display.HTML object>"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Finished [100%]: Average Loss = -55.501\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "with powerrating:\n",
-                "    mean_field = pm.fit(method='advi', n=150_000) #increase n as necessary\n",
-                "    trace = mean_field.sample(5000)"
+                "trace = powerrating.fit(method='advi')"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "1e48f841-c1d9-4e44-b300-eda0aa613dce",
             "metadata": {},
             "source": [
                 "and visualize the results."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
-            "id": "1b7dfa46-4972-4c4c-b009-a146e247df6d",
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/mnt/c/Users/thodson/OneDrive - DOI/Desktop/Projects/software-release/ratingcurve/ratingcurve/ratingmodel.py:318: RuntimeWarning: invalid value encountered in log\n",
-                        "  b1 = np.where(h_tile <= hs, clips, np.log(h_tile-h0))\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "image/png": "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\n",
-                        "text/plain": [
-                            "<Figure size 500x500 with 1 Axes>"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                }
-            ],
-            "source": [
-                "powerrating.plot(trace, None)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 15,
-            "id": "713fd9bb-674c-4f80-ac5d-cc9b6407217e",
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "arviz - WARNING - Shape validation failed: input_shape: (1, 5000), minimum_shape: (chains=2, draws=4)\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "text/html": [
-                            "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
-                            "<table border=\"1\" class=\"dataframe\">\n",
-                            "  <thead>\n",
-                            "    <tr style=\"text-align: right;\">\n",
-                            "      <th></th>\n",
-                            "      <th>mean</th>\n",
-                            "      <th>sd</th>\n",
-                            "      <th>hdi_3%</th>\n",
-                            "      <th>hdi_97%</th>\n",
-                            "      <th>mcse_mean</th>\n",
-                            "      <th>mcse_sd</th>\n",
-                            "      <th>ess_bulk</th>\n",
-                            "      <th>ess_tail</th>\n",
-                            "      <th>r_hat</th>\n",
-                            "    </tr>\n",
-                            "  </thead>\n",
-                            "  <tbody>\n",
-                            "    <tr>\n",
-                            "      <th>w[0]</th>\n",
-                            "      <td>0.968</td>\n",
-                            "      <td>0.001</td>\n",
-                            "      <td>0.965</td>\n",
-                            "      <td>0.971</td>\n",
-                            "      <td>0.000</td>\n",
-                            "      <td>0.000</td>\n",
-                            "      <td>4363.0</td>\n",
-                            "      <td>4715.0</td>\n",
-                            "      <td>NaN</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>w[1]</th>\n",
-                            "      <td>0.072</td>\n",
-                            "      <td>0.004</td>\n",
-                            "      <td>0.065</td>\n",
-                            "      <td>0.079</td>\n",
-                            "      <td>0.000</td>\n",
-                            "      <td>0.000</td>\n",
-                            "      <td>5119.0</td>\n",
-                            "      <td>4678.0</td>\n",
-                            "      <td>NaN</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>w[2]</th>\n",
-                            "      <td>0.308</td>\n",
-                            "      <td>0.006</td>\n",
-                            "      <td>0.297</td>\n",
-                            "      <td>0.319</td>\n",
-                            "      <td>0.000</td>\n",
-                            "      <td>0.000</td>\n",
-                            "      <td>4866.0</td>\n",
-                            "      <td>4850.0</td>\n",
-                            "      <td>NaN</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>a</th>\n",
-                            "      <td>-0.999</td>\n",
-                            "      <td>0.002</td>\n",
-                            "      <td>-1.003</td>\n",
-                            "      <td>-0.996</td>\n",
-                            "      <td>0.000</td>\n",
-                            "      <td>0.000</td>\n",
-                            "      <td>5085.0</td>\n",
-                            "      <td>4869.0</td>\n",
-                            "      <td>NaN</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>sigma</th>\n",
-                            "      <td>0.010</td>\n",
-                            "      <td>0.001</td>\n",
-                            "      <td>0.007</td>\n",
-                            "      <td>0.012</td>\n",
-                            "      <td>0.000</td>\n",
-                            "      <td>0.000</td>\n",
-                            "      <td>4792.0</td>\n",
-                            "      <td>4901.0</td>\n",
-                            "      <td>NaN</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>hs[0, 0]</th>\n",
-                            "      <td>4.932</td>\n",
-                            "      <td>0.001</td>\n",
-                            "      <td>4.930</td>\n",
-                            "      <td>4.933</td>\n",
-                            "      <td>0.000</td>\n",
-                            "      <td>0.000</td>\n",
-                            "      <td>5105.0</td>\n",
-                            "      <td>4897.0</td>\n",
-                            "      <td>NaN</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>hs[1, 0]</th>\n",
-                            "      <td>9.517</td>\n",
-                            "      <td>0.098</td>\n",
-                            "      <td>9.326</td>\n",
-                            "      <td>9.694</td>\n",
-                            "      <td>0.001</td>\n",
-                            "      <td>0.001</td>\n",
-                            "      <td>4540.0</td>\n",
-                            "      <td>4761.0</td>\n",
-                            "      <td>NaN</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>hs[2, 0]</th>\n",
-                            "      <td>10.759</td>\n",
-                            "      <td>0.030</td>\n",
-                            "      <td>10.702</td>\n",
-                            "      <td>10.814</td>\n",
-                            "      <td>0.000</td>\n",
-                            "      <td>0.000</td>\n",
-                            "      <td>5003.0</td>\n",
-                            "      <td>4861.0</td>\n",
-                            "      <td>NaN</td>\n",
-                            "    </tr>\n",
-                            "  </tbody>\n",
-                            "</table>\n",
-                            "</div>"
-                        ],
-                        "text/plain": [
-                            "            mean     sd  hdi_3%  hdi_97%  mcse_mean  mcse_sd  ess_bulk  \\\n",
-                            "w[0]       0.968  0.001   0.965    0.971      0.000    0.000    4363.0   \n",
-                            "w[1]       0.072  0.004   0.065    0.079      0.000    0.000    5119.0   \n",
-                            "w[2]       0.308  0.006   0.297    0.319      0.000    0.000    4866.0   \n",
-                            "a         -0.999  0.002  -1.003   -0.996      0.000    0.000    5085.0   \n",
-                            "sigma      0.010  0.001   0.007    0.012      0.000    0.000    4792.0   \n",
-                            "hs[0, 0]   4.932  0.001   4.930    4.933      0.000    0.000    5105.0   \n",
-                            "hs[1, 0]   9.517  0.098   9.326    9.694      0.001    0.001    4540.0   \n",
-                            "hs[2, 0]  10.759  0.030  10.702   10.814      0.000    0.000    5003.0   \n",
-                            "\n",
-                            "          ess_tail  r_hat  \n",
-                            "w[0]        4715.0    NaN  \n",
-                            "w[1]        4678.0    NaN  \n",
-                            "w[2]        4850.0    NaN  \n",
-                            "a           4869.0    NaN  \n",
-                            "sigma       4901.0    NaN  \n",
-                            "hs[0, 0]    4897.0    NaN  \n",
-                            "hs[1, 0]    4761.0    NaN  \n",
-                            "hs[2, 0]    4861.0    NaN  "
-                        ]
-                    },
-                    "execution_count": 15,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "az.summary(trace, var_names=[\"w\", \"a\", \"sigma\", \"hs\"])"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "f4631ec0-4a76-4fe8-8566-b231f14fdaf3",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "Fitting this model is tricky. If the fit appears poor, here are some steps to try.\n",
-                "1. rerun the model, a new\n",
-                "1. try increasing the number of iterations.\n",
-                "1. try a strong prior on the breakpoints. For example, try `prior={'distribution':'normal', 'mu':[5, 9.5, 10.5], 'sigma':[1, 1, 0.2]})`, which implies we know the true breakpoint within +-0.5 ft.\n",
-                "1. finally, try fitting the model with another method.\n",
+                "import matplotlib.pyplot as plt\n",
+                "fig, ax = plt.subplots()\n",
+                "powerrating.plot(trace, ax=ax)\n",
                 "\n",
-                "ADVI typically underestimates uncertainty and struggles with multi-modal distributions.\n",
-                "NUTS may give better results but will be substantially slower to fit."
+                "# plot the original data for comparison\n",
+                "ax = sim_df.plot(x='q', y='stage', color='red', ls=':', legend=False)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
-            "id": "effa5602-34f5-45f2-8a38-2373b7efc044",
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# NUTS example. This may take several minutes, depending on your CPU.\n",
-                "# n = 4\n",
-                "# with powerrating:\n",
-                "#     trace = pm.sample(tune=1500, chains=n, cores=n, target_accept=0.95)\n",
-                "# \n",
-                "# powerrating.plot(trace)"
+                "az.summary(trace, var_names=[\"w\", \"a\", \"sigma\", \"hs\"])"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "15dca405-e2e7-4021-b271-f5c291c3c2c3",
             "metadata": {},
             "source": [
-                "## Parameterization\n",
-                "The segmented power law is defined as:\n",
-                "\n",
-                "\\begin{align}\n",
-                "    \\log(Q) = a + \\sum_{i=1}^{n} b_i \\log(x - x_{o,i}) H_i(x - x_{o,i})\n",
-                "\\end{align}\n",
-                "where\n",
-                "$Q$ is a vector discharge, \\\n",
-                "$n$ is the number of breakpoints in the rating, \\\n",
-                "$a$ and $b$ are model parameters, \\\n",
-                "$x$ is a vector of stage observations, \\\n",
-                "$x_o$ is a vector of breakpoints, and \\\n",
-                "$H$ is the Heaviside function. \n",
-                "\n",
-                "In a standard linear model $b$ represents the slope of the function with respect the input.\n",
-                "In the segmented power law $b_o$ is the slope and each subsequent $b_i$ are adjustment to the base slope for each segment."
+                "Fitting this model can be tricky.\n",
+                "The most common issue is a poor initialization of the breakpoints.\n",
+                "A fix is under development, but for now, try\n",
+                "1. reinitializing the model `PowerLawRating()`;\n",
+                "1. increasing the number of iterations `n`;\n",
+                "1. a prior on the breakpoints, example, try `prior={'distribution':'normal', 'mu':[5, 9.5, 10.5], 'sigma':[1, 1, 0.2]})`, which implies we know the true breakpoint within +-0.5 ft; or\n",
+                "1. fitting the model with NUTS `fit(method='nuts')`.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "172e914c-a12b-4704-a5d2-ed0e6de7f028",
             "metadata": {},
             "outputs": [],
-            "source": []
+            "source": [
+                "%load_ext watermark\n",
+                "%watermark -n -u -v -iv -w -p pytensor,xarray"
+            ]
         }
     ],
     "metadata": {
-        "colab": {
-            "name": "segmented_power_law_demo.ipynb",
-            "provenance": []
-        },
         "kernelspec": {
-            "display_name": "ratingcurve",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
-            "name": "ratingcurve"
+            "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.0"
-        },
-        "vscode": {
-            "interpreter": {
-                "hash": "8b9dd4e900aaf1c60d488d1bd44e4301837e8879016f95190f3ec6572ae5779a"
-            }
+            "version": "3.9.15"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 4
 }
```

### Comparing `ratingcurve-0.3.4/pyproject.toml` & `ratingcurve-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ratingcurve-0.3.4/ratingcurve/data/chalk_artificial.csv` & `ratingcurve-0.3.5/ratingcurve/data/chalk_artificial.csv`

 * *Files identical despite different names*

### Comparing `ratingcurve-0.3.4/ratingcurve/data/co_channel.csv` & `ratingcurve-0.3.5/ratingcurve/data/co_channel.csv`

 * *Files identical despite different names*

### Comparing `ratingcurve-0.3.4/ratingcurve/data/green_channel.csv` & `ratingcurve-0.3.5/ratingcurve/data/green_channel.csv`

 * *Files identical despite different names*

### Comparing `ratingcurve-0.3.4/ratingcurve/data/provo_natural.csv` & `ratingcurve-0.3.5/ratingcurve/data/provo_natural.csv`

 * *Files identical despite different names*

### Comparing `ratingcurve-0.3.4/ratingcurve/data/simulated_rating.csv` & `ratingcurve-0.3.5/ratingcurve/data/simulated_rating.csv`

 * *Files identical despite different names*

### Comparing `ratingcurve-0.3.4/ratingcurve/plot.py` & `ratingcurve-0.3.5/ratingcurve/plot.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,133 +1,256 @@
 """Plotting functions"""
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 import numpy as np
 import matplotlib.pyplot as plt
+import arviz as az
 
 from matplotlib.ticker import FuncFormatter
 
 if TYPE_CHECKING:
-    from .ratingmodel import PowerLawRating, SplineRating
     from arviz import InferenceData
+    from pandas import DataFrame
 
 
 DEFAULT_FIGSIZE = (5, 5)
+NARROW_LINE = 1
+REGULAR_LINE = NARROW_LINE * 1.5
+
+class RatingMixin:
+    """Parent class for other rating-related mixins
+    """
+    @property
+    def model(self):
+        raise NotImplementedError
+
+    @property
+    def trace(self) -> InferenceData:
+        """ArviZ InferenceData object
+
+        Returns
+        -------
+        ArviZ InferenceData object
+        """
+        return self.__last_trace
+    
+    @trace.setter
+    def trace(self, value):
+        self.__last_trace = value
+
+    def summary(self, trace: InferenceData=None, var_names: list=None) -> DataFrame:
+        """Summary of rating model parameters
+        
+        Parameters
+        ----------
+        trace : ArviZ InferenceData
+        var_names : list of str
+            List of variables to include in summary
+            
+        Returns
+        -------
+        DataFrame summary of rating model parameters
+        """
+        if trace is None:
+            trace = self.trace
+        return az.summary(trace, var_names)
 
 
-class PlotMixin:
+class PlotMixin(RatingMixin):
     """Mixin class for plotting rating models
     """
-    def setup_plot(rating, ax=None):
+    @staticmethod
+    def setup_plot(ax=None):
         """Plots rating curve
 
         Parameters
         ----------
-        trace : ArviZ InferenceData
+        ax : matplotlib axes
+
+        Returns
+        -------
         ax : matplotlib axes
         """
         if ax is None:
             fig, ax = plt.subplots(1, figsize=DEFAULT_FIGSIZE)
 
         return ax
+ 
+    def plot(self, trace: InferenceData=None, ax=None) -> None:
+        """Plots rating curve
+
+        Parameters
+        ----------
+        trace : ArviZ InferenceData
+        ax : matplotlib axes
+        """
+        if trace is None:
+            trace = self.trace
+
+        ax = self.setup_plot(ax=ax)
+        self._format_rating_plot(ax)
+
+        rating_table = self.table(trace)
+        h = rating_table['stage']
+        q = rating_table['discharge']
+        sigma = rating_table['gse']
+        ax.plot(q, h, color='black', lw=NARROW_LINE)
+        q_u = q * (sigma)**1.96  # this should be 2 sigma
+        q_l = q / (sigma)**1.96
+        ax.fill_betweenx(h, x1=q_u, x2=q_l, color='lightgray')
 
-    def plot_residuals(rating, trace: InferenceData, ax=None):
+        self.plot_gagings(ax=ax)
+
+    def plot_residuals(self, trace: InferenceData=None, ax=None) -> None:
         """Plots residuals
 
         Parameters
         ----------
         trace : ArviZ InferenceData
         ax : matplotlib axes
         """
-        ax = rating.setup_plot(ax=ax)
+        if trace is None:
+            trace = self.trace
+
+        ax = self.setup_plot(ax=ax)
+        self._format_rating_plot(ax)
 
         # TODO: this could be a function
-        if rating.q_sigma is not None:
-            q_sigma = rating.q_sigma
+        if self.q_sigma is not None:
+            q_sigma = self.q_sigma
         else:
             q_sigma = None
 
         # approximate percentage error
-        residuals = rating.residuals(trace) * 100
-        ax.errorbar(y=rating.h_obs, x=residuals, xerr=q_sigma*2*100, fmt="o", lw=1)
-        rating._format_residual_plot(ax)
+        residuals = self.residuals(trace) * 100
+        ax.errorbar(y=self.h_obs, x=residuals, xerr=q_sigma*2*100, fmt="o",
+                    lw=NARROW_LINE,
+                    markersize=4,
+                    markerfacecolor='none',
+                    markeredgecolor='black',
+                    ecolor='black')
+        self._format_residual_plot(ax)
+
+    def plot_gagings(self, ax=None) -> None:
+        """Plot gagings with uncertainty
+
+        Parameters
+        ----------
+        ax : matplotlib axes, optional
+        """
+        ax = self.setup_plot(ax=ax)
+
+        # TODO: safely get these
+        q_sigma = self.q_sigma
+        h_obs = self.h_obs
+        q_obs = self.q_obs
 
-    def _format_rating_plot(rating, ax):
+        if q_sigma is not None:
+            sigma_2 = 1.96 * (np.exp(q_sigma) - 1)*np.abs(q_obs)
+
+        else:
+            sigma_2 = 0
+
+        ax.errorbar(y=h_obs, x=q_obs, xerr=sigma_2, fmt="o", lw=1,
+                    color='black',
+                    markersize=4,
+                    markerfacecolor='none')
+        self._format_rating_plot(ax)
+
+    @staticmethod
+    def _format_rating_plot(ax) -> None:
         """Format rating plot
 
         Parameters
         ----------
         ax : matplotlib axes
         """
         ax.set_ylabel('Stage')
         ax.set_xlabel('Discharge')
         ax.get_xaxis().set_major_formatter(FuncFormatter(lambda x, p: format(int(x), ',')))
 
-    def _format_residual_plot(rating, ax):
+    @staticmethod
+    def _format_residual_plot(ax) -> None:
         """Format residual plot
 
         Parameters
         ----------
         ax : matplotlib axes
         """
         ax.set_ylabel('Stage')
         ax.set_xlabel('Percentage Error')
 
-        ax.axvline(0, color='grey', linestyle='solid')
+        ax.axvline(0, color='gray', linestyle='solid')
         xlim = ax.get_xlim()
         x_max = max(abs(xlim[0]), abs(xlim[1]))
         ax.set_xlim(-x_max, x_max)
 
 
 class SplinePlotMixin(PlotMixin):
     """Mixin class for plotting spline rating models
     """
-    def plot(self, trace: InferenceData, ax=None):
+    def plot(self, trace: InferenceData=None, ax=None):
         """Plots rating curve
 
         Parameters
         ----------
         trace : ArviZ InferenceData
         ax : matplotlib axes
         """
         ax = self.setup_plot(ax=ax)
-        self._format_rating_plot(ax)
-        _plot_spline_rating(self, trace, ax=ax)
+        self._plot_knots(ax=ax)
+        super().plot(trace, ax=ax)
+
+    def _plot_knots(self, ax):
+        """Plot spline knots
+
+        Parameters
+        ----------
+        ax : matplotlib axes
+        """
+        [ax.axhline(k, color='lightgray', linestyle='dotted', linewidth=NARROW_LINE) for k in self._dmatrix.knots]
 
 
 class PowerLawPlotMixin(PlotMixin):
     """Mixin class for plotting power law rating models
     """
-    def plot(self, trace: InferenceData, ax=None):
+    def plot(self, trace: InferenceData=None, ax=None):
         """Plots rating curve
 
         Parameters
         ----------
         trace : ArviZ InferenceData
         ax : matplotlib axes
+
+        TODO: this function might be cleaner as a wrapper around PlotMixin.plot
         """
+        if trace is None:
+            trace = self.trace
+
         ax = self.setup_plot(ax=ax)
-        self._format_rating_plot(ax)
         self._plot_transitions(trace, ax=ax)
-        _plot_power_law_rating(self, trace, ax=ax)
+        super().plot(trace, ax=ax)
 
-    def plot_residuals(self, trace: InferenceData, ax=None):
+    def plot_residuals(self, trace: InferenceData=None, ax=None):
         """Plots residuals
 
         Parameters
         ----------
         trace : ArviZ InferenceData
         ax : matplotlib axes
         """
+        if trace is None:
+            trace = self.trace
+
         ax = self.setup_plot(ax=ax)
         self._plot_transitions(trace, ax=ax)
         super().plot_residuals(trace, ax=ax)
 
-    def _plot_transitions(self, trace, ax):
+    def _plot_transitions(self, trace: InferenceData, ax):
         """Plot transitions (breakpoints)
 
         Parameters
         ----------
         trace : ArviZ InferenceData
             Inference data containing transition points (hs)
         ax : matplotlib axes
@@ -136,105 +259,8 @@
 
         alpha = 0.05
         hs_u = hs.mean(dim=['chain', 'draw']).data
         hs_lower = hs.quantile(alpha/2, dim=['chain', 'draw']).data.flatten()
         hs_upper = hs.quantile(1 - alpha/2, dim=['chain', 'draw']).data.flatten()
 
         [ax.axhspan(l, u, color='whitesmoke') for u, l in zip(hs_lower, hs_upper)]
-        [ax.axhline(u, color='grey', linestyle='dotted') for u in hs_u]
-
-
-def _plot_spline_rating(rating: SplineRating, trace: InferenceData, ax=None):
-    """Plots sline power law rating model
-
-    Parameters
-    ----------
-    rating : SplineRating
-        Spline rating model
-    trace : ArviZ InferenceData
-    ax : matplotlib axes
-
-    Returns
-    -------
-    figure, axes
-    """
-    q_obs = rating.q_obs
-    h_obs = rating.h_obs
-
-    if rating.q_sigma is not None:
-        q_sigma = rating.q_sigma
-    else:
-        q_sigma = None
-
-    _plot_gagings(h_obs, q_obs, q_sigma, ax=ax)
-
-    _plot_rating(rating.table(trace), ax=ax)
-
-
-def _plot_power_law_rating(rating: PowerLawRating, trace: InferenceData, ax=None):
-    """Plots segmented power law rating model
-
-    Parameters
-    ----------
-    rating : PowerLawRating
-    trace : ArviZ InferenceData
-    ax : matplotlib axes
-
-    Returns
-    -------
-    figure, axes
-    """
-    q_obs = rating.q_obs
-    h_obs = rating.h_obs
-
-    if rating.q_sigma is not None:
-        q_sigma = rating.q_sigma
-    else:
-        q_sigma = None
-
-    _plot_gagings(h_obs, q_obs, q_sigma, ax=ax)
-    _plot_rating(rating.table(trace), ax=ax)
-
-
-def _plot_rating(rating_table, ax=None):
-    """"Plot rating table with uncertainty
-
-    TODO This function is hack. Should be able to generate posterior predictions directly,
-    but this version of pymc seems to have bug.
-
-    Parameters
-    ----------
-    rating_table : pandas DataFrame
-    ax : matplotlib axes, optional
-    """
-    h = rating_table['stage']
-    q = rating_table['discharge']
-    sigma = rating_table['sigma']
-    ax.plot(q, h, color='black')
-    q_u = q * (sigma)**1.96  # this should be 2 sigma
-    q_l = q / (sigma)**1.96
-    ax.fill_betweenx(h, x1=q_u, x2=q_l, color='lightgray')
-
-
-def _plot_gagings(h_obs, q_obs, q_sigma=None, ax=None):
-    """Plot gagings with uncertainty
-
-    Parameters
-    ----------
-    h_obs : array-like
-        Stage observations.
-    q_obs : array-like
-        Discharge observations.
-    q_sigma : array-like, optional
-        Discharge uncertainty (1 sigma)
-    ax : matplotlib axes, optional
-    """
-    if ax is None:
-        fig, ax = plt.subplots(1, figsize=DEFAULT_FIGSIZE)
-
-    if q_sigma is not None:
-        sigma_2 = 1.96 * (np.exp(q_sigma) - 1)*np.abs(q_obs)
-
-    else:
-        sigma_2 = 0
-
-    ax.errorbar(y=h_obs, x=q_obs, xerr=sigma_2, fmt="o")
+        [ax.axhline(u, color='lightgray', linestyle='dotted', linewidth=NARROW_LINE) for u in hs_u]
```

### Comparing `ratingcurve-0.3.4/ratingcurve/ratingmodel.py` & `ratingcurve-0.3.5/ratingcurve/experimental.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,294 +1,238 @@
-"""Streamflow rating models"""
+"""Experimental streamflow rating models"""
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 import numpy as np
 import pymc as pm
 import arviz as az
 import pytensor.tensor as at
 
 from dataclasses import dataclass, asdict
 from pymc import Model
 from pandas import DataFrame
 
 
 from .transform import LogZTransform, Dmatrix
-from .plot import PowerLawPlotMixin, SplinePlotMixin
+#from .plot import PowerLawPlotMixin, SplinePlotMixin
+#from .sklearn import RegressorMixin
+from .ratingmodel import PowerLawRating, RatingData
 
 if TYPE_CHECKING:
     from arviz import InferenceData
     from numpy.typing import ArrayLike
 
 
-class Rating(Model):
-    """Abstract base class for rating models
+class ReitanRating(PowerLawRating):
+    """Experimental multi-segment power law rating using the Reitan parameterization.
+
+    Unlike Reitan Eq. 5, this version uses a fixed offset for each segment (ho).
     """
-    def __init__(self, name='', model=None):
-        """Initialize rating model
+    def __init__(
+        self,
+        q,
+        h,
+        segments,
+        prior={'distribution': 'uniform'},
+        q_sigma=None,
+        name='',
+        model=None):
+        """Create a multi-segment power law rating model
 
         Parameters
         ----------
-        name : str
-          Name that will be used as prefix for names of all random variables defined within model
+        q, h: array-like
+            Input arrays of discharge (q) and gage height (h) observations.
+        q_sigma : array-like
+            Input array of discharge uncertainty in units of discharge.
+        segments : int
+            Number of segments in the rating.
+        prior : dict
+            Prior knowledge of breakpoint locations.
         """
-        super().__init__(name, model)
-
-    def fit(self, method="advi", n=150_000):
-        mean_field = pm.fit(method=method, n=n, model=self.model)
-        return mean_field
-
-    def sample(self, n_samples, n_tune):
-        with self.model:
-            trace = pm.sample(50_000)
-        return trace
 
-    def table(self, trace, h=None, step=0.01, extend=1.1) -> DataFrame:
-        """Return stage-discharge rating table
+        super(PowerLawRating, self).__init__(q, h, name, model)
 
-        Parameters
-        ----------
-        trace : ArviZ InferenceData
-            Trace from MCMC sampling
-        h : array-like
-            Stage values to compute rating table. If None, then use the range of observations.
-        step : float
-            Step size for stage values
-        extend : float
-            Extend range of discharge values by this factor
+        self.segments = segments
+        self.prior = prior
+        self.q_obs = q
+        self.q_transform = LogZTransform(self.q_obs)
+        self.y = self.q_transform.transform(self.q_obs)
 
-        Returns
-        -------
-        DataFrame
-            Rating table with columns 'stage', 'discharge', and 'sigma'
-        """
-        if h is None:
-            h = stage_range(self.h_obs.min(), self.h_obs.max() * extend, step=step)
-            ratingdata = self.predict(trace, h)
-            table = DataFrame(asdict(ratingdata))
-            table = table[table['discharge'] <= self.q_obs.max() * extend]
+        COORDS = {"obs": np.arange(len(self.y)), "splines": np.arange(segments)}
+        self.add_coords(COORDS)
 
+        # transform observational uncertainty to log scale
+        if q_sigma is None:
+            self.q_sigma = 0
         else:
-            ratingdata = self.predict(trace, h)
-            table = DataFrame(asdict(ratingdata))
+            self.q_sigma = np.log(1 + q_sigma/q)
 
-        return table.round({'discharge': 2, 'stage': 2, 'sigma': 4})
-    
-    def residuals(self, trace: InferenceData) -> ArrayLike:
-        """Compute residuals of rating model
+        self.h_obs = h
 
-        Parameters
-        ----------
-        trace : arviz.InferenceData
-          Arviz ``InferenceData`` object containing posterior samples of model parameters.
+        # observations
+        h = pm.MutableData("h", self.h_obs)
+        q_sigma = pm.MutableData("q_sigma", self.q_sigma)
+
+        # fixed parameters
+        # taking the log of h0_offset produces the clipping boundaries in Fig 1, from Reitan et al. 2019
+        self._ho = np.ones((self.segments, 1))
+        self._ho[0] = 0
+
+        # priors
+        # see Le Coz 2014 for default values, but typically between 1.5 and 2.5
+        #w = pm.Normal("w", mu=1.6, sigma=0.5, dims="splines")
+        w = pm.TruncatedNormal("w", mu=1.6, sigma=1.0, lower=0.1, dims="splines") # lower is somewhat arbitrary
+        a = pm.Normal("a", mu=0, sigma=2)
+
+        # set priors on break points
+        if self.prior['distribution'] == 'normal':
+            hs = self.set_normal_prior()
+        elif self.prior['distribution'] == 'uniform':
+            hs = self.set_uniform_prior()
+        else:
+            raise NotImplementedError('Prior distribution not implemented')
+
+        # likelihood
+        ho = self._ho
+        inf = at.constant([np.inf], dtype='float64').reshape((-1, 1 ))
+        hs1 = at.concatenate([hs, inf])
+
+        b = at.log( at.clip(h - hs, 0, hs1[1:] - hs) + ho) #best but suspect ho is accumulating (ho added to each segment)
+        sigma = pm.HalfCauchy("sigma", beta=0.1)
+        mu = pm.Normal("mu", a + at.dot(w, b), sigma + q_sigma, observed=self.y)
 
-        Returns
-        -------
-        residuals : array-like
-          Log residuals of rating model
-        """
-        q_pred = self.predict(trace, self.h_obs).discharge
-        return np.array(np.log(self.q_obs) - np.log(q_pred))
-    
     def predict(self, trace: InferenceData, h: ArrayLike) -> RatingData:
         """Predicts values of new data with a trained rating model
 
         Parameters
         ----------
-        trace : arviz.InferenceData
-          Arviz ``InferenceData`` object containing posterior samples of model parameters.
+        trace : ArviZ InferenceData
         h : array-like
-          Stages at which to predict discharge.
+            Stages at which to predict discharge.
 
         Returns
         -------
         RatingData
-            dataclass with stage, discharge, and sigma.
-        """
-        raise NotImplementedError
-
-    def save(self, filename: str) -> None:
-        """Save model to file
-        """
-        raise NotImplementedError
-
-    @staticmethod
-    def load(filename: str) -> Model:
-        """Load a saved model
+            Dataframe with columns 'stage', 'discharge', and 'sigma' containing predicted discharge and uncertainty.
         """
-        raise NotImplementedError
+        trace = az.extract(trace)
+        sample = trace.sample.shape[0]
+        a = trace['a'].values
+        w = trace['w'].values
+        w2 = np.expand_dims(w.T, -1) #FIX
+        hs = np.moveaxis(trace['hs'].values, -1, 0)
+        sigma = trace['sigma'].values
 
-    def _format_ratingdata(self, h: ArrayLike, q_z: ArrayLike) -> RatingData:
-        """Helper function that formats RatingData
+        clips = np.zeros((hs.shape[1], 1))
+        clips[0] = -np.inf
+        h_tile = np.tile(h, sample).reshape(sample, 1, -1)
 
-        Parameters
-        ----------
-        h : array-like
-            Stage values.
-        q_z : array-like
-            Predicted discharge values.
+        ho = self._ho
+        inf = np.array(np.inf).reshape(-1, 1)
+        hs1 = np.pad(hs, ((0,0), (0,1), (0,0)), 'constant', constant_values=np.inf )
+        b = np.log( np.clip(h - hs, 0, hs1[:,1:] - hs) + ho)
+        q_z = a + (b*w2).sum(axis=1).T
+        e = np.random.normal(0, sigma, sample)
 
-        Returns
-        -------
-        RatingData
-            dataclass with stage, discharge, and sigma.
-        """
-        transform = self.q_transform
+        return self._format_ratingdata(h=h, q_z=q_z+e)
 
-        return RatingData(stage=h.squeeze(),
-                          discharge=transform.mean(q_z).squeeze(),
-                          sigma=transform.sigma(q_z).squeeze())
 
+class LeCozRating(PowerLawRating):
+    """Experimental multi-segment power law rating using the LeCoz (2014) parameterization.
 
-class PowerLawRating(Rating, PowerLawPlotMixin):
-    """Multi-segment power law rating using Heaviside parameterization.
     """
     def __init__(
         self,
         q,
         h,
         segments,
         prior={'distribution': 'uniform'},
         q_sigma=None,
+        m=None,
         name='',
         model=None):
         """Create a multi-segment power law rating model
 
         Parameters
         ----------
         q, h: array-like
             Input arrays of discharge (q) and gage height (h) observations.
         q_sigma : array-like
             Input array of discharge uncertainty in units of discharge.
+        m : array-like
+            Hydrologic control matrix.
         segments : int
             Number of segments in the rating.
         prior : dict
             Prior knowledge of breakpoint locations.
         """
 
-        super().__init__(name, model)
+        super(PowerLawRating, self).__init__(q, h, name, model)
 
         self.segments = segments
         self.prior = prior
         self.q_obs = q
         self.q_transform = LogZTransform(self.q_obs)
         self.y = self.q_transform.transform(self.q_obs)
 
+        COORDS = {"obs": np.arange(len(self.y)), "splines": np.arange(segments)}
+        self.add_coords(COORDS)
+
         # transform observational uncertainty to log scale
         if q_sigma is None:
             self.q_sigma = 0
         else:
             self.q_sigma = np.log(1 + q_sigma/q)
 
-        self.h_obs = h
-
-        self._inf = [np.inf]
-
-        # clipping boundary
-        clips = np.zeros((self.segments, 1))
-        clips[0] = -np.inf
-        self._clips = at.constant(clips)
-
-        # create h0 offsets
-        self._h0_offsets = np.ones((self.segments, 1))
-        self._h0_offsets[0] = 0
-
-        self.COORDS = {"obs": np.arange(len(self.y)), "splines": np.arange(segments)}
-
-        # compute initval
-        self._hs_lower_bounds = np.zeros((self.segments, 1)) + self.h_obs.min()
-        self._hs_lower_bounds[0] = 0
-
-        self._hs_upper_bounds = np.zeros((self.segments, 1)) + self.h_obs.max()
-        self._hs_upper_bounds[0] = self.h_obs.min() - 1e-6 # TODO compute threshold
-
-        # set random init on unit interval then scale based on bounds
-        self._setup_powerlaw()
-
-    def set_normal_prior(self):
-        """Normal prior for breakpoints
-
-        Sets an expected value for each breakpoint (mu) with uncertainty (sigma).
-        This can be very helpful when convergence is poor.
-
-        prior={'distribution': 'normal', 'mu': [], 'sigma': []}
-        """
-        with Model(coords=self.COORDS) as model:
-
-            self._init_hs = np.sort(np.array(self.prior['mu']))
-            self._init_hs = self._init_hs.reshape((self.segments, 1))
-
-            prior_mu = np.array(self.prior['mu']).reshape((self.segments, 1))
-            prior_sigma = np.array(self.prior['sigma']).reshape((self.segments, 1))
-
-            hs_ = pm.TruncatedNormal('hs_',
-                                     mu=prior_mu,
-                                     sigma=prior_sigma,
-                                     lower=self._hs_lower_bounds,
-                                     upper=self._hs_upper_bounds,
-                                     shape=(self.segments, 1),
-                                     initval=self._init_hs)
-
-            hs = pm.Deterministic('hs', at.sort(hs_, axis=0))
-        return hs
-
-    def set_uniform_prior(self):
-        """Uniform prior for breakpoints
-
-        Make no prior assumption about the location of the breakpoints, only their number.
-
-        prior={distribution:'uniform', initval: []}
-
-        TODO: clean this up
-        """
-        self._init_hs = self.prior.get('initval', None)
-
-        if self._init_hs is None:
-            self._init_hs = np.random.rand(self.segments, 1) \
-                * (self._hs_upper_bounds - self._hs_lower_bounds) \
-                + self._hs_lower_bounds
-            self._init_hs = np.sort(self._init_hs, axis=0)  # not necessary?
-
+        if m is None:
+            self.m = np.eye(self.segments)
         else:
-            self._init_hs = np.sort(np.array(self._init_hs)).reshape((self.segments, 1))
+            self.m = at.constant(m)
 
-        with Model(coords=self.COORDS) as model:
-            hs_ = pm.Uniform('hs_',
-                             lower=self._hs_lower_bounds,
-                             upper=self._hs_upper_bounds,
-                             shape=(self.segments, 1),
-                             initval=self._init_hs)
-
-            # Sorting reduces multimodality. The benifit increases with fewer observations.
-            hs = pm.Deterministic('hs', at.sort(hs_, axis=0))
-
-        return hs
-
-    def _setup_powerlaw(self):
-        """Helper function that defines model
-        """
-        with Model(coords=self.COORDS) as model:
-            h = pm.MutableData("h", self.h_obs)
-            w_mu = np.zeros(self.segments)
-            # see Le Coz 2014 for default values, but typical between 1.5 and 2.5
-            w_mu[0] = 1.6 
-            w = pm.Normal("w", mu=w_mu, sigma=0.5, dims="splines")
-            a = pm.Normal("a", mu=0, sigma=2)
-
-            # set prior on break points
-            if self.prior['distribution'] == 'normal':
-                hs = self.set_normal_prior()
-            else:
-                hs = self.set_uniform_prior()
+        self.h_obs = h
+        # observations
+        h = pm.MutableData("h", self.h_obs)
+        q_sigma = pm.MutableData("q_sigma", self.q_sigma)
+
+        # fixed parameters
+        # taking the log of h0_offset produces the clipping boundaries in Fig 1, from Reitan et al. 2019
+        #self._ho = np.ones((self.segments, 1))
+        #self._ho[0] = 0
+
+        # priors
+        # see Le Coz 2014 for default values, but typically between 1.5 and 2.5
+        #w = pm.Normal("w", mu=1.6, sigma=0.5, dims="splines")
+        w = pm.TruncatedNormal("w", mu=1.6, sigma=1.0, lower=0.1, dims="splines") # lower is somewhat arbitrary
+        a = pm.Normal("a", mu=0, sigma=3, dims="splines")
+
+        # set priors on break points
+        if self.prior['distribution'] == 'normal':
+            hs = self.set_normal_prior()
+        elif self.prior['distribution'] == 'uniform':
+            hs = self.set_uniform_prior()
+        else:
+            raise NotImplementedError('Prior distribution not implemented')
 
-            h0 = hs - self._h0_offsets
-            b = pm.Deterministic('b', at.switch(at.le(h, hs), self._clips, at.log(h-h0)))
+        # likelihood
+        inf = at.constant([np.inf], dtype='float64').reshape((-1, 1 ))
+        hs1 = at.concatenate([hs, inf])
+
+        #i = at.switch( (h > hs) & (h <= hs1[1:]), 1, 0)
+        #x = at.clip( h - hs, 1e-6, hs1[1:] - hs )
+        #b = a + w * at.log(x).T
+        ##q = at.sum(i * at.dot(self.m, at.exp(b.T)), axis=0)
+        #q = at.sum(i * at.exp(b.T), axis=0)
+        i = at.switch( (h > hs) & (h <= hs1[1:]), 1, 0)
+        x = at.clip( h - hs, 1e-6, hs1[1:] - hs )
+        b = at.exp(a) * (x).T**w
+        q = at.sum(i * at.dot(self.m, b.T), axis=0)
 
-            sigma = pm.HalfCauchy("sigma", beta=1) + self.q_sigma
-            mu = pm.Normal("mu", a + at.dot(w, b), sigma, observed=self.y)
+        sigma = pm.HalfCauchy("sigma", beta=0.1)
+        mu = pm.Normal("mu", at.log(q), sigma + q_sigma, observed=self.y)
 
     def predict(self, trace: InferenceData, h: ArrayLike) -> RatingData:
         """Predicts values of new data with a trained rating model
 
         Parameters
         ----------
         trace : ArviZ InferenceData
@@ -308,133 +252,132 @@
         hs = np.moveaxis(trace['hs'].values, -1, 0)
         sigma = trace['sigma'].values
 
         clips = np.zeros((hs.shape[1], 1))
         clips[0] = -np.inf
         h_tile = np.tile(h, sample).reshape(sample, 1, -1)
 
-        h0_offset = np.ones_like(clips)
-        h0_offset[0] = 0
-        h0 = hs - h0_offset
-        b1 = np.where(h_tile <= hs, clips, np.log(h_tile-h0))
-        q_z = a + (b1*w2).sum(axis=1).T 
+        ho = self._ho
+        inf = np.array(np.inf).reshape(-1, 1)
+        hs1 = np.pad(hs, ((0,0), (0,1), (0,0)), 'constant', constant_values=np.inf )
+        b = np.log( np.clip(h - hs, 0, hs1[:,1:] - hs) + ho)
+        q_z = a + (b*w2).sum(axis=1).T
         e = np.random.normal(0, sigma, sample)
 
         return self._format_ratingdata(h=h, q_z=q_z+e)
 
 
-class SplineRating(Rating, SplinePlotMixin):
-    """Natural spline rating model
-    """
 
-    def __init__(self, q, h, q_sigma=None, mean=0, sd=1, df=5, name='', model=None):
-        """Create a natural spline rating model
+class ISORating(PowerLawRating):
+    """Experimental multi-segment power law rating using the Reitan parameterization.
+
+    Unlike Reitan Eq. 5, this version uses a fixed offset for each segment (ho).
+    """
+    def __init__(
+        self,
+        q,
+        h,
+        segments,
+        prior={'distribution': 'uniform'},
+        q_sigma=None,
+        name='',
+        model=None):
+        """Create a multi-segment power law rating model
 
         Parameters
         ----------
         q, h: array-like
-            Input arrays of discharge (q) and stage (h) observations.
-        q_sigma : array-like, optional
+            Input arrays of discharge (q) and gage height (h) observations.
+        q_sigma : array-like
             Input array of discharge uncertainty in units of discharge.
-        knots : arrak-like
-            Stage value locations of the spline knots.
-        mean, sd : float
-            Prior mean and standard deviation for the spline coefficients.
-        df : int
-            Degrees of freedom for the spline coefficients.
+        segments : int
+            Number of segments in the rating.
+        prior : dict
+            Prior knowledge of breakpoint locations.
         """
-        super().__init__(name, model)
+
+        super(PowerLawRating, self).__init__(q, h, name, model)
+
+        self.segments = segments
+        self.prior = prior
         self.q_obs = q
-        self.h_obs = h
         self.q_transform = LogZTransform(self.q_obs)
         self.y = self.q_transform.transform(self.q_obs)
 
+        COORDS = {"obs": np.arange(len(self.y)), "splines": np.arange(segments)}
+        self.add_coords(COORDS)
+
         # transform observational uncertainty to log scale
         if q_sigma is None:
             self.q_sigma = 0
         else:
             self.q_sigma = np.log(1 + q_sigma/q)
 
-        self._dmatrix = Dmatrix(self.h_obs, df, 'cr')
-        self.d_transform = self._dmatrix.transform
-
-        self.B = self.d_transform(h)
-        B = pm.MutableData("B", self.B)
+        self.h_obs = h
 
-        COORDS = {"obs": np.arange(len(self.y)), "splines": np.arange(self.B.shape[1])}
-        self.add_coords(COORDS)
+        # observations
+        h = pm.MutableData("h", self.h_obs)
+        q_sigma = pm.MutableData("q_sigma", self.q_sigma)
+
+        # priors
+        # see Le Coz 2014 for default values, but typically between 1.5 and 2.5
+        w = pm.TruncatedNormal("w", mu=2, sigma=0.4, lower=0.5, dims="splines") # lower is somewhat arbitrary
+        a = pm.Normal("a", mu=0, sigma=3, dims='splines') # a is scale dependent
+        #TEST a = pm.Normal("a", mu=0, sigma=3) # a is scale dependent
+
+        # set priors on break points
+        if self.prior['distribution'] == 'normal':
+            hs = self.set_normal_prior()
+        elif self.prior['distribution'] == 'uniform':
+            hs = self.set_uniform_prior()
+        else:
+            raise NotImplementedError('Prior distribution not implemented')
 
-        w = pm.Normal("w", mu=mean, sigma=sd, dims="splines")
+        # likelihood
+        inf = at.constant([np.inf], dtype='float64').reshape((-1, 1 ))
+        hs1 = at.concatenate([hs, inf])
+        x = at.clip(h - hs, 1e-6, hs1[1:] - hs) # could use at.switch instead
+        #TEST b = at.exp(w * at.log(x.T))
+        #TEST q = a + at.log(at.sum(b, axis=1))
+        b = at.exp(a + w * at.log(x.T))
+        q = at.log(at.sum(b, axis=1))
 
-        sigma = pm.HalfCauchy("sigma", beta=1) + self.q_sigma
-        mu = pm.Normal("mu", at.dot(B, w.T), sigma, observed=self.y, dims="obs")
+        sigma = pm.HalfCauchy("sigma", beta=0.1)
+        mu = pm.Normal("mu", q, sigma + q_sigma, observed=self.y)
 
     def predict(self, trace: InferenceData, h: ArrayLike) -> RatingData:
         """Predicts values of new data with a trained rating model
 
         Parameters
         ----------
         trace : ArviZ InferenceData
         h : array-like
             Stages at which to predict discharge.
 
         Returns
         -------
         RatingData
-            dataclass with stage, discharge, and sigma.
+            Dataframe with columns 'stage', 'discharge', and 'sigma' containing predicted discharge and uncertainty.
         """
         trace = az.extract(trace)
         sample = trace.sample.shape[0]
-        w = trace['w'].values.squeeze()
-        B = self.d_transform(h)
+        a = trace['a'].values
+        w = trace['w'].values
+        w2 = np.expand_dims(w.T, -1) #FIX
+        hs = np.moveaxis(trace['hs'].values, -1, 0)
         sigma = trace['sigma'].values
-        q_z = np.dot(B, w)
-        e = np.random.normal(0, sigma, sample)
-
-        return self._format_ratingdata(h=h, q_z=q_z+e)
-
-
-@dataclass
-class RatingData():
-    """Dataclass for rating model output
-    Attributes
-    ----------
-    stage : array-like
-        Stage values.
-    discharge : array-like
-        Discharge values.
-    sigma : array-like
-        Discharge uncertainty.
-    """
-    stage: ArrayLike
-    discharge: ArrayLike
-    sigma: ArrayLike
-
-
-def stage_range(minimum: float, maximum: float, step: float = 0.01):
-    """Returns a range of stage values
-
-    To compute the range, round down (up) to the nearest step for
-    the minumum (maximum).
 
-    Parameters
-    ----------
-    h_min, h_max : float
-        Minimum and maximum stage (h) observations.
-    """
-    start = minimum - (minimum % step)
-    stop = maximum + (maximum % step)
-
-    return np.arange(start, stop, step)
+        clips = np.zeros((hs.shape[1], 1))
+        clips[0] = -np.inf
+        h_tile = np.tile(h, sample).reshape(sample, 1, -1)
 
+        inf = np.array(np.inf).reshape(-1, 1)
+        hs1 = np.pad(hs, ((0,0), (0,1), (0,0)), 'constant', constant_values=np.inf )
 
-def compute_knots(minimum: float, maximum: float, n: int):
-    """Return list of spline knots
+        x = np.clip(h - hs, 1e-6, hs1[:,1:] - hs)
+        #b = at.switch(h > hs, at.exp(a + w * at.log(x.T)), 0 )
+        b = np.exp(a + w * np.log(x.T))
+        q_z = np.log(np.sum(b, axis=1))
+        e = np.random.normal(0, sigma, sample)
 
-    Parameters
-    ----------
-    minimum, maximum : float
-        Minimum and maximum stage (h) observations.
-    n : int
-        Number of knots.
-    """
-    return np.linspace(minimum, maximum, n)
+        return self._format_ratingdata(h=h, q_z=q_z+e)
+
```

### Comparing `ratingcurve-0.3.4/ratingcurve/transform.py` & `ratingcurve-0.3.5/ratingcurve/transform.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,23 +35,14 @@
             Transformed data.
         """
         return x
 
     def untransform(self, x: ArrayLike) -> ArrayLike:
         return x
 
-    def mean(self):
-        raise NotImplementedError
-
-    def sigma(self):
-        raise NotImplementedError
-
-    def median(self):
-        raise NotImplementedError
-
 
 class ZTransform(Transform):
     """Z-transforms data to have zero mean and unit variance
     """
 
     def __init__(self, x: ArrayLike):
         """Create a ZTransform object
@@ -140,62 +131,14 @@
         -------
         ArrayLike
             log z-scores transformed back to original units.
         """
         log_x = super().untransform(z)
         return np.exp(log_x)
 
-    def mean(self, z: ArrayLike, axis: int = 1) -> ArrayLike:
-        """Compute mean.
-
-        Parameters
-        ----------
-        z : array_like
-          Transformed data.
-
-        Returns
-        -------
-        ArrayLike
-            Arithmetic mean.
-        """
-        x = self.untransform(z)
-        return x.mean(axis=axis)
-
-    def sigma(self, z: ArrayLike, axis: int = 1) -> ArrayLike:
-        """Compute standard deviation.
-
-        Parameters
-        ----------
-        z : array_like
-          Transformed data.
-
-        Returns
-        -------
-        ArrayLike
-            Multiplicative standard deviation.
-        """
-        sigma = z.std(axis=axis)
-        return np.exp(sigma)
-    
-    def median(self, z: ArrayLike, axis: int = 1) -> ArrayLike:
-        """Compute median.
-
-        Parameters
-        ----------
-        z : array_like
-          Transformed data.
-
-        Returns
-        -------
-        ArrayLike
-            Median or geometric mean.
-        """
-        x = self.untransform(z)
-        return x.median(axis=axis)
-
 
 class UnitTransform(Transform):
     """Transforms data to the unit (0 to 1) interval.
     """
     def __init__(self, x: ArrayLike):
         """Create UnitTransform of array
 
@@ -236,26 +179,34 @@
         """
         return x*self.max_
 
 
 class Dmatrix():
     """Transform for spline design matrix
     """
-    def __init__(self, stage: ArrayLike, df: int, form: str = 'cr'):
+    def __init__(self, stage: ArrayLike, df: int, form: str = 'cr') -> None:
         """Create a Dmatrix object
+
+        Create a design matrix for a natural cubic spline, which is a cubic
+        spline that is additionally constrained to be linear at the boundaries.
+        Due to this constraint, the total degrees of freedom equals the number
+        of knots minus 1.
         
         Parameters
         ----------
         stage : array_like
           Stage data
         df : int
           Degrees of freedom
         form : str
           Spline form
+
         """
+        n_knots = df - 1
+        self.knots = compute_knots(stage.min(), stage.max(), n=n_knots)
         temp = dmatrix(f"{form}(stage, df={df}) - 1", {"stage": stage})
         self.design_info = temp.design_info
 
     def transform(self, stage: ArrayLike) -> ArrayLike:
         """Transform stage using spline design matrix
  
         Parameters
@@ -265,7 +216,25 @@
 
         Returns
         -------
         ArrayLike
             Transformed data
         """
         return np.asarray(build_design_matrices([self.design_info], {"stage": stage})).squeeze()
+
+
+def compute_knots(minimum: float, maximum: float, n: int) -> ArrayLike:
+    """Return list of spline knots
+
+    Parameters
+    ----------
+    minimum, maximum : float
+        Minimum and maximum stage (h) observations.
+    n : int
+        Number of knots.
+
+    Returns
+    -------
+    ArrayLike
+        List of spline knots.
+    """
+    return np.linspace(minimum, maximum, n)
```

### Comparing `ratingcurve-0.3.4/ratingcurve.egg-info/PKG-INFO` & `ratingcurve-0.3.5/ratingcurve.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratingcurve
-Version: 0.3.4
+Version: 0.3.5
 Summary: A library for fitting multi-segment stage-discharge rating curves.
 Maintainer-email: Timothy Hodson <thodson@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, this project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -56,75 +56,63 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
 
 # ratingcurve
-*A Python library for fitting stage-discharge rating curves.*
+*A Python library for fitting hydrologic rating curves.*
 
-Use `ratingcurve` to fit streamflow ratings with a segmented power law,
-which is the the most common model used by USGS.
-
-At this time, the library is for research and is not ready for operation. 
+In hydrology, a rating curve is a mathematical relationship between streamflow and water surface elevation (stage).
+Because stage is much easier to measure than streamflow, almost all streamflow timeseries are generated from rating curves.
+Historically, those ratings were fitted by hand, which can be time consuming and error prone.
+`ratingcurve` provides an easy-to-use algorithm for fitting the standard form of rating curve, the segmented power law.
 
 ## Installation
 Install using pip
 ```sh
 pip install ratingcurve
 ```
 or conda
 ```sh
-# acreate a new environment
-conda create -n ratingcurve
-conda activate ratingcurve
 conda install -c conda-forge ratingcurve
-# add environment to jupyter
-python -m ipykernel install --user --name=ratingcurve
 ```
 
 ## Getting Started
-The [`segmented-power-law-demo.ipynb`](https://github.com/thodson-usgs/ratingcurve/blob/main/notebooks/segmented-power-law-demo.ipynb)
-notebook demonstrates basic use of the package.
-You can try it out in Google Colab
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/thodson-usgs/ratingcurve/blob/master/notebooks/segmented-power-law-demo.ipynb)
-
-or locally using the environment created in the previous step
-```sh
-conda activate base # or your prefered jupyter lab environment
-jupyter lab
-```
-then open the notebook and select the `ratingcurve` kernel that was installed earlier.
-
-A simple example is given below.
+This [`tutorial`](https://github.com/thodson-usgs/ratingcurve/blob/main/docs/notebooks/segmented-power-law-tutorial.ipynb)
+notebook demonstrates basic usage of the package.
+Try it locally or in Colab.
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/thodson-usgs/ratingcurve/blob/main/docs/notebooks/segmented-power-law-tutorial.ipynb)
 
 ```python
 from ratingcurve.ratingmodel import PowerLawRating
 from ratingcurve import data
 
 # load tutorial data
 df = data.load('green channel')
 
-# setup model
-segments = 2
+# initialize the model
 powerrating = PowerLawRating(q=df['q'],
                              h=df['stage'], 
                              q_sigma=df['q_sigma'],
-                             segments=segments)
+                             segments=2)
                                    
-# fit model, then simulate the rating
-with powerrating:
-    mean_field = pm.fit(n=150_000)
-    trace = mean_field.sample(5000)
-    
+# fit the model
+trace = powerrating.fit()
 powerrating.plot(trace)
 ```
-![example plot](https://github.com/thodson-usgs/ratingcurve/blob/main/paper/green_example.png?raw=true)
+![example plot](https://github.com/thodson-usgs/ratingcurve/blob/main/docs/assets/green-channel-rating-plot.png?raw=true)
+
+
+Generate a rating table that can be imported into other applications.
+```python
+powerating.table(trace)
+```
 
-See the [notebooks](https://github.com/thodson-usgs/ratingcurve/tree/main/notebooks) for more examples.
+For more, see the [documentation](https://thodson-usgs.github.io/ratingcurve/meta/intro.html).
 
 ## Disclaimer
 
 This software is preliminary or provisional and is subject to revision. 
 It is being provided to meet the need for timely best science.
 The software has not received final approval by the U.S. Geological Survey (USGS).
 No warranty, expressed or implied, is made by the USGS or the U.S. Government as to the functionality of the software and related material nor shall the fact of release constitute any such warranty.
```

### Comparing `ratingcurve-0.3.4/ratingcurve.egg-info/SOURCES.txt` & `ratingcurve-0.3.5/ratingcurve.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,32 +11,52 @@
 requirements.txt
 setup.py
 .devcontainer/Dockerfile
 .devcontainer/devcontainer.json
 .devcontainer/noop.txt
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/review-checklist.md
+.github/workflows/deploy-book.yml
 .github/workflows/python-package.yml
 .github/workflows/python-publish.yml
-notebooks/model-evaluation-demo.ipynb
-notebooks/segmented-power-law-demo.ipynb
-notebooks/spline-demo.ipynb
-paper/green_example.png
+docs/_config.yml
+docs/_toc.yml
+docs/api.rst
+docs/references.bib
+docs/requirements-doc.txt
+docs/assets/green-channel-rating-plot.png
+docs/meta/background.md
+docs/meta/implementation.md
+docs/meta/installation.md
+docs/meta/intro.md
+docs/meta/troubleshooting.md
+docs/meta/tutorials.md
+docs/notebooks/getting-started-tutorial.ipynb
+docs/notebooks/model-selection-tutorial.ipynb
+docs/notebooks/segmented-power-law-tutorial.ipynb
+docs/notebooks/spline-tutorial.ipynb
 ratingcurve/__init__.py
 ratingcurve/_version.py
+ratingcurve/experimental.py
 ratingcurve/plot.py
 ratingcurve/ratingmodel.py
+ratingcurve/sklearn.py
 ratingcurve/transform.py
 ratingcurve.egg-info/PKG-INFO
 ratingcurve.egg-info/SOURCES.txt
 ratingcurve.egg-info/dependency_links.txt
 ratingcurve.egg-info/requires.txt
 ratingcurve.egg-info/top_level.txt
 ratingcurve/data/__init__.py
 ratingcurve/data/chalk_artificial.csv
+ratingcurve/data/chalk_artificial.md
 ratingcurve/data/co_channel.csv
+ratingcurve/data/co_channel.md
 ratingcurve/data/green_channel.csv
+ratingcurve/data/green_channel.md
 ratingcurve/data/provo_natural.csv
+ratingcurve/data/provo_natural.md
 ratingcurve/data/simulated_rating.csv
+ratingcurve/data/simulated_rating.md
 ratingcurve/tests/__init__.py
 ratingcurve/tests/test_ratingmodel.py
 ratingcurve/tests/test_transform.py
```

