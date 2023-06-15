# Comparing `tmp/boli_orbital_api-0.9b14.tar.gz` & `tmp/boli_orbital_api-0.9b15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boli_orbital_api-0.9b14.tar", max compression
+gzip compressed data, was "boli_orbital_api-0.9b15.tar", max compression
```

## Comparing `boli_orbital_api-0.9b14.tar` & `boli_orbital_api-0.9b15.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     6425 2023-06-07 13:34:10.219390 boli_orbital_api-0.9b14/.gitignore
--rw-r--r--   0        0        0      541 2023-06-05 19:49:57.553690 boli_orbital_api-0.9b14/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-06-05 20:23:02.778565 boli_orbital_api-0.9b14/LICENSE
--rw-r--r--   0        0        0     2772 2023-06-03 22:55:11.905218 boli_orbital_api-0.9b14/README.md
--rw-r--r--   0        0        0     2922 2023-06-03 22:55:11.858554 boli_orbital_api-0.9b14/README_ES.md
--rw-r--r--   0        0        0     1305 2023-06-05 20:18:34.246061 boli_orbital_api-0.9b14/TODO.md
--rw-r--r--   0        0        0       42 2023-06-07 13:32:45.641287 boli_orbital_api-0.9b14/boli_orbital_api/__init__.py
--rw-r--r--   0        0        0     2724 2023-06-09 18:45:51.900962 boli_orbital_api-0.9b14/boli_orbital_api/logger.py
--rw-r--r--   0        0        0    62361 2023-06-09 18:45:51.784297 boli_orbital_api-0.9b14/boli_orbital_api/rpc.py
--rw-r--r--   0        0        0       14 2023-06-02 00:43:19.185603 boli_orbital_api-0.9b14/docs/using.md
--rw-r--r--   0        0        0     1255 2023-06-09 18:45:51.830963 boli_orbital_api-0.9b14/pyproject.toml
--rw-r--r--   0        0        0       16 2023-06-01 22:31:09.954549 boli_orbital_api-0.9b14/requirements.txt
--rw-r--r--   0        0        0      100 2023-06-09 18:43:19.823212 boli_orbital_api-0.9b14/requirements_freezed.txt
--rw-r--r--   0        0        0        0 2023-05-31 19:36:48.526207 boli_orbital_api-0.9b14/tests/__init__.py
--rw-r--r--   0        0        0      409 2023-06-05 19:41:08.195877 boli_orbital_api-0.9b14/tests/test.py
--rw-r--r--   0        0        0     3793 1970-01-01 00:00:00.000000 boli_orbital_api-0.9b14/PKG-INFO
+-rw-r--r--   0        0        0     6425 2023-06-07 13:34:10.219390 boli_orbital_api-0.9b15/.gitignore
+-rw-r--r--   0        0        0      649 2023-06-15 18:04:16.375821 boli_orbital_api-0.9b15/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-06-05 20:23:02.778565 boli_orbital_api-0.9b15/LICENSE
+-rw-r--r--   0        0        0     2772 2023-06-03 22:55:11.905218 boli_orbital_api-0.9b15/README.md
+-rw-r--r--   0        0        0     2922 2023-06-03 22:55:11.858554 boli_orbital_api-0.9b15/README_ES.md
+-rw-r--r--   0        0        0     1305 2023-06-05 20:18:34.246061 boli_orbital_api-0.9b15/TODO.md
+-rw-r--r--   0        0        0       42 2023-06-07 13:32:45.641287 boli_orbital_api-0.9b15/boli_orbital_api/__init__.py
+-rw-r--r--   0        0        0     2724 2023-06-09 18:45:51.900962 boli_orbital_api-0.9b15/boli_orbital_api/logger.py
+-rw-r--r--   0        0        0    62629 2023-06-15 17:47:08.136008 boli_orbital_api-0.9b15/boli_orbital_api/rpc.py
+-rw-r--r--   0        0        0       14 2023-06-02 00:43:19.185603 boli_orbital_api-0.9b15/docs/using.md
+-rw-r--r--   0        0        0     1255 2023-06-15 16:37:07.716044 boli_orbital_api-0.9b15/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-06-01 22:31:09.954549 boli_orbital_api-0.9b15/requirements.txt
+-rw-r--r--   0        0        0      100 2023-06-09 18:43:19.823212 boli_orbital_api-0.9b15/requirements_freezed.txt
+-rw-r--r--   0        0        0        0 2023-05-31 19:36:48.526207 boli_orbital_api-0.9b15/tests/__init__.py
+-rw-r--r--   0        0        0      409 2023-06-05 19:41:08.195877 boli_orbital_api-0.9b15/tests/test.py
+-rw-r--r--   0        0        0     3793 1970-01-01 00:00:00.000000 boli_orbital_api-0.9b15/PKG-INFO
```

### Comparing `boli_orbital_api-0.9b14/.gitignore` & `boli_orbital_api-0.9b15/.gitignore`

 * *Files identical despite different names*

### Comparing `boli_orbital_api-0.9b14/CHANGELOG.md` & `boli_orbital_api-0.9b15/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [0.9b13] - 2023-06-23
+## [0.9b15] - 2023-06-15
+Public beta release 15.
+Added binary data from raw_call, and masternode_list_conf
+
+## [0.9b13] - 2023-06-05
 Public beta release 13
 
-## [0.9b2] - 2023-06-21
+## [0.9b2] - 2023-06-01
 Private beta release 2
 
 ## [0.0.1] - 2021-03-08
 
 - Bolivarcoin DAO
   Proposal: [Propuesta DAO a superbloque 764,336 para desarrollo API y APPs periféricas alrededor del núcleo](https://bit.ly/Superbloque764336)
```

### Comparing `boli_orbital_api-0.9b14/LICENSE` & `boli_orbital_api-0.9b15/LICENSE`

 * *Files identical despite different names*

### Comparing `boli_orbital_api-0.9b14/README.md` & `boli_orbital_api-0.9b15/README.md`

 * *Files identical despite different names*

### Comparing `boli_orbital_api-0.9b14/README_ES.md` & `boli_orbital_api-0.9b15/README_ES.md`

 * *Files identical despite different names*

### Comparing `boli_orbital_api-0.9b14/TODO.md` & `boli_orbital_api-0.9b15/TODO.md`

 * *Files identical despite different names*

### Comparing `boli_orbital_api-0.9b14/boli_orbital_api/logger.py` & `boli_orbital_api-0.9b15/boli_orbital_api/logger.py`

 * *Files identical despite different names*

### Comparing `boli_orbital_api-0.9b14/boli_orbital_api/rpc.py` & `boli_orbital_api-0.9b15/boli_orbital_api/rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         BOLICOIN COMPATIBLE VERSION: v2.0.0.2-g
         Bolicoin/Bolivarcoin platform and cryptocurrency from http://bolis.info
 
     __author__: "Asdrúbal Velásquez Lagrave - Twitter/Telegram: @Visionario"
     __copyright__: "2018-2023"
     __credits__: [""]
     __license__: "MIT"
-    __version__: 0.9b14
+    __version__: 0.9b15
     __maintainer__: "Asdrúbal Velásquez Lagrave"
     __email__: "hello@orbital.center"
     __status__: "BETA"
     __app_name__: "Node API Rpc main class for Bolivarcoin/Bolicoin blockchain (Layer 1)",
     __url__: "https://orbital.center"
 
 """
@@ -29,15 +29,15 @@
     "GobjectListTypes",
     "MasternodeCountOptions",
     "MasternodeStartModes",
     "About",
     "VERSION",
 ]
 
-VERSION = "0.9b14"
+VERSION = "0.9b15"
 
 # LOGGER
 logger = setup_logger(__name__)
 
 
 class GobjectListSignals:
     """See gobject_list()"""
@@ -746,15 +746,15 @@
         return _process_result(self.raw_call("masternode", params=['winners']))
 
     def masternode_list_conf(self) -> dict:
         """
         Print masternode.conf in JSON format
         masternode list-conf
         """
-        return _process_result(self.raw_call("masternode", params=['list-conf']))
+        return _process_result(self.raw_call("masternode", params=['list-conf'], return_binary=True))
 
     def masternode_start_alias(self, alias) -> dict:
         """
         Start single remote masternode by assigned alias configured in masternode.conf
 
         masternode start-alias alias
 
@@ -1166,27 +1166,33 @@
         logger.debug("Connecting node...")
         self._check_online_status()
 
     def raw_call(
             self,
             method: str,
             params=None,
+            return_binary=False
     ) -> Any:
         """ Rpc communication raw_call main method
 
         It will return:
-        # OK
+        # OK JSON
         {"result": response.json()['result'], 'errors': None} When OK
 
+        # OK BINARY
+        {"result": response.content, 'errors': None} When OK
+
         # Server responds but NOT OK
         {"result": response.json()['result'], 'errors': None} When server responds but error in command or sintaxis
 
         # NO connect or communication fail
         {"result": response, 'errors': f'{e}'}
 
+        return_binary: Some methods prefer use binary version instead JSON
+
         """
 
         self._data["params"] = [] if params is None else params
 
         self._data["method"] = method
 
         logger.debug(f"raw_call: method:{method} params:{params}")
@@ -1197,19 +1203,20 @@
             response = post(
                 url=f'{self.scheme}://{self.server_ip}:{self.rpc_port}/',
                 headers=self._headers,
                 data=dumps(self._data),
                 auth=(self.rpc_user, self.rpc_password)
             )
 
-            # print("raw_call_result", response.status_code, response.json())
-
             if response.status_code == 200:
                 self._valid_node = True
-                return {"result": response.json()['result'], 'errors': None}
+                if return_binary:
+                    return {"result": response.content, 'errors': None}
+                else:
+                    return {"result": response.json()['result'], 'errors': None}
 
             else:
                 self._valid_node = False
                 return {"result": response.json()['result'], 'errors': response.json()['error']}
 
 
         except request_exceptions.RequestException as e:
```

### Comparing `boli_orbital_api-0.9b14/pyproject.toml` & `boli_orbital_api-0.9b15/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "boli_orbital_api"
-version = "0.9b14"
+version = "0.9b15"
 description = "Orbital API RPC for Bolivarcoin/Bolicoin blockchain"
 authors = ["Asdrubal Velasquez Lagrave <hello@orbital.center>"]
 maintainers = ["Asdrubal Velasquez Lagrave <hello@orbital.center>"]
 repository = "https://github.com/Visionario/BoliOrbitalAPI"
 homepage = "https://orbital.center"
 keywords = ["bolicoin", "bolivarcoin", "criptocurrency", "blockchain", "api"]
 classifiers = [
```

### Comparing `boli_orbital_api-0.9b14/PKG-INFO` & `boli_orbital_api-0.9b15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boli-orbital-api
-Version: 0.9b14
+Version: 0.9b15
 Summary: Orbital API RPC for Bolivarcoin/Bolicoin blockchain
 Home-page: https://orbital.center
 License: MIT
 Keywords: bolicoin,bolivarcoin,criptocurrency,blockchain,api
 Author: Asdrubal Velasquez Lagrave
 Author-email: hello@orbital.center
 Maintainer: Asdrubal Velasquez Lagrave
```

