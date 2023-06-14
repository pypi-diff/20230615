# Comparing `tmp/myoktros-0.0.1.tar.gz` & `tmp/myoktros-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "myoktros-0.0.2.tar", max compression
```

## Comparing `myoktros-0.0.1.tar` & `myoktros-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,9 @@
--rwxr-xr-x   0        0        0     5664 2020-02-02 00:00:00.000000 myoktros-0.0.1/assets/position_confirmed.mp3
--rwxr-xr-x   0        0        0     5184 2020-02-02 00:00:00.000000 myoktros-0.0.1/assets/position_deleted.mp3
--rwxr-xr-x   0        0        0     5184 2020-02-02 00:00:00.000000 myoktros-0.0.1/assets/standard_mode.mp3
--rwxr-xr-x   0        0        0     4320 2020-02-02 00:00:00.000000 myoktros-0.0.1/assets/teach_mode.mp3
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 myoktros-0.0.1/docker-ros2-xarm/Dockerfile
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 myoktros-0.0.1/docker-ros2-xarm/README.md
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 myoktros-0.0.1/docker-ros2-xarm/entrypoint.sh
--rwxr-xr-x   0        0        0     1904 2020-02-02 00:00:00.000000 myoktros-0.0.1/src/myoktros/__init__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 myoktros-0.0.1/src/myoktros/gesture.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 myoktros-0.0.1/src/myoktros/mode.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 myoktros-0.0.1/src/myoktros/ros.py
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 myoktros-0.0.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 myoktros-0.0.1/LICENSE
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 myoktros-0.0.1/README.md
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 myoktros-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 myoktros-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-06-14 23:53:33.677031 myoktros-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3769 2023-06-14 23:53:33.677031 myoktros-0.0.2/README.md
+-rw-r--r--   0        0        0     3214 2023-06-14 23:54:22.933186 myoktros-0.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0     4374 2023-06-14 23:53:33.681031 myoktros-0.0.2/src/myoktros/__init__.py
+-rw-r--r--   0        0        0     2054 2023-06-14 23:53:33.681031 myoktros-0.0.2/src/myoktros/gesture.py
+-rw-r--r--   0        0        0      128 2023-06-14 23:53:33.681031 myoktros-0.0.2/src/myoktros/kt_mode.py
+-rw-r--r--   0        0        0     6158 2023-06-14 23:53:33.681031 myoktros-0.0.2/src/myoktros/myo_manager.py
+-rw-r--r--   0        0        0     4337 2023-06-14 23:53:33.681031 myoktros-0.0.2/src/myoktros/ros.py
+-rw-r--r--   0        0        0     4437 1970-01-01 00:00:00.000000 myoktros-0.0.2/PKG-INFO
```

### Comparing `myoktros-0.0.1/src/myoktros/ros.py` & `myoktros-0.0.2/src/myoktros/ros.py`

 * *Files identical despite different names*

### Comparing `myoktros-0.0.1/LICENSE` & `myoktros-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `myoktros-0.0.1/pyproject.toml` & `myoktros-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,40 @@
-[build-system]
-requires = ["hatchling>=1.17.1", "hatch-vcs>=0.3.0"]
-build-backend = "hatchling.build"
-
 [project]
-name = "myoktros"
+name = "MyoKTROS"
 authors = [
-  { name="Felix Wohlgemuth" },
   { name="Iori Mizutani", email="iori.mizutani@gmail.com" },
+  { name="Felix Wohlgemuth", email="felixwohlgemuth@gmx.ch" },
 ]
 maintainers = [
   { name="Iori Mizutani", email="iori.mizutani@gmail.com" },
 ]
 description = "Myo EMG-based KT system for ROS"
 readme = "README.md"
-requires-python = ">=3.10"
-dependencies = [
-    "dl-myo>=0.1.5",
-]
 classifiers = [
     "Environment :: Console",
     "Framework :: AsyncIO",
+    "Framework :: Robot Framework :: Tool",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Human Machine Interfaces",
 ]
 dynamic = ["version"]
 
-[project.scripts]
-myoktros = "myoktros:entrypoint"
-
 [project.urls]
 "Homepage" = "https://github.com/Interactions-HSG/MyoKTROS"
 "Bug Tracker" = "https://github.com/Interactions-HSG/MyoKTROS/issues"
 
-[tool.hatch.version]
-source = "vcs"
-
-[tool.hatch.version.raw-options]
-version_scheme = "python-simplified-semver"
-local_scheme = "no-local-version"
-parentdir_prefix_version = "v"
-git_describe_command = ["git", "describe", "--dirty", "--tags", "--long", "--match", "v*"]
-
-[tool.hatch.build.targets.sdist]
-exclude = [
-  "/.github",
-]
-
 [tool.black]
 line-length = 120
 skip-string-normalization = true
-target-version = ["py311"]
+target-version = ["py310"]
 
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
 select = ["E", "F"]
 ignore = []
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
@@ -89,17 +64,64 @@
     "venv",
 ]
 # Same as Black.
 line-length = 120
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 # Assume Python 3.10.
-target-version = "py311"
+target-version = "py310"
 
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
+
+[tool.coverage.run]
+branch = true
+
+[tool.coverage.paths]
+tests = ["tests"]
+
+[tool.coverage.report]
+exclude_lines = [
+  "no cov",
+  "if __name__ == .__main__.:",
+  "if TYPE_CHECKING:",
+]
+
+[tool.poetry]
+name = "MyoKTROS"
+version = "0.0.2"
+description = "Myo EMG-based KT system for ROS"
+authors = ["Iori Mizutani <iori.mizutani@gmail.com>"]
+license = "MIT"
+readme = "README.md"
+
+[tool.poetry.dependencies]
+python = ">=3.9,<3.11"
+dl-myo = ">=0.2.0"
+joblib = "^1.2.0"
+numpy = "^1.24.3"
+pandas = "^2.0.2"
+scikit-learn = "^1.2.2"
+tensorflow = ">=2.12.0"
+
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+pytest = "^7.3.2"
+pytest-cov = "^4.1.0"
+
+[tool.poetry.scripts]
+myoktros = "myoktros:entrypoint"
+
+[tool.poetry-dynamic-versioning]
+enable = false
+vcs = "git"
+style = "semver"
+
+[build-system]
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
```

