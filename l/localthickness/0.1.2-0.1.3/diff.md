# Comparing `tmp/localthickness-0.1.2.tar.gz` & `tmp/localthickness-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localthickness-0.1.2.tar", last modified: Mon Apr 10 17:52:01 2023, max compression
+gzip compressed data, was "localthickness-0.1.3.tar", last modified: Wed Jun 14 22:32:58 2023, max compression
```

## Comparing `localthickness-0.1.2.tar` & `localthickness-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 VAND       (502) staff       (20)        0 2023-04-10 17:52:01.165019 localthickness-0.1.2/
--rw-r--r--   0 VAND       (502) staff       (20)    35149 2022-10-22 19:35:32.000000 localthickness-0.1.2/LICENSE
--rw-r--r--   0 VAND       (502) staff       (20)     1038 2023-04-10 17:52:01.164893 localthickness-0.1.2/PKG-INFO
--rw-r--r--   0 VAND       (502) staff       (20)      726 2023-04-10 07:35:16.000000 localthickness-0.1.2/README.md
-drwxr-xr-x   0 VAND       (502) staff       (20)        0 2023-04-10 17:52:01.164669 localthickness-0.1.2/localthickness.egg-info/
--rw-r--r--   0 VAND       (502) staff       (20)     1038 2023-04-10 17:52:01.000000 localthickness-0.1.2/localthickness.egg-info/PKG-INFO
--rw-r--r--   0 VAND       (502) staff       (20)      233 2023-04-10 17:52:01.000000 localthickness-0.1.2/localthickness.egg-info/SOURCES.txt
--rw-r--r--   0 VAND       (502) staff       (20)        1 2023-04-10 17:52:01.000000 localthickness-0.1.2/localthickness.egg-info/dependency_links.txt
--rw-r--r--   0 VAND       (502) staff       (20)       10 2023-04-10 17:52:01.000000 localthickness-0.1.2/localthickness.egg-info/requires.txt
--rw-r--r--   0 VAND       (502) staff       (20)       15 2023-04-10 17:52:01.000000 localthickness-0.1.2/localthickness.egg-info/top_level.txt
--rwx------   0 VAND       (502) staff       (20)    18962 2023-04-10 12:54:44.000000 localthickness-0.1.2/localthickness.py
--rw-r--r--   0 VAND       (502) staff       (20)       38 2023-04-10 17:52:01.165069 localthickness-0.1.2/setup.cfg
--rw-r--r--   0 VAND       (502) staff       (20)      579 2023-03-05 23:22:51.000000 localthickness-0.1.2/setup.py
+drwxr-xr-x   0 VAND       (502) staff       (20)        0 2023-06-14 22:32:58.694208 localthickness-0.1.3/
+-rw-r--r--   0 VAND       (502) staff       (20)    35149 2022-10-22 19:35:32.000000 localthickness-0.1.3/LICENSE
+-rw-r--r--   0 VAND       (502) staff       (20)     1769 2023-06-14 22:32:58.694071 localthickness-0.1.3/PKG-INFO
+-rw-r--r--   0 VAND       (502) staff       (20)     1457 2023-06-07 18:23:50.000000 localthickness-0.1.3/README.md
+drwxr-xr-x   0 VAND       (502) staff       (20)        0 2023-06-14 22:32:58.693852 localthickness-0.1.3/localthickness.egg-info/
+-rw-r--r--   0 VAND       (502) staff       (20)     1769 2023-06-14 22:32:58.000000 localthickness-0.1.3/localthickness.egg-info/PKG-INFO
+-rw-r--r--   0 VAND       (502) staff       (20)      233 2023-06-14 22:32:58.000000 localthickness-0.1.3/localthickness.egg-info/SOURCES.txt
+-rw-r--r--   0 VAND       (502) staff       (20)        1 2023-06-14 22:32:58.000000 localthickness-0.1.3/localthickness.egg-info/dependency_links.txt
+-rw-r--r--   0 VAND       (502) staff       (20)       10 2023-06-14 22:32:58.000000 localthickness-0.1.3/localthickness.egg-info/requires.txt
+-rw-r--r--   0 VAND       (502) staff       (20)       15 2023-06-14 22:32:58.000000 localthickness-0.1.3/localthickness.egg-info/top_level.txt
+-rwx------   0 VAND       (502) staff       (20)    19017 2023-06-14 22:09:52.000000 localthickness-0.1.3/localthickness.py
+-rw-r--r--   0 VAND       (502) staff       (20)       38 2023-06-14 22:32:58.694256 localthickness-0.1.3/setup.cfg
+-rw-r--r--   0 VAND       (502) staff       (20)      579 2023-06-14 22:11:37.000000 localthickness-0.1.3/setup.py
```

### Comparing `localthickness-0.1.2/LICENSE` & `localthickness-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `localthickness-0.1.2/localthickness.py` & `localthickness-0.1.3/localthickness.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,15 +337,15 @@
     ax.set_title(f'slice z={z}')
     fig.canvas.mpl_connect('key_press_event', key_press)
     plt.show()
 
 
 #%% HELPING FUNCTIONS
 
-def create_test_volume(dim, sigma=7, threshold=0, boundary=0, frame = True, seed = None):
+def create_test_volume(dim, sigma=7, threshold=0, boundary=0, frame=True, seed=None):
     """ Creates test volume for local thickness and porosity analysis.
     Arguments:
         dim: tuple giving the size of the volume
         sigma: smoothing scale, higher value - smoother objects
         threshold: a value close to 0, larger value - less material (smaller objects)
         boundary: strength of imposing object boundary pulled inwards
         frame: one-voxel frame of False 
@@ -400,21 +400,21 @@
     gray = ~(thickness>0)  
     if blend:
         gray = edt.edt(gray) - edt.edt(~gray) - gray + 0.5
         gray = np.clip(gray, -25, 25)
         gray = np.exp(0.1 * gray)
         gray = gray / (gray + 1)  # values between 0 and 1 with 0.5 at interface
     
-    if dilate:
+    
+    for i in range(dilate):  # if dilate is True, only once
         thickness = dilate3d(thickness)
 
     return thickness, gray, maxval
 
 
-
 def save_thickness_volumes(thickness, filename_root, **options):
     '''Saves results of local thickness analysis in two volumes suitable for
     visualization in paraview.
     Inputs:
         thickness: local thickness volume, a 3D numpy array, where 0 is 
             bacground and positive values are thickness.
         filename_root: root of the filename, sufixes will be added 
@@ -441,14 +441,15 @@
             t_rgba = cmap(t/maxval)
             if paraview_alpha:
                 t_rgba[:, :, 3] = 1 - t_rgba[:, :, 3]  # flipping opacity to work with paraview
             rgba.write((255*t_rgba).astype(np.uint8), photometric='rgb', extrasamples = 'ASSOCALPHA') 
             # rgb.write((255*t_rgba[:, :, :3]).astype(np.uint8), photometric='rgb')
     
 
+
 #%% VTK WRITE FUNCTIONS
 
 def save_gray2vtk(volume, filename, filetype='ASCII', origin=(0,0,0),
                   spacing=(1,1,1), dataname='gray'):
     ''' Writes a vtk file with grayscace volume data.
     Arguments:
        volume: a grayscale volume, values will be saved as floats
@@ -480,14 +481,15 @@
             volume = volume.astype('float32') # Pareview expects 4-bytes float 
             volume.byteswap(True) # Paraview expects big-endian 
             volume.tofile(f)
     else: # ASCII
         with open(filename, 'a') as f:
             np.savetxt(f,volume.ravel(),fmt='%.5g', newline= ' ')
         
+        
 def save_rgba2vtk(rgba, dim, filename, filetype='ASCII'):
     ''' Writes a vtk file with RGBA volume data.
     Arguments:
        rgba: an array of shape (N,4) containing RGBA values
        dim: volume shape, such that prod(dim) = N
        filename: filename with .vtk extension
        filetype: file type 'ASCII' or 'BINARY'. Writing a binary file might not
```

### Comparing `localthickness-0.1.2/setup.py` & `localthickness-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = 'localthickness',
-    version = '0.1.2',
+    version = '0.1.3',
     description = 'Fast local thickness in 3D and 2D.',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/vedranaa/local-thickness',
     author = 'VA Dahl and AB Dahl',
     author_email = 'vand@dtu.dk, abda@dtu.dk',
     license ='GPL-3.0 license',
```

