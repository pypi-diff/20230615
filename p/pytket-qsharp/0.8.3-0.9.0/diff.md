# Comparing `tmp/pytket-qsharp-0.8.3.tar.gz` & `tmp/pytket-qsharp-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytket-qsharp-0.8.3.tar", last modified: Tue Feb  9 16:58:45 2021, max compression
+gzip compressed data, was "pytket-qsharp-0.9.0.tar", last modified: Tue Mar  2 14:35:23 2021, max compression
```

## Comparing `pytket-qsharp-0.8.3.tar` & `pytket-qsharp-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-09 16:58:45.789248 pytket-qsharp-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-02-09 16:56:45.000000 pytket-qsharp-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3837 2021-02-09 16:58:45.789248 pytket-qsharp-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2354 2021-02-09 16:56:45.000000 pytket-qsharp-0.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-02-09 16:56:45.000000 pytket-qsharp-0.8.3/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-09 16:58:45.785247 pytket-qsharp-0.8.3/pytket/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-09 16:58:45.785247 pytket-qsharp-0.8.3/pytket/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-09 16:58:45.785247 pytket-qsharp-0.8.3/pytket/extensions/backends/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-09 16:58:45.785247 pytket-qsharp-0.8.3/pytket/extensions/backends/qsharp/
--rw-r--r--   0 runner    (1001) docker     (121)      673 2021-02-09 16:56:45.000000 pytket-qsharp-0.8.3/pytket/extensions/backends/qsharp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-02-09 16:58:45.000000 pytket-qsharp-0.8.3/pytket/extensions/backends/qsharp/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     9312 2021-02-09 16:56:45.000000 pytket-qsharp-0.8.3/pytket/extensions/backends/qsharp/azure_quantum.py
--rw-r--r--   0 runner    (1001) docker     (121)     5270 2021-02-09 16:56:45.000000 pytket-qsharp-0.8.3/pytket/extensions/backends/qsharp/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      757 2021-02-09 16:56:45.000000 pytket-qsharp-0.8.3/pytket/extensions/backends/qsharp/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2002 2021-02-09 16:56:45.000000 pytket-qsharp-0.8.3/pytket/extensions/backends/qsharp/estimator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1337 2021-02-09 16:56:45.000000 pytket-qsharp-0.8.3/pytket/extensions/backends/qsharp/simulator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2490 2021-02-09 16:56:45.000000 pytket-qsharp-0.8.3/pytket/extensions/backends/qsharp/toffoli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-09 16:58:45.785247 pytket-qsharp-0.8.3/pytket/extensions/qsharp/
--rw-r--r--   0 runner    (1001) docker     (121)      366 2021-02-09 16:56:45.000000 pytket-qsharp-0.8.3/pytket/extensions/qsharp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4502 2021-02-09 16:56:45.000000 pytket-qsharp-0.8.3/pytket/extensions/qsharp/qsharp_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-09 16:58:45.785247 pytket-qsharp-0.8.3/pytket_qsharp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3837 2021-02-09 16:58:45.000000 pytket-qsharp-0.8.3/pytket_qsharp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      714 2021-02-09 16:58:45.000000 pytket-qsharp-0.8.3/pytket_qsharp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-09 16:58:45.000000 pytket-qsharp-0.8.3/pytket_qsharp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-09 16:58:45.000000 pytket-qsharp-0.8.3/pytket_qsharp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-02-09 16:58:45.000000 pytket-qsharp-0.8.3/pytket_qsharp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-02-09 16:58:45.000000 pytket-qsharp-0.8.3/pytket_qsharp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-02-09 16:58:45.789248 pytket-qsharp-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1819 2021-02-09 16:56:45.000000 pytket-qsharp-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 14:35:23.161313 pytket-qsharp-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2021-03-02 14:31:42.000000 pytket-qsharp-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3501 2021-03-02 14:35:23.161313 pytket-qsharp-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2136 2021-03-02 14:31:42.000000 pytket-qsharp-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-03-02 14:31:42.000000 pytket-qsharp-0.9.0/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 14:35:23.157312 pytket-qsharp-0.9.0/pytket/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 14:35:23.157312 pytket-qsharp-0.9.0/pytket/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 14:35:23.157312 pytket-qsharp-0.9.0/pytket/extensions/qsharp/
+-rw-r--r--   0 runner    (1001) docker     (121)      959 2021-03-02 14:31:42.000000 pytket-qsharp-0.9.0/pytket/extensions/qsharp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-03-02 14:35:23.000000 pytket-qsharp-0.9.0/pytket/extensions/qsharp/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 14:35:23.157312 pytket-qsharp-0.9.0/pytket/extensions/qsharp/backends/
+-rw-r--r--   0 runner    (1001) docker     (121)      851 2021-03-02 14:31:42.000000 pytket-qsharp-0.9.0/pytket/extensions/qsharp/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9944 2021-03-02 14:31:42.000000 pytket-qsharp-0.9.0/pytket/extensions/qsharp/backends/azure_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5601 2021-03-02 14:31:42.000000 pytket-qsharp-0.9.0/pytket/extensions/qsharp/backends/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1349 2021-03-02 14:31:42.000000 pytket-qsharp-0.9.0/pytket/extensions/qsharp/backends/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2339 2021-03-02 14:31:42.000000 pytket-qsharp-0.9.0/pytket/extensions/qsharp/backends/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1654 2021-03-02 14:31:42.000000 pytket-qsharp-0.9.0/pytket/extensions/qsharp/backends/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2804 2021-03-02 14:31:42.000000 pytket-qsharp-0.9.0/pytket/extensions/qsharp/backends/toffoli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4820 2021-03-02 14:31:42.000000 pytket-qsharp-0.9.0/pytket/extensions/qsharp/qsharp_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 14:35:23.161313 pytket-qsharp-0.9.0/pytket_qsharp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3501 2021-03-02 14:35:23.000000 pytket-qsharp-0.9.0/pytket_qsharp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2021-03-02 14:35:23.000000 pytket-qsharp-0.9.0/pytket_qsharp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-02 14:35:23.000000 pytket-qsharp-0.9.0/pytket_qsharp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-02 14:35:23.000000 pytket-qsharp-0.9.0/pytket_qsharp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2021-03-02 14:35:23.000000 pytket-qsharp-0.9.0/pytket_qsharp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-03-02 14:35:23.000000 pytket-qsharp-0.9.0/pytket_qsharp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-02 14:35:23.161313 pytket-qsharp-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2046 2021-03-02 14:31:42.000000 pytket-qsharp-0.9.0/setup.py
```

### Comparing `pytket-qsharp-0.8.3/PKG-INFO` & `pytket-qsharp-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pytket-qsharp
-Version: 0.8.3
+Version: 0.9.0
 Summary: Extension for pytket, providing simulators from Microsoft QDK
 Home-page: https://github.com/CQCL/pytket
 Author: Alec Edgington
 Author-email: alec.edgington@cambridgequantum.com
-License: CQC Software Licence
+License: Apache 2
 Description: # pytket-qsharp
         
         [Pytket](https://cqcl.github.io/pytket) is a Python module for interfacing
         with CQC tket, a set of quantum programming tools.
         
         [Azure Quantum](https://azure.microsoft.com/en-gb/services/quantum/) is a portal for accessing
         quantum computers via Microsoft Azure.
@@ -19,15 +19,15 @@
         
         `pytket-qsharp` is an extension to `pytket` that allows `pytket` circuits to be
         executed on remote devices and simulators via Azure Quantum,
         as well as local simulators and resource estimators from the Microsoft QDK.
         
         ## Getting started
         
-        `pytket-qsharp` is available for Python 3.6, 3.7 and 3.8, on Linux, MacOS and Windows. To
+        `pytket-qsharp` is available for Python 3.7, 3.8 and 3.9, on Linux, MacOS and Windows. To
         install, run:
         
         ```pip install pytket-qsharp```
         
         In order to use `pytket-qsharp` you will first need to install the `dotnet` SDK
         (3.1) and the `iqsharp` tool. On some Linux systems it is also necessary to
         modify your `PATH`:
@@ -64,29 +64,21 @@
         * `QsharpToffoliSimulatorBackend`, for simulating a Toffoli circuit using the
         QDK;
         
         * `QsharpEstimatorBackend`, for estimating various quantum resources of a
         circuit using the QDK. This provides a `get_resources` method, which returns a
         dictionary.
         
-        ## LICENCE
-        
-        Copyright 2020-2021 Cambridge Quantum Computing
-        
-        You may not use this product except in compliance with the Licence. You may view
-        the License [here](https://cqcl.github.io/pytket/build/html/licence.html).
-        
 Platform: UNKNOWN
 Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pytket-qsharp-0.8.3/README.md` & `pytket-qsharp-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 `pytket-qsharp` is an extension to `pytket` that allows `pytket` circuits to be
 executed on remote devices and simulators via Azure Quantum,
 as well as local simulators and resource estimators from the Microsoft QDK.
 
 ## Getting started
 
-`pytket-qsharp` is available for Python 3.6, 3.7 and 3.8, on Linux, MacOS and Windows. To
+`pytket-qsharp` is available for Python 3.7, 3.8 and 3.9, on Linux, MacOS and Windows. To
 install, run:
 
 ```pip install pytket-qsharp```
 
 In order to use `pytket-qsharp` you will first need to install the `dotnet` SDK
 (3.1) and the `iqsharp` tool. On some Linux systems it is also necessary to
 modify your `PATH`:
@@ -55,14 +55,7 @@
 
 * `QsharpToffoliSimulatorBackend`, for simulating a Toffoli circuit using the
 QDK;
 
 * `QsharpEstimatorBackend`, for estimating various quantum resources of a
 circuit using the QDK. This provides a `get_resources` method, which returns a
 dictionary.
-
-## LICENCE
-
-Copyright 2020-2021 Cambridge Quantum Computing
-
-You may not use this product except in compliance with the Licence. You may view
-the License [here](https://cqcl.github.io/pytket/build/html/licence.html).
```

### Comparing `pytket-qsharp-0.8.3/pytket/extensions/backends/qsharp/azure_quantum.py` & `pytket-qsharp-0.9.0/pytket/extensions/qsharp/backends/azure_quantum.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2021 Cambridge Quantum Computing
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import json
 import time
 from ast import literal_eval
 from collections import Counter
 from typing import TYPE_CHECKING, Dict, Iterable, List, Optional, cast
 
 import qsharp  # type: ignore
@@ -12,17 +26,17 @@
 from pytket.backends.backend import Backend, BackendResult, CircuitStatus, KwargTypes
 from pytket.backends.backend_exceptions import CircuitNotRunError
 from pytket.backends.resulthandle import ResultHandle, _ResultIdTuple
 from pytket.backends.status import StatusEnum
 from pytket.circuit import Circuit  # type: ignore
 from pytket.utils.outcomearray import OutcomeArray
 
-from pytket.extensions.backends.qsharp.config import QSharpConfig
-from pytket.extensions.backends.qsharp.common import _QsharpBaseBackend
-from pytket.extensions.qsharp import tk_to_qsharp
+from pytket.extensions.qsharp.backends.config import QSharpConfig
+from pytket.extensions.qsharp.backends.common import _QsharpBaseBackend
+from pytket.extensions.qsharp.qsharp_convert import tk_to_qsharp
 
 
 if TYPE_CHECKING:
     from qsharp.loader import QSharpCallable  # type: ignore
 
 _DEBUG_HANDLE_PREFIX = "_MACHINE_DEBUG_"
 
@@ -102,15 +116,16 @@
                 config.storage = storage
             print(config.__dict__)
             # check required parameters
             if any(val is None for val in (config.resourceId, config.location)):
                 raise ValueError(
                     "Azure Quantum resourceId and location must be provided as"
                     f" parameter or stored in the config file {get_config_file_path()}"
-                    r"as:{'extensions':{'qsharp':{'resourceId':<val>,'location':<val>}}}"
+                    r" as:{'extensions':{'qsharp':"
+                    r"{'resourceId':<val>,'location':<val>}}}"
                 )
 
             try:
                 target_list = qsharp.azure.connect(**config.__dict__)
             except qsharp.azure.AzureError as e:
                 if e.error_name == "AuthenticationFailed":
                     raise RuntimeError(
```

### Comparing `pytket-qsharp-0.8.3/pytket/extensions/backends/qsharp/common.py` & `pytket-qsharp-0.9.0/pytket/extensions/qsharp/backends/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Copyright 2020-2021 Cambridge Quantum Computing
 #
-# You may not use this file except in compliance with the Licence.
-# You may obtain a copy of the Licence in the LICENCE file accompanying
-# these documents or at:
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-#     https://cqcl.github.io/pytket/build/html/licence.html
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 from typing import (
     TYPE_CHECKING,
     Iterable,
     List,
     MutableMapping,
     Optional,
@@ -41,15 +47,15 @@
     GateSetPredicate,
     NoClassicalControlPredicate,
     NoFastFeedforwardPredicate,
     Predicate,
     NoMidMeasurePredicate,
     NoSymbolsPredicate,
 )
-from pytket.extensions.qsharp import tk_to_qsharp
+from pytket.extensions.qsharp.qsharp_convert import tk_to_qsharp
 
 if TYPE_CHECKING:
     from qsharp.loader import QSharpCallable  # type: ignore
     from pytket.device import Device  # type: ignore
 
 
 def _from_tk1(a: float, b: float, c: float) -> Circuit:
@@ -154,15 +160,15 @@
     def circuit_status(self, handle: ResultHandle) -> CircuitStatus:
         if handle in self._cache:
             return CircuitStatus(StatusEnum.COMPLETED)
         raise CircuitNotRunError(handle)
 
     def _calculate_results(
         self, qscall: "QSharpCallable", n_shots: Optional[int] = None
-    ) -> Union[BackendResult, "MutableMapping"]:
+    ) -> Union[BackendResult, MutableMapping]:
         raise NotImplementedError()
 
     def process_circuits(
         self,
         circuits: Iterable[Circuit],
         n_shots: Optional[int] = None,
         valid_check: bool = True,
```

### Comparing `pytket-qsharp-0.8.3/pytket/extensions/backends/qsharp/estimator.py` & `pytket-qsharp-0.9.0/pytket/extensions/qsharp/backends/estimator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Copyright 2020-2021 Cambridge Quantum Computing
 #
-# You may not use this file except in compliance with the Licence.
-# You may obtain a copy of the Licence in the LICENCE file accompanying
-# these documents or at:
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-#     https://cqcl.github.io/pytket/build/html/licence.html
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 from typing import TYPE_CHECKING, Optional, Union, Dict
 
 from pytket.backends import ResultHandle, StatusEnum
 from pytket.circuit import Circuit  # type: ignore
 
 from .common import _QsharpBaseBackend, BackendResult
@@ -43,10 +49,11 @@
         elif isinstance(circuit, ResultHandle):
             handle = circuit
             circ_status = self.circuit_status(handle)
             if circ_status.status is not StatusEnum.COMPLETED:
                 raise ValueError(f"Handle is '{circ_status}'")
         else:
             raise TypeError(
-                "Provide either a Circuit to run or a ResultHandle to a previously submitted circuit."
+                "Provide either a Circuit to run or a ResultHandle to a previously "
+                "submitted circuit."
             )
         return self._cache[handle]["resource"]  # type: ignore
```

### Comparing `pytket-qsharp-0.8.3/pytket/extensions/backends/qsharp/simulator.py` & `pytket-qsharp-0.9.0/pytket/extensions/qsharp/backends/simulator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # Copyright 2020-2021 Cambridge Quantum Computing
 #
-# You may not use this file except in compliance with the Licence.
-# You may obtain a copy of the Licence in the LICENCE file accompanying
-# these documents or at:
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-#     https://cqcl.github.io/pytket/build/html/licence.html
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 from typing import TYPE_CHECKING, Optional
-
 import numpy as np
-from .common import _QsharpSimBaseBackend, BackendResult
 from pytket.utils.outcomearray import OutcomeArray
+from .common import _QsharpSimBaseBackend, BackendResult
 
 if TYPE_CHECKING:
     from qsharp.loader import QSharpCallable  # type: ignore
 
 
 class QsharpSimulatorBackend(_QsharpSimBaseBackend):
     """Backend for simulating a circuit using the QDK."""
```

### Comparing `pytket-qsharp-0.8.3/pytket/extensions/backends/qsharp/toffoli.py` & `pytket-qsharp-0.9.0/pytket/extensions/qsharp/backends/toffoli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # Copyright 2020-2021 Cambridge Quantum Computing
 #
-# You may not use this file except in compliance with the Licence.
-# You may obtain a copy of the Licence in the LICENCE file accompanying
-# these documents or at:
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-#     https://cqcl.github.io/pytket/build/html/licence.html
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 from typing import TYPE_CHECKING, MutableMapping, Optional, Union
 import numpy as np
-
 from pytket.circuit import Circuit, OpType  # type: ignore
 from pytket.passes import BasePass, RebaseCustom  # type: ignore
-
-from .common import _QsharpSimBaseBackend, BackendResult
 from pytket.utils.outcomearray import OutcomeArray
+from .common import _QsharpSimBaseBackend, BackendResult
 
 if TYPE_CHECKING:
     from qsharp.loader import QSharpCallable  # type: ignore
 
 
 def is_approx_0_mod_2(x: float, tol: float = 1e-10) -> bool:
     x %= 2  # --> [0,2)
@@ -52,15 +56,15 @@
             Circuit(),  # cx_replacement (irrelevant)
             {OpType.X},  # singleqs
             toffoli_from_tk1,
         )  # tk1_replacement
 
     def _calculate_results(
         self, qscall: "QSharpCallable", n_shots: Optional[int] = None
-    ) -> Union[BackendResult, "MutableMapping"]:
+    ) -> Union[BackendResult, MutableMapping]:
         if n_shots:
             shots_ar = np.array(
                 [qscall.toffoli_simulate() for _ in range(n_shots)], dtype=np.uint8
             )
             shots = OutcomeArray.from_readouts(shots_ar)  # type: ignore
             # ^ type ignore as array is ok for Sequence[Sequence[int]]
             # outputs should correspond to default register,
```

### Comparing `pytket-qsharp-0.8.3/pytket/extensions/qsharp/qsharp_convert.py` & `pytket-qsharp-0.9.0/pytket/extensions/qsharp/qsharp_convert.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 # Copyright 2020-2021 Cambridge Quantum Computing
 #
-# You may not use this file except in compliance with the Licence.
-# You may obtain a copy of the Licence in the LICENCE file accompanying
-# these documents or at:
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-#     https://cqcl.github.io/pytket/build/html/licence.html
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 """Methods to allow conversion from tket to Q#
 """
 
-from pytket.circuit import Circuit, OpType, Op  # type: ignore
-from pytket.pauli import Pauli  # type: ignore
 from typing import List, Tuple
 from math import pi
+from pytket.circuit import Circuit, OpType, Op  # type: ignore
+from pytket.pauli import Pauli  # type: ignore
 
 qs_pauli = {Pauli.I: "PauliI", Pauli.X: "PauliX", Pauli.Y: "PauliY", Pauli.Z: "PauliZ"}
 
 
 def cmd_body(op: Op, qbs: List[int]) -> str:
     optype = op.type
```

### Comparing `pytket-qsharp-0.8.3/pytket_qsharp.egg-info/PKG-INFO` & `pytket-qsharp-0.9.0/pytket_qsharp.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pytket-qsharp
-Version: 0.8.3
+Version: 0.9.0
 Summary: Extension for pytket, providing simulators from Microsoft QDK
 Home-page: https://github.com/CQCL/pytket
 Author: Alec Edgington
 Author-email: alec.edgington@cambridgequantum.com
-License: CQC Software Licence
+License: Apache 2
 Description: # pytket-qsharp
         
         [Pytket](https://cqcl.github.io/pytket) is a Python module for interfacing
         with CQC tket, a set of quantum programming tools.
         
         [Azure Quantum](https://azure.microsoft.com/en-gb/services/quantum/) is a portal for accessing
         quantum computers via Microsoft Azure.
@@ -19,15 +19,15 @@
         
         `pytket-qsharp` is an extension to `pytket` that allows `pytket` circuits to be
         executed on remote devices and simulators via Azure Quantum,
         as well as local simulators and resource estimators from the Microsoft QDK.
         
         ## Getting started
         
-        `pytket-qsharp` is available for Python 3.6, 3.7 and 3.8, on Linux, MacOS and Windows. To
+        `pytket-qsharp` is available for Python 3.7, 3.8 and 3.9, on Linux, MacOS and Windows. To
         install, run:
         
         ```pip install pytket-qsharp```
         
         In order to use `pytket-qsharp` you will first need to install the `dotnet` SDK
         (3.1) and the `iqsharp` tool. On some Linux systems it is also necessary to
         modify your `PATH`:
@@ -64,29 +64,21 @@
         * `QsharpToffoliSimulatorBackend`, for simulating a Toffoli circuit using the
         QDK;
         
         * `QsharpEstimatorBackend`, for estimating various quantum resources of a
         circuit using the QDK. This provides a `get_resources` method, which returns a
         dictionary.
         
-        ## LICENCE
-        
-        Copyright 2020-2021 Cambridge Quantum Computing
-        
-        You may not use this product except in compliance with the Licence. You may view
-        the License [here](https://cqcl.github.io/pytket/build/html/licence.html).
-        
 Platform: UNKNOWN
 Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pytket-qsharp-0.8.3/pytket_qsharp.egg-info/SOURCES.txt` & `pytket-qsharp-0.9.0/pytket_qsharp.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 MANIFEST.in
 README.md
 _metadata.py
 setup.py
-pytket/extensions/backends/qsharp/__init__.py
-pytket/extensions/backends/qsharp/_metadata.py
-pytket/extensions/backends/qsharp/azure_quantum.py
-pytket/extensions/backends/qsharp/common.py
-pytket/extensions/backends/qsharp/config.py
-pytket/extensions/backends/qsharp/estimator.py
-pytket/extensions/backends/qsharp/simulator.py
-pytket/extensions/backends/qsharp/toffoli.py
 pytket/extensions/qsharp/__init__.py
+pytket/extensions/qsharp/_metadata.py
 pytket/extensions/qsharp/qsharp_convert.py
+pytket/extensions/qsharp/backends/__init__.py
+pytket/extensions/qsharp/backends/azure_quantum.py
+pytket/extensions/qsharp/backends/common.py
+pytket/extensions/qsharp/backends/config.py
+pytket/extensions/qsharp/backends/estimator.py
+pytket/extensions/qsharp/backends/simulator.py
+pytket/extensions/qsharp/backends/toffoli.py
 pytket_qsharp.egg-info/PKG-INFO
 pytket_qsharp.egg-info/SOURCES.txt
 pytket_qsharp.egg-info/dependency_links.txt
 pytket_qsharp.egg-info/not-zip-safe
 pytket_qsharp.egg-info/requires.txt
 pytket_qsharp.egg-info/top_level.txt
```

### Comparing `pytket-qsharp-0.8.3/setup.py` & `pytket-qsharp-0.9.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 # Copyright 2020-2021 Cambridge Quantum Computing
 #
-# You may not use this file except in compliance with the Licence.
-# You may obtain a copy of the Licence in the LICENCE file accompanying
-# these documents or at:
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-#     https://cqcl.github.io/pytket/build/html/licence.html
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-import setuptools  # type: ignore
-from setuptools import setup, find_namespace_packages
 import shutil
 import os
+from setuptools import setup, find_namespace_packages  # type: ignore
 
 metadata: dict = {}
 with open("_metadata.py") as fp:
     exec(fp.read(), metadata)
 shutil.copy(
     "_metadata.py",
-    os.path.join("pytket", "extensions", "backends", "qsharp", "_metadata.py"),
+    os.path.join("pytket", "extensions", "qsharp", "_metadata.py"),
 )
 
 setup(
     name=metadata["__extension_name__"],
     version=metadata["__extension_version__"],
     author="Alec Edgington",
     author_email="alec.edgington@cambridgequantum.com",
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     url="https://github.com/CQCL/pytket",
     description="Extension for pytket, providing simulators from Microsoft QDK",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    license="CQC Software Licence",
+    license="Apache 2",
     packages=find_namespace_packages(include=["pytket.*"]),
     include_package_data=True,
-    install_requires=["pytket ~= 0.7.1", "qsharp ~= 0.14.2011"],
+    install_requires=["pytket ~= 0.8.0", "qsharp ~= 0.14.2011"],
     classifiers=[
         "Environment :: Console",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "License :: Other/Proprietary License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
         "Operating System :: Microsoft :: Windows",
```

