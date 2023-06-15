# Comparing `tmp/llvm-installer-1.3.2.tar.gz` & `tmp/llvm-installer-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llvm-installer-1.3.2.tar", last modified: Thu May 11 18:19:50 2023, max compression
+gzip compressed data, was "llvm-installer-1.3.3.tar", last modified: Thu Jun 15 02:27:19 2023, max compression
```

## Comparing `llvm-installer-1.3.2.tar` & `llvm-installer-1.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-05-11 18:19:50.693847 llvm-installer-1.3.2/
--rw-r--r--   0 mikhail    (503) staff       (20)    11358 2022-05-26 15:06:09.000000 llvm-installer-1.3.2/LICENSE
--rw-r--r--   0 mikhail    (503) staff       (20)      989 2023-05-11 18:19:50.693715 llvm-installer-1.3.2/PKG-INFO
--rw-r--r--   0 mikhail    (503) staff       (20)      643 2022-07-07 03:18:16.000000 llvm-installer-1.3.2/README.md
--rw-r--r--   0 mikhail    (503) staff       (20)       38 2023-05-11 18:19:50.693926 llvm-installer-1.3.2/setup.cfg
--rw-r--r--   0 mikhail    (503) staff       (20)     2235 2023-05-11 18:19:27.000000 llvm-installer-1.3.2/setup.py
-drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-05-11 18:19:50.690242 llvm-installer-1.3.2/src/
-drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-05-11 18:19:50.692015 llvm-installer-1.3.2/src/llvm_installer/
--rw-r--r--   0 mikhail    (503) staff       (20)    11455 2022-08-17 05:24:37.000000 llvm-installer-1.3.2/src/llvm_installer/__init__.py
--rw-r--r--   0 mikhail    (503) staff       (20)     1641 2022-07-07 03:54:15.000000 llvm-installer-1.3.2/src/llvm_installer/__main__.py
--rw-r--r--   0 mikhail    (503) staff       (20)        0 2022-05-26 15:06:09.000000 llvm-installer-1.3.2/src/llvm_installer/py.typed
--rw-r--r--   0 mikhail    (503) staff       (20)    84030 2023-05-11 18:18:08.000000 llvm-installer-1.3.2/src/llvm_installer/release_tags.json
-drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-05-11 18:19:50.693503 llvm-installer-1.3.2/src/llvm_installer.egg-info/
--rw-r--r--   0 mikhail    (503) staff       (20)      989 2023-05-11 18:19:50.000000 llvm-installer-1.3.2/src/llvm_installer.egg-info/PKG-INFO
--rw-r--r--   0 mikhail    (503) staff       (20)      407 2023-05-11 18:19:50.000000 llvm-installer-1.3.2/src/llvm_installer.egg-info/SOURCES.txt
--rw-r--r--   0 mikhail    (503) staff       (20)        1 2023-05-11 18:19:50.000000 llvm-installer-1.3.2/src/llvm_installer.egg-info/dependency_links.txt
--rw-r--r--   0 mikhail    (503) staff       (20)       64 2023-05-11 18:19:50.000000 llvm-installer-1.3.2/src/llvm_installer.egg-info/entry_points.txt
--rw-r--r--   0 mikhail    (503) staff       (20)       86 2023-05-11 18:19:50.000000 llvm-installer-1.3.2/src/llvm_installer.egg-info/requires.txt
--rw-r--r--   0 mikhail    (503) staff       (20)       15 2023-05-11 18:19:50.000000 llvm-installer-1.3.2/src/llvm_installer.egg-info/top_level.txt
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-06-15 02:27:19.228204 llvm-installer-1.3.3/
+-rw-r--r--   0 mikhail    (503) staff       (20)    11358 2022-05-26 15:06:09.000000 llvm-installer-1.3.3/LICENSE
+-rw-r--r--   0 mikhail    (503) staff       (20)      989 2023-06-15 02:27:19.228056 llvm-installer-1.3.3/PKG-INFO
+-rw-r--r--   0 mikhail    (503) staff       (20)      643 2022-07-07 03:18:16.000000 llvm-installer-1.3.3/README.md
+-rw-r--r--   0 mikhail    (503) staff       (20)       38 2023-06-15 02:27:19.228257 llvm-installer-1.3.3/setup.cfg
+-rw-r--r--   0 mikhail    (503) staff       (20)     2235 2023-06-15 02:27:00.000000 llvm-installer-1.3.3/setup.py
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-06-15 02:27:19.225084 llvm-installer-1.3.3/src/
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-06-15 02:27:19.226613 llvm-installer-1.3.3/src/llvm_installer/
+-rw-r--r--   0 mikhail    (503) staff       (20)    11455 2022-08-17 05:24:37.000000 llvm-installer-1.3.3/src/llvm_installer/__init__.py
+-rw-r--r--   0 mikhail    (503) staff       (20)     1641 2022-07-07 03:54:15.000000 llvm-installer-1.3.3/src/llvm_installer/__main__.py
+-rw-r--r--   0 mikhail    (503) staff       (20)        0 2022-05-26 15:06:09.000000 llvm-installer-1.3.3/src/llvm_installer/py.typed
+-rw-r--r--   0 mikhail    (503) staff       (20)    89306 2023-06-15 02:24:50.000000 llvm-installer-1.3.3/src/llvm_installer/release_tags.json
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-06-15 02:27:19.227658 llvm-installer-1.3.3/src/llvm_installer.egg-info/
+-rw-r--r--   0 mikhail    (503) staff       (20)      989 2023-06-15 02:27:19.000000 llvm-installer-1.3.3/src/llvm_installer.egg-info/PKG-INFO
+-rw-r--r--   0 mikhail    (503) staff       (20)      407 2023-06-15 02:27:19.000000 llvm-installer-1.3.3/src/llvm_installer.egg-info/SOURCES.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)        1 2023-06-15 02:27:19.000000 llvm-installer-1.3.3/src/llvm_installer.egg-info/dependency_links.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)       64 2023-06-15 02:27:19.000000 llvm-installer-1.3.3/src/llvm_installer.egg-info/entry_points.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)       86 2023-06-15 02:27:19.000000 llvm-installer-1.3.3/src/llvm_installer.egg-info/requires.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)       15 2023-06-15 02:27:19.000000 llvm-installer-1.3.3/src/llvm_installer.egg-info/top_level.txt
```

### Comparing `llvm-installer-1.3.2/LICENSE` & `llvm-installer-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llvm-installer-1.3.2/PKG-INFO` & `llvm-installer-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llvm-installer
-Version: 1.3.2
+Version: 1.3.3
 Summary: Allows installing pre-built LLVM packages for various operating systems
 Home-page: https://github.com/yugabyte/llvm-installer
 Author: Mikhail Bautin
 Author-email: mbautin@users.noreply.github.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `llvm-installer-1.3.2/README.md` & `llvm-installer-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `llvm-installer-1.3.2/setup.py` & `llvm-installer-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     from os import path
     this_directory = path.abspath(path.dirname(__file__))
     with open(path.join(this_directory, 'README.md'), encoding='utf-8') as readme_file:
         long_description = readme_file.read()
 
     setup(
         name='llvm-installer',
-        version='1.3.2',
+        version='1.3.3',
         url='https://github.com/yugabyte/llvm-installer',
         author='Mikhail Bautin',
         author_email='mbautin@users.noreply.github.com',
         description='Allows installing pre-built LLVM packages for various operating systems',
         packages=find_packages(where='src'),
         package_dir={"": "src"},
         package_data={'llvm_installer': ['py.typed', 'release_tags.json']},
```

### Comparing `llvm-installer-1.3.2/src/llvm_installer/__init__.py` & `llvm-installer-1.3.3/src/llvm_installer/__init__.py`

 * *Files identical despite different names*

### Comparing `llvm-installer-1.3.2/src/llvm_installer/__main__.py` & `llvm-installer-1.3.3/src/llvm_installer/__main__.py`

 * *Files identical despite different names*

### Comparing `llvm-installer-1.3.2/src/llvm_installer/release_tags.json` & `llvm-installer-1.3.3/src/llvm_installer/release_tags.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {"'parsed_tags'": "{insert: [(152, OrderedDict([('architecture', 'aarch64'), "*

 * *                  "('is_old_tag_without_os_and_arch', False), ('major_version', 16), "*

 * *                  "('minor_version', 0), ('patch_version', 5), ('sha1_prefix', '0eb3e9aa'), "*

 * *                  "('short_os_name_and_version', 'almalinux8'), ('tag', "*

 * *                  "'v16.0.5-yb-1-1686611089-0eb3e9aa-almalinux8-aarch64'), ('timestamp', "*

 * *                  "'1686611089'), ('version', '16.0.5'), ('version_suffix', 'yb-1'), "*

 * * […]*

```diff
@@ -2125,14 +2125,28 @@
             "tag": "v16.0.3-yb-1-1683790678-c8b432af-almalinux8-aarch64",
             "timestamp": "1683790678",
             "version": "16.0.3",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "aarch64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 5,
+            "sha1_prefix": "0eb3e9aa",
+            "short_os_name_and_version": "almalinux8",
+            "tag": "v16.0.5-yb-1-1686611089-0eb3e9aa-almalinux8-aarch64",
+            "timestamp": "1686611089",
+            "version": "16.0.5",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "7ea85397",
             "short_os_name_and_version": "almalinux8",
@@ -2185,14 +2199,42 @@
             "yb_suffix_version": 1
         },
         {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
+            "patch_version": 5,
+            "sha1_prefix": "0eb3e9aa",
+            "short_os_name_and_version": "almalinux8",
+            "tag": "v16.0.5-yb-1-1686555214-0eb3e9aa-almalinux8-x86_64",
+            "timestamp": "1686555214",
+            "version": "16.0.5",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
+            "architecture": "aarch64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 5,
+            "sha1_prefix": "0eb3e9aa",
+            "short_os_name_and_version": "almalinux9",
+            "tag": "v16.0.5-yb-1-1686688521-0eb3e9aa-almalinux9-aarch64",
+            "timestamp": "1686688521",
+            "version": "16.0.5",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
             "patch_version": 1,
             "sha1_prefix": "58dbb949",
             "short_os_name_and_version": "almalinux9",
             "tag": "v16.0.1-yb-1-1680849004-58dbb949-almalinux9-x86_64",
             "timestamp": "1680849004",
             "version": "16.0.1",
             "version_suffix": "yb-1",
@@ -2237,14 +2279,28 @@
             "tag": "v16.0.3-yb-1-1683787641-c8b432af-almalinux9-x86_64",
             "timestamp": "1683787641",
             "version": "16.0.3",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 5,
+            "sha1_prefix": "0eb3e9aa",
+            "short_os_name_and_version": "almalinux9",
+            "tag": "v16.0.5-yb-1-1686556777-0eb3e9aa-almalinux9-x86_64",
+            "timestamp": "1686556777",
+            "version": "16.0.5",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "aarch64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "7ea85397",
             "short_os_name_and_version": "centos7",
@@ -2279,14 +2335,28 @@
             "tag": "v16.0.3-yb-1-1683785203-c8b432af-centos7-aarch64",
             "timestamp": "1683785203",
             "version": "16.0.3",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "aarch64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 5,
+            "sha1_prefix": "0eb3e9aa",
+            "short_os_name_and_version": "centos7",
+            "tag": "v16.0.5-yb-1-1686605662-0eb3e9aa-centos7-aarch64",
+            "timestamp": "1686605662",
+            "version": "16.0.5",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "7ea85397",
             "short_os_name_and_version": "centos7",
@@ -2363,14 +2433,28 @@
             "tag": "v16.0.3-yb-1-1683784713-c8b432af-centos7-x86_64",
             "timestamp": "1683784713",
             "version": "16.0.3",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 5,
+            "sha1_prefix": "0eb3e9aa",
+            "short_os_name_and_version": "centos7",
+            "tag": "v16.0.5-yb-1-1686553603-0eb3e9aa-centos7-x86_64",
+            "timestamp": "1686553603",
+            "version": "16.0.5",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "arm64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "7ea85397",
             "short_os_name_and_version": "macos",
@@ -2433,14 +2517,28 @@
             "tag": "v16.0.3-yb-1-1683785495-c8b432af-macos-arm64",
             "timestamp": "1683785495",
             "version": "16.0.3",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "arm64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 5,
+            "sha1_prefix": "0eb3e9aa",
+            "short_os_name_and_version": "macos",
+            "tag": "v16.0.5-yb-1-1686728933-0eb3e9aa-macos-arm64",
+            "timestamp": "1686728933",
+            "version": "16.0.5",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
             "patch_version": 1,
             "sha1_prefix": "58dbb949",
             "short_os_name_and_version": "macos",
@@ -2489,14 +2587,28 @@
             "tag": "v16.0.3-yb-1-1683817162-c8b432af-macos-x86_64",
             "timestamp": "1683817162",
             "version": "16.0.3",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 5,
+            "sha1_prefix": "0eb3e9aa",
+            "short_os_name_and_version": "macos",
+            "tag": "v16.0.5-yb-1-1686772482-0eb3e9aa-macos-x86_64",
+            "timestamp": "1686772482",
+            "version": "16.0.5",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "aarch64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "7ea85397",
             "short_os_name_and_version": "ubuntu20.04",
@@ -2531,14 +2643,28 @@
             "tag": "v16.0.3-yb-1-1683796047-c8b432af-ubuntu20.04-aarch64",
             "timestamp": "1683796047",
             "version": "16.0.3",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "aarch64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 5,
+            "sha1_prefix": "0eb3e9aa",
+            "short_os_name_and_version": "ubuntu20.04",
+            "tag": "v16.0.5-yb-1-1686616372-0eb3e9aa-ubuntu20.04-aarch64",
+            "timestamp": "1686616372",
+            "version": "16.0.5",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "7ea85397",
             "short_os_name_and_version": "ubuntu20.04",
@@ -2587,14 +2713,28 @@
             "tag": "v16.0.3-yb-1-1683789090-c8b432af-ubuntu20.04-x86_64",
             "timestamp": "1683789090",
             "version": "16.0.3",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 5,
+            "sha1_prefix": "0eb3e9aa",
+            "short_os_name_and_version": "ubuntu20.04",
+            "tag": "v16.0.5-yb-1-1686558353-0eb3e9aa-ubuntu20.04-x86_64",
+            "timestamp": "1686558353",
+            "version": "16.0.5",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "aarch64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "7ea85397",
             "short_os_name_and_version": "ubuntu22.04",
@@ -2629,14 +2769,28 @@
             "tag": "v16.0.3-yb-1-1683801442-c8b432af-ubuntu22.04-aarch64",
             "timestamp": "1683801442",
             "version": "16.0.3",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "aarch64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 5,
+            "sha1_prefix": "0eb3e9aa",
+            "short_os_name_and_version": "ubuntu22.04",
+            "tag": "v16.0.5-yb-1-1686621781-0eb3e9aa-ubuntu22.04-aarch64",
+            "timestamp": "1686621781",
+            "version": "16.0.5",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "7ea85397",
             "short_os_name_and_version": "ubuntu22.04",
@@ -2683,10 +2837,24 @@
             "sha1_prefix": "c8b432af",
             "short_os_name_and_version": "ubuntu22.04",
             "tag": "v16.0.3-yb-1-1683790564-c8b432af-ubuntu22.04-x86_64",
             "timestamp": "1683790564",
             "version": "16.0.3",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
+        },
+        {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 5,
+            "sha1_prefix": "0eb3e9aa",
+            "short_os_name_and_version": "ubuntu22.04",
+            "tag": "v16.0.5-yb-1-1686559964-0eb3e9aa-ubuntu22.04-x86_64",
+            "timestamp": "1686559964",
+            "version": "16.0.5",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
         }
     ]
 }
```

### Comparing `llvm-installer-1.3.2/src/llvm_installer.egg-info/PKG-INFO` & `llvm-installer-1.3.3/src/llvm_installer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llvm-installer
-Version: 1.3.2
+Version: 1.3.3
 Summary: Allows installing pre-built LLVM packages for various operating systems
 Home-page: https://github.com/yugabyte/llvm-installer
 Author: Mikhail Bautin
 Author-email: mbautin@users.noreply.github.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

