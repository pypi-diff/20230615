# Comparing `tmp/pysmart365-0.0.7.tar.gz` & `tmp/pysmart365-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmart365-0.0.7.tar", last modified: Mon Jun  5 15:19:27 2023, max compression
+gzip compressed data, was "pysmart365-0.0.8.tar", last modified: Thu Jun 15 10:38:07 2023, max compression
```

## Comparing `pysmart365-0.0.7.tar` & `pysmart365-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 15:19:27.198267 pysmart365-0.0.7/
--rw-rw-rw-   0        0        0    35803 2023-06-02 13:24:19.000000 pysmart365-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      353 2023-06-05 15:19:27.197269 pysmart365-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      583 2023-06-02 13:24:19.000000 pysmart365-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 15:19:27.191285 pysmart365-0.0.7/pysmart365/
--rw-rw-rw-   0        0        0     1028 2023-06-02 13:27:34.000000 pysmart365-0.0.7/pysmart365/MicroSoftware.py
--rw-rw-rw-   0        0        0     2218 2023-06-02 13:27:19.000000 pysmart365-0.0.7/pysmart365/__init__.py
--rw-rw-rw-   0        0        0      535 2023-06-05 15:09:19.000000 pysmart365-0.0.7/pysmart365/modules.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:19:27.196271 pysmart365-0.0.7/pysmart365.egg-info/
--rw-rw-rw-   0        0        0      353 2023-06-05 15:19:27.000000 pysmart365-0.0.7/pysmart365.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-06-05 15:19:27.000000 pysmart365-0.0.7/pysmart365.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 15:19:27.000000 pysmart365-0.0.7/pysmart365.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2023-06-05 15:19:27.000000 pysmart365-0.0.7/pysmart365.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-05 15:19:27.000000 pysmart365-0.0.7/pysmart365.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 15:19:27.198267 pysmart365-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      710 2023-06-05 15:17:36.000000 pysmart365-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 10:38:07.081788 pysmart365-0.0.8/
+-rw-rw-rw-   0        0        0    35803 2023-06-02 13:24:19.000000 pysmart365-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      353 2023-06-15 10:38:07.081788 pysmart365-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      583 2023-06-02 13:24:19.000000 pysmart365-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 10:38:07.059729 pysmart365-0.0.8/pysmart365/
+-rw-rw-rw-   0        0        0     3561 2023-06-15 10:27:55.000000 pysmart365-0.0.8/pysmart365/MicroSoftware.py
+-rw-rw-rw-   0        0        0     1822 2023-06-15 10:30:41.000000 pysmart365-0.0.8/pysmart365/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-06-15 10:28:22.000000 pysmart365-0.0.8/pysmart365/modules.py
+drwxrwxrwx   0        0        0        0 2023-06-15 10:38:07.080829 pysmart365-0.0.8/pysmart365.egg-info/
+-rw-rw-rw-   0        0        0      353 2023-06-15 10:38:06.000000 pysmart365-0.0.8/pysmart365.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-06-15 10:38:06.000000 pysmart365-0.0.8/pysmart365.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 10:38:06.000000 pysmart365-0.0.8/pysmart365.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-06-15 10:38:06.000000 pysmart365-0.0.8/pysmart365.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-15 10:38:06.000000 pysmart365-0.0.8/pysmart365.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 10:38:07.082786 pysmart365-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      734 2023-06-15 10:31:55.000000 pysmart365-0.0.8/setup.py
```

### Comparing `pysmart365-0.0.7/LICENSE` & `pysmart365-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmart365-0.0.7/README.md` & `pysmart365-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pysmart365-0.0.7/pysmart365/__init__.py` & `pysmart365-0.0.8/pysmart365/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,59 +3,51 @@
 
 import subprocess
 import platform
 from customtkinter import *
 from tkinter import messagebox
 import sys
 
-def turn_off(time):
+def turn_off(time: float) -> None:
     '''
     Shutdown pc directly without gui graphics.
     '''
     if time is None or 0:
         subprocess.run(['shutdown', '-s', '-t', '0'])
     else:
         subprocess.run(['shutdown', '-s', '-t', f'{time}'])
-def restart(time):
+def restart(time: float) -> None:
     '''
     Restart pc with or without time
     '''
     if time is None or 0:
         subprocess.run(['shutdown', '-r', '-t', '0'])
     else:
         subprocess.run(['shutdown', '-r', '-t', f'{time}'])
-def restart_with_advancedmode(time):
+def restart_with_advancedmode(time: float) -> None:
     '''
     Restart pc to advanced mode available on WIndows 10 and 11 or successive version.
     '''
     if time is None or 0:
         subprocess.run(['shutdown', '-r', '-o', '-t', '0'])
     else:
         subprocess.run(['shutdown', '-r', '-o', '-t', f'{time}'])
 def turn_off_with_gui():
     '''
     Turn Off pc with gui available on Windows 10 and 11 or successive version.
     '''
     check_windows_version = platform.win32_ver()[0]
     if check_windows_version == '7' or '8':
-        shutdowngui = CTk()
-        width = 200
-        height = 100
-        x = (shutdowngui.winfo_screenwidth() - width) // 2
-        y = (shutdowngui.winfo_screenheight() - height) // 2
-        shutdowngui.geometry(f"{width}x{height}+{x}+{y}")
-        shutdowngui.title("Turn Off pc in gui mode")
-        shutdown = CTkButton(shutdowngui, text="Turn Off", command=lambda: turn_off(time=0))
-        shutdown.place(relx=0.5, rely=0.5, anchor='center')
-        shutdowngui.mainloop()
+        pass
     else:
         subprocess.run(['slidetoshutdown'])
 def copyright_view(year, company):
     '''
     Enter the copyright text that will be displayed with the name that you can customize and the year using the attribute 'company' for the name and 'year' for the year.
     Example if i write copyright_view(year='2022 - 2023', company= 'Informatic365')
     then displays "© Copyright 2022 - 2023 Informatic365".
     '''
     get = f'© Copyright {year} {company}'
     return get
-def close():
-    sys.exit()
+class close():
+    def __init__(self) -> None:
+        sys.exit()
```

### Comparing `pysmart365-0.0.7/pysmart365/modules.py` & `pysmart365-0.0.8/pysmart365/modules.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,8 +11,13 @@
 import firebase_admin
 from firebase_admin import db, auth, credentials, firestore, app_check, App, datetime
 import sys
 import configparser
 import argparse
 import flask
 from flask import Flask, views, app, config, globals, helpers, logging, cli, ctx, sessions, debughelpers, testing, wrappers, blueprints, scaffold
-from ttkbootstrap import *
+from ttkbootstrap import *
+from flask import *
+import random
+import string
+from customtkinter import *
+import pywinauto
```

### Comparing `pysmart365-0.0.7/setup.py` & `pysmart365-0.0.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import *
 setup(
     author="Runkang",
     author_email="informatic3650@gmail.com",
     name="pysmart365",
     packages=['pysmart365'],
-    version='0.0.7',
+    version='0.0.8',
     long_description='''This module is to simplify the functions of MicroSoftware and SmartSoft.''',
     description='This module is to simplify the functions of MicroSoftware and SmartSoft.',
     install_requires=[
         'screeninfo',
         'pandas',
         'pyautogui',
         'pytube',
         'pytube3',
         'firebase_admin',
         'customtkinter',
         'requests',
         'flask',
         'ttkbootstrap',
-        'configparse'
+        'configparse',
+        'pywinauto'
         ],
     url="https://github.com/informatic365/PySmart365/"
-)
+)
```

