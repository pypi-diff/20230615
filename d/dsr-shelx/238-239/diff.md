# Comparing `tmp/dsr_shelx-238.tar.gz` & `tmp/dsr_shelx-239.tar.gz`

## Comparing `dsr_shelx-238.tar` & `dsr_shelx-239.tar`

### file list

```diff
@@ -1,380 +1,380 @@
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dsr_shelx-238/.gitattributes
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 dsr_shelx-238/README
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dsr_shelx-238/requirements.txt
--rw-r--r--   0        0        0  1246304 2020-02-02 00:00:00.000000 dsr_shelx-238/example/p21c.hkl
--rw-r--r--   0        0        0    11911 2020-02-02 00:00:00.000000 dsr_shelx-238/example/p21c.res
--rw-r--r--   0        0        0    18020 2020-02-02 00:00:00.000000 dsr_shelx-238/example/p21c_final.res
--rw-r--r--   0        0        0    11805 2020-02-02 00:00:00.000000 dsr_shelx-238/example/p21c_step0.res
--rw-r--r--   0        0        0    11889 2020-02-02 00:00:00.000000 dsr_shelx-238/example/p21c_step1.res
--rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 dsr_shelx-238/example/p21c_step2.ins
--rw-r--r--   0        0        0    15909 2020-02-02 00:00:00.000000 dsr_shelx-238/example/p21c_step3.res
--rw-r--r--   0        0        0  1259586 2020-02-02 00:00:00.000000 dsr_shelx-238/example/p21n_cf3.hkl
--rw-r--r--   0        0        0     7064 2020-02-02 00:00:00.000000 dsr_shelx-238/example/p21n_cf3.ins
--rw-r--r--   0        0        0     7064 2020-02-02 00:00:00.000000 dsr_shelx-238/example/p21n_cf3.res
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/__init__.py
--rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/afix.py
--rw-r--r--   0        0        0    31800 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/atomhandling.py
--rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/atoms.py
--rw-r--r--   0        0        0    35671 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/cf3fit.py
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/constants.py
--rw-r--r--   0        0        0    50324 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/dbfile.py
--rwxr-xr-x   0        0        0      298 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/dsr
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/dsr.bat
--rw-r--r--   0        0        0    20825 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/dsr.py
--rw-r--r--   0        0        0   163958 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/dsr_db.txt
--rw-r--r--   0        0        0    13793 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/dsrparse.py
--rw-r--r--   0        0        0    12247 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/elements.py
--rw-r--r--   0        0        0    15987 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/export.py
--rw-r--r--   0        0        0    39464 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/misc.py
--rw-r--r--   0        0        0    97821 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/olex_dsr_db.txt
--rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/options.py
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/pyperclip.py
--rw-r--r--   0        0        0    16940 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/refine.py
--rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/resfile.py
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/resi.py
--rw-r--r--   0        0        0    21682 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/restraints.py
--rw-r--r--   0        0        0     8522 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/selfupdate.py
--rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/sql_export.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/terminalsize.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/version.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/fit/LICENSE.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/fit/__init__.py
--rw-r--r--   0        0        0    16846 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/fit/quatfit.py
--rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/__init__.py
--rw-r--r--   0        0        0    15985 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/ctx_base.py
--rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/ctx_fp.py
--rw-r--r--   0        0        0    17211 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/ctx_iv.py
--rw-r--r--   0        0        0    49448 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/ctx_mp.py
--rw-r--r--   0        0        0    37730 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/ctx_mp_python.py
--rw-r--r--   0        0        0   280518 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/function_docs.py
--rw-r--r--   0        0        0    29253 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/identification.py
--rw-r--r--   0        0        0    18561 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/math2.py
--rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/rational.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/usertools.py
--rw-r--r--   0        0        0    10627 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/visualization.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/calculus/__init__.py
--rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/calculus/approximation.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/calculus/calculus.py
--rw-r--r--   0        0        0    20226 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/calculus/differentiation.py
--rw-r--r--   0        0        0    73295 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/calculus/extrapolation.py
--rw-r--r--   0        0        0    31135 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/calculus/inverselaplace.py
--rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/calculus/odes.py
--rw-r--r--   0        0        0    32856 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/calculus/optimization.py
--rw-r--r--   0        0        0     7877 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/calculus/polynomials.py
--rw-r--r--   0        0        0    38487 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/calculus/quadrature.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/__init__.py
--rw-r--r--   0        0        0    37938 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/bessel.py
--rw-r--r--   0        0        0    42299 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/elliptic.py
--rw-r--r--   0        0        0    11644 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/expintegrals.py
--rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/factorials.py
--rw-r--r--   0        0        0    18100 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/functions.py
--rw-r--r--   0        0        0    51570 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/hypergeometric.py
--rw-r--r--   0        0        0    16097 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/orthogonal.py
--rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/qfunctions.py
--rw-r--r--   0        0        0    46184 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/rszeta.py
--rw-r--r--   0        0        0    37320 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/theta.py
--rw-r--r--   0        0        0    36389 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/zeta.py
--rw-r--r--   0        0        0    30858 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/zetazeros.py
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/libmp/__init__.py
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/libmp/backend.py
--rw-r--r--   0        0        0    71458 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/libmp/gammazeta.py
--rw-r--r--   0        0        0    43861 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libelefun.py
--rw-r--r--   0        0        0    36624 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libhyper.py
--rw-r--r--   0        0        0    16688 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libintmath.py
--rw-r--r--   0        0        0    26875 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libmpc.py
--rw-r--r--   0        0        0    45022 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libmpf.py
--rw-r--r--   0        0        0    27622 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libmpi.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/matrices/__init__.py
--rw-r--r--   0        0        0    18609 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/matrices/calculus.py
--rw-r--r--   0        0        0    24394 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/matrices/eigen.py
--rw-r--r--   0        0        0    58534 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/matrices/eigen_symmetric.py
--rw-r--r--   0        0        0    26962 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/matrices/linalg.py
--rw-r--r--   0        0        0    32168 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/matrices/matrices.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/__init__.py
--rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/conftest.py
--rw-r--r--   0        0        0    15858 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/convert.py
--rw-r--r--   0        0        0    56245 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/convert_matrix.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/exception.py
--rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/lazy_imports.py
--rw-r--r--   0        0        0    10204 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/relabel.py
--rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/__init__.py
--rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/asteroidal.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/boundary.py
--rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bridges.py
--rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/chains.py
--rw-r--r--   0        0        0    14376 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/chordal.py
--rw-r--r--   0        0        0    26631 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/clique.py
--rw-r--r--   0        0        0    18789 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/cluster.py
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/communicability_alg.py
--rw-r--r--   0        0        0    15869 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/core.py
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/covering.py
--rw-r--r--   0        0        0     9722 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/cuts.py
--rw-r--r--   0        0        0    21677 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/cycles.py
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/d_separation.py
--rw-r--r--   0        0        0    36881 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/dag.py
--rw-r--r--   0        0        0    22803 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/distance_measures.py
--rw-r--r--   0        0        0     6872 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/distance_regular.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/dominance.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/dominating.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/efficiency_measures.py
--rw-r--r--   0        0        0    13602 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/euler.py
--rw-r--r--   0        0        0    11392 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/graph_hashing.py
--rw-r--r--   0        0        0    13449 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/graphical.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/hierarchy.py
--rw-r--r--   0        0        0     6152 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/hybrid.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isolate.py
--rw-r--r--   0        0        0    19792 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/link_prediction.py
--rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/lowest_common_ancestors.py
--rw-r--r--   0        0        0    42801 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/matching.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/mis.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/moral.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/non_randomness.py
--rw-r--r--   0        0        0    16320 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/planar_drawing.py
--rw-r--r--   0        0        0    39410 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/planarity.py
--rw-r--r--   0        0        0    10826 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/polynomials.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/reciprocity.py
--rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/regular.py
--rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/richclub.py
--rw-r--r--   0        0        0    59768 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/similarity.py
--rw-r--r--   0        0        0    30243 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/simple_paths.py
--rw-r--r--   0        0        0    13085 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/smallworld.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/smetric.py
--rw-r--r--   0        0        0    10038 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/sparsifiers.py
--rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/structuralholes.py
--rw-r--r--   0        0        0    22926 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/summarization.py
--rw-r--r--   0        0        0     9819 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/swap.py
--rw-r--r--   0        0        0    31010 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/threshold.py
--rw-r--r--   0        0        0    11584 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tournament.py
--rw-r--r--   0        0        0    13476 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/triads.py
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/vitality.py
--rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/voronoi.py
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/wiener.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/__init__.py
--rw-r--r--   0        0        0     7181 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/clique.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/clustering_coefficient.py
--rw-r--r--   0        0        0    12716 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/connectivity.py
--rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/distance_measures.py
--rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/dominating_set.py
--rw-r--r--   0        0        0    13223 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/kcomponents.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/matching.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/maxcut.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/ramsey.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/steinertree.py
--rw-r--r--   0        0        0    54262 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/traveling_salesman.py
--rw-r--r--   0        0        0     8106 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/treewidth.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/vertex_cover.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/__init__.py
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/connectivity.py
--rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/correlation.py
--rw-r--r--   0        0        0     9094 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/mixing.py
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/neighbor_degree.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/pairs.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/__init__.py
--rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/basic.py
--rw-r--r--   0        0        0     8412 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/centrality.py
--rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/cluster.py
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/covering.py
--rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/edgelist.py
--rw-r--r--   0        0        0    19961 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/generators.py
--rw-r--r--   0        0        0    21273 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/matching.py
--rw-r--r--   0        0        0     6382 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/matrix.py
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/projection.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/redundancy.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/spectral.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/__init__.py
--rw-r--r--   0        0        0    14324 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/betweenness.py
--rw-r--r--   0        0        0     9655 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/betweenness_subset.py
--rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/closeness.py
--rw-r--r--   0        0        0    11766 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/current_flow_betweenness.py
--rw-r--r--   0        0        0     7976 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/current_flow_betweenness_subset.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/current_flow_closeness.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/degree_alg.py
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/dispersion.py
--rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/eigenvector.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/flow_matrix.py
--rw-r--r--   0        0        0    27731 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/group.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/harmonic.py
--rw-r--r--   0        0        0    10674 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/katz.py
--rw-r--r--   0        0        0     6801 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/load.py
--rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/percolation.py
--rw-r--r--   0        0        0     6947 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/reaching.py
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/second_order.py
--rw-r--r--   0        0        0     9506 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/subgraph_alg.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/trophic.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/voterank_alg.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/coloring/__init__.py
--rw-r--r--   0        0        0    16571 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/coloring/equitable_coloring.py
--rw-r--r--   0        0        0    19573 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/coloring/greedy_coloring.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/__init__.py
--rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/asyn_fluid.py
--rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/centrality.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/community_utils.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/kclique.py
--rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/kernighan_lin.py
--rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/label_propagation.py
--rw-r--r--   0        0        0    13682 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/louvain.py
--rw-r--r--   0        0        0     8048 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/lukes.py
--rw-r--r--   0        0        0    19281 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/modularity_max.py
--rw-r--r--   0        0        0    14610 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/quality.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/__init__.py
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/attracting.py
--rw-r--r--   0        0        0    12501 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/biconnected.py
--rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/connected.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/semiconnected.py
--rw-r--r--   0        0        0    11896 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/strongly_connected.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/weakly_connected.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/__init__.py
--rw-r--r--   0        0        0    29734 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/connectivity.py
--rw-r--r--   0        0        0    22640 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/cuts.py
--rw-r--r--   0        0        0    14425 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/disjoint_paths.py
--rw-r--r--   0        0        0    43788 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/edge_augmentation.py
--rw-r--r--   0        0        0    20687 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/edge_kcomponents.py
--rw-r--r--   0        0        0     8222 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/kcomponents.py
--rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/kcutsets.py
--rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/stoerwagner.py
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/utils.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/__init__.py
--rw-r--r--   0        0        0    13238 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/boykovkolmogorov.py
--rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/capacityscaling.py
--rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/dinitz_alg.py
--rw-r--r--   0        0        0     7956 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/edmondskarp.py
--rw-r--r--   0        0        0     6267 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/gomory_hu.py
--rw-r--r--   0        0        0    22715 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/maxflow.py
--rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/mincost.py
--rw-r--r--   0        0        0    25089 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/networksimplex.py
--rw-r--r--   0        0        0    15621 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/preflowpush.py
--rw-r--r--   0        0        0    10272 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/shortestaugmentingpath.py
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/utils.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/__init__.py
--rw-r--r--   0        0        0    43599 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/ismags.py
--rw-r--r--   0        0        0     6382 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/isomorph.py
--rw-r--r--   0        0        0    40556 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/isomorphvf2.py
--rw-r--r--   0        0        0    10936 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/matchhelpers.py
--rw-r--r--   0        0        0    10949 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/temporalisomorphvf2.py
--rw-r--r--   0        0        0     9258 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/tree_isomorphism.py
--rw-r--r--   0        0        0     7496 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/vf2userfunc.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/link_analysis/__init__.py
--rw-r--r--   0        0        0    11889 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/link_analysis/hits_alg.py
--rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/link_analysis/pagerank_alg.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/minors/__init__.py
--rw-r--r--   0        0        0    21714 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/minors/contraction.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/node_classification/__init__.py
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/node_classification/hmn.py
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/node_classification/lgc.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/node_classification/utils.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/operators/__init__.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/operators/all.py
--rw-r--r--   0        0        0    12902 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/operators/binary.py
--rw-r--r--   0        0        0    13857 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/operators/product.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/operators/unary.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/__init__.py
--rw-r--r--   0        0        0     6990 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/astar.py
--rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/dense.py
--rw-r--r--   0        0        0    20139 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/generic.py
--rw-r--r--   0        0        0    14928 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/unweighted.py
--rw-r--r--   0        0        0    80039 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/weighted.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/__init__.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/beamsearch.py
--rw-r--r--   0        0        0    14161 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/breadth_first_search.py
--rw-r--r--   0        0        0    12842 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/depth_first_search.py
--rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/edgebfs.py
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/edgedfs.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/__init__.py
--rw-r--r--   0        0        0    36255 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/branchings.py
--rw-r--r--   0        0        0    12987 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/coding.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/decomposition.py
--rw-r--r--   0        0        0    39261 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/mst.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/operations.py
--rw-r--r--   0        0        0     7497 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/recognition.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/__init__.py
--rw-r--r--   0        0        0    15471 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/coreviews.py
--rw-r--r--   0        0        0    44427 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/digraph.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/filters.py
--rw-r--r--   0        0        0    36626 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/function.py
--rw-r--r--   0        0        0    66826 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/graph.py
--rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/graphviews.py
--rw-r--r--   0        0        0    35867 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/multidigraph.py
--rw-r--r--   0        0        0    45810 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/multigraph.py
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/ordered.py
--rw-r--r--   0        0        0    45714 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/reportviews.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/drawing/__init__.py
--rw-r--r--   0        0        0    35778 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/drawing/layout.py
--rw-r--r--   0        0        0    15396 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/drawing/nx_agraph.py
--rw-r--r--   0        0        0    14091 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/drawing/nx_pydot.py
--rw-r--r--   0        0        0    48373 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/drawing/nx_pylab.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/__init__.py
--rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/atlas.dat.gz
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/atlas.py
--rw-r--r--   0        0        0    23801 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/classic.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/cographs.py
--rw-r--r--   0        0        0    34429 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/community.py
--rw-r--r--   0        0        0    29817 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/degree_seq.py
--rw-r--r--   0        0        0    16676 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/directed.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/duplication.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/ego.py
--rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/expanders.py
--rw-r--r--   0        0        0    29482 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/geometric.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/harary_graph.py
--rw-r--r--   0        0        0    14128 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/internet_as_graphs.py
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/intersection.py
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/interval_graph.py
--rw-r--r--   0        0        0    24785 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/joint_degree_seq.py
--rw-r--r--   0        0        0    13223 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/lattice.py
--rw-r--r--   0        0        0    17654 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/line.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/mycielski.py
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/nonisomorphic_trees.py
--rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/random_clustered.py
--rw-r--r--   0        0        0    44337 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/random_graphs.py
--rw-r--r--   0        0        0    30426 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/small.py
--rw-r--r--   0        0        0    22759 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/social.py
--rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/spectral_graph_forge.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/stochastic.py
--rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/sudoku.py
--rw-r--r--   0        0        0    14146 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/trees.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/triads.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/linalg/__init__.py
--rw-r--r--   0        0        0    18281 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/linalg/algebraicconnectivity.py
--rw-r--r--   0        0        0    15658 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/linalg/attrmatrix.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/linalg/bethehessianmatrix.py
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/linalg/graphmatrix.py
--rw-r--r--   0        0        0    13986 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/linalg/laplacianmatrix.py
--rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/linalg/modularitymatrix.py
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/linalg/spectrum.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/__init__.py
--rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/adjlist.py
--rw-r--r--   0        0        0    14079 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/edgelist.py
--rw-r--r--   0        0        0    39511 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/gexf.py
--rw-r--r--   0        0        0    30016 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/gml.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/gpickle.py
--rw-r--r--   0        0        0    11301 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/graph6.py
--rw-r--r--   0        0        0    39163 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/graphml.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/leda.py
--rw-r--r--   0        0        0    11201 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/multiline_adjlist.py
--rw-r--r--   0        0        0    12183 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/nx_shp.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/nx_yaml.py
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/p2g.py
--rw-r--r--   0        0        0     8636 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/pajek.py
--rw-r--r--   0        0        0    10217 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/sparse6.py
--rw-r--r--   0        0        0     6498 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/text.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/__init__.py
--rw-r--r--   0        0        0     4745 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/adjacency.py
--rw-r--r--   0        0        0     8142 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/cytoscape.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/jit.py
--rw-r--r--   0        0        0    11619 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/node_link.py
--rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/tree.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/testing/__init__.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/testing/test.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/testing/utils.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/utils/__init__.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/utils/contextmanagers.py
--rw-r--r--   0        0        0    46493 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/utils/decorators.py
--rw-r--r--   0        0        0    10391 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/utils/heaps.py
--rw-r--r--   0        0        0     9138 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/utils/mapped_queue.py
--rw-r--r--   0        0        0    20390 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/utils/misc.py
--rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/utils/random_sequence.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/utils/rcm.py
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/utils/union_find.py
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 dsr_shelx-238/.gitignore
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 dsr_shelx-238/README.md
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 dsr_shelx-238/pyproject.toml
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 dsr_shelx-238/PKG-INFO
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dsr_shelx-239/.gitattributes
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 dsr_shelx-239/README
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dsr_shelx-239/requirements.txt
+-rw-r--r--   0        0        0  1246304 2020-02-02 00:00:00.000000 dsr_shelx-239/example/p21c.hkl
+-rw-r--r--   0        0        0    11911 2020-02-02 00:00:00.000000 dsr_shelx-239/example/p21c.res
+-rw-r--r--   0        0        0    18020 2020-02-02 00:00:00.000000 dsr_shelx-239/example/p21c_final.res
+-rw-r--r--   0        0        0    11805 2020-02-02 00:00:00.000000 dsr_shelx-239/example/p21c_step0.res
+-rw-r--r--   0        0        0    11889 2020-02-02 00:00:00.000000 dsr_shelx-239/example/p21c_step1.res
+-rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 dsr_shelx-239/example/p21c_step2.ins
+-rw-r--r--   0        0        0    15909 2020-02-02 00:00:00.000000 dsr_shelx-239/example/p21c_step3.res
+-rw-r--r--   0        0        0  1259586 2020-02-02 00:00:00.000000 dsr_shelx-239/example/p21n_cf3.hkl
+-rw-r--r--   0        0        0     7064 2020-02-02 00:00:00.000000 dsr_shelx-239/example/p21n_cf3.ins
+-rw-r--r--   0        0        0     7064 2020-02-02 00:00:00.000000 dsr_shelx-239/example/p21n_cf3.res
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/__init__.py
+-rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/afix.py
+-rw-r--r--   0        0        0    31800 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/atomhandling.py
+-rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/atoms.py
+-rw-r--r--   0        0        0    35671 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/cf3fit.py
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/constants.py
+-rw-r--r--   0        0        0    50642 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/dbfile.py
+-rwxr-xr-x   0        0        0      298 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/dsr
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/dsr.bat
+-rw-r--r--   0        0        0    20825 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/dsr.py
+-rw-r--r--   0        0        0   163958 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/dsr_db.txt
+-rw-r--r--   0        0        0    13793 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/dsrparse.py
+-rw-r--r--   0        0        0    12247 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/elements.py
+-rw-r--r--   0        0        0    15987 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/export.py
+-rw-r--r--   0        0        0    39464 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/misc.py
+-rw-r--r--   0        0        0    97821 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/olex_dsr_db.txt
+-rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/options.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/pyperclip.py
+-rw-r--r--   0        0        0    16940 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/refine.py
+-rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/resfile.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/resi.py
+-rw-r--r--   0        0        0    21682 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/restraints.py
+-rw-r--r--   0        0        0     8522 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/selfupdate.py
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/sql_export.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/terminalsize.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/version.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/fit/LICENSE.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/fit/__init__.py
+-rw-r--r--   0        0        0    16846 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/fit/quatfit.py
+-rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/__init__.py
+-rw-r--r--   0        0        0    15985 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/ctx_base.py
+-rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/ctx_fp.py
+-rw-r--r--   0        0        0    17211 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/ctx_iv.py
+-rw-r--r--   0        0        0    49448 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/ctx_mp.py
+-rw-r--r--   0        0        0    37730 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/ctx_mp_python.py
+-rw-r--r--   0        0        0   280518 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/function_docs.py
+-rw-r--r--   0        0        0    29253 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/identification.py
+-rw-r--r--   0        0        0    18561 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/math2.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/rational.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/usertools.py
+-rw-r--r--   0        0        0    10627 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/visualization.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/calculus/__init__.py
+-rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/calculus/approximation.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/calculus/calculus.py
+-rw-r--r--   0        0        0    20226 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/calculus/differentiation.py
+-rw-r--r--   0        0        0    73295 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/calculus/extrapolation.py
+-rw-r--r--   0        0        0    31135 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/calculus/inverselaplace.py
+-rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/calculus/odes.py
+-rw-r--r--   0        0        0    32856 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/calculus/optimization.py
+-rw-r--r--   0        0        0     7877 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/calculus/polynomials.py
+-rw-r--r--   0        0        0    38487 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/calculus/quadrature.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/functions/__init__.py
+-rw-r--r--   0        0        0    37938 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/functions/bessel.py
+-rw-r--r--   0        0        0    42299 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/functions/elliptic.py
+-rw-r--r--   0        0        0    11644 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/functions/expintegrals.py
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/functions/factorials.py
+-rw-r--r--   0        0        0    18100 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/functions/functions.py
+-rw-r--r--   0        0        0    51570 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/functions/hypergeometric.py
+-rw-r--r--   0        0        0    16097 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/functions/orthogonal.py
+-rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/functions/qfunctions.py
+-rw-r--r--   0        0        0    46184 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/functions/rszeta.py
+-rw-r--r--   0        0        0    37320 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/functions/theta.py
+-rw-r--r--   0        0        0    36389 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/functions/zeta.py
+-rw-r--r--   0        0        0    30858 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/functions/zetazeros.py
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/libmp/__init__.py
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/libmp/backend.py
+-rw-r--r--   0        0        0    71458 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/libmp/gammazeta.py
+-rw-r--r--   0        0        0    43861 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/libmp/libelefun.py
+-rw-r--r--   0        0        0    36624 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/libmp/libhyper.py
+-rw-r--r--   0        0        0    16688 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/libmp/libintmath.py
+-rw-r--r--   0        0        0    26875 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/libmp/libmpc.py
+-rw-r--r--   0        0        0    45022 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/libmp/libmpf.py
+-rw-r--r--   0        0        0    27622 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/libmp/libmpi.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/matrices/__init__.py
+-rw-r--r--   0        0        0    18609 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/matrices/calculus.py
+-rw-r--r--   0        0        0    24394 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/matrices/eigen.py
+-rw-r--r--   0        0        0    58534 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/matrices/eigen_symmetric.py
+-rw-r--r--   0        0        0    26962 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/matrices/linalg.py
+-rw-r--r--   0        0        0    32168 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/mpmath/matrices/matrices.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/__init__.py
+-rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/conftest.py
+-rw-r--r--   0        0        0    15858 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/convert.py
+-rw-r--r--   0        0        0    56245 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/convert_matrix.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/exception.py
+-rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/lazy_imports.py
+-rw-r--r--   0        0        0    10204 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/relabel.py
+-rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/__init__.py
+-rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/asteroidal.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/boundary.py
+-rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bridges.py
+-rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/chains.py
+-rw-r--r--   0        0        0    14376 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/chordal.py
+-rw-r--r--   0        0        0    26631 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/clique.py
+-rw-r--r--   0        0        0    18789 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/cluster.py
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/communicability_alg.py
+-rw-r--r--   0        0        0    15869 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/core.py
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/covering.py
+-rw-r--r--   0        0        0     9722 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/cuts.py
+-rw-r--r--   0        0        0    21677 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/cycles.py
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/d_separation.py
+-rw-r--r--   0        0        0    36881 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/dag.py
+-rw-r--r--   0        0        0    22803 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/distance_measures.py
+-rw-r--r--   0        0        0     6872 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/distance_regular.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/dominance.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/dominating.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/efficiency_measures.py
+-rw-r--r--   0        0        0    13602 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/euler.py
+-rw-r--r--   0        0        0    11392 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/graph_hashing.py
+-rw-r--r--   0        0        0    13449 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/graphical.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/hierarchy.py
+-rw-r--r--   0        0        0     6152 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/hybrid.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/isolate.py
+-rw-r--r--   0        0        0    19792 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/link_prediction.py
+-rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/lowest_common_ancestors.py
+-rw-r--r--   0        0        0    42801 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/matching.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/mis.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/moral.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/non_randomness.py
+-rw-r--r--   0        0        0    16320 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/planar_drawing.py
+-rw-r--r--   0        0        0    39410 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/planarity.py
+-rw-r--r--   0        0        0    10826 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/polynomials.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/reciprocity.py
+-rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/regular.py
+-rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/richclub.py
+-rw-r--r--   0        0        0    59768 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/similarity.py
+-rw-r--r--   0        0        0    30243 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/simple_paths.py
+-rw-r--r--   0        0        0    13085 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/smallworld.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/smetric.py
+-rw-r--r--   0        0        0    10038 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/sparsifiers.py
+-rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/structuralholes.py
+-rw-r--r--   0        0        0    22926 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/summarization.py
+-rw-r--r--   0        0        0     9819 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/swap.py
+-rw-r--r--   0        0        0    31010 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/threshold.py
+-rw-r--r--   0        0        0    11584 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/tournament.py
+-rw-r--r--   0        0        0    13476 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/triads.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/vitality.py
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/voronoi.py
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/wiener.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/__init__.py
+-rw-r--r--   0        0        0     7181 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/clique.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/clustering_coefficient.py
+-rw-r--r--   0        0        0    12716 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/connectivity.py
+-rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/distance_measures.py
+-rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/dominating_set.py
+-rw-r--r--   0        0        0    13223 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/kcomponents.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/matching.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/maxcut.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/ramsey.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/steinertree.py
+-rw-r--r--   0        0        0    54262 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/traveling_salesman.py
+-rw-r--r--   0        0        0     8106 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/treewidth.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/vertex_cover.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/assortativity/__init__.py
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/assortativity/connectivity.py
+-rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/assortativity/correlation.py
+-rw-r--r--   0        0        0     9094 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/assortativity/mixing.py
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/assortativity/neighbor_degree.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/assortativity/pairs.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/__init__.py
+-rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/basic.py
+-rw-r--r--   0        0        0     8412 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/centrality.py
+-rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/cluster.py
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/covering.py
+-rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/edgelist.py
+-rw-r--r--   0        0        0    19961 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/generators.py
+-rw-r--r--   0        0        0    21273 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/matching.py
+-rw-r--r--   0        0        0     6382 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/matrix.py
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/projection.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/redundancy.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/spectral.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/__init__.py
+-rw-r--r--   0        0        0    14324 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/betweenness.py
+-rw-r--r--   0        0        0     9655 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/betweenness_subset.py
+-rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/closeness.py
+-rw-r--r--   0        0        0    11766 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/current_flow_betweenness.py
+-rw-r--r--   0        0        0     7976 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/current_flow_betweenness_subset.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/current_flow_closeness.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/degree_alg.py
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/dispersion.py
+-rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/eigenvector.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/flow_matrix.py
+-rw-r--r--   0        0        0    27731 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/group.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/harmonic.py
+-rw-r--r--   0        0        0    10674 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/katz.py
+-rw-r--r--   0        0        0     6801 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/load.py
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/percolation.py
+-rw-r--r--   0        0        0     6947 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/reaching.py
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/second_order.py
+-rw-r--r--   0        0        0     9506 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/subgraph_alg.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/trophic.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/voterank_alg.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/coloring/__init__.py
+-rw-r--r--   0        0        0    16571 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/coloring/equitable_coloring.py
+-rw-r--r--   0        0        0    19573 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/coloring/greedy_coloring.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/__init__.py
+-rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/asyn_fluid.py
+-rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/centrality.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/community_utils.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/kclique.py
+-rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/kernighan_lin.py
+-rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/label_propagation.py
+-rw-r--r--   0        0        0    13682 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/louvain.py
+-rw-r--r--   0        0        0     8048 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/lukes.py
+-rw-r--r--   0        0        0    19281 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/modularity_max.py
+-rw-r--r--   0        0        0    14610 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/quality.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/components/__init__.py
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/components/attracting.py
+-rw-r--r--   0        0        0    12501 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/components/biconnected.py
+-rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/components/connected.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/components/semiconnected.py
+-rw-r--r--   0        0        0    11896 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/components/strongly_connected.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/components/weakly_connected.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/connectivity/__init__.py
+-rw-r--r--   0        0        0    29734 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/connectivity/connectivity.py
+-rw-r--r--   0        0        0    22640 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/connectivity/cuts.py
+-rw-r--r--   0        0        0    14425 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/connectivity/disjoint_paths.py
+-rw-r--r--   0        0        0    43788 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/connectivity/edge_augmentation.py
+-rw-r--r--   0        0        0    20687 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/connectivity/edge_kcomponents.py
+-rw-r--r--   0        0        0     8222 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/connectivity/kcomponents.py
+-rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/connectivity/kcutsets.py
+-rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/connectivity/stoerwagner.py
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/connectivity/utils.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/__init__.py
+-rw-r--r--   0        0        0    13238 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/boykovkolmogorov.py
+-rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/capacityscaling.py
+-rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/dinitz_alg.py
+-rw-r--r--   0        0        0     7956 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/edmondskarp.py
+-rw-r--r--   0        0        0     6267 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/gomory_hu.py
+-rw-r--r--   0        0        0    22715 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/maxflow.py
+-rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/mincost.py
+-rw-r--r--   0        0        0    25089 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/networksimplex.py
+-rw-r--r--   0        0        0    15621 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/preflowpush.py
+-rw-r--r--   0        0        0    10272 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/shortestaugmentingpath.py
+-rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/utils.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/isomorphism/__init__.py
+-rw-r--r--   0        0        0    43599 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/isomorphism/ismags.py
+-rw-r--r--   0        0        0     6382 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/isomorphism/isomorph.py
+-rw-r--r--   0        0        0    40556 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/isomorphism/isomorphvf2.py
+-rw-r--r--   0        0        0    10936 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/isomorphism/matchhelpers.py
+-rw-r--r--   0        0        0    10949 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/isomorphism/temporalisomorphvf2.py
+-rw-r--r--   0        0        0     9258 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/isomorphism/tree_isomorphism.py
+-rw-r--r--   0        0        0     7496 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/isomorphism/vf2userfunc.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/link_analysis/__init__.py
+-rw-r--r--   0        0        0    11889 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/link_analysis/hits_alg.py
+-rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/link_analysis/pagerank_alg.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/minors/__init__.py
+-rw-r--r--   0        0        0    21714 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/minors/contraction.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/node_classification/__init__.py
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/node_classification/hmn.py
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/node_classification/lgc.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/node_classification/utils.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/operators/__init__.py
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/operators/all.py
+-rw-r--r--   0        0        0    12902 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/operators/binary.py
+-rw-r--r--   0        0        0    13857 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/operators/product.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/operators/unary.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/shortest_paths/__init__.py
+-rw-r--r--   0        0        0     6990 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/shortest_paths/astar.py
+-rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/shortest_paths/dense.py
+-rw-r--r--   0        0        0    20139 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/shortest_paths/generic.py
+-rw-r--r--   0        0        0    14928 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/shortest_paths/unweighted.py
+-rw-r--r--   0        0        0    80039 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/shortest_paths/weighted.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/traversal/__init__.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/traversal/beamsearch.py
+-rw-r--r--   0        0        0    14161 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/traversal/breadth_first_search.py
+-rw-r--r--   0        0        0    12842 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/traversal/depth_first_search.py
+-rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/traversal/edgebfs.py
+-rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/traversal/edgedfs.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/tree/__init__.py
+-rw-r--r--   0        0        0    36255 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/tree/branchings.py
+-rw-r--r--   0        0        0    12987 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/tree/coding.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/tree/decomposition.py
+-rw-r--r--   0        0        0    39261 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/tree/mst.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/tree/operations.py
+-rw-r--r--   0        0        0     7497 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/algorithms/tree/recognition.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/classes/__init__.py
+-rw-r--r--   0        0        0    15471 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/classes/coreviews.py
+-rw-r--r--   0        0        0    44427 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/classes/digraph.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/classes/filters.py
+-rw-r--r--   0        0        0    36626 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/classes/function.py
+-rw-r--r--   0        0        0    66826 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/classes/graph.py
+-rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/classes/graphviews.py
+-rw-r--r--   0        0        0    35867 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/classes/multidigraph.py
+-rw-r--r--   0        0        0    45810 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/classes/multigraph.py
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/classes/ordered.py
+-rw-r--r--   0        0        0    45714 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/classes/reportviews.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/drawing/__init__.py
+-rw-r--r--   0        0        0    35778 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/drawing/layout.py
+-rw-r--r--   0        0        0    15396 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/drawing/nx_agraph.py
+-rw-r--r--   0        0        0    14091 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/drawing/nx_pydot.py
+-rw-r--r--   0        0        0    48373 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/drawing/nx_pylab.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/__init__.py
+-rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/atlas.dat.gz
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/atlas.py
+-rw-r--r--   0        0        0    23801 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/classic.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/cographs.py
+-rw-r--r--   0        0        0    34429 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/community.py
+-rw-r--r--   0        0        0    29817 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/degree_seq.py
+-rw-r--r--   0        0        0    16676 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/directed.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/duplication.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/ego.py
+-rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/expanders.py
+-rw-r--r--   0        0        0    29482 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/geometric.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/harary_graph.py
+-rw-r--r--   0        0        0    14128 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/internet_as_graphs.py
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/intersection.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/interval_graph.py
+-rw-r--r--   0        0        0    24785 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/joint_degree_seq.py
+-rw-r--r--   0        0        0    13223 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/lattice.py
+-rw-r--r--   0        0        0    17654 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/line.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/mycielski.py
+-rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/nonisomorphic_trees.py
+-rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/random_clustered.py
+-rw-r--r--   0        0        0    44337 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/random_graphs.py
+-rw-r--r--   0        0        0    30426 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/small.py
+-rw-r--r--   0        0        0    22759 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/social.py
+-rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/spectral_graph_forge.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/stochastic.py
+-rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/sudoku.py
+-rw-r--r--   0        0        0    14146 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/trees.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/generators/triads.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/linalg/__init__.py
+-rw-r--r--   0        0        0    18281 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/linalg/algebraicconnectivity.py
+-rw-r--r--   0        0        0    15658 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/linalg/attrmatrix.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/linalg/bethehessianmatrix.py
+-rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/linalg/graphmatrix.py
+-rw-r--r--   0        0        0    13986 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/linalg/laplacianmatrix.py
+-rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/linalg/modularitymatrix.py
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/linalg/spectrum.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/__init__.py
+-rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/adjlist.py
+-rw-r--r--   0        0        0    14079 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/edgelist.py
+-rw-r--r--   0        0        0    39511 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/gexf.py
+-rw-r--r--   0        0        0    30016 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/gml.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/gpickle.py
+-rw-r--r--   0        0        0    11301 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/graph6.py
+-rw-r--r--   0        0        0    39163 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/graphml.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/leda.py
+-rw-r--r--   0        0        0    11201 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/multiline_adjlist.py
+-rw-r--r--   0        0        0    12183 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/nx_shp.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/nx_yaml.py
+-rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/p2g.py
+-rw-r--r--   0        0        0     8636 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/pajek.py
+-rw-r--r--   0        0        0    10217 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/sparse6.py
+-rw-r--r--   0        0        0     6498 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/text.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/json_graph/__init__.py
+-rw-r--r--   0        0        0     4745 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/json_graph/adjacency.py
+-rw-r--r--   0        0        0     8142 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/json_graph/cytoscape.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/json_graph/jit.py
+-rw-r--r--   0        0        0    11619 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/json_graph/node_link.py
+-rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/readwrite/json_graph/tree.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/testing/__init__.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/testing/test.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/testing/utils.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/utils/__init__.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/utils/contextmanagers.py
+-rw-r--r--   0        0        0    46493 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/utils/decorators.py
+-rw-r--r--   0        0        0    10391 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/utils/heaps.py
+-rw-r--r--   0        0        0     9138 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/utils/mapped_queue.py
+-rw-r--r--   0        0        0    20390 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/utils/misc.py
+-rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/utils/random_sequence.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/utils/rcm.py
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 dsr_shelx-239/src/dsr_shelx/networkx/utils/union_find.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 dsr_shelx-239/.gitignore
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 dsr_shelx-239/README.md
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 dsr_shelx-239/pyproject.toml
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 dsr_shelx-239/PKG-INFO
```

### Comparing `dsr_shelx-238/.gitattributes` & `dsr_shelx-239/.gitattributes`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/README` & `dsr_shelx-239/README`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/example/p21c.hkl` & `dsr_shelx-239/example/p21c.hkl`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/example/p21c.res` & `dsr_shelx-239/example/p21c.res`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/example/p21c_final.res` & `dsr_shelx-239/example/p21c_final.res`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/example/p21c_step0.res` & `dsr_shelx-239/example/p21c_step0.res`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/example/p21c_step1.res` & `dsr_shelx-239/example/p21c_step1.res`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/example/p21c_step2.ins` & `dsr_shelx-239/example/p21c_step2.ins`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/example/p21c_step3.res` & `dsr_shelx-239/example/p21c_step3.res`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/example/p21n_cf3.hkl` & `dsr_shelx-239/example/p21n_cf3.hkl`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/example/p21n_cf3.ins` & `dsr_shelx-239/example/p21n_cf3.ins`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/example/p21n_cf3.res` & `dsr_shelx-239/example/p21n_cf3.res`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/afix.py` & `dsr_shelx-239/src/dsr_shelx/afix.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/atomhandling.py` & `dsr_shelx-239/src/dsr_shelx/atomhandling.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/atoms.py` & `dsr_shelx-239/src/dsr_shelx/atoms.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/cf3fit.py` & `dsr_shelx-239/src/dsr_shelx/cf3fit.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/constants.py` & `dsr_shelx-239/src/dsr_shelx/constants.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/dbfile.py` & `dsr_shelx-239/src/dsr_shelx/dbfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 
 import os
 import re
 import sys
 import tarfile
 from copy import deepcopy
+from pathlib import Path
 from typing import List, Dict
 
 from atomhandling import get_atomtypes
 from atoms import Element
 from constants import atomregex, SHX_CARDS, RESTRAINT_CARDS, sep_line
 from misc import atomic_distance, nalimov_test, std_dev, median, pairwise, \
     unwrap_head_lines, dice_coefficient2, frac_to_cart
@@ -1109,14 +1110,24 @@
         """
         warns for import errors
         """
         print('*** Unable to import GRADE file {} GRADE import to DSR '
               'relies on GRADE v1.100 and up. ***'.format(filename))
         sys.exit()
 
+    def format_atomlist(self, atomlist: List[str]) -> List[str]:
+        formatted_list = []
+        for y in atomlist:
+            atom_name = y[1]
+            atom_name = ''.join([x for x in atom_name if x.isalpha()])
+            formatted_string = f'{y[0]:<6} -{self.el.get_atomic_number(atom_name)}  {float(y[2]):>8.3f}' \
+                               f'{float(y[3]):>8.3f}{float(y[4]):>8.3f}'
+            formatted_list.append(formatted_string)
+        return formatted_list
+
     def write_user_database(self):
         """
         writes content of existing dsr_user_db.txt and the imported GRADE entry to
         the dsr_user_db.txt
         """
         fragments = list(self._db)
         imported_entry = self.bild_grade_db_entry()
@@ -1125,52 +1136,54 @@
         for i in fragments:
             if self._db[i]['dbname'] == 'dsr_user_db':
                 user_db_names.append(self._db[i]['name'])
         # try to write the new dbentry:
         try:
             with open(self.user_db_path, 'w') as f:
                 for name in grade_db_names:
-                    print('Importing {} ({}) to user database...'.format(self._resi_name, name))
-                    atomlist = imported_entry[name]['atoms']
-                    comments = imported_entry[name]['comments']
-                    comments = '\n'.join([' '.join(i) for i in comments if i])
-                    head = '\n'.join([' '.join(x) for x in imported_entry[name]['restraints']])
-                    atoms = '\n'.join(['{:<6} -{}  {:>8.3f}{:>8.3f}{:>8.3f}' \
-                                      .format(y[0], self.el.get_atomic_number(y[1]), float(y[2]), float(y[3]),
-                                              float(y[4])) for y in atomlist])
-                    resi_name = str(name)
-                    cell = '  '.join(imported_entry[name]['cell'])
-                    dbentry = '<{}> \n{} \nRESI {} \n{} \n{} \n{} \n</{}>\n''\
-                        '.format(resi_name, comments, resi_name, head, cell, atoms, resi_name)
+                    print(f'Importing {self._resi_name} ({name}) to user database...')
+                    dbentry = self.compile_dbentry(imported_entry, name)
                     f.write(dbentry)
         except IOError as e:
             print(e)
             sys.exit()
         # try to write existing dbentries:
         try:
             with open(self.user_db_path, 'a+') as fu:
                 for tag in fragments:
                     if self._db[tag]['dbname'] == 'dsr_user_db':
                         atomlist = self._db[tag]['atoms']
                         head = '\n'.join([''.join(x) for x in self._db[tag]['restraints']])
-                        atoms = '\n'.join(['{:<6}{:<2}{:>8.3f}{:>8.3f}{:>8.3f}'
-                                          .format(y[0], y[1], float(y[2]), float(y[3]), float(y[4])) for y in atomlist])
+                        atoms = '\n'.join([f'{y[0]:<6}{y[1]:<2}{float(y[2]):>8.3f}'
+                                           f'{float(y[3]):>8.3f}{float(y[4]):>8.3f}' for y in atomlist])
                         resi_name = self._db[tag]['resi']
                         comments = '\n'.join(self._db[tag]['comments'])
                         name = self._db[tag]['name']
                         comments = "REM Name: {}\n{}".format(name, comments)
                         fragline = 'FRAG 17 {} {} {} {} {} {}'.format(*self._db[tag]['cell'])
-                        dbentry = '\n<{}> \n{} \nRESI {} \n{} \n{} \n{} \n</{}>\n' \
-                                  ''.format(tag, comments, resi_name, head, fragline, atoms, tag)
+                        dbentry = (f'\n<{tag}> \n{comments} \nRESI {resi_name} \n'
+                                   f'{head} \n{fragline} \n{atoms} \n</{tag}>\n')
                         fu.write(dbentry)
         except IOError as e:
             print(e)
             sys.exit()
         print('User database successfully updated.')
 
+    def compile_dbentry(self, imported_entry: dict, name: str) -> str:
+        atomlist = imported_entry[name]['atoms']
+        comments = imported_entry[name]['comments']
+        comments = '\n'.join([' '.join(i) for i in comments if i])
+        head = '\n'.join([' '.join(x) for x in imported_entry[name]['restraints']])
+        atoms = '\n'.join(self.format_atomlist(atomlist))
+        resi_name = str(name)
+        cell = '  '.join(imported_entry[name]['cell'])
+        dbentry = (f'<{resi_name}> \n{comments} \nRESI {resi_name} \n'
+                   f'{head} \n{cell} \n{atoms} \n</{resi_name}>\n')
+        return dbentry
+
 
 if __name__ == '__main__':
     """
     import doctest
     failed, attempted = doctest.testmod()  # verbose=True)
     if failed == 0:
         print('passed all {} tests!'.format(attempted))
```

### Comparing `dsr_shelx-238/src/dsr_shelx/dsr.bat` & `dsr_shelx-239/src/dsr_shelx/dsr.bat`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/dsr.py` & `dsr_shelx-239/src/dsr_shelx/dsr.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/dsr_db.txt` & `dsr_shelx-239/src/dsr_shelx/dsr_db.txt`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/dsrparse.py` & `dsr_shelx-239/src/dsr_shelx/dsrparse.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/elements.py` & `dsr_shelx-239/src/dsr_shelx/elements.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/export.py` & `dsr_shelx-239/src/dsr_shelx/export.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/misc.py` & `dsr_shelx-239/src/dsr_shelx/misc.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/olex_dsr_db.txt` & `dsr_shelx-239/src/dsr_shelx/olex_dsr_db.txt`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/options.py` & `dsr_shelx-239/src/dsr_shelx/options.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/pyperclip.py` & `dsr_shelx-239/src/dsr_shelx/pyperclip.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/refine.py` & `dsr_shelx-239/src/dsr_shelx/refine.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/resfile.py` & `dsr_shelx-239/src/dsr_shelx/resfile.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/resi.py` & `dsr_shelx-239/src/dsr_shelx/resi.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/restraints.py` & `dsr_shelx-239/src/dsr_shelx/restraints.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/selfupdate.py` & `dsr_shelx-239/src/dsr_shelx/selfupdate.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/sql_export.py` & `dsr_shelx-239/src/dsr_shelx/sql_export.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/terminalsize.py` & `dsr_shelx-239/src/dsr_shelx/terminalsize.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/fit/LICENSE.txt` & `dsr_shelx-239/src/dsr_shelx/fit/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/fit/quatfit.py` & `dsr_shelx-239/src/dsr_shelx/fit/quatfit.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/__init__.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/ctx_base.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/ctx_base.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/ctx_fp.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/ctx_fp.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/ctx_iv.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/ctx_iv.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/ctx_mp.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/ctx_mp.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/ctx_mp_python.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/ctx_mp_python.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/function_docs.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/function_docs.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/identification.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/identification.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/math2.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/math2.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/rational.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/rational.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/usertools.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/usertools.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/visualization.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/visualization.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/calculus/approximation.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/calculus/approximation.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/calculus/differentiation.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/calculus/differentiation.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/calculus/extrapolation.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/calculus/extrapolation.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/calculus/inverselaplace.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/calculus/inverselaplace.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/calculus/odes.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/calculus/odes.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/calculus/optimization.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/calculus/optimization.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/calculus/polynomials.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/calculus/polynomials.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/calculus/quadrature.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/calculus/quadrature.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/functions/bessel.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/functions/bessel.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/functions/elliptic.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/functions/elliptic.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/functions/expintegrals.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/functions/expintegrals.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/functions/factorials.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/functions/factorials.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/functions/functions.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/functions/functions.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/functions/hypergeometric.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/functions/hypergeometric.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/functions/orthogonal.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/functions/orthogonal.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/functions/qfunctions.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/functions/qfunctions.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/functions/rszeta.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/functions/rszeta.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/functions/theta.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/functions/theta.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/functions/zeta.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/functions/zeta.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/functions/zetazeros.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/functions/zetazeros.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/libmp/__init__.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/libmp/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/libmp/backend.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/libmp/backend.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/libmp/gammazeta.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/libmp/gammazeta.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libelefun.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/libmp/libelefun.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libhyper.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/libmp/libhyper.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libintmath.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/libmp/libintmath.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libmpc.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/libmp/libmpc.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libmpf.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/libmp/libmpf.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libmpi.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/libmp/libmpi.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/matrices/calculus.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/matrices/calculus.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/matrices/eigen.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/matrices/eigen.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/matrices/eigen_symmetric.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/matrices/eigen_symmetric.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/matrices/linalg.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/matrices/linalg.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/mpmath/matrices/matrices.py` & `dsr_shelx-239/src/dsr_shelx/mpmath/matrices/matrices.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/__init__.py` & `dsr_shelx-239/src/dsr_shelx/networkx/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/conftest.py` & `dsr_shelx-239/src/dsr_shelx/networkx/conftest.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/convert.py` & `dsr_shelx-239/src/dsr_shelx/networkx/convert.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/convert_matrix.py` & `dsr_shelx-239/src/dsr_shelx/networkx/convert_matrix.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/exception.py` & `dsr_shelx-239/src/dsr_shelx/networkx/exception.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/lazy_imports.py` & `dsr_shelx-239/src/dsr_shelx/networkx/lazy_imports.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/relabel.py` & `dsr_shelx-239/src/dsr_shelx/networkx/relabel.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/__init__.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/asteroidal.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/asteroidal.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/boundary.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/boundary.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bridges.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bridges.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/chains.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/chains.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/chordal.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/chordal.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/clique.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/clique.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/cluster.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/cluster.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/communicability_alg.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/communicability_alg.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/core.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/core.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/covering.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/covering.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/cuts.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/cuts.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/cycles.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/cycles.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/d_separation.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/d_separation.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/dag.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/dag.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/distance_measures.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/distance_measures.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/distance_regular.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/distance_regular.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/dominance.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/dominance.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/dominating.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/dominating.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/efficiency_measures.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/efficiency_measures.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/euler.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/euler.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/graph_hashing.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/graph_hashing.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/graphical.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/graphical.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/hierarchy.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/hierarchy.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/hybrid.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/hybrid.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isolate.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/isolate.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/link_prediction.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/link_prediction.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/lowest_common_ancestors.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/lowest_common_ancestors.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/matching.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/matching.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/mis.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/mis.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/moral.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/moral.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/non_randomness.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/non_randomness.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/planar_drawing.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/planar_drawing.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/planarity.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/planarity.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/polynomials.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/polynomials.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/reciprocity.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/reciprocity.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/regular.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/regular.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/richclub.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/richclub.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/similarity.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/similarity.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/simple_paths.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/simple_paths.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/smallworld.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/smallworld.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/smetric.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/smetric.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/sparsifiers.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/sparsifiers.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/structuralholes.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/structuralholes.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/summarization.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/summarization.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/swap.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/swap.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/threshold.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/threshold.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tournament.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/tournament.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/triads.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/triads.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/vitality.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/vitality.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/voronoi.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/voronoi.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/wiener.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/wiener.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/__init__.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/clique.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/clique.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/clustering_coefficient.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/clustering_coefficient.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/connectivity.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/connectivity.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/distance_measures.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/distance_measures.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/dominating_set.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/dominating_set.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/kcomponents.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/kcomponents.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/matching.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/matching.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/maxcut.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/maxcut.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/ramsey.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/ramsey.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/steinertree.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/steinertree.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/traveling_salesman.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/traveling_salesman.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/treewidth.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/treewidth.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/vertex_cover.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/approximation/vertex_cover.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/connectivity.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/assortativity/connectivity.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/correlation.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/assortativity/correlation.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/mixing.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/assortativity/mixing.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/neighbor_degree.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/assortativity/neighbor_degree.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/pairs.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/assortativity/pairs.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/__init__.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/basic.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/basic.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/centrality.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/centrality.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/cluster.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/cluster.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/covering.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/covering.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/edgelist.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/edgelist.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/generators.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/generators.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/matching.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/matching.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/matrix.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/matrix.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/projection.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/projection.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/redundancy.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/redundancy.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/spectral.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/bipartite/spectral.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/__init__.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/betweenness.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/betweenness.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/betweenness_subset.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/betweenness_subset.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/closeness.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/closeness.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/current_flow_betweenness.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/current_flow_betweenness.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/current_flow_betweenness_subset.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/current_flow_betweenness_subset.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/current_flow_closeness.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/current_flow_closeness.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/degree_alg.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/degree_alg.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/dispersion.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/dispersion.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/eigenvector.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/eigenvector.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/flow_matrix.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/flow_matrix.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/group.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/group.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/harmonic.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/harmonic.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/katz.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/katz.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/load.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/load.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/percolation.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/percolation.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/reaching.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/reaching.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/second_order.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/second_order.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/subgraph_alg.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/subgraph_alg.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/trophic.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/trophic.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/voterank_alg.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/centrality/voterank_alg.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/coloring/equitable_coloring.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/coloring/equitable_coloring.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/coloring/greedy_coloring.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/coloring/greedy_coloring.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/__init__.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/asyn_fluid.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/asyn_fluid.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/centrality.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/centrality.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/community_utils.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/community_utils.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/kclique.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/kclique.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/kernighan_lin.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/kernighan_lin.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/label_propagation.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/label_propagation.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/louvain.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/louvain.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/lukes.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/lukes.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/modularity_max.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/modularity_max.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/quality.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/community/quality.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/attracting.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/components/attracting.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/biconnected.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/components/biconnected.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/connected.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/components/connected.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/semiconnected.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/components/semiconnected.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/strongly_connected.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/components/strongly_connected.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/weakly_connected.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/components/weakly_connected.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/connectivity.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/connectivity/connectivity.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/cuts.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/connectivity/cuts.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/disjoint_paths.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/connectivity/disjoint_paths.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/edge_augmentation.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/connectivity/edge_augmentation.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/edge_kcomponents.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/connectivity/edge_kcomponents.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/kcomponents.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/connectivity/kcomponents.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/kcutsets.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/connectivity/kcutsets.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/stoerwagner.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/connectivity/stoerwagner.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/utils.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/connectivity/utils.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/boykovkolmogorov.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/boykovkolmogorov.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/capacityscaling.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/capacityscaling.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/dinitz_alg.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/dinitz_alg.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/edmondskarp.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/edmondskarp.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/gomory_hu.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/gomory_hu.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/maxflow.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/maxflow.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/mincost.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/mincost.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/networksimplex.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/networksimplex.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/preflowpush.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/preflowpush.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/shortestaugmentingpath.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/shortestaugmentingpath.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/utils.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/flow/utils.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/ismags.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/isomorphism/ismags.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/isomorph.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/isomorphism/isomorph.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/isomorphvf2.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/isomorphism/isomorphvf2.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/matchhelpers.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/isomorphism/matchhelpers.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/temporalisomorphvf2.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/isomorphism/temporalisomorphvf2.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/tree_isomorphism.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/isomorphism/tree_isomorphism.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/vf2userfunc.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/isomorphism/vf2userfunc.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/link_analysis/hits_alg.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/link_analysis/hits_alg.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/link_analysis/pagerank_alg.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/link_analysis/pagerank_alg.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/minors/__init__.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/minors/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/minors/contraction.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/minors/contraction.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/node_classification/__init__.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/node_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/node_classification/hmn.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/node_classification/hmn.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/node_classification/lgc.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/node_classification/lgc.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/node_classification/utils.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/node_classification/utils.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/operators/all.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/operators/all.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/operators/binary.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/operators/binary.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/operators/product.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/operators/product.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/operators/unary.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/operators/unary.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/astar.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/shortest_paths/astar.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/dense.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/shortest_paths/dense.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/generic.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/shortest_paths/generic.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/unweighted.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/shortest_paths/unweighted.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/weighted.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/shortest_paths/weighted.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/beamsearch.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/traversal/beamsearch.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/breadth_first_search.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/traversal/breadth_first_search.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/depth_first_search.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/traversal/depth_first_search.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/edgebfs.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/traversal/edgebfs.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/edgedfs.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/traversal/edgedfs.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/branchings.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/tree/branchings.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/coding.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/tree/coding.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/decomposition.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/tree/decomposition.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/mst.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/tree/mst.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/operations.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/tree/operations.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/recognition.py` & `dsr_shelx-239/src/dsr_shelx/networkx/algorithms/tree/recognition.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/classes/coreviews.py` & `dsr_shelx-239/src/dsr_shelx/networkx/classes/coreviews.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/classes/digraph.py` & `dsr_shelx-239/src/dsr_shelx/networkx/classes/digraph.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/classes/filters.py` & `dsr_shelx-239/src/dsr_shelx/networkx/classes/filters.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/classes/function.py` & `dsr_shelx-239/src/dsr_shelx/networkx/classes/function.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/classes/graph.py` & `dsr_shelx-239/src/dsr_shelx/networkx/classes/graph.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/classes/graphviews.py` & `dsr_shelx-239/src/dsr_shelx/networkx/classes/graphviews.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/classes/multidigraph.py` & `dsr_shelx-239/src/dsr_shelx/networkx/classes/multidigraph.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/classes/multigraph.py` & `dsr_shelx-239/src/dsr_shelx/networkx/classes/multigraph.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/classes/ordered.py` & `dsr_shelx-239/src/dsr_shelx/networkx/classes/ordered.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/classes/reportviews.py` & `dsr_shelx-239/src/dsr_shelx/networkx/classes/reportviews.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/drawing/layout.py` & `dsr_shelx-239/src/dsr_shelx/networkx/drawing/layout.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/drawing/nx_agraph.py` & `dsr_shelx-239/src/dsr_shelx/networkx/drawing/nx_agraph.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/drawing/nx_pydot.py` & `dsr_shelx-239/src/dsr_shelx/networkx/drawing/nx_pydot.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/drawing/nx_pylab.py` & `dsr_shelx-239/src/dsr_shelx/networkx/drawing/nx_pylab.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/__init__.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/atlas.dat.gz` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/atlas.dat.gz`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/atlas.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/atlas.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/classic.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/classic.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/cographs.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/cographs.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/community.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/community.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/degree_seq.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/degree_seq.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/directed.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/directed.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/duplication.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/duplication.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/ego.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/ego.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/expanders.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/expanders.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/geometric.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/geometric.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/harary_graph.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/harary_graph.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/internet_as_graphs.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/internet_as_graphs.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/intersection.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/intersection.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/interval_graph.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/interval_graph.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/joint_degree_seq.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/joint_degree_seq.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/lattice.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/lattice.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/line.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/line.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/mycielski.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/mycielski.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/nonisomorphic_trees.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/nonisomorphic_trees.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/random_clustered.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/random_clustered.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/random_graphs.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/random_graphs.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/small.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/small.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/social.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/social.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/spectral_graph_forge.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/spectral_graph_forge.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/stochastic.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/stochastic.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/sudoku.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/sudoku.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/trees.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/trees.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/generators/triads.py` & `dsr_shelx-239/src/dsr_shelx/networkx/generators/triads.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/linalg/__init__.py` & `dsr_shelx-239/src/dsr_shelx/networkx/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/linalg/algebraicconnectivity.py` & `dsr_shelx-239/src/dsr_shelx/networkx/linalg/algebraicconnectivity.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/linalg/attrmatrix.py` & `dsr_shelx-239/src/dsr_shelx/networkx/linalg/attrmatrix.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/linalg/bethehessianmatrix.py` & `dsr_shelx-239/src/dsr_shelx/networkx/linalg/bethehessianmatrix.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/linalg/graphmatrix.py` & `dsr_shelx-239/src/dsr_shelx/networkx/linalg/graphmatrix.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/linalg/laplacianmatrix.py` & `dsr_shelx-239/src/dsr_shelx/networkx/linalg/laplacianmatrix.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/linalg/modularitymatrix.py` & `dsr_shelx-239/src/dsr_shelx/networkx/linalg/modularitymatrix.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/linalg/spectrum.py` & `dsr_shelx-239/src/dsr_shelx/networkx/linalg/spectrum.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/__init__.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/adjlist.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/adjlist.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/edgelist.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/edgelist.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/gexf.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/gexf.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/gml.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/gml.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/gpickle.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/gpickle.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/graph6.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/graph6.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/graphml.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/graphml.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/leda.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/leda.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/multiline_adjlist.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/multiline_adjlist.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/nx_shp.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/nx_shp.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/nx_yaml.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/nx_yaml.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/p2g.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/p2g.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/pajek.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/pajek.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/sparse6.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/sparse6.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/text.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/text.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/__init__.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/json_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/adjacency.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/json_graph/adjacency.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/cytoscape.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/json_graph/cytoscape.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/jit.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/json_graph/jit.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/node_link.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/json_graph/node_link.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/tree.py` & `dsr_shelx-239/src/dsr_shelx/networkx/readwrite/json_graph/tree.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/testing/test.py` & `dsr_shelx-239/src/dsr_shelx/networkx/testing/test.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/testing/utils.py` & `dsr_shelx-239/src/dsr_shelx/networkx/testing/utils.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/utils/contextmanagers.py` & `dsr_shelx-239/src/dsr_shelx/networkx/utils/contextmanagers.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/utils/decorators.py` & `dsr_shelx-239/src/dsr_shelx/networkx/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/utils/heaps.py` & `dsr_shelx-239/src/dsr_shelx/networkx/utils/heaps.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/utils/mapped_queue.py` & `dsr_shelx-239/src/dsr_shelx/networkx/utils/mapped_queue.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/utils/misc.py` & `dsr_shelx-239/src/dsr_shelx/networkx/utils/misc.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/utils/random_sequence.py` & `dsr_shelx-239/src/dsr_shelx/networkx/utils/random_sequence.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/utils/rcm.py` & `dsr_shelx-239/src/dsr_shelx/networkx/utils/rcm.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/src/dsr_shelx/networkx/utils/union_find.py` & `dsr_shelx-239/src/dsr_shelx/networkx/utils/union_find.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/.gitignore` & `dsr_shelx-239/.gitignore`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/README.md` & `dsr_shelx-239/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 * [The homepage](https://dkratzert.de/dsr.html)
 
 I apologize for the messy code. This was my first bigger project...
 
 You have either a command line version:
 ```
 C:\Users\daniel>dsr
------------------------------------------------------ D S R - v211 -------------------------------------
+----------------------------------------------------- D S R - v238 -------------------------------------
 Disordered Structure Refinement (DSR)
 
 Example DSR .res file command line:
 REM DSR PUT/REPLACE "Fragment" WITH C1 C2 C3 ON Q1 Q2 Q3 PART 1 OCC -21 =
   RESI DFIX
 ---------------------------------------------------------------------------------------------------------
    PUT:     Just put the fragment source atoms here.
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 SHELXL .res files. The user inserts a special command in the SHELXL .res file
 and the DSR program reads this information to put a molecule or fragment with
 the desired atoms on the position of the target atoms or q-peaks in the unit
 cell. Bond restraints can be either applied from the database to the molecule
 or automatically generated. * [The homepage](https://dkratzert.de/dsr.html) I
 apologize for the messy code. This was my first bigger project... You have
 either a command line version: ``` C:\Users\daniel>dsr ------------------------
------------------------------ D S R - v211 ------------------------------------
+----------------------------- D S R - v238 ------------------------------------
 - Disordered Structure Refinement (DSR) Example DSR .res file command line: REM
 DSR PUT/REPLACE "Fragment" WITH C1 C2 C3 ON Q1 Q2 Q3 PART 1 OCC -21 = RESI DFIX
 -------------------------------------------------------------------------------
 -------------------------- PUT: Just put the fragment source atoms here.
 REPLACE: Replace atoms of PART 0 in 1.3 A distance around target atoms. -------
 -------------------------------------------------------------------------------
 ------------------- optional arguments: -h, --help show this help message and
```

### Comparing `dsr_shelx-238/pyproject.toml` & `dsr_shelx-239/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dsr_shelx-238/PKG-INFO` & `dsr_shelx-239/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsr_shelx
-Version: 238
+Version: 239
 Summary: A program to model disorder in small-molecule X-ray structures
 Project-URL: Homepage, https://dkratzert.de/dsr.html
 Project-URL: Bug Tracker, https://github.com/dkratzert/DSR/issues
 Author-email: Daniel Kratzert <dkratzert@gmx.de>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,15 +35,15 @@
 * [The homepage](https://dkratzert.de/dsr.html)
 
 I apologize for the messy code. This was my first bigger project...
 
 You have either a command line version:
 ```
 C:\Users\daniel>dsr
------------------------------------------------------ D S R - v211 -------------------------------------
+----------------------------------------------------- D S R - v238 -------------------------------------
 Disordered Structure Refinement (DSR)
 
 Example DSR .res file command line:
 REM DSR PUT/REPLACE "Fragment" WITH C1 C2 C3 ON Q1 Q2 Q3 PART 1 OCC -21 =
   RESI DFIX
 ---------------------------------------------------------------------------------------------------------
    PUT:     Just put the fragment source atoms here.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dsr_shelx Version: 238 Summary: A program to model
+Metadata-Version: 2.1 Name: dsr_shelx Version: 239 Summary: A program to model
 disorder in small-molecule X-ray structures Project-URL: Homepage, https://
 dkratzert.de/dsr.html Project-URL: Bug Tracker, https://github.com/dkratzert/
 DSR/issues Author-email: Daniel Kratzert
 gmx.de> Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier: Topic
 :: Scientific/Engineering :: Chemistry Requires-Python: >=3.9 Description-
@@ -18,15 +18,15 @@
 command in the SHELXL .res file and the DSR program reads this information to
 put a molecule or fragment with the desired atoms on the position of the target
 atoms or q-peaks in the unit cell. Bond restraints can be either applied from
 the database to the molecule or automatically generated. * [The homepage]
 (https://dkratzert.de/dsr.html) I apologize for the messy code. This was my
 first bigger project... You have either a command line version: ``` C:
 \Users\daniel>dsr ----------------------------------------------------- D S R -
-v211 ------------------------------------- Disordered Structure Refinement
+v238 ------------------------------------- Disordered Structure Refinement
 (DSR) Example DSR .res file command line: REM DSR PUT/REPLACE "Fragment" WITH
 C1 C2 C3 ON Q1 Q2 Q3 PART 1 OCC -21 = RESI DFIX -------------------------------
 -------------------------------------------------------------------------- PUT:
 Just put the fragment source atoms here. REPLACE: Replace atoms of PART 0 in
 1.3 A distance around target atoms. -------------------------------------------
 -------------------------------------------------------------- optional
 arguments: -h, --help show this help message and exit -r "res file" ["res file"
```

