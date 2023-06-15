# Comparing `tmp/boardgen-0.6.2.tar.gz` & `tmp/boardgen-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boardgen-0.6.2.tar", max compression
+gzip compressed data, was "boardgen-0.7.0.tar", max compression
```

## Comparing `boardgen-0.6.2.tar` & `boardgen-0.7.0.tar`

### file list

```diff
@@ -1,79 +1,86 @@
--rw-r--r--   0        0        0     1076 2023-05-29 14:14:22.593899 boardgen-0.6.2/LICENSE
--rw-r--r--   0        0        0     4785 2023-05-29 14:14:22.593899 boardgen-0.6.2/README.md
--rw-r--r--   0        0        0      353 2023-05-29 14:14:22.593899 boardgen-0.6.2/boardgen/__init__.py
--rw-r--r--   0        0        0    11411 2023-05-29 14:14:22.593899 boardgen-0.6.2/boardgen/cli.py
--rw-r--r--   0        0        0       92 2023-05-29 14:14:22.593899 boardgen-0.6.2/boardgen/core/__init__.py
--rw-r--r--   0        0        0     2146 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/core/cache.py
--rw-r--r--   0        0        0     9853 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/core/core.py
--rw-r--r--   0        0        0      925 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/core/getters.py
--rw-r--r--   0        0        0      773 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/mixins.py
--rw-r--r--   0        0        0      439 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/models/__init__.py
--rw-r--r--   0        0        0     1705 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/models/board.py
--rw-r--r--   0        0        0     1015 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/models/enums.py
--rw-r--r--   0        0        0     1156 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/models/flash_region.py
--rw-r--r--   0        0        0     1257 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/models/pcb.py
--rw-r--r--   0        0        0     2348 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/models/role.py
--rw-r--r--   0        0        0      358 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/models/template.py
--rw-r--r--   0        0        0      117 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/readme/__init__.py
--rw-r--r--   0        0        0     2229 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/readme/parts.py
--rw-r--r--   0        0        0     8123 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/readme/writer.py
--rw-r--r--   0        0        0      109 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/boards/README.md
--rw-r--r--   0        0        0      589 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/flash.json
--rw-r--r--   0        0        0      831 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/presets.json
--rw-r--r--   0        0        0     1497 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/roles.json
--rw-r--r--   0        0        0      398 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/label_line_2mm_down.json
--rw-r--r--   0        0        0      412 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/label_line_2mm_up.json
--rw-r--r--   0        0        0      690 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/labels_horz5_2mm.json
--rw-r--r--   0        0        0      829 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/labels_horz6_2mm.json
--rw-r--r--   0        0        0      967 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/labels_horz7_2mm.json
--rw-r--r--   0        0        0     1106 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/labels_horz8_2mm.json
--rw-r--r--   0        0        0      133 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pad_10x25.json
--rw-r--r--   0        0        0      525 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pads_horz5_2mm.json
--rw-r--r--   0        0        0      631 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pads_horz6_2mm.json
--rw-r--r--   0        0        0      386 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pin_horz_2mm_cast_hole.json
--rw-r--r--   0        0        0      244 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pin_horz_2mm_cast_nohole.json
--rw-r--r--   0        0        0      388 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pin_vert_2mm_cast_hole.json
--rw-r--r--   0        0        0      245 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pin_vert_2mm_cast_nohole.json
--rw-r--r--   0        0        0      540 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pins_horz5_2mm_0.7mm.json
--rw-r--r--   0        0        0      649 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pins_horz6_2mm_0.7mm.json
--rw-r--r--   0        0        0      757 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pins_horz7_2mm_0.7mm.json
--rw-r--r--   0        0        0      866 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pins_horz8_2mm_0.7mm.json
--rw-r--r--   0        0        0      789 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pins_vert7_2mm_0.7mm.json
--rw-r--r--   0        0        0      902 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/pins_vert8_2mm_0.7mm.json
--rw-r--r--   0        0        0       80 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/test_pad_1mm.json
--rw-r--r--   0        0        0      980 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/shapes/tuya2-pcb.json
--rw-r--r--   0        0        0     2931 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/custom-20x24-22.json
--rw-r--r--   0        0        0     2594 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/esp12e-21.json
--rw-r--r--   0        0        0     2640 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/esp12e-22.json
--rw-r--r--   0        0        0      256 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/esp12e-shield-nohole.json
--rw-r--r--   0        0        0      233 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/esp12e-shield.json
--rw-r--r--   0        0        0      233 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/esp12s-shield.json
--rw-r--r--   0        0        0     1666 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/esp12s.json
--rw-r--r--   0        0        0     1222 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/rf-15mm-type1.json
--rw-r--r--   0        0        0     1224 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/rf-16mm-type1.json
--rw-r--r--   0        0        0     1226 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/rf-20mm-type1.json
--rw-r--r--   0        0        0      450 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/tuya-16x24.json
--rw-r--r--   0        0        0      227 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/tuya2-shield.json
--rw-r--r--   0        0        0     1308 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/tuya2.json
--rw-r--r--   0        0        0      229 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/tuya2l-shield.json
--rw-r--r--   0        0        0      909 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/res/templates/tuya2l.json
--rw-r--r--   0        0        0      341 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/__init__.py
--rw-r--r--   0        0        0     4324 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/base.py
--rw-r--r--   0        0        0     1120 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/circle.py
--rw-r--r--   0        0        0     1268 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/fill_style.py
--rw-r--r--   0        0        0     2268 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/group.py
--rw-r--r--   0        0        0      182 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/label/__init__.py
--rw-r--r--   0        0        0     1706 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/label/block.py
--rw-r--r--   0        0        0      543 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/label/io_line.py
--rw-r--r--   0        0        0     3306 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/label/label.py
--rw-r--r--   0        0        0     1082 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/rect.py
--rw-r--r--   0        0        0      833 2023-05-29 14:14:22.597899 boardgen-0.6.2/boardgen/shapes/text.py
--rw-r--r--   0        0        0     2003 2023-05-29 14:14:22.601899 boardgen-0.6.2/boardgen/utils.py
--rw-r--r--   0        0        0      119 2023-05-29 14:14:22.601899 boardgen-0.6.2/boardgen/variant/__init__.py
--rw-r--r--   0        0        0      362 2023-05-29 14:14:22.601899 boardgen-0.6.2/boardgen/variant/features.py
--rw-r--r--   0        0        0     6271 2023-05-29 14:14:22.601899 boardgen-0.6.2/boardgen/variant/parts.py
--rw-r--r--   0        0        0      319 2023-05-29 14:14:22.601899 boardgen-0.6.2/boardgen/variant/section.py
--rw-r--r--   0        0        0     8502 2023-05-29 14:14:22.601899 boardgen-0.6.2/boardgen/variant/writer.py
--rw-r--r--   0        0        0     8765 2023-05-29 14:14:22.601899 boardgen-0.6.2/boardgen/vector.py
--rw-r--r--   0        0        0      546 2023-05-29 14:14:22.601899 boardgen-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     5427 1970-01-01 00:00:00.000000 boardgen-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-15 18:45:53.655918 boardgen-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4785 2023-06-15 18:45:53.655918 boardgen-0.7.0/README.md
+-rw-r--r--   0        0        0      353 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/__init__.py
+-rw-r--r--   0        0        0     9220 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/cli.py
+-rw-r--r--   0        0        0       92 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/core/__init__.py
+-rw-r--r--   0        0        0     2543 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/core/cache.py
+-rw-r--r--   0        0        0     9760 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/core/core.py
+-rw-r--r--   0        0        0     1325 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/core/getters.py
+-rw-r--r--   0        0        0     1891 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/draw_util.py
+-rw-r--r--   0        0        0      773 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/mixins.py
+-rw-r--r--   0        0        0      439 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/models/__init__.py
+-rw-r--r--   0        0        0     1705 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/models/board.py
+-rw-r--r--   0        0        0     1015 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/models/enums.py
+-rw-r--r--   0        0        0     1156 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/models/flash_region.py
+-rw-r--r--   0        0        0     1257 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/models/pcb.py
+-rw-r--r--   0        0        0     2348 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/models/role.py
+-rw-r--r--   0        0        0      358 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/models/template.py
+-rw-r--r--   0        0        0      117 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/readme/__init__.py
+-rw-r--r--   0        0        0     2229 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/readme/parts.py
+-rw-r--r--   0        0        0     8123 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/readme/writer.py
+-rw-r--r--   0        0        0      109 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/boards/README.md
+-rw-r--r--   0        0        0      589 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/flash.json
+-rw-r--r--   0        0        0      831 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/presets.json
+-rw-r--r--   0        0        0     1497 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/roles.json
+-rw-r--r--   0        0        0      398 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/label_line_2mm_down.json
+-rw-r--r--   0        0        0      412 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/label_line_2mm_up.json
+-rw-r--r--   0        0        0      690 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/labels_horz5_2mm.json
+-rw-r--r--   0        0        0      829 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/labels_horz6_2mm.json
+-rw-r--r--   0        0        0      967 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/labels_horz7_2mm.json
+-rw-r--r--   0        0        0     1106 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/labels_horz8_2mm.json
+-rw-r--r--   0        0        0      133 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pad_10x25.json
+-rw-r--r--   0        0        0      525 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pads_horz5_2mm.json
+-rw-r--r--   0        0        0      631 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pads_horz6_2mm.json
+-rw-r--r--   0        0        0      386 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pin_horz_2mm_cast_hole.json
+-rw-r--r--   0        0        0      244 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pin_horz_2mm_cast_nohole.json
+-rw-r--r--   0        0        0      388 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pin_vert_2mm_cast_hole.json
+-rw-r--r--   0        0        0      245 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pin_vert_2mm_cast_nohole.json
+-rw-r--r--   0        0        0      540 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pins_horz5_2mm_0.7mm.json
+-rw-r--r--   0        0        0      649 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pins_horz6_2mm_0.7mm.json
+-rw-r--r--   0        0        0      757 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pins_horz7_2mm_0.7mm.json
+-rw-r--r--   0        0        0      866 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pins_horz8_2mm_0.7mm.json
+-rw-r--r--   0        0        0      789 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pins_vert7_2mm_0.7mm.json
+-rw-r--r--   0        0        0      902 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pins_vert8_2mm_0.7mm.json
+-rw-r--r--   0        0        0       80 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/test_pad_1mm.json
+-rw-r--r--   0        0        0      980 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/tuya2-pcb.json
+-rw-r--r--   0        0        0     2931 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/custom-20x24-22.json
+-rw-r--r--   0        0        0     2594 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/esp12e-21.json
+-rw-r--r--   0        0        0     2640 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/esp12e-22.json
+-rw-r--r--   0        0        0      256 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/esp12e-shield-nohole.json
+-rw-r--r--   0        0        0      233 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/esp12e-shield.json
+-rw-r--r--   0        0        0      233 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/esp12s-shield.json
+-rw-r--r--   0        0        0     1666 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/esp12s.json
+-rw-r--r--   0        0        0     1222 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/rf-15mm-type1.json
+-rw-r--r--   0        0        0     1224 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/rf-16mm-type1.json
+-rw-r--r--   0        0        0     1226 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/rf-20mm-type1.json
+-rw-r--r--   0        0        0      450 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/tuya-16x24.json
+-rw-r--r--   0        0        0      227 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/tuya2-shield.json
+-rw-r--r--   0        0        0     1308 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/tuya2.json
+-rw-r--r--   0        0        0      229 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/tuya2l-shield.json
+-rw-r--r--   0        0        0      909 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/tuya2l.json
+-rw-r--r--   0        0        0      341 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/shapes/__init__.py
+-rw-r--r--   0        0        0     4369 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/shapes/base.py
+-rw-r--r--   0        0        0     1158 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/shapes/circle.py
+-rw-r--r--   0        0        0     1283 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/shapes/fill_style.py
+-rw-r--r--   0        0        0     2268 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/shapes/group.py
+-rw-r--r--   0        0        0      182 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/shapes/label/__init__.py
+-rw-r--r--   0        0        0     1745 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/shapes/label/block.py
+-rw-r--r--   0        0        0      543 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/shapes/label/io_line.py
+-rw-r--r--   0        0        0     3306 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/shapes/label/label.py
+-rw-r--r--   0        0        0     1120 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/shapes/rect.py
+-rw-r--r--   0        0        0      867 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/shapes/text.py
+-rw-r--r--   0        0        0     2238 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/utils.py
+-rw-r--r--   0        0        0      119 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/variant/__init__.py
+-rw-r--r--   0        0        0      362 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/variant/features.py
+-rw-r--r--   0        0        0     6271 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/variant/parts.py
+-rw-r--r--   0        0        0      319 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/variant/section.py
+-rw-r--r--   0        0        0     8502 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/variant/writer.py
+-rw-r--r--   0        0        0     8765 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/vector.py
+-rw-r--r--   0        0        0      503 2023-06-15 18:45:53.659918 boardgen-0.7.0/ltctplugin/boardgen/__init__.py
+-rw-r--r--   0        0        0     4140 2023-06-15 18:45:53.659918 boardgen-0.7.0/ltctplugin/boardgen/boardgen.wxui
+-rw-r--r--   0        0        0     5230 2023-06-15 18:45:53.659918 boardgen-0.7.0/ltctplugin/boardgen/boardgen.xrc
+-rw-r--r--   0        0        0    11614 2023-06-15 18:45:53.659918 boardgen-0.7.0/ltctplugin/boardgen/gui.py
+-rw-r--r--   0        0        0     1321 2023-06-15 18:45:53.659918 boardgen-0.7.0/ltctplugin/boardgen/svg.py
+-rw-r--r--   0        0        0     3555 2023-06-15 18:45:53.659918 boardgen-0.7.0/ltctplugin/boardgen/utils.py
+-rw-r--r--   0        0        0      668 2023-06-15 18:45:53.659918 boardgen-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5463 1970-01-01 00:00:00.000000 boardgen-0.7.0/PKG-INFO
```

### Comparing `boardgen-0.6.2/LICENSE` & `boardgen-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/README.md` & `boardgen-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/cli.py` & `boardgen-0.7.0/boardgen/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 
 import os
 from os.path import isfile, join
 
 import click
 from click import echo
 from devtools import debug
-from svgwrite import Drawing, shapes
-from svgwrite.utils import AutoID
 
 from . import Core
-from .models import Board, Side, Template
+from .draw_util import draw_shapes, get_pcb_images
+from .models import Board, Template
 from .readme.writer import ReadmeWriter
-from .shapes.label import Label
 from .utils import load_json
 from .variant.writer import VariantWriter
 from .vector import V
 
 core = Core()
 
 
@@ -76,15 +74,16 @@
 @click.option("--output", "-o", default=".", help="Output directory")
 @click.option("--subdir", "-O", is_flag=True, help="Output into per-board subdirectory")
 @click.option("--width", "-w", default=1024, help="Image width (px)")
 @click.option("--height", "-h", default=500, help="Image height (px)")
 @click.option(
     "--scale",
     "-s",
-    default=12,
+    default=None,
+    type=float,
     help="Diagram size (bigger if scale larger); 0 means automatic",
 )
 @click.option(
     "--canvas/--no-canvas",
     "-c/-C",
     default=True,
     help="Draw a white background with black border",
@@ -111,94 +110,32 @@
         ctx.exit()
 
     px_size = V(width, height)
 
     if output:
         os.makedirs(output, exist_ok=True)
 
-    sides = [Side.FRONT, Side.BACK]
-
     scale_arg = scale
 
     for board in boards:
         board: Board
         if not board.pcb or not board.pcb.templates:
             echo(f"Skipping '{board.name}'...")
             continue
         echo(f"Drawing '{board.name}'...")
 
         pcb = board.pcb
-        images = []
-
-        AutoID._set_value(1)
-        dwg = Drawing(size=px_size.tuple)
 
-        scale = scale_arg
-        if pcb.scale and pcb.scale < scale:
-            scale = pcb.scale
-
-        for side in sides:
-            try:
-                (pcb_pos1, pcb_pos2) = pcb.get_pos(side)
-            except ValueError:
-                continue
-            labels_list = []
-            size = pcb_pos2 - pcb_pos1
-            pos1 = pcb_pos1
-            if labels:
-                (labels_list, labels_pos1, labels_pos2) = core.build_labels(pcb, side)
-                if labels_list:
-                    pos1 = V(
-                        min(pcb_pos1.x, labels_pos1.x), min(pcb_pos1.y, labels_pos1.y)
-                    )
-                    pos2 = V(
-                        max(pcb_pos2.x, labels_pos2.x), max(pcb_pos2.y, labels_pos2.y)
-                    )
-                    size = pos2 - pos1
-                else:
-                    continue
-            images += [
-                (side, pos1, size, labels_list),
-            ]
-
-        # stack horizontally
-        part_size = V(px_size.x / len(images), px_size.y)
-        part_pos = [V(part_size.x * i, 0) for i in range(len(images))]
-
-        if scale:
-            vb_size = px_size / scale
+        if scale_arg is None:
+            scale = pcb.scale or 12
         else:
-            scale = 99999
-            size_pad = part_size * 0.90  # 5% padding from each side
-            for _, _, size, _ in images:
-                scale = min(scale, size_pad.x / size.x, size_pad.y / size.y)
-            echo(" - calculated scale: %.2f" % scale)
-            vb_size = px_size / scale
-
-        dwg.viewbox(width=vb_size.x, height=vb_size.y)
-
-        if canvas:
-            bg = shapes.Rect(insert=(0, 0), size=vb_size.tuple)
-            bg.fill(color="white")
-            bg.stroke(color="black", width=0.1)
-            dwg.add(bg)
-
-        for i, (side, pos1, size, labels_list) in enumerate(images):
-            pcb_pos = ((part_size / scale) - size) / 2
-            pcb_pos += part_pos[i] / scale
-            pcb_pos -= pos1
-            if canvas:
-                pcb_pos.x -= 0.05
-            pcb.draw(dwg, side, pcb_pos)
-            if labels:
-                for label in labels_list:
-                    label: Label
-                    label.move(pcb_pos)
-                    label.draw(dwg)
-                    label.move(-pcb_pos)
+            scale = scale_arg
+
+        images = get_pcb_images(core, pcb, labels)
+        dwg = draw_shapes(px_size, scale, images, canvas)
 
         svg = join(output, f"{board.id}.svg")
         if subdir:
             os.makedirs(join(output, board.id), exist_ok=True)
             svg = join(output, board.id, f"pinout_{board.id}.svg")
         with open(svg, "w", encoding="utf-8") as f:
             dwg.write(f, pretty=True, indent=4)
```

### Comparing `boardgen-0.6.2/boardgen/core/cache.py` & `boardgen-0.7.0/boardgen/core/cache.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # Copyright (c) Kuba Szczodrzyński 2022-05-12.
 
 from abc import ABC
 from glob import glob
 from os.path import basename, isfile, join
+from typing import Callable, Optional
 
 from ..utils import load_json, merge_dicts
 
 
 class CoreCache(ABC):
     _cache: dict[str, dict[str, dict]] = {
         "boards": {},
+        "board_objs": {},
         "shapes": {},
         "templates": {},
     }
+    json_hook: Optional[Callable[[str, str, dict, Optional[str]], None]] = None
 
     def get_dirs(self, type: str) -> list[str]:
         attr_name = f"_dirs_{type}"
         if not hasattr(self, attr_name):
             return []
         return getattr(self, attr_name)
 
@@ -26,44 +29,48 @@
         for dir in dirs:
             for file in glob(join(dir, "*.json")):
                 files.add(basename(file).rpartition(".")[0])
         return files
 
     def load_json(self, type: str, name: str) -> dict | None:
         if name in self._cache[type]:
+            if self.json_hook:
+                self.json_hook(type, name, self._cache[type][name], None)
             return self._cache[type][name]
         dirs = self.get_dirs(type)
         for dir in dirs:
             file = join(dir, f"{name}.json")
             if isfile(file):
                 data = load_json(file)
                 self._cache[type][name] = data
+                if self.json_hook:
+                    self.json_hook(type, name, data, file)
                 return data
         return None
 
     def load_shape(self, name: str) -> dict:
         return self.load_json("shapes", name)
 
     def load_board_base(self, name: str) -> dict:
         name = join("_base", name)
         return self.load_json("boards", name)
 
-    def load_board(self, name: str) -> dict:
-        if name in self._cache["boards"]:
-            return self._cache["boards"][name]
+    def load_board(self, name: str, allow_cache: bool = True) -> dict:
+        if allow_cache and name in self._cache["board_objs"]:
+            return self._cache["board_objs"][name]
         manifest = self.load_json("boards", name)
         if "_base" in manifest:
             bases = manifest["_base"]
             if not isinstance(bases, list):
                 bases = [bases]
 
             result = {}
             for base in bases:
                 base_manifest = self.load_board_base(base)
                 merge_dicts(result, base_manifest)
             merge_dicts(result, manifest)
             manifest = result
-        self._cache["boards"][name] = manifest
+        self._cache["board_objs"][name] = manifest
         return manifest
 
     def load_template(self, name: str) -> dict:
         return self.load_json("templates", name)
```

### Comparing `boardgen-0.6.2/boardgen/core/core.py` & `boardgen-0.7.0/boardgen/core/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 # Copyright (c) Kuba Szczodrzyński 2022-05-11.
 
 import json
 import re
+from copy import deepcopy
 from importlib.metadata import version
 from os.path import dirname, isfile, join
 
 from ..mixins import HasId, ParentType
-from ..models import Board, FlashRegion, Pcb, Role, RoleType, ShapeType, Side, Template
+from ..models import Board, FlashRegion, Pcb, RoleType, ShapeType, Side, Template
 from ..models.enums import RoleValue
 from ..shapes.base import Shape
 from ..shapes.circle import Circle
 from ..shapes.group import ShapeGroup
 from ..shapes.label import Label
 from ..shapes.rect import Rect
 from ..shapes.text import Text
-from ..utils import load_json, var
+from ..utils import var
 from ..vector import V
 from .cache import CoreCache
 from .getters import CoreGetters
 
 
 class Core(CoreCache, CoreGetters):
     shape_ctors: dict[ShapeType, type]
     is_libretiny: bool = False
 
     _dir_base: str
     _dirs_boards: list[str]
     _dirs_shapes: list[str]
     _dirs_templates: list[str]
-    _file_presets: str
-    _file_roles: str
-    _presets: dict[str, dict] = None
-    _roles: dict[RoleType, Role] = None
-    _flash: dict[str, str] = None
 
     def __init__(self) -> None:
         self._dir_base = join(dirname(__file__), "..", "res")
         self._dirs_boards = [
             join(dirname(__file__), "..", "..", "..", "..", "boards"),
             join(self._dir_base, "boards"),
             "boards",
@@ -97,19 +93,19 @@
     def add_custom_json(
         self,
         presets: dict = None,
         roles: dict = None,
         flash: dict = None,
     ):
         if presets:
-            self.presets |= presets
+            self.presets.update(presets)
         if roles:
-            self.roles |= roles
+            self.roles.update(roles)
         if flash:
-            self.flash |= flash
+            self.flash.update(flash)
 
     def build_shapes(self, name: str, parent: ParentType, pos: V = None) -> list[Shape]:
         """Load the specified shape JSON into a list of Shape objects.
 
         Args:
             name (str): Shape name.
             parent (ParentType): Parent object (Shape, Pcb, etc).
@@ -147,14 +143,15 @@
     def get_board(self, name: str) -> Board:
         """Load and build the specified board.
 
         Args:
             name (str): Board name.
         """
         manifest = self.load_board(name)
+        manifest = deepcopy(manifest)
         pcb = manifest.get("pcb", None)
         pinout = pcb.get("pinout", None) if pcb else None
         ic_pins = pcb.get("ic", None) if pcb else None
 
         if pinout:
             for roles in pinout.values():
                 roles: dict[str, RoleValue]
```

### Comparing `boardgen-0.6.2/boardgen/mixins.py` & `boardgen-0.7.0/boardgen/mixins.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/models/board.py` & `boardgen-0.7.0/boardgen/models/board.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/models/enums.py` & `boardgen-0.7.0/boardgen/models/enums.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/models/flash_region.py` & `boardgen-0.7.0/boardgen/models/flash_region.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/models/pcb.py` & `boardgen-0.7.0/boardgen/models/pcb.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/models/role.py` & `boardgen-0.7.0/boardgen/models/role.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/readme/parts.py` & `boardgen-0.7.0/boardgen/readme/parts.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/readme/writer.py` & `boardgen-0.7.0/boardgen/readme/writer.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/flash.json` & `boardgen-0.7.0/boardgen/res/flash.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/presets.json` & `boardgen-0.7.0/boardgen/res/presets.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/roles.json` & `boardgen-0.7.0/boardgen/res/roles.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/shapes/labels_horz5_2mm.json` & `boardgen-0.7.0/boardgen/res/shapes/labels_horz5_2mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/shapes/labels_horz6_2mm.json` & `boardgen-0.7.0/boardgen/res/shapes/labels_horz6_2mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/shapes/labels_horz7_2mm.json` & `boardgen-0.7.0/boardgen/res/shapes/labels_horz7_2mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/shapes/labels_horz8_2mm.json` & `boardgen-0.7.0/boardgen/res/shapes/labels_horz8_2mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/shapes/pads_horz5_2mm.json` & `boardgen-0.7.0/boardgen/res/shapes/pads_horz5_2mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/shapes/pads_horz6_2mm.json` & `boardgen-0.7.0/boardgen/res/shapes/pads_horz6_2mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/shapes/pins_horz5_2mm_0.7mm.json` & `boardgen-0.7.0/boardgen/res/shapes/pins_horz5_2mm_0.7mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/shapes/pins_horz6_2mm_0.7mm.json` & `boardgen-0.7.0/boardgen/res/shapes/pins_horz6_2mm_0.7mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/shapes/pins_horz7_2mm_0.7mm.json` & `boardgen-0.7.0/boardgen/res/shapes/pins_horz7_2mm_0.7mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/shapes/pins_horz8_2mm_0.7mm.json` & `boardgen-0.7.0/boardgen/res/shapes/pins_horz8_2mm_0.7mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/shapes/pins_vert7_2mm_0.7mm.json` & `boardgen-0.7.0/boardgen/res/shapes/pins_vert7_2mm_0.7mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/shapes/pins_vert8_2mm_0.7mm.json` & `boardgen-0.7.0/boardgen/res/shapes/pins_vert8_2mm_0.7mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/shapes/tuya2-pcb.json` & `boardgen-0.7.0/boardgen/res/shapes/tuya2-pcb.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/templates/custom-20x24-22.json` & `boardgen-0.7.0/boardgen/res/templates/custom-20x24-22.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/templates/esp12e-21.json` & `boardgen-0.7.0/boardgen/res/templates/esp12e-21.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/templates/esp12e-22.json` & `boardgen-0.7.0/boardgen/res/templates/esp12e-22.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/templates/esp12s.json` & `boardgen-0.7.0/boardgen/res/templates/esp12s.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/templates/rf-15mm-type1.json` & `boardgen-0.7.0/boardgen/res/templates/rf-15mm-type1.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/templates/rf-16mm-type1.json` & `boardgen-0.7.0/boardgen/res/templates/rf-16mm-type1.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/templates/rf-20mm-type1.json` & `boardgen-0.7.0/boardgen/res/templates/rf-20mm-type1.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/templates/tuya2.json` & `boardgen-0.7.0/boardgen/res/templates/tuya2.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/res/templates/tuya2l.json` & `boardgen-0.7.0/boardgen/res/templates/tuya2l.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/shapes/base.py` & `boardgen-0.7.0/boardgen/shapes/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Copyright (c) Kuba Szczodrzyński 2022-05-11.
 
 import json
+from copy import deepcopy
 from typing import Any
 
 from pydantic.color import Color
 from svgwrite import Drawing
 
 from ..mixins import HasId, HasVars
 from ..models.enums import LabelDir, RoleType, ShapeType
-from ..utils import Model, splitxy, var
+from ..utils import EvalFloat, Model, splitxy, var
 from ..vector import V
 
 
 def remap(shape: dict):
     tuples = ["pos", "size"]
     for tpl in tuples:
         if tpl in shape:
@@ -26,28 +27,28 @@
 
 class Shape(Model, HasId):
     base_id: str = None
     pos: V
 
     # for pad labels
     label_dir: LabelDir = None
-    label_size: float = None
+    label_size: EvalFloat = None
 
     def draw(self, dwg: Drawing):
         raise NotImplementedError()
 
     @staticmethod
     def deserialize(
         core,
         parent: HasId | HasVars | Any,
         data: dict,
         # offset: tuple[float, float] = None,
     ) -> "Shape":
         # do not modify source object
-        data = dict(data)
+        data = deepcopy(data)
         # allow includes without specified type
         if "type" not in data and "name" in data:
             data["type"] = "include"
 
         # prepend id with parent id path
         if isinstance(parent, HasId):
             if parent.fullid and "id" in data:
```

### Comparing `boardgen-0.6.2/boardgen/shapes/circle.py` & `boardgen-0.7.0/boardgen/shapes/circle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Copyright (c) Kuba Szczodrzyński 2022-05-12.
 
 from svgwrite import Drawing, shapes
 
+from ..utils import EvalFloat
 from .base import Shape
 from .fill_style import FillStyle
 
 
 class Circle(Shape):
-    r: float = None
-    d: float = None
+    r: EvalFloat = None
+    d: EvalFloat = None
     fill: FillStyle = None
     stroke: FillStyle = None
 
     def __init__(self, *a, **kw):
         super().__init__(*a, **kw)
         if not self.r and not self.d:
             raise ValueError("No radius or diameter")
```

### Comparing `boardgen-0.6.2/boardgen/shapes/fill_style.py` & `boardgen-0.7.0/boardgen/shapes/fill_style.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Copyright (c) Kuba Szczodrzyński 2022-05-12.
 
 from pydantic.color import Color
 from svgwrite import Drawing
 from svgwrite.gradients import LinearGradient
 from svgwrite.mixins import Presentation
 
-from ..utils import Model
+from ..utils import EvalFloat, Model
 from ..vector import V
 
 
 class FillStyle(Model):
     color: Color = None
     lgrad: tuple[V, Color, V, Color] = None
-    width: float = None
+    width: EvalFloat = None
 
     def apply_to(self, dwg: Drawing, el: Presentation, stroke: bool = False):
         color = None
         if self.color:
             color = self.color.as_hex()
         elif self.lgrad:
             unit = max(*self.lgrad[0].tuple, *self.lgrad[2].tuple)
```

### Comparing `boardgen-0.6.2/boardgen/shapes/group.py` & `boardgen-0.7.0/boardgen/shapes/group.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/shapes/label/block.py` & `boardgen-0.7.0/boardgen/shapes/label/block.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 from math import radians, tan
 
 from svgwrite import Drawing
 from svgwrite.container import Group
 from svgwrite.shapes import Rect
 from svgwrite.text import Text
 
+from ...utils import EvalFloat
 from ...vector import V
 from ..base import LabelShape
 
 
 class Block(LabelShape):
     text: str
     padding: V = V(0.1, 0.2)
-    radius: float = 0.3
-    angle: float = 15
+    radius: EvalFloat = 0.3
+    angle: EvalFloat = 15
 
     def draw(self, dwg: Drawing):
         g = Group()
         bg = Rect(
             insert=(0, 0),
             size=self.size.tuple,
             rx=self.radius,
```

### Comparing `boardgen-0.6.2/boardgen/shapes/label/io_line.py` & `boardgen-0.7.0/boardgen/shapes/label/io_line.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/shapes/label/label.py` & `boardgen-0.7.0/boardgen/shapes/label/label.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/shapes/rect.py` & `boardgen-0.7.0/boardgen/shapes/rect.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Copyright (c) Kuba Szczodrzyński 2022-05-12.
 
 from pydantic import Field
 from svgwrite import Drawing, shapes
 
+from ..utils import EvalFloat
 from ..vector import V
 from .base import Shape
 from .fill_style import FillStyle
 
 
 class Rect(Shape):
     size_v: V = Field(alias="size")
-    rx: float = None
-    ry: float = None
+    rx: EvalFloat = None
+    ry: EvalFloat = None
     fill: FillStyle = None
     stroke: FillStyle = None
 
     def draw(self, dwg: Drawing):
         if self.stroke and self.stroke.width:
             self.pos += (self.stroke.width / 2, self.stroke.width / 2)
             self.size_v -= (self.stroke.width, self.stroke.width)
```

### Comparing `boardgen-0.6.2/boardgen/shapes/text.py` & `boardgen-0.7.0/boardgen/shapes/text.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Copyright (c) Kuba Szczodrzyński 2022-05-12.
 
 from svgwrite import Drawing, text
 
+from ..utils import EvalFloat
 from .base import Shape
 from .fill_style import FillStyle
 
 
 class Text(Shape):
     text: str
-    font_size: float
+    font_size: EvalFloat
     fill: FillStyle = None
 
     def draw(self, dwg: Drawing):
         txt = text.Text(
             text=self.text,
             insert=self.pos.tuple,
             id=self.fullid,
```

### Comparing `boardgen-0.6.2/boardgen/utils.py` & `boardgen-0.7.0/boardgen/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,26 @@
 
 
 class Model(BaseModel):
     class Config:
         arbitrary_types_allowed = True
 
 
+class EvalFloat(float):
+    @classmethod
+    def __get_validators__(cls):
+        yield cls.validate
+
+    @classmethod
+    def validate(cls, v):
+        if isinstance(v, str):
+            return str_to_num(v)
+        return float(v)
+
+
 def var(s: str, vars: dict) -> str:
     s_prev = s
     while "${" in s:
         for key, value in vars.items():
             s = s.replace(f"${{{key}}}", str(value))
         if s == s_prev:
             # no replacements made anymore
```

### Comparing `boardgen-0.6.2/boardgen/variant/parts.py` & `boardgen-0.7.0/boardgen/variant/parts.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/variant/writer.py` & `boardgen-0.7.0/boardgen/variant/writer.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/boardgen/vector.py` & `boardgen-0.7.0/boardgen/vector.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.6.2/pyproject.toml` & `boardgen-0.7.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 [tool.poetry]
 name = "boardgen"
-version = "0.6.2"
-description = "Board pinout diagram generator"
+version = "0.7.0"
+description = "Board pinout diagram generator (with ltchiptool plugin GUI editor)"
 authors = ["Kuba Szczodrzyński <kuba@szczodrzynski.pl>"]
 license = "MIT"
 readme = "README.md"
+packages = [
+    { include = "boardgen" },
+    { include = "ltctplugin/boardgen" },
+]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^1.9.0"
 click = "^8.1.3"
 svgwrite = "^1.4.2"
 devtools = "^0.8.0"
```

### Comparing `boardgen-0.6.2/PKG-INFO` & `boardgen-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: boardgen
-Version: 0.6.2
-Summary: Board pinout diagram generator
+Version: 0.7.0
+Summary: Board pinout diagram generator (with ltchiptool plugin GUI editor)
 License: MIT
 Author: Kuba Szczodrzyński
 Author-email: kuba@szczodrzynski.pl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

