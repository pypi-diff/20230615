# Comparing `tmp/HandGestureRec-0.1.4.tar.gz` & `tmp/HandGestureRec-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HandGestureRec-0.1.4.tar", last modified: Wed Jun 14 13:20:48 2023, max compression
+gzip compressed data, was "HandGestureRec-0.1.5.tar", last modified: Thu Jun 15 19:48:08 2023, max compression
```

## Comparing `HandGestureRec-0.1.4.tar` & `HandGestureRec-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ahmadbodayr   (501) staff       (20)        0 2023-06-14 13:20:48.397395 HandGestureRec-0.1.4/
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1069 2023-06-13 20:47:04.000000 HandGestureRec-0.1.4/LICENSE
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2814 2023-06-14 13:20:48.397242 HandGestureRec-0.1.4/PKG-INFO
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2522 2023-06-14 13:19:40.000000 HandGestureRec-0.1.4/README.md
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)       38 2023-06-14 13:20:48.397432 HandGestureRec-0.1.4/setup.cfg
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1143 2023-06-14 13:20:46.000000 HandGestureRec-0.1.4/setup.py
-drwxr-xr-x   0 ahmadbodayr   (501) staff       (20)        0 2023-06-14 13:20:48.396310 HandGestureRec-0.1.4/src/
-drwxr-xr-x   0 ahmadbodayr   (501) staff       (20)        0 2023-06-14 13:20:48.397076 HandGestureRec-0.1.4/src/HandGestureRec.egg-info/
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2814 2023-06-14 13:20:48.000000 HandGestureRec-0.1.4/src/HandGestureRec.egg-info/PKG-INFO
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)      414 2023-06-14 13:20:48.000000 HandGestureRec-0.1.4/src/HandGestureRec.egg-info/SOURCES.txt
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)        1 2023-06-14 13:20:48.000000 HandGestureRec-0.1.4/src/HandGestureRec.egg-info/dependency_links.txt
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)       47 2023-06-14 13:20:48.000000 HandGestureRec-0.1.4/src/HandGestureRec.egg-info/entry_points.txt
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)       67 2023-06-14 13:20:48.000000 HandGestureRec-0.1.4/src/HandGestureRec.egg-info/requires.txt
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)       85 2023-06-14 13:20:48.000000 HandGestureRec-0.1.4/src/HandGestureRec.egg-info/top_level.txt
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)    11233 2023-06-13 18:28:48.000000 HandGestureRec-0.1.4/src/MLScript_2.py
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     3459 2023-06-11 20:53:14.000000 HandGestureRec-0.1.4/src/main.py
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2805 2023-05-17 13:36:20.000000 HandGestureRec-0.1.4/src/mainView.py
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1588 2023-06-12 21:52:36.000000 HandGestureRec-0.1.4/src/modelTestingView.py
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     4229 2023-05-21 00:52:06.000000 HandGestureRec-0.1.4/src/myDataSetsView.py
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1309 2023-05-20 23:46:55.000000 HandGestureRec-0.1.4/src/myGesturesView.py
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2569 2023-06-12 23:00:37.000000 HandGestureRec-0.1.4/src/myModelsView.py
+drwxr-xr-x   0 ahmadbodayr   (501) staff       (20)        0 2023-06-15 19:48:08.590620 HandGestureRec-0.1.5/
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1069 2023-06-13 20:47:04.000000 HandGestureRec-0.1.5/LICENSE
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2926 2023-06-15 19:48:08.590474 HandGestureRec-0.1.5/PKG-INFO
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2601 2023-06-15 19:26:27.000000 HandGestureRec-0.1.5/README.md
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)       38 2023-06-15 19:48:08.590656 HandGestureRec-0.1.5/setup.cfg
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1175 2023-06-15 19:46:33.000000 HandGestureRec-0.1.5/setup.py
+drwxr-xr-x   0 ahmadbodayr   (501) staff       (20)        0 2023-06-15 19:48:08.589584 HandGestureRec-0.1.5/src/
+drwxr-xr-x   0 ahmadbodayr   (501) staff       (20)        0 2023-06-15 19:48:08.590302 HandGestureRec-0.1.5/src/HandGestureRec.egg-info/
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2926 2023-06-15 19:48:08.000000 HandGestureRec-0.1.5/src/HandGestureRec.egg-info/PKG-INFO
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)      412 2023-06-15 19:48:08.000000 HandGestureRec-0.1.5/src/HandGestureRec.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)        1 2023-06-15 19:48:08.000000 HandGestureRec-0.1.5/src/HandGestureRec.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)       48 2023-06-15 19:48:08.000000 HandGestureRec-0.1.5/src/HandGestureRec.egg-info/entry_points.txt
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)       67 2023-06-15 19:48:08.000000 HandGestureRec-0.1.5/src/HandGestureRec.egg-info/requires.txt
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)       83 2023-06-15 19:48:08.000000 HandGestureRec-0.1.5/src/HandGestureRec.egg-info/top_level.txt
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)    11233 2023-06-13 18:28:48.000000 HandGestureRec-0.1.5/src/MLScript.py
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     3457 2023-06-15 19:43:15.000000 HandGestureRec-0.1.5/src/main.py
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2797 2023-06-15 19:43:15.000000 HandGestureRec-0.1.5/src/mainView.py
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1582 2023-06-15 19:43:15.000000 HandGestureRec-0.1.5/src/modelTestingView.py
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     4213 2023-06-15 19:43:15.000000 HandGestureRec-0.1.5/src/myDataSetsView.py
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1303 2023-06-15 19:43:15.000000 HandGestureRec-0.1.5/src/myGesturesView.py
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2555 2023-06-15 19:43:15.000000 HandGestureRec-0.1.5/src/myModelsView.py
```

### Comparing `HandGestureRec-0.1.4/LICENSE` & `HandGestureRec-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `HandGestureRec-0.1.4/PKG-INFO` & `HandGestureRec-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: HandGestureRec
-Version: 0.1.4
-Summary: m1 macs version
+Version: 0.1.5
+Summary: Dynamic hand gesture detection library using ML.
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HandGestureRec
 # Short Summary:
+ ## The library is open source  https://github.com/AhmadBodayr/HandGestureRec 
 This is a dynamic hand gesture detection library, the user can interact with the library using a GUI built using Tkinter.
 ## Implementation: 
 The library uses the webcam as the sensor and it gives the user access to the webcam using opencv, then the handlandmarks are collected using MediaPipe.
 ## GUI:
 The GUI is the main way for the user to interact with the toolkit. It is written in Tkinter for python wich is the default GUI library for Python. The GUI is simple and easy to use.
 ## The Backend:
 It is comprised of:
```

### Comparing `HandGestureRec-0.1.4/README.md` & `HandGestureRec-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # HandGestureRec
 # Short Summary:
+ ## The library is open source  https://github.com/AhmadBodayr/HandGestureRec 
 This is a dynamic hand gesture detection library, the user can interact with the library using a GUI built using Tkinter.
 ## Implementation: 
 The library uses the webcam as the sensor and it gives the user access to the webcam using opencv, then the handlandmarks are collected using MediaPipe.
 ## GUI:
 The GUI is the main way for the user to interact with the toolkit. It is written in Tkinter for python wich is the default GUI library for Python. The GUI is simple and easy to use.
 ## The Backend:
 It is comprised of:
```

### Comparing `HandGestureRec-0.1.4/setup.py` & `HandGestureRec-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,29 +8,29 @@
     else:
         tfversion = "tensorflow"
         
 setup(
     long_description=long_description, 
     long_description_content_type="text/markdown",
     name='HandGestureRec',
-    version='0.1.4',
-    description='m1 macs version',
+    version='0.1.5',
+    description='Dynamic hand gesture detection library using ML.',
     packages=find_packages(),
     py_modules=[
         "main",
-        "MLScript_2",
+        "MLScript",
         "mainView",
         "modelTestingView",
         "myDataSetsView",
         "myGesturesView",
         "myModelsView",
     ],
     entry_points={
         'console_scripts': [
-            'runHandGestureRec = main:run',
+            'execHandGestureRec = main:run',
         ],
     },
     install_requires=[
         "scikit-learn",
         'mediapipe',
         'opencv-python',
         tfversion,
```

### Comparing `HandGestureRec-0.1.4/src/HandGestureRec.egg-info/PKG-INFO` & `HandGestureRec-0.1.5/src/HandGestureRec.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: HandGestureRec
-Version: 0.1.4
-Summary: m1 macs version
+Version: 0.1.5
+Summary: Dynamic hand gesture detection library using ML.
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HandGestureRec
 # Short Summary:
+ ## The library is open source  https://github.com/AhmadBodayr/HandGestureRec 
 This is a dynamic hand gesture detection library, the user can interact with the library using a GUI built using Tkinter.
 ## Implementation: 
 The library uses the webcam as the sensor and it gives the user access to the webcam using opencv, then the handlandmarks are collected using MediaPipe.
 ## GUI:
 The GUI is the main way for the user to interact with the toolkit. It is written in Tkinter for python wich is the default GUI library for Python. The GUI is simple and easy to use.
 ## The Backend:
 It is comprised of:
```

### Comparing `HandGestureRec-0.1.4/src/MLScript_2.py` & `HandGestureRec-0.1.5/src/MLScript.py`

 * *Files identical despite different names*

### Comparing `HandGestureRec-0.1.4/src/main.py` & `HandGestureRec-0.1.5/src/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import os
 import sys
 import time
-import MLScript_2
+import MLScript
 import mainView
 import tkinter as tk
 from tkinter import *
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
```

### Comparing `HandGestureRec-0.1.4/src/mainView.py` & `HandGestureRec-0.1.5/src/mainView.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import tkinter as tk
 from tkinter import *
-import MLScript_2
+import MLScript
 import myGesturesView
 import myModelsView
 import myDataSetsView
 import modelTestingView
 import os
 class MainView(tk.Frame):
     definedGestures = 0
@@ -38,17 +38,17 @@
         self.myModels_button.pack(side=tk.BOTTOM, pady=10)
         self.testModels_button.pack(side=tk.BOTTOM, pady=10)
         self.myDataSets_button.pack(side=tk.BOTTOM, pady=10)
     
     def gestureTaking(self, gesture):
         if gesture == "":
             return
-        MLScript_2.define_gestures(gesture)
-        MLScript_2.create_Gestures_folder()
-        MLScript_2.data_collection_cam_loop()
+        MLScript.define_gestures(gesture)
+        MLScript.create_Gestures_folder()
+        MLScript.data_collection_cam_loop()
         self.gestureName_entry.delete(0, tk.END) 
         self.definedGestures += 1
         self.pack_forget()
         self.pack()
 
     def goToMyGesturesView(self):
         self.pack_forget()
```

### Comparing `HandGestureRec-0.1.4/src/modelTestingView.py` & `HandGestureRec-0.1.5/src/modelTestingView.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import tkinter as tk
 from tkinter import *
-import MLScript_2
+import MLScript
 import shutil
 import mainView
 import os
 class ModelTestingView(tk.Frame):
     back_button = None
     modelsBox = None
     models_label = None
@@ -16,30 +16,30 @@
         self.howTo = tk.Label(self, text=" Select a model from below and press test model", pady=10)
         self.howTo.pack()
         self.back_button = tk.Button(self, text="Back", font=("Arial",15), command=self.backToMainView)
         self.back_button.pack(side=tk.BOTTOM)
         self.modelsBox= Listbox(self, selectmode=SINGLE)
         self.createdModels_label = tk.Label(self, text="Created Models")
         self.createdModels_label.pack()
-        for entry in os.scandir(MLScript_2.DATA_PATH3):
+        for entry in os.scandir(MLScript.DATA_PATH3):
             if entry.is_dir() and entry.name != ".DS_Store":
                 self.modelsBox.insert(tk.END, entry.name)
         self.modelsBox.pack()
         self.testModel_button = tk.Button(self, text="Test Model", font=("Arial",15), command=self.testModel)
         self.testModel_button.pack(pady=20)
 
     def backToMainView(self):
         self.pack_forget()
         mainView.MainView(self.parent).pack()
     
     def testModel(self):
         selected_index = self.modelsBox.curselection() 
         if selected_index:
             selectedModel = self.modelsBox.get(selected_index)
-            MLScript_2.realtime_testing(selectedModel)
+            MLScript.realtime_testing(selectedModel)
```

### Comparing `HandGestureRec-0.1.4/src/myDataSetsView.py` & `HandGestureRec-0.1.5/src/myDataSetsView.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import tkinter as tk
 from tkinter import *
-import MLScript_2
+import MLScript
 import shutil
 import mainView
 import os
 class MyDataSetsView(tk.Frame):
     back_button = None
     
     definedGesturesBox = None
@@ -23,23 +23,23 @@
         self.howTo = tk.Label(self, text="To create a dataset choose a name for it, then choose gestures from the predefined getsures, then select create Dataset", pady=10)
         self.howTo.pack()
         self.definedGesturesBox = Listbox(self, selectmode=tk.MULTIPLE)
         self.dataSetsBox = Listbox(self)
         self.selectedGesturesBox = Listbox(self)
         self.gestures_label = tk.Label(self, text="Defined Gestures")
         self.gestures_label.pack()
-        gestures = os.listdir(MLScript_2.DATA_PATH)
-        sets = os.listdir(MLScript_2.DATA_PATH2)
-        folders = [item for item in gestures if os.path.isdir(os.path.join(MLScript_2.DATA_PATH, item))]
+        gestures = os.listdir(MLScript.DATA_PATH)
+        sets = os.listdir(MLScript.DATA_PATH2)
+        folders = [item for item in gestures if os.path.isdir(os.path.join(MLScript.DATA_PATH, item))]
         for i in folders:
             self.definedGesturesBox.insert(tk.END, i)
         self.definedGesturesBox.pack()
         self.dataSets_label = tk.Label(self, text="Defined DataSets")
         self.dataSets_label.pack()    
-        folders = [item for item in sets if os.path.isdir(os.path.join(MLScript_2.DATA_PATH2, item))]
+        folders = [item for item in sets if os.path.isdir(os.path.join(MLScript.DATA_PATH2, item))]
         for i in folders:
             self.dataSetsBox.insert(tk.END, i)
         self.dataSetsBox.pack()
         self.selectedGestures_label = tk.Label(self, text="Selected Gestures")
         self.selectedGestures_label.pack()
         self.selectedGesturesBox.pack()
         self.name_label = tk.Label(self, text="Enter Your DataSet Name: ")
@@ -68,23 +68,23 @@
             self.selectedGesturesBox.insert(tk.END, item)
 
     def emptySet(self):
         self.selectedGesturesBox.delete(0, tk.END)
 
     def createDataSet(self):
         if self.dataSetName_entry.get() != "" and self.selectedGesturesBox.size != 0:
-            dest_dir = os.path.join(MLScript_2.DATA_PATH2, self.dataSetName_entry.get())
+            dest_dir = os.path.join(MLScript.DATA_PATH2, self.dataSetName_entry.get())
             if os.path.exists(dest_dir):
                 print(f"Directory {dest_dir} already exists.")
                 return
             os.makedirs(dest_dir)
             selected_items = self.selectedGesturesBox.get(0, tk.END)
             for gesture in selected_items:
-                src_dir = os.path.join(MLScript_2.DATA_PATH, gesture)
-                dest_dir = os.path.join(MLScript_2.DATA_PATH2, self.dataSetName_entry.get(), gesture)
+                src_dir = os.path.join(MLScript.DATA_PATH, gesture)
+                dest_dir = os.path.join(MLScript.DATA_PATH2, self.dataSetName_entry.get(), gesture)
                 if os.path.isdir(src_dir):
                     shutil.copytree(src_dir, dest_dir)
                 else:
                     shutil.copy(src_dir, dest_dir)
             self.dataSetsBox.insert(tk.END, self.dataSetName_entry.get())
             self.dataSetName_entry.delete(0, tk.END)
             self.selectedGesturesBox.delete(0, tk.END)
```

### Comparing `HandGestureRec-0.1.4/src/myGesturesView.py` & `HandGestureRec-0.1.5/src/myGesturesView.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import tkinter as tk
 from tkinter import *
-import MLScript_2
+import MLScript
 import mainView
 import os
 class MyGesturesView(tk.Frame):
     back_button = None
     showAllGestures_button = None
     listbox = None
     title_label = None
@@ -18,16 +18,16 @@
         self.listbox = Listbox(self)
        
     def showAllGestures(self):
         if not self.title_label:
             self.title_label = tk.Label(self, text="Defined gestures")
             self.title_label.pack()
         self.listbox.delete(0, tk.END)
-        items = os.listdir(MLScript_2.DATA_PATH)
-        folders = [item for item in items if os.path.isdir(os.path.join(MLScript_2.DATA_PATH, item))]
+        items = os.listdir(MLScript.DATA_PATH)
+        folders = [item for item in items if os.path.isdir(os.path.join(MLScript.DATA_PATH, item))]
         for i in folders:
             self.listbox.insert(tk.END, i)
         self.listbox.pack()
 
     def backToMainView(self):
         self.pack_forget()
         mainView.MainView(self.parent).pack()
```

### Comparing `HandGestureRec-0.1.4/src/myModelsView.py` & `HandGestureRec-0.1.5/src/myModelsView.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import tkinter as tk
 from tkinter import *
-import MLScript_2
+import MLScript
 import shutil
 import mainView
 import os
 class MyModelsView(tk.Frame):
     back_button = None
     modelsBox = None
     dataSetsBox = None
@@ -18,25 +18,25 @@
         self.parent = parent
         self.howTo = tk.Label(self, text="To create a model, select a predefined dataset then press create model", pady=10)
         self.howTo.pack()
         self.back_button = tk.Button(self, text="Back", font=("Arial",15), command=self.backToMainView)
         self.back_button.pack(side=tk.BOTTOM)
         self.dataSetsBox = Listbox(self, selectmode=tk.SINGLE)
         self.modelsBox= Listbox(self)
-        sets = os.listdir(MLScript_2.DATA_PATH2)
-        models = os.listdir(MLScript_2.DATA_PATH3)
+        sets = os.listdir(MLScript.DATA_PATH2)
+        models = os.listdir(MLScript.DATA_PATH3)
         self.dataSets_label = tk.Label(self, text="Defined DataSets")
         self.dataSets_label.pack()    
-        folders = [item for item in sets if os.path.isdir(os.path.join(MLScript_2.DATA_PATH2, item))]
+        folders = [item for item in sets if os.path.isdir(os.path.join(MLScript.DATA_PATH2, item))]
         for i in folders:
             self.dataSetsBox.insert(tk.END, i)
         self.dataSetsBox.pack()
         self.createdModels_label = tk.Label(self, text="Created Models")
         self.createdModels_label.pack()
-        for entry in os.scandir(MLScript_2.DATA_PATH3):
+        for entry in os.scandir(MLScript.DATA_PATH3):
             if entry.is_dir():
                 self.modelsBox.insert(tk.END, entry.name)
         self.modelsBox.pack()
         self.createModel_button = tk.Button(self, text="create Model", font=("Arial",15), command=self.createModel)
         self.createModel_button.pack(pady=20)
         
         
@@ -49,16 +49,16 @@
     
     def createModel(self):
         selected_index = self.dataSetsBox.curselection()  # Get the index of the selected item
         if selected_index:
             self.creationInProgress_label = tk.Label(self, text="Creating your model this might take a few minutes !", font=("Arial", 25, "bold"), pady=10)
             self.creationInProgress_label.pack()
             selectedSet = self.dataSetsBox.get(selected_index)
-            MLScript_2.build_data_and_labels(selectedSet)
-            MLScript_2.build_ML_model(selectedSet)
+            MLScript.build_data_and_labels(selectedSet)
+            MLScript.build_ML_model(selectedSet)
             self.creationInProgress_label.pack_forget()
             self.modelsBox.insert(tk.END, selectedSet)
```

