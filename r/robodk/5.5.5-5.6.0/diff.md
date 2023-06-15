# Comparing `tmp/robodk-5.5.5-py2.py3-none-any.whl.zip` & `tmp/robodk-5.6.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 112526 bytes, number of entries: 15
+Zip file size: 112821 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-02 02:24 pylint_robodk/__init__.py
 -rw-rw-rw-  2.0 fat     1551 b- defN 22-Feb-02 02:24 pylint_robodk/pylint_robodk.py
 -rw-rw-rw-  2.0 fat     1516 b- defN 23-Mar-09 14:20 robodk/__init__.py
 -rw-rw-rw-  2.0 fat    52619 b- defN 23-Mar-28 13:48 robodk/roboapps.py
--rw-rw-rw-  2.0 fat    45464 b- defN 23-Mar-28 13:48 robodk/robodialogs.py
+-rw-rw-rw-  2.0 fat    45672 b- defN 23-May-09 11:53 robodk/robodialogs.py
 -rw-rw-rw-  2.0 fat    12502 b- defN 23-Mar-09 14:20 robodk/robofileio.py
--rw-rw-rw-  2.0 fat   326660 b- defN 23-Mar-28 14:43 robodk/robolink.py
+-rw-rw-rw-  2.0 fat   326752 b- defN 23-May-17 15:39 robodk/robolink.py
 -rw-rw-rw-  2.0 fat    10012 b- defN 23-Apr-06 17:28 robodk/robolinkutils.py
--rw-rw-rw-  2.0 fat    68442 b- defN 23-Mar-27 23:23 robodk/robomath.py
+-rw-rw-rw-  2.0 fat    68988 b- defN 23-Jun-14 12:26 robodk/robomath.py
 -rw-rw-rw-  2.0 fat     1210 b- defN 22-Feb-02 02:29 robolink/__init__.py
--rw-rw-rw-  2.0 fat      587 b- defN 23-Apr-10 19:34 robodk-5.5.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    12710 b- defN 23-Apr-10 19:34 robodk-5.5.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-10 19:34 robodk-5.5.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       30 b- defN 23-Apr-10 19:34 robodk-5.5.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1167 b- defN 23-Apr-10 19:34 robodk-5.5.5.dist-info/RECORD
-15 files, 534580 bytes uncompressed, 110634 bytes compressed:  79.3%
+-rw-rw-rw-  2.0 fat      587 b- defN 23-Jun-15 18:36 robodk-5.6.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    12823 b- defN 23-Jun-15 18:36 robodk-5.6.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-15 18:36 robodk-5.6.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       30 b- defN 23-Jun-15 18:36 robodk-5.6.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1167 b- defN 23-Jun-15 18:36 robodk-5.6.0.dist-info/RECORD
+15 files, 535539 bytes uncompressed, 110929 bytes compressed:  79.3%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: robodk/robomath.py
 Comment: 
 
 Filename: robolink/__init__.py
 Comment: 
 
-Filename: robodk-5.5.5.dist-info/LICENSE
+Filename: robodk-5.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: robodk-5.5.5.dist-info/METADATA
+Filename: robodk-5.6.0.dist-info/METADATA
 Comment: 
 
-Filename: robodk-5.5.5.dist-info/WHEEL
+Filename: robodk-5.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: robodk-5.5.5.dist-info/top_level.txt
+Filename: robodk-5.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: robodk-5.5.5.dist-info/RECORD
+Filename: robodk-5.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## robodk/robodialogs.py

```diff
@@ -207,27 +207,33 @@
     """
     if ENABLE_QT:
         return DialogsQt.getOpenFolder(path_preference, strtitle)
     else:
         return DialogsTk.getOpenFolder(path_preference, strtitle)
 
 
-def getSaveFolder(path_preference=DEFAULT_FOLDER, strtitle='Save to Folder'):
+def getSaveFolder(path_preference=DEFAULT_FOLDER, strtitle='Save to Folder', **kwargs):
     """
     Pop up a folder dialog window to select a folder to save into.
     Returns the path of the folder as a string.
 
     :param str path_preference: The initial folder path, optional
     :param str strtitle: The dialog title, optional
 
     :return: The folder path, or None if the user cancels
     :rtype: str
 
     .. seealso:: :func:`~robodk.robodialogs.getOpenFolder`
     """
+    # For backward compatibility
+    if 'path_programs' in kwargs:
+        path_preference = kwargs['path_programs']
+    if 'popup_msg' in kwargs:
+        strtitle = kwargs['popup_msg']
+
     if ENABLE_QT:
         return DialogsQt.getSaveFolder(path_preference, strtitle)
     else:
         return DialogsTk.getSaveFolder(path_preference, strtitle)
 
 
 def ShowMessage(msg, title=None):
@@ -906,15 +912,15 @@
                     label = QtWidgets.QLabel(msg, self)
                     label.setWordWrap(True)
                     label.setSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Fixed)
 
                 # Create the widget holding the value
                 self.widget, self.funcs = value_to_qt_widget(value)
                 if self.widget is None:
-                    raise Exception(f"Invalid or unsupported input type: {value}")
+                    raise Exception(f"Invalid or unsupported input type: {str(value)}")
 
                 # Add the static buttons
                 button_box = QtWidgets.QDialogButtonBox(QtWidgets.QDialogButtonBox.StandardButton.Ok | QtWidgets.QDialogButtonBox.StandardButton.Cancel, QtCore.Qt.Horizontal, self)
                 QtCore.QObject.connect(button_box, QtCore.SIGNAL('accepted()'), self, QtCore.SLOT('accept()'))
                 QtCore.QObject.connect(button_box, QtCore.SIGNAL('rejected()'), self, QtCore.SLOT('reject()'))
 
                 # Add the 'Restore Defaults' button
```

## robodk/robolink.py

```diff
@@ -62,14 +62,15 @@
 INS_TYPE_CHANGETOOL = 4  #: Set Tool instruction type of a :class:`.ITEM_TYPE_INSTRUCTION`
 INS_TYPE_CHANGEROBOT = 5  #: Set Robot instruction type of a :class:`.ITEM_TYPE_INSTRUCTION`
 INS_TYPE_PAUSE = 6  #: Pause instruction type of a :class:`.ITEM_TYPE_INSTRUCTION`
 INS_TYPE_EVENT = 7  #: Simulation Event instruction type of a :class:`.ITEM_TYPE_INSTRUCTION`
 INS_TYPE_CODE = 8  #: Code instruction type of a :class:`.ITEM_TYPE_INSTRUCTION`
 INS_TYPE_PRINT = 9  #: Show Message instruction type of a :class:`.ITEM_TYPE_INSTRUCTION`
 INS_TYPE_ROUNDING = 10  #: Rounding instruction type of a :class:`.ITEM_TYPE_INSTRUCTION`
+INS_TYPE_IO = 11  #: Set or Wait I/O instruction type of a :class:`.ITEM_TYPE_INSTRUCTION`
 
 # Move types
 MOVE_TYPE_INVALID = -1  #: Invalid move type of a :class:`.ITEM_TYPE_INSTRUCTION`
 MOVE_TYPE_JOINT = 1  #: Joint move (MoveJ) type of a :class:`.ITEM_TYPE_INSTRUCTION`
 MOVE_TYPE_LINEAR = 2  #: Linear move (MoveL) type of a :class:`.ITEM_TYPE_INSTRUCTION`
 MOVE_TYPE_CIRCULAR = 3  #: Circular move (MoveC) type of a :class:`.ITEM_TYPE_INSTRUCTION`
 MOVE_TYPE_LINEARSEARCH = 5  #: Linear search move (SearchL) type of a :class:`.ITEM_TYPE_INSTRUCTION`
```

## robodk/robomath.py

```diff
@@ -1080,15 +1080,26 @@
     """Projects a point to a line"""
     vpaxe2point = subs3(point, paxe)
     dist = dot(vaxe, vpaxe2point) / dot(vaxe, vaxe)
     return add3(paxe, mult3(vaxe, dist))
 
 
 def fitPlane(points):
-    """Best fits a plane to a cloud of points"""
+    """Returns the equation and normal for a best fit plane to a cloud of points.
+    
+    Uses singular value decomposition to produce a least squares fit to a plane. Points must have centroid at [0, 0, 0]. Must provide at least 4 points.
+    
+    :param array-like points: a 3xN array of points. Each column represents one point.
+    :type array_like:
+    
+    :return: pplane: the equation of the best-fit plane, in the form b(1)*X + b(2)*Y +b(3)*Z + b(4) = 0.
+    :rtype: array_like
+    :return: vplane: the normal vector of the best-fit plane.
+    :rtype: list of floats
+    """
     import numpy as np
     XYZ = np.array(points)
     [rows, cols] = XYZ.shape
     # Set up constraint equations of the form  AB = 0,
     # where B is a column vector of the plane coefficients
     # in the form b(1)*X + b(2)*Y +b(3)*Z + b(4) = 0.
     p = (np.ones((rows, 1)))
```

## Comparing `robodk-5.5.5.dist-info/LICENSE` & `robodk-5.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `robodk-5.5.5.dist-info/METADATA` & `robodk-5.6.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robodk
-Version: 5.5.5
+Version: 5.6.0
 Summary: RoboDK tools for simulating and programming industrial robots (implements the RoboDK API)
 Home-page: https://robodk.com/doc/en/PythonAPI/index.html
 Author: RoboDK Inc.
 Author-email: info@robodk.com
 License: Apache Software License
 Keywords: industrial robot,simulation,offline programming,robot programming,robotics,online programming,3D simulator,post processors
 Platform: UNKNOWN
@@ -61,17 +61,19 @@
 While RoboDK's graphical user interface can be used to create programs, it is possible to extend the robot controller limitations by using a universal programming language such as Python.
 The following page provides an overview of the RoboDK API using Python: <https://robodk.com/offline-programming>.
 
 The `robodk` package is available on [PyPi](https://pypi.python.org/pypi/robodk/).
 
 ![Python programming in RoboDK](https://raw.githubusercontent.com/RoboDK/RoboDK-API/master/Python/Python-Programming-RoboDK.png)
 
-RoboDK can be used for a wide range of applications, such as 3D printing, robot machining, synchronizing multiple robots, pick and place, and so on.
- * [Industrial Robot application examples](https://robodk.com/examples)
- * [RoboDK Blog](https://robodk.com/blog)
+RoboDK can be used for a wide range of robot manufacturing applications, such as robot machining, 3D printing, synchronizing multiple robots, pick and place, and so on.
+ * [Industrial Robot application examples](https://robodk.com/stations)
+ * [Robot library](https://robodk.com/library)
+ * [RoboDK Blog](https://robodk.com/blog/)
+ * [RoboDK Forum](https://robodk.com/forum/)
 
 **Important:** The RoboDK API is not the same as the [RoboDK Plug-In interface](https://robodk.com/doc/en/PlugIns/index.html).
 
 Documentation
 ---------------
 
 The `robodk` package includes the following modules:
```

## Comparing `robodk-5.5.5.dist-info/RECORD` & `robodk-5.6.0.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 pylint_robodk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pylint_robodk/pylint_robodk.py,sha256=iYjRh4qyQKnB-lTY_YJuRu8931imrzzKH9JLNwPUC1c,1551
 robodk/__init__.py,sha256=AKKmH90Q2slRJHJwWCjbPMdPDuU1Nm_bBTxH5HXHi18,1516
 robodk/roboapps.py,sha256=4ASX0n1emCtszBBjVpaehUYwb0SVAbeJi1du2XrmTIs,52619
-robodk/robodialogs.py,sha256=bZbt3iekQpmHHTQDRiEOxm_lOBFBpP4z1INssN5QMIM,45464
+robodk/robodialogs.py,sha256=_r6SNV4fsJF25jdjdQ9jypLJcMJ66_88b_i3CyOo7Cs,45672
 robodk/robofileio.py,sha256=bECjUE05RKE-9uGRexOinYKrOV4dsLrLzPKt4YcLfqg,12502
-robodk/robolink.py,sha256=XicOC2gllTTxzjR5l8wVEtdiMuxjbdGHhO36n7TXgSs,326660
+robodk/robolink.py,sha256=az0xPrrHci1bQjiQ_Q9Gn8AoHO5Dq8CVHjkFmhj8kwg,326752
 robodk/robolinkutils.py,sha256=mGfOtayuhnLlFHFy1hvaK52NbeunH-e-MWabKfUrG9M,10012
-robodk/robomath.py,sha256=V_zrtpTaamR9QP1TAgEbL3rInzgDRfx2QgHAzXL-nC8,68442
+robodk/robomath.py,sha256=ntGNaSLHNRHWpFOIWFO6nqbAm5H2HThHjtMR_uEKn00,68988
 robolink/__init__.py,sha256=RqchTjeRBU7Hnko58B9xHigsffzo9R6nlNs83zA5NhU,1210
-robodk-5.5.5.dist-info/LICENSE,sha256=D5sOGFtT_R0frDUaM9bm7RVnQJ_G2ivMdr1DRZCu8WU,587
-robodk-5.5.5.dist-info/METADATA,sha256=CcsHXlrCasL0HJEqvTKfBvkQRy8iMfPoEul2q7j1xuI,12710
-robodk-5.5.5.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-robodk-5.5.5.dist-info/top_level.txt,sha256=3CTL620vD_h4LfM0G4AXCDqkk8qr2UpQZMQU_gYi9Sc,30
-robodk-5.5.5.dist-info/RECORD,,
+robodk-5.6.0.dist-info/LICENSE,sha256=D5sOGFtT_R0frDUaM9bm7RVnQJ_G2ivMdr1DRZCu8WU,587
+robodk-5.6.0.dist-info/METADATA,sha256=JrOFqIbUC1sYGN8kw_s1s6cG8sGYy_rk50rarywnY8w,12823
+robodk-5.6.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+robodk-5.6.0.dist-info/top_level.txt,sha256=3CTL620vD_h4LfM0G4AXCDqkk8qr2UpQZMQU_gYi9Sc,30
+robodk-5.6.0.dist-info/RECORD,,
```

