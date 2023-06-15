# Comparing `tmp/napatrackmater-3.7.7.tar.gz` & `tmp/napatrackmater-3.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-i54lffzu/napatrackmater-3.7.7.tar", last modified: Wed Jun 14 08:19:56 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-00rw5a1q/napatrackmater-3.7.8.tar", last modified: Thu Jun 15 20:53:18 2023, max compression
```

## Comparing `napatrackmater-3.7.7.tar` & `napatrackmater-3.7.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-14 08:19:56.681998 napatrackmater-3.7.7/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.7.7/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-14 08:19:56.675925 napatrackmater-3.7.7/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.7.7/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-14 08:19:56.462034 napatrackmater-3.7.7/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.7.7/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.7.7/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   110394 2023-06-11 19:02:37.000000 napatrackmater-3.7.7/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.7.7/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.7.7/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    14305 2023-06-14 08:19:13.000000 napatrackmater-3.7.7/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.7.7/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.7.7/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.7.7/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-14 08:19:32.000000 napatrackmater-3.7.7/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-14 08:19:56.644260 napatrackmater-3.7.7/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-14 08:19:55.000000 napatrackmater-3.7.7/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-14 08:19:56.000000 napatrackmater-3.7.7/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-14 08:19:55.000000 napatrackmater-3.7.7/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-14 08:19:55.000000 napatrackmater-3.7.7/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-14 08:19:55.000000 napatrackmater-3.7.7/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-14 08:19:55.000000 napatrackmater-3.7.7/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-14 08:19:56.684005 napatrackmater-3.7.7/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.7.7/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-15 20:53:18.562601 napatrackmater-3.7.8/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.7.8/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-15 20:53:18.558343 napatrackmater-3.7.8/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.7.8/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-15 20:53:18.357553 napatrackmater-3.7.8/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.7.8/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.7.8/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   110394 2023-06-11 19:02:37.000000 napatrackmater-3.7.8/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16426 2023-06-15 20:52:31.000000 napatrackmater-3.7.8/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.7.8/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    14304 2023-06-15 20:51:11.000000 napatrackmater-3.7.8/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.7.8/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.7.8/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.7.8/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-15 20:52:39.000000 napatrackmater-3.7.8/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-15 20:53:18.524700 napatrackmater-3.7.8/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-15 20:53:17.000000 napatrackmater-3.7.8/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-15 20:53:17.000000 napatrackmater-3.7.8/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-15 20:53:17.000000 napatrackmater-3.7.8/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-15 20:53:17.000000 napatrackmater-3.7.8/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-15 20:53:17.000000 napatrackmater-3.7.8/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-15 20:53:17.000000 napatrackmater-3.7.8/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-15 20:53:18.563779 napatrackmater-3.7.8/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.7.8/setup.py
```

### Comparing `napatrackmater-3.7.7/LICENSE` & `napatrackmater-3.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.7/PKG-INFO` & `napatrackmater-3.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.7.7
+Version: 3.7.8
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.7.7/README.md` & `napatrackmater-3.7.8/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.7/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.7.8/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.7/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.7.8/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.7/napatrackmater/Trackmate.py` & `napatrackmater-3.7.8/napatrackmater/Trackmate.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.7/napatrackmater/Trackvector.py` & `napatrackmater-3.7.8/napatrackmater/Trackvector.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,24 +210,24 @@
                       nested_unique_dynamic_properties = self.unique_dynamic_properties[k]
                       nested_unique_shape_properties = self.unique_shape_properties[k]
                       for current_unique_id in nested_unique_dynamic_properties.keys():
                              
                              unique_dynamic_properties_tracklet = nested_unique_dynamic_properties[current_unique_id]
                              current_time, speed, motion_angle, acceleration, distance_cell_mask, radial_angle, cell_axis_mask = unique_dynamic_properties_tracklet
                              unique_shape_properties_tracklet = nested_unique_shape_properties[current_unique_id]
-                             current_time, current_z, current_y, current_x, radius, volume, eccentricity_comp_first, eccentricity_comp_second, surface_area, current_cluster_class, current_cluster_class_score = unique_shape_properties_tracklet
+                             current_time, current_z, current_y, current_x, radius, volume, eccentricity_comp_first, eccentricity_comp_second, surface_area = unique_shape_properties_tracklet
                              
                              track_id_array = np.ones(current_time.shape)
                              dividing_array = np.ones(current_time.shape)
                              number_dividing_array = np.ones(current_time.shape)
                              for i in range(track_id_array.shape[0]):
                                     track_id_array[i] = track_id_array[i] * current_unique_id
                                     dividing_array[i] = dividing_array[i] * dividing 
                                     number_dividing_array[i] = number_dividing_array[i] * number_dividing
-                             self.current_shape_dynamic_vectors.append([ track_id_array, current_time, current_z, current_y, current_x, dividing_array, number_dividing_array, radius, volume, eccentricity_comp_first, eccentricity_comp_second, surface_area, current_cluster_class, speed, motion_angle, acceleration, distance_cell_mask, radial_angle, cell_axis_mask])
+                             self.current_shape_dynamic_vectors.append([ track_id_array, current_time, current_z, current_y, current_x, dividing_array, number_dividing_array, radius, volume, eccentricity_comp_first, eccentricity_comp_second, surface_area, speed, motion_angle, acceleration, distance_cell_mask, radial_angle, cell_axis_mask])
 
           
                print(f'returning shape and dynamic vectors as list {len(self.current_shape_dynamic_vectors)}')
 
 
         def _interactive_function(self):
                
@@ -291,19 +291,15 @@
                                           
                                           "volume_pixels": 
                                                  np.asarray(unique_tracks_properties, dtype="float64")[:, 6],
                                           
                                           "acceleration": 
                                                  np.asarray(unique_tracks_properties, dtype="float64")[:, 7],
                                    
-                                          "cluster_class": 
-                                                 np.asarray(unique_tracks_properties, dtype="float64")[:, 8],
-                                          
-                                          "cluster_score": 
-                                                 np.asarray(unique_tracks_properties, dtype="float64")[:, 9],
+                                       
                                           
                                           }   
                                 for layer in list(self._viewer.layers):
                                    if (
                                           "Track" == layer.name
                                           or "Boxes" == layer.name
                                           or "Track_points" == layer.name
```

### Comparing `napatrackmater-3.7.7/napatrackmater/__init__.py` & `napatrackmater-3.7.8/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.7/napatrackmater/clustering.py` & `napatrackmater-3.7.8/napatrackmater/clustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         output_labels = output_labels + [int(float(label_input)) for label_input in labels]
         for outputs in outputs_list:
             output_cloud_eccentricity = output_cloud_eccentricity +  [tuple(get_eccentricity(cloud_input.detach().cpu().numpy()))[0] for cloud_input in outputs]
             output_largest_eigenvector = output_largest_eigenvector + [get_eccentricity(cloud_input.detach().cpu().numpy())[1] for cloud_input in outputs]
             output_largest_eigenvalue = output_largest_eigenvalue + [get_eccentricity(cloud_input.detach().cpu().numpy())[2] for cloud_input in outputs]
             output_dimensions = output_dimensions + [get_eccentricity(cloud_input.detach().cpu().numpy())[3] for cloud_input in outputs]
             output_cloud_surface_area = output_cloud_surface_area + [float(get_surface_area(cloud_input.detach().cpu().numpy())) for cloud_input in outputs]
-                    
+                   
         return output_labels, output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue, output_dimensions, output_cloud_surface_area             
 
 
        
 
 def _label_cluster(label_image, num_points, min_size, ndim):
```

### Comparing `napatrackmater-3.7.7/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.7.8/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.7/napatrackmater/fate_mapping.py` & `napatrackmater-3.7.8/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.7/napatrackmater/pretrained.py` & `napatrackmater-3.7.8/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.7/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.7.8/napatrackmater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.7.7
+Version: 3.7.8
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.7.7/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.7.8/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.7/setup.py` & `napatrackmater-3.7.8/setup.py`

 * *Files identical despite different names*

