# Comparing `tmp/neon-skill-communication-0.1.1a1.tar.gz` & `tmp/neon-skill-communication-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-communication-0.1.1a1.tar", last modified: Thu Jun 15 20:52:23 2023, max compression
+gzip compressed data, was "neon-skill-communication-0.1.1a2.tar", last modified: Thu Jun 15 21:11:18 2023, max compression
```

## Comparing `neon-skill-communication-0.1.1a1.tar` & `neon-skill-communication-0.1.1a2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:22.997925 neon-skill-communication-0.1.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 20:52:17.000000 neon-skill-communication-0.1.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-15 20:52:22.997925 neon-skill-communication-0.1.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-15 20:52:17.000000 neon-skill-communication-0.1.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13462 2023-06-15 20:52:17.000000 neon-skill-communication-0.1.1a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:22.993925 neon-skill-communication-0.1.1a1/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:22.993925 neon-skill-communication-0.1.1a1/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:22.993925 neon-skill-communication-0.1.1a1/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 20:52:17.000000 neon-skill-communication-0.1.1a1/locale/en-us/dialog/cant_call.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 20:52:17.000000 neon-skill-communication-0.1.1a1/locale/en-us/dialog/cant_send.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-15 20:52:17.000000 neon-skill-communication-0.1.1a1/locale/en-us/dialog/one_moment.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:22.993925 neon-skill-communication-0.1.1a1/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-15 20:52:17.000000 neon-skill-communication-0.1.1a1/locale/en-us/vocab/call.intent
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 20:52:17.000000 neon-skill-communication-0.1.1a1/locale/en-us/vocab/draft.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 20:52:17.000000 neon-skill-communication-0.1.1a1/locale/en-us/vocab/message.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 20:52:17.000000 neon-skill-communication-0.1.1a1/locale/en-us/vocab/neon.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:22.997925 neon-skill-communication-0.1.1a1/neon_skill_communication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-15 20:52:22.000000 neon-skill-communication-0.1.1a1/neon_skill_communication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-15 20:52:22.000000 neon-skill-communication-0.1.1a1/neon_skill_communication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 20:52:22.000000 neon-skill-communication-0.1.1a1/neon_skill_communication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-15 20:52:22.000000 neon-skill-communication-0.1.1a1/neon_skill_communication.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 20:52:22.000000 neon-skill-communication-0.1.1a1/neon_skill_communication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 20:52:22.000000 neon-skill-communication-0.1.1a1/neon_skill_communication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 20:52:22.997925 neon-skill-communication-0.1.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-15 20:52:17.000000 neon-skill-communication-0.1.1a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-15 20:52:17.000000 neon-skill-communication-0.1.1a1/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:22.997925 neon-skill-communication-0.1.1a1/test/
--rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-06-15 20:52:17.000000 neon-skill-communication-0.1.1a1/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 20:52:17.000000 neon-skill-communication-0.1.1a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:11:18.361865 neon-skill-communication-0.1.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 21:11:14.000000 neon-skill-communication-0.1.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-15 21:11:18.361865 neon-skill-communication-0.1.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-15 21:11:14.000000 neon-skill-communication-0.1.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13462 2023-06-15 21:11:14.000000 neon-skill-communication-0.1.1a2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:11:18.361865 neon-skill-communication-0.1.1a2/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:11:18.361865 neon-skill-communication-0.1.1a2/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:11:18.361865 neon-skill-communication-0.1.1a2/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 21:11:14.000000 neon-skill-communication-0.1.1a2/locale/en-us/dialog/cant_call.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 21:11:14.000000 neon-skill-communication-0.1.1a2/locale/en-us/dialog/cant_send.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-15 21:11:14.000000 neon-skill-communication-0.1.1a2/locale/en-us/dialog/one_moment.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:11:18.361865 neon-skill-communication-0.1.1a2/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-15 21:11:14.000000 neon-skill-communication-0.1.1a2/locale/en-us/vocab/call.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 21:11:14.000000 neon-skill-communication-0.1.1a2/locale/en-us/vocab/draft.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 21:11:14.000000 neon-skill-communication-0.1.1a2/locale/en-us/vocab/message.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 21:11:14.000000 neon-skill-communication-0.1.1a2/locale/en-us/vocab/neon.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:11:18.361865 neon-skill-communication-0.1.1a2/neon_skill_communication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-15 21:11:18.000000 neon-skill-communication-0.1.1a2/neon_skill_communication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-15 21:11:18.000000 neon-skill-communication-0.1.1a2/neon_skill_communication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:11:18.000000 neon-skill-communication-0.1.1a2/neon_skill_communication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-15 21:11:18.000000 neon-skill-communication-0.1.1a2/neon_skill_communication.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 21:11:18.000000 neon-skill-communication-0.1.1a2/neon_skill_communication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 21:11:18.000000 neon-skill-communication-0.1.1a2/neon_skill_communication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 21:11:18.361865 neon-skill-communication-0.1.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-15 21:11:14.000000 neon-skill-communication-0.1.1a2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-15 21:11:14.000000 neon-skill-communication-0.1.1a2/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:11:18.361865 neon-skill-communication-0.1.1a2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-06-15 21:11:14.000000 neon-skill-communication-0.1.1a2/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 21:11:14.000000 neon-skill-communication-0.1.1a2/version.py
```

### Comparing `neon-skill-communication-0.1.1a1/LICENSE.md` & `neon-skill-communication-0.1.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-communication-0.1.1a1/PKG-INFO` & `neon-skill-communication-0.1.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-communication
-Version: 0.1.1a1
+Version: 0.1.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-communication
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-communication-0.1.1a1/README.md` & `neon-skill-communication-0.1.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-communication-0.1.1a1/__init__.py` & `neon-skill-communication-0.1.1a2/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-communication-0.1.1a1/neon_skill_communication.egg-info/PKG-INFO` & `neon-skill-communication-0.1.1a2/neon_skill_communication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-communication
-Version: 0.1.1a1
+Version: 0.1.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-communication
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-communication-0.1.1a1/neon_skill_communication.egg-info/SOURCES.txt` & `neon-skill-communication-0.1.1a2/neon_skill_communication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-communication-0.1.1a1/setup.py` & `neon-skill-communication-0.1.1a2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 from setuptools import setup
 from os import getenv, path, walk
 
 SKILL_NAME = "skill-communication"
 SKILL_PKG = SKILL_NAME.replace('-', '_')
 # skill_id=package_name:SkillClass
 PLUGIN_ENTRY_POINT = f'{SKILL_NAME}.neongeckocom={SKILL_PKG}:CommunicationSkill'
+BASE_PATH = path.abspath(path.dirname(__file__))
 
 
 def get_requirements(requirements_filename: str):
-    requirements_file = path.join(path.abspath(path.dirname(__file__)),
-                                  requirements_filename)
+    requirements_file = path.join(BASE_PATH, requirements_filename)
     with open(requirements_file, 'r', encoding='utf-8') as r:
         requirements = r.readlines()
     requirements = [r.strip() for r in requirements if r.strip()
                     and not r.strip().startswith("#")]
 
     for i in range(0, len(requirements)):
         r = requirements[i]
@@ -55,31 +55,31 @@
                     r.replace("github.com",
                               f"{getenv('GITHUB_TOKEN')}@github.com")
     return requirements
 
 
 def find_resource_files():
     resource_base_dirs = ("locale", "ui", "vocab", "dialog", "regex")
-    base_dir = path.dirname(__file__)
+    base_dir = BASE_PATH
     package_data = ["skill.json"]
     for res in resource_base_dirs:
         if path.isdir(path.join(base_dir, res)):
             for (directory, _, files) in walk(path.join(base_dir, res)):
                 if files:
                     package_data.append(
                         path.join(directory.replace(base_dir, "").lstrip('/'),
                                   '*'))
 #    print(package_data)
     return package_data
 
 
-with open("README.md", "r") as f:
+with open(path.join(BASE_PATH, "README.md"), "r") as f:
     long_description = f.read()
 
-with open("./version.py", "r", encoding="utf-8") as v:
+with open(path.join(BASE_PATH, "version.py"), "r", encoding="utf-8") as v:
     for line in v.readlines():
         if line.startswith("__version__"):
             if '"' in line:
                 version = line.split('"')[1]
             else:
                 version = line.split("'")[1]
```

### Comparing `neon-skill-communication-0.1.1a1/skill.json` & `neon-skill-communication-0.1.1a2/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-communication-0.1.1a1/test/test_skill.py` & `neon-skill-communication-0.1.1a2/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-communication-0.1.1a1/version.py` & `neon-skill-communication-0.1.1a2/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.1.1a1"
+__version__ = "0.1.1a2"
```

