# Comparing `tmp/codestripper-0.1.2.tar.gz` & `tmp/codestripper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codestripper-0.1.2.tar", max compression
+gzip compressed data, was "codestripper-0.1.3.tar", max compression
```

## Comparing `codestripper-0.1.2.tar` & `codestripper-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1080 2023-03-16 12:12:41.822926 codestripper-0.1.2/LICENSE
--rw-r--r--   0        0        0     6868 2023-03-16 12:12:41.822926 codestripper-0.1.2/README.md
--rw-r--r--   0        0        0       65 2023-03-16 12:12:41.822926 codestripper-0.1.2/codestripper/__init__.py
--rw-r--r--   0        0        0       85 2023-03-16 12:12:41.822926 codestripper-0.1.2/codestripper/__main__.py
--rw-r--r--   0        0        0     2157 2023-03-16 12:12:41.822926 codestripper-0.1.2/codestripper/cli.py
--rw-r--r--   0        0        0     3549 2023-03-16 12:12:41.822926 codestripper-0.1.2/codestripper/code_stripper.py
--rw-r--r--   0        0        0      585 2023-03-16 12:12:41.822926 codestripper-0.1.2/codestripper/errors.py
--rw-r--r--   0        0        0      471 2023-03-16 12:12:41.822926 codestripper-0.1.2/codestripper/tags/__init__.py
--rw-r--r--   0        0        0      328 2023-03-16 12:12:41.822926 codestripper-0.1.2/codestripper/tags/add.py
--rw-r--r--   0        0        0      142 2023-03-16 12:12:41.822926 codestripper-0.1.2/codestripper/tags/errors.py
--rw-r--r--   0        0        0      439 2023-03-16 12:12:41.822926 codestripper-0.1.2/codestripper/tags/ignore_file.py
--rw-r--r--   0        0        0     1707 2023-03-16 12:12:41.822926 codestripper-0.1.2/codestripper/tags/legacy.py
--rw-r--r--   0        0        0      799 2023-03-16 12:12:41.822926 codestripper-0.1.2/codestripper/tags/remove.py
--rw-r--r--   0        0        0      290 2023-03-16 12:12:41.822926 codestripper-0.1.2/codestripper/tags/replace.py
--rw-r--r--   0        0        0     3266 2023-03-16 12:12:41.822926 codestripper-0.1.2/codestripper/tags/tag.py
--rw-r--r--   0        0        0     1040 2023-03-16 12:12:41.822926 codestripper-0.1.2/codestripper/tags/uncomment.py
--rw-r--r--   0        0        0     5486 2023-03-16 12:12:41.822926 codestripper-0.1.2/codestripper/tokenizer.py
--rw-r--r--   0        0        0      141 2023-03-16 12:12:41.822926 codestripper-0.1.2/codestripper/utils/__init__.py
--rw-r--r--   0        0        0     2540 2023-03-16 12:12:41.822926 codestripper-0.1.2/codestripper/utils/file.py
--rw-r--r--   0        0        0     1660 2023-03-16 12:12:41.822926 codestripper-0.1.2/codestripper/utils/logger.py
--rw-r--r--   0        0        0      686 2023-03-16 12:12:41.822926 codestripper-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7594 1970-01-01 00:00:00.000000 codestripper-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-06-15 13:17:19.776094 codestripper-0.1.3/LICENSE
+-rw-r--r--   0        0        0     6868 2023-06-15 13:17:19.776094 codestripper-0.1.3/README.md
+-rw-r--r--   0        0        0       65 2023-06-15 13:17:19.776094 codestripper-0.1.3/codestripper/__init__.py
+-rw-r--r--   0        0        0       85 2023-06-15 13:17:19.776094 codestripper-0.1.3/codestripper/__main__.py
+-rw-r--r--   0        0        0     2157 2023-06-15 13:17:19.776094 codestripper-0.1.3/codestripper/cli.py
+-rw-r--r--   0        0        0     3903 2023-06-15 13:17:19.776094 codestripper-0.1.3/codestripper/code_stripper.py
+-rw-r--r--   0        0        0      878 2023-06-15 13:17:19.776094 codestripper-0.1.3/codestripper/errors.py
+-rw-r--r--   0        0        0      471 2023-06-15 13:17:19.776094 codestripper-0.1.3/codestripper/tags/__init__.py
+-rw-r--r--   0        0        0      328 2023-06-15 13:17:19.776094 codestripper-0.1.3/codestripper/tags/add.py
+-rw-r--r--   0        0        0      142 2023-06-15 13:17:19.776094 codestripper-0.1.3/codestripper/tags/errors.py
+-rw-r--r--   0        0        0      439 2023-06-15 13:17:19.776094 codestripper-0.1.3/codestripper/tags/ignore_file.py
+-rw-r--r--   0        0        0     1707 2023-06-15 13:17:19.776094 codestripper-0.1.3/codestripper/tags/legacy.py
+-rw-r--r--   0        0        0      799 2023-06-15 13:17:19.776094 codestripper-0.1.3/codestripper/tags/remove.py
+-rw-r--r--   0        0        0      290 2023-06-15 13:17:19.776094 codestripper-0.1.3/codestripper/tags/replace.py
+-rw-r--r--   0        0        0     3266 2023-06-15 13:17:19.776094 codestripper-0.1.3/codestripper/tags/tag.py
+-rw-r--r--   0        0        0     1040 2023-06-15 13:17:19.776094 codestripper-0.1.3/codestripper/tags/uncomment.py
+-rw-r--r--   0        0        0     5795 2023-06-15 13:17:19.776094 codestripper-0.1.3/codestripper/tokenizer.py
+-rw-r--r--   0        0        0      141 2023-06-15 13:17:19.776094 codestripper-0.1.3/codestripper/utils/__init__.py
+-rw-r--r--   0        0        0     2507 2023-06-15 13:17:19.776094 codestripper-0.1.3/codestripper/utils/file.py
+-rw-r--r--   0        0        0     1660 2023-06-15 13:17:19.776094 codestripper-0.1.3/codestripper/utils/logger.py
+-rw-r--r--   0        0        0      686 2023-06-15 13:17:19.776094 codestripper-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7594 1970-01-01 00:00:00.000000 codestripper-0.1.3/PKG-INFO
```

### Comparing `codestripper-0.1.2/LICENSE` & `codestripper-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `codestripper-0.1.2/README.md` & `codestripper-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `codestripper-0.1.2/codestripper/cli.py` & `codestripper-0.1.3/codestripper/cli.py`

 * *Files identical despite different names*

### Comparing `codestripper-0.1.2/codestripper/code_stripper.py` & `codestripper-0.1.3/codestripper/code_stripper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 import logging
 import os.path
+import shutil
 from pathlib import Path
 from typing import Union, Iterable, List
 
-from codestripper.errors import InvalidTagError
+from codestripper.errors import InvalidTagError, TokenizerError
 from codestripper.tags import IgnoreFileError
 from codestripper.tags.tag import Tag, RangeTag
 from codestripper.tokenizer import Tokenizer
 from codestripper.utils import get_working_directory
 
 logger = logging.getLogger("codestripper")
 
 
 def strip_files(files: Iterable[str], working_directory: Union[str, None] = None, comment: str = "//",
                 output: Union[Path, str] = "out", dry_run: bool = False) -> List[str]:
     cwd = get_working_directory(working_directory)
     out = os.path.join(os.getcwd(), output)
+    if os.path.isdir(out):
+        shutil.rmtree(out)
     stripped_files: List[str] = []
     for file in files:
         with open(os.path.join(cwd, file), 'r') as handle:
             content = handle.read()
         if content is not None:
             try:
                 stripped = CodeStripper(content, comment).strip()
             except IgnoreFileError:
-                logger.info(f"File '{file} is ignore, because of ignore tag'")
+                logger.info(f"File '{file}' is ignored, because of ignore tag")
                 continue
+            except TokenizerError as te:
+                logger.error(f"{file}:{te.line_number}: {te.message}")
+                break
+            except InvalidTagError as ie:
+                logger.error(f"{file}:{ie.line_number}: {ie.message}")
+                break
             stripped_files.append(file)
             if dry_run:
                 logger.info(stripped)
             else:
                 path = os.path.join(out, file)
                 os.makedirs(os.path.dirname(path), exist_ok=True)
                 with open(path, 'w+') as handle:
```

### Comparing `codestripper-0.1.2/codestripper/tags/legacy.py` & `codestripper-0.1.3/codestripper/tags/legacy.py`

 * *Files identical despite different names*

### Comparing `codestripper-0.1.2/codestripper/tags/remove.py` & `codestripper-0.1.3/codestripper/tags/remove.py`

 * *Files identical despite different names*

### Comparing `codestripper-0.1.2/codestripper/tags/tag.py` & `codestripper-0.1.3/codestripper/tags/tag.py`

 * *Files identical despite different names*

### Comparing `codestripper-0.1.2/codestripper/tags/uncomment.py` & `codestripper-0.1.3/codestripper/tags/uncomment.py`

 * *Files identical despite different names*

### Comparing `codestripper-0.1.2/codestripper/tokenizer.py` & `codestripper-0.1.3/codestripper/tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 from typing import Optional, Set, Dict, Callable, List, Pattern, Tuple, Type
 
+from codestripper.errors import TokenizerError
 from codestripper.tags import ReplaceTag, UncommentCloseTag, IgnoreFileTag, RemoveOpenTag, RemoveCloseTag, \
     UncommentOpenTag, LegacyOpenTag, LegacyCloseTag, RemoveTag, AddTag
 from codestripper.tags.tag import SingleTag, Tag, RangeOpenTag, RangeCloseTag, RangeTag, TagData
 
 default_tags: Set[Type[SingleTag]] = {
     IgnoreFileTag,
     RemoveOpenTag,
@@ -68,32 +69,35 @@
                 line_start = line_end
             elif kind is None:
                 continue  # All groups should be named
             else:
                 data = self.__create_tag_data(self.content, line_number, line_start, line_end, match, parameter)
                 tag = Tokenizer.mappings[kind](data)
                 self.__handle_tag(tag)
-        if len(self.open_stack) != 0 or len(self.range_stack) != 0:
-            raise AssertionError("Stack not empty!")
+        if len(self.open_stack) != 0:
+            t = self.open_stack[0]
+            raise TokenizerError(t, f"There is still an unclosed {t.__class__.__name__} tag!")
+        # if len(self.range_stack) != 0:
+        #     raise TokenizerError(self.range_stack[0][0], f"")
         return self.ordered_tags
 
     def __add_range_stack(self, index: int, tag: Tag) -> None:
         if index not in self.range_stack:
             self.range_stack[index] = []
         self.range_stack[index].append(tag)  # type: ignore
 
     def __handle_tag(self, tag: Tag) -> None:
         if isinstance(tag, RangeOpenTag):
             self.open_stack.append(tag)
         elif isinstance(tag, RangeCloseTag):
             if len(self.open_stack) == 0:
-                raise AssertionError("Stack is empty")
+                raise TokenizerError(tag, f"Cannot close tag {tag.__class__.__name__}, as there is no matching open tag")
             range_open = self.open_stack.pop()
             if range_open.parent != tag.parent:
-                raise AssertionError(f"Cannot match closing tag: {tag} to open tag: {range_open}")
+                raise TokenizerError(tag, f"Cannot match closing tag: {tag.__class__.__name__} to open tag: {range_open.__class__.__name__}")
             range_tag: RangeTag = tag.parent(range_open, tag)
             index = len(self.open_stack)
             embedded = self.range_stack.pop(index + 1, None)
             if embedded is not None:
                 range_tag.add_tags(embedded)
 
             if index > 0:
```

### Comparing `codestripper-0.1.2/codestripper/utils/file.py` & `codestripper-0.1.3/codestripper/utils/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,19 +34,19 @@
         self.recursive = recursive
         self.old_cwd = os.getcwd()
         self.cwd = get_working_directory(working_directory)
 
     def __get_normalized_files(self, file_names: Iterable[str], relative_to: Path, recursive=True) -> \
             Generator[str, None, None]:
         for file_name in file_names:
-            path = Path(os.path.join(self.cwd, file_name)).resolve().as_posix()
+            path = os.path.join(self.cwd, file_name)
             for file in glob.glob(path, recursive=recursive):
                 tmp = Path(file).relative_to(relative_to)
                 if tmp.is_file():
-                    yield tmp.as_posix()
+                    yield str(tmp)
 
     def __convert_to_paths_set(self, file_names: Iterable[str], recursive=True) -> Set[str]:
         """Convert the file name(s) that are passed as CLI arguments to file paths (can contain GLOB)"""
         files = set()
         for file in self.__get_normalized_files(file_names, Path(self.cwd), recursive):
             files.add(file)
         return files
```

### Comparing `codestripper-0.1.2/codestripper/utils/logger.py` & `codestripper-0.1.3/codestripper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `codestripper-0.1.2/pyproject.toml` & `codestripper-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codestripper"
-version = "0.1.2"
+version = "0.1.3"
 description = "CodeStripper used to strip code from assignments"
 authors = ["Bonajo <m.bonajo@fontys.nl>"]
 maintainers = ["Bonajo <m.bonajo@fontys.nl>"]
 homepage = "https://github.com/FontysVenlo/codestripper"
 repository = "https://github.com/FontysVenlo/codestripper"
 readme = "README.md"
 packages = [{include = "codestripper"}]
```

### Comparing `codestripper-0.1.2/PKG-INFO` & `codestripper-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codestripper
-Version: 0.1.2
+Version: 0.1.3
 Summary: CodeStripper used to strip code from assignments
 Home-page: https://github.com/FontysVenlo/codestripper
 License: MIT
 Author: Bonajo
 Author-email: m.bonajo@fontys.nl
 Maintainer: Bonajo
 Maintainer-email: m.bonajo@fontys.nl
```

