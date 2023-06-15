# Comparing `tmp/amin_qvm-1.0.5.tar.gz` & `tmp/amin_qvm-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amin_qvm-1.0.5.tar", last modified: Wed Jun 14 13:28:10 2023, max compression
+gzip compressed data, was "amin_qvm-1.0.6.tar", last modified: Thu Jun 15 03:04:38 2023, max compression
```

## Comparing `amin_qvm-1.0.5.tar` & `amin_qvm-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 13:28:10.470252 amin_qvm-1.0.5/
--rw-rw-rw-   0        0        0     1094 2023-06-14 10:51:44.000000 amin_qvm-1.0.5/LICENSE.ttxt
--rw-rw-rw-   0        0        0     6043 2023-06-14 13:28:10.469256 amin_qvm-1.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 13:28:10.418693 amin_qvm-1.0.5/amin_qvm/
--rw-rw-rw-   0        0        0    89322 2023-06-14 11:39:44.000000 amin_qvm-1.0.5/amin_qvm/QuantumComputer.py
--rw-rw-rw-   0        0        0        0 2023-06-14 11:00:38.000000 amin_qvm-1.0.5/amin_qvm/__init__.py
--rw-rw-rw-   0        0        0     3770 2023-06-14 12:36:27.000000 amin_qvm-1.0.5/amin_qvm/functions.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:28:10.466256 amin_qvm-1.0.5/amin_qvm.egg-info/
--rw-rw-rw-   0        0        0     6043 2023-06-14 13:28:10.000000 amin_qvm-1.0.5/amin_qvm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-06-14 13:28:10.000000 amin_qvm-1.0.5/amin_qvm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 13:28:10.000000 amin_qvm-1.0.5/amin_qvm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-14 13:28:10.000000 amin_qvm-1.0.5/amin_qvm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 13:28:10.000000 amin_qvm-1.0.5/amin_qvm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 13:28:10.474276 amin_qvm-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1183 2023-06-14 13:28:06.000000 amin_qvm-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 03:04:38.467513 amin_qvm-1.0.6/
+-rw-rw-rw-   0        0        0     1094 2023-06-14 10:51:44.000000 amin_qvm-1.0.6/LICENSE.ttxt
+-rw-rw-rw-   0        0        0     6048 2023-06-15 03:04:38.465546 amin_qvm-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 03:04:38.434144 amin_qvm-1.0.6/amin_qvm/
+-rw-rw-rw-   0        0        0    89322 2023-06-15 02:42:02.000000 amin_qvm-1.0.6/amin_qvm/QuantumComputer.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 11:00:38.000000 amin_qvm-1.0.6/amin_qvm/__init__.py
+-rw-rw-rw-   0        0        0     3843 2023-06-14 14:56:01.000000 amin_qvm-1.0.6/amin_qvm/functions.py
+-rw-rw-rw-   0        0        0      543 2023-06-14 14:56:39.000000 amin_qvm-1.0.6/amin_qvm/test.py
+drwxrwxrwx   0        0        0        0 2023-06-15 03:04:38.463548 amin_qvm-1.0.6/amin_qvm.egg-info/
+-rw-rw-rw-   0        0        0     6048 2023-06-15 03:04:38.000000 amin_qvm-1.0.6/amin_qvm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-06-15 03:04:38.000000 amin_qvm-1.0.6/amin_qvm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 03:04:38.000000 amin_qvm-1.0.6/amin_qvm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-15 03:04:38.000000 amin_qvm-1.0.6/amin_qvm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 03:04:38.000000 amin_qvm-1.0.6/amin_qvm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 03:04:38.469510 amin_qvm-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1183 2023-06-15 03:04:34.000000 amin_qvm-1.0.6/setup.py
```

### Comparing `amin_qvm-1.0.5/LICENSE.ttxt` & `amin_qvm-1.0.6/LICENSE.ttxt`

 * *Files identical despite different names*

### Comparing `amin_qvm-1.0.5/PKG-INFO` & `amin_qvm-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amin_qvm
-Version: 1.0.5
+Version: 1.0.6
 Summary: Amin-QVM: Quantum Computing Library
 Home-page: https://github.com/amin1029384756/QVM
 Author: Amin Alogaili
 Author-email: aminalogai@gmail.com
 Keywords: quantum computing library simulation amin alogaili QVM aminalogaili
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 
 You won't believe it, but this code supports 100% of the examples from the IBM tutorial. Yep, every single one. And it's not just limited to that. There are tons of additional tests and examples that you can explore. The whole implementation is pretty compact too, with only 675 lines of code for the 5-qubit quantum computer simulator. Plus, there are twice as many lines dedicated to test programs and examples.
 
 To give you a taste of what you can do, check out this example. You can create a quantum computer object, write some mind-bending code in the Quantum Composer style, and execute it. In this case, we're creating a super cool GHZ state:
 
 .. code-block:: python
 
-   from amin_qvm import QuantumComputer
+   from amin_qvm.QuantumComputer import *
 
    ghz_example_code = """
    h q[0];
    h q[1];
    x q[2];
    cx q[1], q[2];
    cx q[0], q[2];
@@ -43,15 +43,15 @@
    Probability.pretty_print_probabilities(qc.qubits.get_quantum_register_containing("q0").get_state())
 
 And voila! It will print out the probabilities of different states. Mind-blowing, right?
 
 You can also dive deeper into the quantum realm by working with individual states and gates directly in pure Python. It's like being a quantum wizard! You can create states, apply gates, and see the magic unfold. Here's an example based on the "Swap Qubits" tutorial from IBM:
 
 .. code-block:: python
-
+   
    # Swap Qubits example IBM tutorial Section IV, Page 2
    qc = QuantumComputer()
    qc.apply_gate(Gate.X, "q2")
    qc.apply_two_qubit_gate_CNOT("q1", "q2")
    qc.apply_gate(Gate.H, "q1")
    qc.apply_gate(Gate.H, "q2")
    qc.apply_two_qubit_gate_CNOT("q1", "q2")
```

### Comparing `amin_qvm-1.0.5/amin_qvm/QuantumComputer.py` & `amin_qvm-1.0.6/amin_qvm/QuantumComputer.py`

 * *Files identical despite different names*

### Comparing `amin_qvm-1.0.5/amin_qvm/functions.py` & `amin_qvm-1.0.6/amin_qvm/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from qiskit import QuantumCircuit, Aer, execute
 import pennylane as qml
 from pennylane import numpy as np
 from sklearn.preprocessing import StandardScaler
 
 
 def quantum_model(params, x):
-    qml.Rot(*params[0], wires=0)
-    qml.Rot(*params[1], wires=1)
+    dev = qml.device("default.qubit", wires=2)
+    qml.Rot(*params[0], wires=0)(*x)
+    qml.Rot(*params[1], wires=1)(*x)
     qml.CNOT(wires=[0, 1])
-    qml.Rot(*params[2], wires=0)
-    qml.Rot(*params[3], wires=1)
-    return qml.expval(qml.PauliZ(0))
+    qml.Rot(*params[2], wires=0)(*x)
+    qml.Rot(*params[3], wires=1)(*x)
+    return qml.expval(qml.PauliZ(0))(dev)
+
+
 
 
 def cost(params, X, Y):
     predictions = [quantum_model(params, x) for x in X]
     return np.mean((predictions - Y) ** 2)
```

### Comparing `amin_qvm-1.0.5/amin_qvm.egg-info/PKG-INFO` & `amin_qvm-1.0.6/amin_qvm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amin-qvm
-Version: 1.0.5
+Version: 1.0.6
 Summary: Amin-QVM: Quantum Computing Library
 Home-page: https://github.com/amin1029384756/QVM
 Author: Amin Alogaili
 Author-email: aminalogai@gmail.com
 Keywords: quantum computing library simulation amin alogaili QVM aminalogaili
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 
 You won't believe it, but this code supports 100% of the examples from the IBM tutorial. Yep, every single one. And it's not just limited to that. There are tons of additional tests and examples that you can explore. The whole implementation is pretty compact too, with only 675 lines of code for the 5-qubit quantum computer simulator. Plus, there are twice as many lines dedicated to test programs and examples.
 
 To give you a taste of what you can do, check out this example. You can create a quantum computer object, write some mind-bending code in the Quantum Composer style, and execute it. In this case, we're creating a super cool GHZ state:
 
 .. code-block:: python
 
-   from amin_qvm import QuantumComputer
+   from amin_qvm.QuantumComputer import *
 
    ghz_example_code = """
    h q[0];
    h q[1];
    x q[2];
    cx q[1], q[2];
    cx q[0], q[2];
@@ -43,15 +43,15 @@
    Probability.pretty_print_probabilities(qc.qubits.get_quantum_register_containing("q0").get_state())
 
 And voila! It will print out the probabilities of different states. Mind-blowing, right?
 
 You can also dive deeper into the quantum realm by working with individual states and gates directly in pure Python. It's like being a quantum wizard! You can create states, apply gates, and see the magic unfold. Here's an example based on the "Swap Qubits" tutorial from IBM:
 
 .. code-block:: python
-
+   
    # Swap Qubits example IBM tutorial Section IV, Page 2
    qc = QuantumComputer()
    qc.apply_gate(Gate.X, "q2")
    qc.apply_two_qubit_gate_CNOT("q1", "q2")
    qc.apply_gate(Gate.H, "q1")
    qc.apply_gate(Gate.H, "q2")
    qc.apply_two_qubit_gate_CNOT("q1", "q2")
```

### Comparing `amin_qvm-1.0.5/setup.py` & `amin_qvm-1.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'numpy',
     'qiskit',
     'pennylane',
     'scikit-learn',
 ]
 setup(
     name='amin_qvm',
-    version='1.0.5',
+    version='1.0.6',
     author='Amin Alogaili',
     author_email='aminalogai@gmail.com',
     description='Amin-QVM: Quantum Computing Library',
     long_description=long_description,
     url='https://github.com/amin1029384756/QVM',
     packages=['amin_qvm'],
     classifiers=[
```

