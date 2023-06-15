# Comparing `tmp/toolstr-0.9.5.tar.gz` & `tmp/toolstr-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolstr-0.9.5.tar", last modified: Fri May 19 02:50:18 2023, max compression
+gzip compressed data, was "toolstr-0.9.6.tar", last modified: Thu Jun 15 06:36:11 2023, max compression
```

## Comparing `toolstr-0.9.5.tar` & `toolstr-0.9.6.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0       80 2023-01-01 01:26:00.835967 toolstr-0.9.5/.gitignore
--rw-r--r--   0        0        0     1084 2022-12-09 18:24:40.520680 toolstr-0.9.5/LICENSE
--rw-r--r--   0        0        0     8107 2022-12-09 18:24:40.520919 toolstr-0.9.5/README.md
--rw-r--r--   0        0        0      612 2023-05-09 04:42:34.474533 toolstr-0.9.5/pyproject.toml
--rw-r--r--   0        0        0      268 2023-05-19 02:49:50.256020 toolstr-0.9.5/toolstr/__init__.py
--rw-r--r--   0        0        0       28 2023-05-19 00:35:26.933408 toolstr-0.9.5/toolstr/buffers/__init__.py
--rw-r--r--   0        0        0      416 2023-05-19 00:38:07.842409 toolstr-0.9.5/toolstr/buffers/stdout_utils.py
--rw-r--r--   0        0        0      475 2022-12-09 18:24:40.521992 toolstr-0.9.5/toolstr/charts/README.md
--rw-r--r--   0        0        0      134 2022-12-09 18:24:40.522217 toolstr-0.9.5/toolstr/charts/__init__.py
--rw-r--r--   0        0        0    12629 2022-12-09 18:24:40.522525 toolstr-0.9.5/toolstr/charts/braille_utils.py
--rw-r--r--   0        0        0     2412 2022-12-09 18:24:40.522810 toolstr-0.9.5/toolstr/charts/char_dicts.py
--rw-r--r--   0        0        0     3763 2022-12-09 18:24:40.523072 toolstr-0.9.5/toolstr/charts/grid_utils.py
--rw-r--r--   0        0        0     2247 2022-12-09 18:24:40.523333 toolstr-0.9.5/toolstr/charts/line_utils.py
--rw-r--r--   0        0        0     3682 2022-12-12 20:14:13.660011 toolstr-0.9.5/toolstr/charts/plot_utils.py
--rw-r--r--   0        0        0     7038 2022-12-09 18:24:40.524040 toolstr-0.9.5/toolstr/charts/raster_utils.py
--rw-r--r--   0        0        0     8161 2022-12-12 20:13:58.305050 toolstr-0.9.5/toolstr/charts/render_utils.py
--rw-r--r--   0        0        0     2523 2022-12-09 18:24:40.524620 toolstr-0.9.5/toolstr/charts/sextant_utils.py
--rw-r--r--   0        0        0      186 2023-04-24 03:18:32.307974 toolstr-0.9.5/toolstr/formats/__init__.py
--rw-r--r--   0        0        0     1964 2022-12-09 18:24:40.525217 toolstr-0.9.5/toolstr/formats/bullet_formats.py
--rw-r--r--   0        0        0     1997 2022-12-09 18:24:40.525609 toolstr-0.9.5/toolstr/formats/column_formats.py
--rw-r--r--   0        0        0     7280 2023-03-27 19:55:46.509117 toolstr-0.9.5/toolstr/formats/datatype_formats.py
--rw-r--r--   0        0        0     3143 2022-12-12 07:53:13.190851 toolstr-0.9.5/toolstr/formats/positional_formats.py
--rw-r--r--   0        0        0     2191 2022-12-09 18:24:40.526344 toolstr-0.9.5/toolstr/formats/rich_formats.py
--rw-r--r--   0        0        0     3167 2023-04-24 06:16:05.352543 toolstr-0.9.5/toolstr/formats/template_formats.py
--rw-r--r--   0        0        0       61 2022-12-09 18:24:40.526678 toolstr-0.9.5/toolstr/outlines/__init__.py
--rw-r--r--   0        0        0     9083 2022-12-09 18:24:40.526924 toolstr-0.9.5/toolstr/outlines/outline_chars.py
--rw-r--r--   0        0        0     7359 2023-05-08 16:02:35.196513 toolstr-0.9.5/toolstr/outlines/outline_printing.py
--rw-r--r--   0        0        0        0 2022-12-09 18:24:40.527329 toolstr-0.9.5/toolstr/py.typed
--rw-r--r--   0        0        0     2402 2022-12-12 03:10:49.782218 toolstr-0.9.5/toolstr/spec.py
--rw-r--r--   0        0        0       28 2022-12-12 20:09:48.083313 toolstr-0.9.5/toolstr/summaries/__init__.py
--rw-r--r--   0        0        0     6158 2023-04-05 16:58:38.202042 toolstr-0.9.5/toolstr/summaries/set_summary.py
--rw-r--r--   0        0        0       89 2022-12-09 18:24:40.527921 toolstr-0.9.5/toolstr/tables/__init__.py
--rw-r--r--   0        0        0     5083 2022-12-09 18:24:40.528163 toolstr-0.9.5/toolstr/tables/multiline_tables.py
--rw-r--r--   0        0        0     2983 2023-04-24 06:16:44.834292 toolstr-0.9.5/toolstr/tables/table_adapters.py
--rw-r--r--   0        0        0    33565 2023-05-19 02:48:05.006316 toolstr-0.9.5/toolstr/tables/table_utils.py
--rw-r--r--   0        0        0     8722 1970-01-01 00:00:00.000000 toolstr-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0       80 2023-01-01 01:26:00.835967 toolstr-0.9.6/.gitignore
+-rw-r--r--   0        0        0     1084 2022-12-09 18:24:40.520680 toolstr-0.9.6/LICENSE
+-rw-r--r--   0        0        0     8107 2022-12-09 18:24:40.520919 toolstr-0.9.6/README.md
+-rw-r--r--   0        0        0      612 2023-05-09 04:42:34.474533 toolstr-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0      268 2023-06-15 06:35:44.903539 toolstr-0.9.6/toolstr/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-19 00:35:26.933408 toolstr-0.9.6/toolstr/buffers/__init__.py
+-rw-r--r--   0        0        0      592 2023-06-14 01:27:06.061946 toolstr-0.9.6/toolstr/buffers/stdout_utils.py
+-rw-r--r--   0        0        0      475 2022-12-09 18:24:40.521992 toolstr-0.9.6/toolstr/charts/README.md
+-rw-r--r--   0        0        0      134 2022-12-09 18:24:40.522217 toolstr-0.9.6/toolstr/charts/__init__.py
+-rw-r--r--   0        0        0    12629 2022-12-09 18:24:40.522525 toolstr-0.9.6/toolstr/charts/braille_utils.py
+-rw-r--r--   0        0        0     2412 2022-12-09 18:24:40.522810 toolstr-0.9.6/toolstr/charts/char_dicts.py
+-rw-r--r--   0        0        0     3763 2022-12-09 18:24:40.523072 toolstr-0.9.6/toolstr/charts/grid_utils.py
+-rw-r--r--   0        0        0     2247 2022-12-09 18:24:40.523333 toolstr-0.9.6/toolstr/charts/line_utils.py
+-rw-r--r--   0        0        0     3682 2022-12-12 20:14:13.660011 toolstr-0.9.6/toolstr/charts/plot_utils.py
+-rw-r--r--   0        0        0     7038 2022-12-09 18:24:40.524040 toolstr-0.9.6/toolstr/charts/raster_utils.py
+-rw-r--r--   0        0        0     8161 2022-12-12 20:13:58.305050 toolstr-0.9.6/toolstr/charts/render_utils.py
+-rw-r--r--   0        0        0     2523 2022-12-09 18:24:40.524620 toolstr-0.9.6/toolstr/charts/sextant_utils.py
+-rw-r--r--   0        0        0      186 2023-04-24 03:18:32.307974 toolstr-0.9.6/toolstr/formats/__init__.py
+-rw-r--r--   0        0        0     1964 2022-12-09 18:24:40.525217 toolstr-0.9.6/toolstr/formats/bullet_formats.py
+-rw-r--r--   0        0        0     1997 2022-12-09 18:24:40.525609 toolstr-0.9.6/toolstr/formats/column_formats.py
+-rw-r--r--   0        0        0     7280 2023-03-27 19:55:46.509117 toolstr-0.9.6/toolstr/formats/datatype_formats.py
+-rw-r--r--   0        0        0     3143 2022-12-12 07:53:13.190851 toolstr-0.9.6/toolstr/formats/positional_formats.py
+-rw-r--r--   0        0        0     2191 2023-06-03 05:09:21.785742 toolstr-0.9.6/toolstr/formats/rich_formats.py
+-rw-r--r--   0        0        0     3167 2023-04-24 06:16:05.352543 toolstr-0.9.6/toolstr/formats/template_formats.py
+-rw-r--r--   0        0        0       61 2022-12-09 18:24:40.526678 toolstr-0.9.6/toolstr/outlines/__init__.py
+-rw-r--r--   0        0        0     9083 2022-12-09 18:24:40.526924 toolstr-0.9.6/toolstr/outlines/outline_chars.py
+-rw-r--r--   0        0        0     7359 2023-05-08 16:02:35.196513 toolstr-0.9.6/toolstr/outlines/outline_printing.py
+-rw-r--r--   0        0        0        0 2022-12-09 18:24:40.527329 toolstr-0.9.6/toolstr/py.typed
+-rw-r--r--   0        0        0     2402 2022-12-12 03:10:49.782218 toolstr-0.9.6/toolstr/spec.py
+-rw-r--r--   0        0        0       58 2023-06-13 22:26:15.086201 toolstr-0.9.6/toolstr/summaries/__init__.py
+-rw-r--r--   0        0        0     6145 2023-06-15 06:35:03.583900 toolstr-0.9.6/toolstr/summaries/nested_summary.py
+-rw-r--r--   0        0        0     6158 2023-04-05 16:58:38.202042 toolstr-0.9.6/toolstr/summaries/set_summary.py
+-rw-r--r--   0        0        0       89 2022-12-09 18:24:40.527921 toolstr-0.9.6/toolstr/tables/__init__.py
+-rw-r--r--   0        0        0     5083 2022-12-09 18:24:40.528163 toolstr-0.9.6/toolstr/tables/multiline_tables.py
+-rw-r--r--   0        0        0     2983 2023-04-24 06:16:44.834292 toolstr-0.9.6/toolstr/tables/table_adapters.py
+-rw-r--r--   0        0        0    33536 2023-06-14 01:33:04.639306 toolstr-0.9.6/toolstr/tables/table_utils.py
+-rw-r--r--   0        0        0     8722 1970-01-01 00:00:00.000000 toolstr-0.9.6/PKG-INFO
```

### Comparing `toolstr-0.9.5/LICENSE` & `toolstr-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/README.md` & `toolstr-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/pyproject.toml` & `toolstr-0.9.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/toolstr/charts/braille_utils.py` & `toolstr-0.9.6/toolstr/charts/braille_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/toolstr/charts/char_dicts.py` & `toolstr-0.9.6/toolstr/charts/char_dicts.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/toolstr/charts/grid_utils.py` & `toolstr-0.9.6/toolstr/charts/grid_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/toolstr/charts/line_utils.py` & `toolstr-0.9.6/toolstr/charts/line_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/toolstr/charts/plot_utils.py` & `toolstr-0.9.6/toolstr/charts/plot_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/toolstr/charts/raster_utils.py` & `toolstr-0.9.6/toolstr/charts/raster_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/toolstr/charts/render_utils.py` & `toolstr-0.9.6/toolstr/charts/render_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/toolstr/charts/sextant_utils.py` & `toolstr-0.9.6/toolstr/charts/sextant_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/toolstr/formats/bullet_formats.py` & `toolstr-0.9.6/toolstr/formats/bullet_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/toolstr/formats/column_formats.py` & `toolstr-0.9.6/toolstr/formats/column_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/toolstr/formats/datatype_formats.py` & `toolstr-0.9.6/toolstr/formats/datatype_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/toolstr/formats/positional_formats.py` & `toolstr-0.9.6/toolstr/formats/positional_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/toolstr/formats/rich_formats.py` & `toolstr-0.9.6/toolstr/formats/rich_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/toolstr/formats/template_formats.py` & `toolstr-0.9.6/toolstr/formats/template_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/toolstr/outlines/outline_chars.py` & `toolstr-0.9.6/toolstr/outlines/outline_chars.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/toolstr/outlines/outline_printing.py` & `toolstr-0.9.6/toolstr/outlines/outline_printing.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/toolstr/spec.py` & `toolstr-0.9.6/toolstr/spec.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/toolstr/summaries/set_summary.py` & `toolstr-0.9.6/toolstr/summaries/set_summary.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/toolstr/tables/multiline_tables.py` & `toolstr-0.9.6/toolstr/tables/multiline_tables.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/toolstr/tables/table_adapters.py` & `toolstr-0.9.6/toolstr/tables/table_adapters.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.5/toolstr/tables/table_utils.py` & `toolstr-0.9.6/toolstr/tables/table_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 
 def transpose_table(
     rows: typing.Sequence[typing.Sequence[typing.Any]],
     *,
     labels: typing.Sequence[str] | None = None,
     create_labels: bool = False,
 ) -> TableData:
-
     if labels is not None:
         rows = [labels] + list(rows)
     new_rows = list(zip(*rows))
 
     if create_labels:
         new_labels = new_rows[0]
         new_rows = new_rows[1:]
@@ -115,15 +114,14 @@
     label_justify: ColumnData[spec.HorizontalJustification] | None = None,
     label_vertical_justify: ColumnData[spec.VerticalJustification]
     | None = 'bottom',
     style: Style | None = None,
     column_styles: ColumnData[Style] | None = None,
     label_style: ColumnData[Style] | None = None,
 ) -> str | None:
-
     # filter row separators
     rows, separator_indices = _filter_separator_indices(rows, separate_all_rows)
 
     # check missing columns
     rows, labels = _fix_missing_data(rows, labels, missing_columns, empty_str)
 
     # sort rows
@@ -176,45 +174,41 @@
         return table_as_str
     else:
         _print_table(table_as_str, use_styles, console, file)
         return None
 
 
 def _should_use_styles(use_styles: bool | None) -> bool:
-
     # check that value of use_styles has proper value
     if not isinstance(use_styles, bool) and use_styles is not None:
         raise Exception('use_styles should be bool or None')
 
     if use_styles is None:
-
         # use styles if rich is importable
         try:
             import rich
 
             use_styles = True
         except ImportError:
             use_styles = False
 
     elif use_styles:
-
         # test whether rich can be imported
         try:
             import rich
         except ImportError:
             raise Exception('rich required for styles, e.g. `pip install rich`')
 
     return use_styles
 
 
 def _filter_separator_indices(
     rows: typing.Sequence[None | typing.Sequence[typing.Any]],
     separate_all_rows: bool,
 ) -> tuple[list[typing.Sequence[typing.Any]], set[int]]:
-
     filtered: list[typing.Sequence[typing.Any]] = []
     indices = set()
     for row in rows:
         if row is None:
             index = len(filtered) - 1
             if index < 0:
                 raise Exception('cannot start with a row separator')
@@ -230,15 +224,14 @@
 
 def _fix_missing_data(
     rows: list[typing.Sequence[typing.Any]],
     labels: typing.Sequence[str] | None,
     missing_columns: typing.Literal['clip', 'fill', 'error'],
     empty_str: str,
 ) -> tuple[list[typing.Sequence[typing.Any]], typing.Sequence[str] | None]:
-
     if len(rows) > 0:
         min_columns = 1_000_000_000
         max_columns = 0
         for row in rows:
             n_row_columns = len(row)
             min_columns = min(min_columns, n_row_columns)
             max_columns = max(max_columns, n_row_columns)
@@ -301,15 +294,14 @@
     | None,
     label_vertical_justify: ColumnData[spec.VerticalJustification] | None,
     use_styles: bool | None,
     style: Style | None,
     column_styles: ColumnData[Style] | None,
     label_style: ColumnData[Style] | None,
 ) -> tuple[list[list[str]], list[list[str]], typing.Sequence[int], bool]:
-
     # determine number of columns
     if len(rows) > 0:
         n_columns = len(rows[0])
     elif labels is not None:
         n_columns = len(labels)
     else:
         return [], [], [], False
@@ -366,15 +358,14 @@
         for str_label in str_labels
     ]
 
     # add styles to rows and label
     if use_styles is None:
         use_styles = _should_use_styles(use_styles)
     if use_styles:
-
         # arrange column style specifications
         column_styles = _convert_column_dict_to_list(
             column_styles, n_columns, labels
         )
 
         # style rows
         str_cells = _stylize_rows(
@@ -411,23 +402,21 @@
     return str_cells, str_labels, column_widths, use_styles
 
 
 def _get_column_widths(
     str_cells: list[list[str]],
     max_column_widths: typing.Sequence[int | None] | None,
 ) -> list[int]:
-
     if len(str_cells) > 0:
         n_columns = len(str_cells[0])
     else:
         return []
     column_widths: list[int] = [0] * n_columns
     for row_str_cells in str_cells:
         for c, str_cell in enumerate(row_str_cells):
-
             if '[' in str_cell:
                 import rich.text
 
                 cell_width = rich.text.Text.from_markup(str_cell).cell_len
             else:
                 cell_width = len(str_cell)
             if cell_width > column_widths[c]:
@@ -480,15 +469,14 @@
             raise Exception('mismatching number of columns')
         return column_data
 
     elif isinstance(column_data, str):
         return [column_data] * n_columns  # type: ignore
 
     elif isinstance(column_data, dict):
-
         if all(isinstance(item, int) for item in column_data.keys()):
             return [column_data.get(c) for c in range(n_columns)]
         elif all(isinstance(item, str) for item in column_data.keys()):
             if labels is None:
                 raise Exception('must provide labels for named column data')
             return [column_data.get(label) for label in labels]
         else:
@@ -505,15 +493,14 @@
     | int
     | typing.Sequence[str]
     | typing.Sequence[int]
     | None = None,
     sort_key: typing.Callable[..., typing.Any] | None = None,
     descending: bool = False,
 ) -> list[typing.Sequence[typing.Any]]:
-
     if sort_column is not None and sort_key is not None:
         raise Exception('should not specify both sort_key and sort_column')
     for raw_row in rows:
         if raw_row is None:
             raise Exception('cannot sort gap rows equal to None')
 
     # sort by values of particular columns
@@ -560,30 +547,27 @@
     format: FormatKwargs | None,
     column_formats: typing.Sequence[None | typing.Mapping[str, typing.Any]]
     | None,
     empty_str: str,
 ) -> list[str]:
     row_str_cells = []
     for c, cell in enumerate(row):
-
         if cell is None:
             cell = empty_str
 
         # convert to str
         if isinstance(cell, str):
             as_str = cell
         else:
-
             # include numpy types
             if (
                 isinstance(cell, (int, float))
                 or type(cell).__name__.startswith('int')
                 or type(cell).__name__.startswith('float')
             ):
-
                 # get format kwargs
                 cell_format: typing.Mapping[str, typing.Any] | None
                 cell_format = None
                 if column_formats is not None:
                     cell_format = column_formats[c]
                 if format is not None and cell_format is None:
                     cell_format = format
@@ -624,25 +608,23 @@
         rich_cell = rich.text.Text.from_markup(cell)
         length = len(rich_cell.plain)
 
         width = column_widths[c]
         if length == width:
             output.append(cell)
         elif length > width:
-
             # trim
 
             if width >= 3:
                 trimmed = rich_cell.fit(width - 3)[0].markup + '...'
             else:
                 trimmed = '.' * width
             output.append(trimmed)
 
         else:
-
             # determine justification
             cell_justify = None
             if column_justify is not None:
                 cell_justify = column_justify[c]
             if cell_justify is None:
                 cell_justify = justify
 
@@ -656,21 +638,18 @@
     rows: typing.Sequence[typing.Sequence[typing.Any]],
     str_rows: list[list[str]],
     labels: typing.Sequence[typing.Any] | None,
     str_labels: list[list[str]],
     style: Style | None,
     column_styles: ColumnData[Style] | None,
 ) -> list[list[str]]:
-
     stylized_rows = []
     for r, (row, str_row) in enumerate(zip(rows, str_rows)):
-
         stylized_row = []
         for c, (cell, str_cell) in enumerate(zip(row, str_row)):
-
             # use column style if specified, otherwise use global style
             if column_styles is not None and column_styles[c] is not None:
                 cell_style: Style | None = column_styles[c]
             elif style is not None:
                 cell_style = style
             else:
                 cell_style = None
@@ -700,15 +679,14 @@
 
     return stylized_rows
 
 
 def _process_label_location(
     label_location: HeaderLocation | None,
 ) -> tuple[bool, bool]:
-
     if isinstance(label_location, str):
         top_label = label_location == 'top'
         bottom_label = label_location == 'bottom'
     elif isinstance(label_location, (tuple, list)):
         top_label = 'top' in label_location
         bottom_label = 'bottom' in label_location
     elif label_location is None:
@@ -731,15 +709,14 @@
     border: str | spec.BorderChars | None,
     label_border: str | spec.BorderChars | None,
     outer_border: bool | str | spec.BorderChars | None,
     column_gap: int | str | None,
     outer_gap: int | str | None,
     separator_indices: set[int],
 ) -> str:
-
     import rich.text
 
     # use compact format
     if compact:
         if outer_gap is None:
             outer_gap = ''
         if column_gap is None:
@@ -805,15 +782,14 @@
         border=border,
         column_gap=column_gap,
         outer_gap=outer_gap,
     )
 
     # render label as strs
     if len(str_labels) > 0:
-
         # build label delimiter
         if not label_equals_outer and not label_equals_inner:
             label_vertical = ' '
         else:
             label_vertical = label_border['vertical']
         label_delimiter = column_gap + label_vertical + column_gap
 
@@ -859,15 +835,14 @@
     top_label = False
     bottom_label = False
     if len(str_labels) > 0:
         top_label, bottom_label = _process_label_location(label_location)
 
     # add outer borders
     if outer_border is not None:
-
         # get outer parameters
         if outer_equals_inner:
             outer_left_t = outer_border['left_t']
             outer_right_t = outer_border['right_t']
         else:
             outer_left_t = outer_border['vertical']
             outer_right_t = outer_border['vertical']
@@ -1005,15 +980,14 @@
 def _build_row_separator(
     column_widths: typing.Sequence[int],
     border: spec.BorderChars,
     column_gap: str,
     outer_gap: str,
     cross_symbol: spec.BorderCharName = 'cross',
 ) -> str:
-
     horizontal = border['horizontal']
     cross = border[cross_symbol]
 
     cgap = len(column_gap)
     ogap = len(outer_gap)
 
     delimiter = cgap * horizontal + cross + cgap * horizontal
@@ -1023,17 +997,15 @@
 
 def _print_table(
     table_as_str: str,
     use_styles: bool,
     console: rich.console.Console | None,
     file: typing.TextIO | None,
 ) -> None:
-
     if use_styles:
-
         if console is None:
             import rich.console
 
             console = rich.console.Console(
                 file=file,
                 theme=rich.theme.Theme(inherit=False),
                 width=10000,
@@ -1047,15 +1019,14 @@
 def clip_rows(
     rows: list[typing.Sequence[typing.Any]],
     n: int,
     *,
     clip_position: Literal['start', 'middle', 'end'] = 'end',
     fill: str | None = '...',
 ) -> list[typing.Sequence[typing.Any]]:
-
     if len(rows) <= n:
         return rows
 
     # construct fill
     if fill is not None:
         n_columns = len(rows[0])
         fill_rows: list[typing.Sequence[typing.Any]] = [[fill] * n_columns]
```

### Comparing `toolstr-0.9.5/PKG-INFO` & `toolstr-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolstr
-Version: 0.9.5
+Version: 0.9.6
 Summary: toolstr is a suite of str processing tools, including formatting and drawing
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: tooltime>=0.2.10
 Requires-Dist: typing-extensions>=4.0.0
 Requires-Dist: scikit-image>=0.19.2 ; extra == "full"
 Requires-Dist: rich>=12.1.0 ; extra == "full"
```

