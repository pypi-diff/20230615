# Comparing `tmp/tidy3d-2.2.3.tar.gz` & `tmp/tidy3d-2.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidy3d-2.2.3.tar", last modified: Thu Jun 15 19:54:33 2023, max compression
+gzip compressed data, was "tidy3d-2.3.0rc1.tar", last modified: Mon Jun  5 20:08:20 2023, max compression
```

## Comparing `tidy3d-2.2.3.tar` & `tidy3d-2.3.0rc1.tar`

### file list

```diff
@@ -1,194 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.643191 tidy3d-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-06-15 19:54:17.000000 tidy3d-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-15 19:54:17.000000 tidy3d-2.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-15 19:54:33.643191 tidy3d-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-06-15 19:54:17.000000 tidy3d-2.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-15 19:54:17.000000 tidy3d-2.2.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.607203 tidy3d-2.2.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-15 19:54:17.000000 tidy3d-2.2.3/requirements/basic.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-15 19:54:17.000000 tidy3d-2.2.3/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-15 19:54:17.000000 tidy3d-2.2.3/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 19:54:17.000000 tidy3d-2.2.3/requirements/gdspy.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 19:54:17.000000 tidy3d-2.2.3/requirements/gdstk.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-15 19:54:17.000000 tidy3d-2.2.3/requirements/jax.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 19:54:17.000000 tidy3d-2.2.3/requirements/trimesh.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-15 19:54:17.000000 tidy3d-2.2.3/requirements/web.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 19:54:17.000000 tidy3d-2.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 19:54:33.643191 tidy3d-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-15 19:54:17.000000 tidy3d-2.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.607203 tidy3d-2.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.607203 tidy3d-2.2.3/tests/_test_local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/_test_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/_test_local/_test_adjoint_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/_test_local/_test_data_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/_test_local/_test_fit_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/_test_local/_test_plugins_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/_test_local/_test_web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.615201 tidy3d-2.2.3/tests/test_components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_components/test_IO.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_components/test_apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_components/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_components/test_boundaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_components/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_components/test_field_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_components/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_components/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_components/test_grid_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_components/test_medium.py
--rw-r--r--   0 runner    (1001) docker     (123)    23843 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_components/test_meshgenerate.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_components/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_components/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    21134 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_components/test_sidewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    53136 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_components/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_components/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_components/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_components/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.615201 tidy3d-2.2.3/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_data/test_data_arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)    19395 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_data/test_monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_data/test_sim_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.615201 tidy3d-2.2.3/tests/test_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_package/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_package/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_package/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_package/test_make_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_package/test_material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_package/test_parametric_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.619199 tidy3d-2.2.3/tests/test_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41852 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_plugins/test_adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_plugins/test_component_modeler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_plugins/test_dispersion_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_plugins/test_mode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_plugins/test_polyslab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_plugins/test_resonance_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_plugins/test_waveguide.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.619199 tidy3d-2.2.3/tests/test_web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_web/mock_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_web/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_web/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_web/test_material_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_web/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_web/test_tidy3d_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_web/test_tidy3d_material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_web/test_tidy3d_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/test_web/test_webapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    16947 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.623198 tidy3d-2.2.3/tidy3d/
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.627196 tidy3d-2.2.3/tidy3d/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/boundary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.627196 tidy3d-2.2.3/tidy3d/components/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/data/data_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    78767 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/data/monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    28054 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/data/sim_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/field_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)   146570 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.631195 tidy3d-2.2.3/tidy3d/components/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14955 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/grid/grid_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    47556 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/grid/mesher.py
--rw-r--r--   0 runner    (1001) docker     (123)    68574 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    29507 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)   117908 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    33364 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/components/viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.631195 tidy3d-2.2.3/tidy3d/material_library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/material_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62029 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/material_library/material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/material_library/material_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/material_library/parametric_materials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.631195 tidy3d-2.2.3/tidy3d/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.631195 tidy3d-2.2.3/tidy3d/plugins/adjoint/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/adjoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.631195 tidy3d-2.2.3/tidy3d/plugins/adjoint/components/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/adjoint/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/adjoint/components/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.631195 tidy3d-2.2.3/tidy3d/plugins/adjoint/components/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/adjoint/components/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/adjoint/components/data/data_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/adjoint/components/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/adjoint/components/data/monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/adjoint/components/data/sim_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23786 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/adjoint/components/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/adjoint/components/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)    17903 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/adjoint/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/adjoint/components/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/adjoint/components/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    29963 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/adjoint/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.631195 tidy3d-2.2.3/tidy3d/plugins/dispersion/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/dispersion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23663 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/dispersion/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/dispersion/fit_web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.635194 tidy3d-2.2.3/tidy3d/plugins/mode/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/mode/derivatives.py
--rw-r--r--   0 runner    (1001) docker     (123)    25720 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/mode/mode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    27752 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/mode/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/mode/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.635194 tidy3d-2.2.3/tidy3d/plugins/polyslab/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/polyslab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/polyslab/polyslab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.635194 tidy3d-2.2.3/tidy3d/plugins/resonance/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/resonance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/resonance/resonance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.635194 tidy3d-2.2.3/tidy3d/plugins/smatrix/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/smatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/smatrix/smatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.635194 tidy3d-2.2.3/tidy3d/plugins/waveguide/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/waveguide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35573 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/plugins/waveguide/rectangular_dielectric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/updater.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.639192 tidy3d-2.2.3/tidy3d/web/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/web/asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)   275233 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/web/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/web/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.643191 tidy3d-2.2.3/tidy3d/web/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/web/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/web/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/web/cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/web/cli/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/web/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20751 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/web/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/web/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/web/http_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/web/httputils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/web/material_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/web/material_libray.py
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/web/s3utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16508 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/web/simulation_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/web/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/web/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    24366 2023-06-15 19:54:17.000000 tidy3d-2.2.3/tidy3d/web/webapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:54:33.623198 tidy3d-2.2.3/tidy3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-15 19:54:33.000000 tidy3d-2.2.3/tidy3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-06-15 19:54:33.000000 tidy3d-2.2.3/tidy3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:54:33.000000 tidy3d-2.2.3/tidy3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 19:54:33.000000 tidy3d-2.2.3/tidy3d.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-15 19:54:33.000000 tidy3d-2.2.3/tidy3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 19:54:33.000000 tidy3d-2.2.3/tidy3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.304961 tidy3d-2.3.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-06-05 20:08:20.304961 tidy3d-2.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.288961 tidy3d-2.3.0rc1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/requirements/basic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/requirements/gdspy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/requirements/gdstk.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/requirements/jax.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/requirements/trimesh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/requirements/web.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 20:08:20.304961 tidy3d-2.3.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.288961 tidy3d-2.3.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.288961 tidy3d-2.3.0rc1/tests/_test_local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/_test_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/_test_local/_test_adjoint_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/_test_local/_test_data_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/_test_local/_test_fit_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/_test_local/_test_plugins_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/_test_local/_test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.292961 tidy3d-2.3.0rc1/tests/test_components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32452 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_field_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_grid_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23843 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_meshgenerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21134 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_sidewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53649 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.292961 tidy3d-2.3.0rc1/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_data/test_data_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19395 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_data/test_monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_data/test_sim_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.292961 tidy3d-2.3.0rc1/tests/test_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_package/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_package/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_package/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_package/test_make_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_package/test_material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_package/test_parametric_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.292961 tidy3d-2.3.0rc1/tests/test_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41852 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_plugins/test_adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_plugins/test_component_modeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_plugins/test_dispersion_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_plugins/test_mode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_plugins/test_polyslab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_plugins/test_resonance_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_plugins/test_waveguide.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.292961 tidy3d-2.3.0rc1/tests/test_web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_web/mock_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_web/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_web/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_web/test_material_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_web/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_web/test_tidy3d_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_web/test_tidy3d_material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_web/test_tidy3d_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_web/test_webapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.296961 tidy3d-2.3.0rc1/tidy3d/
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.296961 tidy3d-2.3.0rc1/tidy3d/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26944 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/boundary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.296961 tidy3d-2.3.0rc1/tidy3d/components/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14272 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/data/data_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78767 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/data/monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28054 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/data/sim_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/field_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146898 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.300961 tidy3d-2.3.0rc1/tidy3d/components/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14955 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/grid/grid_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47556 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/grid/mesher.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114593 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29507 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119586 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32775 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.300961 tidy3d-2.3.0rc1/tidy3d/material_library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/material_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62029 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/material_library/material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/material_library/material_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/material_library/parametric_materials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.300961 tidy3d-2.3.0rc1/tidy3d/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.300961 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.300961 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.300961 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/data/data_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/data/monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/data/sim_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23786 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20217 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17771 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30051 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.300961 tidy3d-2.3.0rc1/tidy3d/plugins/dispersion/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/dispersion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21590 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/dispersion/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/dispersion/fit_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13262 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/dispersion/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.300961 tidy3d-2.3.0rc1/tidy3d/plugins/mode/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/mode/derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25720 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/mode/mode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27752 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/mode/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/mode/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.300961 tidy3d-2.3.0rc1/tidy3d/plugins/polyslab/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/polyslab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/polyslab/polyslab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.304961 tidy3d-2.3.0rc1/tidy3d/plugins/resonance/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/resonance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/resonance/resonance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.304961 tidy3d-2.3.0rc1/tidy3d/plugins/smatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/smatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/smatrix/smatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.304961 tidy3d-2.3.0rc1/tidy3d/plugins/waveguide/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/waveguide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35573 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/waveguide/rectangular_dielectric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.304961 tidy3d-2.3.0rc1/tidy3d/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)   275233 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.304961 tidy3d-2.3.0rc1/tidy3d/web/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/cli/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20751 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/http_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/httputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/material_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/material_libray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/s3utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16498 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/simulation_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24457 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/webapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.296961 tidy3d-2.3.0rc1/tidy3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-06-05 20:08:20.000000 tidy3d-2.3.0rc1/tidy3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-06-05 20:08:20.000000 tidy3d-2.3.0rc1/tidy3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:08:20.000000 tidy3d-2.3.0rc1/tidy3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-05 20:08:20.000000 tidy3d-2.3.0rc1/tidy3d.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-05 20:08:20.000000 tidy3d-2.3.0rc1/tidy3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 20:08:20.000000 tidy3d-2.3.0rc1/tidy3d.egg-info/top_level.txt
```

### Comparing `tidy3d-2.2.3/LICENSE` & `tidy3d-2.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/PKG-INFO` & `tidy3d-2.3.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.2.3
+Version: 2.3.0rc1
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Project-URL: Bug Tracker, https://github.com/flexcompute/tidy3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy3d-2.2.3/README.md` & `tidy3d-2.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/setup.py` & `tidy3d-2.3.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/_test_local/_test_adjoint_performance.py` & `tidy3d-2.3.0rc1/tests/_test_local/_test_adjoint_performance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/_test_local/_test_data_performance.py` & `tidy3d-2.3.0rc1/tests/_test_local/_test_data_performance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/_test_local/_test_fit_web.py` & `tidy3d-2.3.0rc1/tests/_test_local/_test_fit_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/_test_local/_test_plugins_web.py` & `tidy3d-2.3.0rc1/tests/_test_local/_test_plugins_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/_test_local/_test_web.py` & `tidy3d-2.3.0rc1/tests/_test_local/_test_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_components/test_IO.py` & `tidy3d-2.3.0rc1/tests/test_components/test_IO.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 
 
 def set_datasets_to_none(sim):
     sim_dict = sim.dict()
     for src in sim_dict["sources"]:
         if src["type"] == "CustomFieldSource":
             src["field_dataset"] = None
+        elif src["type"] == "CustomCurrentSource":
+            src["current_dataset"] = None
     for structure in sim_dict["structures"]:
         if structure["geometry"]["type"] == "TriangleMesh":
             structure["geometry"]["mesh_dataset"] = None
     return td.Simulation.parse_obj(sim_dict)
 
 
 @clear_tmp
```

### Comparing `tidy3d-2.2.3/tests/test_components/test_apodization.py` & `tidy3d-2.3.0rc1/tests/test_components/test_apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_components/test_base.py` & `tidy3d-2.3.0rc1/tests/test_components/test_base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_components/test_boundaries.py` & `tidy3d-2.3.0rc1/tests/test_components/test_boundaries.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_components/test_field_projection.py` & `tidy3d-2.3.0rc1/tests/test_components/test_field_projection.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_components/test_geometry.py` & `tidy3d-2.3.0rc1/tests/test_components/test_geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_components/test_grid.py` & `tidy3d-2.3.0rc1/tests/test_components/test_grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_components/test_grid_spec.py` & `tidy3d-2.3.0rc1/tests/test_components/test_grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_components/test_medium.py` & `tidy3d-2.3.0rc1/tests/test_components/test_medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_components/test_meshgenerate.py` & `tidy3d-2.3.0rc1/tests/test_components/test_meshgenerate.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_components/test_mode.py` & `tidy3d-2.3.0rc1/tests/test_components/test_mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_components/test_monitor.py` & `tidy3d-2.3.0rc1/tests/test_components/test_monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_components/test_sidewall.py` & `tidy3d-2.3.0rc1/tests/test_components/test_sidewall.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_components/test_simulation.py` & `tidy3d-2.3.0rc1/tests/test_components/test_simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import matplotlib.pylab as plt
 
 import numpy as np
 import tidy3d as td
 from tidy3d.exceptions import SetupError, ValidationError, Tidy3dKeyError
 from tidy3d.components import simulation
 from tidy3d.components.simulation import MAX_NUM_MEDIUMS
-from ..utils import assert_log_level, SIM_FULL, log_capture
+from ..utils import assert_log_level, SIM_FULL, log_capture, run_emulated, clear_tmp
 from tidy3d.constants import LARGE_NUMBER
 
 SIM = td.Simulation(size=(1, 1, 1), run_time=1e-12, grid_spec=td.GridSpec(wavelength=1.0))
 
 _, AX = plt.subplots()
 
 RTOL = 0.01
@@ -481,14 +481,18 @@
     SIM_FULL._add_cbar(eps_min=1, eps_max=2, ax=ax)
 
 
 def test_plot():
     SIM_FULL.plot(x=0, ax=AX)
 
 
+def test_plot_3d():
+    SIM_FULL.plot_3d()
+
+
 def test_structure_alpha():
     _ = SIM_FULL.plot_structures_eps(x=0, ax=AX, alpha=None)
     _ = SIM_FULL.plot_structures_eps(x=0, ax=AX, alpha=-1)
     _ = SIM_FULL.plot_structures_eps(x=0, ax=AX, alpha=1)
     _ = SIM_FULL.plot_structures_eps(x=0, ax=AX, alpha=0.5)
     _ = SIM_FULL.plot_structures_eps(x=0, ax=AX, alpha=0.5, cbar=True)
     new_structs = [
@@ -1459,14 +1463,15 @@
         geometry=td.Box(size=(1, 1, 1), center=(-1, 0, 0)),
         medium=td.PoleResidue(eps_inf=0.16, poles=[(1 + 1j, 2 + 2j)]),
     )
     sim_new = sim.copy(update=dict(structures=[structure]))
     assert sim_new.dt == 0.4 * dt
 
 
+@clear_tmp
 def test_sim_volumetric_structures():
     """Test volumetric equivalent of 2D materials."""
     sigma = 0.45
     thickness = 0.01
     medium = td.Medium2D.from_medium(td.Medium(conductivity=sigma), thickness=thickness)
     grid_dl = 0.03
     box = td.Structure(geometry=td.Box(size=(td.inf, td.inf, 0)), medium=medium)
@@ -1510,19 +1515,25 @@
         geometry=td.Box(size=(td.inf, td.inf, 0)),
         medium=td.Medium2D.from_medium(td.PEC, thickness=thickness),
     )
     below = td.Structure(
         geometry=td.Box.from_bounds([-td.inf, -td.inf, -1000], [td.inf, td.inf, 0]),
         medium=aniso_medium,
     )
-
+    monitor = td.FieldMonitor(
+        center=(0, 0, 0),
+        size=(td.inf, 0, td.inf),
+        freqs=(1.5e14),
+        name="field_xz",
+    )
     sim = td.Simulation(
         size=(10, 10, 10),
         structures=[below, box],
         sources=[src],
+        monitors=[monitor],
         boundary_spec=td.BoundarySpec(
             x=td.Boundary.pml(num_layers=5),
             y=td.Boundary.pml(num_layers=5),
             z=td.Boundary.pml(num_layers=5),
         ),
         grid_spec=td.GridSpec.uniform(dl=grid_dl),
         run_time=1e-12,
@@ -1534,14 +1545,20 @@
     )
     assert np.isclose(sim.volumetric_structures[1].medium.yy.to_medium().permittivity, 1, rtol=RTOL)
     assert np.isclose(
         sim.volumetric_structures[1].medium.xx.to_medium().conductivity,
         LARGE_NUMBER * thickness / grid_dl,
         rtol=RTOL,
     )
+    # check that plotting 2d material doesn't raise an error
+    sim_data = run_emulated(sim)
+    sim_data.plot_field(ax=AX, field_monitor_name="field_xz", field_name="Ex", val="real")
+    _ = sim.plot_eps(ax=AX, x=0, alpha=0.2)
+    _ = sim.plot(ax=AX, x=0)
+
     # nonuniform sub/super-strate should error
     below_half = td.Structure(
         geometry=td.Box.from_bounds([-100, -td.inf, -1000], [0, td.inf, 0]),
         medium=aniso_medium,
     )
 
     sim = td.Simulation(
```

### Comparing `tidy3d-2.2.3/tests/test_components/test_source.py` & `tidy3d-2.3.0rc1/tests/test_components/test_source.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_components/test_types.py` & `tidy3d-2.3.0rc1/tests/test_components/test_types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_data/test_data_arrays.py` & `tidy3d-2.3.0rc1/tests/test_data/test_data_arrays.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_data/test_monitor_data.py` & `tidy3d-2.3.0rc1/tests/test_data/test_monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_data/test_sim_data.py` & `tidy3d-2.3.0rc1/tests/test_data/test_sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_package/test_config.py` & `tidy3d-2.3.0rc1/tests/test_package/test_config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_package/test_make_script.py` & `tidy3d-2.3.0rc1/tests/test_package/test_make_script.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_package/test_material_library.py` & `tidy3d-2.3.0rc1/tests/test_package/test_material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_package/test_parametric_variants.py` & `tidy3d-2.3.0rc1/tests/test_package/test_parametric_variants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_plugins/test_adjoint.py` & `tidy3d-2.3.0rc1/tests/test_plugins/test_adjoint.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_plugins/test_component_modeler.py` & `tidy3d-2.3.0rc1/tests/test_plugins/test_component_modeler.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_plugins/test_mode_solver.py` & `tidy3d-2.3.0rc1/tests/test_plugins/test_mode_solver.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_plugins/test_polyslab.py` & `tidy3d-2.3.0rc1/tests/test_plugins/test_polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_plugins/test_resonance_finder.py` & `tidy3d-2.3.0rc1/tests/test_plugins/test_resonance_finder.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_plugins/test_waveguide.py` & `tidy3d-2.3.0rc1/tests/test_plugins/test_waveguide.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_web/test_auth.py` & `tidy3d-2.3.0rc1/tests/test_web/test_auth.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_web/test_cli.py` & `tidy3d-2.3.0rc1/tests/test_web/test_cli.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_web/test_material_fitter.py` & `tidy3d-2.3.0rc1/tests/test_web/test_material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_web/test_tidy3d_folder.py` & `tidy3d-2.3.0rc1/tests/test_web/test_tidy3d_folder.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_web/test_tidy3d_material_library.py` & `tidy3d-2.3.0rc1/tests/test_web/test_tidy3d_material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tests/test_web/test_tidy3d_task.py` & `tidy3d-2.3.0rc1/tests/test_web/test_tidy3d_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     responses.add(
         responses.POST,
         f"{Env.current.web_api_endpoint}/tidy3d/projects/1234/tasks",
         match=[
             matchers.json_params_matcher(
                 {
                     "taskName": "test task",
-                    "callbackUrl": None,
+                    "call_back_url": None,
                     "simulationType": "tidy3d",
                     "parentTasks": None,
                 }
             )
         ],
         json={
             "data": {
@@ -176,15 +176,15 @@
     responses.add(
         responses.POST,
         f"{Env.current.web_api_endpoint}/tidy3d/projects/1234/tasks",
         match=[
             matchers.json_params_matcher(
                 {
                     "taskName": "test task",
-                    "callbackUrl": None,
+                    "call_back_url": None,
                     "simulationType": "tidy3d",
                     "parentTasks": None,
                 }
             )
         ],
         json={
             "data": {
```

### Comparing `tidy3d-2.2.3/tests/test_web/test_webapi.py` & `tidy3d-2.3.0rc1/tests/test_web/test_webapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     responses.add(
         responses.POST,
         f"{Env.current.web_api_endpoint}/tidy3d/projects/{TASK_ID}/tasks",
         match=[
             matchers.json_params_matcher(
                 {
                     "taskName": TASK_NAME,
-                    "callbackUrl": None,
+                    "call_back_url": None,
                     "simulationType": "tidy3d",
                     "parentTasks": None,
                 }
             )
         ],
         json={
             "data": {
```

### Comparing `tidy3d-2.2.3/tests/utils.py` & `tidy3d-2.3.0rc1/tests/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,18 @@
             medium=Debye(eps_inf=2.0, coeffs=[(1, 3)]),
         ),
         Structure(
             geometry=Box(size=(1, 1, 1), center=(-1, 0, 0)),
             medium=Drude(eps_inf=2.0, coeffs=[(1, 3)]),
         ),
         Structure(
+            geometry=Box(size=(1, 0, 1), center=(-1, 0, 0)),
+            medium=Medium2D.from_medium(Medium(conductivity=0.45), thickness=0.01),
+        ),
+        Structure(
             geometry=GeometryGroup(geometries=[Box(size=(1, 1, 1), center=(-1, 0, 0))]),
             medium=PEC,
         ),
         Structure(
             geometry=Cylinder(radius=1.0, length=2.0, center=(1.0, 0.0, -1.0), axis=1),
             medium=AnisotropicMedium(
                 xx=td.Medium(permittivity=1),
@@ -200,14 +204,33 @@
                 Ex=ScalarFieldDataArray(
                     np.ones((101, 101, 1, 1)),
                     coords=dict(
                         x=np.linspace(-1, 1, 101),
                         y=np.linspace(-1, 1, 101),
                         z=np.array([0]),
                         f=[2e14],
+                    ),
+                )
+            ),
+        ),
+        CustomCurrentSource(
+            center=(0, 1, 2),
+            size=(2, 2, 0),
+            source_time=GaussianPulse(
+                freq0=2e14,
+                fwidth=4e13,
+            ),
+            current_dataset=FieldDataset(
+                Ex=ScalarFieldDataArray(
+                    np.ones((101, 101, 1, 1)),
+                    coords=dict(
+                        x=np.linspace(-1, 1, 101),
+                        y=np.linspace(-1, 1, 101),
+                        z=np.array([0]),
+                        f=[2e14],
                     ),
                 )
             ),
         ),
         TFSF(
             center=(1, 2, -3),
             size=(2.5, 2.5, 0.5),
```

### Comparing `tidy3d-2.2.3/tidy3d/__init__.py` & `tidy3d-2.3.0rc1/tidy3d/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 # geometry
 from .components.geometry import Box, Sphere, Cylinder, PolySlab, GeometryGroup
 from .components.geometry import TriangleMesh
 
 # medium
 from .components.medium import Medium, PoleResidue, AnisotropicMedium, PEC, PECMedium, Medium2D
 from .components.medium import Sellmeier, Debye, Drude, Lorentz
-from .components.medium import CustomMedium, FullyAnisotropicMedium
+from .components.medium import CustomMedium, CustomPoleResidue
+from .components.medium import CustomSellmeier, FullyAnisotropicMedium
+from .components.medium import CustomLorentz, CustomDrude, CustomDebye, CustomAnisotropicMedium
 from .components.transformation import RotationAroundAxis
 
 # structures
 from .components.structure import Structure, MeshOverrideStructure
 
 # modes
 from .components.mode import ModeSpec
@@ -23,15 +25,15 @@
 # apodization
 from .components.apodization import ApodizationSpec
 
 # sources
 from .components.source import GaussianPulse, ContinuousWave
 from .components.source import UniformCurrentSource, PlaneWave, ModeSource, PointDipole
 from .components.source import GaussianBeam, AstigmaticGaussianBeam
-from .components.source import CustomFieldSource, TFSF
+from .components.source import CustomFieldSource, TFSF, CustomCurrentSource
 
 # monitors
 from .components.monitor import FieldMonitor, FieldTimeMonitor, FluxMonitor, FluxTimeMonitor
 from .components.monitor import ModeMonitor, ModeSolverMonitor, PermittivityMonitor
 from .components.monitor import FieldProjectionAngleMonitor, FieldProjectionCartesianMonitor
 from .components.monitor import FieldProjectionKSpaceMonitor, FieldProjectionSurface
 from .components.monitor import DiffractionMonitor
@@ -41,15 +43,15 @@
 
 # field projection
 
 from .components.field_projection import FieldProjector
 
 # data
 from .components.data.data_array import ScalarFieldDataArray, ScalarModeFieldDataArray
-from .components.data.data_array import ScalarFieldTimeDataArray
+from .components.data.data_array import ScalarFieldTimeDataArray, SpatialDataArray
 from .components.data.data_array import ModeAmpsDataArray, ModeIndexDataArray
 from .components.data.data_array import FluxDataArray, FluxTimeDataArray
 from .components.data.data_array import FieldProjectionAngleDataArray
 from .components.data.data_array import FieldProjectionCartesianDataArray
 from .components.data.data_array import FieldProjectionKSpaceDataArray
 from .components.data.data_array import DiffractionDataArray
 from .components.data.dataset import FieldDataset, FieldTimeDataset
```

### Comparing `tidy3d-2.2.3/tidy3d/__main__.py` & `tidy3d-2.3.0rc1/tidy3d/__main__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/components/apodization.py` & `tidy3d-2.3.0rc1/tidy3d/components/apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/components/base.py` & `tidy3d-2.3.0rc1/tidy3d/components/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pylint:disable=too-many-public-methods
 """global configuration / base class for pydantic models used to make simulation."""
 from __future__ import annotations
 
 import json
 from functools import wraps
-from typing import List, Callable
+from typing import List, Callable, Dict, Union, Tuple, Any
 
 import rich
 import pydantic
 from pydantic.fields import ModelField
 import yaml
 import numpy as np
 import h5py
@@ -72,16 +72,20 @@
         try:
             return super().__hash__(self)
         except TypeError:
             return hash(self.json())
 
     def __init__(self, **kwargs):
         """Init method, includes post-init validators."""
-        super().__init__(**kwargs)
-        self._post_init_validators()
+        log.begin_capture()
+        try:
+            super().__init__(**kwargs)
+            self._post_init_validators()
+        finally:
+            log.end_capture(self)
 
     def _post_init_validators(self) -> None:
         """Call validators taking ``self`` that get run after init, implement in subclasses."""
 
     def __init_subclass__(cls) -> None:
         """Things that are done to each of the models."""
 
@@ -433,14 +437,18 @@
             Dictionary containing the model.
 
         Example
         -------
         >>> sim_dict = Simulation.dict_from_hdf5(fname='folder/sim.hdf5') # doctest: +SKIP
         """
 
+        def is_data_array(value: Any) -> bool:
+            """Whether a value is supposed to be a data array based on the contents."""
+            return isinstance(value, str) and value in DATA_ARRAY_MAP
+
         def load_data_from_file(model_dict: dict, group_path: str = "") -> None:
             """For every DataArray item in dictionary, load path of hdf5 group as value."""
 
             for key, value in model_dict.items():
 
                 subpath = f"{group_path}/{key}"
 
@@ -452,24 +460,31 @@
                             group_path=subpath,
                             model_dict=model_dict,
                             key=key,
                             value=value,
                         )
 
                 # write the path to the element of the json dict where the data_array should be
-                if isinstance(value, str) and value in DATA_ARRAY_MAP:
+                if is_data_array(value):
                     data_array_type = DATA_ARRAY_MAP[value]
                     model_dict[key] = data_array_type.from_hdf5(fname=fname, group_path=subpath)
                     continue
 
                 # if a list, assign each element a unique key, recurse
                 if isinstance(value, (list, tuple)):
+
                     value_dict = cls.tuple_to_dict(tuple_values=value)
                     load_data_from_file(model_dict=value_dict, group_path=subpath)
 
+                    # handle case of nested list of DataArray elements
+                    val_tuple = list(value_dict.values())
+                    for ind, (model_item, value_item) in enumerate(zip(model_dict[key], val_tuple)):
+                        if is_data_array(model_item):
+                            model_dict[key][ind] = value_item
+
                 # if a dict, recurse
                 elif isinstance(value, dict):
                     load_data_from_file(model_dict=value, group_path=subpath)
 
         with h5py.File(fname, "r") as f_handle:
             json_string = f_handle[JSON_TAG][()]
             model_dict = json.loads(json_string)
@@ -685,7 +700,38 @@
         # add in remaining things in the docs
         if original_docstrings:
             doc += "\n"
             doc += original_docstrings
 
         doc += "\n"
         cls.__doc__ = doc
+
+    def get_submodels_by_hash(self) -> Dict[int, List[Union[str, Tuple[str, int]]]]:
+        """Return a dictionary of this object's sub-models indexed by their hash values."""
+        fields = {}
+        for key in self.__fields__:
+            field = getattr(self, key)
+
+            if isinstance(field, Tidy3dBaseModel):
+                hash_ = hash(field)
+                if hash_ not in fields:
+                    fields[hash_] = []
+                fields[hash_].append(key)
+
+            # Do we need to consider np.ndarray here?
+            elif isinstance(field, (list, tuple, np.ndarray)):
+                for index, sub_field in enumerate(field):
+                    if isinstance(sub_field, Tidy3dBaseModel):
+                        hash_ = hash(sub_field)
+                        if hash_ not in fields:
+                            fields[hash_] = []
+                        fields[hash_].append((key, index))
+
+            elif isinstance(field, dict):
+                for index, sub_field in field.items():
+                    if isinstance(sub_field, Tidy3dBaseModel):
+                        hash_ = hash(sub_field)
+                        if hash_ not in fields:
+                            fields[hash_] = []
+                        fields[hash_].append((key, index))
+
+        return fields
```

### Comparing `tidy3d-2.2.3/tidy3d/components/boundary.py` & `tidy3d-2.3.0rc1/tidy3d/components/boundary.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/components/data/data_array.py` & `tidy3d-2.3.0rc1/tidy3d/components/data/data_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,14 +218,31 @@
     >>> data = MixedModeDataArray((1+1j) * np.random.random((3, 4, 2)), coords=coords)
     """
 
     __slots__ = ()
     _dims = ("f", "mode_index_0", "mode_index_1")
 
 
+class SpatialDataArray(DataArray):
+    """Spatial distribution.
+
+    Example
+    -------
+    >>> x = [1,2]
+    >>> y = [2,3,4]
+    >>> z = [3,4,5,6]
+    >>> coords = dict(x=x, y=y, z=z)
+    >>> fd = SpatialDataArray((1+1j) * np.random.random((2,3,4)), coords=coords)
+    """
+
+    __slots__ = ()
+    _dims = ("x", "y", "z")
+    _data_attrs = {"long_name": "field value"}
+
+
 class ScalarFieldDataArray(DataArray):
     """Spatial distribution in the frequency-domain.
 
     Example
     -------
     >>> x = [1,2]
     >>> y = [2,3,4]
@@ -421,14 +438,15 @@
 
     __slots__ = ()
     _dims = ("face_index", "vertex_index", "axis")
     _data_attrs = {"long_name": "surface mesh triangles"}
 
 
 DATA_ARRAY_TYPES = [
+    SpatialDataArray,
     ScalarFieldDataArray,
     ScalarFieldTimeDataArray,
     ScalarModeFieldDataArray,
     FluxDataArray,
     FluxTimeDataArray,
     ModeAmpsDataArray,
     ModeIndexDataArray,
```

### Comparing `tidy3d-2.2.3/tidy3d/components/data/dataset.py` & `tidy3d-2.3.0rc1/tidy3d/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/components/data/monitor_data.py` & `tidy3d-2.3.0rc1/tidy3d/components/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/components/data/sim_data.py` & `tidy3d-2.3.0rc1/tidy3d/components/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/components/field_projection.py` & `tidy3d-2.3.0rc1/tidy3d/components/field_projection.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/components/geometry.py` & `tidy3d-2.3.0rc1/tidy3d/components/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import List, Tuple, Union, Any, Callable, Optional
 from math import isclose
 import functools
 
 import pydantic
 import numpy as np
 from matplotlib import patches, path
-from shapely.geometry import Point, Polygon, box, MultiPolygon
+from shapely.geometry import Point, Polygon, box, MultiPolygon, LineString
 from shapely.validation import make_valid
 
 from .base import Tidy3dBaseModel, cached_property
 from .types import Bound, Size, Coordinate, Axis, Coordinate2D, ArrayFloat3D, PlanePosition
 from .types import Vertices, Ax, Shapely, annotate_type
 from .viz import add_ax_if_none, equal_aspect
 from .viz import PLOT_BUFFER, ARROW_LENGTH, arrow_style
@@ -44,14 +44,16 @@
 
 # sampling polygon along dilation for validating polygon to be
 # non self-intersecting during the entire dilation process
 _N_SAMPLE_POLYGON_INTERSECT = 5
 # for sampling conical frustum in visualization
 _N_SAMPLE_CURVE_SHAPELY = 40
 _IS_CLOSE_RTOL = np.finfo(float).eps
+# for shapely circular shapes discretization in visualization
+_N_SHAPELY_QUAD_SEGS = 200
 
 
 Points = ArrayFloat3D
 
 
 # pylint:disable=too-many-public-methods
 class Geometry(Tidy3dBaseModel, ABC):
@@ -415,16 +417,20 @@
         ax.set_aspect("equal")
         ax.set_title(f"cross section at {'xyz'[axis]}={position:.2f}")
         return ax
 
     def plot_shape(self, shape: Shapely, plot_params: PlotParams, ax: Ax) -> Ax:
         """Defines how a shape is plotted on a matplotlib axes."""
         _shape = self.evaluate_inf_shape(shape)
-        patch = polygon_patch(_shape, **plot_params.to_kwargs())
-        ax.add_artist(patch)
+        if isinstance(_shape, LineString):
+            xs, ys = zip(*_shape.coords)
+            ax.plot(xs, ys, color=plot_params.edgecolor)
+        else:
+            patch = polygon_patch(_shape, **plot_params.to_kwargs())
+            ax.add_artist(patch)
         return ax
 
     @classmethod
     def strip_coords(
         cls, shape: Shapely
     ) -> Tuple[List[float], List[float], Tuple[List[float], List[float]]]:
         """Get the exterior and list of interior xy coords for a shape.
@@ -1588,15 +1594,15 @@
         axis, position = self.parse_xyz_kwargs(x=x, y=y, z=z)
         if not self.intersects_axis_position(axis, position):
             return []
         z0, (x0, y0) = self.pop_axis(self.center, axis=axis)
         intersect_dist = self._intersect_dist(position, z0)
         if not intersect_dist:
             return []
-        return [Point(x0, y0).buffer(0.5 * intersect_dist)]
+        return [Point(x0, y0).buffer(0.5 * intersect_dist, quad_segs=_N_SHAPELY_QUAD_SEGS)]
 
     @cached_property
     def bounds(self) -> Bound:
         """Returns bounding box min and max coordinates.
 
         Returns
         -------
@@ -1702,15 +1708,15 @@
         # radius at z
         radius_offset = self._radius_z(z)
 
         if radius_offset <= 0:
             return []
 
         _, (x0, y0) = self.pop_axis(self.center, axis=self.axis)
-        return [Point(x0, y0).buffer(radius_offset)]
+        return [Point(x0, y0).buffer(radius_offset, quad_segs=_N_SHAPELY_QUAD_SEGS)]
 
     def _intersections_side(self, position, axis):  # pylint:disable=too-many-locals
         """Find shapely geometries intersecting cylindrical geometry with axis orthogonal to length.
         When ``sidewall_angle`` is nonzero, so that it's in fact a conical frustum or cone, the
         cross section can contain hyperbolic curves. This is currently approximated by a polygon
         of many vertices.
```

### Comparing `tidy3d-2.2.3/tidy3d/components/grid/grid.py` & `tidy3d-2.3.0rc1/tidy3d/components/grid/grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/components/grid/grid_spec.py` & `tidy3d-2.3.0rc1/tidy3d/components/grid/grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/components/grid/mesher.py` & `tidy3d-2.3.0rc1/tidy3d/components/grid/mesher.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/components/medium.py` & `tidy3d-2.3.0rc1/tidy3d/components/medium.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # pylint: disable=invalid-name, too-many-lines
 """Defines properties of the medium / materials"""
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import Tuple, Union, Callable, Optional, Dict, List
 import functools
+from math import isclose
 
 import pydantic as pd
 import numpy as np
 import xarray as xr
 
 from .base import Tidy3dBaseModel, cached_property
 from .grid.grid import Coords, Grid
-from .types import PoleAndResidue, Ax, FreqBound, TYPE_TAG_STR, InterpMethod, Bound, ArrayComplex4D
+from .types import PoleAndResidue, Ax, FreqBound, TYPE_TAG_STR, InterpMethod, Bound, ArrayComplex3D
 from .types import Axis, TensorReal
 from .data.dataset import PermittivityDataset
-from .data.data_array import ScalarFieldDataArray
+from .data.data_array import SpatialDataArray, ScalarFieldDataArray
 from .viz import add_ax_if_none
 from .geometry import Geometry
 from .validators import validate_name_str
 from ..constants import C_0, pec_val, EPSILON_0, LARGE_NUMBER, fp_eps
 from ..constants import HERTZ, CONDUCTIVITY, PERMITTIVITY, RADPERSEC, MICROMETER, SECOND
 from ..exceptions import ValidationError, SetupError
 from ..log import log
@@ -327,23 +328,228 @@
         omega = freq * 2 * np.pi
         eps_complex = self.eps_model(freq)
         eps_inf = self.eps_model(np.inf)
         sigma = (eps_inf - eps_complex) * 1j * omega * EPSILON_0
         return sigma
 
 
+class AbstractCustomMedium(AbstractMedium, ABC):
+    """A spatially varying medium."""
+
+    interp_method: InterpMethod = pd.Field(
+        "nearest",
+        title="Interpolation method",
+        description="Interpolation method to obtain permittivity values "
+        "that are not supplied at the Yee grids; For grids outside the range "
+        "of the supplied data, extrapolation will be applied. When the extrapolated "
+        "value is smaller (greater) than the minimal (maximal) of the supplied data, "
+        "the extrapolated value will take the minimal (maximal) of the supplied data.",
+    )
+
+    @cached_property
+    @abstractmethod
+    def is_isotropic(self) -> bool:
+        """The medium is isotropic or anisotropic."""
+
+    def _interp_method(self, comp: Axis) -> InterpMethod:  # pylint:disable=unused-argument
+        """Interpolation method applied to comp."""
+        return self.interp_method
+
+    @abstractmethod
+    def eps_dataarray_freq(
+        self, frequency: float
+    ) -> Tuple[SpatialDataArray, SpatialDataArray, SpatialDataArray]:
+        """Permittivity array at ``frequency``.
+
+        Parameters
+        ----------
+        frequency : float
+            Frequency to evaluate permittivity at (Hz).
+
+        Returns
+        -------
+        Tuple[:class:`.SpatialDataArray`, :class:`.SpatialDataArray`, :class:`.SpatialDataArray`]
+            The permittivity evaluated at ``frequency``.
+        """
+
+    def eps_diagonal_on_grid(
+        self,
+        frequency: float,
+        coords: Coords,
+    ) -> Tuple[ArrayComplex3D, ArrayComplex3D, ArrayComplex3D]:
+        """Spatial profile of main diagonal of the complex-valued permittivity
+        at ``frequency`` interpolated at the supplied coordinates.
+
+        Parameters
+        ----------
+        frequency : float
+            Frequency to evaluate permittivity at (Hz).
+        coords : :class:`.Coords`
+            The grid point coordinates over which interpolation is performed.
+
+        Returns
+        -------
+        Tuple[ArrayComplex3D, ArrayComplex3D, ArrayComplex3D]
+            The complex-valued permittivity tensor at ``frequency`` interpolated
+            at the supplied coordinate.
+        """
+        eps_spatial = self.eps_dataarray_freq(frequency)
+        if self.is_isotropic:
+            eps_interp = self._interp(eps_spatial[0], coords, self._interp_method(0)).values
+            return (eps_interp, eps_interp, eps_interp)
+        return tuple(
+            self._interp(eps_comp, coords, self._interp_method(comp)).values
+            for comp, eps_comp in enumerate(eps_spatial)
+        )
+
+    def eps_comp_on_grid(
+        self,
+        row: Axis,
+        col: Axis,
+        frequency: float,
+        coords: Coords,
+    ) -> ArrayComplex3D:
+        """Spatial profile of a single component of the complex-valued permittivity tensor at
+        ``frequency`` interpolated at the supplied coordinates.
+
+        Parameters
+        ----------
+        row : int
+            Component's row in the permittivity tensor (0, 1, or 2 for x, y, or z respectively).
+        col : int
+            Component's column in the permittivity tensor (0, 1, or 2 for x, y, or z respectively).
+        frequency : float
+            Frequency to evaluate permittivity at (Hz).
+        coords : :class:`.Coords`
+            The grid point coordinates over which interpolation is performed.
+
+        Returns
+        -------
+        ArrayComplex3D
+            Single component of the complex-valued permittivity tensor at ``frequency`` interpolated
+            at the supplied coordinates.
+        """
+
+        if row == col:
+            return self.eps_diagonal_on_grid(frequency, coords)[row]
+        return 0j
+
+    @ensure_freq_in_range
+    def eps_model(self, frequency: float) -> complex:
+        """Complex-valued spatially averaged permittivity as a function of frequency."""
+        if self.is_isotropic:
+            return np.mean(self.eps_dataarray_freq(frequency)[0].values)
+        return np.mean(
+            [np.mean(eps_comp.values) for eps_comp in self.eps_dataarray_freq(frequency)]
+        )
+
+    @ensure_freq_in_range
+    def eps_diagonal(self, frequency: float) -> Tuple[complex, complex, complex]:
+        """Main diagonal of the complex-valued permittivity tensor
+        at ``frequency``. Spatially, we take max{||eps||}, so that autoMesh generation
+        works appropriately.
+        """
+        eps_spatial = self.eps_dataarray_freq(frequency)
+        if self.is_isotropic:
+            eps_comp = eps_spatial[0].values.ravel()
+            eps = eps_comp[np.argmax(np.abs(eps_comp))]
+            return (eps, eps, eps)
+        eps_spatial_array = (eps_comp.values.ravel() for eps_comp in eps_spatial)
+        return tuple(eps_comp[np.argmax(np.abs(eps_comp))] for eps_comp in eps_spatial_array)
+
+    @staticmethod
+    def _validate_isreal_dataarray(dataarray: SpatialDataArray) -> bool:
+        """Validate that the dataarray is real"""
+        return np.all(np.isreal(dataarray.values))
+
+    @staticmethod
+    def _validate_isreal_dataarray_tuple(dataarray_tuple: Tuple[SpatialDataArray, ...]) -> bool:
+        """Validate that the dataarray is real"""
+        return np.all([AbstractCustomMedium._validate_isreal_dataarray(f) for f in dataarray_tuple])
+
+    @staticmethod
+    def _interp(
+        spatial_dataarray: Union[SpatialDataArray, ScalarFieldDataArray],
+        coord_interp: Coords,
+        interp_method: InterpMethod,
+    ) -> Union[SpatialDataArray, ScalarFieldDataArray]:
+        """
+        Enhance xarray's ``.interp`` in two ways:
+            1) Check if the coordinate of the supplied data are in monotically increasing order.
+            If they are, apply the faster ``assume_sorted=True``.
+
+            2) For axes of single entry, instead of error, apply ``isel()`` along the axis.
+
+            3) When linear interp is applied, in the extrapolated region, filter values smaller
+            or larger than the original data's min(max) will be replaced with the original min(max).
+
+        Parameters
+        ----------
+        spatial_dataarray: Union[:class:`.SpatialDataArray`, :class:`.ScalarFieldDataArray`]
+            Supplied scalar dataset
+        coord_interp : :class:`.Coords`
+            The grid point coordinates over which interpolation is performed.
+        interp_method : :class:`.InterpMethod`
+            Interpolation method.
+
+        Returns
+        -------
+        Union[:class:`.SpatialDataArray`, :class:`.ScalarFieldDataArray`]
+            The interpolated spatial dataset.
+        """
+
+        all_coords = "xyz"
+        is_single_entry = [spatial_dataarray.sizes[ax] == 1 for ax in all_coords]
+        interp_ax = [
+            ax for (ax, single_entry) in zip(all_coords, is_single_entry) if not single_entry
+        ]
+        isel_ax = [ax for ax in all_coords if ax not in interp_ax]
+
+        # apply isel for the axis containing single entry
+        if len(isel_ax) > 0:
+            spatial_dataarray = spatial_dataarray.isel(
+                {ax: [0] * len(coord_interp.to_dict[ax]) for ax in isel_ax}
+            )
+            spatial_dataarray = spatial_dataarray.assign_coords(
+                {ax: coord_interp.to_dict[ax] for ax in isel_ax}
+            )
+            if len(interp_ax) == 0:
+                return spatial_dataarray
+
+        # Apply interp for the rest
+        #   first check if it's sorted
+        is_sorted = all((np.all(np.diff(spatial_dataarray.coords[f]) > 0) for f in interp_ax))
+        interp_param = dict(
+            kwargs={"fill_value": FILL_VALUE},
+            assume_sorted=is_sorted,
+            method=interp_method,
+        )
+        #   interpolation
+        interp_dataarray = spatial_dataarray.interp(
+            {ax: coord_interp.to_dict[ax] for ax in interp_ax},
+            **interp_param,
+        )
+
+        # filter any values larger/smaller than the original data's max/min.
+        max_val = max(spatial_dataarray.values.ravel())
+        min_val = min(spatial_dataarray.values.ravel())
+        interp_dataarray = interp_dataarray.where(interp_dataarray >= min_val, min_val)
+        interp_dataarray = interp_dataarray.where(interp_dataarray <= max_val, max_val)
+        return interp_dataarray
+
+
 """ Dispersionless Medium """
 
 # PEC keyword
 class PECMedium(AbstractMedium):
     """Perfect electrical conductor class.
 
     Note
     ----
-    To avoid confusion from duplicate PECs, should import ``tidy3d.PEC`` instance directly.
+    To avoid confusion from duplicate PECs, must import ``tidy3d.PEC`` instance directly.
     """
 
     def eps_model(self, frequency: float) -> complex:
 
         # return something like frequency with value of pec_val + 0j
         return 0j * frequency + pec_val
 
@@ -373,15 +579,15 @@
         1.0, ge=1.0, title="Permittivity", description="Relative permittivity.", units=PERMITTIVITY
     )
 
     conductivity: float = pd.Field(
         0.0,
         ge=0.0,
         title="Conductivity",
-        description="Electric conductivity.  Defined such that the imaginary part of the complex "
+        description="Electric conductivity. Defined such that the imaginary part of the complex "
         "permittivity at angular frequency omega is given by conductivity/omega.",
         units=CONDUCTIVITY,
     )
 
     @cached_property
     def n_cfl(self):
         """This property computes the index of refraction related to CFL condition, so that
@@ -418,352 +624,559 @@
         :class:`Medium`
             medium containing the corresponding ``permittivity`` and ``conductivity``.
         """
         eps, sigma = AbstractMedium.nk_to_eps_sigma(n, k, freq)
         return cls(permittivity=eps, conductivity=sigma, **kwargs)
 
 
-class CustomMedium(AbstractMedium):
+class CustomIsotropicMedium(AbstractCustomMedium, Medium):
     """:class:`.Medium` with user-supplied permittivity distribution.
+    (This class is for internal use in v2.0; it will be renamed as `CustomMedium` in v3.0.)
 
     Example
     -------
     >>> Nx, Ny, Nz = 10, 9, 8
     >>> X = np.linspace(-1, 1, Nx)
     >>> Y = np.linspace(-1, 1, Ny)
     >>> Z = np.linspace(-1, 1, Nz)
-    >>> freqs = [2e14]
-    >>> data = np.ones((Nx, Ny, Nz, 1))
-    >>> eps_diagonal_data = ScalarFieldDataArray(data, coords=dict(x=X, y=Y, z=Z, f=freqs))
-    >>> eps_components = {f"eps_{d}{d}": eps_diagonal_data for d in "xyz"}
-    >>> eps_dataset = PermittivityDataset(**eps_components)
-    >>> dielectric = CustomMedium(eps_dataset=eps_dataset, name='my_medium')
+    >>> coords = dict(x=X, y=Y, z=Z)
+    >>> permittivity= SpatialDataArray(np.ones((Nx, Ny, Nz)), coords=coords)
+    >>> conductivity= SpatialDataArray(np.ones((Nx, Ny, Nz)), coords=coords)
+    >>> dielectric = CustomIsotropicMedium(permittivity=permittivity, conductivity=conductivity)
     >>> eps = dielectric.eps_model(200e12)
     """
 
-    eps_dataset: PermittivityDataset = pd.Field(
+    permittivity: SpatialDataArray = pd.Field(
         ...,
-        title="Permittivity Dataset",
-        description="User-supplied dataset containing complex-valued permittivity "
-        "as a function of space. Permittivity distribution over the Yee-grid will be "
-        "interpolated based on ``interp_method``.",
+        title="Permittivity",
+        description="Relative permittivity.",
+        units=PERMITTIVITY,
     )
 
-    interp_method: InterpMethod = pd.Field(
-        "nearest",
-        title="Interpolation method",
-        description="Interpolation method to obtain permittivity values "
-        "that are not supplied at the Yee grids; For grids outside the range "
-        "of the supplied data, extrapolation will be applied. When the extrapolated "
-        "value is smaller (greater) than the minimal (maximal) of the supplied data, "
-        "the extrapolated value will take the minimal (maximal) of the supplied data.",
+    conductivity: Optional[SpatialDataArray] = pd.Field(
+        None,
+        title="Conductivity",
+        description="Electric conductivity. Defined such that the imaginary part of the complex "
+        "permittivity at angular frequency omega is given by conductivity/omega.",
+        units=CONDUCTIVITY,
+    )
+
+    @pd.validator("permittivity", always=True)
+    def _eps_inf_greater_no_less_than_one(cls, val):
+        """Assert any eps_inf must be >=1"""
+
+        if not CustomIsotropicMedium._validate_isreal_dataarray(val):
+            raise SetupError("'permittivity' must be real.")
+
+        if np.any(val.values < 1):
+            raise SetupError("'permittivity' must be no less than one.")
+
+        return val
+
+    @pd.validator("conductivity", always=True)
+    def _conductivity_non_negative_correct_shape(cls, val, values):
+        """Assert conductivity>=0"""
+
+        if val is None:
+            return val
+
+        if values.get("permittivity") is None:
+            raise ValidationError("'permittivity' failed validation.")
+
+        if not CustomIsotropicMedium._validate_isreal_dataarray(val):
+            raise SetupError("'conductivity' must be real.")
+
+        if np.any(val.values < 0):
+            raise SetupError("'conductivity' must be non-negative.")
+
+        if values["permittivity"].coords != val.coords:
+            raise SetupError("'permittivity' and 'conductivity' must have the same coordinates.")
+        return val
+
+    @cached_property
+    def n_cfl(self):
+        """This property computes the index of refraction related to CFL condition, so that
+        the FDTD with this medium is stable when the time step size that doesn't take
+        material factor into account is multiplied by ``n_cfl``.
+
+        For dispersiveless medium, it equals ``sqrt(permittivity)``.
+        """
+        return np.sqrt(np.min(self.permittivity.values))
+
+    @cached_property
+    def is_isotropic(self):
+        """Whether the medium is isotropic."""
+        return True
+
+    def eps_dataarray_freq(
+        self, frequency: float
+    ) -> Tuple[SpatialDataArray, SpatialDataArray, SpatialDataArray]:
+        """Permittivity array at ``frequency``.
+
+        Parameters
+        ----------
+        frequency : float
+            Frequency to evaluate permittivity at (Hz).
+
+        Returns
+        -------
+        Tuple[:class:`.SpatialDataArray`, :class:`.SpatialDataArray`, :class:`.SpatialDataArray`]
+            The permittivity evaluated at ``frequency``.
+        """
+        conductivity = self.conductivity
+        if conductivity is None:
+            conductivity = xr.zeros_like(self.permittivity)
+        eps = self.eps_sigma_to_eps_complex(self.permittivity, conductivity, frequency)
+        return (eps, eps, eps)
+
+
+class CustomMedium(AbstractCustomMedium):
+    """:class:`.Medium` with user-supplied permittivity distribution.
+
+    Example
+    -------
+    >>> Nx, Ny, Nz = 10, 9, 8
+    >>> X = np.linspace(-1, 1, Nx)
+    >>> Y = np.linspace(-1, 1, Ny)
+    >>> Z = np.linspace(-1, 1, Nz)
+    >>> coords = dict(x=X, y=Y, z=Z)
+    >>> permittivity= SpatialDataArray(np.ones((Nx, Ny, Nz)), coords=coords)
+    >>> conductivity= SpatialDataArray(np.ones((Nx, Ny, Nz)), coords=coords)
+    >>> dielectric = CustomMedium(permittivity=permittivity, conductivity=conductivity)
+    >>> eps = dielectric.eps_model(200e12)
+    """
+
+    permittivity: Optional[SpatialDataArray] = pd.Field(
+        None,
+        title="Permittivity",
+        description="Spatial profile of relative permittivity.",
+        units=PERMITTIVITY,
+    )
+
+    conductivity: Optional[SpatialDataArray] = pd.Field(
+        None,
+        title="Conductivity",
+        description="Spatial profile Electric conductivity. Defined such "
+        "that the imaginary part of the complex permittivity at angular "
+        "frequency omega is given by conductivity/omega.",
+        units=CONDUCTIVITY,
     )
 
+    eps_dataset: Optional[PermittivityDataset] = pd.Field(
+        None,
+        title="Permittivity Dataset",
+        description="[To be deprecated] User-supplied dataset containing complex-valued "
+        "permittivity as a function of space. Permittivity distribution over the Yee-grid "
+        "will be interpolated based on ``interp_method``.",
+    )
+
+    @pd.root_validator(pre=True)
+    def _deprecation_dataset(cls, values):
+        """Raise deprecation warning if dataset supplied and convert to dataset."""
+
+        eps_dataset = values.get("eps_dataset")
+        permittivity = values.get("permittivity")
+        conductivity = values.get("conductivity")
+
+        # Incomplete custom medium definition.
+        if eps_dataset is None and permittivity is None and conductivity is None:
+            raise SetupError("Missing spatial profiles of 'permittivity' or 'eps_dataset'.")
+        if eps_dataset is None and permittivity is None:
+            raise SetupError("Missing spatial profiles of 'permittivity'.")
+
+        # Definition racing
+        if eps_dataset is not None and (permittivity is not None or conductivity is not None):
+            raise SetupError(
+                "Please either define 'permittivity' and 'conductivity', or 'eps_dataset', "
+                "but not both simultaneously."
+            )
+
+        if eps_dataset is None:
+            return values
+
+        # TODO: sometime before 3.0, uncomment these lines to warn users to start using new API
+        # if isinstance(eps_dataset, dict):
+        #     eps_components = [eps_dataset[f"eps_{dim}{dim}"] for dim in "xyz"]
+        # else:
+        #     eps_components = [eps_dataset.eps_xx, eps_dataset.eps_yy, eps_dataset.eps_zz]
+
+        # is_isotropic = eps_components[0] == eps_components[1] == eps_components[2]
+
+        # if is_isotropic:
+        #     # deprecation warning for isotropic custom medium
+        #     log.warning(
+        #         "For spatially varying isotropic medium, the 'eps_dataset' field "
+        #         "is being replaced by 'permittivity' and 'conductivity' in v3.0. "
+        #         "We recommend you change your scripts to be compatible with the new API."
+        #     )
+        # else:
+        #     # deprecation warning for anisotropic custom medium
+        #     log.warning(
+        #         "For spatially varying anisotropic medium, this class is being replaced "
+        #         "by 'CustomAnisotropicMedium' in v3.0. "
+        #         "We recommend you change your scripts to be compatible with the new API."
+        #     )
+
+        return values
+
     @pd.validator("eps_dataset", always=True)
-    def _single_frequency(cls, val):
+    def _eps_dataset_single_frequency(cls, val):
         """Assert only one frequency supplied."""
+        if val is None:
+            return val
+
         for name, eps_dataset_component in val.field_components.items():
             freqs = eps_dataset_component.f
             if len(freqs) != 1:
                 raise SetupError(
                     f"'eps_dataset.{name}' must have a single frequency, "
                     f"but it contains {len(freqs)} frequencies."
                 )
         return val
 
     @pd.validator("eps_dataset", always=True)
-    def _eps_inf_greater_no_less_than_one_sigma_positive(cls, val):
+    def _eps_dataset_eps_inf_greater_no_less_than_one_sigma_positive(cls, val):
         """Assert any eps_inf must be >=1"""
+        if val is None:
+            return val
 
         for comp in ["eps_xx", "eps_yy", "eps_zz"]:
-            eps_inf, sigma = CustomMedium.eps_complex_to_eps_sigma(
+            eps_real, sigma = CustomMedium.eps_complex_to_eps_sigma(
                 val.field_components[comp], val.field_components[comp].f
             )
-            if np.any(eps_inf.values < 1):
+            if np.any(eps_real.values < 1):
                 raise SetupError(
                     "Permittivity at infinite frequency at any spatial point "
                     "must be no less than one."
                 )
             if np.any(sigma.values < 0):
                 raise SetupError(
                     "Negative imaginary part of refrative index leads to a gain medium, "
                     "which is not supported."
                 )
         return val
 
+    @pd.validator("permittivity", always=True)
+    def _eps_inf_greater_no_less_than_one(cls, val):
+        """Assert any eps_inf must be >=1"""
+        if val is None:
+            return val
+
+        if not CustomMedium._validate_isreal_dataarray(val):
+            raise SetupError("'permittivity' must be real.")
+
+        if np.any(val.values < 1):
+            raise SetupError("'permittivity' must be no less than one.")
+
+        return val
+
+    @pd.validator("conductivity", always=True)
+    def _conductivity_non_negative_correct_shape(cls, val, values):
+        """Assert conductivity>=0"""
+
+        if val is None:
+            return val
+
+        if values.get("permittivity") is None:
+            raise ValidationError("'permittivity' failed validation.")
+
+        if not CustomMedium._validate_isreal_dataarray(val):
+            raise SetupError("'conductivity' must be real.")
+
+        if np.any(val.values < 0):
+            raise SetupError("'conductivity' must be non-negative.")
+
+        if values["permittivity"].coords != val.coords:
+            raise SetupError("'permittivity' and 'conductivity' must have the same coordinates.")
+        return val
+
+    @cached_property
+    def is_isotropic(self) -> bool:
+        """Check if the medium is isotropic or anisotropic."""
+        if self.eps_dataset is None:
+            return True
+        if self.eps_dataset.eps_xx == self.eps_dataset.eps_yy == self.eps_dataset.eps_zz:
+            return True
+        return False
+
+    @cached_property
+    def freqs(self) -> np.ndarray:
+        """float array of frequencies.
+        This field is to be deprecated in v3.0.
+        """
+        # return dummy values in this case
+        if self.eps_dataset is None:
+            return np.array([0, 0, 0])
+        return np.array(
+            [
+                self.eps_dataset.eps_xx.coords["f"],
+                self.eps_dataset.eps_yy.coords["f"],
+                self.eps_dataset.eps_zz.coords["f"],
+            ]
+        )
+
+    @cached_property
+    def _medium(self):
+        """Internal representation in the form of
+        either `CustomIsotropicMedium` or `CustomAnisotropicMedium`.
+        """
+        # isotropic
+        if self.eps_dataset is None:
+            return CustomIsotropicMedium(
+                permittivity=self.permittivity,
+                conductivity=self.conductivity,
+                interp_method=self.interp_method,
+            )
+        # isotropic, but with `eps_dataset`
+        if self.is_isotropic:
+            eps_real, sigma = CustomMedium.eps_complex_to_eps_sigma(
+                np.array(self.eps_dataset.eps_xx.values), self.freqs[0]
+            )
+            coords = self.eps_dataset.eps_xx.coords
+            eps_real = ScalarFieldDataArray(eps_real, coords=coords)
+            sigma = ScalarFieldDataArray(sigma, coords=coords)
+            eps_real = SpatialDataArray(eps_real.squeeze(dim="f", drop=True))
+            sigma = SpatialDataArray(sigma.squeeze(dim="f", drop=True))
+            return CustomIsotropicMedium(
+                permittivity=eps_real,
+                conductivity=sigma,
+                interp_method=self.interp_method,
+            )
+        # anisotropic
+        eps_field_components = self.eps_dataset.field_components
+        mat_comp = {"interp_method": self.interp_method}
+        for comp in ["xx", "yy", "zz"]:
+            eps_real, sigma = CustomMedium.eps_complex_to_eps_sigma(
+                eps_field_components["eps_" + comp], eps_field_components["eps_" + comp].coords["f"]
+            )
+            eps_real = SpatialDataArray(eps_real.squeeze(dim="f", drop=True))
+            sigma = SpatialDataArray(sigma.squeeze(dim="f", drop=True))
+            mat_comp.update(
+                {
+                    comp: CustomIsotropicMedium(
+                        permittivity=eps_real, conductivity=sigma, interp_method=self.interp_method
+                    )
+                }
+            )
+        return CustomAnisotropicMediumInternal(**mat_comp)
+
+    def _interp_method(self, comp: Axis) -> InterpMethod:
+        """Interpolation method applied to comp."""
+        return self._medium._interp_method(comp)  # pylint:disable=protected-access
+
     @cached_property
     def n_cfl(self):
         """This property computes the index of refraction related to CFL condition, so that
         the FDTD with this medium is stable when the time step size that doesn't take
         material factor into account is multiplied by ``n_cfl```.
 
         For dispersiveless custom medium, it equals ``min[sqrt(eps_inf)]``, where ``min``
         is performed over all components and spatial points.
         """
-        eps_array_min = [
-            float(np.min(eps_array.real))
-            for _, eps_array in self.eps_dataset.field_components.items()
-        ]
-        return np.sqrt(min(eps_array_min))
+        return self._medium.n_cfl
 
-    @ensure_freq_in_range
-    def eps_dataset_freq(self, frequency: float) -> PermittivityDataset:
-        """Permittivity dataset at ``frequency``. The dispersion comes
-        from DC conductivity that results in nonzero Im[eps].
+    def eps_dataarray_freq(
+        self, frequency: float
+    ) -> Tuple[SpatialDataArray, SpatialDataArray, SpatialDataArray]:
+        """Permittivity array at ``frequency``. ()
 
         Parameters
         ----------
         frequency : float
             Frequency to evaluate permittivity at (Hz).
 
         Returns
         -------
-        :class:`.PermittivityDataset`
+        Tuple[:class:`.SpatialDataArray`, :class:`.SpatialDataArray`, :class:`.SpatialDataArray`]
             The permittivity evaluated at ``frequency``.
         """
-
-        new_field_components = {}
-        for name, eps_dataset_component in self.eps_dataset.field_components.items():
-            freq = eps_dataset_component.coords["f"][0]
-            eps_freq = (
-                eps_dataset_component.real + 1j * eps_dataset_component.imag * freq / frequency
-            )
-            eps_freq = eps_freq.assign_coords({"f": [frequency]})
-            new_field_components.update({name: eps_freq})
-        return PermittivityDataset(**new_field_components)
+        return self._medium.eps_dataarray_freq(frequency)
 
     def eps_diagonal_on_grid(
         self,
         frequency: float,
         coords: Coords,
-    ) -> Tuple[ArrayComplex4D, ArrayComplex4D, ArrayComplex4D]:
+    ) -> Tuple[ArrayComplex3D, ArrayComplex3D, ArrayComplex3D]:
         """Spatial profile of main diagonal of the complex-valued permittivity
         at ``frequency`` interpolated at the supplied coordinates.
 
         Parameters
         ----------
         frequency : float
             Frequency to evaluate permittivity at (Hz).
         coords : :class:`.Coords`
             The grid point coordinates over which interpolation is performed.
 
         Returns
         -------
-        Tuple[np.ndarray, np.ndarray, np.ndarray]
+        Tuple[ArrayComplex3D, ArrayComplex3D, ArrayComplex3D]
             The complex-valued permittivity tensor at ``frequency`` interpolated
             at the supplied coordinate.
         """
-
-        eps_freq = self.eps_dataset_freq(frequency)
-        interp_shape = [len(coord_comp) for coord_comp in coords.to_list]
-        eps_list = [
-            np.array(
-                self._interp(eps_freq.field_components[comp], coords, self.interp_method)
-            ).reshape(interp_shape)
-            for comp in ["eps_xx", "eps_yy", "eps_zz"]
-        ]
-        return tuple(eps_list)
-
-    def eps_comp_on_grid(
-        self,
-        row: Axis,
-        col: Axis,
-        frequency: float,
-        coords: Coords,
-    ) -> ArrayComplex4D:
-        """Spatial profile of a single component of the complex-valued permittivity tensor at
-        ``frequency`` interpolated at the supplied coordinates.
-
-        Parameters
-        ----------
-        row : int
-            Component's row in the permittivity tensor (0, 1, or 2 for x, y, or z respectively).
-        col : int
-            Component's column in the permittivity tensor (0, 1, or 2 for x, y, or z respectively).
-        frequency : float
-            Frequency to evaluate permittivity at (Hz).
-        coords : :class:`.Coords`
-            The grid point coordinates over which interpolation is performed.
-
-        Returns
-        -------
-        np.ndarray
-            Single component of the complex-valued permittivity tensor at ``frequency`` interpolated
-            at the supplied coordinates.
-        """
-
-        if row == col:
-            eps_freq = self.eps_dataset_freq(frequency)
-            interp_shape = [len(coord_comp) for coord_comp in coords.to_list]
-            comp = ["eps_xx", "eps_yy", "eps_zz"][row]
-            eps = self._interp(eps_freq.field_components[comp], coords, self.interp_method)
-            eps = np.array(eps).reshape(interp_shape)
-            return eps
-        return 0
+        return self._medium.eps_diagonal_on_grid(frequency, coords)
 
     @ensure_freq_in_range
     def eps_diagonal(self, frequency: float) -> Tuple[complex, complex, complex]:
         """Main diagonal of the complex-valued permittivity tensor
         at ``frequency``. Spatially, we take max{|eps|}, so that autoMesh generation
         works appropriately.
         """
-        eps_freq = self.eps_dataset_freq(frequency)
-        eps_np_list = [
-            np.array(sclr_fld).ravel() for _, sclr_fld in eps_freq.field_components.items()
-        ]
-        eps_list = [eps_comp[np.argmax(np.abs(eps_comp))] for eps_comp in eps_np_list]
-        return tuple(eps_list)
+        return self._medium.eps_diagonal(frequency)
 
     @ensure_freq_in_range
     def eps_model(self, frequency: float) -> complex:
         """Spatial and polarizaiton average of complex-valued permittivity
         as a function of frequency.
         """
-        eps_freq = self.eps_dataset_freq(frequency)
-        eps_array_avgs = [np.mean(eps_array) for _, eps_array in eps_freq.field_components.items()]
-        return np.mean(eps_array_avgs)
+        return self._medium.eps_model(frequency)
 
     @classmethod
     def from_eps_raw(
-        cls, eps: ScalarFieldDataArray, interp_method: InterpMethod = "nearest"
+        cls,
+        eps: Union[ScalarFieldDataArray, SpatialDataArray],
+        freq: float = None,
+        interp_method: InterpMethod = "nearest",
     ) -> CustomMedium:
         """Construct a :class:`.CustomMedium` from datasets containing raw permittivity values.
 
         Parameters
         ----------
-        eps : :class:`.ScalarFieldDataArray`
+        eps : Union[:class:`.SpatialDataArray`, :class:`.ScalarFieldDataArray`]
             Dataset containing complex-valued permittivity as a function of space.
+        freq : float, optional
+            Frequency at which ``eps`` are defined.
         interp_method : :class:`.InterpMethod`, optional
-                Interpolation method to obtain permittivity values that are not supplied
-                at the Yee grids.
+            Interpolation method to obtain permittivity values that are not supplied
+            at the Yee grids.
+
+        Note
+        ----
+        For lossy medium that has a complex-valued ``eps``, if ``eps`` is supplied through
+        :class:`.SpatialDataArray`, which doesn't contain frequency information,
+        the ``freq`` kwarg will be used to evaluate the permittivity and conductivity.
+        Alternatively, ``eps`` can be supplied through :class:`.ScalarFieldDataArray`,
+        which contains a frequency coordinate.
+        In this case, leave ``freq`` kwarg as the default of ``None``.
 
         Returns
         -------
         :class:`.CustomMedium`
             Medium containing the spatially varying permittivity data.
         """
-        field_components = {field_name: eps.copy() for field_name in ("eps_xx", "eps_yy", "eps_zz")}
-        eps_dataset = PermittivityDataset(**field_components)
-        return cls(eps_dataset=eps_dataset, interp_method=interp_method)
+        if isinstance(eps, SpatialDataArray):
+            # purely real, not need to know `freq`
+            if CustomMedium._validate_isreal_dataarray(eps):
+                return cls(permittivity=eps, interp_method=interp_method)
+            # complex permittivity, needs to know `freq`
+            if freq is None:
+                raise SetupError(
+                    "For a complex 'eps', 'freq' at which 'eps' is defined must be supplied",
+                )
+            eps_real, sigma = CustomMedium.eps_complex_to_eps_sigma(eps, freq)
+            return cls(permittivity=eps_real, conductivity=sigma, interp_method=interp_method)
+
+        # eps is ScalarFieldDataArray
+        # contradictory definition of frequency
+        freq_data = eps.coords["f"].data[0]
+        if freq is not None and not isclose(freq, freq_data):
+            raise SetupError(
+                "'freq' value is inconsistent with the coordinate 'f'"
+                "in 'eps' DataArray. It's unclear at which frequency 'eps' "
+                "is defined. Please leave 'freq=None' to use the frequency "
+                "value in the DataArray."
+            )
+        eps_real, sigma = CustomMedium.eps_complex_to_eps_sigma(eps, freq_data)
+        eps_real = SpatialDataArray(eps_real.squeeze(dim="f", drop=True))
+        sigma = SpatialDataArray(sigma.squeeze(dim="f", drop=True))
+        return cls(permittivity=eps_real, conductivity=sigma, interp_method=interp_method)
 
     @classmethod
     def from_nk(
         cls,
-        n: ScalarFieldDataArray,
-        k: Optional[ScalarFieldDataArray] = None,
+        n: Union[ScalarFieldDataArray, SpatialDataArray],
+        k: Optional[Union[ScalarFieldDataArray, SpatialDataArray]] = None,
+        freq: float = None,
         interp_method: InterpMethod = "nearest",
     ) -> CustomMedium:
         """Construct a :class:`.CustomMedium` from datasets containing n and k values.
 
         Parameters
         ----------
-        n : :class:`.ScalarFieldDataArray`
+        n : Union[:class:`.SpatialDataArray`, :class:`.ScalarFieldDataArray`]
             Real part of refractive index.
-        k : :class:`.ScalarFieldDataArray` = None
-            Imaginary part of refrative index.
+        k : Union[:class:`.SpatialDataArray`, :class:`.ScalarFieldDataArray`], optional
+            Imaginary part of refrative index for lossy medium.
+        freq : float, optional
+            Frequency at which ``n`` and ``k`` are defined.
         interp_method : :class:`.InterpMethod`, optional
-                Interpolation method to obtain permittivity values that are not supplied
-                at the Yee grids.
+            Interpolation method to obtain permittivity values that are not supplied
+            at the Yee grids.
+
+        Note
+        ----
+        For lossy medium, if both ``n`` and ``k`` are supplied through
+        :class:`.SpatialDataArray`, which doesn't contain frequency information,
+        the ``freq`` kwarg will be used to evaluate the permittivity and conductivity.
+        Alternatively, ``n`` and ``k`` can be supplied through :class:`.ScalarFieldDataArray`,
+        which contains a frequency coordinate.
+        In this case, leave ``freq`` kwarg as the default of ``None``.
 
         Returns
         -------
         :class:`.CustomMedium`
             Medium containing the spatially varying permittivity data.
         """
+        # lossless
         if k is None:
-            k = xr.zeros_like(n)
-
+            if isinstance(n, ScalarFieldDataArray):
+                n = SpatialDataArray(n.squeeze(dim="f", drop=True))
+            freq = 0  # dummy value
+            eps_real, _ = CustomMedium.nk_to_eps_sigma(n, 0 * n, freq)
+            return cls(permittivity=eps_real, interp_method=interp_method)
+
+        # lossy case
+        if n.coords.keys() != k.coords.keys():
+            raise SetupError("'n' and 'k' must be of the same type.")
         if n.coords != k.coords:
-            raise SetupError("`n` and `k` must have same coordinates.")
-
-        eps_values = Medium.nk_to_eps_complex(n=n.data, k=k.data)
-        coords = {k: np.array(v) for k, v in n.coords.items()}
-        eps_scalar_field_data = ScalarFieldDataArray(eps_values, coords=coords)
-        return cls.from_eps_raw(eps=eps_scalar_field_data, interp_method=interp_method)
-
-    @staticmethod
-    def _interp(
-        scalar_dataset: ScalarFieldDataArray,
-        coord_interp: Coords,
-        interp_method: InterpMethod,
-    ) -> ScalarFieldDataArray:
-        """
-        Enhance xarray's ``.interp`` in two ways:
-            1) Check if the coordinate of the supplied data are in monotically increasing order.
-            If they are, apply the faster ``assume_sorted=True``.
-
-            2) For axes of single entry, instead of error, apply ``isel()`` along the axis.
-
-            3) When linear interp is applied, in the extrapolated region, filter values smaller
-            or larger than the original data's min(max) will be replaced with the original min(max).
-
-        Parameters
-        ----------
-        scalar_dataset : :class:`.ScalarFieldDataArray`
-            Supplied scalar dataset.
-        coord_interp : :class:`.Coords`
-            The grid point coordinates over which interpolation is performed.
-        interp_method : :class:`.InterpMethod`
-            Interpolation method.
-
-        Returns
-        -------
-        :class:`.ScalarFieldDataArray`
-            The interpolated scalar dataset.
-        """
+            raise SetupError("'n' and 'k' must have same coordinates.")
 
-        # check in x/y/z axes, which of them are supplied with a single entry.
-        all_coords = "xyz"
-        is_single_entry = [scalar_dataset.sizes[ax] == 1 for ax in all_coords]
-        interp_ax = [
-            ax for (ax, single_entry) in zip(all_coords, is_single_entry) if not single_entry
-        ]
-        isel_ax = [ax for ax in all_coords if ax not in interp_ax]
+        # k is a SpatialDataArray
+        if isinstance(k, SpatialDataArray):
+            if freq is None:
+                raise SetupError(
+                    "For a lossy medium, must supply 'freq' at which to convert 'n' "
+                    "and 'k' to a complex valued permittivity."
+                )
+            eps_real, sigma = CustomMedium.nk_to_eps_sigma(n, k, freq)
+            return cls(permittivity=eps_real, conductivity=sigma, interp_method=interp_method)
 
-        # apply isel for the axis containing single entry
-        if len(isel_ax) > 0:
-            scalar_dataset = scalar_dataset.isel(
-                {ax: [0] * len(coord_interp.to_dict[ax]) for ax in isel_ax}
+        # k is a ScalarFieldDataArray
+        freq_data = k.coords["f"].data[0]
+        if freq is not None and not isclose(freq, freq_data):
+            raise SetupError(
+                "'freq' value is inconsistent with the coordinate 'f'"
+                "in 'k' DataArray. It's unclear at which frequency 'k' "
+                "is defined. Please leave 'freq=None' to use the frequency "
+                "value in the DataArray."
             )
-            scalar_dataset = scalar_dataset.assign_coords(
-                {ax: coord_interp.to_dict[ax] for ax in isel_ax}
-            )
-            if len(interp_ax) == 0:
-                return scalar_dataset
 
-        # Apply interp for the rest
-        #   first check if it's sorted
-        is_sorted = all((np.all(np.diff(scalar_dataset.coords[f]) > 0) for f in interp_ax))
-        interp_param = dict(
-            kwargs={"fill_value": FILL_VALUE},
-            assume_sorted=is_sorted,
-            method=interp_method,
-        )
-        #   interpolation
-        interp_dataset = scalar_dataset.interp(
-            {ax: coord_interp.to_dict[ax] for ax in interp_ax},
-            **interp_param,
-        )
-
-        # filter any values larger/smaller than the original data's max/min.
-        max_val = max(scalar_dataset.values.ravel())
-        min_val = min(scalar_dataset.values.ravel())
-        interp_dataset = interp_dataset.where(interp_dataset >= min_val, min_val)
-        interp_dataset = interp_dataset.where(interp_dataset <= max_val, max_val)
-        return interp_dataset
+        eps_real, sigma = CustomMedium.nk_to_eps_sigma(n, k, freq_data)
+        eps_real = SpatialDataArray(eps_real.squeeze(dim="f", drop=True))
+        sigma = SpatialDataArray(sigma.squeeze(dim="f", drop=True))
+        return cls(permittivity=eps_real, conductivity=sigma, interp_method=interp_method)
 
     def grids(self, bounds: Bound) -> Dict[str, Grid]:
         """Make a :class:`.Grid` corresponding to the data in each ``eps_ii`` component.
         The min and max coordinates along each dimension are bounded by ``bounds``."""
 
         rmin, rmax = bounds
         pt_mins = dict(zip("xyz", rmin))
         pt_maxs = dict(zip("xyz", rmax))
 
-        def make_grid(scalar_field: ScalarFieldDataArray) -> Grid:
+        def make_grid(scalar_field: Union[ScalarFieldDataArray, SpatialDataArray]) -> Grid:
             """Make a grid for a single dataset."""
 
             def make_bound_coords(coords: np.ndarray, pt_min: float, pt_max: float) -> List[float]:
                 """Convert user supplied coords into boundary coords to use in :class:`.Grid`."""
 
                 # get coordinates of the bondaries halfway between user-supplied data
                 coord_bounds = (coords[1:] + coords[:1]) / 2.0
@@ -804,18 +1217,22 @@
 
 """ Dispersive Media """
 
 
 class DispersiveMedium(AbstractMedium, ABC):
     """A Medium with dispersion (propagation characteristics depend on frequency)"""
 
-    @cached_property
     @abstractmethod
+    def _pole_residue_dict(self) -> Dict:
+        """Dict representation of Medium as a pole-residue model."""
+
+    @cached_property
     def pole_residue(self):
         """Representation of Medium as a pole-residue model."""
+        return PoleResidue(**self._pole_residue_dict())
 
     @cached_property
     def n_cfl(self):
         """This property computes the index of refraction related to CFL condition, so that
         the FDTD with this medium is stable when the time step size that doesn't take
         material factor into account is multiplied by ``n_cfl``.
 
@@ -834,14 +1251,39 @@
     @staticmethod
     def complex_to_tuple(value: complex) -> Tuple[float, float]:
         """Convert a complex number to a tuple of real and imaginary parts."""
 
         return (value.real, value.imag)
 
 
+class CustomDispersiveMedium(AbstractCustomMedium, DispersiveMedium, ABC):
+    """A spatially varying dispersive medium."""
+
+    @cached_property
+    def n_cfl(self):
+        """This property computes the index of refraction related to CFL condition, so that
+        the FDTD with this medium is stable when the time step size that doesn't take
+        material factor into account is multiplied by ``n_cfl``.
+
+        For PoleResidue model, it equals ``sqrt(eps_inf)``
+        [https://ieeexplore.ieee.org/document/9082879].
+        """
+        return np.sqrt(np.min(self.pole_residue.eps_inf.values))
+
+    @cached_property
+    def is_isotropic(self):
+        """Whether the medium is isotropic."""
+        return True
+
+    @cached_property
+    def pole_residue(self):
+        """Representation of Medium as a pole-residue model."""
+        return CustomPoleResidue(**self._pole_residue_dict(), interp_method=self.interp_method)
+
+
 class PoleResidue(DispersiveMedium):
     """A dispersive medium described by the pole-residue pair model.
     The frequency-dependence of the complex-valued permittivity is described by:
 
     Note
     ----
     .. math::
@@ -879,19 +1321,18 @@
         for (a, c) in self.poles:
             a_cc = np.conj(a)
             c_cc = np.conj(c)
             eps -= c / (1j * omega + a)
             eps -= c_cc / (1j * omega + a_cc)
         return eps
 
-    @cached_property
-    def pole_residue(self):
-        """Representation of Medium as a pole-residue model."""
+    def _pole_residue_dict(self) -> Dict:
+        """Dict representation of Medium as a pole-residue model."""
 
-        return PoleResidue(
+        return dict(
             eps_inf=self.eps_inf,
             poles=self.poles,
             frequency_range=self.frequency_range,
             name=self.name,
         )
 
     def __str__(self):
@@ -941,14 +1382,159 @@
         return Medium(
             permittivity=self.eps_inf,
             conductivity=np.real(sigma),
             frequency_range=self.frequency_range,
         )
 
 
+class CustomPoleResidue(CustomDispersiveMedium, PoleResidue):
+    """A spatially varying dispersive medium described by the pole-residue pair model.
+    The frequency-dependence of the complex-valued permittivity is described by:
+
+    Note
+    ----
+    .. math::
+
+        \\epsilon(\\omega) = \\epsilon_\\infty - \\sum_i
+        \\left[\\frac{c_i}{j \\omega + a_i} +
+        \\frac{c_i^*}{j \\omega + a_i^*}\\right]
+
+    Example
+    -------
+    >>> x = np.linspace(-1, 1, 5)
+    >>> y = np.linspace(-1, 1, 6)
+    >>> z = np.linspace(-1, 1, 7)
+    >>> coords = dict(x=x, y=y, z=z)
+    >>> eps_inf = SpatialDataArray(np.ones((5, 6, 7)), coords=coords)
+    >>> a1 = SpatialDataArray(np.random.random((5, 6, 7)), coords=coords)
+    >>> c1 = SpatialDataArray(np.random.random((5, 6, 7)), coords=coords)
+    >>> a2 = SpatialDataArray(np.random.random((5, 6, 7)), coords=coords)
+    >>> c2 = SpatialDataArray(np.random.random((5, 6, 7)), coords=coords)
+    >>> pole_res = CustomPoleResidue(eps_inf=eps_inf, poles=[(a1, c1), (a2, c2)])
+    >>> eps = pole_res.eps_model(200e12)
+    """
+
+    eps_inf: SpatialDataArray = pd.Field(
+        ...,
+        title="Epsilon at Infinity",
+        description="Relative permittivity at infinite frequency (:math:`\\epsilon_\\infty`).",
+        units=PERMITTIVITY,
+    )
+
+    poles: Tuple[Tuple[SpatialDataArray, SpatialDataArray], ...] = pd.Field(
+        (),
+        title="Poles",
+        description="Tuple of complex-valued (:math:`a_i, c_i`) poles for the model.",
+        units=(RADPERSEC, RADPERSEC),
+    )
+
+    @pd.validator("eps_inf", always=True)
+    def _eps_inf_positive(cls, val):
+        """eps_inf must be positive"""
+        if not CustomDispersiveMedium._validate_isreal_dataarray(val):
+            raise SetupError("'eps_inf' must be real.")
+        if np.any(val < 0):
+            raise SetupError("'eps_inf' must be positive.")
+        return val
+
+    @pd.validator("poles", always=True)
+    def _poles_correct_shape(cls, val, values):
+        """poles must have the same shape."""
+        if values.get("eps_inf") is None:
+            raise ValidationError("'eps_inf' failed validation.")
+
+        expected_coords = values["eps_inf"].coords
+        for coeffs in val:
+            for coeff in coeffs:
+                if coeff.coords != expected_coords:
+                    raise SetupError(
+                        "All pole coefficients 'a' and 'c' must have the same coordinates; "
+                        "The coordinates must also be consistent with 'eps_inf'."
+                    )
+        return val
+
+    def eps_dataarray_freq(
+        self, frequency: float
+    ) -> Tuple[SpatialDataArray, SpatialDataArray, SpatialDataArray]:
+        """Permittivity array at ``frequency``.
+
+        Parameters
+        ----------
+        frequency : float
+            Frequency to evaluate permittivity at (Hz).
+
+        Returns
+        -------
+        Tuple[:class:`.SpatialDataArray`, :class:`.SpatialDataArray`, :class:`.SpatialDataArray`]
+            The permittivity evaluated at ``frequency``.
+        """
+        eps = PoleResidue.eps_model(self, frequency)
+        return (eps, eps, eps)
+
+    def poles_on_grid(self, coords: Coords) -> Tuple[Tuple[ArrayComplex3D, ArrayComplex3D], ...]:
+        """Spatial profile of poles interpolated at the supplied coordinates.
+
+        Parameters
+        ----------
+        coords : :class:`.Coords`
+            The grid point coordinates over which interpolation is performed.
+
+        Returns
+        -------
+        Tuple[Tuple[ArrayComplex3D, ArrayComplex3D], ...]
+            The poles interpolated at the supplied coordinate.
+        """
+
+        def fun_interp(input_data: SpatialDataArray) -> ArrayComplex3D:
+            return self._interp(input_data, coords, self.interp_method).values
+
+        return tuple((fun_interp(a), fun_interp(c)) for (a, c) in self.poles)
+
+    @classmethod
+    def from_medium(cls, medium: CustomMedium) -> "CustomPoleResidue":
+        """Convert a :class:`.CustomMedium` to a pole residue model.
+
+        Parameters
+        ----------
+        medium: :class:`.CustomMedium`
+            The medium with permittivity and conductivity to convert.
+
+        Returns
+        -------
+        :class:`.CustomPoleResidue`
+            The pole residue equivalent.
+        """
+        poles = [(0, medium.conductivity / (2 * EPSILON_0))]
+        return CustomPoleResidue(
+            eps_inf=medium.permittivity, poles=poles, frequency_range=medium.frequency_range
+        )
+
+    def to_medium(self) -> CustomMedium:
+        """Convert to a :class:`.CustomMedium`.
+        Requires the pole residue model to only have a pole at 0 frequency,
+        corresponding to a constant conductivity term.
+
+        Returns
+        -------
+        :class:`.CustomMedium`
+            The non-dispersive equivalent with constant permittivity and conductivity.
+        """
+        res = 0
+        for (a, c) in self.poles:
+            if abs(a) > fp_eps:
+                raise ValidationError("Cannot convert dispersive 'PoleResidue' to 'Medium'.")
+            res += (c + np.conj(c)) / 2
+        sigma = res * 2 * EPSILON_0
+        return CustomMedium(
+            permittivity=self.eps_inf,
+            conductivity=np.real(sigma),
+            frequency_range=self.frequency_range,
+        )
+
+
 class Sellmeier(DispersiveMedium):
     """A dispersive medium described by the Sellmeier model.
     The frequency-dependence of the refractive index is described by:
 
     Note
     ----
     .. math::
@@ -980,32 +1566,33 @@
     @ensure_freq_in_range
     def eps_model(self, frequency: float) -> complex:
         """Complex-valued permittivity as a function of frequency."""
 
         n = self._n_model(frequency)
         return AbstractMedium.nk_to_eps_complex(n)
 
-    @cached_property
-    def pole_residue(self):
-        """Representation of Medium as a pole-residue model."""
-
+    def _pole_residue_dict(self) -> Dict:
+        """Dict representation of Medium as a pole-residue model"""
         poles = []
         for (B, C) in self.coeffs:
             beta = 2 * np.pi * C_0 / np.sqrt(C)
             alpha = -0.5 * beta * B
             a = 1j * beta
             c = 1j * alpha
             poles.append((a, c))
+        return dict(eps_inf=1, poles=poles, frequency_range=self.frequency_range, name=self.name)
 
-        return PoleResidue(
-            eps_inf=1,
-            poles=poles,
-            frequency_range=self.frequency_range,
-            name=self.name,
-        )
+    @staticmethod
+    def _from_dispersion_to_coeffs(n: float, freq: float, dn_dwvl: float):
+        """Compute Sellmeier coefficients from dispersion."""
+        wvl = C_0 / np.array(freq)
+        nsqm1 = n**2 - 1
+        c_coeff = -(wvl**3) * n * dn_dwvl / (nsqm1 - wvl * n * dn_dwvl)
+        b_coeff = (wvl**2 - c_coeff) / wvl**2 * nsqm1
+        return [(b_coeff, c_coeff)]
 
     @classmethod
     def from_dispersion(cls, n: float, freq: float, dn_dwvl: float = 0, **kwargs):
         """Convert ``n`` and wavelength dispersion ``dn_dwvl`` values at frequency ``freq`` to
         a single-pole :class:`Sellmeier` medium.
 
         Parameters
@@ -1024,22 +1611,124 @@
             valuesat at the prvoided frequency.
         """
 
         if dn_dwvl >= 0:
             raise ValidationError("Dispersion ``dn_dwvl`` must be smaller than zero.")
         if n < 1:
             raise ValidationError("Refractive index ``n`` cannot be smaller than one.")
+        return cls(coeffs=cls._from_dispersion_to_coeffs(n, freq, dn_dwvl), **kwargs)
 
-        wvl = C_0 / np.array(freq)
-        nsqm1 = n**2 - 1
-        c_coeff = -(wvl**3) * n * dn_dwvl / (nsqm1 - wvl * n * dn_dwvl)
-        b_coeff = (wvl**2 - c_coeff) / wvl**2 * nsqm1
-        coeffs = [(b_coeff, c_coeff)]
 
-        return cls(coeffs=coeffs, **kwargs)
+class CustomSellmeier(CustomDispersiveMedium, Sellmeier):
+    """A spatially varying dispersive medium described by the Sellmeier model.
+    The frequency-dependence of the refractive index is described by:
+
+    Note
+    ----
+    .. math::
+
+        n(\\lambda)^2 = 1 + \\sum_i \\frac{B_i \\lambda^2}{\\lambda^2 - C_i}
+
+    Example
+    -------
+    >>> x = np.linspace(-1, 1, 5)
+    >>> y = np.linspace(-1, 1, 6)
+    >>> z = np.linspace(-1, 1, 7)
+    >>> coords = dict(x=x, y=y, z=z)
+    >>> b1 = SpatialDataArray(np.random.random((5, 6, 7)), coords=coords)
+    >>> c1 = SpatialDataArray(np.random.random((5, 6, 7)), coords=coords)
+    >>> sellmeier_medium = CustomSellmeier(coeffs=[(b1,c1),])
+    >>> eps = sellmeier_medium.eps_model(200e12)
+    """
+
+    coeffs: Tuple[Tuple[SpatialDataArray, SpatialDataArray], ...] = pd.Field(
+        title="Coefficients",
+        description="List of Sellmeier (:math:`B_i, C_i`) coefficients.",
+        units=(None, MICROMETER + "^2"),
+    )
+
+    @pd.validator("coeffs", always=True)
+    def _correct_shape_and_sign(cls, val):
+        """every term in coeffs must have the same shape, and B>=0 and C>0."""
+        expected_coords = val[0][0].coords
+        for (B, C) in val:
+            if B.coords != expected_coords or C.coords != expected_coords:
+                raise SetupError("Every term in 'coeffs' must have the same coordinates.")
+            if not CustomDispersiveMedium._validate_isreal_dataarray_tuple((B, C)):
+                raise SetupError("'B' and 'C' must be real.")
+            if np.any(C <= 0):
+                raise SetupError("'C' must be positive.")
+        return val
+
+    def _pole_residue_dict(self) -> Dict:
+        """Dict representation of Medium as a pole-residue model."""
+        poles_dict = Sellmeier._pole_residue_dict(self)
+        poles_dict.update({"eps_inf": xr.ones_like(self.coeffs[0][0])})
+        return poles_dict
+
+    def eps_dataarray_freq(
+        self, frequency: float
+    ) -> Tuple[SpatialDataArray, SpatialDataArray, SpatialDataArray]:
+        """Permittivity array at ``frequency``.
+
+        Parameters
+        ----------
+        frequency : float
+            Frequency to evaluate permittivity at (Hz).
+
+        Returns
+        -------
+        Tuple[:class:`.SpatialDataArray`, :class:`.SpatialDataArray`, :class:`.SpatialDataArray`]
+            The permittivity evaluated at ``frequency``.
+        """
+        eps = Sellmeier.eps_model(self, frequency)
+        return (eps, eps, eps)
+
+    @classmethod
+    def from_dispersion(
+        cls,
+        n: SpatialDataArray,
+        freq: float,
+        dn_dwvl: SpatialDataArray,
+        interp_method="nearest",
+        **kwargs,
+    ):  # pylint:disable=signature-differs
+        """Convert ``n`` and wavelength dispersion ``dn_dwvl`` values at frequency ``freq`` to
+        a single-pole :class:`CustomSellmeier` medium.
+
+        Parameters
+        ----------
+        n : :class:`.SpatialDataArray`
+            Real part of refractive index. Must be larger than or equal to one.
+        dn_dwvl : :class:`.SpatialDataArray`
+            Derivative of the refractive index with wavelength (1/um). Must be negative.
+        freq : float
+            Frequency at which ``n`` and ``dn_dwvl`` are sampled.
+        interp_method : :class:`.InterpMethod`, optional
+            Interpolation method to obtain permittivity values that are not supplied
+            at the Yee grids.
+
+        Returns
+        -------
+        :class:`.CustomSellmeier`
+            Single-pole Sellmeier medium with the prvoided refractive index and index dispersion
+            valuesat at the prvoided frequency.
+        """
+
+        if n.shape != dn_dwvl.shape:
+            raise ValidationError("'n' and'dn_dwvl' must have the same dimension.")
+        if np.any(dn_dwvl >= 0):
+            raise ValidationError("Dispersion ``dn_dwvl`` must be smaller than zero.")
+        if np.any(n < 1):
+            raise ValidationError("Refractive index ``n`` cannot be smaller than one.")
+        return cls(
+            coeffs=cls._from_dispersion_to_coeffs(n, freq, dn_dwvl),
+            interp_method=interp_method,
+            **kwargs,
+        )
 
 
 class Lorentz(DispersiveMedium):
     """A dispersive medium described by the Lorentz model.
     The frequency-dependence of the complex-valued permittivity is described by:
 
     Note
@@ -1065,53 +1754,174 @@
     coeffs: Tuple[Tuple[float, float, float], ...] = pd.Field(
         ...,
         title="Coefficients",
         description="List of (:math:`\\Delta\\epsilon_i, f_i, \\delta_i`) values for model.",
         units=(PERMITTIVITY, HERTZ, HERTZ),
     )
 
+    @pd.validator("coeffs", always=True)
+    def _coeffs_unequal_f_delta(cls, val):
+        """f and delta cannot be exactly the same."""
+        for (_, f, delta) in val:
+            if f == delta:
+                raise SetupError("'f' and 'delta' cannot take equal values.")
+        return val
+
     @ensure_freq_in_range
     def eps_model(self, frequency: float) -> complex:
         """Complex-valued permittivity as a function of frequency."""
 
         eps = self.eps_inf + 0.0j
         for (de, f, delta) in self.coeffs:
             eps += (de * f**2) / (f**2 - 2j * frequency * delta - frequency**2)
         return eps
 
-    @cached_property
-    def pole_residue(self):
-        """Representation of Medium as a pole-residue model."""
+    def _pole_residue_dict(self) -> Dict:
+        """Dict representation of Medium as a pole-residue model."""
 
         poles = []
         for (de, f, delta) in self.coeffs:
 
             w = 2 * np.pi * f
             d = 2 * np.pi * delta
 
-            if d > w:
+            if self._all_larger(d, w):
                 r = np.sqrt(d * d - w * w) + 0j
                 a0 = -d + r
                 c0 = de * w**2 / 4 / r
                 a1 = -d - r
                 c1 = -c0
                 poles.extend(((a0, c0), (a1, c1)))
             else:
                 r = np.sqrt(w * w - d * d)
                 a = -d - 1j * r
                 c = 1j * de * w**2 / 2 / r
                 poles.append((a, c))
 
-        return PoleResidue(
+        return dict(
             eps_inf=self.eps_inf,
             poles=poles,
             frequency_range=self.frequency_range,
             name=self.name,
         )
 
+    @staticmethod
+    def _all_larger(coeff_a, coeff_b) -> bool:
+        """`coeff_a` and `coeff_b` can be either float or SpatialDataArray."""
+        if isinstance(coeff_a, SpatialDataArray):
+            return np.all(coeff_a.values > coeff_b.values)
+        return coeff_a > coeff_b
+
+
+class CustomLorentz(CustomDispersiveMedium, Lorentz):
+    """A spatially varying dispersive medium described by the Lorentz model.
+    The frequency-dependence of the complex-valued permittivity is described by:
+
+    Note
+    ----
+    .. math::
+
+        \\epsilon(f) = \\epsilon_\\infty + \\sum_i
+        \\frac{\\Delta\\epsilon_i f_i^2}{f_i^2 - 2jf\\delta_i - f^2}
+
+    Example
+    -------
+    >>> x = np.linspace(-1, 1, 5)
+    >>> y = np.linspace(-1, 1, 6)
+    >>> z = np.linspace(-1, 1, 7)
+    >>> coords = dict(x=x, y=y, z=z)
+    >>> eps_inf = SpatialDataArray(np.ones((5, 6, 7)), coords=coords)
+    >>> d_epsilon = SpatialDataArray(np.random.random((5, 6, 7)), coords=coords)
+    >>> f = SpatialDataArray(1+np.random.random((5, 6, 7)), coords=coords)
+    >>> delta = SpatialDataArray(np.random.random((5, 6, 7)), coords=coords)
+    >>> lorentz_medium = CustomLorentz(eps_inf=eps_inf, coeffs=[(d_epsilon,f,delta),])
+    >>> eps = lorentz_medium.eps_model(200e12)
+    """
+
+    eps_inf: SpatialDataArray = pd.Field(
+        ...,
+        title="Epsilon at Infinity",
+        description="Relative permittivity at infinite frequency (:math:`\\epsilon_\\infty`).",
+        units=PERMITTIVITY,
+    )
+
+    coeffs: Tuple[Tuple[SpatialDataArray, SpatialDataArray, SpatialDataArray], ...] = pd.Field(
+        ...,
+        title="Coefficients",
+        description="List of (:math:`\\Delta\\epsilon_i, f_i, \\delta_i`) values for model.",
+        units=(PERMITTIVITY, HERTZ, HERTZ),
+    )
+
+    @pd.validator("eps_inf", always=True)
+    def _eps_inf_positive(cls, val):
+        """eps_inf must be positive"""
+        if not CustomDispersiveMedium._validate_isreal_dataarray(val):
+            raise SetupError("'eps_inf' must be real.")
+        if np.any(val < 0):
+            raise SetupError("'eps_inf' must be positive.")
+        return val
+
+    @pd.validator("coeffs", always=True)
+    def _coeffs_unequal_f_delta(cls, val):
+        """f and delta cannot be exactly the same.
+        Not needed for now because we have a more strict
+        validator `_coeffs_delta_all_smaller_or_larger_than_fi`.
+        """
+        return val
+
+    @pd.validator("coeffs", always=True)
+    def _coeffs_correct_shape_and_sign(cls, val, values):
+        """coeffs must have consistent shape and sign."""
+        if values.get("eps_inf") is None:
+            raise ValidationError("'eps_inf' failed validation.")
+
+        expected_coords = values["eps_inf"].coords
+        for (de, f, delta) in val:
+            if (
+                de.coords != expected_coords
+                or f.coords != expected_coords
+                or delta.coords != expected_coords
+            ):
+                raise SetupError(
+                    "All terms in 'coeffs' must have the same coordinates; "
+                    "The coordinates must also be consistent with 'eps_inf'."
+                )
+            if not CustomDispersiveMedium._validate_isreal_dataarray_tuple((de, f, delta)):
+                raise SetupError("All terms in 'coeffs' must be real.")
+        return val
+
+    @pd.validator("coeffs", always=True)
+    def _coeffs_delta_all_smaller_or_larger_than_fi(cls, val):
+        """We restrict either all f>delta or all f<delta for now."""
+        for (_, f, delta) in val:
+            if not (Lorentz._all_larger(f, delta) or Lorentz._all_larger(delta, f)):
+                raise SetupError(
+                    "Coefficients in 'coeffs' are restricted to have "
+                    "either all 'delta'<'f' or all 'delta'>'f'."
+                )
+        return val
+
+    def eps_dataarray_freq(
+        self, frequency: float
+    ) -> Tuple[SpatialDataArray, SpatialDataArray, SpatialDataArray]:
+        """Permittivity array at ``frequency``.
+
+        Parameters
+        ----------
+        frequency : float
+            Frequency to evaluate permittivity at (Hz).
+
+        Returns
+        -------
+        Tuple[:class:`.SpatialDataArray`, :class:`.SpatialDataArray`, :class:`.SpatialDataArray`]
+            The permittivity evaluated at ``frequency``.
+        """
+        eps = Lorentz.eps_model(self, frequency)
+        return (eps, eps, eps)
+
 
 class Drude(DispersiveMedium):
     """A dispersive medium described by the Drude model.
     The frequency-dependence of the complex-valued permittivity is described by:
 
     Note
     ----
@@ -1145,39 +1955,128 @@
         """Complex-valued permittivity as a function of frequency."""
 
         eps = self.eps_inf + 0.0j
         for (f, delta) in self.coeffs:
             eps -= (f**2) / (frequency**2 + 1j * frequency * delta)
         return eps
 
-    @cached_property
-    def pole_residue(self):
-        """Representation of Medium as a pole-residue model."""
+    def _pole_residue_dict(self) -> Dict:
+        """Dict representation of Medium as a pole-residue model."""
 
         poles = []
-        a0 = 0j
 
         for (f, delta) in self.coeffs:
 
             w = 2 * np.pi * f
             d = 2 * np.pi * delta
 
             c0 = (w**2) / 2 / d + 0j
             c1 = -c0
             a1 = -d + 0j
 
+            if isinstance(c0, complex):
+                a0 = 0j
+            else:
+                a0 = xr.zeros_like(c0)
+
             poles.extend(((a0, c0), (a1, c1)))
-        return PoleResidue(
+
+        return dict(
             eps_inf=self.eps_inf,
             poles=poles,
             frequency_range=self.frequency_range,
             name=self.name,
         )
 
 
+class CustomDrude(CustomDispersiveMedium, Drude):
+    """A spatially varying dispersive medium described by the Drude model.
+    The frequency-dependence of the complex-valued permittivity is described by:
+
+    Note
+    ----
+    .. math::
+
+        \\epsilon(f) = \\epsilon_\\infty - \\sum_i
+        \\frac{ f_i^2}{f^2 + jf\\delta_i}
+
+    Example
+    -------
+    >>> x = np.linspace(-1, 1, 5)
+    >>> y = np.linspace(-1, 1, 6)
+    >>> z = np.linspace(-1, 1, 7)
+    >>> coords = dict(x=x, y=y, z=z)
+    >>> eps_inf = SpatialDataArray(np.ones((5, 6, 7)), coords=coords)
+    >>> f1 = SpatialDataArray(np.random.random((5, 6, 7)), coords=coords)
+    >>> delta1 = SpatialDataArray(np.random.random((5, 6, 7)), coords=coords)
+    >>> drude_medium = CustomDrude(eps_inf=eps_inf, coeffs=[(f1,delta1),])
+    >>> eps = drude_medium.eps_model(200e12)
+    """
+
+    eps_inf: SpatialDataArray = pd.Field(
+        ...,
+        title="Epsilon at Infinity",
+        description="Relative permittivity at infinite frequency (:math:`\\epsilon_\\infty`).",
+        units=PERMITTIVITY,
+    )
+
+    coeffs: Tuple[Tuple[SpatialDataArray, SpatialDataArray], ...] = pd.Field(
+        ...,
+        title="Coefficients",
+        description="List of (:math:`f_i, \\delta_i`) values for model.",
+        units=(HERTZ, HERTZ),
+    )
+
+    @pd.validator("eps_inf", always=True)
+    def _eps_inf_positive(cls, val):
+        """eps_inf must be positive"""
+        if not CustomDispersiveMedium._validate_isreal_dataarray(val):
+            raise SetupError("'eps_inf' must be real.")
+        if np.any(val < 0):
+            raise SetupError("'eps_inf' must be positive.")
+        return val
+
+    @pd.validator("coeffs", always=True)
+    def _coeffs_correct_shape_and_sign(cls, val, values):
+        """coeffs must have consistent shape and sign."""
+        if values.get("eps_inf") is None:
+            raise ValidationError("'eps_inf' failed validation.")
+
+        expected_coords = values["eps_inf"].coords
+        for (f, delta) in val:
+            if f.coords != expected_coords or delta.coords != expected_coords:
+                raise SetupError(
+                    "All terms in 'coeffs' must have the same coordinates; "
+                    "The coordinates must also be consistent with 'eps_inf'."
+                )
+            if not CustomDispersiveMedium._validate_isreal_dataarray_tuple((f, delta)):
+                raise SetupError("All terms in 'coeffs' must be real.")
+            if np.any(delta < 0):
+                raise SetupError("'delta' must be non-negative.")
+        return val
+
+    def eps_dataarray_freq(
+        self, frequency: float
+    ) -> Tuple[SpatialDataArray, SpatialDataArray, SpatialDataArray]:
+        """Permittivity array at ``frequency``.
+
+        Parameters
+        ----------
+        frequency : float
+            Frequency to evaluate permittivity at (Hz).
+
+        Returns
+        -------
+        Tuple[:class:`.SpatialDataArray`, :class:`.SpatialDataArray`, :class:`.SpatialDataArray`]
+            The permittivity evaluated at ``frequency``.
+        """
+        eps = Drude.eps_model(self, frequency)
+        return (eps, eps, eps)
+
+
 class Debye(DispersiveMedium):
     """A dispersive medium described by the Debye model.
     The frequency-dependence of the complex-valued permittivity is described by:
 
     Note
     ----
     .. math::
@@ -1210,34 +2109,127 @@
         """Complex-valued permittivity as a function of frequency."""
 
         eps = self.eps_inf + 0.0j
         for (de, tau) in self.coeffs:
             eps += de / (1 - 1j * frequency * tau)
         return eps
 
-    @cached_property
-    def pole_residue(self):
-        """Representation of Medium as a pole-residue model."""
+    def _pole_residue_dict(self):
+        """Dict representation of Medium as a pole-residue model."""
 
         poles = []
         for (de, tau) in self.coeffs:
             a = -2 * np.pi / tau + 0j
             c = -0.5 * de * a
 
             poles.append((a, c))
 
-        return PoleResidue(
+        return dict(
             eps_inf=self.eps_inf,
             poles=poles,
             frequency_range=self.frequency_range,
             name=self.name,
         )
 
 
-IsotropicMediumType = Union[Medium, PoleResidue, Sellmeier, Lorentz, Debye, Drude]
+class CustomDebye(CustomDispersiveMedium, Debye):
+    """A spatially varying dispersive medium described by the Debye model.
+    The frequency-dependence of the complex-valued permittivity is described by:
+
+    Note
+    ----
+    .. math::
+
+        \\epsilon(f) = \\epsilon_\\infty + \\sum_i
+        \\frac{\\Delta\\epsilon_i}{1 - jf\\tau_i}
+
+    Example
+    -------
+    >>> x = np.linspace(-1, 1, 5)
+    >>> y = np.linspace(-1, 1, 6)
+    >>> z = np.linspace(-1, 1, 7)
+    >>> coords = dict(x=x, y=y, z=z)
+    >>> eps_inf = SpatialDataArray(1+np.random.random((5, 6, 7)), coords=coords)
+    >>> eps1 = SpatialDataArray(np.random.random((5, 6, 7)), coords=coords)
+    >>> tau1 = SpatialDataArray(np.random.random((5, 6, 7)), coords=coords)
+    >>> debye_medium = CustomDebye(eps_inf=eps_inf, coeffs=[(eps1,tau1),])
+    >>> eps = debye_medium.eps_model(200e12)
+    """
+
+    eps_inf: SpatialDataArray = pd.Field(
+        ...,
+        title="Epsilon at Infinity",
+        description="Relative permittivity at infinite frequency (:math:`\\epsilon_\\infty`).",
+        units=PERMITTIVITY,
+    )
+
+    coeffs: Tuple[Tuple[SpatialDataArray, SpatialDataArray], ...] = pd.Field(
+        ...,
+        title="Coefficients",
+        description="List of (:math:`\\Delta\\epsilon_i, \\tau_i`) values for model.",
+        units=(PERMITTIVITY, SECOND),
+    )
+
+    @pd.validator("eps_inf", always=True)
+    def _eps_inf_positive(cls, val):
+        """eps_inf must be positive"""
+        if not CustomDispersiveMedium._validate_isreal_dataarray(val):
+            raise SetupError("'eps_inf' must be real.")
+        if np.any(val < 0):
+            raise SetupError("'eps_inf' must be positive.")
+        return val
+
+    @pd.validator("coeffs", always=True)
+    def _coeffs_correct_shape_and_sign(cls, val, values):
+        """coeffs must have consistent shape and sign."""
+        if values.get("eps_inf") is None:
+            raise ValidationError("'eps_inf' failed validation.")
+
+        expected_coords = values["eps_inf"].coords
+        for (de, tau) in val:
+            if de.coords != expected_coords or tau.coords != expected_coords:
+                raise SetupError(
+                    "All terms in 'coeffs' must have the same coordinates; "
+                    "The coordinates must also be consistent with 'eps_inf'."
+                )
+            if not CustomDispersiveMedium._validate_isreal_dataarray_tuple((de, tau)):
+                raise SetupError("All terms in 'coeffs' must be real.")
+            if np.any(tau <= 0):
+                raise SetupError("'tau' must be positive.")
+        return val
+
+    def eps_dataarray_freq(
+        self, frequency: float
+    ) -> Tuple[SpatialDataArray, SpatialDataArray, SpatialDataArray]:
+        """Permittivity array at ``frequency``.
+
+        Parameters
+        ----------
+        frequency : float
+            Frequency to evaluate permittivity at (Hz).
+
+        Returns
+        -------
+        Tuple[:class:`.SpatialDataArray`, :class:`.SpatialDataArray`, :class:`.SpatialDataArray`]
+            The permittivity evaluated at ``frequency``.
+        """
+        eps = Debye.eps_model(self, frequency)
+        return (eps, eps, eps)
+
+
+IsotropicUniformMediumType = Union[Medium, PoleResidue, Sellmeier, Lorentz, Debye, Drude]
+IsotropicCustomMediumType = Union[
+    CustomPoleResidue,
+    CustomSellmeier,
+    CustomLorentz,
+    CustomDebye,
+    CustomDrude,
+]
+IsotropicCustomMediumInternalType = Union[IsotropicCustomMediumType, CustomIsotropicMedium]
+IsotropicMediumType = Union[IsotropicCustomMediumType, IsotropicUniformMediumType]
 
 
 class AnisotropicMedium(AbstractMedium):
     """Diagonally anisotropic medium.
 
     Note
     ----
@@ -1247,29 +2239,29 @@
     -------
     >>> medium_xx = Medium(permittivity=4.0)
     >>> medium_yy = Medium(permittivity=4.1)
     >>> medium_zz = Medium(permittivity=3.9)
     >>> anisotropic_dielectric = AnisotropicMedium(xx=medium_xx, yy=medium_yy, zz=medium_zz)
     """
 
-    xx: IsotropicMediumType = pd.Field(
+    xx: IsotropicUniformMediumType = pd.Field(
         ...,
         title="XX Component",
         description="Medium describing the xx-component of the diagonal permittivity tensor.",
         discriminator=TYPE_TAG_STR,
     )
 
-    yy: IsotropicMediumType = pd.Field(
+    yy: IsotropicUniformMediumType = pd.Field(
         ...,
         title="YY Component",
         description="Medium describing the yy-component of the diagonal permittivity tensor.",
         discriminator=TYPE_TAG_STR,
     )
 
-    zz: IsotropicMediumType = pd.Field(
+    zz: IsotropicUniformMediumType = pd.Field(
         ...,
         title="ZZ Component",
         description="Medium describing the zz-component of the diagonal permittivity tensor.",
         discriminator=TYPE_TAG_STR,
     )
 
     @cached_property
@@ -1343,15 +2335,15 @@
         ax.set_xlabel("frequency (THz)")
         ax.set_title("medium dispersion")
         ax.legend()
         ax.set_aspect("auto")
         return ax
 
     @property
-    def elements(self) -> Dict[str, IsotropicMediumType]:
+    def elements(self) -> Dict[str, IsotropicUniformMediumType]:
         """The diagonal elements of the medium as a dictionary."""
         return dict(xx=self.xx, yy=self.yy, zz=self.zz)
 
 
 class FullyAnisotropicMedium(AbstractMedium):
     """Fully anisotropic medium including all 9 components of the permittivity and conductivity
     tensors. Provided permittivity tensor and the symmetric part of the conductivity tensor must
@@ -1550,27 +2542,200 @@
             k_line.set_label(f"k, eps_{label} {direction_str}")
             n_line.set_label(f"n, eps_{label} {direction_str}")
 
         ax.legend()
         return ax
 
 
+class CustomAnisotropicMedium(AbstractCustomMedium, AnisotropicMedium):
+    """Diagonally anisotropic medium with spatially varying permittivity in each component.
+
+    Note
+    ----
+    Only diagonal anisotropy is currently supported.
+
+    Example
+    -------
+    >>> Nx, Ny, Nz = 10, 9, 8
+    >>> x = np.linspace(-1, 1, Nx)
+    >>> y = np.linspace(-1, 1, Ny)
+    >>> z = np.linspace(-1, 1, Nz)
+    >>> coords = dict(x=x, y=y, z=z)
+    >>> permittivity= SpatialDataArray(np.ones((Nx, Ny, Nz)), coords=coords)
+    >>> conductivity= SpatialDataArray(np.ones((Nx, Ny, Nz)), coords=coords)
+    >>> medium_xx = CustomMedium(permittivity=permittivity, conductivity=conductivity)
+    >>> medium_yy = CustomMedium(permittivity=permittivity, conductivity=conductivity)
+    >>> d_epsilon = SpatialDataArray(np.random.random((Nx, Ny, Nz)), coords=coords)
+    >>> f = SpatialDataArray(1+np.random.random((Nx, Ny, Nz)), coords=coords)
+    >>> delta = SpatialDataArray(np.random.random((Nx, Ny, Nz)), coords=coords)
+    >>> medium_zz = CustomLorentz(eps_inf=permittivity, coeffs=[(d_epsilon,f,delta),])
+    >>> anisotropic_dielectric = CustomAnisotropicMedium(xx=medium_xx, yy=medium_yy, zz=medium_zz)
+    """
+
+    xx: Union[IsotropicCustomMediumType, CustomMedium] = pd.Field(
+        ...,
+        title="XX Component",
+        description="Medium describing the xx-component of the diagonal permittivity tensor.",
+        discriminator=TYPE_TAG_STR,
+    )
+
+    yy: Union[IsotropicCustomMediumType, CustomMedium] = pd.Field(
+        ...,
+        title="YY Component",
+        description="Medium describing the yy-component of the diagonal permittivity tensor.",
+        discriminator=TYPE_TAG_STR,
+    )
+
+    zz: Union[IsotropicCustomMediumType, CustomMedium] = pd.Field(
+        ...,
+        title="ZZ Component",
+        description="Medium describing the zz-component of the diagonal permittivity tensor.",
+        discriminator=TYPE_TAG_STR,
+    )
+
+    interp_method: Optional[InterpMethod] = pd.Field(
+        None,
+        title="Interpolation method",
+        description="When the value is 'None', each component will follow its own "
+        "interpolation method. When the value is other than 'None', the interpolation "
+        "method specified by this field will override the one in each component.",
+    )
+
+    @pd.validator("xx", always=True)
+    def _isotropic_xx(cls, val):
+        """If it's `CustomMedium`, make sure it's isotropic."""
+        if isinstance(val, CustomMedium) and not val.is_isotropic:
+            raise SetupError("The xx-component medium type is not isotropic.")
+        return val
+
+    @pd.validator("yy", always=True)
+    def _isotropic_yy(cls, val):
+        """If it's `CustomMedium`, make sure it's isotropic."""
+        if isinstance(val, CustomMedium) and not val.is_isotropic:
+            raise SetupError("The yy-component medium type is not isotropic.")
+        return val
+
+    @pd.validator("zz", always=True)
+    def _isotropic_zz(cls, val):
+        """If it's `CustomMedium`, make sure it's isotropic."""
+        if isinstance(val, CustomMedium) and not val.is_isotropic:
+            raise SetupError("The zz-component medium type is not isotropic.")
+        return val
+
+    @cached_property
+    def n_cfl(self):
+        """This property computes the index of refraction related to CFL condition, so that
+        the FDTD with this medium is stable when the time step size that doesn't take
+        material factor into account is multiplied by ``n_cfl``.
+
+        For this medium, it takes the minimal of ``n_clf`` in all components.
+        """
+        return min((mat_component.n_cfl for mat_component in self.components.values()))
+
+    @cached_property
+    def is_isotropic(self):
+        """Whether the medium is isotropic."""
+        return False
+
+    def _interp_method(self, comp: Axis) -> InterpMethod:
+        """Interpolation method applied to comp."""
+        # override `interp_method` in components if self.interp_method is not None
+        if self.interp_method is not None:
+            return self.interp_method
+        # use component's interp_method
+        comp_map = ["xx", "yy", "zz"]
+        return self.components[comp_map[comp]].interp_method
+
+    def eps_dataarray_freq(
+        self, frequency: float
+    ) -> Tuple[SpatialDataArray, SpatialDataArray, SpatialDataArray]:
+        """Permittivity array at ``frequency``.
+
+        Parameters
+        ----------
+        frequency : float
+            Frequency to evaluate permittivity at (Hz).
+
+        Returns
+        -------
+        Tuple[:class:`.SpatialDataArray`, :class:`.SpatialDataArray`, :class:`.SpatialDataArray`]
+            The permittivity evaluated at ``frequency``.
+        """
+        return tuple(
+            mat_component.eps_dataarray_freq(frequency)[ind]
+            for ind, mat_component in enumerate(self.components.values())
+        )
+
+
+class CustomAnisotropicMediumInternal(CustomAnisotropicMedium):
+    """Diagonally anisotropic medium with spatially varying permittivity in each component.
+
+    Note
+    ----
+    Only diagonal anisotropy is currently supported.
+
+    Example
+    -------
+    >>> Nx, Ny, Nz = 10, 9, 8
+    >>> X = np.linspace(-1, 1, Nx)
+    >>> Y = np.linspace(-1, 1, Ny)
+    >>> Z = np.linspace(-1, 1, Nz)
+    >>> coords = dict(x=X, y=Y, z=Z)
+    >>> permittivity= SpatialDataArray(np.ones((Nx, Ny, Nz)), coords=coords)
+    >>> conductivity= SpatialDataArray(np.ones((Nx, Ny, Nz)), coords=coords)
+    >>> medium_xx = CustomMedium(permittivity=permittivity, conductivity=conductivity)
+    >>> medium_yy = CustomMedium(permittivity=permittivity, conductivity=conductivity)
+    >>> d_epsilon = SpatialDataArray(np.random.random((Nx, Ny, Nz)), coords=coords)
+    >>> f = SpatialDataArray(1+np.random.random((Nx, Ny, Nz)), coords=coords)
+    >>> delta = SpatialDataArray(np.random.random((Nx, Ny, Nz)), coords=coords)
+    >>> medium_zz = CustomLorentz(eps_inf=permittivity, coeffs=[(d_epsilon,f,delta),])
+    >>> anisotropic_dielectric = CustomAnisotropicMedium(xx=medium_xx, yy=medium_yy, zz=medium_zz)
+    """
+
+    xx: Union[IsotropicCustomMediumInternalType, CustomMedium] = pd.Field(
+        ...,
+        title="XX Component",
+        description="Medium describing the xx-component of the diagonal permittivity tensor.",
+        discriminator=TYPE_TAG_STR,
+    )
+
+    yy: Union[IsotropicCustomMediumInternalType, CustomMedium] = pd.Field(
+        ...,
+        title="YY Component",
+        description="Medium describing the yy-component of the diagonal permittivity tensor.",
+        discriminator=TYPE_TAG_STR,
+    )
+
+    zz: Union[IsotropicCustomMediumInternalType, CustomMedium] = pd.Field(
+        ...,
+        title="ZZ Component",
+        description="Medium describing the zz-component of the diagonal permittivity tensor.",
+        discriminator=TYPE_TAG_STR,
+    )
+
+
 # types of mediums that can be used in Simulation and Structures
 
 MediumType3D = Union[
     Medium,
-    CustomMedium,
     AnisotropicMedium,
     PECMedium,
     PoleResidue,
     Sellmeier,
     Lorentz,
     Debye,
     Drude,
     FullyAnisotropicMedium,
+    CustomMedium,
+    CustomPoleResidue,
+    CustomSellmeier,
+    CustomLorentz,
+    CustomDebye,
+    CustomDrude,
+    CustomAnisotropicMedium,
 ]
 
 
 class Medium2D(AbstractMedium):
     """2D diagonally anisotropic medium.
 
     Note
@@ -1580,38 +2745,40 @@
     Example
     -------
     >>> drude_medium = Drude(eps_inf=2.0, coeffs=[(1,2), (3,4)])
     >>> medium2d = Medium2D(ss=drude_medium, tt=drude_medium)
 
     """
 
-    ss: IsotropicMediumType = pd.Field(
+    ss: IsotropicUniformMediumType = pd.Field(
         ...,
         title="SS Component",
         description="Medium describing the ss-component of the diagonal permittivity tensor. "
         "The ss-component refers to the in-plane dimension of the medium that is the first "
         "component in order of 'x', 'y', 'z'. "
         "If the 2D material is normal to the y-axis, for example, then this determines the "
         "xx-component of the corresponding 3D medium.",
         discriminator=TYPE_TAG_STR,
     )
 
-    tt: IsotropicMediumType = pd.Field(
+    tt: IsotropicUniformMediumType = pd.Field(
         ...,
         title="TT Component",
         description="Medium describing the tt-component of the diagonal permittivity tensor. "
         "The tt-component refers to the in-plane dimension of the medium that is the second "
         "component in order of 'x', 'y', 'z'. "
         "If the 2D material is normal to the y-axis, for example, then this determines the "
         "zz-component of the corresponding 3D medium.",
         discriminator=TYPE_TAG_STR,
     )
 
     @classmethod
-    def _weighted_avg(cls, meds: List[IsotropicMediumType], weights: List[float]) -> PoleResidue:
+    def _weighted_avg(
+        cls, meds: List[IsotropicUniformMediumType], weights: List[float]
+    ) -> PoleResidue:
         """Average ``meds`` with weights ``weights``."""
         eps_inf = 1
         poles = []
         for (med, weight) in zip(meds, weights):
             if isinstance(med, DispersiveMedium):
                 pole_res = med.pole_residue
                 eps_inf += weight * (med.pole_residue.eps_inf - 1)
@@ -1655,15 +2822,15 @@
 
         Returns
         -------
         :class:`.AnisotropicMedium`
             The 3D material corresponding to this 2D material.
         """
 
-        def get_component(med: MediumType3D, comp: Axis) -> IsotropicMediumType:
+        def get_component(med: MediumType3D, comp: Axis) -> IsotropicUniformMediumType:
             """Extract the ``comp`` component of ``med``."""
             if isinstance(med, AnisotropicMedium):
                 dim = "xyz"[comp]
                 element_name = dim + dim
                 return med.elements[element_name]
             return med
 
@@ -1708,15 +2875,14 @@
 
         Returns
         -------
         :class:`.AnisotropicMedium`
             The 3D equivalent of this 2D medium.
         """
         media = list(self.elements.values())
-        print(media)
         media_weighted = [self._weighted_avg([medium], [1 / thickness]) for medium in media]
         media_3d = Geometry.unpop_axis(ax_coord=Medium(), plane_coords=media_weighted, axis=axis)
         media_3d_kwargs = {dim + dim: medium for dim, medium in zip("xyz", media_3d)}
         return AnisotropicMedium(**media_3d_kwargs, frequency_range=self.frequency_range)
 
     def to_pole_residue(self, thickness: float) -> PoleResidue:
         """Generate a :class:`.PoleResidue` equivalent of a given thickness.
@@ -1734,15 +2900,15 @@
         """
         return self._weighted_avg(
             [self.ss, self.tt], [1 / (2 * thickness), 1 / (2 * thickness)]
         ).updated_copy(frequency_range=self.frequency_range)
 
     def to_medium(self, thickness: float) -> Medium:
         """Generate a :class:`.Medium` equivalent of a given thickness.
-        The 2D medium should be isotropic in-plane (otherwise the components are averaged)
+        The 2D medium must be isotropic in-plane (otherwise the components are averaged)
         and non-dispersive besides a constant conductivity.
 
         Parameters
         ----------
         thickness: float
             The thickness of the desired 3D medium.
 
@@ -1894,15 +3060,15 @@
         -------
         complex
             Complex conductivity at this frequency.
         """
         return np.mean([self.ss.sigma_model(freq), self.tt.sigma_model(freq)], axis=0)
 
     @property
-    def elements(self) -> Dict[str, IsotropicMediumType]:
+    def elements(self) -> Dict[str, IsotropicUniformMediumType]:
         """The diagonal elements of the 2D medium as a dictionary."""
         return dict(ss=self.ss, tt=self.tt)
 
     @cached_property
     def n_cfl(self):
         """This property computes the index of refraction related to CFL condition, so that
         the FDTD with this medium is stable when the time step size that doesn't take
```

### Comparing `tidy3d-2.2.3/tidy3d/components/mode.py` & `tidy3d-2.3.0rc1/tidy3d/components/mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/components/monitor.py` & `tidy3d-2.3.0rc1/tidy3d/components/monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/components/simulation.py` & `tidy3d-2.3.0rc1/tidy3d/components/simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,29 +15,30 @@
 from .validators import assert_unique_names, assert_objects_in_sim_bounds
 from .validators import validate_mode_objects_symmetry
 from .geometry import Box, TriangleMesh, Geometry, PolySlab, Cylinder
 from .types import Ax, Shapely, FreqBound, Axis, annotate_type, Symmetry
 from .grid.grid import Coords1D, Grid, Coords
 from .grid.grid_spec import GridSpec, UniformGrid, AutoGrid
 from .medium import Medium, MediumType, AbstractMedium, PECMedium
-from .medium import CustomMedium, Medium2D, MediumType3D
+from .medium import AbstractCustomMedium, Medium2D, MediumType3D
 from .medium import AnisotropicMedium, FullyAnisotropicMedium
 from .boundary import BoundarySpec, BlochBoundary, PECBoundary, PMCBoundary, Periodic
 from .boundary import PML, StablePML, Absorber, AbsorberSpec
 from .structure import Structure
 from .source import SourceType, PlaneWave, GaussianBeam, AstigmaticGaussianBeam, CustomFieldSource
+from .source import CustomCurrentSource
 from .source import TFSF, Source
 from .monitor import MonitorType, Monitor, FreqMonitor
 from .monitor import AbstractFieldMonitor, DiffractionMonitor, AbstractFieldProjectionMonitor
 from .data.dataset import Dataset
 from .viz import add_ax_if_none, equal_aspect
 
 from .viz import MEDIUM_CMAP, STRUCTURE_EPS_CMAP, PlotParams, plot_params_symmetry, polygon_path
 from .viz import plot_params_structure, plot_params_pml, plot_params_override_structures
-from .viz import plot_params_pec, plot_params_pmc, plot_params_bloch
+from .viz import plot_params_pec, plot_params_pmc, plot_params_bloch, plot_sim_3d
 
 from ..version import __version__
 from ..constants import C_0, SECOND, inf
 from ..exceptions import Tidy3dKeyError, SetupError, ValidationError, Tidy3dError
 from ..log import log
 from ..updater import Updater
 
@@ -439,29 +440,28 @@
         if val is None:
             return val
 
         sim_box = Box(size=values.get("size"), center=values.get("center"))
         sim_bound_min, sim_bound_max = sim_box.bounds
         sim_bounds = list(sim_bound_min) + list(sim_bound_max)
 
-        for istruct, structure in enumerate(val):
-            struct_bound_min, struct_bound_max = structure.geometry.bounds
-            struct_bounds = list(struct_bound_min) + list(struct_bound_max)
-
-            for sim_val, struct_val in zip(sim_bounds, struct_bounds):
-
-                if isclose(sim_val, struct_val):
-                    log.warning(
-                        f"Structure at structures[{istruct}] has bounds that extend exactly to "
-                        "simulation edges. This can cause unexpected behavior. "
-                        "If intending to extend the structure to infinity along one dimension, "
-                        "use td.inf as a size variable instead to make this explicit. "
-                        f"Skipping check for structure indexes > {istruct}."
-                    )
-                    return val
+        with log as consolidated_logger:
+            for istruct, structure in enumerate(val):
+                struct_bound_min, struct_bound_max = structure.geometry.bounds
+                struct_bounds = list(struct_bound_min) + list(struct_bound_max)
+
+                for sim_val, struct_val in zip(sim_bounds, struct_bounds):
+
+                    if isclose(sim_val, struct_val):
+                        consolidated_logger.warning(
+                            f"Structure at structures[{istruct}] has bounds that extend exactly to "
+                            "simulation edges. This can cause unexpected behavior. "
+                            "If intending to extend the structure to infinity along one dimension, "
+                            "use td.inf as a size variable instead to make this explicit."
+                        )
 
         return val
 
     @pydantic.validator("boundary_spec", always=True)
     def _structures_not_close_pml(cls, val, values):  # pylint:disable=too-many-locals
         """Warn if any structures lie at the simulation boundaries."""
 
@@ -472,55 +472,54 @@
         structures = values.get("structures")
         sources = values.get("sources")
 
         if (not structures) or (not sources):
 
             return val
 
-        def warn(istruct, side):
-            """Warning message for a structure too close to PML."""
-            log.warning(
-                f"Structure at structures[{istruct}] was detected as being less "
-                f"than half of a central wavelength from a PML on side {side}. "
-                "To avoid inaccurate results, please increase gap between "
-                "any structures and PML or fully extend structure through the pml. "
-                f"Skipping check for structure indexes > {istruct}."
-            )
+        with log as consolidated_logger:
 
-        for istruct, structure in enumerate(structures):
-            struct_bound_min, struct_bound_max = structure.geometry.bounds
+            def warn(istruct, side):
+                """Warning message for a structure too close to PML."""
+                consolidated_logger.warning(
+                    f"Structure at structures[{istruct}] was detected as being less "
+                    f"than half of a central wavelength from a PML on side {side}. "
+                    "To avoid inaccurate results, please increase gap between "
+                    "any structures and PML or fully extend structure through the pml."
+                )
 
-            for source in sources:
-                lambda0 = C_0 / source.source_time.freq0
+            for istruct, structure in enumerate(structures):
+                struct_bound_min, struct_bound_max = structure.geometry.bounds
 
-                zipped = zip(["x", "y", "z"], sim_bound_min, struct_bound_min, boundaries)
-                for axis, sim_val, struct_val, boundary in zipped:
-                    # The test is required only for PML and stable PML
-                    if not isinstance(boundary[0], (PML, StablePML)):
-                        continue
-                    if (
-                        boundary[0].num_layers > 0
-                        and struct_val > sim_val
-                        and abs(sim_val - struct_val) < lambda0 / 2
-                    ):
-                        warn(istruct, axis + "-min")
-                        return val
+                for source in sources:
+                    lambda0 = C_0 / source.source_time.freq0
 
-                zipped = zip(["x", "y", "z"], sim_bound_max, struct_bound_max, boundaries)
-                for axis, sim_val, struct_val, boundary in zipped:
-                    # The test is required only for PML and stable PML
-                    if not isinstance(boundary[1], (PML, StablePML)):
-                        continue
-                    if (
-                        boundary[1].num_layers > 0
-                        and struct_val < sim_val
-                        and abs(sim_val - struct_val) < lambda0 / 2
-                    ):
-                        warn(istruct, axis + "-max")
-                        return val
+                    zipped = zip(["x", "y", "z"], sim_bound_min, struct_bound_min, boundaries)
+                    for axis, sim_val, struct_val, boundary in zipped:
+                        # The test is required only for PML and stable PML
+                        if not isinstance(boundary[0], (PML, StablePML)):
+                            continue
+                        if (
+                            boundary[0].num_layers > 0
+                            and struct_val > sim_val
+                            and abs(sim_val - struct_val) < lambda0 / 2
+                        ):
+                            warn(istruct, axis + "-min")
+
+                    zipped = zip(["x", "y", "z"], sim_bound_max, struct_bound_max, boundaries)
+                    for axis, sim_val, struct_val, boundary in zipped:
+                        # The test is required only for PML and stable PML
+                        if not isinstance(boundary[1], (PML, StablePML)):
+                            continue
+                        if (
+                            boundary[1].num_layers > 0
+                            and struct_val < sim_val
+                            and abs(sim_val - struct_val) < lambda0 / 2
+                        ):
+                            warn(istruct, axis + "-max")
 
         return val
 
     @pydantic.validator("monitors", always=True)
     def _warn_monitor_mediums_frequency_range(cls, val, values):
         """Warn user if any DFT monitors have frequencies outside of medium frequency range."""
 
@@ -528,39 +527,42 @@
             return val
 
         structures = values.get("structures")
         structures = structures or []
         medium_bg = values.get("medium")
         mediums = [medium_bg] + [structure.medium for structure in structures]
 
-        for monitor_index, monitor in enumerate(val):
-            if not isinstance(monitor, FreqMonitor):
-                continue
+        with log as consolidated_logger:
+            for monitor_index, monitor in enumerate(val):
+                if not isinstance(monitor, FreqMonitor):
+                    continue
 
-            freqs = np.array(monitor.freqs)
-            for medium_index, medium in enumerate(mediums):
+                freqs = np.array(monitor.freqs)
+                fmin_mon = freqs.min()
+                fmax_mon = freqs.max()
+                for medium_index, medium in enumerate(mediums):
 
-                # skip mediums that have no freq range (all freqs valid)
-                if medium.frequency_range is None:
-                    continue
+                    # skip mediums that have no freq range (all freqs valid)
+                    if medium.frequency_range is None:
+                        continue
 
-                # make sure medium frequency range includes all monitor frequencies
-                fmin_med, fmax_med = medium.frequency_range
-                if np.any(freqs < fmin_med) or np.any(freqs > fmax_med):
-                    if medium_index == 0:
-                        medium_str = "The simulation background medium"
-                    else:
-                        medium_str = f"The medium associated with structures[{medium_index-1}]"
+                    # make sure medium frequency range includes all monitor frequencies
+                    fmin_med, fmax_med = medium.frequency_range
+                    if fmin_mon < fmin_med or fmax_mon > fmax_med:
+                        if medium_index == 0:
+                            medium_str = "The simulation background medium"
+                        else:
+                            medium_str = f"The medium associated with structures[{medium_index-1}]"
 
-                    log.warning(
-                        f"{medium_str} has a frequency range: ({fmin_med:2e}, {fmax_med:2e}) "
-                        "(Hz) that does not fully cover the frequencies contained in "
-                        f"monitors[{monitor_index}]. "
-                        "This can cause inaccuracies in the recorded results."
-                    )
+                        consolidated_logger.warning(
+                            f"{medium_str} has a frequency range: ({fmin_med:2e}, {fmax_med:2e}) "
+                            "(Hz) that does not fully cover the frequencies contained in "
+                            f"monitors[{monitor_index}]. "
+                            "This can cause inaccuracies in the recorded results."
+                        )
 
         return val
 
     @pydantic.validator("monitors", always=True)
     def _warn_monitor_simulation_frequency_range(cls, val, values):
         """Warn if any DFT monitors have frequencies outside of the simulation frequency range."""
 
@@ -578,25 +580,26 @@
         if not source_ranges:
             log.warning("No sources in simulation.")
             return val
 
         freq_min = min((freq_range[0] for freq_range in source_ranges), default=0.0)
         freq_max = max((freq_range[1] for freq_range in source_ranges), default=0.0)
 
-        for monitor_index, monitor in enumerate(val):
-            if not isinstance(monitor, FreqMonitor):
-                continue
+        with log as consolidated_logger:
+            for monitor_index, monitor in enumerate(val):
+                if not isinstance(monitor, FreqMonitor):
+                    continue
 
-            freqs = np.array(monitor.freqs)
-            if np.any(freqs < freq_min) or np.any(freqs > freq_max):
-                log.warning(
-                    f"monitors[{monitor_index}] contains frequencies "
-                    f"outside of the simulation frequency range ({freq_min:2e}, {freq_max:2e})"
-                    "(Hz) as defined by the sources."
-                )
+                freqs = np.array(monitor.freqs)
+                if freqs.min() < freq_min or freqs.max() > freq_max:
+                    consolidated_logger.warning(
+                        f"monitors[{monitor_index}] contains frequencies "
+                        f"outside of the simulation frequency range ({freq_min:2e}, {freq_max:2e})"
+                        "(Hz) as defined by the sources."
+                    )
         return val
 
     @pydantic.validator("monitors", always=True)
     def diffraction_monitor_boundaries(cls, val, values):
         """If any :class:`.DiffractionMonitor` exists, ensure boundary conditions in the
         transverse directions are periodic or Bloch."""
         monitors = val
@@ -656,32 +659,34 @@
         """Warn if the projection distance is large for exact projections."""
 
         if val is None:
             return val
 
         sim_size = values.get("size")
 
-        for idx, monitor in enumerate(val):
-            if isinstance(monitor, AbstractFieldProjectionMonitor):
-                if (
-                    np.abs(monitor.proj_distance) > 1.0e4 * np.max(sim_size)
-                    and not monitor.far_field_approx
-                ):
-                    monitor = monitor.copy(update={"far_field_approx": True})
-                    val = list(val)
-                    val[idx] = monitor
-                    val = tuple(val)
-                    log.warning(
-                        "A very large projection distance was set for the field projection "
-                        f"monitor '{monitor.name}'. Using exact field projections may result in "
-                        "precision loss for large distances; automatically enabling far-field "
-                        "approximations ('far_field_approx = True') for better precision. "
-                        "To insist on exact projections, consider using client-side projections "
-                        "via the 'FieldProjector' class, where higher precision is available."
-                    )
+        with log as consolidated_logger:
+            for idx, monitor in enumerate(val):
+                if isinstance(monitor, AbstractFieldProjectionMonitor):
+                    if (
+                        np.abs(monitor.proj_distance) > 1.0e4 * np.max(sim_size)
+                        and not monitor.far_field_approx
+                    ):
+                        monitor = monitor.copy(update={"far_field_approx": True})
+                        val = list(val)
+                        val[idx] = monitor
+                        val = tuple(val)
+                        consolidated_logger.warning(
+                            "A very large projection distance was set for the field projection "
+                            f"monitor '{monitor.name}'. Using exact field projections may result "
+                            "in precision loss for large distances; automatically enabling "
+                            "far-field approximations ('far_field_approx = True') for better "
+                            "precision. To insist on exact projections, consider using client-side "
+                            "projections via the 'FieldProjector' class, where higher precision is "
+                            "available."
+                        )
         return val
 
     @pydantic.validator("monitors", always=True)
     def diffraction_monitor_medium(cls, val, values):
         """If any :class:`.DiffractionMonitor` exists, ensure is does not lie in a lossy medium."""
         monitors = val
         structures = values.get("structures")
@@ -703,47 +708,46 @@
             return val
 
         structures = values.get("structures")
         structures = structures or []
         medium_bg = values.get("medium")
         mediums = [medium_bg] + [structure.medium for structure in structures]
 
-        for source_index, source in enumerate(values.get("sources")):
-            freq0 = source.source_time.freq0
-
-            for medium_index, medium in enumerate(mediums):
+        with log as consolidated_logger:
+            for source_index, source in enumerate(values.get("sources")):
+                freq0 = source.source_time.freq0
 
-                # min wavelength in PEC is meaningless and we'll get divide by inf errors
-                if isinstance(medium, PECMedium):
-                    continue
-                # min wavelength in Medium2D is meaningless
-                if isinstance(medium, Medium2D):
-                    continue
+                for medium_index, medium in enumerate(mediums):
 
-                eps_material = medium.eps_model(freq0)
-                n_material, _ = medium.eps_complex_to_nk(eps_material)
-                lambda_min = C_0 / freq0 / n_material
+                    # min wavelength in PEC is meaningless and we'll get divide by inf errors
+                    if isinstance(medium, PECMedium):
+                        continue
+                    # min wavelength in Medium2D is meaningless
+                    if isinstance(medium, Medium2D):
+                        continue
 
-                for key, grid_spec in zip("xyz", (val.grid_x, val.grid_y, val.grid_z)):
-                    if (
-                        isinstance(grid_spec, UniformGrid)
-                        and grid_spec.dl > lambda_min / MIN_GRIDS_PER_WVL
-                    ):
-                        log.warning(
-                            f"The grid step in {key} has a value of {grid_spec.dl:.4f} (um)"
-                            ", which was detected as being large when compared to the "
-                            f"central wavelength of sources[{source_index}] "
-                            f"within the simulation medium "
-                            f"associated with structures[{medium_index + 1}], given by "
-                            f"{lambda_min:.4f} (um). "
-                            "To avoid inaccuracies, it is recommended the grid size is reduced. "
-                            f"Skipping check for structure indexes > {medium_index + 1}."
-                        )
-                        return val
-                        # TODO: warn about custom grid spec
+                    eps_material = medium.eps_model(freq0)
+                    n_material, _ = medium.eps_complex_to_nk(eps_material)
+                    lambda_min = C_0 / freq0 / n_material
+
+                    for key, grid_spec in zip("xyz", (val.grid_x, val.grid_y, val.grid_z)):
+                        if (
+                            isinstance(grid_spec, UniformGrid)
+                            and grid_spec.dl > lambda_min / MIN_GRIDS_PER_WVL
+                        ):
+                            consolidated_logger.warning(
+                                f"The grid step in {key} has a value of {grid_spec.dl:.4f} (um)"
+                                ", which was detected as being large when compared to the "
+                                f"central wavelength of sources[{source_index}] "
+                                f"within the simulation medium "
+                                f"associated with structures[{medium_index + 1}], given by "
+                                f"{lambda_min:.4f} (um). To avoid inaccuracies, "
+                                "it is recommended the grid size is reduced. "
+                            )
+                            # TODO: warn about custom grid spec
 
         return val
 
     @pydantic.validator("sources", always=True)
     def _source_homogeneous_isotropic(cls, val, values):
         """Error if a plane wave or gaussian beam source is not in a homogeneous and isotropic
         region.
@@ -818,73 +822,74 @@
     def _validate_no_structures_pml(self) -> None:
         """Ensure no structures terminate / have bounds inside of PML."""
 
         pml_thicks = np.array(self.pml_thicknesses).T
         sim_bounds = self.bounds
         bound_spec = self.boundary_spec.to_list
 
-        for i, structure in enumerate(self.structures):
-            geo_bounds = structure.geometry.bounds
-            for sim_bound, geo_bound, pml_thick, bound_dim, pm_val in zip(
-                sim_bounds, geo_bounds, pml_thicks, bound_spec, (-1, 1)
-            ):
-                for sim_pos, geo_pos, pml, bound_edge in zip(
-                    sim_bound, geo_bound, pml_thick, bound_dim
+        with log as consolidated_logger:
+            for i, structure in enumerate(self.structures):
+                geo_bounds = structure.geometry.bounds
+                for sim_bound, geo_bound, pml_thick, bound_dim, pm_val in zip(
+                    sim_bounds, geo_bounds, pml_thicks, bound_spec, (-1, 1)
                 ):
-                    sim_pos_pml = sim_pos + pm_val * pml
-                    in_pml_plus = (pm_val > 0) and (sim_pos < geo_pos <= sim_pos_pml)
-                    in_pml_mnus = (pm_val < 0) and (sim_pos > geo_pos >= sim_pos_pml)
-                    if not isinstance(bound_edge, Absorber) and (in_pml_plus or in_pml_mnus):
-                        log.warning(
-                            f"A bound of Simulation.structures[{i}] was detected as being within "
-                            "the simulation PML. We recommend extending structures to infinity or "
-                            "completely outside of the simulation PML to "
-                            "avoid unexpected effects when the structures are not translationally "
-                            "invariant within the PML. Skipping rest of structures."
-                        )
-                        return
+                    for sim_pos, geo_pos, pml, bound_edge in zip(
+                        sim_bound, geo_bound, pml_thick, bound_dim
+                    ):
+                        sim_pos_pml = sim_pos + pm_val * pml
+                        in_pml_plus = (pm_val > 0) and (sim_pos < geo_pos <= sim_pos_pml)
+                        in_pml_mnus = (pm_val < 0) and (sim_pos > geo_pos >= sim_pos_pml)
+                        if not isinstance(bound_edge, Absorber) and (in_pml_plus or in_pml_mnus):
+                            consolidated_logger.warning(
+                                f"A bound of Simulation.structures[{i}] was detected as being "
+                                "within the simulation PML. We recommend extending structures to "
+                                "infinity or completely outside of the simulation PML to avoid "
+                                "unexpected effects when the structures are not translationally "
+                                "invariant within the PML."
+                            )
 
     def _validate_tfsf_nonuniform_grid(self) -> None:
         """Warn if the grid is nonuniform along the directions tangential to the injection plane,
         inside the TFSF box.
         """
         # if the grid is uniform in all directions, there's no need to proceed
         if not (self.grid_spec.auto_grid_used or self.grid_spec.custom_grid_used):
             return
 
-        for source in self.sources:
-            if not isinstance(source, TFSF):
-                continue
-
-            centers = self.grid.centers.to_list
-            sizes = self.grid.sizes.to_list
-            tfsf_bounds = source.bounds
-            _, plane_inds = source.pop_axis([0, 1, 2], axis=source.injection_axis)
-            grid_list = [self.grid_spec.grid_x, self.grid_spec.grid_y, self.grid_spec.grid_z]
-            for ind in plane_inds:
-                grid_type = grid_list[ind]
-                if isinstance(grid_type, UniformGrid):
+        with log as consolidated_logger:
+            for source in self.sources:
+                if not isinstance(source, TFSF):
                     continue
 
-                sizes_in_tfsf = [
-                    size
-                    for size, center in zip(sizes[ind], centers[ind])
-                    if tfsf_bounds[0][ind] <= center <= tfsf_bounds[1][ind]
-                ]
+                centers = self.grid.centers.to_list
+                sizes = self.grid.sizes.to_list
+                tfsf_bounds = source.bounds
+                _, plane_inds = source.pop_axis([0, 1, 2], axis=source.injection_axis)
+                grid_list = [self.grid_spec.grid_x, self.grid_spec.grid_y, self.grid_spec.grid_z]
+                for ind in plane_inds:
+                    grid_type = grid_list[ind]
+                    if isinstance(grid_type, UniformGrid):
+                        continue
 
-                # check if all the grid sizes are sufficiently unequal
-                if not np.all(np.isclose(sizes_in_tfsf, sizes_in_tfsf[0])):
-                    log.warning(
-                        f"The grid is nonuniform along the '{'xyz'[ind]}' axis, which may lead "
-                        "to sub-optimal cancellation of the incident field in the scattered-field "
-                        "region for the total-field scattered-field (TFSF) source "
-                        f"'{source.name}'. For best results, we recommended ensuring a uniform "
-                        "grid in both directions tangential to the TFSF injection axis, "
-                        f"'{'xyz'[source.injection_axis]}'. "
-                    )
+                    sizes_in_tfsf = [
+                        size
+                        for size, center in zip(sizes[ind], centers[ind])
+                        if tfsf_bounds[0][ind] <= center <= tfsf_bounds[1][ind]
+                    ]
+
+                    # check if all the grid sizes are sufficiently unequal
+                    if not np.all(np.isclose(sizes_in_tfsf, sizes_in_tfsf[0])):
+                        consolidated_logger.warning(
+                            f"The grid is nonuniform along the '{'xyz'[ind]}' axis, which may lead "
+                            "to sub-optimal cancellation of the incident field in the "
+                            "scattered-field region for the total-field scattered-field (TFSF) "
+                            f"source '{source.name}'. For best results, we recommended ensuring a "
+                            "uniform grid in both directions tangential to the TFSF injection "
+                            f"axis, '{'xyz'[source.injection_axis]}'."
+                        )
 
     """ Pre submit validation (before web.upload()) """
 
     def validate_pre_upload(self) -> None:
         """Validate the fully initialized simulation is ok for upload to our servers."""
         self._validate_size()
         self._validate_monitor_size()
@@ -920,32 +925,33 @@
     def _validate_monitor_size(self) -> None:
         """Ensures the monitors arent storing too much data before simulation is uploaded."""
 
         tmesh = self.tmesh
         grid = self.grid
 
         total_size_gb = 0
-        for monitor in self.monitors:
-            monitor_inds = grid.discretize_inds(monitor, extend=True)
-            num_cells = [inds[1] - inds[0] for inds in monitor_inds]
-            # take monitor downsampling into account
-            if isinstance(monitor, AbstractFieldMonitor):
-                num_cells = monitor.downsampled_num_cells(num_cells)
-            num_cells = np.prod(num_cells)
-            monitor_size = monitor.storage_size(num_cells=num_cells, tmesh=tmesh)
-            monitor_size_gb = monitor_size / 2**30
-
-            if monitor_size_gb > WARN_MONITOR_DATA_SIZE_GB:
-                log.warning(
-                    f"Monitor '{monitor.name}' estimated storage is {monitor_size_gb:1.2f}GB. "
-                    "Consider making it smaller, using fewer frequencies, or spatial or temporal "
-                    "downsampling using 'interval_space' and 'interval', respectively."
-                )
+        with log as consolidated_logger:
+            for monitor in self.monitors:
+                monitor_inds = grid.discretize_inds(monitor, extend=True)
+                num_cells = [inds[1] - inds[0] for inds in monitor_inds]
+                # take monitor downsampling into account
+                if isinstance(monitor, AbstractFieldMonitor):
+                    num_cells = monitor.downsampled_num_cells(num_cells)
+                num_cells = np.prod(num_cells)
+                monitor_size = monitor.storage_size(num_cells=num_cells, tmesh=tmesh)
+                monitor_size_gb = monitor_size / 2**30
+
+                if monitor_size_gb > WARN_MONITOR_DATA_SIZE_GB:
+                    consolidated_logger.warning(
+                        f"Monitor '{monitor.name}' estimated storage is {monitor_size_gb:1.2f}GB. "
+                        "Consider making it smaller, using fewer frequencies, or spatial or "
+                        "temporal downsampling using 'interval_space' and 'interval', respectively."
+                    )
 
-            total_size_gb += monitor_size_gb
+                total_size_gb += monitor_size_gb
 
         if total_size_gb > MAX_SIMULATION_DATA_SIZE_GB:
             raise SetupError(
                 f"Simulation's monitors have {total_size_gb:.2f}GB of estimated storage, "
                 f"a maximum of {MAX_SIMULATION_DATA_SIZE_GB:.2f}GB are allowed."
             )
 
@@ -982,15 +988,15 @@
                 if surface.name[-2] != "xyz"[source.injection_axis]:
                     sidewall_surfaces.append(surface)
                     intersecting_structs = self.intersecting_structures(
                         test_object=surface, structures=self.structures
                     )
 
                     if any(
-                        isinstance(struct.medium, (CustomMedium, FullyAnisotropicMedium))
+                        isinstance(struct.medium, (AbstractCustomMedium, FullyAnisotropicMedium))
                         for struct in intersecting_structs
                     ):
                         raise SetupError(
                             f"The surfaces of TFSF source '{source.name}' must not intersect any "
                             "structures containing a 'CustomMedium' or a 'FullyAnisotropicMedium'."
                         )
 
@@ -1439,31 +1445,31 @@
         # alpha is None just means plot without any transparency
         if alpha is None:
             alpha = 1
 
         if alpha <= 0:
             return ax
 
-        if alpha < 1 and not isinstance(self.medium, CustomMedium):
+        if alpha < 1 and not isinstance(self.medium, AbstractCustomMedium):
             axis, position = Box.parse_xyz_kwargs(x=x, y=y, z=z)
             center = Box.unpop_axis(position, (0, 0), axis=axis)
             size = Box.unpop_axis(0, (inf, inf), axis=axis)
             plane = Box(center=center, size=size)
             medium_shapes = self._filter_structures_plane(structures=structures, plane=plane)
         else:
             structures = [self.background_structure] + list(structures)
             medium_shapes = self._get_structures_plane(structures=structures, x=x, y=y, z=z)
 
         eps_min, eps_max = self.eps_bounds(freq=freq)
         for (medium, shape) in medium_shapes:
             # if the background medium is custom medium, it needs to be rendered separately
-            if medium == self.medium and alpha < 1 and not isinstance(medium, CustomMedium):
+            if medium == self.medium and alpha < 1 and not isinstance(medium, AbstractCustomMedium):
                 continue
             # no need to add patches for custom medium
-            if not isinstance(medium, CustomMedium):
+            if not isinstance(medium, AbstractCustomMedium):
                 ax = self._plot_shape_structure_eps(
                     freq=freq,
                     alpha=alpha,
                     medium=medium,
                     eps_min=eps_min,
                     eps_max=eps_max,
                     reverse=reverse,
@@ -1492,25 +1498,30 @@
 
         medium_list = [self.medium] + list(self.mediums)
         medium_list = [medium for medium in medium_list if not isinstance(medium, PECMedium)]
         # regular medium
         eps_list = [
             medium.eps_model(freq).real
             for medium in medium_list
-            if not isinstance(medium, CustomMedium)
+            if not isinstance(medium, AbstractCustomMedium)
         ]
         eps_min = min(1, min(eps_list))
         eps_max = max(1, max(eps_list))
         # custom medium, the min and max in the supplied dataset over all components and
         # spatial locations.
-        for mat in [medium for medium in medium_list if isinstance(medium, CustomMedium)]:
-            eps_dataset_at_freq = mat.eps_dataset_freq(freq)
-            for eps_component in eps_dataset_at_freq.field_components.values():
-                eps_min = min(eps_min, np.min(eps_component.real.values.ravel()))
-                eps_max = max(eps_max, np.max(eps_component.real.values.ravel()))
+        for mat in [medium for medium in medium_list if isinstance(medium, AbstractCustomMedium)]:
+            eps_dataarray = mat.eps_dataarray_freq(freq)
+            eps_min = min(
+                eps_min,
+                min((np.min(eps_comp.real.values.ravel()) for eps_comp in eps_dataarray)),
+            )
+            eps_max = max(
+                eps_max,
+                max((np.max(eps_comp.real.values.ravel()) for eps_comp in eps_dataarray)),
+            )
         return eps_min, eps_max
 
     def _pcolormesh_shape_custom_medium_structure_eps(
         self,
         x: float,
         y: float,
         z: float,
@@ -2208,14 +2219,18 @@
         """
         source_ranges = [source.source_time.frequency_range() for source in self.sources]
         freq_min = min((freq_range[0] for freq_range in source_ranges), default=0.0)
         freq_max = max((freq_range[1] for freq_range in source_ranges), default=0.0)
 
         return (freq_min, freq_max)
 
+    def plot_3d(self) -> None:
+        """Render 3D plot of ``Simulation`` (in jupyter notebook only)."""
+        return plot_sim_3d(self)
+
     """ Discretization """
 
     @cached_property
     def dt(self) -> float:
         """Simulation time step (distance).
 
         Returns
@@ -2267,29 +2282,31 @@
         )
 
         # Handle 2D materials if ``AutoGrid`` is used for in-plane directions
         # must use original grid for the normal directions of all 2d materials
         grid_axes = [False, False, False]
         # must use volumetric grid for the ``AutoGrid`` in-plane directions of 2d materials
         volumetric_grid_axes = [False, False, False]
-        for structure in self.structures:
-            if isinstance(structure.medium, Medium2D):
-                normal = structure.geometry._normal_2dmaterial  # pylint:disable=protected-access
-                grid_axes[normal] = True
-                for axis, grid_axis in enumerate(
-                    [self.grid_spec.grid_x, self.grid_spec.grid_y, self.grid_spec.grid_z]
-                ):
-                    if isinstance(grid_axis, AutoGrid):
-                        if axis != normal:
-                            volumetric_grid_axes[axis] = True
-                        else:
-                            log.warning(
-                                "Using 'AutoGrid' for the normal direction of a 2D material "
-                                "may generate a grid that is not sufficiently fine."
-                            )
+        with log as consolidated_logger:
+            for structure in self.structures:
+                if isinstance(structure.medium, Medium2D):
+                    # pylint:disable=protected-access
+                    normal = structure.geometry._normal_2dmaterial
+                    grid_axes[normal] = True
+                    for axis, grid_axis in enumerate(
+                        [self.grid_spec.grid_x, self.grid_spec.grid_y, self.grid_spec.grid_z]
+                    ):
+                        if isinstance(grid_axis, AutoGrid):
+                            if axis != normal:
+                                volumetric_grid_axes[axis] = True
+                            else:
+                                consolidated_logger.warning(
+                                    "Using 'AutoGrid' for the normal direction of a 2D material "
+                                    "may generate a grid that is not sufficiently fine."
+                                )
         coords_all = [None, None, None]
         for axis in range(3):
             if grid_axes[axis] and volumetric_grid_axes[axis]:
                 raise ValidationError(
                     "Unable to generate grid. Cannot use 'AutoGrid' for "
                     "an axis that is in-plane to one 2D material and normal to another."
                 )
@@ -2577,39 +2594,40 @@
             arrays = (np.array(coords.x), np.array(coords.y), np.array(coords.z))
             eps_background = get_eps(
                 structure=self.background_structure, frequency=freq, coords=coords
             )
             shape = tuple(len(array) for array in arrays)
             eps_array = eps_background * np.ones(shape, dtype=complex)
             # replace 2d materials with volumetric equivalents
-            for structure in self.volumetric_structures:
-                # Indexing subset within the bounds of the structure
-                # pylint:disable=protected-access
-                inds = structure.geometry._inds_inside_bounds(*arrays)
-
-                # Get permittivity on meshgrid over the reduced coordinates
-                coords_reduced = tuple(arr[ind] for arr, ind in zip(arrays, inds))
-                if any(coords.size == 0 for coords in coords_reduced):
-                    continue
+            with log as consolidated_logger:
+                for structure in self.volumetric_structures:
+                    # Indexing subset within the bounds of the structure
+                    # pylint:disable=protected-access
+                    inds = structure.geometry._inds_inside_bounds(*arrays)
+
+                    # Get permittivity on meshgrid over the reduced coordinates
+                    coords_reduced = tuple(arr[ind] for arr, ind in zip(arrays, inds))
+                    if any(coords.size == 0 for coords in coords_reduced):
+                        continue
 
-                red_coords = Coords(**dict(zip("xyz", coords_reduced)))
-                eps_structure = get_eps(structure=structure, frequency=freq, coords=red_coords)
+                    red_coords = Coords(**dict(zip("xyz", coords_reduced)))
+                    eps_structure = get_eps(structure=structure, frequency=freq, coords=red_coords)
 
-                if isinstance(structure.geometry, TriangleMesh):
-                    log.warning(
-                        "Client-side permittivity of a 'TriangleMesh' may be "
-                        "inaccurate if the mesh is not unionized. We recommend unionizing "
-                        "all meshes before import. A 'PermittivityMonitor' can be used to "
-                        "obtain the true permittivity and check that the surface mesh is "
-                        "loaded correctly."
-                    )
+                    if isinstance(structure.geometry, TriangleMesh):
+                        consolidated_logger.warning(
+                            "Client-side permittivity of a 'TriangleMesh' may be "
+                            "inaccurate if the mesh is not unionized. We recommend unionizing "
+                            "all meshes before import. A 'PermittivityMonitor' can be used to "
+                            "obtain the true permittivity and check that the surface mesh is "
+                            "loaded correctly."
+                        )
 
-                # Update permittivity array at selected indexes within the geometry
-                is_inside = structure.geometry.inside_meshgrid(*coords_reduced)
-                eps_array[inds][is_inside] = (eps_structure * is_inside)[is_inside]
+                    # Update permittivity array at selected indexes within the geometry
+                    is_inside = structure.geometry.inside_meshgrid(*coords_reduced)
+                    eps_array[inds][is_inside] = (eps_structure * is_inside)[is_inside]
 
             coords = dict(zip("xyz", arrays))
             return xr.DataArray(eps_array, coords=coords, dims=("x", "y", "z"))
 
         # combine all data into dictionary
         if coord_key[0] == "E":
             # off-diagonal componets are sampled at respective locations (eg. `eps_xy` at `Ex`)
@@ -2619,24 +2637,27 @@
         return make_eps_data(coords)
 
     @property
     def custom_datasets(self) -> List[Dataset]:
         """List of custom datasets for verification purposes. If the list is not empty, then
         the simulation needs to be exported to hdf5 to store the data.
         """
-        datasets_source = [
+        datasets_field_source = [
             src.field_dataset for src in self.sources if isinstance(src, CustomFieldSource)
         ]
-        datasets_medium = [mat.eps_dataset for mat in self.mediums if isinstance(mat, CustomMedium)]
+        datasets_current_source = [
+            src.current_dataset for src in self.sources if isinstance(src, CustomCurrentSource)
+        ]
+        datasets_medium = [mat for mat in self.mediums if isinstance(mat, AbstractCustomMedium)]
         datasets_geometry = [
             struct.geometry.mesh_dataset
             for struct in self.structures
             if isinstance(struct.geometry, TriangleMesh)
         ]
-        return datasets_source + datasets_medium + datasets_geometry
+        return datasets_field_source + datasets_current_source + datasets_medium + datasets_geometry
 
     def _volumetric_structures_grid(self, grid: Grid) -> Tuple[Structure]:
         """Generate a tuple of structures wherein any 2D materials are converted to 3D
         volumetric equivalents, using ``grid`` as the simulation grid."""
 
         if not any(isinstance(medium, Medium2D) for medium in self.mediums):
             return self.structures
```

### Comparing `tidy3d-2.2.3/tidy3d/components/source.py` & `tidy3d-2.3.0rc1/tidy3d/components/source.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 from abc import ABC, abstractmethod
 from typing import Union, Tuple, Optional
 
 from typing_extensions import Literal
 import pydantic
 import numpy as np
 
-from .base import Tidy3dBaseModel, cached_property, DATA_ARRAY_MAP
+from .base import Tidy3dBaseModel, cached_property
 
 from .types import Direction, Polarization, Ax, FreqBound, ArrayFloat1D, Axis, PlotVal
 from .validators import assert_plane, assert_volumetric, validate_name_str, get_value
+from .validators import warn_if_dataset_none, assert_single_freq_in_range
 from .data.dataset import FieldDataset
 from .geometry import Box, Coordinate
 from .mode import ModeSpec
 from .viz import add_ax_if_none, PlotParams, plot_params_source
 from .viz import ARROW_COLOR_SOURCE, ARROW_ALPHA, ARROW_COLOR_POLARIZATION
 from ..constants import RADIAN, HERTZ, MICROMETER, GLANCING_CUTOFF
 from ..constants import inf  # pylint:disable=unused-import
@@ -440,14 +441,54 @@
         title="Enable Interpolation",
         description="If ``False``, the dipole is placed at the nearest Yee grid point "
         "based on the chosen ``polarization``. If ``True``, uses linear interpolation "
         "so that effectively the dipole is placed at the exact position requested.",
     )
 
 
+class CustomCurrentSource(Source):
+    """Implements a source corresponding to an input dataset containing ``E`` and ``H`` fields.
+    Injects the specified components of the ``E`` and ``H`` dataset directly as ``J`` and ``M``
+    current distributions in the FDTD solver.
+
+    Note
+    ----
+        If only the ``E`` or only the ``H`` fields are provided, the source will not be directional,
+        but will inject equal power in both directions instead.
+
+    Example
+    -------
+    >>> from tidy3d import ScalarFieldDataArray
+    >>> pulse = GaussianPulse(freq0=200e12, fwidth=20e12)
+    >>> x = np.linspace(-1, 1, 101)
+    >>> y = np.linspace(-1, 1, 101)
+    >>> z = np.array([0])
+    >>> f = [2e14]
+    >>> coords = dict(x=x, y=y, z=z, f=f)
+    >>> scalar_field = ScalarFieldDataArray(np.ones((101, 101, 1, 1)), coords=coords)
+    >>> dataset = FieldDataset(Ex=scalar_field)
+    >>> custom_source = CustomCurrentSource(
+    ...     center=(1, 1, 1),
+    ...     size=(2, 2, 0),
+    ...     source_time=pulse,
+    ...     current_dataset=dataset)
+
+    """
+
+    current_dataset: Optional[FieldDataset] = pydantic.Field(
+        ...,
+        title="Current Dataset",
+        description=":class:`.FieldDataset` containing the desired frequency-domain "
+        "electric and magnetic current patterns to inject.",
+    )
+
+    _current_dataset_none_warning = warn_if_dataset_none("current_dataset")
+    _current_dataset_single_freq = assert_single_freq_in_range("current_dataset")
+
+
 class FieldSource(Source, ABC):
     """A Source defined by the desired E and/or H fields."""
 
 
 """ Field Sources can be defined either on a (1) surface or (2) volume. Defines injection_axis """
 
 
@@ -579,44 +620,16 @@
     field_dataset: Optional[FieldDataset] = pydantic.Field(
         ...,
         title="Field Dataset",
         description=":class:`.FieldDataset` containing the desired frequency-domain "
         "fields patterns to inject. At least one tangetial field component must be specified.",
     )
 
-    @pydantic.validator("field_dataset", pre=True, always=True)
-    def _warn_if_none(cls, val: FieldDataset) -> FieldDataset:
-        """Warn if the DataArrays fail to load."""
-        if isinstance(val, dict):
-            if any((v in DATA_ARRAY_MAP for _, v in val.items() if isinstance(v, str))):
-                log.warning("Loading 'field_dataset' without data.")
-                return None
-        return val
-
-    @pydantic.validator("field_dataset", always=True)
-    def _single_frequency_in_range(cls, val: FieldDataset, values: dict) -> FieldDataset:
-        """Assert only one frequency supplied and it's in source time range."""
-        if val is None:
-            return val
-        source_time = get_value(key="source_time", values=values)
-        fmin, fmax = source_time.frequency_range()
-        for name, scalar_field in val.field_components.items():
-            freqs = scalar_field.f
-            if len(freqs) != 1:
-                raise SetupError(
-                    f"'field_dataset.{name}' must have a single frequency, "
-                    f"contains {len(freqs)} frequencies."
-                )
-            freq = float(freqs[0])
-            if (freq < fmin) or (freq > fmax):
-                raise SetupError(
-                    f"'field_dataset.{name}' contains frequency: {freq:.2e} Hz, which is outside "
-                    f"of the 'source_time' frequency range [{fmin:.2e}-{fmax:.2e}] Hz."
-                )
-        return val
+    _field_dataset_none_warning = warn_if_dataset_none("field_dataset")
+    _field_dataset_single_freq = assert_single_freq_in_range("field_dataset")
 
     @pydantic.validator("field_dataset", always=True)
     def _tangential_component_defined(cls, val: FieldDataset, values: dict) -> FieldDataset:
         """Assert that at least one tangential field component is provided."""
         if val is None:
             return val
         size = get_value(key="size", values=values)
@@ -625,29 +638,14 @@
         for field in "EH":
             for cmp_name in (cmp1, cmp2):
                 tangential_field = field + cmp_name
                 if tangential_field in val.field_components:
                     return val
         raise SetupError("No tangential field found in the suppled 'field_dataset'.")
 
-    @pydantic.validator("field_dataset", always=True)
-    def _tangential_fields_span_source(cls, val: FieldDataset, values: dict) -> FieldDataset:
-        """Assert that provided data spans source bounds in the frame with the source center as the
-        origin."""
-        if val is None:
-            return val
-        size = get_value(key="size", values=values)
-        for name, field in val.field_components.items():
-            for dim, dim_name in enumerate("xyz"):
-                in_bounds_min = np.amin(field.coords[dim_name]) <= -size[dim] / 2 + DATA_SPAN_TOL
-                in_bounds_max = np.amax(field.coords[dim_name]) >= size[dim] / 2 - DATA_SPAN_TOL
-                if not (in_bounds_min and in_bounds_max):
-                    raise SetupError(f"Data for field {name} does not span the source plane.")
-        return val
-
 
 """ Source current profiles defined by (1) angle or (2) desired mode. Sets theta and phi angles."""
 
 
 class AngledFieldSource(DirectionalSource, ABC):
     """A FieldSource defined with a an angled direction of propagation. The direction is defined by
     the polar and azimuth angles w.r.t. an injection axis, as well as forward ``+`` or
@@ -906,9 +904,10 @@
     UniformCurrentSource,
     PointDipole,
     GaussianBeam,
     AstigmaticGaussianBeam,
     ModeSource,
     PlaneWave,
     CustomFieldSource,
+    CustomCurrentSource,
     TFSF,
 ]
```

### Comparing `tidy3d-2.2.3/tidy3d/components/structure.py` & `tidy3d-2.3.0rc1/tidy3d/components/structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Defines Geometric objects with Medium properties."""
 from typing import Union, Tuple, Optional
 import pydantic
 
 from .base import Tidy3dBaseModel
 from .validators import validate_name_str
 from .geometry import GeometryType
-from .medium import MediumType, CustomMedium, Medium2D
+from .medium import MediumType, AbstractCustomMedium, Medium2D
 from .types import Ax, TYPE_TAG_STR, Axis
 from .viz import add_ax_if_none, equal_aspect
 from .grid.grid import Coords
 from ..constants import MICROMETER
 from ..exceptions import SetupError
 
 
@@ -88,15 +88,15 @@
             Frequency to evaluate permittivity at (Hz).
 
         Returns
         -------
         complex
             The diagonal elements of the relative permittivity tensor evaluated at ``frequency``.
         """
-        if isinstance(self.medium, CustomMedium):
+        if isinstance(self.medium, AbstractCustomMedium):
             return self.medium.eps_diagonal_on_grid(frequency=frequency, coords=coords)
         return self.medium.eps_diagonal(frequency=frequency)
 
     @pydantic.validator("medium", always=True)
     def _check_2d_geometry(cls, val, values):
         """Medium2D is only consistent with certain geometry types"""
         if isinstance(val, Medium2D):
@@ -122,15 +122,15 @@
             Frequency to evaluate permittivity at (Hz).
 
         Returns
         -------
         complex
            Element of the relative permittivity tensor evaluated at ``frequency``.
         """
-        if isinstance(self.medium, CustomMedium):
+        if isinstance(self.medium, AbstractCustomMedium):
             return self.medium.eps_comp_on_grid(
                 row=row, col=col, frequency=frequency, coords=coords
             )
         return self.medium.eps_comp(row=row, col=col, frequency=frequency)
 
 
 class MeshOverrideStructure(AbstractStructure):
```

### Comparing `tidy3d-2.2.3/tidy3d/components/transformation.py` & `tidy3d-2.3.0rc1/tidy3d/components/transformation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/components/types.py` & `tidy3d-2.3.0rc1/tidy3d/components/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/components/validators.py` & `tidy3d-2.3.0rc1/tidy3d/components/validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 """ Defines various validation functions that get used to ensure inputs are legit """
 from typing import Any
 
 import pydantic
 
 from .geometry import Box
 from ..exceptions import ValidationError, SetupError
+from .data.dataset import Dataset, FieldDataset
+from .base import DATA_ARRAY_MAP
+from ..log import log
 
 """ Explanation of pydantic validators:
 
     Validators are class methods that are added to the models to validate their fields (kwargs).
     The functions on this page return validators based on config arguments
     and are generally in multiple components of tidy3d.
     The inner functions (validators) are decorated with @pydantic.validator, which is configured.
@@ -195,7 +198,50 @@
         """Ensure val is not None if the symmetry is non-zero along any dimension."""
         symmetry = values.get("symmetry")
         if any(sym_val != 0 for sym_val in symmetry) and val is None:
             raise SetupError(f"'{field_name}' must be provided if symmetry present.")
         return val
 
     return _make_required
+
+
+def warn_if_dataset_none(field_name: str):
+    """Warn if a Dataset field has None in its dictionary."""
+
+    @pydantic.validator(field_name, pre=True, always=True, allow_reuse=True)
+    def _warn_if_none(cls, val: Dataset) -> Dataset:
+        """Warn if the DataArrays fail to load."""
+        if isinstance(val, dict):
+            if any((v in DATA_ARRAY_MAP for _, v in val.items() if isinstance(v, str))):
+                log.warning(f"Loading {field_name} without data.")
+                return None
+        return val
+
+    return _warn_if_none
+
+
+def assert_single_freq_in_range(field_name: str):
+    """Assert only one frequency supplied in source and it's in source time range."""
+
+    @pydantic.validator(field_name, always=True, allow_reuse=True)
+    def _single_frequency_in_range(cls, val: FieldDataset, values: dict) -> FieldDataset:
+        """Assert only one frequency supplied and it's in source time range."""
+        if val is None:
+            return val
+        source_time = get_value(key="source_time", values=values)
+        fmin, fmax = source_time.frequency_range()
+        for name, scalar_field in val.field_components.items():
+            freqs = scalar_field.f
+            if len(freqs) != 1:
+                raise SetupError(
+                    f"'{field_name}.{name}' must have a single frequency, "
+                    f"contains {len(freqs)} frequencies."
+                )
+            freq = float(freqs[0])
+            if (freq < fmin) or (freq > fmax):
+                raise SetupError(
+                    f"'{field_name}.{name}' contains frequency: {freq:.2e} Hz, which is outside "
+                    f"of the 'source_time' frequency range [{fmin:.2e}-{fmax:.2e}] Hz."
+                )
+        return val
+
+    return _single_frequency_in_range
```

### Comparing `tidy3d-2.2.3/tidy3d/components/viz.py` & `tidy3d-2.3.0rc1/tidy3d/components/viz.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # pylint: disable=invalid-name
 """ utilities for plotting """
 from __future__ import annotations
 
 from typing import Any
 from functools import wraps
+import random
+import time
 
 import matplotlib.pylab as plt
 from matplotlib.patches import PathPatch, ArrowStyle
 from matplotlib.path import Path
 from numpy import array, concatenate, ones
 import pydantic as pd
 
 from .types import Ax
 from .base import Tidy3dBaseModel
+from ..exceptions import SetupError
 
 """ Constants """
 
 # add this around extents of plots
 PLOT_BUFFER = 0.3
 
 ARROW_COLOR_MONITOR = "orange"
@@ -218,7 +221,47 @@
 
     """
     return PathPatch(polygon_path(polygon), **kwargs)
 
 
 """End descartes modification
 ================================================================================================="""
+
+
+def plot_sim_3d(sim) -> None:
+    """Make 3D display of simulation in ipyython notebook."""
+
+    try:
+        # pylint:disable=import-outside-toplevel
+        from IPython.display import display, HTML
+    except ImportError as e:
+        raise SetupError(
+            "3D plotting requires ipython to be installed "
+            "and the code to be running on a jupyter notebook."
+        ) from e
+
+    uuid = str(int(time.time() * 1000)) + str(random.randint(0, 100000))
+    # pylint:disable=protected-access
+    js_code = f"""
+    window.postMessageToViewer{uuid} = event => {{
+        if(event.data.type === 'viewer'&&event.data.uuid==='{uuid}'){{
+            document.getElementById('simulation-viewer{uuid}').contentWindow.postMessage({{ type: 'jupyter', uuid:'{uuid}', value:{sim._json_string}}}, '*')
+        }}
+    }};
+    window.addEventListener(
+        'message',
+        window.postMessageToViewer{uuid},
+        false
+    );
+    """
+    viewer_url = (
+        "https://feature-simulation-viewer.d3a9gfg7glllfq.amplifyapp.com/simulation-viewer?uuid="
+        + str(uuid)
+    )
+    html_code = f"""
+    <iframe id="simulation-viewer{uuid}" src={viewer_url} width="800" height="800"></iframe>
+    <script>
+        {js_code}
+    </script>
+    """
+
+    return display(HTML(html_code))
```

### Comparing `tidy3d-2.2.3/tidy3d/config.py` & `tidy3d-2.3.0rc1/tidy3d/config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/constants.py` & `tidy3d-2.3.0rc1/tidy3d/constants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/exceptions.py` & `tidy3d-2.3.0rc1/tidy3d/exceptions.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/material_library/material_library.py` & `tidy3d-2.3.0rc1/tidy3d/material_library/material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/material_library/material_reference.py` & `tidy3d-2.3.0rc1/tidy3d/material_library/material_reference.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/material_library/parametric_materials.py` & `tidy3d-2.3.0rc1/tidy3d/material_library/parametric_materials.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/plugins/adjoint/__init__.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/plugins/adjoint/components/base.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/plugins/adjoint/components/data/data_array.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/data/data_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,18 @@
     @pd.validator("values", always=True)
     def _convert_values_to_np(cls, val):
         """Convert supplied values to numpy if they are list (from file)."""
         if isinstance(val, list):
             return np.array(val)
         return val
 
+    def __eq__(self, other) -> bool:
+        """Check if two ``JaxDataArray`` instances are equal."""
+        return jnp.array_equal(self.values, other.values)
+
     # removed because it was slowing things down.
     # @pd.validator("coords", always=True)
     # def _coords_match_values(cls, val, values):
     #     """Make sure the coordinate dimensions and shapes match the values data."""
 
     #     values = values.get("values")
```

### Comparing `tidy3d-2.2.3/tidy3d/plugins/adjoint/components/data/dataset.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/plugins/adjoint/components/data/monitor_data.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/plugins/adjoint/components/data/sim_data.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/plugins/adjoint/components/geometry.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/plugins/adjoint/components/medium.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/medium.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Defines jax-compatible mediums."""
 from __future__ import annotations
 
-from typing import Dict, Tuple, Union, Callable
+from typing import Dict, Tuple, Union, Callable, Optional
 from abc import ABC
 
 import pydantic as pd
 import numpy as np
 import jax.numpy as jnp
 from jax.tree_util import register_pytree_node_class
 import xarray as xr
@@ -260,23 +260,53 @@
 class JaxCustomMedium(CustomMedium, AbstractJaxMedium):
     """A :class:`.CustomMedium` registered with ``jax``.
     Note: The gradient calculation assumes uniform field across the pixel.
     Therefore, the accuracy degrades as the pixel size becomes large
     with respect to the field variation.
     """
 
-    eps_dataset: JaxPermittivityDataset = pd.Field(
-        ...,
+    permittivity: Optional[JaxDataArray] = pd.Field(
+        None,
+        title="Permittivity",
+        description="Spatial profile of relative permittivity.",
+    )
+
+    conductivity: Optional[JaxDataArray] = pd.Field(
+        None,
+        title="Conductivity",
+        description="Spatial profile Electric conductivity.  Defined such "
+        "that the imaginary part of the complex permittivity at angular "
+        "frequency omega is given by conductivity/omega.",
+    )
+
+    eps_dataset: Optional[JaxPermittivityDataset] = pd.Field(
+        None,
         title="Permittivity Dataset",
         description="User-supplied dataset containing complex-valued permittivity "
         "as a function of space. Permittivity distribution over the Yee-grid will be "
         "interpolated based on the data nearest to the grid location.",
         jax_field=True,
     )
 
+    @pd.root_validator(pre=True)
+    def _pre_deprecation_dataset(cls, values):
+        """Don't allow permittivity as a field until we support it."""
+        if values.get("permittivity"):
+            raise SetupError(
+                "'permittivity' is not yet supported in adjoint plugin. "
+                "Please continue to use the 'eps_dataset' field to define the component "
+                "of the permittivity tensor."
+            )
+        return values
+
+    @pd.root_validator(pre=True)
+    def _deprecation_dataset(cls, values):
+        """Raise deprecation warning if dataset supplied and convert to dataset."""
+        return values
+
     @pd.validator("eps_dataset", always=True)
     def _is_not_3d(cls, val):
         """Ensure the custom medium pixels contain at least one dimension with only pixel thick."""
 
         for field_dim in "xyz":
             field_name = f"eps_{field_dim}{field_dim}"
             data_array = val.field_components[field_name]
@@ -306,57 +336,71 @@
                     f"is restricted to have a maximum of {MAX_NUM_CELLS_CUSTOM_MEDIUM} cells. "
                     f"Detected {num_cells_dim} grid cells in the '{field_name}' component ."
                 )
 
         return val
 
     @pd.validator("eps_dataset", always=True)
-    def _single_frequency(cls, val):
+    def _eps_dataset_single_frequency(cls, val):
         """Override of inherited validator."""
         return val
 
     @pd.validator("eps_dataset", always=True)
-    def _eps_inf_greater_no_less_than_one_sigma_positive(cls, val):
+    def _eps_dataset_eps_inf_greater_no_less_than_one_sigma_positive(cls, val):
         """Override of inherited validator."""
         return val
 
-    def eps_dataset_freq(self, frequency: float) -> PermittivityDataset:
-        """Override of inherited validator."""
+    @pd.validator("permittivity", always=True)
+    def _eps_inf_greater_no_less_than_one(cls, val):
+        """Assert any eps_inf must be >=1"""
+        return val
+
+    @pd.validator("conductivity", always=True)
+    def _conductivity_non_negative_correct_shape(cls, val, values):
+        """Assert conductivity>=0"""
+        return val
+
+    def eps_dataarray_freq(self, frequency: float):
+        """ "Permittivity array at ``frequency``"""
         as_custom_medium = self.to_medium()
-        return as_custom_medium.eps_dataset_freq(frequency=frequency)
+        return as_custom_medium.eps_dataarray_freq(frequency)
 
     def to_medium(self) -> CustomMedium:
         """Convert :class:`.JaxMedium` instance to :class:`.Medium`"""
         self_dict = self.dict(exclude={"type"})
         eps_field_components = {}
         for dim in "xyz":
             field_name = f"eps_{dim}{dim}"
             data_array = self_dict["eps_dataset"][field_name]
             values = np.array(data_array["values"])
             coords = data_array["coords"]
             scalar_field = ScalarFieldDataArray(values, coords=coords)
             eps_field_components[field_name] = scalar_field
         eps_dataset = PermittivityDataset(**eps_field_components)
         self_dict["eps_dataset"] = eps_dataset
+        self_dict["permittivity"] = None
+        self_dict["conductivity"] = None
         return CustomMedium.parse_obj(self_dict)
 
     @classmethod
     def from_tidy3d(cls, tidy3d_obj: CustomMedium) -> JaxCustomMedium:
         """Convert :class:`.Tidy3dBaseModel` instance to :class:`.JaxObject`."""
-        obj_dict = tidy3d_obj.dict(exclude={"type", "eps_dataset"})
+        obj_dict = tidy3d_obj.dict(exclude={"type", "eps_dataset", "permittivity", "conductivity"})
         eps_dataset = tidy3d_obj.eps_dataset
         field_components = {}
         for dim in "xyz":
             field_name = f"eps_{dim}{dim}"
             data_array = eps_dataset.field_components[field_name]
             values = data_array.values.tolist()
             coords = {key: np.array(val).tolist() for key, val in data_array.coords.items()}
             field_components[field_name] = JaxDataArray(values=values, coords=coords)
         eps_dataset = JaxPermittivityDataset(**field_components)
         obj_dict["eps_dataset"] = eps_dataset
+        obj_dict["permittivity"] = None
+        obj_dict["conductivity"] = None
         return cls.parse_obj(obj_dict)
 
     # pylint:disable=too-many-locals, unused-argument, too-many-arguments
     def store_vjp(
         self,
         grad_data_fwd: FieldData,
         grad_data_adj: FieldData,
```

### Comparing `tidy3d-2.2.3/tidy3d/plugins/adjoint/components/simulation.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,45 +144,39 @@
         for struct in input_structures:
             geometry = struct.geometry
             size_all_floats = all(isinstance(s, (float, int)) for s in geometry.bound_size)
             cent_all_floats = all(isinstance(c, (float, int)) for c in geometry.bound_center)
             if not (size_all_floats and cent_all_floats):
                 return val
 
-        # check intersections with other input_structures
-        for i, in_struct_i in enumerate(input_structures):
-            geometry_i = in_struct_i.geometry
-            for j in range(i + 1, len(input_structures)):
-                geometry_j = input_structures[j].geometry
-                if geometry_i.intersects(geometry_j):
-                    log.warning(
-                        f"'JaxSimulation.input_structures[{i}]' overlaps or touches "
-                        f"'JaxSimulation.input_structures[{j}]'. "
-                        "Geometric gradients for overlapping input structures may contain errors. "
-                        "Skipping the rest of the structures."
-                    )
-                    return val
+        with log as consolidated_logger:
+            # check intersections with other input_structures
+            for i, in_struct_i in enumerate(input_structures):
+                geometry_i = in_struct_i.geometry
+                for j in range(i + 1, len(input_structures)):
+                    if geometry_i.intersects(input_structures[j].geometry):
+                        consolidated_logger.warning(
+                            f"'JaxSimulation.input_structures[{i}]' overlaps or touches "
+                            f"'JaxSimulation.input_structures[{j}]'. Geometric gradients for "
+                            "overlapping input structures may contain errors."
+                        )
 
-        # check JaxPolySlab intersections with background structures
-        for i, in_struct_i in enumerate(input_structures):
-            geometry_i = in_struct_i.geometry
-            if not isinstance(geometry_i, JaxPolySlab):
-                continue
-            for j, struct_j in enumerate(structures):
-                geometry_j = struct_j.geometry
-                if geometry_i.intersects(geometry_j):
-                    log.warning(
-                        f"'JaxPolySlab'-containing 'JaxSimulation.input_structures[{i}]' "
-                        f"intersects with 'JaxSimulation.structures[{j}]'. "
-                        "Note that in this version of the adjoint plugin, there may be errors "
-                        "in the gradient when "
-                        "'JaxPolySlab' intersects with background structures. "
-                        "Skipping the rest of the structures."
-                    )
-                    return val
+            # check JaxPolySlab intersections with background structures
+            for i, in_struct_i in enumerate(input_structures):
+                geometry_i = in_struct_i.geometry
+                if not isinstance(geometry_i, JaxPolySlab):
+                    continue
+                for j, struct_j in enumerate(structures):
+                    if geometry_i.intersects(struct_j.geometry):
+                        consolidated_logger.warning(
+                            f"'JaxPolySlab'-containing 'JaxSimulation.input_structures[{i}]' "
+                            f"intersects with 'JaxSimulation.structures[{j}]'. Note that in this "
+                            "version of the adjoint plugin, there may be errors in the gradient "
+                            "when 'JaxPolySlab' intersects with background structures."
+                        )
 
         return val
 
     @staticmethod
     def get_freq_adjoint(output_monitors: List[Monitor]) -> float:
         """Return the single adjoint frequency stripped from the output monitors."""
```

### Comparing `tidy3d-2.2.3/tidy3d/plugins/adjoint/components/structure.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/structure.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/plugins/adjoint/components/types.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/plugins/adjoint/web.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/web.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import pydantic as pd
 from jax import custom_vjp
 from jax.tree_util import register_pytree_node_class
 
 from ...components.simulation import Simulation
 from ...components.data.sim_data import SimulationData
 from ...web.webapi import run as web_run
+from ...web.webapi import wait_for_connection
 from ...web.s3utils import download_file, upload_file
 from ...web.asynchronous import run_async as web_run_async
 from ...web.container import BatchData, DEFAULT_DATA_DIR, Job, Batch
 from ...components.types import Literal
 
 from .components.base import JaxObject
 from .components.simulation import JaxSimulation, JaxInfo
@@ -186,28 +187,30 @@
 
     return (sim_vjp,)
 
 
 """TO DO: IMPLEMENT this section IN WEBAPI """
 
 
+@wait_for_connection
 def upload_jax_info(jax_info: JaxInfo, task_id: str, verbose: bool) -> None:
     """Upload jax_info for a task with a given task_id."""
 
     data_file = tempfile.NamedTemporaryFile(suffix=".json")  # pylint:disable=consider-using-with
     data_file.close()
     jax_info.to_file(data_file.name)
     upload_file(
         task_id,
         data_file.name,
         JAX_INFO_FILE,
         verbose=verbose,
     )
 
 
+@wait_for_connection
 def download_sim_vjp(task_id: str, verbose: bool) -> JaxSimulation:
     """Download the vjp loaded simulation from the server to return to jax."""
 
     data_file = tempfile.NamedTemporaryFile(suffix=".hdf5")  # pylint:disable=consider-using-with
     data_file.close()
     download_file(task_id, SIM_VJP_FILE, to_file=data_file.name, verbose=verbose)
     return JaxSimulation.from_file(data_file.name)
```

### Comparing `tidy3d-2.2.3/tidy3d/plugins/dispersion/fit.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/dispersion/fit.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,327 +1,265 @@
 """Fit PoleResidue Dispersion models to optical NK data
 """
 
-from typing import Tuple, List, Optional, Union
+from typing import Tuple, List, Optional
 import csv
 import codecs
 import requests
 
 import scipy.optimize as opt
 import numpy as np
 from rich.progress import Progress
 from pydantic import Field, validator
 
 from ...log import log
-from ...components.base import Tidy3dBaseModel
+from ...components.base import Tidy3dBaseModel, cached_property
 from ...components.medium import PoleResidue, AbstractMedium
 from ...components.viz import add_ax_if_none
 from ...components.types import Ax, ArrayFloat1D
 from ...constants import C_0, HBAR, MICROMETER
 from ...exceptions import ValidationError, WebError, SetupError
 from ...web.config import DEFAULT_CONFIG as Config
 
 
 class DispersionFitter(Tidy3dBaseModel):
     """Tool for fitting refractive index data to get a
     dispersive medium described by :class:`.PoleResidue` model."""
 
-    wvl_um: Union[Tuple[float, ...], ArrayFloat1D] = Field(
+    wvl_um: ArrayFloat1D = Field(
         ...,
         title="Wavelength data",
         description="Wavelength data in micrometers.",
         units=MICROMETER,
     )
 
-    n_data: Union[Tuple[float, ...], ArrayFloat1D] = Field(
+    n_data: ArrayFloat1D = Field(
         ...,
         title="Index of refraction data",
         description="Real part of the complex index of refraction.",
     )
 
-    k_data: Union[Tuple[float, ...], ArrayFloat1D] = Field(
+    k_data: ArrayFloat1D = Field(
         None,
         title="Extinction coefficient data",
         description="Imaginary part of the complex index of refraction.",
     )
 
     wvl_range: Tuple[Optional[float], Optional[float]] = Field(
         (None, None),
         title="Wavelength range [wvl_min,wvl_max] for fitting",
-        description="Truncate the wavelength-nk data to wavelength range "
-        "[wvl_min,wvl_max] for fitting",
+        description="Truncate the wavelength, n and k data to the wavelength range '[wvl_min, "
+        "wvl_max]' for fitting.",
         units=MICROMETER,
     )
 
     @validator("wvl_um", always=True)
     def _setup_wvl(cls, val):
-        """Convert wvl_um to a numpy array"""
-        if len(val) < 1:
-            raise ValidationError("The length of data cannot be empty.")
-        return np.array(val)
+        """Convert wvl_um to a numpy array."""
+        if val.size == 0:
+            raise ValidationError("Wavelength data cannot be empty.")
+        return val
 
     @validator("n_data", always=True)
     def _ndata_length_match_wvl(cls, val, values):
         """Validate n_data"""
-        _val = np.array(val)
-        if _val.shape != values["wvl_um"].shape:
-            raise ValidationError("The length of n_data doesn't match wvl_um.")
-        return _val
+        if val.shape != values["wvl_um"].shape:
+            raise ValidationError("The length of 'n_data' doesn't match 'wvl_um'.")
+        return val
 
     @validator("k_data", always=True)
     def _kdata_setup_and_length_match(cls, val, values):
-        """
-        validate the length of k_data, or setup k if it's None
-        """
+        """Validate the length of k_data, or setup k if it's None."""
         if val is None:
             return np.zeros_like(values["wvl_um"])
-        _val = np.array(val)
-        if _val.shape != values["wvl_um"].shape:
-            raise ValidationError("The length of k_data doesn't match wvl_um.")
-        return _val
-
-    def _filter_wvl_range(
-        self, wvl_min: float = None, wvl_max: float = None
-    ) -> Tuple[Tuple[float, ...], Tuple[float, ...], Tuple[float, ...]]:
-        """
-        Filter the wavelength-nk data to wavelength range [wvl_min,wvl_max]
-        for fitting.
+        if val.shape != values["wvl_um"].shape:
+            raise ValidationError("The length of 'k_data' doesn't match 'wvl_um'.")
+        return val
 
-        Parameters
-        ----------
-        wvl_min : float, optional
-            The beginning of wavelength range. Unit: micron
-        wvl_max : float, optional
-            The end of wavelength range. Unit: micron
+    @cached_property
+    def data_in_range(self) -> Tuple[ArrayFloat1D, ArrayFloat1D, ArrayFloat1D]:
+        """Filter the wavelength-nk data to wavelength range for fitting.
 
         Returns
         -------
-        Tuple[Tuple[float, ...], Tuple[float, ...], Tuple[float, ...]]
+        Tuple[ArrayFloat1D, ArrayFloat1D, ArrayFloat1D]
             Filtered wvl_um, n_data, k_data
-
         """
 
         ind_select = np.ones(self.wvl_um.shape, dtype=bool)
-        if wvl_min is not None:
-            ind_select = np.logical_and(self.wvl_um >= wvl_min, ind_select)
+        if self.wvl_range[0] is not None:
+            ind_select = np.logical_and(self.wvl_um >= self.wvl_range[0], ind_select)
 
-        if wvl_max is not None:
-            ind_select = np.logical_and(self.wvl_um <= wvl_max, ind_select)
+        if self.wvl_range[1] is not None:
+            ind_select = np.logical_and(self.wvl_um <= self.wvl_range[1], ind_select)
 
         if not np.any(ind_select):
-            raise SetupError("No data within [wvl_min,wvl_max]")
+            raise SetupError("No data within 'wvl_range'")
 
         return self.wvl_um[ind_select], self.n_data[ind_select], self.k_data[ind_select]
 
-    @property
+    @cached_property
     def lossy(self) -> bool:
         """Find out if the medium is lossy or lossless
         based on the filtered input data.
 
         Returns
         -------
         bool
             True for lossy medium; False for lossless medium
         """
-        _, _, k_data = self._filter_wvl_range(wvl_min=self.wvl_range[0], wvl_max=self.wvl_range[1])
-        if k_data is None:
-            return False
-        if not np.any(k_data):
-            return False
-        return True
+        _, _, k_data = self.data_in_range
+        return k_data is not None and np.any(k_data)
 
     @property
     def eps_data(self) -> complex:
         """Convert filtered input n(k) data into complex permittivity.
 
         Returns
         -------
         complex
             Complex-valued relative permittivty.
         """
-        _, n_data, k_data = self._filter_wvl_range(
-            wvl_min=self.wvl_range[0], wvl_max=self.wvl_range[1]
-        )
+        _, n_data, k_data = self.data_in_range
         return AbstractMedium.nk_to_eps_complex(n=n_data, k=k_data)
 
     @property
     def freqs(self) -> Tuple[float, ...]:
         """Convert filtered input wavelength data to frequency.
 
         Returns
         -------
         Tuple[float, ...]
             Frequency array converted from filtered input wavelength data
         """
 
-        wvl_um, _, _ = self._filter_wvl_range(wvl_min=self.wvl_range[0], wvl_max=self.wvl_range[1])
+        wvl_um, _, _ = self.data_in_range
         return C_0 / wvl_um
 
     @property
     def frequency_range(self) -> Tuple[float, float]:
         """Frequency range of filtered input data
 
         Returns
         -------
         Tuple[float, float]
             The minimal frequency and the maximal frequency
         """
 
-        return (np.min(self.freqs), np.max(self.freqs))
-
-    @staticmethod
-    def _unpack_complex(complex_num):
-        """Returns real and imaginary parts from complex number.
-
-        Parameters
-        ----------
-        complex_num : complex
-            Complex number.
-
-        Returns
-        -------
-        Tuple[float, float]
-            Real and imaginary parts of the complex number.
-        """
-        return complex_num.real, complex_num.imag
-
-    @staticmethod
-    def _pack_complex(real_part, imag_part):
-        """Returns complex number from real and imaginary parts.
-
-        Parameters
-        ----------
-        real_part : float
-            Real part of the complex number.
-        imag_part : float
-            Imaginary part of the complex number.
-
-        Returns
-        -------
-        complex
-            The complex number.
-        """
-        return real_part + 1j * imag_part
+        return self.freqs.min(), self.freqs.max()
 
     @staticmethod
     def _unpack_coeffs(coeffs):
-        """Unpacks coefficient vector into complex pole parameters.
+        """Unpack coefficient vector into complex pole parameters.
 
         Parameters
         ----------
         coeffs : np.ndarray[real]
             Array of real coefficients for the pole residue fit.
 
         Returns
         -------
         Tuple[np.ndarray[complex], np.ndarray[complex]]
             "a" and "c" poles for the PoleResidue model.
         """
         assert len(coeffs) % 4 == 0, "len(coeffs) must be multiple of 4."
-        num_poles = len(coeffs) // 4
-        indices = 4 * np.arange(num_poles)
 
-        a_real = coeffs[indices + 0]
-        a_imag = coeffs[indices + 1]
-        c_real = coeffs[indices + 2]
-        c_imag = coeffs[indices + 3]
+        a_real = coeffs[0::4]
+        a_imag = coeffs[1::4]
+        c_real = coeffs[2::4]
+        c_imag = coeffs[3::4]
 
-        poles_a = DispersionFitter._pack_complex(a_real, a_imag)
-        poles_c = DispersionFitter._pack_complex(c_real, c_imag)
+        poles_a = a_real + 1j * a_imag
+        poles_c = c_real + 1j * c_imag
         return poles_a, poles_c
 
     @staticmethod
     def _pack_coeffs(pole_a, pole_c):
-        """Packs complex a and c pole parameters into coefficient array.
+        """Pack complex a and c pole parameters into coefficient array.
 
         Parameters
         ----------
         pole_a : np.ndarray[complex]
             Array of complex "a" poles for the PoleResidue dispersive model.
         pole_c : np.ndarray[complex]
             Array of complex "c" poles for the PoleResidue dispersive model.
 
         Returns
         -------
         np.ndarray[float]
             Array of real coefficients for the pole residue fit.
         """
-        a_real, a_imag = DispersionFitter._unpack_complex(pole_a)
-        c_real, c_imag = DispersionFitter._unpack_complex(pole_c)
-        stacked_coeffs = np.stack((a_real, a_imag, c_real, c_imag), axis=1)
+        stacked_coeffs = np.stack((pole_a.real, pole_a.imag, pole_c.real, pole_c.imag), axis=1)
         return stacked_coeffs.flatten()
 
     @staticmethod
     def _coeffs_to_poles(coeffs):
-        """Converts model coefficients to poles.
+        """Convert model coefficients to poles.
 
         Parameters
         ----------
         coeffs : np.ndarray[float]
             Array of real coefficients for the pole residue fit.
 
         Returns
         -------
         List[Tuple[complex, complex]]
             List of complex poles (a, c)
         """
         coeffs_scaled = coeffs / HBAR
         poles_a, poles_c = DispersionFitter._unpack_coeffs(coeffs_scaled)
-        # poles = [((a.real, a.imag), (c.real, c.imag)) for (a, c) in zip(poles_a, poles_c)]
-        return [(complex(a), complex(c)) for (a, c) in zip(poles_a, poles_c)]
+        return list(zip(poles_a, poles_c))
 
     @staticmethod
     def _poles_to_coeffs(poles):
-        """Converts poles to model coefficients.
+        """Convert poles to model coefficients.
 
         Parameters
         ----------
         poles : List[Tuple[complex, complex]]
             List of complex poles (a, c)
 
         Returns
         -------
         np.ndarray[float]
             Array of real coefficients for the pole residue fit.
         """
-        poles_a, poles_c = np.array([[a, c] for (a, c) in poles]).T
-        coeffs = DispersionFitter._pack_coeffs(poles_a, poles_c)
+        poles = np.array(poles, dtype=complex)
+        coeffs = DispersionFitter._pack_coeffs(poles[:, 0], poles[:, 1])
         return coeffs * HBAR
 
     @staticmethod
     def _eV_to_Hz(f_eV: float):  # pylint:disable=invalid-name
-        """convert frequency in unit of eV to Hz
+        """Convert frequency in unit of eV to Hz.
 
         Parameters
         ----------
         f_eV : float
             Frequency in unit of eV
         """
-
-        return f_eV / HBAR / 2 / np.pi
+        return f_eV / (HBAR * 2 * np.pi)
 
     @staticmethod
     def _Hz_to_eV(f_Hz: float):  # pylint:disable=invalid-name
-        """convert frequency in unit of Hz to eV
+        """Convert frequency in unit of Hz to eV.
 
         Parameters
         ----------
         f_Hz : float
             Frequency in unit of Hz
         """
-
         return f_Hz * HBAR * 2 * np.pi
 
     def fit(
         self,
         num_poles: int = 1,
         num_tries: int = 50,
         tolerance_rms: float = 1e-2,
     ) -> Tuple[PoleResidue, float]:
-        """Fits data a number of times and returns best results.
+        """Fit data a number of times and returns best results.
 
         Parameters
         ----------
         num_poles : int, optional
             Number of poles in the model.
         num_tries : int, optional
             Number of optimizations to run with random initial guess.
@@ -350,32 +288,38 @@
 
                 # if improvement, set the best RMS and coeffs
                 if rms_error < best_rms:
                     best_rms = rms_error
                     best_medium = medium
 
                 progress.update(
-                    task, advance=1, description=f"best RMS error so far: {best_rms:.2e}"
+                    task,
+                    advance=1,
+                    description=f"Best RMS error so far: {best_rms:.3g}",
+                    refresh=True,
                 )
 
                 # if below tolerance, return
                 if best_rms < tolerance_rms:
-                    log.info(f"\tfound optimal fit with RMS error = {best_rms:.2e}, returning")
+                    progress.update(
+                        task,
+                        completed=num_tries,
+                        description=f"Best RMS error: {best_rms:.3g}",
+                        refresh=True,
+                    )
+                    log.info("Found optimal fit with RMS error %.3g", best_rms)
                     return best_medium, best_rms
 
         # if exited loop, did not reach tolerance (warn)
-        log.warning(
-            f"\twarning: did not find fit "
-            f"with RMS error under tolerance_rms of {tolerance_rms:.2e}"
-        )
-        log.info(f"\treturning best fit with RMS error {best_rms:.2e}")
+        log.warning("Unable to fit with RMS error under 'tolerance_rms' of %.3g", tolerance_rms)
+        log.info("Returning best fit with RMS error %.3g", best_rms)
         return best_medium, best_rms
 
     def _make_medium(self, coeffs):
-        """returns medium from coeffs from optimizer
+        """Return medium from coeffs from optimizer.
 
         Parameters
         ----------
         coeffs : np.ndarray[float]
             Array of real coefficients for the pole residue fit.
 
         Returns
@@ -399,50 +343,51 @@
 
         Returns
         -------
         Tuple[:class:`.PoleResidue`, float]
             Results of single fit: (dispersive medium, RMS error).
         """
 
+        # NOTE: Not used
         def constraint(coeffs, _grad=None):
-            """Evaluates the nonlinear stability criterion of
-            Hongjin Choi, Jae-Woo Baek, and Kyung-Young Jung,
-            "Comprehensive Study on Numerical Aspects of Modified
-            Lorentz Model Based Dispersive FDTD Formulations,"
-            IEEE TAP 2019.  Note: not used.
+            """Evaluate the nonlinear stability criterion of Hongjin Choi, Jae-Woo Baek, and
+            Kyung-Young Jung, "Comprehensive Study on Numerical Aspects of Modified Lorentz Model
+            Based Dispersive FDTD Formulations," IEEE TAP 2019.
 
             Parameters
             ----------
             coeffs : np.ndarray[float]
                 Array of real coefficients for the pole residue fit.
             _grad : np.ndarray[float]
                 Gradient of ``constraint`` w.r.t coeffs, not used.
 
             Returns
             -------
             float
                 Value of constraint.
             """
             poles_a, poles_c = DispersionFitter._unpack_coeffs(coeffs)
-            a_real, a_imag = DispersionFitter._unpack_complex(poles_a)
-            c_real, c_imag = DispersionFitter._unpack_complex(poles_c)
+            a_real = poles_a.real
+            a_imag = poles_a.imag
+            c_real = poles_c.real
+            c_imag = poles_c.imag
             prstar = a_real * c_real + a_imag * c_imag
             res = 2 * prstar * a_real - c_real * (a_real * a_real + a_imag * a_imag)
             res[res >= 0] = 0
             return np.sum(res)
 
-        def obj(coeffs, _grad=None):
-            """objective function for fit
+        def objective(coeffs, _grad=None):
+            """Objective function for fit
 
             Parameters
             ----------
             coeffs : np.ndarray[float]
                 Array of real coefficients for the pole residue fit.
             _grad : np.ndarray[float]
-                Gradient of ``obj`` w.r.t coeffs, not used.
+                Gradient of ``objective`` w.r.t coeffs, not used.
 
             Returns
             -------
             float
                 RMS error correponding to current coeffs.
             """
 
@@ -455,99 +400,91 @@
         # set initial guess
         num_coeffs = num_poles * 4
         coeffs0 = 2 * (np.random.random(num_coeffs) - 0.5)
 
         # set bounds
         bounds_upper = np.zeros(num_coeffs, dtype=float)
         bounds_lower = np.zeros(num_coeffs, dtype=float)
-        indices = 4 * np.arange(num_poles)
 
         if self.lossy:
             # if lossy, the real parts can take on values
-            bounds_lower[indices] = -np.inf
-            bounds_upper[indices + 2] = np.inf
-            coeffs0[indices] = -np.abs(coeffs0[indices])
-            coeffs0[indices + 2] = +np.abs(coeffs0[indices + 2])
+            bounds_lower[0::4] = -np.inf
+            bounds_upper[2::4] = np.inf
+            coeffs0[0::4] = -np.abs(coeffs0[0::4])
+            coeffs0[2::4] = +np.abs(coeffs0[2::4])
         else:
             # otherwise, they need to be 0
-            coeffs0[indices] = 0
-            coeffs0[indices + 2] = 0
+            coeffs0[0::2] = 0
 
-        bounds_lower[indices + 1] = -np.inf
-        bounds_upper[indices + 1] = np.inf
-        bounds_lower[indices + 3] = -np.inf
-        bounds_upper[indices + 3] = np.inf
+        bounds_lower[1::2] = -np.inf
+        bounds_upper[1::2] = np.inf
 
         bounds = list(zip(bounds_lower, bounds_upper))
 
         # TODO: set up constraint properly
         scipy_constraint = opt.NonlinearConstraint(constraint, lb=0, ub=np.inf)
 
         # TODO: set options properly
         res = opt.minimize(
-            obj,
+            objective,
             coeffs0,
             args=(),
             method="SLSQP",
             bounds=bounds,
             constraints=(scipy_constraint,),
             tol=1e-7,
             callback=None,
             options=dict(maxiter=10000),
         )
 
         coeffs = res.x
-        rms_error = obj(coeffs)
+        rms_error = objective(coeffs)
 
         # set the latest fit
         medium = self._make_medium(coeffs)
         return medium, rms_error
 
     @add_ax_if_none
     def plot(
         self,
         medium: PoleResidue = None,
-        wvl_um: Tuple[float, ...] = None,
+        wvl_um: ArrayFloat1D = None,
         ax: Ax = None,
     ) -> Ax:
         """Make plot of model vs data, at a set of wavelengths (if supplied).
 
         Parameters
         ----------
         medium : :class:`.PoleResidue` = None
             medium containing model to plot against data
-        wvl_um : Tuple[float, ...] = None
+        wvl_um : ArrayFloat1D = None
             Wavelengths to evaluate model at for plot in micrometers.
         ax : matplotlib.axes._subplots.Axes = None
             Axes to plot the data on, if None, a new one is created.
 
         Returns
         -------
         matplotlib.axis.Axes
             Matplotlib axis corresponding to plot.
         """
 
-        if wvl_um is None:
-            wvl_um = C_0 / self.freqs
-
-        freqs = C_0 / wvl_um
-        eps_model = medium.eps_model(freqs)
-        n_model, k_model = AbstractMedium.eps_complex_to_nk(eps_model)
-
-        dot_sizes = 25
-        linewidth = 3
-
-        _ = ax.scatter(self.wvl_um, self.n_data, s=dot_sizes, c="black", label="n (data)")
-        ax.plot(wvl_um, n_model, linewidth=linewidth, color="crimson", label="n (model)")
-
+        ax.plot(self.wvl_um, self.n_data, "x", label="n (data)")
         if self.lossy:
-            ax.scatter(self.wvl_um, self.k_data, s=dot_sizes, c="black", label="k (data)")
-            ax.plot(wvl_um, k_model, linewidth=linewidth, color="blueviolet", label="k (model)")
+            ax.plot(self.wvl_um, self.k_data, "+", label="k (data)")
+
+        if medium:
+            if wvl_um is None:
+                wvl_um = C_0 / self.freqs
+            eps_model = medium.eps_model(C_0 / wvl_um)
+            n_model, k_model = AbstractMedium.eps_complex_to_nk(eps_model)
+            ax.plot(wvl_um, n_model, label="n (model)")
+            if self.lossy:
+                ax.plot(wvl_um, k_model, label="k (model)")
 
-        ax.set_ylabel("value")
+        ax.set_ylabel("n, k")
         ax.set_xlabel("Wavelength ($\\mu m$)")
         ax.legend()
 
         return ax
 
     @staticmethod
     def _validate_url_load(data_load: List):
```

### Comparing `tidy3d-2.2.3/tidy3d/plugins/dispersion/fit_web.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/dispersion/web.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,45 @@
-"""Fit PoleResidue Dispersion models to optical NK data based on web service
-"""
+"""Fit PoleResidue Dispersion models to optical NK data based on web service"""
+
+from __future__ import annotations
+
 import ssl
 from typing import Tuple, Optional
 from enum import Enum
 import requests
+import pydantic
 from pydantic import PositiveInt, NonNegativeFloat, PositiveFloat, Field, validator
 
 from ...log import log
 from ...components.base import Tidy3dBaseModel
 from ...components.types import Literal
 from ...components.medium import PoleResidue
 from ...constants import MICROMETER, HERTZ
 from ...exceptions import WebError, Tidy3dError, SetupError
 from ...web.httputils import get_headers
-from ...web.config import DEFAULT_CONFIG as Config
+from ...web.config import DEFAULT_CONFIG
+
 from .fit import DispersionFitter
 
 
 BOUND_MAX_FACTOR = 10
 
+URL_ENV = {
+    "local": "http://127.0.0.1:8000",
+    "dev": "https://tidy3d-service.dev-simulation.cloud",
+    "prod": "https://tidy3d-service.simulation.cloud",
+}
+
+
+class ExceptionCodes(Enum):
+    """HTTP exception codes to handle individually."""
+
+    GATEWAY_TIMEOUT = 504
+    NOT_FOUND = 404
+
 
 class AdvancedFitterParam(Tidy3dBaseModel):
     """Advanced fitter parameters"""
 
     bound_amp: NonNegativeFloat = Field(
         None,
         title="Upper bound of oscillator strength",
@@ -86,15 +103,14 @@
             raise SetupError(
                 "The upper bound 'bound_f' cannot be smaller "
                 "than the lower bound 'bound_f_lower'."
             )
         return val
 
 
-# FitterData will be used internally
 class FitterData(AdvancedFitterParam):
     """Data class for request body of Fitter where dipsersion data is input through tuple."""
 
     wvl_um: Tuple[float, ...] = Field(
         ...,
         title="Wavelengths",
         description="A set of wavelengths for dispersion data.",
@@ -132,195 +148,217 @@
     bound_f: PositiveFloat = Field(
         100.0,
         title="Upper bound of pole frequency",
         description="Upper bound of pole frequency in the model.",
         units="eV",
     )
 
-
-URL_ENV = {
-    "local": "http://127.0.0.1:8000",
-    "dev": "https://tidy3d-service.dev-simulation.cloud",
-    "prod": "https://tidy3d-service.simulation.cloud",
-}
-
-
-class ExceptionCodes(Enum):
-    """HTTP exception codes to handle individually."""
-
-    GATEWAY_TIMEOUT = 504
-    NOT_FOUND = 404
-
-
-class StableDispersionFitter(DispersionFitter):
-
-    """Stable fitter based on web service"""
-
-    @staticmethod
-    def _set_url(config_env: Literal["default", "dev", "prod", "local"] = "default"):
-        """Set the url of python web service
-
-        Parameters
-        ----------
-        config_env : Literal["default", "dev", "prod", "local"], optional
-            Service environment to pick from
-        """
-
-        _env = config_env
-        if _env == "default":
-            from ...web.config import DEFAULT_CONFIG  # pylint:disable=import-outside-toplevel
-
-            _env = "dev" if "dev" in DEFAULT_CONFIG.web_api_endpoint else "prod"
-        return URL_ENV[_env]
-
     @staticmethod
-    def _setup_server(url_server: str):
-        """set up web server access
-
-        Parameters
-        ----------
-        url_server : str
-            URL for the server
-        """
-
-        try:
-            # test connection
-            resp = requests.get(f"{url_server}/health", verify=Config.ssl_verify)
-            resp.raise_for_status()
-        except (requests.exceptions.SSLError, ssl.SSLError):
-            log.info("disable the ssl verify and retry")
-            Config.ssl_verify = False
-            resp = requests.get(f"{url_server}/health", verify=Config.ssl_verify)
-        except Exception as e:
-            raise WebError("Connection to the server failed. Please try again.") from e
-
-        return get_headers()
-
-    def _setup_webdata(
-        self,
+    def create(
+        fitter: DispersionFitter,
         num_poles: PositiveInt,
         num_tries: PositiveInt,
         tolerance_rms: NonNegativeFloat,
         advanced_param: AdvancedFitterParam,
     ) -> FitterData:
-        """Setup FitterData to be provided to webservice
+        """Setup FitterData to be provided to web service
 
         Parameters
         ----------
+        fitter : DispersionFitter
+            Fitter with the data to fit.
         num_poles : PositiveInt
             Number of poles in the model.
         num_tries : PositiveInt
             Number of optimizations to run with random initial guess.
         tolerance_rms : NonNegativeFloat
             RMS error below which the fit is successful and the result is returned.
         advanced_param : :class:`AdvancedFitterParam`
             Other advanced parameters.
 
         Returns
         -------
         :class:`FitterData`
-            Data class for request body of Fitter where dipsersion
+            Data class for request body of Fitter where dispersion
             data is input through tuple.
         """
 
         # set up bound_f, bound_amp
         if advanced_param.bound_f is None:
-            new_bound_f = advanced_param.bound_f_lower + self.frequency_range[1] * BOUND_MAX_FACTOR
+            new_bound_f = (
+                advanced_param.bound_f_lower + fitter.frequency_range[1] * BOUND_MAX_FACTOR
+            )
             advanced_param = advanced_param.copy(update={"bound_f": new_bound_f})
         if advanced_param.bound_amp is None:
-            new_bound_amp = self.frequency_range[1] * BOUND_MAX_FACTOR
+            new_bound_amp = fitter.frequency_range[1] * BOUND_MAX_FACTOR
             advanced_param = advanced_param.copy(update={"bound_amp": new_bound_amp})
 
-        wvl_um, n_data, k_data = self._filter_wvl_range(
-            wvl_min=self.wvl_range[0], wvl_max=self.wvl_range[1]
-        )
+        wvl_um, n_data, k_data = fitter.data_in_range
 
-        if self.lossy:
+        if fitter.lossy:
             k_data = k_data.tolist()
         else:
             k_data = None
 
-        web_data = FitterData(
+        # pylint: disable=protected-access
+        task = FitterData(
             wvl_um=wvl_um.tolist(),
             n_data=n_data.tolist(),
             k_data=k_data,
             num_poles=num_poles,
             num_tries=num_tries,
             tolerance_rms=tolerance_rms,
-            bound_amp=self._Hz_to_eV(advanced_param.bound_amp),
-            bound_f=self._Hz_to_eV(advanced_param.bound_f),
-            bound_f_lower=self._Hz_to_eV(advanced_param.bound_f_lower),
+            bound_amp=fitter._Hz_to_eV(advanced_param.bound_amp),
+            bound_f=fitter._Hz_to_eV(advanced_param.bound_f),
+            bound_f_lower=fitter._Hz_to_eV(advanced_param.bound_f_lower),
             bound_eps_inf=advanced_param.bound_eps_inf,
             constraint=advanced_param.constraint,
             nlopt_maxeval=advanced_param.nlopt_maxeval,
             random_seed=advanced_param.random_seed,
         )
-        return web_data
+        return task
 
-    def fit(  # pylint:disable=arguments-differ, too-many-locals
-        self,
-        num_poles: PositiveInt = 1,
-        num_tries: PositiveInt = 50,
-        tolerance_rms: NonNegativeFloat = 1e-2,
-        advanced_param: AdvancedFitterParam = AdvancedFitterParam(),
-    ) -> Tuple[PoleResidue, float]:
-        """Fits data a number of times and returns best results.
+    @staticmethod
+    def _set_url(config_env: Literal["default", "dev", "prod", "local"] = "default"):
+        """Set the url of python web service
 
         Parameters
         ----------
-        num_poles : PositiveInt, optional
-            Number of poles in the model.
-        num_tries : PositiveInt, optional
-            Number of optimizations to run with random initial guess.
-        tolerance_rms : NonNegativeFloat, optional
-            RMS error below which the fit is successful and the result is returned.
-        advanced_param : :class:`AdvancedFitterParam`, optional
-            Other advanced parameters.
+        config_env : Literal["default", "dev", "prod", "local"], optional
+            Service environment to pick from
+        """
+
+        _env = config_env
+        if _env == "default":
+            _env = "dev" if "dev" in DEFAULT_CONFIG.web_api_endpoint else "prod"
+        return URL_ENV[_env]
+
+    @staticmethod
+    def _setup_server(url_server: str):
+        """set up web server access
+
+        Parameters
+        ----------
+        url_server : str
+            URL for the server
+        """
+
+        try:
+            # test connection
+            resp = requests.get(f"{url_server}/health", verify=DEFAULT_CONFIG.ssl_verify)
+            resp.raise_for_status()
+        except (requests.exceptions.SSLError, ssl.SSLError):
+            log.info("Retrying with SSL verification disabled.")
+            DEFAULT_CONFIG.ssl_verify = False
+            resp = requests.get(f"{url_server}/health", verify=DEFAULT_CONFIG.ssl_verify)
+        except Exception as e:
+            raise WebError("Connection to the server failed. Please try again.") from e
+
+        return get_headers()
+
+    def run(self) -> Tuple[PoleResidue, float]:
+        """Execute the data fit using the stable fitter in the server.
 
         Returns
         -------
         Tuple[:class:`.PoleResidue`, float]
             Best results of multiple fits: (dispersive medium, RMS error).
         """
 
-        # get url
         url_server = self._set_url("default")
         headers = self._setup_server(url_server)
 
-        # setup web_data
-        web_data = self._setup_webdata(num_poles, num_tries, tolerance_rms, advanced_param)
-
         resp = requests.post(
             f"{url_server}/dispersion/fit",
             headers=headers,
-            data=web_data.json(),
-            verify=Config.ssl_verify,
+            data=self.json(),
+            verify=DEFAULT_CONFIG.ssl_verify,
         )
 
         try:
             resp.raise_for_status()
         except Exception as e:
             if resp.status_code == ExceptionCodes.GATEWAY_TIMEOUT.value:
-                raise Tidy3dError(
-                    "Fitter failed due to timeout. Try to decrease "
-                    "the number of tries, the number of inner iterations, "
-                    "to relax RMS tolerance, or to use the 'hard' constraint."
-                ) from e
+                msg = (
+                    (
+                        "Fitter failed due to timeout. Try to decrease the number of tries or "
+                        "inner iterations, to relax the RMS tolerance, or to use the 'hard' "
+                        "constraint."
+                    )
+                    if self.constraint != "hard"
+                    else (
+                        "Fitter failed due to timeout. Try to decrease the number of tries or "
+                        "inner iterations, or to relax the RMS tolerance."
+                    )
+                )
+                raise Tidy3dError(msg) from e
 
             raise WebError(
-                "Fitter failed. Try again, or tune the parameters, or contact us for more help."
+                "Fitter failed. Try again, tune the parameters, or contact us for more help."
             ) from e
 
         run_result = resp.json()
         best_medium = PoleResidue.parse_raw(run_result["message"])
         best_rms = float(run_result["rms"])
 
-        if best_rms < tolerance_rms:
-            log.info(f"\tfound optimal fit with RMS error = {best_rms:.2e}, returning")
+        if best_rms < self.tolerance_rms:
+            log.info("Found optimal fit with RMS error %.3g", best_rms)
         else:
             log.warning(
-                f"\twarning: did not find fit "
-                f"with RMS error under tolerance_rms of {tolerance_rms:.2e}"
+                "Unable to fit with RMS error under 'tolerance_rms' of %.3g", self.tolerance_rms
             )
-            log.info(f"\treturning best fit with RMS error {best_rms:.2e}")
+            log.info("Returning best fit with RMS error %.3g", best_rms)
 
         return best_medium, best_rms
+
+
+def run(
+    fitter: DispersionFitter,
+    num_poles: PositiveInt = 1,
+    num_tries: PositiveInt = 50,
+    tolerance_rms: NonNegativeFloat = 1e-2,
+    advanced_param: AdvancedFitterParam = AdvancedFitterParam(),
+) -> Tuple[PoleResidue, float]:
+    """Execute the data fit using the stable fitter in the server.
+
+    Parameters
+    ----------
+    fitter : DispersionFitter
+        Fitter with the data to fit.
+    num_poles : PositiveInt, optional
+        Number of poles in the model.
+    num_tries : PositiveInt, optional
+        Number of optimizations to run with random initial guess.
+    tolerance_rms : NonNegativeFloat, optional
+        RMS error below which the fit is successful and the result is returned.
+    advanced_param : :class:`AdvancedFitterParam`, optional
+        Advanced parameters passed on to the server.
+
+    Returns
+    -------
+    Tuple[:class:`.PoleResidue`, float]
+        Best results of multiple fits: (dispersive medium, RMS error).
+    """
+    task = FitterData.create(fitter, num_poles, num_tries, tolerance_rms, advanced_param)
+    return task.run()
+
+
+class StableDispersionFitter(DispersionFitter):
+    """Deprecated."""
+
+    @pydantic.root_validator()
+    def _deprecate_stable_fitter(cls, values):
+        log.warning(
+            "'StableDispersionFitter' has been deprecated. Use 'DispersionFitter' with "
+            "'tidy3d.plugins.dispersion.web.run' to access the stable fitter from the web server."
+        )
+        return values
+
+    def fit(  # pylint:disable=arguments-differ, too-many-locals
+        self,
+        num_poles: PositiveInt = 1,
+        num_tries: PositiveInt = 50,
+        tolerance_rms: NonNegativeFloat = 1e-2,
+        advanced_param: AdvancedFitterParam = AdvancedFitterParam(),
+    ) -> Tuple[PoleResidue, float]:
+        """Deprecated."""
+        return run(self, num_poles, num_tries, tolerance_rms, advanced_param)
```

### Comparing `tidy3d-2.2.3/tidy3d/plugins/mode/derivatives.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/mode/derivatives.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/plugins/mode/mode_solver.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/mode/mode_solver.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/plugins/mode/solver.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/mode/solver.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/plugins/mode/transforms.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/mode/transforms.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/plugins/polyslab/polyslab.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/polyslab/polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/plugins/resonance/resonance.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/resonance/resonance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/plugins/smatrix/smatrix.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/smatrix/smatrix.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/plugins/waveguide/rectangular_dielectric.py` & `tidy3d-2.3.0rc1/tidy3d/plugins/waveguide/rectangular_dielectric.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/updater.py` & `tidy3d-2.3.0rc1/tidy3d/updater.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/web/__init__.py` & `tidy3d-2.3.0rc1/tidy3d/web/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/web/asynchronous.py` & `tidy3d-2.3.0rc1/tidy3d/web/asynchronous.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/web/auth.py` & `tidy3d-2.3.0rc1/tidy3d/web/auth.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/web/cacert.pem` & `tidy3d-2.3.0rc1/tidy3d/web/cacert.pem`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/web/cli/app.py` & `tidy3d-2.3.0rc1/tidy3d/web/cli/app.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/web/cli/migrate.py` & `tidy3d-2.3.0rc1/tidy3d/web/cli/migrate.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/web/config.py` & `tidy3d-2.3.0rc1/tidy3d/web/config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/web/container.py` & `tidy3d-2.3.0rc1/tidy3d/web/container.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/web/environment.py` & `tidy3d-2.3.0rc1/tidy3d/web/environment.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/web/http_management.py` & `tidy3d-2.3.0rc1/tidy3d/web/http_management.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/web/httputils.py` & `tidy3d-2.3.0rc1/tidy3d/web/httputils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/web/material_fitter.py` & `tidy3d-2.3.0rc1/tidy3d/web/material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/web/material_libray.py` & `tidy3d-2.3.0rc1/tidy3d/web/material_libray.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/web/s3utils.py` & `tidy3d-2.3.0rc1/tidy3d/web/s3utils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/web/simulation_task.py` & `tidy3d-2.3.0rc1/tidy3d/web/simulation_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,16 +182,16 @@
 
     # pylint: disable=arguments-differ,too-many-arguments
     @classmethod
     def create(
         cls,
         simulation: Simulation,
         task_name: str,
-        folder_name: str = "default",
-        callback_url: str = None,
+        folder_name="default",
+        call_back_url=None,
         simulation_type: str = "tidy3d",
         parent_tasks: List[str] = None,
     ) -> SimulationTask:
         """Create a new task on the server.
 
         Parameters
         ----------
@@ -224,15 +224,15 @@
             folder = Folder.create(folder_name)
         FOLDER_CACHE[folder_name] = folder
 
         resp = http.post(
             f"tidy3d/projects/{folder.folder_id}/tasks",
             {
                 "taskName": task_name,
-                "callbackUrl": callback_url,
+                "call_back_url": call_back_url,
                 "simulationType": simulation_type,
                 "parentTasks": parent_tasks,
             },
         )
 
         return SimulationTask(**resp, simulation=simulation, folder=folder)
```

### Comparing `tidy3d-2.2.3/tidy3d/web/task.py` & `tidy3d-2.3.0rc1/tidy3d/web/task.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/web/types.py` & `tidy3d-2.3.0rc1/tidy3d/web/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.3/tidy3d/web/webapi.py` & `tidy3d-2.3.0rc1/tidy3d/web/webapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 import os
 import time
 from datetime import datetime, timedelta
 from typing import List, Dict, Callable
 from functools import wraps
 
-from requests import HTTPError
+from requests import HTTPError, ReadTimeout
 from requests.exceptions import ConnectionError as ConnErr
+from requests.exceptions import JSONDecodeError
 from urllib3.exceptions import NewConnectionError
 
 import pytz
 from rich.console import Console
 from rich.progress import Progress
 
 from .environment import Env
@@ -48,15 +49,15 @@
             """Function to return including connection waiting."""
             time_start = time.time()
             warned_previously = False
 
             while (time.time() - time_start) < wait_time_sec:
                 try:
                     return web_fn(*args, **kwargs)
-                except (ConnErr, ConnectionError, NewConnectionError):
+                except (ConnErr, ConnectionError, NewConnectionError, ReadTimeout, JSONDecodeError):
                     if not warned_previously:
                         log.warning(f"No connection: Retrying for {wait_time_sec} seconds.")
                         warned_previously = True
                     time.sleep(REFRESH_TIME)
 
             raise WebError("No internet connection: giving up on connection waiting.")
```

### Comparing `tidy3d-2.2.3/tidy3d.egg-info/PKG-INFO` & `tidy3d-2.3.0rc1/tidy3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.2.3
+Version: 2.3.0rc1
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Project-URL: Bug Tracker, https://github.com/flexcompute/tidy3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy3d-2.2.3/tidy3d.egg-info/SOURCES.txt` & `tidy3d-2.3.0rc1/tidy3d.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 tidy3d/plugins/adjoint/components/data/data_array.py
 tidy3d/plugins/adjoint/components/data/dataset.py
 tidy3d/plugins/adjoint/components/data/monitor_data.py
 tidy3d/plugins/adjoint/components/data/sim_data.py
 tidy3d/plugins/dispersion/__init__.py
 tidy3d/plugins/dispersion/fit.py
 tidy3d/plugins/dispersion/fit_web.py
+tidy3d/plugins/dispersion/web.py
 tidy3d/plugins/mode/__init__.py
 tidy3d/plugins/mode/derivatives.py
 tidy3d/plugins/mode/mode_solver.py
 tidy3d/plugins/mode/solver.py
 tidy3d/plugins/mode/transforms.py
 tidy3d/plugins/polyslab/__init__.py
 tidy3d/plugins/polyslab/polyslab.py
```

### Comparing `tidy3d-2.2.3/tidy3d.egg-info/requires.txt` & `tidy3d-2.3.0rc1/tidy3d.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 black==22.3.0
 pylint
 tox
 pytest
 pytest-timeout
 memory_profiler
 dill
+ipython
 
 [gdspy]
 gdspy
 
 [gdstk]
 gdstk
```

