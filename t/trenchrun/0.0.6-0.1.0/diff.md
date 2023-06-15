# Comparing `tmp/trenchrun-0.0.6.tar.gz` & `tmp/trenchrun-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trenchrun-0.0.6.tar", last modified: Thu Mar 30 18:24:19 2023, max compression
+gzip compressed data, was "trenchrun-0.1.0.tar", last modified: Thu Jun 15 21:04:52 2023, max compression
```

## Comparing `trenchrun-0.0.6.tar` & `trenchrun-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:24:19.370870 trenchrun-0.0.6/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11347 2023-03-30 18:23:56.000000 trenchrun-0.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-03-30 18:24:19.366870 trenchrun-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-30 18:23:56.000000 trenchrun-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-30 18:23:56.000000 trenchrun-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 18:24:19.370870 trenchrun-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:24:19.366870 trenchrun-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:24:19.366870 trenchrun-0.0.6/src/trenchrun/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-30 18:23:56.000000 trenchrun-0.0.6/src/trenchrun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-30 18:23:56.000000 trenchrun-0.0.6/src/trenchrun/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-03-30 18:23:56.000000 trenchrun-0.0.6/src/trenchrun/argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-03-30 18:23:56.000000 trenchrun-0.0.6/src/trenchrun/blend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-03-30 18:23:56.000000 trenchrun-0.0.6/src/trenchrun/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-30 18:23:56.000000 trenchrun-0.0.6/src/trenchrun/do.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-30 18:23:56.000000 trenchrun-0.0.6/src/trenchrun/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-30 18:23:56.000000 trenchrun-0.0.6/src/trenchrun/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:24:19.366870 trenchrun-0.0.6/src/trenchrun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-03-30 18:24:19.000000 trenchrun-0.0.6/src/trenchrun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-30 18:24:19.000000 trenchrun-0.0.6/src/trenchrun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 18:24:19.000000 trenchrun-0.0.6/src/trenchrun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-30 18:24:19.000000 trenchrun-0.0.6/src/trenchrun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 18:24:19.000000 trenchrun-0.0.6/src/trenchrun.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-30 18:24:19.000000 trenchrun-0.0.6/src/trenchrun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-30 18:24:19.000000 trenchrun-0.0.6/src/trenchrun.egg-info/top_level.txt
+drwxr-xr-x   0 hobu       (501) staff       (20)        0 2023-06-15 21:04:52.806777 trenchrun-0.1.0/
+-rwxr-xr-x   0 hobu       (501) staff       (20)    11347 2023-03-15 20:00:25.000000 trenchrun-0.1.0/LICENSE.txt
+-rw-r--r--   0 hobu       (501) staff       (20)     1058 2023-06-15 21:04:52.806647 trenchrun-0.1.0/PKG-INFO
+-rw-r--r--   0 hobu       (501) staff       (20)      337 2023-03-16 19:48:24.000000 trenchrun-0.1.0/README.md
+-rw-r--r--   0 hobu       (501) staff       (20)     1055 2023-06-15 18:12:53.000000 trenchrun-0.1.0/pyproject.toml
+-rw-r--r--   0 hobu       (501) staff       (20)       38 2023-06-15 21:04:52.806815 trenchrun-0.1.0/setup.cfg
+drwxr-xr-x   0 hobu       (501) staff       (20)        0 2023-06-15 21:04:52.802653 trenchrun-0.1.0/src/
+drwxr-xr-x   0 hobu       (501) staff       (20)        0 2023-06-15 21:04:52.805286 trenchrun-0.1.0/src/trenchrun/
+-rw-r--r--   0 hobu       (501) staff       (20)       20 2023-06-15 21:04:03.000000 trenchrun-0.1.0/src/trenchrun/__init__.py
+-rw-r--r--   0 hobu       (501) staff       (20)      126 2023-06-15 19:35:25.000000 trenchrun-0.1.0/src/trenchrun/__main__.py
+-rw-r--r--   0 hobu       (501) staff       (20)     2764 2023-06-15 19:37:32.000000 trenchrun-0.1.0/src/trenchrun/argparser.py
+-rw-r--r--   0 hobu       (501) staff       (20)     5017 2023-06-15 13:43:01.000000 trenchrun-0.1.0/src/trenchrun/blend.py
+-rw-r--r--   0 hobu       (501) staff       (20)     4664 2023-06-15 14:07:02.000000 trenchrun-0.1.0/src/trenchrun/data.py
+-rw-r--r--   0 hobu       (501) staff       (20)      402 2023-06-15 18:05:21.000000 trenchrun-0.1.0/src/trenchrun/do.py
+-rw-r--r--   0 hobu       (501) staff       (20)      330 2023-03-15 20:00:25.000000 trenchrun-0.1.0/src/trenchrun/logs.py
+-rw-r--r--   0 hobu       (501) staff       (20)      556 2023-06-15 19:35:20.000000 trenchrun-0.1.0/src/trenchrun/main.py
+-rw-r--r--   0 hobu       (501) staff       (20)     3831 2023-06-15 20:58:14.000000 trenchrun-0.1.0/src/trenchrun/rls.py
+drwxr-xr-x   0 hobu       (501) staff       (20)        0 2023-06-15 21:04:52.806488 trenchrun-0.1.0/src/trenchrun.egg-info/
+-rw-r--r--   0 hobu       (501) staff       (20)     1058 2023-06-15 21:04:52.000000 trenchrun-0.1.0/src/trenchrun.egg-info/PKG-INFO
+-rw-r--r--   0 hobu       (501) staff       (20)      505 2023-06-15 21:04:52.000000 trenchrun-0.1.0/src/trenchrun.egg-info/SOURCES.txt
+-rw-r--r--   0 hobu       (501) staff       (20)        1 2023-06-15 21:04:52.000000 trenchrun-0.1.0/src/trenchrun.egg-info/dependency_links.txt
+-rw-r--r--   0 hobu       (501) staff       (20)       83 2023-06-15 21:04:52.000000 trenchrun-0.1.0/src/trenchrun.egg-info/entry_points.txt
+-rw-r--r--   0 hobu       (501) staff       (20)        1 2023-03-15 20:19:17.000000 trenchrun-0.1.0/src/trenchrun.egg-info/not-zip-safe
+-rw-r--r--   0 hobu       (501) staff       (20)       18 2023-06-15 21:04:52.000000 trenchrun-0.1.0/src/trenchrun.egg-info/requires.txt
+-rw-r--r--   0 hobu       (501) staff       (20)       10 2023-06-15 21:04:52.000000 trenchrun-0.1.0/src/trenchrun.egg-info/top_level.txt
```

### Comparing `trenchrun-0.0.6/LICENSE.txt` & `trenchrun-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `trenchrun-0.0.6/PKG-INFO` & `trenchrun-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trenchrun
-Version: 0.0.6
+Version: 0.1.0
 Summary: Compute the Death Star trenchrun image from lidar data
 Author-email: Howard Butler <howard@hobu.co>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/hobuinc/trenchrun
 Project-URL: repository, https://github.com/hobuinc/trenchrun
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
```

### Comparing `trenchrun-0.0.6/pyproject.toml` & `trenchrun-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -33,8 +33,9 @@
 
 [build-system]
 requires = ["setuptools>=64.0"]
 build-backend = "setuptools.build_meta"
 
 [project.scripts]
 trenchrun = "trenchrun.__main__:main"
+rls = "trenchrun.__main__:rls"
```

### Comparing `trenchrun-0.0.6/src/trenchrun/argparser.py` & `trenchrun-0.1.0/src/trenchrun/argparser.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pathlib
 
 
-def get_parser(args):
+def get_trenchrun_parser(args):
 
     import argparse
 
     parser = argparse.ArgumentParser(description='Compute the Ambient Absorption imagery product for lidar')
     parser.add_argument('input',
                         help='PDAL-readable lidar content as a file or a pipeline', type=pathlib.Path)
     parser.add_argument('--output',
@@ -25,7 +25,36 @@
     parser.add_argument('--debug',
                         action='store_true',
                         help='print debug messages to stderr')
 
 
     args = parser.parse_args(args)
     return args
+
+def get_rls_parser(args):
+
+    import argparse
+
+    parser = argparse.ArgumentParser(description='Compute a line of sight mask along a route for a digital surface model and a line ')
+    parser.add_argument('input',
+                        help='GDAL-readable DSM content', type=pathlib.Path)
+    parser.add_argument('line',
+                        help='Linestring to use for RLS', type=str)
+    parser.add_argument('--line_srs',
+                        help='SRS of Linestring (assumed EPSG:4326 if not specified)', type=str)
+    parser.add_argument('--output',
+                        help='Output mask filename', type=str, default='rls-mask')
+    parser.add_argument('--output-path',
+                        help='Path to write output data', type=pathlib.Path, default=pathlib.Path.cwd())
+    parser.add_argument('--height',
+                        help='Target height to compute viewshed', type=float, default=2.0)
+    parser.add_argument('--density',
+                        help='Step density along the line to compute viewsheds', type=float, default=10.0)
+    parser.add_argument('--range',
+                        help='Range to compute maximum visibility (500m)', type=int, default=int(500))
+    parser.add_argument('--debug',
+                        action='store_true',
+                        help='print debug messages to stderr')
+
+
+    args = parser.parse_args(args)
+    return args
```

### Comparing `trenchrun-0.0.6/src/trenchrun/blend.py` & `trenchrun-0.1.0/src/trenchrun/blend.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import trenchrun
 
 import numpy as np
 import numpy.ma as ma
 from osgeo import gdal
 gdal.UseExceptions()
 
+from .data import Intensity, DSM, Daylight
 
 def readBand(filename,
              bandNumber,
              npDataType = np.float32,
              normalize = False):
 
     ds = gdal.Open(filename)
@@ -38,44 +39,52 @@
     projection = ds.GetProjection()
     output['projection'] = ds.GetProjection()
     output['metadata'] = ds.GetMetadata()
     output['transform'] = ds.GetGeoTransform()
     return output
 
 class Blend(object):
-    def __init__(self, data):
-        self.data = data
-
-    def do(self):
-        intensityFilename = str(self.data.args.intensityPath)
-        daylightFilename = str(self.data.args.aoPath)
+    def __init__(self, intensity: Intensity, dsm: DSM, daylight: Daylight):
+        self.intensity = intensity
+        self.daylight = daylight
+        self.dsm = dsm
+
+    def write(self, args):
+        intensityFilename = str(self.intensity.path)
+        daylightFilename = str(self.daylight.path)
         intensity = readBand(intensityFilename, 1, np.float32, True)
         daylight = readBand(daylightFilename, 1)
+        dsm = readBand(str(self.dsm.path), 1)
+
+        if intensity.shape != daylight.shape:
+            breakpoint()
+            x, y = intensity.shape
+            daylight = daylight[0:x, 0:y]
 
         logs.logger.info(f'Intensity shape {intensity.shape} ')
-        logs.logger.info(f'Daylight shape {intensity.shape} ')
+        logs.logger.info(f'Daylight shape {daylight.shape} ')
 
         intensity_mask = ma.getmask(intensity)
         daylight_mask = ma.getmask(daylight)
-        if self.data.args.blue:
+        if args.blue:
             cmap = mpl.cm.Blues_r
         else:
             cmap = mpl.cm.Greys_r
 
+        breakpoint()
         intensity_RGBA = cmap(intensity)
-        intensity_RGBA[...,3] = np.full(intensity.shape, self.data.args.alpha)
+        intensity_RGBA[...,3] = np.full(intensity.shape, args.alpha)
 
         cmap = mpl.cm.Greys_r
         daylight_RGB = cmap(daylight)
 
         RGBA = intensity_RGBA * 0.5 + daylight_RGB * 0.5
 
         numBands = RGBA.shape[2]
 
-
         nodata = 255
         big = (RGBA*255).astype(np.uint8)
         for i in range(numBands):
             ma.putmask(big[...,i], intensity_mask, nodata)
             ma.putmask(big[...,i], daylight_mask, nodata)
 
         tifpath = f"/vsimem/{str(uuid.uuid4())}.tif"
@@ -93,42 +102,42 @@
             band.SetNoDataValue(nodata)
 
         png = gdal.GetDriverByName("PNG")
 
         description='daylight exposure mixed with lidar intensity'
         title = 'Absorptive Daylight Exposure'
 
-        if self.data.args.full_output:
-            output = str(self.data.args.output_path / f"{self.data.args.output}-trenchrun.png")
+        if args.full_output:
+            output = str(args.output_path / f"{args.output}-trenchrun.png")
             png.CreateCopy( output, rast, 0,
                 [ f'TITLE={title}', f'COMMENT={description}' ] )
 
-        output = str(self.data.args.output_path / f"{self.data.args.output}-trenchrun.tif")
+        output = str(args.output_path / f"{args.output}-trenchrun.tif")
         logs.logger.info(f'writing trenchrun to {output}')
         ds = gtif.CreateCopy( output, rast, 0,
             [ 'COMPRESS=Deflate', 'TILED=YES','PREDICTOR=2' ] )
 
         if 'AREA_OR_POINT' in info['metadata']:
             ds.SetMetadataItem('AREA_OR_POINT', info['metadata']['AREA_OR_POINT'])
 
         ds.SetMetadataItem('TIFFTAG_SOFTWARE',f'Trenchrun {trenchrun.__version__}')
         ds.SetMetadataItem('TIFFTAG_IMAGEDESCRIPTION',f'{description}')
         ds.SetMetadataItem('TIFFTAG_DOCUMENTNAME',f'{title}')
 
-        if self.data.args.full_output:
-            ao = gdal.Open(str(self.data.args.aoPath))
-            output = str(self.data.args.output_path / f"{self.data.args.output}-occlusion.tif")
+        if args.full_output:
+            ao = gdal.Open(str(self.daylight.path))
+            output = str(args.output_path / f"{args.output}-occlusion.tif")
             logs.logger.info(f'writing ambient occlusion to {output}')
             ds = gtif.CreateCopy( output, ao, 0,
                 [ 'COMPRESS=Deflate', 'TILED=YES','PREDICTOR=2' ] )
 
-            ao = gdal.Open(str(self.data.args.dsmPath))
-            output = str(self.data.args.output_path / f"{self.data.args.output}-dsm.tif")
+            ao = gdal.Open(str(self.dsm.path))
+            output = str(args.output_path / f"{args.output}-dsm.tif")
             logs.logger.info(f'writing dsm to {output}')
             ds = gtif.CreateCopy( output, ao, 0,
                 [ 'COMPRESS=LZW', 'TILED=YES','PREDICTOR=3' ] )
 
-            ao = gdal.Open(str(self.data.args.intensityPath))
-            output = str(self.data.args.output_path / f"{self.data.args.output}-intensity.tif")
+            ao = gdal.Open(str(self.intensity.path))
+            output = str(args.output_path / f"{args.output}-intensity.tif")
             logs.logger.info(f'writing intensity to {output}')
             ds = gtif.CreateCopy( output, ao, 0,
                 [ 'COMPRESS=LZW', 'TILED=YES','PREDICTOR=2' ] )
```

### Comparing `trenchrun-0.0.6/src/trenchrun/data.py` & `trenchrun-0.1.0/src/trenchrun/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,130 +20,149 @@
     if p.returncode != 0:
         error = ret[1].decode('utf-8','replace')
         raise RuntimeError(error)
 
     response = ret[0].decode('utf-8','replace')
     return response
 
-class Data(object):
-    def __init__(self, args):
+class Product(object):
+    def __init__(self, reader):
+        self.reader = reader
+        self.path = pathlib.Path(tempfile.NamedTemporaryFile(suffix='.tif', delete=False).name)
+        self.validate()
 
-        self.args = args
-
-        if '.json' in self.args.input.suffixes:
-            self.inputType = 'pipeline'
-        else:
-            self.inputType = 'readable'
-
-        self.args.intensityPath = pathlib.Path(tempfile.NamedTemporaryFile(suffix='.tif', delete=False).name)
-        self.args.dsmPath = pathlib.Path(tempfile.NamedTemporaryFile(suffix='.tif', delete=False).name)
-        self.args.aoPath = pathlib.Path(tempfile.NamedTemporaryFile(suffix='.tif', delete=False).name)
-        self.checkValidData()
-
-    def readPipeline(self):
-        if self.inputType != 'pipeline':
-            raise RuntimeError("Data type is not pipeline!")
-        j = self.args.input.read_bytes().decode('utf-8')
-        stages = pdal.pipeline._parse_stages(j)
-        p = pdal.Pipeline(stages)
-
-        # strip off any writers we're making our own
-        stages = []
-        for stage in p.stages:
-            if stage.type.split('.')[0] != 'writers':
-                stages.append(stage)
-
-        p = pdal.Pipeline(stages)
-        return p
+    def __del__(self):
+        self.path.unlink()
 
+    def getStage(self):
+        pass
 
-    def readFile(self):
-        reader = pdal.Reader(str(self.args.input))
-        pipeline = reader.pipeline()
-        return pipeline
+    def validate(self):
+        pass
 
-    def __del__(self):
-        self.args.intensityPath.unlink()
-        self.args.dsmPath.unlink()
-        self.args.aoPath.unlink()
+    def process(self):
+        stage = self.getStage()
 
-    def checkValidData(self):
+        pipeline = self.reader.get() | stage
 
-        if self.inputType == 'pipeline':
-            reader = self.readPipeline()
+        count = 0
+        if pipeline.streamable:
+            count = pipeline.execute_streaming(chunk_size=self.reader.args.chunk_size)
         else:
-            reader = self.readFile()
+            count = pipeline.execute()
+        logs.logger.info(f'Wrote {self.name} product for {count} points')
 
-        qi = reader.quickinfo
-        for key in qi:
-            dimensions = [i.strip() for i in qi[key]['dimensions'].split(',')]
-            if 'Intensity' not in dimensions:
-                raise RuntimeError("Intensity information not available, this tool cannot run")
+class Intensity(Product):
+    def __init__(self, reader):
+        self.name = 'Intensity'
+        super().__init__(reader)
 
-    def getReader(self):
-        reader = None
-        if self.args.reader_args:
-            with open(self.args.reader_args,'r') as f:
-                j = json.loads(f.read())
-            reader = pdal.Reader(filename=str(self.args.input), *j)
-        else:
-            reader = pdal.Reader(filename=str(self.args.input))
-        return reader
 
-    def getWriters(self):
-        intensity = pdal.Writer.gdal(
-            filename=str(self.args.intensityPath),
+    def getStage(self):
+        stage = pdal.Writer.gdal(
+            filename=str(self.path),
             data_type='uint16_t',
             dimension='Intensity',
             output_type = 'idw',
-            resolution=self.args.resolution,
+            resolution=self.reader.args.resolution,
         )
-        dsm = pdal.Writer.gdal(
-            filename=str(self.args.dsmPath),
-            data_type='float',
-            dimension='Z',
-            output_type = 'idw',
-            resolution=self.args.resolution,
-        )
-        return intensity | dsm
 
-    def getPipeline(self):
-        if self.inputType == 'pipeline':
-            reader = self.readPipeline()
-        else:
-            reader = self.readFile()
+        return stage
+
+    def validate(self):
+        qi = self.reader.get().quickinfo
+        for key in qi:
+            dimensions = [i.strip() for i in qi[key]['dimensions'].split(',')]
+            if self.name not in dimensions:
+                raise RuntimeError(f"{self.name} information not available, this tool cannot run")
 
-        writers = self.getWriters()
-        stage = reader | writers
 
+class DSM(Product):
+    def __init__(self, reader):
+        self.name = 'DSM'
+        super().__init__(reader)
+
+
+    def getStage(self):
+        stage = pdal.Writer.gdal(filename=str(self.path),
+                                 data_type='float',
+                                 dimension='Z',
+                                 output_type = 'idw',
+                                 resolution=self.reader.args.resolution)
         return stage
 
-
-    def execute(self):
-        pipeline = self.getPipeline()
-        count = 0
-        if pipeline.streamable:
-            count = pipeline.execute_streaming(chunk_size=self.args.chunk_size)
-        else:
-            count = pipeline.execute()
-        logs.logger.info(f'Wrote intensity and dsm for {count} points')
+class Daylight(object):
+    def __init__(self, dsm: DSM):
+        self.name = 'Daylight'        
+        self.path = pathlib.Path(tempfile.NamedTemporaryFile(suffix='.tif', delete=False).name)
+        self.dsm = dsm
 
     def getImageCenter(self):
         # Run our pipeline
 
-        command = f'gdalinfo -json {self.args.dsmPath}'
+        command = f'gdalinfo -json {self.dsm.path}'
         response = run(command)
         j = json.loads(response)
         corner = j['wgs84Extent']['coordinates'][0][0]
         logs.logger.info(f'Fetched image center {corner}')
         return corner
-    def ambient_occlusion(self):
+
+
+    def process(self):
+
         lng, lat = self.getImageCenter()
 
         command = f"""whitebox_tools -r=TimeInDaylight  \
-        -i {self.args.dsmPath} -o {self.args.aoPath}  --az_fraction=15.0 \
+        -i {self.dsm.path} -o {self.path}  --az_fraction=15.0 \
         --max_dist=100.0 --lat={lat:.5f} --long={lng:.5f} """
         logs.logger.info(f"Processing ambient occlusion '{command}'")
         response = run(command)
         logs.logger.info(f"Processed ambient occlusion ")
 
 
+class Reader(object):
+    def __init__(self, args ):
+        self.args = args
+        self.name = 'Reader'
+
+        self.reader_args = None
+        if 'reader_args' in self.args:
+            with open(self.args.reader_args,'r') as f:
+                self.reader_args = json.loads(f.read())
+
+        if '.json' in self.args.input.suffixes:
+            self.inputType = 'pipeline'
+        else:
+            self.inputType = 'readable'
+
+    def get(self):
+        if self.inputType == 'pipeline':
+            reader = self.readPipeline()
+        else:
+            reader = readFile()
+
+        return reader
+    def readFile(self):
+        reader = pdal.Reader(str(self.args.input), *self.reader_args)
+        pipeline = reader.pipeline()
+        breakpoint()
+        return pipeline
+
+    def readPipeline(self):
+        if self.inputType != 'pipeline':
+            raise RuntimeError("Data type is not pipeline!")
+        j = self.args.input.read_bytes().decode('utf-8')
+        stages = pdal.pipeline._parse_stages(j)
+        p = pdal.Pipeline(stages)
+
+        # strip off any writers we're making our own
+        stages = []
+        for stage in p.stages:
+            if stage.type.split('.')[0] != 'writers':
+                stages.append(stage)
+
+        p = pdal.Pipeline(stages)
+        return p
+
+
+
+
```

### Comparing `trenchrun-0.0.6/src/trenchrun.egg-info/PKG-INFO` & `trenchrun-0.1.0/src/trenchrun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trenchrun
-Version: 0.0.6
+Version: 0.1.0
 Summary: Compute the Death Star trenchrun image from lidar data
 Author-email: Howard Butler <howard@hobu.co>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/hobuinc/trenchrun
 Project-URL: repository, https://github.com/hobuinc/trenchrun
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
```

