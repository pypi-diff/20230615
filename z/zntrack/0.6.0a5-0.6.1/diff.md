# Comparing `tmp/zntrack-0.6.0a5.tar.gz` & `tmp/zntrack-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zntrack-0.6.0a5.tar", max compression
+gzip compressed data, was "zntrack-0.6.1.tar", max compression
```

## Comparing `zntrack-0.6.0a5.tar` & `zntrack-0.6.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0    13576 2023-01-31 09:35:21.669596 zntrack-0.6.0a5/LICENSE
--rw-r--r--   0        0        0     6025 2023-04-10 18:32:22.981943 zntrack-0.6.0a5/README.md
--rw-r--r--   0        0        0     2299 2023-04-10 18:32:22.981943 zntrack-0.6.0a5/pyproject.toml
--rw-r--r--   0        0        0      715 2023-03-28 15:55:39.672257 zntrack-0.6.0a5/zntrack/__init__.py
--rw-r--r--   0        0        0     2940 2023-04-08 19:50:48.755766 zntrack-0.6.0a5/zntrack/cli/__init__.py
--rw-r--r--   0        0        0       30 2023-03-16 14:38:52.662721 zntrack-0.6.0a5/zntrack/core/__init__.py
--rw-r--r--   0        0        0    10646 2023-04-05 10:56:52.273202 zntrack-0.6.0a5/zntrack/core/node.py
--rw-r--r--   0        0        0    14022 2023-03-16 14:38:52.672721 zntrack-0.6.0a5/zntrack/core/nodify.py
--rw-r--r--   0        0        0     2078 2023-04-09 21:25:48.681300 zntrack-0.6.0a5/zntrack/exceptions/__init__.py
--rw-r--r--   0        0        0      195 2023-03-16 14:38:52.672721 zntrack-0.6.0a5/zntrack/fields/__init__.py
--rw-r--r--   0        0        0     5135 2023-04-10 18:15:43.822843 zntrack-0.6.0a5/zntrack/fields/dvc/__init__.py
--rw-r--r--   0        0        0     9915 2023-04-10 18:15:43.822843 zntrack-0.6.0a5/zntrack/fields/field.py
--rw-r--r--   0        0        0     3562 2023-04-08 19:50:48.755766 zntrack-0.6.0a5/zntrack/fields/meta/__init__.py
--rw-r--r--   0        0        0    16041 2023-04-10 18:15:43.822843 zntrack-0.6.0a5/zntrack/fields/zn/__init__.py
--rw-r--r--   0        0        0     2647 2023-03-16 14:38:52.692721 zntrack-0.6.0a5/zntrack/notebooks/jupyter.py
--rw-r--r--   0        0        0      133 2023-03-16 14:38:52.692721 zntrack-0.6.0a5/zntrack/project/__init__.py
--rw-r--r--   0        0        0     9694 2023-04-10 18:32:22.981943 zntrack-0.6.0a5/zntrack/project/zntrack_project.py
--rw-r--r--   0        0        0     1822 2023-03-16 14:38:52.702721 zntrack-0.6.0a5/zntrack/tools/__init__.py
--rw-r--r--   0        0        0     6065 2023-03-28 16:02:45.147573 zntrack-0.6.0a5/zntrack/utils/__init__.py
--rw-r--r--   0        0        0     2161 2023-01-31 09:35:21.909593 zntrack-0.6.0a5/zntrack/utils/cli.py
--rw-r--r--   0        0        0     3354 2023-04-10 11:58:36.429618 zntrack-0.6.0a5/zntrack/utils/config.py
--rw-r--r--   0        0        0     4727 2023-03-06 10:02:12.898384 zntrack-0.6.0a5/zntrack/utils/file_io.py
--rw-r--r--   0        0        0     1500 2023-03-17 15:52:43.708117 zntrack-0.6.0a5/zntrack/utils/node_wd.py
--rw-r--r--   0        0        0     7166 1970-01-01 00:00:00.000000 zntrack-0.6.0a5/PKG-INFO
+-rw-r--r--   0        0        0    13576 2023-01-31 09:35:21.669596 zntrack-0.6.1/LICENSE
+-rw-r--r--   0        0        0     6396 2023-05-30 07:36:43.136455 zntrack-0.6.1/README.md
+-rw-r--r--   0        0        0     2320 2023-06-15 14:22:03.077439 zntrack-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      770 2023-05-30 07:36:43.146455 zntrack-0.6.1/zntrack/__init__.py
+-rw-r--r--   0        0        0     2940 2023-04-08 19:50:48.755766 zntrack-0.6.1/zntrack/cli/__init__.py
+-rw-r--r--   0        0        0       30 2023-03-16 14:38:52.662721 zntrack-0.6.1/zntrack/core/__init__.py
+-rw-r--r--   0        0        0     3353 2023-05-30 07:36:43.146455 zntrack-0.6.1/zntrack/core/load.py
+-rw-r--r--   0        0        0    11277 2023-06-15 13:55:07.555376 zntrack-0.6.1/zntrack/core/node.py
+-rw-r--r--   0        0        0    14022 2023-03-16 14:38:52.672721 zntrack-0.6.1/zntrack/core/nodify.py
+-rw-r--r--   0        0        0     2080 2023-04-11 11:21:14.631288 zntrack-0.6.1/zntrack/exceptions/__init__.py
+-rw-r--r--   0        0        0      195 2023-03-16 14:38:52.672721 zntrack-0.6.1/zntrack/fields/__init__.py
+-rw-r--r--   0        0        0     5135 2023-04-10 18:15:43.822843 zntrack-0.6.1/zntrack/fields/dvc/__init__.py
+-rw-r--r--   0        0        0     9915 2023-04-10 18:15:43.822843 zntrack-0.6.1/zntrack/fields/field.py
+-rw-r--r--   0        0        0     3562 2023-04-08 19:50:48.755766 zntrack-0.6.1/zntrack/fields/meta/__init__.py
+-rw-r--r--   0        0        0    16145 2023-05-26 12:06:51.613839 zntrack-0.6.1/zntrack/fields/zn/__init__.py
+-rw-r--r--   0        0        0     2648 2023-05-26 07:06:39.819686 zntrack-0.6.1/zntrack/notebooks/jupyter.py
+-rw-r--r--   0        0        0      159 2023-06-15 13:55:07.555376 zntrack-0.6.1/zntrack/project/__init__.py
+-rw-r--r--   0        0        0    12971 2023-06-15 14:22:03.087439 zntrack-0.6.1/zntrack/project/zntrack_project.py
+-rw-r--r--   0        0        0     1822 2023-03-16 14:38:52.702721 zntrack-0.6.1/zntrack/tools/__init__.py
+-rw-r--r--   0        0        0     5909 2023-05-26 07:06:39.829686 zntrack-0.6.1/zntrack/utils/__init__.py
+-rw-r--r--   0        0        0     2161 2023-01-31 09:35:21.909593 zntrack-0.6.1/zntrack/utils/cli.py
+-rw-r--r--   0        0        0     3354 2023-04-10 11:58:36.429618 zntrack-0.6.1/zntrack/utils/config.py
+-rw-r--r--   0        0        0     4776 2023-04-26 09:50:10.373360 zntrack-0.6.1/zntrack/utils/file_io.py
+-rw-r--r--   0        0        0     1500 2023-03-17 15:52:43.708117 zntrack-0.6.1/zntrack/utils/node_wd.py
+-rw-r--r--   0        0        0     7535 1970-01-01 00:00:00.000000 zntrack-0.6.1/PKG-INFO
```

### Comparing `zntrack-0.6.0a5/LICENSE` & `zntrack-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.0a5/README.md` & `zntrack-0.6.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,114 +6,151 @@
 [![code-style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black/)
 [![Documentation](https://readthedocs.org/projects/zntrack/badge/?version=latest)](https://zntrack.readthedocs.io/en/latest/?badge=latest)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zincware/ZnTrack/HEAD)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6472850.svg)](https://doi.org/10.5281/zenodo.6472850)
 [![ZnTrack](https://img.shields.io/badge/Powered%20by-ZnTrack-%23007CB0)](https://zntrack.readthedocs.io/en/latest/)
 [![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
 
-
-
-
 ![Logo](https://raw.githubusercontent.com/zincware/ZnTrack/main/docs/source/_static/logo_ZnTrack.png)
 
 # ZnTrack: A Parameter Tracking Package for Python
 
-ZnTrack ``zɪŋk træk`` is a lightweight and easy-to-use package for tracking parameters in your Python projects using DVC.
-With ZnTrack, you can define parameters in Python classes and monitor how they change over time.
-This information can then be used to compare the results of different runs, identify computational bottlenecks, and avoid the re-running of code components where parameters have not changed.
+ZnTrack `zɪŋk træk` is a lightweight and easy-to-use package for tracking
+parameters in your Python projects using DVC. With ZnTrack, you can define
+parameters in Python classes and monitor how they change over time. This
+information can then be used to compare the results of different runs, identify
+computational bottlenecks, and avoid the re-running of code components where
+parameters have not changed.
 
 ## Key Features
-- Parameter, output and metric tracking: ZnTrack makes it easy to store and track the values of parameters in your Python code. It further allows you to store any outputs produced and gives an easy interface to define metrics.
-- Lightweight and database-free: Unlike other parameter tracking solutions, ZnTrack is lightweight and does not require any databases.
+
+- Parameter, output and metric tracking: ZnTrack makes it easy to store and
+  track the values of parameters in your Python code. It further allows you to
+  store any outputs produced and gives an easy interface to define metrics.
+- Lightweight and database-free: Unlike other parameter tracking solutions,
+  ZnTrack is lightweight and does not require any databases.
 
 ## Getting Started
-To get started with ZnTrack, you can install it via pip: ```pip install zntrack```
 
-Next, you can start using ZnTrack to track parameters, outputs and metrics in your Python code.
-Here's an example of how to use ZnTrack to track the value of a parameter in a Python class.
-Start in an empty directory and run ``git init`` and ``dvc init`` for preparation.
+To get started with ZnTrack, you can install it via pip: `pip install zntrack`
 
-Then put the following into a python file called `hello_world.py` and call it with `python hello_world.py`.
+Next, you can start using ZnTrack to track parameters, outputs and metrics in
+your Python code. Here's an example of how to use ZnTrack to track the value of
+a parameter in a Python class. Start in an empty directory and run `git init`
+and `dvc init` for preparation.
+
+Then put the following into a python file called `hello_world.py` and call it
+with `python hello_world.py`.
 
 ```python
-from zntrack import Node, zn
+import zntrack
 from random import randrange
 
 
-class HelloWorld(Node):
+class HelloWorld(zntrack.Node):
     """Define a ZnTrack Node"""
     # parameter to be tracked
-    max_number: int = zn.params()
+    max_number: int = zntrack.zn.params()
     # parameter to store as output
-    random_number: int = zn.outs()
-    
+    random_number: int = zntrack.zn.outs()
+
     def run(self):
         """Command to be run by DVC"""
         self.random_number = randrange(self.max_number)
-        
+
 if __name__ == "__main__":
     # Write the computational graph
     with zntrack.Project() as project:
         hello_world = HelloWorld(max_number=512)
     project.run()
 ```
 
-This will create a [DVC](https://dvc.org) stage ``HelloWorld``.
-The workflow is defined in ``dvc.yaml`` and the parameters are stored in ``params.yaml``.
+This will create a [DVC](https://dvc.org) stage `HelloWorld`. The workflow is
+defined in `dvc.yaml` and the parameters are stored in `params.yaml`.
+
+This will run the workflow with `dvc repro` automatically. Once the graph is
+executed, the results, i.e. the random number can be accessed directly by the
+Node object.
 
-This will run the workflow with ``dvc repro`` automatically.
-Once the graph is executed, the results, i.e. the random number can be accessed directly by the Node object.
 ```python
 hello_world.load()
-print(hello_world.random_numer)
+print(hello_world.random_number)
 ```
-An overview of all the ZnTrack features as well as more detailed examples can be found in the [ZnTrack Documentation](https://zntrack.readthedocs.io/en/latest/).
+
+> ## Tip
+>
+> You can easily load this Node directly from a repository.
+>
+> ```python
+> import zntrack
+>
+> node = zntrack.from_rev(
+>     "HelloWorld",
+>     remote="https://github.com/PythonFZ/ZnTrackExamples.git",
+>     rev="b9316bf",
+> )
+> ```
+>
+> Try accessing the `max_number` parameter and `random_number` output. All Nodes
+> from this and many other repositories can be loaded like this.
+
+An overview of all the ZnTrack features as well as more detailed examples can be
+found in the [ZnTrack Documentation](https://zntrack.readthedocs.io/en/latest/).
 
 ## Wrap Python Functions
-ZnTrack also provides tools to convert a Python function into a DVC Node.
-This approach is much more lightweight compared to the class-based approach with only a reduced set of functionality.
-Therefore, it is recommended for smaller nodes that do not need the additional toolset that the class-based approach provides.
 
-````python
+ZnTrack also provides tools to convert a Python function into a DVC Node. This
+approach is much more lightweight compared to the class-based approach with only
+a reduced set of functionality. Therefore, it is recommended for smaller nodes
+that do not need the additional toolset that the class-based approach provides.
+
+```python
 from zntrack import nodify, NodeConfig
 import pathlib
 
 @nodify(outs=pathlib.Path("text.txt"), params={"text": "Lorem Ipsum"})
 def write_text(cfg: NodeConfig):
     cfg.outs.write_text(
         cfg.params.text
     )
 # build the DVC graph
 with zntrack.Project() as project:
     write_text()
 project.run()
-````
+```
 
-The ``cfg`` dataclass passed to the function provides access to all configured files
-and parameters via [dot4dict](https://github.com/zincware/dot4dict). The function body
-will be executed by the ``dvc repro`` command or if ran via `write_text(run=True)`.
-All parameters are loaded from or stored in ``params.yaml``.
+The `cfg` dataclass passed to the function provides access to all configured
+files and parameters via [dot4dict](https://github.com/zincware/dot4dict). The
+function body will be executed by the `dvc repro` command or if ran via
+`write_text(run=True)`. All parameters are loaded from or stored in
+`params.yaml`.
 
 # Technical Details
 
-
 ## ZnTrack as an Object-Relational Mapping for DVC
 
-On a fundamental level the ZnTrack package provides an easy-to-use interface for DVC directly from Python.
-It handles all the computational overhead of reading config files, defining outputs in the `dvc.yaml` as well as in the script and much more.
+On a fundamental level the ZnTrack package provides an easy-to-use interface for
+DVC directly from Python. It handles all the computational overhead of reading
+config files, defining outputs in the `dvc.yaml` as well as in the script and
+much more.
 
 For more information on DVC visit their [homepage](https://dvc.org/doc).
 
-Copyright
-=========
+# Copyright
 
-This project is distributed under the [Apache License Version 2.0](https://github.com/zincware/ZnTrack/blob/main/LICENSE).
+This project is distributed under the
+[Apache License Version 2.0](https://github.com/zincware/ZnTrack/blob/main/LICENSE).
 
 ## Similar Tools
-The following (incomplete) list of other projects that either work together with ZnTrack or can achieve similar results with slightly different goals or programming languages.
+
+The following (incomplete) list of other projects that either work together with
+ZnTrack or can achieve similar results with slightly different goals or
+programming languages.
 
 - [DVC](https://dvc.org/) - Main dependency of ZnTrack for Data Version Control.
 - [dvthis](https://github.com/jcpsantiago/dvthis) - Introduce DVC to R.
-- [DAGsHub Client](https://github.com/DAGsHub/client) - Logging parameters from within .Python 
+- [DAGsHub Client](https://github.com/DAGsHub/client) - Logging parameters from
+  within .Python
 - [MLFlow](https://mlflow.org/) - A Machine Learning Lifecycle Platform.
 - [Metaflow](https://metaflow.org/) - A framework for real-life data science.
-- [Hydra](https://hydra.cc/) - A framework for elegantly configuring complex applications
+- [Hydra](https://hydra.cc/) - A framework for elegantly configuring complex
+  applications
```

### Comparing `zntrack-0.6.0a5/pyproject.toml` & `zntrack-0.6.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ZnTrack"
-version = "0.6.0a5"
+version = "0.6.1"
 description = "Create, Run and Benchmark DVC Pipelines in Python"
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 license = "Apache-2.0"
 keywords=["data-science", "data-version-control", "machine-learning", "reproducibility", "collaboration"]
 readme = "README.md"
 
 
@@ -36,19 +36,16 @@
 numpy = "^1.23"
 matplotlib = "^3.5.2"
 ase = "^3.22.1"
 pre-commit = "^2.20.0"
 coverage = "^6.4"
 nbmake = "^1.3.3"
 pytest-xdist = "^2.5.0"
-
-[tool.poetry.group.lint.dependencies]
-black = "^23.1.0"
-isort = "^5.12.0"
-ruff = "^0.0.252"
+optuna = "^3.1.1"
+scikit-learn = "^1.2.2"
 
 [tool.poetry.group.notebook.dependencies]
 jupyterlab = "^3.4.3"
 
 [tool.poetry.group.docs.dependencies]
 furo = "^2022.12.7"
 sphinx-copybutton = "^0.5.1"
@@ -105,15 +102,20 @@
 [tool.ruff]
 line-length = 90
 
 select = ["E", "F", "D", "N", "C", "I"] #, "ANN"]
 extend-ignore = [
     "D213", "D203",
     "D401",
-    "N802", "N801"
+    "N802", "N801",
+    "C901", # for now
 ]
 
 exclude = [
     "tmp",
     "tests",
     "docs",
 ]
+
+
+[tool.codespell]
+skip = "poetry.lock,examples/*"
```

### Comparing `zntrack-0.6.0a5/zntrack/__init__.py` & `zntrack-0.6.1/zntrack/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """ZnTrack - Create, visualize, run & benchmark DVC pipelines in Python.
 
 GitHub: https://github.com/zincware/ZnTrack
 """
 import importlib.metadata
 
 from zntrack import exceptions, tools
+from zntrack.core.load import from_rev
 from zntrack.core.node import Node
 from zntrack.core.nodify import NodeConfig, nodify
 from zntrack.fields import Field, FieldGroup, LazyField, dvc, meta, zn
 from zntrack.project import Project
 from zntrack.utils import config
 from zntrack.utils.node_wd import nwd
 
@@ -25,8 +26,9 @@
     "Field",
     "LazyField",
     "FieldGroup",
     "nodify",
     "NodeConfig",
     "tools",
     "exceptions",
+    "from_rev",
 ]
```

### Comparing `zntrack-0.6.0a5/zntrack/cli/__init__.py` & `zntrack-0.6.1/zntrack/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.0a5/zntrack/core/node.py` & `zntrack-0.6.1/zntrack/core/node.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,35 @@
-"""The Node class."""
+"""The ZnTrack Node class."""
 from __future__ import annotations
 
 import contextlib
 import dataclasses
 import functools
 import importlib
 import logging
 import pathlib
+import time
 import typing
 
 import dvc.api
 import dvc.cli
+import dvc.utils.strictyaml
 import znflow
 import zninit
 import znjson
 
 from zntrack import exceptions
 from zntrack.notebooks.jupyter import jupyter_class_to_file
-from zntrack.utils import NodeStatusResults, deprecated, module_handler, run_dvc_cmd
+from zntrack.utils import (
+    NodeStatusResults,
+    deprecated,
+    file_io,
+    module_handler,
+    run_dvc_cmd,
+)
 from zntrack.utils.config import config
 
 log = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
 class NodeStatus:
@@ -51,18 +59,24 @@
         """Get the file system of the Node."""
         log.warning("Deprecated. Use 'state.fs' instead.")
         return self.fs
 
     @functools.cached_property
     def fs(self) -> dvc.api.DVCFileSystem:
         """Get the file system of the Node."""
-        return dvc.api.DVCFileSystem(
-            url=self.remote,
-            rev=self.rev,
-        )
+        for _ in range(10):
+            try:
+                return dvc.api.DVCFileSystem(
+                    url=self.remote,
+                    rev=self.rev,
+                )
+            except dvc.utils.strictyaml.YAMLValidationError as err:
+                log.debug(err)
+                time.sleep(0.1)
+        raise dvc.utils.strictyaml.YAMLValidationError
 
 
 class _NameDescriptor(zninit.Descriptor):
     """A descriptor for the name attribute."""
 
     def __get__(self, instance, owner=None):
         if instance is None:
@@ -151,20 +165,27 @@
         if not nwd.exists():
             nwd.mkdir(parents=True)
         return nwd
 
     def save(self, parameter: bool = True, results: bool = True) -> None:
         """Save the node's output to disk."""
         # TODO have an option to save and run dvc commit afterwards.
+
+        # TODO: check if there is a difference in saving
+        # a loaded node vs a new node and why
         from zntrack.fields import Field, FieldGroup
 
         # Jupyter Notebook
         if config.nb_name:
             self.convert_notebook(config.nb_name)
 
+        if parameter:
+            file_io.clear_config_file(file="params.yaml", node_name=self.name)
+            file_io.clear_config_file(file="zntrack.json", node_name=self.name)
+
         for attr in zninit.get_descriptors(Field, self=self):
             if attr.group == FieldGroup.PARAMETER and parameter:
                 attr.save(self)
             if attr.group == FieldGroup.RESULT and results:
                 attr.save(self)
             if attr.group is None:
                 raise ValueError(
```

### Comparing `zntrack-0.6.0a5/zntrack/core/nodify.py` & `zntrack-0.6.1/zntrack/core/nodify.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.0a5/zntrack/exceptions/__init__.py` & `zntrack-0.6.1/zntrack/exceptions/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,14 @@
 
         Parameters
         ----------
         node: Node
             The node that is already on the graph.
         """
         msg = (
-            f"Node name {node.name} is already used in the graph. Please use"
+            f"Node name '{node.name}' is already used in the graph. Please use"
             " 'name=...' to specify a unique name or set the project attribute"
             " 'automatic_node_names=True' to automatically add a number to"
             " the name. Alternatively, set the project attribute 'force=True'"
             " to overwrite existing nodes."
         )
         super().__init__(msg)
```

### Comparing `zntrack-0.6.0a5/zntrack/fields/dvc/__init__.py` & `zntrack-0.6.1/zntrack/fields/dvc/__init__.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.0a5/zntrack/fields/field.py` & `zntrack-0.6.1/zntrack/fields/field.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.0a5/zntrack/fields/meta/__init__.py` & `zntrack-0.6.1/zntrack/fields/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.0a5/zntrack/fields/zn/__init__.py` & `zntrack-0.6.1/zntrack/fields/zn/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 import znflow
 import znflow.utils
 import zninit
 import znjson
 from znflow import handler
 
 from zntrack import exceptions
-from zntrack.fields.field import DataIsLazyError, Field, FieldGroup, LazyField, PlotsMixin
+from zntrack.fields.field import (
+    DataIsLazyError,
+    Field,
+    FieldGroup,
+    LazyField,
+    PlotsMixin,
+)
 from zntrack.utils import module_handler, update_key_val
 
 if typing.TYPE_CHECKING:
     from zntrack import Node
 log = logging.getLogger(__name__)
 
 
@@ -135,15 +141,15 @@
         with open(file, "w") as f:
             yaml.safe_dump(params_dict, f, indent=4)
 
     def get_data(self, instance: "Node") -> any:
         """Get the value of the field from the file."""
         file = self.get_files(instance)[0]
         params_dict = yaml.safe_load(instance.state.fs.read_text(file))
-        value = params_dict[instance.name].get(self.name, None)
+        value = params_dict[instance.name][self.name]
         return json.loads(json.dumps(value), cls=znjson.ZnDecoder)
 
     def get_stage_add_argument(self, instance: "Node") -> typing.List[tuple]:
         """Get the DVC stage add argument for this field.
 
         Parameters
         ----------
@@ -389,15 +395,15 @@
     The other Node will provide its parameters and methods to be used.
     From a graph standpoint, it will add these parameters and methods to the Node
     it is attached to.
     The Node will not execute its run method or save any results to disk.
     """
 
     def __set__(self, instance, value):
-        """Disbale the _graph_ in the value 'Node'."""
+        """Disable the _graph_ in the value 'Node'."""
         if value is None:
             return super().__set__(instance, value)
 
         for entry in value if isinstance(value, (list, tuple)) else [value]:
             if hasattr(entry, "_graph_"):
                 entry._graph_ = None
                 if entry.uuid in instance._graph_:
@@ -458,14 +464,16 @@
                 "stage",
                 "add",
                 "--name",
                 name,
                 "--force",
                 "--outs",
                 f"nodes/{name}/hash",
+                "--params",
+                f"zntrack.json:{instance.name}.{self.name}",
             ]
             field_cmds = []
             for attr in zninit.get_descriptors(Params, self=node):
                 field_cmds += attr.get_stage_add_argument(node)
 
             for field_cmd in set(field_cmds):
                 _cmd += list(field_cmd)
```

### Comparing `zntrack-0.6.0a5/zntrack/notebooks/jupyter.py` & `zntrack-0.6.1/zntrack/notebooks/jupyter.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     log_jupyter_warning()
     log.debug(f"Converting {nb_name} to file {module_name}.py")
     nb_name = pathlib.Path(nb_name)
 
     subprocess.run(
         ["jupyter", "nbconvert", "--to", "script", nb_name.as_posix()],
-        capture_output=config.log_level > logging.INFO,
+        capture_output=config.log_level > logging.DEBUG,
         check=True,
     )
 
     reading_class = False
     found_node = False
 
     imports = ""
```

### Comparing `zntrack-0.6.0a5/zntrack/project/zntrack_project.py` & `zntrack-0.6.1/zntrack/project/zntrack_project.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,23 +3,26 @@
 
 import contextlib
 import dataclasses
 import json
 import logging
 import pathlib
 import shutil
+import subprocess
+import typing
 
+import dvc.api
 import git
 import yaml
 import znflow
 from znflow.handler import UpdateConnectors
 
 from zntrack import exceptions
 from zntrack.core.node import Node, get_dvc_cmd
-from zntrack.utils import capture_run_dvc_cmd, run_dvc_cmd
+from zntrack.utils import run_dvc_cmd
 
 log = logging.getLogger(__name__)
 
 
 def _initalize():
     """Initialize the project."""
     try:
@@ -33,14 +36,29 @@
         pathlib.Path("zntrack.json").write_text(json.dumps({}))
         pathlib.Path("dvc.yaml").write_text(yaml.safe_dump({}))
         pathlib.Path("params.yaml").write_text(yaml.safe_dump({}))
         repo.git.add(A=True)
         repo.index.commit("Project initialized.")
 
 
+class ZnTrackGraph(znflow.DiGraph):
+    """Subclass of the znflow.DiGraph."""
+
+    project: Project = None
+
+    def add_node(self, node_for_adding, **attr):
+        """Rename Nodes if required."""
+        value = super().add_node(node_for_adding, **attr)
+        self.project.update_node_names(check=False)
+        # this is called in __new__ and therefore,
+        # the name might not be set correctly.
+        # update node names only works, if name is not set.
+        return value
+
+
 @dataclasses.dataclass
 class Project:
     """The ZnTrack Project class.
 
     Attributes
     ----------
     graph : znflow.DiGraph
@@ -53,31 +71,34 @@
     automatic_node_names : bool, default = False
         If True, automatically add a number to the node name if the name is already
             used in the graph.
     force : bool, default = False
         overwrite existing nodes.
     """
 
-    graph: znflow.DiGraph = dataclasses.field(default_factory=znflow.DiGraph, init=False)
+    graph: znflow.DiGraph = dataclasses.field(default_factory=ZnTrackGraph, init=False)
     initialize: bool = True
     remove_existing_graph: bool = False
     automatic_node_names: bool = False
     force: bool = False
 
+    _groups: list = dataclasses.field(default_factory=list, init=False, repr=False)
+
     def __post_init__(self):
         """Initialize the Project.
 
         Attributes
         ----------
         initialize : bool, default = True
             If True, initialize a git repository and a dvc repository.
         remove_existing_graph : bool, default = False
             If True, remove 'dvc.yaml', 'zntrack.json' and 'params.yaml'
               before writing new nodes.
         """
+        self.graph.project = self
         if self.initialize:
             _initalize()
         if self.remove_existing_graph:
             # we remove the files that typically contain the graph definition
             pathlib.Path("zntrack.json").unlink(missing_ok=True)
             pathlib.Path("dvc.yaml").unlink(missing_ok=True)
             pathlib.Path("params.yaml").unlink(missing_ok=True)
@@ -87,34 +108,56 @@
         """Enter the graph context."""
         self.graph.__enter__(*args, **kwargs)
         return self
 
     def __exit__(self, *args, **kwargs):
         """Exit the graph context."""
         self.graph.__exit__(*args, **kwargs)
-        if not self.force:
-            self.update_node_names()
+        self.update_node_names()
 
-    def update_node_names(self):
+    def update_node_names(self, check=True):
         """Update the node names to be unique."""
         node_names = []
         for node_uuid in self.graph.get_sorted_nodes():
             node: Node = self.graph.nodes[node_uuid]["value"]
-            if self.automatic_node_names:
-                if node.name in node_names:
+            if node.name in node_names:
+                if self.automatic_node_names:
                     idx = 1
                     while f"{node.name}_{idx}" in node_names:
                         idx += 1
                     node.name = f"{node.name}_{idx}"
                     log.debug(f"Updating {node.name = }")
 
-            elif node.name in node_names:
-                raise exceptions.DuplicateNodeNameError(node)
+                elif not self.force and check:
+                    raise exceptions.DuplicateNodeNameError(node)
             node_names.append(node.name)
 
+    @contextlib.contextmanager
+    def group(self, name: str = None):
+        """Group nodes together.
+
+        Parameters
+        ----------
+        name : str, optional
+            The name of the group. If None, the group will be named 'GroupX' where X is
+            the number of groups + 1.
+        """
+        if name is None:
+            name = f"Group{len(self._groups) + 1}"
+        self._groups.append(name)
+
+        existing_nodes = self.graph.get_sorted_nodes()
+        try:
+            yield
+        finally:
+            for node_uuid in self.graph.get_sorted_nodes():
+                node: Node = self.graph.nodes[node_uuid]["value"]
+                if node_uuid not in existing_nodes:
+                    node.name = f"{name}_{node.name}"
+
     def run(
         self,
         eager=False,
         repro: bool = True,
         optional: dict = None,
         save: bool = True,
         environment: dict = None,
@@ -162,14 +205,22 @@
                 for x in cmd:
                     run_dvc_cmd(x)
                 node.save(results=False)
         if not eager and repro:
             run_dvc_cmd(["repro"])
             # TODO should we load the nodes here? Maybe, if lazy loading is implemented.
 
+    def build(self, environment: dict = None, optional: dict = None) -> None:
+        """Build the project graph without running it."""
+        self.run(repro=False, environment=environment, optional=optional)
+
+    def repro(self) -> None:
+        """Run dvc repro."""
+        run_dvc_cmd(["repro"])
+
     def _handle_environment(self, environment: dict):
         """Write global environment variables to the env.yaml file."""
         if environment is not None:
             file = pathlib.Path("env.yaml")
             try:
                 context = yaml.safe_load(file.read_text())
             except FileNotFoundError:
@@ -188,14 +239,22 @@
         """Get the nodes in the project."""
         nodes = {}
         for node_uuid in self.graph.get_sorted_nodes():
             node = self.graph.nodes[node_uuid]["value"]
             nodes[node.name] = node
         return nodes
 
+    def remove(self, name):
+        """Remove all nodes with the given name from the project."""
+        # TODO there should never be multiple nodes with the same name
+        for node_uuid in self.graph.get_sorted_nodes():
+            node = self.graph.nodes[node_uuid]["value"]
+            if node.name == name:
+                self.graph.remove_node(node_uuid)
+
     @property
     def nodes(self) -> dict[str, znflow.Node]:
         """Get the nodes in the project."""
         return self.get_nodes()
 
     def create_branch(self, name: str) -> "Branch":
         """Create a branch in the project."""
@@ -207,26 +266,52 @@
     def create_experiment(self, name: str = None, queue: bool = True) -> Experiment:
         """Create a new experiment."""
         # TODO: return an experiment object that allows you to load the results
         # TODO this context manager WILL NOT ADD new nodes to the graph.
 
         exp = Experiment(name, project=self)
 
-        yield exp
+        repo = git.Repo()
+        dirty = repo.is_dirty()
+        if dirty:
+            repo.git.stash("save", "--include-untracked")
+
+        force = self.force
+        self.force = True
+        with self:
+            yield exp
+        self.run(repro=False)  # save nodes and update dvc.yaml
+        self.force = force
 
-        for node_uuid in self.graph.get_sorted_nodes():
-            node: Node = self.graph.nodes[node_uuid]["value"]
-            node.save(results=False)
-
-        cmd = ["exp", "run"]
+        cmd = ["dvc", "exp", "run"]
         if queue:
             cmd.append("--queue")
         if name is not None:
             cmd.extend(["--name", name])
-        exp.name = capture_run_dvc_cmd(cmd).split("'")[1]
+        try:
+            proc = subprocess.run(cmd, capture_output=True, check=True)
+            # "Reproducing", "Experiment", "'exp-name'"
+            exp.name = proc.stdout.decode("utf-8").split()[2].replace("'", "")
+        finally:
+            repo.git.reset("--hard")
+            repo.git.clean("-fd")
+            if dirty:
+                repo.git.stash("pop")
+        if not queue:
+            exp.apply()
+
+    @property
+    def experiments(self, *args, **kwargs) -> dict[str, Experiment]:
+        """List all experiments."""
+        experiments = dvc.api.exp_show(*args, **kwargs)
+        return {
+            experiment["Experiment"]: Experiment(experiment["rev"], project=self)
+            for experiment in experiments
+            if experiment["Experiment"] is not None
+        }
 
     def run_exp(self, jobs: int = 1) -> None:
         """Run all queued experiments."""
         run_dvc_cmd(["exp", "run", "--run-all", "--jobs", str(jobs)])
 
     @property
     def branches(self):
@@ -237,28 +322,37 @@
 
 @dataclasses.dataclass
 class Experiment:
     """A DVC Experiment."""
 
     name: str
     project: Project
+    # TODO the project can not be used. The graph could be different.
+    #  Project must be loaded from rev.
+    # TODO name / rev / remote ...
 
     nodes: dict = dataclasses.field(default_factory=dict, init=False, repr=False)
 
+    def apply(self) -> None:
+        """Apply the experiment."""
+        run_dvc_cmd(["exp", "apply", self.name])
+
     def load(self) -> None:
         """Load the nodes from this experiment."""
         self.nodes = {
             name: node.from_rev(name=name, rev=self.name)
             for name, node in self.project.get_nodes().items()
         }
 
-    def __getitem__(self, key) -> Node:
+    def __getitem__(self, key: typing.Union[str, Node]) -> Node:
         """Get the Node from the experiment."""
         if len(self.nodes) == 0:
             self.load()
+        if isinstance(key, Node):
+            key = key.name
         return self.nodes[key]
 
 
 @dataclasses.dataclass
 class Branch:
     """The ZnTrack Branch class for managing experiments."""
```

### Comparing `zntrack-0.6.0a5/zntrack/tools/__init__.py` & `zntrack-0.6.1/zntrack/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.0a5/zntrack/utils/__init__.py` & `zntrack-0.6.1/zntrack/utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import enum
 import logging
 import os
 import pathlib
 import shutil
 import sys
 import tempfile
-import unittest.mock
 
 import dvc.cli
 
 from zntrack.utils import cli
 from zntrack.utils.config import config
 
 __all__ = [
@@ -54,14 +53,16 @@
     """
     if config.nb_name:
         try:
             return f"{config.nb_class_path}.{obj.__name__}"
         except AttributeError:
             return f"{config.nb_class_path}.{obj.__class__.__name__}"
     if obj.__module__ != "__main__":
+        if hasattr(obj, "_module_"):  # allow module override
+            return obj._module_
         return obj.__module__
     if pathlib.Path(sys.argv[0]).stem == "ipykernel_launcher":
         # special case for e.g. testing
         return obj.__module__
     return pathlib.Path(sys.argv[0]).stem
 
 
@@ -117,21 +118,14 @@
     # fix for https://github.com/iterative/dvc/issues/8631
     for logger_name, logger in logging.root.manager.loggerDict.items():
         if logger_name.startswith("zntrack"):
             logger.disabled = False
     return return_code
 
 
-def capture_run_dvc_cmd(script) -> str:
-    """Try to caputre the output of the DVC command."""
-    with unittest.mock.patch("dvc.ui.ui.write") as magic_mock:
-        run_dvc_cmd(script)
-    return magic_mock.call_args.args[0]
-
-
 def update_key_val(values, instance):
     """Update the keys {rev, remote} based on the instance state.
 
     If the value of keys is None, the value is updated based on the instance
     state. Otherwise, it is assumed the Node depends on a specific rev or remote.
     """
     if isinstance(values, (list, tuple)):
```

### Comparing `zntrack-0.6.0a5/zntrack/utils/cli.py` & `zntrack-0.6.1/zntrack/utils/cli.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.0a5/zntrack/utils/config.py` & `zntrack-0.6.1/zntrack/utils/config.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.0a5/zntrack/utils/file_io.py` & `zntrack-0.6.1/zntrack/utils/file_io.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,24 +58,25 @@
         file.write_text(yaml.safe_dump(value, indent=4))
     elif file.suffix == ".json":
         file.write_text(json.dumps(value, indent=4, cls=znjson.ZnEncoder))
     else:
         raise ValueError(f"File with suffix {file.suffix} is not supported")
 
 
-def clear_config_file(file: pathlib.Path, node_name: str):
+def clear_config_file(file: typing.Union[pathlib.Path, str], node_name: str):
     """Clear the entries in the files for the given node name.
 
     Parameters
     ----------
     file: pathlib.Path
         The file to read from, e.g. params.yaml / zntrack.json
     node_name: str
         The name of the Node
     """
+    file = pathlib.Path(file)
     try:
         file_content = read_file(file)
     except FileNotFoundError:
         file_content = {}
 
     _ = file_content.pop(node_name, None)
     write_file(file, value=file_content)
```

### Comparing `zntrack-0.6.0a5/zntrack/utils/node_wd.py` & `zntrack-0.6.1/zntrack/utils/node_wd.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.6.0a5/PKG-INFO` & `zntrack-0.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zntrack
-Version: 0.6.0a5
+Version: 0.6.1
 Summary: Create, Run and Benchmark DVC Pipelines in Python
 License: Apache-2.0
 Keywords: data-science,data-version-control,machine-learning,reproducibility,collaboration
 Author: zincwarecode
 Author-email: zincwarecode@gmail.com
 Requires-Python: >=3.8,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -34,115 +34,152 @@
 [![code-style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black/)
 [![Documentation](https://readthedocs.org/projects/zntrack/badge/?version=latest)](https://zntrack.readthedocs.io/en/latest/?badge=latest)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zincware/ZnTrack/HEAD)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6472850.svg)](https://doi.org/10.5281/zenodo.6472850)
 [![ZnTrack](https://img.shields.io/badge/Powered%20by-ZnTrack-%23007CB0)](https://zntrack.readthedocs.io/en/latest/)
 [![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
 
-
-
-
 ![Logo](https://raw.githubusercontent.com/zincware/ZnTrack/main/docs/source/_static/logo_ZnTrack.png)
 
 # ZnTrack: A Parameter Tracking Package for Python
 
-ZnTrack ``zɪŋk træk`` is a lightweight and easy-to-use package for tracking parameters in your Python projects using DVC.
-With ZnTrack, you can define parameters in Python classes and monitor how they change over time.
-This information can then be used to compare the results of different runs, identify computational bottlenecks, and avoid the re-running of code components where parameters have not changed.
+ZnTrack `zɪŋk træk` is a lightweight and easy-to-use package for tracking
+parameters in your Python projects using DVC. With ZnTrack, you can define
+parameters in Python classes and monitor how they change over time. This
+information can then be used to compare the results of different runs, identify
+computational bottlenecks, and avoid the re-running of code components where
+parameters have not changed.
 
 ## Key Features
-- Parameter, output and metric tracking: ZnTrack makes it easy to store and track the values of parameters in your Python code. It further allows you to store any outputs produced and gives an easy interface to define metrics.
-- Lightweight and database-free: Unlike other parameter tracking solutions, ZnTrack is lightweight and does not require any databases.
+
+- Parameter, output and metric tracking: ZnTrack makes it easy to store and
+  track the values of parameters in your Python code. It further allows you to
+  store any outputs produced and gives an easy interface to define metrics.
+- Lightweight and database-free: Unlike other parameter tracking solutions,
+  ZnTrack is lightweight and does not require any databases.
 
 ## Getting Started
-To get started with ZnTrack, you can install it via pip: ```pip install zntrack```
 
-Next, you can start using ZnTrack to track parameters, outputs and metrics in your Python code.
-Here's an example of how to use ZnTrack to track the value of a parameter in a Python class.
-Start in an empty directory and run ``git init`` and ``dvc init`` for preparation.
+To get started with ZnTrack, you can install it via pip: `pip install zntrack`
 
-Then put the following into a python file called `hello_world.py` and call it with `python hello_world.py`.
+Next, you can start using ZnTrack to track parameters, outputs and metrics in
+your Python code. Here's an example of how to use ZnTrack to track the value of
+a parameter in a Python class. Start in an empty directory and run `git init`
+and `dvc init` for preparation.
+
+Then put the following into a python file called `hello_world.py` and call it
+with `python hello_world.py`.
 
 ```python
-from zntrack import Node, zn
+import zntrack
 from random import randrange
 
 
-class HelloWorld(Node):
+class HelloWorld(zntrack.Node):
     """Define a ZnTrack Node"""
     # parameter to be tracked
-    max_number: int = zn.params()
+    max_number: int = zntrack.zn.params()
     # parameter to store as output
-    random_number: int = zn.outs()
-    
+    random_number: int = zntrack.zn.outs()
+
     def run(self):
         """Command to be run by DVC"""
         self.random_number = randrange(self.max_number)
-        
+
 if __name__ == "__main__":
     # Write the computational graph
     with zntrack.Project() as project:
         hello_world = HelloWorld(max_number=512)
     project.run()
 ```
 
-This will create a [DVC](https://dvc.org) stage ``HelloWorld``.
-The workflow is defined in ``dvc.yaml`` and the parameters are stored in ``params.yaml``.
+This will create a [DVC](https://dvc.org) stage `HelloWorld`. The workflow is
+defined in `dvc.yaml` and the parameters are stored in `params.yaml`.
+
+This will run the workflow with `dvc repro` automatically. Once the graph is
+executed, the results, i.e. the random number can be accessed directly by the
+Node object.
 
-This will run the workflow with ``dvc repro`` automatically.
-Once the graph is executed, the results, i.e. the random number can be accessed directly by the Node object.
 ```python
 hello_world.load()
-print(hello_world.random_numer)
+print(hello_world.random_number)
 ```
-An overview of all the ZnTrack features as well as more detailed examples can be found in the [ZnTrack Documentation](https://zntrack.readthedocs.io/en/latest/).
+
+> ## Tip
+>
+> You can easily load this Node directly from a repository.
+>
+> ```python
+> import zntrack
+>
+> node = zntrack.from_rev(
+>     "HelloWorld",
+>     remote="https://github.com/PythonFZ/ZnTrackExamples.git",
+>     rev="b9316bf",
+> )
+> ```
+>
+> Try accessing the `max_number` parameter and `random_number` output. All Nodes
+> from this and many other repositories can be loaded like this.
+
+An overview of all the ZnTrack features as well as more detailed examples can be
+found in the [ZnTrack Documentation](https://zntrack.readthedocs.io/en/latest/).
 
 ## Wrap Python Functions
-ZnTrack also provides tools to convert a Python function into a DVC Node.
-This approach is much more lightweight compared to the class-based approach with only a reduced set of functionality.
-Therefore, it is recommended for smaller nodes that do not need the additional toolset that the class-based approach provides.
 
-````python
+ZnTrack also provides tools to convert a Python function into a DVC Node. This
+approach is much more lightweight compared to the class-based approach with only
+a reduced set of functionality. Therefore, it is recommended for smaller nodes
+that do not need the additional toolset that the class-based approach provides.
+
+```python
 from zntrack import nodify, NodeConfig
 import pathlib
 
 @nodify(outs=pathlib.Path("text.txt"), params={"text": "Lorem Ipsum"})
 def write_text(cfg: NodeConfig):
     cfg.outs.write_text(
         cfg.params.text
     )
 # build the DVC graph
 with zntrack.Project() as project:
     write_text()
 project.run()
-````
+```
 
-The ``cfg`` dataclass passed to the function provides access to all configured files
-and parameters via [dot4dict](https://github.com/zincware/dot4dict). The function body
-will be executed by the ``dvc repro`` command or if ran via `write_text(run=True)`.
-All parameters are loaded from or stored in ``params.yaml``.
+The `cfg` dataclass passed to the function provides access to all configured
+files and parameters via [dot4dict](https://github.com/zincware/dot4dict). The
+function body will be executed by the `dvc repro` command or if ran via
+`write_text(run=True)`. All parameters are loaded from or stored in
+`params.yaml`.
 
 # Technical Details
 
-
 ## ZnTrack as an Object-Relational Mapping for DVC
 
-On a fundamental level the ZnTrack package provides an easy-to-use interface for DVC directly from Python.
-It handles all the computational overhead of reading config files, defining outputs in the `dvc.yaml` as well as in the script and much more.
+On a fundamental level the ZnTrack package provides an easy-to-use interface for
+DVC directly from Python. It handles all the computational overhead of reading
+config files, defining outputs in the `dvc.yaml` as well as in the script and
+much more.
 
 For more information on DVC visit their [homepage](https://dvc.org/doc).
 
-Copyright
-=========
+# Copyright
 
-This project is distributed under the [Apache License Version 2.0](https://github.com/zincware/ZnTrack/blob/main/LICENSE).
+This project is distributed under the
+[Apache License Version 2.0](https://github.com/zincware/ZnTrack/blob/main/LICENSE).
 
 ## Similar Tools
-The following (incomplete) list of other projects that either work together with ZnTrack or can achieve similar results with slightly different goals or programming languages.
+
+The following (incomplete) list of other projects that either work together with
+ZnTrack or can achieve similar results with slightly different goals or
+programming languages.
 
 - [DVC](https://dvc.org/) - Main dependency of ZnTrack for Data Version Control.
 - [dvthis](https://github.com/jcpsantiago/dvthis) - Introduce DVC to R.
-- [DAGsHub Client](https://github.com/DAGsHub/client) - Logging parameters from within .Python 
+- [DAGsHub Client](https://github.com/DAGsHub/client) - Logging parameters from
+  within .Python
 - [MLFlow](https://mlflow.org/) - A Machine Learning Lifecycle Platform.
 - [Metaflow](https://metaflow.org/) - A framework for real-life data science.
-- [Hydra](https://hydra.cc/) - A framework for elegantly configuring complex applications
+- [Hydra](https://hydra.cc/) - A framework for elegantly configuring complex
+  applications
```

