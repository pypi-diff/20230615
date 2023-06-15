# Comparing `tmp/pyenv-encrypt-0.1.0.tar.gz` & `tmp/pyenv-encrypt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenv-encrypt-0.1.0.tar", last modified: Thu Jun  8 01:54:31 2023, max compression
+gzip compressed data, was "pyenv-encrypt-0.1.1.tar", last modified: Thu Jun 15 17:14:40 2023, max compression
```

## Comparing `pyenv-encrypt-0.1.0.tar` & `pyenv-encrypt-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:54:31.488946 pyenv-encrypt-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-08 01:54:17.000000 pyenv-encrypt-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-08 01:54:31.488946 pyenv-encrypt-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-08 01:54:17.000000 pyenv-encrypt-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:54:31.484946 pyenv-encrypt-0.1.0/pyenv_enc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:54:17.000000 pyenv-encrypt-0.1.0/pyenv_enc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-06-08 01:54:17.000000 pyenv-encrypt-0.1.0/pyenv_enc/enc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:54:31.488946 pyenv-encrypt-0.1.0/pyenv_encrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-08 01:54:31.000000 pyenv-encrypt-0.1.0/pyenv_encrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-08 01:54:31.000000 pyenv-encrypt-0.1.0/pyenv_encrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 01:54:31.000000 pyenv-encrypt-0.1.0/pyenv_encrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 01:54:31.000000 pyenv-encrypt-0.1.0/pyenv_encrypt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 01:54:31.000000 pyenv-encrypt-0.1.0/pyenv_encrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 01:54:31.000000 pyenv-encrypt-0.1.0/pyenv_encrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-08 01:54:17.000000 pyenv-encrypt-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 01:54:31.488946 pyenv-encrypt-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:14:40.873376 pyenv-encrypt-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-15 17:14:28.000000 pyenv-encrypt-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-15 17:14:40.873376 pyenv-encrypt-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-15 17:14:28.000000 pyenv-encrypt-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:14:40.869377 pyenv-encrypt-0.1.1/pyenv_enc/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 17:14:29.000000 pyenv-encrypt-0.1.1/pyenv_enc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-15 17:14:29.000000 pyenv-encrypt-0.1.1/pyenv_enc/enc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:14:40.873376 pyenv-encrypt-0.1.1/pyenv_encrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-15 17:14:40.000000 pyenv-encrypt-0.1.1/pyenv_encrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-15 17:14:40.000000 pyenv-encrypt-0.1.1/pyenv_encrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 17:14:40.000000 pyenv-encrypt-0.1.1/pyenv_encrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 17:14:40.000000 pyenv-encrypt-0.1.1/pyenv_encrypt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 17:14:40.000000 pyenv-encrypt-0.1.1/pyenv_encrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 17:14:40.000000 pyenv-encrypt-0.1.1/pyenv_encrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-15 17:14:29.000000 pyenv-encrypt-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 17:14:40.873376 pyenv-encrypt-0.1.1/setup.cfg
```

### Comparing `pyenv-encrypt-0.1.0/LICENSE` & `pyenv-encrypt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenv-encrypt-0.1.0/PKG-INFO` & `pyenv-encrypt-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenv-encrypt
-Version: 0.1.0
+Version: 0.1.1
 Summary: GPG based env file encryptor utility.
 Author-email: Akhlak Mahmood <akhlakm@gatech.edu>
 Project-URL: Homepage, https://github.com/akhlakm/pyenv-encrypt
 Project-URL: Bug Tracker, https://github.com/akhlakm/pyenv-encrypt/issues
 Keywords: encryption,development
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyenv-encrypt-0.1.0/README.md` & `pyenv-encrypt-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyenv-encrypt-0.1.0/pyenv_enc/enc.py` & `pyenv-encrypt-0.1.1/pyenv_enc/enc.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,21 +76,21 @@
         print("Error - no public key found:", userid)
         return False
 
 
 def read_file(file: str) -> dict:
     with open(file, 'r') as fp:
         if file.endswith(".yaml") or file.endswith(".yml"):
-            print("Loading YAML file:", file)
+            # print("Loading YAML file:", file)
             return yaml.safe_load(fp)
         elif file.endswith(".json"):
-            print("Loading JSON file:", file)
+            # print("Loading JSON file:", file)
             return json.load(fp)
         else:
-            print("Loading ENV file:", file)
+            # print("Loading ENV file:", file)
             return dotenv_values(stream=fp)
 
 
 def save_file(file: str, data: dict):
     with open(file, 'w+') as fp:
         if file.endswith(".yaml") or file.endswith(".yml"):
             yaml.dump(data, fp, indent=4)
@@ -132,52 +132,58 @@
     value = "-----BEGIN PGP MESSAGE-----\n\n" + value
     value = value + "-----END PGP MESSAGE-----"
     command = f"gpg -d"
     encvalue = exec(command, stdin=value).stdout
     return str(encvalue, encoding="utf-8")
 
 
+def encrypted(value : str) -> bool:
+    return type(value) == str and value.startswith(_MARKUP)
+
+
 def encrypt_data(userid: str, data: dict) -> dict:
     """
     Recursively loop over a dictionary and encrypt all string fields.
     
     """
     for key, value in data.items():
         # encrypt the string values
-        if type(value) == str and not value.startswith(_MARKUP):
+        if not encrypted(value):
             data[key] = gpg_encrypt(userid, value)
         elif type(value) == dict:
             data[key] = encrypt_data(userid, value)
         elif type(value) == list:
             for i in range(len(value)):
-                if type(value[i]) == str and not value[i].startswith(_MARKUP):
+                if not encrypted(value[i]):
                     value[i] = gpg_encrypt(userid, value[i])
             data[key] = value
     return data
 
 
 def decrypt_data(data: dict) -> dict:
     """
     Recursively loop over a dictionary and decrypt all string fields.
     
     """
     for key, value in data.items():
         # decrypt the string values
-        if type(value) == str and value.startswith(_MARKUP):
+        if encrypted(value):
             data[key] = gpg_decrypt(value)
         elif type(value) == dict:
             data[key] = decrypt_data(value)
         elif type(value) == list:
             for i in range(len(value)):
-                if type(value[i]) == str and value[i].startswith(_MARKUP):
+                if encrypted(value[i]):
                     value[i] = gpg_decrypt(value[i])
             data[key] = value
 
     return data
 
+
+
 def main():
     args = parse_arguments()
 
     if args.user is None:
         args.user = os.environ.get('USER', None)
         if args.user is None:
             raise RuntimeError(
```

### Comparing `pyenv-encrypt-0.1.0/pyenv_encrypt.egg-info/PKG-INFO` & `pyenv-encrypt-0.1.1/pyenv_encrypt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenv-encrypt
-Version: 0.1.0
+Version: 0.1.1
 Summary: GPG based env file encryptor utility.
 Author-email: Akhlak Mahmood <akhlakm@gatech.edu>
 Project-URL: Homepage, https://github.com/akhlakm/pyenv-encrypt
 Project-URL: Bug Tracker, https://github.com/akhlakm/pyenv-encrypt/issues
 Keywords: encryption,development
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyenv-encrypt-0.1.0/pyproject.toml` & `pyenv-encrypt-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyenv-encrypt"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     { name="Akhlak Mahmood", email="akhlakm@gatech.edu" },
 ]
 description = "GPG based env file encryptor utility."
 readme = "README.md"
 requires-python = ">=3.0"
```

