# Comparing `tmp/peak-mas-1.0.8.tar.gz` & `tmp/peak-mas-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peak-mas-1.0.8.tar", last modified: Tue May 16 09:15:10 2023, max compression
+gzip compressed data, was "peak-mas-1.0.9.tar", last modified: Fri May 19 14:26:25 2023, max compression
```

## Comparing `peak-mas-1.0.8.tar` & `peak-mas-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-16 09:15:10.958342 peak-mas-1.0.8/
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)    35148 2022-11-16 18:35:26.000000 peak-mas-1.0.8/LICENSE
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     6943 2023-05-16 09:15:10.958342 peak-mas-1.0.8/PKG-INFO
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     5994 2023-05-02 14:41:35.000000 peak-mas-1.0.8/README.md
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     1664 2023-05-16 09:15:01.000000 peak-mas-1.0.8/pyproject.toml
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)       38 2023-05-16 09:15:10.959342 peak-mas-1.0.8/setup.cfg
-drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-16 09:15:10.956343 peak-mas-1.0.8/src/
-drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-16 09:15:10.957342 peak-mas-1.0.8/src/peak/
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      603 2023-05-16 09:15:01.000000 peak-mas-1.0.8/src/peak/__init__.py
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     3303 2023-05-16 09:04:22.000000 peak-mas-1.0.8/src/peak/__main__.py
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)    17777 2023-05-02 14:40:53.000000 peak-mas-1.0.8/src/peak/agents.py
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     3519 2023-05-02 14:40:53.000000 peak-mas-1.0.8/src/peak/behaviours.py
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     3571 2023-05-16 09:09:16.000000 peak-mas-1.0.8/src/peak/bootloader.py
-drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-16 09:15:10.957342 peak-mas-1.0.8/src/peak/cli/
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2022-11-16 18:35:26.000000 peak-mas-1.0.8/src/peak/cli/__init__.py
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      845 2023-05-02 14:40:53.000000 peak-mas-1.0.8/src/peak/cli/df.py
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     2853 2023-05-16 09:12:51.000000 peak-mas-1.0.8/src/peak/cli/mas.py
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     6727 2023-05-02 14:40:53.000000 peak-mas-1.0.8/src/peak/core.py
-drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-16 09:15:10.958342 peak-mas-1.0.8/src/peak_mas.egg-info/
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     6943 2023-05-16 09:15:10.000000 peak-mas-1.0.8/src/peak_mas.egg-info/PKG-INFO
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      438 2023-05-16 09:15:10.000000 peak-mas-1.0.8/src/peak_mas.egg-info/SOURCES.txt
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)        1 2023-05-16 09:15:10.000000 peak-mas-1.0.8/src/peak_mas.egg-info/dependency_links.txt
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)       44 2023-05-16 09:15:10.000000 peak-mas-1.0.8/src/peak_mas.egg-info/entry_points.txt
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      119 2023-05-16 09:15:10.000000 peak-mas-1.0.8/src/peak_mas.egg-info/requires.txt
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)        5 2023-05-16 09:15:10.000000 peak-mas-1.0.8/src/peak_mas.egg-info/top_level.txt
+drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-19 14:26:25.042127 peak-mas-1.0.9/
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)    35148 2022-11-16 18:35:26.000000 peak-mas-1.0.9/LICENSE
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     6943 2023-05-19 14:26:25.042127 peak-mas-1.0.9/PKG-INFO
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     5994 2023-05-02 14:41:35.000000 peak-mas-1.0.9/README.md
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     1664 2023-05-19 14:26:15.000000 peak-mas-1.0.9/pyproject.toml
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)       38 2023-05-19 14:26:25.042127 peak-mas-1.0.9/setup.cfg
+drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-19 14:26:25.038127 peak-mas-1.0.9/src/
+drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-19 14:26:25.040127 peak-mas-1.0.9/src/peak/
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      603 2023-05-19 14:26:15.000000 peak-mas-1.0.9/src/peak/__init__.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     3303 2023-05-16 09:04:22.000000 peak-mas-1.0.9/src/peak/__main__.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)    17777 2023-05-02 14:40:53.000000 peak-mas-1.0.9/src/peak/agents.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     3519 2023-05-02 14:40:53.000000 peak-mas-1.0.9/src/peak/behaviours.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     3605 2023-05-18 12:45:32.000000 peak-mas-1.0.9/src/peak/bootloader.py
+drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-19 14:26:25.041127 peak-mas-1.0.9/src/peak/cli/
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2022-11-16 18:35:26.000000 peak-mas-1.0.9/src/peak/cli/__init__.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      845 2023-05-02 14:40:53.000000 peak-mas-1.0.9/src/peak/cli/df.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     2817 2023-05-19 14:25:32.000000 peak-mas-1.0.9/src/peak/cli/mas.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     7455 2023-05-19 14:25:32.000000 peak-mas-1.0.9/src/peak/core.py
+drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-19 14:26:25.041127 peak-mas-1.0.9/src/peak_mas.egg-info/
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     6943 2023-05-19 14:26:25.000000 peak-mas-1.0.9/src/peak_mas.egg-info/PKG-INFO
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      438 2023-05-19 14:26:25.000000 peak-mas-1.0.9/src/peak_mas.egg-info/SOURCES.txt
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)        1 2023-05-19 14:26:25.000000 peak-mas-1.0.9/src/peak_mas.egg-info/dependency_links.txt
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)       44 2023-05-19 14:26:25.000000 peak-mas-1.0.9/src/peak_mas.egg-info/entry_points.txt
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      119 2023-05-19 14:26:25.000000 peak-mas-1.0.9/src/peak_mas.egg-info/requires.txt
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)        5 2023-05-19 14:26:25.000000 peak-mas-1.0.9/src/peak_mas.egg-info/top_level.txt
```

### Comparing `peak-mas-1.0.8/LICENSE` & `peak-mas-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `peak-mas-1.0.8/PKG-INFO` & `peak-mas-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peak-mas
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python-based framework for heterogeneous agent communities
 Author-email: Bruno Ribeiro <brgri@isep.ipp.pt>
 Project-URL: Homepage, https://www.gecad.isep.ipp.pt/peak
 Project-URL: Github, https://github.com/gecad-group/peak-mas
 Keywords: framework,multiagent,agent-based,ecosystem,spade,xmpp
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `peak-mas-1.0.8/README.md` & `peak-mas-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `peak-mas-1.0.8/pyproject.toml` & `peak-mas-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "peak-mas"
-version = "1.0.8"
+version = "1.0.9"
 description = "Python-based framework for heterogeneous agent communities"
 readme = "README.md"
 authors = [{ name = "Bruno Ribeiro", email = "brgri@isep.ipp.pt" }]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -38,15 +38,15 @@
 Homepage = "https://www.gecad.isep.ipp.pt/peak"
 Github = "https://github.com/gecad-group/peak-mas"
 
 [project.scripts]
 peak = "peak.__main__:main"
 
 [tool.bumpver]
-current_version = "1.0.8"
+current_version = "1.0.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "chore: bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `peak-mas-1.0.8/src/peak/__init__.py` & `peak-mas-1.0.9/src/peak/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 from peak.agents import *
 from peak.behaviours import *
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 __author__ = "Bruno Ribeiro"
 __email__ = "brgri@isep.ipp.pt"
-__version__ = "1.0.8"
+__version__ = "1.0.9"
```

### Comparing `peak-mas-1.0.8/src/peak/__main__.py` & `peak-mas-1.0.9/src/peak/__main__.py`

 * *Files identical despite different names*

### Comparing `peak-mas-1.0.8/src/peak/agents.py` & `peak-mas-1.0.9/src/peak/agents.py`

 * *Files identical despite different names*

### Comparing `peak-mas-1.0.8/src/peak/behaviours.py` & `peak-mas-1.0.9/src/peak/behaviours.py`

 * *Files identical despite different names*

### Comparing `peak-mas-1.0.8/src/peak/bootloader.py` & `peak-mas-1.0.9/src/peak/bootloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     asyncio.run(_wait_for_processes(procs))
 
 
 def boot_agent(
     file: Path,
     jid: JID,
     cid: int,
-    log_level: int,
+    log_level: str,
     verify_security: bool,
 ):
     """Configures logging system and boots the agent.
 
     Args:
         file: File path where the agent's class is.
         jid: JID of the agent.
@@ -64,14 +64,15 @@
     os.makedirs(logs_folder, exist_ok=True)
     sys.stdout = open(log_file, "a", buffering=1)
     sys.stderr = sys.stdout
     handler = logging.FileHandler(log_file)
     handler.setFormatter(
         logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
     )
+    log_level = log_level.upper()
     logger.parent.handlers = []
     logger.parent.addHandler(handler)
     logger.parent.setLevel(log_level)
     handler.setLevel(log_level)
 
     logger.info("Creating agent from file")
     agent_class = _get_class(file)
```

### Comparing `peak-mas-1.0.8/src/peak/cli/df.py` & `peak-mas-1.0.9/src/peak/cli/df.py`

 * *Files identical despite different names*

### Comparing `peak-mas-1.0.8/src/peak/cli/mas.py` & `peak-mas-1.0.9/src/peak/cli/mas.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import sys
 from argparse import ArgumentTypeError
-from logging import getLevelName, getLogger
+from logging import getLogger
 from pathlib import Path
 
 import yaml
 
 from peak import JID
 from peak.bootloader import bootloader
 
 _logger = getLogger(__name__)
 
 
 def agent_exec(
     file: Path,
     jid: JID,
-    clones: int = 1,
-    log_level: int = getLevelName("INFO"),
+    clones: int,
+    log_level: str,
     verify_security: bool = False,
     *args,
     **kargs,
 ):
     """Executes a single agent.
 
     Args:
@@ -47,15 +47,15 @@
         agent = kwargs.copy()
         agents.append(agent)
         kwargs["jid"] = kwargs["jid"].replace(localpart=f"{name}{cid}")
         kwargs["cid"] = cid
     bootloader(agents)
 
 
-def multi_agent_exec(file: Path, log_level, *args, **kargs):
+def multi_agent_exec(file: Path, log_level: str, *args, **kargs):
     """Executes agents using a YAML configuration file.
 
     Args:
         file: Path to the agent's python file.
     """
 
     _logger.info("Parsing YAML file")
```

### Comparing `peak-mas-1.0.8/src/peak/core.py` & `peak-mas-1.0.9/src/peak/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import asyncio
 import logging as _logging
 from abc import ABCMeta as _ABCMeta
-from typing import Dict, List
+from typing import Dict, List, Optional
 
 import aioxmpp as _aioxmpp
 import spade as _spade
 from aioxmpp import JID
 from aioxmpp.callbacks import first_signal
 
 _module_logger = _logging.getLogger(__name__)
@@ -48,25 +49,47 @@
         self.message_dispatcher.register_callback(
             _aioxmpp.MessageType.NORMAL,
             None,
             self._message_received,
         )
 
 
-class _Behaviour:
+class _BehaviourMixin:
     """Adds XMPP functinalities to SPADE's base behaviours.
 
     Acts as Mixin in the SPADE's behaviours.
 
     Attributes:
         logger (:obj:`Logger`): Used to log every event in a behaviour."""
 
     agent: Agent
     _logger = _module_logger.getChild("_Behaviour")
 
+    async def receive(
+        self, timeout: Optional[float] = None
+    ) -> Optional[_spade.message.Message]:
+        """
+        Receives a message for this behaviour and waits `timeout` seconds.
+        If timeout is `None`, it will wait until it receives a message.
+
+        Note: Redefinition of the receive method of SPADE Behaviours
+
+        Args:
+            timeout (float, optional): number of seconds until return
+
+        Returns:
+            Message | None
+        """
+        coro = self.queue.get()
+        try:
+            msg = await asyncio.wait_for(coro, timeout=timeout)
+        except asyncio.TimeoutError:
+            msg = None
+        return msg
+
     async def join_community(self, jid: str):
         """Joins a community.
 
         Args:
             jid (str): XMPP identifier of the community.
 
         Raises:
@@ -176,25 +199,27 @@
         self._logger.debug(f"Waiting for behaviour: {behaviour}")
         if not behaviour.is_running:
             self.agent.add_behaviour(behaviour, template)
         await behaviour.join()
 
 
 class OneShotBehaviour(
-    _spade.behaviour.OneShotBehaviour, _Behaviour, metaclass=_ABCMeta
+    _BehaviourMixin, _spade.behaviour.OneShotBehaviour, metaclass=_ABCMeta
 ):
     """This behaviour is only executed once."""
 
 
 class PeriodicBehaviour(
-    _spade.behaviour.PeriodicBehaviour, _Behaviour, metaclass=_ABCMeta
+    _BehaviourMixin, _spade.behaviour.PeriodicBehaviour, metaclass=_ABCMeta
 ):
     """This behaviour is executed periodically with an interval."""
 
 
-class CyclicBehaviour(_spade.behaviour.CyclicBehaviour, _Behaviour, metaclass=_ABCMeta):
+class CyclicBehaviour(
+    _BehaviourMixin, _spade.behaviour.CyclicBehaviour, metaclass=_ABCMeta
+):
     """This behaviour is executed cyclically until it is stopped."""
 
 
-class FSMBehaviour(_spade.behaviour.FSMBehaviour, _Behaviour, metaclass=_ABCMeta):
+class FSMBehaviour(_BehaviourMixin, _spade.behaviour.FSMBehaviour, metaclass=_ABCMeta):
     """A behaviour composed of states (oneshotbehaviours) that may transition from one
     state to another."""
```

### Comparing `peak-mas-1.0.8/src/peak_mas.egg-info/PKG-INFO` & `peak-mas-1.0.9/src/peak_mas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peak-mas
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python-based framework for heterogeneous agent communities
 Author-email: Bruno Ribeiro <brgri@isep.ipp.pt>
 Project-URL: Homepage, https://www.gecad.isep.ipp.pt/peak
 Project-URL: Github, https://github.com/gecad-group/peak-mas
 Keywords: framework,multiagent,agent-based,ecosystem,spade,xmpp
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

