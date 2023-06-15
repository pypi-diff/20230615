# Comparing `tmp/biblelib-0.2.8.tar.gz` & `tmp/biblelib-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biblelib-0.2.8.tar", max compression
+gzip compressed data, was "biblelib-0.2.9.tar", max compression
```

## Comparing `biblelib-0.2.8.tar` & `biblelib-0.2.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     3326 2023-05-12 17:59:15.958698 biblelib-0.2.8/LICENSE.md
--rw-r--r--   0        0        0     3337 2023-05-12 17:50:39.199097 biblelib-0.2.8/LICENSE.md~
--rw-r--r--   0        0        0     2048 2023-05-12 17:45:43.797503 biblelib-0.2.8/README.md
--rw-r--r--   0        0        0      207 2022-11-11 00:55:36.561996 biblelib-0.2.8/biblelib/__init__.py
--rw-r--r--   0        0        0      946 2023-05-12 17:25:25.324552 biblelib-0.2.8/biblelib/book/ReadMe.md
--rw-r--r--   0        0        0      350 2023-03-24 13:53:37.422750 biblelib-0.2.8/biblelib/book/__init__.py
--rw-r--r--   0        0        0    12780 2023-04-22 23:14:16.335752 biblelib-0.2.8/biblelib/book/book.py
--rw-r--r--   0        0        0     4755 2023-05-30 01:05:17.747681 biblelib-0.2.8/biblelib/book/books.tsv
--rw-r--r--   0        0        0      474 2023-04-09 04:44:24.570950 biblelib-0.2.8/biblelib/unit/__init__.py
--rw-r--r--   0        0        0     5788 2023-04-10 12:29:36.110427 biblelib-0.2.8/biblelib/unit/book.py
--rw-r--r--   0        0        0     1770 2023-03-30 03:30:47.201892 biblelib-0.2.8/biblelib/unit/bookchapters.tsv
--rw-r--r--   0        0        0     6972 2023-04-10 12:30:22.815665 biblelib-0.2.8/biblelib/unit/chapter.py
--rw-r--r--   0        0        0     1770 2023-03-24 23:24:06.076120 biblelib-0.2.8/biblelib/unit/chapters.tsv
--rw-r--r--   0        0        0    23363 2023-03-30 03:30:50.093429 biblelib-0.2.8/biblelib/unit/chapterverses.tsv
--rw-r--r--   0        0        0    29962 2023-03-30 03:30:33.249866 biblelib-0.2.8/biblelib/unit/tempchapter.py
--rw-r--r--   0        0        0     3332 2023-03-30 05:04:49.035453 biblelib-0.2.8/biblelib/unit/unit.py
--rw-r--r--   0        0        0     1240 2023-03-24 18:41:28.150962 biblelib-0.2.8/biblelib/unit/verse.py
--rw-r--r--   0        0        0     1348 2023-05-12 17:27:37.060726 biblelib-0.2.8/biblelib/versification/ReadMe.md
--rw-r--r--   0        0        0   431827 2021-10-25 18:19:51.303000 biblelib-0.2.8/biblelib/versification/vref-bcv.txt
--rw-r--r--   0        0        0   431827 2021-10-25 18:19:51.303000 biblelib-0.2.8/biblelib/versification/vref.txt
--rw-r--r--   0        0        0      199 2023-05-08 18:22:24.370434 biblelib-0.2.8/biblelib/versification/vrefmap.py
--rw-r--r--   0        0        0      786 2023-05-26 19:35:46.225675 biblelib-0.2.8/biblelib/word/__init__.py
--rw-r--r--   0        0        0    16067 2023-05-30 00:44:58.415393 biblelib-0.2.8/biblelib/word/bcvwpid.py
--rw-r--r--   0        0        0     4432 2022-11-17 00:30:21.039343 biblelib-0.2.8/biblelib/word/mappings.py
--rw-r--r--   0        0        0     1189 2023-05-30 01:06:40.167862 biblelib-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     2843 1970-01-01 00:00:00.000000 biblelib-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     3326 2023-05-12 17:59:15.958698 biblelib-0.2.9/LICENSE.md
+-rw-r--r--   0        0        0     3337 2023-05-12 17:50:39.199097 biblelib-0.2.9/LICENSE.md~
+-rw-r--r--   0        0        0     2048 2023-05-12 17:45:43.797503 biblelib-0.2.9/README.md
+-rw-r--r--   0        0        0      207 2022-11-11 00:55:36.561996 biblelib-0.2.9/biblelib/__init__.py
+-rw-r--r--   0        0        0      946 2023-05-12 17:25:25.324552 biblelib-0.2.9/biblelib/book/ReadMe.md
+-rw-r--r--   0        0        0      350 2023-03-24 13:53:37.422750 biblelib-0.2.9/biblelib/book/__init__.py
+-rw-r--r--   0        0        0    13486 2023-05-30 16:48:10.045751 biblelib-0.2.9/biblelib/book/book.py
+-rw-r--r--   0        0        0     4755 2023-05-30 01:05:17.747681 biblelib-0.2.9/biblelib/book/books.tsv
+-rw-r--r--   0        0        0      474 2023-04-09 04:44:24.570950 biblelib-0.2.9/biblelib/unit/__init__.py
+-rw-r--r--   0        0        0     5788 2023-04-10 12:29:36.110427 biblelib-0.2.9/biblelib/unit/book.py
+-rw-r--r--   0        0        0     1770 2023-03-30 03:30:47.201892 biblelib-0.2.9/biblelib/unit/bookchapters.tsv
+-rw-r--r--   0        0        0     6972 2023-04-10 12:30:22.815665 biblelib-0.2.9/biblelib/unit/chapter.py
+-rw-r--r--   0        0        0     1770 2023-03-24 23:24:06.076120 biblelib-0.2.9/biblelib/unit/chapters.tsv
+-rw-r--r--   0        0        0    23363 2023-03-30 03:30:50.093429 biblelib-0.2.9/biblelib/unit/chapterverses.tsv
+-rw-r--r--   0        0        0    29962 2023-03-30 03:30:33.249866 biblelib-0.2.9/biblelib/unit/tempchapter.py
+-rw-r--r--   0        0        0     3332 2023-03-30 05:04:49.035453 biblelib-0.2.9/biblelib/unit/unit.py
+-rw-r--r--   0        0        0     1240 2023-03-24 18:41:28.150962 biblelib-0.2.9/biblelib/unit/verse.py
+-rw-r--r--   0        0        0     1348 2023-05-12 17:27:37.060726 biblelib-0.2.9/biblelib/versification/ReadMe.md
+-rw-r--r--   0        0        0   431827 2021-10-25 18:19:51.303000 biblelib-0.2.9/biblelib/versification/vref-bcv.txt
+-rw-r--r--   0        0        0   431827 2021-10-25 18:19:51.303000 biblelib-0.2.9/biblelib/versification/vref.txt
+-rw-r--r--   0        0        0      199 2023-05-08 18:22:24.370434 biblelib-0.2.9/biblelib/versification/vrefmap.py
+-rw-r--r--   0        0        0      812 2023-05-30 15:27:41.696166 biblelib-0.2.9/biblelib/word/__init__.py
+-rw-r--r--   0        0        0    17403 2023-05-30 17:10:39.344817 biblelib-0.2.9/biblelib/word/bcvwpid.py
+-rw-r--r--   0        0        0     4432 2022-11-17 00:30:21.039343 biblelib-0.2.9/biblelib/word/mappings.py
+-rw-r--r--   0        0        0     1189 2023-05-30 17:15:29.528137 biblelib-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     2843 1970-01-01 00:00:00.000000 biblelib-0.2.9/PKG-INFO
```

### Comparing `biblelib-0.2.8/LICENSE.md` & `biblelib-0.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.8/LICENSE.md~` & `biblelib-0.2.9/LICENSE.md~`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.8/README.md` & `biblelib-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.8/biblelib/book/ReadMe.md` & `biblelib-0.2.9/biblelib/book/ReadMe.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.8/biblelib/book/book.py` & `biblelib-0.2.9/biblelib/book/book.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 """
 
 from collections import UserDict
 from csv import DictReader
 from dataclasses import dataclass, field
 from pathlib import Path
+import re
 from typing import Union
 
 
 # This directory: where books.tsv is also located.
 BOOKSPATH = Path(__file__).parent
 
 
@@ -181,14 +182,16 @@
     # - Catholic
     # - JPS/Tanakh
     # there are others: LXX? Syriac, Ethiopian, etc.
     source: Path = BOOKSPATH / "books.tsv"
     mappingfields: set = set(Book._fieldnames)
     canon: str = "Protestant"
     logosmap: dict = {}
+    namemap: dict = {}
+    nameregexp: str = ""
     osismap: dict = {}
     usfmnumbermap: dict = {}
 
     def __init__(self, sourcefile: str = "", canon: str = "Protestant") -> None:
         """Initialize a Books instance.
 
         Instantiates a dict whose keys are 3-character USFM names.
@@ -214,14 +217,20 @@
             # make sure the fieldnames in the file are the same as the
             # dataclass attributes
             fieldnameset: set = set(reader.fieldnames[0].split("\t"))
             assert not fieldnameset.difference(
                 self.mappingfields
             ), f"Fieldname discrepancy header: {fieldnameset} vs {self.mappingfields}"
             self.data = {row["usfmname"]: self.rowtobook(row) for row in reader}
+        # initialize here so you have nameregexp before calling fromname()
+        self.namemap = {b.name: b for _, b in self.data.items()}
+        # use this for matching a reference string to determine if
+        # it's only a book name. Hack like checking for a space or
+        # number are not roubst enough.
+        self.nameregexp = re.compile("|".join(self.namemap.keys()))
 
     @staticmethod
     def rowtobook(row: dict) -> Book:
         """Convert a raw dict read from TSV to data for Book."""
         # logosID should be an int
         row["logosID"] = int(row["logosID"])
         # zero-pad initial USFM numbers
@@ -246,14 +255,23 @@
                 logosID = int(logosID)
         if not self.logosmap:
             # initialize on demand
             self.logosmap = {b.logosID: b for _, b in self.data.items()}
         assert logosID in self.logosmap, f"Invalid logosID {logosID}"
         return self.logosmap[logosID]
 
+    def fromname(self, bookname: str) -> Book:
+        """Return the book instance for a book name.
+
+        Args:
+            bookname: the full name  to use in looking up the Book,
+                like "Matthew".
+        """
+        return self.namemap[bookname]
+
     def fromosis(self, osisID: str) -> Book:
         """Return the book instance for an OSIS identifier.
 
         Args:
             osisID: the OSIS identifier to use in looking up the Book,
                 like "Matt".
         """
```

### Comparing `biblelib-0.2.8/biblelib/book/books.tsv` & `biblelib-0.2.9/biblelib/book/books.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.8/biblelib/unit/book.py` & `biblelib-0.2.9/biblelib/unit/book.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.8/biblelib/unit/bookchapters.tsv` & `biblelib-0.2.9/biblelib/unit/bookchapters.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.8/biblelib/unit/chapter.py` & `biblelib-0.2.9/biblelib/unit/chapter.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.8/biblelib/unit/chapters.tsv` & `biblelib-0.2.9/biblelib/unit/chapters.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.8/biblelib/unit/chapterverses.tsv` & `biblelib-0.2.9/biblelib/unit/chapterverses.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.8/biblelib/unit/tempchapter.py` & `biblelib-0.2.9/biblelib/unit/tempchapter.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.8/biblelib/unit/unit.py` & `biblelib-0.2.9/biblelib/unit/unit.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.8/biblelib/unit/verse.py` & `biblelib-0.2.9/biblelib/unit/verse.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.8/biblelib/versification/ReadMe.md` & `biblelib-0.2.9/biblelib/versification/ReadMe.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.8/biblelib/versification/vref-bcv.txt` & `biblelib-0.2.9/biblelib/versification/vref-bcv.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.8/biblelib/versification/vref.txt` & `biblelib-0.2.9/biblelib/versification/vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.8/biblelib/word/__init__.py` & `biblelib-0.2.9/biblelib/word/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,19 +11,20 @@
   [Clear-Bible/macula-greek](https://github.com/Clear-Bible/macula-greek):
   Syntax trees, morphology, and linguistic annotations for the Greek
   New Testament
 
 """
 
 from .mappings import Mapping, Mappings
-from .bcvwpid import fromlogos, fromosis, fromusfm, BID, BCID, BCVID, BCVWPID
+from .bcvwpid import fromlogos, fromname, fromosis, fromusfm, BID, BCID, BCVID, BCVWPID
 
 __all__ = [
     # bcvwpid
     "fromlogos",
+    "fromname",
     "fromosis",
     "fromusfm",
     "BID",
     "BCID",
     "BCVID",
     "BCVWPID",
     # words
```

### Comparing `biblelib-0.2.8/biblelib/word/bcvwpid.py` & `biblelib-0.2.9/biblelib/word/bcvwpid.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,14 @@
 - methods for rendering in various formats
 
 """
 
 
 from dataclasses import dataclass, field
 
-# import re
-# from typing import Union
-
 from biblelib.book import Books
 
 BOOKS = Books()
 
 
 @dataclass(order=True)
 class BID:
@@ -397,28 +394,62 @@
     references like MRK 4:8. Does not handle ranges or non-numeric
     verses like 'title'. Does not check the validity of chapter and
     verse numbers for the book. Book name must be correctly cased.
 
     """
     if " " not in ref:
         # book only
-        usfmbook = BOOKS.fromosis(ref.capitalize()).usfmnumber
+        usfmbook = BOOKS.fromosis(ref).usfmnumber
         return BID((usfmbook))
     else:
         bookabbrev, rest = ref.split(" ", 1)
         usfmbook = BOOKS.fromosis(bookabbrev).usfmnumber
         if ":" not in rest:
             # book and chapter
             return BCID(f"{usfmbook}{pad3(rest)}")
         else:
             # book, chapter, verse
             chapter, verse = rest.split(":", 1)
             return BCVID(f"{usfmbook}{pad3(chapter)}{pad3(verse)}")
 
 
+def fromname(ref) -> BID | BCID | BCVID:
+    """Return a BCV instance for a full name reference.
+
+    Only handles book, book + chapter, and book chapter verse
+    references like 1 Corinthians 4:8. Does not handle ranges or
+    non-numeric verses like 'title'. Does not check the validity of
+    chapter and verse numbers for the book. Book name must be
+    correctly cased.
+
+    """
+    # complex check because book names can contain spaces and other numbers
+    # must match a regexp of all the book names, and be the same length
+    namematch = BOOKS.nameregexp.match(ref)
+    assert namematch, f"Invalid name reference: {ref}"
+    if len(ref) == (namematch.end() - namematch.start()):
+        # book only
+        usfmbook = BOOKS.fromname(ref).usfmnumber
+        return BID((usfmbook))
+    else:
+        # split namematch at the end of the match
+        bookname, rest = ref[: namematch.end()], ref[(namematch.end() + 1) :]
+        usfmbook = BOOKS.fromname(bookname).usfmnumber
+        if ":" not in rest:
+            # book and chapter
+            return BCID(f"{usfmbook}{pad3(rest)}")
+        else:
+            # book, chapter, verse
+            try:
+                chapter, verse = rest.split(":", 1)
+                return BCVID(f"{usfmbook}{pad3(chapter)}{pad3(verse)}")
+            except Exception as e:
+                raise ValueError(f"Invalid BCV values: {ref}\n{e}")
+
+
 def fromusfm(ref) -> BID | BCID | BCVID:
     """Return a BCV instance for a USFM-based reference.
 
     Only handles book, book + chapter, and book chapter verse
     references like MRK 4:8. Does not handle ranges or non-numeric
     verses like 'title'. Does not check the validity of chapter and
     verse numbers for the book.
```

### Comparing `biblelib-0.2.8/biblelib/word/mappings.py` & `biblelib-0.2.9/biblelib/word/mappings.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.8/pyproject.toml` & `biblelib-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "biblelib"
-version = "0.2.8"
+version = "0.2.9"
 description = "Utilities for working with metadata for Bible books, references, pericopes, and other units."
 authors = ["Sean Boisen <sean.boisen@gmail.com>"]
 repository = "https://github.com/Clear-Bible/Biblelib/"
 # documentation = "https://sboisen.github.io/Biblelib/"
 readme = "README.md"
 packages = [
   {include = "biblelib"}
```

### Comparing `biblelib-0.2.8/PKG-INFO` & `biblelib-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biblelib
-Version: 0.2.8
+Version: 0.2.9
 Summary: Utilities for working with metadata for Bible books, references, pericopes, and other units.
 Home-page: https://github.com/Clear-Bible/Biblelib/
 Author: Sean Boisen
 Author-email: sean.boisen@gmail.com
 Requires-Python: >=3.8,<=3.11
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

