# Comparing `tmp/banana_hep-0.6.8.tar.gz` & `tmp/banana_hep-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "banana_hep-0.6.8.tar", max compression
+gzip compressed data, was "banana_hep-0.6.9.tar", max compression
```

## Comparing `banana_hep-0.6.8.tar` & `banana_hep-0.6.9.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0    35149 2023-02-13 15:02:26.688887 banana_hep-0.6.8/LICENSE
--rw-r--r--   0        0        0     1295 2023-02-13 15:02:26.688887 banana_hep-0.6.8/README.md
--rw-r--r--   0        0        0     2930 2023-02-13 15:03:00.476568 banana_hep-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     1077 2023-02-13 15:03:00.476568 banana_hep-0.6.8/src/banana/__init__.py
--rw-r--r--   0        0        0        0 2023-02-13 15:02:26.704887 banana_hep-0.6.8/src/banana/benchmark/__init__.py
--rw-r--r--   0        0        0        0 2023-02-13 15:02:26.704887 banana_hep-0.6.8/src/banana/benchmark/external/__init__.py
--rw-r--r--   0        0        0     4628 2023-02-13 15:02:26.704887 banana_hep-0.6.8/src/banana/benchmark/external/apfel_utils.py
--rw-r--r--   0        0        0     3142 2023-02-13 15:02:26.704887 banana_hep-0.6.8/src/banana/benchmark/external/apfel_xgrid.yaml
--rw-r--r--   0        0        0    11289 2023-02-13 15:02:26.704887 banana_hep-0.6.8/src/banana/benchmark/runner.py
--rw-r--r--   0        0        0     3024 2023-02-13 15:02:26.704887 banana_hep-0.6.8/src/banana/cfg.py
--rw-r--r--   0        0        0        6 2023-02-13 15:02:26.704887 banana_hep-0.6.8/src/banana/data/.gitignore
--rw-r--r--   0        0        0      578 2023-02-13 15:02:26.704887 banana_hep-0.6.8/src/banana/data/__init__.py
--rw-r--r--   0        0        0     3496 2023-02-13 15:02:26.704887 banana_hep-0.6.8/src/banana/data/db.py
--rw-r--r--   0        0        0     3684 2023-02-13 15:02:26.704887 banana_hep-0.6.8/src/banana/data/dfdict.py
--rw-r--r--   0        0        0     8076 2023-02-13 15:02:26.704887 banana_hep-0.6.8/src/banana/data/sql.py
--rw-r--r--   0        0        0      768 2023-02-13 15:02:26.704887 banana_hep-0.6.8/src/banana/data/theories.py
--rw-r--r--   0        0        0      692 2023-02-13 15:02:26.704887 banana_hep-0.6.8/src/banana/data/theory_template.yaml
--rw-r--r--   0        0        0     3268 2023-02-13 15:02:26.704887 banana_hep-0.6.8/src/banana/navigator/__init__.py
--rw-r--r--   0        0        0    17061 2023-02-13 15:02:26.704887 banana_hep-0.6.8/src/banana/navigator/navigator.py
--rw-r--r--   0        0        0     3778 2023-02-13 15:02:26.704887 banana_hep-0.6.8/src/banana/navigator/table_manager.py
--rw-r--r--   0        0        0     1495 2023-02-13 15:02:26.704887 banana_hep-0.6.8/src/banana/navigator/utils.py
--rw-r--r--   0        0        0     4188 2023-02-13 15:02:26.704887 banana_hep-0.6.8/src/banana/toy.py
--rw-r--r--   0        0        0      319 2023-02-13 15:02:26.704887 banana_hep-0.6.8/src/banana/utils.py
--rw-r--r--   0        0        0     2542 1970-01-01 00:00:00.000000 banana_hep-0.6.8/setup.py
--rw-r--r--   0        0        0     2699 1970-01-01 00:00:00.000000 banana_hep-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-15 14:30:38.503130 banana_hep-0.6.9/LICENSE
+-rw-r--r--   0        0        0     1295 2023-06-15 14:30:38.503130 banana_hep-0.6.9/README.md
+-rw-r--r--   0        0        0     2729 2023-06-15 14:31:16.751904 banana_hep-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     1053 2023-06-15 14:31:16.755904 banana_hep-0.6.9/src/banana/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 14:30:38.515130 banana_hep-0.6.9/src/banana/benchmark/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 14:30:38.515130 banana_hep-0.6.9/src/banana/benchmark/external/__init__.py
+-rw-r--r--   0        0        0     4599 2023-06-15 14:30:38.515130 banana_hep-0.6.9/src/banana/benchmark/external/apfel_utils.py
+-rw-r--r--   0        0        0     3142 2023-06-15 14:30:38.515130 banana_hep-0.6.9/src/banana/benchmark/external/apfel_xgrid.yaml
+-rw-r--r--   0        0        0    11263 2023-06-15 14:30:38.515130 banana_hep-0.6.9/src/banana/benchmark/runner.py
+-rw-r--r--   0        0        0     2995 2023-06-15 14:30:38.515130 banana_hep-0.6.9/src/banana/cfg.py
+-rw-r--r--   0        0        0        6 2023-06-15 14:30:38.515130 banana_hep-0.6.9/src/banana/data/.gitignore
+-rw-r--r--   0        0        0      554 2023-06-15 14:30:38.515130 banana_hep-0.6.9/src/banana/data/__init__.py
+-rw-r--r--   0        0        0     3471 2023-06-15 14:30:38.515130 banana_hep-0.6.9/src/banana/data/db.py
+-rw-r--r--   0        0        0     3659 2023-06-15 14:30:38.515130 banana_hep-0.6.9/src/banana/data/dfdict.py
+-rw-r--r--   0        0        0     8052 2023-06-15 14:30:38.515130 banana_hep-0.6.9/src/banana/data/sql.py
+-rw-r--r--   0        0        0      745 2023-06-15 14:30:38.515130 banana_hep-0.6.9/src/banana/data/theories.py
+-rw-r--r--   0        0        0      692 2023-06-15 14:30:38.515130 banana_hep-0.6.9/src/banana/data/theory_template.yaml
+-rw-r--r--   0        0        0     3244 2023-06-15 14:30:38.515130 banana_hep-0.6.9/src/banana/navigator/__init__.py
+-rw-r--r--   0        0        0    17037 2023-06-15 14:30:38.515130 banana_hep-0.6.9/src/banana/navigator/navigator.py
+-rw-r--r--   0        0        0     3753 2023-06-15 14:30:38.515130 banana_hep-0.6.9/src/banana/navigator/table_manager.py
+-rw-r--r--   0        0        0     1471 2023-06-15 14:30:38.515130 banana_hep-0.6.9/src/banana/navigator/utils.py
+-rw-r--r--   0        0        0     4164 2023-06-15 14:30:38.515130 banana_hep-0.6.9/src/banana/toy.py
+-rw-r--r--   0        0        0      295 2023-06-15 14:30:38.515130 banana_hep-0.6.9/src/banana/utils.py
+-rw-r--r--   0        0        0     2410 1970-01-01 00:00:00.000000 banana_hep-0.6.9/PKG-INFO
```

### Comparing `banana_hep-0.6.8/LICENSE` & `banana_hep-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `banana_hep-0.6.8/README.md` & `banana_hep-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `banana_hep-0.6.8/pyproject.toml` & `banana_hep-0.6.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "banana-hep"
-version = "0.6.8"
+version = "0.6.9"
 description = "Benchmark QCD physics"
 readme = "README.md"
 authors = [
   "Andrea Barontini <andrea.barontini@mi.infn.it>",
   "Alessandro Candido <alessandro.candido@mi.infn.it>",
   "Felix Hekhorn <felix.hekhorn@mi.infn.it>",
   "Niccolò Laurenti <niccolo.laurenti@mi.infn.it>",
@@ -25,77 +25,77 @@
   "src/banana/data/theory_template.yaml",
 ]
 packages = [{ include = "banana", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.8.0,<3.12"
 ipython = "^8.1.0"
-SQLAlchemy = "^1.4.29"
+SQLAlchemy = "^1.4.29,<=2.0"
 numpy = "^1.21.0"
 pandas = "^1.3.5"
 matplotlib = "^3.5.1"
 rich = "^12.4.4"
 PyYAML = "^6.0"
 click = "^8.0.3"
 pendulum = "^2.1.2"
-# docs dependencies (for readthedocs)
-Sphinx = { version = "^4.3.2", optional = true }
-sphinx-rtd-theme = { version = "^1.0.0", optional = true }
-sphinxcontrib-bibtex = { version = "^2.4.1", optional = true }
 appdirs = "^1.4.4"
 
-[tool.poetry.dev-dependencies]
-pdbpp = "^0.10.3"
-pylint = "^2.12.2"
-pytest = "^6.2.5"
-pytest-cov = "^3.0.0"
-pytest-env = "^0.6.2"
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
 Sphinx = "^4.3.2"
 sphinx-rtd-theme = "^1.0.0"
 sphinxcontrib-bibtex = "^2.4.1"
+
+[tool.poetry.group.test]
+optional = true
+
+[tool.poetry.group.test.dependencies]
+pytest = "^7.1.3"
+pytest-cov = "4.0.0"
+pylint = "^2.12.2"
 pyfakefs = "^4.5.3"
 
-[tool.poetry.extras]
-pineappl = ["pineappl"]
-docs = ["sphinx", "sphinx-rtd-theme", "sphinxcontrib-bibtex"]
+[tool.poetry.group.dev.dependencies]
+pdbpp = "^0.10.3"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 dirty = true
 
 [tool.poetry-dynamic-versioning.substitution]
 files = ["src/banana/__init__.py"]
 
 [tool.poe.tasks]
 coverage = "$BROWSER htmlcov/index.html"
 test = "pytest tests"
 test-cov = ["test", "coverage"]
-lint = "pylint src/ -E"
-lint-warnings = "pylint src/ --exit-zero"
+lint = "pylint src/**/*.py -E"
+lint-warnings = "pylint src/**/*.py --exit-zero"
 docs = { "shell" = "cd docs; make html" }
 docs-view = { "shell" = "cd docs; make view" }
 docs-server = { "shell" = "cd docs; make server" }
 docs-clean = { "shell" = "cd docs; make clean" }
 docs-cleanall = { "shell" = "cd docs; make cleanall" }
 
 [tool.pytest.ini_options]
 addopts = [
   '--cov=banana',
   '--cov-report=html',
   '--cov-report=xml',
   '--strict-markers',
 ]
-env = ["NUMBA_DISABLE_JIT=1"]
 
 [tool.pylint.master]
 # extensions not to check
-extension-pkg-whitelist = ["numpy", "numba", "lhapdf", "pegasus"]
-ignore-paths = ["benchmarks/", "doc/", "tests/"]
+extension-pkg-whitelist = ["numpy", "lhapdf"]
+ignore-paths = ["benchmarks/", "docs/", "tests/"]
 # has to be 1 as pylint is NOT threadsafe
 jobs = 1
 [tool.pylint.messages_control]
 disable = ["invalid-name", "fixme"]
 [tool.pylint.reports]
 # Available formats are:
 # text, parseable, colorized, json and msvs (visual studio).
```

### Comparing `banana_hep-0.6.8/src/banana/__init__.py` & `banana_hep-0.6.9/src/banana/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 import pathlib
 
 from . import cfg
 
-__version__ = "0.6.8"
+__version__ = "0.6.9"
 
 
 def register(path):
     """Register configurations.
 
     This function is provided for its simple heuristics for configuration file
     detection.
```

### Comparing `banana_hep-0.6.8/src/banana/benchmark/external/apfel_utils.py` & `banana_hep-0.6.9/src/banana/benchmark/external/apfel_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# -*- coding: utf-8 -*-
-from math import isnan
+import numpy as np
+
 
 def load_apfel(theory, ocard, pdf, use_external_grid=True):
     """
     Set APFEL parameter from ``theory`` dictionary.
 
     Parameters
     ----------
@@ -43,17 +43,17 @@
         apfel.SetAlphaEvolution("expanded")
     else:
         raise RuntimeError("ERROR: Unrecognised MODEV:", theory.get("ModEv"))
 
     # Coupling
     apfel.SetAlphaQCDRef(theory.get("alphas"), theory.get("Qref"))
     if theory.get("QED"):
-        if isnan(theory.get("QrefQED")) or not theory.get("QrefQED"):
+        if not np.isclose(theory.get("Qedref"), theory.get("Qref")):
             raise ValueError("Fixed alphaqed is not implemented in APFEL!")
-        apfel.SetAlphaQEDRef(theory.get("alphaqed"), theory.get("QrefQED"))
+        apfel.SetAlphaQEDRef(theory.get("alphaqed"), theory.get("Qedref"))
 
     # EW
     apfel.SetWMass(theory.get("MW"))
     apfel.SetZMass(theory.get("MZ"))
     apfel.SetGFermi(theory["GF"])
     apfel.SetSin2ThetaW(theory["SIN2TW"])
```

### Comparing `banana_hep-0.6.8/src/banana/benchmark/external/apfel_xgrid.yaml` & `banana_hep-0.6.9/src/banana/benchmark/external/apfel_xgrid.yaml`

 * *Files identical despite different names*

### Comparing `banana_hep-0.6.8/src/banana/benchmark/runner.py` & `banana_hep-0.6.9/src/banana/benchmark/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 import abc
 import hashlib
 import itertools
 import pathlib
 import pickle
 import subprocess
 from collections.abc import Iterable
@@ -84,15 +82,14 @@
 
 
 default_log = {"t_hash": b"", "o_hash": b"", "pdf": "", "external": "", "log": b""}
 default_log = dict(sorted(default_log.items()))
 
 
 class BenchmarkRunner:
-
     banana_cfg = {}
     """Global configuration"""
 
     external = ""
     """External reference program name"""
 
     console = rich.console.Console()
```

### Comparing `banana_hep-0.6.8/src/banana/cfg.py` & `banana_hep-0.6.9/src/banana/cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Configurations related objects.
 
 This module contains the functions used to manage configurations.
 Moreover, the actual loaded configurations are stored in the module variable
 :data:`cfg`, that is used as the source of truth for them.
 
 """
@@ -96,15 +95,15 @@
     Returns
     -------
     dict
         loaded configurations
 
     """
     cfg = {}
-    with open(path, "r", encoding="utf-8") as o:
+    with open(path, encoding="utf-8") as o:
         cfg = yaml.safe_load(o)
 
     try:
         root = pathlib.Path(cfg["root"])
         if not root.is_absolute():
             root = pathlib.Path(path).parent / root
     except KeyError:
```

### Comparing `banana_hep-0.6.8/src/banana/data/__init__.py` & `banana_hep-0.6.9/src/banana/data/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 Module to collect utilites to help with the data generation:
 """
 import itertools
 
 
 def cartesian_product(inp):
```

### Comparing `banana_hep-0.6.8/src/banana/data/db.py` & `banana_hep-0.6.9/src/banana/data/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 Actually using ``String`` it's pointless, since SQLite has only one text type
 and it is ``TEXT``, and the maximum length is coherently ignored by SQLite.
 Nevertheless the information is stored in the DB, even if the DBMS won't use it,
 so we can keep declaring a size for fields where it matters.
 
 Same considerations apply to datetime, with the further gain that SQLite it's
@@ -52,15 +51,15 @@
     Q0 = Column(Float)
     QED = Column(Integer)
     nfref = Column(Integer)
     Qmb = Column(Float)
     Qmc = Column(Float)
     Qmt = Column(Float)
     Qref = Column(Float)
-    QrefQED = Column(Float)
+    Qedref = Column(Float)
     SIN2TW = Column(Float)
     SxOrd = Column(Text)
     SxRes = Column(Integer)
     TMC = Column(Integer)
     XIF = Column(Float)
     XIR = Column(Float)
     alphaqed = Column(Float)
```

### Comparing `banana_hep-0.6.8/src/banana/data/dfdict.py` & `banana_hep-0.6.9/src/banana/data/dfdict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 import pandas as pd
 import rich
 import rich.box
 import rich.markdown
 import rich.panel
```

### Comparing `banana_hep-0.6.8/src/banana/data/sql.py` & `banana_hep-0.6.9/src/banana/data/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 import copy
 import hashlib
 import pickle
 from datetime import datetime, timezone
 
 import numpy as np
 import pandas as pd
```

### Comparing `banana_hep-0.6.8/src/banana/data/theories.py` & `banana_hep-0.6.9/src/banana/data/theories.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# -*- coding: utf-8 -*-
 import pathlib
 
 import yaml
 
 from . import db, sql
 
 _here = pathlib.Path(__file__).parent
 
 # load default theory
 default_card = {}
 with open(_here / "theory_template.yaml", encoding="utf-8") as f:
     default_card = yaml.safe_load(f)
 default_card = dict(sorted(default_card.items()))
 
+
 # db interface
 def load(session, updates):
     """Load theories.
 
     Parameters
     ----------
     session : sqlalchemy.orm.session.Session
```

### Comparing `banana_hep-0.6.8/src/banana/data/theory_template.yaml` & `banana_hep-0.6.9/src/banana/data/theory_template.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 fact_to_ren_scale_ratio: 1.0
 NfFF: 3
 MaxNfAs: 6
 MaxNfPdf: 6
 Q0: 1.0
 alphas: 0.11800000000000001
 Qref: 91.2
-QrefQED: 91.2
+Qedref: 91.2
 nfref: null
 nf0: null
 QED: 0
 alphaqed: 0.007496251999999999
 SxRes: 0
 SxOrd: "LL"
 HQ: "POLE"
@@ -42,8 +42,8 @@
 SIN2TW: 0.23126
 TMC: 0
 MP: 0.938
 Comments: "LO baseline for small-x res"
 global_nx: 0
 EScaleVar: 1
 ModSV: null
-n3lo_ad_variation: [0,0,0,0]
+n3lo_ad_variation: [0,0,0,0]
```

### Comparing `banana_hep-0.6.8/src/banana/navigator/__init__.py` & `banana_hep-0.6.9/src/banana/navigator/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 import inspect
 
 import IPython
 from traitlets.config import loader
 
 from .. import cfg
 from .navigator import c, l, o, t
```

### Comparing `banana_hep-0.6.8/src/banana/navigator/navigator.py` & `banana_hep-0.6.9/src/banana/navigator/navigator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 import abc
 import datetime as dt
 import textwrap
 
 import numpy as np
 import pandas as pd
 import pendulum
```

### Comparing `banana_hep-0.6.8/src/banana/navigator/table_manager.py` & `banana_hep-0.6.9/src/banana/navigator/table_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 from ..data import sql
 
 
 class TableManager:
     """
     Wrapper to a single table
```

### Comparing `banana_hep-0.6.8/src/banana/navigator/utils.py` & `banana_hep-0.6.9/src/banana/navigator/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 def compare_dicts(
     d1, d2, exclude_underscored=False, key_width=20, value_width=30, exclude_keys=None
 ):
     """Compare similar dictionaries.
 
     Check which entries of the two dictionaries are different, and output the
     values.
```

### Comparing `banana_hep-0.6.8/src/banana/toy.py` & `banana_hep-0.6.9/src/banana/toy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# -*- coding: utf-8 -*-
 """
 This module contains the Toy PDF.
 
 It is defined at the initial scale :math:`Q = sqrt(2) GeV`.
 """
 
 
 class toyPDFSet:
     """Fake PDF set"""
+
     def __init__(self, name):
         self.name = name
 
 
-class MockPDF():
+class MockPDF:
     """Imitates a lhapdf.PDF"""
 
     name = None
     xpdf = {}
 
     def xfxQ2(self, pid, x, _Q2):
         """Get the PDF xf(x) value at (x,q2) for the given PID.
@@ -80,14 +80,15 @@
         "Return the corresponding PDFSet"
         return toyPDFSet(self.name)
 
     def hasFlavor(self, pid):
         """Contains a pdf for pid?"""
         return pid in ([21, 22] + list(range(-6, 6 + 1)))
 
+
 class toyPDF_unpolarized(MockPDF):
     """ToyLH unpolarized implementation."""
 
     def __init__(self):
         N_uv = 5.107200e0
         auv = 0.8e0
         buv = 3e0
```

### Comparing `banana_hep-0.6.8/PKG-INFO` & `banana_hep-0.6.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,33 @@
 Metadata-Version: 2.1
 Name: banana-hep
-Version: 0.6.8
+Version: 0.6.9
 Summary: Benchmark QCD physics
 Home-page: https://github.com/N3PDF/banana
 Author: Andrea Barontini
 Author-email: andrea.barontini@mi.infn.it
 Requires-Python: >=3.8.0,<3.12
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
-Provides-Extra: docs
-Provides-Extra: pineappl
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: SQLAlchemy (>=1.4.29,<2.0.0)
-Requires-Dist: Sphinx (>=4.3.2,<5.0.0) ; extra == "docs"
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: click (>=8.0.3,<9.0.0)
 Requires-Dist: ipython (>=8.1.0,<9.0.0)
 Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
 Requires-Dist: pandas (>=1.3.5,<2.0.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: rich (>=12.4.4,<13.0.0)
-Requires-Dist: sphinx-rtd-theme (>=1.0.0,<2.0.0) ; extra == "docs"
-Requires-Dist: sphinxcontrib-bibtex (>=2.4.1,<3.0.0) ; extra == "docs"
 Project-URL: Repository, https://github.com/N3PDF/banana
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://n3pdf.github.io/banana/"><img alt="Banana" src="https://raw.githubusercontent.com/N3PDF/banana/main/docs/_assets/logo.png" width=700></a>
 </p>
```

#### html2text {}

```diff
@@ -1,24 +1,20 @@
-Metadata-Version: 2.1 Name: banana-hep Version: 0.6.8 Summary: Benchmark QCD
+Metadata-Version: 2.1 Name: banana-hep Version: 0.6.9 Summary: Benchmark QCD
 physics Home-page: https://github.com/N3PDF/banana Author: Andrea Barontini
 Author-email: andrea.barontini@mi.infn.it Requires-Python: >=3.8.0,<3.12
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Physics Provides-Extra: docs
-Provides-Extra: pineappl Requires-Dist: PyYAML (>=6.0,<7.0) Requires-Dist:
-SQLAlchemy (>=1.4.29,<2.0.0) Requires-Dist: Sphinx (>=4.3.2,<5.0.0) ; extra ==
-"docs" Requires-Dist: appdirs (>=1.4.4,<2.0.0) Requires-Dist: click
+Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Physics Requires-Dist: PyYAML (>=6.0,<7.0) Requires-Dist: SQLAlchemy
+(>=1.4.29,<2.0.0) Requires-Dist: appdirs (>=1.4.4,<2.0.0) Requires-Dist: click
 (>=8.0.3,<9.0.0) Requires-Dist: ipython (>=8.1.0,<9.0.0) Requires-Dist:
 matplotlib (>=3.5.1,<4.0.0) Requires-Dist: numpy (>=1.21.0,<2.0.0) Requires-
 Dist: pandas (>=1.3.5,<2.0.0) Requires-Dist: pendulum (>=2.1.2,<3.0.0)
-Requires-Dist: rich (>=12.4.4,<13.0.0) Requires-Dist: sphinx-rtd-theme
-(>=1.0.0,<2.0.0) ; extra == "docs" Requires-Dist: sphinxcontrib-bibtex
-(>=2.4.1,<3.0.0) ; extra == "docs" Project-URL: Repository, https://github.com/
-N3PDF/banana Description-Content-Type: text/markdown
+Requires-Dist: rich (>=12.4.4,<13.0.0) Project-URL: Repository, https://
+github.com/N3PDF/banana Description-Content-Type: text/markdown
                                    [Banana]
    [Tests] [Documentation_Status] [PyPI] [DOI] [https://codecov.io/gh/N3PDF/
        banana/branch/main/graph/badge.svg?token=L9XIAXV77R] [CodeFactor]
 # banana: Benchmarking AgaiNst Apfel aNd Anything This is the base package of
 ekomark and yadmark
```

