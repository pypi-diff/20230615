# Comparing `tmp/xplorts-0.5.tar.gz` & `tmp/xplorts-0.6.tar.gz`

## Comparing `xplorts-0.5.tar` & `xplorts-0.6.tar`

### file list

```diff
@@ -1,63 +1,68 @@
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 xplorts-0.5/.gitignore
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 xplorts-0.5/LICENSE
--rw-r--r--   0        0        0     9304 2020-02-02 00:00:00.000000 xplorts-0.5/README.md
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 xplorts-0.5/_NOTES.ipynb
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 xplorts-0.5/pyproject.toml
--rw-r--r--   0        0        0    52377 2020-02-02 00:00:00.000000 xplorts-0.5/data/oph annual bespoke.csv
--rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 xplorts-0.5/data/oph annual by division.csv
--rw-r--r--   0        0        0    20878 2020-02-02 00:00:00.000000 xplorts-0.5/data/oph annual by section.csv
--rw-r--r--   0        0        0    93088 2020-02-02 00:00:00.000000 xplorts-0.5/data/oph quarterly by section.csv
--rw-r--r--   0        0        0  2542592 2020-02-02 00:00:00.000000 xplorts-0.5/data/outputperhourworked.xls
--rw-r--r--   0        0        0  1285776 2020-02-02 00:00:00.000000 xplorts-0.5/docs/html/xplor_lprod oph annual by section.html
--rw-r--r--   0        0        0  1775672 2020-02-02 00:00:00.000000 xplorts-0.5/docs/html/xplor_lprod oph quarterly by section.html
--rw-r--r--   0        0        0    10443 2020-02-02 00:00:00.000000 xplorts-0.5/docs/png/slideselect_date.png
--rw-r--r--   0        0        0    10834 2020-02-02 00:00:00.000000 xplorts-0.5/docs/png/slideselect_industry.png
--rw-r--r--   0        0        0    46598 2020-02-02 00:00:00.000000 xplorts-0.5/docs/png/xplor_lprod_lines_thumbnail_large.png
--rw-r--r--   0        0        0    28431 2020-02-02 00:00:00.000000 xplorts-0.5/docs/png/xplor_lprod_snapcomp_thumbnail_large.png
--rw-r--r--   0        0        0    20261 2020-02-02 00:00:00.000000 xplorts-0.5/docs/png/xplor_lprod_thumbnail.png
--rw-r--r--   0        0        0    37746 2020-02-02 00:00:00.000000 xplorts-0.5/docs/png/xplor_lprod_tscomp_thumbnail_large.png
--rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/__init__.py
--rw-r--r--   0        0        0    32735 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/base.ipynb
--rw-r--r--   0        0        0    16036 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/base.py
--rw-r--r--   0        0        0    12058 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/dutils.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/ghostbokeh.py
--rw-r--r--   0        0        0     6615 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/slideselect.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/dblprod/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/dblprod/__main__.py
--rw-r--r--   0        0        0    19722 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/dblprod/dblprod.py
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/dblprod/prodgrowsnap.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/dblprod/prodgrowts.py
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/dblprod/prodlines.py
--rw-r--r--   0        0        0     8401 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/dblprod/xpdblprod.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/lines/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/lines/__main__.py
--rw-r--r--   0        0        0    13206 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/lines/lines.py
--rw-r--r--   0        0        0     6863 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/lines/xplines.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/scatter/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/scatter/__main__.py
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/scatter/scatter.py
--rw-r--r--   0        0        0     9992 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/scatter/xpscatter.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/snapcomp/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/snapcomp/__main__.py
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/snapcomp/snapcomp.py
--rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/snapcomp/xpsnapcomp.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/stacks/__init__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/stacks/__main__.py
--rw-r--r--   0        0        0     9599 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/stacks/bokeh_stacks.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/stacks/stacks.py
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/stacks/stacks_util.py
--rw-r--r--   0        0        0     8697 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/stacks/xpstacks.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/tscomp/__init__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/tscomp/__main__.py
--rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/tscomp/tscomp.py
--rw-r--r--   0        0        0     7899 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/tscomp/xptscomp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/utils/__init__.py
--rw-r--r--   0        0        0     8004 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/utils/ukons_lprod_to_csv.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 xplorts-0.5/tests/conftest.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 xplorts-0.5/tests/test_dblprod.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 xplorts-0.5/tests/test_lines.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 xplorts-0.5/tests/test_scatter.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 xplorts-0.5/tests/test_snapcomp.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 xplorts-0.5/tests/test_stacks.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 xplorts-0.5/tests/test_tscomp.py
--rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 xplorts-0.5/PKG-INFO
+-rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 xplorts-0.6/_NOTES.ipynb
+-rw-r--r--   0        0        0  1246655 2020-02-02 00:00:00.000000 xplorts-0.6/tt.html
+-rw-r--r--   0        0        0    52377 2020-02-02 00:00:00.000000 xplorts-0.6/data/oph annual bespoke.csv
+-rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 xplorts-0.6/data/oph annual by division.csv
+-rw-r--r--   0        0        0    20878 2020-02-02 00:00:00.000000 xplorts-0.6/data/oph annual by section.csv
+-rw-r--r--   0        0        0    93088 2020-02-02 00:00:00.000000 xplorts-0.6/data/oph quarterly by section.csv
+-rw-r--r--   0        0        0  2542592 2020-02-02 00:00:00.000000 xplorts-0.6/data/outputperhourworked.xls
+-rw-r--r--   0        0        0  1285776 2020-02-02 00:00:00.000000 xplorts-0.6/docs/html/xplor_lprod oph annual by section.html
+-rw-r--r--   0        0        0  1775672 2020-02-02 00:00:00.000000 xplorts-0.6/docs/html/xplor_lprod oph quarterly by section.html
+-rw-r--r--   0        0        0    10443 2020-02-02 00:00:00.000000 xplorts-0.6/docs/png/slideselect_date.png
+-rw-r--r--   0        0        0    10834 2020-02-02 00:00:00.000000 xplorts-0.6/docs/png/slideselect_industry.png
+-rw-r--r--   0        0        0    46598 2020-02-02 00:00:00.000000 xplorts-0.6/docs/png/xplor_lprod_lines_thumbnail_large.png
+-rw-r--r--   0        0        0    28431 2020-02-02 00:00:00.000000 xplorts-0.6/docs/png/xplor_lprod_snapcomp_thumbnail_large.png
+-rw-r--r--   0        0        0    20261 2020-02-02 00:00:00.000000 xplorts-0.6/docs/png/xplor_lprod_thumbnail.png
+-rw-r--r--   0        0        0    37746 2020-02-02 00:00:00.000000 xplorts-0.6/docs/png/xplor_lprod_tscomp_thumbnail_large.png
+-rw-r--r--   0        0        0   947883 2020-02-02 00:00:00.000000 xplorts-0.6/src/tt.html
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 xplorts-0.6/src/tt.py
+-rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/__init__.py
+-rw-r--r--   0        0        0    32735 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/base.ipynb
+-rw-r--r--   0        0        0    16803 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/base.py
+-rw-r--r--   0        0        0    12058 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/dutils.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/ghostbokeh.py
+-rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/slideselect.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/dblprod/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/dblprod/__main__.py
+-rw-r--r--   0        0        0    19722 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/dblprod/dblprod.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/dblprod/prodgrowsnap.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/dblprod/prodgrowts.py
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/dblprod/prodlines.py
+-rw-r--r--   0        0        0     8401 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/dblprod/xpdblprod.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/heatmap/__init__.py
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/heatmap/heatmap.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/lines/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/lines/__main__.py
+-rw-r--r--   0        0        0    13921 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/lines/lines.py
+-rw-r--r--   0        0        0     6863 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/lines/xplines.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/scatter/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/scatter/__main__.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/scatter/scatter.py
+-rw-r--r--   0        0        0    10074 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/scatter/xpscatter.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/snapcomp/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/snapcomp/__main__.py
+-rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/snapcomp/snapcomp.py
+-rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/snapcomp/xpsnapcomp.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/stacks/__init__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/stacks/__main__.py
+-rw-r--r--   0        0        0     9599 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/stacks/bokeh_stacks.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/stacks/stacks.py
+-rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/stacks/stacks_util.py
+-rw-r--r--   0        0        0     8683 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/stacks/xpstacks.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/tscomp/__init__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/tscomp/__main__.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/tscomp/tscomp.py
+-rw-r--r--   0        0        0     7899 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/tscomp/xptscomp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/utils/__init__.py
+-rw-r--r--   0        0        0     8004 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/utils/ukons_lprod_to_csv.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 xplorts-0.6/tests/conftest.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 xplorts-0.6/tests/test_dblprod.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 xplorts-0.6/tests/test_lines.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 xplorts-0.6/tests/test_scatter.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 xplorts-0.6/tests/test_snapcomp.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 xplorts-0.6/tests/test_stacks.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 xplorts-0.6/tests/test_tscomp.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 xplorts-0.6/.gitignore
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 xplorts-0.6/LICENSE
+-rw-r--r--   0        0        0     9304 2020-02-02 00:00:00.000000 xplorts-0.6/README.md
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 xplorts-0.6/pyproject.toml
+-rw-r--r--   0        0        0    15776 2020-02-02 00:00:00.000000 xplorts-0.6/PKG-INFO
```

### Comparing `xplorts-0.5/.gitignore` & `xplorts-0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/LICENSE` & `xplorts-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/README.md` & `xplorts-0.6/README.md`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/_NOTES.ipynb` & `xplorts-0.6/_NOTES.ipynb`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9614049145299145%*

 * *Differences: {"'cells'": "{0: {'id': 'bba9b8bb'}, 1: {'id': 'b553d7ca'}, 2: {'id': '779f4ad6'}, 3: {'id': "*

 * *            "'1e77bc6f', 'source': {insert: [(0, '#  "*

 * *            "https://packaging.python.org/en/latest/tutorials/packaging-projects/')]}}, 4: {'id': "*

 * *            "'e93e203e'}, 5: {'id': 'bc2e0f5e'}, 6: {'id': '5185b873'}, 7: {'id': '0c6051f0'}, 8: "*

 * *            "{'id': 'c29cc13b'}, 9: {'id': 'e88ad3a9'}, insert: [(10, OrderedDict([('cell_type', "*

 * *            "'markdown'), ('id', 'a7b41048'), ('metadata', Orde […]*

```diff
@@ -1,115 +1,174 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "a531217d",
+            "id": "bba9b8bb",
             "metadata": {},
             "source": [
                 "# Notes on preparing xplorts package\n",
                 "1. Prepare the package"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
-            "id": "38ef467d",
+            "id": "b553d7ca",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# (Terminal)\n",
                 "#> cd xplor_time_series\n",
                 "#> conda activate python36_plus_hv2\n",
                 "#> rm dist/*  # clear out old distributions"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "bb906b02",
+            "id": "779f4ad6",
             "metadata": {},
             "source": [
                 "2. Build the package and upload to PyPI or testpypi"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
-            "id": "27b12926",
+            "id": "1e77bc6f",
             "metadata": {},
             "outputs": [],
             "source": [
+                "#  https://packaging.python.org/en/latest/tutorials/packaging-projects/",
                 "#> python3 -m build\n",
                 "#> python3 -m twine upload --repository testpipy dist/*\n",
                 "\n",
                 "## Username:  __token__\n",
                 "## Password:  <paste in token>"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "5bd4bc96",
+            "id": "e93e203e",
             "metadata": {},
             "source": [
                 "3. Update pip (Mac only, maybe no longer required)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a667ff1b",
+            "id": "bc2e0f5e",
             "metadata": {},
             "outputs": [],
             "source": [
                 "## If pip is not at least 9.0.3\n",
                 "## If you are running macOS/OS X version 10.12 or older, then you ought to upgrade to the latest pip (9.0.3) \n",
                 "## https://stackoverflow.com/questions/49748063/pip-install-fails-for-every-package-could-not-find-a-version-that-satisfies#49748494\n",
                 "#> curl https://bootstrap.pypa.io/get-pip.py | python\n",
                 "#> pip install --upgrade setuptools"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "fecb4eed",
+            "id": "5185b873",
             "metadata": {},
             "source": [
                 "4. Make test environment and install package"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
-            "id": "40cebda5",
+            "id": "0c6051f0",
             "metadata": {},
             "outputs": [],
             "source": [
                 "#> conda env create -n xplorts \"python=3.6\"\n",
                 "#> conda activate xplorts"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
-            "id": "b4998559",
+            "id": "c29cc13b",
             "metadata": {},
             "outputs": [],
             "source": [
                 "#xplorts> pip install \"bokeh>=2.3.2\" \"numpy>=1.19.2\" \"pandas>=1.1.5\" \"pyyaml>=5.4.1\"\n",
                 "#xplorts> pip install --index-url https://test.pypi.org/simple/ --no-deps xplorts"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "3cc0d311",
+            "id": "e88ad3a9",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# does note work...\n",
                 "#xplorts> pip install \"bokeh>=2.3.2\" \"numpy>=1.19.2\" \"pandas>=1.1.5\" \"yaml>=0.2.5\"\n"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "a7b41048",
+            "metadata": {},
+            "source": [
+                "## Creating an environment with bokeh >= 3.1 to match ONS environment\n",
+                "\n",
+                "```\n",
+                "> conda create -n p38_xp python=3.8  # Try newer Python.\n",
+                "> conda activate p38_xp\n",
+                "> python -m pip install --upgrade pip\n",
+                "> python -m pip install xplorts\n",
+                "```\n"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "2eb81ccf",
+            "metadata": {},
+            "source": [
+                "#### Python versions older than 3.8 limit bokeh to earlier versions.\n",
+                "```\n",
+                "> conda create -n p36_xp --clone python36\n",
+                "> conda activate p36_xp\n",
+                "> python -m pip install xplorts\n",
+                "```\n",
+                "This installs bokeh 2.3.2."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "ca1cfa1d",
+            "metadata": {},
+            "source": [
+                "```\n",
+                "> conda create -n bokeh31 python=3.6 bokeh\n",
+                "```\n",
+                "This installs bokeh 1.4.  Why such early version?  Maybe because that's what's in the Anaconda install?\n",
+                "\n",
+                "```\n",
+                "> conda create -n bokeh31 python=3.6\n",
+                "> python -m pip install --upgrade pip\n",
+                "> python -m pip install --upgrade bokeh\n",
+                "```\n",
+                "This installed bokeh 2.3.3. New versions require more recent version of Python!\n",
+                "* [NO] pip might use local version from cache instead of newer version from pypi?  See https://stackoverflow.com/a/17153977/16327476\n",
+                "** Maybe try: conda -m pip install --no-cache-dir --upgrade bokeh\n",
+                "* Bokeh might have a requirement that interacts with obscure stuff we had to install to get Jupyter to work on our matchine?\n",
+                "\n",
+                "\n",
+                "```\n",
+                "> conda create -n p38_xp python=3.8  # Try newer Python.\n",
+                "> conda activate p38_xp\n",
+                "> python -m pip install --upgrade pip\n",
+                "> python -m pip install xplorts\n",
+                "```\n"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `xplorts-0.5/pyproject.toml` & `xplorts-0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xplorts"
-version = "0.5"
+version = "0.6"
 authors = [
   { name="Todd M Bailey", email="tmb@baileywick.plus.com" },
 ]
 description = "Make standalone interactive HTML charts to explore time series datasets"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `xplorts-0.5/data/oph annual bespoke.csv` & `xplorts-0.6/data/oph annual bespoke.csv`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/data/oph annual by division.csv` & `xplorts-0.6/data/oph annual by division.csv`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/data/oph annual by section.csv` & `xplorts-0.6/data/oph annual by section.csv`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/data/oph quarterly by section.csv` & `xplorts-0.6/data/oph quarterly by section.csv`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/data/outputperhourworked.xls` & `xplorts-0.6/data/outputperhourworked.xls`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/docs/html/xplor_lprod oph annual by section.html` & `xplorts-0.6/docs/html/xplor_lprod oph annual by section.html`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/docs/html/xplor_lprod oph quarterly by section.html` & `xplorts-0.6/docs/html/xplor_lprod oph quarterly by section.html`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/docs/png/slideselect_date.png` & `xplorts-0.6/docs/png/slideselect_date.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/docs/png/slideselect_industry.png` & `xplorts-0.6/docs/png/slideselect_industry.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/docs/png/xplor_lprod_lines_thumbnail_large.png` & `xplorts-0.6/docs/png/xplor_lprod_lines_thumbnail_large.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/docs/png/xplor_lprod_snapcomp_thumbnail_large.png` & `xplorts-0.6/docs/png/xplor_lprod_snapcomp_thumbnail_large.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/docs/png/xplor_lprod_thumbnail.png` & `xplorts-0.6/docs/png/xplor_lprod_thumbnail.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/docs/png/xplor_lprod_tscomp_thumbnail_large.png` & `xplorts-0.6/docs/png/xplor_lprod_tscomp_thumbnail_large.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/src/xplorts/__init__.py` & `xplorts-0.6/src/xplorts/__init__.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/src/xplorts/base.ipynb` & `xplorts-0.6/src/xplorts/base.ipynb`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/src/xplorts/base.py` & `xplorts-0.6/src/xplorts/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,27 +38,46 @@
 
 #%%
 
 from bokeh import palettes
 from bokeh.io import output_file
 from bokeh.models import (CDSView, ColumnDataSource, CustomJS, GroupFilter, FactorRange, 
                           HoverTool, Legend, LegendItem)
-from bokeh.models.formatters import FuncTickFormatter
+from bokeh.models import formatters as bk_formatters
+#from bokeh.models.formatters import FuncTickFormatter
 from bokeh.plotting import figure
+from bokeh.util.warnings import BokehDeprecationWarning
+
+import functools
+import operator
 
 import pandas as pd
 from pandas.api.types import is_datetime64_any_dtype as is_datetime
 from pathlib import Path
 
+import warnings
+
 # Imports from this package.
 from xplorts.dutils import dict_fill
 from xplorts.slideselect import SlideSelect
 
 #%%
 
+# Use CustomJSTickFormatter for newer bokeh, or 
+# FuncTickFormatter for older bokeh.    
+def _custom_tick_formatter(code):
+    try:
+        cls = bk_formatters.CustomJSTickFormatter
+    except AttributeError:
+        cls = bk_formatters.FuncTickFormatter
+    return cls(code=code)
+
+
+#%%
+
 def add_hover_tool(fig, renderers, *tooltips, simplify=True, **kwargs):
     """
     Add a hover tool to a Bokeh figure, for given renderers
     
     Parameters
     ----------
     fig : Bokeh Figure
@@ -247,19 +266,41 @@
          columns=["industry", "year", "sales"]
     )
     cds = ColumnDataSource(data)
     view = factor_view(cds, "category")
     """
     
     assert isinstance(source, ColumnDataSource), f"source must be ColumnDataSource, not {type(source)}"
-    
-    view = CDSView(
-        source=source,
-        filters=factor_filters(by, source=source, **kwargs)
-    )
+
+    # Get list of one or more filters.
+    filters = factor_filters(by, source=source, **kwargs)
+    with warnings.catch_warnings():
+        # Catch deprecations from bokeh CDSView if necessary.
+        warnings.simplefilter("error")
+        try:
+            # Use legacy call with gratuitous CDSView.source property.
+            view = CDSView(
+                source=source,
+                filters=filters
+            )
+        except (AttributeError, BokehDeprecationWarning):
+            # Use newer call without CDSView.source property.
+            if len(filters):
+                if len(filters) == 1:
+                    # use the single filter as is.
+                    filter = filters[0]
+                else:
+                    # Combine multiple filters with logical `and`.
+                    filter = functools.reduce(operator.and_, filters)
+                    
+                view = CDSView(filter=filter)
+            else:
+                # No filters to apply.
+                view = CDSView()
+        
     return view
 
 
 def filter_widget(options, title=None, start_value="first"):
     """
     Make a widget to select among values of a sequence
     """
@@ -333,15 +374,15 @@
     fopts.update(kwargs)
     fig = figure(**fopts)
     
     if suppress_factors:
         # Suppress most lowest level categorical tick labels.
         # If tick labels are tuples, higher levels will be displayed
         # as normal.
-        tf_margins_only = FuncTickFormatter(
+        tf_margins_only = _custom_tick_formatter(
             code="""
             if ((index == 0) | (index == ticks.length - 1)) {
                 return tick;
             } else {
                 return '';
             }
             """
@@ -357,30 +398,28 @@
         fig.add_layout(legend, place=legend_place)
     
     fig.toolbar.logo = None
     
     return fig
 
 
-def link_widgets_to_groupfilters(widgets, view=None, source=None, filters=None):
+def link_widgets_to_groupfilters(widgets, source, filter):
     """
     Link values of widgets to corresponding GroupFilter objects
     
     Parameters
     ----------
     widgets : Bokeh widget or list of widgets
         The `value` property of each widget will be linked to the
         `group` property of the corresponding `GroupFilter`.  If there are
         more widgets than filters, the excess widgets are ignored.
-    view : CDSView, optional
-        Provides `source` and `filters` if they are not specified directly.
     source : ColumnDataSource
         Data source, which will be configured to emit a change signal when
         a filter's `group` property changes, to re-render the relevant figure.
-    filters : GroupFilter or sequence of GroupFilter
+    filter : GroupFilter or sequence of GroupFilter
         The `group` property of each filter will be updated whenever the
         `value` of the corresponding widget changes, and `source` will emit
         a change signal whenever the `group` property of a filter changes.  If
         there are more filters than widgets, excess filters are ignored.
     
     Examples
     --------
@@ -388,39 +427,25 @@
     from base import factor_view
     source = ColumnDataSource({"industry": ["A", "B"],
                                "growth": [10, 12]})
     view_by_factor = factor_view(source, "industry")
     widget = SlideSelect(options=["A", "B"],
                          name="industry_filter")  # Show this in a layout.
     link_widgets_to_groupfilters(widget, 
-                                 view=view_by_factor)
-    
-    # Source and filter can be specified directly.
-    link_widgets_to_groupfilters(widget, 
                                  source=source,
-                                 filters=view_by_factor.filters)
+                                 filter=view_by_factor.filters)
     """
-
-    if all(x is None for x in (view, source, filters)):
-        raise ValueError("Must either specify source and filters, or view")
-    
-    if source is None:
-        source = view.source
-    
-    if filters is None:
-        # Find filters in view, assumed to correspond to widgets.
-        filters = view.filters
     
     # Wrap singleton widget or filter, for convenience.
     if not isinstance(widgets, (list, tuple)):
         widgets = [widgets]
-    if not isinstance(filters, (list, tuple)):
-        filters = [filters]
+    if not isinstance(filter, (list, tuple)):
+        filter = [filter]
         
-    for widget, filt in zip(widgets, filters):
+    for widget, filt in zip(widgets, filter):
         # Link widget to the GroupFilter.
         assert isinstance(filt, GroupFilter)
         widget.js_link("value", other=filt, other_attr="group")
 
         # Signal change in data when filter `group` attribute changes, 
         # so chart refreshes.
         filt.js_on_change(
```

### Comparing `xplorts-0.5/src/xplorts/dutils.py` & `xplorts-0.6/src/xplorts/dutils.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/src/xplorts/ghostbokeh.py` & `xplorts-0.6/src/xplorts/ghostbokeh.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/src/xplorts/slideselect.py` & `xplorts-0.6/src/xplorts/slideselect.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,57 +13,57 @@
 """
 
 # =============================================================================
 # To do
 # Allow options from dict
 #
 # Suppress hover display on slider
-# 
+#
 # =============================================================================
 
 from bokeh.models import Column, CustomJS, Div, Select, Slider
 from bokeh.layouts import column, row
 from bokeh.io import show
 
 from xplorts.ghostbokeh import GhostBokeh
 
 #%%
 
 class SlideSelect(GhostBokeh, Column):
     """
     A bokeh combination widget that can be linked to Javascript callbacks
-    
+
     Includes support for options that are strings, or dictionaries
     that map to strings.
-    
+
     This class helps to create interactive objects with Bokeh, but does not
     sync with those objects after they go live in a browser.
-    
+
     Properties
     -------
     handle
         An object that can be linked to Javascript for interactively
         responding to changes in the selected value. Read-only.
-    
+
     options: list
         List of select options.  Read-only.
-    
+
     value: str
         Selected value.  Read/write.  Does not sync with the widget after it
         goes live in a browser.
     """
 
     #_js_option_array = None
 
     def __new__(cls, options, *args, title="Selection", **kwargs):
         option_keys = (
             list(options.keys()) if isinstance(options, dict)
             else options
         )
-        
+
         bk_select = Select(options=option_keys, value=option_keys[0], title=title)
         bk_slider = Slider(start=0, end=len(options)-1, value=0, step=1, title=None)
 
         # Link select option to slider value.
         bk_select.js_on_change('value',
             CustomJS(args={"other": bk_slider},
                      code="other.value = this.options.indexOf(this.value) \n" \
@@ -83,135 +83,136 @@
             bk_select,
             bk_slider
         ]
 
         # Make a bokeh layout, and coerce the class type.
         obj = column(*args, children=children, **kwargs)  # Force consistent child sizing.
         obj.__class__ = cls
-        
+
         # Use bokeh model for Column to generate javascript to display this object.
         obj.__qualified_model__ = "Column"
 
         return obj
-    
+
     def __init__(self, options, *args, **kwargs):
         """
         Creates a subclass of Bokeh Column that contains a drop-down select
         widget and a slider widget for a common set of options.
-        
+
         Parameters
         ----------
         options : dict, or iterable
             Options to be assigned to the browser-side `_js_option_array`.
-            
+
         args, kwargs
             Other other arguments are used by `__new__`.
         """
         option_values = (
             list(options.values()) if isinstance(options, dict)
             else options
         )
         self._js_option_array = option_values
 
 
     @property
     def _js_value_str(self):
         """
         Javascript code snippet to retrieve selected value
-        
+
         The selected value is placed in X_value, where X is
         the `.name` attribute of the selection widget.
         """
         if self._js_option_array is None:
             js_code = f"const {self.name}_value = {self.name}.value"
         else:
             js_code = f"""
                 const {self.name}_lookup = {self._js_option_array}
                 const {self.name}_value = {self.name}_lookup[{self.name}.value]
             """
         return js_code
-    
+
     @property
     def handle(self):
         """
         Object that can be linked to Javascript for standalone interactivity
         """
         return self.children[0]
 
     @property
     def options(self):
         """
         List of options available for selection.
         """
         return self.handle.options
-    
+
     @property
     def value(self):
         """
         Selected value.  Read/write.  Does not sync with the widget after it
         goes live in a browser.
         """
         return self.handle.value
-    
+
     @value.setter
     def value(self, value):
         """Set server-side widget value"""
         bk_select, bk_slider = self.children
         bk_slider.value = bk_select.options.index(value)
         bk_select.value = value
-    
+
 ## Define js_link() et al to access properties of select widget if necessary.
 
 def flexi_method(method_name):
     """
     Return an instance method that applies a named method flexibly
-    
+
     Parameters
     ----------
     method_name: str
         Method to apply.
-    
+
     Return
     ------
     Instance method, with signature (self, *args, **kwargs).
-    
-        The named method is sought first in the instance's super-class.  
-        If not found in the super-class, or if found but it returns a 
-        ValueError, then the named method is sought in the first of the 
+
+        The named method is sought first in the instance's super-class.
+        If not found in the super-class, or if found but it returns a
+        ValueError, then the named method is sought in the first of the
         instance's .children.
-    
+
     Examples
     --------
     class MyClass(Column):
         js_link = flexi_method("js_link")
-    
-    
+
+
     """
     def wrapper(self, *args, **kwargs):
         try:
             # Apply method to whole container, if possible.
             super_class = super(type(self), self)
             result = getattr(super_class, method_name)(*args, **kwargs)
         except (ValueError, AttributeError):
             # Apply to select widget.
             result = getattr(self.children[0], method_name)(*args, **kwargs)
         return result
     return wrapper
-    
+
 # Monkey patch SlideSelect.js_*() methods.
-js_methods = [method for method in dir(SlideSelect) if method.startswith("js_")]
+# js_methods = [method for method in dir(SlideSelect) if method.startswith("js_")]
+js_methods = ["js_link", "js_on_change", "js_on_event"]
 for method_name in js_methods:
     setattr(SlideSelect, method_name, flexi_method(method_name))
 
 
 #%% Move to test?
 
 if False:
     ss = SlideSelect(options=["a", "b", "c"])
-    
+
     result = Div(
         text="""
             <p>?</p>
             """,
         width=200,
         height=30,
     )
```

### Comparing `xplorts-0.5/src/xplorts/dblprod/__init__.py` & `xplorts-0.6/src/xplorts/dblprod/__init__.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/src/xplorts/dblprod/dblprod.py` & `xplorts-0.6/src/xplorts/dblprod/dblprod.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/src/xplorts/dblprod/prodgrowsnap.py` & `xplorts-0.6/src/xplorts/dblprod/prodgrowsnap.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/src/xplorts/dblprod/prodgrowts.py` & `xplorts-0.6/src/xplorts/dblprod/prodgrowts.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/src/xplorts/dblprod/prodlines.py` & `xplorts-0.6/src/xplorts/dblprod/prodlines.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/src/xplorts/dblprod/xpdblprod.py` & `xplorts-0.6/src/xplorts/dblprod/xpdblprod.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/src/xplorts/lines/lines.py` & `xplorts-0.6/src/xplorts/lines/lines.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Functions
 ---------
 grouped_multi_lines
     Add a multi-line plot to a figure, with legend entries and hover tooltip.
 
 link_widget_to_lines
-    Arrange to update the `visible` property of multi-line renderers 
+    Arrange to update the `visible` property of multi-line renderers
     in the browser when a selection changes.
 """
 
 #%%
 from bokeh import palettes
 from bokeh.layouts import layout
 from bokeh.models import (ColumnDataSource, CustomJS, CustomJSHover, LegendItem)
@@ -27,32 +27,32 @@
 
 
 #%%
 
 def link_widget_to_lines(widget, renderers):
     """
     Attach callback to selection widget, to update visibility of renderers
-    
+
     The JS callback is triggered by changes to the `value` property of
     the widget.  When triggered, the callback hides the current renderer
     and unhides the renderer indexed by the new value of the widget.
-    
+
     The first time it is triggered the callback hides the first renderer.
     To work correctly with a different initial visible renderer other than
-    renderers[0], set the `.option_index` property of the widget to the 
+    renderers[0], set the `.option_index` property of the widget to the
     index of the initial visible renderer.
-    
+
     Parameters
     ----------
     widget: Bokeh widget or layout
         May be an object with a `value` attribute and a method `js_on_change()`,
-        like a Bokeh widget.  Alternatively, may be an object with a `handle` 
+        like a Bokeh widget.  Alternatively, may be an object with a `handle`
         attribute which is itself an object with a `value` attribute and a method
         `js_on_change()`, like a `SlideSelect` layout of two widgets.
-    
+
     renderers: list
         List of Bokeh renderers, typically from the `renderers` property of a
         Bokeh `figure`.  The callback will set the `visible` property of individual
         renderers to hide the currently visible one and unhide the one selected
         by the new value of `widget`.
     """
     # Get widget handle (e.g. for SlideSelect), else link directly to widget.
@@ -66,23 +66,23 @@
                 console.log('> JS callback');
                 const option_index = this.options.indexOf(this.value);
 
                 if (!("recent_index" in this))
                     this.previous_index = 0;  // Assume first glyph might be visible.
                 else if (option_index != this.recent_index)
                     this.previous_index = this.recent_index;
-                                
+
                 // Hide currently visible glyph.
                 glyphs[this.previous_index].visible = false;
                 console.log('Made glyph ' + this.option_index + ' INvisible');
 
                 // Show glyph currently selected by widget.
                 glyphs[option_index].visible = true;
                 console.log('Made glyph ' + option_index + ' visible');
-                
+
                 // Save current option_index to check next time.
                 this.recent_index = option_index;
             """
         ))
 
 
 
@@ -96,112 +96,129 @@
             var result = value[special_vars["segment_index"]];
         else
             // Use (scalar?) value directly.
             result = value;
         return "" + result;
     """)
 
+# Flexible formatter to pick one number out of a list (as for
+# multi_line `xs` or `ys`), and format it with one decimal place.
+# Safe to use on scalar values too.
+# Intl.NumberFormat('de-DE', { minimumFractionDigits: 2, maximumFractionDigits: 2 }).format(num)
+#  https://stackoverflow.com/a/69647144/16327476
+_hover_segment_fixedvalue = CustomJSHover(
+    code="""
+        console.log("> _hover_segment_fixedvalue", value);
+        if (Array.isArray(value))
+            // Index into value with segment_index (e.g. for multi-line).
+            var result = value[special_vars["segment_index"]];
+        else
+            // Use (scalar?) value directly.
+            result = value;
+        result = Intl.NumberFormat('en-US', { minimumFractionDigits: 1, maximumFractionDigits: 1 }).format(result);
+        return "" + result;
+    """)
 
 #%%
 
 class _MultilineDataBuilder():
     """
     Maps names of columns to lists of lists, or sequences or arrays
-    
-    A class with helper methods to build 
+
+    A class with helper methods to build
     columns appropriate for `multi_line` glyphs.
-    
+
     Methods
     -------
-    
+
     """
-    
+
     data = pd.DataFrame()
-    
+
     def __init__(self, xs, data_variables=None, iv_variable=None, hover_data=None,
                  options={}, **kwargs):
-    
+
         if iv_variable is None:
             iv_variable = xs.name
         xs = list(xs)
-        
+
         if data_variables is None:
             if kwargs == {}:
                 raise ValueError("missing data_variables")
             # Use (first) kwarg as column name for list of variable names.
             index_name, data_variables = kwargs.pop(next(iter(kwargs)))
-            
+
             # Give warning about excess kwargs.
             if len(kwargs):
                 warnings.warn(f"extra keywords ignored: {kwargs.keys()}")
         else:
             # Define default name for column of variable names.
             index_name = "variable"
 
         # Start dataframe with one row per variable.
         index = pd.Index(data_variables, name=index_name)
         self.data = pd.DataFrame(index=index)
 
         # Use same independent axis for each variable.
         self.fill_column(iv_variable, xs)
-        
+
         if hover_data is not None:
             # Use same IV axis hover data for each variable.
             self.fill_column(hover_data.name, list(hover_data))
-        
+
         self.options(options)
-        
+
     def fill_column(self, column, value):
         """
         Assign the same value to each row
         """
-        
+
         self.data[column] = [value] * len(self.data.index)
-    
+
     def set_column(self, column, values):
         """
         Assign values to corresponding rows of a column
-        
+
         Values can be a scalar, a list with one value per row,
         a Series, or a mapping.
         """
-        
+
         # Coerce setting to Series compatible with .data.
         #  - Scalar will broadcast to fill column.
         #  - List must be same length as .data.index.
         #  - Mapping or series will use keys to match index.
         s = pd.Series(values, index=self.data.index)
         self.data[column] = s
 
     def options(self, *args, **kwargs):
         """
         Set columns with per-variable values
         """
-        
+
         if len(args):
             assert len(args) == 1, "expected at most one positional argument"
             assert isinstance(args[0], dict), "positional argument should be a mapping"
             # Use positional argument as mapping, overriden by any kwargs.
             kwargs = {**(args[0]), **kwargs}
 
         for option_name, setting in kwargs.items():
             self.set_column(option_name, setting)
 
     @property
     def as_cds(self):
         """
         Coerce data to ColumnDataSource suitable for multi_line()
         """
-        
+
         # Coerce to dict of dict; {column: {row: value, ...}, ...}.
         dod = self.data.reset_index().to_dict()
         # Collapse to dict of lists; {column: [value, ...], ...}.
         dol = {column: list(d.values()) for column, d in dod.items()}
         return ColumnDataSource(dol)
-        
+
 
 #%%
 
 def grouped_multi_lines(
     fig,
     data,
     iv_variable,
@@ -209,74 +226,74 @@
     by = None,
     cds_options={},
     tooltips=[],  # optional
     **kwargs):
     """
     Add multi_line chart overlays to a plot, for time series data with
     a set of factor levels.
-    
-    Adds to a Bokeh `figure`, one `multi_line` glyph for each unique value of 
+
+    Adds to a Bokeh `figure`, one `multi_line` glyph for each unique value of
     `by`, with legend entries and hover tooltip.
-    
+
     Dates are plotted along the horizontal axis.  The first `multi_line`
     is initially visible and the rest are hidden by setting their `visible`
     property to `False`.
-    
+
     Parameters
     ----------
     fig: Bokeh Figure
         Figure to add to.
     data: DataFrame, DataFrameGroupBy
         Data columns must include a date variable, a categorical factor variable,
         and one or more value variables.
     iv_variable: str or dict
         If str, the name of a data column, which will be shown on the horizontal
-        axis.  
-        
+        axis.
+
         If dict, should map key "plot" to a variable to show on the
         horizontal axis and should map key "hover" to a corresponding variable
         to display in hover information.  This is often useful when displaying
         quarterly dates as nested categories like `("2020", "Q1")`.
     data_variables: list
         Names of data columns.  The chart will show a line for each data
         variable.
     by: str, default None
-        Name of a categorical factor variable.  Required if `data` is a 
-        `DataFrame`, ignored if `data` is a `DataFrameGroupBy` object.  
+        Name of a categorical factor variable.  Required if `data` is a
+        `DataFrame`, ignored if `data` is a `DataFrameGroupBy` object.
         A multi_line glyph will be created for each unique value of the
         `by` variable.
     cds_options: dict, default {}
        Mapping from column names to lists, to specify plotting attributes
        for multi_lines.  Each list should have a value for each of the
        data_variables, in the same order.
     tool_tips: list, default []
         Pre-existing tooltips to add to the hover tool in addition to the
         default tooltips.
     """
-    
+
     if data_variables in (None, []):
         # Return empty list of renderers.
         return []
-    
+
     # Wrap single data variable in list if necessary.
     if isinstance(data_variables, str):
         data_variables = [data_variables]
-    
+
     if isinstance(data, DataFrameGroupBy):
         grouped = data
     else:
         # Group data, preserving order of `by`.
         grouped = data.groupby(by=by, sort=False)
-    
+
     if isinstance(iv_variable, dict):
         iv_plot_variable = iv_variable["plot"]
         iv_hover_variable = iv_variable["hover"]
     else:
         iv_plot_variable = iv_hover_variable = iv_variable
-    
+
     # Make template multi_line_data based on first group.
     _, df0 = next(iter(grouped))
     mldata = _MultilineDataBuilder(
         df0[iv_plot_variable],
         data_variables,
         hover_data = (df0[iv_hover_variable] if iv_hover_variable != iv_plot_variable
                       else None),
@@ -290,62 +307,64 @@
         mldata.set_column(
             "value",
             [list(group_df[var]) for var in data_variables]
         )
         mldata.set_column("group", group_name)
 
         fig.multi_line(
-            xs=iv_plot_variable, 
+            xs=iv_plot_variable,
             ys="value",
             name="lines_" + group_name,
             source=mldata.as_cds,
             visible=False,
             **kwargs
         )
-        
+
     lines = fig.renderers[next_renderer_idx:]
 
     # Show first set of lines.
     first_multi_line = lines[0]
     first_multi_line.visible = True
 
     # Add to legend.
     new_legend_items = [
             # Include legend item for each variable,
             #  using styles from the first multi_line renderer.
-            LegendItem(label=var, 
-                       renderers=[first_multi_line], 
+            LegendItem(label=var,
+                       renderers=[first_multi_line],
                        index=i
                       ) \
             for i, var in enumerate(data_variables)
     ]
     extend_legend_items(
         fig,
         items=new_legend_items,
     )
-    
-    
+
+
     ## Define hover info for lines.
     # Show name of hovered glyph, along with hover-date and the value.
-    lines_tooltip = f"@variable @{iv_hover_variable}{{custom}}: $data_y{{0,0.0}}"
-    add_hover_tool(fig, lines, 
-                   ("line", lines_tooltip), 
+    # lines_tooltip = f"@variable @{iv_hover_variable}{{custom}}: $data_y{{0,0.0}}"
+    lines_tooltip = f"@variable @{iv_hover_variable}{{custom}}: @value{{custom}}"
+    add_hover_tool(fig, lines,
+                   ("line", lines_tooltip),
                    (by if by is not None else "group", "@group"),
                    *tooltips,
                    attachment="vertical",
-                   formatters={f'@{iv_hover_variable}': _hover_segment_value},
+                   formatters={f'@{iv_hover_variable}': _hover_segment_value,
+                               '@value': _hover_segment_fixedvalue},
                    name="Hover lines",
                    description="Hover lines",
                   )
 
     return(lines)
 
 
 #%% Move to test.
-    
+
 if False: #__name__ == "__main__":
     # Make a test chart to show in Jupyter.
     df_data = pd.DataFrame.from_records([
         dict(date=2001, industry='A', gva_idx=100, hours_idx=100),
         dict(date=2002, industry='A', gva_idx=105, hours_idx=102),
         dict(date=2003, industry='A', gva_idx=110, hours_idx=105),
         dict(date=2001, industry='B', gva_idx=100, hours_idx=100),
@@ -355,26 +374,26 @@
     df_data["oph_idx"] = 100 * df_data["gva_idx"] / df_data["hours_idx"]
     df_data["periodicity"] = "annual"
 
     # Make standard date variables.
     df_data["date"] = pd.to_datetime(df_data["date"].astype(str)).dt.to_period("A")
     df_data["year"] = df_data["date"].dt.year
     df_data["quarter"] = df_data["date"].dt.quarter
-    
+
     # Make a slide-select widget to choose industry.
     widget = SlideSelect(options=list(df_data["industry"].unique()),
                          name="industry_select")
-    
-    fig = grouped_multi_lines(df_data, 
+
+    fig = grouped_multi_lines(df_data,
                               data_variables=["oph_idx", "gva_idx", "hours_idx"],
                               palette=palettes.Category20_3[::-1],
                               by="industry",
                               line_style_map={"hours_idx": "dashed"},
                               widget=widget)
-    
+
     app = layout([
         [widget],
         [fig]
     ])
 
     show(app)
```

### Comparing `xplorts-0.5/src/xplorts/lines/xplines.py` & `xplorts-0.6/src/xplorts/lines/xplines.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/src/xplorts/scatter/scatter.py` & `xplorts-0.6/src/xplorts/scatter/scatter.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/src/xplorts/scatter/xpscatter.py` & `xplorts-0.6/src/xplorts/scatter/xpscatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Make standalone interactive marker charts for categorical data
 
 When run from the command line, reads data from a `csv` file and
 creates an HTML document that displays an interactive line chart.
-    
-    In the `csv` file, the first row of data defines column names.  
+
+    In the `csv` file, the first row of data defines column names.
     The file should include:
-        - a column of independent variable categories, 
-        - a column of category names for a split factor, and 
+        - a column of independent variable categories,
+        - a column of category names for a split factor, and
         - one or more columns of data values to be plotted as markers
-          against the independent variable.  
-    
+          against the independent variable.
+
     An interactive chart is created, with widgets to select one of the split
     factor category names (from a pulldown list or a slider), and a chart with
     one series of markers for each value column.  The independent variable is
     plotted against either the x or y axis.
 
 
 Command line interface
@@ -58,86 +58,86 @@
 import pandas as pd
 from pathlib import Path
 import sys
 import yaml
 
 ## Imports from this package
 from xplorts.scatter import grouped_scatter
-from xplorts.base import (factor_view, 
-                          filter_widget, iv_dv_figure, 
+from xplorts.base import (factor_view,
+                          filter_widget, iv_dv_figure,
                           link_widgets_to_groupfilters, set_output_file, variables_cmap)
 from xplorts.slideselect import SlideSelect
 
 #%%
 
 def _parse_args():
     """
     Parse command line arguments
-    
+
     Returns
     -------
     `argparse.Namespace` object
-    
+
     Examples
     --------
     args = _parse_args()
     data = pd.read_csv(args.datafile)
-    
+
     Resources
     ---------
     [argparse — Parser for command-line options, arguments and sub-commands](https://docs.python.org/3/library/argparse.html#dest)
     """
     # Check command line arguments.
     parser = argparse.ArgumentParser(
         prog="python -m xplorts.scatter",
         description="Create interactive scatter plot for data series with a split factor"
     )
-    parser.add_argument("datafile", 
+    parser.add_argument("datafile",
                         help="File (CSV) with data series and split factor")
     parser.add_argument("-b", "--by", type=str,
                         help="Factor variable for splits")
 
     iv_group = parser.add_mutually_exclusive_group()
     iv_group.add_argument("-x", type=str,
                           help="Independent variable, for horizontal axis")
     iv_group.add_argument("-y", type=str,
                           help="Independent variable, for vertical axis")
 
     parser.add_argument("-m", "--marker", type=str,
                         help="Shape to use for markers.  Passed to Bokeh `Figure.scatter()`.")
 
-    parser.add_argument("-v", "--values", 
+    parser.add_argument("-v", "--values",
                         nargs="+", type=str,
                         help="Dependent variables to plot against independent variable")
-    
-    parser.add_argument("-g", "--args", 
+
+    parser.add_argument("-g", "--args",
                         type=str,
                         help="Keyword arguments for grouped_scatter(), specified as YAML mapping")
 
-    parser.add_argument("-t", "--save", type=str, 
+    parser.add_argument("-t", "--save", type=str,
                         help="Name of interactive .html to save, if different from the datafile base")
 
-    parser.add_argument("-s", "--show", action="store_true", 
+    parser.add_argument("-s", "--show", action="store_true",
                         help="Show interactive .html")
     args = parser.parse_args()
 
     # Unpack YAML args into dict of keyword args for grouped_multi_lines().
     args.args = {} if args.args is None else yaml.safe_load(args.args)
     return(args)
 
 #%%
 def main():
     """
     Parse command line arguments and make a scatter chart
     """
-    
+
     args = _parse_args()
 
     data = pd.read_csv(args.datafile, dtype=str)
-    
+
     # Unpack args specifying which columns to use.
     if all(getattr(args, arg) is None for arg in ["x", "y", "by", "values"]):
         # Get datevar from first column, byvar from second, values from remaining.
         iv_axis = "x"
         iv_variable, byvar = data.columns[:2]
         datavars = data.columns[2:]
     else:
@@ -146,38 +146,41 @@
         datavars = args.values
         if args.x is not None:
             iv_axis = "x"
             iv_variable = args.x
         else:
             iv_axis = "y"
             iv_variable = args.y
-            
+
     marker = args.marker or "circle"
-    
+
     title = "scatter: " + Path(args.datafile).stem
-    
+
     # Configure output file for interactive html.
     set_output_file(
         args.save or args.datafile,
         title = title
     )
-    
+
     # Convert str to float so we can plot the data.
     data[datavars] = data[datavars].astype(float)
-    
+
     # Make a slide-select widget to choose factor level.
     widget = SlideSelect(options=list(data[byvar].unique()),
                          name=byvar + "_select")
 
     source = ColumnDataSource(data)
     view_by_factor = factor_view(source, byvar)
+    # Get .filter attribute (newer bokeh) or .filters (pre bokeh 3.0).
+    filter = getattr(view_by_factor, "filter", None) or view_by_factor.filters
+
+    link_widgets_to_groupfilters(widget,
+                                 source=source,
+                                 filter=filter)
 
-    link_widgets_to_groupfilters(widget, 
-                                 view=view_by_factor)
-    
     # Map variables to colors.
     default_color_map = variables_cmap(datavars,
                                        "Category10_10")
 
     # Labels for axis.
     iv_data = data[iv_variable].unique()
     iv_data = reversed(iv_data) if iv_axis == "y" else list(iv_data)
@@ -195,33 +198,33 @@
             iv_variable=iv_variable,
             marker_variable=var,
             marker=marker,
             source=source,
             view=view_by_factor,
             color=default_color_map[var],
             **args.args)
-    
+
     # Make app that shows widget and chart.
     app = layout([
         Div(text="<h1>" + title),  # Show title as level 1 heading.
         [widget],
         [fig]
     ])
-    
+
     if args.show:
         show(app)  # Save file and display in web browser.
     else:
         save(app)  # Save file.
 
-    
+
 if __name__ == "__main__":
     sys.exit(main())
 
 #%% Move to test
-    
+
 if False:
     df_data = pd.DataFrame([
         (2001, 'A', 100, 100),
         (2002, 'A', 105, 102),
         (2003, 'A', 110, 105),
 
         (2001, 'B', 100, 100),
@@ -246,21 +249,21 @@
     df_growth = df_data.copy().reset_index(drop=True)
     df_growth["growth_offset"] = pd.to_datetime("2001").year - df_growth["date"].dt.year
 
     # Apply offset to data variables to calculate growths.
     baseline_index = df_growth.index + df_growth["growth_offset"]
     baseline = df_growth[data_variables].iloc[baseline_index, :].reset_index(drop=True)
     df_growth[data_variables] = (df_growth[data_variables] / baseline - 1) * 100
-    
+
     # Reverse sign where relevant.
     df_growth[sign_reverse_variables] *= -1
     sign_reverse_map = {name: name + " (sign reversed)" for name in sign_reverse_variables}
     df_growth.rename(columns=sign_reverse_map, inplace=True)
     growth_variables = [sign_reverse_map.get(name, name) for name in data_variables]
-        
+
     factor = "industry"
     factor_levels = sorted(df_data[factor].unique())
 
     #dates = sorted(df_data["date"].unique())
 
     ##df_growth.to_csv("oph_gva_hours_growth_by_ab.csv")
 
@@ -299,15 +302,15 @@
         widget=filter_widget,
         color_map={},
         palette=None,
         fig=None,
         fig_options={}
     )
 
-    
+
 
     # Make app that shows widget and chart.
     app = layout([
         [filter_widget],
         [fig, hbars]
     ])
```

### Comparing `xplorts-0.5/src/xplorts/snapcomp/__init__.py` & `xplorts-0.6/src/xplorts/snapcomp/__init__.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/src/xplorts/snapcomp/snapcomp.py` & `xplorts-0.6/src/xplorts/snapcomp/snapcomp.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,78 +31,78 @@
     scatter_args={},
     bar_args={},
 ):
     """
     Interactive chart showing snapshot components and total by split group
     """
 
-    source = ColumnDataSource(data)    
+    source = ColumnDataSource(data)
     view_by_factor = factor_view(source, by)
 
     # Make scatter chart first, for sake of legend.
     markers = grouped_scatter(
         fig,
         iv_axis="y",
         iv_variable=y,
         marker_variable=marker_variable,
         source=source,
         view=view_by_factor,
         **scatter_args
     )
     fig._scatter = [markers]
-    
+
     # Make stacked bars showing components.
-    tooltips = ([] if marker_variable is None 
-                else             
+    tooltips = ([] if marker_variable is None
+                else
                     # Show value of line, regardless.
                     [(marker_variable, f"@{marker_variable}{{0,0.0}}")]
                )
     bars = grouped_stack(
         fig,
         iv_axis="y",
         iv_variable=y,
         bar_variables=bar_variables,
         source=source,
         view=view_by_factor,
         #tooltips=tooltips,
         **bar_args,
     )
     fig._stacked = bars
-    
-    ## Define hover info for whole figure.    
+
+    ## Define hover info for whole figure.
     if isinstance(y, dict):
         iv_hover_variable = y["hover"]
     else:
         iv_hover_variable = y
 
     tooltips = [(by, f"@{{{by}}}"),
                 (iv_hover_variable, f"@{{{iv_hover_variable}}}")]
     if marker_variable is not None:
         tooltips.append(
             (marker_variable, f"@{{{marker_variable}}}{{0[.]0 a}}")
         )
     tooltips.extend((bar, f"@{{{bar}}}{{0[.]0 a}}") for bar in bar_variables)
-    
-    hover = add_hover_tool(fig, 
+
+    hover = add_hover_tool(fig,
                            bars[0:1],  # Show tips just once for the stack, not for every glyph.
                            *tooltips,
                            name="Hover bar stack",
                            description="Hover bar stack",
                            mode="hline",
                            point_policy = 'follow_mouse',
                            attachment="vertical",
                            show_arrow = False,
                           )
-    
+
     if fig.toolbar.active_inspect == "auto":
         # Activate just the new hover tool.
         fig.toolbar.active_inspect = hover
     else:
         # Add the new hover to list of active inspectors.
-        fig.toolbar.active_inspect = fig.toolbar.active_inspect.append(hover)    
+        fig.toolbar.active_inspect = fig.toolbar.active_inspect.append(hover)
 
     return [markers] + bars
 
 #%%
 
 def link_widget_to_snapcomp_figure(widget, fig=None, renderers=None):
     if renderers is None:
@@ -110,14 +110,20 @@
         sample = fig._stacked[0]
     elif isinstance(renderers, list):
         # Use first renderer.
         sample = renderers[0]
     else:
         # Assume we have a single renderer.
         sample = renderers
-    for cds_filter in sample.view.filters:
+
+    # Get .filter attribute (newer bokeh) or .filters (pre bokeh 3.0).
+    view = sample.view
+    filter = getattr(view, "filter", None)
+    filters = [filter] if filter is not None else view.filters
+
+    for cds_filter in filters:
         # Sync filter to widget.
         cds_filter.group = widget.value
     # Sync groupfilters to widget (for multi-lines?).
     link_widgets_to_groupfilters(widget,
-                                 source=sample.data_source, 
-                                 view=sample.view)
+                                 source=sample.data_source,
+                                 filter=filters)
```

### Comparing `xplorts-0.5/src/xplorts/snapcomp/xpsnapcomp.py` & `xplorts-0.6/src/xplorts/snapcomp/xpsnapcomp.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/src/xplorts/stacks/bokeh_stacks.py` & `xplorts-0.6/src/xplorts/stacks/bokeh_stacks.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/src/xplorts/stacks/stacks.py` & `xplorts-0.6/src/xplorts/stacks/stacks.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/src/xplorts/stacks/stacks_util.py` & `xplorts-0.6/src/xplorts/stacks/stacks_util.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/src/xplorts/stacks/xpstacks.py` & `xplorts-0.6/src/xplorts/stacks/xpstacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 Make standalone interactive stacked bar charts for categorical data.
 
 When imported as a module, the function `grouped_stack()` is defined.
 
 When run from the command line, `stacks` reads data from a `csv` file
 and creates an HTML document that displays an interactive stacked bar chart.
 
-    The `stacks` command reads data from a `csv` file.  The first row 
+    The `stacks` command reads data from a `csv` file.  The first row
     of data defines column names.  The file should include:
         - a column of category names for an independent variable,
-        - a column of category names for a split factor, and 
+        - a column of category names for a split factor, and
         - one or more columns of data values to be plotted as stacked bars
-          against the independent variable.  The data values can include a 
+          against the independent variable.  The data values can include a
           mix of positive and negative values.
-    
+
     An interactive chart is created, with widgets to select one of the
-    split factor category names (from a pulldown list or a slider), and a 
+    split factor category names (from a pulldown list or a slider), and a
     chart with stacked bars for the value columns.  The independent variable
     can be plotted along either the vertical or horizontal axis.
 
 
 Command line interface
 ----------------------
 usage: stacks.py [-h] [-b BY] [-x X | -y Y] [-v VALUES [VALUES ...]] [-g ARGS]
@@ -57,66 +57,66 @@
 import pandas as pd
 from pathlib import Path
 import sys
 import yaml
 
 ## Imports from this package
 from xplorts.stacks import grouped_stack
-from xplorts.base import (factor_view, iv_dv_figure, 
+from xplorts.base import (factor_view, iv_dv_figure,
                           link_widgets_to_groupfilters, set_output_file, variables_cmap)
 from xplorts.slideselect import SlideSelect
 
 #%%
 
 def _parse_args():
     """
     Parse command line arguments
-    
+
     Returns
     -------
     `argparse.Namespace` object
-    
+
     Examples
     --------
     args = _parse_args()
     data = pd.read_csv(args.datafile)
-    
+
     Resources
     ---------
     [argparse — Parser for command-line options, arguments and sub-commands](https://docs.python.org/3/library/argparse.html#dest)
     """
     # Check command line arguments.
     parser = argparse.ArgumentParser(
         prog="python -m xplorts.stacks",
         description="Create interactive stacked bars for data series with a split factor"
     )
-    parser.add_argument("datafile", 
+    parser.add_argument("datafile",
                         help="Name of .csv file with data series and split factor")
     parser.add_argument("-b", "--by", type=str,
                         help="Name of factor variable for splits")
 
 
     iv_group = parser.add_mutually_exclusive_group()
     iv_group.add_argument("-x", type=str,
                           help="Name of independent variable, for horizontal axis")
     iv_group.add_argument("-y", type=str,
                           help="Name of independent variable, for vertical axis")
 
-    parser.add_argument("-v", "--values", 
+    parser.add_argument("-v", "--values",
                         nargs="+", type=str,
                         help="Dependent variables to show as stacked bars")
-    parser.add_argument("-g", "--args", 
+    parser.add_argument("-g", "--args",
                         type=str,
                         help="Keyword arguments for grouped_stack(), specified as YAML mapping")
 
-    
-    parser.add_argument("-t", "--save", type=str, 
+
+    parser.add_argument("-t", "--save", type=str,
                         help="Name of interactive .html to save, if different from the datafile base")
 
-    parser.add_argument("-s", "--show", action="store_true", 
+    parser.add_argument("-s", "--show", action="store_true",
                         help="Show interactive .html")
     args = parser.parse_args()
 
     # Unpack YAML args into dict of keyword args for grouped_multi_lines().
     args.args = {} if args.args is None else yaml.safe_load(args.args)
     return(args)
 
@@ -124,15 +124,15 @@
 #%%
 
 def main():
     args = _parse_args()
     print(args)
 
     data = pd.read_csv(args.datafile, dtype=str)
-    
+
     # Unpack args specifying which columns to use.
     if all(getattr(args, arg) is None for arg in ["x", "y", "by", "values"]):
         # Get datevar from first column, byvar from second, values from remaining.
         iv_axis = "x"
         iv_variable, byvar = data.columns[:2]
         datavars = data.columns[2:]
     else:
@@ -141,33 +141,34 @@
         datavars = args.values
         if args.x is not None:
             iv_axis = "x"
             iv_variable = args.x
         else:
             iv_axis = "y"
             iv_variable = args.y
-    
+
     title = "stacks: " + Path(args.datafile).stem
-    
+
     # Configure output file for interactive html.
     set_output_file(
         args.save or args.datafile,
         title = title
     )
-    
+
     # Make a slide-select widget to choose factor level.
     widget = SlideSelect(options=list(data[byvar].unique()),
                          name=byvar + "_select")
 
     source = ColumnDataSource(data)
     view_by_factor = factor_view(source, byvar)
 
-    link_widgets_to_groupfilters(widget, 
-                                 view=view_by_factor)
-    
+    link_widgets_to_groupfilters(widget,
+                                 source=source,
+                                 filter=view_by_factor.filters)
+
     # Map variables to colors.
     default_color_map = variables_cmap(datavars,
                                        "Category10_10")
     default_bar_colors = [default_color_map[var] for var in datavars]
 
     # Labels for axis.
     iv_data = data[iv_variable].unique()
@@ -184,22 +185,22 @@
         iv_axis=iv_axis,
         iv_variable=iv_variable,
         bar_variables=datavars,
         source=source,
         view=view_by_factor,
         color=default_bar_colors,
         **args.args)
-    
+
     # Make app that shows widget and chart.
     app = layout([
         Div(text="<h1>" + title),  # Show title as level 1 heading.
         [widget],
         [fig]
     ])
-    
+
     if args.show:
         show(app)  # Save file and display in web browser.
     else:
         save(app)  # Save file.
 
 #%%
 
@@ -218,17 +219,17 @@
         (2002, 'B', 90, 102),
         (2003, 'B', 95, 98)
     ], columns=["date", "industry", "gva", "hours worked"])
     df_data["oph"] = 100 * df_data["gva"] / df_data["hours worked"]
     df_data["date"] = df_data["date"].astype(str)
 
     factor = "industry"
-    
+
     from base import growth_vars
-    df_growth = growth_vars(df_data, columns=["gva", "hours worked", "oph"], 
+    df_growth = growth_vars(df_data, columns=["gva", "hours worked", "oph"],
                             reverse="hours worked", by=factor,
                             reverse_suffix=" (sign reversed)")
 
 
     factor_levels = sorted(df_data[factor].unique())
     filter_widget = SlideSelect(options=factor_levels,
                                 name=factor + "_filter")  # Show this in a layout.
@@ -236,19 +237,19 @@
     fig = iv_dv_figure(
         iv_data = df_growth["date"],
         iv_axis = "x",
     )
 
     source = ColumnDataSource(df_growth)
     view_by_factor = factor_view(source, factor)
-    
+
     bar_variables = ["gva", "hours worked (sign reversed)"]
     color_map = {v: color for v, color in zip(bar_variables,
                                               palettes.Category20_3)}
-    
+
 
     vbars = grouped_stack(
         fig,
         iv_axis="x",
         iv_variable="date",
         bar_variables=bar_variables,
         color_map=color_map,
```

### Comparing `xplorts-0.5/src/xplorts/tscomp/__init__.py` & `xplorts-0.6/src/xplorts/tscomp/__init__.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/src/xplorts/tscomp/tscomp.py` & `xplorts-0.6/src/xplorts/tscomp/tscomp.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Link a select widget to components series to show one level of split group
 """
 
 #%%
 from bokeh.models import ColumnDataSource
 
 ## Imports from this package
-from ..base import (add_hover_tool, factor_view, 
+from ..base import (add_hover_tool, factor_view,
                           link_widgets_to_groupfilters)
 from ..lines import grouped_multi_lines, link_widget_to_lines
 from ..stacks import grouped_stack
 
 #%%
 def ts_components_figure(
     fig,
@@ -31,97 +31,100 @@
     by=None,
     line_variable=None,
     line_args={},
     bar_args={},
 ):
     """
     Interactive chart showing time series components and total by split group
-    
+
     Parameters
     ----------
     date_variable: str or dict
         If str, the name of a data column, which will be shown on the horizontal
-        axis.  
-        
+        axis.
+
         If dict, should map key "plot" to a variable to show on the
         horizontal axis and should map key "hover" to a corresponding variable
         to display in hover information.  This is often useful when displaying
-        quarterly dates as nested categories like `("2020", "Q1")`.    
+        quarterly dates as nested categories like `("2020", "Q1")`.
 
     """
 
     # Make line chart first, for sake of legend.
     lines = grouped_multi_lines(
         fig,
         data,
         iv_variable=date_variable,
         data_variables=line_variable,
         by=by,
         **line_args
     )
 
-    source = ColumnDataSource(data)    
+    source = ColumnDataSource(data)
     view_by_factor = factor_view(source, by)
-    
+
     # Make stacked bars showing components.
     bars = grouped_stack(
         fig,
         iv_axis="x",
         iv_variable=date_variable,
         bar_variables=bar_variables,
         source=source,
         view=view_by_factor,
         **bar_args,
     )
-    
-    ## Define hover info for whole figure.    
+
+    ## Define hover info for whole figure.
     if isinstance(date_variable, dict):
         iv_hover_variable = date_variable["hover"]
     else:
         iv_hover_variable = date_variable
 
     tooltips = [(by, f"@{{{by}}}"),
                 (iv_hover_variable, f"@{{{iv_hover_variable}}}")]
     if line_variable is not None:
         tooltips.append(
             (line_variable, f"@{{{line_variable}}}{{0[.]0 a}}")
         )
     tooltips.extend((bar, f"@{{{bar}}}{{0[.]0 a}}") for bar in bar_variables)
-    
-    hover = add_hover_tool(fig, 
+
+    hover = add_hover_tool(fig,
                            bars[0:1],  # Show tips just once for the stack, not for every glyph.
                            *tooltips,
                            name="Hover bar stack",
                            description="Hover bar stack",
                            mode="vline",
                            point_policy = 'follow_mouse',
                            attachment="horizontal",
                            show_arrow = False,
                           )
-    
+
     if fig.toolbar.active_inspect == "auto":
         # Activate just the new hover tool.
         fig.toolbar.active_inspect = hover
     else:
         # Add the new hover to list of active inspectors.
-        fig.toolbar.active_inspect = fig.toolbar.active_inspect.append(hover)    
-    
+        fig.toolbar.active_inspect = fig.toolbar.active_inspect.append(hover)
+
     fig._lines = lines
     fig._stacked = bars
-    
+
     return lines + bars
 
 #%%
 def link_widget_to_tscomp_figure(widget, fig=None, lines=None, bars=None):
     """
-    
+
     """
     if lines is None:
         lines = fig._lines
     if bars is None:
         bars = fig._stacked
     source = bars[0].data_source
     view = bars[0].view
+    # Get .filter attribute (newer bokeh) or .filters (pre bokeh 3.0).
+    filter = getattr(view, "filter", None) or view.filters
+
     link_widget_to_lines(widget, lines)
     link_widgets_to_groupfilters(widget,
-                                 source=source, 
-                                 view=view)
+                                 source=source,
+                                 filter=filter)
```

### Comparing `xplorts-0.5/src/xplorts/tscomp/xptscomp.py` & `xplorts-0.6/src/xplorts/tscomp/xptscomp.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/src/xplorts/utils/ukons_lprod_to_csv.py` & `xplorts-0.6/src/xplorts/utils/ukons_lprod_to_csv.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/tests/conftest.py` & `xplorts-0.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/tests/test_dblprod.py` & `xplorts-0.6/tests/test_dblprod.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/tests/test_lines.py` & `xplorts-0.6/tests/test_lines.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/tests/test_scatter.py` & `xplorts-0.6/tests/test_scatter.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/tests/test_snapcomp.py` & `xplorts-0.6/tests/test_snapcomp.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/tests/test_stacks.py` & `xplorts-0.6/tests/test_stacks.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/tests/test_tscomp.py` & `xplorts-0.6/tests/test_tscomp.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.5/PKG-INFO` & `xplorts-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: xplorts
-Version: 0.5
+Version: 0.6
 Summary: Make standalone interactive HTML charts to explore time series datasets
-Project-URL: Bug Tracker, https://github.com/xplorts/xplorts/issues
 Project-URL: Homepage, https://github.com/xplorts/xplorts
+Project-URL: Bug Tracker, https://github.com/xplorts/xplorts/issues
 Author-email: Todd M Bailey <tmb@baileywick.plus.com>
 License: Copyright 2023 Todd Bailey
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
         
@@ -87,14 +87,15 @@
         
         
         ### Output per hour worked
         
         The datasets `oph annual bespoke.csv`, `oph annual by division.csv`, `oph annual by section.csv`, `oph quarterly by section.csv` are extracts from `outputperhourworked.xls`, which was downloaded from [Output per hour worked, UK](https://www.ons.gov.uk/economy/economicoutputandproductivity/productivitymeasures/datasets/outputperhourworkeduk).
         
         Source: Office for National Statistics licensed under the Open Government Licence v.3.0
+License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Requires-Dist: bokeh>=2.3.2
 Requires-Dist: numpy>=1.19.2
```

