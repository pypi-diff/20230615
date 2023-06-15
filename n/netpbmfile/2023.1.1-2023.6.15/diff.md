# Comparing `tmp/netpbmfile-2023.1.1.tar.gz` & `tmp/netpbmfile-2023.6.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netpbmfile-2023.1.1.tar", last modified: Sun Jan  1 08:54:19 2023, max compression
+gzip compressed data, was "netpbmfile-2023.6.15.tar", last modified: Thu Jun 15 17:37:48 2023, max compression
```

## Comparing `netpbmfile-2023.1.1.tar` & `netpbmfile-2023.6.15.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-01-01 08:54:19.494452 netpbmfile-2023.1.1/
--rw-rw-rw-   0        0        0     1559 2023-01-01 08:54:17.000000 netpbmfile-2023.1.1/LICENSE
--rw-rw-rw-   0        0        0      421 2023-01-01 03:01:04.000000 netpbmfile-2023.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5040 2023-01-01 08:54:19.494452 netpbmfile-2023.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4106 2023-01-01 08:54:17.000000 netpbmfile-2023.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-01-01 08:54:19.485513 netpbmfile-2023.1.1/netpbmfile/
--rw-rw-rw-   0        0        0      110 2020-01-01 10:25:54.000000 netpbmfile-2023.1.1/netpbmfile/__init__.py
--rw-rw-rw-   0        0        0      141 2020-01-09 14:46:14.000000 netpbmfile-2023.1.1/netpbmfile/__main__.py
--rw-rw-rw-   0        0        0    38306 2023-01-01 08:53:37.000000 netpbmfile-2023.1.1/netpbmfile/netpbmfile.py
-drwxrwxrwx   0        0        0        0 2023-01-01 08:54:19.493547 netpbmfile-2023.1.1/netpbmfile.egg-info/
--rw-rw-rw-   0        0        0     5040 2023-01-01 08:54:18.000000 netpbmfile-2023.1.1/netpbmfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-01-01 08:54:19.000000 netpbmfile-2023.1.1/netpbmfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-01 08:54:18.000000 netpbmfile-2023.1.1/netpbmfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-01-01 08:54:18.000000 netpbmfile-2023.1.1/netpbmfile.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       41 2023-01-01 08:54:18.000000 netpbmfile-2023.1.1/netpbmfile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-01-01 08:54:18.000000 netpbmfile-2023.1.1/netpbmfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-01 08:54:19.494452 netpbmfile-2023.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2596 2022-10-25 19:59:23.000000 netpbmfile-2023.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-01 08:54:19.494452 netpbmfile-2023.1.1/tests/
--rw-rw-rw-   0        0        0      659 2022-12-29 21:08:30.000000 netpbmfile-2023.1.1/tests/conftest.py
--rw-rw-rw-   0        0        0    31872 2022-12-28 01:08:37.000000 netpbmfile-2023.1.1/tests/data.npy
--rw-rw-rw-   0        0        0    15441 2023-01-01 08:50:42.000000 netpbmfile-2023.1.1/tests/test_netpbmfile.py
+drwxrwxrwx   0        0        0        0 2023-06-15 17:37:48.253497 netpbmfile-2023.6.15/
+-rw-rw-rw-   0        0        0     1559 2023-06-15 17:37:43.000000 netpbmfile-2023.6.15/LICENSE
+-rw-rw-rw-   0        0        0      421 2023-01-01 03:01:04.000000 netpbmfile-2023.6.15/MANIFEST.in
+-rw-rw-rw-   0        0        0     5137 2023-06-15 17:37:48.253497 netpbmfile-2023.6.15/PKG-INFO
+-rw-rw-rw-   0        0        0     4201 2023-06-15 17:37:43.000000 netpbmfile-2023.6.15/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-15 17:37:48.237854 netpbmfile-2023.6.15/netpbmfile/
+-rw-rw-rw-   0        0        0      110 2020-01-01 10:25:54.000000 netpbmfile-2023.6.15/netpbmfile/__init__.py
+-rw-rw-rw-   0        0        0      141 2020-01-09 14:46:14.000000 netpbmfile-2023.6.15/netpbmfile/__main__.py
+-rw-rw-rw-   0        0        0    38418 2023-06-15 17:25:26.000000 netpbmfile-2023.6.15/netpbmfile/netpbmfile.py
+drwxrwxrwx   0        0        0        0 2023-06-15 17:37:48.253497 netpbmfile-2023.6.15/netpbmfile.egg-info/
+-rw-rw-rw-   0        0        0     5137 2023-06-15 17:37:47.000000 netpbmfile-2023.6.15/netpbmfile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-06-15 17:37:48.000000 netpbmfile-2023.6.15/netpbmfile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 17:37:47.000000 netpbmfile-2023.6.15/netpbmfile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-15 17:37:47.000000 netpbmfile-2023.6.15/netpbmfile.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       41 2023-06-15 17:37:47.000000 netpbmfile-2023.6.15/netpbmfile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-15 17:37:47.000000 netpbmfile-2023.6.15/netpbmfile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 17:37:48.253497 netpbmfile-2023.6.15/setup.cfg
+-rw-rw-rw-   0        0        0     2621 2023-06-15 17:25:57.000000 netpbmfile-2023.6.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 17:37:48.253497 netpbmfile-2023.6.15/tests/
+-rw-rw-rw-   0        0        0      659 2022-12-29 21:08:30.000000 netpbmfile-2023.6.15/tests/conftest.py
+-rw-rw-rw-   0        0        0    31872 2022-12-28 01:08:37.000000 netpbmfile-2023.6.15/tests/data.npy
+-rw-rw-rw-   0        0        0    15522 2023-06-15 17:37:21.000000 netpbmfile-2023.6.15/tests/test_netpbmfile.py
```

### Comparing `netpbmfile-2023.1.1/LICENSE` & `netpbmfile-2023.6.15/LICENSE`

 * *Files identical despite different names*

### Comparing `netpbmfile-2023.1.1/PKG-INFO` & `netpbmfile-2023.6.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: netpbmfile
-Version: 2023.1.1
+Version: 2023.6.15
 Summary: Read and write Netpbm files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/netpbmfile/issues
 Project-URL: Source Code, https://github.com/cgohlke/netpbmfile
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Provides-Extra: all
 License-File: LICENSE
 
 Read and write Netpbm files
 ===========================
 
@@ -42,15 +42,15 @@
 
 The PGX format is specified in ITU-T Rec. T.803.
 
 No gamma correction or scaling is performed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.1.1
+:Version: 2023.6.15
 
 Quickstart
 ----------
 
 Install the netpbmfile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/netpbmfile/>`_::
 
@@ -60,23 +60,28 @@
 
 Source code and support are available on
 `GitHub <https://github.com/cgohlke/netpbmfile>`_.
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.9, 3.11.1 <https://www.python.org>`_
-- `NumPy 1.23.5 <https://pypi.org/project/numpy/>`_
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.4, 3.12.0b2
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
 
 Revisions
 ---------
 
+2023.6.15
+
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+- Improve type hints.
+
 2023.1.1
 
 - Several breaking changes:
 - Rename magicnum to magicnumber (breaking).
 - Rename tupltypes to tupltype (breaking).
 - Change magicnumber and header properties to str (breaking).
 - Replace pam parameter with magicnumber (breaking).
```

### Comparing `netpbmfile-2023.1.1/README.rst` & `netpbmfile-2023.6.15/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 The PGX format is specified in ITU-T Rec. T.803.
 
 No gamma correction or scaling is performed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.1.1
+:Version: 2023.6.15
 
 Quickstart
 ----------
 
 Install the netpbmfile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/netpbmfile/>`_::
 
@@ -35,23 +35,28 @@
 
 Source code and support are available on
 `GitHub <https://github.com/cgohlke/netpbmfile>`_.
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.9, 3.11.1 <https://www.python.org>`_
-- `NumPy 1.23.5 <https://pypi.org/project/numpy/>`_
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.4, 3.12.0b2
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
 
 Revisions
 ---------
 
+2023.6.15
+
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+- Improve type hints.
+
 2023.1.1
 
 - Several breaking changes:
 - Rename magicnum to magicnumber (breaking).
 - Rename tupltypes to tupltype (breaking).
 - Change magicnumber and header properties to str (breaking).
 - Replace pam parameter with magicnumber (breaking).
```

### Comparing `netpbmfile-2023.1.1/netpbmfile/netpbmfile.py` & `netpbmfile-2023.6.15/netpbmfile/netpbmfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 The PGX format is specified in ITU-T Rec. T.803.
 
 No gamma correction or scaling is performed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.1.1
+:Version: 2023.6.15
 
 Quickstart
 ----------
 
 Install the netpbmfile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/netpbmfile/>`_::
 
@@ -65,23 +65,28 @@
 
 Source code and support are available on
 `GitHub <https://github.com/cgohlke/netpbmfile>`_.
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.9, 3.11.1 <https://www.python.org>`_
-- `NumPy 1.23.5 <https://pypi.org/project/numpy/>`_
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.4, 3.12.0b2
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
 
 Revisions
 ---------
 
+2023.6.15
+
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+- Improve type hints.
+
 2023.1.1
 
 - Several breaking changes:
 - Rename magicnum to magicnumber (breaking).
 - Rename tupltypes to tupltype (breaking).
 - Change magicnumber and header properties to str (breaking).
 - Replace pam parameter with magicnumber (breaking).
@@ -182,39 +187,34 @@
 
     $ python -m netpbmfile _tmp.pgm
 
 """
 
 from __future__ import annotations
 
-__version__ = '2023.1.1'
+__version__ = '2023.6.15'
 
 __all__ = ['imread', 'imwrite', 'imsave', 'NetpbmFile']
 
 import sys
 import os
 import re
 import math
 import warnings
 
 import numpy
 
-
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from typing import BinaryIO, Iterable, Literal, Union
+    from typing import Any, BinaryIO, Literal, Union
+    from collections.abc import Iterable
 
-    try:
-        from numpy.typing import ArrayLike
-    except ImportError:
-        # numpy < 1.20
-        from numpy import ndarray as ArrayLike
+    from numpy.typing import ArrayLike, NDArray
 
-    PathLike = Union[str, os.PathLike]
     ByteOrder = Union[Literal['>'], Literal['<']]
     MagicNumber = Union[
         Literal['P1'],
         Literal['P2'],
         Literal['P3'],
         Literal['P4'],
         Literal['P5'],
@@ -225,16 +225,19 @@
         Literal['PF'],
         Literal['PF4'],
         Literal['P7 332'],
     ]
 
 
 def imread(
-    file: PathLike | BinaryIO, /, *, byteorder: ByteOrder | None = None
-) -> numpy.ndarray:
+    file: str | os.PathLike[Any] | BinaryIO,
+    /,
+    *,
+    byteorder: ByteOrder | None = None,
+) -> NDArray[Any]:
     """Return image data from Netpbm file.
 
     Parameters:
         file:
             Name of file or open binary file to read.
         byteorder:
             Byte order of image data in file.
@@ -244,15 +247,15 @@
     """
     with NetpbmFile(file, byteorder=byteorder) as netpbm:
         image = netpbm.asarray()
     return image
 
 
 def imwrite(
-    file: PathLike | BinaryIO,
+    file: str | os.PathLike[Any] | BinaryIO,
     data: ArrayLike,
     /,
     *,
     magicnumber: MagicNumber | None = None,
     maxval: int | None = None,
     tupltype: str | None = None,
     byteorder: ByteOrder | None = None,
@@ -339,21 +342,21 @@
 
     filename: str
     """File name."""
 
     tupltype: str
     """Kind of PAM image."""
 
-    dtype: numpy.dtype
+    dtype: numpy.dtype[Any]
     """Data type of image array."""
 
     dataoffset: int
     """Position of image data in file."""
 
-    _data: numpy.ndarray | None
+    _data: NDArray[Any] | None
     _fh: BinaryIO | None
 
     MAGIC_NUMBER: dict[str, str] = {
         'P1': 'BLACKANDWHITE',
         'P2': 'GRAYSCALE',
         'P3': 'RGB',
         'P4': 'BLACKANDWHITE',
@@ -365,15 +368,15 @@
         'PF': 'RGB_FLOAT',
         'PF4': 'RGB_ALPHA_FLOAT',
         'PG': 'GRAYSCALE',
     }
 
     def __init__(
         self,
-        file: PathLike | BinaryIO | None,
+        file: str | os.PathLike[Any] | BinaryIO | None,
         /,
         *,
         byteorder: ByteOrder | None = None,
     ) -> None:
         # initialize instance from filename or open file
         self.header = ''
         self.magicnumber = 'P7'
@@ -430,15 +433,15 @@
         if byteorder is not None:
             self.byteorder = byteorder
 
         if self.magicnumber in 'P1 P4':
             dtype = 'bool_'
         elif self.magicnumber in 'PF4 Pf':
             dtype = self.byteorder + 'f4'
-        elif self.magicnumber == 'PG':
+        elif self.magicnumber in 'PG':
             dtype = self.byteorder + self.dtype.char
         elif self.maxval < 256:
             dtype = 'u1'
         elif self.maxval < 65536:
             dtype = self.byteorder + 'u2'
         elif self.maxval < 2**32:
             dtype = self.byteorder + 'u4'
@@ -450,15 +453,15 @@
         if self.magicnumber in 'P1 P2 P3':
             self.frames = 1
         else:
             bytecount = self._fh.seek(0, 2) - len(self.header)
             shape = [
                 self.height,
                 int(math.ceil(self.width / 8))
-                if self.magicnumber == 'P4'
+                if self.magicnumber in 'P4'
                 else self.width,
                 self.depth,
                 self.dtype.itemsize,
             ]
             self.frames = max(1, bytecount // product(shape))
 
     @classmethod
@@ -613,15 +616,15 @@
         return self
 
     def asarray(
         self,
         *,
         copy: bool = True,
         cache: bool = False,
-    ) -> numpy.ndarray:
+    ) -> NDArray[Any]:
         """Return image array.
 
         Parameters:
             copy:
                 Return a copy of image array.
             cache:
                 Keep a copy of image data after reading from file.
@@ -635,15 +638,15 @@
                 self._data = data
             else:
                 return data
         return numpy.copy(data) if copy else data
 
     def write(
         self,
-        file: PathLike | BinaryIO,
+        file: str | os.PathLike[Any] | BinaryIO,
         /,
         *,
         magicnumber: MagicNumber | None = None,
         byteorder: ByteOrder | None = None,
         comment: str | None = None,
     ) -> None:
         """Write instance to file.
@@ -820,15 +823,15 @@
         elif bitdepth <= 32:
             self.dtype = numpy.dtype(
                 self.byteorder + ('i4' if signed else 'u4')
             )
         else:
             raise ValueError(f'bitdepth {bitdepth} out of range')
 
-    def _read_data(self, fh: BinaryIO) -> numpy.ndarray:
+    def _read_data(self, fh: BinaryIO) -> NDArray[Any]:
         """Return image data from open file."""
         fh.seek(self.dataoffset)
 
         bilevel = self.magicnumber in 'P1 P4'
         dtype = self.dtype if not bilevel else numpy.dtype('u1')
         depth = self.depth if self.magicnumber != 'P7 332' else 1
         shape = [-1, self.height, self.width, depth]
@@ -1025,15 +1028,15 @@
                 f'{self.width} {self.height} {self.maxval}\n'
             )
         raise ValueError(f'writing {magicnumber!r} format not supported')
 
     def __enter__(self) -> NetpbmFile:
         return self
 
-    def __exit__(self, exc_type, exc_value, traceback):
+    def __exit__(self, exc_type, exc_value, traceback):  # type: ignore
         self.close()
 
     def __repr__(self) -> str:
         if self.filename:
             arg = f'{os.path.split(os.path.normcase(self.filename))[-1]!r}'
         elif self._fh is not None:
             arg = str(type(self._fh).__name__)
@@ -1059,23 +1062,23 @@
     """Return product of sequence of numbers."""
     prod = 1
     for i in iterable:
         prod *= i
     return prod
 
 
-def indent(*args) -> str:
+def indent(*args: Any) -> str:
     """Return joined string representations of objects with indented lines."""
     text = '\n'.join(str(arg) for arg in args)
     return '\n'.join(
         ('  ' + line if line else line) for line in text.splitlines() if line
     )[2:]
 
 
-def log_warning(msg, *args, **kwargs):
+def log_warning(msg: object, *args: object, **kwargs: Any) -> None:
     """Log message with level WARNING."""
     import logging
 
     logging.getLogger('netpbmfile').warning(msg, *args, **kwargs)
 
 
 def main(argv: list[str] | None = None) -> int:
```

### Comparing `netpbmfile-2023.1.1/netpbmfile.egg-info/PKG-INFO` & `netpbmfile-2023.6.15/netpbmfile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: netpbmfile
-Version: 2023.1.1
+Version: 2023.6.15
 Summary: Read and write Netpbm files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/netpbmfile/issues
 Project-URL: Source Code, https://github.com/cgohlke/netpbmfile
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Provides-Extra: all
 License-File: LICENSE
 
 Read and write Netpbm files
 ===========================
 
@@ -42,15 +42,15 @@
 
 The PGX format is specified in ITU-T Rec. T.803.
 
 No gamma correction or scaling is performed.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.1.1
+:Version: 2023.6.15
 
 Quickstart
 ----------
 
 Install the netpbmfile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/netpbmfile/>`_::
 
@@ -60,23 +60,28 @@
 
 Source code and support are available on
 `GitHub <https://github.com/cgohlke/netpbmfile>`_.
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.9, 3.11.1 <https://www.python.org>`_
-- `NumPy 1.23.5 <https://pypi.org/project/numpy/>`_
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.4, 3.12.0b2
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
 
 Revisions
 ---------
 
+2023.6.15
+
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+- Improve type hints.
+
 2023.1.1
 
 - Several breaking changes:
 - Rename magicnum to magicnumber (breaking).
 - Rename tupltypes to tupltype (breaking).
 - Change magicnumber and header properties to str (breaking).
 - Replace pam parameter with magicnumber (breaking).
```

### Comparing `netpbmfile-2023.1.1/setup.py` & `netpbmfile-2023.6.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         raise ValueError(f'{pattern!r} not found')
     return match.groups()[0]
 
 
 with open('netpbmfile/netpbmfile.py') as fh:
     code = fh.read().replace('\r\n', '\n').replace('\r', '\n')
 
-version = search(r"__version__ = '(.*?)'", code)
+version = search(r"__version__ = '(.*?)'", code).replace('.x.x', '.dev')
 version += ('.' + buildnumber) if buildnumber else ''
 
 description = search(r'"""(.*)\.(?:\r\n|\r|\n)', code)
 
 readme = search(
     r'(?:\r\n|\r|\n){2}"""(.*)"""(?:\r\n|\r|\n){2}from __future__',
     code,
@@ -78,13 +78,13 @@
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: BSD License',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

### Comparing `netpbmfile-2023.1.1/tests/conftest.py` & `netpbmfile-2023.6.15/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `netpbmfile-2023.1.1/tests/data.npy` & `netpbmfile-2023.6.15/tests/data.npy`

 * *Files identical despite different names*

### Comparing `netpbmfile-2023.1.1/tests/test_netpbmfile.py` & `netpbmfile-2023.6.15/tests/test_netpbmfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 """Unittests for the netpbmfile package.
 
-:Version: 2023.1.1
+:Version: 2023.6.15
 
 """
 
 import os
 import sys
 import tempfile
 import hashlib
@@ -321,14 +321,15 @@
         (480, 640),
         65535,
         b'\xd2I&\xe6\xe1\xa0\x93\x03\x80^M\xdd\x02\xb5\xb5\x17',
     ),
 ]
 
 
+@pytest.mark.skipif(__doc__ is None, reason='__doc__ is None')
 def test_version():
     """Assert netpbmfile versions match docstrings."""
     ver = ':Version: ' + netpbmfile.__version__
     assert ver in __doc__
     assert ver in netpbmfile.__doc__
 
 
@@ -397,15 +398,15 @@
 
     byteorder = '<' if dtype[:2] == '<u' else None
     multitext = magicnumber in 'P1 P2 P3' and axes[0] == 'I'
     if multitext:
         axes = axes[1:]
         shape = shape[1:]
 
-    with NetpbmFile(filepath, byteorder=byteorder) as fh:
+    with NetpbmFile(filepath, byteorder=byteorder) as fh:  # type: ignore
         assert str(fh)
         assert fh.magicnumber == magicnumber
         # assert fh.tupltype == tupltype
         tupltype = fh.tupltype
         assert fh.axes == axes
         assert fh.shape == shape
         assert fh.dtype == dtype
```

