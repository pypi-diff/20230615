# Comparing `tmp/CellConstructor-1.3.1.tar.gz` & `tmp/CellConstructor-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CellConstructor-1.3.1.tar", last modified: Tue Jun  6 10:21:31 2023, max compression
+gzip compressed data, was "CellConstructor-1.3.2.tar", last modified: Mon Jun 12 08:59:45 2023, max compression
```

## Comparing `CellConstructor-1.3.1.tar` & `CellConstructor-1.3.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:21:31.103285 CellConstructor-1.3.1/
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:21:31.099285 CellConstructor-1.3.1/CModules/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3003 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/CModules/LinAlg.c
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      513 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/CModules/LinAlg.h
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1456 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/CModules/wrapper3.c
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:21:31.099285 CellConstructor-1.3.1/CellConstructor.egg-info/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      265 2023-06-06 10:21:31.000000 CellConstructor-1.3.1/CellConstructor.egg-info/PKG-INFO
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     2202 2023-06-06 10:21:31.000000 CellConstructor-1.3.1/CellConstructor.egg-info/SOURCES.txt
--rw-rw-r--   0 monacell  (1001) monacell  (1001)        1 2023-06-06 10:21:31.000000 CellConstructor-1.3.1/CellConstructor.egg-info/dependency_links.txt
--rw-rw-r--   0 monacell  (1001) monacell  (1001)       76 2023-06-06 10:21:31.000000 CellConstructor-1.3.1/CellConstructor.egg-info/top_level.txt
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:21:31.103285 CellConstructor-1.3.1/FModules/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     5987 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/constants.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3156 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/contract_two_phonon_propagator.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     2178 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/cryst_to_car.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    19129 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/eff_charge_interp.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      965 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/eqvect.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4087 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/error_handler.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     9261 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/fc_supercell_from_dyn.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      798 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/flush_unit.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     5008 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/from_matdyn.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    11598 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/get_equivalent_atoms.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      924 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/get_latvec.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    74669 2023-06-06 10:19:07.000000 CellConstructor-1.3.1/FModules/get_lf.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1352 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/get_q_grid_fast.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     5315 2023-06-06 10:19:07.000000 CellConstructor-1.3.1/FModules/get_scattering_q_grid.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      650 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/get_translations.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4802 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/interp.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1457 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/invmat.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3924 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/io_global.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     2825 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/kind.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     5974 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/q2qstar_out.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     2526 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/q_gen.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1888 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/recips.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     2456 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/rotate_and_add_dyn.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     9920 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/second_order_ASR.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     8148 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/second_order_centering.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    16589 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/set_asr.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1932 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/set_tau.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     2605 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/sgam_ph.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3484 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/smallgq.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4071 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/star_q.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     7243 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/symdynph_gq_new.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    37200 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/symm_base.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     2406 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/symm_matrix.f90
--rwxrwxr-x   0 monacell  (1001) monacell  (1001)    36499 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/symmetry_high_rank.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1652 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/symvector.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    14041 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/third_order_ASR.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    23138 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/third_order_centering.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    28528 2023-06-06 10:19:07.000000 CellConstructor-1.3.1/FModules/third_order_cond.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    30927 2023-06-06 10:19:07.000000 CellConstructor-1.3.1/FModules/third_order_cond_centering.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    19863 2023-06-06 10:19:07.000000 CellConstructor-1.3.1/FModules/third_order_dynbubble.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1030 2023-06-06 10:19:07.000000 CellConstructor-1.3.1/FModules/third_order_interpol.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1765 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/trntnsc.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1483 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/FModules/unwrap_tensors.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    35149 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/LICENSE.md
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      138 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/MANIFEST.in
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      265 2023-06-06 10:21:31.103285 CellConstructor-1.3.1/PKG-INFO
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     5484 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/README.md
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:21:31.103285 CellConstructor-1.3.1/cellconstructor/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     5067 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/cellconstructor/AnharmonicForceFields.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     8677 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/cellconstructor/Bands.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)   139731 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/cellconstructor/ForceTensor.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    63428 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/cellconstructor/Manipulate.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    75839 2023-06-06 10:19:07.000000 CellConstructor-1.3.1/cellconstructor/Methods.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     5568 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/cellconstructor/Moro_object.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)   185234 2023-02-15 11:33:51.000000 CellConstructor-1.3.1/cellconstructor/Phonons.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    13887 2023-02-15 11:18:26.000000 CellConstructor-1.3.1/cellconstructor/Settings.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    86900 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/cellconstructor/Spectral.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    85957 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/cellconstructor/Structure.py
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:21:31.103285 CellConstructor-1.3.1/cellconstructor/SymData/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      112 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/cellconstructor/SymData/15.dat
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      220 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/cellconstructor/SymData/36.dat
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      106 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/cellconstructor/SymData/36_red.dat
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      115 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/cellconstructor/SymData/60.dat
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      254 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/cellconstructor/SymData/64.bcs
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     2155 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/cellconstructor/SymData/64.dat
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1104 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/cellconstructor/SymData/convert_sym.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)   181899 2023-06-06 10:19:07.000000 CellConstructor-1.3.1/cellconstructor/ThermalConductivity.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     7242 2023-02-16 11:37:18.000000 CellConstructor-1.3.1/cellconstructor/Timer.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      963 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/cellconstructor/Units.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      641 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/cellconstructor/__init__.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    17679 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/cellconstructor/calculators.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)   111752 2023-02-15 11:37:20.000000 CellConstructor-1.3.1/cellconstructor/symmetries.py
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 10:21:31.103285 CellConstructor-1.3.1/scripts/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    32848 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/scripts/cellconstructor_test.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1629 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/scripts/symmetrize_dynmat.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      754 2023-02-13 14:55:58.000000 CellConstructor-1.3.1/scripts/view_scf_atoms.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)       38 2023-06-06 10:21:31.103285 CellConstructor-1.3.1/setup.cfg
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4457 2023-06-06 10:21:21.000000 CellConstructor-1.3.1/setup.py
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-12 08:59:45.038278 CellConstructor-1.3.2/
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-12 08:59:44.942276 CellConstructor-1.3.2/CModules/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3003 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/CModules/LinAlg.c
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      513 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/CModules/LinAlg.h
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1456 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/CModules/wrapper3.c
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-12 08:59:44.942276 CellConstructor-1.3.2/CellConstructor.egg-info/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      265 2023-06-12 08:59:44.000000 CellConstructor-1.3.2/CellConstructor.egg-info/PKG-INFO
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     2202 2023-06-12 08:59:44.000000 CellConstructor-1.3.2/CellConstructor.egg-info/SOURCES.txt
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)        1 2023-06-12 08:59:44.000000 CellConstructor-1.3.2/CellConstructor.egg-info/dependency_links.txt
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)       76 2023-06-12 08:59:44.000000 CellConstructor-1.3.2/CellConstructor.egg-info/top_level.txt
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-12 08:59:44.954276 CellConstructor-1.3.2/FModules/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     5987 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/constants.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3156 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/contract_two_phonon_propagator.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     2178 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/cryst_to_car.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    19129 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/eff_charge_interp.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      965 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/eqvect.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4087 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/error_handler.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     9261 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/fc_supercell_from_dyn.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      798 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/flush_unit.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     5008 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/from_matdyn.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    11598 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/get_equivalent_atoms.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      924 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/get_latvec.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    74669 2023-06-06 10:19:07.000000 CellConstructor-1.3.2/FModules/get_lf.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1352 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/get_q_grid_fast.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     5315 2023-06-06 10:19:07.000000 CellConstructor-1.3.2/FModules/get_scattering_q_grid.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      650 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/get_translations.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4802 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/interp.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1457 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/invmat.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3924 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/io_global.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     2825 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/kind.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     5974 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/q2qstar_out.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     2526 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/q_gen.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1888 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/recips.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     2456 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/rotate_and_add_dyn.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     9920 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/second_order_ASR.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     8148 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/second_order_centering.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    16589 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/set_asr.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1932 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/set_tau.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     2605 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/sgam_ph.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3484 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/smallgq.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4071 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/star_q.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     7243 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/symdynph_gq_new.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    37200 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/symm_base.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     2406 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/symm_matrix.f90
+-rwxrwxr-x   0 monacell  (1001) monacell  (1001)    36499 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/symmetry_high_rank.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1652 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/symvector.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    14041 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/third_order_ASR.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    23138 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/third_order_centering.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    28528 2023-06-06 10:19:07.000000 CellConstructor-1.3.2/FModules/third_order_cond.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    30927 2023-06-06 10:19:07.000000 CellConstructor-1.3.2/FModules/third_order_cond_centering.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    19863 2023-06-06 10:19:07.000000 CellConstructor-1.3.2/FModules/third_order_dynbubble.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1030 2023-06-06 10:19:07.000000 CellConstructor-1.3.2/FModules/third_order_interpol.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1765 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/trntnsc.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1483 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/FModules/unwrap_tensors.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    35149 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/LICENSE.md
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      138 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/MANIFEST.in
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      265 2023-06-12 08:59:45.038278 CellConstructor-1.3.2/PKG-INFO
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     5484 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/README.md
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-12 08:59:45.002277 CellConstructor-1.3.2/cellconstructor/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     5067 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/cellconstructor/AnharmonicForceFields.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     8677 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/cellconstructor/Bands.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)   139969 2023-06-12 08:59:04.000000 CellConstructor-1.3.2/cellconstructor/ForceTensor.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    63428 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/cellconstructor/Manipulate.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    75839 2023-06-06 10:19:07.000000 CellConstructor-1.3.2/cellconstructor/Methods.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     5568 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/cellconstructor/Moro_object.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)   185234 2023-02-15 11:33:51.000000 CellConstructor-1.3.2/cellconstructor/Phonons.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    13887 2023-02-15 11:18:26.000000 CellConstructor-1.3.2/cellconstructor/Settings.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)   106975 2023-06-12 08:59:04.000000 CellConstructor-1.3.2/cellconstructor/Spectral.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    85957 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/cellconstructor/Structure.py
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-12 08:59:45.026277 CellConstructor-1.3.2/cellconstructor/SymData/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      112 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/cellconstructor/SymData/15.dat
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      220 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/cellconstructor/SymData/36.dat
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      106 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/cellconstructor/SymData/36_red.dat
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      115 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/cellconstructor/SymData/60.dat
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      254 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/cellconstructor/SymData/64.bcs
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     2155 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/cellconstructor/SymData/64.dat
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1104 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/cellconstructor/SymData/convert_sym.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)   181899 2023-06-06 10:19:07.000000 CellConstructor-1.3.2/cellconstructor/ThermalConductivity.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     7242 2023-02-16 11:37:18.000000 CellConstructor-1.3.2/cellconstructor/Timer.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      963 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/cellconstructor/Units.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      641 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/cellconstructor/__init__.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    17679 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/cellconstructor/calculators.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)   111752 2023-02-15 11:37:20.000000 CellConstructor-1.3.2/cellconstructor/symmetries.py
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-12 08:59:45.034278 CellConstructor-1.3.2/scripts/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    32848 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/scripts/cellconstructor_test.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1629 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/scripts/symmetrize_dynmat.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      754 2023-02-13 14:55:58.000000 CellConstructor-1.3.2/scripts/view_scf_atoms.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)       38 2023-06-12 08:59:45.038278 CellConstructor-1.3.2/setup.cfg
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4457 2023-06-12 08:59:30.000000 CellConstructor-1.3.2/setup.py
```

### Comparing `CellConstructor-1.3.1/CModules/LinAlg.c` & `CellConstructor-1.3.2/CModules/LinAlg.c`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/CModules/LinAlg.h` & `CellConstructor-1.3.2/CModules/LinAlg.h`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/CModules/wrapper3.c` & `CellConstructor-1.3.2/CModules/wrapper3.c`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/CellConstructor.egg-info/SOURCES.txt` & `CellConstructor-1.3.2/CellConstructor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/constants.f90` & `CellConstructor-1.3.2/FModules/constants.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/contract_two_phonon_propagator.f90` & `CellConstructor-1.3.2/FModules/contract_two_phonon_propagator.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/cryst_to_car.f90` & `CellConstructor-1.3.2/FModules/cryst_to_car.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/eff_charge_interp.f90` & `CellConstructor-1.3.2/FModules/eff_charge_interp.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/eqvect.f90` & `CellConstructor-1.3.2/FModules/eqvect.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/error_handler.f90` & `CellConstructor-1.3.2/FModules/error_handler.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/fc_supercell_from_dyn.f90` & `CellConstructor-1.3.2/FModules/fc_supercell_from_dyn.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/flush_unit.f90` & `CellConstructor-1.3.2/FModules/flush_unit.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/from_matdyn.f90` & `CellConstructor-1.3.2/FModules/from_matdyn.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/get_equivalent_atoms.f90` & `CellConstructor-1.3.2/FModules/get_equivalent_atoms.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/get_latvec.f90` & `CellConstructor-1.3.2/FModules/get_latvec.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/get_lf.f90` & `CellConstructor-1.3.2/FModules/get_lf.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/get_q_grid_fast.f90` & `CellConstructor-1.3.2/FModules/get_q_grid_fast.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/get_scattering_q_grid.f90` & `CellConstructor-1.3.2/FModules/get_scattering_q_grid.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/get_translations.f90` & `CellConstructor-1.3.2/FModules/get_translations.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/interp.f90` & `CellConstructor-1.3.2/FModules/interp.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/invmat.f90` & `CellConstructor-1.3.2/FModules/invmat.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/io_global.f90` & `CellConstructor-1.3.2/FModules/io_global.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/kind.f90` & `CellConstructor-1.3.2/FModules/kind.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/q2qstar_out.f90` & `CellConstructor-1.3.2/FModules/q2qstar_out.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/q_gen.f90` & `CellConstructor-1.3.2/FModules/q_gen.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/recips.f90` & `CellConstructor-1.3.2/FModules/recips.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/rotate_and_add_dyn.f90` & `CellConstructor-1.3.2/FModules/rotate_and_add_dyn.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/second_order_ASR.f90` & `CellConstructor-1.3.2/FModules/second_order_ASR.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/second_order_centering.f90` & `CellConstructor-1.3.2/FModules/second_order_centering.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/set_asr.f90` & `CellConstructor-1.3.2/FModules/set_asr.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/set_tau.f90` & `CellConstructor-1.3.2/FModules/set_tau.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/sgam_ph.f90` & `CellConstructor-1.3.2/FModules/sgam_ph.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/smallgq.f90` & `CellConstructor-1.3.2/FModules/smallgq.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/star_q.f90` & `CellConstructor-1.3.2/FModules/star_q.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/symdynph_gq_new.f90` & `CellConstructor-1.3.2/FModules/symdynph_gq_new.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/symm_base.f90` & `CellConstructor-1.3.2/FModules/symm_base.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/symm_matrix.f90` & `CellConstructor-1.3.2/FModules/symm_matrix.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/symmetry_high_rank.f90` & `CellConstructor-1.3.2/FModules/symmetry_high_rank.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/symvector.f90` & `CellConstructor-1.3.2/FModules/symvector.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/third_order_ASR.f90` & `CellConstructor-1.3.2/FModules/third_order_ASR.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/third_order_centering.f90` & `CellConstructor-1.3.2/FModules/third_order_centering.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/third_order_cond.f90` & `CellConstructor-1.3.2/FModules/third_order_cond.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/third_order_cond_centering.f90` & `CellConstructor-1.3.2/FModules/third_order_cond_centering.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/third_order_dynbubble.f90` & `CellConstructor-1.3.2/FModules/third_order_dynbubble.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/third_order_interpol.f90` & `CellConstructor-1.3.2/FModules/third_order_interpol.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/trntnsc.f90` & `CellConstructor-1.3.2/FModules/trntnsc.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/FModules/unwrap_tensors.f90` & `CellConstructor-1.3.2/FModules/unwrap_tensors.f90`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/LICENSE.md` & `CellConstructor-1.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/README.md` & `CellConstructor-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/cellconstructor/AnharmonicForceFields.py` & `CellConstructor-1.3.2/cellconstructor/AnharmonicForceFields.py`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/cellconstructor/Bands.py` & `CellConstructor-1.3.2/cellconstructor/Bands.py`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/cellconstructor/ForceTensor.py` & `CellConstructor-1.3.2/cellconstructor/ForceTensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1123,17 +1123,23 @@
 
 # Third order force constant tensor
 class Tensor3():
     """
     This class defines the 3rank tensors, like 3rd force constants.
     """
 
-    def __init__(self, unitcell_structure, supercell_structure, supercell_size):
+    def __init__(self, unitcell_structure=None, supercell_structure=None, supercell_size=None,dyn=None):
         #GenericTensor.__init__(self, *args, **kwargs)
         
+        if dyn != None:
+            unitcell_structure=dyn.structure
+            supercell_size=dyn.GetSupercell()
+            supercell_structure=dyn.structure.generate_supercell(supercell_size)
+        
+        
         n_sup = np.prod(supercell_size)
         nat = unitcell_structure.N_atoms
         
         nat_sc= n_sup * nat
         
         self.n_sup = n_sup
         self.n_R = n_sup**2
```

### Comparing `CellConstructor-1.3.1/cellconstructor/Manipulate.py` & `CellConstructor-1.3.2/cellconstructor/Manipulate.py`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/cellconstructor/Methods.py` & `CellConstructor-1.3.2/cellconstructor/Methods.py`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/cellconstructor/Moro_object.py` & `CellConstructor-1.3.2/cellconstructor/Moro_object.py`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/cellconstructor/Phonons.py` & `CellConstructor-1.3.2/cellconstructor/Phonons.py`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/cellconstructor/Settings.py` & `CellConstructor-1.3.2/cellconstructor/Settings.py`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/cellconstructor/Spectral.py` & `CellConstructor-1.3.2/cellconstructor/Spectral.py`

 * *Files 11% similar despite different names*

```diff
@@ -599,16 +599,16 @@
     return spectral_func
 
 
 def get_full_dynamic_correction_along_path(dyn, 
                                            tensor3, 
                                            k_grid,  
                                            e1, de, e0,
-                                           sm1, sm0, 
-                                           sm1_id, sm0_id,
+                                           sm1=1.0, sm0=1.0, 
+                                           sm1_id=None, sm0_id=None,
                                            nsm=1,
                                            T=0,
                                            q_path=[0.0,0.0,0.0],                                           
                                            q_path_file=None,
                                            print_path = True,                                           
                                            static_limit = False, 
                                            notransl = True, 
@@ -677,15 +677,15 @@
                     (defaul = True)
         diag approx : logical
                     If True, the off-diagonal terms of the slef-energy are discarded
                     (the same result can be obtained in a cheaper way by using the 
                     corresponding function)
                     (default : False)
         filename_sp  : string 
-                      filename_sp_[id_smear]_[smear].dat
+                      filename_sp_[smear].dat
                       is the file where the result is written. 
                       Format: length of the path (in 2pi/Alat), 
                       energy (cm-1),spectral function (1/cm-1)
                       (default: "full_spectral_func")        
         d3_scale_factor : float 
                           If present, the 3rd order FC is multiplied by this factor
                           (e.g. it can be used to make tests about the perturbative limit)
@@ -704,14 +704,21 @@
     print(" ") 
     print(" T= {:>5.1f} K".format(T))
     print(" k grid= {} x {} x {} ".format(*tuple(k_grid))) 
     if static_limit :
         print(" ")
         print(" - The static limit is considered - ")
         print(" ")
+    else:
+        print(" ")        
+        print(" Smearing values: ")
+        print(" ")            
+        for sm in np.linspace(sm0,sm1,nsm):
+            print("     sm= {:>6.2f} cm-1".format(sm))  
+        print(" ")         
     if diag_approx :
         print(" ")
         print(" - The off-diagonal terms of the self-energy are discarded - ")
         print(" ")     
  
  
     if ( tensor2 == None ):
@@ -752,15 +759,20 @@
         print(" ")        
     # ==========================================================================================     
  
     #  ======================= Energy & Smearing ==========================================    
     # energy   in input is in cm-1
     # smearing in input is in cm-1
     # converto to Ry
-
+    if sm1_id != None and sm0_id != None:
+        for sm in np.linspace(sm0_id,sm1_id,nsm):
+                print("     sm_id= {:>6.2f} cm-1".format(sm))  
+    else:
+        sm1_id=de*2.0
+        sm0_id=de*2.0 
     # list of energies
     energies=np.arange(e0,e1,de)/CC.Units.RY_TO_CM
     ne=energies.shape[0]
     # list of smearing
     if nsm == 1 : 
         sm1=sm0
         sm1_id=sm0_id
@@ -781,41 +793,65 @@
                                                       diag_approx, verbose=False )    
     
         # convert from 1/Ry to 1/cm-1
         spectralf /= CC.Units.RY_TO_CM
     
 
         # ==================================================================================   
- 
+        #
         # print the result
-        for  ism in range(nsm):
-            #
-            name="{:5.2f}".format(smear_id_cm[ism]).strip()+"_"+"{:6.1f}".format(smear_cm[ism]).strip()
+        #
+        if static_limit :
             #
-            filename_new=filename_sp+'_'+name+'.dat'
+            filename_new=filename_sp+'_static.dat'
             if iq == 0:
                 with open(filename_new,'w') as f:
                     f.write(" # ------------------------------------------------------------- \n")
                     f.write(" # len (2pi/Angstrom), energy (cm-1), spectral function (1/cm-1) \n")
                     f.write(" # ------------------------------------------------------------- \n")
                     for ie, ene in enumerate(energies_cm):
-                        f.write("{:>10.6f}\t{:>11.7f}\t{:>11.7f}\n".format(x_length[iq],ene,spectralf[ie,ism]))
+                        f.write("{:>10.6f}\t{:>11.7f}\t{:>11.7f}\n".format(x_length[iq],ene,spectralf[ie,0]))
                     f.write("\n")
             else:
                 with open(filename_new,'a') as f:
                     for ie, ene in enumerate(energies_cm):
-                        f.write("{:>10.6f}\t{:>11.7f}\t{:>11.7f}\n".format(x_length[iq],ene,spectralf[ie,ism]))
-                    f.write("\n")
-                
- 
- 
-    print(" ")
-    print(" Results printed in "+filename_sp+'_[id_smear]_[smear].dat')
-    print(" ")      
+                        f.write("{:>10.6f}\t{:>11.7f}\t{:>11.7f}\n".format(x_length[iq],ene,spectralf[ie,0]))
+                    f.write("\n")           
+            #
+        else:
+            #
+            for  ism in range(nsm):
+                #
+                #name="{:5.2f}".format(smear_id_cm[ism]).strip()+"_"+"{:6.1f}".format(smear_cm[ism]).strip()
+                name="{:6.1f}".format(smear_cm[ism]).strip()
+                #
+                filename_new=filename_sp+'_'+name+'.dat'
+                if iq == 0:
+                    with open(filename_new,'w') as f:
+                        f.write(" # ------------------------------------------------------------- \n")
+                        f.write(" # len (2pi/Angstrom), energy (cm-1), spectral function (1/cm-1) \n")
+                        f.write(" # ------------------------------------------------------------- \n")
+                        for ie, ene in enumerate(energies_cm):
+                            f.write("{:>10.6f}\t{:>11.7f}\t{:>11.7f}\n".format(x_length[iq],ene,spectralf[ie,ism]))
+                        f.write("\n")
+                else:
+                    with open(filename_new,'a') as f:
+                        for ie, ene in enumerate(energies_cm):
+                            f.write("{:>10.6f}\t{:>11.7f}\t{:>11.7f}\n".format(x_length[iq],ene,spectralf[ie,ism]))
+                        f.write("\n")
+                    
  
+    if static_limit : 
+        print(" ")
+        print(" Results printed in "+filename_sp+'_static.dat')
+        print(" ")      
+    else:
+        print(" ")
+        print(" Results printed in "+filename_sp+'_[smear].dat')
+        print(" ")               
  
  
 
 
 
 
 # ========================= DIAGONAL SELF-ENERGY DYNAMIC CORRECTION  =========================      
@@ -948,15 +984,15 @@
     CC.Settings.SetupParallel()
 
     d_bubble_mod =CC.Settings.GoParallel(compute_k, k_points, reduce_op = "+")
     
     # divide by the N_k factor
     d_bubble_mod /= len(k_points) # (ne,nsmear,n_mod)
     #
-    np.savetxt("db_new",d_bubble_mod[:,-1,-1])
+    # np.savetxt("db_new",d_bubble_mod[:,-1,-1])
     #
     spectralf=thirdorder.third_order_bubble.compute_spectralf_diag(smear_id,energies,w_q,
                                                                    d_bubble_mod,
                                                                    nat,ne,nsm)    
                                                                     # (ne, n_mod, nsmear)
 
     w2_q_ext=w2_q[None,None,...]
@@ -1727,16 +1763,19 @@
         d3_pols = np.einsum("abc, ci -> abi", d3_pols, pols_mq_mk)
         
         t4 = time.time()
         
         
         nsm=smear.shape[0]
         n_mod=3*structure.N_atoms 
+        
         # Fortran duty ====
         
+        selfnrg  = np.zeros ( (n_mod,nsm ), dtype= np.complex128, order="F")
+        
         selfnrg  = thirdorder.third_order_bubble.compute_perturb_selfnrg(smear,T,
                                                             np.array([w_q,w_k,w_mq_mk]).T,
                                                             np.array([is_q_gamma,is_k_gamma,is_mq_mk_gamma]),
                                                             d3_pols,nsm,n_mod)                
 
         t5 = time.time()
         
@@ -1978,7 +2017,430 @@
     print(" Results printed in "+filename_shift_lw+'_'+'[smear].dat')
     print(" ")      
     print(" ")
     print(" Results printed in "+filename_freq_dyn+'_'+'[smear].dat')
     print(" ")      
 
 
+
+
+
+ # ===== ONE-SHOT & PERTURBATIVE CORRECTION TO SSCHA FREQUENCY (SHIFT and LINEWIDTH) =====================             
+ 
+ 
+def get_os_perturb_dynamic_selfnrg(tensor2, tensor3, 
+                            k_grid, q, 
+                            smear,
+                            T,
+                            verbose= False):
+        
+    structure = tensor2.unitcell_structure
+    
+    # Get the integration points 
+    k_points = CC.symmetries.GetQGrid(structure.unit_cell, k_grid)
+    
+        
+    # Get the phi2 in q
+    phi2_q = tensor2.Interpolate(q, asr = False)
+
+    # dynamical matrix in q
+    m = np.tile(structure.get_masses_array(), (3,1)).T.ravel()    
+    mm_mat = np.sqrt(np.outer(m, m))
+    mm_inv_mat = 1 / mm_mat
+    #
+    d2_q = phi2_q * mm_inv_mat
+    
+    # Diagonalize the dynamical matrix in q
+    w2_q, pols_q = np.linalg.eigh(d2_q)
+    
+    # Check if the q point is gamma
+    is_q_gamma = CC.Methods.is_gamma(structure.unit_cell, q)
+    
+    if is_q_gamma:
+        w2_q[0:3]=0.0
+    if not (w2_q >= 0.0).all():
+        print('q= ',q, '    (2pi/A)')
+        print('w(q)= ',np.sign(w2_q)*np.sqrt(np.abs(w2_q))*CC.Units.RY_TO_CM,'  (cm-1)')
+        print('Cannot continue with SSCHA negative frequencies')
+        exit()
+    w_q=np.sqrt(w2_q)   
+    
+    def compute_k(k):
+        # phi3 in q, k, -q - k
+        t1 = time.time()        
+        phi3=tensor3.Interpolate(k,-q-k, asr = False)
+        t2 = time.time()
+        # phi2 in k
+        phi2_k = tensor2.Interpolate(k, asr = False) 
+
+        # phi2 in -q-k
+        phi2_mq_mk = tensor2.Interpolate(-q -k, asr = False)
+
+        t3 = time.time()
+        
+        # dynamical matrices (divide by the masses)
+        d2_k = phi2_k * mm_inv_mat
+        d2_mq_mk = phi2_mq_mk * mm_inv_mat
+        
+        # Diagonalize the dynamical matrices
+        w2_k, pols_k = np.linalg.eigh(d2_k)
+        w2_mq_mk, pols_mq_mk = np.linalg.eigh(d2_mq_mk)
+        
+        
+        is_k_gamma = CC.Methods.is_gamma(structure.unit_cell, k)
+        is_mq_mk_gamma = CC.Methods.is_gamma(structure.unit_cell, -q-k)
+        
+        if is_k_gamma:
+            w2_k[0:3]=0.0
+        if not (w2_k >= 0.0).all():
+            print('k= ',k, '    (2pi/A)')
+            print('w(k)= ',np.sign(w2_k)*np.sqrt(np.abs(w2_k))*CC.Units.RY_TO_CM,'  (cm-1)')
+            print('Cannot continue with SSCHA negative frequencies')
+            exit()
+        w_k=np.sqrt(w2_k)
+
+        if is_mq_mk_gamma:
+            w2_mq_mk[0:3]=0.0
+        if not (w2_mq_mk >= 0.0).all():
+            print('-q-k= ',-q-k, '    (2pi/A)')
+            print('w(-q-k)= ',np.sign(w2_mq_mk)*np.sqrt(np.abs(w2_mq_mk))*CC.Units.RY_TO_CM,'  (cm-1)')
+            print('Cannot continue with SSCHA negative frequencies')
+            exit()
+        w_mq_mk=np.sqrt(w2_mq_mk)
+        
+        # Dividing the phi3 by the sqare root of masses
+        d3 = np.einsum("abc, a, b, c -> abc", phi3, 1/np.sqrt(m), 1/np.sqrt(m), 1/np.sqrt(m))
+
+        # d3 in mode components
+        # d3_pols = np.einsum("abc, ai, bj, ck -> ijk", d3, pols_mq, pols_k, pols_q_mk)
+        d3_pols = np.einsum("abc, ai -> ibc", d3, pols_q)
+        d3_pols = np.einsum("abc, bi -> aic", d3_pols, pols_k)
+        d3_pols = np.einsum("abc, ci -> abi", d3_pols, pols_mq_mk)
+        
+        t4 = time.time()
+        
+        
+        nsm=smear.shape[0]
+        n_mod=3*structure.N_atoms 
+        
+        # Fortran duty ====
+        
+        selfnrg  = np.zeros ( (n_mod,nsm ), dtype= np.complex128, order="F")
+        
+        selfnrg  = thirdorder.third_order_bubble.compute_perturb_selfnrg(smear,T,
+                                                            np.array([w_q,w_k,w_mq_mk]).T,
+                                                            np.array([is_q_gamma,is_k_gamma,is_mq_mk_gamma]),
+                                                            d3_pols,nsm,n_mod)                
+
+        t5 = time.time()
+        
+        if verbose:
+            print("Time to interpolate the third order: {} s".format(t2 - t1))
+            print("Time to interpolate the second order: {} s".format(t3 - t2))
+            print("Time to transform the tensors: {} s".format(t4 - t3))
+            print("Time to compute the bubble: {} s".format(t5 - t4))
+        
+        return selfnrg    
+    
+    CC.Settings.SetupParallel()
+
+    selfnrg =CC.Settings.GoParallel(compute_k, k_points, reduce_op = "+")
+
+    # divide by the N_k factor
+    selfnrg /= len(k_points) # (n_mod,nsigma)
+    
+    w_q_ext=w_q[...,None]
+    w2_q_ext=w2_q[...,None]
+   
+    z_os=np.sqrt(selfnrg + w2_q_ext) # (A20) PHYSICAL REVIEW B 97, 214101 (2018)
+    shift_os=z_os.real-w_q_ext
+    hwhm_os=-z_os.imag
+    
+    z_pert=np.divide(selfnrg, 2*w_q_ext, out=np.zeros_like(selfnrg), where=w_q_ext!=0)    # -w_q_ext
+    shift_pert=z_pert.real
+    hwhm_pert=-z_pert.imag
+
+    return w_q, shift_pert, hwhm_pert, shift_os, hwhm_os
+ 
+
+
+def get_os_perturb_dynamic_correction_along_path(dyn, tensor3, 
+                                           k_grid,                                              
+                                           sm1, sm0,
+                                           nsm=1,
+                                           q_path=[0.0,0.0,0.0],
+                                           q_path_file=None,
+                                           print_path = True,
+                                           T=0, 
+                                           filename_shift_lw  = 'v2_freq_shift_hwhm',                                           
+                                           filename_freq_dyn = 'freq_dynamic',                                           
+                                           d3_scale_factor=None,
+                                           tensor2= None):                                           
+
+
+    """
+    The frequency shift (with respect to the SSCHA frequency) and linewidth are computed with 
+    the one-shot and the perturbative formula with respect to the SSCHA frequency.
+    
+    Parameters
+    ----------
+    
+        dyn : Phonons()
+            The harmonic / SSCHA dynamical matrix
+        tensor3 : Tensor3()
+            The third order force constant matrix
+        k_grid : list(len = 3)
+            The integration grid on the Brillouin zone        
+        sm0, sm1 : float      
+              Minimum and maximum value of the smearing (cm-1) to compute the self-energy   
+
+        Optional
+        --------
+
+        nsm : integer
+              Number of smearings to consider         
+              (default = 1)
+        T : float
+            The temperature 
+            (default: 0 K)
+        q_path : list of triplets
+                 Path of the q-points of the Brillouin Zone, in 2pi/Anstrom units,
+                 where the caculation is performed 
+                 (defualt: [0.0,0.0,0.0])            
+        q_path_file : string
+                      Name of the file where the q_path can be read. 
+                      Format: column of triples, q points in 2pi/Angstrom
+                      If the name of the file is present, it has the
+                      priority over the q_path value 
+                      (default: None)
+        print_path : logical
+                     If True (and the path is composed of more then one q-point), 
+                     a file 'path_len.dat' is printed.
+                     Format: column of 4 values, coordinates of 
+                     the q-point and path length (in 2pi/Angstrom) .
+                     (default: True)  
+        filename_shift_lw : string      
+                            filename_shift_lw_[id_smear]_[smear].dat
+                            is the file where
+                            len (2pi/Angstrom), SSCHA freq (cm-1), shift (cm-1) , HWHM (cm-1)
+                            are printed.
+                            (default: "v2_freq_shit_hwhm")
+        filename_freq_dyn :  string                   
+                             filename_freq_dyn_[id_smear]_[smear].dat
+                             is the file where
+                             len (2pi/Angstrom), freq (cm-1) (sorted in ascending order), HWHM (cm-1)
+                             are printed. 
+                             (default: "freq_dynamic")                                       
+        d3_scale_factor : float 
+                          If present, the 3rd order FC is multiplied by this factor
+                          (e.g. it can be used to make tests about the perturbative limit)
+                          (default: None)
+        tensor2 : ndarray( size = (3*nat, 3*nat), dtype = np.float)
+                  If present, this 2nd order FC overwrites the one 
+                  obtained from dyn.
+                  (default: None)  
+        
+    """
+
+
+
+    print(" ") 
+    print(" ===========================================" ) 
+    print("   Bubble perturbative dynamic correction   " ) 
+    print(" ===========================================" )
+    print(" ") 
+    print(" T= {:>5.1f} K".format(T))
+    print(" k grid= {} x {} x {} ".format(*tuple(k_grid)))
+    print(" ")
+    print(" Smearing values: ")
+    print(" ")
+    for sm in np.linspace(sm0,sm1,nsm):
+        print("     sm= {:>6.2f} cm-1".format(sm))  
+    print(" ") 
+    print(" ===========================================" ) 
+    print(" " ) 
+
+    if ( tensor2 == None ):
+        
+        # Prepare the tensor2
+        tensor2 = CC.ForceTensor.Tensor2(dyn.structure, dyn.structure.generate_supercell(dyn.GetSupercell()), dyn.GetSupercell())
+        tensor2.SetupFromPhonons(dyn)
+        tensor2.Center()     
+
+    # Scale the FC3 ===========================================================================
+    if  d3_scale_factor != None :
+            print(" ")
+            print("d3 scaling : d3 -> d3 x {:>7.3f}".format(d3_scale_factor))
+            print(" ")
+            tensor3.tensor=tensor3.tensor*d3_scale_factor
+    #  ================================== q-PATH ===============================================   
+    if  q_path_file == None:
+        q_path=np.array(q_path)
+    else:
+        print(" ")
+        print(" q_path read from "+q_path_file)
+        print(" ")        
+        q_path=np.loadtxt(q_path_file)
+    if len(q_path.shape) == 1 : q_path=np.expand_dims(q_path,axis=0)    
+    # Get the length of the q path
+    x_length = np.zeros(len(q_path))        
+    q_tot = np.sqrt(np.sum(np.diff(np.array(q_path), axis = 0)**2, axis = 1))
+    x_length[1:] = q_tot
+    x_length=np.cumsum(x_length)
+    x_length_exp=np.expand_dims(x_length,axis=0) 
+    # print the path q-points and length
+    if print_path and (q_path.shape[0] > 1) :
+        fmt_txt=['%11.7f\t','%11.7f\t','%11.7f\t\t','%10.6f\t']
+        result=np.hstack((q_path,x_length_exp.T))        
+        np.savetxt('path_len.dat',result,fmt=fmt_txt)
+        print(" ")
+        print(" Path printed in path_len.dat ")
+        print(" ")        
+    #  ======================= Smearing ==========================================    
+    # smearing in input is in cm-1
+    # converto to Ry
+    # list of smearing
+    #
+    if nsm == 1 : 
+        sm1=sm0
+    smear=np.linspace(sm0,sm1,nsm)/CC.Units.RY_TO_CM
+    #  ======================== Calculation ==========================================        
+    n_mod=3*dyn.structure.N_atoms
+    shift_pert     = np.zeros( ( n_mod, nsm), dtype = np.float64 ) # q-point,mode,smear
+    hwhm_pert      = np.zeros( ( n_mod, nsm), dtype = np.float64 ) # q-point,mode,smear
+    shift_os       = np.zeros( ( n_mod, nsm), dtype = np.float64 ) # q-point,mode,smear
+    hwhm_os        = np.zeros( ( n_mod, nsm), dtype = np.float64 ) # q-point,mode,smear    
+    wq             = np.zeros( ( n_mod), dtype = np.float64 )      # q-point,mode
+    #
+    smear_cm = smear * CC.Units.RY_TO_CM
+    
+    for iq, q in enumerate(q_path):              
+        wq[:],shift_pert[:,:], hwhm_pert[:,:],shift_os[:,:], hwhm_os[:,:]  = get_os_perturb_dynamic_selfnrg(tensor2, 
+                                                                                                            tensor3,
+                                                                                                            k_grid, 
+                                                                                                            np.array(q),
+                                                                                                            smear, T, 
+                                                                                                            verbose=False )            
+    
+        # print results
+        wq*=CC.Units.RY_TO_CM
+        shift_os*=CC.Units.RY_TO_CM
+        hwhm_os*=CC.Units.RY_TO_CM
+        shift_pert*=CC.Units.RY_TO_CM
+        hwhm_pert*=CC.Units.RY_TO_CM        
+        #
+        #==================== SORTING ===============================
+        wq_os_shifted=wq[...,None]+shift_os
+        sortidx_os=np.argsort(wq_os_shifted,axis=0)
+        wq_os_shifted_sorted=np.take_along_axis(wq_os_shifted, sortidx_os, 0)
+        hwhm_os_sorted=np.take_along_axis(hwhm_os, sortidx_os, 0)
+        
+        wq_pert_shifted=wq[...,None]+shift_pert
+        sortidx_pert=np.argsort(wq_pert_shifted,axis=0)        
+        wq_pert_shifted_sorted=np.take_along_axis(wq_pert_shifted, sortidx_pert, 0)
+        hwhm_pert_sorted=np.take_along_axis(hwhm_pert, sortidx_pert, 0)    
+        #=============== Print Results ===============================    
+        # one shot
+        #
+        for  ism in range(nsm):
+            #
+            name="{:6.2f}".format(smear_cm[ism]).strip()
+            #
+            # v2 freq, corresponding  shift & hwhm
+            #
+            filename_new=filename_shift_lw+'_'+name+'.os.dat'
+            fmt="{:>10.6f}\t"+"\t{:>11.7f}"*(3*n_mod)+"\n"
+            if iq == 0:
+                with open(filename_new,'w') as f:
+                    f.write("# --------------------------------------------------------------------- \n")
+                    f.write("# len (2pi/Angstrom), sscha freq (cm-1), freq shift (cm-1), hwhm (cm-1) \n")
+                    f.write("# --------------------------------------------------------------------- \n") 
+                    out=np.concatenate((wq[:],shift_os[:,ism], 
+                                    hwhm_os[:,ism]))
+                    f.write(fmt.format(x_length[iq],*out))
+            else:
+                with open(filename_new,'a') as f:
+                    out=np.concatenate((wq[:],shift_os[:,ism], 
+                                    hwhm_os[:,ism]))
+                    f.write(fmt.format(x_length[iq],*out))
+            #
+            name="{:6.1f}".format(smear_cm[ism]).strip()
+            #
+            # shifted freq sorted, corresponding hwhm 
+            #
+            filename_new=filename_freq_dyn+'_'+name+'.os.dat'
+            fmt="{:>10.6f}\t"+"\t{:>11.7f}"*(2*n_mod)+"\n"
+            if iq == 0:
+                with open(filename_new,'w') as f:
+                    f.write("# ----------------------------------------------------------------- \n")
+                    f.write("# len (2pi/Angstrom), sscha+shift freq (sorted) (cm-1), hwhm (cm-1) \n")            
+                    f.write("# ----------------------------------------------------------------- \n")
+                    out=np.concatenate((wq_os_shifted_sorted[:,ism],
+                                    hwhm_os_sorted[:,ism]))
+                    f.write(fmt.format(x_length[iq],*out))
+            else:
+                with open(filename_new,'a') as f:
+                    out=np.concatenate((wq_os_shifted_sorted[:,ism],
+                                    hwhm_os_sorted[:,ism]))
+                    f.write(fmt.format(x_length[iq],*out))
+        #
+        # perturb
+        #
+        for  ism in range(nsm):
+            #
+            name="{:6.2f}".format(smear_cm[ism]).strip()
+            #
+            # v2 freq, corresponding  shift & hwhm
+            #
+            filename_new=filename_shift_lw+'_'+name+'.pert.dat'
+            fmt="{:>10.6f}\t"+"\t{:>11.7f}"*(3*n_mod)+"\n"
+            if iq == 0:
+                with open(filename_new,'w') as f:
+                    f.write("# --------------------------------------------------------------------- \n")
+                    f.write("# len (2pi/Angstrom), sscha freq (cm-1), freq shift (cm-1), hwhm (cm-1) \n")
+                    f.write("# --------------------------------------------------------------------- \n") 
+                    out=np.concatenate((wq[:],shift_pert[:,ism], 
+                                    hwhm_pert[:,ism]))
+                    f.write(fmt.format(x_length[iq],*out))
+            else:
+                with open(filename_new,'a') as f:
+                    out=np.concatenate((wq[:],shift_pert[:,ism], 
+                                    hwhm_pert[:,ism]))
+                    f.write(fmt.format(x_length[iq],*out))
+            #
+            name="{:6.1f}".format(smear_cm[ism]).strip()
+            #
+            # shifted freq sorted, corresponding hwhm 
+            #
+            filename_new=filename_freq_dyn+'_'+name+'.pert.dat'
+            fmt="{:>10.6f}\t"+"\t{:>11.7f}"*(2*n_mod)+"\n"
+            if iq == 0:
+                with open(filename_new,'w') as f:
+                    f.write("# ----------------------------------------------------------------- \n")
+                    f.write("# len (2pi/Angstrom), sscha+shift freq (sorted) (cm-1), hwhm (cm-1) \n")            
+                    f.write("# ----------------------------------------------------------------- \n")
+                    out=np.concatenate((wq_pert_shifted_sorted[:,ism],
+                                    hwhm_pert_sorted[:,ism]))
+                    f.write(fmt.format(x_length[iq],*out))
+            else:
+                with open(filename_new,'a') as f:
+                    out=np.concatenate((wq_pert_shifted_sorted[:,ism],
+                                    hwhm_pert_sorted[:,ism]))
+                    f.write(fmt.format(x_length[iq],*out))
+                
+
+
+
+    print(" ")
+    print(" Results printed in "+filename_shift_lw+'_'+'[smear].os/pert.dat')
+    print(" ")      
+    print(" ")
+    print(" Results printed in "+filename_freq_dyn+'_'+'[smear].os/pert.dat')
+    print(" ")      
+
+
+
+
+
+
+
+
```

### Comparing `CellConstructor-1.3.1/cellconstructor/Structure.py` & `CellConstructor-1.3.2/cellconstructor/Structure.py`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/cellconstructor/SymData/convert_sym.py` & `CellConstructor-1.3.2/cellconstructor/SymData/convert_sym.py`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/cellconstructor/ThermalConductivity.py` & `CellConstructor-1.3.2/cellconstructor/ThermalConductivity.py`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/cellconstructor/Timer.py` & `CellConstructor-1.3.2/cellconstructor/Timer.py`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/cellconstructor/Units.py` & `CellConstructor-1.3.2/cellconstructor/Units.py`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/cellconstructor/__init__.py` & `CellConstructor-1.3.2/cellconstructor/__init__.py`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/cellconstructor/calculators.py` & `CellConstructor-1.3.2/cellconstructor/calculators.py`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/cellconstructor/symmetries.py` & `CellConstructor-1.3.2/cellconstructor/symmetries.py`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/scripts/cellconstructor_test.py` & `CellConstructor-1.3.2/scripts/cellconstructor_test.py`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/scripts/symmetrize_dynmat.py` & `CellConstructor-1.3.2/scripts/symmetrize_dynmat.py`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/scripts/view_scf_atoms.py` & `CellConstructor-1.3.2/scripts/view_scf_atoms.py`

 * *Files identical despite different names*

### Comparing `CellConstructor-1.3.1/setup.py` & `CellConstructor-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                       sources = ["CModules/LinAlg.c", WRAPPER]
                       )
 
 
 
 
 setup( name = "CellConstructor",
-       version = "1.3.1",
+       version = "1.3.2",
        description = "Python utilities that is interfaced with ASE for atomic crystal analysis",
        author = "Lorenzo Monacelli",
        url = "https://github.com/mesonepigreco/CellConstructor",
        packages = ["cellconstructor"],
        package_dir = {"cellconstructor": "cellconstructor"},
        package_data = {"cellconstructor": ["SymData/*.dat"]},
        setup_requires = ["numpy", "ase", "scipy"],
```

