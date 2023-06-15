# Comparing `tmp/OApackage-2.7.7.tar.gz` & `tmp/OApackage-2.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OApackage-2.7.7.tar", last modified: Tue May 16 07:39:37 2023, max compression
+gzip compressed data, was "OApackage-2.7.8.tar", last modified: Wed Jun 14 21:33:23 2023, max compression
```

## Comparing `OApackage-2.7.7.tar` & `OApackage-2.7.8.tar`

### file list

```diff
@@ -1,454 +1,454 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.636482 OApackage-2.7.7/
--rw-rw-rw-   0        0        0       89 2023-05-16 07:33:53.000000 OApackage-2.7.7/CONTRIBUTORS.md
--rw-rw-rw-   0        0        0     2229 2023-05-16 07:33:53.000000 OApackage-2.7.7/LICENSE
--rw-rw-rw-   0        0        0      390 2023-05-16 07:33:53.000000 OApackage-2.7.7/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.379256 OApackage-2.7.7/OApackage.egg-info/
--rw-rw-rw-   0        0        0     4638 2023-05-16 07:39:37.000000 OApackage-2.7.7/OApackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13655 2023-05-16 07:39:37.000000 OApackage-2.7.7/OApackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 07:39:37.000000 OApackage-2.7.7/OApackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-16 07:37:48.000000 OApackage-2.7.7/OApackage.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      105 2023-05-16 07:39:37.000000 OApackage-2.7.7/OApackage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-05-16 07:39:37.000000 OApackage-2.7.7/OApackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4638 2023-05-16 07:39:37.652107 OApackage-2.7.7/PKG-INFO
--rw-rw-rw-   0        0        0     3610 2023-05-16 07:33:53.000000 OApackage-2.7.7/README.md
--rw-rw-rw-   0        0        0    34426 2023-05-16 07:33:54.000000 OApackage-2.7.7/doxy2swig.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.363316 OApackage-2.7.7/misc/
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.379256 OApackage-2.7.7/misc/scripts/
--rw-rw-rw-   0        0        0      767 2023-05-16 07:33:54.000000 OApackage-2.7.7/misc/scripts/example_oapackage_python.py
--rw-rw-rw-   0        0        0   105735 2023-05-16 07:33:54.000000 OApackage-2.7.7/numpy.i
--rw-rw-rw-   0        0        0       48 2023-05-16 07:33:54.000000 OApackage-2.7.7/oaconfig.txt
--rw-rw-rw-   0        0        0   144029 2023-05-16 07:33:54.000000 OApackage-2.7.7/oadoxy.i
--rw-rw-rw-   0        0        0    16256 2023-05-16 07:33:54.000000 OApackage-2.7.7/oalib.i
--rw-rw-rw-   0        0        0   421148 2023-05-16 07:35:59.000000 OApackage-2.7.7/oalib.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.394565 OApackage-2.7.7/oapackage/
--rw-rw-rw-   0        0        0    21582 2023-05-16 07:33:54.000000 OApackage-2.7.7/oapackage/Doptim.py
--rw-rw-rw-   0        0        0     2128 2023-05-16 07:33:54.000000 OApackage-2.7.7/oapackage/__init__.py
--rw-rw-rw-   0        0        0     5620 2023-05-16 07:33:54.000000 OApackage-2.7.7/oapackage/_scanf.py
--rw-rw-rw-   0        0        0     4150 2023-05-16 07:33:54.000000 OApackage-2.7.7/oapackage/conference.py
--rw-rw-rw-   0        0        0     3569 2023-05-16 07:33:54.000000 OApackage-2.7.7/oapackage/graphtools.py
--rw-rw-rw-   0        0        0    21493 2023-05-16 07:33:54.000000 OApackage-2.7.7/oapackage/markup.py
--rw-rw-rw-   0        0        0    38474 2023-05-16 07:33:54.000000 OApackage-2.7.7/oapackage/oahelper.py
--rw-rw-rw-   0        0        0      316 2023-05-16 07:33:54.000000 OApackage-2.7.7/oapackage/scanf.py
--rw-rw-rw-   0        0        0      839 2023-05-16 07:33:54.000000 OApackage-2.7.7/pyproject.toml
--rw-rw-rw-   0        0        0      187 2023-05-16 07:39:37.652107 OApackage-2.7.7/setup.cfg
--rw-rw-rw-   0        0        0    12267 2023-05-16 07:33:54.000000 OApackage-2.7.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.412303 OApackage-2.7.7/src/
--rw-rw-rw-   0        0        0    16020 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Deff.cpp
--rw-rw-rw-   0        0        0     3902 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Deff.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.441457 OApackage-2.7.7/src/Eigen/
--rw-rw-rw-   0        0        0      694 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/CMakeLists.txt
--rw-rw-rw-   0        0        0     1206 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/Cholesky
--rw-rw-rw-   0        0        0     1900 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/CholmodSupport
--rw-rw-rw-   0        0        0    17969 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/Core
--rw-rw-rw-   0        0        0      122 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/Dense
--rw-rw-rw-   0        0        0       35 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/Eigen
--rw-rw-rw-   0        0        0     1822 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/Eigenvalues
--rw-rw-rw-   0        0        0     2050 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/Geometry
--rw-rw-rw-   0        0        0      874 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/Householder
--rw-rw-rw-   0        0        0     2083 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/IterativeLinearSolvers
--rw-rw-rw-   0        0        0      939 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/Jacobi
--rw-rw-rw-   0        0        0     1433 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/LU
--rw-rw-rw-   0        0        0      991 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/MetisSupport
--rw-rw-rw-   0        0        0     2483 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/OrderingMethods
--rw-rw-rw-   0        0        0     1676 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/PaStiXSupport
--rw-rw-rw-   0        0        0     1116 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/PardisoSupport
--rw-rw-rw-   0        0        0     1317 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/QR
--rw-rw-rw-   0        0        0      945 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/QtAlignedMalloc
--rw-rw-rw-   0        0        0     1162 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/SPQRSupport
--rw-rw-rw-   0        0        0     1629 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/SVD
--rw-rw-rw-   0        0        0      919 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/Sparse
--rw-rw-rw-   0        0        0     1371 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/SparseCholesky
--rw-rw-rw-   0        0        0     2240 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/SparseCore
--rw-rw-rw-   0        0        0     1713 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/SparseLU
--rw-rw-rw-   0        0        0     1222 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/SparseQR
--rw-rw-rw-   0        0        0      797 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/StdDeque
--rw-rw-rw-   0        0        0      726 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/StdList
--rw-rw-rw-   0        0        0      803 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/StdVector
--rw-rw-rw-   0        0        0     2243 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/SuperLUSupport
--rw-rw-rw-   0        0        0     1382 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/UmfPackSupport
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.363316 OApackage-2.7.7/src/Eigen/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.441457 OApackage-2.7.7/src/Eigen/src/Cholesky/
--rw-rw-rw-   0        0        0    24440 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Cholesky/LDLT.h
--rw-rw-rw-   0        0        0    18395 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Cholesky/LLT.h
--rw-rw-rw-   0        0        0     3974 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.441457 OApackage-2.7.7/src/Eigen/src/CholmodSupport/
--rw-rw-rw-   0        0        0    22307 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.488316 OApackage-2.7.7/src/Eigen/src/Core/
--rw-rw-rw-   0        0        0    12218 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Array.h
--rw-rw-rw-   0        0        0     8179 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/ArrayBase.h
--rw-rw-rw-   0        0        0     6775 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/ArrayWrapper.h
--rw-rw-rw-   0        0        0     2720 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Assign.h
--rw-rw-rw-   0        0        0    38153 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/AssignEvaluator.h
--rw-rw-rw-   0        0        0    12479 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Assign_MKL.h
--rw-rw-rw-   0        0        0    13910 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/BandMatrix.h
--rw-rw-rw-   0        0        0    18064 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Block.h
--rw-rw-rw-   0        0        0     4249 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/BooleanRedux.h
--rw-rw-rw-   0        0        0     5689 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/CommaInitializer.h
--rw-rw-rw-   0        0        0     6970 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/ConditionEstimator.h
--rw-rw-rw-   0        0        0    62197 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/CoreEvaluators.h
--rw-rw-rw-   0        0        0     4525 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/CoreIterators.h
--rw-rw-rw-   0        0        0     7593 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/CwiseBinaryOp.h
--rw-rw-rw-   0        0        0    31424 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/CwiseNullaryOp.h
--rw-rw-rw-   0        0        0     8256 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/CwiseTernaryOp.h
--rw-rw-rw-   0        0        0     3877 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/CwiseUnaryOp.h
--rw-rw-rw-   0        0        0     5282 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/CwiseUnaryView.h
--rw-rw-rw-   0        0        0    27420 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/DenseBase.h
--rw-rw-rw-   0        0        0    24212 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/DenseCoeffsBase.h
--rw-rw-rw-   0        0        0    21959 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/DenseStorage.h
--rw-rw-rw-   0        0        0     9597 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Diagonal.h
--rw-rw-rw-   0        0        0    12666 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/DiagonalMatrix.h
--rw-rw-rw-   0        0        0      970 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/DiagonalProduct.h
--rw-rw-rw-   0        0        0    11507 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Dot.h
--rw-rw-rw-   0        0        0     5619 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/EigenBase.h
--rw-rw-rw-   0        0        0     4769 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/ForceAlignedAccess.h
--rw-rw-rw-   0        0        0     5705 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Fuzzy.h
--rw-rw-rw-   0        0        0    21123 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/GeneralProduct.h
--rw-rw-rw-   0        0        0    22185 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/GenericPacketMath.h
--rw-rw-rw-   0        0        0    10222 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/GlobalFunctions.h
--rw-rw-rw-   0        0        0     7076 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/IO.h
--rw-rw-rw-   0        0        0     3519 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Inverse.h
--rw-rw-rw-   0        0        0     7239 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Map.h
--rw-rw-rw-   0        0        0    10621 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/MapBase.h
--rw-rw-rw-   0        0        0    40402 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/MathFunctions.h
--rw-rw-rw-   0        0        0     3369 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/MathFunctionsImpl.h
--rw-rw-rw-   0        0        0    19170 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Matrix.h
--rw-rw-rw-   0        0        0    22154 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/MatrixBase.h
--rw-rw-rw-   0        0        0     3400 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/NestByValue.h
--rw-rw-rw-   0        0        0     3582 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/NoAlias.h
--rw-rw-rw-   0        0        0     9234 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/NumTraits.h
--rw-rw-rw-   0        0        0    21646 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/PermutationMatrix.h
--rw-rw-rw-   0        0        0    45180 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/PlainObjectBase.h
--rw-rw-rw-   0        0        0     7235 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Product.h
--rw-rw-rw-   0        0        0    49497 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/ProductEvaluators.h
--rw-rw-rw-   0        0        0     6379 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Random.h
--rw-rw-rw-   0        0        0    17852 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Redux.h
--rw-rw-rw-   0        0        0    12800 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Ref.h
--rw-rw-rw-   0        0        0     5595 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Replicate.h
--rw-rw-rw-   0        0        0     4200 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/ReturnByValue.h
--rw-rw-rw-   0        0        0     7073 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Reverse.h
--rw-rw-rw-   0        0        0     6020 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Select.h
--rw-rw-rw-   0        0        0    14245 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/SelfAdjointView.h
--rw-rw-rw-   0        0        0     1697 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-rw-rw-   0        0        0     6795 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Solve.h
--rw-rw-rw-   0        0        0     9031 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/SolveTriangular.h
--rw-rw-rw-   0        0        0     4365 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/SolverBase.h
--rw-rw-rw-   0        0        0     7692 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/StableNorm.h
--rw-rw-rw-   0        0        0     3865 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Stride.h
--rw-rw-rw-   0        0        0     2683 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Swap.h
--rw-rw-rw-   0        0        0    14777 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Transpose.h
--rw-rw-rw-   0        0        0    14386 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Transpositions.h
--rw-rw-rw-   0        0        0    37234 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/TriangularMatrix.h
--rw-rw-rw-   0        0        0     3462 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/VectorBlock.h
--rw-rw-rw-   0        0        0    29441 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/VectorwiseOp.h
--rw-rw-rw-   0        0        0     8074 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Visitor.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.363316 OApackage-2.7.7/src/Eigen/src/Core/arch/
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.488316 OApackage-2.7.7/src/Eigen/src/Core/arch/AVX/
--rw-rw-rw-   0        0        0    18037 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/AVX/Complex.h
--rw-rw-rw-   0        0        0    17776 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-rw-rw-   0        0        0    27787 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-rw-rw-   0        0        0     1194 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.488316 OApackage-2.7.7/src/Eigen/src/Core/arch/AVX512/
--rw-rw-rw-   0        0        0    15733 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-rw-rw-   0        0        0    50936 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/AVX512/PacketMath.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.488316 OApackage-2.7.7/src/Eigen/src/Core/arch/AltiVec/
--rw-rw-rw-   0        0        0    16443 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-rw-rw-   0        0        0    10797 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-rw-rw-   0        0        0    37671 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.488316 OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/
--rw-rw-rw-   0        0        0     4240 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/Complex.h
--rw-rw-rw-   0        0        0    22059 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/Half.h
--rw-rw-rw-   0        0        0     2387 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/MathFunctions.h
--rw-rw-rw-   0        0        0    10744 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/PacketMath.h
--rw-rw-rw-   0        0        0    35442 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
--rw-rw-rw-   0        0        0     5509 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/TypeCasting.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.488316 OApackage-2.7.7/src/Eigen/src/Core/arch/Default/
--rw-rw-rw-   0        0        0     1989 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-rw-rw-   0        0        0     1746 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/Default/Settings.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.503941 OApackage-2.7.7/src/Eigen/src/Core/arch/NEON/
--rw-rw-rw-   0        0        0    17706 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/NEON/Complex.h
--rw-rw-rw-   0        0        0     2846 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-rw-rw-   0        0        0    28726 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/NEON/PacketMath.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.503941 OApackage-2.7.7/src/Eigen/src/Core/arch/SSE/
--rw-rw-rw-   0        0        0    19426 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/SSE/Complex.h
--rw-rw-rw-   0        0        0    18888 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/SSE/MathFunctions.h
--rw-rw-rw-   0        0        0    35825 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-rw-rw-   0        0        0     1759 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.503941 OApackage-2.7.7/src/Eigen/src/Core/arch/ZVector/
--rw-rw-rw-   0        0        0    15366 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/ZVector/Complex.h
--rw-rw-rw-   0        0        0     4418 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rw-rw-rw-   0        0        0    32283 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.503941 OApackage-2.7.7/src/Eigen/src/Core/functors/
--rw-rw-rw-   0        0        0     6284 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-rw-rw-   0        0        0    18263 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/functors/BinaryFunctors.h
--rw-rw-rw-   0        0        0     8229 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/functors/NullaryFunctors.h
--rw-rw-rw-   0        0        0     4400 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/functors/StlFunctors.h
--rw-rw-rw-   0        0        0      607 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/functors/TernaryFunctors.h
--rw-rw-rw-   0        0        0    27944 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/functors/UnaryFunctors.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.519566 OApackage-2.7.7/src/Eigen/src/Core/products/
--rw-rw-rw-   0        0        0    81106 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-rw-rw-   0        0        0    18478 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-rw-rw-   0        0        0    15188 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-rw-rw-   0        0        0     6907 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-rw-rw-   0        0        0     5017 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-rw-rw-   0        0        0    26808 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-rw-rw-   0        0        0     6368 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-rw-rw-   0        0        0     4905 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/Parallelizer.h
--rw-rw-rw-   0        0        0    19632 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-rw-rw-   0        0        0    11198 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-rw-rw-   0        0        0     9901 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-rw-rw-   0        0        0     5209 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-rw-rw-   0        0        0     6105 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointProduct.h
--rw-rw-rw-   0        0        0     4066 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-rw-rw-   0        0        0    20403 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-rw-rw-   0        0        0    13743 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-rw-rw-   0        0        0    14722 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-rw-rw-   0        0        0    10571 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-rw-rw-   0        0        0    13979 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-rw-rw-   0        0        0     6513 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-rw-rw-   0        0        0     5741 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/TriangularSolverVector.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.527083 OApackage-2.7.7/src/Eigen/src/Core/util/
--rw-rw-rw-   0        0        0    15722 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/BlasUtil.h
--rw-rw-rw-   0        0        0    21579 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/Constants.h
--rw-rw-rw-   0        0        0     3564 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-rw-rw-   0        0        0    14150 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/ForwardDeclarations.h
--rw-rw-rw-   0        0        0     4026 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/MKL_support.h
--rw-rw-rw-   0        0        0    36570 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/Macros.h
--rw-rw-rw-   0        0        0    40154 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/Memory.h
--rw-rw-rw-   0        0        0    19365 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/Meta.h
--rw-rw-rw-   0        0        0       85 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/NonMPL2.h
--rw-rw-rw-   0        0        0      809 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-rw-rw-   0        0        0    10518 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/StaticAssert.h
--rw-rw-rw-   0        0        0    34198 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/XprHelper.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.527083 OApackage-2.7.7/src/Eigen/src/Eigenvalues/
--rw-rw-rw-   0        0        0    12558 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-rw-rw-   0        0        0    17021 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-rw-rw-   0        0        0     4178 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-rw-rw-   0        0        0    22944 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/EigenSolver.h
--rw-rw-rw-   0        0        0    17176 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-rw-rw-   0        0        0     9715 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-rw-rw-   0        0        0    14351 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-rw-rw-   0        0        0     5679 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-rw-rw-   0        0        0    23586 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/RealQZ.h
--rw-rw-rw-   0        0        0    20288 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/RealSchur.h
--rw-rw-rw-   0        0        0     3650 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-rw-rw-   0        0        0    33674 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-rw-rw-   0        0        0     4104 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-rw-rw-   0        0        0    22444 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.542746 OApackage-2.7.7/src/Eigen/src/Geometry/
--rw-rw-rw-   0        0        0    14815 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/AlignedBox.h
--rw-rw-rw-   0        0        0     8423 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/AngleAxis.h
--rw-rw-rw-   0        0        0     3639 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/EulerAngles.h
--rw-rw-rw-   0        0        0    20539 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/Homogeneous.h
--rw-rw-rw-   0        0        0    11961 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/Hyperplane.h
--rw-rw-rw-   0        0        0     8949 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/OrthoMethods.h
--rw-rw-rw-   0        0        0     8308 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/ParametrizedLine.h
--rw-rw-rw-   0        0        0    32152 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/Quaternion.h
--rw-rw-rw-   0        0        0     6877 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/Rotation2D.h
--rw-rw-rw-   0        0        0     8063 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/RotationBase.h
--rw-rw-rw-   0        0        0     6324 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/Scaling.h
--rw-rw-rw-   0        0        0    60514 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/Transform.h
--rw-rw-rw-   0        0        0     7773 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/Translation.h
--rw-rw-rw-   0        0        0     6191 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/Umeyama.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.542746 OApackage-2.7.7/src/Eigen/src/Geometry/arch/
--rw-rw-rw-   0        0        0     5387 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/arch/Geometry_SSE.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.542746 OApackage-2.7.7/src/Eigen/src/Householder/
--rw-rw-rw-   0        0        0     4481 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Householder/BlockHouseholder.h
--rw-rw-rw-   0        0        0     5345 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Householder/Householder.h
--rw-rw-rw-   0        0        0    20603 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Householder/HouseholderSequence.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.542746 OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/
--rw-rw-rw-   0        0        0     6755 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-rw-rw-   0        0        0     7253 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-rw-rw-   0        0        0     9184 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-rw-rw-   0        0        0    15062 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-rw-rw-   0        0        0    15234 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-rw-rw-   0        0        0    11527 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-rw-rw-   0        0        0     7762 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-rw-rw-   0        0        0     4158 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.542746 OApackage-2.7.7/src/Eigen/src/Jacobi/
--rw-rw-rw-   0        0        0    15957 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Jacobi/Jacobi.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.558360 OApackage-2.7.7/src/Eigen/src/LU/
--rw-rw-rw-   0        0        0     3057 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/LU/Determinant.h
--rw-rw-rw-   0        0        0    32803 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/LU/FullPivLU.h
--rw-rw-rw-   0        0        0    15064 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/LU/InverseImpl.h
--rw-rw-rw-   0        0        0    21478 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/LU/PartialPivLU.h
--rw-rw-rw-   0        0        0     3555 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.558360 OApackage-2.7.7/src/Eigen/src/LU/arch/
--rw-rw-rw-   0        0        0    13669 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/LU/arch/Inverse_SSE.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.558360 OApackage-2.7.7/src/Eigen/src/MetisSupport/
--rw-rw-rw-   0        0        0     4588 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/MetisSupport/MetisSupport.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.558360 OApackage-2.7.7/src/Eigen/src/OrderingMethods/
--rw-rw-rw-   0        0        0    16396 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/OrderingMethods/Amd.h
--rw-rw-rw-   0        0        0    62266 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-rw-rw-   0        0        0     5229 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/OrderingMethods/Ordering.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.558360 OApackage-2.7.7/src/Eigen/src/PaStiXSupport/
--rw-rw-rw-   0        0        0    22248 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.558360 OApackage-2.7.7/src/Eigen/src/PardisoSupport/
--rw-rw-rw-   0        0        0    20032 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.558360 OApackage-2.7.7/src/Eigen/src/QR/
--rw-rw-rw-   0        0        0    24881 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/QR/ColPivHouseholderQR.h
--rw-rw-rw-   0        0        0     4662 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-rw-rw-   0        0        0    20805 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-rw-rw-   0        0        0    25478 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/QR/FullPivHouseholderQR.h
--rw-rw-rw-   0        0        0    14022 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/QR/HouseholderQR.h
--rw-rw-rw-   0        0        0     2993 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.558360 OApackage-2.7.7/src/Eigen/src/SPQRSupport/
--rw-rw-rw-   0        0        0    11405 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.558360 OApackage-2.7.7/src/Eigen/src/SVD/
--rw-rw-rw-   0        0        0    48778 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SVD/BDCSVD.h
--rw-rw-rw-   0        0        0    32949 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SVD/JacobiSVD.h
--rw-rw-rw-   0        0        0     5099 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-rw-rw-   0        0        0    12650 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SVD/SVDBase.h
--rw-rw-rw-   0        0        0    15957 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SVD/UpperBidiagonalization.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.558360 OApackage-2.7.7/src/Eigen/src/SparseCholesky/
--rw-rw-rw-   0        0        0    24010 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-rw-rw-   0        0        0     6898 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.589672 OApackage-2.7.7/src/Eigen/src/SparseCore/
--rw-rw-rw-   0        0        0    10537 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/AmbiVector.h
--rw-rw-rw-   0        0        0     8164 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/CompressedStorage.h
--rw-rw-rw-   0        0        0    13178 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-rw-rw-   0        0        0     2191 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-rw-rw-   0        0        0     8080 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseAssign.h
--rw-rw-rw-   0        0        0    25592 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseBlock.h
--rw-rw-rw-   0        0        0     6485 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseColEtree.h
--rw-rw-rw-   0        0        0    12720 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-rw-rw-   0        0        0    25840 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-rw-rw-   0        0        0     4711 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-rw-rw-   0        0        0    12487 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-rw-rw-   0        0        0     5808 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-rw-rw-   0        0        0     3080 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseDot.h
--rw-rw-rw-   0        0        0     1107 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseFuzzy.h
--rw-rw-rw-   0        0        0    12589 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseMap.h
--rw-rw-rw-   0        0        0    52349 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseMatrix.h
--rw-rw-rw-   0        0        0    17923 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-rw-rw-   0        0        0     7329 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparsePermutation.h
--rw-rw-rw-   0        0        0     7049 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseProduct.h
--rw-rw-rw-   0        0        0     1699 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseRedux.h
--rw-rw-rw-   0        0        0    15492 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseRef.h
--rw-rw-rw-   0        0        0    25715 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-rw-rw-   0        0        0     4424 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseSolverBase.h
--rw-rw-rw-   0        0        0     8704 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-rw-rw-   0        0        0     3175 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseTranspose.h
--rw-rw-rw-   0        0        0     6437 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseTriangularView.h
--rw-rw-rw-   0        0        0     6602 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseUtil.h
--rw-rw-rw-   0        0        0    14831 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseVector.h
--rw-rw-rw-   0        0        0     8110 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseView.h
--rw-rw-rw-   0        0        0     9657 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/TriangularSolver.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.589672 OApackage-2.7.7/src/Eigen/src/SparseLU/
--rw-rw-rw-   0        0        0    27923 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU.h
--rw-rw-rw-   0        0        0     4303 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLUImpl.h
--rw-rw-rw-   0        0        0     7601 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-rw-rw-   0        0        0     4974 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-rw-rw-   0        0        0    10022 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-rw-rw-   0        0        0     2049 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-rw-rw-   0        0        0     6712 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-rw-rw-   0        0        0     6582 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-rw-rw-   0        0        0     3681 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-rw-rw-   0        0        0    10216 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-rw-rw-   0        0        0     4181 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-rw-rw-   0        0        0     5723 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-rw-rw-   0        0        0     8486 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-rw-rw-   0        0        0     9028 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-rw-rw-   0        0        0     4979 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-rw-rw-   0        0        0     4545 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-rw-rw-   0        0        0     2889 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.589672 OApackage-2.7.7/src/Eigen/src/SparseQR/
--rw-rw-rw-   0        0        0    28373 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseQR/SparseQR.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.589672 OApackage-2.7.7/src/Eigen/src/StlSupport/
--rw-rw-rw-   0        0        0     5117 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/StlSupport/StdDeque.h
--rw-rw-rw-   0        0        0     4147 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/StlSupport/StdList.h
--rw-rw-rw-   0        0        0     5330 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/StlSupport/StdVector.h
--rw-rw-rw-   0        0        0     2809 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/StlSupport/details.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.589672 OApackage-2.7.7/src/Eigen/src/SuperLUSupport/
--rw-rw-rw-   0        0        0    34341 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.589672 OApackage-2.7.7/src/Eigen/src/UmfPackSupport/
--rw-rw-rw-   0        0        0    17202 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.605246 OApackage-2.7.7/src/Eigen/src/misc/
--rw-rw-rw-   0        0        0     2913 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/misc/Image.h
--rw-rw-rw-   0        0        0     2742 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/misc/Kernel.h
--rw-rw-rw-   0        0        0     1748 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/misc/RealSvd2x2.h
--rw-rw-rw-   0        0        0    30560 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/misc/blas.h
--rw-rw-rw-   0        0        0     7834 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/misc/lapack.h
--rw-rw-rw-   0        0        0  1058368 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/misc/lapacke.h
--rw-rw-rw-   0        0        0      474 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/misc/lapacke_mangling.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.621722 OApackage-2.7.7/src/Eigen/src/plugins/
--rw-rw-rw-   0        0        0    13132 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-rw-rw-   0        0        0    16929 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-rw-rw-   0        0        0    37403 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/plugins/BlockMethods.h
--rw-rw-rw-   0        0        0     4828 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-rw-rw-   0        0        0     5621 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-rw-rw-   0        0        0     6375 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-rw-rw-   0        0        0     2937 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-rw-rw-   0        0        0      121 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/InfInt.cpp
--rw-rw-rw-   0        0        0    33528 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/InfInt.h
--rw-rw-rw-   0        0        0    30719 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/anyoption.cpp
--rw-rw-rw-   0        0        0    11552 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/anyoption.h
--rw-rw-rw-   0        0        0    57087 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/arrayproperties.cpp
--rw-rw-rw-   0        0        0    25076 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/arrayproperties.h
--rw-rw-rw-   0        0        0   231991 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/arraytools.cpp
--rw-rw-rw-   0        0        0    63495 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/arraytools.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.621722 OApackage-2.7.7/src/bitarray/
--rw-rw-rw-   0        0        0    15816 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/bitarray/bit_array.cpp
--rw-rw-rw-   0        0        0     4769 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/bitarray/bit_array.h
--rw-rw-rw-   0        0        0     4482 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/bitarray/bit_array_test.cpp
--rw-rw-rw-   0        0        0   125312 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/conference.cpp
--rw-rw-rw-   0        0        0    21129 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/conference.h
--rw-rw-rw-   0        0        0     8792 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/depth_extend.cpp
--rw-rw-rw-   0        0        0     1413 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/depth_extend.h
--rw-rw-rw-   0        0        0    37361 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/evenodd.cpp
--rw-rw-rw-   0        0        0    19179 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/evenodd.h
--rw-rw-rw-   0        0        0    40268 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/extend.cpp
--rw-rw-rw-   0        0        0     9929 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/extend.h
--rw-rw-rw-   0        0        0    15876 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/graphtools.cpp
--rw-rw-rw-   0        0        0     3041 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/graphtools.h
--rw-rw-rw-   0        0        0    91267 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/lmc.cpp
--rw-rw-rw-   0        0        0    20620 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/lmc.h
--rw-rw-rw-   0        0        0     8461 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/mathtools.cpp
--rw-rw-rw-   0        0        0    57619 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/mathtools.h
--rw-rw-rw-   0        0        0    16314 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/md5.cpp
--rw-rw-rw-   0        0        0      274 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/md5.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.621722 OApackage-2.7.7/src/mpitools/
--rw-rw-rw-   0        0        0    10354 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/mpitools/mpitools.cpp
--rw-rw-rw-   0        0        0     3256 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/mpitools/mpitools.h
--rw-rw-rw-   0        0        0     7926 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/msstdint.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.636482 OApackage-2.7.7/src/nauty/
--rw-rw-rw-   0        0        0    47137 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/gtools.c
--rw-rw-rw-   0        0        0     8276 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/gtools.h
--rw-rw-rw-   0        0        0    25673 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/naugraph.c
--rw-rw-rw-   0        0        0     9584 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/naugroup.c
--rw-rw-rw-   0        0        0     1451 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/naugroup.h
--rw-rw-rw-   0        0        0     4681 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/naurng.c
--rw-rw-rw-   0        0        0     1143 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/naurng.h
--rw-rw-rw-   0        0        0     4542 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/nausparse.h
--rw-rw-rw-   0        0        0    28418 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/nautil.c
--rw-rw-rw-   0        0        0    65854 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/nautinv.c
--rw-rw-rw-   0        0        0     2470 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/nautinv.h
--rw-rw-rw-   0        0        0    14184 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/naututil.h
--rw-rw-rw-   0        0        0    46615 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/nauty.c
--rw-rw-rw-   0        0        0    53904 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/nauty.h
--rw-rw-rw-   0        0        0    26910 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/schreier.c
--rw-rw-rw-   0        0        0     2741 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/schreier.h
--rw-rw-rw-   0        0        0    10479 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/sorttemplates.c
--rw-rw-rw-   0        0        0    46007 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nonroot.cpp
--rw-rw-rw-   0        0        0     1343 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nonroot.h
--rw-rw-rw-   0        0        0     5133 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/oaoptions.cpp
--rw-rw-rw-   0        0        0     1761 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/oaoptions.h
--rw-rw-rw-   0        0        0       16 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/pareto.cpp
--rw-rw-rw-   0        0        0    11534 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/pareto.h
--rw-rw-rw-   0        0        0      728 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/printfheader.h
--rw-rw-rw-   0        0        0    26632 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/strength.cpp
--rw-rw-rw-   0        0        0     6070 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/strength.h
--rw-rw-rw-   0        0        0    12014 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/tools.cpp
--rw-rw-rw-   0        0        0    14609 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/tools.h
--rw-rw-rw-   0        0        0     6761 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/unittests.cpp
--rw-rw-rw-   0        0        0      611 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/unittests.h
--rw-rw-rw-   0        0        0       35 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/version.h
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.636482 OApackage-2.7.7/tests/
--rw-rw-rw-   0        0        0        0 2023-05-16 07:33:54.000000 OApackage-2.7.7/tests/__init__.py
--rw-rw-rw-   0        0        0     5904 2023-05-16 07:33:54.000000 OApackage-2.7.7/tests/test_Doptim.py
--rw-rw-rw-   0        0        0     4427 2023-05-16 07:33:54.000000 OApackage-2.7.7/tests/test_conference.py
--rw-rw-rw-   0        0        0    34777 2023-05-16 07:33:54.000000 OApackage-2.7.7/tests/test_cpplibrary.py
--rw-rw-rw-   0        0        0     1188 2023-05-16 07:33:54.000000 OApackage-2.7.7/tests/test_cpplibrary_gwlp.py
--rw-rw-rw-   0        0        0      897 2023-05-16 07:33:54.000000 OApackage-2.7.7/tests/test_cpplibrary_macwilliams.py
--rw-rw-rw-   0        0        0     1446 2023-05-16 07:33:54.000000 OApackage-2.7.7/tests/test_nauty.py
--rw-rw-rw-   0        0        0    16691 2023-05-16 07:33:54.000000 OApackage-2.7.7/tests/test_oapackage.py
--rw-rw-rw-   0        0        0      625 2023-05-16 07:33:54.000000 OApackage-2.7.7/tests/test_oapackage_graphtools.py
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.222917 OApackage-2.7.8/
+-rw-rw-rw-   0        0        0       89 2023-06-14 21:28:19.000000 OApackage-2.7.8/CONTRIBUTORS.md
+-rw-rw-rw-   0        0        0     2229 2023-06-14 21:28:19.000000 OApackage-2.7.8/LICENSE
+-rw-rw-rw-   0        0        0      390 2023-06-14 21:28:19.000000 OApackage-2.7.8/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.002962 OApackage-2.7.8/OApackage.egg-info/
+-rw-rw-rw-   0        0        0     4638 2023-06-14 21:33:22.000000 OApackage-2.7.8/OApackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13655 2023-06-14 21:33:22.000000 OApackage-2.7.8/OApackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 21:33:22.000000 OApackage-2.7.8/OApackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-14 21:31:46.000000 OApackage-2.7.8/OApackage.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      105 2023-06-14 21:33:22.000000 OApackage-2.7.8/OApackage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-06-14 21:33:22.000000 OApackage-2.7.8/OApackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4638 2023-06-14 21:33:23.222917 OApackage-2.7.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3610 2023-06-14 21:28:19.000000 OApackage-2.7.8/README.md
+-rw-rw-rw-   0        0        0    34426 2023-06-14 21:28:19.000000 OApackage-2.7.8/doxy2swig.py
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:22.987366 OApackage-2.7.8/misc/
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.002962 OApackage-2.7.8/misc/scripts/
+-rw-rw-rw-   0        0        0      767 2023-06-14 21:28:19.000000 OApackage-2.7.8/misc/scripts/example_oapackage_python.py
+-rw-rw-rw-   0        0        0   105735 2023-06-14 21:28:19.000000 OApackage-2.7.8/numpy.i
+-rw-rw-rw-   0        0        0       48 2023-06-14 21:28:19.000000 OApackage-2.7.8/oaconfig.txt
+-rw-rw-rw-   0        0        0   144029 2023-06-14 21:28:19.000000 OApackage-2.7.8/oadoxy.i
+-rw-rw-rw-   0        0        0    16256 2023-06-14 21:28:19.000000 OApackage-2.7.8/oalib.i
+-rw-rw-rw-   0        0        0   421148 2023-06-14 21:30:09.000000 OApackage-2.7.8/oalib.py
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.002962 OApackage-2.7.8/oapackage/
+-rw-rw-rw-   0        0        0    21582 2023-06-14 21:28:19.000000 OApackage-2.7.8/oapackage/Doptim.py
+-rw-rw-rw-   0        0        0     2128 2023-06-14 21:28:19.000000 OApackage-2.7.8/oapackage/__init__.py
+-rw-rw-rw-   0        0        0     5620 2023-06-14 21:28:19.000000 OApackage-2.7.8/oapackage/_scanf.py
+-rw-rw-rw-   0        0        0     4150 2023-06-14 21:28:19.000000 OApackage-2.7.8/oapackage/conference.py
+-rw-rw-rw-   0        0        0     3569 2023-06-14 21:28:19.000000 OApackage-2.7.8/oapackage/graphtools.py
+-rw-rw-rw-   0        0        0    21493 2023-06-14 21:28:19.000000 OApackage-2.7.8/oapackage/markup.py
+-rw-rw-rw-   0        0        0    38474 2023-06-14 21:28:19.000000 OApackage-2.7.8/oapackage/oahelper.py
+-rw-rw-rw-   0        0        0      316 2023-06-14 21:28:19.000000 OApackage-2.7.8/oapackage/scanf.py
+-rw-rw-rw-   0        0        0      973 2023-06-14 21:28:19.000000 OApackage-2.7.8/pyproject.toml
+-rw-rw-rw-   0        0        0      187 2023-06-14 21:33:23.222917 OApackage-2.7.8/setup.cfg
+-rw-rw-rw-   0        0        0    12267 2023-06-14 21:28:19.000000 OApackage-2.7.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.035418 OApackage-2.7.8/src/
+-rw-rw-rw-   0        0        0    16020 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Deff.cpp
+-rw-rw-rw-   0        0        0     3902 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Deff.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.051043 OApackage-2.7.8/src/Eigen/
+-rw-rw-rw-   0        0        0      694 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1206 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/Cholesky
+-rw-rw-rw-   0        0        0     1900 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/CholmodSupport
+-rw-rw-rw-   0        0        0    17969 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/Core
+-rw-rw-rw-   0        0        0      122 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/Dense
+-rw-rw-rw-   0        0        0       35 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/Eigen
+-rw-rw-rw-   0        0        0     1822 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/Eigenvalues
+-rw-rw-rw-   0        0        0     2050 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/Geometry
+-rw-rw-rw-   0        0        0      874 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/Householder
+-rw-rw-rw-   0        0        0     2083 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/IterativeLinearSolvers
+-rw-rw-rw-   0        0        0      939 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/Jacobi
+-rw-rw-rw-   0        0        0     1433 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/LU
+-rw-rw-rw-   0        0        0      991 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/MetisSupport
+-rw-rw-rw-   0        0        0     2483 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/OrderingMethods
+-rw-rw-rw-   0        0        0     1676 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/PaStiXSupport
+-rw-rw-rw-   0        0        0     1116 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/PardisoSupport
+-rw-rw-rw-   0        0        0     1317 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/QR
+-rw-rw-rw-   0        0        0      945 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/QtAlignedMalloc
+-rw-rw-rw-   0        0        0     1162 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/SPQRSupport
+-rw-rw-rw-   0        0        0     1629 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/SVD
+-rw-rw-rw-   0        0        0      919 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/Sparse
+-rw-rw-rw-   0        0        0     1371 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/SparseCholesky
+-rw-rw-rw-   0        0        0     2240 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/SparseCore
+-rw-rw-rw-   0        0        0     1713 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/SparseLU
+-rw-rw-rw-   0        0        0     1222 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/SparseQR
+-rw-rw-rw-   0        0        0      797 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/StdDeque
+-rw-rw-rw-   0        0        0      726 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/StdList
+-rw-rw-rw-   0        0        0      803 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/StdVector
+-rw-rw-rw-   0        0        0     2243 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/SuperLUSupport
+-rw-rw-rw-   0        0        0     1382 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/UmfPackSupport
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:22.987366 OApackage-2.7.8/src/Eigen/src/
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.051043 OApackage-2.7.8/src/Eigen/src/Cholesky/
+-rw-rw-rw-   0        0        0    24440 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Cholesky/LDLT.h
+-rw-rw-rw-   0        0        0    18395 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Cholesky/LLT.h
+-rw-rw-rw-   0        0        0     3974 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.051043 OApackage-2.7.8/src/Eigen/src/CholmodSupport/
+-rw-rw-rw-   0        0        0    22307 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.082293 OApackage-2.7.8/src/Eigen/src/Core/
+-rw-rw-rw-   0        0        0    12218 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Array.h
+-rw-rw-rw-   0        0        0     8179 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/ArrayBase.h
+-rw-rw-rw-   0        0        0     6775 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/ArrayWrapper.h
+-rw-rw-rw-   0        0        0     2720 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Assign.h
+-rw-rw-rw-   0        0        0    38153 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/AssignEvaluator.h
+-rw-rw-rw-   0        0        0    12479 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Assign_MKL.h
+-rw-rw-rw-   0        0        0    13910 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/BandMatrix.h
+-rw-rw-rw-   0        0        0    18064 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Block.h
+-rw-rw-rw-   0        0        0     4249 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/BooleanRedux.h
+-rw-rw-rw-   0        0        0     5689 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/CommaInitializer.h
+-rw-rw-rw-   0        0        0     6970 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/ConditionEstimator.h
+-rw-rw-rw-   0        0        0    62197 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/CoreEvaluators.h
+-rw-rw-rw-   0        0        0     4525 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/CoreIterators.h
+-rw-rw-rw-   0        0        0     7593 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/CwiseBinaryOp.h
+-rw-rw-rw-   0        0        0    31424 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/CwiseNullaryOp.h
+-rw-rw-rw-   0        0        0     8256 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/CwiseTernaryOp.h
+-rw-rw-rw-   0        0        0     3877 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/CwiseUnaryOp.h
+-rw-rw-rw-   0        0        0     5282 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/CwiseUnaryView.h
+-rw-rw-rw-   0        0        0    27420 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/DenseBase.h
+-rw-rw-rw-   0        0        0    24212 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/DenseCoeffsBase.h
+-rw-rw-rw-   0        0        0    21959 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/DenseStorage.h
+-rw-rw-rw-   0        0        0     9597 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Diagonal.h
+-rw-rw-rw-   0        0        0    12666 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/DiagonalMatrix.h
+-rw-rw-rw-   0        0        0      970 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/DiagonalProduct.h
+-rw-rw-rw-   0        0        0    11507 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Dot.h
+-rw-rw-rw-   0        0        0     5619 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/EigenBase.h
+-rw-rw-rw-   0        0        0     4769 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/ForceAlignedAccess.h
+-rw-rw-rw-   0        0        0     5705 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Fuzzy.h
+-rw-rw-rw-   0        0        0    21123 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/GeneralProduct.h
+-rw-rw-rw-   0        0        0    22185 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/GenericPacketMath.h
+-rw-rw-rw-   0        0        0    10222 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/GlobalFunctions.h
+-rw-rw-rw-   0        0        0     7076 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/IO.h
+-rw-rw-rw-   0        0        0     3519 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Inverse.h
+-rw-rw-rw-   0        0        0     7239 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Map.h
+-rw-rw-rw-   0        0        0    10621 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/MapBase.h
+-rw-rw-rw-   0        0        0    40402 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/MathFunctions.h
+-rw-rw-rw-   0        0        0     3369 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/MathFunctionsImpl.h
+-rw-rw-rw-   0        0        0    19170 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Matrix.h
+-rw-rw-rw-   0        0        0    22154 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/MatrixBase.h
+-rw-rw-rw-   0        0        0     3400 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/NestByValue.h
+-rw-rw-rw-   0        0        0     3582 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/NoAlias.h
+-rw-rw-rw-   0        0        0     9234 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/NumTraits.h
+-rw-rw-rw-   0        0        0    21646 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/PermutationMatrix.h
+-rw-rw-rw-   0        0        0    45180 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/PlainObjectBase.h
+-rw-rw-rw-   0        0        0     7235 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Product.h
+-rw-rw-rw-   0        0        0    49497 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/ProductEvaluators.h
+-rw-rw-rw-   0        0        0     6379 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Random.h
+-rw-rw-rw-   0        0        0    17852 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Redux.h
+-rw-rw-rw-   0        0        0    12800 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Ref.h
+-rw-rw-rw-   0        0        0     5595 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Replicate.h
+-rw-rw-rw-   0        0        0     4200 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/ReturnByValue.h
+-rw-rw-rw-   0        0        0     7073 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Reverse.h
+-rw-rw-rw-   0        0        0     6020 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Select.h
+-rw-rw-rw-   0        0        0    14245 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/SelfAdjointView.h
+-rw-rw-rw-   0        0        0     1697 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-rw-rw-   0        0        0     6795 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Solve.h
+-rw-rw-rw-   0        0        0     9031 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/SolveTriangular.h
+-rw-rw-rw-   0        0        0     4365 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/SolverBase.h
+-rw-rw-rw-   0        0        0     7692 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/StableNorm.h
+-rw-rw-rw-   0        0        0     3865 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Stride.h
+-rw-rw-rw-   0        0        0     2683 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Swap.h
+-rw-rw-rw-   0        0        0    14777 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Transpose.h
+-rw-rw-rw-   0        0        0    14386 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Transpositions.h
+-rw-rw-rw-   0        0        0    37234 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/TriangularMatrix.h
+-rw-rw-rw-   0        0        0     3462 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/VectorBlock.h
+-rw-rw-rw-   0        0        0    29441 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/VectorwiseOp.h
+-rw-rw-rw-   0        0        0     8074 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/Visitor.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:22.987366 OApackage-2.7.8/src/Eigen/src/Core/arch/
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.097949 OApackage-2.7.8/src/Eigen/src/Core/arch/AVX/
+-rw-rw-rw-   0        0        0    18037 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/AVX/Complex.h
+-rw-rw-rw-   0        0        0    17776 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-rw-rw-   0        0        0    27787 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-rw-rw-   0        0        0     1194 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.097949 OApackage-2.7.8/src/Eigen/src/Core/arch/AVX512/
+-rw-rw-rw-   0        0        0    15733 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-rw-rw-   0        0        0    50936 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/AVX512/PacketMath.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.097949 OApackage-2.7.8/src/Eigen/src/Core/arch/AltiVec/
+-rw-rw-rw-   0        0        0    16443 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-rw-rw-   0        0        0    10797 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-rw-rw-   0        0        0    37671 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.097949 OApackage-2.7.8/src/Eigen/src/Core/arch/CUDA/
+-rw-rw-rw-   0        0        0     4240 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/CUDA/Complex.h
+-rw-rw-rw-   0        0        0    22059 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/CUDA/Half.h
+-rw-rw-rw-   0        0        0     2387 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/CUDA/MathFunctions.h
+-rw-rw-rw-   0        0        0    10744 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/CUDA/PacketMath.h
+-rw-rw-rw-   0        0        0    35442 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
+-rw-rw-rw-   0        0        0     5509 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/CUDA/TypeCasting.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.097949 OApackage-2.7.8/src/Eigen/src/Core/arch/Default/
+-rw-rw-rw-   0        0        0     1989 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-rw-rw-   0        0        0     1746 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/Default/Settings.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.097949 OApackage-2.7.8/src/Eigen/src/Core/arch/NEON/
+-rw-rw-rw-   0        0        0    17706 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/NEON/Complex.h
+-rw-rw-rw-   0        0        0     2846 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-rw-rw-   0        0        0    28726 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/NEON/PacketMath.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.097949 OApackage-2.7.8/src/Eigen/src/Core/arch/SSE/
+-rw-rw-rw-   0        0        0    19426 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/SSE/Complex.h
+-rw-rw-rw-   0        0        0    18888 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rw-rw-rw-   0        0        0    35825 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-rw-rw-   0        0        0     1759 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.113543 OApackage-2.7.8/src/Eigen/src/Core/arch/ZVector/
+-rw-rw-rw-   0        0        0    15366 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-rw-rw-   0        0        0     4418 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rw-rw-rw-   0        0        0    32283 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.113543 OApackage-2.7.8/src/Eigen/src/Core/functors/
+-rw-rw-rw-   0        0        0     6284 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-rw-rw-   0        0        0    18263 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-rw-rw-   0        0        0     8229 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-rw-rw-   0        0        0     4400 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/functors/StlFunctors.h
+-rw-rw-rw-   0        0        0      607 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-rw-rw-   0        0        0    27944 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/functors/UnaryFunctors.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.129168 OApackage-2.7.8/src/Eigen/src/Core/products/
+-rw-rw-rw-   0        0        0    81106 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-rw-rw-   0        0        0    18478 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-rw-rw-   0        0        0    15188 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-rw-rw-   0        0        0     6907 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-rw-rw-   0        0        0     5017 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-rw-rw-   0        0        0    26808 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-rw-rw-   0        0        0     6368 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-rw-rw-   0        0        0     4905 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/products/Parallelizer.h
+-rw-rw-rw-   0        0        0    19632 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-rw-rw-   0        0        0    11198 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-rw-rw-   0        0        0     9901 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-rw-rw-   0        0        0     5209 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-rw-rw-   0        0        0     6105 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-rw-rw-   0        0        0     4066 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-rw-rw-   0        0        0    20403 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-rw-rw-   0        0        0    13743 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-rw-rw-   0        0        0    14722 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-rw-rw-   0        0        0    10571 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-rw-rw-   0        0        0    13979 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-rw-rw-   0        0        0     6513 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-rw-rw-   0        0        0     5741 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/products/TriangularSolverVector.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.129168 OApackage-2.7.8/src/Eigen/src/Core/util/
+-rw-rw-rw-   0        0        0    15722 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/util/BlasUtil.h
+-rw-rw-rw-   0        0        0    21579 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/util/Constants.h
+-rw-rw-rw-   0        0        0     3564 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-rw-rw-   0        0        0    14150 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-rw-rw-   0        0        0     4026 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/util/MKL_support.h
+-rw-rw-rw-   0        0        0    36570 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/util/Macros.h
+-rw-rw-rw-   0        0        0    40154 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/util/Memory.h
+-rw-rw-rw-   0        0        0    19365 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/util/Meta.h
+-rw-rw-rw-   0        0        0       85 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/util/NonMPL2.h
+-rw-rw-rw-   0        0        0      809 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-rw-rw-   0        0        0    10518 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/util/StaticAssert.h
+-rw-rw-rw-   0        0        0    34198 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Core/util/XprHelper.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.144792 OApackage-2.7.8/src/Eigen/src/Eigenvalues/
+-rw-rw-rw-   0        0        0    12558 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-rw-rw-   0        0        0    17021 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-rw-rw-   0        0        0     4178 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-rw-rw-   0        0        0    22944 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-rw-rw-   0        0        0    17176 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-rw-rw-   0        0        0     9715 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-rw-rw-   0        0        0    14351 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-rw-rw-   0        0        0     5679 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-rw-rw-   0        0        0    23586 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Eigenvalues/RealQZ.h
+-rw-rw-rw-   0        0        0    20288 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Eigenvalues/RealSchur.h
+-rw-rw-rw-   0        0        0     3650 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-rw-rw-   0        0        0    33674 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-rw-rw-   0        0        0     4104 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-rw-rw-   0        0        0    22444 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.144792 OApackage-2.7.8/src/Eigen/src/Geometry/
+-rw-rw-rw-   0        0        0    14815 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Geometry/AlignedBox.h
+-rw-rw-rw-   0        0        0     8423 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Geometry/AngleAxis.h
+-rw-rw-rw-   0        0        0     3639 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Geometry/EulerAngles.h
+-rw-rw-rw-   0        0        0    20539 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Geometry/Homogeneous.h
+-rw-rw-rw-   0        0        0    11961 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Geometry/Hyperplane.h
+-rw-rw-rw-   0        0        0     8949 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Geometry/OrthoMethods.h
+-rw-rw-rw-   0        0        0     8308 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Geometry/ParametrizedLine.h
+-rw-rw-rw-   0        0        0    32152 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Geometry/Quaternion.h
+-rw-rw-rw-   0        0        0     6877 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Geometry/Rotation2D.h
+-rw-rw-rw-   0        0        0     8063 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Geometry/RotationBase.h
+-rw-rw-rw-   0        0        0     6324 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Geometry/Scaling.h
+-rw-rw-rw-   0        0        0    60514 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Geometry/Transform.h
+-rw-rw-rw-   0        0        0     7773 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Geometry/Translation.h
+-rw-rw-rw-   0        0        0     6191 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Geometry/Umeyama.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.144792 OApackage-2.7.8/src/Eigen/src/Geometry/arch/
+-rw-rw-rw-   0        0        0     5387 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Geometry/arch/Geometry_SSE.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.144792 OApackage-2.7.8/src/Eigen/src/Householder/
+-rw-rw-rw-   0        0        0     4481 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Householder/BlockHouseholder.h
+-rw-rw-rw-   0        0        0     5345 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Householder/Householder.h
+-rw-rw-rw-   0        0        0    20603 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Householder/HouseholderSequence.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.160417 OApackage-2.7.8/src/Eigen/src/IterativeLinearSolvers/
+-rw-rw-rw-   0        0        0     6755 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-rw-rw-   0        0        0     7253 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-rw-rw-   0        0        0     9184 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-rw-rw-   0        0        0    15062 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-rw-rw-   0        0        0    15234 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-rw-rw-   0        0        0    11527 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-rw-rw-   0        0        0     7762 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-rw-rw-   0        0        0     4158 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.160417 OApackage-2.7.8/src/Eigen/src/Jacobi/
+-rw-rw-rw-   0        0        0    15957 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/Jacobi/Jacobi.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.160417 OApackage-2.7.8/src/Eigen/src/LU/
+-rw-rw-rw-   0        0        0     3057 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/LU/Determinant.h
+-rw-rw-rw-   0        0        0    32803 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/LU/FullPivLU.h
+-rw-rw-rw-   0        0        0    15064 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/LU/InverseImpl.h
+-rw-rw-rw-   0        0        0    21478 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/LU/PartialPivLU.h
+-rw-rw-rw-   0        0        0     3555 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.160417 OApackage-2.7.8/src/Eigen/src/LU/arch/
+-rw-rw-rw-   0        0        0    13669 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/LU/arch/Inverse_SSE.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.160417 OApackage-2.7.8/src/Eigen/src/MetisSupport/
+-rw-rw-rw-   0        0        0     4588 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/MetisSupport/MetisSupport.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.160417 OApackage-2.7.8/src/Eigen/src/OrderingMethods/
+-rw-rw-rw-   0        0        0    16396 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/OrderingMethods/Amd.h
+-rw-rw-rw-   0        0        0    62266 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-rw-rw-   0        0        0     5229 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/OrderingMethods/Ordering.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.160417 OApackage-2.7.8/src/Eigen/src/PaStiXSupport/
+-rw-rw-rw-   0        0        0    22248 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.160417 OApackage-2.7.8/src/Eigen/src/PardisoSupport/
+-rw-rw-rw-   0        0        0    20032 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.160417 OApackage-2.7.8/src/Eigen/src/QR/
+-rw-rw-rw-   0        0        0    24881 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-rw-rw-   0        0        0     4662 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-rw-rw-   0        0        0    20805 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-rw-rw-   0        0        0    25478 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-rw-rw-   0        0        0    14022 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/QR/HouseholderQR.h
+-rw-rw-rw-   0        0        0     2993 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.160417 OApackage-2.7.8/src/Eigen/src/SPQRSupport/
+-rw-rw-rw-   0        0        0    11405 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.176042 OApackage-2.7.8/src/Eigen/src/SVD/
+-rw-rw-rw-   0        0        0    48778 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SVD/BDCSVD.h
+-rw-rw-rw-   0        0        0    32949 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SVD/JacobiSVD.h
+-rw-rw-rw-   0        0        0     5099 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-rw-rw-   0        0        0    12650 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SVD/SVDBase.h
+-rw-rw-rw-   0        0        0    15957 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SVD/UpperBidiagonalization.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.176042 OApackage-2.7.8/src/Eigen/src/SparseCholesky/
+-rw-rw-rw-   0        0        0    24010 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-rw-rw-   0        0        0     6898 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.191668 OApackage-2.7.8/src/Eigen/src/SparseCore/
+-rw-rw-rw-   0        0        0    10537 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/AmbiVector.h
+-rw-rw-rw-   0        0        0     8164 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/CompressedStorage.h
+-rw-rw-rw-   0        0        0    13178 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-rw-rw-   0        0        0     2191 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-rw-rw-   0        0        0     8080 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseAssign.h
+-rw-rw-rw-   0        0        0    25592 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseBlock.h
+-rw-rw-rw-   0        0        0     6485 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseColEtree.h
+-rw-rw-rw-   0        0        0    12720 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-rw-rw-   0        0        0    25840 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-rw-rw-   0        0        0     4711 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-rw-rw-   0        0        0    12487 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-rw-rw-   0        0        0     5808 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-rw-rw-   0        0        0     3080 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseDot.h
+-rw-rw-rw-   0        0        0     1107 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-rw-rw-   0        0        0    12589 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseMap.h
+-rw-rw-rw-   0        0        0    52349 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseMatrix.h
+-rw-rw-rw-   0        0        0    17923 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-rw-rw-   0        0        0     7329 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparsePermutation.h
+-rw-rw-rw-   0        0        0     7049 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseProduct.h
+-rw-rw-rw-   0        0        0     1699 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseRedux.h
+-rw-rw-rw-   0        0        0    15492 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseRef.h
+-rw-rw-rw-   0        0        0    25715 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-rw-rw-   0        0        0     4424 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-rw-rw-   0        0        0     8704 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-rw-rw-   0        0        0     3175 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseTranspose.h
+-rw-rw-rw-   0        0        0     6437 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-rw-rw-   0        0        0     6602 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseUtil.h
+-rw-rw-rw-   0        0        0    14831 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseVector.h
+-rw-rw-rw-   0        0        0     8110 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/SparseView.h
+-rw-rw-rw-   0        0        0     9657 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseCore/TriangularSolver.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.191668 OApackage-2.7.8/src/Eigen/src/SparseLU/
+-rw-rw-rw-   0        0        0    27923 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU.h
+-rw-rw-rw-   0        0        0     4303 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-rw-rw-   0        0        0     7601 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-rw-rw-   0        0        0     4974 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-rw-rw-   0        0        0    10022 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-rw-rw-   0        0        0     2049 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-rw-rw-   0        0        0     6712 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-rw-rw-   0        0        0     6582 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-rw-rw-   0        0        0     3681 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-rw-rw-   0        0        0    10216 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-rw-rw-   0        0        0     4181 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-rw-rw-   0        0        0     5723 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-rw-rw-   0        0        0     8486 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-rw-rw-   0        0        0     9028 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-rw-rw-   0        0        0     4979 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-rw-rw-   0        0        0     4545 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-rw-rw-   0        0        0     2889 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.191668 OApackage-2.7.8/src/Eigen/src/SparseQR/
+-rw-rw-rw-   0        0        0    28373 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SparseQR/SparseQR.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.191668 OApackage-2.7.8/src/Eigen/src/StlSupport/
+-rw-rw-rw-   0        0        0     5117 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/StlSupport/StdDeque.h
+-rw-rw-rw-   0        0        0     4147 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/StlSupport/StdList.h
+-rw-rw-rw-   0        0        0     5330 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/StlSupport/StdVector.h
+-rw-rw-rw-   0        0        0     2809 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/StlSupport/details.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.207293 OApackage-2.7.8/src/Eigen/src/SuperLUSupport/
+-rw-rw-rw-   0        0        0    34341 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.207293 OApackage-2.7.8/src/Eigen/src/UmfPackSupport/
+-rw-rw-rw-   0        0        0    17202 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.207293 OApackage-2.7.8/src/Eigen/src/misc/
+-rw-rw-rw-   0        0        0     2913 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/misc/Image.h
+-rw-rw-rw-   0        0        0     2742 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/misc/Kernel.h
+-rw-rw-rw-   0        0        0     1748 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/misc/RealSvd2x2.h
+-rw-rw-rw-   0        0        0    30560 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/misc/blas.h
+-rw-rw-rw-   0        0        0     7834 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/misc/lapack.h
+-rw-rw-rw-   0        0        0  1058368 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/misc/lapacke.h
+-rw-rw-rw-   0        0        0      474 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/misc/lapacke_mangling.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.207293 OApackage-2.7.8/src/Eigen/src/plugins/
+-rw-rw-rw-   0        0        0    13132 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-rw-rw-   0        0        0    16929 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-rw-rw-   0        0        0    37403 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/plugins/BlockMethods.h
+-rw-rw-rw-   0        0        0     4828 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-rw-rw-   0        0        0     5621 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-rw-rw-   0        0        0     6375 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-rw-rw-   0        0        0     2937 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-rw-rw-   0        0        0      121 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/InfInt.cpp
+-rw-rw-rw-   0        0        0    33528 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/InfInt.h
+-rw-rw-rw-   0        0        0    30719 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/anyoption.cpp
+-rw-rw-rw-   0        0        0    11552 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/anyoption.h
+-rw-rw-rw-   0        0        0    57087 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/arrayproperties.cpp
+-rw-rw-rw-   0        0        0    25076 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/arrayproperties.h
+-rw-rw-rw-   0        0        0   231991 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/arraytools.cpp
+-rw-rw-rw-   0        0        0    63495 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/arraytools.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.207293 OApackage-2.7.8/src/bitarray/
+-rw-rw-rw-   0        0        0    15816 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/bitarray/bit_array.cpp
+-rw-rw-rw-   0        0        0     4769 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/bitarray/bit_array.h
+-rw-rw-rw-   0        0        0     4482 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/bitarray/bit_array_test.cpp
+-rw-rw-rw-   0        0        0   125312 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/conference.cpp
+-rw-rw-rw-   0        0        0    21129 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/conference.h
+-rw-rw-rw-   0        0        0     8792 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/depth_extend.cpp
+-rw-rw-rw-   0        0        0     1413 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/depth_extend.h
+-rw-rw-rw-   0        0        0    37361 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/evenodd.cpp
+-rw-rw-rw-   0        0        0    19179 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/evenodd.h
+-rw-rw-rw-   0        0        0    40262 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/extend.cpp
+-rw-rw-rw-   0        0        0     9930 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/extend.h
+-rw-rw-rw-   0        0        0    15876 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/graphtools.cpp
+-rw-rw-rw-   0        0        0     3041 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/graphtools.h
+-rw-rw-rw-   0        0        0    91267 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/lmc.cpp
+-rw-rw-rw-   0        0        0    20620 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/lmc.h
+-rw-rw-rw-   0        0        0     8461 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/mathtools.cpp
+-rw-rw-rw-   0        0        0    57619 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/mathtools.h
+-rw-rw-rw-   0        0        0    16314 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/md5.cpp
+-rw-rw-rw-   0        0        0      274 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/md5.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.207293 OApackage-2.7.8/src/mpitools/
+-rw-rw-rw-   0        0        0    10354 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/mpitools/mpitools.cpp
+-rw-rw-rw-   0        0        0     3256 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/mpitools/mpitools.h
+-rw-rw-rw-   0        0        0     7926 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/msstdint.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.222917 OApackage-2.7.8/src/nauty/
+-rw-rw-rw-   0        0        0    47137 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/nauty/gtools.c
+-rw-rw-rw-   0        0        0     8276 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/nauty/gtools.h
+-rw-rw-rw-   0        0        0    25673 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/nauty/naugraph.c
+-rw-rw-rw-   0        0        0     9584 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/nauty/naugroup.c
+-rw-rw-rw-   0        0        0     1451 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/nauty/naugroup.h
+-rw-rw-rw-   0        0        0     4681 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/nauty/naurng.c
+-rw-rw-rw-   0        0        0     1143 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/nauty/naurng.h
+-rw-rw-rw-   0        0        0     4542 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/nauty/nausparse.h
+-rw-rw-rw-   0        0        0    28418 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/nauty/nautil.c
+-rw-rw-rw-   0        0        0    65854 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/nauty/nautinv.c
+-rw-rw-rw-   0        0        0     2470 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/nauty/nautinv.h
+-rw-rw-rw-   0        0        0    14184 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/nauty/naututil.h
+-rw-rw-rw-   0        0        0    46615 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/nauty/nauty.c
+-rw-rw-rw-   0        0        0    53904 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/nauty/nauty.h
+-rw-rw-rw-   0        0        0    26910 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/nauty/schreier.c
+-rw-rw-rw-   0        0        0     2741 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/nauty/schreier.h
+-rw-rw-rw-   0        0        0    10479 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/nauty/sorttemplates.c
+-rw-rw-rw-   0        0        0    46007 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/nonroot.cpp
+-rw-rw-rw-   0        0        0     1343 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/nonroot.h
+-rw-rw-rw-   0        0        0     5133 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/oaoptions.cpp
+-rw-rw-rw-   0        0        0     1761 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/oaoptions.h
+-rw-rw-rw-   0        0        0       16 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/pareto.cpp
+-rw-rw-rw-   0        0        0    11534 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/pareto.h
+-rw-rw-rw-   0        0        0      728 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/printfheader.h
+-rw-rw-rw-   0        0        0    26632 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/strength.cpp
+-rw-rw-rw-   0        0        0     6070 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/strength.h
+-rw-rw-rw-   0        0        0    12014 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/tools.cpp
+-rw-rw-rw-   0        0        0    14609 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/tools.h
+-rw-rw-rw-   0        0        0     6761 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/unittests.cpp
+-rw-rw-rw-   0        0        0      611 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/unittests.h
+-rw-rw-rw-   0        0        0       35 2023-06-14 21:28:19.000000 OApackage-2.7.8/src/version.h
+drwxrwxrwx   0        0        0        0 2023-06-14 21:33:23.222917 OApackage-2.7.8/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:28:19.000000 OApackage-2.7.8/tests/__init__.py
+-rw-rw-rw-   0        0        0     5904 2023-06-14 21:28:19.000000 OApackage-2.7.8/tests/test_Doptim.py
+-rw-rw-rw-   0        0        0     4427 2023-06-14 21:28:19.000000 OApackage-2.7.8/tests/test_conference.py
+-rw-rw-rw-   0        0        0    34777 2023-06-14 21:28:19.000000 OApackage-2.7.8/tests/test_cpplibrary.py
+-rw-rw-rw-   0        0        0     1188 2023-06-14 21:28:19.000000 OApackage-2.7.8/tests/test_cpplibrary_gwlp.py
+-rw-rw-rw-   0        0        0      897 2023-06-14 21:28:19.000000 OApackage-2.7.8/tests/test_cpplibrary_macwilliams.py
+-rw-rw-rw-   0        0        0     1446 2023-06-14 21:28:19.000000 OApackage-2.7.8/tests/test_nauty.py
+-rw-rw-rw-   0        0        0    16691 2023-06-14 21:28:19.000000 OApackage-2.7.8/tests/test_oapackage.py
+-rw-rw-rw-   0        0        0      625 2023-06-14 21:28:19.000000 OApackage-2.7.8/tests/test_oapackage_graphtools.py
```

### Comparing `OApackage-2.7.7/LICENSE` & `OApackage-2.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/OApackage.egg-info/PKG-INFO` & `OApackage-2.7.8/OApackage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OApackage
-Version: 2.7.7
+Version: 2.7.8
 Summary: Package to generate and analyse orthogonal arrays, conference designs and optimal designs
 Home-page: http://www.pietereendebak.nl/oapackage/index.html
 Author: Pieter Eendebak
 Author-email: pieter.eendebak@gmail.com
 License: BSD
 Keywords: orthogonal arrays, design of experiments, conference designs, isomorphism testing
 Platform: UNKNOWN
```

### Comparing `OApackage-2.7.7/OApackage.egg-info/SOURCES.txt` & `OApackage-2.7.8/OApackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/PKG-INFO` & `OApackage-2.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OApackage
-Version: 2.7.7
+Version: 2.7.8
 Summary: Package to generate and analyse orthogonal arrays, conference designs and optimal designs
 Home-page: http://www.pietereendebak.nl/oapackage/index.html
 Author: Pieter Eendebak
 Author-email: pieter.eendebak@gmail.com
 License: BSD
 Keywords: orthogonal arrays, design of experiments, conference designs, isomorphism testing
 Platform: UNKNOWN
```

### Comparing `OApackage-2.7.7/README.md` & `OApackage-2.7.8/README.md`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/doxy2swig.py` & `OApackage-2.7.8/doxy2swig.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/misc/scripts/example_oapackage_python.py` & `OApackage-2.7.8/misc/scripts/example_oapackage_python.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/numpy.i` & `OApackage-2.7.8/numpy.i`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/oadoxy.i` & `OApackage-2.7.8/oadoxy.i`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/oalib.i` & `OApackage-2.7.8/oalib.i`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/oalib.py` & `OApackage-2.7.8/oalib.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/oapackage/Doptim.py` & `OApackage-2.7.8/oapackage/Doptim.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/oapackage/__init__.py` & `OApackage-2.7.8/oapackage/__init__.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/oapackage/_scanf.py` & `OApackage-2.7.8/oapackage/_scanf.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/oapackage/conference.py` & `OApackage-2.7.8/oapackage/conference.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/oapackage/graphtools.py` & `OApackage-2.7.8/oapackage/graphtools.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/oapackage/markup.py` & `OApackage-2.7.8/oapackage/markup.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/oapackage/oahelper.py` & `OApackage-2.7.8/oapackage/oahelper.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/pyproject.toml` & `OApackage-2.7.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+[build-system]
+# Minimum requirements for the build system to execute.
+requires = ["numpy", "setuptools"]  # PEP 508 specifications.
+
 [tool.autopep8]
 max_line_length = 120
 # ignore = ["E501", "W6"]
 
 [tool.isort]
 profile = "black"
 line_length = 120
```

### Comparing `OApackage-2.7.7/setup.py` & `OApackage-2.7.8/setup.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Deff.cpp` & `OApackage-2.7.8/src/Deff.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Deff.h` & `OApackage-2.7.8/src/Deff.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/CMakeLists.txt` & `OApackage-2.7.8/src/Eigen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/Cholesky` & `OApackage-2.7.8/src/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/CholmodSupport` & `OApackage-2.7.8/src/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/Core` & `OApackage-2.7.8/src/Eigen/Core`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/Eigenvalues` & `OApackage-2.7.8/src/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/Geometry` & `OApackage-2.7.8/src/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/Householder` & `OApackage-2.7.8/src/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/IterativeLinearSolvers` & `OApackage-2.7.8/src/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/Jacobi` & `OApackage-2.7.8/src/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/LU` & `OApackage-2.7.8/src/Eigen/LU`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/MetisSupport` & `OApackage-2.7.8/src/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/OrderingMethods` & `OApackage-2.7.8/src/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/PaStiXSupport` & `OApackage-2.7.8/src/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/PardisoSupport` & `OApackage-2.7.8/src/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/QR` & `OApackage-2.7.8/src/Eigen/QR`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/QtAlignedMalloc` & `OApackage-2.7.8/src/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/SPQRSupport` & `OApackage-2.7.8/src/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/SVD` & `OApackage-2.7.8/src/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/Sparse` & `OApackage-2.7.8/src/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/SparseCholesky` & `OApackage-2.7.8/src/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/SparseCore` & `OApackage-2.7.8/src/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/SparseLU` & `OApackage-2.7.8/src/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/SparseQR` & `OApackage-2.7.8/src/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/StdDeque` & `OApackage-2.7.8/src/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/StdList` & `OApackage-2.7.8/src/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/StdVector` & `OApackage-2.7.8/src/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/SuperLUSupport` & `OApackage-2.7.8/src/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/UmfPackSupport` & `OApackage-2.7.8/src/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Cholesky/LDLT.h` & `OApackage-2.7.8/src/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Cholesky/LLT.h` & `OApackage-2.7.8/src/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Cholesky/LLT_LAPACKE.h` & `OApackage-2.7.8/src/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/CholmodSupport/CholmodSupport.h` & `OApackage-2.7.8/src/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Array.h` & `OApackage-2.7.8/src/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/ArrayBase.h` & `OApackage-2.7.8/src/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/ArrayWrapper.h` & `OApackage-2.7.8/src/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Assign.h` & `OApackage-2.7.8/src/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/AssignEvaluator.h` & `OApackage-2.7.8/src/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Assign_MKL.h` & `OApackage-2.7.8/src/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/BandMatrix.h` & `OApackage-2.7.8/src/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Block.h` & `OApackage-2.7.8/src/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/BooleanRedux.h` & `OApackage-2.7.8/src/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/CommaInitializer.h` & `OApackage-2.7.8/src/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/ConditionEstimator.h` & `OApackage-2.7.8/src/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/CoreEvaluators.h` & `OApackage-2.7.8/src/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/CoreIterators.h` & `OApackage-2.7.8/src/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/CwiseBinaryOp.h` & `OApackage-2.7.8/src/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/CwiseNullaryOp.h` & `OApackage-2.7.8/src/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/CwiseTernaryOp.h` & `OApackage-2.7.8/src/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/CwiseUnaryOp.h` & `OApackage-2.7.8/src/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/CwiseUnaryView.h` & `OApackage-2.7.8/src/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/DenseBase.h` & `OApackage-2.7.8/src/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/DenseCoeffsBase.h` & `OApackage-2.7.8/src/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/DenseStorage.h` & `OApackage-2.7.8/src/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Diagonal.h` & `OApackage-2.7.8/src/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/DiagonalMatrix.h` & `OApackage-2.7.8/src/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/DiagonalProduct.h` & `OApackage-2.7.8/src/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Dot.h` & `OApackage-2.7.8/src/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/EigenBase.h` & `OApackage-2.7.8/src/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/ForceAlignedAccess.h` & `OApackage-2.7.8/src/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Fuzzy.h` & `OApackage-2.7.8/src/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/GeneralProduct.h` & `OApackage-2.7.8/src/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/GenericPacketMath.h` & `OApackage-2.7.8/src/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/GlobalFunctions.h` & `OApackage-2.7.8/src/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/IO.h` & `OApackage-2.7.8/src/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Inverse.h` & `OApackage-2.7.8/src/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Map.h` & `OApackage-2.7.8/src/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/MapBase.h` & `OApackage-2.7.8/src/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/MathFunctions.h` & `OApackage-2.7.8/src/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/MathFunctionsImpl.h` & `OApackage-2.7.8/src/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Matrix.h` & `OApackage-2.7.8/src/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/MatrixBase.h` & `OApackage-2.7.8/src/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/NestByValue.h` & `OApackage-2.7.8/src/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/NoAlias.h` & `OApackage-2.7.8/src/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/NumTraits.h` & `OApackage-2.7.8/src/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/PermutationMatrix.h` & `OApackage-2.7.8/src/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/PlainObjectBase.h` & `OApackage-2.7.8/src/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Product.h` & `OApackage-2.7.8/src/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/ProductEvaluators.h` & `OApackage-2.7.8/src/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Random.h` & `OApackage-2.7.8/src/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Redux.h` & `OApackage-2.7.8/src/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Ref.h` & `OApackage-2.7.8/src/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Replicate.h` & `OApackage-2.7.8/src/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/ReturnByValue.h` & `OApackage-2.7.8/src/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Reverse.h` & `OApackage-2.7.8/src/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Select.h` & `OApackage-2.7.8/src/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/SelfAdjointView.h` & `OApackage-2.7.8/src/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/SelfCwiseBinaryOp.h` & `OApackage-2.7.8/src/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Solve.h` & `OApackage-2.7.8/src/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/SolveTriangular.h` & `OApackage-2.7.8/src/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/SolverBase.h` & `OApackage-2.7.8/src/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/StableNorm.h` & `OApackage-2.7.8/src/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Stride.h` & `OApackage-2.7.8/src/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Swap.h` & `OApackage-2.7.8/src/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Transpose.h` & `OApackage-2.7.8/src/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Transpositions.h` & `OApackage-2.7.8/src/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/TriangularMatrix.h` & `OApackage-2.7.8/src/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/VectorBlock.h` & `OApackage-2.7.8/src/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/VectorwiseOp.h` & `OApackage-2.7.8/src/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/Visitor.h` & `OApackage-2.7.8/src/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/AVX/Complex.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/AVX/MathFunctions.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/AVX/PacketMath.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/AVX/TypeCasting.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/AVX512/PacketMath.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/AltiVec/Complex.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/Complex.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/Half.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/CUDA/Half.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/MathFunctions.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/CUDA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/PacketMath.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/CUDA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/PacketMathHalf.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/CUDA/PacketMathHalf.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/TypeCasting.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/CUDA/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/Default/ConjHelper.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/Default/Settings.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/NEON/Complex.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/NEON/MathFunctions.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/NEON/PacketMath.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/SSE/Complex.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/SSE/MathFunctions.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/SSE/PacketMath.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/SSE/TypeCasting.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/ZVector/Complex.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/arch/ZVector/PacketMath.h` & `OApackage-2.7.8/src/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/functors/AssignmentFunctors.h` & `OApackage-2.7.8/src/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/functors/BinaryFunctors.h` & `OApackage-2.7.8/src/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/functors/NullaryFunctors.h` & `OApackage-2.7.8/src/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/functors/StlFunctors.h` & `OApackage-2.7.8/src/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/functors/TernaryFunctors.h` & `OApackage-2.7.8/src/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/functors/UnaryFunctors.h` & `OApackage-2.7.8/src/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `OApackage-2.7.8/src/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `OApackage-2.7.8/src/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `OApackage-2.7.8/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `OApackage-2.7.8/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `OApackage-2.7.8/src/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixVector.h` & `OApackage-2.7.8/src/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `OApackage-2.7.8/src/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/products/Parallelizer.h` & `OApackage-2.7.8/src/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `OApackage-2.7.8/src/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `OApackage-2.7.8/src/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `OApackage-2.7.8/src/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `OApackage-2.7.8/src/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointProduct.h` & `OApackage-2.7.8/src/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointRank2Update.h` & `OApackage-2.7.8/src/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `OApackage-2.7.8/src/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `OApackage-2.7.8/src/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/products/TriangularMatrixVector.h` & `OApackage-2.7.8/src/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `OApackage-2.7.8/src/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/products/TriangularSolverMatrix.h` & `OApackage-2.7.8/src/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `OApackage-2.7.8/src/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/products/TriangularSolverVector.h` & `OApackage-2.7.8/src/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/util/BlasUtil.h` & `OApackage-2.7.8/src/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/util/Constants.h` & `OApackage-2.7.8/src/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/util/DisableStupidWarnings.h` & `OApackage-2.7.8/src/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/util/ForwardDeclarations.h` & `OApackage-2.7.8/src/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/util/MKL_support.h` & `OApackage-2.7.8/src/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/util/Macros.h` & `OApackage-2.7.8/src/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/util/Memory.h` & `OApackage-2.7.8/src/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/util/Meta.h` & `OApackage-2.7.8/src/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/util/ReenableStupidWarnings.h` & `OApackage-2.7.8/src/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/util/StaticAssert.h` & `OApackage-2.7.8/src/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Core/util/XprHelper.h` & `OApackage-2.7.8/src/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `OApackage-2.7.8/src/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Eigenvalues/ComplexSchur.h` & `OApackage-2.7.8/src/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `OApackage-2.7.8/src/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Eigenvalues/EigenSolver.h` & `OApackage-2.7.8/src/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `OApackage-2.7.8/src/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `OApackage-2.7.8/src/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `OApackage-2.7.8/src/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `OApackage-2.7.8/src/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Eigenvalues/RealQZ.h` & `OApackage-2.7.8/src/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Eigenvalues/RealSchur.h` & `OApackage-2.7.8/src/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `OApackage-2.7.8/src/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `OApackage-2.7.8/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `OApackage-2.7.8/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Eigenvalues/Tridiagonalization.h` & `OApackage-2.7.8/src/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Geometry/AlignedBox.h` & `OApackage-2.7.8/src/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Geometry/AngleAxis.h` & `OApackage-2.7.8/src/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Geometry/EulerAngles.h` & `OApackage-2.7.8/src/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Geometry/Homogeneous.h` & `OApackage-2.7.8/src/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Geometry/Hyperplane.h` & `OApackage-2.7.8/src/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Geometry/OrthoMethods.h` & `OApackage-2.7.8/src/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Geometry/ParametrizedLine.h` & `OApackage-2.7.8/src/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Geometry/Quaternion.h` & `OApackage-2.7.8/src/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Geometry/Rotation2D.h` & `OApackage-2.7.8/src/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Geometry/RotationBase.h` & `OApackage-2.7.8/src/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Geometry/Scaling.h` & `OApackage-2.7.8/src/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Geometry/Transform.h` & `OApackage-2.7.8/src/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Geometry/Translation.h` & `OApackage-2.7.8/src/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Geometry/Umeyama.h` & `OApackage-2.7.8/src/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Geometry/arch/Geometry_SSE.h` & `OApackage-2.7.8/src/Eigen/src/Geometry/arch/Geometry_SSE.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Householder/BlockHouseholder.h` & `OApackage-2.7.8/src/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Householder/Householder.h` & `OApackage-2.7.8/src/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Householder/HouseholderSequence.h` & `OApackage-2.7.8/src/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `OApackage-2.7.8/src/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `OApackage-2.7.8/src/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `OApackage-2.7.8/src/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `OApackage-2.7.8/src/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `OApackage-2.7.8/src/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `OApackage-2.7.8/src/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `OApackage-2.7.8/src/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `OApackage-2.7.8/src/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/Jacobi/Jacobi.h` & `OApackage-2.7.8/src/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/LU/Determinant.h` & `OApackage-2.7.8/src/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/LU/FullPivLU.h` & `OApackage-2.7.8/src/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/LU/InverseImpl.h` & `OApackage-2.7.8/src/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/LU/PartialPivLU.h` & `OApackage-2.7.8/src/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `OApackage-2.7.8/src/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/LU/arch/Inverse_SSE.h` & `OApackage-2.7.8/src/Eigen/src/LU/arch/Inverse_SSE.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/MetisSupport/MetisSupport.h` & `OApackage-2.7.8/src/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/OrderingMethods/Amd.h` & `OApackage-2.7.8/src/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `OApackage-2.7.8/src/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/OrderingMethods/Ordering.h` & `OApackage-2.7.8/src/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `OApackage-2.7.8/src/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/PardisoSupport/PardisoSupport.h` & `OApackage-2.7.8/src/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/QR/ColPivHouseholderQR.h` & `OApackage-2.7.8/src/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `OApackage-2.7.8/src/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `OApackage-2.7.8/src/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/QR/FullPivHouseholderQR.h` & `OApackage-2.7.8/src/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/QR/HouseholderQR.h` & `OApackage-2.7.8/src/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `OApackage-2.7.8/src/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `OApackage-2.7.8/src/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SVD/BDCSVD.h` & `OApackage-2.7.8/src/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SVD/JacobiSVD.h` & `OApackage-2.7.8/src/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `OApackage-2.7.8/src/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SVD/SVDBase.h` & `OApackage-2.7.8/src/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SVD/UpperBidiagonalization.h` & `OApackage-2.7.8/src/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `OApackage-2.7.8/src/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `OApackage-2.7.8/src/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/AmbiVector.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/CompressedStorage.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/MappedSparseMatrix.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseAssign.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseBlock.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseColEtree.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseCompressedBase.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseDenseProduct.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseDot.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseFuzzy.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseMap.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseMatrix.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseMatrixBase.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparsePermutation.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseProduct.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseRedux.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseRef.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseSolverBase.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseTranspose.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseTriangularView.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseUtil.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseVector.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseView.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseCore/TriangularSolver.h` & `OApackage-2.7.8/src/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU.h` & `OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLUImpl.h` & `OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_Memory.h` & `OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_Structs.h` & `OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_Utils.h` & `OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_pivotL.h` & `OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_pruneL.h` & `OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `OApackage-2.7.8/src/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SparseQR/SparseQR.h` & `OApackage-2.7.8/src/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/StlSupport/StdDeque.h` & `OApackage-2.7.8/src/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/StlSupport/StdList.h` & `OApackage-2.7.8/src/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/StlSupport/StdVector.h` & `OApackage-2.7.8/src/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/StlSupport/details.h` & `OApackage-2.7.8/src/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `OApackage-2.7.8/src/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `OApackage-2.7.8/src/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/misc/Image.h` & `OApackage-2.7.8/src/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/misc/Kernel.h` & `OApackage-2.7.8/src/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/misc/RealSvd2x2.h` & `OApackage-2.7.8/src/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/misc/blas.h` & `OApackage-2.7.8/src/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/misc/lapack.h` & `OApackage-2.7.8/src/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/misc/lapacke.h` & `OApackage-2.7.8/src/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `OApackage-2.7.8/src/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `OApackage-2.7.8/src/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/plugins/BlockMethods.h` & `OApackage-2.7.8/src/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `OApackage-2.7.8/src/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `OApackage-2.7.8/src/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `OApackage-2.7.8/src/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `OApackage-2.7.8/src/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/InfInt.h` & `OApackage-2.7.8/src/InfInt.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/anyoption.cpp` & `OApackage-2.7.8/src/anyoption.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/anyoption.h` & `OApackage-2.7.8/src/anyoption.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/arrayproperties.cpp` & `OApackage-2.7.8/src/arrayproperties.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/arrayproperties.h` & `OApackage-2.7.8/src/arrayproperties.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/arraytools.cpp` & `OApackage-2.7.8/src/arraytools.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/arraytools.h` & `OApackage-2.7.8/src/arraytools.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/bitarray/bit_array.cpp` & `OApackage-2.7.8/src/bitarray/bit_array.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/bitarray/bit_array.h` & `OApackage-2.7.8/src/bitarray/bit_array.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/bitarray/bit_array_test.cpp` & `OApackage-2.7.8/src/bitarray/bit_array_test.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/conference.cpp` & `OApackage-2.7.8/src/conference.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/conference.h` & `OApackage-2.7.8/src/conference.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/depth_extend.cpp` & `OApackage-2.7.8/src/depth_extend.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/depth_extend.h` & `OApackage-2.7.8/src/depth_extend.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/evenodd.cpp` & `OApackage-2.7.8/src/evenodd.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/evenodd.h` & `OApackage-2.7.8/src/evenodd.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/extend.cpp` & `OApackage-2.7.8/src/extend.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -737,18 +737,18 @@
 }
 
 inline void showLoopProgress (array_t *array, const int col_offset, const rowindex_t N, const int node_rank = 0,
                               int nlmcarrays = -1) {
 
         static unsigned long long nloops = 0;
         nloops++;
-        if (nloops % 50 * 1000 == 0) {
+        if (nloops % 100 * 1000 == 0) {
                 fflush (stdout);
 
-                if (nloops % (500 * 1000 * 1000) == 0) {
+                if (nloops % (1000 * 1000 * 1000) == 0) {
                     if (checkloglevel(QUIET)) {
                         std::cout << "node [" << node_rank << "]: extend loop " << nloops / (1000 * 1000);
                         cout << "m, ";
                         print_perm (array + col_offset, N, 28);
                     }
                 }
         }
@@ -918,15 +918,15 @@
                         narrays++;
 
                         if ((narrays % oaextend.nLMC == 0) ||
                             ((get_time_ms () - extendTime) > oaextend.singleExtendTime)) {
                                 extendTime = get_time_ms ();
                                 if (log_print (QUIET, "")) {
                                         logstream (QUIET) << printfstring ("  OA extension: ") << narrays
-                                                          << " arrays checked, " << extensions.size ()
+                                                          << " arrays checked, " << nlmcarrays
                                                           << " solutions so far";
                                         logstream (QUIET) << ", time " << printtime ();
                                         myprintf ("  OA extension: current row: ");
                                         print_perm (array + col_offset, N, 36);
                                 }
                         }
```

### Comparing `OApackage-2.7.7/src/extend.h` & `OApackage-2.7.8/src/extend.h`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
       public:
 	/** Options for the extension algorithm
 	 *
 	 *
 	 */
         OAextend ()
-            : singleExtendTime (10.0), nLMC (40000), checkarrays (1), check_maximal (0), use_row_symmetry (1),
+            : singleExtendTime (10.0), nLMC (100000), checkarrays (1), check_maximal (0), use_row_symmetry (1),
               init_column_previous (1), extendarraymode (extendarray_mode_t::APPENDFULL), j5structure (J5_45), algmode (MODE_AUTOSELECT){};
 	/// @copydoc OAextend()
         OAextend (const OAextend &o) : singleExtendTime (o.singleExtendTime) {
                 this->nLMC = o.nLMC;
                 this->checkarrays = o.checkarrays;
                 this->use_row_symmetry = o.use_row_symmetry;
                 this->init_column_previous = o.init_column_previous;
```

### Comparing `OApackage-2.7.7/src/graphtools.cpp` & `OApackage-2.7.8/src/graphtools.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/graphtools.h` & `OApackage-2.7.8/src/graphtools.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/lmc.cpp` & `OApackage-2.7.8/src/lmc.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/lmc.h` & `OApackage-2.7.8/src/lmc.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/mathtools.cpp` & `OApackage-2.7.8/src/mathtools.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/mathtools.h` & `OApackage-2.7.8/src/mathtools.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/md5.cpp` & `OApackage-2.7.8/src/md5.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/mpitools/mpitools.cpp` & `OApackage-2.7.8/src/mpitools/mpitools.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/mpitools/mpitools.h` & `OApackage-2.7.8/src/mpitools/mpitools.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/msstdint.h` & `OApackage-2.7.8/src/msstdint.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/nauty/gtools.c` & `OApackage-2.7.8/src/nauty/gtools.c`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/nauty/gtools.h` & `OApackage-2.7.8/src/nauty/gtools.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/nauty/naugraph.c` & `OApackage-2.7.8/src/nauty/naugraph.c`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/nauty/naugroup.c` & `OApackage-2.7.8/src/nauty/naugroup.c`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/nauty/naugroup.h` & `OApackage-2.7.8/src/nauty/naugroup.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/nauty/naurng.c` & `OApackage-2.7.8/src/nauty/naurng.c`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/nauty/naurng.h` & `OApackage-2.7.8/src/nauty/naurng.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/nauty/nausparse.h` & `OApackage-2.7.8/src/nauty/nausparse.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/nauty/nautil.c` & `OApackage-2.7.8/src/nauty/nautil.c`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/nauty/nautinv.c` & `OApackage-2.7.8/src/nauty/nautinv.c`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/nauty/nautinv.h` & `OApackage-2.7.8/src/nauty/nautinv.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/nauty/naututil.h` & `OApackage-2.7.8/src/nauty/naututil.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/nauty/nauty.c` & `OApackage-2.7.8/src/nauty/nauty.c`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/nauty/nauty.h` & `OApackage-2.7.8/src/nauty/nauty.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/nauty/schreier.c` & `OApackage-2.7.8/src/nauty/schreier.c`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/nauty/schreier.h` & `OApackage-2.7.8/src/nauty/schreier.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/nauty/sorttemplates.c` & `OApackage-2.7.8/src/nauty/sorttemplates.c`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/nonroot.cpp` & `OApackage-2.7.8/src/nonroot.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/nonroot.h` & `OApackage-2.7.8/src/nonroot.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/oaoptions.cpp` & `OApackage-2.7.8/src/oaoptions.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/oaoptions.h` & `OApackage-2.7.8/src/oaoptions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/pareto.h` & `OApackage-2.7.8/src/pareto.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/printfheader.h` & `OApackage-2.7.8/src/printfheader.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/strength.cpp` & `OApackage-2.7.8/src/strength.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/strength.h` & `OApackage-2.7.8/src/strength.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/tools.cpp` & `OApackage-2.7.8/src/tools.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/tools.h` & `OApackage-2.7.8/src/tools.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/unittests.cpp` & `OApackage-2.7.8/src/unittests.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/src/unittests.h` & `OApackage-2.7.8/src/unittests.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/tests/test_Doptim.py` & `OApackage-2.7.8/tests/test_Doptim.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/tests/test_conference.py` & `OApackage-2.7.8/tests/test_conference.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/tests/test_cpplibrary.py` & `OApackage-2.7.8/tests/test_cpplibrary.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/tests/test_cpplibrary_gwlp.py` & `OApackage-2.7.8/tests/test_cpplibrary_gwlp.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/tests/test_cpplibrary_macwilliams.py` & `OApackage-2.7.8/tests/test_cpplibrary_macwilliams.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/tests/test_nauty.py` & `OApackage-2.7.8/tests/test_nauty.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/tests/test_oapackage.py` & `OApackage-2.7.8/tests/test_oapackage.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.7/tests/test_oapackage_graphtools.py` & `OApackage-2.7.8/tests/test_oapackage_graphtools.py`

 * *Files identical despite different names*

