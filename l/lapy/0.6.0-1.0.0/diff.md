# Comparing `tmp/lapy-0.6.0.tar.gz` & `tmp/lapy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lapy-0.6.0.tar", last modified: Wed May 17 15:43:27 2023, max compression
+gzip compressed data, was "lapy-1.0.0.tar", last modified: Thu Jun 15 15:36:18 2023, max compression
```

## Comparing `lapy-0.6.0.tar` & `lapy-1.0.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:43:27.714751 lapy-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-17 15:42:50.000000 lapy-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-05-17 15:43:27.714751 lapy-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-17 15:42:50.000000 lapy-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:43:27.710751 lapy-0.6.0/lapy/
--rw-r--r--   0 runner    (1001) docker     (123)    19846 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/Conformal.py
--rw-r--r--   0 runner    (1001) docker     (123)    24972 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/DiffGeo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/FuncIO.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/Heat.py
--rw-r--r--   0 runner    (1001) docker     (123)    20770 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/Plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/ShapeDNA.py
--rw-r--r--   0 runner    (1001) docker     (123)    30698 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/Solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/TetIO.py
--rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/TetMesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/TriaIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    42560 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/TriaMesh.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:43:27.710751 lapy-0.6.0/lapy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/commands/sys_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/read_geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:43:27.714751 lapy-0.6.0/lapy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/utils/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/utils/_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:43:27.710751 lapy-0.6.0/lapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-05-17 15:43:27.000000 lapy-0.6.0/lapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-17 15:43:27.000000 lapy-0.6.0/lapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:43:27.000000 lapy-0.6.0/lapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-17 15:43:27.000000 lapy-0.6.0/lapy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-17 15:43:27.000000 lapy-0.6.0/lapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 15:43:27.000000 lapy-0.6.0/lapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-17 15:42:50.000000 lapy-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 15:43:27.714751 lapy-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 15:42:50.000000 lapy-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:36:18.305629 lapy-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-15 15:35:41.000000 lapy-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-06-15 15:36:18.305629 lapy-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-15 15:35:41.000000 lapy-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:36:18.305629 lapy-1.0.0/lapy/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-15 15:35:41.000000 lapy-1.0.0/lapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-06-15 15:35:41.000000 lapy-1.0.0/lapy/_read_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-06-15 15:35:41.000000 lapy-1.0.0/lapy/_tet_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16518 2023-06-15 15:35:41.000000 lapy-1.0.0/lapy/_tria_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 15:35:41.000000 lapy-1.0.0/lapy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:36:18.305629 lapy-1.0.0/lapy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:35:41.000000 lapy-1.0.0/lapy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-15 15:35:41.000000 lapy-1.0.0/lapy/commands/sys_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16378 2023-06-15 15:35:41.000000 lapy-1.0.0/lapy/conformal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24995 2023-06-15 15:35:41.000000 lapy-1.0.0/lapy/diffgeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-15 15:35:41.000000 lapy-1.0.0/lapy/heat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-15 15:35:41.000000 lapy-1.0.0/lapy/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20764 2023-06-15 15:35:41.000000 lapy-1.0.0/lapy/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-06-15 15:35:41.000000 lapy-1.0.0/lapy/shapedna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30701 2023-06-15 15:35:41.000000 lapy-1.0.0/lapy/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-06-15 15:35:41.000000 lapy-1.0.0/lapy/tet_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40528 2023-06-15 15:35:41.000000 lapy-1.0.0/lapy/tria_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:36:18.305629 lapy-1.0.0/lapy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-15 15:35:41.000000 lapy-1.0.0/lapy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-15 15:35:41.000000 lapy-1.0.0/lapy/utils/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-15 15:35:41.000000 lapy-1.0.0/lapy/utils/_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:36:18.305629 lapy-1.0.0/lapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-06-15 15:36:18.000000 lapy-1.0.0/lapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-15 15:36:18.000000 lapy-1.0.0/lapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:36:18.000000 lapy-1.0.0/lapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 15:36:18.000000 lapy-1.0.0/lapy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-15 15:36:18.000000 lapy-1.0.0/lapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 15:36:18.000000 lapy-1.0.0/lapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-15 15:35:41.000000 lapy-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 15:36:18.305629 lapy-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 15:35:41.000000 lapy-1.0.0/setup.py
```

### Comparing `lapy-0.6.0/LICENSE` & `lapy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lapy-0.6.0/PKG-INFO` & `lapy-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lapy
-Version: 0.6.0
+Version: 1.0.0
 Summary: A package for differential geometry on meshes (Laplace, FEM)
 Author-email: Martin Reuter <martin.reuter@dzne.de>
 Maintainer-email: Martin Reuter <martin.reuter@dzne.de>
 License: MIT License
         
         Copyright (c) 2020 Deep Medical Imaging Lab (PI Reuter)
         
@@ -22,16 +22,16 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: homepage, https://github.com/Deep-MI/LaPy
-Project-URL: documentation, https://github.com/Deep-MI/LaPy
+Project-URL: homepage, https://Deep-MI.github.io/LaPy/dev/index.html
+Project-URL: documentation, https://Deep-MI.github.io/LaPy/dev/index.html
 Project-URL: source, https://github.com/Deep-MI/LaPy
 Project-URL: tracker, https://github.com/Deep-MI/LaPy/issues
 Keywords: python,Laplace,FEM,ShapeDNA,BrainPrint,Triangle Mesh,Tetrahedra Mesh,Geodesics in Heat,Mean Curvature Flow
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -42,42 +42,47 @@
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: chol
+Provides-Extra: doc
 Provides-Extra: style
 Provides-Extra: test
 Provides-Extra: all
 Provides-Extra: full
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/lapy.svg)](https://pypi.org/project/lapy/)
 # LaPy
 
-LaPy is a package to compute spectral features (Laplace-Beltrami operator) on
-tetrahedral and triangle meshes. It is written purely in python 3 without
-sacrificing speed as almost all loops are vectorized, drawing upon efficient
-and sparse mesh data structures. It is basically a port of the C++ ShapeDNA
-project with extended differential geometry capabilities.
+LaPy is an open-source Python package for differential geometry on triangle
+and tetrahedra meshes. It includes an FEM solver to estimate the Laplace,
+Poisson or Heat equations. Further functionality includes the computations
+of gradients, divergence, mean-curvature flow, conformal mappings, 
+geodesics, ShapeDNA (Laplace spectra), and IO and plotting methods. 
+
+LaPy is written purely in Python 3 without sacrificing speed as almost all
+loops are vectorized, drawing upon efficient and sparse mesh data structures.
 
 ## Contents:
 
-- TriaMesh: a class for triangle meshes offering various operations, such as
+- **TriaMesh**: a class for triangle meshes offering various operations, such as
   fixing orientation, smoothing, curvature, boundary, quality, normals, and
-  various efficient mesh datastructure (edges, adjacency matrices)
-- TetMesh: a class for tetrahedral meshes (orientation, boundary ...)
-- TriaIO, TetIO: for both tets and trias from off, vtk, etc. formats
-- FuncIO: import/export vertex functions and eigenvector files
-- Solver: a class for linear FEM computation (Laplace stiffness and mass
+  various efficient mesh datastructures (edges, adjacency matrices). IO from
+  OFF, VTK and other formats.
+- **TetMesh**: a class for tetrahedral meshes (orientation, boundary, IO ...)
+- **Solver**: a class for linear FEM computation (Laplace stiffness and mass
   matrix, fast and sparse eigenvalue solver, anisotropic Laplace, Poisson)
-- DiffGeo: compute gradients, divergence, mean curvature flow, etc.
-- Heat: for heat kernel and diffusion
-- ShapeDNA: compute the ShapeDNA descriptor of surfaces and solids
-- Plot: functions for interactive visualization (wrapping plotly)
+- **io**: module for IO of vertex functions and eigenvector files
+- **diffgeo**: module for gradients, divergence, mean curvature flow, etc.
+- **heat**: module for heat kernel and diffusion
+- **shapedna**: module for the ShapeDNA descriptor of surfaces and solids
+- **plot**: module for interactive visualizations (wrapping plotly)
 
 ## Usage:
 
 The LaPy package is a comprehensive collection of scripts, so we refer to the
 'help' function and docstring of each module / function / class for usage info.
 For example:
 
@@ -88,43 +93,47 @@
 ```
 
 In the `examples` subdirectory, we provide several Jupyter notebooks that
 illustrate prototypical use cases of the toolbox.
 
 ## Installation:
 
-Use the following code to download, build and install a package from this
-repository into your local Python package directory:
+Use the following code to install the latest release of LaPy into your local
+Python package directory:
 
 `python3 -m pip install lapy`
 
 Use the following code to install the dev package in editable mode to a location of
 your choice:
 
 `python3 -m pip install --user --src /my/preferred/location --editable git+https://github.com/Deep-MI/Lapy.git#egg=lapy`
 
-Several functions, e.g. the Solver, require a sparse matrix decomposition, for which either the LU decomposition (from scipy sparse) or the faster Cholesky decomposition (from scikit-sparse cholmod) can be used. The default is to use the LU decomposition. If the parameter flag use_cholmod is True, the code will try to import cholmod from the scikit-sparse package. If this fails, an error will be thrown. If you would like to use cholmod, you need to install scikit-sparse separately. It cannot be listed among LaPy's dependencies as that causes errors with pip. scikit-sparse requires numpy and scipy to be installed separately beforehand.
+Several functions, e.g. the Solver, require a sparse matrix decomposition, for which either the LU decomposition (from scipy sparse, default) or the faster Cholesky decomposition (from scikit-sparse cholmod, recommended) can be used. If the parameter flag use_cholmod is True, the code will try to import cholmod from the scikit-sparse package. If this fails, an error will be thrown. If you would like to use cholmod, you need to install scikit-sparse separately, as pip currently cannot install it (conda can). scikit-sparse requires numpy and scipy to be installed separately beforehand.
+
+## API Documentation
+
+The API Documentation can be found at https://deep-mi.org/LaPy .
 
 ## References:
 
 If you use this software for a publication please cite both these papers:
 
-[1] Laplace-Beltrami spectra as 'Shape-DNA' of surfaces and solids. Reuter M, Wolter F-E, Peinecke N. Computer-Aided Design. 2006;38(4):342-366. http://dx.doi.org/10.1016/j.cad.2005.10.011
+**[1]** Laplace-Beltrami spectra as 'Shape-DNA' of surfaces and solids. Reuter M, Wolter F-E, Peinecke N. Computer-Aided Design. 2006;38(4):342-366. http://dx.doi.org/10.1016/j.cad.2005.10.011
 
-[2] BrainPrint: a discriminative characterization of brain morphology. Wachinger C, Golland P, Kremen W, Fischl B, Reuter M. Neuroimage. 2015;109:232-48. http://dx.doi.org/10.1016/j.neuroimage.2015.01.032 http://www.ncbi.nlm.nih.gov/pubmed/25613439
+**[2]** BrainPrint: a discriminative characterization of brain morphology. Wachinger C, Golland P, Kremen W, Fischl B, Reuter M. Neuroimage. 2015;109:232-48. http://dx.doi.org/10.1016/j.neuroimage.2015.01.032 http://www.ncbi.nlm.nih.gov/pubmed/25613439
 
-[1] introduces the FEM methods and the Laplace spectra for shape analysis, while [2] focusses on medical applications.
+Shape-DNA [1] introduces the FEM methods and the Laplace spectra for shape analysis, while BrainPrint [2] focusses on medical applications.
 
-For Geodesics please cite:
+For Geodesics please also cite:
 
 [3] Crane K, Weischedel C, Wardetzky M. Geodesics in heat: A new approach to computing distance based on heat flow. ACM Transactions on Graphics. https://doi.org/10.1145/2516971.2516977
 
 For non-singular mean curvature flow please cite:
 
 [4] Kazhdan M, Solomon J, Ben-Chen M. 2012. Can Mean-Curvature Flow be Modified to be Non-singular? Comput. Graph. Forum 31, 5, 1745–1754.
 https://doi.org/10.1111/j.1467-8659.2012.03179.x
 
 For conformal mapping please cite:
 
 [5] Choi PT, Lam KC, Lui LM. FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization for Genus-0 Closed Brain Surfaces. SIAM Journal on Imaging Sciences, vol. 8, no. 1, pp. 67-94, 2015. https://doi.org/10.1137/130950008
 
-We also invite you to check out our lab webpage at https://deep-mi.org
+We invite you to check out our lab webpage at https://deep-mi.org
```

### Comparing `lapy-0.6.0/README.md` & `lapy-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,33 @@
+[![PyPI version](https://badge.fury.io/py/lapy.svg)](https://pypi.org/project/lapy/)
 # LaPy
 
-LaPy is a package to compute spectral features (Laplace-Beltrami operator) on
-tetrahedral and triangle meshes. It is written purely in python 3 without
-sacrificing speed as almost all loops are vectorized, drawing upon efficient
-and sparse mesh data structures. It is basically a port of the C++ ShapeDNA
-project with extended differential geometry capabilities.
+LaPy is an open-source Python package for differential geometry on triangle
+and tetrahedra meshes. It includes an FEM solver to estimate the Laplace,
+Poisson or Heat equations. Further functionality includes the computations
+of gradients, divergence, mean-curvature flow, conformal mappings, 
+geodesics, ShapeDNA (Laplace spectra), and IO and plotting methods. 
+
+LaPy is written purely in Python 3 without sacrificing speed as almost all
+loops are vectorized, drawing upon efficient and sparse mesh data structures.
 
 ## Contents:
 
-- TriaMesh: a class for triangle meshes offering various operations, such as
+- **TriaMesh**: a class for triangle meshes offering various operations, such as
   fixing orientation, smoothing, curvature, boundary, quality, normals, and
-  various efficient mesh datastructure (edges, adjacency matrices)
-- TetMesh: a class for tetrahedral meshes (orientation, boundary ...)
-- TriaIO, TetIO: for both tets and trias from off, vtk, etc. formats
-- FuncIO: import/export vertex functions and eigenvector files
-- Solver: a class for linear FEM computation (Laplace stiffness and mass
+  various efficient mesh datastructures (edges, adjacency matrices). IO from
+  OFF, VTK and other formats.
+- **TetMesh**: a class for tetrahedral meshes (orientation, boundary, IO ...)
+- **Solver**: a class for linear FEM computation (Laplace stiffness and mass
   matrix, fast and sparse eigenvalue solver, anisotropic Laplace, Poisson)
-- DiffGeo: compute gradients, divergence, mean curvature flow, etc.
-- Heat: for heat kernel and diffusion
-- ShapeDNA: compute the ShapeDNA descriptor of surfaces and solids
-- Plot: functions for interactive visualization (wrapping plotly)
+- **io**: module for IO of vertex functions and eigenvector files
+- **diffgeo**: module for gradients, divergence, mean curvature flow, etc.
+- **heat**: module for heat kernel and diffusion
+- **shapedna**: module for the ShapeDNA descriptor of surfaces and solids
+- **plot**: module for interactive visualizations (wrapping plotly)
 
 ## Usage:
 
 The LaPy package is a comprehensive collection of scripts, so we refer to the
 'help' function and docstring of each module / function / class for usage info.
 For example:
 
@@ -34,43 +38,47 @@
 ```
 
 In the `examples` subdirectory, we provide several Jupyter notebooks that
 illustrate prototypical use cases of the toolbox.
 
 ## Installation:
 
-Use the following code to download, build and install a package from this
-repository into your local Python package directory:
+Use the following code to install the latest release of LaPy into your local
+Python package directory:
 
 `python3 -m pip install lapy`
 
 Use the following code to install the dev package in editable mode to a location of
 your choice:
 
 `python3 -m pip install --user --src /my/preferred/location --editable git+https://github.com/Deep-MI/Lapy.git#egg=lapy`
 
-Several functions, e.g. the Solver, require a sparse matrix decomposition, for which either the LU decomposition (from scipy sparse) or the faster Cholesky decomposition (from scikit-sparse cholmod) can be used. The default is to use the LU decomposition. If the parameter flag use_cholmod is True, the code will try to import cholmod from the scikit-sparse package. If this fails, an error will be thrown. If you would like to use cholmod, you need to install scikit-sparse separately. It cannot be listed among LaPy's dependencies as that causes errors with pip. scikit-sparse requires numpy and scipy to be installed separately beforehand.
+Several functions, e.g. the Solver, require a sparse matrix decomposition, for which either the LU decomposition (from scipy sparse, default) or the faster Cholesky decomposition (from scikit-sparse cholmod, recommended) can be used. If the parameter flag use_cholmod is True, the code will try to import cholmod from the scikit-sparse package. If this fails, an error will be thrown. If you would like to use cholmod, you need to install scikit-sparse separately, as pip currently cannot install it (conda can). scikit-sparse requires numpy and scipy to be installed separately beforehand.
+
+## API Documentation
+
+The API Documentation can be found at https://deep-mi.org/LaPy .
 
 ## References:
 
 If you use this software for a publication please cite both these papers:
 
-[1] Laplace-Beltrami spectra as 'Shape-DNA' of surfaces and solids. Reuter M, Wolter F-E, Peinecke N. Computer-Aided Design. 2006;38(4):342-366. http://dx.doi.org/10.1016/j.cad.2005.10.011
+**[1]** Laplace-Beltrami spectra as 'Shape-DNA' of surfaces and solids. Reuter M, Wolter F-E, Peinecke N. Computer-Aided Design. 2006;38(4):342-366. http://dx.doi.org/10.1016/j.cad.2005.10.011
 
-[2] BrainPrint: a discriminative characterization of brain morphology. Wachinger C, Golland P, Kremen W, Fischl B, Reuter M. Neuroimage. 2015;109:232-48. http://dx.doi.org/10.1016/j.neuroimage.2015.01.032 http://www.ncbi.nlm.nih.gov/pubmed/25613439
+**[2]** BrainPrint: a discriminative characterization of brain morphology. Wachinger C, Golland P, Kremen W, Fischl B, Reuter M. Neuroimage. 2015;109:232-48. http://dx.doi.org/10.1016/j.neuroimage.2015.01.032 http://www.ncbi.nlm.nih.gov/pubmed/25613439
 
-[1] introduces the FEM methods and the Laplace spectra for shape analysis, while [2] focusses on medical applications.
+Shape-DNA [1] introduces the FEM methods and the Laplace spectra for shape analysis, while BrainPrint [2] focusses on medical applications.
 
-For Geodesics please cite:
+For Geodesics please also cite:
 
 [3] Crane K, Weischedel C, Wardetzky M. Geodesics in heat: A new approach to computing distance based on heat flow. ACM Transactions on Graphics. https://doi.org/10.1145/2516971.2516977
 
 For non-singular mean curvature flow please cite:
 
 [4] Kazhdan M, Solomon J, Ben-Chen M. 2012. Can Mean-Curvature Flow be Modified to be Non-singular? Comput. Graph. Forum 31, 5, 1745–1754.
 https://doi.org/10.1111/j.1467-8659.2012.03179.x
 
 For conformal mapping please cite:
 
 [5] Choi PT, Lam KC, Lui LM. FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization for Genus-0 Closed Brain Surfaces. SIAM Journal on Imaging Sciences, vol. 8, no. 1, pp. 67-94, 2015. https://doi.org/10.1137/130950008
 
-We also invite you to check out our lab webpage at https://deep-mi.org
+We invite you to check out our lab webpage at https://deep-mi.org
```

### Comparing `lapy-0.6.0/lapy/Conformal.py` & `lapy-1.0.0/lapy/conformal.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,66 +1,53 @@
-# Adopted from Matlab code at
-# https://github.com/garyptchoi/spherical-conformal-map
-# with this
-# Copyright (c) 2013-2020, Gary Pui-Tung Choi
-# https://math.mit.edu/~ptchoi
-# and has been distributed with the Apache 2 License
-
-# If you use this code in your own work, please cite the following paper:
-# [1] P. T. Choi, K. C. Lam, and L. M. Lui,
-# "FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization for Genus-0
-#  Closed Brain Surfaces."
-# SIAM Journal on Imaging Sciences, vol. 8, no. 1, pp. 67-94, 2015.
+"""Computes spherical conformal mappings of triangle meshes.
 
+Functions are adopted from Matlab code at
+https://github.com/garyptchoi/spherical-conformal-map
+with this
+Copyright (c) 2013-2020, Gary Pui-Tung Choi
+https://math.mit.edu/~ptchoi
+and has been distributed with the Apache 2 License.
+
+Notes
+-----
+If you use this code in your own work, please cite the following paper:
+
+[1] P. T. Choi, K. C. Lam, and L. M. Lui,
+"FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization for Genus-0
+Closed Brain Surfaces."
+SIAM Journal on Imaging Sciences, vol. 8, no. 1, pp. 67-94, 2015.
+"""
 
 import importlib
 
 import numpy as np
 from scipy import sparse
 from scipy.optimize import minimize
 
-from .Solver import Solver
-from .TriaMesh import TriaMesh
+from . import Solver, TriaMesh
 from .utils._imports import import_optional_dependency
 
 
 def spherical_conformal_map(tria, use_cholmod=False):
-    """
-    A linear method for computing spherical conformal map of a genus-0 closed surface
+    """Linear method for computing spherical conformal map of a genus-0 closed surface.
 
     Parameters
     ----------
     tria : TriaMesh
-        vertices and faces
+        Triangle mesh.
     use_cholmod : bool, default=False
         Which solver to use:
-            * True : Use Cholesky decomposition from scikit-sparse cholmod
-            * False: Use spsolve (LU decomposition)        
+            * True : Use Cholesky decomposition from scikit-sparse cholmod.
+            * False: Use spsolve (LU decomposition).
 
     Returns
     -------
-    mapping: np.ndarray of shape (n,3)
-        vertex coordinates of the spherical conformal parameterization
-
-    Notes
-    -------
-    If you use this code in your own work, please cite the following paper:
-    [1] P. T. Choi, K. C. Lam, and L. M. Lui,
-       "FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization
-       for Genus-0 Closed Brain Surfaces."
-       SIAM Journal on Imaging Sciences, vol. 8, no. 1, pp. 67-94, 2015.
-
-    Adopted from Matlab code at
-    https://github.com/garyptchoi/spherical-conformal-map
-    with this
-    Copyright (c) 2013-2020, Gary Pui-Tung Choi
-    https://math.mit.edu/~ptchoi
-    and has been distributed with the Apache 2 License
+    mapping: array
+        Vertex coordinates (3d) of the spherical conformal parameterization.
     """
-
     # Check whether the input mesh is spherical topology (genus-0)
     if tria.euler() != 2:
         print("ERROR: The mesh is not a genus-0 closed surface ..")
         raise ValueError("not genus-0")
 
     # Find the most regular triangle as the "big triangle"
     tquals = tria.tria_qualities()
@@ -106,15 +93,15 @@
     c[p0], c[p1], c[p2] = x0, x1, x2
     d = np.zeros((nv, 1))
     d[p0], d[p1], d[p2] = y0, y1, y2
     rhs = np.empty(c.shape[:-1], dtype=complex)
     rhs.real = c.flatten()
     rhs.imag = d.flatten()
 
-    z = sparse_symmetric_solve(M, rhs, use_cholmod=use_cholmod)
+    z = _sparse_symmetric_solve(M, rhs, use_cholmod=use_cholmod)
     z = np.squeeze(np.array(z))
     z = z - np.mean(z, axis=0)
 
     # inverse stereographic projection (not scaled well)
     S = inverse_stereographic(z)
 
     # Find optimal big triangle size
@@ -169,69 +156,60 @@
     )
 
     # compute the Beltrami coefficient (value per triangle)
     triasouth = TriaMesh(P, tria.t)
     mu = beltrami_coefficient(triasouth, tria.v)
 
     # compose the map with another quasi-conformal map to cancel the distortion
-    mapping = linear_beltrami_solver(triasouth, mu, fixed, P[fixed, :], use_cholmod=use_cholmod)
+    mapping = linear_beltrami_solver(
+        triasouth, mu, fixed, P[fixed, :], use_cholmod=use_cholmod
+    )
 
     if np.isnan(np.sum(mapping)):
         # if the result has NaN entries, then most probably the number of
         # boundary constraints is not large enough
         # increase the number of boundary constrains and run again
         print("South pole compsed map has nan value(s)!")
         fixnum = fixnum * 5  # again, this number can be changed
         fixed = idx[0 : np.minimum(nv, fixnum)]
-        mapping = linear_beltrami_solver(triasouth, mu, fixed, P[fixed, :], use_cholmod=use_cholmod)
+        mapping = linear_beltrami_solver(
+            triasouth, mu, fixed, P[fixed, :], use_cholmod=use_cholmod
+        )
         if np.isnan(np.sum(mapping)):
             mapping = P  # use the old result
 
     # inverse south pole stereographic projection
     mapping = inverse_stereographic(mapping)
     return mapping
 
 
 def mobius_area_correction_spherical(tria, mapping):
-    """
-    Find an optimal Mobius transformation for reducing the area distortion
-    of a spherical conformal parameterization using the method in [1].
+    r"""Find an improved Mobius transformation to reduce distortion.
+
+    This helps reducing the area distortion of
+    a spherical conformal parameterization using the method in
+    Choi et al, SIAM Journal on Imaging Sciences, 2020.
 
     Parameters
-    -------
+    ----------
     tria : TriaMesh
-        (vertices, triangle) of genus-0 closed triangle mesh
-    mapping : np.ndarray of shape (n,3)
-        vertex coordinates of the spherical conformal parameterization
+        Genus-0 closed triangle mesh.
+    mapping : array
+        Vertex coordinates of the spherical conformal parameterization.
 
     Returns
     -------
-    map_mobius: np.ndarray of shape (n,3)
-        vertex coordinates of the updated spherical conformal parameterization
-    result: OptimizeResult
-        the optimal parameters (x) for the Mobius transformation, where
-            f(z) = \frac{az+b}{cz+d}
-                = ((x(1)+x(2)*1j)*z+(x(3)+x(4)*1j))/((x(5)+x(6)*1j)*z+(x(7)+x(8)*1j))
-
-    Notes
-    -------
-    If you use this code in your own work, please cite the following paper:
-    [1] G. P. T. Choi, Y. Leung-Liu, X. Gu, and L. M. Lui,
-        "Parallelizable global conformal parameterization
-        of simply-connected surfaces via partial welding."
-        SIAM Journal on Imaging Sciences, 2020.
-
-    Adopted by Martin Reuter from Matlab code at
-    https://github.com/garyptchoi/spherical-conformal-map
-    with this
-    Copyright (c) 2019-2020, Gary Pui-Tung Choi
-    https://scholar.harvard.edu/choi
-    and has been distributed with the Apache 2 License
-    """
-
+    map_mobius: array
+        Vertex coordinates (3d) of the updated spherical conformal parameterization.
+    result: array
+        Optimal parameters (x) for the Mobius transformation, where
+
+        .. math::
+            f(z) = \frac{az+b}{cz+d} = \frac{(x(1)+x(2)*1j)*z+(x(3)+x(4)*1j)}{(x(5)+x(6)*1j)*z+(x(7)+x(8)*1j)}.
+    """  # noqa: E501
     # Compute the tria areas with normalization
     area_t = tria.tria_areas()
     area_t = area_t / area_t.sum()
     # Project the sphere onto the plane
     z = stereographic(mapping)
 
     def area_map(xx):
@@ -271,45 +249,29 @@
         (x[4] + x[5] * 1j) * z + (x[6] + x[7] * 1j)
     )
     map_mobius = inverse_stereographic(fz)
     return map_mobius, result
 
 
 def beltrami_coefficient(tria, mapping):
-    """
-    Compute the Beltrami coefficient of a mapping.
+    """Compute the Beltrami coefficient of a mapping.
 
     Parameters
     ----------
     tria : TriaMesh
-        (vertices, triangle) of genus-0 closed triangle mesh
-        TriaMesh should be planar mapping on complex plane
-    mapping : np.ndarray of shape (n,3)
-        coordinates of the spherical conformal parameterization
+        Genus-0 closed triangle mesh.
+        Should be planar mapping on complex plane.
+    mapping : array
+        3D coordinates of the spherical conformal parameterization.
 
     Returns
     -------
-    mu: np.ndarray of complex beltrami coefficient per triangle
-
-    Notes
-    -------
-    If you use this code in your own work, please cite the following paper:
-    [1] P. T. Choi, K. C. Lam, and L. M. Lui,
-    "FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization
-    for Genus-0 Closed Brain Surfaces."
-    SIAM Journal on Imaging Sciences, vol. 8, no. 1, pp. 67-94, 2015.
-
-    Adopted by Martin Reuter from Matlab code at
-    https://github.com/garyptchoi/spherical-conformal-map
-    with this
-    Copyright (c) 2013-2020, Gary Pui-Tung Choi
-    https://math.mit.edu/~ptchoi
-    and has been distributed with the Apache 2 License
+    mu : array
+        Complex Beltrami coefficient per triangle.
     """
-
     # here we should be in the plane
     if np.amax(tria.v[:, 2]) - np.amin(tria.v[:, 2]) > 0.001:
         print("ERROR: mesh should be on complex plane ..")
         raise ValueError("not planar")
 
     # get 2d vetrices, edges and area
     v0 = (tria.v[tria.t[:, 0], :])[:, :-1]
@@ -348,52 +310,37 @@
     F = dXdu * dXdv + dYdu * dYdv + dZdu * dZdv
     mu = (E - G + 2j * F) / (E + G + 2.0 * np.sqrt(E * G - F**2))
 
     return mu
 
 
 def linear_beltrami_solver(tria, mu, landmark, target, use_cholmod=False):
-    """
-    Linear Beltrami solver
+    """Linear Beltrami solver.
 
     Parameters
     ----------
     tria : TriaMesh
-        (vertices, triangle) of genus-0 closed triangle mesh
-        TriaMesh should be planar mapping on complex plane
-    mu : np.array of complex beltrami coefficients
-    landmark : np.ndarray of fixed vertex indices
-    target : np.ndarray of shape (n,3)
-        2D landmark target coordinates (third coordinate is zero)
+        Genus-0 closed triangle mesh.
+        Should be planar mapping on complex plane.
+    mu : array_like
+        Complex Beltrami coefficients.
+    landmark : array_like
+        Fixed vertex indices.
+    target : array
+        3d array with 2d landmark target coordinates (3rd coordinate is zero).
     use_cholmod : bool, default=False
         Which solver to use:
-            * True : Use Cholesky decomposition from scikit-sparse cholmod
-            * False: Use spsolve (LU decomposition)             
+            * True : Use Cholesky decomposition from scikit-sparse cholmod.
+            * False: Use spsolve (LU decomposition).
 
     Returns
     -------
-    mapping : np.ndarray of shape (n,3)
-        vertex coordinates of new mapping
-
-    Notes
-    ------
-    If you use this code in your own work, please cite the following paper:
-    [1] P. T. Choi, K. C. Lam, and L. M. Lui,
-    "FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization
-    for Genus-0 Closed Brain Surfaces."
-    SIAM Journal on Imaging Sciences, vol. 8, no. 1, pp. 67-94, 2015.
-
-    Adopted by Martin Reuter from Matlab code at
-    https://github.com/garyptchoi/spherical-conformal-map
-    with this
-    Copyright (c) 2013-2020, Gary Pui-Tung Choi
-    https://math.mit.edu/~ptchoi
-    and has been distributed with the Apache 2 License
+    mapping : array
+        3d vertex coordinates of new mapping.
     """
-
     # here we should be in the plane
     if np.amax(tria.v[:, 2]) - np.amin(tria.v[:, 2]) > 0.001:
         print("ERROR: mesh should be on complex plane ..")
         raise ValueError("not planar")
 
     af = (1.0 - 2 * np.real(mu) + np.abs(mu) ** 2) / (1.0 - np.abs(mu) ** 2)
     bf = -2.0 * np.imag(mu) / (1.0 - np.abs(mu) ** 2)
@@ -453,39 +400,40 @@
     Azero = sparse.csc_matrix((mval, (mrow, landmark[mcol])), shape=(nv, nv))
     Aones = sparse.csr_matrix(
         (np.ones(landmark.shape[0]), (landmark, landmark)), shape=(nv, nv)
     )
     A = A - Azero + Aones
     A.eliminate_zeros()
 
-    x = sparse_symmetric_solve(A, b, use_cholmod=use_cholmod)
+    x = _sparse_symmetric_solve(A, b, use_cholmod=use_cholmod)
 
     mapping = np.squeeze(np.array(x))
     mapping = np.column_stack((np.real(mapping), np.imag(mapping)))
     return mapping
 
 
-def sparse_symmetric_solve(A, b, use_cholmod=False):
-    """
-    A sparse symmetric solver for ``A x = b``
+def _sparse_symmetric_solve(A, b, use_cholmod=False):
+    """Sparse symmetric solver for ``A x = b``.
 
     Parameters
     ----------
-    A : sparse matrix of shape (n, n)
-    b : np.ndarray vector of length n
+    A : csc_matrix of shape (n, n)
+        Sparse symmetric matrix.
+    b : array of length n
+        Vector for right hand side of equation.
     use_cholmod : bool, default=False
         Which solver to use:
-            * True : Use Cholesky decomposition from scikit-sparse cholmod
-            * False: Use spsolve (LU decomposition)
+            * True : Use Cholesky decomposition from scikit-sparse cholmod.
+            * False: Use spsolve (LU decomposition).
 
     Returns
     -------
-    x: np.ndarray of length n, solution to  ``A x = b``
+    x: array of length n
+        Solution to  ``A x = b``.
     """
-
     if use_cholmod:
         sksparse = import_optional_dependency("sksparse", raise_error=True)
         importlib.import_module(".cholmod", sksparse.__name__)
     else:
         sksparse = None
     if use_cholmod:
         print("Solver: Cholesky decomposition from scikit-sparse cholmod ...")
@@ -497,83 +445,49 @@
         print("Solver: spsolve (LU decomposition) ...")
         lu = splu(A)
         x = lu.solve(b)
     return x
 
 
 def stereographic(u):
-    """
-    Map sphere to complex plane via stereographic projection
+    """Map sphere to complex plane via stereographic projection.
 
     Parameters
     ----------
-    u : np.ndarray of shape (n,3)
-        u represents the three vertex coordinates
+    u : array of shape (n, 3)
+        Represents the three vertex coordinates.
 
     Returns
     -------
-    v: np.ndarray of n complex numbers
-       stereographic map of u in complex plane
-
-    Notes
-    -------
-    If you use this code in your own work, please cite the following paper:
-    [1] P. T. Choi, K. C. Lam, and L. M. Lui,
-    "FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization
-     for Genus-0 Closed Brain Surfaces."
-    SIAM Journal on Imaging Sciences, vol. 8, no. 1, pp. 67-94, 2015.
-
-    Adopted by Martin Reuter from Matlab code at
-    https://github.com/garyptchoi/spherical-conformal-map
-    with this
-    Copyright (c) 2013-2020, Gary Pui-Tung Choi
-    https://math.mit.edu/~ptchoi
-    and has been distributed with the Apache 2 License
+    v: array of n complex numbers
+       Stereographic map of u in complex plane.
     """
-
     x = u[:, 0]
     y = u[:, 1]
     z = u[:, 2]
     v = np.empty(u.shape[:-1], dtype=complex)
     v.real = (x / (1 - z)).flatten()
     v.imag = (y / (1 - z)).flatten()
     return v
 
 
 def inverse_stereographic(u):
-    """
-    Map from complex plane to sphere via inverse stereographic projection
+    """Map from complex plane to sphere via inverse stereographic projection.
 
     Parameters
     ----------
-    u : np.ndarray
-        can be complex array, or two columns (real,img)
-        for coordinates on complex plane
+    u : array_like
+        Can be complex array, or two columns (real, img)
+        for coordinates on complex plane.
 
     Returns
     -------
-    v: np.ndarray of shape (n,3)
-        coordinates on sphere in 3D
-
-    Notes
-    -------
-    If you use this code in your own work, please cite the following paper:
-    [1] P. T. Choi, K. C. Lam, and L. M. Lui,
-    "FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization
-     for Genus-0 Closed Brain Surfaces."
-    SIAM Journal on Imaging Sciences, vol. 8, no. 1, pp. 67-94, 2015.
-
-    Adopted by Martin Reuter from Matlab code at
-    https://github.com/garyptchoi/spherical-conformal-map
-    with this
-    Copyright (c) 2013-2020, Gary Pui-Tung Choi
-    https://math.mit.edu/~ptchoi
-    and has been distributed with the Apache 2 License
+    v: array of shape (n, 3)
+        Coordinates on sphere in 3D.
     """
-
     if np.iscomplexobj(u):
         x = u.real
         y = u.imag
     else:
         x = u[:, 0]
         y = u[:, 1]
     z = 1 + x**2 + y**2
```

### Comparing `lapy-0.6.0/lapy/DiffGeo.py` & `lapy-1.0.0/lapy/diffgeo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,121 +1,126 @@
-import numpy as np
+"""Differential Geometry Functions for meshes.
+
+This module includes gradient, divergence, curvature, geodesics,
+mean curvature flow etc. 
+
+Note, the interface is not yet final, some functions are split into
+tet and tria versions.
+"""
+
 import importlib
+
+import numpy as np
 from scipy import sparse
 
-from .Solver import Solver
-from .TriaMesh import TriaMesh
+from . import Solver, TriaMesh
 from .utils._imports import import_optional_dependency
 
 
 def compute_gradient(geom, vfunc):
-    """
-    Computes gradient of a vertex function f
+    """Compute gradient of a vertex function f.
 
     Parameters
-    -------
+    ----------
     geom : TriaMesh or TetMesh
-        geometry vertices
-    vfunc : function
-        scalar function at vertices
+        Mesh geometry.
+    vfunc : array
+        Scalar function at vertices.
 
     Returns
     -------
-    tfunc : function
-        3d vector function of gradient
+    tfunc : array
+        3d gradient vector at each element.
 
     Raises
-    -------
-    ValueError: Unknown geometry type
+    ------
+    ValueError
+        If unknown geometry type.
     """
-
     if type(geom).__name__ == "TriaMesh":
         return tria_compute_gradient(geom, vfunc)
     elif type(geom).__name__ == "TetMesh":
         return tet_compute_gradient(geom, vfunc)
     else:
         raise ValueError('Geometry type "' + type(geom).__name__ + '" unknown')
 
 
 def compute_divergence(geom, vfunc):
-    """
-    Computes divergence of a vertex function f
+    """Compute divergence of a vertex function f.
 
     Parameters
     ----------
     geom : TriaMesh or TetMesh
-        geometry vertices
-    vfunc : function
-        scalar function at vertices
+        Mesh geometry.
+    vfunc : array
+        Scalar function at vertices.
 
     Returns
     -------
-    vfunc : function
-        scalar function of divergence
+    vfunc : array
+        Scalar function of divergence at vertices.
 
     Raises
-    -------
-    ValueError: unknown geometry type
+    ------
+    ValueError
+        If unknown geometry type.
     """
     if type(geom).__name__ == "TriaMesh":
         return tria_compute_divergence(geom, vfunc)
     elif type(geom).__name__ == "TetMesh":
         return tet_compute_divergence(geom, vfunc)
     else:
         raise ValueError('Geometry type "' + type(geom).__name__ + '" unknown')
 
 
 def compute_rotated_f(geom, vfunc):
-    """
-    Compute function whose level sets are orthgonal to the ones of vfunc
+    """Compute function whose level sets are orthgonal to the ones of vfunc.
 
     Parameters
     ----------
     geom : TriaMesh
-        geometry vertices
-    vfunc : function
-        scalar function at vertices
+        Mesh geometry.
+    vfunc : array
+        Scalar function at vertices.
 
     Returns
     -------
-    vfunc : function
-        rotated function
+    vfunc : array
+        Rotated function at vertices.
 
     Raises
-    -------
-    Value Error: Unknown geometry type
+    ------
+    ValueError
+        If unknown geometry type.
     """
-
     if type(geom).__name__ == "TriaMesh":
         return tria_compute_rotated_f(geom, vfunc)
     else:
         raise ValueError('Geometry type "' + type(geom).__name__ + '" not implemented')
 
 
 def compute_geodesic_f(geom, vfunc):
-    """
-    Computes function with normalized gradient (geodesic distance)
+    """Compute function with normalized gradient (geodesic distance).
 
     Computes gradient, normalizes it and computes function with this normalized
     gradient by solving the Poisson equation with the divergence of grad.
     This idea is also described in the paper "Geodesics in Heat" for triangles.
 
     Parameters
     ----------
     geom : TriaMesh, TetMesh
-        geometry vertices
-    vfunc : function
-        scalar function at vertices
+        Mesh geometry.
+    vfunc : array
+        Scalar function at vertices.
 
     Returns
     -------
-    vfunc : function
-        scalar geodesic function at vertices
+    vfunc : array
+        Scalar geodesic function at vertices.
     """
-
     gradf = compute_gradient(geom, vfunc)
     # normalize gradient
     gradnorm = gradf / np.sqrt((gradf**2).sum(1))[:, np.newaxis]
     gradnorm = np.nan_to_num(gradnorm)
     divf = compute_divergence(geom, gradnorm)
     fem = Solver(geom, lump=True)
     # as long as div does not care about weighing with a Bi,
@@ -123,34 +128,31 @@
     fem.mass = sparse.eye(fem.stiffness.shape[0], dtype=fem.stiffness.dtype)
     vf = fem.poisson(divf)
     vf -= min(vf)
     return vf
 
 
 def tria_compute_geodesic_f(tria, vfunc):
-    """
-    Computes function with normalized gradient (geodesic distance)
+    """Compute function with normalized gradient (geodesic distance).
 
     Computes gradient, normalizes it and computes function with this normalized
     gradient by solving the Poisson equation with the divergence of grad.
     This idea is also described in the paper "Geodesics in Heat".
 
     Parameters
     ----------
     tria : TriaMesh
-        geometry vertices
-            v           vertices
-            t           triangles
-    vfunc : function
-        scalar function at vertices
+        Triangle mesh.
+    vfunc : array
+        Scalar function at vertices.
 
     Returns
     -------
-    vfunc: function
-        scalar geodesic function at vertices
+    vfunc: array
+        Scalar geodesic function at vertices.
     """
     gradf = tria_compute_gradient(tria, vfunc)
     # normalize gradient
     gradnorm = gradf / np.sqrt((gradf**2).sum(1))[:, np.newaxis]
     gradnorm = np.nan_to_num(gradnorm)
     divf = tria_compute_divergence(tria, gradnorm)
     fem = Solver(tria)
@@ -161,44 +163,42 @@
     vf = fem.poisson(divf)
     vf -= min(vf)
     return vf
 
 
 # note , numexpr could speed up the following functions if necessary
 def tria_compute_gradient(tria, vfunc):
-    """
-    Computes gradient of a vertex function f (for each triangle)
+    r"""Compute gradient of a vertex function f (for each triangle).
+
+    .. math::
+        grad(f) &= [ (f_j - f_i) (vi-vk)' + (f_k - f_i) (vj-vi)' ] / (2 A) \\
+                &= [ f_i (vk-vj)' + f_j (vi-vk)' +  f_k (vj-vi)' ] / (2 A)
 
-    grad(f) = [ (f_j - f_i) (vi-vk)' + (f_k - f_i) (vj-vi)' ] / (2 A)
-            = [ f_i (vk-vj)' + f_j (vi-vk)' +  f_k (vj-vi)' ] / (2 A)
     for triangle (vi,vj,vk) with area A, where (.)' is 90 degrees rotated
     edge, which is equal to cross(n,vec).
 
     Parameters
     ----------
     tria : TriaMesh
-        geometry vertices
-            v           vertices
-            t           triangles
-    vfunc : function
-        scalar function at vertices
+        Triangle mesh.
+    vfunc : array
+        Scalar function at vertices.
 
     Returns
     -------
-    vfunc: function
-        3d vector function of gradient at triangles where
+    tfunc: array
+        3d gradient vector at triangles.
 
     Notes
-    -------
-    numexpr could speed up this functions if necessary
-
+    -----
+    Numexpr could speed up this functions if necessary.
     Good background to read:
     http://dgd.service.tu-berlin.de/wordpress/vismathws10/2012/10/17/gradient-of-scalar-functions/
     Mancinelli, Livesu, Puppo, Gradient Field Estimation on Triangle Meshes
-      http://pers.ge.imati.cnr.it/livesu/papers/MLP18/MLP18.pdf
+    http://pers.ge.imati.cnr.it/livesu/papers/MLP18/MLP18.pdf
     Desbrun ...
     """
     import sys
 
     v0 = tria.v[tria.t[:, 0], :]
     v1 = tria.v[tria.t[:, 1], :]
     v2 = tria.v[tria.t[:, 2], :]
@@ -217,41 +217,36 @@
     c2 = vfunc[tria.t[:, 2], np.newaxis] * e2
     # divided by 2 * area and rotate edge sum
     tfunc = lni * np.cross(n, (c0 + c1 + c2))
     return tfunc
 
 
 def tria_compute_divergence(tria, tfunc):
-    """
-    Computes integrated divergence of a 3d triangle function f (for each vertex)
+    """Compute integrated divergence of a 3d triangle function f (for each vertex).
 
     Divergence is the flux density leaving or entering a point.
-
     Note: this is the integrated divergence, you may want to multiply
     with B^-1 to get back the function in some applications
 
     Parameters
     ----------
     tria : TriaMesh
-        geometry vertices
-            v           vertices
-            t           triangles
-    tfunc : function
-        3d vector field on triangles
+        Triangle mesh.
+    tfunc : array
+        3d vector field on triangles.
 
     Returns
     -------
-    vfunc: function
-        scalar function of divergence at vertices
+    vfunc: array
+        Scalar function of divergence at vertices.
 
     Notes
-    -------
-    numexpr could speed up this functions if necessary
+    -----
+    Numexpr could speed up this functions if necessary.
     """
-
     import sys
 
     v0 = tria.v[tria.t[:, 0], :]
     v1 = tria.v[tria.t[:, 1], :]
     v2 = tria.v[tria.t[:, 2], :]
     e2 = v1 - v0
     e0 = v2 - v1
@@ -281,42 +276,38 @@
     vfunc = np.squeeze(
         np.asarray(0.5 * sparse.csc_matrix((dat, (i, j))).todense(), dtype=tfunc.dtype)
     )
     return vfunc
 
 
 def tria_compute_divergence2(tria, tfunc):
-    """
-    Computes integrated divergence of a 3d triangle function f (for each vertex)
+    """Compute integrated divergence of a 3d triangle function f (for each vertex).
 
     Divergence is the flux density leaving or entering a point.
     It can be measured by summing the dot product of the vector
     field with the normals to the outer edges of the 1-ring triangles
     around a vertex. Summing < tfunc , e_ij cross n >
-
     Note: this is the integrated divergence, you may want to multiply
     with B^-1 to get back the function in some applications
 
     Parameters
     ----------
     tria : TriaMesh
-        geometry vertices
-            v           vertices
-            t           triangles
-    tfunc : function
-        3d vector field on triangles
+        Triangle mesh.
+    tfunc : array
+        3d vector field on triangles.
 
     Returns
     -------
-    vfunc: function
-        scalar function of divergence at vertices
+    vfunc: array
+        Scalar function of divergence at vertices.
 
     Notes
-    -------
-    numexpr could speed up this functions if necessary
+    -----
+    Numexpr could speed-up this functions if necessary.
     """
     import sys
 
     v0 = tria.v[tria.t[:, 0], :]
     v1 = tria.v[tria.t[:, 1], :]
     v2 = tria.v[tria.t[:, 2], :]
     e2 = v1 - v0
@@ -338,39 +329,35 @@
     j = np.zeros((3 * len(tria.t), 1), dtype=int).reshape(-1)
     dat = np.column_stack((x0, x1, x2)).reshape(-1)
     vfunc = np.squeeze(np.asarray(0.5 * sparse.csc_matrix((dat, (i, j))).todense()))
     return vfunc
 
 
 def tria_compute_rotated_f(tria, vfunc):
-    """
-    Compute function whose level sets are orthgonal to the ones of vfunc.
+    """Compute function whose level sets are orthgonal to the ones of vfunc.
 
     This is done by rotating the gradient around the normal by 90 degrees,
     then solving the Poisson equations with the divergence of rotated grad.
 
     Parameters
     ----------
     tria : TriaMesh
-        geometry vertices
-            v           vertices
-            t           triangles
-    vfunc : function
-        scalar function at triangles
+        Triangle mesh.
+    vfunc : array
+        Scalar function at vertices.
 
     Returns
     -------
-    vfunc: function
-        rotated function
+    vfunc: array
+        Rotated scalar function at vertices.
 
     Notes
-    -------
-    numexpr could speed up this functions if necessary
+    -----
+    Numexpr could speed up this functions if necessary.
     """
-
     gradf = tria_compute_gradient(tria, vfunc)
     tn = tria.tria_normals()
     # lg = np.sqrt(np.sum(gradf * gradf, axis=1))
     # lgi = np.divide(1.0,lg)[:,np.newaxis]
     # gradf *= lgi
     gradf = np.cross(tn, gradf)
     divf = tria_compute_divergence(tria, gradf)
@@ -382,49 +369,48 @@
     vf = fem.poisson(divf)
     return vf
 
 
 def tria_mean_curvature_flow(
     tria, max_iter=30, stop_eps=1e-13, step=1.0, use_cholmod=False
 ):
-    """
-    mean_curvature_flow iteratively flows a triangle mesh along mean curvature
-    normal (non-singular, see Kazhdan 2012)
+    """Flow a triangle mesh along the mean curvature normal.
 
+    mean_curvature_flow iteratively flows a triangle mesh along mean curvature
+    normal (non-singular, see Kazhdan 2012).
     This uses the algorithm described in Kazhdan 2012 "Can mean curvature flow be
     made non-singular" which uses the Laplace-Beltrami operator but keeps the
     stiffness matrix (A) fixed and only adjusts the mass matrix (B) during the
     steps. It will normalize surface area of the mesh and translate the barycenter
     to the origin. Closed meshes will map to the unit sphere.
 
     Parameters
     ----------
     tria : TriaMesh
-         object of vertices and triangles
+        Triangle mesh.
     max_iter : int, default=30
-        maximal number of steps
+        Maximal number of steps.
     stop_eps : float, default=1e-13
-        stopping threshold
+        Stopping threshold.
     step : float, default=1.0
-        Euler step size
+        Euler step size.
     use_cholmod : bool, default=False
         Which solver to use:
-            * True : Use Cholesky decomposition from scikit-sparse cholmod
-            * False: Use spsolve (LU decomposition)
+            * True : Use Cholesky decomposition from scikit-sparse cholmod.
+            * False: Use spsolve (LU decomposition).
 
     Returns
     -------
     tria : TriaMesh
-        vertices and triangles
+        Triangle mesh after flow.
 
     Notes
-    -------
-    numexpr could speed up this functions if necessary
+    -----
+    Numexpr could speed up this functions if necessary.
     """
-
     if use_cholmod:
         sksparse = import_optional_dependency("sksparse", raise_error=True)
         importlib.import_module(".cholmod", sksparse.__name__)
     else:
         sksparse = None
     # pre-normalize
     trianorm = TriaMesh(tria.v, tria.t)
@@ -460,42 +446,42 @@
         if diff < stop_eps:
             print("Converged after {} iterations.".format(x + 1))
             break
     return trianorm
 
 
 def tria_spherical_project(tria, flow_iter=3, debug=False):
-    """
-    spherical(tria) computes the first three non-constant eigenfunctions
-           and then projects the spectral embedding onto a sphere. This works
-           when the first functions have a single closed zero level set,
-           splitting the mesh into two domains each. Depending on the original
-           shape triangles could get inverted. We also flip the functions
-           according to the axes that they are aligned with for the special
-           case of brain surfaces in FreeSurfer coordinates.
+    """Compute the first 3 non-constant eigenfunctions and project the spectral embedding onto a sphere.
+
+    Computes the first three non-constant eigenfunctions
+    and then projects the spectral embedding onto a sphere. This works
+    when the first functions have a single closed zero level set,
+    splitting the mesh into two domains each. Depending on the original
+    shape triangles could get inverted. We also flip the functions
+    according to the axes that they are aligned with for the special
+    case of brain surfaces in FreeSurfer coordinates.
 
     Parameters
     ----------
     tria : TriaMesh
-        object of vertices and triangles
+        Triangle mesh.
     flow_iter : int, default=3
-        mean curv flow iterations (3 should be enough)
+        Mean curv flow iterations (3 should be enough).
     debug : bool, default=False
-        prints debug values if true
+        Prints debug values if True.
 
     Returns
     -------
     tria: TriaMesh
-        object of vertices and triangles
+        Triangle mesh.
 
     Notes
     -----
-    numexpr could speed up this functions if necessary
-    """
-
+    Numexpr could speed up this functions if necessary.
+    """  # noqa: E501
     import math
 
     if not tria.is_closed():
         raise ValueError("Error: Can only project closed meshes!")
 
     # sub-function to compute flipped area of trias where normal
     # points towards origin, meaningful for the sphere, centered at zero
@@ -521,15 +507,15 @@
         data["Creator"] = "spherically_project.py"
         data["Refine"] = 0
         data["Degree"] = 1
         data["Dimension"] = 2
         data["Elements"] = tria.t.shape[0]
         data["DoF"] = evecs.shape[0]
         data["NumEW"] = 4
-        from .FuncIO import export_ev
+        from .io import export_ev
 
         export_ev(data, "debug.ev")
 
     # flip efuncs to align to coordinates consistently
     ev1 = evecs[:, 1]
     # ev1maxi = np.argmax(ev1)
     # ev1mini = np.argmin(ev1)
@@ -669,46 +655,47 @@
         # sys.exit(1)
         raise ValueError("spat vol (orthogonality) should be above .6")
 
     return trianew
 
 
 def tet_compute_gradient(tet, vfunc):
-    """
-    Computes gradient of a vertex function f (for each tetra)
+    r"""Compute gradient of a vertex function f (for each tetra).
 
-    grad(f) = [  (f_j - f_i) (vi-vk) x (vh-vk)
-               + (f_k - f_i) (vi-vh) x (vj-vh)
-               + (f_h - f_i) (vk-vi) x (vj-vi) ] / (2 V)
-            = [  f_i (?-?) x ( ? -?)
-               + f_j (vi-vk) x (vh-vk)
-               + f_k (vi-vh) x (vj-vh)
-               + f_h (vk-vi) x (vj-vi) ] / (2 V)
-    for tetrahedron (vi,vj,vk,vh) with volume V.
+    For a tetrahedron (vi,vj,vk,vh) with volume V we have:
+    
+    .. math::
+        grad(f) &= [  (f_j - f_i) (vi-vk) x (vh-vk) \\
+                &   + (f_k - f_i) (vi-vh) x (vj-vh) \\
+                &   + (f_h - f_i) (vk-vi) x (vj-vi) ] / (2 V) \\
+                &= [  f_i (?-?) x ( ? -?) \\
+                &   + f_j (vi-vk) x (vh-vk) \\
+                &   + f_k (vi-vh) x (vj-vh) \\
+                &   + f_h (vk-vi) x (vj-vi) ] / (2 V).
 
     Parameters
     ----------
     tet : TetMesh
-    vfunc : function
-        scalar function at vertices
+        Tetraheral mesh.
+    vfunc : array
+        Scalar function at vertices.
 
     Returns
     -------
-    tfunc : function
-        3d vector function of gradient at tetras
+    tfunc : array of shape (n, 3)
+        3d gradient vector at tetras.
 
     Notes
     -----
-    numexpr could speed up this functions if necessary
-
+    Numexpr could speed up this functions if necessary.
     Good background to read:
     Mancinelli, Livesu, Puppo, Gradient Field Estimation on Triangle Meshes
     http://pers.ge.imati.cnr.it/livesu/papers/MLP18/MLP18.pdf
-    http://dgd.service.tu-berlin.de/wordpress/vismathws10/2012/10/17/gradient-of-scalar-functions/
-    Desbrun ...
+    http://dgd.service.tu-berlin.de/wordpress/vismathws10/2012/10/17/gradient-of-scalar-functions
+    Desbrun et al.
     """
     import sys
 
     v0 = tet.v[tet.t[:, 0], :]
     v1 = tet.v[tet.t[:, 1], :]
     v2 = tet.v[tet.t[:, 2], :]
     v3 = tet.v[tet.t[:, 3], :]
@@ -736,39 +723,38 @@
     )
     # divided by parallelepiped vol
     tfunc = voli * (c1 + c2 + c3)
     return tfunc
 
 
 def tet_compute_divergence(tet, tfunc):
-    """
-    Computes integrated divergence of a 3d tetra function f (for each vertex)
+    """Compute integrated divergence of a 3d tetra function f (for each vertex).
 
     Divergence is the flux density leaving or entering a point.
     It can be measured by summing the dot product of the vector
     field with the normals to the outer faces of the 1-ring tetras
     around a vertex. Summing < tfunc , n_tria_oposite_v >
 
     Parameters
     ----------
     tet : TetMesh
-    tfunc : function
-        3d vector field on tets
+        Tetrahedral mesh.
+    tfunc : array
+        3d vector field on tets.
 
     Returns
     -------
-    vfunc: function
-        scalar function of divergence at vertices
+    vfunc: array
+        Scalar function of divergence at vertices.
 
     Notes
     -----
-    this is the integrated divergence, you may want to multiply
-    with B^-1 to get back the function in some applications
+    This is the integrated divergence, you may want to multiply
+    with B^-1 to get back the function in some applications.
     """
-
     v0 = tet.v[tet.t[:, 0], :]
     v1 = tet.v[tet.t[:, 1], :]
     v2 = tet.v[tet.t[:, 2], :]
     v3 = tet.v[tet.t[:, 3], :]
     e0 = v1 - v0
     e1 = v2 - v1
     e2 = v2 - v0
```

### Comparing `lapy-0.6.0/lapy/FuncIO.py` & `lapy-1.0.0/lapy/io.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,122 +1,66 @@
-import numpy as np
-
-
-def import_vfunc_deprecated(infile):
-    """
-    Imports vertex function from txt file. Values can be separated by ; or ,
-    and surrounded by {} or () brackets. Also first line can have the
-    keyword "Solution:", i.e. the PSOL format from ShapeDNA
-
-    Parameters
-    ----------
-    infile : str
-        filename of input
-
-    Returns
-    -------
-    vals : list
-        list of vfunc parameters
+"""Functions to read and write spectra and vertex functions."""
 
-    Notes
-    ------
-    deprecated, use import_vfunc() instead
-    """
-
-    import re
+import numpy as np
 
-    try:
-        f = open(infile, "r")
-    except IOError:
-        print("[File " + infile + " not found or not readable]")
-        return
-    txt = f.readlines()
-    i = 0
-    vals = list()
-    while i < len(txt):
-        if "Solution:" in txt[i]:
-            i = i + 1
-            tmp1 = list()
-            while i < len(txt):
-                if txt[i].isspace():
-                    break
-                tmp1.append(txt[i].strip())
-                i = i + 1
-            for tmp2 in re.split("[;,]", re.sub("[{()}]", "", "".join(tmp1))):
-                vals.append(float(tmp2))
-            # del (tmp1, tmp2)
-        i = i + 1
-    return vals
 
+def read_vfunc(filename):
+    """Import vertex functions from txt file.
 
-def import_vfunc(filename):
-    """
-    Imports vertex function from txt file. Values can be separated by ; or ,
-    and surrounded by {} or () brackets. Also first line can have the
-    keyword "Solution:", i.e. the PSOL format from ShapeDNA
+    Values can be separated by ``;`` or ``,`` and surrounded by ``{}`` or ``()``
+    brackets. Also first line can have the keyword "Solution:", i.e. the PSOL format
+    from ShapeDNA.
 
     Parameters
     ----------
     filename : str
-        filename of input
+        Filename of input.
 
     Returns
     -------
-    vals : np.ndarray
-        list of vfunc parameters
+    vals : array
+        List of vfunc parameters.
     """
-
     import re
 
-    import numpy as np
-
     try:
         with open(filename) as f:
             txt = f.readlines()
     except IOError:
         print("[File " + filename + " not found or not readable]")
         return
-
     txt = [x.strip() for x in txt]
-
     txt.remove("Solution:")
-
     txt = [re.sub("[{()}]", "", x) for x in txt]
-
     if len(txt) == 1:
         txt = [re.split("[,;]", x) for x in txt][0]
-
-    txt = [np.float(x) for x in txt]
-
+    txt = [float(x) for x in txt]
     # txt = np.array(txt)
-
     return txt
 
 
-def import_ev(infile):
-    """
-    Load EV file
+def read_ev(filename):
+    """Load EV file.
 
     Parameters
     ----------
-    infile : str
-        filename of input
+    filename : str
+        Filename of input.
 
     Returns
     -------
     d: dict
-        dictionary of eigenvalues, eigenvectors (optional), and associated
-        information
+        Dictionary of eigenvalues, eigenvectors (optional), and associated
+        information.
     """
-
     # open file
     try:
-        f = open(infile, "r")
+        f = open(filename, "r")
     except IOError:
-        print("[File " + infile + " not found or not readable]")
+        print("[File " + filename + " not found or not readable]")
         return
     # read file (and get rid of all \n)
     ll = f.read().splitlines()
     # define data structure
     d = dict()
     # go through each line and parse it
     i = 0
@@ -177,23 +121,23 @@
                 evals = ll[i].strip().replace("{", "").replace("}", "")
             else:
                 evals = str()
                 while ll[i].find("}") < 0:
                     evals = evals + ll[i].strip().replace("{", "").replace("}", "")
                     i = i + 1
                 evals = evals + ll[i].strip().replace("{", "").replace("}", "")
-            evals = np.array(evals.split(";")).astype(np.float)
+            evals = np.array(evals.split(";")).astype(float)
             d.update({"Eigenvalues": evals})
             i = i + 1
         elif ll[i].lstrip().startswith("Eigenvectors"):
             i = i + 1
             while not (ll[i].strip().startswith("sizes")):
                 i = i + 1
             d.update(
-                {"EigenvectorsSize": np.array(ll[i].strip().split()[1:]).astype(np.int)}
+                {"EigenvectorsSize": np.array(ll[i].strip().split()[1:]).astype(int)}
             )
             i = i + 1
             while ll[i].find("{") < 0:  # possibly introduce termination criterion
                 i = i + 1
             if ll[i].find("}") >= 0:  # '{' and '}' on the same line
                 evecs = ll[i].strip().replace("{", "").replace("}", "")
             else:
@@ -204,15 +148,15 @@
                     ).replace("(", "").replace(")", "")
                     i = i + 1
                 evecs = evecs + ll[i].strip().replace("{", "").replace("}", "").replace(
                     "(", ""
                 ).replace(")", "")
             evecs = np.array(
                 evecs.replace(";", " ").replace(",", " ").strip().split()
-            ).astype(np.float)
+            ).astype(float)
             if len(evecs) == (d["EigenvectorsSize"][0] * d["EigenvectorsSize"][1]):
                 evecs = np.transpose(np.reshape(evecs, d["EigenvectorsSize"][1::-1]))
                 d.update({"Eigenvectors": evecs})
             else:
                 print(
                     "[Length of eigenvectors is not "
                     + str(d["EigenvectorsSize"][0])
@@ -225,33 +169,30 @@
             i = i + 1
     # close file
     f.close()
     # return dict
     return d
 
 
-def export_ev(outfile, d):
-    """
-    Save EV data structures as txt file (format from ShapeDNA)
-    usage: exportEV(data,outfile)
+def write_ev(filename, d):
+    """Save EV data structures as txt file (format from ShapeDNA).
 
     Parameters
     ----------
-    outfile : str
-        filename to save to
+    filename : str
+        Filename to save to.
     d : dict
-        dictionary of eigenvalues, eigenvectors (optional), and associated
-        information
+        Dictionary of eigenvalues, eigenvectors (optional), and associated
+        information.
     """
-
     # open file
     try:
-        f = open(outfile, "w")
+        f = open(filename, "w")
     except IOError:
-        print("[File " + outfile + " not writable]")
+        print("[File " + filename + " not writable]")
         return
     # check data structure
     if "Eigenvalues" not in d:
         print("ERROR: no Eigenvalues specified")
         exit(1)
     # ...
     # Write
@@ -322,28 +263,27 @@
             )
         )
         f.write(") }\n")
     # close file
     f.close()
 
 
-def export_vfunc(outfile, vfunc):
-    """
-    Exports vertex function in PSOL txt file:
+def write_vfunc(filename, vfunc):
+    """Save vertex in PSOL txt file.
+
     First line "Solution:", "," separated values inside ()
 
     Parameters
     ----------
-    outfile : str
-        filename to save to
+    filename : str
+        Filename to save to.
     vfunc : array_like
-        list of vfunc parameters
+        List of vfunc parameters.
     """
-
     try:
-        f = open(outfile, "w")
+        f = open(filename, "w")
     except IOError:
-        print("[File " + outfile + " not writable]")
+        print("[File " + filename + " not writable]")
         return
     f.write("Solution:\n")
     f.write("(" + ",".join(vfunc.astype(str)) + ")")
     f.close()
```

### Comparing `lapy-0.6.0/lapy/Heat.py` & `lapy-1.0.0/lapy/heat.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,111 +1,114 @@
+"""Functions for computing heat kernel and diffusion.
+
+Inputs are eigenvalues and eigenvectors (for heat kernel) and the
+mesh geometries (tet or tria mesh) for heat diffusion. 
+"""
+
 import importlib
+from typing import Optional
 
 import numpy as np
 
 from .utils._imports import import_optional_dependency
 
 
 def diagonal(t, x, evecs, evals, n):
-    """
-    Computes heat kernel diagonal ( K(t,x,x,) )
-    for a given time t (can be a vector)
-    using only the first n smallest eigenvalues and eigenvectors
+    """Compute heat kernel diagonal ( K(t,x,x,) ).
+
+    For a given time t (can be a vector)
+    using only the first n smallest eigenvalues and eigenvectors.
 
     Parameters
     ----------
-    t : float or np.ndarray
-        time or a row vector of time values
-    x : np.ndarray
-        vertex ids for the positions of K(t,x,x)
-    evecs : np.ndarray
-        eigenvectors (matrix: vnum x evecsnum)
-    evals : np.ndarray
-        vector of eigenvalues (col vector: evecsnum x 1)
+    t : float | array
+        Time or a row vector of time values.
+    x : array
+        Vertex ids for the positions of K(t,x,x).
+    evecs : array
+        Eigenvectors (matrix: vnum x evecsnum).
+    evals : array
+        Vector of eigenvalues (col vector: evecsnum x 1).
     n : int
-        number of evecs and vals to use (smaller or equal length)
+        Number of evecs and vals to use (smaller or equal length).
 
     Returns
     -------
-    h:
-        matrix, rows: vertices selected in x, cols: times in t
+    h : array
+        Matrix, rows: vertices selected in x, cols: times in t.
     """
-
     # maybe add code to check dimensions of input and flip axis if necessary
     h = np.matmul(evecs[x, 0:n] * evecs[x, 0:n], np.exp(-np.matmul(evals[0:n], t)))
     return h
 
 
 def kernel(t, vfix, evecs, evals, n):
-    """
-    Computes heat kernel from all points to a fixed point (vfix)
-    for a given time t (using only the first n smallest eigenvalues
-    and eigenvectors)
+    r"""Compute heat kernel from all points to a fixed point (vfix).
 
-    K_t (p,q) = sum_j exp(-eval_j t) evec_j(p) evec_j(q)
+    For a given time t (using only the first n smallest eigenvalues
+    and eigenvectors):
+
+    .. math::
+        K_t (p,q) = \sum_j \ exp(-eval_j \ t) \ evec_j(p) \ evec_j(q)
 
     Parameters
     ----------
-    t : number or np.ndarray
-        time (can also be a row vector, if passing multiple times)
-    vfix : np.ndarray
-        fixed vertex index
-    evecs : np.ndarray
-        matrix of eigenvectors (M x N), M = #vertices, N=#eigenvectors
-    evals : np.ndarray
-        col vector of eigenvalues (N)
+    t : float | array
+        Time (can also be a row vector, if passing multiple times).
+    vfix : array
+        Fixed vertex index.
+    evecs : array
+        Matrix of eigenvectors (M x N), M=#vertices, N=#eigenvectors.
+    evals : array
+        Column vector of eigenvalues (N).
     n : int
-        number of eigenvalues/vectors used in heat kernel (n<=N)
+        Number of eigenvalues/vectors used in heat kernel (n<=N).
 
     Returns
     -------
-    h : np.ndarray
-        matrix m rows: all vertices, cols: times in t
+    h : array
+        Matrix m rows: all vertices, cols: times in t.
     """
-
     # h = evecs * ( exp(-evals * t) .* repmat(evecs(vfix,:)',1,length(t))  )
     h = np.matmul(evecs[:, 0:n], (np.exp(np.matmul(-evals[0:n], t)) * evecs[vfix, 0:n]))
     return h
 
 
-def diffusion(geometry, vids, m=1.0, aniso=None, use_cholmod=False):
-    """
-    Computes heat diffusion from initial vertices in vids using
-    backward Euler solution for time t:
+def diffusion(geometry, vids, m=1.0, aniso: Optional[int] = None, use_cholmod=False):
+    """Compute the heat diffusion from initial vertices in vids.
 
-      t = m * avg_edge_length^2
+    It uses the backward Euler solution :math:`t = m l^2`, where l describes
+    the average edge length.
 
     Parameters
     ----------
-    geometry : TriaMesh or TetMesh
-        Object on which to run diffusion
-    vids : array_like
-        vertex index or indices where initial heat is applied
+    geometry : TriaMesh | TetMesh
+        Geometric object on which to run diffusion.
+    vids : array
+        Vertex index or indices where initial heat is applied.
     m : float, default=1.0
-        factor  to compute time of heat evolution:
-                    t = m * avg_edge_length^2
-    aniso : , Default=None
-
+        Factor to compute time of heat evolution.
+    aniso : int
+        Number of smoothing iterations for curvature computation on vertices.
     use_cholmod : bool, default=False
         Which solver to use:
-            * True : Use Cholesky decomposition from scikit-sparse cholmod
-            * False: Use spsolve (LU decomposition)
+            * True : Use Cholesky decomposition from scikit-sparse cholmod.
+            * False: Use spsolve (LU decomposition).
 
     Returns
     -------
-    vfunc: function
-        heat diffusion at vertices
+    vfunc: array of shape (n, 1)
+        Heat diffusion at vertices.
     """
-
     if use_cholmod:
         sksparse = import_optional_dependency("sksparse", raise_error=True)
         importlib.import_module(".cholmod", sksparse.__name__)
     else:
         sksparse = None
-    from .Solver import Solver
+    from . import Solver
 
     nv = len(geometry.v)
     fem = Solver(geometry, lump=True, aniso=aniso)
     # time of heat evolution:
     t = m * geometry.avg_edge_length() ** 2
     # backward Euler matrix:
     hmat = fem.mass + t * fem.stiffness
```

### Comparing `lapy-0.6.0/lapy/Plot.py` & `lapy-1.0.0/lapy/plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-"""
-Dependency:
-    plotly 3.6
+"""Functions for plotting Tet and Tria Meshes with overlays.
+
+For visualizing results in a juypter notebook use this::
+
+    .. code-block:: python
 
-In jupyter notebook do this:
-    import plotly
-    plotly.offline.init_notebook_mode(connected=True)
+        import plotly
+        plotly.offline.init_notebook_mode(connected=True)
+        ...
 """
+
 import re
 from bisect import bisect
 
 import numpy as np
 import plotly
 import plotly.graph_objs as go
 
-# import matplotlib.cm as cm
-from .TetMesh import TetMesh
+from . import TetMesh
 
 
 def _get_color_levels():
-    """returns a pre-set colorscale
+    """Return a pre-set colorscale.
 
     Returns
     -------
     colorscale: array_like of shape (38, 2)
-        vector color for different levels
+        Vector color for different levels.
     """
-
     color1 = "rgb(55, 155, 255)"
     color2 = "rgb(255, 255, 0)"
     colorscale = [
         [0, color1],
         [0.09999, color1],
         [0.1, color2],
         [0.105, color2],
@@ -68,30 +69,28 @@
         [0.9050001, color1],
         [1, color1],
     ]
     return colorscale
 
 
 def _get_colorscale(vmin, vmax):
-    """
-    put together a colorscale map depending on the range of v-values
-    Parameters
+    """Put together a colorscale map depending on the range of v-values.
 
+    Parameters
     ----------
     vmin : float
-        minimum value
+        Minimum value.
     vmax : float
-        maximum value
+        Maximum value.
 
     Returns
     -------
     colorscale: array_like of shape (2,2)
-        colorscale map
+        Colorscale map.
     """
-
     if vmin > vmax:
         raise ValueError("incorrect relation between vmin and vmax")
     # color definitions
     posstart = "rgb(255, 0, 0)"
     posstop = "rgb(255, 255, 51)"
     negstart = "rgb(51, 255, 255)"
     negstop = "rgb(0, 0, 255)"
@@ -133,29 +132,28 @@
                 [zz + zero + eps, posstart],
                 [1, posstop],
             ]
     return colorscale
 
 
 def _get_colorval(t, colormap):
-    """turn a scalar value into a color value
+    """Turn a scalar value into a color value.
 
     Parameters
     ----------
     t : float
-        must be 0...1
+        Scalar must be 0...1.
     colormap : array_like
-        list of values and color code strings (should have entries at least for 0 and 1)
+        List of values and color code strings (with entries at least for 0 and 1).
 
     Returns
     -------
     cstr/*: str
-        interpolated color for this value of t
+        Interpolated color for this value of t.
     """
-
     if t == 0:
         return colormap[0][1]
     if t == 1:
         return colormap[-1][1]
     # ok here we need to interpolate
     # first find two colors before and after
     columns = list(zip(*colormap))
@@ -174,34 +172,32 @@
     cval = np.rint(rv1 + tt * (rv2 - rv1)).astype(int)
     # format as string again
     cstr = "rgb(%d, %d, %d)" % (cval[0], cval[1], cval[2])
     return cstr
 
 
 def _map_z2color(zval, colormap, zmin, zmax):
-    """
-    map the normalized value zval to a corresponding color in the colormap
+    """Map the normalized value zval to a corresponding color in the colormap.
 
     Parameters
     ----------
     zval : float
-        value to be mapped
-    colormap : matplotlib.colors.LinearSegmentedColormap or np.ndarray
-        list of values and color code strings
+        Value to be mapped.
+    colormap : matplotlib.colors.LinearSegmentedColormap | array
+        List of values and color code strings.
     zmin : float
-        minimum
+        Minimum.
     zmax : float
-        minimum
+        Maximum.
 
     Returns
     -------
     rgb : str
-        corresponding color of the zval
+        Corresponding color of the zval.
     """
-
     if zmin > zmax:
         raise ValueError("incorrect relation between zmin and zmax")
 
     t = (zval - zmin) / float((zmax - zmin))  # normalize val
     if type(colormap) == "matplotlib.colors.LinearSegmentedColormap":
         r, g, b, alpha = colormap(t)
         rgb = (
@@ -233,72 +229,64 @@
     flatshading=False,
     xrange=None,
     yrange=None,
     zrange=None,
     showcaxis=False,
     caxis=None,
 ):
-    """
-    plot tetra meshes
+    """Plot tetra meshes.
 
-    the tetra mesh will be converted to its tria boundary mesh,
+    The tetra mesh will be converted to its tria boundary mesh,
     and only this will be plotted.
 
     Parameters
     ----------
-    tetra : lapy.TetMesh.TetMesh
-        tetraheral mesh to plot
-    vfunc : function, Default=None
-        scalar function at vertices
+    tetra : lapy.TetMesh
+        Tetraheral mesh to plot.
+    vfunc : array_like, Default=None
+        Scalar function at vertices.
     plot_edges : bool, Default=False
-        whether to plot edges or not
+        Whether to plot edges or not.
     plot_levels : bool, Default=False
-        whether to plot levels or not
-    tfunc : function, Default=None
-        3d vector function of gradient
+        Whether to plot levels or not.
+    tfunc : array_like, Default=None
+        3d vector function of gradient.
     cutting : str, Default=None
-        to view the 'interior' of the tetra mesh, one or more cutting
+        To view the 'interior' of the tetra mesh, one or more cutting
         criteria can be defined as input arguments to this function:
-
         e.g. cutting=('x<-10') or cutting=('z>=5') or cutting=('f>4')
-
         where x,y,z represent dimensions 0,1,2 of the vertex array,
         and f represents the vfunc (which cannot be None if f is used
-        to define a cutting criterion)
+        to define a cutting criterion).
     edge_color : str, Default="rgb(50,50,50)"
-        color of the edge
+        Color of the edge.
     html_output : bool, Default=False
-        weather or not to give out as html output
+        Whether or not to give out as html output.
     width : int, Default=800
-        width of the plot (in px)
+        Width of the plot (in px).
     height : int, Default=800
-        height  of the plot (in px)
+        Height  of the plot (in px).
     flatshading : bool, Default=False
-        whether normal smoothing is applied to the meshes or not
+        Whether normal smoothing is applied to the meshes or not.
     xrange : list or tuple of shape (2, 1)
-        Sets the range of the x-axis
+        Sets the range of the x-axis.
     yrange : list or tuple of shape (2, 1)
-        Sets the range of the y-axis
-    zrange :  list or tuple of shape (2, 1)
-        Sets the range of the z-axis
+        Sets the range of the y-axis.
+    zrange : list or tuple of shape (2, 1)
+        Sets the range of the z-axis.
     showcaxis : bool, Default=False
-        whether a colorbar is displayed or not
+        Whether a colorbar is displayed or not.
     caxis : list or tuple of shape (2, 1):
         Sets the bound of the color domain.
         caxis[0] is lower bound caxis[1] upper bound.
-        Elements are int or float
+        Elements are int or float.
     """
-
     if type(tetra).__name__ != "TetMesh":
         raise ValueError("plot_tet_mesh works only on TetMesh class")
 
-    # from plotTriaMesh import plotTriaMesh
-    # from tria import is_oriented
-    # from tetra import tetra_get_boundary_tria, tetra_fix_orientation
-
     # evaluate cutting criteria
     if cutting is not None:
         # check inputs
         if type(cutting) is not list:
             cutting = [cutting]
 
         # check if vfunc is defined when functional thresholds are used, otherwise exit
@@ -396,68 +384,67 @@
     height=800,
     camera=None,
     html_output=False,
     export_png=None,
     scale_png=1.0,
     no_display=False,
 ):
-    """
-    plot tria mesh
+    """Plot tria mesh.
 
     Parameters
     ----------
-    tria : lapy.TriaMesh.Triamesh
-        triangle mesh to plot
-    vfunc : function, Default=None
-        scalar function at vertices
-    tfunc : function, Default=None
-        3d vector function of gradient
+    tria : lapy.TriaMesh
+        Triangle mesh to plot.
+    vfunc : array_like, Default=None
+        Scalar function at vertices.
+    tfunc : array_like, Default=None
+        3d vector function of gradient.
     vcolor : list of str, Default=None
-        Sets the color of each vertex
+        Sets the color of each vertex.
     tcolor : list of str, Default=None
-         Sets the color of each face
+         Sets the color of each face.
     showcaxis : bool, Default=False
-        whether a colorbar is displayed or not
+        Whether a colorbar is displayed or not.
     caxis : list or tuple of shape (2, 1):
         Sets the bound of the color domain.
         caxis[0] is lower bound caxis[1] upper bound.
-        Elements are int or float
+        Elements are int or float.
     xrange : list or tuple of shape (2, 1)
-        Sets the range of the x-axis
+        Sets the range of the x-axis.
     yrange : list or tuple of shape (2, 1)
-        Sets the range of the y-axis
-    zrange :  list or tuple of shape (2, 1)
-        Sets the range of the z-axis
+        Sets the range of the y-axis.
+    zrange : list or tuple of shape (2, 1)
+        Sets the range of the z-axis.
     plot_edges : bool, Default=False
-        whether to plot edges or not
+        Whether to plot edges or not.
     plot_levels : bool, Default=False
-        whether to plot levels or not
+        Whether to plot levels or not.
     edge_color : str, Default="rgb(50,50,50)"
-        color of the edge
+        Color of the edges.
     tic_color : str, Default="rgb(50,200,10)"
-        color of the ticks
+        Color of the ticks.
     background_color : str, Default=None
-        color of background
+        Color of background.
     flatshading : bool, Default=False
-        whether normal smoothing is applied to the meshes or not
+        Whether normal smoothing is applied to the meshes or not.
     width : int, Default=800
-        width of the plot (in px)
+        Width of the plot (in px).
     height : int, Default=800
-        height  of the plot (in px)
-    camera :
+        Height  of the plot (in px).
+    camera : dict of str, Default=None
+        Camera describing center, eye and up direction.
     html_output : bool, Default=False
-        weather or not to give out as html output
-    export_png : str or writeable, Default=None
-        local file path or a writeable object to write the image on
+        Whether or not to give out as html output.
+    export_png : str, Default=None
+        Local file path or file object to write the image to.
     scale_png : int or float
-        scale factor of image. >1.0 increase resolution; <1.0 decrease resolution
+        Scale factor of image. >1.0 increase resolution; <1.0 decrease resolution.
     no_display : bool, Default=False
-        whether to plot on display or not
+        Whether to plot on display or not.
     """
-
     # interesting example codes:
     # https://plot.ly/~empet/14749/mesh3d-with-intensities-and-flatshading/#/
 
     if type(tria).__name__ != "TriaMesh":
         raise ValueError("plot_tria_mesh works only on TriaMesh class")
 
     if (vfunc is not None or tfunc is not None) and (
```

### Comparing `lapy-0.6.0/lapy/ShapeDNA.py` & `lapy-1.0.0/lapy/shapedna.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,56 @@
+"""Functions for computing and comparing Laplace spectra.
+
+Includes code for solving the anisotropic Laplace-Beltrami eigenvalue
+problem as well as functions for normalization and comparison of 
+Laplace spectra. 
+"""
+
 import numpy as np
 import scipy.spatial.distance as di
 
-from .Solver import Solver
-from .TetMesh import TetMesh  # noqa: F401
-from .TriaMesh import TriaMesh  # noqa: F401
+from . import Solver
 
-# compute shapeDNA
 
-
-def compute_shapedna(geom, k=50, lump=False, aniso=None, aniso_smooth=10, use_cholmod=False):
-    """
-    a function to compute the shapeDNA descriptor for triangle or tetrahedral
-    meshes
+def compute_shapedna(
+    geom, k=50, lump=False, aniso=None, aniso_smooth=10, use_cholmod=False
+):
+    """Compute the shapeDNA descriptor for triangle or tetrahedral meshes.
 
     Parameters
     ----------
     geom : TriaMesh or TetMesh
-        geometry object
+        Mesh geometry.
     k : int, default=50
-        number of eigenfunctions / eigenvalues
-    lump : bool, Default=False
-        If True, lump the mass matrix (diagonal)
-            (See 'lapy.Solver.Solver' class)
-    aniso :  float or tuple of shape (2,)
+        Number of eigenfunctions / eigenvalues.
+    lump : bool, default=False
+        If True, lump the mass matrix (diagonal).
+            (See 'lapy.Solver.Solver' class).
+    aniso : float or tuple of shape (2,)
         Anisotropy for curvature based anisotopic Laplace.
-            (See 'lapy.Solver.Solver' class)
+            (See 'lapy.Solver.Solver' class).
     aniso_smooth : int
         Number of smoothing iterations for curvature computation on vertices.
-            (See 'lapy.Solver.Solver' class)
+            (See 'lapy.Solver.Solver' class).
     use_cholmod : bool, default: False
         If True, attempts to use the Cholesky decomposition for improved execution
-        speed. Requires the ``scikit-sparse`` library. If it can not be found, an error 
+        speed. Requires the ``scikit-sparse`` library. If it can not be found, an error
         will be thrown.
-        If False, will use slower LU decomposition.            
+        If False, will use slower LU decomposition.
 
     Returns
     -------
     ev : dict
-         a dictionary, including 'Eigenvalues' and 'Eigenvectors' fields
+        A dictionary, including 'Eigenvalues' and 'Eigenvectors' fields.
     """
-
     # get fem, evals, evecs
 
-    fem = Solver(geom, lump=lump, aniso=aniso, aniso_smooth=aniso_smooth, use_cholmod=use_cholmod)
+    fem = Solver(
+        geom, lump=lump, aniso=aniso, aniso_smooth=aniso_smooth, use_cholmod=use_cholmod
+    )
     evals, evecs = fem.eigs(k=k)
 
     # write ev
 
     evDict = dict()
     evDict["Refine"] = 0
     evDict["Degree"] = 1
@@ -59,38 +63,33 @@
     evDict["NumEW"] = k
     evDict["Eigenvalues"] = evals
     evDict["Eigenvectors"] = evecs
 
     return evDict
 
 
-# function for ev normalization
-
-
 def normalize_ev(geom, evals, method="geometry"):
-    """
-    a function for surface / volume normalization
+    """Normalize a surface or a volume.
 
     Parameters
     ----------
     geom : TriaMesh or TetMesh
-        geometry object
+        Mesh geometry.
     evals : array_like
-        vector of eigenvalues
+        Set of sorted eigenvalues.
     method : str
-        either "surface", "volume", or "geometry";
+        Either "surface", "volume", or "geometry";
         "geometry" will perform surface normalization for
-        2D objects, and volume normalization for 3D objects
+        2D objects, and volume normalization for 3D objects.
 
     Returns
     -------
     array_like
-        vector of reweighted eigenvalues
+        Vector of re-weighted eigenvalues.
     """
-
     if method == "surface":
         vol = geom.area()
 
         return evals * vol ** np.divide(2.0, 2.0)
 
     elif method == "volume":
         if type(geom).__name__ == "TriaMesh":
@@ -119,57 +118,48 @@
             bnd.orient_()
 
             vol = bnd.volume()
 
             return evals * vol ** np.divide(2.0, 3.0)
 
 
-# function for linear reweighting
-
-
 def reweight_ev(evals):
-    """
-    a function for linear reweighting
+    """Apply linear re-weighting.
 
     Parameters
     ----------
     evals : array_like
-        vector of eigenvalues
+        Set of sorted eigenvalues.
 
     Returns
     -------
     evals: array_like
-        vector of reweighted eigenvalues
+        Vector of re-weighted eigenvalues.
     """
-
     # evals[1:] = evals[1:] / np.arange(1, len(evals))
     evals = evals / np.arange(1, len(evals) + 1)
 
     return evals
 
 
-# compute distance
-
-
 def compute_distance(ev1, ev2, dist="euc"):
-    """
-    a function to compute the shape asymmetry from two shapeDNA descriptors
-    for triangle or tetrahedral meshes
+    """Compute the shape dissimilarity from two shapeDNA descriptors.
 
     Parameters
     ----------
-    ev1, ev2 : float
-        eigenvalues
+    ev1 : array_like
+        First set of sorted eigenvalues.
+    ev2 : array_like
+        Second set of sorted eigenvalues.
     dist : str
-        distance measure; currently only 'euc' (euclidean)
+        Distance measure; currently only 'euc' (Euclidean).
 
     Returns
     -------
-    * :  double
-        a distance measure
+    * : float
+        Distance between the eigenvalue arrays.
     """
-
     if dist == "euc":
         return di.euclidean(ev1, ev2)
     else:
         print("Only euclidean distance is currently implemented.")
         return
```

### Comparing `lapy-0.6.0/lapy/Solver.py` & `lapy-1.0.0/lapy/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import sys
 import importlib
+import sys
 from typing import Optional, Tuple, Union
 
 import numpy as np
 from scipy import sparse
 
-from .TetMesh import TetMesh
-from .TriaMesh import TriaMesh
+from .tet_mesh import TetMesh
+from .tria_mesh import TriaMesh
 from .utils._imports import import_optional_dependency
 
 
 class Solver:
-    """A linear FEM solver for Laplace Eigenvalue problems and Poisson Equation.
+    """FEM solver for Laplace Eigenvalue and Poisson Equation.
 
     Inputs can be geometry classes which have vertices and elements.
     Currently `~lapy.TriaMesh` and `~lapy.TetMesh` are implemented.
     FEM matrices (stiffness (or A) and mass matrix (or B)) are computed
     during the construction. After that the Eigenvalue solver (`lapy.Solver.eigs`) or
     Poisson Solver (`lapy.Solver.poisson`) can be called.
 
@@ -28,19 +28,19 @@
     aniso : float | tuple of shape (2,)
         Anisotropy for curvature based anisotopic Laplace.
         If a tuple ``(a_min, a_max), differentially affects the minimum and maximum
         curvature directions. e.g. ``(0, 50)`` will set scaling to 1 into the minimum
         curvature direction, even if the maximum curvature is large in those regions (
         i.e. isotropic in regions with large maximum curvature and minimum curvature
         close to 0, i.e. a concave cylinder).
-    aniso_smooth : int
+    aniso_smooth : int | None
         Number of smoothing iterations for curvature computation on vertices.
     use_cholmod : bool, default: False
         If True, attempts to use the Cholesky decomposition for improved execution
-        speed. Requires the ``scikit-sparse`` library. If it can not be found, an error 
+        speed. Requires the ``scikit-sparse`` library. If it can not be found, an error
         will be thrown.
         If False, will use slower LU decomposition.
 
     Notes
     -----
     The class has a static member to create the mass matrix of `~lapy.TriaMesh` for
     external function that do not need stiffness.
@@ -299,17 +299,17 @@
         Returns
         -------
         B : csc_matrix of shape (n, n)
             Sparse symmetric positive definite matrix.
 
         Notes
         -----
-        This only returns the mass matrix ``B`` of the Eigenvalue problem:
-        ``A x = lambda B x``. The area of the surface mesh can be obtained via
-        ``B.sum()``.
+            This only returns the mass matrix ``B`` of the Eigenvalue problem:
+            ``A x = lambda B x``. The area of the surface mesh can be obtained via
+            ``B.sum()``.
         """  # noqa: E501
         # Compute vertex coordinates and a difference vector for each triangle:
         t1 = tria.t[:, 0]
         t2 = tria.t[:, 1]
         t3 = tria.t[:, 2]
         v1 = tria.v[t1, :]
         v2 = tria.v[t2, :]
@@ -621,15 +621,15 @@
         ----------
         k : int
             The number of eigenvalues and eigenvectors desired. ``k`` must be smaller
             than ``N``. It is not possible to compute all eigenvectors of a matrix.
 
         Returns
         -------
-        eigenvalues : array of shape (k)
+        eigenvalues : array of shape (k,)
             Array of k eigenvalues. For closed meshes or Neumann boundary condition,
             ``0`` will be the first eigenvalue (with constant eigenvector).
         eigenvectors : array of shape (N, k)
             Array representing the k eigenvectors. The column ``eigenvectors[:, i]`` is
             the eigenvector corresponding to ``eigenvalues[i]``.
         """
         from scipy.sparse.linalg import LinearOperator, eigsh
```

### Comparing `lapy-0.6.0/lapy/TetIO.py` & `lapy-1.0.0/lapy/_tet_io.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,39 @@
-#!/usr/bin/env python
-# -*- coding: latin-1 -*-
-#
-# Original Author: Martin Reuter
-# Date: Jul-5-2018
-#
+"""Functions for IO of Tetrahedra Meshes.
+
+Should be called via the TetMesh member functions.
+"""
 
 import os.path
 
 import numpy as np
 
-from .TetMesh import TetMesh
-
 
-def import_gmsh(infile):
-    """
-    Load GMSH tetrahedron mesh
+def read_gmsh(filename):
+    """Load GMSH tetrahedron mesh.
 
     Parameters
     ----------
-    infile : str
-        filename to load
+    filename : str
+        Filename to load.
 
     Returns
     -------
     tet : TetMesh
-        Object of loaded  GMSH tetrahedron mesh
+        Object of loaded  GMSH tetrahedron mesh.
     """
-
-    extension = os.path.splitext(infile)[1]
+    extension = os.path.splitext(filename)[1]
     verbose = 1
     if verbose > 0:
         print("--> GMSH format         ... ")
     if extension != ".msh":
         print("[no .msh file] --> FAILED\n")
         return
     try:
-        f = open(infile, "r")
+        f = open(filename, "r")
     except IOError:
         print("[file not found or not readable]\n")
         return
     line = f.readline()
     if not line.startswith("$MeshFormat"):
         print("[$MeshFormat keyword not found] --> FAILED\n")
         f.close()
@@ -106,37 +100,37 @@
     if not line.startswith("$EndElements"):
         print("Line: ", line, " \n")
         print("[$EndElements keyword not found] --> FAILED\n")
         f.close()
         return
     f.close()
     print(" --> DONE ( V: " + str(v.shape[0]) + " , T: " + str(t.shape[0]) + " )\n")
+    from . import TetMesh
+
     return TetMesh(v, t)
 
 
-def import_vtk(infile):
-    """
-    Load VTK tetrahedron mesh
+def read_vtk(filename):
+    """Load VTK tetrahedron mesh.
 
     Parameters
     ----------
-    infile : str
-        filename to load
+    filename : str
+        Filename to load.
 
     Returns
     -------
     tet : TetMesh
-        Object of loaded  VTK tetrahedron mesh
+        Object of loaded  VTK tetrahedron mesh.
     """
-
     verbose = 1
     if verbose > 0:
         print("--> VTK format         ... ")
     try:
-        f = open(infile, "r")
+        f = open(filename, "r")
     except IOError:
         print("[file not found or not readable]\n")
         return
     # skip comments
     line = f.readline()
     while line[0] == "#":
         line = f.readline()
@@ -193,34 +187,34 @@
             return
         t = np.delete(t, 0, 1)
     else:
         print("[read: " + line + " expected POLYGONS or CELLS] --> FAILED\n")
         return
     f.close()
     print(" --> DONE ( V: " + str(v.shape[0]) + " , T: " + str(t.shape[0]) + " )\n")
+    from . import TetMesh
+
     return TetMesh(v, t)
 
 
-def export_vtk(tet, outfile):
-    """
-    Save VTK file
+def write_vtk(tet, filename):
+    """Save VTK file.
 
     Parameters
     ----------
     tet : TetMesh
-        tetrahedron mesh to save
-    outfile : str
-        filename to save to
+        Tetrahedron mesh to save.
+    filename : str
+        Filename to save to.
     """
-
     # open file
     try:
-        f = open(outfile, "w")
+        f = open(filename, "w")
     except IOError:
-        print("[File " + outfile + " not writable]")
+        print("[File " + filename + " not writable]")
         return
     # check data structure
     # ...
     # Write
     f.write("# vtk DataFile Version 1.0\n")
     f.write("vtk output\n")
     f.write("ASCII\n")
```

### Comparing `lapy-0.6.0/lapy/TetMesh.py` & `lapy-1.0.0/lapy/tet_mesh.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,136 +1,140 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-"""
-
-Dependency:
-    Scipy 0.10 or later for sparse matrix support
-
-
-Original Author: Martin Reuter
-Date: Feb-01-2019
-"""
-
 import numpy as np
 from scipy import sparse
 
+from . import _tet_io as io
+
 
 class TetMesh:
-    """
-    A class representing a tetraheral mesh
+    """Class representing a tetraheral mesh.
+
+    This is an efficient implementation of a tetrahedral mesh data structure
+    with core functionality using sparse matrices internally (Scipy).
 
-    Attributes
-    -------
+    Parameters
+    ----------
     v : array_like
-        List of lists of 3 float coordinates
+        List of lists of 3 float coordinates.
     t : array_like
-        List of lists of 4 int of indices (>=0) into v array
-    adj_sym : scipy.sparse.csc_matrix
-        symmetric adjacency matrix as csc sparse matrix
-
-    Methods
-    -------
-    construct_adj_sym()
-        Creates adjacency symmetric matrix
-    has_free_vertices()
-        Checks if the vertex list has more vertices than what is used in tetra
-    is_oriented()
-        Check if tet mesh is oriented
-    avg_edge_length()
-        Get average edge lengths in tet mesh
-    boundary_tria(tetfunc)
-        Get boundary triangle mesh of tetrahedra
-    rm_free_vertices_()
-        Remove unused (free) vertices from v and t
-    orient_()
-        Ensure that tet mesh is oriented
+        List of lists of 4 int of indices (>=0) into ``v`` array.
+        Ordering is important: so that t0, t1, t2 are oriented
+        counterclockwise when looking from above, and t3 is
+        on top of that triangle.
+
+    Notes
+    -----
+    The class has static class methods to read tetrahera meshes from
+    `GMSH <https://gmsh.info/doc/texinfo/gmsh.html#MSH-file-format>`_
+    and `VTK <https://examples.vtk.org/site/VTKFileFormats/>`_ files.
     """
 
     def __init__(self, v, t):
-        """Constructor
-
-        Parameters
-        ----------
-        v : array_like
-            List of lists of 3 float coordinates
-        t : array_like
-            List of lists of 4 int of indices (>=0) into v array
-            Ordering is important: so that t0,t1,t2 are oriented
-            counterclockwise when looking from above, and t3 is
-            on top of that triangle.
-
-        Raises
-        -------
-        ValueError
-            Max index exceeds number of vertices
-        """
-
         self.v = np.array(v)
         self.t = np.array(t)
         vnum = np.max(self.v.shape)
         if np.max(self.t) >= vnum:
             raise ValueError("Max index exceeds number of vertices")
         # put more checks here (e.g. the dim 3 conditions on columns)
         # self.orient_()
         self.adj_sym = self.construct_adj_sym()
 
+    @classmethod
+    def read_gmsh(cls, filename):
+        """Load GMSH tetrahedron mesh.
+
+        Parameters
+        ----------
+        filename : str
+            Filename to load.
+
+        Returns
+        -------
+        tet : TetMesh
+            Object of loaded GMSH tetrahedron mesh.
+        """
+        return io.read_gmsh(filename)
+
+    @classmethod
+    def read_vtk(cls, filename):
+        """Load VTK tetrahedron mesh.
+
+        Parameters
+        ----------
+        filename : str
+            Filename to load.
+
+        Returns
+        -------
+        tet : TetMesh
+            Object of loaded VTK tetrahedron mesh.
+        """
+        return io.read_vtk(filename)
+
+    def write_vtk(self, filename):
+        """Save as VTK file.
+
+        Parameters
+        ----------
+        filename : str
+            Filename to save to.
+        """
+        io.write_vtk(self, filename)
+
     def construct_adj_sym(self):
-        """Creates adjacency symmetric matrix
+        """Create adjacency symmetric matrix.
 
         The adjacency matrix will be symmetric. Each inner
         edge will get the number of tetrahedra that contain this edge.
         Inner edges are usually 3 or larger, boundary, 2 or 1.
         Works on tetras only.
 
         Returns
         -------
-        adj : scipy.sparse.csc_matrix
-            symmetric adjacency matrix as csc sparse matrix
+        adj : csc_matrix
+            Symmetric adjacency matrix as csc sparse matrix.
         """
-
         t1 = self.t[:, 0]
         t2 = self.t[:, 1]
         t3 = self.t[:, 2]
         t4 = self.t[:, 3]
         i = np.column_stack((t1, t2, t2, t3, t3, t1, t1, t2, t3, t4, t4, t4)).reshape(
             -1
         )
         j = np.column_stack((t2, t1, t3, t2, t1, t3, t4, t4, t4, t1, t2, t3)).reshape(
             -1
         )
         adj = sparse.csc_matrix((np.ones(i.shape), (i, j)))
         return adj
 
     def has_free_vertices(self):
-        """
-        Checks if the vertex list has more vertices than what is used in tetra
-        (same implementation as in TriaMesh)
+        """Check if the vertex list has more vertices than what is used in tetra.
+
+        (same implementation as in `~lapy.TriaMesh`)
 
         Returns
         -------
         bool
-            whether vertex list has more vertices than tetra or not
+            Whether vertex list has more vertices than tetra or not.
         """
-
         vnum = np.max(self.v.shape)
         vnumt = len(np.unique(self.t.reshape(-1)))
         return vnum != vnumt
 
     def is_oriented(self):
-        """
-        Check if tet mesh is oriented. True if all tetrahedra are oriented
+        """Check if tet mesh is oriented.
+
+        True if all tetrahedra are oriented
         so that v0,v1,v2 are oriented counterclockwise when looking from above,
         and v3 is on top of that triangle.
 
         Returns
         -------
         oriented: bool
-            True if max(adj_directed)=1
+            True if ``max(adj_directed)=1``.
         """
-
         # Compute vertex coordinates and a difference vector for each triangle:
         t0 = self.t[:, 0]
         t1 = self.t[:, 1]
         t2 = self.t[:, 2]
         t3 = self.t[:, 3]
         v0 = self.v[t0, :]
         v1 = self.v[t1, :]
@@ -152,55 +156,55 @@
             print("We have degenerated zero-volume tetrahedra")
             return False
         else:
             print("Orientations are not uniform")
             return False
 
     def avg_edge_length(self):
-        """
-        Get average edge lengths in tet mesh
+        """Get average edge lengths in tet mesh.
 
         Returns
         -------
-        double
-            average edge length
+        float
+            Average edge length.
         """
-
         # get only upper off-diag elements from symmetric adj matrix
         triadj = sparse.triu(self.adj_sym, 1, format="coo")
         edgelens = np.sqrt(
             ((self.v[triadj.row, :] - self.v[triadj.col, :]) ** 2).sum(1)
         )
         return edgelens.mean()
 
     def boundary_tria(self, tetfunc=None):
-        """
-        Get boundary triangle mesh of tetrahedra (can have multiple connected
-        components). Tria will have same vertices (including free vertices),
+        """Get boundary triangle mesh of tetrahedra.
+
+        It can have multiple connected components.
+        Tria will have same vertices (including free vertices),
         so that the tria indices agree with the tet-mesh, in case we want to
         transfer information back, e.g. a FEM boundary condition, or to access
         a TetMesh vertex function with TriaMesh.t indices.
 
-        !! Note, that it seems to be returning non-oriented triangle meshes,
-        may need some debugging, until then use tria.orient_() after this. !!
+        .. warning::
+
+            Note, that it seems to be returning non-oriented triangle meshes,
+            may need some debugging, until then use tria.orient_() after this.
 
         Parameters
         ----------
-        tetfunc : array_like, Default=None
-            List of tetra function values (optional)
+        tetfunc : array | None
+            List of tetra function values (optional).
 
         Returns
         -------
         TriaMesh
-            TriaMesh of boundary (potentially >1 components)
-        triafunc array_like
-            List of tria function values (if tetfunc passed)
+            TriaMesh of boundary (potentially >1 components).
+        triafunc : array
+            List of tria function values (only returned if ``tetfunc`` is provided).
         """
-
-        from .TriaMesh import TriaMesh
+        from . import TriaMesh
 
         # get all triangles
         allt = np.vstack(
             (
                 self.t[:, np.array([3, 1, 2])],
                 self.t[:, np.array([2, 0, 3])],
                 self.t[:, np.array([1, 3, 0])],
@@ -220,35 +224,29 @@
             alltidx = np.tile(np.arange(self.t.shape[0]), 4)
             tidx = alltidx[indices[count == 1]]
             triafunc = tetfunc[tidx]
             return TriaMesh(self.v, tria), triafunc
         return TriaMesh(self.v, tria)
 
     def rm_free_vertices_(self):
-        """
-        Remove unused (free) vertices from v and t. These are vertices that are not
-        used in any triangle. They can produce problems when constructing, e.g.,
-        Laplace matrices.
+        """Remove unused (free) vertices from v and t.
+
+        These are vertices that are not used in any triangle. They can produce problems
+        when constructing, e.g., Laplace matrices.
 
         Will update v and t in mesh.
-        Same implementation as in TriaMesh
+        Same implementation as in `~lapy.TriaMesh`.
 
         Returns
         -------
-        vkeep: np.ndarray
-            Indices (from original list) of kept vertices
-        vdel: np.ndarray
-            Indices of deleted (unused) vertices
-
-        Raises
-        -------
-        ValueError
-            Max index exceeds number of vertices
+        vkeep: array
+            Indices (from original list) of kept vertices.
+        vdel: array
+            Indices of deleted (unused) vertices.
         """
-
         tflat = self.t.reshape(-1)
         vnum = np.max(self.v.shape)
         if np.max(tflat) >= vnum:
             raise ValueError("Max index exceeds number of vertices")
         # determine which vertices to keep
         vkeep = np.full(vnum, False, dtype=bool)
         vkeep[tflat] = True
@@ -266,25 +264,25 @@
         # convert vkeep to index list
         vkeep = np.nonzero(vkeep)[0]
         self.v = vnew
         self.t = tnew
         return vkeep, vdel
 
     def orient_(self):
-        """
-        Ensure that tet mesh is oriented. Re-orient tetras so that
+        """Ensure that tet mesh is oriented.
+
+        Re-orient tetras so that
         v0,v1,v2 are oriented counterclockwise when looking from above,
         and v3 is on top of that triangle.
 
         Returns
         -------
         onum : int
-            number of re-oriented tetras
+            Number of re-oriented tetras.
         """
-
         # Compute vertex coordinates and a difference vector for each tetra:
         t0 = self.t[:, 0]
         t1 = self.t[:, 1]
         t2 = self.t[:, 2]
         t3 = self.t[:, 3]
         v0 = self.v[t0, :]
         v1 = self.v[t1, :]
```

### Comparing `lapy-0.6.0/lapy/TriaIO.py` & `lapy-1.0.0/lapy/_tria_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,64 @@
-#!/usr/bin/env python
-# -*- coding: latin-1 -*-
+"""Functions for IO of Triangle Meshes.
 
+Should be called via the TriaMesh member functions.
+"""
 
 import numpy as np
 
-from .TriaMesh import TriaMesh
 
-
-def import_fssurf(infile):
-    """
-    Load triangle mesh from FreeSurfer surface geometry file
+def read_fssurf(filename):
+    """Load triangle mesh from FreeSurfer surface geometry file.
 
     Parameters
     ----------
-    infile : str
-        filename to load
+    filename : str
+        Filename to load.
 
     Returns
     -------
     TriaMesh
-        loaded triangle mesh
+        Loaded triangle mesh.
     """
-
     verbose = 1
     if verbose > 0:
         print("--> FS Surf format     ... ")
     try:
         # here we use our copy to also support surfaces from dev (and maybe v7*?)
         # these have an empty line and mess up Nibabel
         # once this is fixed in nibabel we can switch back
-        from .read_geometry import read_geometry
+        from ._read_geometry import read_geometry
 
-        surf = read_geometry(infile, read_metadata=True)
+        surf = read_geometry(filename, read_metadata=True)
     except IOError:
         print("[file not found or not readable]\n")
         return
+    from . import TriaMesh
 
     return TriaMesh(surf[0], surf[1], fsinfo=surf[2])
 
 
-def import_off(infile):
-    """
-    Load triangle mesh from OFF txt file
+def read_off(filename):
+    """Load triangle mesh from OFF txt file.
 
     Parameters
     ----------
-    infile : str
-        filename to load
+    filename : str
+        Filename to load.
 
     Returns
     -------
     TriaMesh
-        loaded triangle mesh
+        Loaded triangle mesh.
     """
-
     verbose = 1
     if verbose > 0:
         print("--> OFF format         ... ")
     try:
-        f = open(infile, "r")
+        f = open(filename, "r")
     except IOError:
         print("[file not found or not readable]\n")
         return
     line = f.readline()
     while line[0] == "#":
         line = f.readline()
     if not line.startswith("OFF"):
@@ -88,38 +84,37 @@
     if np.amax(t[:, 0]) != 3:
         print("[no triangle data] --> FAILED\n")
         f.close()
         return
     t = t[:, 1:]
     f.close()
     print(" --> DONE ( V: " + str(v.shape[0]) + " , T: " + str(t.shape[0]) + " )\n")
+    from . import TriaMesh
+
     return TriaMesh(v, t)
 
 
-def import_vtk(infile):
-    """
-    Load triangle mesh from VTK txt file
-    :return:    TriaMesh
+def read_vtk(filename):
+    """Load triangle mesh from VTK txt file.
 
     Parameters
     ----------
-    infile : str
-        filename to load
+    filename : str
+        Filename to load.
 
     Returns
     -------
     TriaMesh
-        loaded triangle mesh
+        Loaded triangle mesh.
     """
-
     verbose = 1
     if verbose > 0:
         print("--> VTK format         ... ")
     try:
-        f = open(infile, "r")
+        f = open(filename, "r")
     except IOError:
         print("[file not found or not readable]\n")
         return
     # skip comments
     line = f.readline()
     while line[0] == "#":
         line = f.readline()
@@ -200,47 +195,47 @@
                 tt.append(tria)
         t = np.array(tt)
     else:
         print("[read: " + line + " expected POLYGONS or TRIANGLE_STRIPS] --> FAILED\n")
         return
     f.close()
     print(" --> DONE ( V: " + str(v.shape[0]) + " , T: " + str(t.shape[0]) + " )\n")
+    from . import TriaMesh
+
     return TriaMesh(v, t)
 
 
-def import_gmsh(infile):
-    """
-    Load GMSH tetra mesh ASCII Format
+def read_gmsh(filename):
+    """Load GMSH tetra mesh ASCII Format.
 
     Parameters
     ----------
-    infile : str
-        filename to load
+    filename : str
+        Filename to load.
 
     Returns
     -------
-    points : np.ndarray
-        List of points
+    points : array
+        List of points.
     cells : array_like
-        List of cells
+        List of cells.
     point_data : array_like
-        data of points
+        Data of points.
     cell_data : aray_like
-        data of cells
+        Data of cells.
     field_data : array_like
-        data of fields
+        Data of fields.
 
     Notes
-    -------
+    -----
     http://geuz.org/gmsh/doc/texinfo/gmsh.html#MSH-ASCII-file-format
     .. moduleauthor:: Nico Schloemer <nico.schloemer@gmail.com>
     LICENSE MIT
     https://github.com/nschloe/meshio
     """
-
     import logging
     import struct
 
     import numpy
 
     num_nodes_per_cell = {
         "vertex": 1,
@@ -287,15 +282,15 @@
     _meshio_to_gmsh_type = {v: k for k, v in _gmsh_to_meshio_type.items()}  # noqa: F841
 
     verbose = 1
     if verbose > 0:
         print("--> GMSH format         ... ")
 
     try:
-        f = open(infile, "r")
+        f = open(filename, "r")
     except IOError:
         print("[file not found or not readable]\n")
         return
 
     # Initialize the data optional data fields
     points = []
     cells = {}
@@ -469,32 +464,29 @@
 
     if has_additional_tag_data:
         logging.warning("The file contains tag data that couldn't be processed.")
 
     return points, cells, point_data, cell_data, field_data
 
 
-def export_vtk(tria, outfile):
-    """
-    Save VTK file
-    usage: exportVTK(TriaMesh,outfile)
+def write_vtk(tria, filename):
+    """Save VTK file.
 
     Parameters
     ----------
     tria : TriaMesh
-        Triangle mesh to save
-    outfile : str
-        filename to save to
+        Triangle mesh to save.
+    filename : str
+        Filename to save to.
     """
-
     # open file
     try:
-        f = open(outfile, "w")
+        f = open(filename, "w")
     except IOError:
-        print("[File " + outfile + " not writable]")
+        print("[File " + filename + " not writable]")
         return
     # check data structure
     # ...
     # Write
     f.write("# vtk DataFile Version 1.0\n")
     f.write("vtk output\n")
     f.write("ASCII\n")
@@ -512,30 +504,25 @@
     )
     for i in range(np.shape(tria.t)[0]):
         f.write(" ".join(map(str, np.append(3, tria.t[i, :]))))
         f.write("\n")
     f.close()
 
 
-def export_fssurf(tria, outfile):
-    """
-    Save Freesurfer Surface Geometry file (wrap Nibabel)
+def write_fssurf(tria, filename):
+    """Save Freesurfer Surface Geometry file (wrap Nibabel).
 
     Parameters
     ----------
     tria : TriaMesh
-        Triangle mesh to save
-    outfile : str
-        filename to save to
-
-    Returns
-    -------
-    None
+        Triangle mesh to save.
+    filename : str
+        Filename to save to.
     """
     # open file
     try:
         from nibabel.freesurfer.io import write_geometry
 
-        write_geometry(outfile, tria.v, tria.t, volume_info=tria.fsinfo)
+        write_geometry(filename, tria.v, tria.t, volume_info=tria.fsinfo)
     except IOError:
-        print("[File " + outfile + " not writable]")
+        print("[File " + filename + " not writable]")
         return
```

### Comparing `lapy-0.6.0/lapy/TriaMesh.py` & `lapy-1.0.0/lapy/tria_mesh.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,130 +1,53 @@
+import sys
+
 import numpy as np
 from scipy import sparse
 
-"""
-
-Dependency:
-    Scipy 0.10 or later for sparse matrix support
+from . import _tria_io as io
 
 
-Original Author: Martin Reuter
-Date: Feb-01-2019
-"""
+class TriaMesh:
+    """Class representing a triangle mesh.
 
+    This is an efficient implementation of a triangle mesh data structure
+    with core functionality using sparse matrices internally (Scipy).
 
-class TriaMesh:
-    """
-    A class representing a triangle mesh
+    Parameters
+    ----------
+    v : array_like
+        List of lists of 3 float coordinates.
+    t : array_like
+        List of lists of 3 int of indices (>= 0) into ``v`` array
+        Ordering is important: All triangles should be
+        oriented in the same way (counter-clockwise, when
+        looking from above).
+    fsinfo : dict | None
+        FreeSurfer Surface Header Info.
 
     Attributes
-    -------
+    ----------
     v : array_like
-        List of lists of 3 float coordinates
+        List of lists of 3 float coordinates.
     t : array_like
-        List of lists of 4 int of indices (>=0) into v array
-    adj_sym : scipy.sparse.csc_matrix
-        symmetric adjacency matrix as csc sparse matrix
-    adj_dir :
-        directed adjacency matrix as csc sparse matrix
-    fsinfo :
-        FreeSurfer Surface Header Info
-
-    Methods
-    -------
-    _construct_adj_sym()
-        Constructs symmetric adjacency matrix
-    _construct_adj_dir()
-        Constructs directed adjacency matrix of triangle mesh t
-    construct_adj_dir_tidx()
-        Constructs directed adjacency matrix of triangle mesh t
-        containing the triangle indices
-    is_closed()
-        Check if triangle mesh is closed
-    is_manifold()
-        Check if triangle mesh is manifold
-    is_oriented()
-        Check if triangle mesh is oriented
-    euler()
-        Computes the Euler Characteristic
-    tria_areas()
-        Computes the area of triangles
-    area()
-        Computes the total surface area of triangle mesh
-    volume()
-        Computes the volume of closed triangle mesh
-    vertex_degrees()
-        Computes the vertex degrees
-    vertex_areas()
-        Computes the area associated to each vertex
-    avg_edge_length()
-        Computes the average edge length of the mesh
-    tria_normals()
-        Computes triangle normals
-    vertex_normals()
-        computes vertex normals
-    has_free_vertices()
-        Checks if the vertex list has more vertices
-    tria_qualities()
-        Computes triangle quality for each triangle in mesh
-    boundary_loops()
-        Computes a tuple of boundary loops
-    centroid()
-        Computes centroid of triangle mesh as a weighted average of triangle centers
-    edges(with_boundary=False)
-        Compute vertices and adjacent triangle ids for each edge
-    curvature(smoothit=3)
-        Compute various curvature values at vertices.
-    curvature_tria(smoothit=3)
-        Compute min and max curvature and directions
-    normalize_()
-        Normalizes TriaMesh to unit surface area
-    rm_free_vertices_()
-        Remove unused (free) vertices from v and t
-    refine_(it=1)
-        Refines the triangle mesh
-    normal_offset_(d)
-        moves vertices along normal by distance d
-    orient_()
-        re-orients triangles of manifold mesh to be consistent
-    map_tfunc_to_vfunc(tfunc, weighted=False)
-        Maps function for each tria to each vertex
-    map_vfunc_to_tfunc(vfunc)
-        Maps function for each vertex to each triangle
-    smooth_vfunc(vfunc, n=1):
-        Smoothes vector float function on the mesh iteratively
-    smooth_(n=1)
-        Smoothes mesh in place for a number of iterations
+        List of lists of 3 int of indices (>= 0) into ``v`` array.
+    adj_sym : csc_matrix
+        Symmetric adjacency matrix as csc sparse matrix.
+    adj_dir : csc_matrix
+        Directed adjacency matrix as csc sparse matrix.
+    fsinfo : dict | None
+        FreeSurfer Surface Header Info.
+
+    Notes
+    -----
+    The class has static class methods to read triangle meshes from FreeSurfer,
+    OFF, and VTK file formats.
     """
 
     def __init__(self, v, t, fsinfo=None):
-        """Constructor
-
-        Parameters
-        ----------
-        v : array_like
-            List of lists of 3 float coordinates
-        t : array_like
-            List of lists of 3 int of indices (>=0) into v array
-            Ordering is important: All triangles should be
-            oriented the same way (counter-clockwise, when
-            looking from above)
-        fsinfo : dict, Default=None
-            FreeSurfer Surface Header Info
-
-        Raises
-        -------
-        ValueError
-            Max index exceeds number of vertices
-        ValurError
-            Triangles should have 3 vertices
-        ValueError
-            Vertices should have 3 coordinates
-        """
-
         self.v = np.array(v)
         self.t = np.array(t)
         # transpose if necessary
         if self.v.shape[0] < self.v.shape[1]:
             self.v = self.v.T
         if self.t.shape[0] < self.t.shape[1]:
             self.t = self.t.T
@@ -137,87 +60,144 @@
         if self.v.shape[1] != 3:
             raise ValueError("Vertices should have 3 coordinates")
         # Compute adjacency matrices
         self.adj_sym = self._construct_adj_sym()
         self.adj_dir = self._construct_adj_dir()
         self.fsinfo = fsinfo  # place for Freesurfer Header info
 
-    def _construct_adj_sym(self):
+    @classmethod
+    def read_fssurf(cls, filename):
+        """Load triangle mesh from FreeSurfer surface geometry file.
+
+        Parameters
+        ----------
+        filename : str
+            Filename to load.
+
+        Returns
+        -------
+        TriaMesh
+            Loaded triangle mesh.
+        """
+        return io.read_fssurf(filename)
+
+    @classmethod
+    def read_off(cls, filename):
+        """Load triangle mesh from OFF txt file.
+
+        Parameters
+        ----------
+        filename : str
+            Filename to load.
+
+        Returns
+        -------
+        TriaMesh
+            Loaded triangle mesh.
+        """
+        return io.read_off(filename)
+
+    @classmethod
+    def read_vtk(cls, filename):
+        """Load triangle mesh from VTK txt file.
+
+        Parameters
+        ----------
+        filename : str
+            Filename to load.
+
+        Returns
+        -------
+        TriaMesh
+            Loaded triangle mesh.
+        """
+        return io.read_vtk(filename)
+
+    def write_vtk(self, filename):
+        """Save as VTK file.
+
+        Parameters
+        ----------
+        filename : str
+            Filename to save to.
         """
-        Constructs symmetric adjacency matrix (edge graph) of triangle mesh t
+        io.write_vtk(self, filename)
+
+    def write_fssurf(self, filename):
+        """Save as Freesurfer Surface Geometry file (wrap Nibabel).
+
+        Parameters
+        ----------
+        filename : str
+            Filename to save to.
+        """
+        io.write_fssurf(self, filename)
+
+    def _construct_adj_sym(self):
+        """Construct symmetric adjacency matrix (edge graph) of triangle mesh.
+
         Operates only on triangles.
 
         Returns
         -------
-        scipy.sparse.csc_matrix
-            Sparse symmetric CSC matrix
+        csc_matrix
             The non-directed adjacency matrix
             will be symmetric. Each inner edge (i,j) will have
             the number of triangles that contain this edge.
             Inner edges usually 2, boundary edges 1. Higher
             numbers can occur when there are non-manifold triangles.
             The sparse matrix can be binarized via:
-            adj.data = np.ones(adj.data.shape)
+            adj.data = np.ones(adj.data.shape).
         """
-
         t0 = self.t[:, 0]
         t1 = self.t[:, 1]
         t2 = self.t[:, 2]
         i = np.column_stack((t0, t1, t1, t2, t2, t0)).reshape(-1)
         j = np.column_stack((t1, t0, t2, t1, t0, t2)).reshape(-1)
         dat = np.ones(i.shape)
         n = self.v.shape[0]
         return sparse.csc_matrix((dat, (i, j)), shape=(n, n))
 
     def _construct_adj_dir(self):
-        """
-        Constructs directed adjacency matrix (edge graph) of triangle mesh t
+        """Construct directed adjacency matrix (edge graph) of triangle mesh.
+
         Operates only on triangles.
 
         Returns
         -------
-        scipy.sparse.csc_matrix
-            Sparse CSC matrix
+        csc_matrix
             The directed adjacency matrix is not symmetric if
             boundaries exist or if mesh is non-manifold.
             For manifold meshes, there are only entries with
             value 1. Symmetric entries are inner edges. Non-symmetric
             are boundary edges. The direction prescribes a direction
             on the boundary loops. Adding the matrix to its transpose
             creates the non-directed version.
         """
-
         t0 = self.t[:, 0]
         t1 = self.t[:, 1]
         t2 = self.t[:, 2]
         i = np.column_stack((t0, t1, t2)).reshape(-1)
         j = np.column_stack((t1, t2, t0)).reshape(-1)
         dat = np.ones(i.shape)
         n = self.v.shape[0]
         return sparse.csc_matrix((dat, (i, j)), shape=(n, n))
 
     def construct_adj_dir_tidx(self):
-        """
-        Constructs directed adjacency matrix (edge graph) of triangle mesh t
-        containing the triangle indices (only for non-manifold meshes)
-        Operates only on triangles.
+        """Construct directed adjacency matrix (edge graph) of triangle mesh.
+
+        The directed adjacency matrix contains the triangle indices (only for
+        non-manifold meshes). Operates only on triangles.
 
         Returns
         -------
-        scipy.sparse.csc_matrix
-            Sparse CSC matrix
+        csc_matrix
             Similar to adj_dir, but stores the tria idx+1 instead
             of one in the matrix (allows lookup of vertex to tria).
-
-        Raises
-        -------
-        ValueError
-            Can only tidx matrix for oriented triangle meshes!
         """
-
         if not self.is_oriented():
             raise ValueError(
                 "Error: Can only tidx matrix for oriented triangle meshes!"
             )
         t0 = self.t[:, 0]
         t1 = self.t[:, 1]
         t2 = self.t[:, 2]
@@ -225,121 +205,112 @@
         j = np.column_stack((t1, t2, t0)).reshape(-1)
         # store tria idx +1  (zero means no edge here)
         dat = np.repeat(np.arange(1, self.t.shape[0] + 1), 3)
         n = self.v.shape[0]
         return sparse.csc_matrix((dat, (i, j)), shape=(n, n))
 
     def is_closed(self):
-        """
-        Check if triangle mesh is closed (no boundary edges)
+        """Check if triangle mesh is closed (no boundary edges).
+
         Operates only on triangles
 
         Returns
         -------
         bool
-            True if no boundary edges in adj matrix
+            True if no boundary edges in adj matrix.
         """
-
         return 1 not in self.adj_sym.data
 
     def is_manifold(self):
-        """
-        Check if triangle mesh is manifold (no edges with >2 triangles)
+        """Check if triangle mesh is manifold (no edges with >2 triangles).
+
         Operates only on triangles
 
         Returns
         -------
-        bool:
-            True if no edges with > 2 triangles
+        bool
+            True if no edges with > 2 triangles.
         """
-
         return np.max(self.adj_sym.data) <= 2
 
     def is_oriented(self):
-        """
-        Check if triangle mesh is oriented. True if all triangles are oriented
-        counter-clockwise, when looking from above.
-        Operates only on triangles
+        """Check if triangle mesh is oriented.
+
+        True if all triangles are oriented counter-clockwise, when looking from
+        above. Operates only on triangles.
 
         Returns
         -------
         bool
-            True if max(adj_directed)=1
+            True if ``max(adj_directed)=1``.
         """
-
         return np.max(self.adj_dir.data) == 1
 
     def euler(self):
-        """
-        Computes the Euler Characteristic (=#V-#E+#T)
-        Operates only on triangles
+        """Compute the Euler Characteristic.
+
+        The Euler characteristic is the number of vertices minus the number
+        of edges plus the number of triangles  (= #V - #E + #T). For example,
+        it is 2 for the sphere and 0 for the torus.
+        This operates only on triangles array.
 
         Returns
         -------
         int
-            Euler Characteristic (2=sphere,0=torus)
+            Euler characteristic.
         """
-
         # v can contain unused vertices so we get vnum from trias
         vnum = len(np.unique(self.t.reshape(-1)))
         tnum = np.max(self.t.shape)
         enum = int(self.adj_sym.nnz / 2)
         return vnum - enum + tnum
 
     def tria_areas(self):
-        """
-        Computes the area of triangles using Heron's formula
+        """Compute the area of triangles using Heron's formula.
+
+        `Heron's formula <https://en.wikipedia.org/wiki/Heron%27s_formula>`_
+        computes the area of a triangle by using the three edge lengths.
 
         Returns
         -------
-        areas : np.ndarray
-            array with areas of each triangle
+        areas : array
+            Array with areas of each triangle.
         """
-
         v0 = self.v[self.t[:, 0], :]
         v1 = self.v[self.t[:, 1], :]
         v2 = self.v[self.t[:, 2], :]
         v1mv0 = v1 - v0
         v2mv1 = v2 - v1
         v0mv2 = v0 - v2
         a = np.sqrt(np.sum(v1mv0 * v1mv0, axis=1))
         b = np.sqrt(np.sum(v2mv1 * v2mv1, axis=1))
         c = np.sqrt(np.sum(v0mv2 * v0mv2, axis=1))
         ph = 0.5 * (a + b + c)
         areas = np.sqrt(ph * (ph - a) * (ph - b) * (ph - c))
         return areas
 
     def area(self):
-        """
-        Computes the total surface area of triangle mesh
+        """Compute the total surface area of triangle mesh.
 
         Returns
         -------
         float
-            Total surface area
+            Total surface area.
         """
-
         areas = self.tria_areas()
         return np.sum(areas)
 
     def volume(self):
-        """
-        Computes the volume of closed triangle mesh, summing tetrahedra at origin
+        """Compute the volume of closed triangle mesh, summing tetrahedra at origin.
 
         Returns
         -------
         vol : float
-            Total enclosed volume
-
-        Raises
-        -------
-        ValueError
-            can only compute volume for oriented triangle meshes
+            Total enclosed volume.
         """
-
         if not self.is_closed():
             return 0.0
         if not self.is_oriented():
             raise ValueError(
                 "Error: Can only compute volume for oriented triangle meshes!"
             )
         v0 = self.v[self.t[:, 0], :]
@@ -349,78 +320,69 @@
         v2mv0 = v2 - v0
         cr = np.cross(v1mv0, v2mv0)
         spatvol = np.sum(v0 * cr, axis=1)
         vol = np.sum(spatvol) / 6.0
         return vol
 
     def vertex_degrees(self):
-        """
-        Computes the vertex degrees (number of edges at each vertex)
+        """Compute the vertex degrees (number of edges at each vertex).
 
         Returns
         -------
-        vdeg : np.ndarray
-            Array of vertex degrees
+        vdeg : array
+            Array of vertex degrees.
         """
-
         vdeg = np.bincount(self.t.reshape(-1))
         return vdeg
 
     def vertex_areas(self):
-        """
-        Computes the area associated to each vertex (1/3 of one-ring trias)
+        """Compute the area associated to each vertex (1/3 of one-ring trias).
 
         Returns
         -------
-        vareas : np.ndarray
-            Array of vertex areas
+        vareas : array
+            Array of vertex areas.
         """
-
         v0 = self.v[self.t[:, 0], :]
         v1 = self.v[self.t[:, 1], :]
         v2 = self.v[self.t[:, 2], :]
         v1mv0 = v1 - v0
         v2mv0 = v2 - v0
         cr = np.cross(v1mv0, v2mv0)
         area = 0.5 * np.sqrt(np.sum(cr * cr, axis=1))
         area3 = np.repeat(area[:, np.newaxis], 3, 1)
         # varea = accumarray(t(:),area3(:))./3;
         vareas = np.bincount(self.t.reshape(-1), area3.reshape(-1)) / 3.0
         return vareas
 
     def avg_edge_length(self):
-        """
-        Computes the average edge length of the mesh
+        """Compute the average edge length of the mesh.
 
         Returns
         -------
         float
-            Avg. edge length
+            Average edge length.
         """
-
         # get only upper off-diag elements from symmetric adj matrix
         triadj = sparse.triu(self.adj_sym, 1, format="coo")
         edgelens = np.sqrt(
             ((self.v[triadj.row, :] - self.v[triadj.col, :]) ** 2).sum(1)
         )
         return edgelens.mean()
 
     def tria_normals(self):
-        """
-        Computes triangle normals
-        Ordering of trias is important: counterclockwise when looking
+        """Compute triangle normals.
+
+        Ordering of triangles is important: counterclockwise when looking.
 
         Returns
         -------
-        n : np.ndarray
-            normals (num triangles X 3 )
+        n : array of shape (n_triangles, 3)
+            Triangle normals.
         """
-
-        import sys
-
         # Compute vertex coordinates and a difference vectors for each triangle:
         v0 = self.v[self.t[:, 0], :]
         v1 = self.v[self.t[:, 1], :]
         v2 = self.v[self.t[:, 2], :]
         v1mv0 = v1 - v0
         v2mv0 = v2 - v0
         # Compute cross product
@@ -431,32 +393,27 @@
         # lni = np.divide(1.0, ln)
         # n[:, 0] *= lni
         # n[:, 1] *= lni
         # n[:, 2] *= lni
         return n
 
     def vertex_normals(self):
-        """
+        """Compute vertex normals.
+
         get_vertex_normals(v,t) computes vertex normals
             Triangle normals around each vertex are averaged, weighted
             by the angle that they contribute.
             Ordering is important: counterclockwise when looking
             at the triangle from above.
 
         Returns
         -------
-        n : np.ndarray
-            normals (num triangles X 3 )
-
-        Raises
-        -------
-        ValueError
-            Vertex normals are meaningless for un-oriented triangle meshes!
+        n : array of shape (n_triangles, 3)
+            Vertex normals.
         """
-
         if not self.is_oriented():
             raise ValueError(
                 "Error: Vertex normals are meaningless for un-oriented triangle meshes!"
             )
         import sys
 
         # Compute vertex coordinates and a difference vector for each triangle:
@@ -484,42 +441,42 @@
         # lni = np.divide(1.0, ln)
         # n[:, 0] *= lni
         # n[:, 1] *= lni
         # n[:, 2] *= lni
         return n
 
     def has_free_vertices(self):
-        """
-        Checks if the vertex list has more vertices than what is used in tria
+        """Check if the vertex list has more vertices than what is used in tria.
 
         Returns
         -------
         bool
-            whether vertex list has more vertices or not
+            Whether vertex list has more vertices or not.
         """
-
         vnum = np.max(self.v.shape)
         vnumt = len(np.unique(self.t.reshape(-1)))
         return vnum != vnumt
 
     def tria_qualities(self):
-        """
-        Computes triangle quality for each triangle in mesh where
+        """Compute triangle quality for each triangle in mesh where.
+
         q = 4 sqrt(3) A / (e1^2 + e2^2 + e3^2 )
         where A is the triangle area and ei the edge length of the three edges.
-        This measure is used by FEMLAB and can also be found in:
-            R.E. Bank, PLTMG ..., Frontiers in Appl. Math. (7), 1990.
         Constants are chosen so that q=1 for the equilateral triangle.
 
+        .. note::
+
+            This measure is used by FEMLAB and can also be found in:
+            R.E. Bank, PLTMG ..., Frontiers in Appl. Math. (7), 1990.
+
         Returns
         -------
-        np.ndarray
-            Array with triangle qualities
+        array
+            Array with triangle qualities.
         """
-
         # Compute vertex coordinates and a difference vectors for each triangle:
         v0 = self.v[self.t[:, 0], :]
         v1 = self.v[self.t[:, 1], :]
         v2 = self.v[self.t[:, 2], :]
         v1mv0 = v1 - v0
         v2mv1 = v2 - v1
         v0mv2 = v0 - v2
@@ -528,32 +485,26 @@
         # compute length (2*area)
         ln = np.sqrt(np.sum(n * n, axis=1))
         q = 2.0 * np.sqrt(3) * ln
         es = (v1mv0 * v1mv0).sum(1) + (v2mv1 * v2mv1).sum(1) + (v0mv2 * v0mv2).sum(1)
         return q / es
 
     def boundary_loops(self):
-        """
-        Computes a tuple of boundary loops. Meshes can have 0 or more boundary
-        loops, which are cycles in the directed adjacency graph of the boundary
-        edges.
+        """Compute a tuple of boundary loops.
+
+        Meshes can have 0 or more boundary loops, which are cycles in the directed
+        adjacency graph of the boundary edges.
         Works on trias only. Could fail if loops are connected via a single
         vertex (like a figure 8). That case needs debugging.
 
         Returns
         -------
-        loops : np.ndarray
-            List of lists with boundary loops
-
-        Raises
-        -------
-        ValueError
-            tria not manifold (edges with more than 2 triangles)!
+        loops : list of list
+            List of lists with boundary loops.
         """
-
         if not self.is_manifold():
             raise ValueError(
                 "Error: tria not manifold (edges with more than 2 triangles)!"
             )
         if self.is_closed():
             return []
         # get directed matrix of only boundary edges
@@ -587,29 +538,28 @@
             if len(nz) > 0:
                 firstcol = nz[0] - 1
             else:
                 firstcol = []
         return loops
 
     def centroid(self):
-        """
-        Computes centroid of triangle mesh as a weighted average of triangle
-        centers. The weight is determined by the triangle area.
+        """Compute centroid of triangle mesh as a weighted average of triangle centers.
+
+        The weight is determined by the triangle area.
         (This could be done much faster if a FEM lumped mass matrix M is
         already available where this would be M*v, because it is equivalent
         with averaging vertices weighted by vertex area)
 
         Returns
         -------
         centroid : float
-            The centroid of the mesh
+            The centroid of the mesh.
         totalarea : float
-            he total area of the mesh
+            The total area of the mesh.
         """
-
         v0 = self.v[self.t[:, 0], :]
         v1 = self.v[self.t[:, 1], :]
         v2 = self.v[self.t[:, 2], :]
         v2mv1 = v2 - v1
         v0mv2 = v0 - v2
         # Compute cross product and area for each triangle:
         cr = np.cross(v2mv1, v0mv2)
@@ -617,43 +567,36 @@
         totalarea = areas.sum()
         areas = areas / totalarea
         centers = (1.0 / 3.0) * (v0 + v1 + v2)
         c = centers * areas[:, np.newaxis]
         return np.sum(c, axis=0), totalarea
 
     def edges(self, with_boundary=False):
-        """
-        Compute vertices and adjacent triangle ids for each edge
+        """Compute vertices and adjacent triangle ids for each edge.
 
         Parameters
         ----------
-        with_boundary : bool, Default=False
-            also work on boundary half edges, default ignore
+        with_boundary : bool
+            Also work on boundary half edges, default ignore.
 
         Returns
         -------
-        vids : np.ndarray
-            column array with starting and end vertex for each unique inner edge
-        tids : np.ndarray
+        vids : array
+            Column array with starting and end vertex for each unique inner edge.
+        tids : array
             2 column array with triangle containing the half edge
             from vids[0,:] to vids [1,:] in first column and the
-            neighboring triangle in the second column
-        bdrvids : np.ndarray
-            if with_boundary is true: 2 column array with each
-            boundary half-edge
-        bdrtids : np.ndarray
-            if with_boundary is true: 1 column array with the
-            associated triangle to each boundary edge
-
-        Raises
-        -------
-        ValueError
-            Error: Can only compute edge information for oriented meshes!
+            neighboring triangle in the second column.
+        bdrvids : array
+            If with_boundary is true: 2 column array with each
+            boundary half-edge.
+        bdrtids : array
+            If with_boundary is true: 1 column array with the
+            associated triangle to each boundary edge.
         """
-
         if not self.is_oriented():
             raise ValueError(
                 "Error: Can only compute edge information for oriented meshes!"
             )
         adjtria = self.construct_adj_dir_tidx().tolil()
         # for boundary edges, we can just remove those edges (implicitly a zero angle)
         bdredges = []
@@ -675,49 +618,48 @@
         bdrv = np.array(np.nonzero(bdredges)).T
         nzids = bdrtrias > -1
         bdrv = bdrv[nzids, :]
         bdrtrias = bdrtrias[nzids].reshape(-1, 1)
         return vids, tids, bdrv, bdrtrias
 
     def curvature(self, smoothit=3):
-        """
-        Compute various curvature values at vertices.
+        """Compute various curvature values at vertices.
+
+        .. note::
 
-        For the algorithm see e.g.
-        Pierre Alliez, David Cohen-Steiner, Olivier Devillers,
-        Bruno Levy, and Mathieu Desbrun.
-        Anisotropic Polygonal Remeshing.
-        ACM Transactions on Graphics, 2003.
+            For the algorithm see e.g.
+            Pierre Alliez, David Cohen-Steiner, Olivier Devillers,
+            Bruno Levy, and Mathieu Desbrun.
+            Anisotropic Polygonal Remeshing.
+            ACM Transactions on Graphics, 2003.
 
         Parameters
         ----------
-        smoothit : int, Default=3
-            smoothing iterations on vertex functions
+        smoothit : int
+            Smoothing iterations on vertex functions.
 
         Returns
         -------
-        u_min : np.ndarray
-            minimal curvature directions (vnum x 3)
-        u_max : np.ndarray
-             maximal curvature directions (vnum x 3)
-        c_min : np.ndarray
-             minimal curvature
-        c_max : np.ndarray
-             maximal curvature
-        c_mean : np.ndarray
-            mean curvature: (c_min + c_max) / 2.0
-        c_gauss : np.ndarray
-           Gauss curvature: c_min * c_max
-        normals : np.ndarray
-           normals (vnum x 3)
+        u_min : array of shape (vnum, 3)
+            Minimal curvature directions.
+        u_max : array of shape (vnum, 3)
+            Maximal curvature directions.
+        c_min : array
+            Minimal curvature.
+        c_max : array
+            Maximal curvature.
+        c_mean : array
+            Mean curvature ``(c_min + c_max) / 2.0m``.
+        c_gauss : array
+           Gauss curvature ``c_min * c_maxm``.
+        normals : array of shape (vnum, 3)
+           Normals.
         """
-
         # import warnings
         # warnings.filterwarnings('error')
-        import sys
 
         # get edge information for inner edges (vertex ids and tria ids):
         vids, tids = self.edges()
         # compute normals for each tria
         tnormals = self.tria_normals()
         # compute dot product of normals at each edge
         sprod = np.sum(tnormals[tids[:, 0], :] * tnormals[tids[:, 1], :], axis=1)
@@ -806,37 +748,36 @@
         u_cross = np.cross(u_min, u_max)
         d = np.sum(np.multiply(u_cross, normals), axis=1)
         i = np.squeeze(np.where(d < 0))
         u_max[i, :] = -u_max[i, :]
         return u_min, u_max, c_min, c_max, c_mean, c_gauss, normals
 
     def curvature_tria(self, smoothit=3):
-        """
-        Compute min and max curvature and directions (orthogonal and in tria plane)
-        for each triangle. First we compute these values on vertices and then smooth
+        """Compute min and max curvature and directions (orthogonal and in tria plane).
+
+        First we compute these values on vertices and then smooth
         there. Finally they get mapped to the trias (averaging) and projected onto
         the triangle plane, and orthogonalized.
 
         Parameters
         ----------
-        smoothit : int, Default=3
-            number of smoothing iterations for curvature computation on vertices
+        smoothit : int
+            Number of smoothing iterations for curvature computation on vertices.
 
         Returns
         -------
-        u_min : np.ndarray
-            min curvature direction on triangles
-        u_max : np.ndarray
-            max curvature direction on triangles
-        c_min : np.ndarray
-            min curvature on triangles
-        c_max : np.ndarray
-            max curvature on triangles
+        u_min : array
+            Min curvature direction on triangles.
+        u_max : array
+            Max curvature direction on triangles.
+        c_min : array
+            Min curvature on triangles.
+        c_max : array
+            Max curvature on triangles.
         """
-
         u_min, u_max, c_min, c_max, c_mean, c_gauss, normals = self.curvature(smoothit)
 
         # pool vertex functions (u_min and u_max) to triangles:
         tumin = self.map_vfunc_to_tfunc(u_min)
         # tumax = self.map_vfunc_to_tfunc(u_max)
         tcmin = self.map_vfunc_to_tfunc(c_min)
         tcmax = self.map_vfunc_to_tfunc(c_max)
@@ -868,42 +809,36 @@
         # tumax3 = np.sign(np.sum(np.cross(tumin, tumax) * tn, axis=1)).reshape(-1, 1)
         #           * tumax2
         # I wonder how much changes, if we first map umax to tria and then
         #   find orthogonal umin next?
         return tumin2, tumax2, tcmin, tcmax
 
     def normalize_(self):
-        """
-        Normalizes TriaMesh to unit surface area with a centroid at the origin.
+        """Normalize TriaMesh to unit surface area and centroid at the origin.
+
         Modifies the vertices.
         """
         centroid, area = self.centroid()
         self.v = (1.0 / np.sqrt(area)) * (self.v - centroid)
 
     def rm_free_vertices_(self):
-        """
-        Remove unused (free) vertices from v and t. These are vertices that are not
-        used in any triangle. They can produce problems when constructing, e.g.,
-        Laplace matrices.
+        """Remove unused (free) vertices.
+
+        Free vertices are vertices that are not used in any triangle.
+        They can produce problems when constructing, e.g., Laplace matrices.
 
         Will update v and t in mesh.
 
         Returns
         -------
-        vkeep : np.ndarray
-            Indices (from original list) of kept vertices
-        vdel : np.ndarray
-            Indices of deleted (unused) vertices
-
-        Raises
-        ------
-        Value Error
-            Max index exceeds number of vertices
+        vkeep : array
+            Indices (from original list) of kept vertices.
+        vdel : array
+            Indices of deleted (unused) vertices.
         """
-
         tflat = self.t.reshape(-1)
         vnum = np.max(self.v.shape)
         if np.max(tflat) >= vnum:
             raise ValueError("Max index exceeds number of vertices")
         # determine which vertices to keep
         vkeep = np.full(vnum, False, dtype=bool)
         vkeep[tflat] = True
@@ -921,25 +856,24 @@
         # convert vkeep to index list
         vkeep = np.nonzero(vkeep)[0]
         # set new vertices and tria and re-init adj matrices
         self.__init__(vnew, tnew)
         return vkeep, vdel
 
     def refine_(self, it=1):
-        """
-        Refines the triangle mesh by placing new vertex on each edge midpoint
-        and thus creating 4 similar triangles from one parent triangle.
-        Modifies mesh in place
+        """Refine the triangle mesh by placing new vertex on each edge midpoint.
+
+        Thus creates 4 similar triangles from one parent triangle.
+        Modifies mesh in place.
 
         Parameters
         ----------
-        it : int, default=1
-            number of iterations
+        it : int
+            Number of iterations.
         """
-
         for x in range(it):
             # make symmetric adj matrix to upper triangle
             adjtriu = sparse.triu(self.adj_sym, 0, format="csr")
             # create new vertex index for each edge
             edgeno = adjtriu.data.shape[0]
             vno = self.v.shape[0]
             adjtriu.data = np.arange(vno, vno + edgeno)
@@ -958,54 +892,50 @@
             t3 = np.column_stack((self.t[:, 2], e3, e2))
             t4 = np.column_stack((e1, e2, e3))
             tnew = np.reshape(np.concatenate((t1, t2, t3, t4), axis=1), (-1, 3))
             # set new vertices and tria and re-init adj matrices
             self.__init__(vnew, tnew)
 
     def normal_offset_(self, d):
-        """
+        """Move vertices along normal by distance ``d``.
+
         normal_offset(d) moves vertices along normal by distance d
 
         Parameters
         ----------
-        d : int or np.ndarray
-            move distance
+        d : int | array
+            Move distance.
         """
-
         n = self.vertex_normals()
         vn = self.v + d * n
         self.v = vn
         # no need to re-init, only changed vertices
 
     def orient_(self):
-        """
-        orient_ re-orients triangles of manifold mesh to be consistent, so that vertices
-        are listed counter-clockwise, when looking from above (outside).
+        """Re-orient triangles of manifold mesh to be consistent.
+
+        Re-orients triangles of manifold mesh to be consistent, so that vertices are
+        listed counter-clockwise, when looking from above (outside).
 
         Algorithm:
-        1. Construct list for each half-edge with its triangle and edge direction
-        2. Drop boundary half-edges and find half-edge pairs
-        3. Construct sparse matrix with triangle neighbors, with entry 1 for opposite
-            half edges and -1 for parallel half-edges (normal flip across this edge)
-        4. Flood mesh from first tria using triangle neighbor matrix
-            - keeping track of sign
-        5. When flooded, negative sign for a triangle indicates it needs to be flipped
-        6. If global volume is negative, flip everything (first tria was wrong)
+
+        * Construct list for each half-edge with its triangle and edge direction
+        * Drop boundary half-edges and find half-edge pairs
+        * Construct sparse matrix with triangle neighbors, with entry 1 for opposite
+          half edges and -1 for parallel half-edges (normal flip across this edge)
+        * Flood mesh from first tria using triangle neighbor matrix and keeping track of
+          sign
+        * When flooded, negative sign for a triangle indicates it needs to be flipped
+        * If global volume is negative, flip everything (first tria was wrong)
 
         Returns
         -------
         flipped : int
-            number of trias flipped
-
-        Raises
-        ------
-        ValueError
-            Without boundary edges, all should have two triangles!
+            Number of trias flipped.
         """
-
         tnew = self.t
         flipped = 0
         if not self.is_oriented():
             # get half edges
             t0 = self.t[:, 0]
             t1 = self.t[:, 1]
             t2 = self.t[:, 2]
@@ -1082,41 +1012,35 @@
         if self.volume() < 0:
             tnew[:, [1, 2]] = tnew[:, [2, 1]]
             self.__init__(self.v, tnew)
             flipped = tnew.shape[0] - flipped
         return flipped
 
     def map_tfunc_to_vfunc(self, tfunc, weighted=False):
-        """
-        Maps function for each tria to each vertex by attributing 1/3 to each
+        """Map tria function to vertices by attributing 1/3 to each vertex of triangle.
+
         Uses vertices and trias.
 
         Parameters
         ----------
-        tfunc : np.ndarray
-            Float vector or matrix (#t x N) of values at vertices
+        tfunc : array
+            Float vector or matrix (#t x N) of values at vertices.
         weighted : bool, default=False
             False, weigh only by 1/3, e.g. to compute
             vertex areas from tria areas
             True, weigh by triangle area / 3, e.g. to
             integrate a function defined on the trias,
             for example integrating the "one" function
             will also yield the vertex areas.
 
         Returns
         -------
-        vfunc : np.ndarray
-            Function on vertices vector or matrix (#v x N)
-
-        Raises
-        -------
-        ValueError
-            length of tfunc needs to match number of triangles
+        vfunc : array
+            Function on vertices vector or matrix (#v x N).
         """
-
         if self.t.shape[0] != tfunc.shape[0]:
             raise ValueError(
                 "Error: length of tfunc needs to match number of triangles"
             )
         tfunca = np.array(tfunc)
         # make sure tfunc is 2D (even with only 1-dim input)
         if tfunca.ndim == 1:
@@ -1127,57 +1051,49 @@
         vfunc = np.zeros((self.v.shape[0], tfunca.shape[1]))
         np.add.at(vfunc, self.t[:, 0], tfunca)
         np.add.at(vfunc, self.t[:, 1], tfunca)
         np.add.at(vfunc, self.t[:, 2], tfunca)
         return np.squeeze(vfunc / 3.0)
 
     def map_vfunc_to_tfunc(self, vfunc):
-        """
-        Maps function for each vertex to each triangle by attributing 1/3 to each
+        """Map vertex function to triangles by attributing 1/3 to each.
+
         Uses number of vertices and trias
 
         Parameters
         ----------
-        vfunc : np.ndarray
-            Float vector or matrix (#t x N) of values at vertices
+        vfunc : array
+            Float vector or matrix (#t x N) of values at vertices.
 
         Returns
         -------
-        tfunc
-            Function on trias vector or matrix (#t x N)
-
-        Raises
-        -------
-        ValueError
-            length of vfunc needs to match number of vertices
+        tfunc : array
+            Function on trias vector or matrix (#t x N).
         """
-
         if self.v.shape[0] != vfunc.shape[0]:
             raise ValueError("Error: length of vfunc needs to match number of vertices")
         vfunc = np.array(vfunc) / 3.0
         tfunc = np.sum(vfunc[self.t], axis=1)
         return tfunc
 
     def smooth_vfunc(self, vfunc, n=1):
-        """
-        Smoothes vector float function on the mesh iteratively
+        """Smooth the mesh or a vertex function iteratively.
 
         Parameters
         ----------
-        vfunc : no.ndarray
-            Float vector of values at vertices, if empty, use vertex coordinates
+        vfunc : array
+            Float vector of values at vertices, if empty, use vertex coordinates.
         n : int, default=1
-            Number of iterations for smoothing
+            Number of iterations for smoothing.
 
         Returns
         -------
-        vfunc : Function
-            Smoothed surface vertex function
+        vfunc : array
+            Smoothed surface vertex function.
         """
-
         if vfunc is None:
             vfunc = self.v
         vfunc = np.array(vfunc)
         if self.v.shape[0] != vfunc.shape[0]:
             raise ValueError("Error: length of vfunc needs to match number of vertices")
         areas = self.vertex_areas()[:, np.newaxis]
         adj = self.adj_sym.copy()
@@ -1192,19 +1108,17 @@
         # apply sparse matrix n times (fast in spite of loop)
         vout = adj2.dot(vfunc)
         for i in range(n - 1):
             vout = adj2.dot(vout)
         return vout
 
     def smooth_(self, n=1):
-        """
-        Smoothes mesh in place for a number of iterations
+        """Smooth the mesh iteratively in-place.
 
         Parameters
         ----------
-        n : int, default=1
-            smoothing iterations
+        n : int
+            Smoothing iterations.
         """
-
         vfunc = self.smooth_vfunc(self.v, n)
         self.v = vfunc
         return
```

### Comparing `lapy-0.6.0/lapy/read_geometry.py` & `lapy-1.0.0/lapy/_read_geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,8 @@
-# IMPORTS
-import warnings
-from collections import OrderedDict
-
-import numpy as np
-
-"""
-Read FreeSurfer geometry (fix for dev, ll 126-128);
+"""Read FreeSurfer geometry (fix for dev, ll 126-128).
 
 Code was taken from nibabel.freesurfer package
 (https://github.com/nipy/nibabel/blob/master/nibabel/freesurfer/io.py).
 This software is licensed under the following license:
 
 The MIT License
 
@@ -36,45 +29,50 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
+import warnings
+from collections import OrderedDict
+
+import numpy as np
+
 
 def _fread3(fobj):
-    """Read a 3-byte int from an open binary file object
+    """Read a 3-byte int from an open binary file object.
+
     Parameters
     ----------
     fobj : file
         File descriptor
+
     Returns
     -------
     n : int
         A 3 byte int
     """
-
     b1, b2, b3 = np.fromfile(fobj, ">u1", 3)
     return (b1 << 16) + (b2 << 8) + b3
 
 
 def _read_volume_info(fobj):
-    """Helper for reading the footer from a surface file.
+    """Read the footer from a surface file.
 
     Parameters
     ----------
     fobj : file
         File descriptor
 
     Returns
     -------
-    volume_info: np.ndarray
+    volume_info : array
         Key-value pairs found in the file.
     """
-
     volume_info = OrderedDict()
     head = np.fromfile(fobj, ">i4", 1)
     if not np.array_equal(head, [20]):  # Read two bytes more
         head = np.concatenate([head, np.fromfile(fobj, ">i4", 2)])
         if not np.array_equal(head, [2, 0, 20]) and not np.array_equal(
             head, [2, 1, 20]
         ):
@@ -137,15 +135,14 @@
     volume_info : OrderedDict
         Returned only if `read_metadata` is True.  Key-value pairs found in the
         geometry file.
     create_stamp : str
         Returned only if `read_stamp` is True.  The comment added by the
         program that saved the file.
     """
-
     volume_info = OrderedDict()
 
     TRIANGLE_MAGIC = 16777214
 
     with open(filepath, "rb") as fobj:
         magic = _fread3(fobj)
```

### Comparing `lapy-0.6.0/lapy/utils/_config.py` & `lapy-1.0.0/lapy/utils/_config.py`

 * *Files identical despite different names*

### Comparing `lapy-0.6.0/lapy/utils/_imports.py` & `lapy-1.0.0/lapy/utils/_imports.py`

 * *Files identical despite different names*

### Comparing `lapy-0.6.0/lapy.egg-info/PKG-INFO` & `lapy-1.0.0/lapy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lapy
-Version: 0.6.0
+Version: 1.0.0
 Summary: A package for differential geometry on meshes (Laplace, FEM)
 Author-email: Martin Reuter <martin.reuter@dzne.de>
 Maintainer-email: Martin Reuter <martin.reuter@dzne.de>
 License: MIT License
         
         Copyright (c) 2020 Deep Medical Imaging Lab (PI Reuter)
         
@@ -22,16 +22,16 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: homepage, https://github.com/Deep-MI/LaPy
-Project-URL: documentation, https://github.com/Deep-MI/LaPy
+Project-URL: homepage, https://Deep-MI.github.io/LaPy/dev/index.html
+Project-URL: documentation, https://Deep-MI.github.io/LaPy/dev/index.html
 Project-URL: source, https://github.com/Deep-MI/LaPy
 Project-URL: tracker, https://github.com/Deep-MI/LaPy/issues
 Keywords: python,Laplace,FEM,ShapeDNA,BrainPrint,Triangle Mesh,Tetrahedra Mesh,Geodesics in Heat,Mean Curvature Flow
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -42,42 +42,47 @@
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: chol
+Provides-Extra: doc
 Provides-Extra: style
 Provides-Extra: test
 Provides-Extra: all
 Provides-Extra: full
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/lapy.svg)](https://pypi.org/project/lapy/)
 # LaPy
 
-LaPy is a package to compute spectral features (Laplace-Beltrami operator) on
-tetrahedral and triangle meshes. It is written purely in python 3 without
-sacrificing speed as almost all loops are vectorized, drawing upon efficient
-and sparse mesh data structures. It is basically a port of the C++ ShapeDNA
-project with extended differential geometry capabilities.
+LaPy is an open-source Python package for differential geometry on triangle
+and tetrahedra meshes. It includes an FEM solver to estimate the Laplace,
+Poisson or Heat equations. Further functionality includes the computations
+of gradients, divergence, mean-curvature flow, conformal mappings, 
+geodesics, ShapeDNA (Laplace spectra), and IO and plotting methods. 
+
+LaPy is written purely in Python 3 without sacrificing speed as almost all
+loops are vectorized, drawing upon efficient and sparse mesh data structures.
 
 ## Contents:
 
-- TriaMesh: a class for triangle meshes offering various operations, such as
+- **TriaMesh**: a class for triangle meshes offering various operations, such as
   fixing orientation, smoothing, curvature, boundary, quality, normals, and
-  various efficient mesh datastructure (edges, adjacency matrices)
-- TetMesh: a class for tetrahedral meshes (orientation, boundary ...)
-- TriaIO, TetIO: for both tets and trias from off, vtk, etc. formats
-- FuncIO: import/export vertex functions and eigenvector files
-- Solver: a class for linear FEM computation (Laplace stiffness and mass
+  various efficient mesh datastructures (edges, adjacency matrices). IO from
+  OFF, VTK and other formats.
+- **TetMesh**: a class for tetrahedral meshes (orientation, boundary, IO ...)
+- **Solver**: a class for linear FEM computation (Laplace stiffness and mass
   matrix, fast and sparse eigenvalue solver, anisotropic Laplace, Poisson)
-- DiffGeo: compute gradients, divergence, mean curvature flow, etc.
-- Heat: for heat kernel and diffusion
-- ShapeDNA: compute the ShapeDNA descriptor of surfaces and solids
-- Plot: functions for interactive visualization (wrapping plotly)
+- **io**: module for IO of vertex functions and eigenvector files
+- **diffgeo**: module for gradients, divergence, mean curvature flow, etc.
+- **heat**: module for heat kernel and diffusion
+- **shapedna**: module for the ShapeDNA descriptor of surfaces and solids
+- **plot**: module for interactive visualizations (wrapping plotly)
 
 ## Usage:
 
 The LaPy package is a comprehensive collection of scripts, so we refer to the
 'help' function and docstring of each module / function / class for usage info.
 For example:
 
@@ -88,43 +93,47 @@
 ```
 
 In the `examples` subdirectory, we provide several Jupyter notebooks that
 illustrate prototypical use cases of the toolbox.
 
 ## Installation:
 
-Use the following code to download, build and install a package from this
-repository into your local Python package directory:
+Use the following code to install the latest release of LaPy into your local
+Python package directory:
 
 `python3 -m pip install lapy`
 
 Use the following code to install the dev package in editable mode to a location of
 your choice:
 
 `python3 -m pip install --user --src /my/preferred/location --editable git+https://github.com/Deep-MI/Lapy.git#egg=lapy`
 
-Several functions, e.g. the Solver, require a sparse matrix decomposition, for which either the LU decomposition (from scipy sparse) or the faster Cholesky decomposition (from scikit-sparse cholmod) can be used. The default is to use the LU decomposition. If the parameter flag use_cholmod is True, the code will try to import cholmod from the scikit-sparse package. If this fails, an error will be thrown. If you would like to use cholmod, you need to install scikit-sparse separately. It cannot be listed among LaPy's dependencies as that causes errors with pip. scikit-sparse requires numpy and scipy to be installed separately beforehand.
+Several functions, e.g. the Solver, require a sparse matrix decomposition, for which either the LU decomposition (from scipy sparse, default) or the faster Cholesky decomposition (from scikit-sparse cholmod, recommended) can be used. If the parameter flag use_cholmod is True, the code will try to import cholmod from the scikit-sparse package. If this fails, an error will be thrown. If you would like to use cholmod, you need to install scikit-sparse separately, as pip currently cannot install it (conda can). scikit-sparse requires numpy and scipy to be installed separately beforehand.
+
+## API Documentation
+
+The API Documentation can be found at https://deep-mi.org/LaPy .
 
 ## References:
 
 If you use this software for a publication please cite both these papers:
 
-[1] Laplace-Beltrami spectra as 'Shape-DNA' of surfaces and solids. Reuter M, Wolter F-E, Peinecke N. Computer-Aided Design. 2006;38(4):342-366. http://dx.doi.org/10.1016/j.cad.2005.10.011
+**[1]** Laplace-Beltrami spectra as 'Shape-DNA' of surfaces and solids. Reuter M, Wolter F-E, Peinecke N. Computer-Aided Design. 2006;38(4):342-366. http://dx.doi.org/10.1016/j.cad.2005.10.011
 
-[2] BrainPrint: a discriminative characterization of brain morphology. Wachinger C, Golland P, Kremen W, Fischl B, Reuter M. Neuroimage. 2015;109:232-48. http://dx.doi.org/10.1016/j.neuroimage.2015.01.032 http://www.ncbi.nlm.nih.gov/pubmed/25613439
+**[2]** BrainPrint: a discriminative characterization of brain morphology. Wachinger C, Golland P, Kremen W, Fischl B, Reuter M. Neuroimage. 2015;109:232-48. http://dx.doi.org/10.1016/j.neuroimage.2015.01.032 http://www.ncbi.nlm.nih.gov/pubmed/25613439
 
-[1] introduces the FEM methods and the Laplace spectra for shape analysis, while [2] focusses on medical applications.
+Shape-DNA [1] introduces the FEM methods and the Laplace spectra for shape analysis, while BrainPrint [2] focusses on medical applications.
 
-For Geodesics please cite:
+For Geodesics please also cite:
 
 [3] Crane K, Weischedel C, Wardetzky M. Geodesics in heat: A new approach to computing distance based on heat flow. ACM Transactions on Graphics. https://doi.org/10.1145/2516971.2516977
 
 For non-singular mean curvature flow please cite:
 
 [4] Kazhdan M, Solomon J, Ben-Chen M. 2012. Can Mean-Curvature Flow be Modified to be Non-singular? Comput. Graph. Forum 31, 5, 1745–1754.
 https://doi.org/10.1111/j.1467-8659.2012.03179.x
 
 For conformal mapping please cite:
 
 [5] Choi PT, Lam KC, Lui LM. FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization for Genus-0 Closed Brain Surfaces. SIAM Journal on Imaging Sciences, vol. 8, no. 1, pp. 67-94, 2015. https://doi.org/10.1137/130950008
 
-We also invite you to check out our lab webpage at https://deep-mi.org
+We invite you to check out our lab webpage at https://deep-mi.org
```

### Comparing `lapy-0.6.0/pyproject.toml` & `lapy-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools >= 61.0.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'lapy'
-version = '0.6.0'
+version = '1.0.0'
 description = 'A package for differential geometry on meshes (Laplace, FEM)'
 readme = 'README.md'
 license = {file = 'LICENSE'}
 requires-python = '>=3.8'
 authors = [
     {name = 'Martin Reuter', email = 'martin.reuter@dzne.de'},
 ]
@@ -51,21 +51,33 @@
 build = [
     'build',
     'twine',
 ]
 chol = [
     'scikit-sparse',
 ]
+doc = [
+    'furo',
+    'matplotlib',
+    'memory-profiler',
+    'numpydoc',
+    'sphinx',
+    'sphinxcontrib-bibtex',
+    'sphinx-copybutton',
+    'sphinx-design',
+    'sphinx-gallery',
+    'sphinx-issues',
+]
 style = [
     'bibclean',
     'black',
     'codespell',
     'isort',
-    'flake8',
     'pydocstyle[toml]',
+    'ruff',
 ]
 test = [
     'pytest',
     'pytest-cov',
     'pytest-timeout',
 ]
 all = [
@@ -76,16 +88,16 @@
     'lapy[test]',
 ]
 full = [
     'lapy[all]',
 ]
 
 [project.urls]
-homepage = 'https://github.com/Deep-MI/LaPy'
-documentation = 'https://github.com/Deep-MI/LaPy'
+homepage = 'https://Deep-MI.github.io/LaPy/dev/index.html'
+documentation = 'https://Deep-MI.github.io/LaPy/dev/index.html'
 source = 'https://github.com/Deep-MI/LaPy'
 tracker = 'https://github.com/Deep-MI/LaPy/issues'
 
 [project.scripts]
 lapy-sys_info = 'lapy.commands.sys_info:run'
 
 [tool.setuptools]
@@ -98,39 +110,53 @@
 [tool.black]
 line-length = 88
 target-version = ['py38']
 include = '\.pyi?$'
 extend-exclude = '''
 (
       __pycache__
-    | \.github
+    | .github
     | setup.py
     | data/
+    | doc/
     | examples/
+    | tutorials/
 )
 '''
 
 [tool.isort]
 profile = 'black'
 multi_line_output = 3
 line_length = 88
 py_version = 38
 extend_skip_glob = [
     'setup.py',
     'data/*',
+    'doc/*',
     'examples/*',
+    'tutorials/*',
 ]
 
 [tool.pydocstyle]
 convention = 'numpy'
 ignore-decorators = '(copy_doc|property|.*setter|.*getter|pyqtSlot|Slot)'
 match = '^(?!setup|__init__|test_).*\.py'
 match-dir = '^lapy.*'
 add_ignore = 'D100,D104,D107'
 
+[tool.ruff]
+line-length = 88
+extend-exclude = [
+    "doc",
+    "setup.py",
+]
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = ["F401"]
+
 [tool.pytest.ini_options]
 minversion = '6.0'
 addopts = '--durations 20 --junit-xml=junit-results.xml --verbose'
 filterwarnings = []
 
 [tool.coverage.run]
 branch = true
```

