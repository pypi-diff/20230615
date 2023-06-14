# Comparing `tmp/focalnet-tf-0.0.1.tar.gz` & `tmp/focalnet-tf-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\focalnet-tf-0.0.1.tar", last modified: Sun Jun 11 22:13:03 2023, max compression
+gzip compressed data, was "dist\focalnet-tf-0.0.2.tar", last modified: Wed Jun 14 23:50:24 2023, max compression
```

## Comparing `focalnet-tf-0.0.1.tar` & `focalnet-tf-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 22:13:03.000000 focalnet-tf-0.0.1/
--rw-rw-rw-   0        0        0     1086 2023-06-11 19:49:16.000000 focalnet-tf-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4288 2023-06-11 22:13:03.000000 focalnet-tf-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3727 2023-06-11 20:34:38.000000 focalnet-tf-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 22:13:03.000000 focalnet-tf-0.0.1/focalnet/
--rw-rw-rw-   0        0        0      195 2023-06-11 13:35:42.000000 focalnet-tf-0.0.1/focalnet/__init__.py
--rw-rw-rw-   0        0        0     1667 2023-06-11 22:12:59.000000 focalnet-tf-0.0.1/focalnet/download_weights.py
--rw-rw-rw-   0        0        0     1680 2023-06-04 22:28:23.000000 focalnet-tf-0.0.1/focalnet/drop.py
--rw-rw-rw-   0        0        0    23057 2023-06-11 20:51:44.000000 focalnet-tf-0.0.1/focalnet/focalnet.py
--rw-rw-rw-   0        0        0     5288 2023-06-11 10:56:27.000000 focalnet-tf-0.0.1/focalnet/focalnet_utils.py
--rw-rw-rw-   0        0        0    35363 2023-06-09 22:50:12.000000 focalnet-tf-0.0.1/focalnet/imagenet-1k.json
--rw-rw-rw-   0        0        0   872487 2023-06-10 00:38:09.000000 focalnet-tf-0.0.1/focalnet/imagenet-21k.json
--rw-rw-rw-   0        0        0   773963 2023-06-10 00:38:09.000000 focalnet-tf-0.0.1/focalnet/imagenet-22k-reorder.json
-drwxrwxrwx   0        0        0        0 2023-06-11 22:13:03.000000 focalnet-tf-0.0.1/focalnet_tf.egg-info/
--rw-rw-rw-   0        0        0     4288 2023-06-11 22:13:02.000000 focalnet-tf-0.0.1/focalnet_tf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-06-11 22:13:02.000000 focalnet-tf-0.0.1/focalnet_tf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 22:13:02.000000 focalnet-tf-0.0.1/focalnet_tf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-11 22:13:02.000000 focalnet-tf-0.0.1/focalnet_tf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-11 22:13:02.000000 focalnet-tf-0.0.1/focalnet_tf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 22:13:03.000000 focalnet-tf-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1105 2023-06-11 20:57:26.000000 focalnet-tf-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 22:13:03.000000 focalnet-tf-0.0.1/tests/
--rw-rw-rw-   0        0        0     7608 2023-06-11 20:50:45.000000 focalnet-tf-0.0.1/tests/test_focalnet.py
--rw-rw-rw-   0        0        0    15498 2023-06-11 20:50:53.000000 focalnet-tf-0.0.1/tests/test_reproductible.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:50:24.000000 focalnet-tf-0.0.2/
+-rw-rw-rw-   0        0        0     1086 2023-06-11 19:49:16.000000 focalnet-tf-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4288 2023-06-14 23:50:24.000000 focalnet-tf-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3727 2023-06-11 20:34:38.000000 focalnet-tf-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 23:50:24.000000 focalnet-tf-0.0.2/focalnet/
+-rw-rw-rw-   0        0        0      195 2023-06-11 13:35:42.000000 focalnet-tf-0.0.2/focalnet/__init__.py
+-rw-rw-rw-   0        0        0     1667 2023-06-11 22:12:59.000000 focalnet-tf-0.0.2/focalnet/download_weights.py
+-rw-rw-rw-   0        0        0     1680 2023-06-04 22:28:23.000000 focalnet-tf-0.0.2/focalnet/drop.py
+-rw-rw-rw-   0        0        0    23191 2023-06-14 23:09:34.000000 focalnet-tf-0.0.2/focalnet/focalnet.py
+-rw-rw-rw-   0        0        0     5289 2023-06-14 23:48:00.000000 focalnet-tf-0.0.2/focalnet/focalnet_utils.py
+-rw-rw-rw-   0        0        0    35363 2023-06-09 22:50:12.000000 focalnet-tf-0.0.2/focalnet/imagenet-1k.json
+-rw-rw-rw-   0        0        0   872487 2023-06-10 00:38:09.000000 focalnet-tf-0.0.2/focalnet/imagenet-21k.json
+-rw-rw-rw-   0        0        0   773963 2023-06-10 00:38:09.000000 focalnet-tf-0.0.2/focalnet/imagenet-22k-reorder.json
+drwxrwxrwx   0        0        0        0 2023-06-14 23:50:24.000000 focalnet-tf-0.0.2/focalnet_tf.egg-info/
+-rw-rw-rw-   0        0        0     4288 2023-06-14 23:50:23.000000 focalnet-tf-0.0.2/focalnet_tf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-06-14 23:50:23.000000 focalnet-tf-0.0.2/focalnet_tf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 23:50:23.000000 focalnet-tf-0.0.2/focalnet_tf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-14 23:50:23.000000 focalnet-tf-0.0.2/focalnet_tf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 23:50:23.000000 focalnet-tf-0.0.2/focalnet_tf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 23:50:24.000000 focalnet-tf-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1105 2023-06-14 23:49:06.000000 focalnet-tf-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:50:24.000000 focalnet-tf-0.0.2/tests/
+-rw-rw-rw-   0        0        0     7608 2023-06-11 20:50:45.000000 focalnet-tf-0.0.2/tests/test_focalnet.py
+-rw-rw-rw-   0        0        0    15498 2023-06-11 20:50:53.000000 focalnet-tf-0.0.2/tests/test_reproductible.py
```

### Comparing `focalnet-tf-0.0.1/LICENSE` & `focalnet-tf-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.1/PKG-INFO` & `focalnet-tf-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: focalnet-tf
-Version: 0.0.1
+Version: 0.0.2
 Summary: Re-implementation of FocalNet for tensorflow 2.X
 Home-page: https://github.com/Shiro-LK/focalnet-tf
 Download-URL: https://github.com/Shiro-LK/focalnet-tf.git
 Author: Shiro-LK
 Author-email: shirosaki94@gmail.com
 License: MIT License
 Keywords: focalnet,tensorflow
```

### Comparing `focalnet-tf-0.0.1/README.md` & `focalnet-tf-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.1/focalnet/download_weights.py` & `focalnet-tf-0.0.2/focalnet/download_weights.py`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.1/focalnet/drop.py` & `focalnet-tf-0.0.2/focalnet/drop.py`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.1/focalnet/focalnet.py` & `focalnet-tf-0.0.2/focalnet/focalnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -420,15 +420,18 @@
                 normalize_modulator=False, 
                 pooling="avg",
                 include_top=True,
                 name=None,
                 act_head=None,
                 **kwargs):
         super().__init__(name=name)
-
+        if type(img_size) == int:
+            img_size = (img_size, img_size)
+        
+        assert type(img_size) == tuple
         self.num_layers = len(depths)
         embed_dim = [embed_dim * (2 ** i) for i in range(self.num_layers)]
 
         self.num_classes = num_classes
         self.embed_dim = embed_dim
         self.patch_norm = patch_norm
         self.num_features = embed_dim[-1]
@@ -479,15 +482,15 @@
                     )
             self.layers_.append(layer)
 
         self.norm = norm_layer(epsilon=1e-5, name="norm")
         self.avgpool = GlobalAveragePooling1D() if pooling == "avg" else GlobalMaxPooling1D() if pooling == "max" else None
         self.head = Dense(num_classes, name="head", activation=act_head, dtype=tf.float32) if num_classes > 0 and include_top else  Identity()
         self.return_modulator = False
-        self.build((1, img_size, img_size, 3))
+        self.build((1, img_size[0], img_size[1], 3))
 
     def set_return_modulator(self, do_return=True):
         self.return_modulator = do_return 
 
     def extract_features(self, x, return_modulator):
         x, H, W = self.patch_embed(x)
         x = self.pos_drop(x)
```

### Comparing `focalnet-tf-0.0.1/focalnet/focalnet_utils.py` & `focalnet-tf-0.0.2/focalnet/focalnet_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     idx2label = [data[str(k)]  for k in range(len(data))]
     return idx2label 
 
 imagenet1k = imagenet_1k()
 imagenet22k = imagenet_22k()
 
 
-def load_focalnet(model_name, input_shape=(224, 224, 3), pretrained=False, return_model=True, num_classes=None, **kwargs):
+def load_focalnet(model_name, input_shape=(224, 224, 3), pretrained=False, return_model=False, num_classes=None, **kwargs):
     #print(kwargs)
     focal_levels=[2,2,2,2]
     focal_windows = [3, 3, 3, 3]
     use_conv_embed = False 
     use_postln = False 
     use_layerscale = False 
     normalize_modulator = False
```

### Comparing `focalnet-tf-0.0.1/focalnet/imagenet-1k.json` & `focalnet-tf-0.0.2/focalnet/imagenet-1k.json`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.1/focalnet/imagenet-21k.json` & `focalnet-tf-0.0.2/focalnet/imagenet-21k.json`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.1/focalnet/imagenet-22k-reorder.json` & `focalnet-tf-0.0.2/focalnet/imagenet-22k-reorder.json`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.1/focalnet_tf.egg-info/PKG-INFO` & `focalnet-tf-0.0.2/focalnet_tf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: focalnet-tf
-Version: 0.0.1
+Version: 0.0.2
 Summary: Re-implementation of FocalNet for tensorflow 2.X
 Home-page: https://github.com/Shiro-LK/focalnet-tf
 Download-URL: https://github.com/Shiro-LK/focalnet-tf.git
 Author: Shiro-LK
 Author-email: shirosaki94@gmail.com
 License: MIT License
 Keywords: focalnet,tensorflow
```

### Comparing `focalnet-tf-0.0.1/setup.py` & `focalnet-tf-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open('README.md', encoding="utf-8-sig") as f:
         README = f.read()
     return README
 
 
 setup(
     name='focalnet-tf',
-    version='0.0.1',    
+    version='0.0.2',    
     description='Re-implementation of FocalNet for tensorflow 2.X',
     author='Shiro-LK',
     author_email='shirosaki94@gmail.com',
     license='MIT License',
     packages=['focalnet'],
     package_data={'focalnet': ['imagenet-1k.json', 'imagenet-21k.json', 'imagenet-22k-reorder.json']},
     long_description=readme(),
```

### Comparing `focalnet-tf-0.0.1/tests/test_focalnet.py` & `focalnet-tf-0.0.2/tests/test_focalnet.py`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.1/tests/test_reproductible.py` & `focalnet-tf-0.0.2/tests/test_reproductible.py`

 * *Files identical despite different names*

