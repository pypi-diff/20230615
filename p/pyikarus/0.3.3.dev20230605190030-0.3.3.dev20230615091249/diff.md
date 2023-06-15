# Comparing `tmp/pyikarus-0.3.3.dev20230605190030.tar.gz` & `tmp/pyikarus-0.3.3.dev20230615091249.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyikarus-0.3.3.dev20230605190030.tar", last modified: Mon Jun  5 19:00:31 2023, max compression
+gzip compressed data, was "pyikarus-0.3.3.dev20230615091249.tar", last modified: Thu Jun 15 09:12:50 2023, max compression
```

## Comparing `pyikarus-0.3.3.dev20230605190030.tar` & `pyikarus-0.3.3.dev20230615091249.tar`

### file list

```diff
@@ -1,332 +1,333 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.169671 pyikarus-0.3.3.dev20230605190030/
--rw-r--r--   0 root         (0) root         (0)      312 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/.bettercodehub.yml
--rw-r--r--   0 root         (0) root         (0)     1300 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/.clang-format
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/.cmake-format
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.121669 pyikarus-0.3.3.dev20230605190030/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.129669 pyikarus-0.3.3.dev20230605190030/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      460 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 root         (0) root         (0)      615 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.129669 pyikarus-0.3.3.dev20230605190030/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      489 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/.github/workflows/codespell.yml
--rw-r--r--   0 root         (0) root         (0)     1034 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/.github/workflows/createDockerContainer.yml
--rw-r--r--   0 root         (0) root         (0)     5615 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/.github/workflows/createRelease.yml
--rw-r--r--   0 root         (0) root         (0)     1834 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/.github/workflows/debian-coverage.yml
--rw-r--r--   0 root         (0) root         (0)     2612 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/.github/workflows/debian.yml
--rw-r--r--   0 root         (0) root         (0)     2042 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/.github/workflows/ghpages.yml
--rw-r--r--   0 root         (0) root         (0)     1712 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/.github/workflows/releasePythonPackage.yml
--rw-r--r--   0 root         (0) root         (0)      314 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/.github/workflows/reuseLint.yml
--rw-r--r--   0 root         (0) root         (0)     3335 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/.github/workflows/runExamples.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.129669 pyikarus-0.3.3.dev20230605190030/.github/workflows/scripts/
--rw-r--r--   0 root         (0) root         (0)     3071 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/.github/workflows/scripts/release.py
--rw-r--r--   0 root         (0) root         (0)     1331 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/.github/workflows/style.yml
--rw-r--r--   0 root         (0) root         (0)      482 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.129669 pyikarus-0.3.3.dev20230605190030/.reuse/
--rw-r--r--   0 root         (0) root         (0)      661 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/.reuse/dep5
--rw-r--r--   0 root         (0) root         (0)     3829 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1251 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5335 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)      784 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/LICENSE.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.133669 pyikarus-0.3.3.dev20230605190030/LICENSES/
--rw-r--r--   0 root         (0) root         (0)    18375 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 root         (0) root         (0)     7048 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/LICENSES/CC0-1.0.txt
--rw-r--r--   0 root         (0) root         (0)    42098 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/LICENSES/LGPL-3.0-or-later.txt
--rw-r--r--   0 root         (0) root         (0)     1078 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/LICENSES/MIT.txt
--rw-r--r--   0 root         (0) root         (0)    16727 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/LICENSES/MPL-2.0.txt
--rw-r--r--   0 root         (0) root         (0)     3732 2023-06-05 19:00:31.169671 pyikarus-0.3.3.dev20230605190030/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3321 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.133669 pyikarus-0.3.3.dev20230605190030/cmake/
--rw-r--r--   0 root         (0) root         (0)      184 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/cmake/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      973 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/cmake/CPM.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.133669 pyikarus-0.3.3.dev20230605190030/cmake/FormatTarget/
--rw-r--r--   0 root         (0) root         (0)     1807 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/cmake/FormatTarget/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.133669 pyikarus-0.3.3.dev20230605190030/cmake/modules/
--rw-r--r--   0 root         (0) root         (0)      715 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/cmake/modules/AddAutoDiffFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      683 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/cmake/modules/AddEigenFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/cmake/modules/AddMatplotppFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      691 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/cmake/modules/AddSpdlogFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      706 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/cmake/modules/AddSpectraFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/cmake/modules/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      436 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/cmake/modules/IkarusMacros.cmake
--rw-r--r--   0 root         (0) root         (0)     2040 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/cmake/tools.cmake
--rw-r--r--   0 root         (0) root         (0)      148 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/codecov.yml
--rw-r--r--   0 root         (0) root         (0)      121 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/codespellignore
--rw-r--r--   0 root         (0) root         (0)     1588 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/config.h.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.133669 pyikarus-0.3.3.dev20230605190030/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.133669 pyikarus-0.3.3.dev20230605190030/docs/BuildLocally/
--rw-r--r--   0 root         (0) root         (0)      439 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/BuildLocally/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      333 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.133669 pyikarus-0.3.3.dev20230605190030/docs/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     1136 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/__pycache__/mkdocs-macros.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
--rw-r--r--   0 root         (0) root         (0)     6961 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/literature.bib
--rw-r--r--   0 root         (0) root         (0)      117 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/literature.bib.license
--rw-r--r--   0 root         (0) root         (0)     1271 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/mkdocs-macros.py
--rw-r--r--   0 root         (0) root         (0)      398 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/mkdocs.insiders.yml
--rw-r--r--   0 root         (0) root         (0)     5042 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/mkdocs.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.121669 pyikarus-0.3.3.dev20230605190030/docs/overrides/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.133669 pyikarus-0.3.3.dev20230605190030/docs/overrides/partials/
--rw-r--r--   0 root         (0) root         (0)     1732 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/overrides/partials/comments.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.137669 pyikarus-0.3.3.dev20230605190030/docs/website/
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/.meta.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.137669 pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/
--rw-r--r--   0 root         (0) root         (0)     4710 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/assembler.md
--rw-r--r--   0 root         (0) root         (0)     6387 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/controlRoutines.md
--rw-r--r--   0 root         (0) root         (0)     2024 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/dirichletBCs.md
--rw-r--r--   0 root         (0) root         (0)     3237 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/feRequirements.md
--rw-r--r--   0 root         (0) root         (0)    12894 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/finiteElements.md
--rw-r--r--   0 root         (0) root         (0)     2745 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/grids.md
--rw-r--r--   0 root         (0) root         (0)     4121 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/index.md
--rw-r--r--   0 root         (0) root         (0)     4932 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/localBasis.md
--rw-r--r--   0 root         (0) root         (0)    44213 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/localFunctions.md
--rw-r--r--   0 root         (0) root         (0)     3978 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/manifolds.md
--rw-r--r--   0 root         (0) root         (0)     2551 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/nonlinearOperator.md
--rw-r--r--   0 root         (0) root         (0)     3086 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/observer.md
--rw-r--r--   0 root         (0) root         (0)     5211 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/solvers.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.137669 pyikarus-0.3.3.dev20230605190030/docs/website/02_examples/
--rw-r--r--   0 root         (0) root         (0)     6655 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/02_examples/cantileverBeam.md
--rw-r--r--   0 root         (0) root         (0)     7251 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/02_examples/computePi.md
--rw-r--r--   0 root         (0) root         (0)     5439 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/02_examples/cooksMembrane.md
--rw-r--r--   0 root         (0) root         (0)     7323 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/02_examples/incompressibleRubberBlock.md
--rw-r--r--   0 root         (0) root         (0)     2164 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/02_examples/index.md
--rw-r--r--   0 root         (0) root         (0)     7774 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/02_examples/kirchhoffPlate.md
--rw-r--r--   0 root         (0) root         (0)     5088 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/02_examples/newtonRaphsonMethod.md
--rw-r--r--   0 root         (0) root         (0)     6164 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/02_examples/nonLinearElasticity.md
--rw-r--r--   0 root         (0) root         (0)     4179 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/02_examples/vonMisesTruss.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.141670 pyikarus-0.3.3.dev20230605190030/docs/website/03_contribution/
--rw-r--r--   0 root         (0) root         (0)     2439 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/03_contribution/buildDocumentationLocally.md
--rw-r--r--   0 root         (0) root         (0)     1002 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/03_contribution/codeStyle.md
--rw-r--r--   0 root         (0) root         (0)     2415 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/03_contribution/howToEdit.md
--rw-r--r--   0 root         (0) root         (0)     1736 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/03_contribution/openTask.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.141670 pyikarus-0.3.3.dev20230605190030/docs/website/04_blog/
--rw-r--r--   0 root         (0) root         (0)      274 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/04_blog/.authors.yml
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/04_blog/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.141670 pyikarus-0.3.3.dev20230605190030/docs/website/04_blog/posts/
--rw-r--r--   0 root         (0) root         (0)     7731 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/04_blog/posts/v0.3.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.141670 pyikarus-0.3.3.dev20230605190030/docs/website/05_cppReferences/
--rw-r--r--   0 root         (0) root         (0)     2324 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/05_cppReferences/cppRef.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.141670 pyikarus-0.3.3.dev20230605190030/docs/website/99_Literature/
--rw-r--r--   0 root         (0) root         (0)      169 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/99_Literature/99_Literature.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.141670 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.141670 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/Installation/
--rw-r--r--   0 root         (0) root         (0)    52795 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
--rw-r--r--   0 root         (0) root         (0)    46250 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/Installation/CMakeOutput.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
--rw-r--r--   0 root         (0) root         (0)     2852 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/Installation/ClionFooter.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
--rw-r--r--   0 root         (0) root         (0)    17924 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
--rw-r--r--   0 root         (0) root         (0)     9455 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.145670 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/builddocumentationlocally/
--rw-r--r--   0 root         (0) root         (0)    35234 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
--rw-r--r--   0 root         (0) root         (0)    62184 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
--rw-r--r--   0 root         (0) root         (0)     2281 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
--rw-r--r--   0 root         (0) root         (0)    40033 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
--rw-r--r--   0 root         (0) root         (0)    25505 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
--rw-r--r--   0 root         (0) root         (0)     8101 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/logo_blue.svg
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/logo_blue.svg.license
--rw-r--r--   0 root         (0) root         (0)     8255 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/logo_white.svg
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/logo_white.svg.license
--rw-r--r--   0 root         (0) root         (0)     4364 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/download.md
--rw-r--r--   0 root         (0) root         (0)      244 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/gallery.md
--rw-r--r--   0 root         (0) root         (0)     1358 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.145670 pyikarus-0.3.3.dev20230605190030/docs/website/javascripts/
--rw-r--r--   0 root         (0) root         (0)      486 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/javascripts/mathjax.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.145670 pyikarus-0.3.3.dev20230605190030/docs/website/stylesheets/
--rw-r--r--   0 root         (0) root         (0)      302 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/docs/website/stylesheets/extra.css
--rw-r--r--   0 root         (0) root         (0)      504 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/dune.module
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.145670 pyikarus-0.3.3.dev20230605190030/ikarus/
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.145670 pyikarus-0.3.3.dev20230605190030/ikarus/assembler/
--rw-r--r--   0 root         (0) root         (0)      268 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/assembler/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    12924 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/assembler/simpleAssemblers.hh
--rw-r--r--   0 root         (0) root         (0)    10714 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/assembler/simpleAssemblers.inl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.145670 pyikarus-0.3.3.dev20230605190030/ikarus/controlRoutines/
--rw-r--r--   0 root         (0) root         (0)      239 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/controlRoutines/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2575 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/controlRoutines/loadControl.hh
--rw-r--r--   0 root         (0) root         (0)     2970 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/controlRoutines/pathFollowingTechnique.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.145670 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/
--rw-r--r--   0 root         (0) root         (0)      349 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/fEparameter.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.145670 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/feBases/
--rw-r--r--   0 root         (0) root         (0)      282 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/feBases/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5311 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/feBases/autodiffFE.hh
--rw-r--r--   0 root         (0) root         (0)     2307 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/feBases/powerBasisFE.hh
--rw-r--r--   0 root         (0) root         (0)     1827 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/feBases/scalarFE.hh
--rw-r--r--   0 root         (0) root         (0)     9346 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/feRequirements.hh
--rw-r--r--   0 root         (0) root         (0)     1338 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/feTraits.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.149670 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    21360 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
--rw-r--r--   0 root         (0) root         (0)    13674 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/linearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.149670 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/materials/
--rw-r--r--   0 root         (0) root         (0)      397 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5699 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/materials/interface.hh
--rw-r--r--   0 root         (0) root         (0)     2718 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
--rw-r--r--   0 root         (0) root         (0)     4635 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/materials/neohooke.hh
--rw-r--r--   0 root         (0) root         (0)     3809 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/materials/strainConversions.hh
--rw-r--r--   0 root         (0) root         (0)     5734 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/materials/svk.hh
--rw-r--r--   0 root         (0) root         (0)      473 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/materials/tags.hh
--rw-r--r--   0 root         (0) root         (0)     7995 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
--rw-r--r--   0 root         (0) root         (0)     1196 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/materials.hh
--rw-r--r--   0 root         (0) root         (0)    15536 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/nonLinearElastic.hh
--rw-r--r--   0 root         (0) root         (0)    12678 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/physicsHelper.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.149670 pyikarus-0.3.3.dev20230605190030/ikarus/io/
--rw-r--r--   0 root         (0) root         (0)      258 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/io/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2350 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/io/resultEvaluators.hh
--rw-r--r--   0 root         (0) root         (0)     3829 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/io/resultFunction.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.149670 pyikarus-0.3.3.dev20230605190030/ikarus/linearAlgebra/
--rw-r--r--   0 root         (0) root         (0)      301 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/linearAlgebra/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6735 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/linearAlgebra/dirichletValues.hh
--rw-r--r--   0 root         (0) root         (0)     7698 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/linearAlgebra/nonLinearOperator.hh
--rw-r--r--   0 root         (0) root         (0)    12303 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/linearAlgebra/truncatedConjugateGradient.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.149670 pyikarus-0.3.3.dev20230605190030/ikarus/python/
--rw-r--r--   0 root         (0) root         (0)      294 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.149670 pyikarus-0.3.3.dev20230605190030/ikarus/python/assembler/
--rw-r--r--   0 root         (0) root         (0)      249 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/python/assembler/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6752 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/python/assembler/flatAssembler.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.149670 pyikarus-0.3.3.dev20230605190030/ikarus/python/basis/
--rw-r--r--   0 root         (0) root         (0)      237 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/python/basis/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1469 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/python/basis/basis.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.149670 pyikarus-0.3.3.dev20230605190030/ikarus/python/dirichletValues/
--rw-r--r--   0 root         (0) root         (0)      257 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/python/dirichletValues/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     4169 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/python/dirichletValues/dirichletValues.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.153670 pyikarus-0.3.3.dev20230605190030/ikarus/python/finiteElements/
--rw-r--r--   0 root         (0) root         (0)      303 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/python/finiteElements/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5220 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/python/finiteElements/linearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.153670 pyikarus-0.3.3.dev20230605190030/ikarus/python/finiteElements/materials/
--rw-r--r--   0 root         (0) root         (0)      268 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/python/finiteElements/materials/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     9949 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/python/finiteElements/materials/material.hh
--rw-r--r--   0 root         (0) root         (0)     5207 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/python/finiteElements/nonLinearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.153670 pyikarus-0.3.3.dev20230605190030/ikarus/python/test/
--rw-r--r--   0 root         (0) root         (0)      511 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/python/test/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3830 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/python/test/linearElasticTest.py
--rw-r--r--   0 root         (0) root         (0)     4340 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/python/test/nonLinearElasticTest.py
--rw-r--r--   0 root         (0) root         (0)      862 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/python/test/setpath.py.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.153670 pyikarus-0.3.3.dev20230605190030/ikarus/python/utils/
--rw-r--r--   0 root         (0) root         (0)      245 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/python/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1185 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/python/utils/boundarypatch.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.153670 pyikarus-0.3.3.dev20230605190030/ikarus/solver/
--rw-r--r--   0 root         (0) root         (0)      211 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/solver/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.153670 pyikarus-0.3.3.dev20230605190030/ikarus/solver/linearSolver/
--rw-r--r--   0 root         (0) root         (0)      244 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/solver/linearSolver/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     8891 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/solver/linearSolver/linearSolver.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.153670 pyikarus-0.3.3.dev20230605190030/ikarus/solver/nonLinearSolver/
--rw-r--r--   0 root         (0) root         (0)      272 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/solver/nonLinearSolver/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5406 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/solver/nonLinearSolver/newtonRaphson.hh
--rw-r--r--   0 root         (0) root         (0)     8297 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
--rw-r--r--   0 root         (0) root         (0)    18574 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/solver/nonLinearSolver/trustRegion.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.157670 pyikarus-0.3.3.dev20230605190030/ikarus/utils/
--rw-r--r--   0 root         (0) root         (0)      712 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1741 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/algorithms.hh
--rw-r--r--   0 root         (0) root         (0)      878 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/autodiffHelper.hh
--rw-r--r--   0 root         (0) root         (0)     1469 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/basis.hh
--rw-r--r--   0 root         (0) root         (0)     6930 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/concepts.hh
--rw-r--r--   0 root         (0) root         (0)      499 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/defaultFunctions.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.157670 pyikarus-0.3.3.dev20230605190030/ikarus/utils/drawing/
--rw-r--r--   0 root         (0) root         (0)      262 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/drawing/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/drawing/griddrawer.hh
--rw-r--r--   0 root         (0) root         (0)      544 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/drawing/matplotHelper.cpp
--rw-r--r--   0 root         (0) root         (0)      703 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/drawing/matplotHelper.hh
--rw-r--r--   0 root         (0) root         (0)     2484 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/duneUtilities.hh
--rw-r--r--   0 root         (0) root         (0)     2347 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/eigenDuneTransformations.hh
--rw-r--r--   0 root         (0) root         (0)      682 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/eigenSparseAddon.hh
--rw-r--r--   0 root         (0) root         (0)     1367 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/findLineSegment.cpp
--rw-r--r--   0 root         (0) root         (0)      724 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/findLineSegment.hh
--rw-r--r--   0 root         (0) root         (0)     3611 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/flatPreBasis.hh
--rw-r--r--   0 root         (0) root         (0)     2171 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/functionSanityChecks.cpp
--rw-r--r--   0 root         (0) root         (0)     6359 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/functionSanityChecks.hh
--rw-r--r--   0 root         (0) root         (0)     3152 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/init.hh
--rw-r--r--   0 root         (0) root         (0)    15244 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/linearAlgebraHelper.hh
--rw-r--r--   0 root         (0) root         (0)     1711 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/makeEnum.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.157670 pyikarus-0.3.3.dev20230605190030/ikarus/utils/observer/
--rw-r--r--   0 root         (0) root         (0)      450 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/observer/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1554 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/observer/controlLogger.hh
--rw-r--r--   0 root         (0) root         (0)     2307 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/observer/controlVTKWriter.hh
--rw-r--r--   0 root         (0) root         (0)      905 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/observer/genericControlObserver.hh
--rw-r--r--   0 root         (0) root         (0)     1053 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/observer/gridDrawerObserver.hh
--rw-r--r--   0 root         (0) root         (0)     1132 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/observer/loadControlObserver.hh
--rw-r--r--   0 root         (0) root         (0)     1985 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/observer/nonLinearSolverLogger.hh
--rw-r--r--   0 root         (0) root         (0)     5497 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/observer/observer.hh
--rw-r--r--   0 root         (0) root         (0)      489 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/observer/observerMessages.hh
--rw-r--r--   0 root         (0) root         (0)     4159 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/pathFollowingFunctions.hh
--rw-r--r--   0 root         (0) root         (0)     1131 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/polyfit.cpp
--rw-r--r--   0 root         (0) root         (0)      570 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/polyfit.hh
--rw-r--r--   0 root         (0) root         (0)    10054 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/tensorUtils.hh
--rw-r--r--   0 root         (0) root         (0)    15149 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus/utils/traits.hh
--rw-r--r--   0 root         (0) root         (0)      432 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/ikarus.pc.in
--rw-r--r--   0 root         (0) root         (0)      196 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/iwyu.imp
--rw-r--r--   0 root         (0) root         (0)      422 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.161670 pyikarus-0.3.3.dev20230605190030/python/
--rw-r--r--   0 root         (0) root         (0)      423 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.161670 pyikarus-0.3.3.dev20230605190030/python/ikarus/
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/python/ikarus/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/python/ikarus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5650 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/python/ikarus/_ikarus.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.161670 pyikarus-0.3.3.dev20230605190030/python/ikarus/assembler/
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/python/ikarus/assembler/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1628 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/python/ikarus/assembler/__init__.py
--rw-r--r--   0 root         (0) root         (0)      790 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/python/ikarus/basis.py
--rw-r--r--   0 root         (0) root         (0)      753 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/python/ikarus/dirichletValues.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.161670 pyikarus-0.3.3.dev20230605190030/python/ikarus/finite_elements/
--rw-r--r--   0 root         (0) root         (0)      173 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/python/ikarus/finite_elements/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3119 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/python/ikarus/finite_elements/__init__.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/python/ikarus/generator.py
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/python/ikarus/materials.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.161670 pyikarus-0.3.3.dev20230605190030/python/ikarus/utils/
--rw-r--r--   0 root         (0) root         (0)      163 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/python/ikarus/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      768 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/python/ikarus/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.161670 pyikarus-0.3.3.dev20230605190030/python/pyikarus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3732 2023-06-05 19:00:31.000000 pyikarus-0.3.3.dev20230605190030/python/pyikarus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10066 2023-06-05 19:00:31.000000 pyikarus-0.3.3.dev20230605190030/python/pyikarus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 19:00:31.000000 pyikarus-0.3.3.dev20230605190030/python/pyikarus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-05 19:00:31.000000 pyikarus-0.3.3.dev20230605190030/python/pyikarus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-05 19:00:31.000000 pyikarus-0.3.3.dev20230605190030/python/pyikarus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/python/setup.py.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.161670 pyikarus-0.3.3.dev20230605190030/sandbox/
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/sandbox/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.161670 pyikarus-0.3.3.dev20230605190030/sandbox/src/
--rw-r--r--   0 root         (0) root         (0)     1220 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/sandbox/src/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.161670 pyikarus-0.3.3.dev20230605190030/sandbox/src/auxiliaryFiles/
--rw-r--r--   0 root         (0) root         (0)   674469 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/sandbox/src/auxiliaryFiles/circle.msh
--rw-r--r--   0 root         (0) root         (0)      320 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/sandbox/src/sandbox.cpp
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 19:00:31.169671 pyikarus-0.3.3.dev20230605190030/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1080 2023-06-05 19:00:30.000000 pyikarus-0.3.3.dev20230605190030/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.165670 pyikarus-0.3.3.dev20230605190030/tests/
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.165670 pyikarus-0.3.3.dev20230605190030/tests/src/
--rw-r--r--   0 root         (0) root         (0)     1408 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3907 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testAssembler.cpp
--rw-r--r--   0 root         (0) root         (0)     1292 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testAutodiffHelper.cpp
--rw-r--r--   0 root         (0) root         (0)    14291 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testCommon.hh
--rw-r--r--   0 root         (0) root         (0)     2639 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testDependencies.cpp
--rw-r--r--   0 root         (0) root         (0)     6520 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testDirichletValue.cpp
--rw-r--r--   0 root         (0) root         (0)     4795 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testEAS.hh
--rw-r--r--   0 root         (0) root         (0)     1600 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testEnhancedAssumedStrains.cpp
--rw-r--r--   0 root         (0) root         (0)     5805 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testFEElement.hh
--rw-r--r--   0 root         (0) root         (0)      571 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testFactories.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:31.169671 pyikarus-0.3.3.dev20230605190030/tests/src/testFiles/
--rw-r--r--   0 root         (0) root         (0)     9028 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testFiles/unstructuredQuadscoarse.msh
--rw-r--r--   0 root         (0) root         (0)      395 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testFiles/unstructuredTest.geo
--rw-r--r--   0 root         (0) root         (0)      497 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testFiles/unstructuredTest.msh
--rw-r--r--   0 root         (0) root         (0)      546 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testFiles/unstructuredTest2.geo
--rw-r--r--   0 root         (0) root         (0)    11431 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testFiles/unstructuredTrianglesfine.msh
--rw-r--r--   0 root         (0) root         (0)     1870 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testFunctionTraits.cpp
--rw-r--r--   0 root         (0) root         (0)     1114 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testHelpers.hh
--rw-r--r--   0 root         (0) root         (0)     3190 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testLinearElasticity.cpp
--rw-r--r--   0 root         (0) root         (0)     2278 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testManifolds.cpp
--rw-r--r--   0 root         (0) root         (0)     7949 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testMaterial.cpp
--rw-r--r--   0 root         (0) root         (0)    15845 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testNonLinearElasticity.hh
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testNonLinearElasticityNeoHooke.cpp
--rw-r--r--   0 root         (0) root         (0)     1121 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testNonLinearElasticitySVK.cpp
--rw-r--r--   0 root         (0) root         (0)     9846 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testNonLinearOperator.cpp
--rw-r--r--   0 root         (0) root         (0)     6251 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testPathFollowing.cpp
--rw-r--r--   0 root         (0) root         (0)     1651 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testPolyFit.cpp
--rw-r--r--   0 root         (0) root         (0)      696 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testPythonConversion.cpp
--rw-r--r--   0 root         (0) root         (0)    17531 2023-06-05 19:00:22.000000 pyikarus-0.3.3.dev20230605190030/tests/src/testTrustRegion.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.466858 pyikarus-0.3.3.dev20230615091249/
+-rw-r--r--   0 root         (0) root         (0)      312 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/.bettercodehub.yml
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/.clang-format
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/.cmake-format
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.386858 pyikarus-0.3.3.dev20230615091249/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.402858 pyikarus-0.3.3.dev20230615091249/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 root         (0) root         (0)      615 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.406858 pyikarus-0.3.3.dev20230615091249/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/.github/workflows/codespell.yml
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/.github/workflows/createDockerContainer.yml
+-rw-r--r--   0 root         (0) root         (0)     5615 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/.github/workflows/createRelease.yml
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/.github/workflows/debian-coverage.yml
+-rw-r--r--   0 root         (0) root         (0)     2612 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/.github/workflows/debian.yml
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/.github/workflows/ghpages.yml
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/.github/workflows/releasePythonPackage.yml
+-rw-r--r--   0 root         (0) root         (0)      314 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/.github/workflows/reuseLint.yml
+-rw-r--r--   0 root         (0) root         (0)     3335 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/.github/workflows/runExamples.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.406858 pyikarus-0.3.3.dev20230615091249/.github/workflows/scripts/
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/.github/workflows/scripts/release.py
+-rw-r--r--   0 root         (0) root         (0)     1331 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/.github/workflows/style.yml
+-rw-r--r--   0 root         (0) root         (0)      482 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.406858 pyikarus-0.3.3.dev20230615091249/.reuse/
+-rw-r--r--   0 root         (0) root         (0)      661 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/.reuse/dep5
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5335 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)      784 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/LICENSE.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.406858 pyikarus-0.3.3.dev20230615091249/LICENSES/
+-rw-r--r--   0 root         (0) root         (0)    18375 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 root         (0) root         (0)    42098 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/LICENSES/MIT.txt
+-rw-r--r--   0 root         (0) root         (0)    16727 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/LICENSES/MPL-2.0.txt
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-06-15 09:12:50.466858 pyikarus-0.3.3.dev20230615091249/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3418 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.406858 pyikarus-0.3.3.dev20230615091249/cmake/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/cmake/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      973 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/cmake/CPM.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.406858 pyikarus-0.3.3.dev20230615091249/cmake/FormatTarget/
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/cmake/FormatTarget/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.410858 pyikarus-0.3.3.dev20230615091249/cmake/modules/
+-rw-r--r--   0 root         (0) root         (0)      715 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/cmake/modules/AddAutoDiffFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      683 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/cmake/modules/AddEigenFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/cmake/modules/AddMatplotppFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      691 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/cmake/modules/AddSpdlogFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      706 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/cmake/modules/AddSpectraFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/cmake/modules/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      436 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/cmake/modules/IkarusMacros.cmake
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/cmake/tools.cmake
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/codecov.yml
+-rw-r--r--   0 root         (0) root         (0)      121 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/codespellignore
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/config.h.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.410858 pyikarus-0.3.3.dev20230615091249/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.410858 pyikarus-0.3.3.dev20230615091249/docs/BuildLocally/
+-rw-r--r--   0 root         (0) root         (0)      439 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/BuildLocally/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      333 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.410858 pyikarus-0.3.3.dev20230615091249/docs/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/__pycache__/mkdocs-macros.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
+-rw-r--r--   0 root         (0) root         (0)     6961 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/literature.bib
+-rw-r--r--   0 root         (0) root         (0)      117 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/literature.bib.license
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/mkdocs-macros.py
+-rw-r--r--   0 root         (0) root         (0)      398 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/mkdocs.insiders.yml
+-rw-r--r--   0 root         (0) root         (0)     5042 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/mkdocs.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.390858 pyikarus-0.3.3.dev20230615091249/docs/overrides/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.410858 pyikarus-0.3.3.dev20230615091249/docs/overrides/partials/
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/overrides/partials/comments.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.414857 pyikarus-0.3.3.dev20230615091249/docs/website/
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/.meta.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.414857 pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/
+-rw-r--r--   0 root         (0) root         (0)     4710 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/assembler.md
+-rw-r--r--   0 root         (0) root         (0)     6387 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/controlRoutines.md
+-rw-r--r--   0 root         (0) root         (0)     2024 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/dirichletBCs.md
+-rw-r--r--   0 root         (0) root         (0)     3237 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/feRequirements.md
+-rw-r--r--   0 root         (0) root         (0)    12894 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/finiteElements.md
+-rw-r--r--   0 root         (0) root         (0)     2745 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/grids.md
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/index.md
+-rw-r--r--   0 root         (0) root         (0)     4932 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/localBasis.md
+-rw-r--r--   0 root         (0) root         (0)    44213 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/localFunctions.md
+-rw-r--r--   0 root         (0) root         (0)     3978 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/manifolds.md
+-rw-r--r--   0 root         (0) root         (0)     2551 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/nonlinearOperator.md
+-rw-r--r--   0 root         (0) root         (0)     3086 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/observer.md
+-rw-r--r--   0 root         (0) root         (0)     5211 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/solvers.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.418858 pyikarus-0.3.3.dev20230615091249/docs/website/02_examples/
+-rw-r--r--   0 root         (0) root         (0)     6655 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/02_examples/cantileverBeam.md
+-rw-r--r--   0 root         (0) root         (0)     7251 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/02_examples/computePi.md
+-rw-r--r--   0 root         (0) root         (0)     5439 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/02_examples/cooksMembrane.md
+-rw-r--r--   0 root         (0) root         (0)     7323 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/02_examples/incompressibleRubberBlock.md
+-rw-r--r--   0 root         (0) root         (0)     2164 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/02_examples/index.md
+-rw-r--r--   0 root         (0) root         (0)     7722 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/02_examples/kirchhoffPlate.md
+-rw-r--r--   0 root         (0) root         (0)     5088 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/02_examples/newtonRaphsonMethod.md
+-rw-r--r--   0 root         (0) root         (0)     6164 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/02_examples/nonLinearElasticity.md
+-rw-r--r--   0 root         (0) root         (0)     4179 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/02_examples/vonMisesTruss.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.418858 pyikarus-0.3.3.dev20230615091249/docs/website/03_contribution/
+-rw-r--r--   0 root         (0) root         (0)     2439 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/03_contribution/buildDocumentationLocally.md
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/03_contribution/codeStyle.md
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/03_contribution/howToEdit.md
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/03_contribution/openTask.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.418858 pyikarus-0.3.3.dev20230615091249/docs/website/04_blog/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/04_blog/.authors.yml
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/04_blog/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.418858 pyikarus-0.3.3.dev20230615091249/docs/website/04_blog/posts/
+-rw-r--r--   0 root         (0) root         (0)     7731 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/04_blog/posts/v0.3.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.418858 pyikarus-0.3.3.dev20230615091249/docs/website/05_cppReferences/
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/05_cppReferences/cppRef.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.422858 pyikarus-0.3.3.dev20230615091249/docs/website/99_Literature/
+-rw-r--r--   0 root         (0) root         (0)      169 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/99_Literature/99_Literature.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.422858 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/
+-rw-r--r--   0 root         (0) root         (0)   280461 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/BigLogo.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.426858 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/Installation/
+-rw-r--r--   0 root         (0) root         (0)    52795 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
+-rw-r--r--   0 root         (0) root         (0)    46250 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/Installation/CMakeOutput.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/Installation/ClionFooter.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
+-rw-r--r--   0 root         (0) root         (0)    17924 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
+-rw-r--r--   0 root         (0) root         (0)     9455 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.426858 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/builddocumentationlocally/
+-rw-r--r--   0 root         (0) root         (0)    35234 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
+-rw-r--r--   0 root         (0) root         (0)    62184 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
+-rw-r--r--   0 root         (0) root         (0)    40033 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
+-rw-r--r--   0 root         (0) root         (0)    25505 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
+-rw-r--r--   0 root         (0) root         (0)   441218 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/logo_blue.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/logo_blue.png.license
+-rw-r--r--   0 root         (0) root         (0)   482004 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/logo_white.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/logo_white.png.license
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/download.md
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/gallery.md
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.426858 pyikarus-0.3.3.dev20230615091249/docs/website/javascripts/
+-rw-r--r--   0 root         (0) root         (0)      486 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/javascripts/mathjax.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.430858 pyikarus-0.3.3.dev20230615091249/docs/website/stylesheets/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/docs/website/stylesheets/extra.css
+-rw-r--r--   0 root         (0) root         (0)      504 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/dune.module
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.430858 pyikarus-0.3.3.dev20230615091249/ikarus/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.430858 pyikarus-0.3.3.dev20230615091249/ikarus/assembler/
+-rw-r--r--   0 root         (0) root         (0)      268 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    12924 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/assembler/simpleAssemblers.hh
+-rw-r--r--   0 root         (0) root         (0)    10714 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/assembler/simpleAssemblers.inl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.430858 pyikarus-0.3.3.dev20230615091249/ikarus/controlRoutines/
+-rw-r--r--   0 root         (0) root         (0)      239 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/controlRoutines/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2575 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/controlRoutines/loadControl.hh
+-rw-r--r--   0 root         (0) root         (0)     2970 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/controlRoutines/pathFollowingTechnique.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.430858 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/fEparameter.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.434858 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/feBases/
+-rw-r--r--   0 root         (0) root         (0)      282 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/feBases/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5311 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/feBases/autodiffFE.hh
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/feBases/powerBasisFE.hh
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/feBases/scalarFE.hh
+-rw-r--r--   0 root         (0) root         (0)     9346 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/feRequirements.hh
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/feTraits.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.434858 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    21360 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
+-rw-r--r--   0 root         (0) root         (0)    14203 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/linearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.434858 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/materials/
+-rw-r--r--   0 root         (0) root         (0)      397 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5699 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/materials/interface.hh
+-rw-r--r--   0 root         (0) root         (0)     2718 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
+-rw-r--r--   0 root         (0) root         (0)     4635 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/materials/neohooke.hh
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/materials/strainConversions.hh
+-rw-r--r--   0 root         (0) root         (0)     5734 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/materials/svk.hh
+-rw-r--r--   0 root         (0) root         (0)      473 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/materials/tags.hh
+-rw-r--r--   0 root         (0) root         (0)     7995 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/materials.hh
+-rw-r--r--   0 root         (0) root         (0)    15991 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/nonLinearElastic.hh
+-rw-r--r--   0 root         (0) root         (0)    12678 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/physicsHelper.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.434858 pyikarus-0.3.3.dev20230615091249/ikarus/io/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/io/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/io/resultEvaluators.hh
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/io/resultFunction.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.438858 pyikarus-0.3.3.dev20230615091249/ikarus/linearAlgebra/
+-rw-r--r--   0 root         (0) root         (0)      301 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/linearAlgebra/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6735 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/linearAlgebra/dirichletValues.hh
+-rw-r--r--   0 root         (0) root         (0)     7698 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/linearAlgebra/nonLinearOperator.hh
+-rw-r--r--   0 root         (0) root         (0)    12303 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/linearAlgebra/truncatedConjugateGradient.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.438858 pyikarus-0.3.3.dev20230615091249/ikarus/python/
+-rw-r--r--   0 root         (0) root         (0)      294 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.438858 pyikarus-0.3.3.dev20230615091249/ikarus/python/assembler/
+-rw-r--r--   0 root         (0) root         (0)      249 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/python/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6752 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/python/assembler/flatAssembler.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.438858 pyikarus-0.3.3.dev20230615091249/ikarus/python/basis/
+-rw-r--r--   0 root         (0) root         (0)      237 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/python/basis/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/python/basis/basis.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.438858 pyikarus-0.3.3.dev20230615091249/ikarus/python/dirichletValues/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/python/dirichletValues/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     4169 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/python/dirichletValues/dirichletValues.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.438858 pyikarus-0.3.3.dev20230615091249/ikarus/python/finiteElements/
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/python/finiteElements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5220 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/python/finiteElements/linearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.438858 pyikarus-0.3.3.dev20230615091249/ikarus/python/finiteElements/materials/
+-rw-r--r--   0 root         (0) root         (0)      268 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/python/finiteElements/materials/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     9949 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/python/finiteElements/materials/material.hh
+-rw-r--r--   0 root         (0) root         (0)     5207 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/python/finiteElements/nonLinearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.442858 pyikarus-0.3.3.dev20230615091249/ikarus/python/test/
+-rw-r--r--   0 root         (0) root         (0)      511 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/python/test/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3830 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/python/test/linearElasticTest.py
+-rw-r--r--   0 root         (0) root         (0)     4340 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/python/test/nonLinearElasticTest.py
+-rw-r--r--   0 root         (0) root         (0)      862 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/python/test/setpath.py.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.442858 pyikarus-0.3.3.dev20230615091249/ikarus/python/utils/
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/python/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/python/utils/boundarypatch.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.442858 pyikarus-0.3.3.dev20230615091249/ikarus/solver/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/solver/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.442858 pyikarus-0.3.3.dev20230615091249/ikarus/solver/linearSolver/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/solver/linearSolver/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     8891 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/solver/linearSolver/linearSolver.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.442858 pyikarus-0.3.3.dev20230615091249/ikarus/solver/nonLinearSolver/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/solver/nonLinearSolver/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5406 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/solver/nonLinearSolver/newtonRaphson.hh
+-rw-r--r--   0 root         (0) root         (0)     8297 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
+-rw-r--r--   0 root         (0) root         (0)    18574 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/solver/nonLinearSolver/trustRegion.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.450858 pyikarus-0.3.3.dev20230615091249/ikarus/utils/
+-rw-r--r--   0 root         (0) root         (0)      712 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/algorithms.hh
+-rw-r--r--   0 root         (0) root         (0)      878 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/autodiffHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/basis.hh
+-rw-r--r--   0 root         (0) root         (0)     6930 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/concepts.hh
+-rw-r--r--   0 root         (0) root         (0)      499 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/defaultFunctions.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.450858 pyikarus-0.3.3.dev20230615091249/ikarus/utils/drawing/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/drawing/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/drawing/griddrawer.hh
+-rw-r--r--   0 root         (0) root         (0)      544 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/drawing/matplotHelper.cpp
+-rw-r--r--   0 root         (0) root         (0)      703 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/drawing/matplotHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/duneUtilities.hh
+-rw-r--r--   0 root         (0) root         (0)     2347 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/eigenDuneTransformations.hh
+-rw-r--r--   0 root         (0) root         (0)      682 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/eigenSparseAddon.hh
+-rw-r--r--   0 root         (0) root         (0)     1367 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/findLineSegment.cpp
+-rw-r--r--   0 root         (0) root         (0)      724 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/findLineSegment.hh
+-rw-r--r--   0 root         (0) root         (0)     3611 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/flatPreBasis.hh
+-rw-r--r--   0 root         (0) root         (0)     2171 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/functionSanityChecks.cpp
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/functionSanityChecks.hh
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/init.hh
+-rw-r--r--   0 root         (0) root         (0)    15244 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/linearAlgebraHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/makeEnum.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.450858 pyikarus-0.3.3.dev20230615091249/ikarus/utils/observer/
+-rw-r--r--   0 root         (0) root         (0)      450 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/observer/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/observer/controlLogger.hh
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/observer/controlVTKWriter.hh
+-rw-r--r--   0 root         (0) root         (0)      905 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/observer/genericControlObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/observer/gridDrawerObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/observer/loadControlObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/observer/nonLinearSolverLogger.hh
+-rw-r--r--   0 root         (0) root         (0)     5497 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/observer/observer.hh
+-rw-r--r--   0 root         (0) root         (0)      489 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/observer/observerMessages.hh
+-rw-r--r--   0 root         (0) root         (0)     4159 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/pathFollowingFunctions.hh
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/polyfit.cpp
+-rw-r--r--   0 root         (0) root         (0)      570 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/polyfit.hh
+-rw-r--r--   0 root         (0) root         (0)    10054 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/tensorUtils.hh
+-rw-r--r--   0 root         (0) root         (0)    15149 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/ikarus/utils/traits.hh
+-rw-r--r--   0 root         (0) root         (0)      432 2023-06-15 09:12:39.000000 pyikarus-0.3.3.dev20230615091249/ikarus.pc.in
+-rw-r--r--   0 root         (0) root         (0)      196 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/iwyu.imp
+-rw-r--r--   0 root         (0) root         (0)      422 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.450858 pyikarus-0.3.3.dev20230615091249/python/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.454858 pyikarus-0.3.3.dev20230615091249/python/ikarus/
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/python/ikarus/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/python/ikarus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5650 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/python/ikarus/_ikarus.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.454858 pyikarus-0.3.3.dev20230615091249/python/ikarus/assembler/
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/python/ikarus/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/python/ikarus/assembler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      790 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/python/ikarus/basis.py
+-rw-r--r--   0 root         (0) root         (0)      753 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/python/ikarus/dirichletValues.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.454858 pyikarus-0.3.3.dev20230615091249/python/ikarus/finite_elements/
+-rw-r--r--   0 root         (0) root         (0)      173 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/python/ikarus/finite_elements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/python/ikarus/finite_elements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/python/ikarus/generator.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/python/ikarus/materials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.454858 pyikarus-0.3.3.dev20230615091249/python/ikarus/utils/
+-rw-r--r--   0 root         (0) root         (0)      163 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/python/ikarus/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      768 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/python/ikarus/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.454858 pyikarus-0.3.3.dev20230615091249/python/pyikarus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-06-15 09:12:50.000000 pyikarus-0.3.3.dev20230615091249/python/pyikarus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10107 2023-06-15 09:12:50.000000 pyikarus-0.3.3.dev20230615091249/python/pyikarus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 09:12:50.000000 pyikarus-0.3.3.dev20230615091249/python/pyikarus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-15 09:12:50.000000 pyikarus-0.3.3.dev20230615091249/python/pyikarus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-15 09:12:50.000000 pyikarus-0.3.3.dev20230615091249/python/pyikarus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/python/setup.py.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.458858 pyikarus-0.3.3.dev20230615091249/sandbox/
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/sandbox/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.458858 pyikarus-0.3.3.dev20230615091249/sandbox/src/
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/sandbox/src/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.458858 pyikarus-0.3.3.dev20230615091249/sandbox/src/auxiliaryFiles/
+-rw-r--r--   0 root         (0) root         (0)   674469 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/sandbox/src/auxiliaryFiles/circle.msh
+-rw-r--r--   0 root         (0) root         (0)      320 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/sandbox/src/sandbox.cpp
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 09:12:50.466858 pyikarus-0.3.3.dev20230615091249/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-06-15 09:12:49.000000 pyikarus-0.3.3.dev20230615091249/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.458858 pyikarus-0.3.3.dev20230615091249/tests/
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.466858 pyikarus-0.3.3.dev20230615091249/tests/src/
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3907 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testAssembler.cpp
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testAutodiffHelper.cpp
+-rw-r--r--   0 root         (0) root         (0)    14291 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testCommon.hh
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testDependencies.cpp
+-rw-r--r--   0 root         (0) root         (0)     6520 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testDirichletValue.cpp
+-rw-r--r--   0 root         (0) root         (0)     4795 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testEAS.hh
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testEnhancedAssumedStrains.cpp
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testFEElement.hh
+-rw-r--r--   0 root         (0) root         (0)      571 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testFactories.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 09:12:50.466858 pyikarus-0.3.3.dev20230615091249/tests/src/testFiles/
+-rw-r--r--   0 root         (0) root         (0)     9028 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testFiles/unstructuredQuadscoarse.msh
+-rw-r--r--   0 root         (0) root         (0)      395 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testFiles/unstructuredTest.geo
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testFiles/unstructuredTest.msh
+-rw-r--r--   0 root         (0) root         (0)      546 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testFiles/unstructuredTest2.geo
+-rw-r--r--   0 root         (0) root         (0)    11431 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testFiles/unstructuredTrianglesfine.msh
+-rw-r--r--   0 root         (0) root         (0)     1870 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testFunctionTraits.cpp
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testHelpers.hh
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testLinearElasticity.cpp
+-rw-r--r--   0 root         (0) root         (0)     2278 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testManifolds.cpp
+-rw-r--r--   0 root         (0) root         (0)     7949 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testMaterial.cpp
+-rw-r--r--   0 root         (0) root         (0)    15845 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testNonLinearElasticity.hh
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testNonLinearElasticityNeoHooke.cpp
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testNonLinearElasticitySVK.cpp
+-rw-r--r--   0 root         (0) root         (0)     9846 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testNonLinearOperator.cpp
+-rw-r--r--   0 root         (0) root         (0)     6251 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testPathFollowing.cpp
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testPolyFit.cpp
+-rw-r--r--   0 root         (0) root         (0)      696 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testPythonConversion.cpp
+-rw-r--r--   0 root         (0) root         (0)    17531 2023-06-15 09:12:40.000000 pyikarus-0.3.3.dev20230615091249/tests/src/testTrustRegion.cpp
```

### Comparing `pyikarus-0.3.3.dev20230605190030/.clang-format` & `pyikarus-0.3.3.dev20230615091249/.clang-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/.cmake-format` & `pyikarus-0.3.3.dev20230615091249/.cmake-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/.github/ISSUE_TEMPLATE/feature_request.md` & `pyikarus-0.3.3.dev20230615091249/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/.github/workflows/createDockerContainer.yml` & `pyikarus-0.3.3.dev20230615091249/.github/workflows/createDockerContainer.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/.github/workflows/createRelease.yml` & `pyikarus-0.3.3.dev20230615091249/.github/workflows/createRelease.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/.github/workflows/debian-coverage.yml` & `pyikarus-0.3.3.dev20230615091249/.github/workflows/debian-coverage.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/.github/workflows/debian.yml` & `pyikarus-0.3.3.dev20230615091249/.github/workflows/debian.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/.github/workflows/ghpages.yml` & `pyikarus-0.3.3.dev20230615091249/.github/workflows/ghpages.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/.github/workflows/releasePythonPackage.yml` & `pyikarus-0.3.3.dev20230615091249/.github/workflows/releasePythonPackage.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/.github/workflows/runExamples.yml` & `pyikarus-0.3.3.dev20230615091249/.github/workflows/runExamples.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/.github/workflows/scripts/release.py` & `pyikarus-0.3.3.dev20230615091249/.github/workflows/scripts/release.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/.github/workflows/style.yml` & `pyikarus-0.3.3.dev20230615091249/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/.reuse/dep5` & `pyikarus-0.3.3.dev20230615091249/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/CHANGELOG.md` & `pyikarus-0.3.3.dev20230615091249/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/CMakeLists.txt` & `pyikarus-0.3.3.dev20230615091249/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/CODE_OF_CONDUCT.md` & `pyikarus-0.3.3.dev20230615091249/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/LICENSE.md` & `pyikarus-0.3.3.dev20230615091249/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/LICENSES/CC-BY-SA-4.0.txt` & `pyikarus-0.3.3.dev20230615091249/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/LICENSES/CC0-1.0.txt` & `pyikarus-0.3.3.dev20230615091249/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/LICENSES/LGPL-3.0-or-later.txt` & `pyikarus-0.3.3.dev20230615091249/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/LICENSES/MIT.txt` & `pyikarus-0.3.3.dev20230615091249/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/LICENSES/MPL-2.0.txt` & `pyikarus-0.3.3.dev20230615091249/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/PKG-INFO` & `pyikarus-0.3.3.dev20230615091249/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.3.dev20230605190030
+Version: 0.3.3.dev20230615091249
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
@@ -13,14 +13,18 @@
 
 <!--
 SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 SPDX-License-Identifier: LGPL-3.0-or-later
 -->
 # Ikarus
 
+<img align="left" src="docs/website/auxiliaryImages/BigLogo.png" width="800">  
+
+<br/><br/>    
+
 [![Debian](https://github.com/ikarus-project/ikarus/actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/workflows/debian.yml)
 [![codecov](https://codecov.io/gh/ikarus-project/ikarus/branch/main/graph/badge.svg?token=zJgggitPMc)](https://codecov.io/gh/ikarus-project/ikarus)
 [![CodeStyle](https://github.com/ikarus-project/ikarus/actions/workflows/style.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/workflows/style.yml)
 [![Docs](https://github.com/ikarus-project/ikarus/actions/workflows/ghpages.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/workflows/ghpages.yml)
 [![CodeFactor](https://www.codefactor.io/repository/github/ikarus-project/ikarus/badge/main)](https://www.codefactor.io/repository/github/ikarus-project/ikarus/overview/main)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/5c588e67d1e541fc9be3c7377297aa8a)](https://www.codacy.com/gh/ikarus-project/ikarus/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ikarus-project/ikarus&amp;utm_campaign=Badge_Grade)
 [![Gitter](https://badges.gitter.im/ikarus-project/community.svg)](https://gitter.im/ikarus-project/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230605190030 Home-
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230615091249 Home-
 page: Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-
 stuttgart.de Classifier: Programming Language :: C++ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License (GPL) Requires-Python: >=3.4 Description-Content-Type: text/
-markdown License-File: LICENSE.md  # Ikarus [![Debian](https://github.com/
-ikarus-project/ikarus/actions/workflows/debian.yml/badge.svg)](https://
-github.com/ikarus-project/ikarus/actions/workflows/debian.yml) [![codecov]
-(https://codecov.io/gh/ikarus-project/ikarus/branch/main/graph/
-badge.svg?token=zJgggitPMc)](https://codecov.io/gh/ikarus-project/ikarus) [!
-[CodeStyle](https://github.com/ikarus-project/ikarus/actions/workflows/
-style.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/
-workflows/style.yml) [![Docs](https://github.com/ikarus-project/ikarus/actions/
-workflows/ghpages.yml/badge.svg)](https://github.com/ikarus-project/ikarus/
-actions/workflows/ghpages.yml) [![CodeFactor](https://www.codefactor.io/
+markdown License-File: LICENSE.md  # Ikarus [docs/website/auxiliaryImages/
+BigLogo.png]
+
+[![Debian](https://github.com/ikarus-project/ikarus/actions/workflows/
+debian.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/
+workflows/debian.yml) [![codecov](https://codecov.io/gh/ikarus-project/ikarus/
+branch/main/graph/badge.svg?token=zJgggitPMc)](https://codecov.io/gh/ikarus-
+project/ikarus) [![CodeStyle](https://github.com/ikarus-project/ikarus/actions/
+workflows/style.yml/badge.svg)](https://github.com/ikarus-project/ikarus/
+actions/workflows/style.yml) [![Docs](https://github.com/ikarus-project/ikarus/
+actions/workflows/ghpages.yml/badge.svg)](https://github.com/ikarus-project/
+ikarus/actions/workflows/ghpages.yml) [![CodeFactor](https://www.codefactor.io/
 repository/github/ikarus-project/ikarus/badge/main)](https://www.codefactor.io/
 repository/github/ikarus-project/ikarus/overview/main) [![Codacy Badge](https:/
 /app.codacy.com/project/badge/Grade/5c588e67d1e541fc9be3c7377297aa8a)](https://
 www.codacy.com/gh/ikarus-project/ikarus/
 dashboard?utm_source=github.com&utm_medium=referral&utm_content=ikarus-project/
 ikarus&utm_campaign=Badge_Grade) [![Gitter](https://badges.gitter.im/ikarus-
 project/community.svg)](https://gitter.im/ikarus-project/
```

### Comparing `pyikarus-0.3.3.dev20230605190030/README.md` & `pyikarus-0.3.3.dev20230615091249/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 <!--
 SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 SPDX-License-Identifier: LGPL-3.0-or-later
 -->
 # Ikarus
 
+<img align="left" src="docs/website/auxiliaryImages/BigLogo.png" width="800">  
+
+<br/><br/>    
+
 [![Debian](https://github.com/ikarus-project/ikarus/actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/workflows/debian.yml)
 [![codecov](https://codecov.io/gh/ikarus-project/ikarus/branch/main/graph/badge.svg?token=zJgggitPMc)](https://codecov.io/gh/ikarus-project/ikarus)
 [![CodeStyle](https://github.com/ikarus-project/ikarus/actions/workflows/style.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/workflows/style.yml)
 [![Docs](https://github.com/ikarus-project/ikarus/actions/workflows/ghpages.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/workflows/ghpages.yml)
 [![CodeFactor](https://www.codefactor.io/repository/github/ikarus-project/ikarus/badge/main)](https://www.codefactor.io/repository/github/ikarus-project/ikarus/overview/main)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/5c588e67d1e541fc9be3c7377297aa8a)](https://www.codacy.com/gh/ikarus-project/ikarus/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ikarus-project/ikarus&amp;utm_campaign=Badge_Grade)
 [![Gitter](https://badges.gitter.im/ikarus-project/community.svg)](https://gitter.im/ikarus-project/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
```

#### html2text {}

```diff
@@ -1,23 +1,25 @@
- # Ikarus [![Debian](https://github.com/ikarus-project/ikarus/actions/
-workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/ikarus/
-actions/workflows/debian.yml) [![codecov](https://codecov.io/gh/ikarus-project/
-ikarus/branch/main/graph/badge.svg?token=zJgggitPMc)](https://codecov.io/gh/
-ikarus-project/ikarus) [![CodeStyle](https://github.com/ikarus-project/ikarus/
-actions/workflows/style.yml/badge.svg)](https://github.com/ikarus-project/
-ikarus/actions/workflows/style.yml) [![Docs](https://github.com/ikarus-project/
-ikarus/actions/workflows/ghpages.yml/badge.svg)](https://github.com/ikarus-
-project/ikarus/actions/workflows/ghpages.yml) [![CodeFactor](https://
-www.codefactor.io/repository/github/ikarus-project/ikarus/badge/main)](https://
-www.codefactor.io/repository/github/ikarus-project/ikarus/overview/main) [!
-[Codacy Badge](https://app.codacy.com/project/badge/Grade/
-5c588e67d1e541fc9be3c7377297aa8a)](https://www.codacy.com/gh/ikarus-project/
-ikarus/dashboard?utm_source=github.com&utm_medium=referral&utm_content=ikarus-
-project/ikarus&utm_campaign=Badge_Grade) [![Gitter](https://badges.gitter.im/
-ikarus-project/community.svg)](https://gitter.im/ikarus-project/
+ # Ikarus [docs/website/auxiliaryImages/BigLogo.png]
+
+[![Debian](https://github.com/ikarus-project/ikarus/actions/workflows/
+debian.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/
+workflows/debian.yml) [![codecov](https://codecov.io/gh/ikarus-project/ikarus/
+branch/main/graph/badge.svg?token=zJgggitPMc)](https://codecov.io/gh/ikarus-
+project/ikarus) [![CodeStyle](https://github.com/ikarus-project/ikarus/actions/
+workflows/style.yml/badge.svg)](https://github.com/ikarus-project/ikarus/
+actions/workflows/style.yml) [![Docs](https://github.com/ikarus-project/ikarus/
+actions/workflows/ghpages.yml/badge.svg)](https://github.com/ikarus-project/
+ikarus/actions/workflows/ghpages.yml) [![CodeFactor](https://www.codefactor.io/
+repository/github/ikarus-project/ikarus/badge/main)](https://www.codefactor.io/
+repository/github/ikarus-project/ikarus/overview/main) [![Codacy Badge](https:/
+/app.codacy.com/project/badge/Grade/5c588e67d1e541fc9be3c7377297aa8a)](https://
+www.codacy.com/gh/ikarus-project/ikarus/
+dashboard?utm_source=github.com&utm_medium=referral&utm_content=ikarus-project/
+ikarus&utm_campaign=Badge_Grade) [![Gitter](https://badges.gitter.im/ikarus-
+project/community.svg)](https://gitter.im/ikarus-project/
 community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge) [![PyPI
 version](https://badge.fury.io/py/pyikarus.svg)](https://badge.fury.io/py/
 pyikarus) [![Release](https://badgen.net/badge/Release/0.3/purple?icon=github)]
 (https://github.com/ikarus-project/ikarus/releases) [![Doi](https://
 img.shields.io/badge/DOI-10.18419%2Fdarus--3303-orange)](https://doi.org/
 10.18419/darus-3303) [![SWH](https://archive.softwareheritage.org/badge/origin/
 https://github.com/ikarus-project/ikarus/)](https://
```

### Comparing `pyikarus-0.3.3.dev20230605190030/cmake/CPM.cmake` & `pyikarus-0.3.3.dev20230615091249/cmake/CPM.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/cmake/FormatTarget/CMakeLists.txt` & `pyikarus-0.3.3.dev20230615091249/cmake/FormatTarget/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/cmake/modules/AddAutoDiffFlags.cmake` & `pyikarus-0.3.3.dev20230615091249/cmake/modules/AddAutoDiffFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/cmake/modules/AddEigenFlags.cmake` & `pyikarus-0.3.3.dev20230615091249/cmake/modules/AddEigenFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/cmake/modules/AddMatplotppFlags.cmake` & `pyikarus-0.3.3.dev20230615091249/cmake/modules/AddMatplotppFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/cmake/modules/AddSpdlogFlags.cmake` & `pyikarus-0.3.3.dev20230615091249/cmake/modules/AddSpdlogFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/cmake/modules/AddSpectraFlags.cmake` & `pyikarus-0.3.3.dev20230615091249/cmake/modules/AddSpectraFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/cmake/tools.cmake` & `pyikarus-0.3.3.dev20230615091249/cmake/tools.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/config.h.cmake` & `pyikarus-0.3.3.dev20230615091249/config.h.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/__pycache__/mkdocs-macros.cpython-39.pyc` & `pyikarus-0.3.3.dev20230615091249/docs/__pycache__/mkdocs-macros.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/literature.bib` & `pyikarus-0.3.3.dev20230615091249/docs/literature.bib`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/mkdocs-macros.py` & `pyikarus-0.3.3.dev20230615091249/docs/mkdocs-macros.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/mkdocs.yml` & `pyikarus-0.3.3.dev20230615091249/docs/mkdocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Copyright
 copyright: 'Copyright &copy; 2021 The Ikarus Developers'
 
 # Configuration
 theme:
   name: material
   custom_dir: overrides
-  logo: auxiliaryImages/logo_white.svg
-  favicon: auxiliaryImages/logo_blue.svg
+  logo: auxiliaryImages/logo_white.png
+  favicon: auxiliaryImages/logo_blue.png
   features:
     - navigation.instant
     - content.code.annotate
     - navigation.tabs
     - navigation.tracking
     - navigation.sections
     - navigation.expand
```

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/overrides/partials/comments.html` & `pyikarus-0.3.3.dev20230615091249/docs/overrides/partials/comments.html`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/assembler.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/assembler.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/controlRoutines.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/controlRoutines.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/dirichletBCs.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/dirichletBCs.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/feRequirements.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/feRequirements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/finiteElements.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/finiteElements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/grids.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/grids.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/index.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/localBasis.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/localBasis.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/localFunctions.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/localFunctions.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/manifolds.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/manifolds.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/nonlinearOperator.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/nonlinearOperator.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/observer.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/observer.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/01_framework/solvers.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/01_framework/solvers.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/02_examples/cantileverBeam.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/02_examples/cantileverBeam.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/02_examples/computePi.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/02_examples/computePi.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/02_examples/cooksMembrane.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/02_examples/cooksMembrane.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/02_examples/incompressibleRubberBlock.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/02_examples/incompressibleRubberBlock.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/02_examples/index.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/02_examples/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/02_examples/kirchhoffPlate.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/02_examples/kirchhoffPlate.md`

 * *Files 3% similar despite different names*

```diff
@@ -73,25 +73,25 @@
 3. The knot vector for the NURBS grid.
 4. Length of the plate
 5. Width of the plate
 6. Control points and the weights for the square plate (the control points are ordered such that all the control points for a particular $x$-position are listed first, followed by the subsequent $x$-positions in ascending order).
 7. Number of control points in either direction.
 8. Creation of the control net.
 9. Binding the `knotSpans` to a particular NURBS `patchData`.
-10. The polynomial degree for the basis in either directions. It can also be calculated from the `knotSpans`.
+10. The polynomial degree for the basis in either direction. It can also be calculated from the `knotSpans`.
 11. Binding the `controlNet` to a particular NURBS `patchData`.
 12. Elevating the polynomial degree for the `patchData` in $x$-direction (`0`) by 1.
 13. Elevating the polynomial degree for the `patchData` in $y$-direction (`1`) by 1.
 14. Creating the grid object from the patch data
 
 In order to obtain the convergence plots, the system is solved five times, with the refinement level 
-increasing by 1 each time using the command `#!cpp grid.globalRefine(1);`. The NURBS basis can be obtained directly from the 
-NURBS grid using the `getPreBasis()` function, as shown below:
+increasing by 1 each time using the command `#!cpp grid.globalRefine(1);`.
+The NURBS basis can be obtained from the freestanding functions `nurbs()`, as shown below:
 ```cpp
-auto basis = Ikarus::makeBasis(gridView, gridView.impl().getPreBasis());
+auto basis = Ikarus::makeBasis(gridView, nurbs());
 ```
 This is followed by specifying the Dirichlet boundary conditions, creating the finite elements and the assembler, 
 solving the system of equations, and post-processing using Paraview as mentioned in the previous examples.
 The analytical solution for the simply supported case is adapted from 
 [Wikipedia](https://en.wikipedia.org/wiki/Bending_of_plates#Simply-supported_plate_with_uniformly-distributed_load) and is also mentioned below: 
 ```cpp
 auto wAna = [&](auto x) {
@@ -149,10 +149,10 @@
 dofsVec.push_back(basis.flat().size());
 l2Evcector.push_back(l2_error);
 ```
 
 ## Takeaways
 
 - NURBS grids can be created using the `dune-iga` module.
-- The basis for the corresponding NURBS grid can be obtained using the `getPreBasis()` function.
+- The basis for the corresponding NURBS grid can be obtained using the `nurbs()` function.
 - The Kirchhoff plate element can be easily implemented by evaluating the energy and using automatic differentiation methods.
 - $L^2$-error can be evaluated to perform convergence studies.
```

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/02_examples/newtonRaphsonMethod.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/02_examples/newtonRaphsonMethod.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/02_examples/nonLinearElasticity.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/02_examples/nonLinearElasticity.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/02_examples/vonMisesTruss.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/02_examples/vonMisesTruss.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/03_contribution/buildDocumentationLocally.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/03_contribution/buildDocumentationLocally.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/03_contribution/codeStyle.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/03_contribution/codeStyle.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/03_contribution/howToEdit.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/03_contribution/howToEdit.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/03_contribution/openTask.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/03_contribution/openTask.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/04_blog/posts/v0.3.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/04_blog/posts/v0.3.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/05_cppReferences/cppRef.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/05_cppReferences/cppRef.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png` & `pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/Installation/CMakeOutput.png` & `pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/Installation/CMakeOutput.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/Installation/ClionFooter.png` & `pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/Installation/ClionFooter.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/Installation/DockerWslSettings.png` & `pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/Installation/DockerWslSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png` & `pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png` & `pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png` & `pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png` & `pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png` & `pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png` & `pyikarus-0.3.3.dev20230615091249/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/download.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/download.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/docs/website/index.md` & `pyikarus-0.3.3.dev20230615091249/docs/website/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 <!--
 SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 SPDX-License-Identifier: CC-BY-SA-4.0
 -->
 
 # Welcome to the documentation of Ikarus
+
+![](auxiliaryImages/BigLogo.png){ align=right width=400 }
+
 Ikarus is a C++-based library built within the finite element architecture. It originated at the [Institute for Structural Mechanics](https://www.ibb.uni-stuttgart.de/en/) at the University of Stuttgart.
 
 This project tries to provide an easy-to-read and an easy-to-use finite element framework.
 It is heavily inspired by the finite element software [DUNE](https://dune-project.org/), the book [DUNE — The Distributed and Unified Numerics Environment](https://www.springer.com/gp/book/9783030597016),
 [deal.II](https://www.dealii.org/) and [Kratos](https://github.com/KratosMultiphysics/Kratos).
 Furthermore, it directly uses several modules from [DUNE](https://dune-project.org/).
 
 The design of CI and the documentation were inspired by [Autodiff](https://autodiff.github.io/)  and [Kratos](https://github.com/KratosMultiphysics/Kratos).
 
 The documentation is built using [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).
 
 Ikarus provides the tools to create one's own examples and rapidly prototype finite element solution algorithms. 
-This is done by using template metaprogramming in C++ to write generic code, which is compiled for the example.
+This is done by using template metaprogramming in C++ to write generic code, which is compiled for the example.
```

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/CMakeLists.txt` & `pyikarus-0.3.3.dev20230615091249/ikarus/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/assembler/simpleAssemblers.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/assembler/simpleAssemblers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/assembler/simpleAssemblers.inl` & `pyikarus-0.3.3.dev20230615091249/ikarus/assembler/simpleAssemblers.inl`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/controlRoutines/loadControl.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/controlRoutines/loadControl.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/controlRoutines/pathFollowingTechnique.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/controlRoutines/pathFollowingTechnique.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/feBases/autodiffFE.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/feBases/autodiffFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/feBases/powerBasisFE.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/feBases/powerBasisFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/feBases/scalarFE.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/feBases/scalarFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/feRequirements.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/feRequirements.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/feTraits.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/feTraits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/linearElastic.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/linearElastic.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 // SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 // SPDX-License-Identifier: LGPL-3.0-or-later
 
 #pragma once
+#include <iosfwd>
+#include <optional>
+#include <type_traits>
 
 #include <dune/common/classname.hh>
 #include <dune/fufem/boundarypatch.hh>
 #include <dune/geometry/quadraturerules.hh>
 #include <dune/geometry/type.hh>
 #include <dune/localfefunctions/expressions/linearStrainsExpr.hh>
 #include <dune/localfefunctions/impl/standardLocalFunction.hh>
@@ -47,18 +50,25 @@
                   NeumannBoundaryLoad p_neumannBoundaryLoad = {})
         : BaseDisp(globalBasis.flat(), element), neumannBoundary{p_neumannBoundary}, emod_{emod}, nu_{nu} {
       this->localView().bind(element);
       auto& first_child = this->localView().tree().child(0);
       const auto& fe    = first_child.finiteElement();
       numberOfNodes     = fe.size();
       dispAtNodes.resize(fe.size());
-      const int order = 2 * (this->localView().tree().child(0).finiteElement().localBasis().order());
-      localBasis      = Dune::CachedLocalBasis(this->localView().tree().child(0).finiteElement().localBasis());
-      localBasis.bind(Dune::QuadratureRules<double, myDim>::rule(this->localView().element().type(), order),
-                      Dune::bindDerivatives(0, 1));
+       order      = 2 * (this->localView().tree().child(0).finiteElement().localBasis().order());
+      localBasis = Dune::CachedLocalBasis(this->localView().tree().child(0).finiteElement().localBasis());
+      if constexpr (requires { this->localView().element().impl().getQuadratureRule(order); })
+        if (this->localView().element().impl().isTrimmed())
+          localBasis.bind(this->localView().element().impl().getQuadratureRule(order), Dune::bindDerivatives(0, 1));
+        else
+          localBasis.bind(Dune::QuadratureRules<double, myDim>::rule(this->localView().element().type(), order),
+                        Dune::bindDerivatives(0, 1));
+      else
+        localBasis.bind(Dune::QuadratureRules<double, myDim>::rule(this->localView().element().type(), order),
+                        Dune::bindDerivatives(0, 1));
 
       if constexpr (!std::is_same_v<VolumeLoad, LoadDefault>) volumeLoad = p_volumeLoad;
       if constexpr (!std::is_same_v<NeumannBoundaryLoad, LoadDefault>) neumannBoundaryLoad = p_neumannBoundaryLoad;
 
       assert(((not p_neumannBoundary and not neumannBoundaryLoad) or (p_neumannBoundary and neumannBoundaryLoad))
              && "If you pass a Neumann boundary you should also pass the function for the Neumann load!");
     }
@@ -160,14 +170,15 @@
                                                           const double&)>
         neumannBoundaryLoad;
     const BoundaryPatch<GridView>* neumannBoundary;
     mutable Dune::BlockVector<Dune::RealTuple<double, Traits::dimension>> dispAtNodes;
     double emod_;
     double nu_;
     size_t numberOfNodes{0};
+    int order{};
 
   protected:
     template <typename ScalarType>
     auto calculateScalarImpl(const FERequirementType& par, const std::optional<const Eigen::VectorX<ScalarType>>& dx
                                                            = std::nullopt) const -> ScalarType {
       const auto u       = getDisplacementFunction(par, dx);
       const auto eps     = getStrainFunction(par, dx);
@@ -190,22 +201,22 @@
         for (const auto& [gpIndex, gp] : eps.viewOverIntegrationPoints()) {
           const auto uVal                              = u.evaluate(gpIndex);
           Eigen::Vector<double, Traits::worlddim> fext = volumeLoad(toEigen(geo.global(gp.position())), lambda);
           energy -= uVal.dot(fext) * geo.integrationElement(gp.position()) * gp.weight();
         }
       }
 
-      // line or surface loads, i.e. neumann boundary
+      // line or surface loads, i.e., neumann boundary
       if (not neumannBoundary and not neumannBoundaryLoad) return energy;
 
       auto element = this->localView().element();
       for (auto&& intersection : intersections(neumannBoundary->gridView(), element)) {
         if (not neumannBoundary->contains(intersection)) continue;
 
-        const auto& quadLine = Dune::QuadratureRules<double, myDim - 1>::rule(intersection.type(), u.order());
+        const auto& quadLine = Dune::QuadratureRules<double, myDim - 1>::rule(intersection.type(), order);
 
         for (const auto& curQuad : quadLine) {
           // Local position of the quadrature point
           const Dune::FieldVector<double, myDim>& quadPos = intersection.geometryInInside().global(curQuad.position());
 
           const double integrationElement = intersection.geometry().integrationElement(curQuad.position());
 
@@ -260,15 +271,15 @@
 
       const auto u = getDisplacementFunction(par, dx);
       auto element = this->localView().element();
       for (auto&& intersection : intersections(neumannBoundary->gridView(), element)) {
         if (not neumannBoundary->contains(intersection)) continue;
 
         // Integration rule along the boundary
-        const auto& quadLine = Dune::QuadratureRules<double, myDim - 1>::rule(intersection.type(), u.order());
+        const auto& quadLine = Dune::QuadratureRules<double, myDim - 1>::rule(intersection.type(), order);
 
         for (const auto& curQuad : quadLine) {
           const Dune::FieldVector<double, myDim>& quadPos = intersection.geometryInInside().global(curQuad.position());
 
           const double integrationElement = intersection.geometry().integrationElement(curQuad.position());
 
           // The value of the local function wrt the i-th coef
```

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/materials/interface.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/materials/interface.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/materials/linearElasticity.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/materials/linearElasticity.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/materials/neohooke.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/materials/neohooke.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/materials/strainConversions.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/materials/strainConversions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/materials/svk.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/materials/svk.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/materials/vanishingStress.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/materials/vanishingStress.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/materials.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/materials.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/mechanics/nonLinearElastic.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/mechanics/nonLinearElastic.hh`

 * *Files 2% similar despite different names*

```diff
@@ -48,18 +48,26 @@
                      NeumannBoundaryLoad p_neumannBoundaryLoad = {})
         : BasePowerFE(globalBasis.flat(), element), neumannBoundary{p_neumannBoundary}, mat{p_mat} {
       this->localView().bind(element);
       auto& first_child = this->localView().tree().child(0);
       const auto& fe    = first_child.finiteElement();
       numberOfNodes     = fe.size();
       dispAtNodes.resize(fe.size());
-      const int order = 2 * (this->localView().tree().child(0).finiteElement().localBasis().order());
+      order = 2 * (this->localView().tree().child(0).finiteElement().localBasis().order());
       localBasis      = Dune::CachedLocalBasis(this->localView().tree().child(0).finiteElement().localBasis());
-      localBasis.bind(Dune::QuadratureRules<double, Traits::mydim>::rule(this->localView().element().type(), order),
-                      Dune::bindDerivatives(0, 1));
+      if constexpr (requires { this->localView().element().impl().getQuadratureRule(order); })
+        if (this->localView().element().impl().isTrimmed())
+          localBasis.bind(this->localView().element().impl().getQuadratureRule(order), Dune::bindDerivatives(0, 1));
+        else
+          localBasis.bind(Dune::QuadratureRules<double, myDim>::rule(this->localView().element().type(), order),
+                          Dune::bindDerivatives(0, 1));
+      else
+        localBasis.bind(Dune::QuadratureRules<double, myDim>::rule(this->localView().element().type(), order),
+                        Dune::bindDerivatives(0, 1));
+
       if constexpr (!std::is_same_v<VolumeLoad, LoadDefault>) volumeLoad = p_volumeLoad;
       if constexpr (!std::is_same_v<NeumannBoundaryLoad, LoadDefault>) neumannBoundaryLoad = p_neumannBoundaryLoad;
 
       assert(((not p_neumannBoundary and not neumannBoundaryLoad) or (p_neumannBoundary and neumannBoundaryLoad))
              && "If you pass a Neumann boundary you should also pass the function for the Neumann load!");
     }
 
@@ -178,14 +186,15 @@
     std::function<Eigen::Vector<double, Traits::worlddim>(const Eigen::Vector<double, Traits::worlddim>&,
                                                           const double&)>
         neumannBoundaryLoad;
     const BoundaryPatch<GridView>* neumannBoundary;
     Material mat;
     mutable Dune::BlockVector<Dune::RealTuple<double, Traits::dimension>> dispAtNodes;
     size_t numberOfNodes{0};
+    int order{};
 
   protected:
     template <typename ScalarType>
     auto calculateScalarImpl(const FERequirementType& par, const std::optional<const Eigen::VectorX<ScalarType>>& dx
                                                            = std::nullopt) const -> ScalarType {
       using namespace Dune::DerivativeDirections;
       using namespace Dune;
@@ -205,23 +214,23 @@
         for (const auto& [gpIndex, gp] : uFunction.viewOverIntegrationPoints()) {
           const auto u                                       = uFunction.evaluate(gpIndex);
           const Eigen::Vector<double, Traits::worlddim> fExt = volumeLoad(toEigen(geo.global(gp.position())), lambda);
           energy -= u.dot(fExt) * geo.integrationElement(gp.position()) * gp.weight();
         }
       }
 
-      // line or surface loads, i.e. neumann boundary
+      // line or surface loads, i.e., neumann boundary
       if (not neumannBoundary and not neumannBoundaryLoad) return energy;
 
       const auto& element = this->localView().element();
       for (auto&& intersection : intersections(neumannBoundary->gridView(), element)) {
         if (not neumannBoundary or not neumannBoundary->contains(intersection)) continue;
 
         const auto& quadLine
-            = Dune::QuadratureRules<double, Traits::mydim - 1>::rule(intersection.type(), uFunction.order());
+            = Dune::QuadratureRules<double, Traits::mydim - 1>::rule(intersection.type(), order);
 
         for (const auto& curQuad : quadLine) {
           // Local position of the quadrature point
           const Dune::FieldVector<double, Traits::mydim>& quadPos
               = intersection.geometryInInside().global(curQuad.position());
 
           const double intElement = intersection.geometry().integrationElement(curQuad.position());
@@ -268,24 +277,24 @@
           for (size_t i = 0; i < numberOfNodes; ++i) {
             const auto udCi = u.evaluateDerivative(gpIndex, wrt(coeff(i)));
             force.template segment<myDim>(myDim * i) -= udCi * fExt * intElement;
           }
         }
       }
 
-      // External forces, boundary forces, i.e. at the Neumann boundary
+      // External forces, boundary forces, i.e., at the Neumann boundary
       if (not neumannBoundary and not neumannBoundaryLoad) return;
 
       const auto u        = getDisplacementFunction(par, dx);
       const auto& element = this->localView().element();
       for (auto&& intersection : intersections(neumannBoundary->gridView(), element)) {
         if (not neumannBoundary->contains(intersection)) continue;
 
         // Integration rule along the boundary
-        const auto& quadLine = Dune::QuadratureRules<double, myDim - 1>::rule(intersection.type(), u.order());
+        const auto& quadLine = Dune::QuadratureRules<double, myDim - 1>::rule(intersection.type(), order);
 
         for (const auto& curQuad : quadLine) {
           const Dune::FieldVector<double, myDim>& quadPos = intersection.geometryInInside().global(curQuad.position());
 
           const double intElement = intersection.geometry().integrationElement(curQuad.position());
 
           // The value of the local function wrt the i-th coefficient
```

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/finiteElements/physicsHelper.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/finiteElements/physicsHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/io/resultEvaluators.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/io/resultEvaluators.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/io/resultFunction.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/io/resultFunction.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/linearAlgebra/dirichletValues.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/linearAlgebra/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/linearAlgebra/nonLinearOperator.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/linearAlgebra/nonLinearOperator.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/linearAlgebra/truncatedConjugateGradient.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/linearAlgebra/truncatedConjugateGradient.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/python/assembler/flatAssembler.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/python/assembler/flatAssembler.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/python/basis/basis.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/python/basis/basis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/python/dirichletValues/dirichletValues.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/python/dirichletValues/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/python/finiteElements/linearElastic.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/python/finiteElements/linearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/python/finiteElements/materials/material.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/python/finiteElements/materials/material.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/python/finiteElements/nonLinearElastic.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/python/finiteElements/nonLinearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/python/test/linearElasticTest.py` & `pyikarus-0.3.3.dev20230615091249/ikarus/python/test/linearElasticTest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/python/test/nonLinearElasticTest.py` & `pyikarus-0.3.3.dev20230615091249/ikarus/python/test/nonLinearElasticTest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/python/test/setpath.py.in` & `pyikarus-0.3.3.dev20230615091249/ikarus/python/test/setpath.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/python/utils/boundarypatch.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/python/utils/boundarypatch.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/solver/linearSolver/linearSolver.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/solver/linearSolver/linearSolver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/solver/nonLinearSolver/newtonRaphson.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/solver/nonLinearSolver/newtonRaphson.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/solver/nonLinearSolver/trustRegion.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/solver/nonLinearSolver/trustRegion.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/CMakeLists.txt` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/algorithms.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/algorithms.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/autodiffHelper.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/autodiffHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/basis.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/basis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/concepts.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/concepts.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/drawing/griddrawer.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/drawing/griddrawer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/drawing/matplotHelper.cpp` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/drawing/matplotHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/drawing/matplotHelper.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/drawing/matplotHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/duneUtilities.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/duneUtilities.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/eigenDuneTransformations.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/eigenDuneTransformations.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/eigenSparseAddon.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/eigenSparseAddon.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/findLineSegment.cpp` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/findLineSegment.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/findLineSegment.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/findLineSegment.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/flatPreBasis.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/flatPreBasis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/functionSanityChecks.cpp` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/functionSanityChecks.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/functionSanityChecks.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/functionSanityChecks.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/init.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/init.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/linearAlgebraHelper.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/linearAlgebraHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/makeEnum.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/makeEnum.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/observer/controlLogger.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/observer/controlLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/observer/controlVTKWriter.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/observer/controlVTKWriter.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/observer/genericControlObserver.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/observer/genericControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/observer/gridDrawerObserver.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/observer/gridDrawerObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/observer/loadControlObserver.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/observer/loadControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/observer/nonLinearSolverLogger.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/observer/nonLinearSolverLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/observer/observer.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/observer/observer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/pathFollowingFunctions.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/pathFollowingFunctions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/polyfit.cpp` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/polyfit.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/polyfit.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/polyfit.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/tensorUtils.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/tensorUtils.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/ikarus/utils/traits.hh` & `pyikarus-0.3.3.dev20230615091249/ikarus/utils/traits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/python/ikarus/__init__.py` & `pyikarus-0.3.3.dev20230615091249/python/ikarus/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/python/ikarus/_ikarus.cc` & `pyikarus-0.3.3.dev20230615091249/python/ikarus/_ikarus.cc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/python/ikarus/assembler/__init__.py` & `pyikarus-0.3.3.dev20230615091249/python/ikarus/assembler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/python/ikarus/basis.py` & `pyikarus-0.3.3.dev20230615091249/python/ikarus/basis.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/python/ikarus/dirichletValues.py` & `pyikarus-0.3.3.dev20230615091249/python/ikarus/dirichletValues.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/python/ikarus/finite_elements/__init__.py` & `pyikarus-0.3.3.dev20230615091249/python/ikarus/finite_elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/python/ikarus/generator.py` & `pyikarus-0.3.3.dev20230615091249/python/ikarus/generator.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/python/ikarus/materials.py` & `pyikarus-0.3.3.dev20230615091249/python/ikarus/materials.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/python/ikarus/utils/__init__.py` & `pyikarus-0.3.3.dev20230615091249/python/ikarus/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/python/pyikarus.egg-info/PKG-INFO` & `pyikarus-0.3.3.dev20230615091249/python/pyikarus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.3.dev20230605190030
+Version: 0.3.3.dev20230615091249
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
@@ -13,14 +13,18 @@
 
 <!--
 SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 SPDX-License-Identifier: LGPL-3.0-or-later
 -->
 # Ikarus
 
+<img align="left" src="docs/website/auxiliaryImages/BigLogo.png" width="800">  
+
+<br/><br/>    
+
 [![Debian](https://github.com/ikarus-project/ikarus/actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/workflows/debian.yml)
 [![codecov](https://codecov.io/gh/ikarus-project/ikarus/branch/main/graph/badge.svg?token=zJgggitPMc)](https://codecov.io/gh/ikarus-project/ikarus)
 [![CodeStyle](https://github.com/ikarus-project/ikarus/actions/workflows/style.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/workflows/style.yml)
 [![Docs](https://github.com/ikarus-project/ikarus/actions/workflows/ghpages.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/workflows/ghpages.yml)
 [![CodeFactor](https://www.codefactor.io/repository/github/ikarus-project/ikarus/badge/main)](https://www.codefactor.io/repository/github/ikarus-project/ikarus/overview/main)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/5c588e67d1e541fc9be3c7377297aa8a)](https://www.codacy.com/gh/ikarus-project/ikarus/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ikarus-project/ikarus&amp;utm_campaign=Badge_Grade)
 [![Gitter](https://badges.gitter.im/ikarus-project/community.svg)](https://gitter.im/ikarus-project/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230605190030 Home-
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230615091249 Home-
 page: Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-
 stuttgart.de Classifier: Programming Language :: C++ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License (GPL) Requires-Python: >=3.4 Description-Content-Type: text/
-markdown License-File: LICENSE.md  # Ikarus [![Debian](https://github.com/
-ikarus-project/ikarus/actions/workflows/debian.yml/badge.svg)](https://
-github.com/ikarus-project/ikarus/actions/workflows/debian.yml) [![codecov]
-(https://codecov.io/gh/ikarus-project/ikarus/branch/main/graph/
-badge.svg?token=zJgggitPMc)](https://codecov.io/gh/ikarus-project/ikarus) [!
-[CodeStyle](https://github.com/ikarus-project/ikarus/actions/workflows/
-style.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/
-workflows/style.yml) [![Docs](https://github.com/ikarus-project/ikarus/actions/
-workflows/ghpages.yml/badge.svg)](https://github.com/ikarus-project/ikarus/
-actions/workflows/ghpages.yml) [![CodeFactor](https://www.codefactor.io/
+markdown License-File: LICENSE.md  # Ikarus [docs/website/auxiliaryImages/
+BigLogo.png]
+
+[![Debian](https://github.com/ikarus-project/ikarus/actions/workflows/
+debian.yml/badge.svg)](https://github.com/ikarus-project/ikarus/actions/
+workflows/debian.yml) [![codecov](https://codecov.io/gh/ikarus-project/ikarus/
+branch/main/graph/badge.svg?token=zJgggitPMc)](https://codecov.io/gh/ikarus-
+project/ikarus) [![CodeStyle](https://github.com/ikarus-project/ikarus/actions/
+workflows/style.yml/badge.svg)](https://github.com/ikarus-project/ikarus/
+actions/workflows/style.yml) [![Docs](https://github.com/ikarus-project/ikarus/
+actions/workflows/ghpages.yml/badge.svg)](https://github.com/ikarus-project/
+ikarus/actions/workflows/ghpages.yml) [![CodeFactor](https://www.codefactor.io/
 repository/github/ikarus-project/ikarus/badge/main)](https://www.codefactor.io/
 repository/github/ikarus-project/ikarus/overview/main) [![Codacy Badge](https:/
 /app.codacy.com/project/badge/Grade/5c588e67d1e541fc9be3c7377297aa8a)](https://
 www.codacy.com/gh/ikarus-project/ikarus/
 dashboard?utm_source=github.com&utm_medium=referral&utm_content=ikarus-project/
 ikarus&utm_campaign=Badge_Grade) [![Gitter](https://badges.gitter.im/ikarus-
 project/community.svg)](https://gitter.im/ikarus-project/
```

### Comparing `pyikarus-0.3.3.dev20230605190030/python/pyikarus.egg-info/SOURCES.txt` & `pyikarus-0.3.3.dev20230615091249/python/pyikarus.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -86,18 +86,19 @@
 docs/website/03_contribution/howToEdit.md
 docs/website/03_contribution/openTask.md
 docs/website/04_blog/.authors.yml
 docs/website/04_blog/index.md
 docs/website/04_blog/posts/v0.3.md
 docs/website/05_cppReferences/cppRef.md
 docs/website/99_Literature/99_Literature.md
-docs/website/auxiliaryImages/logo_blue.svg
-docs/website/auxiliaryImages/logo_blue.svg.license
-docs/website/auxiliaryImages/logo_white.svg
-docs/website/auxiliaryImages/logo_white.svg.license
+docs/website/auxiliaryImages/BigLogo.png
+docs/website/auxiliaryImages/logo_blue.png
+docs/website/auxiliaryImages/logo_blue.png.license
+docs/website/auxiliaryImages/logo_white.png
+docs/website/auxiliaryImages/logo_white.png.license
 docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
 docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
 docs/website/auxiliaryImages/Installation/CMakeOutput.png
 docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
 docs/website/auxiliaryImages/Installation/ClionFooter.png
 docs/website/auxiliaryImages/Installation/ClionFooter.png.license
 docs/website/auxiliaryImages/Installation/DockerWslSettings.png
```

### Comparing `pyikarus-0.3.3.dev20230605190030/python/setup.py.in` & `pyikarus-0.3.3.dev20230615091249/python/setup.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/sandbox/src/CMakeLists.txt` & `pyikarus-0.3.3.dev20230615091249/sandbox/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/sandbox/src/auxiliaryFiles/circle.msh` & `pyikarus-0.3.3.dev20230615091249/sandbox/src/auxiliaryFiles/circle.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/setup.py` & `pyikarus-0.3.3.dev20230615091249/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # build _ikarus
 # cd /tmp/Ikarus
 # /dune/dune-common/build-cmake/run-in-dune-env pip install twine scikit-build
 # git config --global --add safe.directory /tmp/Ikarus
 # /dune/dune-common/build-cmake/run-in-dune-env python setup.py sdist
 # /dune/dune-common/build-cmake/run-in-dune-env python -m twine upload dist/* --verbose
 
-ikarusVersion = "0.3.3.dev20230605190030"
+ikarusVersion = "0.3.3.dev20230615091249"
 duneVersion = "2.9.0"
 
 metadata = metaData(duneVersion)[1]
 metadata["version"] = ikarusVersion
 
 # refactor since ikarus pypi package already exists
 metadata["name"] = "pyikarus"
```

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/CMakeLists.txt` & `pyikarus-0.3.3.dev20230615091249/tests/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testAssembler.cpp` & `pyikarus-0.3.3.dev20230615091249/tests/src/testAssembler.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testAutodiffHelper.cpp` & `pyikarus-0.3.3.dev20230615091249/tests/src/testAutodiffHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testCommon.hh` & `pyikarus-0.3.3.dev20230615091249/tests/src/testCommon.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testDependencies.cpp` & `pyikarus-0.3.3.dev20230615091249/tests/src/testDependencies.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testDirichletValue.cpp` & `pyikarus-0.3.3.dev20230615091249/tests/src/testDirichletValue.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testEAS.hh` & `pyikarus-0.3.3.dev20230615091249/tests/src/testEAS.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testEnhancedAssumedStrains.cpp` & `pyikarus-0.3.3.dev20230615091249/tests/src/testEnhancedAssumedStrains.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testFEElement.hh` & `pyikarus-0.3.3.dev20230615091249/tests/src/testFEElement.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testFactories.hh` & `pyikarus-0.3.3.dev20230615091249/tests/src/testFactories.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testFiles/unstructuredQuadscoarse.msh` & `pyikarus-0.3.3.dev20230615091249/tests/src/testFiles/unstructuredQuadscoarse.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testFiles/unstructuredTest2.geo` & `pyikarus-0.3.3.dev20230615091249/tests/src/testFiles/unstructuredTest2.geo`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testFiles/unstructuredTrianglesfine.msh` & `pyikarus-0.3.3.dev20230615091249/tests/src/testFiles/unstructuredTrianglesfine.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testFunctionTraits.cpp` & `pyikarus-0.3.3.dev20230615091249/tests/src/testFunctionTraits.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testHelpers.hh` & `pyikarus-0.3.3.dev20230615091249/tests/src/testHelpers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testLinearElasticity.cpp` & `pyikarus-0.3.3.dev20230615091249/tests/src/testLinearElasticity.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testManifolds.cpp` & `pyikarus-0.3.3.dev20230615091249/tests/src/testManifolds.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testMaterial.cpp` & `pyikarus-0.3.3.dev20230615091249/tests/src/testMaterial.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testNonLinearElasticity.hh` & `pyikarus-0.3.3.dev20230615091249/tests/src/testNonLinearElasticity.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testNonLinearElasticityNeoHooke.cpp` & `pyikarus-0.3.3.dev20230615091249/tests/src/testNonLinearElasticityNeoHooke.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testNonLinearElasticitySVK.cpp` & `pyikarus-0.3.3.dev20230615091249/tests/src/testNonLinearElasticitySVK.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testNonLinearOperator.cpp` & `pyikarus-0.3.3.dev20230615091249/tests/src/testNonLinearOperator.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testPathFollowing.cpp` & `pyikarus-0.3.3.dev20230615091249/tests/src/testPathFollowing.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testPolyFit.cpp` & `pyikarus-0.3.3.dev20230615091249/tests/src/testPolyFit.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testPythonConversion.cpp` & `pyikarus-0.3.3.dev20230615091249/tests/src/testPythonConversion.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230605190030/tests/src/testTrustRegion.cpp` & `pyikarus-0.3.3.dev20230615091249/tests/src/testTrustRegion.cpp`

 * *Files identical despite different names*

