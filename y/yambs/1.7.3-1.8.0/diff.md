# Comparing `tmp/yambs-1.7.3.tar.gz` & `tmp/yambs-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-1.7.3.tar", last modified: Mon May 29 08:21:15 2023, max compression
+gzip compressed data, was "yambs-1.8.0.tar", last modified: Thu Jun 15 06:08:37 2023, max compression
```

## Comparing `yambs-1.7.3.tar` & `yambs-1.8.0.tar`

### file list

```diff
@@ -1,72 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.289452 yambs-1.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-29 08:19:59.000000 yambs-1.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-29 08:21:15.289452 yambs-1.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-05-29 08:19:59.000000 yambs-1.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-29 08:19:59.000000 yambs-1.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 08:21:15.289452 yambs-1.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-29 08:19:59.000000 yambs-1.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.281452 yambs-1.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-29 08:19:59.000000 yambs-1.7.3/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-29 08:19:59.000000 yambs-1.7.3/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.285452 yambs-1.7.3/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.285452 yambs-1.7.3/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/commands/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/commands/uf2conv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.285452 yambs-1.7.3/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/config/board.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.285452 yambs-1.7.3/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.285452 yambs-1.7.3/yambs/data/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/includes/chips.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/includes/infineon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/includes/microchip.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.285452 yambs-1.7.3/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/schemas/Architecture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/schemas/Toolchain.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.285452 yambs-1.7.3/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/templates/architecture.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/uf2families.json
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/yambs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.289452 yambs-1.7.3/yambs/environment/
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.289452 yambs-1.7.3/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/generate/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/generate/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.289452 yambs-1.7.3/yambs/generate/ninja/
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/generate/ninja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/generate/ninja/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.289452 yambs-1.7.3/yambs/translation/
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.289452 yambs-1.7.3/yambs/uf2/
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/uf2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.285452 yambs-1.7.3/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-29 08:21:15.000000 yambs-1.7.3/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-29 08:21:15.000000 yambs-1.7.3/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 08:21:15.000000 yambs-1.7.3/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-29 08:21:15.000000 yambs-1.7.3/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-29 08:21:15.000000 yambs-1.7.3/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 08:21:15.000000 yambs-1.7.3/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.597098 yambs-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-15 06:07:15.000000 yambs-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-06-15 06:08:37.597098 yambs-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-06-15 06:07:15.000000 yambs-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-15 06:07:15.000000 yambs-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 06:08:37.597098 yambs-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-15 06:07:15.000000 yambs-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.585098 yambs-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-15 06:07:15.000000 yambs-1.8.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-15 06:07:15.000000 yambs-1.8.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.585098 yambs-1.8.0/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.585098 yambs-1.8.0/yambs/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.585098 yambs-1.8.0/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/commands/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/commands/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/commands/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.585098 yambs-1.8.0/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/config/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/config/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/config/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.589098 yambs-1.8.0/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.589098 yambs-1.8.0/yambs/data/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/includes/chips.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/includes/infineon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/includes/microchip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/native.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.589098 yambs-1.8.0/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/schemas/Native.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/schemas/Toolchain.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/schemas/Variant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/schemas/config_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/schemas/targets_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/schemas/toolchain_common.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.589098 yambs-1.8.0/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/compile_commands.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/native_all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/native_build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/native_rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/variant.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/yambs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.589098 yambs-1.8.0/yambs/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/environment/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.597098 yambs-1.8.0/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/generate/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.597098 yambs-1.8.0/yambs/generate/ninja/
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/generate/ninja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/generate/ninja/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/generate/variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.597098 yambs-1.8.0/yambs/translation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.597098 yambs-1.8.0/yambs/uf2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/uf2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.585098 yambs-1.8.0/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-06-15 06:08:37.000000 yambs-1.8.0/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-15 06:08:37.000000 yambs-1.8.0/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:08:37.000000 yambs-1.8.0/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 06:08:37.000000 yambs-1.8.0/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-15 06:08:37.000000 yambs-1.8.0/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 06:08:37.000000 yambs-1.8.0/yambs.egg-info/top_level.txt
```

### Comparing `yambs-1.7.3/LICENSE` & `yambs-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-1.7.3/PKG-INFO` & `yambs-1.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.7.3
+Version: 1.8.0
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=bb422a51478a96037d8ddd3a3e4597a7
+    hash=c88caeb9c6d71c51d9fd724250cd248c
     =====================================
 -->
 
-# yambs ([1.7.3](https://pypi.org/project/yambs/))
+# yambs ([1.8.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
 
@@ -150,29 +150,31 @@
 following a specific convention), put your configuration data here.
 
 # Command-line Options
 
 ```
 $ ./venv3.11/bin/mbs -h
 
-usage: mbs [-h] [--version] [-v] [-C DIR] {gen,uf2conv,noop} ...
+usage: mbs [-h] [--version] [-v] [-C DIR] {gen,native,uf2conv,noop} ...
 
 Yet another meta build-system.
 
 options:
-  -h, --help          show this help message and exit
-  --version           show program's version number and exit
-  -v, --verbose       set to increase logging verbosity
-  -C DIR, --dir DIR   execute from a specific directory
+  -h, --help            show this help message and exit
+  --version             show program's version number and exit
+  -v, --verbose         set to increase logging verbosity
+  -C DIR, --dir DIR     execute from a specific directory
 
 commands:
-  {gen,uf2conv,noop}  set of available commands
-    gen               poll the source tree and generate any new build files
-    uf2conv           Convert to UF2 or flash directly.
-    noop              command stub (does nothing)
+  {gen,native,uf2conv,noop}
+                        set of available commands
+    gen                 poll the source tree and generate any new build files
+    native              generate build files for native-only target projects
+    uf2conv             Convert to UF2 or flash directly.
+    noop                command stub (does nothing)
 
 ```
 
 ## Sub-command Options
 
 ### `gen`
 
@@ -183,14 +185,36 @@
 
 options:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         the path to the top-level configuration file (default:
                         'yambs.yaml')
   -i, --single-pass     only run a single watch iteration
+  -w, --watch           whether or not to continue watching for source tree
+                        changes
+
+```
+
+### `native`
+
+```
+$ ./venv3.11/bin/mbs native -h
+
+usage: mbs native [-h] [-c CONFIG] [-i] [-w] [variants ...]
+
+positional arguments:
+  variants              variants to build (defaults to 'debug' if not
+                        specified)
+
+options:
+  -h, --help            show this help message and exit
+  -c CONFIG, --config CONFIG
+                        the path to the top-level configuration file (default:
+                        'yambs.yaml')
+  -i, --single-pass     only run a single watch iteration
   -w, --watch           whether or not to continue watching for source tree
                         changes
 
 ```
 
 ### `uf2conv`
```

### Comparing `yambs-1.7.3/README.md` & `yambs-1.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=bb422a51478a96037d8ddd3a3e4597a7
+    hash=c88caeb9c6d71c51d9fd724250cd248c
     =====================================
 -->
 
-# yambs ([1.7.3](https://pypi.org/project/yambs/))
+# yambs ([1.8.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
 
@@ -126,29 +126,31 @@
 following a specific convention), put your configuration data here.
 
 # Command-line Options
 
 ```
 $ ./venv3.11/bin/mbs -h
 
-usage: mbs [-h] [--version] [-v] [-C DIR] {gen,uf2conv,noop} ...
+usage: mbs [-h] [--version] [-v] [-C DIR] {gen,native,uf2conv,noop} ...
 
 Yet another meta build-system.
 
 options:
-  -h, --help          show this help message and exit
-  --version           show program's version number and exit
-  -v, --verbose       set to increase logging verbosity
-  -C DIR, --dir DIR   execute from a specific directory
+  -h, --help            show this help message and exit
+  --version             show program's version number and exit
+  -v, --verbose         set to increase logging verbosity
+  -C DIR, --dir DIR     execute from a specific directory
 
 commands:
-  {gen,uf2conv,noop}  set of available commands
-    gen               poll the source tree and generate any new build files
-    uf2conv           Convert to UF2 or flash directly.
-    noop              command stub (does nothing)
+  {gen,native,uf2conv,noop}
+                        set of available commands
+    gen                 poll the source tree and generate any new build files
+    native              generate build files for native-only target projects
+    uf2conv             Convert to UF2 or flash directly.
+    noop                command stub (does nothing)
 
 ```
 
 ## Sub-command Options
 
 ### `gen`
 
@@ -159,14 +161,36 @@
 
 options:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         the path to the top-level configuration file (default:
                         'yambs.yaml')
   -i, --single-pass     only run a single watch iteration
+  -w, --watch           whether or not to continue watching for source tree
+                        changes
+
+```
+
+### `native`
+
+```
+$ ./venv3.11/bin/mbs native -h
+
+usage: mbs native [-h] [-c CONFIG] [-i] [-w] [variants ...]
+
+positional arguments:
+  variants              variants to build (defaults to 'debug' if not
+                        specified)
+
+options:
+  -h, --help            show this help message and exit
+  -c CONFIG, --config CONFIG
+                        the path to the top-level configuration file (default:
+                        'yambs.yaml')
+  -i, --single-pass     only run a single watch iteration
   -w, --watch           whether or not to continue watching for source tree
                         changes
 
 ```
 
 ### `uf2conv`
```

### Comparing `yambs-1.7.3/pyproject.toml` & `yambs-1.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "1.7.3"
+version = "1.8.0"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `yambs-1.7.3/setup.py` & `yambs-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.3/tests/test_entry.py` & `yambs-1.8.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.3/yambs/app.py` & `yambs-1.8.0/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.3/yambs/commands/gen.py` & `yambs-1.8.0/yambs/commands/common.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,28 @@
 """
-An entry-point for the 'gen' command.
+Common command-line argument interfaces.
 """
 
 # built-in
 from argparse import ArgumentParser as _ArgumentParser
 from argparse import Namespace as _Namespace
 from pathlib import Path as _Path
 from sys import executable
 
 # third-party
 from rcmpy.watch import watch
 from rcmpy.watch.params import WatchParams
-from vcorelib.args import CommandFunction as _CommandFunction
 
 # internal
 from yambs import PKG_NAME
-from yambs.config import DEFAULT_CONFIG, load
-from yambs.environment import BuildEnvironment
-from yambs.generate import generate
+from yambs.config.common import DEFAULT_CONFIG
 
 
-def gen_cmd(args: _Namespace) -> int:
-    """Execute the gen command."""
-
-    env = BuildEnvironment(load(path=args.config, root=args.dir))
-    generate(env)
-
-    return (
-        watch(
-            WatchParams(
-                args.dir,
-                _Path(str(env.config.data["src_root"])),
-                [
-                    executable,
-                    "-m",
-                    PKG_NAME,
-                    "-C",
-                    str(args.dir),
-                    "gen",
-                    "-c",
-                    str(args.config),
-                ],
-                False,  # Don't check file contents.
-                single_pass=args.single_pass,
-            )
-        )
-        if args.watch
-        else 0
-    )
-
-
-def add_gen_cmd(parser: _ArgumentParser) -> _CommandFunction:
-    """Add gen-command arguments to its parser."""
+def add_common_args(parser: _ArgumentParser) -> None:
+    """Add common command-line arguments to a parser."""
 
     parser.add_argument(
         "-c",
         "--config",
         type=_Path,
         default=DEFAULT_CONFIG,
         help=(
@@ -72,8 +39,33 @@
     parser.add_argument(
         "-w",
         "--watch",
         action="store_true",
         help="whether or not to continue watching for source tree changes",
     )
 
-    return gen_cmd
+
+def run_watch(args: _Namespace, src_root: _Path, command: str) -> int:
+    """Run the 'watch' command from rcmpy."""
+
+    return (
+        watch(
+            WatchParams(
+                args.dir,
+                src_root,
+                [
+                    executable,
+                    "-m",
+                    PKG_NAME,
+                    "-C",
+                    str(args.dir),
+                    command,
+                    "-c",
+                    str(args.config),
+                ],
+                False,  # Don't check file contents.
+                single_pass=args.single_pass,
+            )
+        )
+        if args.watch
+        else 0
+    )
```

### Comparing `yambs-1.7.3/yambs/commands/uf2conv.py` & `yambs-1.8.0/yambs/commands/uf2conv.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.3/yambs/config/__init__.py` & `yambs-1.8.0/yambs/config/common.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,95 +1,86 @@
 """
-A module implementing a configuration interface for the package.
+A module for common configuration interfaces.
 """
 
 # built-in
 from pathlib import Path
-from typing import Any, Dict, Iterator, List, Tuple
+from typing import Any, Dict, Type, TypeVar
 
 # third-party
 from vcorelib.dict import merge
 from vcorelib.dict.codec import BasicDictCodec as _BasicDictCodec
 from vcorelib.io import ARBITER as _ARBITER
+from vcorelib.io import DEFAULT_INCLUDES_KEY
 from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.paths import Pathlike, find_file, normalize
 
 # internal
 from yambs import PKG_NAME
-from yambs.config.board import Board
-from yambs.schemas import YambsDictCodec as _YambsDictCodec
 
+T = TypeVar("T", bound="CommonConfig")
+DEFAULT_CONFIG = f"{PKG_NAME}.yaml"
 
-class Config(_YambsDictCodec, _BasicDictCodec):
-    """The top-level configuration object for the package."""
-
-    data: Dict[str, Any]
-    root: Path
-    board_data: List[Board]
-    boards_by_name: Dict[str, Board]
-
-    def init(self, data: _JsonObject) -> None:
-        """Initialize this instance."""
-
-        self.data = data
-        self.root = Path()
-        self.boards_by_name = {}
-        self._init_boards()
 
-        self.src_root = self.directory("src_root")
-        self.build_root = self.directory("build_root")
+class CommonConfig(_BasicDictCodec):
+    """A common, base configuration."""
 
-    def _init_boards(self) -> None:
-        """Initialize board data."""
+    data: Dict[str, Any]
 
-        self.board_data = [
-            Board.from_dict(x, self.data["architectures"], self.data["chips"])
-            for x in self.data["boards"]
-        ]
-        for board in self.board_data:
-            self.boards_by_name[board.name] = board
+    root: Path
+    src_root: Path
+    build_root: Path
+    ninja_root: Path
 
     def directory(self, name: str, mkdir: bool = True) -> Path:
         """Get a configurable directory."""
 
         name_root = Path(str(self.data[name]))
         if not name_root.is_absolute():
             name_root = self.root.joinpath(name_root)
 
         if mkdir:
             name_root.mkdir(parents=True, exist_ok=True)
 
         return name_root
 
-    def boards(self) -> Iterator[Tuple[Board, Dict[str, Any]]]:
-        """Iterate over boards."""
-
-        for inst, board in zip(self.board_data, self.data["boards"]):
-            yield inst, board
-
+    def init(self, data: _JsonObject) -> None:
+        """Initialize this instance."""
 
-DEFAULT_CONFIG = f"{PKG_NAME}.yaml"
+        self.data = data
+        self.root = Path()
 
+        self.src_root = self.directory("src_root")
+        self.build_root = self.directory("build_root")
+        self.ninja_root = self.directory("ninja_out")
 
-def load(path: Pathlike = DEFAULT_CONFIG, root: Pathlike = None) -> Config:
-    """Load a configuration."""
+    @classmethod
+    def load(
+        cls: Type[T],
+        path: Pathlike = DEFAULT_CONFIG,
+        package_config: str = DEFAULT_CONFIG,
+        root: Pathlike = None,
+    ) -> T:
+        """Load a configuration."""
 
-    src_config = find_file(DEFAULT_CONFIG, package=PKG_NAME)
-    assert src_config is not None
+        src_config = find_file(package_config, package=PKG_NAME)
+        assert src_config is not None
 
-    result = Config.create(
-        merge(
+        data = merge(
             _ARBITER.decode(
-                src_config, includes_key="includes", require_success=True
+                src_config,
+                includes_key=DEFAULT_INCLUDES_KEY,
+                require_success=True,
             ).data,
-            _ARBITER.decode(path, includes_key="includes").data,
+            _ARBITER.decode(path, includes_key=DEFAULT_INCLUDES_KEY).data,
             # Always allow the project-specific configuration to override
             # package data.
             expect_overwrite=True,
         )
-    )
 
-    if root is not None:
-        result.root = normalize(root)
-        result.root.mkdir(parents=True, exist_ok=True)
+        result = cls.create(data)
+
+        if root is not None:
+            result.root = normalize(root)
+            result.root.mkdir(parents=True, exist_ok=True)
 
-    return result
+        return result
```

### Comparing `yambs-1.7.3/yambs/config/board.py` & `yambs-1.8.0/yambs/config/board.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.3/yambs/data/includes/chips.yaml` & `yambs-1.8.0/yambs/data/includes/chips.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.7.3/yambs/data/includes/infineon.yaml` & `yambs-1.8.0/yambs/data/includes/infineon.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.7.3/yambs/data/includes/microchip.yaml` & `yambs-1.8.0/yambs/data/includes/microchip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.7.3/yambs/data/schemas/Chip.yaml` & `yambs-1.8.0/yambs/data/schemas/Chip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.7.3/yambs/data/templates/rules.ninja.j2` & `yambs-1.8.0/yambs/data/templates/rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-1.7.3/yambs/data/uf2families.json` & `yambs-1.8.0/yambs/data/uf2families.json`

 * *Files identical despite different names*

### Comparing `yambs-1.7.3/yambs/entry.py` & `yambs-1.8.0/yambs/entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.3/yambs/environment/__init__.py` & `yambs-1.8.0/yambs/environment/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,16 +49,14 @@
     def __init__(self, config: Config) -> None:
         """Initialize this instance."""
 
         super().__init__()
 
         self.config = config
 
-        self.ninja_root = self.config.directory("ninja_out")
-
         # Keep track of all overall sources, so that no duplicate rules are
         # generated.
         self.global_sources: Set[Path] = set()
         self.first_party_headers: Set[Path] = set()
 
         # Keep track of sources by board.
         self.by_board: Dict[Board, SourceSets] = {}
```

### Comparing `yambs-1.7.3/yambs/generate/__init__.py` & `yambs-1.8.0/yambs/generate/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,27 +2,25 @@
 A module for generating templated outputs.
 """
 
 # built-in
 from typing import Any, Dict
 
 # third-party
-from datazen.templates import environment
-from jinja2 import FileSystemLoader
 from vcorelib.io import ARBITER
 from vcorelib.paths import resource
 
 # internal
 from yambs import PKG_NAME
 from yambs.environment import BuildEnvironment
 from yambs.generate.architectures import generate as generate_architectures
 from yambs.generate.boards import generate as generate_boards
 from yambs.generate.chips import generate as generate_chips
-from yambs.generate.common import render_template
-from yambs.generate.ninja.format import write_format_target
+from yambs.generate.common import get_jinja, render_template
+from yambs.generate.ninja.format import render_format
 from yambs.generate.toolchains import generate as generate_toolchains
 
 
 def create_board_apps(env: BuildEnvironment) -> None:
     """
     Generate JSON metadata to give other tools a simple lookup to application
     sources (e.g. for loading or deploying).
@@ -35,40 +33,38 @@
     for board in env.config.board_data:
         board_apps[board.name] = {
             short: str(env.config.build_root.joinpath(path))
             for short, path in board.apps.items()
         }
 
     ARBITER.encode(
-        env.ninja_root.joinpath("board_apps.json"),
+        env.config.ninja_root.joinpath("board_apps.json"),
         board_apps,
     )
 
 
 def generate(env: BuildEnvironment) -> None:
     """Generate ninja files."""
 
     templates_dir = resource("templates", package=PKG_NAME)
     assert templates_dir is not None
 
-    jinja = environment(
-        loader=FileSystemLoader([templates_dir], followlinks=True)
-    )
+    jinja = get_jinja()
 
     # Render the top-level configuration. This is the only file that's
     # generated into the root directory.
     render_template(jinja, env.config.root, "build.ninja", env.config.data)
 
     # Generate all other files.
     for gen in [
         generate_chips,
         generate_toolchains,
         generate_architectures,
-        generate_boards,
     ]:
-        gen(jinja, env)
+        gen(jinja, env.config)
+
+    generate_boards(jinja, env)
 
     create_board_apps(env)
 
     # Create format configuration.
-    with env.ninja_root.joinpath("format.ninja").open("w") as path_fd:
-        write_format_target(path_fd, env)
+    render_format(env.config, env.first_party_sources_headers())
```

### Comparing `yambs-1.7.3/yambs/generate/architectures.py` & `yambs-1.8.0/yambs/generate/architectures.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 A module for generating architecture-related files.
 """
 
 # third-party
 from jinja2 import Environment
 
 # internal
-from yambs.environment import BuildEnvironment
+from yambs.config.common import CommonConfig
 from yambs.generate.common import render_template
 
 
-def generate(jinja: Environment, env: BuildEnvironment) -> None:
+def generate(jinja: Environment, config: CommonConfig) -> None:
     """Generate architecture-related ninja files."""
 
-    for name, data in env.config.data["architectures"].items():
-        architectures_root = env.ninja_root.joinpath("architectures", name)
+    for name, data in config.data["architectures"].items():
+        architectures_root = config.ninja_root.joinpath("architectures", name)
         architectures_root.mkdir(parents=True, exist_ok=True)
 
         render_template(
             jinja,
             architectures_root,
             "architecture.ninja",
             data,
```

### Comparing `yambs-1.7.3/yambs/generate/boards.py` & `yambs-1.8.0/yambs/generate/boards.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # third-party
 from jinja2 import Environment
 from vcorelib.paths import rel
 
 # internal
 from yambs.config.board import Board
 from yambs.environment import BuildEnvironment, SourceSets
-from yambs.generate.common import render_template
+from yambs.generate.common import APP_ROOT, render_template
 from yambs.generate.ninja import write_link_lines, write_source_line
 from yambs.translation import is_header, is_source
 
 LOG = getLogger(__name__)
 
 
 def add_dir(
@@ -130,15 +130,15 @@
             env.global_sources,
             board,
         )
 
     # Add application sources.
     app_srcs: Set[Path] = set()
     for kind, path in create_paths_dict(
-        src_root.joinpath("apps"), board
+        src_root.joinpath(APP_ROOT), board
     ).items():
         headers.update(
             add_dir(
                 stream,
                 app_srcs,
                 path,
                 f"{kind} application sources",
@@ -159,20 +159,22 @@
 
 
 def generate(jinja: Environment, env: BuildEnvironment) -> None:
     """Generate board-related ninja files."""
 
     # Render the board manifest and rules file.
     for template in ["all.ninja", "rules.ninja"]:
-        render_template(jinja, env.ninja_root, template, env.config.data)
+        render_template(
+            jinja, env.config.ninja_root, template, env.config.data
+        )
 
     src_root = rel(env.config.src_root)
 
     for board, raw_data in env.config.boards():
-        board_root = env.ninja_root.joinpath("boards", board.name)
+        board_root = env.config.ninja_root.joinpath("boards", board.name)
         board_root.mkdir(parents=True, exist_ok=True)
         render_template(jinja, board_root, "board.ninja", raw_data)
 
         # Perform source-file discovery.
         with board_root.joinpath("sources.ninja").open("w") as path_fd:
             sources = write_sources(path_fd, board, src_root, env)
```

### Comparing `yambs-1.7.3/yambs/generate/chips.py` & `yambs-1.8.0/yambs/generate/chips.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 A module for generating chip-related files.
 """
 
 # third-party
 from jinja2 import Environment
 
 # internal
-from yambs.environment import BuildEnvironment
+from yambs.config.common import CommonConfig
 from yambs.generate.common import render_template
 
 
-def generate(jinja: Environment, env: BuildEnvironment) -> None:
+def generate(jinja: Environment, config: CommonConfig) -> None:
     """Generate chip-related ninja files."""
 
-    for name, data in env.config.data["chips"].items():
-        chips_root = env.ninja_root.joinpath("chips", name)
+    for name, data in config.data["chips"].items():
+        chips_root = config.ninja_root.joinpath("chips", name)
         chips_root.mkdir(parents=True, exist_ok=True)
 
         # Render chip files and linker scripts.
         render_template(
             jinja,
             chips_root,
             "chip.ninja",
```

### Comparing `yambs-1.7.3/yambs/generate/ninja/__init__.py` & `yambs-1.8.0/yambs/generate/ninja/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.3/yambs/schemas.py` & `yambs-1.8.0/yambs/schemas.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 """
 
 # built-in
 from typing import Optional as _Optional
 
 # third-party
 from vcorelib.dict.codec import DictCodec as _DictCodec
+from vcorelib.io import DEFAULT_INCLUDES_KEY
 from vcorelib.schemas.base import SchemaMap as _SchemaMap
 from vcorelib.schemas.json import JsonSchemaMap as _JsonSchemaMap
 
 # internal
 from yambs import PKG_NAME
 
 
 class YambsDictCodec(_DictCodec):
     """
     A simple wrapper for package classes that want to implement DictCodec.
     """
 
     default_schemas: _Optional[_SchemaMap] = _JsonSchemaMap.from_package(
-        PKG_NAME
+        PKG_NAME,
+        includes_key=DEFAULT_INCLUDES_KEY,
     )
```

### Comparing `yambs-1.7.3/yambs/translation/__init__.py` & `yambs-1.8.0/yambs/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.3/yambs/uf2/__init__.py` & `yambs-1.8.0/yambs/uf2/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.3/yambs.egg-info/PKG-INFO` & `yambs-1.8.0/yambs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.7.3
+Version: 1.8.0
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=bb422a51478a96037d8ddd3a3e4597a7
+    hash=c88caeb9c6d71c51d9fd724250cd248c
     =====================================
 -->
 
-# yambs ([1.7.3](https://pypi.org/project/yambs/))
+# yambs ([1.8.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
 
@@ -150,29 +150,31 @@
 following a specific convention), put your configuration data here.
 
 # Command-line Options
 
 ```
 $ ./venv3.11/bin/mbs -h
 
-usage: mbs [-h] [--version] [-v] [-C DIR] {gen,uf2conv,noop} ...
+usage: mbs [-h] [--version] [-v] [-C DIR] {gen,native,uf2conv,noop} ...
 
 Yet another meta build-system.
 
 options:
-  -h, --help          show this help message and exit
-  --version           show program's version number and exit
-  -v, --verbose       set to increase logging verbosity
-  -C DIR, --dir DIR   execute from a specific directory
+  -h, --help            show this help message and exit
+  --version             show program's version number and exit
+  -v, --verbose         set to increase logging verbosity
+  -C DIR, --dir DIR     execute from a specific directory
 
 commands:
-  {gen,uf2conv,noop}  set of available commands
-    gen               poll the source tree and generate any new build files
-    uf2conv           Convert to UF2 or flash directly.
-    noop              command stub (does nothing)
+  {gen,native,uf2conv,noop}
+                        set of available commands
+    gen                 poll the source tree and generate any new build files
+    native              generate build files for native-only target projects
+    uf2conv             Convert to UF2 or flash directly.
+    noop                command stub (does nothing)
 
 ```
 
 ## Sub-command Options
 
 ### `gen`
 
@@ -183,14 +185,36 @@
 
 options:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         the path to the top-level configuration file (default:
                         'yambs.yaml')
   -i, --single-pass     only run a single watch iteration
+  -w, --watch           whether or not to continue watching for source tree
+                        changes
+
+```
+
+### `native`
+
+```
+$ ./venv3.11/bin/mbs native -h
+
+usage: mbs native [-h] [-c CONFIG] [-i] [-w] [variants ...]
+
+positional arguments:
+  variants              variants to build (defaults to 'debug' if not
+                        specified)
+
+options:
+  -h, --help            show this help message and exit
+  -c CONFIG, --config CONFIG
+                        the path to the top-level configuration file (default:
+                        'yambs.yaml')
+  -i, --single-pass     only run a single watch iteration
   -w, --watch           whether or not to continue watching for source tree
                         changes
 
 ```
 
 ### `uf2conv`
```

### Comparing `yambs-1.7.3/yambs.egg-info/SOURCES.txt` & `yambs-1.8.0/yambs.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -14,42 +14,60 @@
 yambs/schemas.py
 yambs.egg-info/PKG-INFO
 yambs.egg-info/SOURCES.txt
 yambs.egg-info/dependency_links.txt
 yambs.egg-info/entry_points.txt
 yambs.egg-info/requires.txt
 yambs.egg-info/top_level.txt
+yambs/aggregation/__init__.py
 yambs/commands/__init__.py
 yambs/commands/all.py
+yambs/commands/common.py
 yambs/commands/gen.py
+yambs/commands/native.py
 yambs/commands/uf2conv.py
 yambs/config/__init__.py
 yambs/config/board.py
+yambs/config/common.py
+yambs/config/native.py
+yambs/data/native.yaml
 yambs/data/uf2families.json
 yambs/data/yambs.yaml
 yambs/data/includes/chips.yaml
 yambs/data/includes/infineon.yaml
 yambs/data/includes/microchip.yaml
 yambs/data/schemas/Architecture.yaml
 yambs/data/schemas/Board.yaml
 yambs/data/schemas/Chip.yaml
 yambs/data/schemas/Config.yaml
+yambs/data/schemas/Native.yaml
 yambs/data/schemas/Toolchain.yaml
+yambs/data/schemas/Variant.yaml
+yambs/data/schemas/config_common.yaml
+yambs/data/schemas/targets_common.yaml
+yambs/data/schemas/toolchain_common.yaml
 yambs/data/templates/all.ninja.j2
 yambs/data/templates/architecture.ninja.j2
 yambs/data/templates/board.ninja.j2
 yambs/data/templates/build.ninja.j2
 yambs/data/templates/chip.ld.j2
 yambs/data/templates/chip.ninja.j2
+yambs/data/templates/compile_commands.ninja.j2
+yambs/data/templates/native_all.ninja.j2
+yambs/data/templates/native_build.ninja.j2
+yambs/data/templates/native_rules.ninja.j2
 yambs/data/templates/rules.ninja.j2
 yambs/data/templates/toolchain.ninja.j2
+yambs/data/templates/variant.ninja.j2
 yambs/environment/__init__.py
+yambs/environment/native.py
 yambs/generate/__init__.py
 yambs/generate/architectures.py
 yambs/generate/boards.py
 yambs/generate/chips.py
 yambs/generate/common.py
 yambs/generate/toolchains.py
+yambs/generate/variants.py
 yambs/generate/ninja/__init__.py
 yambs/generate/ninja/format.py
 yambs/translation/__init__.py
 yambs/uf2/__init__.py
```

