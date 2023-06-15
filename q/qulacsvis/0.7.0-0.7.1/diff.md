# Comparing `tmp/qulacsvis-0.7.0.tar.gz` & `tmp/qulacsvis-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qulacsvis-0.7.0.tar", max compression
+gzip compressed data, was "qulacsvis-0.7.1.tar", max compression
```

## Comparing `qulacsvis-0.7.0.tar` & `qulacsvis-0.7.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1069 2023-03-14 08:24:33.925439 qulacsvis-0.7.0/LICENSE
--rw-r--r--   0        0        0     4131 2023-03-14 08:24:33.925439 qulacsvis-0.7.0/README.md
--rw-r--r--   0        0        0     1063 2023-03-14 08:24:33.925439 qulacsvis-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       50 2023-03-14 08:24:33.925439 qulacsvis-0.7.0/qulacsvis/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:24:33.925439 qulacsvis-0.7.0/qulacsvis/utils/__init__.py
--rw-r--r--   0        0        0     2669 2023-03-14 08:24:33.925439 qulacsvis-0.7.0/qulacsvis/utils/gate.py
--rw-r--r--   0        0        0     3894 2023-03-14 08:24:33.925439 qulacsvis-0.7.0/qulacsvis/utils/latex.py
--rw-r--r--   0        0        0      243 2023-03-14 08:24:33.925439 qulacsvis-0.7.0/qulacsvis/visualization/__init__.py
--rw-r--r--   0        0        0     4503 2023-03-14 08:24:33.925439 qulacsvis-0.7.0/qulacsvis/visualization/circuit_drawer.py
--rw-r--r--   0        0        0     3877 2023-03-14 08:24:33.925439 qulacsvis-0.7.0/qulacsvis/visualization/circuit_parser.py
--rw-r--r--   0        0        0     9389 2023-03-14 08:24:33.925439 qulacsvis-0.7.0/qulacsvis/visualization/latex.py
--rw-r--r--   0        0        0    15987 2023-03-14 08:24:33.925439 qulacsvis-0.7.0/qulacsvis/visualization/matplotlib.py
--rw-r--r--   0        0        0    34179 2023-03-14 08:24:33.925439 qulacsvis-0.7.0/qulacsvis/visualization/text.py
--rw-r--r--   0        0        0     5150 1970-01-01 00:00:00.000000 qulacsvis-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-15 09:04:22.075056 qulacsvis-0.7.1/LICENSE
+-rw-r--r--   0        0        0     4131 2023-06-15 09:04:22.075056 qulacsvis-0.7.1/README.md
+-rw-r--r--   0        0        0     1063 2023-06-15 09:04:22.075056 qulacsvis-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-06-15 09:04:22.075056 qulacsvis-0.7.1/qulacsvis/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 09:04:22.079056 qulacsvis-0.7.1/qulacsvis/utils/__init__.py
+-rw-r--r--   0        0        0     2720 2023-06-15 09:04:22.079056 qulacsvis-0.7.1/qulacsvis/utils/gate.py
+-rw-r--r--   0        0        0     3894 2023-06-15 09:04:22.079056 qulacsvis-0.7.1/qulacsvis/utils/latex.py
+-rw-r--r--   0        0        0      243 2023-06-15 09:04:22.079056 qulacsvis-0.7.1/qulacsvis/visualization/__init__.py
+-rw-r--r--   0        0        0     4503 2023-06-15 09:04:22.079056 qulacsvis-0.7.1/qulacsvis/visualization/circuit_drawer.py
+-rw-r--r--   0        0        0     3877 2023-06-15 09:04:22.079056 qulacsvis-0.7.1/qulacsvis/visualization/circuit_parser.py
+-rw-r--r--   0        0        0     9492 2023-06-15 09:04:22.079056 qulacsvis-0.7.1/qulacsvis/visualization/latex.py
+-rw-r--r--   0        0        0    16480 2023-06-15 09:04:22.079056 qulacsvis-0.7.1/qulacsvis/visualization/matplotlib.py
+-rw-r--r--   0        0        0    34179 2023-06-15 09:04:22.079056 qulacsvis-0.7.1/qulacsvis/visualization/text.py
+-rw-r--r--   0        0        0     5150 1970-01-01 00:00:00.000000 qulacsvis-0.7.1/PKG-INFO
```

### Comparing `qulacsvis-0.7.0/LICENSE` & `qulacsvis-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qulacsvis-0.7.0/README.md` & `qulacsvis-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `qulacsvis-0.7.0/pyproject.toml` & `qulacsvis-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qulacsvis"
-version = "0.7.0"
+version = "0.7.1"
 readme = "README.md"
 description = "visualizers for qulacs"
 repository = "https://github.com/Qulacs-Osaka/qulacs-visualizer"
 homepage = "https://github.com/Qulacs-Osaka/qulacs-visualizer"
 documentation = "https://qulacs-osaka.github.io/qulacs-visualizer"
 authors = ["Qulacs-Osaka <you@example.com>"]
 license = "MIT"
```

### Comparing `qulacsvis-0.7.0/qulacsvis/utils/gate.py` & `qulacsvis-0.7.1/qulacsvis/utils/gate.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "Y-rotation": "RY",
     "Z-rotation": "RZ",
     "Pauli": "Pau",
     "Pauli-rotation": "PR",
     "CZ": "CZ",
     "CNOT": "CX",
     "SWAP": "SWP",
+    "Toffoli": "CCX",
     "Reflection": "Ref",
     "ReversibleBoolean": "ReB",
     "DenseMatrix": "DeM",
     "DinagonalMatrix": "DiM",
     "SparseMatrix": "SpM",
     "Generic gate": "GeG",
     "ParametricRX": "pRX",
@@ -47,14 +48,15 @@
         "Tdag": r"T^\dag",
         "sqrtX": r"\sqrt{X}",
         "sqrtXdag": r"\sqrt{X^\dag}",
         "sqrtY": r"\sqrt{Y}",
         "sqrtYdag": r"\sqrt{Y^\dag}",
         "CNOT": r"\targ",
         "SWAP": r"\qswap",
+        "Toffoli": r"\targ",
         "wire": r"\qw",
         "ghost": "ghost",
     },
 )
 
 
 def to_text_style(gate_name: str) -> str:
```

### Comparing `qulacsvis-0.7.0/qulacsvis/utils/latex.py` & `qulacsvis-0.7.1/qulacsvis/utils/latex.py`

 * *Files identical despite different names*

### Comparing `qulacsvis-0.7.0/qulacsvis/visualization/circuit_drawer.py` & `qulacsvis-0.7.1/qulacsvis/visualization/circuit_drawer.py`

 * *Files identical despite different names*

### Comparing `qulacsvis-0.7.0/qulacsvis/visualization/circuit_parser.py` & `qulacsvis-0.7.1/qulacsvis/visualization/circuit_parser.py`

 * *Files identical despite different names*

### Comparing `qulacsvis-0.7.0/qulacsvis/visualization/latex.py` & `qulacsvis-0.7.1/qulacsvis/visualization/latex.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,16 @@
 
                 if gate.name == "ghost":
                     continue
                 elif gate.name == "wire":
                     continue
                 elif gate.name == "CNOT":
                     self._cnot(current_layer_latex, gate)
+                elif gate.name == "Toffoli":
+                    self._cnot(current_layer_latex, gate)
                 elif gate.name == "SWAP":
                     self._swap(current_layer_latex, gate)
                 elif len(gate.target_bits) > 1:
                     self._multi_gate(current_layer_latex, gate)
                 else:
                     self._gate(current_layer_latex, gate)
```

### Comparing `qulacsvis-0.7.0/qulacsvis/visualization/matplotlib.py` & `qulacsvis-0.7.1/qulacsvis/visualization/matplotlib.py`

 * *Files 5% similar despite different names*

```diff
@@ -182,14 +182,16 @@
                 qubit_ypos = qubit * (GATE_DEFAULT_HEIGHT + GATE_MARGIN_BOTTOM)
                 if gate.name == "ghost":
                     continue
                 elif gate.name == "wire":
                     continue
                 elif gate.name == "CNOT":
                     self._cnot(gate, (layer_xpos, qubit_ypos))
+                elif gate.name == "Toffoli":
+                    self._cnot(gate, (layer_xpos, qubit_ypos))
                 elif gate.name == "SWAP":
                     self._swap(gate, (layer_xpos, qubit_ypos))
                 elif len(gate.target_bits) > 1:
                     self._multi_gate(gate, (layer_xpos, qubit_ypos))
                 else:
                     self._gate_with_size(gate, (layer_xpos, qubit_ypos), 1)
 
@@ -338,15 +340,18 @@
             zorder=PORDER_GATE,
         )
         self._ax.add_patch(box)
 
         if gate.name == "":
             latex_style_gate_str = ""
         else:
-            latex_style_gate_str = f"${to_latex_style(gate.name)}$"
+            try:
+                latex_style_gate_str = f"${to_latex_style(gate.name)}$"
+            except KeyError:
+                latex_style_gate_str = gate.name
 
         self._text(xpos, ypos, latex_style_gate_str)
         self._control_bits(gate.control_bit_infos, (xpos, ypos))
 
     def _multi_gate(self, gate: GateData, xy: Tuple[float, float]) -> None:
         """
         Draw a multi-gate. (e.g., DensityMatrixGate)
@@ -395,22 +400,34 @@
 
         Raise
         -----
         ValueError
             If the gate does not have a control bit.
         """
 
-        xpos, ypos = xy
-        TARGET_QUBIT_RADIUS: Final[float] = 0.4
-
         if gate.control_bit_infos is None:
             raise ValueError("control_bit_infos is None")
         elif gate.control_bit_infos == []:
             raise ValueError("control_bit_infos is empty")
 
+        self._not_mark(xy)
+        self._control_bits(gate.control_bit_infos, xy)
+
+    def _not_mark(self, xy: Tuple[float, float]) -> None:
+        """
+        Draw a "NOT" mark used in CNOT etc.
+
+        Parameters
+        ----------
+        xy : Tuple[float, float]
+            The position of the gate indicating the target bit of NOT.
+        """
+        xpos, ypos = xy
+        TARGET_QUBIT_RADIUS: Final[float] = 0.4
+
         target = patches.Circle(
             xy=(xpos, ypos),
             radius=TARGET_QUBIT_RADIUS,
             fc="w",
             ec="k",
             zorder=PORDER_GATE,
         )
@@ -425,16 +442,14 @@
         # -
         self._line(
             (xpos - TARGET_QUBIT_RADIUS, ypos),
             (xpos + TARGET_QUBIT_RADIUS, ypos),
             zorder=PORDER_TEXT,
         )
 
-        self._control_bits(gate.control_bit_infos, (xpos, ypos))
-
     def _control_bits(
         self, control_bit_infos: List[ControlQubitInfo], xy_from: Tuple[float, float]
     ) -> None:
         """
         Draw control bits.
 
         Parameters
```

### Comparing `qulacsvis-0.7.0/qulacsvis/visualization/text.py` & `qulacsvis-0.7.1/qulacsvis/visualization/text.py`

 * *Files identical despite different names*

### Comparing `qulacsvis-0.7.0/PKG-INFO` & `qulacsvis-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qulacsvis
-Version: 0.7.0
+Version: 0.7.1
 Summary: visualizers for qulacs
 Home-page: https://github.com/Qulacs-Osaka/qulacs-visualizer
 License: MIT
 Author: Qulacs-Osaka
 Author-email: you@example.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

