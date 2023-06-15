# Comparing `tmp/adofaipy-0.0.3.tar.gz` & `tmp/adofaipy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adofaipy-0.0.3.tar", last modified: Wed Jun 14 14:49:34 2023, max compression
+gzip compressed data, was "adofaipy-0.1.0.tar", last modified: Thu Jun 15 16:05:44 2023, max compression
```

## Comparing `adofaipy-0.0.3.tar` & `adofaipy-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 14:49:34.732747 adofaipy-0.0.3/
--rw-rw-rw-   0        0        0      257 2023-06-14 14:49:00.000000 adofaipy-0.0.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1061 2023-05-28 10:23:16.000000 adofaipy-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-05-28 10:21:05.000000 adofaipy-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2263 2023-06-14 14:49:34.732747 adofaipy-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1171 2023-06-14 14:48:56.000000 adofaipy-0.0.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-14 14:49:34.724748 adofaipy-0.0.3/adofaipy/
--rw-rw-rw-   0        0        0    19887 2023-06-14 14:48:42.000000 adofaipy-0.0.3/adofaipy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 14:49:34.730746 adofaipy-0.0.3/adofaipy.egg-info/
--rw-rw-rw-   0        0        0     2263 2023-06-14 14:49:34.000000 adofaipy-0.0.3/adofaipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-06-14 14:49:34.000000 adofaipy-0.0.3/adofaipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 14:49:34.000000 adofaipy-0.0.3/adofaipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 14:49:34.000000 adofaipy-0.0.3/adofaipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 14:49:34.732747 adofaipy-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      733 2023-06-14 14:48:46.000000 adofaipy-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:05:44.939573 adofaipy-0.1.0/
+-rw-rw-rw-   0        0        0      467 2023-06-15 16:04:14.000000 adofaipy-0.1.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1061 2023-05-28 10:23:16.000000 adofaipy-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-05-28 10:21:05.000000 adofaipy-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2521 2023-06-15 16:05:44.937027 adofaipy-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1171 2023-06-14 14:48:56.000000 adofaipy-0.1.0/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 16:05:44.917405 adofaipy-0.1.0/adofaipy/
+-rw-rw-rw-   0        0        0    21546 2023-06-15 16:01:11.000000 adofaipy-0.1.0/adofaipy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:05:44.934017 adofaipy-0.1.0/adofaipy.egg-info/
+-rw-rw-rw-   0        0        0     2521 2023-06-15 16:05:44.000000 adofaipy-0.1.0/adofaipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-06-15 16:05:44.000000 adofaipy-0.1.0/adofaipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 16:05:44.000000 adofaipy-0.1.0/adofaipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 16:05:44.000000 adofaipy-0.1.0/adofaipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 16:05:44.940573 adofaipy-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      733 2023-06-15 16:04:25.000000 adofaipy-0.1.0/setup.py
```

### Comparing `adofaipy-0.0.3/LICENSE.txt` & `adofaipy-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adofaipy-0.0.3/PKG-INFO` & `adofaipy-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: adofaipy
-Version: 0.0.3
+Version: 0.1.0
 Summary: A library that makes automating events in ADOFAI levels more convenient.
 Home-page: UNKNOWN
 Author: M1n3c4rt
 Author-email: vedicbits@gmail.com
 License: MIT
 Description: This is a library that makes automating events in ADOFAI levels more convenient.
         
@@ -27,14 +27,20 @@
         
         writeToFile(filestring : str, filename : str): writes the modified file string to the file. 
         
         
         Change Log
         ==========
         
+        0.1.0 (2023/06/15)
+        ------------------
+        - Minor update
+        - Added dynamic pivot offset, parallax offset, masking and blending fields to addDecoration() and moveDecorations()
+        - Added angleOffset to setSpeed()
+        
         0.0.3 (2023/06/14)
         ------------------
         - Minor bugfix: fixed filename __init__.py
         
         0.0.2 (2023/06/13)
         ------------------
         - Minor bugfix: 're' is no longer a dependency
```

### Comparing `adofaipy-0.0.3/README.txt` & `adofaipy-0.1.0/README.txt`

 * *Files identical despite different names*

### Comparing `adofaipy-0.0.3/adofaipy/__init__.py` & `adofaipy-0.1.0/adofaipy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,16 @@
     return filestring
 
 def writeToFile(filestring : str, filename : str):
     
     with open(filename, "w") as f:
         f.write(filestring)
 
-def setSpeed(floor : int, speedtype="Bpm", bpm=100, bpmmultiplier=1):
-    return "\n\t\t{ \"floor\": " + str(floor) + ", \"eventType\": \"SetSpeed\", \"speedType\": \"" + str(speedtype) + "\", \"beatsPerMinute\": " + str(bpm) + ", \"bpmMultiplier\": " + str(bpmmultiplier) + " }"
+def setSpeed(floor : int, speedtype="Bpm", bpm=100, bpmmultiplier=1, angleoffset=0):
+    return "\n\t\t{ \"floor\": " + str(floor) + ", \"eventType\": \"SetSpeed\", \"speedType\": \"" + str(speedtype) + "\", \"beatsPerMinute\": " + str(bpm) + ", \"bpmMultiplier\": " + str(bpmmultiplier) + ", \"angleOffset\": " + angleoffset + " }"
 
 def twirl(floor : int):
     return "\n\t\t{ \"floor\": " + str(floor) + ", \"eventType\": \"Twirl\" }"
 
 def checkpoint(floor : int, tileoffset=0):
     return "\n\t\t{ \"floor\": " + str(floor) + ", \"eventType\": \"Checkpoint\", \"tileOffset\": " + str(tileoffset) + " }"
 
@@ -109,22 +109,22 @@
 def positionTrack(floor : int, posx=0, posy=0, tile=0, relativeto="ThisTile", rotation=0, scale=100, opacity=100, justthistile=False, editoronly=False):
     
     justthistile = "Enabled" if justthistile == True else "Disabled"
     editoronly = "Enabled" if editoronly == True else "Disabled"
     
     return "\n\t\t{ \"floor\": " + str(floor) + ", \"eventType\": \"PositionTrack\", \"positionOffset\": [" + str(posx) + ", " + str(posy) + "], \"relativeTo\": [" + str(tile) + ", \"" + relativeto + "\"], \"rotation\": " + str(rotation) + ", \"scale\": " + str(scale) + ", \"opacity\": " + str(opacity) + ", \"justThisTile\": \"" + justthistile + "\", \"editorOnly\": \"" + editoronly + "\" }"
 
-def moveDecorations(floor : int, duration=0, tag="sampleTag", image=None, posx : int="null", posy : int="null", rotationoffset : int=None, scalex : int=None, scaley : int=None, color : str=None, opacity : int=None, depth : int=None, parallaxx : int=None, parallaxy : int=None, angleoffset=0, ease="Linear", eventtag=""):
+def moveDecorations(floor : int, duration=0, tag="sampleTag", image=None, posx : int="null", posy : int="null", pivotx : int="null", pivoty : int="null", rotationoffset : int=None, scalex : int=None, scaley : int=None, color : str=None, opacity : int=None, depth : int=None, parallaxx : int=None, parallaxy : int=None, parallaxoffsetx : int="null", parallaxoffsety : int="null", angleoffset=0, ease="Linear", eventtag="", maskingtype : str=None,  usemaskingdepth : bool=None, maskingfrontdepth : int=None, maskingbackdepth : int=None):
 
     imgstring = ""
-    if image!=None:
+    if image != None:
         imgstring = ", \"decorationImage\": \"" + str(image) + "\""
      
     rotstring = ""
-    if rotationoffset!=None:
+    if rotationoffset != None:
         rotstring = ", \"rotationOffset\": " + str(rotationoffset)
 
     scalexstring = ", \"scale\": [100,"
     if scalex != None:
         scalexstring = ", \"scale\": [" + str(scalex) + ","
 
     scaleystring = " 100]"
@@ -132,38 +132,55 @@
         scaleystring = " " + str(scaley) + "]"
 
     if scalex == None and scaley == None:
         scalexstring = ""
         scaleystring = ""
 
     colstring = ""
-    if color!=None:
+    if color != None:
         colstring = ", \"color\": " + str(color)
 
     opacitystring = ""
-    if opacity!=None:
+    if opacity != None:
         opacitystring = ", \"opacity\": " + str(opacity)
 
     depthstring = ""
-    if depth!=None:
-        colstring = ", \"depth\": " + str(depth)
+    if depth != None:
+        depthstring = ", \"depth\": " + str(depth)
 
     parallaxxstring = ", \"parallax\": [0,"
     if parallaxx != None:
         parallaxxstring = ", \"parallax\": [" + str(parallaxx) + ","
 
     parallaxystring = " 0]"
     if parallaxy != None:
         parallaxystring = " " + str(parallaxy) + "]"
 
     if parallaxx == None and parallaxy == None:
         parallaxxstring = ""
         parallaxystring = ""
+    
+    maskingtypestring = ""
+    if maskingtype != None:
+        maskingtypestring = ", \"maskingType\": " + str(maskingtype)
+
+    usemaskingdepthstring = ""
+    if usemaskingdepth != None:
+        usemaskingdepth = "Enabled" if usemaskingdepth == True else "Disabled"
+        usemaskingdepthstring = ", \"useMaskingDepth\": " + str(usemaskingdepth)
+
+    maskingfrontdepthstring = ""
+    if maskingfrontdepth != None:
+        maskingfrontdepthstring = ", \"maskingFrontDepth\": " + str(maskingfrontdepth)
+
+    maskingbackdepthstring = ""
+    if maskingbackdepth != None:
+        maskingbackdepthstring = ", \"maskingBackDepth\": " + str(maskingbackdepth)
 
-    return "{ \"floor\": " + str(floor) + ", \"eventType\": \"MoveDecorations\", \"duration\": " + str(duration) + ", \"tag\": \"" + tag + "\"" + imgstring + ", \"positionOffset\": [" + str(posx) + ", " + str(posy) + "]" + rotstring + scalexstring + scaleystring + colstring + opacitystring + depthstring + parallaxxstring + parallaxystring + ", \"angleOffset\": " + str(angleoffset) + ", \"ease\": \"" + ease + "\", \"eventTag\": \"" + str(eventtag) + "\" }"
+    return "{ \"floor\": " + str(floor) + ", \"eventType\": \"MoveDecorations\", \"duration\": " + str(duration) + ", \"tag\": \"" + tag + "\"" + imgstring + ", \"positionOffset\": [" + str(posx) + ", " + str(posy) + "]" + ", \"pivotOffset\": [" + str(pivotx) + ", " + str(pivoty) + "]" + rotstring + scalexstring + scaleystring + colstring + opacitystring + depthstring + parallaxxstring + parallaxystring + ", \"parallaxOffset\": [" + str(parallaxoffsetx) + ", " + str(parallaxoffsety) + "]" + ", \"angleOffset\": " + str(angleoffset) + ", \"ease\": \"" + ease + "\", \"eventTag\": \"" + str(eventtag) + "\" " + maskingtypestring + usemaskingdepthstring + maskingfrontdepthstring + maskingbackdepthstring + " }"
 
 def setText(floor : int, text="Text", tag="", angleoffset=0, eventtag=""):
     return "\n\t\t{ \"floor\": " + str(floor) + ", \"eventType\": \"SetText\", \"decText\": \"" + text + "\", \"tag\": \"" + tag + "\", \"angleOffset\": " + str(angleoffset) + ", \"eventTag\": \"" + eventtag + "\" }"
 
 
 def customBackground(floor : int, color="000000", bgimage="", imagecolor="ffffff", parallaxx=100, parallaxy=100, bgdisplaymode="FitToScreen", lockrot="Disabled", loopBG="Disabled", unscaledSize=100, angleoffset=0, eventtag=""):
     
@@ -249,13 +266,16 @@
 
 def hold(floor : int, duration = 0, distancemultiplier=100, landinganimation=False):
     
     landinganimation = "Enabled" if landinganimation == True else "Disabled"
 
     return "\n\t\t{ \"floor\": " + str(floor) + ", \"eventType\": \"Hold\", \"duration\": " + str(duration) + ", \"distanceMultiplier\": " + str(distancemultiplier) + ", \"landingAnimation\": \"" + landinganimation + "\" }"
 
-def addDecoration(floor : int, image="", posx=0, posy=0, relativeto="Tile", pivotoffsetx=0, pivotoffsety=0, rotation=0, scalex=100, scaley=100, tilex=1, tiley=1, color="ffffff", opacity=100, depth=-1, parallaxx=0, parallaxy=0, tag="", imagesmoothing=True, failhitbox=False, failhitboxtype="Box", failhitboxscalex=100, failhitboxscaley=100, failhitboxoffsetx=0, failhitboxoffsety=0, failhitboxrotation=0):
+def addDecoration(floor : int, image="", posx=0, posy=0, relativeto="Tile", pivotoffsetx=0, pivotoffsety=0, rotation=0, lockrotation=False, scalex=100, lockscale=False, scaley=100, tilex=1, tiley=1, color="ffffff", opacity=100, depth=-1, parallaxx=0, parallaxy=0, tag="", imagesmoothing=True, blendmode="None", maskingtype="None", failhitbox=False, failhitboxtype="Box", failhitboxscalex=100, failhitboxscaley=100, failhitboxoffsetx=0, failhitboxoffsety=0, failhitboxrotation=0):
     
     imagesmoothing = "Enabled" if imagesmoothing == True else "Disabled"
     failhitbox = "Enabled" if failhitbox == True else "Disabled"
+    lockrotation = "Enabled" if lockrotation == True else "Disabled"
+    lockscale = "Enabled" if lockscale == True else "Disabled"
+    usemaskingdepth = "Enabled" if usemaskingdepth == True else "Disabled"
 
-    return "\n\t\t{ \"floor\": " + str(floor) + ", \"eventType\": \"AddDecoration\", \"decorationImage\": \"" + image + "\", \"position\": [" + str(posx) + ", " + str(posy) + "], \"relativeTo\": \"" + relativeto + "\", \"pivotOffset\": [" + str(pivotoffsetx) + ", " + str(pivotoffsety) + "], \"rotation\": " + str(rotation) + ", \"scale\": [" + str(scalex) + ", " + str(scaley) + "], \"tile\": [" + str(tilex) + ", " + str(tiley) + "], \"color\": \"" + color + "\", \"opacity\": " + str(opacity) + ", \"depth\": " + str(depth) + ", \"parallax\": [" + str(parallaxx) + ", " + str(parallaxy) + "], \"tag\": \"" + tag + "\", \"imageSmoothing\": \"" + imagesmoothing + "\", \"failHitbox\": \"" + failhitbox + "\", \"failHitboxType\": \"" + failhitboxtype + "\", \"failHitboxScale\": [" + str(failhitboxscaley) + ", " + str(failhitboxscalex) + "], \"failHitboxOffset\": [" + str(failhitboxoffsetx) + ", " + str(failhitboxoffsety) + "], \"failHitboxRotation\": " + str(failhitboxrotation) + ", \"components\": \"\",  }"
+    return "\n\t\t{ \"floor\": " + str(floor) + ", \"eventType\": \"AddDecoration\", \"decorationImage\": \"" + image + "\", \"position\": [" + str(posx) + ", " + str(posy) + "], \"relativeTo\": \"" + relativeto + "\", \"pivotOffset\": [" + str(pivotoffsetx) + ", " + str(pivotoffsety) + "], \"rotation\": " + str(rotation) + ", \"lockRotation\": \"" + lockrotation + "\", \"scale\": [" + str(scalex) + ", " + str(scaley) + "]" + ", \"lockScale\": \"" + lockscale + ", \"tile\": [" + str(tilex) + ", " + str(tiley) + "], \"color\": \"" + color + "\", \"opacity\": " + str(opacity) + ", \"depth\": " + str(depth) + ", \"parallax\": [" + str(parallaxx) + ", " + str(parallaxy) + "], \"tag\": \"" + tag + "\", \"imageSmoothing\": \"" + imagesmoothing + "\", \"blendMode\": \"" + blendmode + "\", \"maskingType\": \"" + maskingtype + "\", \"failHitbox\": \"" + failhitbox + "\", \"failHitboxType\": \"" + failhitboxtype + "\", \"failHitboxScale\": [" + str(failhitboxscaley) + ", " + str(failhitboxscalex) + "], \"failHitboxOffset\": [" + str(failhitboxoffsetx) + ", " + str(failhitboxoffsety) + "], \"failHitboxRotation\": " + str(failhitboxrotation) + ", \"components\": \"\",  }"
```

### Comparing `adofaipy-0.0.3/adofaipy.egg-info/PKG-INFO` & `adofaipy-0.1.0/adofaipy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: adofaipy
-Version: 0.0.3
+Version: 0.1.0
 Summary: A library that makes automating events in ADOFAI levels more convenient.
 Home-page: UNKNOWN
 Author: M1n3c4rt
 Author-email: vedicbits@gmail.com
 License: MIT
 Description: This is a library that makes automating events in ADOFAI levels more convenient.
         
@@ -27,14 +27,20 @@
         
         writeToFile(filestring : str, filename : str): writes the modified file string to the file. 
         
         
         Change Log
         ==========
         
+        0.1.0 (2023/06/15)
+        ------------------
+        - Minor update
+        - Added dynamic pivot offset, parallax offset, masking and blending fields to addDecoration() and moveDecorations()
+        - Added angleOffset to setSpeed()
+        
         0.0.3 (2023/06/14)
         ------------------
         - Minor bugfix: fixed filename __init__.py
         
         0.0.2 (2023/06/13)
         ------------------
         - Minor bugfix: 're' is no longer a dependency
```

### Comparing `adofaipy-0.0.3/setup.py` & `adofaipy-0.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3.11'
 ]
  
 setup(
   name='adofaipy',
-  version='0.0.3',
+  version='0.1.0',
   description='A library that makes automating events in ADOFAI levels more convenient.',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='M1n3c4rt',
   author_email='vedicbits@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

