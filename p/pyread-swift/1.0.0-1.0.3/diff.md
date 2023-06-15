# Comparing `tmp/pyread_swift-1.0.0.tar.gz` & `tmp/pyread_swift-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyread_swift-1.0.0.tar", last modified: Mon Feb  6 18:39:38 2023, max compression
+gzip compressed data, was "pyread_swift-1.0.3.tar", last modified: Thu Jun 15 19:16:22 2023, max compression
```

## Comparing `pyread_swift-1.0.0.tar` & `pyread_swift-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-02-06 18:39:38.636515 pyread_swift-1.0.0/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     1553 2023-01-28 14:08:46.000000 pyread_swift-1.0.0/LICENCE
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     7353 2023-02-06 18:39:38.636515 pyread_swift-1.0.0/PKG-INFO
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     5141 2023-02-06 17:31:46.000000 pyread_swift-1.0.0/README.md
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      687 2023-02-06 16:27:14.000000 pyread_swift-1.0.0/pyproject.toml
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       38 2023-02-06 18:39:38.636515 pyread_swift-1.0.0/setup.cfg
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-02-06 18:39:38.636515 pyread_swift-1.0.0/src/
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-02-06 18:39:38.636515 pyread_swift-1.0.0/src/pyread_swift/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      115 2023-01-29 02:36:01.000000 pyread_swift-1.0.0/src/pyread_swift/__init__.py
--rw-r--r--   0 mcalpine  (1000) mcalpine  (1000)     9930 2023-02-06 17:48:38.000000 pyread_swift-1.0.0/src/pyread_swift/io.py
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)    10848 2023-01-29 09:23:09.000000 pyread_swift-1.0.0/src/pyread_swift/read_dataset.py
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     2131 2023-01-29 09:23:09.000000 pyread_swift-1.0.0/src/pyread_swift/read_header.py
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)    11037 2023-01-29 09:23:09.000000 pyread_swift-1.0.0/src/pyread_swift/select_region.py
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     7980 2023-01-29 09:30:37.000000 pyread_swift-1.0.0/src/pyread_swift/split_selection.py
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-02-06 18:39:38.636515 pyread_swift-1.0.0/src/pyread_swift.egg-info/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     7353 2023-02-06 18:39:38.000000 pyread_swift-1.0.0/src/pyread_swift.egg-info/PKG-INFO
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      418 2023-02-06 18:39:38.000000 pyread_swift-1.0.0/src/pyread_swift.egg-info/SOURCES.txt
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)        1 2023-02-06 18:39:38.000000 pyread_swift-1.0.0/src/pyread_swift.egg-info/dependency_links.txt
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       66 2023-02-06 18:39:38.000000 pyread_swift-1.0.0/src/pyread_swift.egg-info/requires.txt
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       13 2023-02-06 18:39:38.000000 pyread_swift-1.0.0/src/pyread_swift.egg-info/top_level.txt
+drwxr-sr-x   0 rttw52   (43278) durham   (64528)        0 2023-06-15 19:16:22.000000 pyread_swift-1.0.3/
+-rw-r--r--   0 rttw52   (43278) durham   (64528)     1553 2023-06-15 19:15:51.000000 pyread_swift-1.0.3/LICENCE
+-rw-r--r--   0 rttw52   (43278) durham   (64528)     7453 2023-06-15 19:16:22.000000 pyread_swift-1.0.3/PKG-INFO
+-rw-r--r--   0 rttw52   (43278) durham   (64528)     5241 2023-06-15 19:15:51.000000 pyread_swift-1.0.3/README.md
+-rw-r--r--   0 rttw52   (43278) durham   (64528)      687 2023-06-15 19:15:51.000000 pyread_swift-1.0.3/pyproject.toml
+-rw-r--r--   0 rttw52   (43278) durham   (64528)       38 2023-06-15 19:16:22.000000 pyread_swift-1.0.3/setup.cfg
+drwxr-sr-x   0 rttw52   (43278) durham   (64528)        0 2023-06-15 19:16:22.000000 pyread_swift-1.0.3/src/
+drwxr-sr-x   0 rttw52   (43278) durham   (64528)        0 2023-06-15 19:16:22.000000 pyread_swift-1.0.3/src/pyread_swift/
+-rw-r--r--   0 rttw52   (43278) durham   (64528)      115 2023-06-15 19:15:51.000000 pyread_swift-1.0.3/src/pyread_swift/__init__.py
+-rw-r--r--   0 rttw52   (43278) durham   (64528)     9930 2023-06-15 19:15:51.000000 pyread_swift-1.0.3/src/pyread_swift/io.py
+-rw-r--r--   0 rttw52   (43278) durham   (64528)    10848 2023-06-15 19:15:51.000000 pyread_swift-1.0.3/src/pyread_swift/read_dataset.py
+-rw-r--r--   0 rttw52   (43278) durham   (64528)     2725 2023-06-15 19:15:51.000000 pyread_swift-1.0.3/src/pyread_swift/read_header.py
+-rw-r--r--   0 rttw52   (43278) durham   (64528)    11037 2023-06-15 19:15:51.000000 pyread_swift-1.0.3/src/pyread_swift/select_region.py
+-rw-r--r--   0 rttw52   (43278) durham   (64528)     7980 2023-06-15 19:15:51.000000 pyread_swift-1.0.3/src/pyread_swift/split_selection.py
+drwxr-sr-x   0 rttw52   (43278) durham   (64528)        0 2023-06-15 19:16:22.000000 pyread_swift-1.0.3/src/pyread_swift.egg-info/
+-rw-r--r--   0 rttw52   (43278) durham   (64528)     7453 2023-06-15 19:16:22.000000 pyread_swift-1.0.3/src/pyread_swift.egg-info/PKG-INFO
+-rw-r--r--   0 rttw52   (43278) durham   (64528)      460 2023-06-15 19:16:22.000000 pyread_swift-1.0.3/src/pyread_swift.egg-info/SOURCES.txt
+-rw-r--r--   0 rttw52   (43278) durham   (64528)        1 2023-06-15 19:16:22.000000 pyread_swift-1.0.3/src/pyread_swift.egg-info/dependency_links.txt
+-rw-r--r--   0 rttw52   (43278) durham   (64528)       66 2023-06-15 19:16:22.000000 pyread_swift-1.0.3/src/pyread_swift.egg-info/requires.txt
+-rw-r--r--   0 rttw52   (43278) durham   (64528)       13 2023-06-15 19:16:22.000000 pyread_swift-1.0.3/src/pyread_swift.egg-info/top_level.txt
+drwxr-sr-x   0 rttw52   (43278) durham   (64528)        0 2023-06-15 19:16:22.000000 pyread_swift-1.0.3/tests/
+-rw-r--r--   0 rttw52   (43278) durham   (64528)     1729 2023-06-15 19:15:51.000000 pyread_swift-1.0.3/tests/test_read.py
+-rw-r--r--   0 rttw52   (43278) durham   (64528)     1457 2023-06-15 19:15:51.000000 pyread_swift-1.0.3/tests/test_read_mpi.py
```

### Comparing `pyread_swift-1.0.0/LICENCE` & `pyread_swift-1.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `pyread_swift-1.0.0/PKG-INFO` & `pyread_swift-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyread_swift
-Version: 1.0.0
+Version: 1.0.3
 Summary: Package to read SWIFT simulation snapshots in MPI.
 Author-email: Stuart McAlpine <stuart.mcalpine@fysik.su.se>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, LSST Dark Energy Science Collaboration (DESC)
         All rights reserved.
         
@@ -44,71 +44,84 @@
 
 ## An MPI read routine for Swift simulation snapshots
 
 ``pyread_swift`` is an MPI read routine for [``swiftsim``](https://github.com/SWIFTSIM/swiftsim) snapshots, very similar in style to John Helly's [``read_eagle``](https://gitlab.cosma.dur.ac.uk/jch/Read_Eagle) code to read EAGLE snapshots.
 
 The package can read ``swiftsim`` snapshots both in "collective" (i.e., multiple MPI ranks read from a single file simultaneously) and "distributed" (i.e., each MPI reads an individual snapshot file part in isolation) modes. 
 
-Can also read in pure serial, if no MPI libraries are installed.
-
 ## Installation
 
 ### Requirements
 
 * `OpenMPI` or other MPI library
 * `python>=3.8`
 
 Recommended modules when working on COSMA7:
 
-* `module load gnu_comp/11.1.0 openmpi/4.1.4 parallel_hdf5/1.12.0 python/3.9.1-C7`
-
-### Installation from source
+```bash
+module load gnu_comp/11.1.0 openmpi/4.1.4 parallel_hdf5/1.12.0 python/3.9.1-C7
+```
 
 Given the need for a parallel HDF5 installation, it is recommended you install ``pyread_swift`` within a virtual/conda environment. However you can ofcourse also install directly into your base Python environment if you prefer.
 
 First make sure your `pip` is up-to-date:
 
-* `python3 -m pip install --upgrade pip`
+```bash
+python3 -m pip install --upgrade pip
+```
+
+### Method 1) Installation from PyPi
+
+The easiest method is to install from [``PyPI``](https://pypi.org/project/pyread-swift/)
+
+```bash
+python3 -m pip install pyread-swift
+```
 
-Then you can install the `pyread_swift` package by typing the following in
+### Method 2) Installation from source
+
+Or, you can install directly from source.
+
+First clone the repo, then you can install the `pyread_swift` package by typing the following in
 the root git directory: 
 
-* `python3 -m pip install .[mpi]`
+```bash
+git clone https://github.com/stuartmcalpine/pyread_swift.git
+cd pyread_swift
+python3 -m pip install .
+```
 
-which will install `pyread_swift` and any dependencies (omit ``[mpi]`` for pure serial version).
+which will install `pyread_swift` and any dependencies.
 
 ### MPI installation for collective reading
 
 If you are using `pyread_swift` to load large snapshots over MPI collectively
 (i.e., multiple cores read in parallel from the same file), a bit of additional
 setup is required.
 
 Make sure you have `hdf5` installed with **parallel** compatibility ([see here for details](https://docs.h5py.org/en/stable/mpi.html)).
 
-Then, uninstall any installed versions of `mpi4py` and `h5py`:
-
-* `python3 -m pip uninstall mpi4py h5py`
-
-and reinstall then from source, with MPI flags:
-
-* `MPICC=mpicc CC=mpicc HDF5_MPI="ON" python3 -m pip install --no-binary=mpi4py mpi4py`
+Then, uninstall any versions of `h5py` and reinstall from source:
 
-* `MPICC=mpicc CC=mpicc HDF5_MPI="ON" python3 -m pip install --no-binary=h5py h5py`
+```bash
+python3 -m pip uninstall h5py
+MPICC=mpicc CC=mpicc HDF5_MPI="ON" python3 -m pip install --no-binary=h5py h5py
+```
 
 If `pip` struggles to find your `HDF5` libraries automatically, e.g., `error: libhdf5.so: cannot open shared object file: No such file or directory`. You may have to specify the path to the HDF5 installation manually, i.e., `HDF5_DIR=/path/to/hdf5/lib` (see [here](https://docs.h5py.org/en/stable/build.html#building-against-parallel-hdf5) for more details).
 
 For our COSMA7 setup, that would be:
 
-`HDF5DIR="/cosma/local/parallel-hdf5//gnu_11.1.0_ompi_4.1.4/1.12.0/"`
+`HDF5_DIR="/cosma/local/parallel-hdf5//gnu_11.1.0_ompi_4.1.4/1.12.0/"`
 
 ## Usage
 
 ``pyread_swift`` is build around a primary read wrapper, called ``SwiftSnapshot``. The snapshot particles are loaded into, stored, and manipulated by this object.
 
-Reading follows the same four steps (see also the examples below):
+Reading follows these four steps (see also the examples below):
 
 * Initialize a ``SwiftSnapshot`` object pointing to the location of the HDF5 file.
 
 * Select the spatial region you want to extract the particles from using the ``select_region()`` routine.
 
 * Split the selection over the MPI ranks using the ``split_selection()`` routine.
```

### Comparing `pyread_swift-1.0.0/README.md` & `pyread_swift-1.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,83 @@
 ## An MPI read routine for Swift simulation snapshots
 
 ``pyread_swift`` is an MPI read routine for [``swiftsim``](https://github.com/SWIFTSIM/swiftsim) snapshots, very similar in style to John Helly's [``read_eagle``](https://gitlab.cosma.dur.ac.uk/jch/Read_Eagle) code to read EAGLE snapshots.
 
 The package can read ``swiftsim`` snapshots both in "collective" (i.e., multiple MPI ranks read from a single file simultaneously) and "distributed" (i.e., each MPI reads an individual snapshot file part in isolation) modes. 
 
-Can also read in pure serial, if no MPI libraries are installed.
-
 ## Installation
 
 ### Requirements
 
 * `OpenMPI` or other MPI library
 * `python>=3.8`
 
 Recommended modules when working on COSMA7:
 
-* `module load gnu_comp/11.1.0 openmpi/4.1.4 parallel_hdf5/1.12.0 python/3.9.1-C7`
-
-### Installation from source
+```bash
+module load gnu_comp/11.1.0 openmpi/4.1.4 parallel_hdf5/1.12.0 python/3.9.1-C7
+```
 
 Given the need for a parallel HDF5 installation, it is recommended you install ``pyread_swift`` within a virtual/conda environment. However you can ofcourse also install directly into your base Python environment if you prefer.
 
 First make sure your `pip` is up-to-date:
 
-* `python3 -m pip install --upgrade pip`
+```bash
+python3 -m pip install --upgrade pip
+```
+
+### Method 1) Installation from PyPi
+
+The easiest method is to install from [``PyPI``](https://pypi.org/project/pyread-swift/)
+
+```bash
+python3 -m pip install pyread-swift
+```
 
-Then you can install the `pyread_swift` package by typing the following in
+### Method 2) Installation from source
+
+Or, you can install directly from source.
+
+First clone the repo, then you can install the `pyread_swift` package by typing the following in
 the root git directory: 
 
-* `python3 -m pip install .[mpi]`
+```bash
+git clone https://github.com/stuartmcalpine/pyread_swift.git
+cd pyread_swift
+python3 -m pip install .
+```
 
-which will install `pyread_swift` and any dependencies (omit ``[mpi]`` for pure serial version).
+which will install `pyread_swift` and any dependencies.
 
 ### MPI installation for collective reading
 
 If you are using `pyread_swift` to load large snapshots over MPI collectively
 (i.e., multiple cores read in parallel from the same file), a bit of additional
 setup is required.
 
 Make sure you have `hdf5` installed with **parallel** compatibility ([see here for details](https://docs.h5py.org/en/stable/mpi.html)).
 
-Then, uninstall any installed versions of `mpi4py` and `h5py`:
-
-* `python3 -m pip uninstall mpi4py h5py`
-
-and reinstall then from source, with MPI flags:
-
-* `MPICC=mpicc CC=mpicc HDF5_MPI="ON" python3 -m pip install --no-binary=mpi4py mpi4py`
+Then, uninstall any versions of `h5py` and reinstall from source:
 
-* `MPICC=mpicc CC=mpicc HDF5_MPI="ON" python3 -m pip install --no-binary=h5py h5py`
+```bash
+python3 -m pip uninstall h5py
+MPICC=mpicc CC=mpicc HDF5_MPI="ON" python3 -m pip install --no-binary=h5py h5py
+```
 
 If `pip` struggles to find your `HDF5` libraries automatically, e.g., `error: libhdf5.so: cannot open shared object file: No such file or directory`. You may have to specify the path to the HDF5 installation manually, i.e., `HDF5_DIR=/path/to/hdf5/lib` (see [here](https://docs.h5py.org/en/stable/build.html#building-against-parallel-hdf5) for more details).
 
 For our COSMA7 setup, that would be:
 
-`HDF5DIR="/cosma/local/parallel-hdf5//gnu_11.1.0_ompi_4.1.4/1.12.0/"`
+`HDF5_DIR="/cosma/local/parallel-hdf5//gnu_11.1.0_ompi_4.1.4/1.12.0/"`
 
 ## Usage
 
 ``pyread_swift`` is build around a primary read wrapper, called ``SwiftSnapshot``. The snapshot particles are loaded into, stored, and manipulated by this object.
 
-Reading follows the same four steps (see also the examples below):
+Reading follows these four steps (see also the examples below):
 
 * Initialize a ``SwiftSnapshot`` object pointing to the location of the HDF5 file.
 
 * Select the spatial region you want to extract the particles from using the ``select_region()`` routine.
 
 * Split the selection over the MPI ranks using the ``split_selection()`` routine.
```

### Comparing `pyread_swift-1.0.0/pyproject.toml` & `pyread_swift-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyread_swift"
-version = "1.0.0"
+version = "1.0.3"
 description = "Package to read SWIFT simulation snapshots in MPI."
 readme = "README.md"
 authors = [{ name = "Stuart McAlpine", email = "stuart.mcalpine@fysik.su.se" }]
 license = { file = "LICENCE" }
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
```

### Comparing `pyread_swift-1.0.0/src/pyread_swift/io.py` & `pyread_swift-1.0.3/src/pyread_swift/io.py`

 * *Files identical despite different names*

### Comparing `pyread_swift-1.0.0/src/pyread_swift/read_dataset.py` & `pyread_swift-1.0.3/src/pyread_swift/read_dataset.py`

 * *Files identical despite different names*

### Comparing `pyread_swift-1.0.0/src/pyread_swift/read_header.py` & `pyread_swift-1.0.3/src/pyread_swift/read_header.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,18 +29,34 @@
             # Load attributes from groups.
             for grp in ["Header", "Cosmology", "Parameters", "RuntimePars"]:
                 if grp not in f:
                     continue
 
                 # Loop over each attribute in the group.
                 for att in f[grp].attrs.keys():
+
+                    # Extract the attribute
+                    tmp = f[grp].attrs.get(att)
+
+                    # Reduce size 1 arrays to a scalar quantity
+                    if type(tmp) == np.ndarray and tmp.size == 1:
+                        tmp = tmp[0]
+
+                    # Check for duplicates
                     if att in header.keys():
-                        print(f"*WARNING* Duplicate header attribute {att}..")
-                        continue
-                    header[att] = f[grp].attrs.get(att)
+                        if not np.isclose(tmp, header[att], atol=1.0e6):
+                            print(
+                                f"*WARNING* Duplicate header attribute {att}",
+                                "with bad match to one another..",
+                            )
+                            continue
+
+                    # Store the attribute.
+                    header[att] = tmp
+
     else:
         header = None
     if params.comm_size > 1:
         header = params.comm.bcast(header)
 
     # Check we have the minimum values.
     _required = ["NumFilesPerSnapshot", "NumPart_ThisFile", "NumPart_Total", "BoxSize"]
@@ -57,10 +73,11 @@
                 header["NumPart_Total_HighWord"][i] * 2**32
             )
             header["NumPart_Total_HighWord"][i] = 0
 
     # Assume boxsize is equal in all dimensions.
     if type(header["BoxSize"]) == list or type(header["BoxSize"]) == np.ndarray:
         if len(header["BoxSize"]) >= 1:
+            header["BoxSize_3D"] = header["BoxSize"]
             header["BoxSize"] = float(header["BoxSize"][0])
 
     return header
```

### Comparing `pyread_swift-1.0.0/src/pyread_swift/select_region.py` & `pyread_swift-1.0.3/src/pyread_swift/select_region.py`

 * *Files identical despite different names*

### Comparing `pyread_swift-1.0.0/src/pyread_swift/split_selection.py` & `pyread_swift-1.0.3/src/pyread_swift/split_selection.py`

 * *Files identical despite different names*

### Comparing `pyread_swift-1.0.0/src/pyread_swift.egg-info/PKG-INFO` & `pyread_swift-1.0.3/src/pyread_swift.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyread-swift
-Version: 1.0.0
+Version: 1.0.3
 Summary: Package to read SWIFT simulation snapshots in MPI.
 Author-email: Stuart McAlpine <stuart.mcalpine@fysik.su.se>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, LSST Dark Energy Science Collaboration (DESC)
         All rights reserved.
         
@@ -44,71 +44,84 @@
 
 ## An MPI read routine for Swift simulation snapshots
 
 ``pyread_swift`` is an MPI read routine for [``swiftsim``](https://github.com/SWIFTSIM/swiftsim) snapshots, very similar in style to John Helly's [``read_eagle``](https://gitlab.cosma.dur.ac.uk/jch/Read_Eagle) code to read EAGLE snapshots.
 
 The package can read ``swiftsim`` snapshots both in "collective" (i.e., multiple MPI ranks read from a single file simultaneously) and "distributed" (i.e., each MPI reads an individual snapshot file part in isolation) modes. 
 
-Can also read in pure serial, if no MPI libraries are installed.
-
 ## Installation
 
 ### Requirements
 
 * `OpenMPI` or other MPI library
 * `python>=3.8`
 
 Recommended modules when working on COSMA7:
 
-* `module load gnu_comp/11.1.0 openmpi/4.1.4 parallel_hdf5/1.12.0 python/3.9.1-C7`
-
-### Installation from source
+```bash
+module load gnu_comp/11.1.0 openmpi/4.1.4 parallel_hdf5/1.12.0 python/3.9.1-C7
+```
 
 Given the need for a parallel HDF5 installation, it is recommended you install ``pyread_swift`` within a virtual/conda environment. However you can ofcourse also install directly into your base Python environment if you prefer.
 
 First make sure your `pip` is up-to-date:
 
-* `python3 -m pip install --upgrade pip`
+```bash
+python3 -m pip install --upgrade pip
+```
+
+### Method 1) Installation from PyPi
+
+The easiest method is to install from [``PyPI``](https://pypi.org/project/pyread-swift/)
+
+```bash
+python3 -m pip install pyread-swift
+```
 
-Then you can install the `pyread_swift` package by typing the following in
+### Method 2) Installation from source
+
+Or, you can install directly from source.
+
+First clone the repo, then you can install the `pyread_swift` package by typing the following in
 the root git directory: 
 
-* `python3 -m pip install .[mpi]`
+```bash
+git clone https://github.com/stuartmcalpine/pyread_swift.git
+cd pyread_swift
+python3 -m pip install .
+```
 
-which will install `pyread_swift` and any dependencies (omit ``[mpi]`` for pure serial version).
+which will install `pyread_swift` and any dependencies.
 
 ### MPI installation for collective reading
 
 If you are using `pyread_swift` to load large snapshots over MPI collectively
 (i.e., multiple cores read in parallel from the same file), a bit of additional
 setup is required.
 
 Make sure you have `hdf5` installed with **parallel** compatibility ([see here for details](https://docs.h5py.org/en/stable/mpi.html)).
 
-Then, uninstall any installed versions of `mpi4py` and `h5py`:
-
-* `python3 -m pip uninstall mpi4py h5py`
-
-and reinstall then from source, with MPI flags:
-
-* `MPICC=mpicc CC=mpicc HDF5_MPI="ON" python3 -m pip install --no-binary=mpi4py mpi4py`
+Then, uninstall any versions of `h5py` and reinstall from source:
 
-* `MPICC=mpicc CC=mpicc HDF5_MPI="ON" python3 -m pip install --no-binary=h5py h5py`
+```bash
+python3 -m pip uninstall h5py
+MPICC=mpicc CC=mpicc HDF5_MPI="ON" python3 -m pip install --no-binary=h5py h5py
+```
 
 If `pip` struggles to find your `HDF5` libraries automatically, e.g., `error: libhdf5.so: cannot open shared object file: No such file or directory`. You may have to specify the path to the HDF5 installation manually, i.e., `HDF5_DIR=/path/to/hdf5/lib` (see [here](https://docs.h5py.org/en/stable/build.html#building-against-parallel-hdf5) for more details).
 
 For our COSMA7 setup, that would be:
 
-`HDF5DIR="/cosma/local/parallel-hdf5//gnu_11.1.0_ompi_4.1.4/1.12.0/"`
+`HDF5_DIR="/cosma/local/parallel-hdf5//gnu_11.1.0_ompi_4.1.4/1.12.0/"`
 
 ## Usage
 
 ``pyread_swift`` is build around a primary read wrapper, called ``SwiftSnapshot``. The snapshot particles are loaded into, stored, and manipulated by this object.
 
-Reading follows the same four steps (see also the examples below):
+Reading follows these four steps (see also the examples below):
 
 * Initialize a ``SwiftSnapshot`` object pointing to the location of the HDF5 file.
 
 * Select the spatial region you want to extract the particles from using the ``select_region()`` routine.
 
 * Split the selection over the MPI ranks using the ``split_selection()`` routine.
```

