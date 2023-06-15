# Comparing `tmp/wiliot-tools-4.0.4.tar.gz` & `tmp/wiliot-tools-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-tools-4.0.4.tar", last modified: Tue Apr 25 08:36:10 2023, max compression
+gzip compressed data, was "wiliot-tools-4.0.5.tar", last modified: Thu Jun 15 07:38:01 2023, max compression
```

## Comparing `wiliot-tools-4.0.4.tar` & `wiliot-tools-4.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:36:10.613059 wiliot-tools-4.0.4/
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     2575 2023-04-25 08:36:10.613059 wiliot-tools-4.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2071 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)     7205 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      330 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-25 08:36:10.613059 wiliot-tools-4.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1870 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:36:10.609059 wiliot-tools-4.0.4/wiliot_tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:36:10.609059 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/
--rw-rw-rw-   0 root         (0) root         (0)     4010 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/feature_flags.py
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/local_gateway_gui.bat
--rw-rw-rw-   0 root         (0) root         (0)    86343 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/local_gateway_gui.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:36:10.613059 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/
--rw-rw-rw-   0 root         (0) root         (0)      639 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/.gwCommands.json
--rw-rw-rw-   0 root         (0) root         (0)     4010 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/configs.gif
--rw-rw-rw-   0 root         (0) root         (0)    17562 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/custom_ep.ui
--rw-rw-rw-   0 root         (0) root         (0)    10355 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/custom_plots.ui
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/debug_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/folder.png
--rw-rw-rw-   0 root         (0) root         (0)    28161 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/gw_debugger.ui
--rw-rw-rw-   0 root         (0) root         (0)     4628 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/gw_macros.py
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:36:10.613059 wiliot-tools-4.0.4/wiliot_tools/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6046 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-25 08:36:10.000000 wiliot-tools-4.0.4/wiliot_tools/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:36:10.609059 wiliot-tools-4.0.4/wiliot_tools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     2575 2023-04-25 08:36:10.000000 wiliot-tools-4.0.4/wiliot_tools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1119 2023-04-25 08:36:10.000000 wiliot-tools-4.0.4/wiliot_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-25 08:36:10.000000 wiliot-tools-4.0.4/wiliot_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-25 08:36:10.000000 wiliot-tools-4.0.4/wiliot_tools.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-25 08:36:10.000000 wiliot-tools-4.0.4/wiliot_tools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       13 2023-04-25 08:36:10.000000 wiliot-tools-4.0.4/wiliot_tools.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 07:38:01.126471 wiliot-tools-4.0.5/
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     2934 2023-06-15 07:38:01.126471 wiliot-tools-4.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2430 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     8491 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      330 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-15 07:38:01.126471 wiliot-tools-4.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1871 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 07:38:01.122471 wiliot-tools-4.0.5/wiliot_tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/wiliot_tools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 07:38:01.122471 wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/
+-rw-rw-rw-   0 root         (0) root         (0)     4010 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/feature_flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/local_gateway_gui.bat
+-rw-rw-rw-   0 root         (0) root         (0)    88267 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/local_gateway_gui.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 07:38:01.122471 wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      639 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/utils/.gwCommands.json
+-rw-rw-rw-   0 root         (0) root         (0)     4010 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/utils/configs.gif
+-rw-rw-rw-   0 root         (0) root         (0)    17562 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/utils/custom_ep.ui
+-rw-rw-rw-   0 root         (0) root         (0)    10355 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/utils/custom_plots.ui
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/utils/debug_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/utils/folder.png
+-rw-rw-rw-   0 root         (0) root         (0)    28161 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/utils/gw_debugger.ui
+-rw-rw-rw-   0 root         (0) root         (0)     5582 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/utils/gw_macros.py
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/wiliot_tools/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 07:38:01.126471 wiliot-tools-4.0.5/wiliot_tools/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/wiliot_tools/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6186 2023-06-15 07:37:47.000000 wiliot-tools-4.0.5/wiliot_tools/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-15 07:38:00.000000 wiliot-tools-4.0.5/wiliot_tools/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 07:38:01.122471 wiliot-tools-4.0.5/wiliot_tools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     2934 2023-06-15 07:38:00.000000 wiliot-tools-4.0.5/wiliot_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2023-06-15 07:38:01.000000 wiliot-tools-4.0.5/wiliot_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-15 07:38:00.000000 wiliot-tools-4.0.5/wiliot_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-15 07:38:00.000000 wiliot-tools-4.0.5/wiliot_tools.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-15 07:38:00.000000 wiliot-tools-4.0.5/wiliot_tools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-06-15 07:38:00.000000 wiliot-tools-4.0.5/wiliot_tools.egg-info/top_level.txt
```

### Comparing `wiliot-tools-4.0.4/LICENSE` & `wiliot-tools-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.0.4/PKG-INFO` & `wiliot-tools-4.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-tools
-Version: 4.0.4
+Version: 4.0.5
 Summary: A library for interacting with Wiliot's private tools
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -55,14 +55,26 @@
 * [Local Gateway GUI](wiliot_tools/local_gateway_gui/local_gateway_gui.py)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.0.5:
+-----------------
+* Gateway GUI - Live Plots:
+  * improve visualization - add sample points, clear after changing feature
+  * add empty feature
+  * add option to save the last configuration
+* Gateway GUI - General:
+  * add sample points
+  * fix libraries compatibility
+  * improve logging from all data type and fix bugs
+  * enhance gw macros
+
 Version 4.0.4:
 -----------------
 * Gateway GUI
     * add mode for printing full UID, advertising address
     * show only Silicon Lab port as options for the gw GUI
     * add button to print the macro file to create new macros.
     * update GUI visualization
```

### Comparing `wiliot-tools-4.0.4/README.md` & `wiliot-tools-4.0.5/wiliot_tools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: wiliot-tools
+Version: 4.0.5
+Summary: A library for interacting with Wiliot's private tools
+Home-page: UNKNOWN
+Author: Wiliot
+Author-email: support@wiliot.com
+License: MIT
+Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PyWiliot: wiliot-tools #
 
 wiliot-tools is a python library for accessing Wiliot's Tools
 
 ## Public Library
 
 ### MAC Installation
@@ -38,14 +55,26 @@
 * [Local Gateway GUI](wiliot_tools/local_gateway_gui/local_gateway_gui.py)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.0.5:
+-----------------
+* Gateway GUI - Live Plots:
+  * improve visualization - add sample points, clear after changing feature
+  * add empty feature
+  * add option to save the last configuration
+* Gateway GUI - General:
+  * add sample points
+  * fix libraries compatibility
+  * improve logging from all data type and fix bugs
+  * enhance gw macros
+
 Version 4.0.4:
 -----------------
 * Gateway GUI
     * add mode for printing full UID, advertising address
     * show only Silicon Lab port as options for the gw GUI
     * add button to print the macro file to create new macros.
     * update GUI visualization
@@ -53,7 +82,9 @@
 Version 4.0.2:
 -----------------
 * First version
 
 
 The package previous content was published under the name 'wiliot' package.
 for more information please read 'wiliot' package's release notes
+
+
```

### Comparing `wiliot-tools-4.0.4/bitbucket-pipelines.yml` & `wiliot-tools-4.0.5/bitbucket-pipelines.yml`

 * *Files 15% similar despite different names*

```diff
@@ -82,14 +82,36 @@
             - python3 setup.py sdist bdist_wheel
             #update version.py with new minor version and build number (first step is done by setup as well- but we want to add build number as well):
             - echo "__version__ = '$version'" > wiliot_tools/version.py
             - echo "build_number = '$BITBUCKET_BUILD_NUMBER'" >> wiliot_tools/version.py
             - aws codeartifact login --tool twine --domain wiliot-cloud --domain-owner 142654642153 --repository pypi
             - twine upload --repository codeartifact dist/*
 
+    publish-full-version-into-new-codearfact:
+      - step:
+          name: Build and publish full version py-wilot into new codeartifact
+          image:
+            name: 096303741971.dkr.ecr.us-east-2.amazonaws.com/ci:0.0.1-alpine
+            aws:
+              access-key: $CLOUD_AWS_ACCESS_KEY_ID
+              secret-key: $CLOUD_AWS_SECRET_ACCESS_KEY
+          script:
+            - pip3 install setuptools_scm wheel twine
+            - pip3 install gitpython
+            # get updated version number:
+            - version="`python3 wiliot_tools/utils/get_version.py`"
+            # update minor version:
+            - python3 setup.py sdist bdist_wheel
+            #update version.py with new minor version and build number (first step is done by setup as well- but we want to add build number as well):
+            - echo "__version__ = '$version'" > wiliot_tools/version.py
+            - echo "build_number = '$BITBUCKET_BUILD_NUMBER'" >> wiliot_tools/version.py
+            - export AWS_ACCESS_KEY_ID=$CLOUD_AWS_ACCESS_KEY_ID AWS_SECRET_ACCESS_KEY=$CLOUD_AWS_SECRET_ACCESS_KEY
+            - aws codeartifact login --region us-east-2 --tool twine --domain wiliot-cloud --domain-owner 096303741971 --repository pypi
+            - twine upload --repository codeartifact dist/*
+
     publish-slim-version-into-pypi:
       - step:
           name: Build and publish slim version py-wilot into pypi
           <<: *wiliot-ci-image
           script:
             - pip3 install setuptools_scm
             - pip3 install gitpython
```

### Comparing `wiliot-tools-4.0.4/setup.py` & `wiliot-tools-4.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,14 @@
                  install_requires=[
                      'setuptools_scm',
                      'pyserial',
                      'pandas',
                      'pygubu==0.16',
                      'bokeh==2.4.1',
                      'MarkupSafe==2.0.1',  # for bokeh
-                     'wiliot-api==4.1.0',
-                     'wiliot-core==4.0.8'
+                     'wiliot-api>=4.1.2',
+                     'wiliot-core>=4.0.13'
                  ],
                  zip_safe=False,
                  python_requires='>=3.6',
                  include_package_data=True,
                  )
```

### Comparing `wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/__init__.py` & `wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/local_gateway_gui.py` & `wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/local_gateway_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,30 +57,31 @@
 #     (B) EVEN IF ANYONE IS ADVISED OF THE POSSIBILITY OF ANY DAMAGES, LOSSES, OR COSTS; AND
 #     (C) EVEN IF ANY REMEDY FAILS OF ITS ESSENTIAL PURPOSE.
 #  """
 import signal
 import socket
 import subprocess
 from os.path import isfile, isdir
-from tkinter import Tk, INSERT, END, filedialog, Toplevel
+from tkinter import Tk, INSERT, END, filedialog, Toplevel, Frame
 from tkinter.font import Font
 import serial.tools.list_ports
 import pygubu
 import json
 import os
 import sys
 import multiprocessing
 import logging
 import datetime
-import time
 import threading
 import pandas as pd
 import numpy as np
 import csv
 import re
+from tkinter import ttk
+import time
 
 from wiliot_core import WiliotGateway, StatType, ActionType, DataType, valid_output_power_vals, valid_bb, \
     valid_sub1g_output_power
 from wiliot_core import TagCollection, PacketList, Packet
 from wiliot_core import WiliotDir
 from wiliot_tools.local_gateway_gui.utils.gw_macros import macros
 from wiliot_tools.local_gateway_gui.utils.debug_mode import debug_flag
@@ -424,14 +425,15 @@
         for d in conv_str:
             if d['msg'] in gw_msg:
                 x = gw_msg.split(d['msg'])[1].split(',')[0]
                 try:
                     int(x)
                     self.config_param[d['param']] = x
                 except Exception as e:
+                    print(e)
                     pass
         self.ui_update('config')
 
     def start_listening(self):
         # start listening:
         self.ObjGW.start_continuous_listener()
         if self.data_handler_listener is None or not self.data_handler_listener.is_alive():
@@ -543,15 +545,15 @@
                                 continue
                             decrypted_packet = self.decrypted_multi_tag.get_last_added_packet()
                             if self.UID_mode:
                                 try:
                                     decrypted_packet_id = decrypted_packet.decoded_data['tag_id']
                                     log_text = 'TagID: ' + decrypted_packet_id
                                 except Exception as e:
-                                    print("Couldn't decrypt packet")
+                                    self.print_function("Couldn't decrypt packet {}".format(decrypted_packet))
                             else:
                                 log_text = decrypted_packet.to_oneline_log()
                             if log_text is None:
                                 continue
 
                             self.print_function(log_text)
 
@@ -598,26 +600,45 @@
                     return
 
     def on_macro_folder(self):
         macro_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'utils', 'gw_macros.py')
         self.print_function(str_in=f"> Go to {macro_path} to edit macros")
 
     def on_update_gw_version(self):
+        # The waiting window
+        loading_window = Tk()
+        loading_window.title('Loading')
+        loading_window.geometry('300x200')
+        loading_window.configure(bg='#ededed')
+        frame = Frame(loading_window, bg='#ededed')
+        frame.place(relx=0.5, rely=0.5, anchor='center')
+        message_label = ttk.Label(frame, text='Loading new version update...', font=("Helvetica", 16),
+                                  background='#ededed')
+        message_label.pack(pady=10)
+        progress = ttk.Progressbar(frame, length=200, mode='indeterminate')
+        progress.pack(pady=10)
+        progress.start()
+        loading_window.grab_set()
+        loading_window.after(30000, lambda: [progress.stop(), loading_window.destroy()])
+        # The actual process
         self.print_function(str_in="> Updating GW version, please wait...")
         version_path_entry = self.builder.get_object('version_path').get()
         if version_path_entry:
             version_path_entry = version_path_entry.strip("\u202a")  # strip left-to-right unicode if exists
             if not os.path.isfile(version_path_entry):
                 self.print_function(str_in="> cannot find the entered gw version file:")
                 return
-
         success_update = self.ObjGW.update_version(versions_path=version_path_entry)
+
         # listen again:
         self.start_listening()
         if success_update:
+            self.builder.get_object('version_path').delete(0, END)
+            self.builder.get_object('version_num_cur').delete('1.0', END)
+            self.builder.get_object('version_num_cur').insert(END, 'current:' + self.ObjGW.sw_version)
             self.print_function(str_in="> Update GW version was completed [{}]".format(self.ObjGW.sw_version))
         else:
             self.print_function(str_in="> Update GW version was failed ")
 
     def on_reset(self):
         self.ObjGW.reset_gw()
         time.sleep(1)
@@ -787,33 +808,36 @@
             f_input = self.builder.get_object('filter_id').get()
             if not f_input == 'filter ids':
                 self.get_filter_text(f_input)
             if LIVE_PLOTS_ENABLE:
                 self.reset_live_plot()
 
     def on_log(self):
+        # Setting the boolean variable's value to opposite when clicking the button
         self.log_state = not self.log_state
+        # Clicking on Start Logging for the first time, or clicking Stop log
         if self.log_state:
             check_log_path = self.get_log_file_name()
             if not check_log_path:
                 self.log_state = False
                 self.print_function(str_in='> Log path is invalid')
                 self.builder.get_object('log_button')['text'] = 'Start Log'
                 return
             try:
                 self.set_logger()
-
+                self.on_clear()
                 self.print_function(str_in='> Start Logging [{}]'.format(self.get_log_file_name()))
                 self.builder.get_object('log_button')['text'] = 'Stop Log'
                 return
             except Exception as e:
                 self.print_function(str_in='> Log path is invalid: {}'.format(e))
                 self.log_state = False
                 self.builder.get_object('log_button')['text'] = 'Start Log'
                 return
+        # Clicking Stop logging
         else:
             self.builder.get_object('log_button')['text'] = 'Start Log'
             self.print_function(str_in='> Stop Logging')
             logging.FileHandler(self.get_log_file_name()).close()
             self.on_processed_data(output_path=self.get_log_file_name())
             # reset log path and user events
             self.log_path = datetime.datetime.now().strftime("%d-%m-%Y_%H-%M-%S") + 'gw_log.{}'.format("log")
@@ -859,15 +883,18 @@
 
     def on_user_event(self, user_event_text=None):
         if user_event_text is None:
             user_event_text = self.builder.get_object('user_event_text').get()
         self.print_function(str_in="user_event_time: {}, User event: {}".format(self.ObjGW.get_curr_timestamp_in_sec(),
                                                                                 user_event_text))
         user_event_row = {'user_event_time': self.ObjGW.get_curr_timestamp_in_sec(), 'user_event_data': user_event_text}
-        self.user_events = self.user_events.append(user_event_row, ignore_index=True)
+        self.user_events = self.user_events = pd.concat([self.user_events,
+                                                         pd.DataFrame(data=[user_event_row.values()],
+                                                                      columns=user_event_row.keys())],
+                                                        axis=0, ignore_index=True)
 
     def on_plot_log(self):
         plots_location = filedialog.askdirectory(initialdir="~/Documents",
                                                  title="Choose output location")
         if plots_location != '':
             if len(self.decrypted_multi_tag) > 0:
                 try:
@@ -1057,15 +1084,19 @@
             if '.log' in log_path:
                 user_event_location = log_path.replace('.log', '_user_event.csv')
             else:
                 user_event_location = log_path.replace('.csv', '_user_event.csv')
             self.user_events.to_csv(user_event_location, index=False)
             try:
                 processed_log_path = log_path.replace('.log', '_packet_process.csv')
-                packet_list = self.extract_packet_list_from_log(log_path=log_path)
+                if self.builder.get_object('data_type').get() == 'statistics' or self.builder.get_object('data_type').get() == 'full_UID_mode':
+                    # self.multi_tag.to_csv(processed_log_path)
+                    packet_list = self.multi_tag.to_packet_list()
+                else:
+                    packet_list = self.extract_packet_list_from_log(log_path=log_path)
                 packet_list.to_csv(processed_log_path)
                 mt_processed_log_path = log_path.replace('.log', '_statistics_process.csv')
                 mt = TagCollection()
                 for packet in packet_list:
                     mt.append(packet)
                 stat_df = mt.get_statistics()
                 stat_df.to_csv(path_or_buf=mt_processed_log_path)
```

### Comparing `wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/.gwCommands.json` & `wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/utils/.gwCommands.json`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/__init__.py` & `wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/configs.gif` & `wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/utils/configs.gif`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/custom_ep.ui` & `wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/utils/custom_ep.ui`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/custom_plots.ui` & `wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/utils/custom_plots.ui`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/gw_debugger.ui` & `wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/utils/gw_debugger.ui`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/gw_macros.py` & `wiliot-tools-4.0.5/wiliot_tools/local_gateway_gui/utils/gw_macros.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,22 +56,44 @@
 #     CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE);
 #     (B) EVEN IF ANYONE IS ADVISED OF THE POSSIBILITY OF ANY DAMAGES, LOSSES, OR COSTS; AND
 #     (C) EVEN IF ANY REMEDY FAILS OF ITS ESSENTIAL PURPOSE.
 #  """
 
 # keys : macro name:
 ## duration [seconds]
-## command - gateway preset commands only
+## command:
+###   gateway commands
+###
 ##
+"""
+keys are the macro name
+each macro contains:
+    * command:
+    ** if starts with !, it is gw command o send
+    ** user_event, it will trigger user event with the specified text under 'values' key
+    ** save log, it will save the log at the specified location under 'values' key
+    * wait : time to wait in seconds after the command is done
+
+"""
 
 macros = {
     "example_macro": [
-        {"wait": 3, "command": "!version"},
-        {"wait": 1, "command": "user_event", 'values': 'Set tag in initial location'},
-        {"wait": 5, "command": "!output_power pos3dBm"},
-        {"wait": 1, "command": "user_event", 'values': 'Pick up tag'},
-        {"wait": 3, "command": "!gateway_app 37 15 5 18"},
-        {"wait": 1, "command": "!cancel"},
-        {"wait": 1, "command": "!version"},
-        {"wait": 1, "command": "save_log", 'values': r'~/Downloads/output.csv'},
+        {"command": "!version", "wait": 3},
+        {"command": "user_event", 'values': 'Set tag in initial location', "wait": 1},
+        {"command": "!output_power pos3dBm", "wait": 5},
+        {"command": "user_event", 'values': 'Pick up tag', "wait": 1},
+        {"command": "!gateway_app 37 15 5 18", "wait": 3},
+        {"command": "!cancel", "wait": 1},
+        {"command": "!version", "wait": 1},
+        {"command": "save_log", 'values': r'~/Downloads/output.csv', "wait": 1},
+    ],
+    "sub1g_calibration": [
+        {"command": "!set_sub_1_ghz_power 29", "wait": 0},
+        {"command": "!set_sub_1_ghz_energizing_frequency 915000", "wait": 0},
+        {"command": "!beacons_backoff 0", "wait": 0},
+        {"command": "user_event", 'values': 'Set new config', "wait": 0},
+        {"command": "!gateway_app 37 15 5 50", "wait": 90},  # test for 90 seconds
+        {"command": "!cancel", "wait": 1},
+        {"command": "user_event", 'values': 'Stop gw app and eneter into brownout', "wait": 300},
+        {"command": "save_log", 'values': r'~/Downloads/output.csv', "wait": 0},
     ]
 }
```

### Comparing `wiliot-tools-4.0.4/wiliot_tools/utils/get_version.py` & `wiliot-tools-4.0.5/wiliot_tools/utils/get_version.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,24 +67,24 @@
     """
 
     @param action_type: can be current - egt the current version, next_patch, next_minor, next_major
     @type action_type: str
     @return: the version number
     @rtype: str
     """
-    version_root = os.path.dirname(os.path.dirname(__file__))
-    git_root = os.path.dirname(version_root)
-    if os.path.isdir(os.path.join(git_root, ".git")):
+    version_root = os.path.dirname(os.path.abspath(os.path.dirname(__file__)))
+    git_root = os.path.abspath(os.path.dirname(version_root))
+    if os.path.isdir(os.path.abspath(os.path.join(git_root, ".git"))):
         version = scm_get_version(root=git_root,
                                   git_describe_command="git describe --long --dirty --tags --match [0-9]*.[0-9]*.[0-9]*")
-    elif os.path.isfile(os.path.join(version_root, "version.py")):
+    elif os.path.isfile(os.path.abspath(os.path.join(version_root, "version.py"))):
         from wiliot_tools.version import __version__
         version = __version__
     else:
-        print("Couldn't get version, retrying setupscm get version")
+        print(f"Couldn't get version from file: {os.path.abspath(os.path.join(version_root, 'version.py'))}, retrying setupscm get version")
         # give SCM another shot.. shouldn't get here:
         version = scm_get_version(root=git_root,
                                   git_describe_command="git describe --long --dirty --tags --match [0-9]*.[0-9]*.[0-9]*")
 
     if action_type == "current":
         return version
     else:
```

### Comparing `wiliot-tools-4.0.4/wiliot_tools.egg-info/PKG-INFO` & `wiliot-tools-4.0.5/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: wiliot-tools
-Version: 4.0.4
-Summary: A library for interacting with Wiliot's private tools
-Home-page: UNKNOWN
-Author: Wiliot
-Author-email: support@wiliot.com
-License: MIT
-Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyWiliot: wiliot-tools #
 
 wiliot-tools is a python library for accessing Wiliot's Tools
 
 ## Public Library
 
 ### MAC Installation
@@ -55,14 +38,26 @@
 * [Local Gateway GUI](wiliot_tools/local_gateway_gui/local_gateway_gui.py)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.0.5:
+-----------------
+* Gateway GUI - Live Plots:
+  * improve visualization - add sample points, clear after changing feature
+  * add empty feature
+  * add option to save the last configuration
+* Gateway GUI - General:
+  * add sample points
+  * fix libraries compatibility
+  * improve logging from all data type and fix bugs
+  * enhance gw macros
+
 Version 4.0.4:
 -----------------
 * Gateway GUI
     * add mode for printing full UID, advertising address
     * show only Silicon Lab port as options for the gw GUI
     * add button to print the macro file to create new macros.
     * update GUI visualization
@@ -70,9 +65,7 @@
 Version 4.0.2:
 -----------------
 * First version
 
 
 The package previous content was published under the name 'wiliot' package.
 for more information please read 'wiliot' package's release notes
-
-
```

### Comparing `wiliot-tools-4.0.4/wiliot_tools.egg-info/SOURCES.txt` & `wiliot-tools-4.0.5/wiliot_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

