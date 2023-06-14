# Comparing `tmp/xgo-pythonlib-0.1.6.tar.gz` & `tmp/xgo-pythonlib-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgo-pythonlib-0.1.6.tar", last modified: Tue Jun 13 03:08:29 2023, max compression
+gzip compressed data, was "xgo-pythonlib-0.1.7.tar", last modified: Wed Jun 14 22:45:43 2023, max compression
```

## Comparing `xgo-pythonlib-0.1.6.tar` & `xgo-pythonlib-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 03:08:29.117126 xgo-pythonlib-0.1.6/
--rw-rw-rw-   0        0        0     1733 2023-06-13 03:08:29.116124 xgo-pythonlib-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1106 2023-06-13 03:08:02.000000 xgo-pythonlib-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 03:08:29.118123 xgo-pythonlib-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     3684 2023-06-13 03:07:54.000000 xgo-pythonlib-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 03:08:29.099122 xgo-pythonlib-0.1.6/xgo_pythonlib.egg-info/
--rw-rw-rw-   0        0        0     1733 2023-06-13 03:08:28.000000 xgo-pythonlib-0.1.6/xgo_pythonlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-06-13 03:08:28.000000 xgo-pythonlib-0.1.6/xgo_pythonlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 03:08:28.000000 xgo-pythonlib-0.1.6/xgo_pythonlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-13 03:08:28.000000 xgo-pythonlib-0.1.6/xgo_pythonlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 03:08:29.102121 xgo-pythonlib-0.1.6/xgoedu/
--rw-rw-rw-   0        0        0    37464 2023-06-12 13:15:04.000000 xgo-pythonlib-0.1.6/xgoedu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 03:08:29.105121 xgo-pythonlib-0.1.6/xgolib/
--rw-rw-rw-   0        0        0    26394 2023-06-13 03:07:35.000000 xgo-pythonlib-0.1.6/xgolib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 03:08:29.113122 xgo-pythonlib-0.1.6/xgoscreen/
--rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.1.6/xgoscreen/LCD_2inch.py
--rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.1.6/xgoscreen/__init__.py
--rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.1.6/xgoscreen/lcdconfig.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:45:43.528756 xgo-pythonlib-0.1.7/
+-rw-rw-rw-   0        0        0     2111 2023-06-14 22:45:43.527756 xgo-pythonlib-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1484 2023-06-14 22:43:47.000000 xgo-pythonlib-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 22:45:43.528756 xgo-pythonlib-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     3744 2023-06-14 22:45:34.000000 xgo-pythonlib-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:45:43.519242 xgo-pythonlib-0.1.7/xgo_pythonlib.egg-info/
+-rw-rw-rw-   0        0        0     2111 2023-06-14 22:45:43.000000 xgo-pythonlib-0.1.7/xgo_pythonlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-06-14 22:45:43.000000 xgo-pythonlib-0.1.7/xgo_pythonlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 22:45:43.000000 xgo-pythonlib-0.1.7/xgo_pythonlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-14 22:45:43.000000 xgo-pythonlib-0.1.7/xgo_pythonlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 22:45:43.521242 xgo-pythonlib-0.1.7/xgoedu/
+-rw-rw-rw-   0        0        0    37464 2023-06-14 02:34:21.000000 xgo-pythonlib-0.1.7/xgoedu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:45:43.522242 xgo-pythonlib-0.1.7/xgolib/
+-rw-rw-rw-   0        0        0    26394 2023-06-13 03:07:35.000000 xgo-pythonlib-0.1.7/xgolib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:45:43.526756 xgo-pythonlib-0.1.7/xgoscreen/
+-rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.1.7/xgoscreen/LCD_2inch.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.1.7/xgoscreen/__init__.py
+-rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.1.7/xgoscreen/lcdconfig.py
```

### Comparing `xgo-pythonlib-0.1.6/PKG-INFO` & `xgo-pythonlib-0.1.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.1.6
+Version: 0.1.7
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -14,17 +14,17 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 
 # XGO-PythonLib
 
-XGO2 robot can be developed using the Python language.The motion,pose,coordinates,gripper and servo of the XGO2 can be controlled via Python. The detailed instructions for use of the library are as follows.
+XGO2 has built-in motion libraries for controlling the movement and various features of the machine dog, including battery level, firmware version, and servo angle. The motion library enables users to control translation and pose movement, as well as single servo and single-leg movement. The education library facilitates camera, screen, key, microphone, and speaker operations, as well as commonly used AI functions such as gesture recognition, face detection, emotional recognition, and age and gender recognition.  The detailed instructions for use of the library are as follows.
 
-PythonLib included xgolib.py xgoedu.py xgoadvance.py.
+PythonLib included xgolib.py and xgoedu.py
 
 [Luwu Dynamics · WIKI](https://www.yuque.com/luwudynamics)
 
 [PythonLib-WIKI](https://www.yuque.com/luwudynamics/cn/mxkaodwpo2h5zmvw)
 
 
 
@@ -33,38 +33,38 @@
 1 Burn the official 0609 img image 
 
 2 Copy all files from the "model" directory to `\home\pi\model`
 
 3 Run this command:
 
 ```
-pip install --upgrade xgo-pythonlib
+sudo pip install --upgrade xgo-pythonlib
 ```
 
 ## Examples
 
 Perform gesture recognition on the current camera and press the "c" key to exit.
 
 ```python
 from xgoedu import XGOEDU 
-edu = XGOEDU()
+XGO_edu = XGOEDU()
 
 while True:
-    result=edu.gestureRecognition()  
+    result=XGO_edu.gestureRecognition()  
     print(result)
-    if edu.xgoButton("c"):  
+    if XGO_edu.xgoButton("c"):  
         break
 ```
 xgolib library example
 ```python
 from xgolib import XGO
-dog = XGO('/dev/ttyAMA0')
+dog = XGO('xgomini')
 dog.action(1)
 ```
-### Lastest Verion:0.1.6
+### Lastest Verion:0.1.7
 
 ### xgolib_version=1.3.1
 
 ### xgoedu_version=1.2.3
```

### Comparing `xgo-pythonlib-0.1.6/setup.py` & `xgo-pythonlib-0.1.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+# python setup.py sdist bdist_wheel
+# twine upload dist/*
 import io
 import os
 import sys
 from shutil import rmtree
 from setuptools import find_packages, setup, Command
 
 NAME = 'xgo-pythonlib'
 DESCRIPTION = 'PythonLib for XGO2-DOG'
 URL = 'https://github.com/Xgorobot/XGO-PythonLib'
 EMAIL = 'hello@xgorobot.com'
 AUTHOR = 'luwudynamics'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.6'
+VERSION = '0.1.7'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

### Comparing `xgo-pythonlib-0.1.6/xgo_pythonlib.egg-info/PKG-INFO` & `xgo-pythonlib-0.1.7/xgo_pythonlib.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.1.6
+Version: 0.1.7
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -14,17 +14,17 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 
 # XGO-PythonLib
 
-XGO2 robot can be developed using the Python language.The motion,pose,coordinates,gripper and servo of the XGO2 can be controlled via Python. The detailed instructions for use of the library are as follows.
+XGO2 has built-in motion libraries for controlling the movement and various features of the machine dog, including battery level, firmware version, and servo angle. The motion library enables users to control translation and pose movement, as well as single servo and single-leg movement. The education library facilitates camera, screen, key, microphone, and speaker operations, as well as commonly used AI functions such as gesture recognition, face detection, emotional recognition, and age and gender recognition.  The detailed instructions for use of the library are as follows.
 
-PythonLib included xgolib.py xgoedu.py xgoadvance.py.
+PythonLib included xgolib.py and xgoedu.py
 
 [Luwu Dynamics · WIKI](https://www.yuque.com/luwudynamics)
 
 [PythonLib-WIKI](https://www.yuque.com/luwudynamics/cn/mxkaodwpo2h5zmvw)
 
 
 
@@ -33,38 +33,38 @@
 1 Burn the official 0609 img image 
 
 2 Copy all files from the "model" directory to `\home\pi\model`
 
 3 Run this command:
 
 ```
-pip install --upgrade xgo-pythonlib
+sudo pip install --upgrade xgo-pythonlib
 ```
 
 ## Examples
 
 Perform gesture recognition on the current camera and press the "c" key to exit.
 
 ```python
 from xgoedu import XGOEDU 
-edu = XGOEDU()
+XGO_edu = XGOEDU()
 
 while True:
-    result=edu.gestureRecognition()  
+    result=XGO_edu.gestureRecognition()  
     print(result)
-    if edu.xgoButton("c"):  
+    if XGO_edu.xgoButton("c"):  
         break
 ```
 xgolib library example
 ```python
 from xgolib import XGO
-dog = XGO('/dev/ttyAMA0')
+dog = XGO('xgomini')
 dog.action(1)
 ```
-### Lastest Verion:0.1.6
+### Lastest Verion:0.1.7
 
 ### xgolib_version=1.3.1
 
 ### xgoedu_version=1.2.3
```

### Comparing `xgo-pythonlib-0.1.6/xgoedu/__init__.py` & `xgo-pythonlib-0.1.7/xgoedu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,23 +204,23 @@
     '''
     filename 文件名 字符串
     '''
     def xgoSpeaker(self,filename):
         path="/home/pi/xgoMusic/"
         os.system("mplayer"+" "+path+filename)
 
-    def xgoVedioAudio(self,filename):
+    def xgovideoAudio(self,filename):
         path="/home/pi/xgoVideos/"
         time.sleep(0.2)  #音画速度同步了 但是时间轴可能不同步 这里调试一下
         cmd="sudo mplayer "+path+filename+" -novideo"
         os.system(cmd)
 
-    def xgoVedio(self,filename):
+    def xgovideo(self,filename):
         path="/home/pi/xgoVideos/"
-        x=threading.Thread(target=self.xgoVedioAudio,args=(filename,))
+        x=threading.Thread(target=self.xgovideoAudio,args=(filename,))
         x.start()
         global counter
         video=cv2.VideoCapture(path+filename)
         fps = video.get(cv2.CAP_PROP_FPS) 
         print(fps)
         init_time=time.time()
         counter=0
@@ -275,15 +275,15 @@
             image = cv2.merge((r,g,b))
             image = cv2.flip(image,1)
             imgok = Image.fromarray(image)
             self.display.ShowImage(imgok)
             if not self.camera_still:
                 break
 
-    def xgoVedioRecord(self,filename="record",seconds=5):
+    def xgovideoRecord(self,filename="record",seconds=5):
         path="/home/pi/xgoVideos/"
         self.camera_still=False
         time.sleep(0.6)
         self.open_camera()
         FPS=15
         fourcc = cv2.VideoWriter_fourcc(*'mp4v')
         width = int(self.cap.get(cv2.CAP_PROP_FRAME_WIDTH))
```

### Comparing `xgo-pythonlib-0.1.6/xgolib/__init__.py` & `xgo-pythonlib-0.1.7/xgolib/__init__.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.1.6/xgoscreen/LCD_2inch.py` & `xgo-pythonlib-0.1.7/xgoscreen/LCD_2inch.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.1.6/xgoscreen/lcdconfig.py` & `xgo-pythonlib-0.1.7/xgoscreen/lcdconfig.py`

 * *Files identical despite different names*

