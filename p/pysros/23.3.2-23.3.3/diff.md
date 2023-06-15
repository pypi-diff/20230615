# Comparing `tmp/pysros-23.3.2.tar.gz` & `tmp/pysros-23.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysros-23.3.2.tar", last modified: Thu Apr 27 23:30:05 2023, max compression
+gzip compressed data, was "pysros-23.3.3.tar", last modified: Thu Jun  1 23:31:46 2023, max compression
```

## Comparing `pysros-23.3.2.tar` & `pysros-23.3.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:30:05.853163 pysros-23.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    17026 2023-04-27 23:29:55.000000 pysros-23.3.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-04-27 23:30:05.853163 pysros-23.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-27 23:29:55.000000 pysros-23.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:30:05.849163 pysros-23.3.2/pysros/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    58667 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/management.py
--rw-r--r--   0 runner    (1001) docker     (123)    20960 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31717 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/model_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    21078 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/model_walker.py
--rw-r--r--   0 runner    (1001) docker     (123)    26080 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    46775 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/request_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/yang_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:30:05.853163 pysros-23.3.2/pysros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-04-27 23:30:05.000000 pysros-23.3.2/pysros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-27 23:30:05.000000 pysros-23.3.2/pysros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:30:05.000000 pysros-23.3.2/pysros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-27 23:30:05.000000 pysros-23.3.2/pysros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 23:30:05.000000 pysros-23.3.2/pysros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 23:30:05.853163 pysros-23.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-27 23:29:55.000000 pysros-23.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:31:46.587482 pysros-23.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    17026 2023-06-01 23:31:33.000000 pysros-23.3.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-01 23:31:46.587482 pysros-23.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-01 23:31:33.000000 pysros-23.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:31:46.587482 pysros-23.3.3/pysros/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58672 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20965 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31722 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/model_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21083 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/model_walker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26085 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46780 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/request_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/yang_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:31:46.587482 pysros-23.3.3/pysros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-01 23:31:46.000000 pysros-23.3.3/pysros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-01 23:31:46.000000 pysros-23.3.3/pysros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 23:31:46.000000 pysros-23.3.3/pysros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 23:31:46.000000 pysros-23.3.3/pysros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 23:31:46.000000 pysros-23.3.3/pysros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 23:31:46.587482 pysros-23.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-01 23:31:33.000000 pysros-23.3.3/setup.py
```

### Comparing `pysros-23.3.2/LICENSE.md` & `pysros-23.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pysros-23.3.2/PKG-INFO` & `pysros-23.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pysros
-Version: 23.3.2
+Version: 23.3.3
 Summary: Python for the Nokia Service Router Operating Systems (pySROS)
 Home-page: https://www.nokia.com
 Author: Nokia
 Author-email: 
-License: Copyright 2021 Nokia.  License available in the LICENSE.md file.
+License: Copyright 2021-2023 Nokia.  License available in the LICENSE.md file.
 Project-URL: Documentation, https://network.developer.nokia.com/static/sr/learn/pysros/latest/
 Project-URL: Source, https://github.com/nokia/pysros
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet
 Classifier: Development Status :: 5 - Production/Stable
@@ -43,15 +43,15 @@
     - With NETCONF enabled and accessible by an authorized user (to execute applications
     remotely)
 - A Python 3 interpreter of version 3.6 or newer when using the pySROS library to
   execute applications remotely
 
 ## License ##
 
-Copyright 2021 Nokia.
+Copyright 2021-2023 Nokia.
 
 The license is located [here](LICENSE.md).
 
 ## Reporting issues ##
 
 Issues, suggestions, and enhancements are welcome.  Please use the Nokia support
 process.  Issues raised in GitHub may be considered for inclusion into the project
```

### Comparing `pysros-23.3.2/README.md` & `pysros-23.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     - With NETCONF enabled and accessible by an authorized user (to execute applications
     remotely)
 - A Python 3 interpreter of version 3.6 or newer when using the pySROS library to
   execute applications remotely
 
 ## License ##
 
-Copyright 2021 Nokia.
+Copyright 2021-2023 Nokia.
 
 The license is located [here](LICENSE.md).
 
 ## Reporting issues ##
 
 Issues, suggestions, and enhancements are welcome.  Please use the Nokia support
 process.  Issues raised in GitHub may be considered for inclusion into the project
```

### Comparing `pysros-23.3.2/pysros/errors.py` & `pysros-23.3.3/pysros/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Nokia
+# Copyright 2021-2023 Nokia
 
 from .exceptions import *
 from .exceptions import make_exception
 
 __doc__ = """This module contains error definitions for pySROS.
 
 .. reviewed by PLM 20211201
```

### Comparing `pysros-23.3.2/pysros/exceptions.py` & `pysros-23.3.3/pysros/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Nokia
+# Copyright 2021-2023 Nokia
 
 __all__ = ("SrosMgmtError", "InvalidPathError", "ModelProcessingError", "InternalError", "SrosConfigConflictError", "ActionTerminatedIncompleteError", "JsonDecodeError", "XmlDecodeError", )
 
 __doc__ = """This module contains exceptions for error handling within pySROS.
 
 .. reviewed by PLM 20211201
 .. reviewed by TechComms 20211202
```

### Comparing `pysros-23.3.2/pysros/identifier.py` & `pysros-23.3.3/pysros/identifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Nokia
+# Copyright 2021-2023 Nokia
 
 import re
 
 from .errors import *
 from .singleton import _Singleton
 
 class LazyBindModule(metaclass=_Singleton):
```

### Comparing `pysros-23.3.2/pysros/management.py` & `pysros-23.3.3/pysros/management.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Nokia
+# Copyright 2021-2023 Nokia
 
 import base64
 import contextlib
 import datetime
 import hashlib
 import os.path
 import pathlib
```

### Comparing `pysros-23.3.2/pysros/model.py` & `pysros-23.3.3/pysros/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Nokia
+# Copyright 2021-2023 Nokia
 
 import copy
 import locale
 import sys
 
 from enum import Enum, IntFlag, IntEnum, auto
 from typing import Any, Dict, List, Optional, Tuple
```

### Comparing `pysros-23.3.2/pysros/model_builder.py` & `pysros-23.3.3/pysros/model_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Nokia
+# Copyright 2021-2023 Nokia
 
 import copy
 import xml.parsers.expat
 
 from collections import defaultdict
 from typing import Dict, DefaultDict, List, Set, Union, Optional
```

### Comparing `pysros-23.3.2/pysros/model_path.py` & `pysros-23.3.3/pysros/model_path.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Nokia
+# Copyright 2021-2023 Nokia
 
 from typing import Dict, Iterable
 
 from .identifier import Identifier
 
 class ModelPath:
     """Representation of path as a sequence of identifiers.
```

### Comparing `pysros-23.3.2/pysros/model_walker.py` & `pysros-23.3.3/pysros/model_walker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Nokia
+# Copyright 2021-2023 Nokia
 
 import contextlib
 import copy
 import json
 
 from enum import Enum, auto
```

### Comparing `pysros-23.3.2/pysros/pprint.py` & `pysros-23.3.3/pysros/pprint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Nokia
+# Copyright 2021-2023 Nokia
 
 from .wrappers import *
 from .errors import *
 
 __all__ = ("TreePrinter", "printTree", "Column", "Padding", "Table", "KeyValueTable", )
 
 __doc__ = """This module contains functions to assist with stylized
```

### Comparing `pysros-23.3.2/pysros/request_data.py` & `pysros-23.3.3/pysros/request_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Nokia
+# Copyright 2021-2023 Nokia
 
 import copy
 import pprint
 import json
 
 from abc import ABC, abstractmethod
 from collections import OrderedDict
```

### Comparing `pysros-23.3.2/pysros/singleton.py` & `pysros-23.3.3/pysros/singleton.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2021-2023 Nokia
+
 class _Singleton(type):
     _instances = {}
     def __new__(cls, *args, **kwargs):
         res = super(_Singleton, cls).__new__(cls, *args, **kwargs)
         res.__copy__     = lambda self: self
         res.__deepcopy__ = lambda self, memo: self
         res.__reduce__   = lambda self: (self.__class__, ())
```

### Comparing `pysros-23.3.2/pysros/tokenizer.py` & `pysros-23.3.3/pysros/tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Nokia
+# Copyright 2021-2023 Nokia
 
 import collections
 import re
 
 from .errors import *
```

### Comparing `pysros-23.3.2/pysros/wrappers.py` & `pysros-23.3.3/pysros/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Nokia
+# Copyright 2021-2023 Nokia
 
 import operator
 
 from abc import ABC, abstractmethod
 
 from .errors import *
 from .singleton import _Empty
```

### Comparing `pysros-23.3.2/pysros/yang_type.py` & `pysros-23.3.3/pysros/yang_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Nokia
+# Copyright 2021-2023 Nokia
 
 import base64
 
 from abc import ABC, abstractmethod
 from collections import OrderedDict, namedtuple
 from enum import Enum
 from typing import Any, Dict, List, Mapping, Optional, Set, Type, Tuple, Union, NamedTuple, Iterable
```

### Comparing `pysros-23.3.2/pysros.egg-info/PKG-INFO` & `pysros-23.3.3/pysros.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pysros
-Version: 23.3.2
+Version: 23.3.3
 Summary: Python for the Nokia Service Router Operating Systems (pySROS)
 Home-page: https://www.nokia.com
 Author: Nokia
 Author-email: 
-License: Copyright 2021 Nokia.  License available in the LICENSE.md file.
+License: Copyright 2021-2023 Nokia.  License available in the LICENSE.md file.
 Project-URL: Documentation, https://network.developer.nokia.com/static/sr/learn/pysros/latest/
 Project-URL: Source, https://github.com/nokia/pysros
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet
 Classifier: Development Status :: 5 - Production/Stable
@@ -43,15 +43,15 @@
     - With NETCONF enabled and accessible by an authorized user (to execute applications
     remotely)
 - A Python 3 interpreter of version 3.6 or newer when using the pySROS library to
   execute applications remotely
 
 ## License ##
 
-Copyright 2021 Nokia.
+Copyright 2021-2023 Nokia.
 
 The license is located [here](LICENSE.md).
 
 ## Reporting issues ##
 
 Issues, suggestions, and enhancements are welcome.  Please use the Nokia support
 process.  Issues raised in GitHub may be considered for inclusion into the project
```

### Comparing `pysros-23.3.2/setup.py` & `pysros-23.3.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='pysros',
-    version='23.3.2',
+    version='23.3.3',
     packages=['pysros'],
     url='https://www.nokia.com',
-    license='Copyright 2021 Nokia.  License available in the LICENSE.md file.',
+    license='Copyright 2021-2023 Nokia.  License available in the LICENSE.md file.',
     author='Nokia',
     author_email='',
     description='Python for the Nokia Service Router Operating Systems (pySROS)',
     project_urls={
         "Documentation": "https://network.developer.nokia.com/static/sr/learn/pysros/latest/",
         "Source": "https://github.com/nokia/pysros",
     },
```

