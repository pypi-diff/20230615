# Comparing `tmp/videoslides-0.0.7.tar.gz` & `tmp/videoslides-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\videoslides-0.0.7.tar", last modified: Sun Jun 11 01:24:50 2023, max compression
+gzip compressed data, was "dist\videoslides-0.0.8.tar", last modified: Thu Jun 15 03:13:33 2023, max compression
```

## Comparing `videoslides-0.0.7.tar` & `videoslides-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 01:24:50.000000 videoslides-0.0.7/
--rw-rw-rw-   0        0        0    42900 2023-06-09 22:00:49.000000 videoslides-0.0.7/esquema.drawio
--rw-rw-rw-   0        0        0     1103 2022-07-12 04:02:52.000000 videoslides-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0       46 2022-07-12 05:01:15.000000 videoslides-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1398 2023-06-11 01:24:50.000000 videoslides-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      767 2022-07-14 02:45:05.000000 videoslides-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-11 01:24:50.000000 videoslides-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2120 2023-06-11 01:23:58.000000 videoslides-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 01:24:50.000000 videoslides-0.0.7/src/
--rw-rw-rw-   0        0        0    45554 2023-06-10 22:06:28.000000 videoslides-0.0.7/src/functions.py
-drwxrwxrwx   0        0        0        0 2023-06-11 01:24:50.000000 videoslides-0.0.7/src/videoslides.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-11 01:24:49.000000 videoslides-0.0.7/src/videoslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1398 2023-06-11 01:24:49.000000 videoslides-0.0.7/src/videoslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-06-11 01:24:49.000000 videoslides-0.0.7/src/videoslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0      303 2023-06-11 01:24:49.000000 videoslides-0.0.7/src/videoslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       22 2023-06-11 01:24:49.000000 videoslides-0.0.7/src/videoslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13489 2023-06-11 01:23:49.000000 videoslides-0.0.7/src/videoslides.py
--rw-rw-rw-   0        0        0        0 2022-07-12 02:31:10.000000 videoslides-0.0.7/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 03:13:33.000000 videoslides-0.0.8/
+-rw-rw-rw-   0        0        0    42900 2023-06-09 22:00:49.000000 videoslides-0.0.8/esquema.drawio
+-rw-rw-rw-   0        0        0     1103 2022-07-12 04:02:52.000000 videoslides-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0       46 2022-07-12 05:01:15.000000 videoslides-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1398 2023-06-15 03:13:33.000000 videoslides-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2022-07-14 02:45:05.000000 videoslides-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 03:13:33.000000 videoslides-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2179 2023-06-15 03:13:15.000000 videoslides-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 03:13:33.000000 videoslides-0.0.8/src/
+-rw-rw-rw-   0        0        0    45609 2023-06-15 03:12:29.000000 videoslides-0.0.8/src/functions.py
+drwxrwxrwx   0        0        0        0 2023-06-15 03:13:33.000000 videoslides-0.0.8/src/videoslides.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-15 03:13:33.000000 videoslides-0.0.8/src/videoslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1398 2023-06-15 03:13:33.000000 videoslides-0.0.8/src/videoslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-06-15 03:13:33.000000 videoslides-0.0.8/src/videoslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      303 2023-06-15 03:13:33.000000 videoslides-0.0.8/src/videoslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       22 2023-06-15 03:13:33.000000 videoslides-0.0.8/src/videoslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13505 2023-06-11 04:53:59.000000 videoslides-0.0.8/src/videoslides.py
+-rw-rw-rw-   0        0        0        0 2022-07-12 02:31:10.000000 videoslides-0.0.8/src/__init__.py
```

### Comparing `videoslides-0.0.7/esquema.drawio` & `videoslides-0.0.8/esquema.drawio`

 * *Files identical despite different names*

### Comparing `videoslides-0.0.7/LICENSE.txt` & `videoslides-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `videoslides-0.0.7/PKG-INFO` & `videoslides-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videoslides
-Version: 0.0.7
+Version: 0.0.8
 Summary: Package made to obtain a text transcription from a video, with a flow from video to frames to structured frames to transcription in a json file 
 Home-page: https://github.com/Zes7one/VideoSlides
 Author: Franco Palma
 Author-email: franco.pm10@gmail.com 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `videoslides-0.0.7/README.md` & `videoslides-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `videoslides-0.0.7/setup.py` & `videoslides-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="videoslides",
-    version='0.0.7',
+    version='0.0.8',
     description='Package made to obtain a text transcription from a video, with a flow from video to frames to structured frames to transcription in a json file ',
     long_description=long_description,
     long_description_content_type="text/markdown",
     py_modules=["videoslides", "functions"],
     package_dir={'':'src'},
     install_requires=[
         "easyocr >= 1.4.1",
@@ -64,8 +64,12 @@
 # py setup.py bdist_wheel sdist
 # cd dist
 # dir 
 
 # Subir a Pypi
 # pip install twine
 # twine upload dist/*
-# twine upload --skip-existing dist/*
+
+
+# Subir a Pypi 2.0
+# py setup.py bdist_wheel sdist
+# twine upload --skip-existing dist/*
```

### Comparing `videoslides-0.0.7/src/functions.py` & `videoslides-0.0.8/src/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1033,30 +1033,31 @@
     return compilado
     # [print(i) for i in compilado ]
 
     [print(f"{conf[index]} --> {i}") for index, i in enumerate(text) if float(conf[index]) > 70] 
     # print(results)
     return data
 
-def upscale_img(img, model, ratio, runtime, gpu):
+def upscale_img(img, pb_path, model, ratio, runtime, gpu):
     """ funcion que mejora imagen segun modelo y escala entregada
     Args:
         img (str): ruta hacia de imagen a mejorar
         model (str): nombre del modelo a usar ('edsr', 'espcn', 'fsrcnn' o 'lapsrn')
         ratio (int): escala a aplicar a la imagen (2, 3 o 4)
         replace (boolean): indicador para reemplazo de img mejorada 
         runtime (boolean): indicador de modo de manejo de imagenes (True: imagen en numpy.array, False: entonces img es ruta de la imagen)
         gpu (boolean): indicador de uso de gpu
     """
     sr = dnn_superres.DnnSuperResImpl_create()
     if not runtime:
         image = img
         img = cv2.imread(img)
     # Read the desired model
-    path = f"./models/{model}_x{ratio}.pb"
+    # path = f"./models/{model}_x{ratio}.pb"
+    path = f"{pb_path}{model}_x{ratio}.pb"
     sr.readModel(path)
     if (gpu):
         # Set CUDA backend and target to enable GPU inference
         sr.setPreferableBackend(cv2.dnn.DNN_BACKEND_CUDA)
         sr.setPreferableTarget(cv2.dnn.DNN_TARGET_CUDA)
     # Set the desired model and scale to get correct pre- and post-processing
     sr.setModel(model.lower(), ratio)
```

### Comparing `videoslides-0.0.7/src/videoslides.egg-info/PKG-INFO` & `videoslides-0.0.8/src/videoslides.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videoslides
-Version: 0.0.7
+Version: 0.0.8
 Summary: Package made to obtain a text transcription from a video, with a flow from video to frames to structured frames to transcription in a json file 
 Home-page: https://github.com/Zes7one/VideoSlides
 Author: Franco Palma
 Author-email: franco.pm10@gmail.com 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `videoslides-0.0.7/src/videoslides.py` & `videoslides-0.0.8/src/videoslides.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,28 +188,28 @@
         if (len(self.slides) == 0):
             self.set_slides()
             msg = "No se tienen las slides, se ejecuta automaticamente el metodo set_slides() para setearla en el atributo slides"
             warnings.warn(f"Warning........... {msg}")
 
         self.transcription = fc.get_transcription(self.video_name, self.frames, self.slides, self.rgb, self.runtime, self.gpu_use, path, ocr) # los dos casos cubiertos 
 
-    def clean_frames(self): 
+    def clean_frames(self, pix_lim = 0.001, ssimv_lim = 0.999): 
         """ Itera sobre los frames comparando usando metricas de calidad de imagen para eliminar las que sean consideradas suficientemente similares
         para el caso de no estar runtime : se elimina el frame de la ruta 
         caso runtime: se crea una nueva lista con los frames correspondientes y se retorna  
         -------------------------------------------------------
         Input:
             No aplica
         Output:
             No aplica
         """
         if(self.runtime):
-            self.frames = fc.clean(self.frames, self.rgb, self.pix_lim, self.ssimv_lim)
+            self.frames = fc.clean(self.frames, self.rgb, pix_lim, ssimv_lim)
         else:
-            fc.clean(self.frames, self.rgb, self.pix_lim, self.ssimv_lim)
+            fc.clean(self.frames, self.rgb, pix_lim, ssimv_lim)
 
     def clean_transc(self):
         """  Desde una transcripcion formateada se eliminan redundancias y luego se eliminan los frames:
         runtime: se filtran sobre el array 
         no runtime: se eliminan los archivos de la ruta de los frames
         -------------------------------------------------------
         Input:
```

