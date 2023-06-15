# Comparing `tmp/textureminer-0.0.2.tar.gz` & `tmp/textureminer-1.0.0.tar.gz`

## Comparing `textureminer-0.0.2.tar` & `textureminer-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 textureminer-0.0.2/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 textureminer-0.0.2/src/textureminer/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 textureminer-0.0.2/src/textureminer/__main__.py
--rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 textureminer-0.0.2/src/textureminer/texture_miner.py
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 textureminer-0.0.2/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 textureminer-0.0.2/LICENSE
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 textureminer-0.0.2/README.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 textureminer-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 textureminer-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 textureminer-1.0.0/requirements.txt
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 textureminer-1.0.0/.vscode/tasks.json
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 textureminer-1.0.0/src/textureminer/__init__.py
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 textureminer-1.0.0/src/textureminer/__main__.py
+-rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 textureminer-1.0.0/src/textureminer/bedrock.py
+-rw-r--r--   0        0        0     7721 2020-02-02 00:00:00.000000 textureminer-1.0.0/src/textureminer/common.py
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 textureminer-1.0.0/src/textureminer/java.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 textureminer-1.0.0/src/textureminer/texts.py
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 textureminer-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 textureminer-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 textureminer-1.0.0/README.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 textureminer-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 textureminer-1.0.0/PKG-INFO
```

### Comparing `textureminer-0.0.2/.gitignore` & `textureminer-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `textureminer-0.0.2/LICENSE` & `textureminer-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `textureminer-0.0.2/README.md` & `textureminer-1.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # [texture_miner](https://4mbl.link/gh/texture-miner)
 
-Texture Miner is a Python script that allows you to extract and scale Minecraft's item and block textures. It automates the process of downloading the necessary files and performing the required operations.
+`textureminer` is a Python script that allows you to extract and scale Minecraft's item and block textures. It automates the process of downloading the necessary files and performing the required operations.
 
 ## Table of Contents
 
 * [Table of Contents](#table-of-contents)
 * [Getting Started](#getting-started)
   * [Prerequisites](#prerequisites)
   * [Installation](#installation)
@@ -18,46 +18,55 @@
 Install/update the [pip](https://pip.pypa.io/en/stable/) package manager.
   ```sh
   python3 -m pip install --upgrade pip
   ```
 It's also recommended to use a [virtual environment](https://docs.python.org/3/library/venv.html).
   * Linux / MacOS
     ```bash
-    python3 -m venv venv-name
+    python3 -m venv <venv-name>
     source venv/bin/activate
     ```
   * Windows
     ```bash
-    python3 -m venv venv-name
-    venv\Scripts\activate
+    python3 -m venv <venv-name>
+    <venv-name>/Scripts/activate
     ```
 
 
 ### Installation
 
 Use pip to install `texture_miner`.
 
 ```sh
 python3 -m pip install --upgrade textureminer
 ```
 
-Install the required libraried as listed on [requirements.txt](./requirements.txt).
+Install the required dependencies as listed on [requirements.txt](./requirements.txt).
 
 ```shell
 python3 -m pip install -r requirements.txt
 ```
 
 ## Usage
 
-To download and scale textures for the most recent stable release do the following.
+To download and scale textures for the most recent stable Java release do the following.
 
 ```python
 python3 -m textureminer
 ```
 
+You can also specify the version and edition.
+
+```python
+python3 -m textureminer <version> <edition>
+
+# for example
+python3 -m textureminer 1.20 java
+```
+
 
 At a high level, the script follows the following steps.
 1. Download the client `.jar` file for the specified version from Mojang's servers.
 2. Extract the textures from the `.jar` file.
 3. Filter the extracted files, only leaving item and block textures to the specified output directory (default: `~/Downloads/mc-textures`).
 4. Scale the textures by a specified factor (default: 100).
 5. Merge the block and item textures into a single directory by default.
```

### Comparing `textureminer-0.0.2/pyproject.toml` & `textureminer-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "textureminer"
-version = "0.0.2"
+version = "1.0.0"
 authors = [
   { name="4MBL" },
 ]
 description = "Script that allows you to extract and scale Minecraft's item and block textures."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.11"
```

### Comparing `textureminer-0.0.2/PKG-INFO` & `textureminer-1.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textureminer
-Version: 0.0.2
+Version: 1.0.0
 Summary: Script that allows you to extract and scale Minecraft's item and block textures.
 Project-URL: Homepage, https://github.com/4MBL/texture-miner
 Project-URL: Bug Tracker, https://github.com/4MBL/texture-miner/issues
 Author: 4MBL
 License: MIT License
         
         Copyright (c) 2023 4MBL
@@ -31,15 +31,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # [texture_miner](https://4mbl.link/gh/texture-miner)
 
-Texture Miner is a Python script that allows you to extract and scale Minecraft's item and block textures. It automates the process of downloading the necessary files and performing the required operations.
+`textureminer` is a Python script that allows you to extract and scale Minecraft's item and block textures. It automates the process of downloading the necessary files and performing the required operations.
 
 ## Table of Contents
 
 * [Table of Contents](#table-of-contents)
 * [Getting Started](#getting-started)
   * [Prerequisites](#prerequisites)
   * [Installation](#installation)
@@ -53,46 +53,55 @@
 Install/update the [pip](https://pip.pypa.io/en/stable/) package manager.
   ```sh
   python3 -m pip install --upgrade pip
   ```
 It's also recommended to use a [virtual environment](https://docs.python.org/3/library/venv.html).
   * Linux / MacOS
     ```bash
-    python3 -m venv venv-name
+    python3 -m venv <venv-name>
     source venv/bin/activate
     ```
   * Windows
     ```bash
-    python3 -m venv venv-name
-    venv\Scripts\activate
+    python3 -m venv <venv-name>
+    <venv-name>/Scripts/activate
     ```
 
 
 ### Installation
 
 Use pip to install `texture_miner`.
 
 ```sh
 python3 -m pip install --upgrade textureminer
 ```
 
-Install the required libraried as listed on [requirements.txt](./requirements.txt).
+Install the required dependencies as listed on [requirements.txt](./requirements.txt).
 
 ```shell
 python3 -m pip install -r requirements.txt
 ```
 
 ## Usage
 
-To download and scale textures for the most recent stable release do the following.
+To download and scale textures for the most recent stable Java release do the following.
 
 ```python
 python3 -m textureminer
 ```
 
+You can also specify the version and edition.
+
+```python
+python3 -m textureminer <version> <edition>
+
+# for example
+python3 -m textureminer 1.20 java
+```
+
 
 At a high level, the script follows the following steps.
 1. Download the client `.jar` file for the specified version from Mojang's servers.
 2. Extract the textures from the `.jar` file.
 3. Filter the extracted files, only leaving item and block textures to the specified output directory (default: `~/Downloads/mc-textures`).
 4. Scale the textures by a specified factor (default: 100).
 5. Merge the block and item textures into a single directory by default.
```

