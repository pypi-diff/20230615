# Comparing `tmp/ccbuilder-0.0.9.tar.gz` & `tmp/ccbuilder-0.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccbuilder-0.0.9.tar", last modified: Fri Jul 29 09:18:51 2022, max compression
+gzip compressed data, was "ccbuilder-0.1.0b0.tar", last modified: Thu Jun 15 14:38:02 2023, max compression
```

## Comparing `ccbuilder-0.0.9.tar` & `ccbuilder-0.1.0b0.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-29 09:18:51.992906 ccbuilder-0.0.9/
--rw-r--r--   0 theo      (1000) theo      (1000)    11368 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/LICENSE
--rw-r--r--   0 theo      (1000) theo      (1000)       54 2022-05-25 09:41:26.000000 ccbuilder-0.0.9/MANIFEST.in
--rw-r--r--   0 theo      (1000) theo      (1000)      681 2022-07-29 09:18:51.992906 ccbuilder-0.0.9/PKG-INFO
--rw-r--r--   0 theo      (1000) theo      (1000)      290 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/README.md
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-29 09:18:51.982906 ccbuilder-0.0.9/ccbuilder/
--rw-r--r--   0 theo      (1000) theo      (1000)     9576 2022-07-29 08:14:28.000000 ccbuilder-0.0.9/ccbuilder/__init__.py
--rw-r--r--   0 theo      (1000) theo      (1000)       75 2022-05-25 09:41:26.000000 ccbuilder-0.0.9/ccbuilder/__main__.py
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-29 09:18:51.982906 ccbuilder-0.0.9/ccbuilder/builder/
--rw-r--r--   0 theo      (1000) theo      (1000)        0 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/builder/__init__.py
--rw-r--r--   0 theo      (1000) theo      (1000)    14768 2022-07-29 08:16:54.000000 ccbuilder-0.0.9/ccbuilder/builder/builder.py
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-29 09:18:51.979572 ccbuilder-0.0.9/ccbuilder/data/
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-29 09:18:51.986239 ccbuilder-0.0.9/ccbuilder/data/patches/
--rw-r--r--   0 theo      (1000) theo      (1000)     1248 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/data/patches/gcc-fix-simple-object-decl-and-use-in-gcc-lto.patch
--rw-r--r--   0 theo      (1000) theo      (1000)      632 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/data/patches/gcc-libsanitizer.sh
--rw-r--r--   0 theo      (1000) theo      (1000)      739 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/data/patches/gcc-simple-object-declaration.patch
--rw-r--r--   0 theo      (1000) theo      (1000)     2761 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/data/patches/gcc-ustat.patch
--rw-r--r--   0 theo      (1000) theo      (1000)     2072 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/data/patches/llvm-GCOpenMPRuntime.cpp-lambda-issues.patch
--rw-r--r--   0 theo      (1000) theo      (1000)      810 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/data/patches/llvm-MicrosoftDemangleNodes-missing-includes.patch
--rw-r--r--   0 theo      (1000) theo      (1000)      955 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/data/patches/llvm-MicrosoftDemangleNodes.h-fix-includes.patch
--rw-r--r--   0 theo      (1000) theo      (1000)  1011052 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/data/patches/patchdb.json
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-29 09:18:51.992906 ccbuilder-0.0.9/ccbuilder/patcher/
--rw-r--r--   0 theo      (1000) theo      (1000)        0 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/patcher/__init__.py
--rw-r--r--   0 theo      (1000) theo      (1000)     6300 2022-07-29 08:14:28.000000 ccbuilder-0.0.9/ccbuilder/patcher/patchdatabase.py
--rw-r--r--   0 theo      (1000) theo      (1000)    20255 2022-07-29 08:14:28.000000 ccbuilder-0.0.9/ccbuilder/patcher/patcher.py
--rw-r--r--   0 theo      (1000) theo      (1000)        0 2022-05-25 09:41:26.000000 ccbuilder-0.0.9/ccbuilder/py.typed
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-29 09:18:51.992906 ccbuilder-0.0.9/ccbuilder/utils/
--rw-r--r--   0 theo      (1000) theo      (1000)        0 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/utils/__init__.py
--rw-r--r--   0 theo      (1000) theo      (1000)    10483 2022-07-29 08:14:28.000000 ccbuilder-0.0.9/ccbuilder/utils/repository.py
--rw-r--r--   0 theo      (1000) theo      (1000)     5648 2022-07-29 08:14:28.000000 ccbuilder-0.0.9/ccbuilder/utils/utils.py
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-29 09:18:51.982906 ccbuilder-0.0.9/ccbuilder.egg-info/
--rw-r--r--   0 theo      (1000) theo      (1000)      681 2022-07-29 09:18:51.000000 ccbuilder-0.0.9/ccbuilder.egg-info/PKG-INFO
--rw-r--r--   0 theo      (1000) theo      (1000)      987 2022-07-29 09:18:51.000000 ccbuilder-0.0.9/ccbuilder.egg-info/SOURCES.txt
--rw-r--r--   0 theo      (1000) theo      (1000)        1 2022-07-29 09:18:51.000000 ccbuilder-0.0.9/ccbuilder.egg-info/dependency_links.txt
--rw-r--r--   0 theo      (1000) theo      (1000)       54 2022-07-29 09:18:51.000000 ccbuilder-0.0.9/ccbuilder.egg-info/entry_points.txt
--rw-r--r--   0 theo      (1000) theo      (1000)       10 2022-07-29 09:18:51.000000 ccbuilder-0.0.9/ccbuilder.egg-info/top_level.txt
--rw-r--r--   0 theo      (1000) theo      (1000)      126 2022-05-25 09:41:26.000000 ccbuilder-0.0.9/pyproject.toml
--rw-r--r--   0 theo      (1000) theo      (1000)      678 2022-07-29 09:18:51.996240 ccbuilder-0.0.9/setup.cfg
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-06-15 14:38:02.082719 ccbuilder-0.1.0b0/
+-rw-r--r--   0 theo      (1000) theo      (1000)    11368 2022-07-05 11:38:26.000000 ccbuilder-0.1.0b0/LICENSE
+-rw-r--r--   0 theo      (1000) theo      (1000)       54 2022-07-05 11:38:26.000000 ccbuilder-0.1.0b0/MANIFEST.in
+-rw-r--r--   0 theo      (1000) theo      (1000)      683 2023-06-15 14:38:02.082719 ccbuilder-0.1.0b0/PKG-INFO
+-rw-r--r--   0 theo      (1000) theo      (1000)      290 2022-07-05 11:38:26.000000 ccbuilder-0.1.0b0/README.md
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-06-15 14:38:02.082719 ccbuilder-0.1.0b0/ccbuilder/
+-rw-r--r--   0 theo      (1000) theo      (1000)    11274 2023-06-15 14:37:28.000000 ccbuilder-0.1.0b0/ccbuilder/__init__.py
+-rw-r--r--   0 theo      (1000) theo      (1000)       75 2022-07-05 11:38:26.000000 ccbuilder-0.1.0b0/ccbuilder/__main__.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     1021 2023-06-15 14:37:28.000000 ccbuilder-0.1.0b0/ccbuilder/bisector.py
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-06-15 14:38:02.082719 ccbuilder-0.1.0b0/ccbuilder/builder/
+-rw-r--r--   0 theo      (1000) theo      (1000)        0 2022-07-05 11:38:26.000000 ccbuilder-0.1.0b0/ccbuilder/builder/__init__.py
+-rw-r--r--   0 theo      (1000) theo      (1000)    14633 2023-06-15 14:37:28.000000 ccbuilder-0.1.0b0/ccbuilder/builder/builder.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     7824 2023-06-15 14:37:28.000000 ccbuilder-0.1.0b0/ccbuilder/compilerstore.py
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-06-15 14:38:02.082719 ccbuilder-0.1.0b0/ccbuilder/data/
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-06-15 14:38:02.082719 ccbuilder-0.1.0b0/ccbuilder/data/patches/
+-rw-r--r--   0 theo      (1000) theo      (1000)     1248 2022-07-05 11:38:26.000000 ccbuilder-0.1.0b0/ccbuilder/data/patches/gcc-fix-simple-object-decl-and-use-in-gcc-lto.patch
+-rw-r--r--   0 theo      (1000) theo      (1000)      632 2022-07-05 11:38:26.000000 ccbuilder-0.1.0b0/ccbuilder/data/patches/gcc-libsanitizer.sh
+-rw-r--r--   0 theo      (1000) theo      (1000)      739 2022-07-05 11:38:26.000000 ccbuilder-0.1.0b0/ccbuilder/data/patches/gcc-simple-object-declaration.patch
+-rw-r--r--   0 theo      (1000) theo      (1000)     2761 2022-07-05 11:38:26.000000 ccbuilder-0.1.0b0/ccbuilder/data/patches/gcc-ustat.patch
+-rw-r--r--   0 theo      (1000) theo      (1000)     2072 2022-07-05 11:38:26.000000 ccbuilder-0.1.0b0/ccbuilder/data/patches/llvm-GCOpenMPRuntime.cpp-lambda-issues.patch
+-rw-r--r--   0 theo      (1000) theo      (1000)      810 2022-07-05 11:38:26.000000 ccbuilder-0.1.0b0/ccbuilder/data/patches/llvm-MicrosoftDemangleNodes-missing-includes.patch
+-rw-r--r--   0 theo      (1000) theo      (1000)      955 2022-07-05 11:38:26.000000 ccbuilder-0.1.0b0/ccbuilder/data/patches/llvm-MicrosoftDemangleNodes.h-fix-includes.patch
+-rw-r--r--   0 theo      (1000) theo      (1000)  1011052 2022-07-05 11:38:26.000000 ccbuilder-0.1.0b0/ccbuilder/data/patches/patchdb.json
+-rw-r--r--   0 theo      (1000) theo      (1000)      167 2023-06-15 14:37:28.000000 ccbuilder-0.1.0b0/ccbuilder/defaults.py
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-06-15 14:38:02.082719 ccbuilder-0.1.0b0/ccbuilder/patcher/
+-rw-r--r--   0 theo      (1000) theo      (1000)        0 2022-07-05 11:38:26.000000 ccbuilder-0.1.0b0/ccbuilder/patcher/__init__.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     6341 2023-06-15 14:37:28.000000 ccbuilder-0.1.0b0/ccbuilder/patcher/patchdatabase.py
+-rw-r--r--   0 theo      (1000) theo      (1000)    20428 2023-06-15 14:37:28.000000 ccbuilder-0.1.0b0/ccbuilder/patcher/patcher.py
+-rw-r--r--   0 theo      (1000) theo      (1000)        0 2022-07-05 11:38:26.000000 ccbuilder-0.1.0b0/ccbuilder/py.typed
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-06-15 14:38:02.082719 ccbuilder-0.1.0b0/ccbuilder/utils/
+-rw-r--r--   0 theo      (1000) theo      (1000)        0 2022-07-05 11:38:26.000000 ccbuilder-0.1.0b0/ccbuilder/utils/__init__.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     3290 2023-06-15 14:37:28.000000 ccbuilder-0.1.0b0/ccbuilder/utils/utils.py
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-06-15 14:38:02.082719 ccbuilder-0.1.0b0/ccbuilder.egg-info/
+-rw-r--r--   0 theo      (1000) theo      (1000)      683 2023-06-15 14:38:02.000000 ccbuilder-0.1.0b0/ccbuilder.egg-info/PKG-INFO
+-rw-r--r--   0 theo      (1000) theo      (1000)     1060 2023-06-15 14:38:02.000000 ccbuilder-0.1.0b0/ccbuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)        1 2023-06-15 14:38:02.000000 ccbuilder-0.1.0b0/ccbuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)       54 2023-06-15 14:38:02.000000 ccbuilder-0.1.0b0/ccbuilder.egg-info/entry_points.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)       16 2023-06-15 14:38:02.000000 ccbuilder-0.1.0b0/ccbuilder.egg-info/requires.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)       10 2023-06-15 14:38:02.000000 ccbuilder-0.1.0b0/ccbuilder.egg-info/top_level.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)      126 2022-07-05 11:38:26.000000 ccbuilder-0.1.0b0/pyproject.toml
+-rw-r--r--   0 theo      (1000) theo      (1000)      718 2023-06-15 14:38:02.082719 ccbuilder-0.1.0b0/setup.cfg
```

### Comparing `ccbuilder-0.0.9/LICENSE` & `ccbuilder-0.1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.9/PKG-INFO` & `ccbuilder-0.1.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccbuilder
-Version: 0.0.9
+Version: 0.1.0b0
 Summary: A clang/gcc compiler builder and patcher
 Home-page: https://github.com/DeadCodeProductions/ccbuilder
 Author: Theodoros Theodoridis
 Author-email: theodort@inf.ethz.ch
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

### Comparing `ccbuilder-0.0.9/ccbuilder/__init__.py` & `ccbuilder-0.1.0b0/ccbuilder/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,49 @@
 import logging
 import os
-import shlex
 from argparse import ArgumentParser, Namespace
 from multiprocessing import cpu_count
 from pathlib import Path
-from subprocess import run
+from typing import Optional
+
+from diopter.repository import (
+    Repo,
+    RepositoryException,
+    Revision,
+    Commit,
+    get_gcc_repo,
+    get_llvm_repo,
+    get_gcc_releases,
+    get_llvm_releases,
+    DEFAULT_REPOS_DIR,
+)
+from diopter.compiler import CompilerProject
 
 from ccbuilder.builder.builder import (
     build_and_install_compiler,
-    BuilderWithoutCache,
     Builder,
     BuildException,
 )
 from ccbuilder.patcher.patchdatabase import PatchDB
 from ccbuilder.patcher.patcher import Patcher
-from ccbuilder.utils.repository import Repo, RepositoryException, Revision, Commit
 from ccbuilder.utils.utils import (
-    CompilerProject,
-    MajorCompilerReleases,
-    CompilerReleases,
-    get_repo,
     get_compiler_info,
     get_compiler_project,
-    find_cached_revisions,
+    initialize_repos,
+    initialize_patches_dir,
+)
+from ccbuilder.compilerstore import (
+    CompilerStore,
+    scan_directory_and_populate_store,
+    load_compiler_store,
+    default_store_file,
+)
+from ccbuilder.defaults import (
+    DEFAULT_PREFIX_PARENT_PATH,
+    DEFAULT_PATCH_DIR,
 )
 
 __all__ = [
     "CompilerProject",
     "Repo",
     "RepositoryException",
     "Revision",
@@ -35,49 +52,25 @@
     "Patcher",
     "build_and_install_compiler",
     "BuilderWithoutCache",
     "Builder",
     "BuildException",
     "CompilerReleases",
     "MajorCompilerReleases",
-    "get_repo",
-    "find_cached_revisions",
+    "get_gcc_repo",
+    "get_llvm_repo",
     "get_compiler_info",
     "get_compiler_project",
+    "initialize_repos",
+    "initialize_patches_dir",
+    "DEFAULT_PREFIX_PARENT_PATH",
+    "DEFAULT_PATCH_DIR",
+    "DEFAULT_REPOS_DIR",
 ]
 
-_ROOT = Path(__file__).parent.absolute()
-
-
-def _initialize(args: Namespace) -> None:
-    from shutil import copy
-
-    repos_path = Path(args.repos_dir)
-    repos_path.mkdir(parents=True, exist_ok=True)
-    llvm = repos_path / "llvm-project"
-    if not llvm.exists():
-        print("Cloning LLVM...")
-        run(
-            shlex.split(f"git clone https://github.com/llvm/llvm-project.git {llvm}"),
-            check=True,
-        )
-    gcc = repos_path / "gcc"
-    if not gcc.exists():
-        print("Cloning GCC...")
-        run(
-            shlex.split(f"git clone git://gcc.gnu.org/git/gcc.git {gcc}"),
-            check=True,
-        )
-    patches_path = Path(args.patches_dir)
-    if not patches_path.exists():
-        patches_path.mkdir(parents=True, exist_ok=True)
-        patches_source_dir = _ROOT / "data" / "patches"
-        for entry in patches_source_dir.iterdir():
-            copy(entry, patches_path / entry.name)
-
 
 def ccbuilder_base_parser() -> ArgumentParser:
     parser = ArgumentParser("ccbuilder", add_help=False)
 
     parser.add_argument(
         "-ll",
         "--log-level",
@@ -94,53 +87,71 @@
     )
     parser.add_argument(
         "--jobs",
         type=int,
         default=cpu_count(),
         help="Number of build jobs (default:use all cores)",
     )
-    default_prefix = str(Path.home() / ".cache" / "ccbuilder-compilers")
+
+    # XXX:the word prefix is a bit misleading, this is the parent of the prefix
+    # Misleading in the way, that it could be mistaken for the installation prefix?
     parser.add_argument(
         "--cache-prefix",
         type=str,
-        default=default_prefix,
-        help=f"Installation prefix (default: {default_prefix})",
+        default=str(DEFAULT_PREFIX_PARENT_PATH),
+        help=f"Installation prefix (default: {DEFAULT_PREFIX_PARENT_PATH})",
     )
-    default_patch_dir = str(Path.home() / ".cache" / "ccbuilder-patches")
+    default_patch_dir = str()
     parser.add_argument(
         "--patches-dir",
         type=str,
-        default=default_patch_dir,
-        help=f"Path to the patches directory (default: {default_patch_dir})",
+        default=str(DEFAULT_PATCH_DIR),
+        help=f"Path to the patches directory (default: {DEFAULT_PATCH_DIR})",
     )
-    default_repos_dir = str(Path.home() / ".cache" / "ccbuilder-repos")
     parser.add_argument(
         "--repos-dir",
         type=str,
-        default=default_repos_dir,
-        help=f"Path to the directory with the compiler repositories (default: {default_repos_dir})",
+        default=str(DEFAULT_REPOS_DIR),
+        help=f"Path to the directory with the compiler repositories (default: {DEFAULT_REPOS_DIR})",
     )
 
     parser.add_argument(
         "--patches",
         nargs="+",
         help="For the 'patcher', this defines which patch(es) to apply. For the 'builder', \
             these are the additional patches to apply to the already existing patches from the PatchDB.",
         type=str,
     )
 
+    parser.add_argument(
+        "--logdir",
+        help="Path to the directory where log files should be stored in. If not specified, ccbuilder will print to stdout.",
+        type=str,
+    )
+
+    parser.add_argument(
+        "--print-releases",
+        action="store_true",
+        default=False,
+        help="Prints the available releases for GCC and LLVM",
+    )
     return parser
 
 
 def ccbuilder_build_parser() -> ArgumentParser:
     parser = ArgumentParser("build", add_help=False)
     parser.add_argument(
         "compiler", choices=["llvm", "gcc"], help="Which compiler to build and install"
     )
     parser.add_argument("revision", type=str, help="Target revision")
+    parser.add_argument(
+        "--additional-configure-flags",
+        type=str,
+        help="Additional flags to pass to configure/cmake",
+    )
     return parser
 
 
 def ccbuilder_patch_parser() -> ArgumentParser:
     parser = ArgumentParser("patch", add_help=False)
     parser.add_argument(
         "compiler", choices=["llvm", "gcc"], help="Which compiler to find patches for"
@@ -164,17 +175,21 @@
     return parser
 
 
 def ccbuilder_cache_parser() -> ArgumentParser:
     parser = ArgumentParser(add_help=False)
     parser.add_argument(
         "action",
-        choices=("clean", "stats"),
+        choices=("clean", "stats", "scan"),
         type=str,
-        help="What you want to do with the cache. Clean will search and remove all unfinished cache entries. `stats` will print some statistics about the cache.",
+        help="What you want to do with the cache. "
+        "Clean will search and remove all unfinished cache entries. "
+        "`stats` will print some statistics about the cache."
+        "`scan` will scan the given directory for compilers and (re-)compute "
+        "the necesary metadata required for retrieving compilers, bisecting, etc.",
     )
     return parser
 
 
 def ccbuilder_parser() -> ArgumentParser:
     """Get the parsers of ccbuilder. Will return you the parent parser
     and the subparser.
@@ -191,30 +206,51 @@
     subparsers.add_parser("cache", parents=[ccbuilder_cache_parser()])
 
     return parser
 
 
 def handle_pull(args: Namespace) -> bool:
     if args.pull:
-        gcc_repo = get_repo(CompilerProject.GCC, Path(args.repos_dir) / "gcc")
-        llvm_repo = get_repo(
-            CompilerProject.LLVM, Path(args.repos_dir) / "llvm-project"
-        )
+        gcc_repo = get_gcc_repo(Path(args.repos_dir) / "gcc")
+        llvm_repo = get_llvm_repo(Path(args.repos_dir) / "llvm-project")
         gcc_repo.pull()
         llvm_repo.pull()
         return True
     return False
 
 
-def handle_build(args: Namespace, bldr: BuilderWithoutCache) -> bool:
+def handle_print_releases(args: Namespace) -> bool:
+    if args.print_releases:
+        print("GCC releases:")
+        for r in get_gcc_releases(get_gcc_repo(Path(args.repos_dir) / "gcc")):
+            print(r)
+
+        print("LLVM releases:")
+        for r in get_llvm_releases(
+            get_llvm_repo(Path(args.repos_dir) / "llvm-project")
+        ):
+            print(r)
+
+        return True
+    return False
+
+
+def handle_build(args: Namespace, bldr: Builder) -> bool:
     # TODO: handle separate repo inputs?
     patches = [Path(p.strip()).absolute() for p in args.patches] if args.patches else []
     if args.command == "build":
         project, _ = get_compiler_info(args.compiler, Path(args.repos_dir))
-        print(bldr.build(project, args.revision.strip(), additional_patches=patches))
+        print(
+            bldr.build(
+                project,
+                args.revision.strip(),
+                additional_patches=patches,
+                configure_flags=args.additional_configure_flags,
+            ).prefix
+        )
         return True
     return False
 
 
 def handle_patch(args: Namespace, bldr: Builder, patchdb: PatchDB) -> bool:
     if args.command == "patch":
         patches = (
@@ -233,76 +269,101 @@
             patcher.find_introducer(project, repo, args.revision.strip())
 
         return True
     return False
 
 
 def handle_cache(args: Namespace, cache_prefix: Path) -> bool:
-    if args.command == "cache":
-        if args.action == "clean":
+    if args.command != "cache":
+        return False
+    match args.action:
+        case "clean":
             print("Cleaning...")
             for c in cache_prefix.iterdir():
                 if c == (cache_prefix / "logs"):
                     continue
                 if not (c / "DONE").exists():
                     try:
                         os.rmdir(c)
                     except FileNotFoundError:
                         print(c, "spooky. It just disappeared...")
                     except OSError:
                         print(c, "is not empty but also not done!")
             print("Done")
-        elif args.action == "stats":
-            count_gcc = 0
-            count_clang = 0
-            for c in cache_prefix.iterdir():
-                if c.name.startswith("llvm"):
-                    count_clang += 1
-                else:
-                    count_gcc += 1
-
+        case "stats":
+            store_filename = default_store_file(cache_prefix)
+            if not store_filename.exists():
+                print(
+                    "No compiler store metadata found. Run `ccbuilder cache scan` first."
+                )
+                exit(0)
+            store = load_compiler_store(store_filename)
+            count_clang = len(store.built_commits(CompilerProject.LLVM))
+            count_gcc = len(store.built_commits(CompilerProject.GCC))
             tot = count_gcc + count_clang
             print("Amount compilers:", tot)
+            print(f"Amount LLVM: {count_clang} {count_clang / tot :.2%}")
+            print(f"Amount GCC: {count_gcc} {count_gcc / tot:.2%}")
+        case "scan":
+            print("Scanning...")
+            store = load_compiler_store(default_store_file(cache_prefix))
+            scan_directory_and_populate_store(cache_prefix, store)
+            print("Done")
             print(
-                "Amount clang: {} {:.2f}%".format(count_clang, count_clang / tot * 100)
+                f"{len(store.built_commits(CompilerProject.GCC))} gcc compilers found"
+            )
+            print(
+                f"{len(store.built_commits(CompilerProject.LLVM))} llvm compilers found"
             )
-            print("Amount GCC: {} {:.2f}%".format(count_gcc, count_gcc / tot * 100))
 
-        return True
-    return False
+    return True
 
 
 def run_as_module() -> None:
     args = ccbuilder_parser().parse_args()
     if args.log_level is not None:
         try:
             num_lvl = getattr(logging, args.log_level.upper())
             logging.basicConfig(level=num_lvl)
         except AttributeError:
             print(f"No such log level {args.log_level.upper()}")
             exit(1)
 
-    _initialize(args)
+    initialize_repos(args.repos_dir)
+    initialize_patches_dir(args.patches_dir)
+
     patchdb = PatchDB(Path(args.patches_dir) / "patchdb.json")
     cache_prefix = Path(args.cache_prefix.strip())
 
+    if handle_print_releases(args):
+        return
     if handle_pull(args):
         return
     if handle_cache(args, cache_prefix):
         return
     repo_dir_prefix = Path(args.repos_dir)
-    llvm_repo = get_repo(CompilerProject.LLVM, repo_dir_prefix / "llvm-project")
-    gcc_repo = get_repo(CompilerProject.LLVM, repo_dir_prefix / "gcc")
+    llvm_repo = get_llvm_repo(repo_dir_prefix / "llvm-project")
+    gcc_repo = get_gcc_repo(repo_dir_prefix / "gcc")
+    store = load_compiler_store(default_store_file(cache_prefix))
+
+    if args.logdir:
+        logdir = Path(args.logdir).absolute()
+        logdir.mkdir(exist_ok=True, parents=True)
+    else:
+        logdir = None
 
     bldr = Builder(
-        Path(args.cache_prefix.strip()),
+        Path(args.cache_prefix.strip()).absolute(),
         gcc_repo=gcc_repo,
         llvm_repo=llvm_repo,
+        cstore=store,
         patchdb=patchdb,
+        logdir=logdir,
         jobs=args.jobs,
     )
+
     if handle_build(args, bldr):
         return
     if handle_patch(args, bldr, patchdb):
         return
     if handle_cache(args, cache_prefix):
         return
```

### Comparing `ccbuilder-0.0.9/ccbuilder/builder/builder.py` & `ccbuilder-0.1.0b0/ccbuilder/builder/builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,107 @@
 import logging
+import json
 import multiprocessing
 import os
+import sys
 import shutil
 import subprocess
 import tempfile
 import time
 from dataclasses import dataclass
 from pathlib import Path
 from types import TracebackType
 from typing import Optional, TextIO
 
+from diopter.repository import Repo, Revision, Commit
+from diopter.compiler import CompilerProject
+
 from ccbuilder.patcher.patchdatabase import PatchDB
-from ccbuilder.utils.repository import Repo, Revision, Commit
+from ccbuilder.compilerstore import CompilerStore, BuiltCompilerInfo
 from ccbuilder.utils.utils import (
-    CompilerProject,
     run_cmd_to_logfile,
     select_repo,
 )
 
 
 class BuildException(Exception):
     pass
 
 
+class DuplicateBuildException(Exception):
+    pass
+
+
+def _worker_alive(worker_indicator: Path) -> bool:
+    if worker_indicator.exists():
+        with open(worker_indicator, "r") as f:
+            worker_pid = int(f.read())
+        try:
+            # Signal to ~check if a process is alive
+            # from man 1 kill
+            # > If signal is 0, then no actual signal is sent, but error checking is still performed.
+            os.kill(worker_pid, 0)
+            return True
+        except OSError:
+            return False
+    return False
+
+
 @dataclass
 class BuildContext:
     """Creates a temporary directory for a build, creates the install prefix
-    and manages the 'communication' between building processes s.t. a compiler is
-    not built twice.
+    and ensures that a compiler is not built twice.
     """
 
     install_prefix: Path
     success_indicator: Path
     project: CompilerProject
     commit_to_build: Commit
-    logdir: Path
+    logdir: Optional[Path]
 
     def __enter__(self) -> tuple[Path, TextIO]:
         self.build_dir = tempfile.mkdtemp()
         os.makedirs(self.install_prefix, exist_ok=True)
+        worker_pid_file = self.install_prefix / "WORKER_PID"
+
+        if worker_pid_file.exists():
+            if _worker_alive(worker_pid_file):
+                raise DuplicateBuildException(
+                    "The compiler is either being built by another process "
+                    "or the cache in a bad state (run ccbuilder cache clean to fix)."
+                )
 
         # Write worker PID
         with open(self.install_prefix / "WORKER_PID", "w") as f:
             f.write(str(os.getpid()))
 
         self.starting_cwd = os.getcwd()
         os.chdir(self.build_dir)
 
-        # Build log file
-        current_time = time.strftime("%Y%m%d-%H%M%S")
-        name = self.project.to_string()
-        build_log_path = (
-            self.logdir / f"{current_time}-{name}-{self.commit_to_build}.log"
-        )
-        self.build_log = open(build_log_path, "a")
-        logging.info(f"Build log at {build_log_path}")
-
-        return (Path(self.build_dir), self.build_log)
+        if self.logdir:
+            # Build log file
+            current_time = time.strftime("%Y%m%d-%H%M%S")
+            name = self.project.to_string()
+            build_log_path = (
+                self.logdir / f"{current_time}-{name}-{self.commit_to_build}.log"
+            )
+            self.build_log = open(build_log_path, "a")
+            logging.info(f"Build log at {build_log_path}")
+            return (Path(self.build_dir), self.build_log)
+        else:
+            return (Path(self.build_dir), sys.stderr)
 
     def __exit__(
         self,
         exc_type: Optional[type[BaseException]],
         exc_value: Optional[BaseException],
         exc_traceback: Optional[TracebackType],
     ) -> None:
-        self.build_log.close()
+        if self.logdir:
+            self.build_log.close()
         shutil.rmtree(self.build_dir)
         os.chdir(self.starting_cwd)
         os.remove(self.install_prefix / "WORKER_PID")
 
         # Build was not successful
         if not self.success_indicator.exists():
             # remove cache entry
@@ -127,77 +160,96 @@
     """
     patches = patchdb.required_patches(commit_to_patch) + additional_patches
     if patches:
         if not apply_patches(working_dir, patches):
             raise BuildException(f"Could not apply patches: {patches}")
 
 
-def llvm_build_and_install(install_prefix: Path, jobs: int, log_file: TextIO) -> None:
+def llvm_build_and_install(
+    install_prefix: Path, jobs: int, log_file: TextIO, configure_flags: str | None
+) -> None:
     """Build and install LLVM. Must only be called in a `BuildContext`.
     May raise a `CalledProcessError`.
 
     Args:
         install_prefix (Path): Install prefix for the build (in the cache).
         jobs (int): Amount of jobs to build with
         log_file (TextIO): File to log the build process to.
+        configure_flags (str | None): additional flags to pass to the configure script or cmake.
 
     Returns:
         None:
     """
     os.chdir("build")
     logging.debug("LLVM: Starting cmake")
-    cmake_cmd = f"cmake ../llvm -G Ninja -DCMAKE_BUILD_TYPE=Release -DLLVM_ENABLE_PROJECTS=clang -DLLVM_INCLUDE_BENCHMARKS=OFF -DLLVM_INCLUDE_TESTS=OFF -DLLVM_USE_NEWPM=ON -DLLVM_TARGETS_TO_BUILD=X86 -DCMAKE_INSTALL_PREFIX={install_prefix} -DLLVM_LINK_LLVM_DYLIB=ON -DLLVM_BUILD_LLVM_DYLIB=ON"
+    cmake_cmd = (
+        "cmake ../llvm -G Ninja -DCMAKE_BUILD_TYPE=Release "
+        "-DLLVM_ENABLE_PROJECTS=clang -DLLVM_INCLUDE_BENCHMARKS=OFF "
+        "-DLLVM_INCLUDE_TESTS=OFF -DLLVM_USE_NEWPM=ON -DLLVM_TARGETS_TO_BUILD=X86 "
+        f"-DCMAKE_INSTALL_PREFIX={install_prefix} -DLLVM_LINK_LLVM_DYLIB=ON -DLLVM_BUILD_LLVM_DYLIB=ON"
+    )
+    if configure_flags:
+        cmake_cmd += " " + configure_flags
 
     run_cmd_to_logfile(
         cmake_cmd, additional_env={"CC": "clang", "CXX": "clang++"}, log_file=log_file
     )
 
     logging.debug("LLVM: Starting to build...")
     run_cmd_to_logfile(f"ninja -j {jobs} install", log_file=log_file)
 
 
-def gcc_build_and_install(install_prefix: Path, jobs: int, log_file: TextIO) -> None:
+def gcc_build_and_install(
+    install_prefix: Path, jobs: int, log_file: TextIO, configure_flags: str | None
+) -> None:
     """Build and install GCC. Must only be called in a `BuildContext`.
     May raise a `CalledProcessError`.
 
     Args:
         install_prefix (Path): Install prefix for the build (in the cache).
         jobs (int): Amount of jobs to build with
         log_file (TextIO): File to log the build process to.
+        configure_flags (str | None): additional flags to pass to the configure script or cmake.
 
     Returns:
         None:
     """
     pre_cmd = "./contrib/download_prerequisites"
     logging.debug("GCC: Starting download_prerequisites")
     run_cmd_to_logfile(pre_cmd, log_file=log_file)
 
     os.chdir("build")
     logging.debug("GCC: Starting configure")
     configure_cmd = (
         "../configure --disable-multilib --disable-bootstrap"
         f" --enable-languages=c,c++ --prefix={install_prefix}"
     )
+    if configure_flags:
+        configure_cmd += " " + configure_flags
     run_cmd_to_logfile(configure_cmd, log_file=log_file)
 
     logging.debug("GCC: Starting to build...")
     run_cmd_to_logfile(f"make -j {jobs}", log_file=log_file)
     run_cmd_to_logfile("make install-strip", log_file=log_file)
 
 
 def _run_build_and_install(
-    project: CompilerProject, install_path: Path, cores: int, log_file: TextIO
+    project: CompilerProject,
+    install_path: Path,
+    cores: int,
+    log_file: TextIO,
+    configure_flags: str | None,
 ) -> Path:
     os.makedirs("build")
     try:
         match project:
             case CompilerProject.GCC:
-                gcc_build_and_install(install_path, cores, log_file)
+                gcc_build_and_install(install_path, cores, log_file, configure_flags)
             case CompilerProject.LLVM:
-                llvm_build_and_install(install_path, cores, log_file)
+                llvm_build_and_install(install_path, cores, log_file, configure_flags)
     except subprocess.CalledProcessError as e:
         raise BuildException(f"Build failed: {e}")
     return install_path
 
 
 def get_install_path(
     cache_prefix: Path, project: CompilerProject, commit: Commit
@@ -218,214 +270,164 @@
         case CompilerProject.LLVM:
             install_name_prefix = "clang"
         case CompilerProject.GCC:
             install_name_prefix = "gcc"
     return cache_prefix / f"{install_name_prefix}-{commit}"
 
 
-def get_executable_postfix(project: CompilerProject) -> Path:
-    match project:
-        case CompilerProject.LLVM:
-            executable_name = "clang"
-        case CompilerProject.GCC:
-            executable_name = "gcc"
-    return Path("bin") / executable_name
-
-
 def build_and_install_compiler(
     project: CompilerProject,
-    rev: Revision,
+    rev: Revision | Commit,
     cache_prefix: Path,
     llvm_repo: Repo,
     gcc_repo: Repo,
     patchdb: PatchDB,
-    get_executable: bool = False,
     jobs: Optional[int] = None,
     additional_patches: Optional[list[Path]] = None,
+    configure_flags: str | None = None,
     logdir: Optional[Path] = None,
 ) -> Path:
     """Build and install a compiler specified via `project` and `rev`.
     Will install to `cache_prefix`/projectname-commit.
 
 
     Args:
         project (CompilerProject): LLVM or GCC.
         rev (Revision): rev
         cache_prefix (Path): cache_prefix
         llvm_repo (Repo): LLVM repository
         gcc_repo (Repo): GCC repository
         patchdb (PatchDB): The PatchDB to use.
-        get_executable (bool): Whether or not to return the path to the executable compiler instead.
         jobs (Optional[int]): Amount of jobs
         additional_patches (Optional[list[Path]]): Additional patches to apply.
+        configure_flags (str | None): additional flags to pass to the configure script or cmake.
         logdir (Optional[Path]): Path to where the build logs are saved.
 
     Returns:
-        Path: `cache_prefix`/projectname-commit or `cache_prefix`/projectname-commit/bin/$compiler if `get_executable` is set.
+        Path: `cache_prefix`/projectname-commit
     """
 
     repo = select_repo(project, llvm_repo, gcc_repo)
     commit = repo.rev_to_commit(rev)
     install_prefix = get_install_path(cache_prefix, project, commit)
     success_indicator = install_prefix / "DONE"
 
-    if not logdir:
-        logdir = cache_prefix / "logs"
-    logdir.mkdir(exist_ok=True, parents=True)
-    with BuildContext(install_prefix, success_indicator, project, commit, logdir) as (
-        tmpdir,
-        build_log,
-    ):
-        run_cmd_to_logfile(
-            f"git -C {str(repo.path)} worktree" f" add {tmpdir} {commit} -f",
-            log_file=build_log,
-        )
-        patch_if_necessary(
-            commit,
-            patchdb,
-            Path(tmpdir),
-            additional_patches if additional_patches else [],
-        )
-        res = _run_build_and_install(
-            project,
-            install_prefix,
-            jobs if jobs else multiprocessing.cpu_count(),
+    if logdir:
+        logdir.mkdir(exist_ok=True, parents=True)
+    try:
+        with BuildContext(
+            install_prefix, success_indicator, project, commit, logdir
+        ) as (
+            tmpdir,
             build_log,
-        )
-        success_indicator.touch()
-        if get_executable:
-            return res / get_executable_postfix(project)
-        return res
+        ):
+            run_cmd_to_logfile(
+                f"git -C {str(repo.path)} worktree" f" add {tmpdir} {commit} -f",
+                log_file=build_log,
+            )
+            patch_if_necessary(
+                commit,
+                patchdb,
+                Path(tmpdir),
+                additional_patches if additional_patches else [],
+            )
+            res = _run_build_and_install(
+                project,
+                install_prefix,
+                jobs if jobs else multiprocessing.cpu_count(),
+                build_log,
+                configure_flags,
+            )
+            success_indicator.touch()
+            with open(success_indicator, "w") as f:
+                json.dump(
+                    {
+                        "revision": rev,
+                        "configure": configure_flags if configure_flags else "",
+                    },
+                    f,
+                )
+    finally:
+        repo.prune_worktree()
+    return res
 
 
-class BuilderWithoutCache:
+class Builder:
     def __init__(
         self,
         cache_prefix: Path,
         gcc_repo: Repo,
         llvm_repo: Repo,
+        cstore: CompilerStore,
         patchdb: Optional[PatchDB] = None,
         jobs: Optional[int] = None,
         logdir: Optional[Path] = None,
     ):
         self.cache_prefix = cache_prefix
         self.gcc_repo = gcc_repo
         self.llvm_repo = llvm_repo
+        self.cstore = cstore
 
         pdb = patchdb if patchdb else PatchDB()
         self.patchdb = pdb
         self.jobs = jobs if jobs else multiprocessing.cpu_count()
         self.logdir = logdir
 
     def build(
         self,
         project: CompilerProject,
-        rev: Revision,
-        get_executable: bool = False,
-        additional_patches: Optional[list[Path]] = None,
-        jobs: Optional[int] = None,
-    ) -> Path:
-        if not jobs and not self.jobs:
-            jobs = multiprocessing.cpu_count()
-        elif not jobs:
-            jobs = self.jobs
-
-        return build_and_install_compiler(
-            project=project,
-            rev=rev,
-            cache_prefix=self.cache_prefix,
-            llvm_repo=self.llvm_repo,
-            gcc_repo=self.gcc_repo,
-            patchdb=self.patchdb,
-            get_executable=get_executable,
-            jobs=jobs,
-            additional_patches=additional_patches,
-            logdir=self.logdir,
-        )
-
-
-def _worker_alive(worker_indicator: Path) -> bool:
-    if worker_indicator.exists():
-        with open(worker_indicator, "r") as f:
-            worker_pid = int(f.read())
-        try:
-            # Signal to ~check if a process is alive
-            # from man 1 kill
-            # > If signal is 0, then no actual signal is sent, but error checking is still performed.
-            os.kill(worker_pid, 0)
-            return True
-        except OSError:
-            return False
-    return False
-
-
-class Builder(BuilderWithoutCache):
-    def build(
-        self,
-        project: CompilerProject,
-        rev: str,
-        get_executable: bool = False,
+        rev: Revision | Commit,
         additional_patches: Optional[list[Path]] = None,
+        configure_flags: str | None = None,
         jobs: Optional[int] = None,
         force: bool = False,
-    ) -> Path:
+    ) -> BuiltCompilerInfo:
         """Build the specified compiler and return the path to the installation location.
         If the specified compiler has already been built, `build` will return the cached path.
 
         Args:
             self:
             project (CompilerProject): Project to build.
             rev (str): Revision of the project to build.
-            get_executable (bool): Whether or not to return the path to the executable compiler instead.
             additional_patches (Optional[list[Path]]): Additional patches to apply.
             jobs (Optional[int]): Amount of jobs to use for the building.
+            configure_flags (str | None): additional flags to pass to the configure script or cmake.
             force (bool): Build the specified compiler even if it has been cached before.
 
         Returns:
-            Path: `cache_prefix`/projectname-commit or `cache_prefix`/projectname-commit/bin/$compiler if `get_executable` is set.
+            Path: `cache_prefix`/projectname-commit
         """
-
         repo = select_repo(project, self.llvm_repo, self.gcc_repo)
-        commit = repo.rev_to_commit(rev)
-        install_path = get_install_path(self.cache_prefix, project, commit)
-        success_indicator = install_path / "DONE"
-        worker_indicator = install_path / "WORKER_PID"
-
-        postfix: Path = get_executable_postfix(project) if get_executable else Path()
-
-        if not force:
-            if success_indicator.exists():
-                return install_path / postfix
-            elif install_path.exists() and _worker_alive(worker_indicator):
+        commit = repo.rev_to_commit(rev.strip())
+        if built_compiler_info := self.cstore.get_built_compiler(project, commit):
+            return built_compiler_info
+        if self.cstore.has_previously_failed_to_build(project, commit) and not force:
+            raise BuildException(
+                f"Compiler {project} {commit} has previously failed to build.\n"
+                "Run with force==True (--force) to try again."
+            )
 
-                logging.info(
-                    f"This compiler seems to be built by some other worker. Need to wait. If there is no other worker, abort this command and run ccbuilder cache clean."
-                )
-                start_time = time.time()
-                counter = 0
-                while (
-                    _worker_alive(worker_indicator)
-                    and not success_indicator.exists()
-                    and install_path.exists()
-                ):
-                    time.sleep(1)
-                    if time.time() - start_time > 15 * 60:
-                        counter += 1
-                        logging.info(
-                            f"{counter*15} minutes have passed waiting. Maybe the cache is in an inconsistent state."
-                        )
-                        start_time = time.time()
-
-                if success_indicator.exists():
-                    return install_path / postfix
-
-                # Someone was building but did not leave the success_indicator
-                # so something went wrong with the build.
-                raise BuildException(f"Other build attempt failed for {install_path}")
-
-        return super().build(
-            project,
-            rev,
-            get_executable=get_executable,
-            additional_patches=additional_patches,
-            jobs=jobs,
-        )
+        if not jobs and not self.jobs:
+            jobs = multiprocessing.cpu_count()
+        elif not jobs:
+            jobs = self.jobs
+
+        try:
+            install_prefix = build_and_install_compiler(
+                project=project,
+                rev=rev,
+                cache_prefix=self.cache_prefix,
+                llvm_repo=self.llvm_repo,
+                gcc_repo=self.gcc_repo,
+                patchdb=self.patchdb,
+                jobs=jobs,
+                additional_patches=additional_patches,
+                configure_flags=configure_flags,
+                logdir=self.logdir,
+            )
+        except BuildException as e:
+            self.cstore.add_failed_to_build_compiler(project, commit)
+            raise e
+
+        compiler_info = BuiltCompilerInfo(project, install_prefix, commit)
+        self.cstore.add_compiler(compiler_info)
+        return compiler_info
```

### Comparing `ccbuilder-0.0.9/ccbuilder/data/patches/gcc-fix-simple-object-decl-and-use-in-gcc-lto.patch` & `ccbuilder-0.1.0b0/ccbuilder/data/patches/gcc-fix-simple-object-decl-and-use-in-gcc-lto.patch`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.9/ccbuilder/data/patches/gcc-libsanitizer.sh` & `ccbuilder-0.1.0b0/ccbuilder/data/patches/gcc-libsanitizer.sh`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.9/ccbuilder/data/patches/gcc-simple-object-declaration.patch` & `ccbuilder-0.1.0b0/ccbuilder/data/patches/gcc-simple-object-declaration.patch`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.9/ccbuilder/data/patches/gcc-ustat.patch` & `ccbuilder-0.1.0b0/ccbuilder/data/patches/gcc-ustat.patch`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.9/ccbuilder/data/patches/llvm-GCOpenMPRuntime.cpp-lambda-issues.patch` & `ccbuilder-0.1.0b0/ccbuilder/data/patches/llvm-GCOpenMPRuntime.cpp-lambda-issues.patch`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.9/ccbuilder/data/patches/llvm-MicrosoftDemangleNodes-missing-includes.patch` & `ccbuilder-0.1.0b0/ccbuilder/data/patches/llvm-MicrosoftDemangleNodes-missing-includes.patch`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.9/ccbuilder/data/patches/llvm-MicrosoftDemangleNodes.h-fix-includes.patch` & `ccbuilder-0.1.0b0/ccbuilder/data/patches/llvm-MicrosoftDemangleNodes.h-fix-includes.patch`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.9/ccbuilder/data/patches/patchdb.json` & `ccbuilder-0.1.0b0/ccbuilder/data/patches/patchdb.json`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.9/ccbuilder/patcher/patchdatabase.py` & `ccbuilder-0.1.0b0/ccbuilder/patcher/patchdatabase.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 
 import json
 import logging
 import os
 from pathlib import Path
 from typing import Any, Callable, TypeVar
 
-from ccbuilder.utils.utils import CompilerProject
+from diopter.compiler import CompilerProject
 
 T = TypeVar("T")
 
 
 def _save_db(func: Callable[..., T]) -> Callable[..., T]:
     def save_decorator(db: PatchDB, *args: list[Any], **kwargs: dict[Any, Any]) -> T:
-
         res = func(db, *args, **kwargs)
         with open(db.path, "w") as f:
             json.dump(db.data, f, indent=4)
         return res
 
     return save_decorator
 
@@ -35,15 +34,17 @@
             if not path_to_db.exists():
                 from shutil import copy
 
                 logging.warning(
                     f"Missing default patch database. Recreating it at {default}..."
                 )
                 os.makedirs(path_to_db.parent, exist_ok=True)
-                for entry in (Path(__file__).parent.parent / "patches").iterdir():
+                for entry in (
+                    Path(__file__).parent.parent / "data" / "patches"
+                ).iterdir():
                     if not (default.parent / entry.name).exists():
                         copy(entry, default.parent / entry.name)
 
         self.path = path_to_db.absolute()
         self.patch_path_prefix = self.path.parent
         self.data: dict[str, Any] = {}
         with open(self.path, "r") as f:
```

### Comparing `ccbuilder-0.0.9/ccbuilder/patcher/patcher.py` & `ccbuilder-0.1.0b0/ccbuilder/patcher/patcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,21 +22,29 @@
 
 import logging
 import math
 from enum import Enum
 from pathlib import Path
 from typing import Optional
 
+from diopter.repository import (
+    Repo,
+    Commit,
+    Revision,
+    get_releases,
+)
+
+from diopter.compiler import CompilerProject
+
+
 from ccbuilder.builder.builder import (
     Builder,
     BuildException,
 )
 from ccbuilder.patcher.patchdatabase import PatchDB
-from ccbuilder.utils.utils import CompilerReleases, CompilerProject
-from ccbuilder.utils.repository import Repo, Commit, Revision
 
 
 class PatchingResult(Enum):
     BuildsWithoutPatching = 1
     BuildsWithPatching = 2
     BuildFailed = 3
 
@@ -47,24 +55,24 @@
         self.patchdb = patchdb
         self.cores = cores
         self.builder = builder
 
     def _build(
         self,
         project: CompilerProject,
-        rev: Revision,
+        rev: Revision | Commit,
         additional_patches: list[Path] = [],
     ) -> None:
         self.builder.build(project, rev=rev, additional_patches=additional_patches)
 
     def _check_building_patches(
         self,
         project: CompilerProject,
         repo: Repo,
-        rev: Revision,
+        rev: Revision | Commit,
         patches: list[Path],
     ) -> PatchingResult:
         if not self.patchdb.requires_all_these_patches(
             repo.rev_to_commit(rev), patches
         ):
             try:
                 logging.info(f"Building {rev} without patches {patches}...")
@@ -91,17 +99,17 @@
 
     def _adjust_bisection_midpoint_after_failure(
         self,
         project: CompilerProject,
         repo: Repo,
         double_fail_counter: int,
         max_double_fail: int,
-        bad: Revision,
-        midpoint: Revision,
-        good: Revision,
+        bad: Commit,
+        midpoint: Commit,
+        good: Commit,
     ) -> Commit:
         """
         Move the midpoint either forwards or backwards (depending on the double_fail_counter)
 
         Returns:
             new midpoint (str)
         """
@@ -132,26 +140,25 @@
         bad_rev: Commit,
         project: CompilerProject,
         repo: Repo,
         patches: list[Path],
         failure_is_good: bool = False,
         max_double_fail: int = 2,
     ) -> tuple[Commit, Commit]:
-
         good = good_rev
         bad = bad_rev
 
         # When building a particular commit and it fails to build
         # without the patches and with the patches, it is considered
         # a double fail.
         double_fail_counter = 0
         encountered_double_fail = False
 
         # Bisection
-        midpoint: str = ""
+        midpoint = Commit("")
         while True:
             if encountered_double_fail:
                 midpoint = self._adjust_bisection_midpoint_after_failure(
                     project,
                     repo,
                     double_fail_counter,
                     max_double_fail,
@@ -208,25 +215,24 @@
         Returns:
             tuple[Optional[Commit], Optional[Commit]]: Common ancestor (w.r.t. releases) that needs no
                 patch and the oldest patchable commit found.
         """
 
         # For now, just assume this is sorted in descending release-recency
         # Using commit dates doesn't really work
-        release_versions = ["trunk"] + CompilerReleases[project]
+        release_versions = ["trunk"] + get_releases(project, repo)
         release_versions.reverse()
 
         tested_ancestors: list[Commit] = []
         no_patch_common_ancestor = None
         oldest_patchable_ancestor = None
         for old_version in release_versions:
-
             logging.info(f"Testing for {old_version}")
             if not repo.is_branch_point_ancestor_wrt_master(
-                old_version, patchable_commit
+                Revision(old_version), Revision(patchable_commit)
             ):
                 if oldest_patchable_ancestor:
                     # XXX: Would something like "All older releases require
                     # patching" make more sense as a warning?
                     logging.warning(
                         f"Found only older releases requiring the patch(es)!"
                     )
@@ -332,15 +338,15 @@
                 repo,
                 patches,
             )
 
             # Insert from introducer to and with patchable_commit as requiring patching
             # This is of course not the complete range but will help when bisecting
             rev_range = f"{introducer}~..{patchable_commit}"
-            commit_list = repo.rev_to_commit_list(rev_range)
+            commit_list = repo.rev_to_commit_list(Revision(rev_range))
             for patch in patches:
                 self.patchdb.save(patch, commit_list, repo)
 
             self.find_fixer_from_introducer_to_releases(
                 introducer=introducer,
                 project=project,
                 repo=repo,
@@ -363,19 +369,19 @@
         patches: list[Path],
     ) -> None:
         logging.info(f"Starting bisection of fixer commits from {introducer}...")
 
         # Find reachable releases
         reachable_releases = [
             repo.rev_to_commit(release)
-            for release in CompilerReleases[project]
+            for release in get_releases(project, repo)
             if repo.is_ancestor(introducer, release)
         ]
 
-        last_needing_patch_list: list[str] = []
+        last_needing_patch_list: list[Commit] = []
         for release in reachable_releases:
             logging.info(f"Searching fixer for release {release}")
 
             patching_result = self._check_building_patches(
                 project, repo, release, patches
             )
 
@@ -396,15 +402,17 @@
                 continue
 
             if patching_result is PatchingResult.BuildFailed:
                 continue
 
             elif patching_result is PatchingResult.BuildsWithPatching:
                 # release only builds with patch, everything to release is to be included
-                commits = repo.rev_to_commit_list(f"{introducer}~1..{release}")
+                commits = repo.rev_to_commit_list(
+                    Revision(f"{introducer}~1..{release}")
+                )
                 for patch in patches:
                     self.patchdb.save(patch, commits, repo)
                 continue
 
             elif patching_result is PatchingResult.BuildsWithoutPatching:
                 # Range A..B is includes B, thus we want B to be the last good one
                 # as good requires the patch
@@ -493,37 +501,39 @@
 
         Returns:
             Commit: introducer commit hash
         """
         logging.info(f"Looking for introducer commit starting at {broken_rev}")
 
         oldest_possible_commit = repo.get_best_common_ancestor(
-            CompilerReleases[project][-1], "main"
+            get_releases(project, repo)[-1], "main"
         )
 
         # === Introducer
         # ====== Search Phase
 
         exp = 0
 
         hit_upper_bound = False
         current_commit = broken_rev
         while True:
             prev_commit = current_commit
-            current_commit = repo.rev_to_commit(broken_rev + f"~{2**exp + 10}")
+            current_commit = Revision(
+                repo.rev_to_commit(broken_rev + f"~{2**exp + 10}")
+            )
             is_ancestor = repo.is_ancestor(oldest_possible_commit, current_commit)
             if hit_upper_bound:
                 msg = (
                     f"Couldn't find buildable ancestor for broken revision {broken_rev}"
                 )
                 logging.critical(msg)
                 raise Exception(msg)
 
             if not is_ancestor and not hit_upper_bound:
-                current_commit = oldest_possible_commit
+                current_commit = Revision(oldest_possible_commit)
                 hit_upper_bound = True
 
             try:
                 logging.info(f"Building {current_commit} in search of buildable one")
                 self._build(project, current_commit)
                 break
             except BuildException as e:
@@ -533,16 +543,16 @@
                 )
 
         # ====== Bisection
         msg = f"Staring bisection between {current_commit} and {prev_commit}, should take at most around {math.log(max(2**exp, 11) - 2**min(exp-1, 0), 2)} steps"
         logging.info(msg)
         print(msg)
         _, introducer = self.bisect_build(
-            good=current_commit,
-            bad=prev_commit,
+            good=Commit(current_commit),
+            bad=Commit(prev_commit),
             project=project,
             repo=repo,
             failure_is_good=False,
         )
         msg = f"Found introducer {introducer}"
         logging.info(msg)
         print(msg)
```

### Comparing `ccbuilder-0.0.9/ccbuilder.egg-info/PKG-INFO` & `ccbuilder-0.1.0b0/ccbuilder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccbuilder
-Version: 0.0.9
+Version: 0.1.0b0
 Summary: A clang/gcc compiler builder and patcher
 Home-page: https://github.com/DeadCodeProductions/ccbuilder
 Author: Theodoros Theodoridis
 Author-email: theodort@inf.ethz.ch
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

### Comparing `ccbuilder-0.0.9/ccbuilder.egg-info/SOURCES.txt` & `ccbuilder-0.1.0b0/ccbuilder.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 ccbuilder/__init__.py
 ccbuilder/__main__.py
+ccbuilder/bisector.py
+ccbuilder/compilerstore.py
+ccbuilder/defaults.py
 ccbuilder/py.typed
 ccbuilder.egg-info/PKG-INFO
 ccbuilder.egg-info/SOURCES.txt
 ccbuilder.egg-info/dependency_links.txt
 ccbuilder.egg-info/entry_points.txt
+ccbuilder.egg-info/requires.txt
 ccbuilder.egg-info/top_level.txt
 ccbuilder/builder/__init__.py
 ccbuilder/builder/builder.py
 ccbuilder/data/patches/gcc-fix-simple-object-decl-and-use-in-gcc-lto.patch
 ccbuilder/data/patches/gcc-libsanitizer.sh
 ccbuilder/data/patches/gcc-simple-object-declaration.patch
 ccbuilder/data/patches/gcc-ustat.patch
@@ -21,9 +25,8 @@
 ccbuilder/data/patches/llvm-MicrosoftDemangleNodes-missing-includes.patch
 ccbuilder/data/patches/llvm-MicrosoftDemangleNodes.h-fix-includes.patch
 ccbuilder/data/patches/patchdb.json
 ccbuilder/patcher/__init__.py
 ccbuilder/patcher/patchdatabase.py
 ccbuilder/patcher/patcher.py
 ccbuilder/utils/__init__.py
-ccbuilder/utils/repository.py
 ccbuilder/utils/utils.py
```

### Comparing `ccbuilder-0.0.9/setup.cfg` & `ccbuilder-0.1.0b0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [metadata]
 name = ccbuilder
-version = 0.0.9
+version = 0.1.0b
 author = Theodoros Theodoridis
 author_email = theodort@inf.ethz.ch
 description = A clang/gcc compiler builder and patcher
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache License 2.0
 url = https://github.com/DeadCodeProductions/ccbuilder
 classifiers = 
 	Programming Language :: Python :: 3
 
 [options]
 packages = find:
 python_requires = >= 3.10
 include_package_data = True
+install_requires = 
+	diopter >= 0.0.23
 
 [options.packages.find]
 include = ccbuilder*
 
 [options.package_data]
 * = *.sh *.patch *.json
```

