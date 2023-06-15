# Comparing `tmp/py_fumen_util-0.2.0.tar.gz` & `tmp/py_fumen_util-0.3.0.tar.gz`

## Comparing `py_fumen_util-0.2.0.tar` & `py_fumen_util-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/__init__.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/__main__.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/fumen_combiner.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/fumen_locker.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/fumen_splitter.py
--rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/glue_fumen.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/grayout_all.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/grayout_last.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/mirror_fumen.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/remove_comment.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/src/py_fumen_util/unglue_fumen.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/LICENSE
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/README.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 py_fumen_util-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 py_fumen_util-0.3.0/src/py_fumen_util/__init__.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 py_fumen_util-0.3.0/src/py_fumen_util/__main__.py
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 py_fumen_util-0.3.0/src/py_fumen_util/assemble.py
+-rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 py_fumen_util-0.3.0/src/py_fumen_util/disassemble.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 py_fumen_util-0.3.0/src/py_fumen_util/grayout.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 py_fumen_util-0.3.0/src/py_fumen_util/grayout_all.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 py_fumen_util-0.3.0/src/py_fumen_util/join.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 py_fumen_util-0.3.0/src/py_fumen_util/lock.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 py_fumen_util-0.3.0/src/py_fumen_util/mirror.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 py_fumen_util-0.3.0/src/py_fumen_util/prune.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 py_fumen_util-0.3.0/src/py_fumen_util/prune_all.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 py_fumen_util-0.3.0/src/py_fumen_util/split.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 py_fumen_util-0.3.0/src/py_fumen_util/uncomment.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 py_fumen_util-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 py_fumen_util-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 py_fumen_util-0.3.0/README.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 py_fumen_util-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 py_fumen_util-0.3.0/PKG-INFO
```

### Comparing `py_fumen_util-0.2.0/src/py_fumen_util/__main__.py` & `py_fumen_util-0.3.0/src/py_fumen_util/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,99 +1,89 @@
 # -*- coding:utf-8 -*-
 
 import argparse
 import sys
 
 from py_fumen_py import *
-from .fumen_combiner import fumen_combiner
-from .fumen_locker import fumen_locker
-from .fumen_splitter import fumen_splitter
-from .glue_fumen import glue_fumen
-from .grayout_all import grayout_all_fumen
-from .grayout_last import grayout_fumen
-from .mirror_fumen import mirror_fumen
-from .remove_comment import remove_comment
-from .unglue_fumen import unglue_fumen
-
-_command_function_map = {
-    'combine': fumen_combiner,
-    'concat' : fumen_combiner,
-    'join': fumen_combiner,
-    'split': fumen_splitter,
-    'glue': glue_fumen,
-    'decompile': glue_fumen,
-    'unglue': unglue_fumen,
-    'compile': unglue_fumen,
-    'gray': grayout_fumen,
-    'grey': grayout_fumen,
-    'grayall': grayout_all_fumen,
-    'greyall': grayout_all_fumen,
-    'lock': fumen_locker,
-    'mirror': mirror_fumen,
-    'flip': mirror_fumen,
-    'uncomment': remove_comment,
+import py_fumen_util
+
+_alias_map = {
+    'combine': 'join',
+    'concat': 'join',
+    'compile': 'assemble',
+    'unglue': 'assemble',
+    'decompile': 'disassemble',
+    'glue': 'disassemble',
+    'greyout': 'grayout',
+    'gray': 'grayout',
+    'grey': 'grayout',
+    'grayoutall': 'grayout_all',
+    'greyoutall': 'grayout_all',
+    'grayall': 'grayout_all',
+    'greyall': 'grayout_all',
+    'pruneall': 'prune_all',
+    'flip': 'mirror',
 }
 
-def usage():
-    return [
+_usage = [
         'commands (case-insensitive):',
-        '    Combine:   Combine multiple Fumens into one',
-        '               Alias: Concat, Join',
-        '    Split:     Split each page into a Fumen',
+        '  join:        Join multiple Fumens into one',
+        '               alias: combine, concat',
+        '  split:       Split each page into a Fumen',
+        '',
+        '  assemble:    Assemble Fumen placements into one page',
+        '               alias: compile, unglue',
+        '  disassemble: Disassemble each Fumen page into tetromino placements',
+        '               alias: decompile, glue',
         '',
-        '    Glue:      Glue each Fumen page into tetromino placements',
-        '               Alias: Decompile',
-        '    Unglue:    Unglue Fumen placements into one page',
-        '               Alias: Compile',
+        '  grayout:     Gray out the last page of each fumen',
+        '               alias: greyout, gray, grey',
+        '  grayoutall:  Gray out all pages of each fumen',
+        '               alias: greyoutall, grayall, greyall',
         '',
-        '    Gray:      Gray out the last page of each fumen',
-        '               Alias: Grey'
-        '    Grayall:   Gray out all pages of each fumen',
-        '               Alias: Greyall',
+        '  prune:       Prune colored minos from the last page of each fumen',
+        '  pruneall:    Prune colored minos from all pages of each fumen',
         '',
-        '    Lock:      Lock the last page of each Fumen and append a new page',
-        '    Mirror:    Mirror Fumen pages',
-        '               Alias: Flip',
-        '    Uncomment: Uncomment Fumen pages',
+        '  lock:        Lock the last page of each Fumen and append a new page',
+        '  mirror:      Mirror Fumen pages',
+        '               alias: flip',
+        '  uncomment:   Uncomment Fumen pages',
     ]
 
 if __name__ == '__main__':
     argparser = argparse.ArgumentParser(
+        formatter_class=argparse.RawDescriptionHelpFormatter,
         description='Tetris Fumen utilies in Python.',
-        prog='python3 -m py_fumen_util'
+        prog='python3 -m py_fumen_util',
+        epilog='\n'.join(_usage)
     )
     argparser.add_argument(
         'command',
         type=str,
         nargs='+',
-        help='Command(s) to execute on the Fumen(s).'
+        help='Command(s) to execute on the Fumen(s).',
     )
     argparser.add_argument(
         'file',
         type=str,
-        help='File with Fumen strings, separated with whitespace and/or linebreak. Use "-" to read from standard input.'
+        help='File with Fumen strings, separated with whitespace and/or linebreak. Use "-" to read from standard input.',
     )
 
-    args = argparser.parse_args(sys.argv[1:])
+    args = argparser.parse_args()
     commands = args.command
     fumen_file = sys.stdin if args.file == '-' else open(args.file, 'r')
     fumen_codes = fumen_file.read().split()
     fumen_file.close()
 
     for command in commands:
-        command_function = _command_function_map.get(command.casefold(), None)
         try:
+            command_function = getattr(
+                py_fumen_util,
+                _alias_map.get(command.casefold(), command)
+            )
             fumen_codes = command_function(fumen_codes)
         except Exception as e:
-            if command_function:
-                print(e)
-            else:
-                print(f'"{command}" is not a valid command.')
-            print()
+            print(f'"{command}" is not a valid command.\n')
             argparser.print_help()
-            print()
-            for line in usage():
-                print(line)
-            exit()
 
     for line in fumen_codes:
         print(line)
```

### Comparing `py_fumen_util-0.2.0/src/py_fumen_util/fumen_splitter.py` & `py_fumen_util-0.3.0/src/py_fumen_util/prune_all.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 # -*- coding: utf-8 -*-
 
 import sys
 
 from py_fumen_py import *
 
-def fumen_splitter(fumen_codes):
-    split_fumen = []
+def prune_all(fumen_codes, print_error=True, keep_invalid=True):
+    results = []
     for code in fumen_codes:
-        input_pages = decode(code)
-        for page in input_pages:
-            if input_pages[0].flags.colorize:
-                page.flags.colorize = True
-            split_fumen.append(encode([page]))
-    return split_fumen
+        try:
+            input_pages = decode(code)
+            for page in input_pages:
+                if page.field:
+                    for line in page.field[:]:
+                        for i, mino in enumerate(line):
+                            if mino.is_colored():
+                                line[i] = Mino._
+            results.append(encode(input_pages))
+        except Exception as e:
+            if keep_invalid:
+                results.append('')
+            if print_error:
+                print(e)
+
+    return results
 
 if __name__ == '__main__':
     if len(sys.argv) > 1:
-        for line in fumen_splitter(' '.join(sys.argv[1:]).split()):
+        for line in prune_all(' '.join(sys.argv[1:]).split()):
             print(line)
```

### Comparing `py_fumen_util-0.2.0/src/py_fumen_util/glue_fumen.py` & `py_fumen_util-0.3.0/src/py_fumen_util/disassemble.py`

 * *Files 8% similar despite different names*

```diff
@@ -123,48 +123,55 @@
     field = field.copy()
     for line in field:
         for i, mino in enumerate(line):
             if mino.is_colored():
                 line[i] = Mino._
     return field
 
-def glue_fumen(fumen_codes):
+def disassemble(fumen_codes, print_error=True, keep_invalid=True):
     all_pieces_arr = []
-    all_fumens = []
+    results = []
     fumen_issues = 0
 
     for code in fumen_codes:
-        input_pages = decode(code)
-        this_glue_fumens = []
-        for page in input_pages:
-            field, n_lineclear = remove_line_clears(page.field.copy())
-            empty_field = make_empty_field(field)
-            all_pieces_arr.clear()
-
-            scan_field(0, field.height()-1, field, [], all_pieces_arr)
-
-            if not all_pieces_arr:
-                print(code, "couldn't be glued")
-                fumen_issues += 1
-
-            for pieces_arr in all_pieces_arr:
-                pages = [Page(field=empty_field, operation=pieces_arr[0])]
-                for operation in pieces_arr[1:]:
-                    pages.append(Page(operation=operation))
-                this_glue_fumens.append(encode(pages))
-
-            if len(all_pieces_arr) > 1:
-                all_fumens.append(
-                    'Warning: {} led to {} outputs: {}'.format(
-                        code, len(all_pieces_arr), ' '.join(this_glue_fumens)
+        try:
+            input_pages = decode(code)
+            this_disassembles = []
+            for page in input_pages:
+                field, n_lineclear = remove_line_clears(page.field.copy())
+                empty_field = make_empty_field(field)
+                all_pieces_arr.clear()
+
+                scan_field(0, field.height()-1, field, [], all_pieces_arr)
+
+                if print_error and not all_pieces_arr:
+                    print(code, "couldn't be disassembled")
+                    fumen_issues += 1
+
+                for pieces_arr in all_pieces_arr:
+                    pages = [Page(field=empty_field, operation=pieces_arr[0])]
+                    for operation in pieces_arr[1:]:
+                        pages.append(Page(operation=operation))
+                    this_disassembles.append(encode(pages))
+
+                if print_error and len(all_pieces_arr) > 1:
+                    results.append(
+                        'Warning: {} led to {} outputs: {}'.format(
+                            code, len(all_pieces_arr), ' '.join(this_disassembles)
+                        )
                     )
-                )
-        all_fumens += this_glue_fumens
+            results += this_disassembles
+        except:
+            if keep_invalid:
+                results.append(Page())
+            if print_error:
+                print(e)
 
-    if fumen_issues > 0:
-        print("Warning: {} fumen couldn't be glued".format(fumen_issues))
-    return all_fumens
+    if print_error and fumen_issues > 0:
+        print("Warning: {} fumen couldn't be disassembled".format(fumen_issues))
+
+    return results
 
 if __name__ == '__main__':
     if len(sys.argv) > 1:
-        for line in glue_fumen(' '.join(sys.argv[1:]).split()):
+        for line in disassemble(' '.join(sys.argv[1:]).split()):
             print(line)
```

### Comparing `py_fumen_util-0.2.0/src/py_fumen_util/grayout_all.py` & `py_fumen_util-0.3.0/src/py_fumen_util/split.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # -*- coding: utf-8 -*-
 
 import sys
 
 from py_fumen_py import *
 
-def grayout_all_fumen(fumen_codes):
-    grayed_fumen = []
+def split(fumen_codes, print_error=True, keep_invalid=True):
+    results = []
     for code in fumen_codes:
-        input_pages = decode(code)
-        for page in input_pages:
-            if page.field:
-                for line in page.field[:]:
-                    for i, mino in enumerate(line):
-                        if mino.is_colored():
-                            line[i] = Mino.X
-        grayed_fumen.append(encode(input_pages))
-    return grayed_fumen
+        try:
+            input_pages = decode(code)
+            for page in input_pages:
+                if input_pages[0].flags.colorize:
+                    page.flags.colorize = True
+                results.append(encode([page]))
+        except Exception as e:
+            if keep_invalid:
+                results.append('')
+            if print_error:
+                print(e)
+
+    return results
 
 if __name__ == '__main__':
     if len(sys.argv) > 1:
-        for line in grayout_all_fumen(' '.join(sys.argv[1:]).split()):
+        for line in split(' '.join(sys.argv[1:]).split()):
             print(line)
```

### Comparing `py_fumen_util-0.2.0/src/py_fumen_util/grayout_last.py` & `py_fumen_util-0.3.0/src/py_fumen_util/grayout.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 # -*- coding: utf-8 -*-
 
 import sys
 
 from py_fumen_py import *
 
-def grayout_fumen(fumen_codes):
-    grayed_fumen = []
+def grayout(fumen_codes, print_error=True, keep_invalid=True):
+    results = []
     for code in fumen_codes:
-        input_pages = decode(code)
-        if input_pages[-1].field:
-            for line in input_pages[-1].field[:]:
-                for i, mino in enumerate(line):
-                    if mino.is_colored():
-                        line[i] = Mino.X
-        grayed_fumen.append(encode(input_pages))
-    return grayed_fumen
+        try:
+            input_pages = decode(code)
+            if input_pages[-1].field:
+                for line in input_pages[-1].field[:]:
+                    for i, mino in enumerate(line):
+                        if mino.is_colored():
+                            line[i] = Mino.X
+            results.append(encode(input_pages))
+        except Exception as e:
+            if keep_invalid:
+                results.append('')
+            if print_error:
+                print(e)
+
+    return results
 
 if __name__ == '__main__':
     if len(sys.argv) > 1:
-        for line in grayout_fumen(' '.join(sys.argv[1:]).split()):
+        for line in grayout(' '.join(sys.argv[1:]).split()):
             print(line)
```

### Comparing `py_fumen_util-0.2.0/src/py_fumen_util/unglue_fumen.py` & `py_fumen_util-0.3.0/src/py_fumen_util/assemble.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,44 +6,51 @@
 
 def cleared_offset(rows_cleared, y):
     for row in rows_cleared:
         if y >= row:
             y += 1
     return y
 
-def unglue_fumen(fumen_codes):
-    unglued_fumen = []
+def assemble(fumen_codes, print_error=True, keep_invalid=True):
+    results = []
 
     for code in fumen_codes:
-        rows_cleared = set()
-        input_pages = decode(code)
-        field = input_pages[0].field.copy()
-
-        for page in input_pages:
-            operation = page.operation
-            if operation is None:
-                print('warning: skipped a page with no operation')
-                continue
-
-            for dx, dy in Operation.shape_at(operation.mino,
-                                             operation.rotation):
-                x = operation.x + dx
-                y = cleared_offset(rows_cleared, operation.y+dy)
-                if field.at(x, y) != Mino._:
-                    print('error: operation overlaps with current field')
-                field.fill(x, y, operation.mino)
-
-            new_rows_cleared = set()
-            for dy in range(-2, 3):
-                y = cleared_offset(rows_cleared, operation.y+dy)
-                if y >= 0 and field.is_lineclear_at(y):
-                    new_rows_cleared.add(y)
-            rows_cleared |= new_rows_cleared
+        try:
+            rows_cleared = set()
+            input_pages = decode(code)
+            field = input_pages[0].field.copy()
+
+            for page in input_pages:
+                operation = page.operation
+                if operation is None:
+                    if print_error:
+                        print('warning: skipped a page with no operation')
+                    continue
+
+                for dx, dy in Operation.shape_at(operation.mino,
+                                                 operation.rotation):
+                    x = operation.x + dx
+                    y = cleared_offset(rows_cleared, operation.y+dy)
+                    if print_error and field.at(x, y) != Mino._:
+                        print('error: operation overlaps with current field')
+                    field.fill(x, y, operation.mino)
+
+                new_rows_cleared = set()
+                for dy in range(-2, 3):
+                    y = cleared_offset(rows_cleared, operation.y+dy)
+                    if y >= 0 and field.is_lineclear_at(y):
+                        new_rows_cleared.add(y)
+                rows_cleared |= new_rows_cleared
+
+            results.append(encode([Page(field=field)]))
+        except Exception as e:
+            if keep_invalid:
+                results.append('')
+            if print_error:
+                print(e)
 
-        unglued_fumen.append(encode([Page(field=field)]))
-
-    return unglued_fumen
+    return results
 
 if __name__ == '__main__':
     if len(sys.argv) > 1:
-        for line in unglue_fumen(' '.join(sys.argv[1:]).split()):
+        for line in assemble(' '.join(sys.argv[1:]).split()):
             print(line)
```

### Comparing `py_fumen_util-0.2.0/.gitignore` & `py_fumen_util-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `py_fumen_util-0.2.0/LICENSE` & `py_fumen_util-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_fumen_util-0.2.0/README.md` & `py_fumen_util-0.3.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -17,20 +17,22 @@
 ```
 
 - `command`: Command(s) to execute on the Fumen(s).
 - `file`: File with Fumen strings, separated with whitespace and/or linebreak. Use "-" to read from standard input.
 
 ### Commands
 
-Commands are case-insensitive.
+ommands are case-insensitive.
 
 |Command|Description|Alias|
 |:-|:-|:-|
-|Combine|Combine multiple Fumens into one|Concat, Join|
-|Split|Split each page into a Fumen||
-|Glue|Glue each Fumen page into tetromino placements|Decompile|
-|Unglue|Unglue Fumen placements into one page|Compile|
-|Gray|Gray out the last of each Fumen|Grey|
-|Grayall|Gray out all pages of each Fumen|Greyall|
-|Lock|Lock the last page of each Fumen and append a new page||
-|Mirror|Mirror Fumen pages|Flip|
-|Uncomment|Uncomment Fumen pages||
+|join|Join multiple Fumens into one|combine concat|
+|split|Split each page into a Fumen||
+|assemble|Assemble Fumen placements into one page|compile, unglue|
+|disassemble|Disassemble each Fumen page into tetrimino placements|decompile, glue|
+|gray|Gray out the last page of each Fumen|grey|
+|grayall|Gray out all pages of each Fumen|greyall|
+|prune|Prune colored minos from the last page of each Fumen||
+|pruneall|Prune colored minos from all pages of each Fumen||
+|lock|Lock the last page of each Fumen and append a new page||
+|mirror|Mirror Fumen pages|flip|
+|uncomment|Uncomment Fumen pages||
```

### Comparing `py_fumen_util-0.2.0/pyproject.toml` & `py_fumen_util-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "py_fumen_util"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
 	{ name="Octupus Tea" },
 ]
 description = "Python implementation of the JavaScript package 'FumenUtil'"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `py_fumen_util-0.2.0/PKG-INFO` & `py_fumen_util-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_fumen_util
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python implementation of the JavaScript package 'FumenUtil'
 Project-URL: Source, https://github.com/OctupusTea/py-fumen-util
 Author: Octupus Tea
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -30,20 +30,22 @@
 ```
 
 - `command`: Command(s) to execute on the Fumen(s).
 - `file`: File with Fumen strings, separated with whitespace and/or linebreak. Use "-" to read from standard input.
 
 ### Commands
 
-Commands are case-insensitive.
+ommands are case-insensitive.
 
 |Command|Description|Alias|
 |:-|:-|:-|
-|Combine|Combine multiple Fumens into one|Concat, Join|
-|Split|Split each page into a Fumen||
-|Glue|Glue each Fumen page into tetromino placements|Decompile|
-|Unglue|Unglue Fumen placements into one page|Compile|
-|Gray|Gray out the last of each Fumen|Grey|
-|Grayall|Gray out all pages of each Fumen|Greyall|
-|Lock|Lock the last page of each Fumen and append a new page||
-|Mirror|Mirror Fumen pages|Flip|
-|Uncomment|Uncomment Fumen pages||
+|join|Join multiple Fumens into one|combine concat|
+|split|Split each page into a Fumen||
+|assemble|Assemble Fumen placements into one page|compile, unglue|
+|disassemble|Disassemble each Fumen page into tetrimino placements|decompile, glue|
+|gray|Gray out the last page of each Fumen|grey|
+|grayall|Gray out all pages of each Fumen|greyall|
+|prune|Prune colored minos from the last page of each Fumen||
+|pruneall|Prune colored minos from all pages of each Fumen||
+|lock|Lock the last page of each Fumen and append a new page||
+|mirror|Mirror Fumen pages|flip|
+|uncomment|Uncomment Fumen pages||
```

