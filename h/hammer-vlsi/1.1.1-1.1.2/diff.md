# Comparing `tmp/hammer_vlsi-1.1.1.tar.gz` & `tmp/hammer_vlsi-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hammer_vlsi-1.1.1.tar", max compression
+gzip compressed data, was "hammer_vlsi-1.1.2.tar", max compression
```

## Comparing `hammer_vlsi-1.1.1.tar` & `hammer_vlsi-1.1.2.tar`

### file list

```diff
@@ -1,402 +1,406 @@
--rw-r--r--   0        0        0     1568 2023-04-20 22:26:21.684385 hammer_vlsi-1.1.1/LICENSE
--rw-r--r--   0        0        0     2297 2023-04-20 22:26:21.684385 hammer_vlsi-1.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/__init__.py
--rw-r--r--   0        0        0    20617 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/cadence/__init__.py
--rw-r--r--   0        0        0      436 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/cadence/defaults.yml
--rw-r--r--   0        0        0      456 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/cadence/defaults_types.yml
--rw-r--r--   0        0        0        0 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/mentor/__init__.py
--rw-r--r--   0        0        0      571 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/mentor/defaults.yml
--rw-r--r--   0        0        0      600 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/mentor/defaults_types.yml
--rw-r--r--   0        0        0        0 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/openroad/__init__.py
--rw-r--r--   0        0        0      189 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/openroad/defaults.yml
--rw-r--r--   0        0        0      207 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/openroad/defaults_types.yml
--rw-r--r--   0        0        0     3592 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/synopsys/__init__.py
--rw-r--r--   0        0        0      494 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/synopsys/defaults.yml
--rw-r--r--   0        0        0      415 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/synopsys/defaults_types.yml
--rw-r--r--   0        0        0     3653 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/common/vivado/vivado_core.py
--rw-r--r--   0        0        0      147 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/config/__init__.py
--rw-r--r--   0        0        0      434 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/config/builtins.yml
--rw-r--r--   0        0        0       81 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/config/common.py
--rw-r--r--   0        0        0    51427 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/config/config_src.py
--rw-r--r--   0        0        0    46353 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/config/defaults.yml
--rw-r--r--   0        0        0    18317 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/config/defaults_types.yml
--rw-r--r--   0        0        0     3904 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/config/yaml2json.py
--rw-r--r--   0        0        0     1467 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/drc/icv/README.md
--rw-r--r--   0        0        0     7030 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/drc/icv/__init__.py
--rw-r--r--   0        0        0     1305 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/drc/icv/defaults.yml
--rw-r--r--   0        0        0     6551 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/drc/magic/__init__.py
--rw-r--r--   0        0        0      617 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/drc/magic/defaults.yml
--rw-r--r--   0        0        0      516 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/drc/mockdrc/__init__.py
--rw-r--r--   0        0        0      421 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/drc/nop/__init__.py
--rw-r--r--   0        0        0     4221 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/drc/openroad/__init__.py
--rw-r--r--   0        0        0      380 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/drc/openroad/defaults.yml
--rw-r--r--   0        0        0    11337 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/formal/conformal/__init__.py
--rw-r--r--   0        0        0      963 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/formal/conformal/defaults.yml
--rwxr-xr-x   0        0        0    16492 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/generate_properties.py
--rw-r--r--   0        0        0      251 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/logging/__init__.py
--rw-r--r--   0        0        0     8650 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/logging/logging.py
--rw-r--r--   0        0        0     2033 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/logging/test.py
--rw-r--r--   0        0        0     9013 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/lvs/icv/__init__.py
--rw-r--r--   0        0        0     1454 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/lvs/icv/defaults.yml
--rw-r--r--   0        0        0      600 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/lvs/mocklvs/__init__.py
--rw-r--r--   0        0        0     8263 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/lvs/netgen/__init__.py
--rw-r--r--   0        0        0      628 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/lvs/netgen/defaults.yml
--rw-r--r--   0        0        0      480 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/lvs/nop/__init__.py
--rw-r--r--   0        0        0    56234 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/par/innovus/__init__.py
--rw-r--r--   0        0        0     1681 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/par/innovus/defaults.yml
--rw-r--r--   0        0        0     2510 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/par/innovus/dump_stackup_to_json.tcl
--rw-r--r--   0        0        0     3461 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/par/mockpar/__init__.py
--rw-r--r--   0        0        0       77 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/par/mockpar/defaults.yml
--rw-r--r--   0        0        0      966 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/par/nop/__init__.py
--rw-r--r--   0        0        0     4816 2023-04-20 22:26:21.700385 hammer_vlsi-1.1.1/hammer/par/openroad/README.md
--rw-r--r--   0        0        0    85243 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/par/openroad/__init__.py
--rw-r--r--   0        0        0     4727 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/par/openroad/defaults.yml
--rw-r--r--   0        0        0     1155 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/par/openroad/defaults_types.yml
--rw-r--r--   0        0        0     1926 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/par/vivado/__init__.py
--rw-r--r--   0        0        0    13460 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/pcb/generic/__init__.py
--rw-r--r--   0        0        0      605 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/pcb/generic/defaults.yml
--rw-r--r--   0        0        0     9710 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/power/joules/__init__.py
--rw-r--r--   0        0        0      450 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/power/joules/defaults.yml
--rw-r--r--   0        0        0    41055 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/power/voltus/__init__.py
--rw-r--r--   0        0        0     1187 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/power/voltus/defaults.yml
--rw-r--r--   0        0        0        0 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/py.typed
--rw-r--r--   0        0        0     1723 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/shell/get_config.py
--rw-r--r--   0        0        0     3538 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/shell/hammer_generate_mdf.py
--rw-r--r--   0        0        0      147 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/shell/hammer_shell_test.py
--rw-r--r--   0        0        0      188 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/shell/hammer_vlsi.py
--rw-r--r--   0        0        0      691 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/shell/readlink_array.py
--rw-r--r--   0        0        0     1532 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/shell/yaml2json.py
--rw-r--r--   0        0        0     1324 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/sim/mocksim/__init__.py
--rw-r--r--   0        0        0       76 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/sim/mocksim/defaults.yml
--rw-r--r--   0        0        0    17431 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/sim/vcs/__init__.py
--rw-r--r--   0        0        0      699 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/sim/vcs/defaults.yml
--rw-r--r--   0        0        0    19752 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/sim/xcelium/__init__.py
--rw-r--r--   0        0        0     1332 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/sim/xcelium/defaults.yml
--rw-r--r--   0        0        0      804 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/sim/xcelium/defaults_types.yml
--rw-r--r--   0        0        0      701 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/sram_generator/mocksram_generator/__init__.py
--rw-r--r--   0        0        0      470 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/sram_generator/nop/__init__.py
--rw-r--r--   0        0        0    18000 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/genus/__init__.py
--rw-r--r--   0        0        0      524 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/genus/defaults.yml
--rw-r--r--   0        0        0     2352 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/mocksynth/__init__.py
--rw-r--r--   0        0        0      211 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/mocksynth/defaults.yml
--rw-r--r--   0        0        0      354 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/nop/__init__.py
--rw-r--r--   0        0        0     2467 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/__init__.py
--rw-r--r--   0        0        0      899 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/defaults.yml
--rw-r--r--   0        0        0      144 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/board.tcl
--rw-r--r--   0        0        0     1419 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/init.tcl
--rw-r--r--   0        0        0      749 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/ip.tcl
--rw-r--r--   0        0        0      360 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/mcs.tcl
--rw-r--r--   0        0        0      247 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/msg.tcl
--rw-r--r--   0        0        0     1847 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/par.tcl
--rw-r--r--   0        0        0      342 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/paths.tcl
--rw-r--r--   0        0        0      426 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/project.tcl
--rw-r--r--   0        0        0     1291 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/prologue.tcl
--rwxr-xr-x   0        0        0      226 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/run-par
--rwxr-xr-x   0        0        0      189 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/run-synthesis
--rw-r--r--   0        0        0      291 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/syn.tcl
--rw-r--r--   0        0        0       26 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/vc707.xdc
--rw-r--r--   0        0        0      183 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/vivado_setup.sh
--rw-r--r--   0        0        0    14891 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/yosys/__init__.py
--rw-r--r--   0        0        0      630 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/yosys/defaults.yml
--rw-r--r--   0        0        0      594 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/synthesis/yosys/defaults_types.yml
--rw-r--r--   0        0        0    59569 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/tech/__init__.py
--rw-r--r--   0        0        0      921 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/tech/specialcells.py
--rw-r--r--   0        0        0    18266 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/tech/stackup.py
--rw-r--r--   0        0        0     4117 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/README.md
--rw-r--r--   0        0        0    13924 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/__init__.py
--rw-r--r--   0        0        0    47808 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/asap7.tech.json
--rw-r--r--   0        0        0     1450 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/calibre.layerprops
--rw-r--r--   0        0        0     3488 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/defaults.yml
--rw-r--r--   0        0        0      155 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/defaults_types.yml
--rwxr-xr-x   0        0        0     4305 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/gds_scale.py
--rw-r--r--   0        0        0      314 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/latch_map.v
--rw-r--r--   0        0        0      657 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/lefdefLayer.map
--rwxr-xr-x   0        0        0     3622 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram-cache-gen.py
--rw-r--r--   0        0        0    54410 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram-cache.json
--rw-r--r--   0        0        0     7899 2023-04-20 22:26:21.704385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/__init__.py
--rw-r--r--   0        0        0    10084 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x16_x4.gds
--rw-r--r--   0        0        0    10784 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x17_x4.gds
--rw-r--r--   0        0        0    17108 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x32_x4.gds
--rw-r--r--   0        0        0    19564 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x37_x4.gds
--rw-r--r--   0        0        0    19916 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x38_x4.gds
--rw-r--r--   0        0        0    22376 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x44_x4.gds
--rw-r--r--   0        0        0    31156 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x64_x4.gds
--rw-r--r--   0        0        0     6580 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x8_x4.gds
--rw-r--r--   0        0        0     7806 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x12_x4.gds
--rw-r--r--   0        0        0     8510 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x14_x4.gds
--rw-r--r--   0        0        0    12022 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x22_x4.gds
--rw-r--r--   0        0        0    20098 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x40_x4.gds
--rw-r--r--   0        0        0    22558 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x46_x4.gds
--rw-r--r--   0        0        0    23610 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x48_x4.gds
--rw-r--r--   0        0        0    30634 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x64_x4.gds
--rw-r--r--   0        0        0     6054 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x8_x4.gds
--rw-r--r--   0        0        0     6756 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW2048x8_x4.gds
--rw-r--r--   0        0        0    58904 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x128_x4.gds
--rw-r--r--   0        0        0    16760 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x32_x4.gds
--rw-r--r--   0        0        0    23080 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x46_x4.gds
--rw-r--r--   0        0        0    23784 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x48_x4.gds
--rw-r--r--   0        0        0    30808 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x64_x4.gds
--rw-r--r--   0        0        0     6228 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x8_x4.gds
--rw-r--r--   0        0        0    23962 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW32x50_x4.gds
--rw-r--r--   0        0        0    10784 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW4096x16_x4.gds
--rw-r--r--   0        0        0     7280 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW4096x8_x4.gds
--rw-r--r--   0        0        0    59078 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x128_x4.gds
--rw-r--r--   0        0        0    16934 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x32_x4.gds
--rw-r--r--   0        0        0    30982 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x64_x4.gds
--rw-r--r--   0        0        0     6402 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x8_x4.gds
--rw-r--r--   0        0        0    58556 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x128_x4.gds
--rw-r--r--   0        0        0    11140 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x20_x4.gds
--rw-r--r--   0        0        0    11492 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x21_x4.gds
--rw-r--r--   0        0        0    11844 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x22_x4.gds
--rw-r--r--   0        0        0    16408 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x32_x4.gds
--rw-r--r--   0        0        0    17112 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x34_x4.gds
--rw-r--r--   0        0        0     5880 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x8_x4.gds
--rw-r--r--   0        0        0    18918 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x16_x4.gds
--rw-r--r--   0        0        0    32966 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x32_x4.gds
--rw-r--r--   0        0        0     8378 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x4_x4.gds
--rw-r--r--   0        0        0    11890 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x8_x4.gds
--rw-r--r--   0        0        0    17858 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x16_x4.gds
--rw-r--r--   0        0        0    31906 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x32_x4.gds
--rw-r--r--   0        0        0     7322 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x4_x4.gds
--rw-r--r--   0        0        0    10834 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x8_x4.gds
--rw-r--r--   0        0        0    18210 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x16_x4.gds
--rw-r--r--   0        0        0    23478 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x22_x4.gds
--rw-r--r--   0        0        0    32258 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x32_x4.gds
--rw-r--r--   0        0        0    32962 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x33_x4.gds
--rw-r--r--   0        0        0    38230 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x39_x4.gds
--rw-r--r--   0        0        0     7674 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x4_x4.gds
--rw-r--r--   0        0        0    11186 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x8_x4.gds
--rw-r--r--   0        0        0    18562 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x16_x4.gds
--rw-r--r--   0        0        0    25586 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x24_x4.gds
--rw-r--r--   0        0        0    32610 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x32_x4.gds
--rw-r--r--   0        0        0     8026 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x4_x4.gds
--rw-r--r--   0        0        0    11538 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x8_x4.gds
--rw-r--r--   0        0        0     7051 2023-04-20 22:26:21.708385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x16_x4.lef
--rw-r--r--   0        0        0     7398 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x17_x4.lef
--rw-r--r--   0        0        0    11742 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x32_x4.lef
--rw-r--r--   0        0        0    13264 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x37_x4.lef
--rw-r--r--   0        0        0    13537 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x38_x4.lef
--rw-r--r--   0        0        0    15249 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x44_x4.lef
--rw-r--r--   0        0        0    21091 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x64_x4.lef
--rw-r--r--   0        0        0     4754 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x8_x4.lef
--rw-r--r--   0        0        0     5494 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x12_x4.lef
--rw-r--r--   0        0        0     6031 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x14_x4.lef
--rw-r--r--   0        0        0     8355 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x22_x4.lef
--rw-r--r--   0        0        0    13650 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x40_x4.lef
--rw-r--r--   0        0        0    15362 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x46_x4.lef
--rw-r--r--   0        0        0    15985 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x48_x4.lef
--rw-r--r--   0        0        0    20654 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x64_x4.lef
--rw-r--r--   0        0        0     4352 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x8_x4.lef
--rw-r--r--   0        0        0     4888 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW2048x8_x4.lef
--rw-r--r--   0        0        0    39648 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x128_x4.lef
--rw-r--r--   0        0        0    11450 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x32_x4.lef
--rw-r--r--   0        0        0    15574 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x46_x4.lef
--rw-r--r--   0        0        0    16119 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x48_x4.lef
--rw-r--r--   0        0        0    20788 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x64_x4.lef
--rw-r--r--   0        0        0     4484 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x8_x4.lef
--rw-r--r--   0        0        0    16251 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW32x50_x4.lef
--rw-r--r--   0        0        0     7417 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW4096x16_x4.lef
--rw-r--r--   0        0        0     5107 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW4096x8_x4.lef
--rw-r--r--   0        0        0    39781 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x128_x4.lef
--rw-r--r--   0        0        0    11583 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x32_x4.lef
--rw-r--r--   0        0        0    20958 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x64_x4.lef
--rw-r--r--   0        0        0     4611 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x8_x4.lef
--rw-r--r--   0        0        0    39308 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x128_x4.lef
--rw-r--r--   0        0        0     7675 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x20_x4.lef
--rw-r--r--   0        0        0     7946 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x21_x4.lef
--rw-r--r--   0        0        0     8218 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x22_x4.lef
--rw-r--r--   0        0        0    11176 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x32_x4.lef
--rw-r--r--   0        0        0    11716 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x34_x4.lef
--rw-r--r--   0        0        0     4218 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x8_x4.lef
--rw-r--r--   0        0        0    12982 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x16_x4.lef
--rw-r--r--   0        0        0    22452 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x32_x4.lef
--rw-r--r--   0        0        0     5940 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x4_x4.lef
--rw-r--r--   0        0        0     8262 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x8_x4.lef
--rw-r--r--   0        0        0    12165 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x16_x4.lef
--rw-r--r--   0        0        0    21631 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x32_x4.lef
--rw-r--r--   0        0        0     5123 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x4_x4.lef
--rw-r--r--   0        0        0     7446 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x8_x4.lef
--rw-r--r--   0        0        0    12437 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x16_x4.lef
--rw-r--r--   0        0        0    15987 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x22_x4.lef
--rw-r--r--   0        0        0    21899 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x32_x4.lef
--rw-r--r--   0        0        0    22455 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x33_x4.lef
--rw-r--r--   0        0        0    26004 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x39_x4.lef
--rw-r--r--   0        0        0     5403 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x4_x4.lef
--rw-r--r--   0        0        0     7718 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x8_x4.lef
--rw-r--r--   0        0        0    12708 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x16_x4.lef
--rw-r--r--   0        0        0    17441 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x24_x4.lef
--rw-r--r--   0        0        0    22174 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x32_x4.lef
--rw-r--r--   0        0        0     5670 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x4_x4.lef
--rw-r--r--   0        0        0     7988 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x8_x4.lef
--rw-r--r--   0        0        0    15410 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x16_lib/SRAM1RW1024x16_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15276 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x16_lib/SRAM1RW1024x16_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15410 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x17_lib/SRAM1RW1024x17_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15276 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x17_lib/SRAM1RW1024x17_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15410 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x32_lib/SRAM1RW1024x32_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15276 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x32_lib/SRAM1RW1024x32_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15410 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x37_lib/SRAM1RW1024x37_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15276 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x37_lib/SRAM1RW1024x37_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15410 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x38_lib/SRAM1RW1024x38_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15276 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x38_lib/SRAM1RW1024x38_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15410 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x44_lib/SRAM1RW1024x44_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15276 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x44_lib/SRAM1RW1024x44_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15410 2023-04-20 22:26:21.712386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x64_lib/SRAM1RW1024x64_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15276 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x64_lib/SRAM1RW1024x64_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15401 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x8_lib/SRAM1RW1024x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15267 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x8_lib/SRAM1RW1024x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15373 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x12_lib/SRAM1RW128x12_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15195 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x12_lib/SRAM1RW128x12_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15373 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x14_lib/SRAM1RW128x14_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15195 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x14_lib/SRAM1RW128x14_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15373 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x22_lib/SRAM1RW128x22_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15195 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x22_lib/SRAM1RW128x22_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15373 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x40_lib/SRAM1RW128x40_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15195 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x40_lib/SRAM1RW128x40_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15373 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x46_lib/SRAM1RW128x46_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15195 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x46_lib/SRAM1RW128x46_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15373 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x48_lib/SRAM1RW128x48_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15195 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x48_lib/SRAM1RW128x48_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15373 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x64_lib/SRAM1RW128x64_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15195 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x64_lib/SRAM1RW128x64_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15364 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x8_lib/SRAM1RW128x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15186 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x8_lib/SRAM1RW128x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15435 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW2048x8_lib/SRAM1RW2048x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15305 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW2048x8_lib/SRAM1RW2048x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15394 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x128_lib/SRAM1RW256x128_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15242 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x128_lib/SRAM1RW256x128_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15385 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x32_lib/SRAM1RW256x32_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15233 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x32_lib/SRAM1RW256x32_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15385 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x46_lib/SRAM1RW256x46_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15233 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x46_lib/SRAM1RW256x46_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15385 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x48_lib/SRAM1RW256x48_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15233 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x48_lib/SRAM1RW256x48_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15385 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x64_lib/SRAM1RW256x64_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15233 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x64_lib/SRAM1RW256x64_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15198 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x8_lib/SRAM1RW256x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15046 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x8_lib/SRAM1RW256x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15345 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW32x50_lib/SRAM1RW32x50_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15211 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW32x50_lib/SRAM1RW32x50_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15504 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x16_lib/SRAM1RW4096x16_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15294 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x16_lib/SRAM1RW4096x16_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15495 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x8_lib/SRAM1RW4096x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15285 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x8_lib/SRAM1RW4096x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15372 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x128_lib/SRAM1RW512x128_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15276 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x128_lib/SRAM1RW512x128_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15363 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x32_lib/SRAM1RW512x32_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15267 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x32_lib/SRAM1RW512x32_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15363 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x64_lib/SRAM1RW512x64_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15267 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x64_lib/SRAM1RW512x64_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15354 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x8_lib/SRAM1RW512x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15258 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x8_lib/SRAM1RW512x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15386 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x128_lib/SRAM1RW64x128_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15224 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x128_lib/SRAM1RW64x128_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15377 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x20_lib/SRAM1RW64x20_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15215 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x20_lib/SRAM1RW64x20_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15377 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x21_lib/SRAM1RW64x21_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15215 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x21_lib/SRAM1RW64x21_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15377 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x22_lib/SRAM1RW64x22_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15215 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x22_lib/SRAM1RW64x22_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15377 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x32_lib/SRAM1RW64x32_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15215 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x32_lib/SRAM1RW64x32_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15377 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x34_lib/SRAM1RW64x34_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15215 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x34_lib/SRAM1RW64x34_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    15368 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x8_lib/SRAM1RW64x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    15206 2023-04-20 22:26:21.716385 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x8_lib/SRAM1RW64x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28859 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x16_lib/SRAM2RW128x16_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28513 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x16_lib/SRAM2RW128x16_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28859 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x32_lib/SRAM2RW128x32_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28513 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x32_lib/SRAM2RW128x32_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28846 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x4_lib/SRAM2RW128x4_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28500 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x4_lib/SRAM2RW128x4_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28846 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x8_lib/SRAM2RW128x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28500 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x8_lib/SRAM2RW128x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28793 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x16_lib/SRAM2RW16x16_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28447 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x16_lib/SRAM2RW16x16_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28793 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x32_lib/SRAM2RW16x32_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28447 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x32_lib/SRAM2RW16x32_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28602 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x4_lib/SRAM2RW16x4_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28256 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x4_lib/SRAM2RW16x4_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28780 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x8_lib/SRAM2RW16x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28434 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x8_lib/SRAM2RW16x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28805 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x16_lib/SRAM2RW32x16_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28547 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x16_lib/SRAM2RW32x16_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28805 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x22_lib/SRAM2RW32x22_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28547 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x22_lib/SRAM2RW32x22_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28805 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x32_lib/SRAM2RW32x32_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28547 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x32_lib/SRAM2RW32x32_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28805 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x33_lib/SRAM2RW32x33_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28547 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x33_lib/SRAM2RW32x33_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28805 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x39_lib/SRAM2RW32x39_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28547 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x39_lib/SRAM2RW32x39_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28792 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x4_lib/SRAM2RW32x4_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28534 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x4_lib/SRAM2RW32x4_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28792 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x8_lib/SRAM2RW32x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28534 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x8_lib/SRAM2RW32x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28869 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x16_lib/SRAM2RW64x16_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28555 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x16_lib/SRAM2RW64x16_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28869 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x24_lib/SRAM2RW64x24_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28555 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x24_lib/SRAM2RW64x24_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28869 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x32_lib/SRAM2RW64x32_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28555 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x32_lib/SRAM2RW64x32_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28856 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x4_lib/SRAM2RW64x4_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28542 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x4_lib/SRAM2RW64x4_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0    28856 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x8_lib/SRAM2RW64x8_PVT_0P63V_100C.lib
--rw-r--r--   0        0        0    28542 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x8_lib/SRAM2RW64x8_PVT_0P77V_0C.lib
--rw-r--r--   0        0        0      773 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/asap7/srams.txt
--rw-r--r--   0        0        0      576 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/nangate45/README.md
--rw-r--r--   0        0        0      365 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/nangate45/__init__.py
--rw-r--r--   0        0        0      952 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/nangate45/defaults.yml
--rw-r--r--   0        0        0     5912 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/nangate45/nangate45.tech.json
--rw-r--r--   0        0        0     1554 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/nangate45/sram-cache.json
--rw-r--r--   0        0        0     2835 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/nangate45/sram_compiler/__init__.py
--rw-r--r--   0        0        0      116 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/nop/__init__.py
--rw-r--r--   0        0        0       33 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/nop/defaults.yml
--rw-r--r--   0        0        0       82 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/nop/nop.tech.json
--rw-r--r--   0        0        0     6649 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/sky130/README.md
--rw-r--r--   0        0        0    14127 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/sky130/__init__.py
--rw-r--r--   0        0        0     5035 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/sky130/defaults.yml
--rw-r--r--   0        0        0      711 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/sky130/defaults_types.yml
--rw-r--r--   0        0        0      899 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/cells-gen.py
--rw-r--r--   0        0        0    11554 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/cells.txt
--rw-r--r--   0        0        0     2907 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/fill.json
--rwxr-xr-x   0        0        0     3552 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/openram/sram-cache-gen.py
--rw-r--r--   0        0        0     5531 2023-04-20 22:26:21.720386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/openram/sram-cache.json
--rw-r--r--   0        0        0      172 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/openram/srams.txt
--rw-r--r--   0        0        0      785 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/setRC.tcl
--rw-r--r--   0        0        0      421 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen-files/beginning.json
--rw-r--r--   0        0        0     1005 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen-files/beginning_nda.json
--rw-r--r--   0        0        0     1597 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen-files/cells.json
--rw-r--r--   0        0        0      114 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen-files/sites.json
--rwxr-xr-x   0        0        0     3221 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen-files/stackups-gen.py
--rw-r--r--   0        0        0     2274 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen-files/stackups.json
--rwxr-xr-x   0        0        0     3259 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen.py
--rw-r--r--   0        0        0     2478 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130_lefpin.map
--rwxr-xr-x   0        0        0     3010 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sram22/sram-cache-gen.py
--rw-r--r--   0        0        0     6699 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sram22/sram-cache.json
--rw-r--r--   0        0        0      320 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sram22/srams.txt
--rw-r--r--   0        0        0    16216 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/sky130.tech.json
--rw-r--r--   0        0        0     6699 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/sram-cache.json
--rw-r--r--   0        0        0    10942 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/sky130/sram_compiler/__init__.py
--rw-r--r--   0        0        0      330 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/vivado/vivado.plsi_config.json
--rw-r--r--   0        0        0      456 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/technology/vivado/vivado.tech.json
--rw-r--r--   0        0        0    12224 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/timing/tempus/__init__.py
--rw-r--r--   0        0        0      605 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/timing/tempus/defaults.yml
--rw-r--r--   0        0        0    14969 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/utils/__init__.py
--rw-r--r--   0        0        0     3300 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/utils/lef_utils.py
--rw-r--r--   0        0        0     1844 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/utils/verilog_utils.py
--rw-r--r--   0        0        0      398 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/__init__.py
--rw-r--r--   0        0        0    92096 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/cli_driver.py
--rw-r--r--   0        0        0    34891 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/constraints.py
--rw-r--r--   0        0        0    84324 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/driver.py
--rw-r--r--   0        0        0    29715 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/hammer_build_systems.py
--rw-r--r--   0        0        0    75866 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/hammer_tool.py
--rw-r--r--   0        0        0    99097 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/hammer_vlsi_impl.py
--rw-r--r--   0        0        0     1655 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/hooks.py
--rw-r--r--   0        0        0    10265 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/submit_command.py
--rw-r--r--   0        0        0    10163 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/units.py
--rw-r--r--   0        0        0       61 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/vendor/__init__.py
--rw-r--r--   0        0        0     6349 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/vendor/def2stream.py
--rw-r--r--   0        0        0    12189 2023-04-20 22:26:21.724386 hammer_vlsi-1.1.1/hammer/vlsi/vendor/openroad.py
--rw-r--r--   0        0        0     2343 2023-04-20 22:27:13.501184 hammer_vlsi-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    10009 1970-01-01 00:00:00.000000 hammer_vlsi-1.1.1/setup.py
--rw-r--r--   0        0        0     3326 1970-01-01 00:00:00.000000 hammer_vlsi-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1568 2023-06-15 16:29:20.222906 hammer_vlsi-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2297 2023-06-15 16:29:20.222906 hammer_vlsi-1.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/common/__init__.py
+-rw-r--r--   0        0        0    20617 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/common/cadence/__init__.py
+-rw-r--r--   0        0        0      436 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/common/cadence/defaults.yml
+-rw-r--r--   0        0        0      456 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/common/cadence/defaults_types.yml
+-rw-r--r--   0        0        0        0 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/common/mentor/__init__.py
+-rw-r--r--   0        0        0      571 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/common/mentor/defaults.yml
+-rw-r--r--   0        0        0      600 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/common/mentor/defaults_types.yml
+-rw-r--r--   0        0        0        0 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/common/openroad/__init__.py
+-rw-r--r--   0        0        0      189 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/common/openroad/defaults.yml
+-rw-r--r--   0        0        0      207 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/common/openroad/defaults_types.yml
+-rw-r--r--   0        0        0     3592 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/common/synopsys/__init__.py
+-rw-r--r--   0        0        0      494 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/common/synopsys/defaults.yml
+-rw-r--r--   0        0        0      415 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/common/synopsys/defaults_types.yml
+-rw-r--r--   0        0        0     3653 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/common/vivado/vivado_core.py
+-rw-r--r--   0        0        0      147 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/config/__init__.py
+-rw-r--r--   0        0        0      434 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/config/builtins.yml
+-rw-r--r--   0        0        0       81 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/config/common.py
+-rw-r--r--   0        0        0    56272 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/config/config_src.py
+-rw-r--r--   0        0        0    46435 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/config/defaults.yml
+-rw-r--r--   0        0        0    18232 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/config/defaults_types.yml
+-rw-r--r--   0        0        0     3904 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/config/yaml2json.py
+-rw-r--r--   0        0        0     1467 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/drc/icv/README.md
+-rw-r--r--   0        0        0     7030 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/drc/icv/__init__.py
+-rw-r--r--   0        0        0     1305 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/drc/icv/defaults.yml
+-rw-r--r--   0        0        0     4332 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/drc/klayout/__init__.py
+-rw-r--r--   0        0        0      215 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/drc/klayout/default_types.yml
+-rw-r--r--   0        0        0      565 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/drc/klayout/defaults.yml
+-rw-r--r--   0        0        0     6551 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/drc/magic/__init__.py
+-rw-r--r--   0        0        0      617 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/drc/magic/defaults.yml
+-rw-r--r--   0        0        0      516 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/drc/mockdrc/__init__.py
+-rw-r--r--   0        0        0      421 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/drc/nop/__init__.py
+-rw-r--r--   0        0        0     4221 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/drc/openroad/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/drc/openroad/defaults.yml
+-rw-r--r--   0        0        0    11337 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/formal/conformal/__init__.py
+-rw-r--r--   0        0        0      963 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/formal/conformal/defaults.yml
+-rwxr-xr-x   0        0        0    16304 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/generate_properties.py
+-rw-r--r--   0        0        0      251 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/logging/__init__.py
+-rw-r--r--   0        0        0     8650 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/logging/logging.py
+-rw-r--r--   0        0        0     2033 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/logging/test.py
+-rw-r--r--   0        0        0     9025 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/lvs/icv/__init__.py
+-rw-r--r--   0        0        0     1454 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/lvs/icv/defaults.yml
+-rw-r--r--   0        0        0     1119 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/lvs/mocklvs/__init__.py
+-rw-r--r--   0        0        0     8275 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/lvs/netgen/__init__.py
+-rw-r--r--   0        0        0      628 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/lvs/netgen/defaults.yml
+-rw-r--r--   0        0        0      480 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/lvs/nop/__init__.py
+-rw-r--r--   0        0        0    57824 2023-06-15 16:29:20.238907 hammer_vlsi-1.1.2/hammer/par/innovus/__init__.py
+-rw-r--r--   0        0        0     1681 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/par/innovus/defaults.yml
+-rw-r--r--   0        0        0     2510 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/par/innovus/dump_stackup_to_json.tcl
+-rw-r--r--   0        0        0     4310 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/par/mockpar/__init__.py
+-rw-r--r--   0        0        0       77 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/par/mockpar/defaults.yml
+-rw-r--r--   0        0        0      966 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/par/nop/__init__.py
+-rw-r--r--   0        0        0     4816 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/par/openroad/README.md
+-rw-r--r--   0        0        0    85923 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/par/openroad/__init__.py
+-rw-r--r--   0        0        0     4727 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/par/openroad/defaults.yml
+-rw-r--r--   0        0        0     1155 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/par/openroad/defaults_types.yml
+-rw-r--r--   0        0        0     1926 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/par/vivado/__init__.py
+-rw-r--r--   0        0        0    13460 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/pcb/generic/__init__.py
+-rw-r--r--   0        0        0      605 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/pcb/generic/defaults.yml
+-rw-r--r--   0        0        0     9710 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/power/joules/__init__.py
+-rw-r--r--   0        0        0      450 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/power/joules/defaults.yml
+-rw-r--r--   0        0        0    41055 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/power/voltus/__init__.py
+-rw-r--r--   0        0        0     1187 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/power/voltus/defaults.yml
+-rw-r--r--   0        0        0        0 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/py.typed
+-rw-r--r--   0        0        0     1723 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/shell/get_config.py
+-rw-r--r--   0        0        0     3538 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/shell/hammer_generate_mdf.py
+-rw-r--r--   0        0        0      147 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/shell/hammer_shell_test.py
+-rw-r--r--   0        0        0      188 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/shell/hammer_vlsi.py
+-rw-r--r--   0        0        0      691 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/shell/readlink_array.py
+-rw-r--r--   0        0        0     1532 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/shell/yaml2json.py
+-rw-r--r--   0        0        0     1324 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/sim/mocksim/__init__.py
+-rw-r--r--   0        0        0       76 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/sim/mocksim/defaults.yml
+-rw-r--r--   0        0        0    17431 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/sim/vcs/__init__.py
+-rw-r--r--   0        0        0      699 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/sim/vcs/defaults.yml
+-rw-r--r--   0        0        0    19752 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/sim/xcelium/__init__.py
+-rw-r--r--   0        0        0     1332 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/sim/xcelium/defaults.yml
+-rw-r--r--   0        0        0      804 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/sim/xcelium/defaults_types.yml
+-rw-r--r--   0        0        0      701 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/sram_generator/mocksram_generator/__init__.py
+-rw-r--r--   0        0        0      470 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/sram_generator/nop/__init__.py
+-rw-r--r--   0        0        0    18454 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/genus/__init__.py
+-rw-r--r--   0        0        0      524 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/genus/defaults.yml
+-rw-r--r--   0        0        0     2352 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/mocksynth/__init__.py
+-rw-r--r--   0        0        0      211 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/mocksynth/defaults.yml
+-rw-r--r--   0        0        0      354 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/nop/__init__.py
+-rw-r--r--   0        0        0     2467 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/vivado/__init__.py
+-rw-r--r--   0        0        0      899 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/vivado/defaults.yml
+-rw-r--r--   0        0        0      144 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/vivado/file_templates/board.tcl
+-rw-r--r--   0        0        0     1419 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/vivado/file_templates/init.tcl
+-rw-r--r--   0        0        0      749 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/vivado/file_templates/ip.tcl
+-rw-r--r--   0        0        0      360 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/vivado/file_templates/mcs.tcl
+-rw-r--r--   0        0        0      247 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/vivado/file_templates/msg.tcl
+-rw-r--r--   0        0        0     1847 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/vivado/file_templates/par.tcl
+-rw-r--r--   0        0        0      342 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/vivado/file_templates/paths.tcl
+-rw-r--r--   0        0        0      426 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/vivado/file_templates/project.tcl
+-rw-r--r--   0        0        0     1291 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/vivado/file_templates/prologue.tcl
+-rwxr-xr-x   0        0        0      226 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/vivado/file_templates/run-par
+-rwxr-xr-x   0        0        0      189 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/vivado/file_templates/run-synthesis
+-rw-r--r--   0        0        0      291 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/vivado/file_templates/syn.tcl
+-rw-r--r--   0        0        0       26 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/vivado/file_templates/vc707.xdc
+-rw-r--r--   0        0        0      183 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/vivado/file_templates/vivado_setup.sh
+-rw-r--r--   0        0        0    14891 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/yosys/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/yosys/defaults.yml
+-rw-r--r--   0        0        0      594 2023-06-15 16:29:20.242908 hammer_vlsi-1.1.2/hammer/synthesis/yosys/defaults_types.yml
+-rw-r--r--   0        0        0    59569 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/tech/__init__.py
+-rw-r--r--   0        0        0      921 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/tech/specialcells.py
+-rw-r--r--   0        0        0    18447 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/tech/stackup.py
+-rw-r--r--   0        0        0     4117 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/README.md
+-rw-r--r--   0        0        0    13840 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/__init__.py
+-rw-r--r--   0        0        0    47808 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/asap7.tech.json
+-rw-r--r--   0        0        0     1450 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/calibre.layerprops
+-rw-r--r--   0        0        0     3401 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/defaults.yml
+-rw-r--r--   0        0        0      155 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/defaults_types.yml
+-rwxr-xr-x   0        0        0     4305 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/gds_scale.py
+-rw-r--r--   0        0        0      314 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/latch_map.v
+-rw-r--r--   0        0        0      657 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/lefdefLayer.map
+-rwxr-xr-x   0        0        0     3622 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram-cache-gen.py
+-rw-r--r--   0        0        0    54410 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram-cache.json
+-rw-r--r--   0        0        0     7899 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/__init__.py
+-rw-r--r--   0        0        0    10084 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x16_x4.gds
+-rw-r--r--   0        0        0    10784 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x17_x4.gds
+-rw-r--r--   0        0        0    17108 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x32_x4.gds
+-rw-r--r--   0        0        0    19564 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x37_x4.gds
+-rw-r--r--   0        0        0    19916 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x38_x4.gds
+-rw-r--r--   0        0        0    22376 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x44_x4.gds
+-rw-r--r--   0        0        0    31156 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x64_x4.gds
+-rw-r--r--   0        0        0     6580 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x8_x4.gds
+-rw-r--r--   0        0        0     7806 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x12_x4.gds
+-rw-r--r--   0        0        0     8510 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x14_x4.gds
+-rw-r--r--   0        0        0    12022 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x22_x4.gds
+-rw-r--r--   0        0        0    20098 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x40_x4.gds
+-rw-r--r--   0        0        0    22558 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x46_x4.gds
+-rw-r--r--   0        0        0    23610 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x48_x4.gds
+-rw-r--r--   0        0        0    30634 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x64_x4.gds
+-rw-r--r--   0        0        0     6054 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x8_x4.gds
+-rw-r--r--   0        0        0     6756 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW2048x8_x4.gds
+-rw-r--r--   0        0        0    58904 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x128_x4.gds
+-rw-r--r--   0        0        0    16760 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x32_x4.gds
+-rw-r--r--   0        0        0    23080 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x46_x4.gds
+-rw-r--r--   0        0        0    23784 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x48_x4.gds
+-rw-r--r--   0        0        0    30808 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x64_x4.gds
+-rw-r--r--   0        0        0     6228 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x8_x4.gds
+-rw-r--r--   0        0        0    23962 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW32x50_x4.gds
+-rw-r--r--   0        0        0    10784 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW4096x16_x4.gds
+-rw-r--r--   0        0        0     7280 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW4096x8_x4.gds
+-rw-r--r--   0        0        0    59078 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x128_x4.gds
+-rw-r--r--   0        0        0    16934 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x32_x4.gds
+-rw-r--r--   0        0        0    30982 2023-06-15 16:29:20.246908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x64_x4.gds
+-rw-r--r--   0        0        0     6402 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x8_x4.gds
+-rw-r--r--   0        0        0    58556 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x128_x4.gds
+-rw-r--r--   0        0        0    11140 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x20_x4.gds
+-rw-r--r--   0        0        0    11492 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x21_x4.gds
+-rw-r--r--   0        0        0    11844 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x22_x4.gds
+-rw-r--r--   0        0        0    16408 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x32_x4.gds
+-rw-r--r--   0        0        0    17112 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x34_x4.gds
+-rw-r--r--   0        0        0     5880 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x8_x4.gds
+-rw-r--r--   0        0        0    18918 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x16_x4.gds
+-rw-r--r--   0        0        0    32966 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x32_x4.gds
+-rw-r--r--   0        0        0     8378 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x4_x4.gds
+-rw-r--r--   0        0        0    11890 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x8_x4.gds
+-rw-r--r--   0        0        0    17858 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x16_x4.gds
+-rw-r--r--   0        0        0    31906 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x32_x4.gds
+-rw-r--r--   0        0        0     7322 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x4_x4.gds
+-rw-r--r--   0        0        0    10834 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x8_x4.gds
+-rw-r--r--   0        0        0    18210 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x16_x4.gds
+-rw-r--r--   0        0        0    23478 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x22_x4.gds
+-rw-r--r--   0        0        0    32258 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x32_x4.gds
+-rw-r--r--   0        0        0    32962 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x33_x4.gds
+-rw-r--r--   0        0        0    38230 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x39_x4.gds
+-rw-r--r--   0        0        0     7674 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x4_x4.gds
+-rw-r--r--   0        0        0    11186 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x8_x4.gds
+-rw-r--r--   0        0        0    18562 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x16_x4.gds
+-rw-r--r--   0        0        0    25586 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x24_x4.gds
+-rw-r--r--   0        0        0    32610 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x32_x4.gds
+-rw-r--r--   0        0        0     8026 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x4_x4.gds
+-rw-r--r--   0        0        0    11538 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x8_x4.gds
+-rw-r--r--   0        0        0     7051 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x16_x4.lef
+-rw-r--r--   0        0        0     7398 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x17_x4.lef
+-rw-r--r--   0        0        0    11742 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x32_x4.lef
+-rw-r--r--   0        0        0    13264 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x37_x4.lef
+-rw-r--r--   0        0        0    13537 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x38_x4.lef
+-rw-r--r--   0        0        0    15249 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x44_x4.lef
+-rw-r--r--   0        0        0    21091 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x64_x4.lef
+-rw-r--r--   0        0        0     4754 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x8_x4.lef
+-rw-r--r--   0        0        0     5494 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x12_x4.lef
+-rw-r--r--   0        0        0     6031 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x14_x4.lef
+-rw-r--r--   0        0        0     8355 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x22_x4.lef
+-rw-r--r--   0        0        0    13650 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x40_x4.lef
+-rw-r--r--   0        0        0    15362 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x46_x4.lef
+-rw-r--r--   0        0        0    15985 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x48_x4.lef
+-rw-r--r--   0        0        0    20654 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x64_x4.lef
+-rw-r--r--   0        0        0     4352 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x8_x4.lef
+-rw-r--r--   0        0        0     4888 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW2048x8_x4.lef
+-rw-r--r--   0        0        0    39648 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x128_x4.lef
+-rw-r--r--   0        0        0    11450 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x32_x4.lef
+-rw-r--r--   0        0        0    15574 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x46_x4.lef
+-rw-r--r--   0        0        0    16119 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x48_x4.lef
+-rw-r--r--   0        0        0    20788 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x64_x4.lef
+-rw-r--r--   0        0        0     4484 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x8_x4.lef
+-rw-r--r--   0        0        0    16251 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW32x50_x4.lef
+-rw-r--r--   0        0        0     7417 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW4096x16_x4.lef
+-rw-r--r--   0        0        0     5107 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW4096x8_x4.lef
+-rw-r--r--   0        0        0    39781 2023-06-15 16:29:20.250908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x128_x4.lef
+-rw-r--r--   0        0        0    11583 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x32_x4.lef
+-rw-r--r--   0        0        0    20958 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x64_x4.lef
+-rw-r--r--   0        0        0     4611 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x8_x4.lef
+-rw-r--r--   0        0        0    39308 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x128_x4.lef
+-rw-r--r--   0        0        0     7675 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x20_x4.lef
+-rw-r--r--   0        0        0     7946 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x21_x4.lef
+-rw-r--r--   0        0        0     8218 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x22_x4.lef
+-rw-r--r--   0        0        0    11176 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x32_x4.lef
+-rw-r--r--   0        0        0    11716 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x34_x4.lef
+-rw-r--r--   0        0        0     4218 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x8_x4.lef
+-rw-r--r--   0        0        0    12982 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x16_x4.lef
+-rw-r--r--   0        0        0    22452 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x32_x4.lef
+-rw-r--r--   0        0        0     5940 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x4_x4.lef
+-rw-r--r--   0        0        0     8262 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x8_x4.lef
+-rw-r--r--   0        0        0    12165 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x16_x4.lef
+-rw-r--r--   0        0        0    21631 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x32_x4.lef
+-rw-r--r--   0        0        0     5123 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x4_x4.lef
+-rw-r--r--   0        0        0     7446 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x8_x4.lef
+-rw-r--r--   0        0        0    12437 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x16_x4.lef
+-rw-r--r--   0        0        0    15987 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x22_x4.lef
+-rw-r--r--   0        0        0    21899 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x32_x4.lef
+-rw-r--r--   0        0        0    22455 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x33_x4.lef
+-rw-r--r--   0        0        0    26004 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x39_x4.lef
+-rw-r--r--   0        0        0     5403 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x4_x4.lef
+-rw-r--r--   0        0        0     7718 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x8_x4.lef
+-rw-r--r--   0        0        0    12708 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x16_x4.lef
+-rw-r--r--   0        0        0    17441 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x24_x4.lef
+-rw-r--r--   0        0        0    22174 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x32_x4.lef
+-rw-r--r--   0        0        0     5670 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x4_x4.lef
+-rw-r--r--   0        0        0     7988 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x8_x4.lef
+-rw-r--r--   0        0        0    15410 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x16_lib/SRAM1RW1024x16_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15276 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x16_lib/SRAM1RW1024x16_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15410 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x17_lib/SRAM1RW1024x17_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15276 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x17_lib/SRAM1RW1024x17_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15410 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x32_lib/SRAM1RW1024x32_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15276 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x32_lib/SRAM1RW1024x32_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15410 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x37_lib/SRAM1RW1024x37_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15276 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x37_lib/SRAM1RW1024x37_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15410 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x38_lib/SRAM1RW1024x38_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15276 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x38_lib/SRAM1RW1024x38_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15410 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x44_lib/SRAM1RW1024x44_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15276 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x44_lib/SRAM1RW1024x44_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15410 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x64_lib/SRAM1RW1024x64_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15276 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x64_lib/SRAM1RW1024x64_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15401 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x8_lib/SRAM1RW1024x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15267 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x8_lib/SRAM1RW1024x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15373 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x12_lib/SRAM1RW128x12_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15195 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x12_lib/SRAM1RW128x12_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15373 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x14_lib/SRAM1RW128x14_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15195 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x14_lib/SRAM1RW128x14_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15373 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x22_lib/SRAM1RW128x22_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15195 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x22_lib/SRAM1RW128x22_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15373 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x40_lib/SRAM1RW128x40_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15195 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x40_lib/SRAM1RW128x40_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15373 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x46_lib/SRAM1RW128x46_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15195 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x46_lib/SRAM1RW128x46_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15373 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x48_lib/SRAM1RW128x48_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15195 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x48_lib/SRAM1RW128x48_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15373 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x64_lib/SRAM1RW128x64_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15195 2023-06-15 16:29:20.254908 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x64_lib/SRAM1RW128x64_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15364 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x8_lib/SRAM1RW128x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15186 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x8_lib/SRAM1RW128x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15435 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW2048x8_lib/SRAM1RW2048x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15305 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW2048x8_lib/SRAM1RW2048x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15394 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x128_lib/SRAM1RW256x128_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15242 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x128_lib/SRAM1RW256x128_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15385 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x32_lib/SRAM1RW256x32_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15233 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x32_lib/SRAM1RW256x32_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15385 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x46_lib/SRAM1RW256x46_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15233 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x46_lib/SRAM1RW256x46_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15385 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x48_lib/SRAM1RW256x48_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15233 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x48_lib/SRAM1RW256x48_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15385 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x64_lib/SRAM1RW256x64_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15233 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x64_lib/SRAM1RW256x64_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15198 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x8_lib/SRAM1RW256x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15046 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x8_lib/SRAM1RW256x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15345 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW32x50_lib/SRAM1RW32x50_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15211 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW32x50_lib/SRAM1RW32x50_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15504 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x16_lib/SRAM1RW4096x16_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15294 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x16_lib/SRAM1RW4096x16_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15495 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x8_lib/SRAM1RW4096x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15285 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x8_lib/SRAM1RW4096x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15372 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x128_lib/SRAM1RW512x128_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15276 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x128_lib/SRAM1RW512x128_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15363 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x32_lib/SRAM1RW512x32_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15267 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x32_lib/SRAM1RW512x32_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15363 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x64_lib/SRAM1RW512x64_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15267 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x64_lib/SRAM1RW512x64_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15354 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x8_lib/SRAM1RW512x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15258 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x8_lib/SRAM1RW512x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15386 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x128_lib/SRAM1RW64x128_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15224 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x128_lib/SRAM1RW64x128_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15377 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x20_lib/SRAM1RW64x20_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15215 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x20_lib/SRAM1RW64x20_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15377 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x21_lib/SRAM1RW64x21_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15215 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x21_lib/SRAM1RW64x21_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15377 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x22_lib/SRAM1RW64x22_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15215 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x22_lib/SRAM1RW64x22_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15377 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x32_lib/SRAM1RW64x32_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15215 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x32_lib/SRAM1RW64x32_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15377 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x34_lib/SRAM1RW64x34_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15215 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x34_lib/SRAM1RW64x34_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    15368 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x8_lib/SRAM1RW64x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    15206 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x8_lib/SRAM1RW64x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28859 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x16_lib/SRAM2RW128x16_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28513 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x16_lib/SRAM2RW128x16_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28859 2023-06-15 16:29:20.258909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x32_lib/SRAM2RW128x32_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28513 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x32_lib/SRAM2RW128x32_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28846 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x4_lib/SRAM2RW128x4_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28500 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x4_lib/SRAM2RW128x4_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28846 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x8_lib/SRAM2RW128x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28500 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x8_lib/SRAM2RW128x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28793 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x16_lib/SRAM2RW16x16_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28447 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x16_lib/SRAM2RW16x16_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28793 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x32_lib/SRAM2RW16x32_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28447 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x32_lib/SRAM2RW16x32_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28602 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x4_lib/SRAM2RW16x4_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28256 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x4_lib/SRAM2RW16x4_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28780 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x8_lib/SRAM2RW16x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28434 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x8_lib/SRAM2RW16x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28805 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x16_lib/SRAM2RW32x16_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28547 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x16_lib/SRAM2RW32x16_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28805 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x22_lib/SRAM2RW32x22_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28547 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x22_lib/SRAM2RW32x22_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28805 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x32_lib/SRAM2RW32x32_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28547 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x32_lib/SRAM2RW32x32_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28805 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x33_lib/SRAM2RW32x33_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28547 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x33_lib/SRAM2RW32x33_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28805 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x39_lib/SRAM2RW32x39_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28547 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x39_lib/SRAM2RW32x39_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28792 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x4_lib/SRAM2RW32x4_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28534 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x4_lib/SRAM2RW32x4_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28792 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x8_lib/SRAM2RW32x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28534 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x8_lib/SRAM2RW32x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28869 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x16_lib/SRAM2RW64x16_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28555 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x16_lib/SRAM2RW64x16_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28869 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x24_lib/SRAM2RW64x24_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28555 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x24_lib/SRAM2RW64x24_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28869 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x32_lib/SRAM2RW64x32_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28555 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x32_lib/SRAM2RW64x32_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28856 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x4_lib/SRAM2RW64x4_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28542 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x4_lib/SRAM2RW64x4_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0    28856 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x8_lib/SRAM2RW64x8_PVT_0P63V_100C.lib
+-rw-r--r--   0        0        0    28542 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x8_lib/SRAM2RW64x8_PVT_0P77V_0C.lib
+-rw-r--r--   0        0        0      773 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/asap7/srams.txt
+-rw-r--r--   0        0        0      576 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/nangate45/README.md
+-rw-r--r--   0        0        0      365 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/nangate45/__init__.py
+-rw-r--r--   0        0        0      952 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/nangate45/defaults.yml
+-rw-r--r--   0        0        0     5912 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/nangate45/nangate45.tech.json
+-rw-r--r--   0        0        0     1554 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/nangate45/sram-cache.json
+-rw-r--r--   0        0        0     2835 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/nangate45/sram_compiler/__init__.py
+-rw-r--r--   0        0        0      116 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/nop/__init__.py
+-rw-r--r--   0        0        0       33 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/nop/defaults.yml
+-rw-r--r--   0        0        0       82 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/nop/nop.tech.json
+-rw-r--r--   0        0        0    10427 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/sky130/README.md
+-rw-r--r--   0        0        0    19207 2023-06-15 16:29:20.262909 hammer_vlsi-1.1.2/hammer/technology/sky130/__init__.py
+-rw-r--r--   0        0        0     5255 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/defaults.yml
+-rw-r--r--   0        0        0      747 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/defaults_types.yml
+-rw-r--r--   0        0        0      899 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/extra/cells-gen.py
+-rw-r--r--   0        0        0    11554 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/extra/cells.txt
+-rw-r--r--   0        0        0     6772 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/extra/efabless_template.io
+-rw-r--r--   0        0        0     2907 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/extra/fill.json
+-rwxr-xr-x   0        0        0     3552 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/extra/openram/sram-cache-gen.py
+-rw-r--r--   0        0        0     5531 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/extra/openram/sram-cache.json
+-rw-r--r--   0        0        0      172 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/extra/openram/srams.txt
+-rw-r--r--   0        0        0     5081 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/extra/s8io.yml
+-rw-r--r--   0        0        0      785 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/extra/setRC.tcl
+-rw-r--r--   0        0        0      421 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/extra/sky130-tech-gen-files/beginning.json
+-rw-r--r--   0        0        0     1152 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/extra/sky130-tech-gen-files/beginning_nda.json
+-rw-r--r--   0        0        0     1597 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/extra/sky130-tech-gen-files/cells.json
+-rw-r--r--   0        0        0      114 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/extra/sky130-tech-gen-files/sites.json
+-rwxr-xr-x   0        0        0     3221 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/extra/sky130-tech-gen-files/stackups-gen.py
+-rw-r--r--   0        0        0     2274 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/extra/sky130-tech-gen-files/stackups.json
+-rwxr-xr-x   0        0        0     6592 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/extra/sky130-tech-gen.py
+-rw-r--r--   0        0        0     2478 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/extra/sky130_lefpin.map
+-rwxr-xr-x   0        0        0     3010 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/extra/sram22/sram-cache-gen.py
+-rw-r--r--   0        0        0     6699 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/extra/sram22/sram-cache.json
+-rw-r--r--   0        0        0      320 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/extra/sram22/srams.txt
+-rw-r--r--   0        0        0    63375 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/sky130.tech.json
+-rw-r--r--   0        0        0     6699 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/sram-cache.json
+-rw-r--r--   0        0        0    10942 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/sky130/sram_compiler/__init__.py
+-rw-r--r--   0        0        0      330 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/vivado/vivado.plsi_config.json
+-rw-r--r--   0        0        0      456 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/technology/vivado/vivado.tech.json
+-rw-r--r--   0        0        0    12224 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/timing/tempus/__init__.py
+-rw-r--r--   0        0        0      605 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/timing/tempus/defaults.yml
+-rw-r--r--   0        0        0    14969 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/utils/__init__.py
+-rw-r--r--   0        0        0     3300 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/utils/lef_utils.py
+-rw-r--r--   0        0        0     1844 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/utils/verilog_utils.py
+-rw-r--r--   0        0        0      398 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/vlsi/__init__.py
+-rw-r--r--   0        0        0    92096 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/vlsi/cli_driver.py
+-rw-r--r--   0        0        0    34891 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/vlsi/constraints.py
+-rw-r--r--   0        0        0    84070 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/vlsi/driver.py
+-rw-r--r--   0        0        0    29733 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/vlsi/hammer_build_systems.py
+-rw-r--r--   0        0        0    76128 2023-06-15 16:29:20.266909 hammer_vlsi-1.1.2/hammer/vlsi/hammer_tool.py
+-rw-r--r--   0        0        0    98711 2023-06-15 16:29:20.270909 hammer_vlsi-1.1.2/hammer/vlsi/hammer_vlsi_impl.py
+-rw-r--r--   0        0        0     1655 2023-06-15 16:29:20.270909 hammer_vlsi-1.1.2/hammer/vlsi/hooks.py
+-rw-r--r--   0        0        0    14068 2023-06-15 16:29:20.270909 hammer_vlsi-1.1.2/hammer/vlsi/submit_command.py
+-rw-r--r--   0        0        0    10163 2023-06-15 16:29:20.270909 hammer_vlsi-1.1.2/hammer/vlsi/units.py
+-rw-r--r--   0        0        0       61 2023-06-15 16:29:20.270909 hammer_vlsi-1.1.2/hammer/vlsi/vendor/__init__.py
+-rw-r--r--   0        0        0     6939 2023-06-15 16:29:20.270909 hammer_vlsi-1.1.2/hammer/vlsi/vendor/def2stream.py
+-rw-r--r--   0        0        0    12189 2023-06-15 16:29:20.270909 hammer_vlsi-1.1.2/hammer/vlsi/vendor/openroad.py
+-rw-r--r--   0        0        0     2331 2023-06-15 16:29:55.201991 hammer_vlsi-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3326 1970-01-01 00:00:00.000000 hammer_vlsi-1.1.2/PKG-INFO
```

### Comparing `hammer_vlsi-1.1.1/LICENSE` & `hammer_vlsi-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/README.md` & `hammer_vlsi-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/common/cadence/__init__.py` & `hammer_vlsi-1.1.2/hammer/common/cadence/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/common/mentor/defaults.yml` & `hammer_vlsi-1.1.2/hammer/common/mentor/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/common/mentor/defaults_types.yml` & `hammer_vlsi-1.1.2/hammer/common/mentor/defaults_types.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/common/synopsys/__init__.py` & `hammer_vlsi-1.1.2/hammer/common/synopsys/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/common/vivado/vivado_core.py` & `hammer_vlsi-1.1.2/hammer/common/vivado/vivado_core.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/config/config_src.py` & `hammer_vlsi-1.1.2/hammer/config/config_src.py`

 * *Files 5% similar despite different names*

```diff
@@ -224,14 +224,102 @@
         return [replace_if_target_setting(target),
                 replace_if_target_setting(append)], "crossappendref"
 
     directives['crossappendref'] = MetaDirective(action=crossappendref_action,
                                                  target_settings=crossappendref_targets,
                                                  rename_target=crossappendref_rename)
 
+    def prepend_action(config_dict: dict, key: str, value: Any) -> None:
+        if key not in config_dict:
+            config_dict[key] = []
+
+        if not isinstance(config_dict[key], list):
+            raise ValueError(f"Trying to prepend to non-list setting {key}")
+        if not isinstance(value, list):
+            raise ValueError(f"Trying to prepend to list {key} with non-list {value}")
+        config_dict[key] = value + config_dict[key]
+
+    def prepend_rename(key: str, value: Any, target_setting: str, replacement_setting: str) -> Optional[Tuple[Any, str]]:
+        return [replacement_setting, value], "crossprepend"
+
+    # prepend depends only on itself
+    directives['prepend'] = MetaDirective(action=prepend_action,
+                                         target_settings=lambda key, value: [key],
+                                         rename_target=prepend_rename)
+
+    def crossprepend_decode(value: Any) -> Tuple[str, list]:
+        assert isinstance(value, list), "crossprepend takes a list of two elements"
+        assert len(value) == 2, "crossprepend takes a list of two elements"
+        target_setting = value[0]  # type: str
+        prepend_value = value[1]  # type: list
+        assert isinstance(target_setting, str), "crossprepend target setting must be a string"
+        assert isinstance(prepend_value, list), "crossprepend must prepend a list"
+        return target_setting, prepend_value
+
+    # crossprepend takes a list that has two elements.
+    # The first is the target list (the list to prepend to), and the second is
+    # a list to prepend to the target list.
+    # e.g. if base has ["1"] and crossprepend has ["base", ["2", "3"]], then
+    # the result will be ["2", "3", "1"].
+    def crossprepend_action(config_dict: dict, key: str, value: Any) -> None:
+        target_setting, prepend_value = crossprepend_decode(value)
+        config_dict[key] = prepend_value + config_dict[target_setting]
+
+    def crossprepend_targets(key: str, value: Any) -> List[str]:
+        target_setting, prepend_value = crossprepend_decode(value)
+        return [target_setting]
+
+    def crossprepend_rename(key: str, value: Any, target_setting: str, replacement_setting: str) -> Optional[
+        Tuple[Any, str]]:
+        crossprepend_target, prepend_value = crossprepend_decode(value)
+        return [replacement_setting if crossprepend_target == target_setting else crossprepend_target,
+                prepend_value], "crossprepend"
+
+    directives['crossprepend'] = MetaDirective(action=crossprepend_action,
+                                              target_settings=crossprepend_targets,
+                                              rename_target=crossprepend_rename)
+
+    def crossprependref_decode(value: Any) -> Tuple[str, str]:
+        assert isinstance(value, list), "crossprependref takes a list of two elements"
+        assert len(value) == 2, "crossprependref takes a list of two elements"
+        target_key = value[0]  # type: str
+        prepend_key = value[1]  # type: str
+        assert isinstance(target_key, str), "crossprependref target setting must be a string"
+        assert isinstance(prepend_key, str), "crossprepend prepend list setting must be a string"
+        return target_key, prepend_key
+
+    # crossprependref takes a list that has two elements.
+    # The first is the target list (the list to prepend to), and the second is
+    # a setting that contains a list to prepend.
+    # e.g. if base has ["1"], app has ["2", "3"], and crossprepend has ["base", "app"], the result
+    # is ["2", "3", "1"].
+    def crossprependref_action(config_dict: dict, key: str, value: Any) -> None:
+        target_setting, prepend_setting = crossprependref_decode(value)
+        config_dict[key] = config_dict[prepend_setting] + config_dict[target_setting]
+
+    def crossprependref_targets(key: str, value: Any) -> List[str]:
+        target_setting, prepend_setting = crossprependref_decode(value)
+        return [target_setting, prepend_setting]
+
+    def crossprependref_rename(key: str, value: Any, target_setting: str, replacement_setting: str) -> Optional[
+        Tuple[Any, str]]:
+        target, prepend = crossprependref_decode(value)
+
+        def replace_if_target_setting(setting: str) -> str:
+            """Helper function to replace the given setting with the
+            replacement if it is equal to target_setting."""
+            return replacement_setting if setting == target_setting else setting
+
+        return [replace_if_target_setting(target),
+                replace_if_target_setting(prepend)], "crossprependref"
+
+    directives['crossprependref'] = MetaDirective(action=crossprependref_action,
+                                                 target_settings=crossprependref_targets,
+                                                 rename_target=crossprependref_rename)
+
     def subst_str(input_str: str, replacement_func: Callable[[str], str]) -> str:
         """Substitute ${...}"""
         return re.sub(__VARIABLE_EXPANSION_REGEX, lambda x: replacement_func(x.group(1)), input_str)
 
     def subst_action(config_dict: dict, key: str, value: Any) -> None:
         def perform_subst(value: Union[str, List[str]]) -> Union[str, List[str]]:
             """
@@ -773,15 +861,15 @@
         :param nullvalue: Value to return out for nulls.
         :param check_type: Flag to enforce type checking
         :return: The given config
         """
         default  = key
         override = default + "_" + suffix
         value = None
-        try: 
+        try:
             value = self.get_config()[override]
         except:
             try:
                 value = self.get_config()[default]
             except:
                 raise KeyError(f"Both base key: {default} and overriden key: {override} are missing.")
 
@@ -897,24 +985,24 @@
         :param key_prefix: Specify a prefix for the given keys.
         :optional_keys: Specify optional keys where if no setting is provided a default value of None will be provided.
         :return: A dictionary of keys and corresponding input values.
         """
 
         opt_dict={}
         for key, default_value in key_default_dict.items():
-            try: 
+            try:
                 if not key_prefix:
                     extracted_value = self.get_setting(f"{key}", default_value)
                 else:
                     extracted_value = self.get_setting(f"{key_prefix}.{key}", default_value)
                 opt_dict[key] = extracted_value
             except KeyError:
                 if key not in optional_keys:
                     raise ValueError(f"Missing a mandatory requested key: {key_prefix}.{key}")
-                else: 
+                else:
                     opt_dict[key] = None
 
         return opt_dict
 
     def update_core(self, core_config: List[dict], core_config_types: List[dict]) -> None:
         """
         Update the core config with the given core config.
```

### Comparing `hammer_vlsi-1.1.1/hammer/config/defaults.yml` & `hammer_vlsi-1.1.2/hammer/config/defaults.yml`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,17 @@
   # TODO: remove this after stackup supports vias ucb-bar/hammer#354
   
   tap_cell_interval: 10.0 # Spacing between columns of tap cells (float)
   # Must be overridden by technology plugin defaults or else you will have DRC/latch-up errors.
 
   tap_cell_offset: 0.0 # Offset of the first column of tape cells from the edge of the floorplan (float)
   # Should be overridden by technology plugin defaults.
+  
+  routing_layers: null # If specified, set/override the [bottom, top] layers used for routing. (Optional[Tuple[int, int]])
+  # Both must match the index number (not name) of layers used in the stackup.
 
   extra_libraries: [] # Extra semiconductor IP libraries/stdcell libs/hard macros. (List[ExtraLibrary])
   # Used for non-technology-vendor-provided custom IP blocks.
   # ExtraLibrary is a struct with two fields:
   # - prefix (Optional[PathPrefix]) - struct that holds a prefix and path.
   #   - path (str) - Path for the prefix below.
   #     For example, if the path is /foo/bar/pll, then a reference of pll/test.txt (assuming 'pll' is the prefix) will
@@ -423,15 +426,16 @@
     svg_file_meta: lazysubst
     shorten_path_depth: 1 # Depth of paths to shorten for better readability in the SVG
     # E.g. top/path/to/inst will shorten to t/p/t/inst for depth of 1 and t/p/top/inst for depth of 2
     # A depth of 0 or less will perform no path shortening.
     # type: int
 
 vlsi.submit:
-  command: "local" # The submit command to use. "none", "local", or null will run on the current host. See hammer_submit_command.py for other options.
+  command: "local" # The submit command to use. "none", "local", or null will run on the current host. "lsf" and "slurm" are also supported.
+  # See hammer/vlsi/submit_command.py for all options and their associated settings.
   settings: [] # type: List[Dict[str, Dict[str, Any]]]
   # The list substitutes settings in order of appearance, and the first Dict key is the command.
   # The second dict key is the name of that command's setting, followed by whatever type it takes.
 
 synthesis.inputs:
 # Specific inputs for the synthesis tool.
 # These inputs are the generic inputs; specific tools ("CAD junk") may require
@@ -638,16 +642,14 @@
   top_module: null # Top RTL module.
 
   layout_file: null # Input layout file
   # Typically a GDSII file from the place and route tool
 
   schematic_files: [] # Input list of schematic files
 
-  ilms: [] # Input list of ILMStructs
-
   hcells_list: [] # Input list of LVS Hcells
 
   additional_lvs_text_mode: "auto" # Valid modes are auto, manual, prepend, and append
   additional_lvs_text: "" # Custom LVS command text to add after the boilerplate commands at the top of the run file
 
 lvs.submit:
   command: "${vlsi.submit.command}"
@@ -680,17 +682,14 @@
     # type: str
     special_cells: null # Key name for the technology's special cells
     # This should exist in the special_cells list in the tech json
     # type: str
     std_cell_rail_layer: null # This should specify the TOPMOST metal layer the standard cells use for power rails
     # Note that this is not usually stackup specific; it is based on the std cell library
     # type: str
-    tap_cell_rail_reference: null # This is used to provide a reference master for generating standard cell rails
-    # Can be a wildcard/glob
-    # type: str
     std_cell_supplies:
     # Names of the power and ground rails of the standard cells
         power: ["VDD"]
         ground: ["VSS"]
 
 # Specific inputs for the simulation tool.
 # These inputs will vary based on if the simulation is for RTL, post synthesis, or post PAR.
```

### Comparing `hammer_vlsi-1.1.1/hammer/config/defaults_types.yml` & `hammer_vlsi-1.1.2/hammer/config/defaults_types.yml`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,17 @@
   # type: float
   tap_cell_interval: float
 
   # Offset of the first column of tape cells from the edge of the floorplan
   # type: float
   tap_cell_offset: float 
 
+  # Set the [bottom, top] layer used for routing. (Optional[Tuple[int, int]])
+  routing_layers: Optional[list[int]]
+
   # Extra semiconductor IP libraries/stdcell libs/hard macros. (List[ExtraLibrary])
   # ExtraLibrary is serialized as a list[dict[str, str]]
   # TODO: Extralibrary does not have a clean JSON serialization as of late
   extra_libraries: list[dict[str, Any]]
 
   # Extra information about macro sizes.
   extra_macro_sizes: list[dict[str, str]]
@@ -352,17 +355,14 @@
 
   # Input layout file
   layout_file: Optional[str]
 
   # Input list of schematic files
   schematic_files: list[str]
 
-  # Input list of ILMStructs
-  ilms: list[dict[str, Any]]
-
   # Input list of Hcells
   hcells_list: list[str]
 
   # Valid modes are auto, manual, prepend, and append
   additional_lvs_text_mode: str
   # Custom LVS command text to add after the boilerplate commands at the top of the run file
   additional_lvs_text: str
@@ -393,17 +393,14 @@
     stackup: Optional[str]
     # Key name for the technology's special cells
     # type: str
     special_cells: Optional[str]
     # This should specify the TOPMOST metal layer the standard cells use for power rails
     # type: str
     std_cell_rail_layer: Optional[str]
-    # This is used to provide a reference master for generating standard cell rails
-    # type: str
-    tap_cell_rail_reference: Optional[str]
 
     # Name of standard cell power/ground rails
     std_cell_supplies:
       power: list[str]
       ground: list[str]
 
 # Specific inputs for the simulation tool.
```

### Comparing `hammer_vlsi-1.1.1/hammer/config/yaml2json.py` & `hammer_vlsi-1.1.2/hammer/config/yaml2json.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/drc/icv/README.md` & `hammer_vlsi-1.1.2/hammer/drc/icv/README.md`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/drc/icv/__init__.py` & `hammer_vlsi-1.1.2/hammer/drc/icv/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/drc/icv/defaults.yml` & `hammer_vlsi-1.1.2/hammer/drc/icv/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/drc/magic/__init__.py` & `hammer_vlsi-1.1.2/hammer/drc/magic/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/drc/magic/defaults.yml` & `hammer_vlsi-1.1.2/hammer/drc/magic/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/drc/mockdrc/__init__.py` & `hammer_vlsi-1.1.2/hammer/drc/mockdrc/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/drc/openroad/__init__.py` & `hammer_vlsi-1.1.2/hammer/drc/openroad/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/formal/conformal/__init__.py` & `hammer_vlsi-1.1.2/hammer/formal/conformal/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/formal/conformal/defaults.yml` & `hammer_vlsi-1.1.2/hammer/formal/conformal/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/generate_properties.py` & `hammer_vlsi-1.1.2/hammer/generate_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,17 +180,15 @@
     HammerLVSTool = Interface(module="HammerLVSTool",
                               filename="vlsi/hammer_vlsi_impl.py",
                               inputs=[
                                   InterfaceVar("layout_file", "str", "path to the input layout file (e.g. a *.gds)"),
                                   InterfaceVar("schematic_files", "List[str]",
                                                "path to the input SPICE or Verilog schematic files (e.g. *.v or *.spi)"),
                                   InterfaceVar("hcells_list", "List[str]",
-                                               "list of cells to explicitly map hierarchically in LVS"),
-                                  InterfaceVar("ilms", "List[ILMStruct]",
-                                               "list of (optional) input ILM information for hierarchical mode")
+                                               "list of cells to explicitly map hierarchically in LVS")
                               ],
                               outputs=[]
                               )
 
     HammerSimTool = Interface(module="HammerSimTool",
                               filename="vlsi/hammer_vlsi_impl.py",
                               inputs=[
```

### Comparing `hammer_vlsi-1.1.1/hammer/logging/logging.py` & `hammer_vlsi-1.1.2/hammer/logging/logging.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/logging/test.py` & `hammer_vlsi-1.1.2/hammer/logging/test.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/lvs/icv/__init__.py` & `hammer_vlsi-1.1.2/hammer/lvs/icv/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     def generate_hcells_file(self) -> None:
         with open(self.hcells_file, "w") as f:
             f.write("")
             # TODO
 
     def generate_top_icv_file(self) -> None:
         library_spice_files = self.technology.read_libs([hammer_tech.filters.spice_filter], hammer_tech.HammerTechnologyUtils.to_plain_item)
-        ilms = list(map(lambda x: x.netlist, self.ilms))  # type: List[str]
+        ilms = list(map(lambda x: x.netlist, self.get_input_ilms()))  # type: List[str]
 
         all_files = library_spice_files + self.schematic_files + ilms
         spice_files = list(filter(lambda x: get_filetype(x) is HammerFiletype.SPICE, all_files))
         verilog_files = list(filter(lambda x: get_filetype(x) is HammerFiletype.VERILOG, all_files))
         unmatched = set(all_files).symmetric_difference(set(spice_files + verilog_files))
         if unmatched:
             raise NotImplementedError("Unsupported netlist type for files: " + str(unmatched))
```

### Comparing `hammer_vlsi-1.1.1/hammer/lvs/icv/defaults.yml` & `hammer_vlsi-1.1.2/hammer/lvs/icv/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/lvs/netgen/__init__.py` & `hammer_vlsi-1.1.2/hammer/lvs/netgen/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         # libs for circuit1. spice format must be specified.
         self.append('puts "Reading layout..."')
         self.append("readnet spice {} 1".format(self.ext2spice_netlist))
 
         # libs for circuit2. auto format detection (somewhat dangerous).
         self.append('puts "Reading schematics..."')
         library_spice_files = self.technology.read_libs([hammer_tech.filters.spice_filter], hammer_tech.HammerTechnologyUtils.to_plain_item)
-        ilms = list(map(lambda x: x.netlist, self.ilms))  # type: List[str]
+        ilms = list(map(lambda x: x.netlist, self.get_input_ilms()))  # type: List[str]
         for sch in self.schematic_files + ilms + library_spice_files:
             self.append('puts "Reading {}..."'.format(sch))
             self.append("readnet {} 2".format(sch))
 
         self.append(self.get_additional_lvs_text())
 
         self.append('puts "Running LVS..."')
```

### Comparing `hammer_vlsi-1.1.1/hammer/lvs/netgen/defaults.yml` & `hammer_vlsi-1.1.2/hammer/lvs/netgen/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/par/innovus/__init__.py` & `hammer_vlsi-1.1.2/hammer/par/innovus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,14 +297,27 @@
         # Run init_design to validate data and start the Cadence place-and-route workflow.
         verbose_append("init_design")
 
         # Setup power settings from cpf/upf
         for l in self.generate_power_spec_commands():
             verbose_append(l)
 
+        # Set the top and bottom global/detail routing layers.
+        # This must happen after the tech LEF is loaded
+        layers = self.get_setting("vlsi.technology.routing_layers")
+        if layers is not None:
+            if self.version() >= self.version_number("201"):
+                verbose_append(f"set_db design_bottom_routing_layer {layers[0]}")
+                verbose_append(f"set_db design_top_routing_layer {layers[1]}")
+            else:
+                verbose_append(f"set_db route_early_global_bottom_layer {layers[0]}")
+                verbose_append(f"set_db route_early_global_top_layer {layers[1]}")
+                verbose_append(f"set_db route_design_bottom_layer {layers[0]}")
+                verbose_append(f"set_db route_design_top_layer {layers[1]}")
+
         # Set design effort.
         verbose_append("set_db design_flow_effort {}".format(self.get_setting("par.innovus.design_flow_effort")))
 
         # Set "don't use" cells.
         for l in self.generate_dont_use_commands():
             self.append(l)
 
@@ -393,19 +406,29 @@
         fp_urx = const.width - const.margins.right
         fp_ury = const.height - const.margins.top
 
         pin_assignments = self.get_pin_assignments()
         self.verbose_append("set_db assign_pins_edit_in_batch true")
 
         promoted_pins = []  # type: List[str]
+        # Set the top/bottom layers for promoting macro pins
+        self.append(f"set_db assign_pins_promoted_macro_bottom_layer {self.get_stackup().get_metal_by_index(1).name}")
+        self.append(f"set_db assign_pins_promoted_macro_top_layer {self.get_stackup().get_metal_by_index(-1).name}")
+        self.append('set all_ppins ""')
         for pin in pin_assignments:
             if pin.preplaced:
-                # First set promoted pins
-                self.verbose_append("set_promoted_macro_pin -pins {{ {p} }}".format(p=pin.pins))
-                promoted_pins.extend(pin.pins.split())
+                # Find the pin object that should be promoted. Only one of the two (driver_pins or load_pins) should be non-empty.
+                self.append(f'set ppins [get_db [get_nets {pin.pins}] .driver_pins]')
+                self.append(f'if {{$ppins eq ""}} {{set ppins [get_db [get_nets {pin.pins}] .load_pins]}}')
+                self.append("lappend all_ppins $ppins")
+                # First promote the pin
+                self.append("set_promoted_macro_pin -insts [get_db $ppins .inst.name] -pins [get_db $ppins .base_name]")
+                # Then set them to don't touch and skip routing
+                self.append("set_dont_touch [get_db $ppins .net]")
+                self.append("set_db [get_db $ppins .net] .skip_routing true")
             else:
                 # TODO: Do we need pin blockages for our layers?
                 # Seems like we will only need special pin blockages if the vias are larger than the straps
 
                 cadence_side = None  # type: Optional[str]
                 if pin.side is not None:
                     if pin.side == "internal":
@@ -457,18 +480,16 @@
                     assign_arg,
                     width_arg,
                     depth_arg
                 ]
 
                 self.verbose_append(" ".join(cmd))
 
-        # In case the * wildcard is used after preplaced pins, this will place promoted pins correctly.
-        # Innovus errors instead of warns if the name matching does not work (e.g. bad wildcards).
-        for ppin in promoted_pins:
-            self.verbose_append("assign_io_pins -move_fixed_pin -pins [get_db [get_db pins -if {{.name == {p} }}] .net.name]".format(p=ppin))
+        # In case the * wildcard is used after preplaced pins, this will put back the promoted pins correctly.
+        self.verbose_append("if {[llength $all_ppins] ne 0} {assign_io_pins -move_fixed_pin -pins [get_db $all_ppins .net.name]}")
 
         self.verbose_append("set_db assign_pins_edit_in_batch false")
         return True
 
     def power_straps(self) -> bool:
         """Place the power straps for the design."""
         power_straps_tcl = os.path.join(self.run_dir, "power_straps.tcl")
@@ -665,15 +686,15 @@
                 self.logger.error(
                     "par.inputs.gds_precision value of \"%s\" must be one of %s" %(
                         gds_precision, ', '.join([str(x) for x in valid_values])));
                 return False
         # "auto", i.e. not "manual", means not specifying anything extra.
 
         self.verbose_append(
-            "write_stream -mode ALL {map_file} {merge_options} {unit} {gds}".format(
+            "write_stream -mode ALL -format stream {map_file} {merge_options} {unit} {gds}".format(
             map_file=map_file,
             merge_options=merge_options,
             gds=self.output_gds_filename,
             unit=unit
         ))
         return True
 
@@ -1005,15 +1026,15 @@
                         output.append("create_place_blockage -area {{{x} {y} {urx} {ury}}}".format(
                             x=constraint.x,
                             y=constraint.y,
                             urx=constraint.x+constraint.width,
                             ury=constraint.y+constraint.height
                         ))
                     if ObstructionType.Route in obs_types:
-                        output.append("create_route_blockage -layers {{{layers}}} -spacing 0 -{area_flag} {{{x} {y} {urx} {ury}}}".format(
+                        output.append("create_route_blockage -except_pg_nets -layers {{{layers}}} -spacing 0 -{area_flag} {{{x} {y} {urx} {ury}}}".format(
                             x=constraint.x,
                             y=constraint.y,
                             urx=constraint.x+constraint.width,
                             ury=constraint.y+constraint.height,
                             area_flag="rects" if self.version() >= self.version_number("181") else "area",
                             layers="all" if constraint.layers is None else " ".join(get_or_else(constraint.layers, []))
                         ))
@@ -1029,15 +1050,15 @@
                 else:
                     assert False, "Should not reach here"
         return [chip_size_constraint] + output
 
     def specify_std_cell_power_straps(self, blockage_spacing: Decimal, bbox: Optional[List[Decimal]], nets: List[str]) -> List[str]:
         """
         Generate a list of TCL commands that build the low-level standard cell power strap rails.
-        This will use the -master option to create power straps based on technology.core.tap_cell_rail_reference.
+        This will use the -master option to create power straps based on the tapcells in the special cells list.
         The layer is set by technology.core.std_cell_rail_layer, which should be the highest metal layer in the std cell rails.
 
         :param bbox: The optional (2N)-point bounding box of the area to generate straps. By default the entire core area is used.
         :param nets: A list of power net names (e.g. ["VDD", "VSS"]). Currently only two are supported.
         :return: A list of TCL commands that will generate power straps on rails.
         """
         layer_name = self.get_setting("technology.core.std_cell_rail_layer")
@@ -1045,20 +1066,20 @@
         results = [
             "# Power strap definition for layer {} (rails):\n".format(layer_name),
             "reset_db -category add_stripes",
             "set_db add_stripes_stacked_via_bottom_layer {}".format(layer_name),
             "set_db add_stripes_stacked_via_top_layer {}".format(layer_name),
             "set_db add_stripes_spacing_from_block {}".format(blockage_spacing)
         ]
-        tapcell = self.get_setting("technology.core.tap_cell_rail_reference")
+        tapcells = self.technology.get_special_cell_by_type(CellType.TapCell)[0].name
         options = [
             "-pin_layer", layer_name,
             "-layer", layer_name,
             "-over_pins", "1",
-            "-master", "\"{}\"".format(tapcell),
+            "-master", "\"{}\"".format(" ".join(tapcells)),
             "-block_ring_bottom_layer_limit", layer_name,
             "-block_ring_top_layer_limit", layer_name,
             "-pad_core_ring_bottom_layer_limit", layer_name,
             "-pad_core_ring_top_layer_limit", layer_name,
             "-direction", str(layer.direction),
             "-width", "pin_width",
             "-nets", "{ %s }" % " ".join(nets)
```

### Comparing `hammer_vlsi-1.1.1/hammer/par/innovus/defaults.yml` & `hammer_vlsi-1.1.2/hammer/par/innovus/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/par/innovus/dump_stackup_to_json.tcl` & `hammer_vlsi-1.1.2/hammer/par/innovus/dump_stackup_to_json.tcl`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/par/nop/__init__.py` & `hammer_vlsi-1.1.2/hammer/par/nop/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/par/openroad/README.md` & `hammer_vlsi-1.1.2/hammer/par/openroad/README.md`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/par/openroad/__init__.py` & `hammer_vlsi-1.1.2/hammer/par/openroad/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,15 +222,15 @@
     def metrics_file(self) -> str:
         return os.path.join(self.metrics_dir, f"metrics-{self._steps_to_run[-1]}.json")
 
     @property
     def fill_cells(self) -> str:
         stdfillers = self.technology.get_special_cell_by_type(CellType.StdFiller)
         return ' '.join(list(map(lambda c: str(c), stdfillers[0].name)))
-    
+
     @property
     def timing_driven(self) -> bool:
         return self.get_setting('par.openroad.timing_driven')
 
     def reports_path(self, rpt_name) -> str:
         return os.path.join(self.reports_dir, rpt_name)
 
@@ -385,20 +385,20 @@
             shutil.copy2(setrc_file, os.path.join(issue_dir, os.path.basename(setrc_file)))
 
         # RCX File
         openrcx_files = self.get_setting('par.openroad.openrcx_techfiles')
         for openrcx_file in openrcx_files:
             if os.path.exists(openrcx_file):
                 shutil.copy2(openrcx_file, os.path.join(issue_dir, os.path.basename(openrcx_file)))
-        
+
         # KLayout tech file
         klayout_techfile_path = self.setup_klayout_techfile()
         if klayout_techfile_path and os.path.exists(klayout_techfile_path):
             shutil.copy2(klayout_techfile_path, os.path.join(issue_dir, os.path.basename(klayout_techfile_path)))
-        
+
         # DEF2Stream file
         def2stream_file = self.get_setting('par.openroad.def2stream_file')
         if os.path.exists(def2stream_file):
             shutil.copy2(def2stream_file, os.path.join(issue_dir, os.path.basename(def2stream_file)))
 
         # Hack par.tcl script
         # Remove abspaths to files since they are now in issue_dir
@@ -1077,29 +1077,35 @@
         # IO Placement
         """)
         self.block_append(self.place_pins_tcl())
         return True
 
 
     def global_placement(self) -> bool:
-        metals=self.get_stackup().metals[1:]
+        layers = self.get_setting("vlsi.technology.routing_layers")
+        if layers is not None:
+            bottom_layer = self.get_stackup().get_metal_by_index(layers[0]).name
+            top_layer = self.get_stackup().get_metal_by_index(layers[1]).name
+        else:
+            metals=self.get_stackup().metals[1:]
+            bottom_layer = metals[0].name
+            top_layer = metals[-1].name
         routing_adj = self.get_setting('par.openroad.global_placement.routing_adjustment')
         spacing = self.get_setting('par.blockage_spacing')
-        idx_clock_bottom_metal=min(2,len(metals)-1)
         density = self.get_setting('par.openroad.global_placement.density')
         padding = self.get_setting('par.openroad.global_placement.placement_padding')
         routability_driven = "-routability_driven" if self.get_setting('par.openroad.global_placement.routability_driven') else ""
         timing_driven = "-timing_driven" if self.timing_driven and self.get_setting('par.openroad.global_placement.timing_driven') else ""
         self.block_append(f"""
         ################################################################
         # Global placement (with placed IOs, timing-driven, and routability-driven)
         # set_dont_use {{{' '.join(self.get_dont_use_list())}}}
         # reduce the routing resources of all routing layers by X%
-        set_global_routing_layer_adjustment {metals[0].name}-{metals[-1].name} {routing_adj}
-        set_routing_layers -signal {metals[0].name}-{metals[-1].name} -clock {metals[idx_clock_bottom_metal].name}-{metals[-1].name}
+        set_global_routing_layer_adjustment {bottom_layer}-{top_layer} {routing_adj}
+        set_routing_layers -signal {bottom_layer}-{top_layer} -clock {bottom_layer}-{top_layer}
         # creates blockages around macros
         # set_macro_extension {spacing}
 
         # -density default is 0.7, overflow default is 0.1
         global_placement -density {density} -pad_left {padding} -pad_right {padding} {routability_driven} {timing_driven}
 
         estimate_parasitics -placement
@@ -1413,14 +1419,20 @@
         with open(source_path, 'r') as sf:
             with open(dest_path, 'w') as df:
                 self.logger.info("Modifying Klayout Techfile: {} -> {}".format
                     (source_path, dest_path))
                 for line in sf:
                     if "<lef-files>merged.lef</lef-files>" in line:
                         continue
+                    if '<no-zero-length-paths>' in line:
+                        """ we want to disallow zero length paths (i.e. convert to a polygon instead)
+                            otherwise calibre throws an error during DRC/LVS
+                            but setting this flag to 'true' doesn't seem to work
+                        """
+                        line = line.replace('<no-zero-length-paths>false','<no-zero-length-paths>true')
                     if '</lefdef>' in line:
                         df.write(insert_lines)
                     df.write(line)
         return str(klayout_techfile_path)
 
 
     def write_gds(self) -> str:
@@ -1479,15 +1491,15 @@
         """, cmds, clean=False, verbose=False)
         return '\n'.join(cmds).strip()
 
 
     def write_regs(self) -> bool:
         # TODO: currently no analagous OpenROAD default script
         return True
-    
+
     def write_reports(self, prefix: str) -> str:
         if self.get_setting('par.openroad.write_reports') and self.timing_driven:
             return f"write_reports {prefix}"
         else:
             return ""
 
     @property
@@ -1503,15 +1515,15 @@
 
     def create_write_reports_tcl(self) -> List[str]:
         '''
         Creates the write_repors.tcl command that is sourced at the beginning of an OpenROAD session,
             and is called with the command "write_reports <prefix>"
         Output report info with header and footer, to be read by the log_to_reports() function
             and written to the appropriate report file after OpenROAD completes.
-        The <cmd>_metric(s) commands tells OpenROAD to dump this metric into the JSON 
+        The <cmd>_metric(s) commands tells OpenROAD to dump this metric into the JSON
             file specified by the -metrics flag in the tool invocation (see self.metrics_file)
         '''
         # NOTE: both report_check_types and report_power commands have [> filename] option but it just generates an empty file...
         write_reports_cmds = [""]
         prefix = "${prefix}"
         self.block_tcl_append("""
         ################################################################
@@ -1703,15 +1715,15 @@
         elif orientation == 'mx90':
             return (x,y)
         elif orientation == 'my90':
             return (x+height,y+width)
         else:
             self.logger.error(f"Invalid orientation {orientation}")
             return (x,y)
-    
+
     def rotate_coordinates(self, origin: Tuple[Decimal, Decimal], orientation: str) -> Tuple[str, str]:
         # TODO: need to figure out origin translations for rotations besides R90/R270
         x = str(origin[0])
         y = str(origin[1])
         if orientation == 'r0':
             return (x,y)
         elif orientation == 'r90':
@@ -1849,15 +1861,15 @@
                     assert False, "Should not reach here"
         return output
 
 
     def specify_std_cell_power_straps(self, blockage_spacing: Decimal, bbox: Optional[List[Decimal]], nets: List[str]) -> List[str]:
         """
         Generate a list of TCL commands that build the low-level standard cell power strap rails.
-        This will use the -master option to create power straps based on technology.core.tap_cell_rail_reference.
+        This will use the -master option to create power straps based on the tapcells in the special cells list.
         The layer is set by technology.core.std_cell_rail_layer, which should be the highest metal layer in the std cell rails.
         :param bbox: The optional (2N)-point bounding box of the area to generate straps. By default the entire core area is used.
         :param nets: A list of power net names (e.g. ["VDD", "VSS"]). Currently only two are supported.
         :return: A list of TCL commands that will generate power straps on rails.
         """
         layer_name = self.get_setting('technology.core.std_cell_rail_layer')
         layer = self.get_stackup().get_metal(layer_name)
```

### Comparing `hammer_vlsi-1.1.1/hammer/par/openroad/defaults.yml` & `hammer_vlsi-1.1.2/hammer/par/openroad/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/par/openroad/defaults_types.yml` & `hammer_vlsi-1.1.2/hammer/par/openroad/defaults_types.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/par/vivado/__init__.py` & `hammer_vlsi-1.1.2/hammer/par/vivado/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/pcb/generic/__init__.py` & `hammer_vlsi-1.1.2/hammer/pcb/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/pcb/generic/defaults.yml` & `hammer_vlsi-1.1.2/hammer/pcb/generic/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/power/joules/__init__.py` & `hammer_vlsi-1.1.2/hammer/power/joules/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/power/voltus/__init__.py` & `hammer_vlsi-1.1.2/hammer/power/voltus/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/power/voltus/defaults.yml` & `hammer_vlsi-1.1.2/hammer/power/voltus/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/shell/get_config.py` & `hammer_vlsi-1.1.2/hammer/shell/get_config.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/shell/hammer_generate_mdf.py` & `hammer_vlsi-1.1.2/hammer/shell/hammer_generate_mdf.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/shell/readlink_array.py` & `hammer_vlsi-1.1.2/hammer/shell/readlink_array.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/shell/yaml2json.py` & `hammer_vlsi-1.1.2/hammer/shell/yaml2json.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/sim/mocksim/__init__.py` & `hammer_vlsi-1.1.2/hammer/sim/mocksim/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/sim/vcs/__init__.py` & `hammer_vlsi-1.1.2/hammer/sim/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/sim/vcs/defaults.yml` & `hammer_vlsi-1.1.2/hammer/sim/vcs/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/sim/xcelium/__init__.py` & `hammer_vlsi-1.1.2/hammer/sim/xcelium/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/sim/xcelium/defaults.yml` & `hammer_vlsi-1.1.2/hammer/sim/xcelium/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/sim/xcelium/defaults_types.yml` & `hammer_vlsi-1.1.2/hammer/sim/xcelium/defaults_types.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/sram_generator/mocksram_generator/__init__.py` & `hammer_vlsi-1.1.2/hammer/sram_generator/mocksram_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/synthesis/genus/__init__.py` & `hammer_vlsi-1.1.2/hammer/synthesis/genus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,19 @@
         if first_step != self.first_step:
             self.verbose_append("read_db pre_{step}".format(step=first_step.name))
         return True
 
     def do_between_steps(self, prev: HammerToolStep, next: HammerToolStep) -> bool:
         assert super().do_between_steps(prev, next)
         # Write a checkpoint to disk.
-        self.verbose_append("write_db -to_file pre_{step}".format(step=next.name))
+        if self.version() >= self.version_number("221"):
+            # -common now enables database reading in Innovus
+            self.verbose_append("write_db -common -to_file pre_{step}".format(step=next.name))
+        else:
+            self.verbose_append("write_db -to_file pre_{step}".format(step=next.name))
         return True
 
     def do_post_steps(self) -> bool:
         assert super().do_post_steps()
         return self.run_genus()
 
     @property
@@ -193,15 +197,14 @@
 
         # Clock gating setup
         if self.get_setting("synthesis.clock_gating_mode") == "auto":
             verbose_append("set_db lp_clock_gating_infer_enable  true")
             # Innovus will create instances named CLKGATE_foo, CLKGATE_bar, etc.
             verbose_append("set_db lp_clock_gating_prefix  {CLKGATE}")
             verbose_append("set_db lp_insert_clock_gating  true")
-            verbose_append("set_db lp_clock_gating_hierarchical true")
             verbose_append("set_db lp_insert_clock_gating_incremental true")
             verbose_append("set_db lp_clock_gating_register_aware true")
 
         # Set up libraries.
         # Read timing libraries.
         mmmc_path = os.path.join(self.run_dir, "mmmc.tcl")
         self.write_contents_to_path(self.generate_mmmc_script(), mmmc_path)
@@ -353,19 +356,23 @@
         else:
             # TODO: remove hardcoded my_view string
             view_name = "my_view"
         verbose_append("write_sdc -view {view} > {file}".format(view=view_name, file=self.mapped_sdc_path))
 
         verbose_append("write_sdf > {run_dir}/{top}.mapped.sdf".format(run_dir=self.run_dir, top=top))
 
-        # We just get "Cannot trace ILM directory. Data corrupted."
-        # -hierarchical needs to be used for non-leaf modules
-        is_hier = self.hierarchical_mode != HierarchicalMode.Leaf # self.hierarchical_mode != HierarchicalMode.Flat
-        verbose_append("write_design -innovus {hier_flag} -gzip_files {top}".format(
-            hier_flag="-hierarchical" if is_hier else "", top=top))
+        if self.version() >= self.version_number("221"):
+            # New write_design is now meant for non-Cadence tools. write_db -common is now for Innovus-compatible databases.
+            verbose_append("write_design -gzip_files {top}".format(top=top))
+        else:
+            # We just get "Cannot trace ILM directory. Data corrupted."
+            # -hierarchical needs to be used for non-leaf modules
+            is_hier = self.hierarchical_mode != HierarchicalMode.Leaf # self.hierarchical_mode != HierarchicalMode.Flat
+            verbose_append("write_design -innovus {hier_flag} -gzip_files {top}".format(
+                hier_flag="-hierarchical" if is_hier else "", top=top))
 
         self.ran_write_outputs = True
 
         return True
 
     def run_genus(self) -> bool:
         verbose_append = self.verbose_append
```

### Comparing `hammer_vlsi-1.1.1/hammer/synthesis/genus/defaults.yml` & `hammer_vlsi-1.1.2/hammer/synthesis/genus/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/synthesis/mocksynth/__init__.py` & `hammer_vlsi-1.1.2/hammer/synthesis/mocksynth/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/synthesis/vivado/__init__.py` & `hammer_vlsi-1.1.2/hammer/synthesis/vivado/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/synthesis/vivado/defaults.yml` & `hammer_vlsi-1.1.2/hammer/synthesis/vivado/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/init.tcl` & `hammer_vlsi-1.1.2/hammer/synthesis/vivado/file_templates/init.tcl`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/ip.tcl` & `hammer_vlsi-1.1.2/hammer/synthesis/vivado/file_templates/ip.tcl`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/par.tcl` & `hammer_vlsi-1.1.2/hammer/synthesis/vivado/file_templates/par.tcl`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/synthesis/vivado/file_templates/prologue.tcl` & `hammer_vlsi-1.1.2/hammer/synthesis/vivado/file_templates/prologue.tcl`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/synthesis/yosys/__init__.py` & `hammer_vlsi-1.1.2/hammer/synthesis/yosys/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/synthesis/yosys/defaults.yml` & `hammer_vlsi-1.1.2/hammer/synthesis/yosys/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/synthesis/yosys/defaults_types.yml` & `hammer_vlsi-1.1.2/hammer/synthesis/yosys/defaults_types.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/tech/__init__.py` & `hammer_vlsi-1.1.2/hammer/tech/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/tech/specialcells.py` & `hammer_vlsi-1.1.2/hammer/tech/specialcells.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/tech/stackup.py` & `hammer_vlsi-1.1.2/hammer/tech/stackup.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,18 +80,18 @@
     index: The order in the stackup (lower is closer to the substrate).
     direction: The preferred routing direction of this metal layer, or
                RoutingDirection.Redistribution for non-routing top-level
                redistribution metals like Aluminium.
     min_width: The minimum wire width for this layer.
     max_width: The maximum wire width for this layer.
     pitch: The minimum cross-mask pitch for this layer (NOT same-mask pitch
-           for multiple-patterned layers). Width of routing grid for a given layer. 
-           To route denser wires on chip, multiple masks are required. 
-           During fabrication, the masks are applied separately with some spatial offsets 
-           to achieve denser line patterning. For more information on multiple-patterning, 
+           for multiple-patterned layers). Width of routing grid for a given layer.
+           To route denser wires on chip, multiple masks are required.
+           During fabrication, the masks are applied separately with some spatial offsets
+           to achieve denser line patterning. For more information on multiple-patterning,
            check https://en.wikipedia.org/wiki/Multiple_patterning
     offset: The routing track offset from the origin for the first track in this layer.
             (0 = first track is on an axis).
     power_strap_widths_and_spacings: A list of WidthSpacingTuples that specify the minimum
                                      spacing rules for an infinitely long wire of variying width.
     power_strap_width_table: A list of allowed metal widths in the technology.
                              Widths smaller than the last number must be quantized to a value in the table.
@@ -389,15 +389,19 @@
             if m.name == name:
                 return m
         raise ValueError("Metal named %s is not defined in stackup %s" % (name, self.name))
 
     def get_metal_by_index(self, index: int) -> Metal:
         """
         Get a given metal layer by index.
+        If index is given as -1, return the highest metal layer (by index).
 
         :param index: Index of the metal layer
         :return: A metal layer object
         """
-        for m in self.metals:
-            if m.index == index:
-                return m
+        if index == -1:
+            return max(self.metals, key=lambda m: m.index)
+        else:
+            for m in self.metals:
+                if m.index == index:
+                    return m
         raise ValueError("Metal with index %d is not defined in stackup %s" % (index, self.name))
```

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/README.md` & `hammer_vlsi-1.1.2/hammer/technology/asap7/README.md`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/__init__.py` & `hammer_vlsi-1.1.2/hammer/technology/asap7/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,17 +196,14 @@
 def asap7_innovus_settings(ht: HammerTool) -> bool:
     assert isinstance(ht, HammerPlaceAndRouteTool), "Innovus settings only for par"
     assert isinstance(ht, TCLTool), "innovus settings can only run on TCL tools"
     """Settings that may need to be reapplied at every tool invocation
     Note that the particular routing layer settings here will persist in Innovus;
     this hook only serves as an example of what commands may need to persist."""
     ht.append('''
-set_db route_design_bottom_routing_layer 2
-set_db route_design_top_routing_layer 7
-
 # Ignore 1e+31 removal arcs for ASYNC DFF cells
 set_db timing_analysis_async_checks no_async
 
 # Via preferences for stripes
 set_db generate_special_via_rule_preference { M7_M6widePWR1p152 M6_M5widePWR1p152 M5_M4widePWR0p864 M4_M3widePWR0p864 M3_M2widePWR0p936 }
 
 # Prevent extending M1 pins in cells
```

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/asap7.tech.json` & `hammer_vlsi-1.1.2/hammer/technology/asap7/asap7.tech.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/calibre.layerprops` & `hammer_vlsi-1.1.2/hammer/technology/asap7/calibre.layerprops`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/defaults.yml` & `hammer_vlsi-1.1.2/hammer/technology/asap7/defaults.yml`

 * *Files 9% similar despite different names*

```diff
@@ -35,20 +35,21 @@
     placement_site: "asap7sc7p5t" # Set standard cell LEF placement site
 
     bump_block_cut_layer: "V9" # Set the layer that blocks vias under bumps
 
     tap_cell_interval: 50.0 # Set the interval and offset for tap cells
     tap_cell_offset: 10.564 # Set the interval and offset for tap cells
 
+    routing_layers: [2, 7]
+
 
 technology.core:
   stackup: "asap7_3Ma_2Mb_2Mc_2Md" # This key should exist in the stackups list in the tech json
   std_cell_rail_layer: "M1" # This should specify the TOPMOST metal layer the standard cells use for power rails
   # Note that this is not usually stackup specific; it is based on the std cell libraries themselves
-  tap_cell_rail_reference: "{TAPCELL*}" # This is used to provide a reference master for generating standard cells
 
 synthesis.yosys:
   latch_map_file: "latch_map.v"
   latch_map_file_meta: prependlocal
 
 par.inputs:
   gds_merge: true # gds_merge: true is mandatory,
```

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/gds_scale.py` & `hammer_vlsi-1.1.2/hammer/technology/asap7/gds_scale.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/lefdefLayer.map` & `hammer_vlsi-1.1.2/hammer/technology/asap7/lefdefLayer.map`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram-cache-gen.py` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram-cache-gen.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram-cache.json` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram-cache.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/__init__.py` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x16_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x16_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x17_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x17_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x32_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x32_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x37_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x37_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x38_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x38_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x44_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x44_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x64_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x64_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x8_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW1024x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x12_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x12_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x14_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x14_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x22_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x22_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x40_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x40_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x46_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x46_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x48_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x48_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x64_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x64_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x8_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW128x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW2048x8_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW2048x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x128_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x128_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x32_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x32_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x46_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x46_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x48_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x48_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x64_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x64_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x8_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW256x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW32x50_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW32x50_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW4096x16_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW4096x16_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW4096x8_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW4096x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x128_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x128_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x32_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x32_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x64_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x64_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x8_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW512x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x128_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x128_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x20_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x20_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x21_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x21_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x22_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x22_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x32_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x32_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x34_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x34_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x8_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM1RW64x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x16_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x16_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x32_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x32_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x4_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x4_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x8_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW128x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x16_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x16_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x32_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x32_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x4_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x4_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x8_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW16x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x16_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x16_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x22_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x22_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x32_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x32_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x33_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x33_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x39_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x39_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x4_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x4_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x8_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW32x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x16_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x16_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x24_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x24_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x32_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x32_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x4_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x4_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x8_x4.gds` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/gds/SRAM2RW64x8_x4.gds`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x16_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x16_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x17_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x17_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x32_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x32_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x37_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x37_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x38_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x38_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x44_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x44_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x64_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x64_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x8_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW1024x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x12_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x12_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x14_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x14_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x22_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x22_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x40_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x40_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x46_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x46_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x48_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x48_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x64_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x64_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x8_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW128x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW2048x8_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW2048x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x128_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x128_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x32_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x32_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x46_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x46_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x48_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x48_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x64_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x64_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x8_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW256x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW32x50_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW32x50_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW4096x16_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW4096x16_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW4096x8_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW4096x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x128_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x128_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x32_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x32_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x64_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x64_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x8_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW512x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x128_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x128_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x20_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x20_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x21_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x21_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x22_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x22_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x32_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x32_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x34_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x34_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x8_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM1RW64x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x16_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x16_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x32_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x32_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x4_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x4_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x8_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW128x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x16_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x16_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x32_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x32_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x4_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x4_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x8_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW16x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x16_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x16_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x22_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x22_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x32_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x32_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x33_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x33_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x39_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x39_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x4_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x4_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x8_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW32x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x16_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x16_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x24_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x24_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x32_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x32_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x4_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x4_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x8_x4.lef` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lef/SRAM2RW64x8_x4.lef`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x16_lib/SRAM1RW1024x16_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x16_lib/SRAM1RW1024x16_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x16_lib/SRAM1RW1024x16_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x16_lib/SRAM1RW1024x16_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x17_lib/SRAM1RW1024x17_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x17_lib/SRAM1RW1024x17_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x17_lib/SRAM1RW1024x17_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x17_lib/SRAM1RW1024x17_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x32_lib/SRAM1RW1024x32_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x32_lib/SRAM1RW1024x32_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x32_lib/SRAM1RW1024x32_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x32_lib/SRAM1RW1024x32_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x37_lib/SRAM1RW1024x37_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x37_lib/SRAM1RW1024x37_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x37_lib/SRAM1RW1024x37_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x37_lib/SRAM1RW1024x37_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x38_lib/SRAM1RW1024x38_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x38_lib/SRAM1RW1024x38_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x38_lib/SRAM1RW1024x38_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x38_lib/SRAM1RW1024x38_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x44_lib/SRAM1RW1024x44_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x44_lib/SRAM1RW1024x44_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x44_lib/SRAM1RW1024x44_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x44_lib/SRAM1RW1024x44_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x64_lib/SRAM1RW1024x64_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x64_lib/SRAM1RW1024x64_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x64_lib/SRAM1RW1024x64_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x64_lib/SRAM1RW1024x64_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x8_lib/SRAM1RW1024x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x8_lib/SRAM1RW1024x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x8_lib/SRAM1RW1024x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW1024x8_lib/SRAM1RW1024x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x12_lib/SRAM1RW128x12_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x12_lib/SRAM1RW128x12_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x12_lib/SRAM1RW128x12_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x12_lib/SRAM1RW128x12_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x14_lib/SRAM1RW128x14_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x14_lib/SRAM1RW128x14_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x14_lib/SRAM1RW128x14_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x14_lib/SRAM1RW128x14_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x22_lib/SRAM1RW128x22_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x22_lib/SRAM1RW128x22_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x22_lib/SRAM1RW128x22_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x22_lib/SRAM1RW128x22_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x40_lib/SRAM1RW128x40_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x40_lib/SRAM1RW128x40_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x40_lib/SRAM1RW128x40_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x40_lib/SRAM1RW128x40_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x46_lib/SRAM1RW128x46_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x46_lib/SRAM1RW128x46_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x46_lib/SRAM1RW128x46_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x46_lib/SRAM1RW128x46_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x48_lib/SRAM1RW128x48_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x48_lib/SRAM1RW128x48_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x48_lib/SRAM1RW128x48_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x48_lib/SRAM1RW128x48_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x64_lib/SRAM1RW128x64_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x64_lib/SRAM1RW128x64_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x64_lib/SRAM1RW128x64_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x64_lib/SRAM1RW128x64_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x8_lib/SRAM1RW128x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x8_lib/SRAM1RW128x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x8_lib/SRAM1RW128x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW128x8_lib/SRAM1RW128x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW2048x8_lib/SRAM1RW2048x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW2048x8_lib/SRAM1RW2048x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW2048x8_lib/SRAM1RW2048x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW2048x8_lib/SRAM1RW2048x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x128_lib/SRAM1RW256x128_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x128_lib/SRAM1RW256x128_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x128_lib/SRAM1RW256x128_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x128_lib/SRAM1RW256x128_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x32_lib/SRAM1RW256x32_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x32_lib/SRAM1RW256x32_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x32_lib/SRAM1RW256x32_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x32_lib/SRAM1RW256x32_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x46_lib/SRAM1RW256x46_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x46_lib/SRAM1RW256x46_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x46_lib/SRAM1RW256x46_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x46_lib/SRAM1RW256x46_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x48_lib/SRAM1RW256x48_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x48_lib/SRAM1RW256x48_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x48_lib/SRAM1RW256x48_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x48_lib/SRAM1RW256x48_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x64_lib/SRAM1RW256x64_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x64_lib/SRAM1RW256x64_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x64_lib/SRAM1RW256x64_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x64_lib/SRAM1RW256x64_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x8_lib/SRAM1RW256x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x8_lib/SRAM1RW256x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x8_lib/SRAM1RW256x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW256x8_lib/SRAM1RW256x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW32x50_lib/SRAM1RW32x50_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW32x50_lib/SRAM1RW32x50_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW32x50_lib/SRAM1RW32x50_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW32x50_lib/SRAM1RW32x50_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x16_lib/SRAM1RW4096x16_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x16_lib/SRAM1RW4096x16_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x16_lib/SRAM1RW4096x16_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x16_lib/SRAM1RW4096x16_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x8_lib/SRAM1RW4096x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x8_lib/SRAM1RW4096x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x8_lib/SRAM1RW4096x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW4096x8_lib/SRAM1RW4096x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x128_lib/SRAM1RW512x128_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x128_lib/SRAM1RW512x128_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x128_lib/SRAM1RW512x128_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x128_lib/SRAM1RW512x128_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x32_lib/SRAM1RW512x32_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x32_lib/SRAM1RW512x32_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x32_lib/SRAM1RW512x32_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x32_lib/SRAM1RW512x32_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x64_lib/SRAM1RW512x64_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x64_lib/SRAM1RW512x64_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x64_lib/SRAM1RW512x64_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x64_lib/SRAM1RW512x64_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x8_lib/SRAM1RW512x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x8_lib/SRAM1RW512x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x8_lib/SRAM1RW512x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW512x8_lib/SRAM1RW512x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x128_lib/SRAM1RW64x128_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x128_lib/SRAM1RW64x128_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x128_lib/SRAM1RW64x128_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x128_lib/SRAM1RW64x128_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x20_lib/SRAM1RW64x20_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x20_lib/SRAM1RW64x20_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x20_lib/SRAM1RW64x20_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x20_lib/SRAM1RW64x20_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x21_lib/SRAM1RW64x21_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x21_lib/SRAM1RW64x21_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x21_lib/SRAM1RW64x21_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x21_lib/SRAM1RW64x21_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x22_lib/SRAM1RW64x22_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x22_lib/SRAM1RW64x22_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x22_lib/SRAM1RW64x22_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x22_lib/SRAM1RW64x22_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x32_lib/SRAM1RW64x32_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x32_lib/SRAM1RW64x32_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x32_lib/SRAM1RW64x32_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x32_lib/SRAM1RW64x32_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x34_lib/SRAM1RW64x34_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x34_lib/SRAM1RW64x34_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x34_lib/SRAM1RW64x34_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x34_lib/SRAM1RW64x34_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x8_lib/SRAM1RW64x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x8_lib/SRAM1RW64x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x8_lib/SRAM1RW64x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM1RW64x8_lib/SRAM1RW64x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x16_lib/SRAM2RW128x16_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x16_lib/SRAM2RW128x16_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x16_lib/SRAM2RW128x16_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x16_lib/SRAM2RW128x16_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x32_lib/SRAM2RW128x32_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x32_lib/SRAM2RW128x32_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x32_lib/SRAM2RW128x32_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x32_lib/SRAM2RW128x32_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x4_lib/SRAM2RW128x4_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x4_lib/SRAM2RW128x4_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x4_lib/SRAM2RW128x4_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x4_lib/SRAM2RW128x4_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x8_lib/SRAM2RW128x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x8_lib/SRAM2RW128x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x8_lib/SRAM2RW128x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW128x8_lib/SRAM2RW128x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x16_lib/SRAM2RW16x16_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x16_lib/SRAM2RW16x16_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x16_lib/SRAM2RW16x16_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x16_lib/SRAM2RW16x16_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x32_lib/SRAM2RW16x32_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x32_lib/SRAM2RW16x32_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x32_lib/SRAM2RW16x32_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x32_lib/SRAM2RW16x32_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x4_lib/SRAM2RW16x4_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x4_lib/SRAM2RW16x4_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x4_lib/SRAM2RW16x4_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x4_lib/SRAM2RW16x4_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x8_lib/SRAM2RW16x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x8_lib/SRAM2RW16x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x8_lib/SRAM2RW16x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW16x8_lib/SRAM2RW16x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x16_lib/SRAM2RW32x16_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x16_lib/SRAM2RW32x16_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x16_lib/SRAM2RW32x16_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x16_lib/SRAM2RW32x16_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x22_lib/SRAM2RW32x22_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x22_lib/SRAM2RW32x22_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x22_lib/SRAM2RW32x22_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x22_lib/SRAM2RW32x22_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x32_lib/SRAM2RW32x32_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x32_lib/SRAM2RW32x32_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x32_lib/SRAM2RW32x32_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x32_lib/SRAM2RW32x32_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x33_lib/SRAM2RW32x33_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x33_lib/SRAM2RW32x33_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x33_lib/SRAM2RW32x33_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x33_lib/SRAM2RW32x33_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x39_lib/SRAM2RW32x39_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x39_lib/SRAM2RW32x39_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x39_lib/SRAM2RW32x39_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x39_lib/SRAM2RW32x39_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x4_lib/SRAM2RW32x4_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x4_lib/SRAM2RW32x4_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x4_lib/SRAM2RW32x4_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x4_lib/SRAM2RW32x4_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x8_lib/SRAM2RW32x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x8_lib/SRAM2RW32x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x8_lib/SRAM2RW32x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW32x8_lib/SRAM2RW32x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x16_lib/SRAM2RW64x16_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x16_lib/SRAM2RW64x16_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x16_lib/SRAM2RW64x16_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x16_lib/SRAM2RW64x16_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x24_lib/SRAM2RW64x24_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x24_lib/SRAM2RW64x24_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x24_lib/SRAM2RW64x24_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x24_lib/SRAM2RW64x24_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x32_lib/SRAM2RW64x32_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x32_lib/SRAM2RW64x32_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x32_lib/SRAM2RW64x32_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x32_lib/SRAM2RW64x32_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x4_lib/SRAM2RW64x4_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x4_lib/SRAM2RW64x4_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x4_lib/SRAM2RW64x4_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x4_lib/SRAM2RW64x4_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x8_lib/SRAM2RW64x8_PVT_0P63V_100C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x8_lib/SRAM2RW64x8_PVT_0P63V_100C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x8_lib/SRAM2RW64x8_PVT_0P77V_0C.lib` & `hammer_vlsi-1.1.2/hammer/technology/asap7/sram_compiler/memories/lib/SRAM2RW64x8_lib/SRAM2RW64x8_PVT_0P77V_0C.lib`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/asap7/srams.txt` & `hammer_vlsi-1.1.2/hammer/technology/asap7/srams.txt`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/nangate45/README.md` & `hammer_vlsi-1.1.2/hammer/technology/nangate45/README.md`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/nangate45/defaults.yml` & `hammer_vlsi-1.1.2/hammer/technology/nangate45/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/nangate45/nangate45.tech.json` & `hammer_vlsi-1.1.2/hammer/technology/nangate45/nangate45.tech.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/nangate45/sram-cache.json` & `hammer_vlsi-1.1.2/hammer/technology/nangate45/sram-cache.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/nangate45/sram_compiler/__init__.py` & `hammer_vlsi-1.1.2/hammer/technology/nangate45/sram_compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/sky130/__init__.py` & `hammer_vlsi-1.1.2/hammer/technology/sky130/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from pathlib import Path
 from typing import NamedTuple, List, Optional, Tuple, Dict, Set, Any
 import importlib
 import json
 
 import hammer.tech
 from hammer.tech import HammerTechnology
-from hammer.vlsi import HammerTool, HammerPlaceAndRouteTool, TCLTool, HammerDRCTool, HammerLVSTool, HammerToolHookAction
+from hammer.vlsi import HammerTool, HammerPlaceAndRouteTool, TCLTool, HammerDRCTool, HammerLVSTool, \
+    HammerToolHookAction, HierarchicalMode
 
 import hammer.tech.specialcells as specialcells
 from hammer.tech.specialcells import CellType, SpecialCell
 
 class SKY130Tech(HammerTechnology):
     """
     Override the HammerTechnology used in `hammer_tech.py`
@@ -27,36 +28,50 @@
         # check whether variables were overriden to point to a valid path
         self.use_nda_files = os.path.exists(self.get_setting("technology.sky130.sky130_nda"))
         self.use_sram22 = os.path.exists(self.get_setting("technology.sky130.sram22_sky130_macros"))
         self.setup_cdl()
         self.setup_verilog()
         self.setup_techlef()
         self.setup_lvs_deck()
+        self.setup_io_lefs()
         print('Loaded Sky130 Tech')
 
 
-    # Copy and hack the cdl, replacing pfet_01v8_hvt/nfet_01v8 with phighvt/nshort
     def setup_cdl(self) -> None:
+        ''' Copy and hack the cdl, replacing pfet_01v8_hvt/nfet_01v8 with
+            respective names in LVS deck
+        '''
         setting_dir = self.get_setting("technology.sky130.sky130A")
         setting_dir = Path(setting_dir)
         source_path = setting_dir / 'libs.ref' / self.library_name / 'cdl' / f'{self.library_name}.cdl'
         if not source_path.exists():
             raise FileNotFoundError(f"CDL not found: {source_path}")
 
         cache_tech_dir_path = Path(self.cache_dir)
         os.makedirs(cache_tech_dir_path, exist_ok=True)
         dest_path = cache_tech_dir_path / f'{self.library_name}.cdl'
 
+        # device names expected in LVS decks
+        if (self.get_setting('vlsi.core.lvs_tool') == "hammer.lvs.calibre"):
+            pmos = 'phighvt'
+            nmos = 'nshort'
+        elif (self.get_setting('vlsi.core.lvs_tool') == "hammer.lvs.netgen"):
+            pmos = 'sky130_fd_pr__pfet_01v8_hvt'
+            nmos = 'sky130_fd_pr__nfet_01v8'
+        else:
+            shutil.copy2(source_path, dest_path)
+            return
+
         with open(source_path, 'r') as sf:
             with open(dest_path, 'w') as df:
                 self.logger.info("Modifying CDL netlist: {} -> {}".format
                     (source_path, dest_path))
                 for line in sf:
-                    line = line.replace('pfet_01v8_hvt', 'phighvt')
-                    line = line.replace('nfet_01v8'    , 'nshort')
+                    line = line.replace('pfet_01v8_hvt', pmos)
+                    line = line.replace('nfet_01v8'    , nmos)
                     df.write(line)
 
     # Copy and hack the verilog
     #   - <library_name>.v: remove 'wire 1' and one endif line to fix syntax errors
     #   - primitives.v: set default nettype to 'wire' instead of 'none'
     #           (the open-source RTL sim tools don't treat undeclared signals as errors)
     def setup_verilog(self) -> None:
@@ -143,14 +158,49 @@
             with open(source_path, 'r') as sf:
                 with open(dest_path, 'w') as df:
                     self.logger.info("Modifying LVS deck: {} -> {}".format
                         (source_path, dest_path))
                     df.write(matcher.sub("", sf.read()))
                     df.write(LVS_DECK_INSERT_LINES)
 
+    # Power pins for clamps must be CLASS CORE
+    # connect/disconnect spacers must be CLASS PAD SPACER, not AREAIO
+    def setup_io_lefs(self) -> None:
+        sky130A_path = Path(self.get_setting('technology.sky130.sky130A'))
+        source_path = sky130A_path / 'libs.ref' / 'sky130_fd_io' / 'lef' / 'sky130_ef_io.lef'
+        if not source_path.exists():
+            raise FileNotFoundError(f"IO LEF not found: {source_path}")
+
+        cache_tech_dir_path = Path(self.cache_dir)
+        os.makedirs(cache_tech_dir_path, exist_ok=True)
+        dest_path = cache_tech_dir_path / 'sky130_ef_io.lef'
+
+        with open(source_path, 'r') as sf:
+            with open(dest_path, 'w') as df:
+                self.logger.info("Modifying IO LEF: {} -> {}".format
+                    (source_path, dest_path))
+                sl = sf.readlines()
+                for net in ['VCCD1', 'VSSD1']:
+                    start = [idx for idx,line in enumerate(sl) if 'PIN ' + net in line]
+                    end = [idx for idx,line in enumerate(sl) if 'END ' + net in line]
+                    intervals = zip(start, end)
+                    for intv in intervals:
+                        port_idx = [idx for idx,line in enumerate(sl[intv[0]:intv[1]]) if 'PORT' in line]
+                        for idx in port_idx:
+                            sl[intv[0]+idx]=sl[intv[0]+idx].replace('PORT', 'PORT\n      CLASS CORE ;')
+                for cell in [
+                    'sky130_ef_io__connect_vcchib_vccd_and_vswitch_vddio_slice_20um',
+                    'sky130_ef_io__disconnect_vccd_slice_5um',
+                    'sky130_ef_io__disconnect_vdda_slice_5um',
+                ]:
+                    # force class to spacer
+                    start = [idx for idx, line in enumerate(sl) if f'MACRO {cell}' in line]
+                    sl[start[0] + 1] = sl[start[0] + 1].replace('AREAIO', 'SPACER')
+                df.writelines(sl)
+
     def get_tech_par_hooks(self, tool_name: str) -> List[HammerToolHookAction]:
         hooks = {
             "innovus": [
             HammerTool.make_post_insertion_hook("init_design",      sky130_innovus_settings),
             HammerTool.make_pre_insertion_hook("place_tap_cells",   sky130_add_endcaps),
             HammerTool.make_pre_insertion_hook("power_straps",      sky130_connect_nets),
             HammerTool.make_pre_insertion_hook("write_design",      sky130_connect_nets2)
@@ -179,15 +229,15 @@
     def openram_sram_names() -> List[str]:
         """ Return a list of cell-names of the OpenRAM SRAMs (that we'll use). """
         return [
             "sky130_sram_1kbyte_1rw1r_32x256_8",
             "sky130_sram_1kbyte_1rw1r_8x1024_8",
             "sky130_sram_2kbyte_1rw1r_32x512_8"
         ]
-    
+
     @staticmethod
     def sky130_sram_names() -> List[str]:
         sky130_sram_names = []
         sram_cache_json = importlib.resources.files("hammer.technology.sky130").joinpath("sram-cache.json").read_text()
         dl = json.loads(sram_cache_json)
         for d in dl:
             sky130_sram_names.append(d['name'])
@@ -258,25 +308,31 @@
 
 ##########################################################
 # Routing attributes  [get_db -category route]
 ##########################################################
 #-------------------------------------------------------------------------------
 set_db route_design_antenna_diode_insertion 1
 set_db route_design_antenna_cell_name "sky130_fd_sc_hd__diode_2"
-set_db route_design_bottom_routing_layer 2
 
 set_db route_design_high_freq_search_repair true
 set_db route_design_detail_post_route_spread_wire true
 set_db route_design_with_si_driven true
 set_db route_design_with_timing_driven true
 set_db route_design_concurrent_minimize_via_count_effort high
 set_db opt_consider_routing_congestion true
 set_db route_design_detail_use_multi_cut_via_effort medium
     '''
     )
+    if ht.hierarchical_mode in {HierarchicalMode.Top, HierarchicalMode.Flat}:
+        ht.append(
+            '''
+# For top module: snap die to manufacturing grid, not placement grid
+set_db floorplan_snap_die_grid manufacturing
+        '''
+        )
     return True
 
 def sky130_connect_nets(ht: HammerTool) -> bool:
     assert isinstance(ht, HammerPlaceAndRouteTool), "connect global nets only for par"
     assert isinstance(ht, TCLTool), "connect global nets can only run on TCL tools"
     for pwr_gnd_net in (ht.get_all_power_nets() + ht.get_all_ground_nets()):
             if pwr_gnd_net.tie is not None:
@@ -303,14 +359,57 @@
 set_db add_endcaps_left_edge        {endcap_cell}
 set_db add_endcaps_right_edge       {endcap_cell}
 add_endcaps
     '''
     )
     return True
 
+def efabless_ring_io(ht: HammerTool) -> bool:
+    assert isinstance(ht, HammerPlaceAndRouteTool), "IO ring instantiation only for par"
+    assert isinstance(ht, TCLTool), "IO ring instantiation can only run on TCL tools"
+    io_file = ht.get_setting("technology.sky130.io_file")
+    ht.append(f"read_io_file {io_file} -no_die_size_adjust")
+    p_nets = list(map(lambda s: s.name, ht.get_independent_power_nets()))
+    g_nets = list(map(lambda s: s.name, ht.get_independent_ground_nets()))
+    ht.append(f'''
+# Global net connections
+connect_global_net VDDA -type pg_pin -pin_base_name VDDA -verbose
+connect_global_net VDDIO -type pg_pin -pin_base_name VDDIO* -verbose
+connect_global_net {p_nets[0]} -type pg_pin -pin_base_name VCCD* -verbose
+connect_global_net {p_nets[0]} -type pg_pin -pin_base_name VCCHIB -verbose
+connect_global_net {p_nets[0]} -type pg_pin -pin_base_name VSWITCH -verbose
+connect_global_net {g_nets[0]} -type pg_pin -pin_base_name VSSA -verbose
+connect_global_net {g_nets[0]} -type pg_pin -pin_base_name VSSIO* -verbose
+connect_global_net {g_nets[0]} -type pg_pin -pin_base_name VSSD* -verbose
+    ''')
+    ht.append('''
+# IO fillers
+set io_fillers {sky130_ef_io__connect_vcchib_vccd_and_vswitch_vddio_slice_20um sky130_ef_io__com_bus_slice_10um sky130_ef_io__com_bus_slice_5um sky130_ef_io__com_bus_slice_1um}
+add_io_fillers -prefix IO_FILLER -io_ring 1 -cells $io_fillers -side top -filler_orient r0
+add_io_fillers -prefix IO_FILLER -io_ring 1 -cells $io_fillers -side right -filler_orient r270
+add_io_fillers -prefix IO_FILLER -io_ring 1 -cells $io_fillers -side bottom -filler_orient r180
+add_io_fillers -prefix IO_FILLER -io_ring 1 -cells $io_fillers -side left -filler_orient r90
+# Fix placement
+set io_filler_insts [get_db insts IO_FILLER_*]
+set_db $io_filler_insts .place_status fixed
+    ''')
+    # An offset of 40um is used to place the core ring inside the core area. It
+    # can be decreased down to 5um as desired, but will require additional
+    # routing / settings to connect the core power stripes to the ring.
+    ht.append(f'''
+# Core ring
+add_rings -follow io -layer met5 -nets {{ {p_nets[0]} {g_nets[0]} }} -offset 40 -width 13 -spacing 3
+route_special -connect pad_pin -nets {{ {p_nets[0]} {g_nets[0]} }} -detailed_log
+    ''')
+    ht.append('''
+# Prevent buffering on TIE_LO_ESD and TIE_HI_ESD
+set_dont_touch [get_db [get_db pins -if {.name == *TIE*ESD}] .net]
+    ''')
+    return True
+
 def drc_blackbox_srams(ht: HammerTool) -> bool:
     assert isinstance(ht, HammerDRCTool), "Exlude SRAMs only in DRC"
     drc_box = ''
     for name in SKY130Tech.sky130_sram_names():
         drc_box += f"\nEXCLUDE CELL {name}"
     run_file = ht.drc_run_file  # type: ignore
     with open(run_file, "a") as f:
```

### Comparing `hammer_vlsi-1.1.1/hammer/technology/sky130/defaults.yml` & `hammer_vlsi-1.1.2/hammer/technology/sky130/defaults.yml`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,17 @@
   pdk_home_meta: lazysubst
   lvs_deck_sources: 
     - "${technology.sky130.pdk_home}/LVS/Calibre/lvsControlFile_s8"
   lvs_deck_sources_meta: lazysubst
 
   drc_blackbox_srams: false
   lvs_blackbox_srams: false
+
+  io_file: "extra/efabless_template.io"  # IO ring - take this template and modify for your own use
+  io_file_meta: prependlocal
   
 
 mentor.extra_env_vars_meta: lazydeepsubst # Mentor environment variables
 # Override this in project
 mentor.extra_env_vars:
   - PDK_HOME: "${technology.sky130.sky130_nda}/s8/V2.0.1"
 
@@ -82,19 +85,20 @@
     placement_site: "unithd" # Set standard cell LEF placement site
 
     bump_block_cut_layer: "via4" # Set the layer that blocks vias under bumps
 
     tap_cell_interval: 15.0 # Set the interval and offset for tap cells
     tap_cell_offset: 5.0
 
+    routing_layers: [2, 6]
+
 technology.core:
   stackup: "sky130_fd_sc_hd" # This key should exist in the stackups list in the tech json
   std_cell_rail_layer: "met1" # This should specify the TOPMOST metal layer the standard cells use for power rails
   # Note that this is not usually stackup specific; it is based on the std cell libraries themselves
-  tap_cell_rail_reference: "sky130_fd_sc_hd__tap*" # This is used to provide a reference master for generating standard cells
   std_cell_supplies: 
   # default power pins are VDD/VSS
     power:  ["VPWR"]
     ground: ["VGND"]
   
 synthesis.yosys:
   latch_map_file: "${technology.sky130.sky130A}/libs.tech/openlane/sky130_fd_sc_hd/latch_map.v"
@@ -102,28 +106,32 @@
 
 par.inputs:
   gds_merge: true
   gds_map_mode: manual
   gds_map_file: "extra/sky130_lefpin.map"
   gds_map_file_meta: prependlocal
 
-par.openroad:
+par.openroad:  # openroad setup/files
   setrc_file: "extra/setRC.tcl"
   setrc_file_meta: prependlocal
   openrcx_techfiles: 
     - "${technology.sky130.sky130A}/libs.tech/openlane/rules.openrcx.sky130A.max.spef_extractor"
     - "${technology.sky130.sky130A}/libs.tech/openlane/rules.openrcx.sky130A.min.spef_extractor"
     - "${technology.sky130.sky130A}/libs.tech/openlane/rules.openrcx.sky130A.nom.spef_extractor"
   openrcx_techfiles_meta: lazysubst
   klayout_techfile_source: "${technology.sky130.sky130A}/libs.tech/klayout/tech/sky130A.lyt"
   klayout_techfile_source_meta: lazysubst
   macro_placement:
     halo: [40, 40]
     orient_all: r90  # required for Sram22
 
+drc.klayout:  # klayout files
+  layout_properties_file: "${technology.sky130.sky130A}/libs.tech/klayout/tech/sky130A.lyp"
+  layout_properties_file_meta: lazysubst
+
 par.power_straps_mode: generate # Power Straps
 par.generate_power_straps_method: by_tracks
 par.blockage_spacing: 2.0
 par.blockage_spacing_top_layer: met4
 par.generate_power_straps_options:
   by_tracks:
     strap_layers:
```

### Comparing `hammer_vlsi-1.1.1/hammer/technology/sky130/defaults_types.yml` & `hammer_vlsi-1.1.2/hammer/technology/sky130/defaults_types.yml`

 * *Files 12% similar despite different names*

```diff
@@ -16,7 +16,10 @@
   openram_lib: str
   # DFFRAM currently not supported
   dffram_lib:  Optional[str]
 
   # Shouldn't need to change these
   pdk_home: Optional[str]
   lvs_deck_sources: Optional[list[str]]
+
+  # Path to IO file
+  io_file: str
```

### Comparing `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/cells-gen.py` & `hammer_vlsi-1.1.2/hammer/technology/sky130/extra/cells-gen.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/cells.txt` & `hammer_vlsi-1.1.2/hammer/technology/sky130/extra/cells.txt`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/fill.json` & `hammer_vlsi-1.1.2/hammer/technology/sky130/extra/fill.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/openram/sram-cache-gen.py` & `hammer_vlsi-1.1.2/hammer/technology/sky130/extra/openram/sram-cache-gen.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/openram/sram-cache.json` & `hammer_vlsi-1.1.2/hammer/technology/sky130/extra/openram/sram-cache.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/setRC.tcl` & `hammer_vlsi-1.1.2/hammer/technology/sky130/extra/setRC.tcl`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen-files/beginning_nda.json` & `hammer_vlsi-1.1.2/hammer/technology/sky130/extra/sky130-tech-gen-files/beginning_nda.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9645833333333332%*

 * *Differences: {"'drc_decks'": "{0: {'deck_name': 'calibre_drc'}, insert: [(1, OrderedDict([('tool_name', "*

 * *                "'klayout'), ('deck_name', 'klayout_drc'), ('path', "*

 * *                "'$SKY130A/libs.tech/klayout/drc/sky130A.lydrc')]))]}",*

 * * "'lvs_decks'": "{0: {'deck_name': 'calibre_lvs'}}"}*

```diff
@@ -1,15 +1,20 @@
 {
     "additional_drc_text": "",
     "additional_lvs_text": "",
     "drc_decks": [
         {
-            "deck_name": "all_drc",
+            "deck_name": "calibre_drc",
             "path": "$SKY130_NDA/s8/V2.0.1/DRC/Calibre/s8_drcRules",
             "tool_name": "calibre"
+        },
+        {
+            "deck_name": "klayout_drc",
+            "path": "$SKY130A/libs.tech/klayout/drc/sky130A.lydrc",
+            "tool_name": "klayout"
         }
     ],
     "grid_unit": "0.001",
     "installs": [
         {
             "id": "$SKY130_NDA",
             "path": "technology.sky130.sky130_nda"
@@ -29,15 +34,15 @@
                 }
             ],
             "verilog_sim": "cache/primitives.v"
         }
     ],
     "lvs_decks": [
         {
-            "deck_name": "all_lvs",
+            "deck_name": "calibre_lvs",
             "old_path": "$SKY130_NDA/s8/V2.0.1/LVS/Calibre/lvsRules_s8",
             "path": "cache/lvsControlFile_s8",
             "tool_name": "calibre"
         }
     ],
     "name": "Skywater 130nm Library",
     "time_unit": "1 ns"
```

### Comparing `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen-files/cells.json` & `hammer_vlsi-1.1.2/hammer/technology/sky130/extra/sky130-tech-gen-files/cells.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen-files/stackups-gen.py` & `hammer_vlsi-1.1.2/hammer/technology/sky130/extra/sky130-tech-gen-files/stackups-gen.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130-tech-gen-files/stackups.json` & `hammer_vlsi-1.1.2/hammer/technology/sky130/extra/sky130-tech-gen-files/stackups.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sky130_lefpin.map` & `hammer_vlsi-1.1.2/hammer/technology/sky130/extra/sky130_lefpin.map`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sram22/sram-cache-gen.py` & `hammer_vlsi-1.1.2/hammer/technology/sky130/extra/sram22/sram-cache-gen.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/sky130/extra/sram22/sram-cache.json` & `hammer_vlsi-1.1.2/hammer/technology/sky130/extra/sram22/sram-cache.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/sky130/sram-cache.json` & `hammer_vlsi-1.1.2/hammer/technology/sky130/sram-cache.json`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/technology/sky130/sram_compiler/__init__.py` & `hammer_vlsi-1.1.2/hammer/technology/sky130/sram_compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/timing/tempus/__init__.py` & `hammer_vlsi-1.1.2/hammer/timing/tempus/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/timing/tempus/defaults.yml` & `hammer_vlsi-1.1.2/hammer/timing/tempus/defaults.yml`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/utils/__init__.py` & `hammer_vlsi-1.1.2/hammer/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/utils/lef_utils.py` & `hammer_vlsi-1.1.2/hammer/utils/lef_utils.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/utils/verilog_utils.py` & `hammer_vlsi-1.1.2/hammer/utils/verilog_utils.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/vlsi/cli_driver.py` & `hammer_vlsi-1.1.2/hammer/vlsi/cli_driver.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/vlsi/constraints.py` & `hammer_vlsi-1.1.2/hammer/vlsi/constraints.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/vlsi/driver.py` & `hammer_vlsi-1.1.2/hammer/vlsi/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -418,15 +418,14 @@
         lvs_tool.submit_command = HammerSubmitCommand.get("lvs", self.database)
         lvs_tool.run_dir = run_dir
 
         lvs_tool.schematic_files = self.database.get_setting("lvs.inputs.schematic_files", nullvalue=[])
         lvs_tool.layout_file = self.database.get_setting("lvs.inputs.layout_file", nullvalue="")
         lvs_tool.top_module = self.database.get_setting("lvs.inputs.top_module", nullvalue="")
         lvs_tool.hcells_list = self.database.get_setting("lvs.inputs.hcells_list", nullvalue=[])
-        lvs_tool.ilms = list(map(lambda x: ILMStruct.from_setting(x), self.database.get_setting("lvs.inputs.ilms", nullvalue=[])))
         missing_inputs = False
         if lvs_tool.top_module == "":
             self.log.error("Top module not specified for LVS")
             missing_inputs = True
         if lvs_tool.layout_file is None:
             self.log.error("No layout file specified for LVS")
             missing_inputs = True
@@ -1169,15 +1168,14 @@
             input_files = deeplist([output_dict["par.outputs.output_netlist"]])
             result = {
                 "timing.inputs.input_files": input_files,
                 "timing.inputs.input_files_meta": "append",
                 "timing.inputs.top_module": output_dict["par.inputs.top_module"],
                 "timing.inputs.spefs": output_dict["par.outputs.spefs"],
                 "timing.inputs.sdf_file": output_dict["par.outputs.sdf_file"],
-                "timing.inputs.ilms": output_dict["par.outputs.output_ilms"],
                 "vlsi.builtins.is_complete": False
             }  # type: Dict[str, Any]
             return result
         except KeyError:
             # KeyError means that the given dictionary is missing output keys.
             return None
 
@@ -1234,15 +1232,15 @@
         Does not merge the results with any project dictionaries.
         :param output_dict: Dict containing par.outputs.*
         :return: vlsi.inputs.* settings generated from output_dict,
                  or None if output_dict was invalid
         """
         try:
             result = {
-                "vlsi.inputs.ilms": output_dict["par.outputs.output_ilms"],
+                "vlsi.inputs.ilms": output_dict["vlsi.inputs.ilms"] + output_dict["par.outputs.output_ilms"],
                 "vlsi.builtins.is_complete": False
             }  # type: Dict[str, Any]
             return result
         except KeyError:
             # KeyError means that the given dictionary is missing output keys.
             return None
 
@@ -1278,15 +1276,14 @@
                  or None if output_dict was invalid
         """
         try:
             result = {
                 "lvs.inputs.top_module": output_dict["par.inputs.top_module"],
                 "lvs.inputs.layout_file": output_dict["par.outputs.output_gds"],
                 "lvs.inputs.schematic_files": [output_dict["par.outputs.output_netlist"]],
-                "lvs.inputs.ilms": output_dict["par.outputs.output_ilms"],
                 "lvs.inputs.hcells_list": output_dict["par.outputs.hcells_list"],
                 "vlsi.builtins.is_complete": False
             }  # type: Dict[str, Any]
             return result
         except KeyError:
             # KeyError means that the given dictionary is missing output keys.
             return None
@@ -1806,11 +1803,11 @@
             output.append((module, constraint_dict))
 
         return (output, dependency_graph)
 
     @property
     def dump_history(self) -> bool:
         return self._dump_history
-    
+
     @dump_history.setter
     def dump_history(self, new_dump_history: bool) -> None:
         self._dump_history = new_dump_history
```

### Comparing `hammer_vlsi-1.1.1/hammer/vlsi/hammer_build_systems.py` & `hammer_vlsi-1.1.2/hammer/vlsi/hammer_build_systems.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,15 @@
         redo-sim-syn-to-power{suffix}:
         \t$(HAMMER_EXEC) {env_confs} -p {sim_syn_out} $(HAMMER_EXTRA_ARGS) -o {power_sim_syn_in} --obj_dir {obj_dir} sim-to-power
 
         redo-syn-to-par{suffix}:
         \t$(HAMMER_EXEC) {env_confs} -p {syn_out} $(HAMMER_EXTRA_ARGS) -o {par_in} --obj_dir {obj_dir} syn-to-par
 
         redo-power-syn{suffix}:
-        \t$(HAMMER_EXEC) {env_confs} -p {power_sim_syn_in} $(HAMMER_EXTRA_ARGS) --power_rundir {power_syn_run_dir} --obj_dir {obj_dir} power{suffix}
+        \t$(HAMMER_EXEC) {env_confs} -p {power_sim_syn_in} -p {power_syn_in} $(HAMMER_EXTRA_ARGS) --power_rundir {power_syn_run_dir} --obj_dir {obj_dir} power{suffix}
 
         redo-par{suffix}:
         \t$(HAMMER_EXEC) {env_confs} -p {par_in} $(HAMMER_EXTRA_ARGS) --obj_dir {obj_dir} par{suffix}
 
         redo-par-to-sim{suffix}:
         \t$(HAMMER_EXEC) {env_confs} -p {par_out} $(HAMMER_EXTRA_ARGS) -o {sim_par_in} --obj_dir {obj_dir} par-to-sim
```

### Comparing `hammer_vlsi-1.1.1/hammer/vlsi/hammer_tool.py` & `hammer_vlsi-1.1.2/hammer/vlsi/hammer_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1103,15 +1103,15 @@
         return self.get_all_supplies("vlsi.inputs.supplies.ground")
 
     def get_independent_ground_nets(self) -> List[Supply]:
         return list(filter(lambda x: x.tie is None, self.get_all_ground_nets()))
 
     def _get_by_bump_dim_pitch(self) -> Dict[str, float]:
         """
-        Return pitches in the x and y directions. 
+        Return pitches in the x and y directions.
         """
         pitch_x = self.get_setting_suffix('vlsi.inputs.bumps.pitch', 'x')
         pitch_y = self.get_setting_suffix('vlsi.inputs.bumps.pitch', 'y')
 
         return {'x': pitch_x, 'y': pitch_y}
 
     def get_bumps(self) -> Optional[BumpsDefinition]:
@@ -1132,15 +1132,15 @@
             cell = None if not "custom_cell" in raw_assign else raw_assign["custom_cell"]
             if name is None and not no_con:
                 self.logger.warning("Invalid bump assignment, neither name nor no_connect specified for bump {x},{y}. Assuming it should be unassigned".format(
                     x=x, y=y))
             else:
                 assignments.append(BumpAssignment(name=name, no_connect=no_con,
                     x=x, y=y, group=group, custom_cell=cell))
-        
+
         pitch_settings = self._get_by_bump_dim_pitch()
 
         return BumpsDefinition(
             x=self.get_setting("vlsi.inputs.bumps.x"),
             y=self.get_setting("vlsi.inputs.bumps.y"),
             pitch_x = Decimal(str(pitch_settings['x'])),
             pitch_y = Decimal(str(pitch_settings['y'])),
@@ -1534,21 +1534,24 @@
     def get_stackup(self) -> Stackup:
         """
         Get the stackup provided by the technology key
         """
         # TODO how does python cache this? Do we need to avoid re-processing this every time?
         return self.technology.get_stackup_by_name(self.get_setting("technology.core.stackup"))
 
-    def get_input_ilms(self) -> List[ILMStruct]:
+    def get_input_ilms(self, full_tree=False) -> List[ILMStruct]:
         """
         Get a list of input ILM modules for hierarchical mode.
+        :param full_tree: if true, obtains the full tree (up to the current level of hierarchy) from vlsi.inputs.ilms.
+        Otherwise, obtains only children ilms from par.outputs.output_ilms
         """
-        ilms = self.get_setting("vlsi.inputs.ilms")  # type: List[dict]
-        assert isinstance(ilms, list)
-        return list(map(ILMStruct.from_setting, ilms))
+        if full_tree:
+            return list(map(ILMStruct.from_setting, self.get_setting("vlsi.inputs.ilms")))
+        else:
+            return list(map(ILMStruct.from_setting, self.get_setting("par.outputs.output_ilms")))
 
     def get_output_load_constraints(self) -> List[OutputLoadConstraint]:
         """
         Get a list of output load constraints as specified in the config.
         """
         output_loads = self.get_setting("vlsi.inputs.output_loads")
         output = []  # type: List[OutputLoadConstraint]
```

### Comparing `hammer_vlsi-1.1.1/hammer/vlsi/hammer_vlsi_impl.py` & `hammer_vlsi-1.1.2/hammer/vlsi/hammer_vlsi_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -385,15 +385,17 @@
     @abstractmethod
     def fill_outputs(self) -> bool:
         pass
 
     def export_config_outputs(self) -> Dict[str, Any]:
         outputs = deepdict(super().export_config_outputs())
         outputs["par.outputs.output_ilms"] = list(map(lambda s: s.to_setting(), self.output_ilms))
-        outputs["par.outputs.output_ilms_meta"] = "append"
+        outputs["par.outputs.output_ilms_meta"] = "append"  # to coalesce ILMs for current level of hierarchy
+        outputs["vlsi.inputs.ilms"] = list(map(lambda s: s.to_setting(), self.get_input_ilms(full_tree=True)))
+        outputs["vlsi.inputs.ilms_meta"] = "append"  # to coalesce ILMs for entire hierarchical tree
         outputs["par.outputs.output_gds"] = str(self.output_gds)
         outputs["par.outputs.output_netlist"] = str(self.output_netlist)
         outputs["par.outputs.output_sim_netlist"] = str(self.output_sim_netlist)
         outputs["par.outputs.hcells_list"] = list(self.hcells_list)
         outputs["par.outputs.seq_cells"] = self.output_seq_cells
         outputs["par.outputs.all_regs"] = self.output_all_regs
         outputs["par.inputs.input_files"] = self.input_files
@@ -1049,15 +1051,15 @@
         return []
 
     @abstractmethod
     def specify_std_cell_power_straps(self, blockage_spacing: Decimal, bbox: Optional[List[Decimal]], nets: List[str]) -> List[str]:
         """
         Generate a list of TCL commands that build the low-level standard cell power strap rails.
         This is a low-level, cad-tool-specific API. It is designed to be called by higher-level methods, so calling this directly is not recommended.
-        This will create power straps based on technology.core.tap_cell_rail_reference.
+        This will create power straps based on the tapcells in the special cells list.
         The layer is set by technology.core.std_cell_rail_layer, which should be the highest metal layer in the std cell rails.
         This method should be called before any calls to specify_power_straps.
 
         :param blockage_spacing: The spacing to leave between the end of a stripe and a macro or routing blockage.
         :param bbox: The optional (2N)-point bounding box of the area to generate straps. By default the entire core area is used.
         :param nets: A list of power net names (e.g. ["VDD", "VSS"]).
         :return: A list of TCL commands that will generate power straps on rails.
@@ -1197,14 +1199,17 @@
 class HammerLVSTool(HammerSignoffTool):
 
     def export_config_outputs(self) -> Dict[str, Any]:
         outputs = deepdict(super().export_config_outputs())
         outputs["lvs.inputs.top_module"] = self.top_module
         return outputs
 
+    def get_input_ilms(self, full_tree=True) -> List[ILMStruct]:
+        return super().get_input_ilms(full_tree)
+
     @abstractmethod
     def fill_outputs(self) -> bool:
         pass
 
     @abstractmethod
     def globally_waived_erc_rules(self) -> List[str]:
         # TODO(johnwright) how to waive specific instances of ERC rules, rather than blanket waivers
@@ -1328,34 +1333,14 @@
     def hcells_list(self, value: List[str]) -> None:
         """Set the list of cells to explicitly map hierarchically in LVS."""
         if not (isinstance(value, List)):
             raise TypeError("hcells_list must be a List[str]")
         self.attr_setter("_hcells_list", value)
 
 
-    @property
-    def ilms(self) -> List[ILMStruct]:
-        """
-        Get the list of (optional) input ILM information for hierarchical mode.
-
-        :return: The list of (optional) input ILM information for hierarchical mode.
-        """
-        try:
-            return self.attr_getter("_ilms", None)
-        except AttributeError:
-            raise ValueError("Nothing set for the list of (optional) input ILM information for hierarchical mode yet")
-
-    @ilms.setter
-    def ilms(self, value: List[ILMStruct]) -> None:
-        """Set the list of (optional) input ILM information for hierarchical mode."""
-        if not (isinstance(value, List)):
-            raise TypeError("ilms must be a List[ILMStruct]")
-        self.attr_setter("_ilms", value)
-
-
     ### Outputs ###
     ### END Generated interface HammerLVSTool ###
 
 
 class HammerSimTool(HammerTool):
 
     def export_config_outputs(self) -> Dict[str, Any]:
@@ -2068,30 +2053,30 @@
         output.append('upf_version 2.0')
         output.append(f'set_design_top {self.top_module}')
         vdd = VoltageValue(self.get_setting("vlsi.inputs.supplies.VDD"))
         #Create Single Power Domain
         output.append(f'create_power_domain {domain} \\')
         output.append(f'\t-elements {{.}}')
         #Get Supply Nets
-        power_nets = self.get_all_power_nets() 
+        power_nets = self.get_all_power_nets()
         ground_nets = self.get_all_ground_nets()
-        #Create Supply Ports 
+        #Create Supply Ports
         for pg_net in (power_nets+ground_nets):
             if(pg_net.pin != None):
                 #Create Supply Nets
                 output.append(f'create_supply_net {pg_net.name} -domain {domain}')
                 output.append(f'create_supply_port {pg_net.name} -domain {domain} \\')
                 output.append(f'\t-direction in')
                 #Connect Supply Net
                 output.append(f'connect_supply_net {pg_net.name} -ports {pg_net.name}')
                 #Set Domain Supply Net
         output.append(f'set_domain_supply_net {domain} \\')
         output.append(f'\t-primary_power_net {power_nets[0].name} \\')
         output.append(f'\t-primary_ground_net {ground_nets[0].name}')
-        #Add Port States 
+        #Add Port States
         for p_net in power_nets:
             if(p_net.pin != None):
                 output.append(f'add_port_state {p_net.name} \\')
                 output.append(f'\t-state {{default {vdd.value}}}')
         for g_net in ground_nets:
             if(g_net.pin != None):
                 output.append(f'add_port_state {g_net.name} \\')
```

### Comparing `hammer_vlsi-1.1.1/hammer/vlsi/hooks.py` & `hammer_vlsi-1.1.2/hammer/vlsi/hooks.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/vlsi/submit_command.py` & `hammer_vlsi-1.1.2/hammer/vlsi/submit_command.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 
 # pylint: disable=bad-continuation
 
 import atexit
 import subprocess
 import termios
 import sys
+import os
 import datetime
 from abc import abstractmethod
 from functools import reduce
 from typing import Any, Dict, List, Tuple, NamedTuple, Optional
 
 from hammer.config import HammerDatabase
 from hammer.logging import HammerVLSILoggingContext
 from hammer.utils import add_dicts, get_or_else
 
 __all__ = ['HammerSubmitCommand', 'HammerLocalSubmitCommand',
-           'HammerLSFSettings', 'HammerLSFSubmitCommand']
+           'HammerLSFSettings', 'HammerLSFSubmitCommand',
+           'HammerSlurmSettings', 'HammerSlurmSubmitCommand']
 
 
 class HammerSubmitCommand:
 
     @abstractmethod
     def submit(self, args: List[str], env: Dict[str, str],
                logger: HammerVLSILoggingContext, cwd: Optional[str] = None) -> Tuple[str, int]:
@@ -76,14 +78,16 @@
 
         submit_command = None  # type: Optional[HammerSubmitCommand]
         if submit_command_mode in {"none", "local"}:  # pylint: disable=no-else-return
             # Do not read the options, return immediately
             return HammerLocalSubmitCommand()
         elif submit_command_mode == "lsf":
             submit_command = HammerLSFSubmitCommand()
+        elif submit_command_mode == "slurm":
+            submit_command = HammerSlurmSubmitCommand()
         else:
             raise NotImplementedError(
                 "Submit command key for {0}: {1} is not implemented".format(
                     tool_namespace, submit_command_mode))
 
         submit_command.read_settings(
             combine_settings(submit_command_settings, submit_command_mode),
@@ -254,7 +258,109 @@
                 output_buf += line
             else:
                 break
         # check errors
         proc.communicate()
 
         return output_buf, proc.returncode
+
+
+class HammerSlurmSettings(NamedTuple('HammerSlurmSettings', [
+    ('srun_binary', str),
+    ('num_cpus', Optional[int]),
+    ('partition', Optional[str]),
+    ('extra_args', Optional[List[str]])
+])):
+    __slots__ = ()
+
+    @staticmethod
+    def from_setting(settings: Dict[str, Any]) -> "HammerSlurmSettings":
+        if not isinstance(settings, dict):
+            raise ValueError("Must be a dictionary")
+        try:
+            srun_binary = settings["srun_binary"]
+        except KeyError:
+            raise ValueError("Missing mandatory key srun_binary for Slurm settings.")
+        try:
+            num_cpus = settings["num_cpus"]
+        except KeyError:
+            num_cpus = None
+        try:
+            partition = settings["partition"]
+        except KeyError:
+            partition = None
+        try:
+            extra_args = settings["extra_args"]
+        except KeyError:
+            extra_args = None
+
+        return HammerSlurmSettings(
+            srun_binary=srun_binary,
+            num_cpus=num_cpus,
+            partition=partition,
+            extra_args=extra_args
+        )
+
+
+class HammerSlurmSubmitCommand(HammerSubmitCommand):
+
+    # TODO use --output to set logfile AND have stdout/stderr output
+    #      Currently there is no option to specify a log file.
+
+    @property
+    def settings(self) -> HammerSlurmSettings:
+        if not hasattr(self, "_settings"):
+            raise ValueError("Nothing set for settings yet")
+        return getattr(self, "_settings")
+
+    @settings.setter
+    def settings(self, value: HammerSlurmSettings) -> None:
+        """
+        Set the settings class variable
+
+        :param value: The HammerSlurmSettings NamedTuple to use
+        """
+        setattr(self, "_settings", value)
+
+    def read_settings(self, settings: Dict[str, Any], tool_namespace: str) -> None:  # pylint: disable=unused-argument
+        self.settings = HammerSlurmSettings.from_setting(settings)
+
+    def srun_args(self) -> List[str]:
+        args = [self.settings.srun_binary]
+        if self.settings.partition is not None:
+            args.extend(["--partition", self.settings.partition])
+        if self.settings.num_cpus is not None:
+            args.extend(["--ntasks", "%d" % self.settings.num_cpus])
+        if self.settings.extra_args is not None:
+            args.extend(self.settings.extra_args)
+        return args
+
+    def submit(self, args: List[str], env: Dict[str, str],
+               logger: HammerVLSILoggingContext, cwd: Optional[str] = None) -> Tuple[str, int]:
+        prog_tag = self.get_program_tag(args)
+
+        subprocess_format_str = 'Executing subprocess: {srun_args} {args}'
+        logger.debug(subprocess_format_str.format(srun_args=' '.join(self.srun_args()),
+                                                  args=' '.join(args)))
+        subprocess_logger = logger.context("Exec " + prog_tag)
+        proc = subprocess.Popen(self.srun_args() + args,
+                                shell=False, stderr=subprocess.STDOUT,
+                                stdout=subprocess.PIPE, env=env, cwd=cwd)
+
+        output_buf = ""
+        # Log output and also capture output at the same time.
+        so = proc.stdout
+        assert so is not None
+        while True:
+            line = so.readline().decode("utf-8")
+            if line != '':
+                subprocess_logger.debug(line.rstrip())
+                output_buf += line
+            else:
+                break
+        # TODO: check errors
+
+        # Refresh output directory (fixes NFS issue)
+        if cwd is not None:
+            os.path.exists(cwd)
+
+        return output_buf, proc.returncode
```

### Comparing `hammer_vlsi-1.1.1/hammer/vlsi/units.py` & `hammer_vlsi-1.1.2/hammer/vlsi/units.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/hammer/vlsi/vendor/def2stream.py` & `hammer_vlsi-1.1.2/hammer/vlsi/vendor/def2stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -194,12 +194,27 @@
   top_only_layout.read(seal_file)
 
   for cell in top_only_layout.top_cells():
     if cell != top_cell:
       print("[INFO] Merging '{0}' as child of '{1}'".format(cell.name, top_cell.name))
       top.insert(pya.CellInstArray(cell.cell_index(), pya.Trans()))
 
+# Remove zero path lengths
+#   this in lyt file doesn't work: <no-zero-length-paths>true</no-zero-length-paths>
+print("Removing zero-length paths...")
+for cell in top_only_layout.each_cell():
+  for layer_idx in top_only_layout.layer_indexes():
+    for shape in cell.each_shape(layer_idx):
+      if shape.is_path():
+        path = shape.path
+        paths = [(p.x, p.y) for p in path.each_point()]
+        paths_unique = set(paths)
+        if len(paths_unique) < len(paths):
+          polygon = path.polygon()
+          print(f"\tlayer_index: {layer_idx},", shape)
+          shape.delete()
+
 # Write out the GDS
 print("[INFO] Writing out GDS/OAS '{0}'".format(out_file))
 top_only_layout.write(out_file)
 
 sys.exit(errors)
```

### Comparing `hammer_vlsi-1.1.1/hammer/vlsi/vendor/openroad.py` & `hammer_vlsi-1.1.2/hammer/vlsi/vendor/openroad.py`

 * *Files identical despite different names*

### Comparing `hammer_vlsi-1.1.1/pyproject.toml` & `hammer_vlsi-1.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hammer-vlsi"
-version = "1.1.1"
+version = "1.1.2"
 description = "Hammer is a physical design framework that wraps around vendor specific technologies and tools to provide a single API to create ASICs."
 authors = ["Colin Schmidt <colin.schmidt@sifive.com>", "Edward Wang <edward.c.wang@compdigitec.com>", "John Wright <johnwright@eecs.berkeley.edu>"]
 maintainers = ["Harrison Liew <harrisonliew@berkeley.edu>", "Daniel Grubb <dpgrubb@berkeley.edu>"]
 readme = "README.md"
 repository = "https://github.com/ucb-bar/hammer"
 packages = [
     {include = "hammer"}
@@ -44,16 +44,15 @@
 sphinx-jsonschema = "^1.19.1"
 sphinx_rtd_size = "^0.2.0"
 pylint = "^2.15"
 
 [[tool.poetry.source]]
 name = "testpypi"
 url = "https://test.pypi.org/legacy/"
-default = false
-secondary = false
+priority = "explicit"
 
 [build-system]
 requires = ["poetry-core>=1.0.8", "setuptools>=65.3"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.tox]
 legacy_tox_ini = """
```

### Comparing `hammer_vlsi-1.1.1/PKG-INFO` & `hammer_vlsi-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hammer-vlsi
-Version: 1.1.1
+Version: 1.1.2
 Summary: Hammer is a physical design framework that wraps around vendor specific technologies and tools to provide a single API to create ASICs.
 Home-page: https://github.com/ucb-bar/hammer
 Author: Colin Schmidt
 Author-email: colin.schmidt@sifive.com
 Maintainer: Harrison Liew
 Maintainer-email: harrisonliew@berkeley.edu
 Requires-Python: >=3.9,<4.0
```

