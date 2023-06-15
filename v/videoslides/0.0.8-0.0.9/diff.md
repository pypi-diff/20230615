# Comparing `tmp/videoslides-0.0.8.tar.gz` & `tmp/videoslides-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\videoslides-0.0.8.tar", last modified: Thu Jun 15 03:13:33 2023, max compression
+gzip compressed data, was "dist\videoslides-0.0.9.tar", last modified: Thu Jun 15 03:30:08 2023, max compression
```

## Comparing `videoslides-0.0.8.tar` & `videoslides-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 03:13:33.000000 videoslides-0.0.8/
--rw-rw-rw-   0        0        0    42900 2023-06-09 22:00:49.000000 videoslides-0.0.8/esquema.drawio
--rw-rw-rw-   0        0        0     1103 2022-07-12 04:02:52.000000 videoslides-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0       46 2022-07-12 05:01:15.000000 videoslides-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1398 2023-06-15 03:13:33.000000 videoslides-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      767 2022-07-14 02:45:05.000000 videoslides-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 03:13:33.000000 videoslides-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2179 2023-06-15 03:13:15.000000 videoslides-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 03:13:33.000000 videoslides-0.0.8/src/
--rw-rw-rw-   0        0        0    45609 2023-06-15 03:12:29.000000 videoslides-0.0.8/src/functions.py
-drwxrwxrwx   0        0        0        0 2023-06-15 03:13:33.000000 videoslides-0.0.8/src/videoslides.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-15 03:13:33.000000 videoslides-0.0.8/src/videoslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1398 2023-06-15 03:13:33.000000 videoslides-0.0.8/src/videoslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-06-15 03:13:33.000000 videoslides-0.0.8/src/videoslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0      303 2023-06-15 03:13:33.000000 videoslides-0.0.8/src/videoslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       22 2023-06-15 03:13:33.000000 videoslides-0.0.8/src/videoslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13505 2023-06-11 04:53:59.000000 videoslides-0.0.8/src/videoslides.py
--rw-rw-rw-   0        0        0        0 2022-07-12 02:31:10.000000 videoslides-0.0.8/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 03:30:08.000000 videoslides-0.0.9/
+-rw-rw-rw-   0        0        0    42900 2023-06-09 22:00:49.000000 videoslides-0.0.9/esquema.drawio
+-rw-rw-rw-   0        0        0     1103 2022-07-12 04:02:52.000000 videoslides-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       46 2022-07-12 05:01:15.000000 videoslides-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1398 2023-06-15 03:30:08.000000 videoslides-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2022-07-14 02:45:05.000000 videoslides-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 03:30:08.000000 videoslides-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2179 2023-06-15 03:29:59.000000 videoslides-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 03:30:08.000000 videoslides-0.0.9/src/
+-rw-rw-rw-   0        0        0    45609 2023-06-15 03:12:29.000000 videoslides-0.0.9/src/functions.py
+drwxrwxrwx   0        0        0        0 2023-06-15 03:30:08.000000 videoslides-0.0.9/src/videoslides.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-15 03:30:07.000000 videoslides-0.0.9/src/videoslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1398 2023-06-15 03:30:07.000000 videoslides-0.0.9/src/videoslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-06-15 03:30:07.000000 videoslides-0.0.9/src/videoslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      303 2023-06-15 03:30:07.000000 videoslides-0.0.9/src/videoslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       22 2023-06-15 03:30:07.000000 videoslides-0.0.9/src/videoslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13523 2023-06-15 03:29:54.000000 videoslides-0.0.9/src/videoslides.py
+-rw-rw-rw-   0        0        0        0 2022-07-12 02:31:10.000000 videoslides-0.0.9/src/__init__.py
```

### Comparing `videoslides-0.0.8/esquema.drawio` & `videoslides-0.0.9/esquema.drawio`

 * *Files identical despite different names*

### Comparing `videoslides-0.0.8/LICENSE.txt` & `videoslides-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `videoslides-0.0.8/PKG-INFO` & `videoslides-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videoslides
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package made to obtain a text transcription from a video, with a flow from video to frames to structured frames to transcription in a json file 
 Home-page: https://github.com/Zes7one/VideoSlides
 Author: Franco Palma
 Author-email: franco.pm10@gmail.com 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `videoslides-0.0.8/README.md` & `videoslides-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `videoslides-0.0.8/setup.py` & `videoslides-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="videoslides",
-    version='0.0.8',
+    version='0.0.9',
     description='Package made to obtain a text transcription from a video, with a flow from video to frames to structured frames to transcription in a json file ',
     long_description=long_description,
     long_description_content_type="text/markdown",
     py_modules=["videoslides", "functions"],
     package_dir={'':'src'},
     install_requires=[
         "easyocr >= 1.4.1",
```

### Comparing `videoslides-0.0.8/src/functions.py` & `videoslides-0.0.9/src/functions.py`

 * *Files identical despite different names*

### Comparing `videoslides-0.0.8/src/videoslides.egg-info/PKG-INFO` & `videoslides-0.0.9/src/videoslides.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videoslides
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package made to obtain a text transcription from a video, with a flow from video to frames to structured frames to transcription in a json file 
 Home-page: https://github.com/Zes7one/VideoSlides
 Author: Franco Palma
 Author-email: franco.pm10@gmail.com 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `videoslides-0.0.8/src/videoslides.py` & `videoslides-0.0.9/src/videoslides.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,34 +239,34 @@
             No aplica
         """
         # tomar frames finales
         print("ENTRO")
         transcription_tesse = fc.get_transcription(self.video_name, self.frames, [], self.rgb, self.runtime, self.gpu_use, 2) # los dos casos cubiertos 
         print(transcription_tesse)
 
-    def improve_quality(self, model, ratio):
+    def improve_quality(self, path, model, ratio):
         """  Funcion mejora calidad de imagenes, ya sea la lista de frames o frames guardados localmente
         -------------------------------------------------------
         Input:
             No aplica
             model
             ratio
         Output:
             No aplica
         """
         # self.frames
         if(self.runtime):
             for index, frame in enumerate(self.frames):
-                self.frames[index] = fc.upscale_img(frame, model, ratio, self.runtime, self.gpu_use)
+                self.frames[index] = fc.upscale_img(frame, path, model, ratio, self.runtime, self.gpu_use)
         else:
             Frames = fc.ls(ruta = self.frames)
             Frames.sort()
             Frames = list(map(fc.addJ ,Frames))
             for index, frame in enumerate(Frames):
-                fc.upscale_img(self.frames+frame, model, ratio, self.runtime, self.gpu_use)
+                fc.upscale_img(self.frames+frame, path, model, ratio, self.runtime, self.gpu_use)
 
 
 
         # TODO: aplicar tesseract en los casos que se encuentre un digito o cifra en self.transcription (puede ir despues de lematization)
         # TODO: REVISAR SI EXISTE ALGUNA FORMA DE ENTREGAR MAYOR VALOR A LA ESTRUCTURACION ( ETIQUETAS ? : TITTLE, COMMENT, NAMES, NUMBER OR DATES)
```

