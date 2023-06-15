# Comparing `tmp/vantage6-common-3.9.0rc2.tar.gz` & `tmp/vantage6-common-3.9.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-common-3.9.0rc2.tar", last modified: Tue May  9 13:37:04 2023, max compression
+gzip compressed data, was "vantage6-common-3.9.0rc4.tar", last modified: Wed May 24 09:34:08 2023, max compression
```

## Comparing `vantage6-common-3.9.0rc2.tar` & `vantage6-common-3.9.0rc4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.050815 vantage6-common-3.9.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-09 13:37:04.050815 vantage6-common-3.9.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 13:37:04.050815 vantage6-common-3.9.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.050815 vantage6-common-3.9.0rc2/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.050815 vantage6-common-3.9.0rc2/vantage6/common/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/__build__
--rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    17964 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.050815 vantage6-common-3.9.0rc2/vantage6/common/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/docker/addons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/docker/network_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/task_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/utest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.050815 vantage6-common-3.9.0rc2/vantage6_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-09 13:37:04.000000 vantage6-common-3.9.0rc2/vantage6_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-09 13:37:04.000000 vantage6-common-3.9.0rc2/vantage6_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:37:04.000000 vantage6-common-3.9.0rc2/vantage6_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-09 13:37:04.000000 vantage6-common-3.9.0rc2/vantage6_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 13:37:04.000000 vantage6-common-3.9.0rc2/vantage6_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:08.497724 vantage6-common-3.9.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-24 09:34:08.497724 vantage6-common-3.9.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:34:08.497724 vantage6-common-3.9.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:08.497724 vantage6-common-3.9.0rc4/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:08.497724 vantage6-common-3.9.0rc4/vantage6/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:08.497724 vantage6-common-3.9.0rc4/vantage6/common/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/docker/addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/docker/network_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/task_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/utest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:08.497724 vantage6-common-3.9.0rc4/vantage6_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-24 09:34:08.000000 vantage6-common-3.9.0rc4/vantage6_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-24 09:34:08.000000 vantage6-common-3.9.0rc4/vantage6_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:34:08.000000 vantage6-common-3.9.0rc4/vantage6_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-24 09:34:08.000000 vantage6-common-3.9.0rc4/vantage6_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 09:34:08.000000 vantage6-common-3.9.0rc4/vantage6_common.egg-info/top_level.txt
```

### Comparing `vantage6-common-3.9.0rc2/PKG-INFO` & `vantage6-common-3.9.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-common
-Version: 3.9.0rc2
+Version: 3.9.0rc4
 Summary: Vantage6 common
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-common Version: 3.9.0rc2 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-common Version: 3.9.0rc4 Summary: Vantage6
 common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-common-3.9.0rc2/setup.py` & `vantage6-common-3.9.0rc4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     packages=find_namespace_packages(),
     python_requires='>=3.6',
     install_requires=[
         'appdirs==1.4.4',
         'click==8.1.3',
         'colorama==0.4.6',
         'cryptography==39.0.1',
-        'docker==6.0.1',
+        'docker==6.1.2',
         'pyfiglet==0.8.post1',
         'PyYAML==6.0',
         'python-dateutil==2.8.2',
         'schema==0.7.5',
     ],
     package_data={
         'vantage6.common': [
```

### Comparing `vantage6-common-3.9.0rc2/vantage6/common/__init__.py` & `vantage6-common-3.9.0rc4/vantage6/common/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     """
     return base64.b64decode(bytes_string.encode(STRING_ENCODING))
 
 
 #
 # CLI prints
 #
-def echo(msg: str, level="info") -> None:
+def echo(msg: str, level: str = "info") -> None:
     """
     Print a message to the CLI.
 
     Parameters
     ----------
     msg: str
         The message to print.
```

### Comparing `vantage6-common-3.9.0rc2/vantage6/common/_version.py` & `vantage6-common-3.9.0rc4/vantage6/common/_version.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.9.0rc2/vantage6/common/colors.py` & `vantage6-common-3.9.0rc4/vantage6/common/colors.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.9.0rc2/vantage6/common/configuration_manager.py` & `vantage6-common-3.9.0rc4/vantage6/common/configuration_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from typing import Any, Type
+from __future__ import annotations
 import yaml
 import collections
 
+from typing import Any, Type
 from pathlib import Path
 from schema import Schema
 
 
 class Configuration(collections.UserDict):
     """Base class to contain a single configuration."""
 
@@ -270,15 +271,15 @@
 
         for env in self.ENVS:
             self.put(env, self._get_environment_from_dict(config, env))
 
     @classmethod
     def from_file(
         cls, path: Path | str, conf_class: Type[Configuration] = Configuration
-    ) -> 'ConfigurationManager':
+    ) -> ConfigurationManager:
         """
         Load a configuration from a file.
 
         Parameters
         ----------
         path: Path | str
             The path to the file to load the configuration from.
```

### Comparing `vantage6-common-3.9.0rc2/vantage6/common/context.py` & `vantage6-common-3.9.0rc4/vantage6/common/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import sys
 import appdirs
 import logging
 import logging.handlers
 
 from pathlib import Path
+from typing import Tuple
 
 from vantage6.common import Singleton, error, Fore, Style, logger_name
 from vantage6.common.colors import ColorStreamHandler
 from vantage6.common.globals import DEFAULT_ENVIRONMENT, APPNAME
 from vantage6.common.configuration_manager import (
     ConfigurationManager
 )
@@ -137,14 +138,15 @@
 
         self_ = cls.__new__(cls)
         self_.name = instance_name
         self_.scope = "system" if system_folders else "user"
         self_.config_dir = Path(path).parent
         self_.config_file = path
         self_.environment = environment
+        self_.instance_type = instance_type
         self_.set_folders(instance_type, instance_name, system_folders)
         module_name = logger_name(__name__)
         self_.log = logging.getLogger(module_name)
         if self_.LOGGING_ENABLED:
             self_.setup_logging()
 
         return self_
@@ -376,15 +378,15 @@
         -------
         str
             Environment
         """
         return self.__environment
 
     @environment.setter
-    def environment(self, env) -> None:
+    def environment(self, env: str) -> None:
         """
         Set the environment.
 
         Parameters
         ----------
         env: str
             Environment
@@ -527,24 +529,22 @@
 
         Exits if the log file can't be created.
         """
         # TODO BvB 2023-03-31: would be nice to refactor this with the other
         # loggers in vantage6.common.log
         log_config = self.config["logging"]
 
-        level = getattr(logging, log_config["level"].upper())
         format_ = log_config["format"]
         datefmt = log_config.get("datefmt", "")
 
         # make sure the log-file exists
         os.makedirs(os.path.dirname(self.log_file), exist_ok=True)
 
         # Create the root logger
-        logger = logging.getLogger()
-        logger.setLevel(level)
+        logger, level = self.configure_logger(None, log_config["level"])
 
         # Create RotatingFileHandler
         try:
             rfh = logging.handlers.RotatingFileHandler(
                 self.log_file,
                 maxBytes=1024*log_config["max_size"],
                 backupCount=log_config["backup_count"]
@@ -561,9 +561,39 @@
         # Check what to do with the console output ...
         if log_config["use_console"]:
             ch = ColorStreamHandler(sys.stdout)
             ch.setLevel(level)
             ch.setFormatter(logging.Formatter(format_, datefmt))
             logger.addHandler(ch)
 
+        # control individual loggers
+        loggers = log_config.get("loggers", [])
+        for logger in loggers:
+            self.configure_logger(logger["name"], logger["level"])
+
         # Finally, capture all warnings using the logging mechanism.
         logging.captureWarnings(True)
+
+    @staticmethod
+    def configure_logger(name: str | None, level: str) \
+            -> Tuple[logging.Logger, int]:
+        """
+        Set the logging level of a logger.
+
+        Parameters
+        ----------
+        name : str
+            Name of the logger to configure. If `None`, the root logger is
+            configured.
+        level : str
+            Logging level to set. Must be one of 'debug', 'info', 'warning',
+            'error', 'critical'.
+
+        Returns
+        -------
+        Tuple[Logger, int]
+            The logger object and the logging level that was set.
+        """
+        logger = logging.getLogger(name)
+        level_ = getattr(logging, level.upper())
+        logger.setLevel(level_)
+        return logger, level
```

### Comparing `vantage6-common-3.9.0rc2/vantage6/common/docker/addons.py` & `vantage6-common-3.9.0rc4/vantage6/common/docker/addons.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.9.0rc2/vantage6/common/docker/network_manager.py` & `vantage6-common-3.9.0rc4/vantage6/common/docker/network_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.9.0rc2/vantage6/common/encryption.py` & `vantage6-common-3.9.0rc4/vantage6/common/encryption.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 these public keys is outside the scope of this module).
 """
 # TODO handle no public key from other organization (should that happen here?)
 import os
 import logging
 
 from pathlib import Path
-from typing import Any
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 from cryptography.hazmat.primitives.asymmetric import padding, rsa
+from cryptography.hazmat.primitives.asymmetric.types import PRIVATE_KEY_TYPES
 from cryptography.hazmat.primitives.serialization import (
     load_pem_private_key,
     load_pem_public_key
 )
 
 from vantage6.common import (
     Singleton,
@@ -101,15 +101,15 @@
         str
             The encrypted data encoded as base64 string.
         """
         return self.bytes_to_str(data)
 
     def decrypt_str_to_bytes(self, data: str) -> bytes:
         """
-        Decrypt base64 encoded *string* `data.
+        Decrypt base64 encoded *string* data.
 
         Parameters
         ----------
         data: str
             The data to decrypt.
 
         Returns
@@ -161,27 +161,32 @@
         ----------
         private_key_file: Path
             The path to the private key file.
         """
         super().__init__()
         self.private_key = self.__load_private_key(private_key_file)
 
-    def __load_private_key(self, private_key_file: Path) -> Any:
+    def __load_private_key(self, private_key_file: Path) -> PRIVATE_KEY_TYPES:
         """
         Load a private key file into this instance.
 
         Parameters
         ----------
         private_key_file: Path
             The path to the private key file.
 
         Returns
         -------
         Any
             The loaded private key.
+
+        Raises
+        ------
+        FileNotFoundError
+            If the private key file does not exist.
         """
 
         if not private_key_file.exists():
             raise FileNotFoundError(
                 f"Private key file {private_key_file} not found.")
 
         self.log.debug("Loading private key")
@@ -311,15 +316,15 @@
         iv = self.bytes_to_str(iv_bytes)
         encrypted_msg = self.bytes_to_str(encrypted_msg_bytes)
 
         return SEPARATOR.join([encrypted_key, iv, encrypted_msg])
 
     def decrypt_str_to_bytes(self, data: str) -> bytes:
         """
-        Decrypt base64 encoded *string* `data.
+        Decrypt base64 encoded *string* data.
 
         Parameters
         ----------
         data: str
             The data to decrypt.
 
         Returns
```

### Comparing `vantage6-common-3.9.0rc2/vantage6/common/globals.py` & `vantage6-common-3.9.0rc4/vantage6/common/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.9.0rc2/vantage6/common/log.py` & `vantage6-common-3.9.0rc4/vantage6/common/log.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.9.0rc2/vantage6/common/task_status.py` & `vantage6-common-3.9.0rc4/vantage6/common/task_status.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.9.0rc2/vantage6/common/utest.py` & `vantage6-common-3.9.0rc4/vantage6/common/utest.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.9.0rc2/vantage6_common.egg-info/PKG-INFO` & `vantage6-common-3.9.0rc4/vantage6_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-common
-Version: 3.9.0rc2
+Version: 3.9.0rc4
 Summary: Vantage6 common
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-common Version: 3.9.0rc2 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-common Version: 3.9.0rc4 Summary: Vantage6
 common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-common-3.9.0rc2/vantage6_common.egg-info/SOURCES.txt` & `vantage6-common-3.9.0rc4/vantage6_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

