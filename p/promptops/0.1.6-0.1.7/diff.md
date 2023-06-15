# Comparing `tmp/promptops-0.1.6.tar.gz` & `tmp/promptops-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptops-0.1.6.tar", last modified: Wed Jun  7 22:03:36 2023, max compression
+gzip compressed data, was "promptops-0.1.7.tar", last modified: Thu Jun 15 19:16:09 2023, max compression
```

## Comparing `promptops-0.1.6.tar` & `promptops-0.1.7.tar`

### file list

```diff
@@ -1,103 +1,107 @@
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.969483 promptops-0.1.6/
--rw-r--r--   0 vasily     (501) staff       (20)    35149 2023-05-24 15:22:16.000000 promptops-0.1.6/LICENSE.txt
--rw-r--r--   0 vasily     (501) staff       (20)     2255 2023-06-07 22:03:36.969644 promptops-0.1.6/PKG-INFO
--rw-r--r--   0 vasily     (501) staff       (20)     1618 2023-06-07 21:55:02.000000 promptops-0.1.6/README.md
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.943019 promptops-0.1.6/local_runner/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/__init__.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.944510 promptops-0.1.6/local_runner/comms/
--rw-r--r--   0 vasily     (501) staff       (20)      133 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/comms/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      432 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/comms/base.py
--rw-r--r--   0 vasily     (501) staff       (20)     2890 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/comms/dtos.py
--rw-r--r--   0 vasily     (501) staff       (20)     1536 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/comms/http_reporter.py
--rw-r--r--   0 vasily     (501) staff       (20)     1671 2023-06-07 21:55:02.000000 promptops-0.1.6/local_runner/comms/ws.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.945187 promptops-0.1.6/local_runner/config/
--rw-r--r--   0 vasily     (501) staff       (20)       48 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/config/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     1720 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/config/config.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.945777 promptops-0.1.6/local_runner/creds/
--rw-r--r--   0 vasily     (501) staff       (20)       77 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/creds/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     1458 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/creds/creds.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.946278 promptops-0.1.6/local_runner/exec/
--rw-r--r--   0 vasily     (501) staff       (20)       54 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/exec/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2317 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/exec/manager.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.947046 promptops-0.1.6/local_runner/handler/
--rw-r--r--   0 vasily     (501) staff       (20)       29 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/handler/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      471 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/handler/censor.py
--rw-r--r--   0 vasily     (501) staff       (20)     3115 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/handler/handler.py
--rw-r--r--   0 vasily     (501) staff       (20)     1361 2023-06-07 21:55:02.000000 promptops-0.1.6/local_runner/main.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.947653 promptops-0.1.6/local_runner/registration/
--rw-r--r--   0 vasily     (501) staff       (20)       56 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/registration/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2523 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/registration/registration.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.948334 promptops-0.1.6/local_runner/tokens/
--rw-r--r--   0 vasily     (501) staff       (20)       27 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/tokens/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2235 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/tokens/issuer.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.952869 promptops-0.1.6/promptops/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     1850 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/corrections.py
--rw-r--r--   0 vasily     (501) staff       (20)     1033 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/feedback.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.955747 promptops-0.1.6/promptops/gitaware/
--rw-r--r--   0 vasily     (501) staff       (20)       42 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/gitaware/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      632 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/gitaware/project.py
--rw-r--r--   0 vasily     (501) staff       (20)     4146 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/history.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.957085 promptops-0.1.6/promptops/index/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/index/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2692 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/index/content.py
--rw-r--r--   0 vasily     (501) staff       (20)     2084 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/index/entry_point.py
--rw-r--r--   0 vasily     (501) staff       (20)     4399 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/index/index_store.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.959503 promptops-0.1.6/promptops/loading/
--rw-r--r--   0 vasily     (501) staff       (20)      131 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/loading/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      677 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/loading/base.py
--rw-r--r--   0 vasily     (501) staff       (20)      481 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/loading/context.py
--rw-r--r--   0 vasily     (501) staff       (20)     1279 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/loading/pong.py
--rw-r--r--   0 vasily     (501) staff       (20)     1344 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/loading/progress.py
--rw-r--r--   0 vasily     (501) staff       (20)     1077 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/loading/promptops.py
--rw-r--r--   0 vasily     (501) staff       (20)     1025 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/loading/simple.py
--rw-r--r--   0 vasily     (501) staff       (20)     8515 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/main.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.961698 promptops-0.1.6/promptops/query/
--rw-r--r--   0 vasily     (501) staff       (20)       30 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/query/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      434 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/query/dtos.py
--rw-r--r--   0 vasily     (501) staff       (20)     4351 2023-05-25 18:38:08.000000 promptops-0.1.6/promptops/query/explanation.py
--rw-r--r--   0 vasily     (501) staff       (20)     4506 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/query/git_repo.py
--rw-r--r--   0 vasily     (501) staff       (20)     1222 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/query/messages.py
--rw-r--r--   0 vasily     (501) staff       (20)    18387 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/query/query.py
--rw-r--r--   0 vasily     (501) staff       (20)     1126 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/query.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.962814 promptops-0.1.6/promptops/recipes/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/recipes/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     8841 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/recipes/creation.py
--rw-r--r--   0 vasily     (501) staff       (20)     5466 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/recipes/terraform.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.963623 promptops-0.1.6/promptops/scrub_secrets/
--rw-r--r--   0 vasily     (501) staff       (20)       55 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/scrub_secrets/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/scrub_secrets/scrub.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.964439 promptops-0.1.6/promptops/secrets/
--rw-r--r--   0 vasily     (501) staff       (20)       55 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/secrets/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/secrets/scrub.py
--rw-r--r--   0 vasily     (501) staff       (20)      364 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/settings.py
--rw-r--r--   0 vasily     (501) staff       (20)     2440 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/settings_store.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.966886 promptops-0.1.6/promptops/shells/
--rw-r--r--   0 vasily     (501) staff       (20)       30 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/shells/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     4861 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/shells/base.py
--rw-r--r--   0 vasily     (501) staff       (20)     1245 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/shells/bash.py
--rw-r--r--   0 vasily     (501) staff       (20)     1097 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/shells/common.py
--rw-r--r--   0 vasily     (501) staff       (20)     1946 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/shells/fish.py
--rw-r--r--   0 vasily     (501) staff       (20)     2767 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/shells/zsh.py
--rw-r--r--   0 vasily     (501) staff       (20)     2902 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/similarity.py
--rw-r--r--   0 vasily     (501) staff       (20)       42 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/trace.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.969034 promptops-0.1.6/promptops/ui/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/ui/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      138 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/ui/input.py
--rw-r--r--   0 vasily     (501) staff       (20)     3070 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/ui/prompts.py
--rw-r--r--   0 vasily     (501) staff       (20)     8990 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/ui/selections.py
--rw-r--r--   0 vasily     (501) staff       (20)      460 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/ui/vim.py
--rw-r--r--   0 vasily     (501) staff       (20)     1099 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/ui.py
--rw-r--r--   0 vasily     (501) staff       (20)     4570 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/user.py
--rw-r--r--   0 vasily     (501) staff       (20)       22 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/version.py
--rw-r--r--   0 vasily     (501) staff       (20)     1632 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/version_check.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.955040 promptops-0.1.6/promptops.egg-info/
--rw-r--r--   0 vasily     (501) staff       (20)     2255 2023-06-07 22:03:36.000000 promptops-0.1.6/promptops.egg-info/PKG-INFO
--rw-r--r--   0 vasily     (501) staff       (20)     2199 2023-06-07 22:03:36.000000 promptops-0.1.6/promptops.egg-info/SOURCES.txt
--rw-r--r--   0 vasily     (501) staff       (20)        1 2023-06-07 22:03:36.000000 promptops-0.1.6/promptops.egg-info/dependency_links.txt
--rw-r--r--   0 vasily     (501) staff       (20)      120 2023-06-07 22:03:36.000000 promptops-0.1.6/promptops.egg-info/entry_points.txt
--rw-r--r--   0 vasily     (501) staff       (20)      209 2023-06-07 22:03:36.000000 promptops-0.1.6/promptops.egg-info/requires.txt
--rw-r--r--   0 vasily     (501) staff       (20)       23 2023-06-07 22:03:36.000000 promptops-0.1.6/promptops.egg-info/top_level.txt
--rw-r--r--   0 vasily     (501) staff       (20)       87 2023-05-24 14:19:51.000000 promptops-0.1.6/pyproject.toml
--rw-r--r--   0 vasily     (501) staff       (20)       78 2023-06-07 22:03:36.970219 promptops-0.1.6/setup.cfg
--rw-r--r--   0 vasily     (501) staff       (20)     1967 2023-05-24 14:41:57.000000 promptops-0.1.6/setup.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.988314 promptops-0.1.7/
+-rw-r--r--   0 vasily     (501) staff       (20)    35149 2023-05-24 15:22:16.000000 promptops-0.1.7/LICENSE.txt
+-rw-r--r--   0 vasily     (501) staff       (20)     2841 2023-06-15 19:16:09.988503 promptops-0.1.7/PKG-INFO
+-rw-r--r--   0 vasily     (501) staff       (20)     2204 2023-06-15 19:15:23.000000 promptops-0.1.7/README.md
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.949813 promptops-0.1.7/local_runner/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/__init__.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.952491 promptops-0.1.7/local_runner/comms/
+-rw-r--r--   0 vasily     (501) staff       (20)      133 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/comms/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      432 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/comms/base.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2890 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/comms/dtos.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1536 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/comms/http_reporter.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1671 2023-06-07 21:55:02.000000 promptops-0.1.7/local_runner/comms/ws.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.953475 promptops-0.1.7/local_runner/config/
+-rw-r--r--   0 vasily     (501) staff       (20)       48 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/config/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1720 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/config/config.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.954411 promptops-0.1.7/local_runner/creds/
+-rw-r--r--   0 vasily     (501) staff       (20)       77 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/creds/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1458 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/creds/creds.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.955319 promptops-0.1.7/local_runner/exec/
+-rw-r--r--   0 vasily     (501) staff       (20)       54 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/exec/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2317 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/exec/manager.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.956605 promptops-0.1.7/local_runner/handler/
+-rw-r--r--   0 vasily     (501) staff       (20)       29 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/handler/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      471 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/handler/censor.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3115 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/handler/handler.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1361 2023-06-07 21:55:02.000000 promptops-0.1.7/local_runner/main.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.957591 promptops-0.1.7/local_runner/registration/
+-rw-r--r--   0 vasily     (501) staff       (20)       56 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/registration/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2523 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/registration/registration.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.958502 promptops-0.1.7/local_runner/tokens/
+-rw-r--r--   0 vasily     (501) staff       (20)       27 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/tokens/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2235 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/tokens/issuer.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.965985 promptops-0.1.7/promptops/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1850 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/corrections.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1033 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/feedback.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.969292 promptops-0.1.7/promptops/gitaware/
+-rw-r--r--   0 vasily     (501) staff       (20)       42 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/gitaware/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      658 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/gitaware/project.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4146 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/history.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.971118 promptops-0.1.7/promptops/index/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/index/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2692 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/index/content.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2084 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/index/entry_point.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4399 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/index/index_store.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.975540 promptops-0.1.7/promptops/loading/
+-rw-r--r--   0 vasily     (501) staff       (20)      131 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/loading/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      677 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/loading/base.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1139 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/loading/cancellable.py
+-rw-r--r--   0 vasily     (501) staff       (20)      481 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/loading/context.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1554 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/loading/multi.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1279 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/loading/pong.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1344 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/loading/progress.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1077 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/loading/promptops.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1025 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/loading/simple.py
+-rw-r--r--   0 vasily     (501) staff       (20)     9999 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/main.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.979297 promptops-0.1.7/promptops/query/
+-rw-r--r--   0 vasily     (501) staff       (20)       30 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/query/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      434 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/query/dtos.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4351 2023-05-25 18:38:08.000000 promptops-0.1.7/promptops/query/explanation.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4506 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/query/git_repo.py
+-rw-r--r--   0 vasily     (501) staff       (20)     9075 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/query/lookup.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1222 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/query/messages.py
+-rw-r--r--   0 vasily     (501) staff       (20)    19626 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/query/query.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1126 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/query.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.980926 promptops-0.1.7/promptops/recipes/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/recipes/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)    12414 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/recipes/creation.py
+-rw-r--r--   0 vasily     (501) staff       (20)      998 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/recipes/run.py
+-rw-r--r--   0 vasily     (501) staff       (20)     6555 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/recipes/terraform.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.981801 promptops-0.1.7/promptops/scrub_secrets/
+-rw-r--r--   0 vasily     (501) staff       (20)       55 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/scrub_secrets/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/scrub_secrets/scrub.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.982798 promptops-0.1.7/promptops/secrets/
+-rw-r--r--   0 vasily     (501) staff       (20)       55 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/secrets/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/secrets/scrub.py
+-rw-r--r--   0 vasily     (501) staff       (20)      364 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/settings.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2440 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/settings_store.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.985464 promptops-0.1.7/promptops/shells/
+-rw-r--r--   0 vasily     (501) staff       (20)       46 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/shells/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4861 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/shells/base.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1245 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/shells/bash.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1154 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/shells/common.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1946 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/shells/fish.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2767 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/shells/zsh.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3206 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/similarity.py
+-rw-r--r--   0 vasily     (501) staff       (20)       42 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/trace.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.987900 promptops-0.1.7/promptops/ui/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/ui/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      138 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/ui/input.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3070 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/ui/prompts.py
+-rw-r--r--   0 vasily     (501) staff       (20)     8990 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/ui/selections.py
+-rw-r--r--   0 vasily     (501) staff       (20)      460 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/ui/vim.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1099 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/ui.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4570 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/user.py
+-rw-r--r--   0 vasily     (501) staff       (20)       22 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/version.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1632 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/version_check.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.968311 promptops-0.1.7/promptops.egg-info/
+-rw-r--r--   0 vasily     (501) staff       (20)     2841 2023-06-15 19:16:09.000000 promptops-0.1.7/promptops.egg-info/PKG-INFO
+-rw-r--r--   0 vasily     (501) staff       (20)     2310 2023-06-15 19:16:09.000000 promptops-0.1.7/promptops.egg-info/SOURCES.txt
+-rw-r--r--   0 vasily     (501) staff       (20)        1 2023-06-15 19:16:09.000000 promptops-0.1.7/promptops.egg-info/dependency_links.txt
+-rw-r--r--   0 vasily     (501) staff       (20)      120 2023-06-15 19:16:09.000000 promptops-0.1.7/promptops.egg-info/entry_points.txt
+-rw-r--r--   0 vasily     (501) staff       (20)      225 2023-06-15 19:16:09.000000 promptops-0.1.7/promptops.egg-info/requires.txt
+-rw-r--r--   0 vasily     (501) staff       (20)       23 2023-06-15 19:16:09.000000 promptops-0.1.7/promptops.egg-info/top_level.txt
+-rw-r--r--   0 vasily     (501) staff       (20)       87 2023-05-24 14:19:51.000000 promptops-0.1.7/pyproject.toml
+-rw-r--r--   0 vasily     (501) staff       (20)       78 2023-06-15 19:16:09.989123 promptops-0.1.7/setup.cfg
+-rw-r--r--   0 vasily     (501) staff       (20)     1994 2023-06-15 19:15:23.000000 promptops-0.1.7/setup.py
```

### Comparing `promptops-0.1.6/LICENSE.txt` & `promptops-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/PKG-INFO` & `promptops-0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptops
-Version: 0.1.6
+Version: 0.1.7
 Summary: Your CLI assistant. Ask questions, get shell commands.
 Home-page: https://promptops.com/
 Author: CtrlStack inc.
 License: GPLv3
 Project-URL: Documentation, https://docs.promptops.com/cli
 Project-URL: Changelog, https://docs.promptops.com/en/stable/changelog.html
 Project-URL: Live demo, https://promptops.com/
@@ -20,16 +20,17 @@
 <img src="https://github.com/promptops/cli/raw/main/media/default.png" />
 
 # Features
 
 - find the right command without leaving the terminal
 - `um` can index your history to find commands you've run before
 - `um` instantly learns from your corrections
-- `um workflow` can help you provision infrastructure
 - simple interface to clarify your question or provide more context
+- NEW in 0.1.6: `um workflow` helps you provision infrastructure (currently terraform only, more coming soon)
+- NEW in 0.1.7: extended reverse search functionality with fuzzy matching and semantic search
 
 # Installation
 
 ## Linux - Ubuntu
 ```shell
 curl -fsSL -o ubuntu-installer.sh https://raw.githubusercontent.com/promptops/cli/main/ubuntu-installer.sh
 chmod 700 ubuntu-installer.sh
@@ -47,24 +48,46 @@
 Make sure you have python 3.10 or more recent
 [python.org downloads](https://www.python.org/downloads/)
 
 ```shell
 pip3 install promptops
 ```
 
+# Configuration
+
+## Enable extended reverse search (Ctrl+E)
+
+Note: currently works only with Zsh
+
+Add the widget and the key binding to your `.zshrc` file
+```shell
+cp ~/.zshrc ~/.zshrc.backup
+echo 'eval "$(promptops lookup --config)"' >> ~/.zshrc
+```
+
+Reload
+```shell
+source ~/.zshrc
+```
+
+## Disable extended reverse search
+
+Remove the eval line from your `.zshrc` file and reload.
+
+
 # Usage
 
 ## um
 
 ```shell
 um <question>
 ```
 
 ```shell
-um workflow <multi-stepped-prompt>
+um recipe <multi-stepped-prompt>
 ```
 
 ## local runner
 
 ```shell
 promptops runner
 ```
@@ -108,7 +131,13 @@
 ```
 
 test with
 
 ```shell
 um get pods
 ```
+
+## Publishing pip release
+
+```shell
+make publish
+```
```

### Comparing `promptops-0.1.6/README.md` & `promptops-0.1.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 <img src="https://github.com/promptops/cli/raw/main/media/default.png" />
 
 # Features
 
 - find the right command without leaving the terminal
 - `um` can index your history to find commands you've run before
 - `um` instantly learns from your corrections
-- `um workflow` can help you provision infrastructure
 - simple interface to clarify your question or provide more context
+- NEW in 0.1.6: `um workflow` helps you provision infrastructure (currently terraform only, more coming soon)
+- NEW in 0.1.7: extended reverse search functionality with fuzzy matching and semantic search
 
 # Installation
 
 ## Linux - Ubuntu
 ```shell
 curl -fsSL -o ubuntu-installer.sh https://raw.githubusercontent.com/promptops/cli/main/ubuntu-installer.sh
 chmod 700 ubuntu-installer.sh
@@ -30,24 +31,46 @@
 Make sure you have python 3.10 or more recent
 [python.org downloads](https://www.python.org/downloads/)
 
 ```shell
 pip3 install promptops
 ```
 
+# Configuration
+
+## Enable extended reverse search (Ctrl+E)
+
+Note: currently works only with Zsh
+
+Add the widget and the key binding to your `.zshrc` file
+```shell
+cp ~/.zshrc ~/.zshrc.backup
+echo 'eval "$(promptops lookup --config)"' >> ~/.zshrc
+```
+
+Reload
+```shell
+source ~/.zshrc
+```
+
+## Disable extended reverse search
+
+Remove the eval line from your `.zshrc` file and reload.
+
+
 # Usage
 
 ## um
 
 ```shell
 um <question>
 ```
 
 ```shell
-um workflow <multi-stepped-prompt>
+um recipe <multi-stepped-prompt>
 ```
 
 ## local runner
 
 ```shell
 promptops runner
 ```
@@ -91,7 +114,13 @@
 ```
 
 test with
 
 ```shell
 um get pods
 ```
+
+## Publishing pip release
+
+```shell
+make publish
+```
```

### Comparing `promptops-0.1.6/local_runner/comms/dtos.py` & `promptops-0.1.7/local_runner/comms/dtos.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/local_runner/comms/http_reporter.py` & `promptops-0.1.7/local_runner/comms/http_reporter.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/local_runner/comms/ws.py` & `promptops-0.1.7/local_runner/comms/ws.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/local_runner/config/config.py` & `promptops-0.1.7/local_runner/config/config.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/local_runner/creds/creds.py` & `promptops-0.1.7/local_runner/creds/creds.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/local_runner/exec/manager.py` & `promptops-0.1.7/local_runner/exec/manager.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/local_runner/handler/handler.py` & `promptops-0.1.7/local_runner/handler/handler.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/local_runner/main.py` & `promptops-0.1.7/local_runner/main.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/local_runner/registration/registration.py` & `promptops-0.1.7/local_runner/registration/registration.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/local_runner/tokens/issuer.py` & `promptops-0.1.7/local_runner/tokens/issuer.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/corrections.py` & `promptops-0.1.7/promptops/corrections.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/feedback.py` & `promptops-0.1.7/promptops/feedback.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/gitaware/project.py` & `promptops-0.1.7/promptops/gitaware/project.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import subprocess
 import logging
 
 
 def git_root():
     try:
-        return subprocess.check_output(["git", "rev-parse", "--show-toplevel"]).decode("utf-8").strip()
+        return subprocess.check_output(["git", "rev-parse", "--show-toplevel"], stderr=subprocess.STDOUT).decode("utf-8").strip()
     except subprocess.CalledProcessError as e:
         logging.debug("return code: %d", e.returncode)
         return None
 
 
 def is_ignored(path):
     try:
```

### Comparing `promptops-0.1.6/promptops/history.py` & `promptops-0.1.7/promptops/history.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/index/content.py` & `promptops-0.1.7/promptops/index/content.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/index/entry_point.py` & `promptops-0.1.7/promptops/index/entry_point.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/index/index_store.py` & `promptops-0.1.7/promptops/index/index_store.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/loading/base.py` & `promptops-0.1.7/promptops/loading/base.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/loading/pong.py` & `promptops-0.1.7/promptops/loading/pong.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/loading/progress.py` & `promptops-0.1.7/promptops/loading/progress.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/loading/promptops.py` & `promptops-0.1.7/promptops/loading/promptops.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/loading/simple.py` & `promptops-0.1.7/promptops/loading/simple.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/main.py` & `promptops-0.1.7/promptops/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,36 +21,53 @@
 import traceback
 
 import logging
 
 from promptops import settings
 from promptops import settings_store
 from promptops import version_check
-from promptops import query
 from promptops import user
-from promptops.recipes.creation import workflow_entrypoint
+from promptops.recipes.creation import recipe_entrypoint
 from promptops.index.entry_point import entry_point as index_entry_point
+from promptops.query.lookup import entry_point as lookup_entry_point
 
 ENDPOINT_ENV = "PROMPTOPS_ENDPOINT"
 
 
 def runner_mode(args):
     from promptops.feedback import feedback
-
-    feedback(
-        {
-            "event": "runner_mode",
-        }
-    )
-
     from local_runner.main import entry_point
 
+    feedback({"event": "runner_mode"})
     entry_point()
 
 
+def query_mode(args):
+    from promptops import query
+    query.query_mode(args)
+
+
+def lookup_mode(args):
+    from promptops.feedback import feedback
+    from promptops.query.lookup import entry_point as lookup_entry_point
+
+    feedback({"event": "lookup_mode"})
+    lookup_entry_point(args)
+
+
+def recipe_mode(args):
+    from promptops.recipes.creation import recipe_entrypoint
+    recipe_entrypoint(args)
+
+
+def index_mode(args):
+    from promptops.index.entry_point import entry_point as index_entry_point
+    index_entry_point(args)
+
+
 def handle_exception(prev_handler):
     def inner(exc_type, exc_value, exc_traceback):
         sys.stderr.flush()
         if prev_handler:
             prev_handler(exc_type, exc_value, exc_traceback)
         error_message = traceback.format_exception(exc_type, exc_value, exc_traceback)
         from promptops.feedback import feedback
@@ -131,29 +148,29 @@
         args.history_context = settings.history_context
     else:
         from promptops import history
 
         history.update_history()
 
     if args.question and len(args.question) > 0:
-        if args.question[0] == 'workflow':
-            return workflow_entrypoint(args)
+        if args.question[0] == 'workflow' or args.question[0] == 'recipe':
+            return recipe_mode(args)
         elif args.question[0] == 'index':
             # index subcommand
             subparser = ArgumentParser(
                 prog=f"{alias} index",
                 usage=f"{alias} index [action]",
                 description=f"{alias} index: manage the indexed data",
             )
             subparser.add_argument("action", choices=["list", "add", "remove", "test"], help="list or update the index")
             subparser.add_argument("--source", help="the source to add or remove")
             subparser.add_argument("--query", help="query to test with")
             sub_args = subparser.parse_args(args.question[1:])
-            return index_entry_point(sub_args)
-    query.query_mode(args)
+            return index_mode(sub_args)
+    query_mode(args)
 
 
 def entry_main():
     # Set the global exception handler
     sys.excepthook = handle_exception(sys.excepthook)
 
     import colorama
@@ -189,28 +206,38 @@
         default=settings.request_explanation,
         help="get faster response",
     )
     parser_question.add_argument(
         "--mode", default=settings.model, choices=["fast", "accurate"], help="fast or accurate (default: %(default)s)"
     )
     parser_question.add_argument("question", nargs=REMAINDER, help="the question to ask")
-    parser_question.set_defaults(func=query.query_mode)
+    parser_question.set_defaults(func=query_mode)
 
     parser_runner = subparsers.add_parser("runner", help="run commands from slack")
     parser_runner.set_defaults(func=runner_mode)
 
-    parser_workflow = subparsers.add_parser("workflow", help="run a complex or multi-stepped script")
+    parser_workflow = subparsers.add_parser("recipe", help="run a complex or multi-stepped script")
     parser_workflow.add_argument("question", nargs=REMAINDER, help="the question to generate scripts for")
-    parser_workflow.set_defaults(func=workflow_entrypoint)
+    parser_workflow.set_defaults(func=recipe_mode)
 
     parser_index = subparsers.add_parser("index", help="manage the indexed data")
     parser_index.add_argument("action", choices=["list", "add", "remove", "test"], help="list or update the index")
     parser_index.add_argument("--source", help="the source to add or remove")
     parser_index.add_argument("--query", help="query to test with")
-    parser_index.set_defaults(func=index_entry_point)
+    parser_index.set_defaults(func=index_mode)
+
+    parser_lookup = subparsers.add_parser("lookup", help="extended reverse search, use --config to configure in your shell")
+    parser_lookup.add_argument("--config", action="store_true", help="print configuration for your shell")
+    parser_lookup.add_argument("command", nargs=REMAINDER, help="the command to lookup")
+    parser_lookup.set_defaults(func=lookup_mode)
+
+    parser_lookup = subparsers.add_parser("lookup", help="extended reverse search, use --config to configure in your shell")
+    parser_lookup.add_argument("--config", help="print configuration for your shell")
+    parser_lookup.add_argument("command", nargs=REMAINDER, help="the command to lookup")
+    parser_lookup.set_defaults(func=lookup_entry_point)
 
     args = parser.parse_args()
 
     registered = user.has_registered()
 
     if not hasattr(args, "func"):
         if args.version:
@@ -231,14 +258,21 @@
         return
 
     if args.verbose:
         logging.basicConfig(level=logging.DEBUG)
     else:
         logging.basicConfig(level=logging.INFO, format="%(message)s")
 
+    if getattr(args, "func") == lookup_mode:
+        if not args.verbose:
+            logging.basicConfig(level=logging.ERROR, format="%(message)s", force=True)
+        # shortcut for lookup
+        args.func(args)
+        return
+
     version_check.version_check()
     if not registered:
         user.register()
         args.history_context = settings.history_context
     else:
         from promptops import history
```

### Comparing `promptops-0.1.6/promptops/query/explanation.py` & `promptops-0.1.7/promptops/query/explanation.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/query/git_repo.py` & `promptops-0.1.7/promptops/query/git_repo.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/query/messages.py` & `promptops-0.1.7/promptops/query/messages.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/query/query.py` & `promptops-0.1.7/promptops/query/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import json
 import logging
 import os
 import sys
 from dataclasses import dataclass
 from copy import copy
 import subprocess
 import threading
 import random
 from typing import Optional
 
+import colorama
 import requests
 from prompt_toolkit import print_formatted_text
 from prompt_toolkit.patch_stdout import patch_stdout
 from prompt_toolkit.formatted_text import HTML, to_formatted_text
 import prompt_toolkit
 
 from promptops import settings
@@ -104,16 +106,23 @@
 def make_revise_option():
     return "\x1b[3m💭️ don't see what you're looking for? try providing more context\x1b[0m"
 
 
 ORIGIN_SYMBOLS = {"history": "📖", "promptops": "✨"}
 
 
+def ellipsis_if_needed(text, max_width, more="..."):
+    if len(text) <= max_width:
+        return text
+    return text[:max_width - len(more)] + more
+
+
 def pretty_result(result: Result):
-    return (ORIGIN_SYMBOLS.get(result.origin, f"[{result.origin[0]}]") + " " if result.origin else "") + result.script
+    text = result.script if result.lang != "text" else colorama.Fore.YELLOW + ellipsis_if_needed(result.script, 120, "...") + colorama.Style.RESET_ALL
+    return (ORIGIN_SYMBOLS.get(result.origin, f"[{result.origin[0]}]") + " " if result.origin else "") + text
 
 
 @dataclass
 class ConfirmResult:
     result: Result = None
     confirmed: str = ""
     question: str = None
@@ -247,15 +256,25 @@
             if selected == prompts.GO_BACK:
                 continue
             elif selected == prompts.EXIT:
                 raise KeyboardInterrupt()
             return ConfirmResult(question=selected, options=[r.script for r in results if r.origin == "promptops"])
         else:
             selected = results[index]
-            if selected.explanation:
+            if selected.lang == "text":
+                print_formatted_text(selected.script)
+                print()
+                selected = prompts.confirm_clarify("")
+                if selected == prompts.GO_BACK:
+                    continue
+                elif selected == prompts.EXIT:
+                    raise KeyboardInterrupt()
+                return ConfirmResult(question=selected,
+                                     options=[r.script for r in results if r.origin == "promptops"])
+            elif selected.explanation:
                 print_formatted_text(HTML(selected.explanation))
                 print()
                 confirmed = prompts.confirm_command(selected.script, False)
             elif selected.origin == "promptops" and settings.request_explanation:
 
                 done_loading = threading.Event()
 
@@ -397,40 +416,44 @@
 
     try:
         cmd, confirmed = input_loop()
     except KeyboardInterrupt:
         feedback({"event": "cancelled"})
         sys.exit(1)
 
-    if (cmd.script != confirmed or len(questions) > 1) and confirmed:
+    if cmd.lang == "text":
+        return
+
+    if confirmed:
         # the user corrected the script
         db = corrections.get_db()
         q = "\n".join(questions)
         vector = similarity.embedding(text=q)
-        db.add(vector, corrections.QATuple(question=q, answer=cmd.script, corrected=confirmed).to_dict())
+        db.update_or_add(vector, corrections.QATuple(question=q, answer=cmd.script, corrected=confirmed).to_dict(), equals=lambda a, b: a["question"] == b["question"])
         logging.debug("added correction to db")
         db.save(os.path.expanduser(settings.corrections_db_path))
         feedback({"event": "corrected"})
 
     feedback({"event": "run"})
     revised_cmd = copy(cmd)
     revised_cmd.script = confirmed
     rc, stderr = run(revised_cmd)
     feedback({"event": "finished", "rc": rc})
 
     while rc != 0:
         corrected_cmd = correction_loop("\n".join(questions), revised_cmd.script, stderr)
         if not corrected_cmd:
             return
+        feedback({"event": "run"})
         rc, stderr = run(corrected_cmd)
         if rc == 0:
             db = corrections.get_db()
             q = "\n".join(questions)
             vector = similarity.embedding(text=q)
-            db.add(vector, corrections.QATuple(question=q, answer=cmd.script, corrected=corrected_cmd.script).to_dict())
+            db.update_or_add(vector, corrections.QATuple(question=q, answer=cmd.script, corrected=corrected_cmd.script).to_dict(), equals=lambda a, b: a["question"] == b["question"])
             logging.debug("added correction to db")
             db.save(os.path.expanduser(settings.corrections_db_path))
         feedback({"event": "finished", "rc": rc, "corrected": True})
 
 
 def query_mode(args):
     if args.verbose:
@@ -500,9 +523,16 @@
         return []
         # raise Exception(f"there was problem with the response, status: {response.status_code}, text: {response.text}")
 
     data = response.json()
     try:
         return [Result.from_dict(entry) for entry in data["suggestions"]]
     except KeyError:
-        logging.debug("response: %s", data)
-        raise
+        logging.debug("no suggestions in response: %s", json.dumps(data, indent=2))
+
+    try:
+        message = data.get("message")
+    except KeyError:
+        message = "-"
+        logging.debug("no message in response: %s", json.dumps(data, indent=2))
+
+    return [Result(script=message, lang="text", explanation="-")]
```

### Comparing `promptops-0.1.6/promptops/query.py` & `promptops-0.1.7/promptops/query.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/scrub_secrets/scrub.py` & `promptops-0.1.7/promptops/scrub_secrets/scrub.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/secrets/scrub.py` & `promptops-0.1.7/promptops/secrets/scrub.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/settings_store.py` & `promptops-0.1.7/promptops/settings_store.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/shells/base.py` & `promptops-0.1.7/promptops/shells/base.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/shells/bash.py` & `promptops-0.1.7/promptops/shells/bash.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/shells/common.py` & `promptops-0.1.7/promptops/shells/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 _shells = {
     "zsh": Zsh,
     "bash": Bash,
     "fish": Fish,
 }
 
 
-def _resolve_shell():
+def get_shell_name():
     proc = psutil.Process(os.getpid())
 
     path = []
     while proc is not None and proc.pid > 0:
         try:
             name = proc.name()
         except TypeError:
             name = proc.name
 
         name = os.path.splitext(name)[0]
         path = [name] + path
 
         if name in _shells:
             logging.debug(f"found shell: {'/'.join(path)}")
-            return _shells[name]()
+            return name
 
         try:
             proc = proc.parent()
         except TypeError:
             proc = proc.parent
 
     from promptops.feedback import feedback
@@ -41,13 +41,15 @@
     feedback(
         {
             "event": "shell_not_found",
             "path": "/".join(path),
         }
     )
     logging.debug(f"shell not supported: {'/'.join(path)}")
-    return NoopShell()
+    return None
 
 
 def get_shell():
-    shell = _resolve_shell()
-    return shell
+    shell_name = get_shell_name()
+    if shell_name is None:
+        return NoopShell()
+    return _shells[shell_name]()
```

### Comparing `promptops-0.1.6/promptops/shells/fish.py` & `promptops-0.1.7/promptops/shells/fish.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/shells/zsh.py` & `promptops-0.1.7/promptops/shells/zsh.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/similarity.py` & `promptops-0.1.7/promptops/similarity.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,23 @@
     def add(self, vector, obj):
         if len(self.vectors) == 0:
             self.vectors = np.expand_dims(vector, axis=0)
         else:
             self.vectors = np.vstack((self.vectors, vector))
         self.objects.append(obj)
 
+    def update_or_add(self, vector, obj, equals: callable=None):
+        if equals is None:
+            equals = lambda a, b: a == b
+        for i, o in enumerate(self.objects):
+            if equals(o, obj):
+                self.vectors[i] = vector
+                return
+        self.add(vector, obj)
+
     def search(self, vector, k=1, min_similarity=0.8):
         # compute cosine similarity
         if len(self.vectors) == 0:
             return []
         scores = np.dot(vector, self.vectors.T).flatten()
         # rank results
         results = np.argsort(scores)[::-1]
```

### Comparing `promptops-0.1.6/promptops/ui/prompts.py` & `promptops-0.1.7/promptops/ui/prompts.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/ui/selections.py` & `promptops-0.1.7/promptops/ui/selections.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/ui.py` & `promptops-0.1.7/promptops/ui.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/user.py` & `promptops-0.1.7/promptops/user.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops/version_check.py` & `promptops-0.1.7/promptops/version_check.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.6/promptops.egg-info/PKG-INFO` & `promptops-0.1.7/promptops.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptops
-Version: 0.1.6
+Version: 0.1.7
 Summary: Your CLI assistant. Ask questions, get shell commands.
 Home-page: https://promptops.com/
 Author: CtrlStack inc.
 License: GPLv3
 Project-URL: Documentation, https://docs.promptops.com/cli
 Project-URL: Changelog, https://docs.promptops.com/en/stable/changelog.html
 Project-URL: Live demo, https://promptops.com/
@@ -20,16 +20,17 @@
 <img src="https://github.com/promptops/cli/raw/main/media/default.png" />
 
 # Features
 
 - find the right command without leaving the terminal
 - `um` can index your history to find commands you've run before
 - `um` instantly learns from your corrections
-- `um workflow` can help you provision infrastructure
 - simple interface to clarify your question or provide more context
+- NEW in 0.1.6: `um workflow` helps you provision infrastructure (currently terraform only, more coming soon)
+- NEW in 0.1.7: extended reverse search functionality with fuzzy matching and semantic search
 
 # Installation
 
 ## Linux - Ubuntu
 ```shell
 curl -fsSL -o ubuntu-installer.sh https://raw.githubusercontent.com/promptops/cli/main/ubuntu-installer.sh
 chmod 700 ubuntu-installer.sh
@@ -47,24 +48,46 @@
 Make sure you have python 3.10 or more recent
 [python.org downloads](https://www.python.org/downloads/)
 
 ```shell
 pip3 install promptops
 ```
 
+# Configuration
+
+## Enable extended reverse search (Ctrl+E)
+
+Note: currently works only with Zsh
+
+Add the widget and the key binding to your `.zshrc` file
+```shell
+cp ~/.zshrc ~/.zshrc.backup
+echo 'eval "$(promptops lookup --config)"' >> ~/.zshrc
+```
+
+Reload
+```shell
+source ~/.zshrc
+```
+
+## Disable extended reverse search
+
+Remove the eval line from your `.zshrc` file and reload.
+
+
 # Usage
 
 ## um
 
 ```shell
 um <question>
 ```
 
 ```shell
-um workflow <multi-stepped-prompt>
+um recipe <multi-stepped-prompt>
 ```
 
 ## local runner
 
 ```shell
 promptops runner
 ```
@@ -108,7 +131,13 @@
 ```
 
 test with
 
 ```shell
 um get pods
 ```
+
+## Publishing pip release
+
+```shell
+make publish
+```
```

### Comparing `promptops-0.1.6/promptops.egg-info/SOURCES.txt` & `promptops-0.1.7/promptops.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -47,27 +47,31 @@
 promptops/gitaware/project.py
 promptops/index/__init__.py
 promptops/index/content.py
 promptops/index/entry_point.py
 promptops/index/index_store.py
 promptops/loading/__init__.py
 promptops/loading/base.py
+promptops/loading/cancellable.py
 promptops/loading/context.py
+promptops/loading/multi.py
 promptops/loading/pong.py
 promptops/loading/progress.py
 promptops/loading/promptops.py
 promptops/loading/simple.py
 promptops/query/__init__.py
 promptops/query/dtos.py
 promptops/query/explanation.py
 promptops/query/git_repo.py
+promptops/query/lookup.py
 promptops/query/messages.py
 promptops/query/query.py
 promptops/recipes/__init__.py
 promptops/recipes/creation.py
+promptops/recipes/run.py
 promptops/recipes/terraform.py
 promptops/scrub_secrets/__init__.py
 promptops/scrub_secrets/scrub.py
 promptops/secrets/__init__.py
 promptops/secrets/scrub.py
 promptops/shells/__init__.py
 promptops/shells/base.py
```

### Comparing `promptops-0.1.6/setup.py` & `promptops-0.1.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         "requests~=2.29.0",
         "websockets~=11.0.2",
         "detect-secrets~=1.4.0",
         "prompt-toolkit~=3.0.38",
         "numpy~=1.24.3",
         "pyperclip~=1.8.2",
         "psutil~=5.9.5",
+        "thefuzz~=0.19.0",
         "boto3~=1.26.131",
         "kubernetes~=26.1.0",
         "setuptools",
         "pip",
     ],
     entry_points="""
         [console_scripts]
```

