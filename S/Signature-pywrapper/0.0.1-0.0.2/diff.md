# Comparing `tmp/Signature_pywrapper-0.0.1.tar.gz` & `tmp/Signature_pywrapper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signature_pywrapper-0.0.1.tar", last modified: Sat Jun  3 11:52:57 2023, max compression
+gzip compressed data, was "Signature_pywrapper-0.0.2.tar", last modified: Thu Jun 15 07:52:45 2023, max compression
```

## Comparing `Signature_pywrapper-0.0.1.tar` & `Signature_pywrapper-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 11:52:57.136966 Signature_pywrapper-0.0.1/
--rw-rw-rw-   0        0        0     1100 2023-06-03 10:58:27.000000 Signature_pywrapper-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3398 2023-06-03 11:52:57.136966 Signature_pywrapper-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2461 2023-06-03 11:49:17.000000 Signature_pywrapper-0.0.1/README.md
--rw-rw-rw-   0        0        0     1344 2023-06-03 11:52:57.146973 Signature_pywrapper-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      123 2023-06-03 10:58:27.000000 Signature_pywrapper-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 11:52:57.079925 Signature_pywrapper-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-03 11:52:57.103943 Signature_pywrapper-0.0.1/src/Signature_pywrapper/
--rw-rw-rw-   0        0        0      143 2023-06-03 11:49:16.000000 Signature_pywrapper-0.0.1/src/Signature_pywrapper/__init__.py
--rw-rw-rw-   0        0        0    58284 2023-06-03 10:58:27.000000 Signature_pywrapper-0.0.1/src/Signature_pywrapper/commons-cli-1.5.0.jar
--rw-rw-rw-   0        0        0     2317 2023-06-03 10:58:27.000000 Signature_pywrapper-0.0.1/src/Signature_pywrapper/eSignature.jar
--rw-rw-rw-   0        0        0     9288 2023-06-03 11:44:47.000000 Signature_pywrapper-0.0.1/src/Signature_pywrapper/signature_wrapper.py
--rw-rw-rw-   0        0        0    97214 2023-06-03 10:58:27.000000 Signature_pywrapper-0.0.1/src/Signature_pywrapper/signatures-1.2-SNAPSHOT.jar
--rw-rw-rw-   0        0        0     3448 2023-06-03 10:58:27.000000 Signature_pywrapper-0.0.1/src/Signature_pywrapper/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-03 11:52:57.135965 Signature_pywrapper-0.0.1/src/Signature_pywrapper.egg-info/
--rw-rw-rw-   0        0        0     3398 2023-06-03 11:52:57.000000 Signature_pywrapper-0.0.1/src/Signature_pywrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      521 2023-06-03 11:52:57.000000 Signature_pywrapper-0.0.1/src/Signature_pywrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 11:52:57.000000 Signature_pywrapper-0.0.1/src/Signature_pywrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      157 2023-06-03 11:52:57.000000 Signature_pywrapper-0.0.1/src/Signature_pywrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-03 11:52:57.000000 Signature_pywrapper-0.0.1/src/Signature_pywrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 07:52:45.493056 Signature_pywrapper-0.0.2/
+-rw-rw-rw-   0        0        0     1100 2023-02-07 12:55:09.000000 Signature_pywrapper-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3398 2023-06-15 07:52:45.493056 Signature_pywrapper-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2461 2023-06-15 07:36:07.000000 Signature_pywrapper-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1344 2023-06-15 07:52:45.506122 Signature_pywrapper-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      123 2023-02-07 12:55:09.000000 Signature_pywrapper-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:52:45.412849 Signature_pywrapper-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-15 07:52:45.452895 Signature_pywrapper-0.0.2/src/Signature_pywrapper/
+-rw-rw-rw-   0        0        0      143 2023-06-15 07:51:06.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper/__init__.py
+-rw-rw-rw-   0        0        0    58284 2020-01-22 14:10:16.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper/commons-cli-1.5.0.jar
+-rw-rw-rw-   0        0        0     2317 2023-06-02 12:59:46.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper/eSignature.jar
+-rw-rw-rw-   0        0        0     9449 2023-06-15 07:50:28.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper/signature_wrapper.py
+-rw-rw-rw-   0        0        0    97214 2023-06-02 08:29:00.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper/signatures-1.2-SNAPSHOT.jar
+-rw-rw-rw-   0        0        0     3448 2023-06-02 13:16:29.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:52:45.491056 Signature_pywrapper-0.0.2/src/Signature_pywrapper.egg-info/
+-rw-rw-rw-   0        0        0     3398 2023-06-15 07:52:45.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      521 2023-06-15 07:52:45.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 07:52:45.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      157 2023-06-15 07:52:45.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-15 07:52:45.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper.egg-info/top_level.txt
```

### Comparing `Signature_pywrapper-0.0.1/LICENSE` & `Signature_pywrapper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Signature_pywrapper-0.0.1/PKG-INFO` & `Signature_pywrapper-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signature_pywrapper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper for signature molecular descriptors
 Home-page: https://github.com/OlivierBeq/Signature_pywrapper
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: signature molecular descriptors,cheminformatics,toxicoinformatics,QSAR
@@ -41,15 +41,15 @@
 
     git clone https://github.com/OlivierBeq/Signature_pywrapper.git
     pip install ./Signature_pywrapper
 
 with pip:
 
 ```bash
-pip install signature-pywrapper
+pip install Signature-pywrapper
 ```
 
 ### Get started
 
 ```python
 from Signature_pywrapper import Signature
```

### Comparing `Signature_pywrapper-0.0.1/README.md` & `Signature_pywrapper-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     git clone https://github.com/OlivierBeq/Signature_pywrapper.git
     pip install ./Signature_pywrapper
 
 with pip:
 
 ```bash
-pip install signature-pywrapper
+pip install Signature-pywrapper
 ```
 
 ### Get started
 
 ```python
 from Signature_pywrapper import Signature
```

### Comparing `Signature_pywrapper-0.0.1/setup.cfg` & `Signature_pywrapper-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `Signature_pywrapper-0.0.1/src/Signature_pywrapper/commons-cli-1.5.0.jar` & `Signature_pywrapper-0.0.2/src/Signature_pywrapper/commons-cli-1.5.0.jar`

 * *Files identical despite different names*

### Comparing `Signature_pywrapper-0.0.1/src/Signature_pywrapper/eSignature.jar` & `Signature_pywrapper-0.0.2/src/Signature_pywrapper/eSignature.jar`

 * *Files identical despite different names*

### Comparing `Signature_pywrapper-0.0.1/src/Signature_pywrapper/signature_wrapper.py` & `Signature_pywrapper-0.0.2/src/Signature_pywrapper/signature_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import pandas as pd
 from bounded_pool_executor import BoundedProcessPoolExecutor
 from rdkit import Chem
 from rdkit.rdBase import BlockLogs
 
 from .utils import install_java, mktempfile, needsHs
 
+
 class Signature:
     """Wrapper to obtain signature molecular descriptors from
     Gilleain Torrance's re-write of Jean-Loup Faulon's signature
     code for molecules (https://github.com/gilleain/signatures/).
 
     The Signature Molecular Descriptor. 2. Enumerating Molecules from Their Extended Valence Sequences
     Jean-Loup Faulon, Carla J. Churchwell, and Donald P. Visco
@@ -39,15 +40,16 @@
         """Instantiate a wrapper to calculate signature molecular descriptors."""
         # Path to the JAR file
         self._jarfile = os.path.abspath(os.path.join(__file__, os.pardir, 'eSignature.jar'))
         # Ensure the jar file exists
         if not os.path.isfile(self._jarfile):
             raise IOError('The required JAR file is not present. Reinstall Signature_pywrapper.')
 
-    def calculate(self, mols: Iterable[Chem.Mol], depth: Union[int, List[int]] = 3, show_banner: bool = True, njobs: int = 1,
+    def calculate(self, mols: Iterable[Chem.Mol], depth: Union[int, List[int]] = 3,
+                  show_banner: bool = True, njobs: int = 1,
                   chunksize: Optional[int] = 1000) -> pd.DataFrame:
         """Calclulate signature descriptors.
 
         :param mols: RDKit molecules for which signature descriptors should be calculated
         :param depth: depth of the signature
         :param show_banner: If True, show notice on signature descriptors usage
         :param njobs: number of concurrent processes
@@ -153,35 +155,35 @@
 
     def _run_command(self, command: str) -> pd.DataFrame:
         """Run the eSignature command.
 
         :param command: The command to be run.
         """
         with Popen(command.split(), stdout=PIPE) as process:
-            results = re.split('\r?\n\r?\n', process.stdout.read().decode()) # results per molecule
+            results = re.split('\r?\n\r?\n', process.stdout.read().decode())  # results per molecule
         # Organize results
         out = []
         for result in results:
             if len(result) > 0:
                 out.append(Counter([line.strip().split('\t')[1] for line in result.split('\n')]))
         values = pd.DataFrame(out)
         values.index.name = 'index'
         return values
 
     def _calculate(self, mols: List[Chem.Mol]) -> pd.DataFrame:
         """Calculate PaDEL descriptors on one process.
 
         :param mols: RDkit molecules for which PaDEL descriptors should be calculated.
         :param depth: depth of each vertex's signature
-        :return: a pandas DataFrame containing signature desciptor values and the path to the temp dir to be removed
+        :return: a pandas DataFrame containing signature descriptor values and the path to the temp dir to be removed
         """
         results = []
         # Run command for each depth
         for i, depth in enumerate(self.depths):
-            if i == 0: # Avoid overwriting SD file
+            if i == 0:  # Avoid overwriting SD file
                 # Prepare inputs
                 command = self._prepare_command(mols, depth)
             else:
                 command = command[: command.rfind(' ') + 1] + f'{depth}'
             # Run command and obtain results
             results.append(self._run_command(command))
         # Combine depths
@@ -193,16 +195,19 @@
         self._cleanup()
         # Insert lines of skipped molecules
         if len(self._skipped):
             results = (pd.DataFrame(np.insert(results.values, self._skipped,
                                               values=[np.NaN] * len(results.columns),
                                               axis=0),
                                     columns=results.columns)
-                       .fillna(0)
-                       .astype(int))
+                       )
+        results = (results.apply(lambda x: pd.to_numeric(x, errors='coerce'))
+                          .fillna(0)
+                          .convert_dtypes()
+                   )
         return results
 
     def _multiproc_calculate(self, mols: List[Chem.Mol]) -> pd.DataFrame:
         """Calculate signature descriptors in thread-safe manner.
 
         :param mols: RDkit molecules for which signature descriptors should be calculated.
         :return: a pandas DataFrame containing signature descriptor values and the path to the temp dir to be removed
```

### Comparing `Signature_pywrapper-0.0.1/src/Signature_pywrapper/signatures-1.2-SNAPSHOT.jar` & `Signature_pywrapper-0.0.2/src/Signature_pywrapper/signatures-1.2-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `Signature_pywrapper-0.0.1/src/Signature_pywrapper/utils.py` & `Signature_pywrapper-0.0.2/src/Signature_pywrapper/utils.py`

 * *Files identical despite different names*

### Comparing `Signature_pywrapper-0.0.1/src/Signature_pywrapper.egg-info/PKG-INFO` & `Signature_pywrapper-0.0.2/src/Signature_pywrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signature-pywrapper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper for signature molecular descriptors
 Home-page: https://github.com/OlivierBeq/Signature_pywrapper
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: signature molecular descriptors,cheminformatics,toxicoinformatics,QSAR
@@ -41,15 +41,15 @@
 
     git clone https://github.com/OlivierBeq/Signature_pywrapper.git
     pip install ./Signature_pywrapper
 
 with pip:
 
 ```bash
-pip install signature-pywrapper
+pip install Signature-pywrapper
 ```
 
 ### Get started
 
 ```python
 from Signature_pywrapper import Signature
```

### Comparing `Signature_pywrapper-0.0.1/src/Signature_pywrapper.egg-info/SOURCES.txt` & `Signature_pywrapper-0.0.2/src/Signature_pywrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

