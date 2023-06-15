# Comparing `tmp/qctrl-commons-8.1.0.tar.gz` & `tmp/qctrl-commons-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl-commons-8.1.0.tar", last modified: Thu Apr 29 03:21:38 2021, max compression
+gzip compressed data, was "qctrl-commons-9.0.0.tar", last modified: Wed May  5 02:15:28 2021, max compression
```

## Comparing `qctrl-commons-8.1.0.tar` & `qctrl-commons-9.0.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0      108 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/DESCRIPTION.md
--rw-r--r--   0        0        0    34692 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/LICENSE
--rw-r--r--   0        0        0     2654 2021-04-29 03:21:00.322003 qctrl-commons-8.1.0/pyproject.toml
--rw-r--r--   0        0        0      717 2021-04-29 03:21:00.334003 qctrl-commons-8.1.0/qctrlcommons/__init__.py
--rw-r--r--   0        0        0     6009 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/qctrlcommons/auth.py
--rw-r--r--   0        0        0     1897 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/qctrlcommons/constants.py
--rw-r--r--   0        0        0    11920 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/qctrlcommons/data_types.py
--rw-r--r--   0        0        0     4384 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/qctrlcommons/exceptions.py
--rw-r--r--   0        0        0      914 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/qctrlcommons/graph.py
--rw-r--r--   0        0        0        0 2021-04-29 03:21:00.334003 qctrl-commons-8.1.0/qctrlcommons/node/__init__.py
--rw-r--r--   0        0        0     3164 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/qctrlcommons/node/attribute.py
--rw-r--r--   0        0        0     4400 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/qctrlcommons/node/base.py
--rw-r--r--   0        0        0    25783 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/qctrlcommons/node/binary.py
--rw-r--r--   0        0        0    12256 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/qctrlcommons/node/core.py
--rw-r--r--   0        0        0    10286 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/qctrlcommons/node/infidelity.py
--rw-r--r--   0        0        0    26937 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/qctrlcommons/node/ms.py
--rw-r--r--   0        0        0     4828 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/qctrlcommons/node/node_data.py
--rw-r--r--   0        0        0     9171 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/qctrlcommons/node/optimization_variable.py
--rw-r--r--   0        0        0    11048 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/qctrlcommons/node/oqs.py
--rw-r--r--   0        0        0    30947 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/qctrlcommons/node/pwc.py
--rw-r--r--   0        0        0     3713 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/qctrlcommons/node/registry.py
--rw-r--r--   0        0        0    21031 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/qctrlcommons/node/sparse.py
--rw-r--r--   0        0        0    22068 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/qctrlcommons/node/stf.py
--rw-r--r--   0        0        0     9108 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/qctrlcommons/node/tensorflow.py
--rw-r--r--   0        0        0     3161 2021-04-29 03:20:44.381858 qctrl-commons-8.1.0/qctrlcommons/node/types.py
--rw-r--r--   0        0        0    32661 2021-04-29 03:20:44.385858 qctrl-commons-8.1.0/qctrlcommons/node/unary.py
--rw-r--r--   0        0        0    13990 2021-04-29 03:20:44.385858 qctrl-commons-8.1.0/qctrlcommons/node/utils.py
--rw-r--r--   0        0        0     3206 2021-04-29 03:20:44.385858 qctrl-commons-8.1.0/qctrlcommons/node/wrapper.py
--rw-r--r--   0        0        0    11296 2021-04-29 03:20:44.385858 qctrl-commons-8.1.0/qctrlcommons/preconditions.py
--rw-r--r--   0        0        0    11168 2021-04-29 03:20:44.385858 qctrl-commons-8.1.0/qctrlcommons/serializers.py
--rw-r--r--   0        0        0     3560 2021-04-29 03:20:44.385858 qctrl-commons-8.1.0/qctrlcommons/utils.py
--rw-r--r--   0        0        0      978 2021-04-29 03:21:38.513995 qctrl-commons-8.1.0/setup.py
--rw-r--r--   0        0        0     1931 2021-04-29 03:21:38.514451 qctrl-commons-8.1.0/PKG-INFO
+-rw-r--r--   0        0        0      108 2021-05-05 02:14:33.506873 qctrl-commons-9.0.0/DESCRIPTION.md
+-rw-r--r--   0        0        0    34692 2021-05-05 02:14:33.506873 qctrl-commons-9.0.0/LICENSE
+-rw-r--r--   0        0        0     2654 2021-05-05 02:14:49.059083 qctrl-commons-9.0.0/pyproject.toml
+-rw-r--r--   0        0        0      717 2021-05-05 02:14:49.071083 qctrl-commons-9.0.0/qctrlcommons/__init__.py
+-rw-r--r--   0        0        0     6009 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/auth.py
+-rw-r--r--   0        0        0     1897 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/constants.py
+-rw-r--r--   0        0        0    12687 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/data_types.py
+-rw-r--r--   0        0        0     4384 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/exceptions.py
+-rw-r--r--   0        0        0      914 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/graph.py
+-rw-r--r--   0        0        0        0 2021-05-05 02:14:49.067083 qctrl-commons-9.0.0/qctrlcommons/node/__init__.py
+-rw-r--r--   0        0        0     3164 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/node/attribute.py
+-rw-r--r--   0        0        0     2798 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/node/base.py
+-rw-r--r--   0        0        0    25133 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/node/binary.py
+-rw-r--r--   0        0        0    12273 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/node/core.py
+-rw-r--r--   0        0        0     6196 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/node/deprecation.py
+-rw-r--r--   0        0        0    10287 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/node/infidelity.py
+-rw-r--r--   0        0        0    26937 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/node/ms.py
+-rw-r--r--   0        0        0     5838 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/node/node_data.py
+-rw-r--r--   0        0        0     6097 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/node/optimization_variable.py
+-rw-r--r--   0        0        0    11048 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/node/oqs.py
+-rw-r--r--   0        0        0    31283 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/node/pwc.py
+-rw-r--r--   0        0        0     3713 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/node/registry.py
+-rw-r--r--   0        0        0    19498 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/node/sparse.py
+-rw-r--r--   0        0        0    22351 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/node/stf.py
+-rw-r--r--   0        0        0     9108 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/node/tensorflow.py
+-rw-r--r--   0        0        0     3161 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/node/types.py
+-rw-r--r--   0        0        0    32358 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/node/unary.py
+-rw-r--r--   0        0        0    13990 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/node/utils.py
+-rw-r--r--   0        0        0     3206 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/node/wrapper.py
+-rw-r--r--   0        0        0    11296 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/preconditions.py
+-rw-r--r--   0        0        0    11212 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/serializers.py
+-rw-r--r--   0        0        0     3560 2021-05-05 02:14:33.510873 qctrl-commons-9.0.0/qctrlcommons/utils.py
+-rw-r--r--   0        0        0      978 2021-05-05 02:15:28.600904 qctrl-commons-9.0.0/setup.py
+-rw-r--r--   0        0        0     1931 2021-05-05 02:15:28.601295 qctrl-commons-9.0.0/PKG-INFO
```

### Comparing `qctrl-commons-8.1.0/LICENSE` & `qctrl-commons-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl-commons-8.1.0/pyproject.toml` & `qctrl-commons-9.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-commons"
-version = "8.1.0"
+version = "9.0.0"
 description = "Q-CTRL Python Commons"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "DESCRIPTION.md"
 homepage = "https://q-ctrl.com"
 repository = ""
```

### Comparing `qctrl-commons-8.1.0/qctrlcommons/__init__.py` & `qctrl-commons-9.0.0/qctrlcommons/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
 """qctrlcommons - a collection of common libraries for the Python language"""
 
-__version__ = "8.1.0"
+__version__ = "9.0.0"
 __author__ = "Q-CTRL <support@q-ctrl.com>"
```

### Comparing `qctrl-commons-8.1.0/qctrlcommons/auth.py` & `qctrl-commons-9.0.0/qctrlcommons/auth.py`

 * *Files identical despite different names*

### Comparing `qctrl-commons-8.1.0/qctrlcommons/constants.py` & `qctrl-commons-9.0.0/qctrlcommons/constants.py`

 * *Files identical despite different names*

### Comparing `qctrl-commons-8.1.0/qctrlcommons/data_types.py` & `qctrl-commons-9.0.0/qctrlcommons/data_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -175,14 +175,49 @@
 
     def decode(self, obj):
         return np.frombuffer(
             base64.b64decode(obj[self.object_key]), dtype=obj["dtype"]
         ).reshape(obj["shape"])
 
 
+class QuantumObject(DataType):
+    """Represent QuTiP QuantumObject Model."""
+
+    def can_encode(self, obj: Any) -> bool:
+        """Checks that the object can be encoded with this class.
+        If it has attribute ``full`` it can be encoded.
+
+        Parameters
+        ----------
+        obj : Any
+            object to be examined.
+
+        Returns
+        -------
+        bool
+            True if the object can be encoded, False otherwise.
+
+        Raises
+        ------
+        RuntimeError
+            if the data type is `None`.
+        """
+
+        return hasattr(obj, "full")
+
+    def encode(self, obj):
+        return obj.full()
+
+    def can_decode(self, obj) -> bool:
+        return False
+
+    def decode(self, obj):
+        raise NotImplementedError
+
+
 class NumpyComplexNumber(DataType):
     """Represent NumpyComplexNumber Model."""
 
     _type = np.complexfloating
     object_key = "base64_encoded_data"
 
     def encode(self, obj) -> dict:
```

### Comparing `qctrl-commons-8.1.0/qctrlcommons/exceptions.py` & `qctrl-commons-9.0.0/qctrlcommons/exceptions.py`

 * *Files identical despite different names*

### Comparing `qctrl-commons-8.1.0/qctrlcommons/graph.py` & `qctrl-commons-9.0.0/qctrlcommons/graph.py`

 * *Files identical despite different names*

### Comparing `qctrl-commons-8.1.0/qctrlcommons/node/attribute.py` & `qctrl-commons-9.0.0/qctrlcommons/node/attribute.py`

 * *Files identical despite different names*

### Comparing `qctrl-commons-8.1.0/qctrlcommons/node/binary.py` & `qctrl-commons-9.0.0/qctrlcommons/node/binary.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
 # pylint: disable=too-many-lines
 """Module for binary operation nodes."""
 
-import warnings
 from typing import Union
 
 import forge
 import numpy as np
 
 from qctrlcommons.exceptions import QctrlException
 from qctrlcommons.node import (
     node_data,
     types,
 )
 from qctrlcommons.node.base import Node
+from qctrlcommons.node.deprecation import deprecated_node
 from qctrlcommons.node.utils import (
     NumericOrFunction,
     is_broadcastable,
     validate_batch_and_values_shapes,
     validate_broadcasted_shape,
     validate_function_output_shapes,
     validate_shape,
@@ -310,30 +310,20 @@
     rtype = Union[types.Tensor, types.TensorPwc, types.Stf]
 
     @classmethod
     def create_node_data(cls, _operation, **kwargs):
         return _create_flexible_binary_node_data(_operation, "subtract", **kwargs)
 
 
+@deprecated_node("subtract")
 class SubtractionDeprecated(Subtraction):
-    r"""
-    This node has been deprecated and will be removed in the future.
-    Please use :py:func:`subtract` instead.
-    """
+    """Deprecated node."""
 
     name = "sub"
 
-    @classmethod
-    def create_node_data(cls, _operation, **kwargs):
-        warnings.warn(
-            "The 'sub' node will be removed in the future. "
-            "Please use 'subtract' instead."
-        )
-        return super().create_node_data(_operation, **kwargs)
-
 
 class Multiplication(Node):
     r"""
     Calculates the element-wise product between numbers, np.ndarrays, Tensors,
     TensorPwcs, or Stfs. You can also use the arithmetic operator ``*`` to calculate their product.
 
     Considering numbers and np.ndarrays as Tensors, if the two objects are of the same type,
@@ -366,30 +356,20 @@
     rtype = Union[types.Tensor, types.TensorPwc, types.Stf]
 
     @classmethod
     def create_node_data(cls, _operation, **kwargs):
         return _create_flexible_binary_node_data(_operation, "multiply", **kwargs)
 
 
+@deprecated_node("multiply")
 class MultiplicationDeprecated(Multiplication):
-    r"""
-    This node has been deprecated and will be removed in the future.
-    Please use :py:func:`multiply` instead.
-    """
+    """Deprecated node."""
 
     name = "mul"
 
-    @classmethod
-    def create_node_data(cls, _operation, **kwargs):
-        warnings.warn(
-            "The 'mul' node will be removed in the future. "
-            "Please use 'multiply' instead."
-        )
-        return super().create_node_data(_operation, **kwargs)
-
 
 class TrueDivision(Node):
     """
     Calculates the element-wise division between numbers, np.ndarrays, Tensors, TensorPwcs,
     or Stfs. You can also use the arithmetic operator ``/`` to calculate their division.
 
     Considering numbers and np.ndarrays as Tensors, if the two objects are of the same type,
```

### Comparing `qctrl-commons-8.1.0/qctrlcommons/node/core.py` & `qctrl-commons-9.0.0/qctrlcommons/node/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,14 @@
     operator : np.ndarray or Tensor
          The target gate :math:`U_\mathrm{target}`. Must be a non-zero partial
          isometry.
     filter_function_projector : np.ndarray, optional
         The orthogonal projection matrix :math:`P` onto the subspace used for
         filter function calculations. If you provide a value then it must be
         Hermitian and idempotent. Defaults to the identity matrix.
-    name : str, optional
-        The name of the node.
 
     Returns
     -------
     Target
         The node containing the specified target information.
 
     See Also
@@ -89,14 +87,15 @@
     """
 
     name = "target"
     args = [
         forge.arg("operator", type=Union[np.ndarray, types.Tensor]),
         forge.arg("filter_function_projector", type=Optional[np.ndarray], default=None),
     ]
+    kwargs = {}  # TargetOperator should not accept `name` as parameter
     rtype = types.Target
 
     @classmethod
     def create_node_data(cls, _operation, **kwargs):
         operator = kwargs.get("operator")
         values_shape = validate_shape(operator, "operator")
```

### Comparing `qctrl-commons-8.1.0/qctrlcommons/node/infidelity.py` & `qctrl-commons-9.0.0/qctrlcommons/node/infidelity.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 
     Returns
     -------
     Tensor
         The infidelity of the given system with respect to the given target at the last time in
         `sample_times`.
         If you provide a batch of Hamiltonians, the function returns a batch of infidelities
-        contaning one infidelity for each Hamiltonian of the input batch.
+        containing one infidelity for each Hamiltonian of the input batch.
 
     See Also
     --------
     infidelity_pwc : Corresponding operation for `TensorPwc` Hamiltonians.
     target : Define the target operation of the time evolution.
     time_evolution_operators_stf : Unitary time evolution operators for quantum systems with
         `Stf` Hamiltonians.
```

### Comparing `qctrl-commons-8.1.0/qctrlcommons/node/ms.py` & `qctrl-commons-9.0.0/qctrlcommons/node/ms.py`

 * *Files identical despite different names*

### Comparing `qctrl-commons-8.1.0/qctrlcommons/node/node_data.py` & `qctrl-commons-9.0.0/qctrlcommons/node/node_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -107,14 +107,21 @@
         # future if we're more strict about client-side validation of iterable inputs, or if we
         # update the backend to be able to iterate over tensors.
         raise TypeError(
             "You cannot iterate over Tensors directly. Instead you can iterate over the indices "
             "and extract elements of the tensor using `tensor[index]`."
         )
 
+    def __repr__(self):
+        return (
+            f'<TensorNode: name="{self.name}", '
+            f'operation_name="{self.operation.operation_name}", '
+            f"shape={self.shape}>"
+        )
+
 
 @dataclass
 class TensorPwcNodeData(NamedNodeData, ArithmeticMixin):
     """
     Wrapper class for TensorPwc type Node.
     """
 
@@ -129,34 +136,59 @@
         """
         node_data = attribute_ops.GetAttributeNode.create_pf()(self, "values")
         shape = (
             tuple(self.batch_shape) + (len(self.durations),) + tuple(self.values_shape)
         )
         return TensorNodeData(node_data.operation, shape=shape)
 
+    def __repr__(self):
+        return (
+            f'<PwcNode: name="{self.name}", '
+            f'operation_name="{self.operation.operation_name}", '
+            f"value_shape={self.values_shape}, batch_shape={self.batch_shape}>"
+        )
+
 
 @dataclass
 class StfNodeData(NodeData, ArithmeticMixin):
     """
     Wrapper class for Stf type Node.
     """
 
     values_shape: Tuple[int]
     batch_shape: Tuple[int]
 
+    def __repr__(self):
+        return (
+            f'<StfNode: operation_name="{self.operation.operation_name}", '
+            f"value_shape={self.values_shape}, batch_shape={self.batch_shape}>"
+        )
+
 
 @dataclass
 class SparsePwcNodeData(NodeData):
     """
     Wrapper class for SparsePwc type Node.
     """
 
     values_shape: Tuple[int]
 
+    def __repr__(self):
+        return (
+            f'<SparsePwcNode: operation_name="{self.operation.operation_name}", '
+            f"value_shape={self.values_shape}>"
+        )
+
 
 @dataclass
-class TargetNodeData(NamedNodeData):
+class TargetNodeData(NodeData):
     """
     Wrapper class for Target type node
     """
 
     values_shape: Tuple[int]
+
+    def __repr__(self):
+        return (
+            f'<TargetNode: operation_name="{self.operation.operation_name}", '
+            f"value_shape={self.values_shape}>"
+        )
```

### Comparing `qctrl-commons-8.1.0/qctrlcommons/node/oqs.py` & `qctrl-commons-9.0.0/qctrlcommons/node/oqs.py`

 * *Files identical despite different names*

### Comparing `qctrl-commons-8.1.0/qctrlcommons/node/pwc.py` & `qctrl-commons-9.0.0/qctrlcommons/node/pwc.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 )
 
 import forge
 import numpy as np
 
 from qctrlcommons.node import types
 from qctrlcommons.node.base import Node
+from qctrlcommons.node.deprecation import deprecated_parameter
 from qctrlcommons.node.node_data import (
     TensorNodeData,
     TensorPwcNodeData,
 )
 from qctrlcommons.node.utils import (
     validate_batch_and_values_shapes,
     validate_hamiltonian,
@@ -601,14 +602,23 @@
             _operation,
             values_shape=values_shape,
             durations=upsampled_durations,
             batch_shape=batch_shape,
         )
 
 
+@deprecated_parameter(
+    deprecated_name="randomized_frequencies_count",
+    new_name="randomized_frequency_count",
+)
+@deprecated_parameter(
+    deprecated_name="optimizable_frequencies_count",
+    new_name="optimizable_frequency_count",
+)
+@deprecated_parameter(deprecated_name="segments_count", new_name="segment_count")
 class RealFourierPwcSignal(Node):
     r"""
     Creates a piecewise-constant signal constructed from Fourier components.
 
     Use this function to create a signal defined in terms of Fourier
     (sine/cosine) basis signals that can be optimized by varying their
     coefficients and, optionally, their frequencies.
@@ -620,32 +630,32 @@
     provide the number of frequencies, and the frequency values are chosen at
     random at the start of each optimization and then held constant).
 
     Parameters
     ----------
     duration : float
         The total duration :math:`\tau` of the signal.
-    segments_count : int
+    segment_count : int
         The number of segments :math:`N` to use for the piecewise-constant
         approximation.
     initial_coefficient_lower_bound : float, optional
         The lower bound :math:`c_\mathrm{min}` on the initial coefficient
         values. Defaults to -1.
     initial_coefficient_upper_bound : float, optional
         The upper bound :math:`c_\mathrm{max}` on the initial coefficient
         values. Defaults to 1.
     fixed_frequencies : list[float], optional
         The fixed non-zero frequencies :math:`\{f_m\}` to use for the Fourier
         basis. Must be non-empty if provided. Must be specified in the inverse
         units of `duration` (for example if `duration` is in seconds, these
         values must be given in Hertz).
-    optimizable_frequencies_count : int, optional
+    optimizable_frequency_count : int, optional
         The number of non-zero frequencies :math:`M` to use, if the
         frequencies can be optimized. Must be greater than zero if provided.
-    randomized_frequencies_count : int, optional
+    randomized_frequency_count : int, optional
         The number of non-zero frequencies :math:`M` to use, if the
         frequencies are to be randomized but fixed. Must be greater than zero
         if provided.
     name : str, optional
         The name of the node.
 
     Returns
@@ -692,54 +702,54 @@
            <https://doi.org/10.1103/PhysRevLett.106.190501>`_
     """
 
     name = "real_fourier_pwc_signal"
     optimizable_variable = True
     args = [
         forge.arg("duration", type=float),
-        forge.arg("segments_count", type=int),
+        forge.arg("segment_count", type=int),
         forge.arg("initial_coefficient_lower_bound", type=float, default=-1),
         forge.arg("initial_coefficient_upper_bound", type=float, default=1),
         forge.arg("fixed_frequencies", type=Optional[List[float]], default=None),
-        forge.arg("optimizable_frequencies_count", type=Optional[int], default=None),
-        forge.arg("randomized_frequencies_count", type=Optional[int], default=None),
+        forge.arg("optimizable_frequency_count", type=Optional[int], default=None),
+        forge.arg("randomized_frequency_count", type=Optional[int], default=None),
     ]
     rtype = types.TensorPwc
 
     @classmethod
     def create_node_data(cls, _operation, **kwargs):
         duration = kwargs.get("duration")
-        segments_count = kwargs.get("segments_count")
+        segment_count = kwargs.get("segment_count")
         check_duration(duration, "duration")
-        check_argument_integer(segments_count, "segments_count")
+        check_argument_integer(segment_count, "segment_count")
         check_argument(
-            segments_count > 0,
+            segment_count > 0,
             "The number of segments must be greater than zero.",
-            {"segments_count": segments_count},
+            {"segment_count": segment_count},
         )
-        durations = duration / segments_count * np.ones(segments_count)
-        optimizable_frequencies_count = kwargs.get("optimizable_frequencies_count")
-        if optimizable_frequencies_count is not None:
+        durations = duration / segment_count * np.ones(segment_count)
+        optimizable_frequency_count = kwargs.get("optimizable_frequency_count")
+        if optimizable_frequency_count is not None:
             check_argument_integer(
-                optimizable_frequencies_count, "optimizable_frequencies_count"
+                optimizable_frequency_count, "optimizable_frequency_count"
             )
             check_argument(
-                optimizable_frequencies_count > 0,
+                optimizable_frequency_count > 0,
                 "The number of optimizable frequencies (if provided) must be greater than zero.",
-                {"optimizable_frequencies_count": optimizable_frequencies_count},
+                {"optimizable_frequency_count": optimizable_frequency_count},
             )
-        randomized_frequencies_count = kwargs.get("randomized_frequencies_count")
-        if randomized_frequencies_count is not None:
+        randomized_frequency_count = kwargs.get("randomized_frequency_count")
+        if randomized_frequency_count is not None:
             check_argument_integer(
-                randomized_frequencies_count, "randomized_frequencies_count"
+                randomized_frequency_count, "randomized_frequency_count"
             )
             check_argument(
-                randomized_frequencies_count > 0,
+                randomized_frequency_count > 0,
                 "The number of randomized frequencies (if provided) must be greater than zero.",
-                {"randomized_frequencies_count": randomized_frequencies_count},
+                {"randomized_frequency_count": randomized_frequency_count},
             )
         return TensorPwcNodeData(
             _operation,
             values_shape=(),
             durations=durations,
             batch_shape=(),
         )
```

### Comparing `qctrl-commons-8.1.0/qctrlcommons/node/registry.py` & `qctrl-commons-9.0.0/qctrlcommons/node/registry.py`

 * *Files identical despite different names*

### Comparing `qctrl-commons-8.1.0/qctrlcommons/node/sparse.py` & `qctrl-commons-9.0.0/qctrlcommons/node/sparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 #
 #     https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 """Module for sparse."""
-import warnings
 from typing import (
     List,
     Optional,
     Union,
 )
 
 import forge
 import numpy as np
 from scipy.sparse import coo_matrix
 
 from qctrlcommons.node import types
 from qctrlcommons.node.base import Node
+from qctrlcommons.node.deprecation import deprecated_node
 from qctrlcommons.node.node_data import (
     SparsePwcNodeData,
     TensorNodeData,
     TensorPwcNodeData,
 )
 from qctrlcommons.node.utils import (
     validate_hamiltonian,
@@ -306,63 +306,14 @@
         if sample_times is None:
             shape = values_shape_state
         else:
             shape = (len(sample_times),) + values_shape_state
         return TensorNodeData(_operation, shape=shape)
 
 
-class EstimatedKrylovSubspaceDimension(Node):
-    r"""
-    This node will be removed in the future.
-    Please use :py:func:`estimated_krylov_subspace_dimension_lanczos` instead.
-    """
-
-    name = "estimated_krylov_subspace_dimension"
-    args = [
-        forge.arg("spectral_range", type=Union[types.Tensor, float]),
-        forge.arg("duration", type=float),
-        forge.arg("maximum_segment_duration", type=float),
-        forge.arg("error_tolerance", type=float, default=1e-6),
-    ]
-    rtype = types.Tensor
-
-    @classmethod
-    def create_node_data(cls, _operation, **kwargs):
-        warnings.warn(
-            "The estimated_krylov_subspace_dimension node will be removed in the future. "
-            "Please use estimated_krylov_subspace_dimension_lanczos instead."
-        )
-        duration = kwargs.get("duration")
-        maximum_segment_duration = kwargs.get("maximum_segment_duration")
-        error_tolerance = kwargs.get("error_tolerance")
-        check_argument(
-            maximum_segment_duration > 0,
-            "The maximum segment duration must be positive.",
-            {"maximum_segment_duration": maximum_segment_duration},
-        )
-        check_argument(
-            duration > 0, "The duration must be positive.", {"duration": duration}
-        )
-        check_argument(
-            maximum_segment_duration <= duration,
-            "The maximum segment duration must be less than or equal to duration.",
-            {
-                "maximum_segment_duration": maximum_segment_duration,
-                "duration": duration,
-            },
-        )
-        check_argument(
-            error_tolerance > 0,
-            "The error tolerance must be positive.",
-            {"error_tolerance": error_tolerance},
-        )
-
-        return TensorNodeData(_operation, shape=())
-
-
 class EstimatedKrylovSubspaceDimensionLanczos(Node):
     r"""
     Calculates an appropriate Krylov subspace dimension (:math:`k`) to use in the Lanczos
     integrator while keeping the total error in the evolution below a given error tolerance.
 
     Note that you can provide your own estimation of the Hamiltonian spectral range or use the
     `spectral_range` operation to perform that calculation.
@@ -454,14 +405,23 @@
             "The error tolerance must be positive.",
             {"error_tolerance": error_tolerance},
         )
 
         return TensorNodeData(_operation, shape=())
 
 
+@deprecated_node("estimated_krylov_subspace_dimension_lanczos")
+class EstimatedKrylovSubspaceDimensionDeprecated(
+    EstimatedKrylovSubspaceDimensionLanczos
+):
+    """Deprecated node."""
+
+    name = "estimated_krylov_subspace_dimension"
+
+
 class SpectralRange(Node):
     r"""
     Obtains the range of the eigenvalues of a Hermitian operator.
 
     This function provides an estimate of the difference between the
     highest and the lowest eigenvalues of the operator. You can adjust its
     precision by modifying its default parameters.
```

### Comparing `qctrl-commons-8.1.0/qctrlcommons/node/stf.py` & `qctrl-commons-9.0.0/qctrlcommons/node/stf.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 )
 
 import forge
 import numpy as np
 
 from qctrlcommons.node import types
 from qctrlcommons.node.base import Node
+from qctrlcommons.node.deprecation import deprecated_parameter
 from qctrlcommons.node.node_data import (
     StfNodeData,
     TensorNodeData,
     TensorPwcNodeData,
 )
 from qctrlcommons.node.utils import (
     validate_batch_and_values_shapes,
@@ -262,14 +263,18 @@
         return StfNodeData(
             _operation,
             values_shape=values_shape,
             batch_shape=batch_shape,
         )
 
 
+@deprecated_parameter(
+    deprecated_name="samples_per_segment", new_name="sample_count_per_segment"
+)
+@deprecated_parameter(deprecated_name="segments_count", new_name="segment_count")
 class DiscretizeStf(Node):
     r"""
     Creates a piecewise-constant function by discretizing a sampleable function.
 
     Use this function to create a piecewise-constant approximation to a sampleable
     function (obtained, for example, by filtering an initial
     piecewise-constant function).
@@ -281,18 +286,18 @@
         function can have any shape. You can also provide a batch of
         functions, in which case the discretization is applied to each
         element of the batch.
     duration : float
         The duration :math:`\tau` over which discretization should be
         performed. The resulting piecewise-constant function has this
         duration.
-    segments_count : int
+    segment_count : int
         The number of segments :math:`N` in the resulting piecewise-constant
         function.
-    samples_per_segment : int, optional
+    sample_count_per_segment : int, optional
         The number of samples :math:`M` of the sampleable function to take when
         calculating the value of each segment in the discretization. Defaults
         to 1.
     name : str, optional
         The name of the node.
 
     Returns
@@ -323,41 +328,41 @@
     sample_stf : Sample an `Stf` at given times.
     """
 
     name = "discretize_stf"
     args = [
         forge.arg("stf", type=types.Stf),
         forge.arg("duration", type=float),
-        forge.arg("segments_count", type=int),
-        forge.arg("samples_per_segment", type=int, default=1),
+        forge.arg("segment_count", type=int),
+        forge.arg("sample_count_per_segment", type=int, default=1),
     ]
     rtype = types.TensorPwc
 
     @classmethod
     def create_node_data(cls, _operation, **kwargs):
         stf = kwargs.get("stf")
         duration = kwargs.get("duration")
-        segments_count = kwargs.get("segments_count")
+        segment_count = kwargs.get("segment_count")
         batch_shape, values_shape = validate_batch_and_values_shapes(
             stf,
             "stf",
         )
-        check_argument_integer(segments_count, "segments_count")
+        check_argument_integer(segment_count, "segment_count")
         check_argument(
-            segments_count > 0,
+            segment_count > 0,
             "The number of segments must be greater than zero.",
-            {"segments_count": segments_count},
+            {"segment_count": segment_count},
         )
-        durations = duration / segments_count * np.ones(segments_count)
-        samples_per_segment = kwargs.get("samples_per_segment")
-        check_argument_integer(samples_per_segment, "samples_per_segment")
+        durations = duration / segment_count * np.ones(segment_count)
+        sample_count_per_segment = kwargs.get("sample_count_per_segment")
+        check_argument_integer(sample_count_per_segment, "sample_count_per_segment")
         check_argument(
-            samples_per_segment > 0,
+            sample_count_per_segment > 0,
             "The number of samples per segment to take must be greater than zero.",
-            {"samples_per_segment": samples_per_segment},
+            {"sample_count_per_segment": sample_count_per_segment},
         )
         return TensorPwcNodeData(
             _operation,
             values_shape=values_shape,
             durations=durations,
             batch_shape=batch_shape,
         )
```

### Comparing `qctrl-commons-8.1.0/qctrlcommons/node/tensorflow.py` & `qctrl-commons-9.0.0/qctrlcommons/node/tensorflow.py`

 * *Files identical despite different names*

### Comparing `qctrl-commons-8.1.0/qctrlcommons/node/types.py` & `qctrl-commons-9.0.0/qctrlcommons/node/types.py`

 * *Files identical despite different names*

### Comparing `qctrl-commons-8.1.0/qctrlcommons/node/unary.py` & `qctrl-commons-9.0.0/qctrlcommons/node/unary.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
 # pylint: disable=too-many-lines
 """Module for unary operation nodes."""
 
-import warnings
 from typing import (
     Tuple,
     Union,
 )
 
 import forge
 import numpy as np
 
 from qctrlcommons.node import (
     node_data,
     types,
 )
 from qctrlcommons.node.base import Node
+from qctrlcommons.node.deprecation import deprecated_node
 from qctrlcommons.node.utils import (
     NumericOrFunction,
     validate_batch_and_values_shapes,
     validate_shape,
 )
 from qctrlcommons.preconditions import (
     check_argument,
@@ -411,28 +411,19 @@
     rtype = Union[types.Tensor, types.TensorPwc, types.Stf]
 
     @classmethod
     def create_node_data(cls, _operation, **kwargs):
         return _create_flexible_unary_node_data(_operation, **kwargs)
 
 
+@deprecated_node("negative")
 class NegDeprecated(Negative):
-    r"""
-    This node has been deprecated and will be removed in the future.
-    Please use :py:func:`negative` instead.
-    """
-    name = "neg"
+    """Deprecated node."""
 
-    @classmethod
-    def create_node_data(cls, _operation, **kwargs):
-        warnings.warn(
-            "The 'neg' node will be removed in the future. "
-            "Please use 'negative' instead."
-        )
-        return super().create_node_data(_operation, **kwargs)
+    name = "neg"
 
 
 class Real(Node):
     r"""
     Returns the element-wise real part of an object. This can be a number, an array,
     a tensor, or a time-dependent function in the form of a TensorPwc or an Stf.
```

### Comparing `qctrl-commons-8.1.0/qctrlcommons/node/utils.py` & `qctrl-commons-9.0.0/qctrlcommons/node/utils.py`

 * *Files identical despite different names*

### Comparing `qctrl-commons-8.1.0/qctrlcommons/node/wrapper.py` & `qctrl-commons-9.0.0/qctrlcommons/node/wrapper.py`

 * *Files identical despite different names*

### Comparing `qctrl-commons-8.1.0/qctrlcommons/preconditions.py` & `qctrl-commons-9.0.0/qctrlcommons/preconditions.py`

 * *Files identical despite different names*

### Comparing `qctrl-commons-8.1.0/qctrlcommons/serializers.py` & `qctrl-commons-9.0.0/qctrlcommons/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     ComplexNumber,
     FloatConstant,
     GraphDataType,
     NumpyArray,
     NumpyComplexNumber,
     NumpyScalar,
     OperationDataType,
+    QuantumObject,
     SliceDataType,
     SparseMatrix,
 )
 
 
 class DataTypeMixin:  # pylint:disable=too-few-public-methods
     """Mixin class that defines the available data types in precedence order.
@@ -47,14 +48,15 @@
         NumpyScalar(),
         ComplexNumber(),
         OperationDataType(),
         GraphDataType(),
         SliceDataType(),
         SparseMatrix(),
         FloatConstant(),
+        QuantumObject(),
     ]
 
 
 class DataTypeDecoder(json.JSONDecoder, DataTypeMixin):
     """Represent DataTypeDecoder Model."""
 
     def __init__(self, *args, **kwargs):
```

### Comparing `qctrl-commons-8.1.0/qctrlcommons/utils.py` & `qctrl-commons-9.0.0/qctrlcommons/utils.py`

 * *Files identical despite different names*

### Comparing `qctrl-commons-8.1.0/setup.py` & `qctrl-commons-9.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'python-forge>=18.6.0,<19.0.0',
  'pythonflow>=0.3.0,<0.4.0',
  'scipy>=1.4.1',
  'toml>=0.10.0,<0.11.0']
 
 setup_kwargs = {
     'name': 'qctrl-commons',
-    'version': '8.1.0',
+    'version': '9.0.0',
     'description': 'Q-CTRL Python Commons',
     'long_description': '# Q-CTRL Python Commons\n\nQ-CTRL Python Commons is a collection of common libraries for the Python language.\n',
     'author': 'Q-CTRL',
     'author_email': 'support@q-ctrl.com',
     'maintainer': 'Q-CTRL',
     'maintainer_email': 'support@q-ctrl.com',
     'url': 'https://q-ctrl.com',
```

### Comparing `qctrl-commons-8.1.0/PKG-INFO` & `qctrl-commons-9.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl-commons
-Version: 8.1.0
+Version: 9.0.0
 Summary: Q-CTRL Python Commons
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: q-ctrl,qctrl,quantum control
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
```

