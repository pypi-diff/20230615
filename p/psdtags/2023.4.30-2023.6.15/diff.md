# Comparing `tmp/psdtags-2023.4.30.tar.gz` & `tmp/psdtags-2023.6.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psdtags-2023.4.30.tar", last modified: Sun Apr 30 05:33:29 2023, max compression
+gzip compressed data, was "psdtags-2023.6.15.tar", last modified: Thu Jun 15 16:48:56 2023, max compression
```

## Comparing `psdtags-2023.4.30.tar` & `psdtags-2023.6.15.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 05:33:29.781501 psdtags-2023.4.30/
--rw-rw-rw-   0        0        0     1559 2023-04-30 05:33:23.000000 psdtags-2023.4.30/LICENSE
--rw-rw-rw-   0        0        0      412 2023-02-08 00:12:46.000000 psdtags-2023.4.30/MANIFEST.in
--rw-rw-rw-   0        0        0     5854 2023-04-30 05:33:29.779523 psdtags-2023.4.30/PKG-INFO
--rw-rw-rw-   0        0        0     4989 2023-04-30 05:33:23.000000 psdtags-2023.4.30/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-30 05:33:29.768753 psdtags-2023.4.30/examples/
--rw-rw-rw-   0        0        0     9931 2023-02-08 20:01:33.000000 psdtags-2023.4.30/examples/layered_tiff.py
--rw-rw-rw-   0        0        0     1685 2023-02-08 17:59:20.000000 psdtags-2023.4.30/examples/product.png
--rw-rw-rw-   0        0        0     2368 2023-02-08 18:00:10.000000 psdtags-2023.4.30/examples/reflection.png
--rw-rw-rw-   0        0        0      875 2023-02-08 17:59:29.000000 psdtags-2023.4.30/examples/shadow.png
-drwxrwxrwx   0        0        0        0 2023-04-30 05:33:29.771754 psdtags-2023.4.30/psdtags/
--rw-rw-rw-   0        0        0      101 2022-01-14 16:45:21.000000 psdtags-2023.4.30/psdtags/__init__.py
--rw-rw-rw-   0        0        0      132 2022-01-14 16:45:31.000000 psdtags-2023.4.30/psdtags/__main__.py
--rw-rw-rw-   0        0        0   124090 2023-04-30 04:37:07.000000 psdtags-2023.4.30/psdtags/psdtags.py
-drwxrwxrwx   0        0        0        0 2023-04-30 05:33:29.778522 psdtags-2023.4.30/psdtags.egg-info/
--rw-rw-rw-   0        0        0     5854 2023-04-30 05:33:28.000000 psdtags-2023.4.30/psdtags.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-04-30 05:33:29.000000 psdtags-2023.4.30/psdtags.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 05:33:28.000000 psdtags-2023.4.30/psdtags.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-04-30 05:33:28.000000 psdtags-2023.4.30/psdtags.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-04-30 05:33:28.000000 psdtags-2023.4.30/psdtags.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-30 05:33:28.000000 psdtags-2023.4.30/psdtags.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 05:33:29.782522 psdtags-2023.4.30/setup.cfg
--rw-rw-rw-   0        0        0     2273 2023-04-30 04:56:40.000000 psdtags-2023.4.30/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:48:56.074364 psdtags-2023.6.15/
+-rw-rw-rw-   0        0        0     1559 2023-06-15 16:48:51.000000 psdtags-2023.6.15/LICENSE
+-rw-rw-rw-   0        0        0      412 2023-02-08 00:12:46.000000 psdtags-2023.6.15/MANIFEST.in
+-rw-rw-rw-   0        0        0     5992 2023-06-15 16:48:56.074364 psdtags-2023.6.15/PKG-INFO
+-rw-rw-rw-   0        0        0     5075 2023-06-15 16:48:51.000000 psdtags-2023.6.15/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-15 16:48:56.058674 psdtags-2023.6.15/examples/
+-rw-rw-rw-   0        0        0     9931 2023-02-08 20:01:33.000000 psdtags-2023.6.15/examples/layered_tiff.py
+-rw-rw-rw-   0        0        0     1685 2023-02-08 17:59:20.000000 psdtags-2023.6.15/examples/product.png
+-rw-rw-rw-   0        0        0     2368 2023-02-08 18:00:10.000000 psdtags-2023.6.15/examples/reflection.png
+-rw-rw-rw-   0        0        0      875 2023-02-08 17:59:29.000000 psdtags-2023.6.15/examples/shadow.png
+drwxrwxrwx   0        0        0        0 2023-06-15 16:48:56.058674 psdtags-2023.6.15/psdtags/
+-rw-rw-rw-   0        0        0      101 2022-01-14 16:45:21.000000 psdtags-2023.6.15/psdtags/__init__.py
+-rw-rw-rw-   0        0        0      132 2022-01-14 16:45:31.000000 psdtags-2023.6.15/psdtags/__main__.py
+-rw-rw-rw-   0        0        0   124577 2023-06-15 16:46:29.000000 psdtags-2023.6.15/psdtags/psdtags.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:48:56.074364 psdtags-2023.6.15/psdtags.egg-info/
+-rw-rw-rw-   0        0        0     5992 2023-06-15 16:48:54.000000 psdtags-2023.6.15/psdtags.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-06-15 16:48:55.000000 psdtags-2023.6.15/psdtags.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 16:48:54.000000 psdtags-2023.6.15/psdtags.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-15 16:48:54.000000 psdtags-2023.6.15/psdtags.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-06-15 16:48:54.000000 psdtags-2023.6.15/psdtags.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-15 16:48:54.000000 psdtags-2023.6.15/psdtags.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 16:48:56.074364 psdtags-2023.6.15/setup.cfg
+-rw-rw-rw-   0        0        0     2348 2023-06-14 20:01:13.000000 psdtags-2023.6.15/setup.py
```

### Comparing `psdtags-2023.4.30/LICENSE` & `psdtags-2023.6.15/LICENSE`

 * *Files identical despite different names*

### Comparing `psdtags-2023.4.30/PKG-INFO` & `psdtags-2023.6.15/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psdtags
-Version: 2023.4.30
+Version: 2023.6.15
 Summary: Read and write layered TIFF ImageSourceData and ImageResources tags
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/psdtags/issues
 Project-URL: Source Code, https://github.com/cgohlke/psdtags
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Provides-Extra: all
 License-File: LICENSE
 
 Read and write layered TIFF ImageSourceData and ImageResources tags
 ===================================================================
 
@@ -36,15 +37,15 @@
 `Adobe Photoshop File Formats Specification (November 2019)
 <https://www.adobe.com/devnet-apps/photoshop/fileformatashtml/>`_.
 
 Adobe Photoshop is a registered trademark of Adobe Systems Inc.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.4.30
+:Version: 2023.6.15
 :DOI: `10.5281/zenodo.7879187 <https://doi.org/10.5281/zenodo.7879187>`_
 
 Quickstart
 ----------
 
 Install the psdtags package and all dependencies from the
 `Python Package Index <https://pypi.org/project/psdtags/>`_::
@@ -62,26 +63,30 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.4, 3.12.0b2
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
 - `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.3.16
   (required for compressing/decompressing image data)
 - `Tifffile <https://pypi.org/project/tifffile/>`_ 2023.4.12
   (required for reading/writing tags from/to TIFF files)
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
   (required for plotting)
 
 Revisions
 ---------
 
+2023.6.15
+
+- Use PsdThumbnailFormat enum for PsdThumbnailBlock.format.
+
 2023.4.30
 
 - Few API changes (breaking).
 - Improve object repr.
 - Drop support for Python 3.8 and numpy < 1.21 (NEP29).
 
 2023.2.18
```

### Comparing `psdtags-2023.4.30/README.rst` & `psdtags-2023.6.15/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 `Adobe Photoshop File Formats Specification (November 2019)
 <https://www.adobe.com/devnet-apps/photoshop/fileformatashtml/>`_.
 
 Adobe Photoshop is a registered trademark of Adobe Systems Inc.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.4.30
+:Version: 2023.6.15
 :DOI: `10.5281/zenodo.7879187 <https://doi.org/10.5281/zenodo.7879187>`_
 
 Quickstart
 ----------
 
 Install the psdtags package and all dependencies from the
 `Python Package Index <https://pypi.org/project/psdtags/>`_::
@@ -39,26 +39,30 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.4, 3.12.0b2
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
 - `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.3.16
   (required for compressing/decompressing image data)
 - `Tifffile <https://pypi.org/project/tifffile/>`_ 2023.4.12
   (required for reading/writing tags from/to TIFF files)
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
   (required for plotting)
 
 Revisions
 ---------
 
+2023.6.15
+
+- Use PsdThumbnailFormat enum for PsdThumbnailBlock.format.
+
 2023.4.30
 
 - Few API changes (breaking).
 - Improve object repr.
 - Drop support for Python 3.8 and numpy < 1.21 (NEP29).
 
 2023.2.18
```

### Comparing `psdtags-2023.4.30/examples/layered_tiff.py` & `psdtags-2023.6.15/examples/layered_tiff.py`

 * *Files identical despite different names*

### Comparing `psdtags-2023.4.30/examples/product.png` & `psdtags-2023.6.15/examples/product.png`

 * *Files identical despite different names*

### Comparing `psdtags-2023.4.30/examples/reflection.png` & `psdtags-2023.6.15/examples/reflection.png`

 * *Files identical despite different names*

### Comparing `psdtags-2023.4.30/examples/shadow.png` & `psdtags-2023.6.15/examples/shadow.png`

 * *Files identical despite different names*

### Comparing `psdtags-2023.4.30/psdtags/psdtags.py` & `psdtags-2023.6.15/psdtags/psdtags.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 `Adobe Photoshop File Formats Specification (November 2019)
 <https://www.adobe.com/devnet-apps/photoshop/fileformatashtml/>`_.
 
 Adobe Photoshop is a registered trademark of Adobe Systems Inc.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.4.30
+:Version: 2023.6.15
 :DOI: `10.5281/zenodo.7879187 <https://doi.org/10.5281/zenodo.7879187>`_
 
 Quickstart
 ----------
 
 Install the psdtags package and all dependencies from the
 `Python Package Index <https://pypi.org/project/psdtags/>`_::
@@ -69,26 +69,30 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.4, 3.12.0b2
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
 - `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.3.16
   (required for compressing/decompressing image data)
 - `Tifffile <https://pypi.org/project/tifffile/>`_ 2023.4.12
   (required for reading/writing tags from/to TIFF files)
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
   (required for plotting)
 
 Revisions
 ---------
 
+2023.6.15
+
+- Use PsdThumbnailFormat enum for PsdThumbnailBlock.format.
+
 2023.4.30
 
 - Few API changes (breaking).
 - Improve object repr.
 - Drop support for Python 3.8 and numpy < 1.21 (NEP29).
 
 2023.2.18
@@ -199,15 +203,15 @@
 Refer to the `layered_tiff.py` example in the source distribution for
 creating a layered TIFF file from individual layer images.
 
 """
 
 from __future__ import annotations
 
-__version__ = '2023.4.30'
+__version__ = '2023.6.15'
 
 __all__ = [
     'PsdBlendMode',
     'PsdBoolean',
     'PsdBytesBlock',
     'PsdChannel',
     'PsdChannelId',
@@ -672,14 +676,29 @@
     def _missing_(cls, value: object) -> object:
         assert isinstance(value, int)
         obj = cls(-1)
         obj._value_ = value
         return obj
 
 
+class PsdThumbnailFormat(enum.IntEnum):
+    """PsdThumbnailBlock format types."""
+
+    UNKNOWN = -1
+    RAW_RGB = 0  # kRawRGB
+    JPEG_RGB = 1  # kJpegRGB
+
+    @classmethod
+    def _missing_(cls, value: object) -> object:
+        assert isinstance(value, int)
+        obj = cls(-1)
+        obj._value_ = value
+        return obj
+
+
 class PsdLayerFlag(enum.IntFlag):
     """Layer record flags."""
 
     TRANSPARENCY_PROTECTED = 1
     VISIBLE = 2
     OBSOLETE = 4
     PHOTOSHOP5 = 8  # 1 for Photoshop 5.0 and later, tells if bit 4 has info
@@ -1476,15 +1495,15 @@
         )
 
     def __repr__(self) -> str:
         if self.data is None:
             data = 'data=None,'
         else:
             data = (
-                'data=...,  # numpy.array('
+                'data=...,  # numpy.ndarray('
                 f"{self.data.shape}, '{self.data.dtype}')"
             )
         return indent(
             f'{self.__class__.__name__}(',
             f'channelid={enumstr(self.channelid)},',
             f'compression={enumstr(self.compression)},',
             data,
@@ -1849,15 +1868,15 @@
         return data
 
     def __repr__(self) -> str:
         if self.colortable is None:
             colortable = None
         else:
             colortable = (
-                '...,  # numpy.zeros('
+                '...,  # numpy.ndarray('
                 f'{self.colortable.shape}, {self.colortable.dtype})'
             )
         return indent(
             f'{self.__class__.__name__}(',
             f'key={enumstr(self.key)},',
             f'imagemode={enumstr(self.imagemode)},',
             f'name={self.name!r},',
@@ -2159,15 +2178,15 @@
         return indent(
             f'{self.__class__.__name__}(',
             f'iswritten={self.iswritten},',
             f'depth={self.depth},',
             f'rectangle={self.rectangle},',
             f'pixeldepth={self.pixeldepth},',
             f'compression={enumstr(self.compression)},',
-            f'data=...,  # numpy.empty({self.shape}, {self.dtype})',
+            f'data=...,  # numpy.ndarray({self.shape}, {self.dtype})',
             end='\n)',
         )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdSectionDividerSetting(PsdKeyABC):
     """Section divider setting (Photoshop 6.0)."""
@@ -2942,15 +2961,15 @@
 
 
 @dataclasses.dataclass(repr=False)
 class PsdThumbnailBlock(PsdResourceBlockABC):
     """Thumbnail resource format."""
 
     resourceid: PsdResourceId
-    format: int
+    format: PsdThumbnailFormat
     width: int
     height: int
     rawdata: bytes
     name: str = ''
 
     @classmethod
     def read(
@@ -2980,15 +2999,15 @@
         assert size == widthbytes * height * planes
         assert size_compressed == length - 28
 
         rawdata = fh.read(length - 28)
         return cls(
             resourceid=resourceid,
             name=name,
-            format=fmt,
+            format=PsdThumbnailFormat(fmt),
             width=width,
             height=height,
             rawdata=rawdata,
         )
 
     def write(self, fh: BinaryIO, psdformat: PsdFormat, /) -> int:
         """Write Thumbnail resource format to open file."""
@@ -3013,22 +3032,20 @@
 
     @property
     def is_bgr(self) -> bool:
         return self.resourceid.value == 1033
 
     @property
     def data(self) -> NDArray[Any]:
-        if self.format == 0:
-            # kRawRGB
+        if self.format == PsdThumbnailFormat.RAW_RGB:
             data = numpy.frombuffer(self.rawdata, dtype=numpy.uint8)
             data.shape = (self.height, (self.width * 24 + 31) // 32 * 4)
             data = data[:, : self.width * 3]
             data = data.reshape(self.height, self.width, 3)
-        elif self.format == 1:
-            # kJpegRGB
+        elif self.format == PsdThumbnailFormat.JPEG_RGB:
             from imagecodecs import jpeg8_decode
 
             data = jpeg8_decode(self.rawdata)
             assert data.shape == (self.height, self.width, 3)
         else:
             raise ValueError(f'unknown PsdThumbnailBlock format {format!r}')
         return data
@@ -3039,15 +3056,15 @@
         return f'{self.__class__.__name__} {self.name!r}'
 
     def __repr__(self) -> str:
         return indent(
             f'{self.__class__.__name__}(',
             f'resourceid={enumstr(self.resourceid)},',
             f'name={self.name!r},' if self.name else '',
-            f'format={self.format},',
+            f'format={enumstr(self.format)},',
             f'width={self.width},',
             f'height={self.height},',
             f'rawdata=...,  # bytes({len(self.rawdata)})',
             end='\n)',
         )
```

### Comparing `psdtags-2023.4.30/psdtags.egg-info/PKG-INFO` & `psdtags-2023.6.15/psdtags.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psdtags
-Version: 2023.4.30
+Version: 2023.6.15
 Summary: Read and write layered TIFF ImageSourceData and ImageResources tags
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/psdtags/issues
 Project-URL: Source Code, https://github.com/cgohlke/psdtags
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Provides-Extra: all
 License-File: LICENSE
 
 Read and write layered TIFF ImageSourceData and ImageResources tags
 ===================================================================
 
@@ -36,15 +37,15 @@
 `Adobe Photoshop File Formats Specification (November 2019)
 <https://www.adobe.com/devnet-apps/photoshop/fileformatashtml/>`_.
 
 Adobe Photoshop is a registered trademark of Adobe Systems Inc.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.4.30
+:Version: 2023.6.15
 :DOI: `10.5281/zenodo.7879187 <https://doi.org/10.5281/zenodo.7879187>`_
 
 Quickstart
 ----------
 
 Install the psdtags package and all dependencies from the
 `Python Package Index <https://pypi.org/project/psdtags/>`_::
@@ -62,26 +63,30 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.4, 3.12.0b2
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
 - `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.3.16
   (required for compressing/decompressing image data)
 - `Tifffile <https://pypi.org/project/tifffile/>`_ 2023.4.12
   (required for reading/writing tags from/to TIFF files)
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
   (required for plotting)
 
 Revisions
 ---------
 
+2023.6.15
+
+- Use PsdThumbnailFormat enum for PsdThumbnailBlock.format.
+
 2023.4.30
 
 - Few API changes (breaking).
 - Improve object repr.
 - Drop support for Python 3.8 and numpy < 1.21 (NEP29).
 
 2023.2.18
```

### Comparing `psdtags-2023.4.30/setup.py` & `psdtags-2023.6.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         raise ValueError(f'{pattern!r} not found')
     return match.groups()[0]
 
 
 with open('psdtags/psdtags.py') as fh:
     code = fh.read()
 
-version = search(r"__version__ = '(.*?)'", code)
+version = search(r"__version__ = '(.*?)'", code).replace('.x.x', '.dev')
 
 description = search(r'"""(.*)\.(?:\r\n|\r|\n)', code)
 
 readme = search(
     r'(?:\r\n|\r|\n){2}"""(.*)"""(?:\r\n|\r|\n){2}from __future__',
     code,
     re.MULTILINE | re.DOTALL,
@@ -73,9 +73,10 @@
         'License :: OSI Approved :: BSD License',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

