# Comparing `tmp/zensvi-0.6.1.tar.gz` & `tmp/zensvi-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zensvi-0.6.1.tar", max compression
+gzip compressed data, was "zensvi-0.6.2.tar", max compression
```

## Comparing `zensvi-0.6.1.tar` & `zensvi-0.6.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.6.1/LICENSE
--rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.6.1/README.md
--rwxr-xr-x   0        0        0      730 2023-06-14 07:08:03.314084 zensvi-0.6.1/pyproject.toml
--rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.6.1/src/zensvi/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.6.1/src/zensvi/cv/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.6.1/src/zensvi/cv/segmentation/__init__.py
--rwxr-xr-x   0        0        0    45667 2023-06-11 12:09:56.000000 zensvi-0.6.1/src/zensvi/cv/segmentation/segmentation.py
--rwxr-xr-x   0        0        0       63 2023-05-30 03:03:24.804064 zensvi-0.6.1/src/zensvi/download/__init__.py
--rwxr-xr-x   0        0        0    46074 2023-06-05 08:53:58.000000 zensvi-0.6.1/src/zensvi/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.6.1/src/zensvi/download/utils/UserAgent.csv
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.6.1/src/zensvi/download/utils/__init__.py
--rwxr-xr-x   0        0        0     8651 2023-06-05 08:53:58.000000 zensvi-0.6.1/src/zensvi/download/utils/geoprocess.py
--rwxr-xr-x   0        0        0     1810 2023-06-05 08:53:58.000000 zensvi-0.6.1/src/zensvi/download/utils/get_pids.py
--rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.6.1/src/zensvi/download/utils/helpers.py
--rwxr-xr-x   0        0        0     6747 2023-06-05 08:53:58.000000 zensvi-0.6.1/src/zensvi/download/utils/imtool.py
--rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.6.1/src/zensvi/download/utils/proxies.csv
--rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.6.1/src/zensvi/transform/__init__.py
--rwxr-xr-x   0        0        0    10503 2023-06-01 06:19:20.344499 zensvi-0.6.1/src/zensvi/transform/transform_image.py
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.6.1/src/zensvi/zensvi.py
--rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 zensvi-0.6.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.6.2/LICENSE
+-rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.6.2/README.md
+-rwxr-xr-x   0        0        0      730 2023-06-15 02:21:29.138242 zensvi-0.6.2/pyproject.toml
+-rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.6.2/src/zensvi/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.6.2/src/zensvi/cv/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.6.2/src/zensvi/cv/segmentation/__init__.py
+-rwxr-xr-x   0        0        0    45621 2023-06-15 01:56:31.384357 zensvi-0.6.2/src/zensvi/cv/segmentation/segmentation.py
+-rwxr-xr-x   0        0        0       63 2023-05-30 03:03:24.804064 zensvi-0.6.2/src/zensvi/download/__init__.py
+-rwxr-xr-x   0        0        0    46074 2023-06-05 08:53:58.000000 zensvi-0.6.2/src/zensvi/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.6.2/src/zensvi/download/utils/UserAgent.csv
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.6.2/src/zensvi/download/utils/__init__.py
+-rwxr-xr-x   0        0        0     8651 2023-06-05 08:53:58.000000 zensvi-0.6.2/src/zensvi/download/utils/geoprocess.py
+-rwxr-xr-x   0        0        0     1810 2023-06-05 08:53:58.000000 zensvi-0.6.2/src/zensvi/download/utils/get_pids.py
+-rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.6.2/src/zensvi/download/utils/helpers.py
+-rwxr-xr-x   0        0        0     6747 2023-06-05 08:53:58.000000 zensvi-0.6.2/src/zensvi/download/utils/imtool.py
+-rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.6.2/src/zensvi/download/utils/proxies.csv
+-rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.6.2/src/zensvi/transform/__init__.py
+-rwxr-xr-x   0        0        0    10503 2023-06-01 06:19:20.344499 zensvi-0.6.2/src/zensvi/transform/transform_image.py
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.6.2/src/zensvi/zensvi.py
+-rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 zensvi-0.6.2/PKG-INFO
```

### Comparing `zensvi-0.6.1/LICENSE` & `zensvi-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.1/README.md` & `zensvi-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.1/pyproject.toml` & `zensvi-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zensvi"
-version = "0.6.1"
+version = "0.6.2"
 description = "This package handles downloading, cleaning, analyzing street view imagery in a one-stop and zen manner."
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
```

### Comparing `zensvi-0.6.1/src/zensvi/cv/segmentation/segmentation.py` & `zensvi-0.6.2/src/zensvi/cv/segmentation/segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -610,15 +610,14 @@
             raise ValueError("At least one of dir_image_output and dir_segmentation_summary_output must not be None.")
         
         # save_image_options as a property of the class
         self.save_image_options = save_image_options
         
         # make directory
         dir_input = Path(dir_input)
-        dir_cache_segmentation_summary = None
         if dir_image_output is not None:
             dir_image_output = Path(dir_image_output)
             dir_image_output.mkdir(parents=True, exist_ok=True)
         if dir_segmentation_summary_output is not None:
             dir_segmentation_summary_output = Path(dir_segmentation_summary_output)
             dir_segmentation_summary_output.mkdir(parents=True, exist_ok=True)
             # Create a new directory called "pixel_ratio_checkpoints"
@@ -637,15 +636,15 @@
                         completed_image_files.update(checkpoint_dict.keys())
 
         # Get the list of all image files and filter the ones that are not completed yet
         # List of possible image file extensions
         image_extensions = [".jpg", ".jpeg", ".png", ".tif", ".tiff", ".bmp", ".dib", ".pbm", ".pgm", ".ppm", ".sr", ".ras", ".exr", ".jp2"]
 
         # Get the list of all image files in the directory that are not completed yet
-        image_file_list = [str(f) for f in Path(dir_input).iterdir() if f.suffix in image_extensions and str(f) not in completed_image_files]
+        image_file_list = [str(f) for f in Path(dir_input).iterdir() if f.suffix in image_extensions and f.stem not in completed_image_files]
 
         outer_batch_size = 1000  # Number of inner batches in one outer batch
         num_outer_batches = (len(image_file_list) + outer_batch_size * batch_size - 1) // (outer_batch_size * batch_size)
 
         for i in tqdm(range(num_outer_batches), desc=f"Processing outer batches of size {min(outer_batch_size * batch_size, len(image_file_list))}"):
             # Get the image files for the current outer batch
             outer_batch_image_file_list = image_file_list[i * outer_batch_size * batch_size : (i+1) * outer_batch_size * batch_size]
```

### Comparing `zensvi-0.6.1/src/zensvi/download/streetview_downloader.py` & `zensvi-0.6.2/src/zensvi/download/streetview_downloader.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.1/src/zensvi/download/utils/UserAgent.csv` & `zensvi-0.6.2/src/zensvi/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.1/src/zensvi/download/utils/geoprocess.py` & `zensvi-0.6.2/src/zensvi/download/utils/geoprocess.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.1/src/zensvi/download/utils/get_pids.py` & `zensvi-0.6.2/src/zensvi/download/utils/get_pids.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.1/src/zensvi/download/utils/helpers.py` & `zensvi-0.6.2/src/zensvi/download/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.1/src/zensvi/download/utils/imtool.py` & `zensvi-0.6.2/src/zensvi/download/utils/imtool.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.1/src/zensvi/download/utils/proxies.csv` & `zensvi-0.6.2/src/zensvi/download/utils/proxies.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.1/src/zensvi/transform/transform_image.py` & `zensvi-0.6.2/src/zensvi/transform/transform_image.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.1/PKG-INFO` & `zensvi-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zensvi
-Version: 0.6.1
+Version: 0.6.2
 Summary: This package handles downloading, cleaning, analyzing street view imagery in a one-stop and zen manner.
 License: MIT
 Author: koito19960406
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

