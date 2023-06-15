# Comparing `tmp/polybeat-0.0.1.tar.gz` & `tmp/polybeat-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polybeat-0.0.1.tar", last modified: Fri Feb 17 07:32:46 2023, max compression
+gzip compressed data, was "polybeat-1.0.0.tar", last modified: Thu Jun 15 20:27:36 2023, max compression
```

## Comparing `polybeat-0.0.1.tar` & `polybeat-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-02-17 07:32:46.647349 polybeat-0.0.1/
--rw-rw-rw-   0        0        0      693 2023-02-17 07:32:46.646336 polybeat-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      128 2023-02-17 06:59:44.000000 polybeat-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-17 07:32:46.624123 polybeat-0.0.1/polybeat/
--rw-rw-rw-   0        0        0     3273 2023-02-17 07:31:39.000000 polybeat-0.0.1/polybeat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-17 07:32:46.643123 polybeat-0.0.1/polybeat/sounds/
--rw-rw-rw-   0        0        0   209324 2023-01-27 06:10:18.000000 polybeat-0.0.1/polybeat/sounds/kick_drum.wav
--rw-rw-rw-   0        0        0   209324 2023-01-26 11:44:41.000000 polybeat-0.0.1/polybeat/sounds/low_bongo.wav
--rw-rw-rw-   0        0        0   209324 2023-01-27 06:10:18.000000 polybeat-0.0.1/polybeat/sounds/open_conga.wav
-drwxrwxrwx   0        0        0        0 2023-02-17 07:32:46.636122 polybeat-0.0.1/polybeat.egg-info/
--rw-rw-rw-   0        0        0      693 2023-02-17 07:32:46.000000 polybeat-0.0.1/polybeat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-02-17 07:32:46.000000 polybeat-0.0.1/polybeat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-17 07:32:46.000000 polybeat-0.0.1/polybeat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-02-17 07:32:46.000000 polybeat-0.0.1/polybeat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-17 07:32:46.647349 polybeat-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      909 2023-02-17 07:26:15.000000 polybeat-0.0.1/setup.py
+drwxrwxrwx   0 pcc       (1000) pcc       (1000)        0 2023-06-15 20:27:36.186970 polybeat-1.0.0/
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)     1679 2023-06-15 20:27:36.184024 polybeat-1.0.0/PKG-INFO
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)     1141 2023-06-15 20:22:34.000000 polybeat-1.0.0/README.md
+drwxrwxrwx   0 pcc       (1000) pcc       (1000)        0 2023-06-15 20:27:35.953982 polybeat-1.0.0/polybeat/
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)     4260 2023-06-15 20:13:07.000000 polybeat-1.0.0/polybeat/__init__.py
+drwxrwxrwx   0 pcc       (1000) pcc       (1000)        0 2023-06-15 20:27:36.154998 polybeat-1.0.0/polybeat/sounds/
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)   209324 2023-01-27 06:10:20.000000 polybeat-1.0.0/polybeat/sounds/kick_drum.wav
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)   209324 2023-01-26 11:44:42.000000 polybeat-1.0.0/polybeat/sounds/low_bongo.wav
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)   209324 2023-01-27 06:10:20.000000 polybeat-1.0.0/polybeat/sounds/open_conga.wav
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)   209324 2023-01-26 11:44:42.000000 polybeat-1.0.0/polybeat/sounds/side_stick.wav
+drwxrwxrwx   0 pcc       (1000) pcc       (1000)        0 2023-06-15 20:27:36.039052 polybeat-1.0.0/polybeat.egg-info/
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)     1679 2023-06-15 20:27:35.000000 polybeat-1.0.0/polybeat.egg-info/PKG-INFO
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)      289 2023-06-15 20:27:35.000000 polybeat-1.0.0/polybeat.egg-info/SOURCES.txt
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)        1 2023-06-15 20:27:35.000000 polybeat-1.0.0/polybeat.egg-info/dependency_links.txt
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)        9 2023-06-15 20:27:35.000000 polybeat-1.0.0/polybeat.egg-info/top_level.txt
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)       38 2023-06-15 20:27:36.187986 polybeat-1.0.0/setup.cfg
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)      911 2023-06-15 17:27:09.000000 polybeat-1.0.0/setup.py
```

### Comparing `polybeat-0.0.1/polybeat/__init__.py` & `polybeat-1.0.0/polybeat/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,60 @@
 from manim import *
 import numpy as np
 import os
+    
+config.disable_caching = True
 
-def play(n_edges=[3,4,12], vols=[0,-2,-6]):
+def play(
+    rhythms=[3,4,6,12],
+    custom_order=None,
+    colors=[RED,YELLOW,BLUE,GREEN],
+    sounds=['kick_drum','open_conga','side_stick','low_bongo'],
+    volumes=[0,-2,-6,-4],
+    cycle_time=1.8,
+    dot_radius=0.16,
+    width_range=[2.5,3.5],
+    preview=True,
+):
     class Polybeat(Scene):
         def construct(self):
-            dr = .16
-            colors = ['#ff7473','#ffc952','#47b8e0']
-            N = len(n_edges)
+            dr = dot_radius
+            N = len(rhythms)
             op = .4
-            T = 1.8
-            sounds = ['kick_drum','open_conga','low_bongo']
-            dirname = os.path.dirname(__file__)
-            sounds = [os.path.join(dirname,'sounds',s) for s in sounds]
-            trs = np.linspace(2.5,3.8,N)
+            T = cycle_time
+            trs = np.linspace(*width_range,N)
+            defaut_dir = os.path.dirname(__file__)
+            defaut_sounds = [os.path.join(defaut_dir,'sounds',s) for s in sounds]
+            if custom_order:
+                idx=custom_order
+            else:
+                idx=list(range(N))[::-1]
 
             circs = [
                 Circle(radius=r).rotate(PI/2)
                 for r in trs
             ]
 
             ps = [
                 [i/n for i in range(n)] 
-                for n in n_edges
+                for n in rhythms
             ]
             vs = [
                 [circs[i].point_from_proportion(p) for p in ps[i]]
                 for i in range(N)
             ]
             geoms = [Polygon(*v).set_stroke(colors[i],14,op) for i,v in enumerate(vs)]
 
             dots = []
             for i in range(N):
                 dots.append(
                     Dot([0,3.5,0], dr*1.5, color=colors[i]).set_opacity(1)
                 )
                 dots[-1]._i = i
-                dots[-1]._n = n_edges[i]
+                dots[-1]._n = rhythms[i]
                 dots[-1]._ps = ps[i]
                 dots[-1]._p = .9999
                 dots[-1]._g = geoms[i]
                 dots[-1]._on = False
 
             def update_dot(d, dt):
                 if d._on:
@@ -51,52 +65,63 @@
                     else:
                         d._g.set_stroke(opacity=op)
 
                     d.move_to(d._g.point_from_proportion(d._p))
                     next_p = (d._p + dt/T) % 1
                     for p in d._ps:
                         if (d._p<=p and next_p>=p) or (next_p < d._p):
-                            self.add_sound(sounds[d._i], 0, vols[d._i])
+                            try:
+                                self.add_sound(defaut_sounds[d._i], 0, volumes[d._i])
+                            except:
+                                self.add_sound(sounds[d._i], 0, volumes[d._i])
                             geoms[d._i].set_stroke(opacity=1)
                             break
                     d._p = next_p
                 else:
                     d.set_opacity(0)
                     d._g.set_stroke(opacity=0)
                     d._p = .9999
             for d in dots[::-1]: 
                 d.add_updater(update_dot)
 
-            def play(i0,i1,i2):
-                dots[i0]._on = True
-                self.wait(T)
-                dots[i1]._on = True
-                self.wait(T*2)
-                dots[i2]._on = True
-
-                self.wait(T*7)
-
-                dots[i0]._on = False
-                self.wait(T*2)
-                dots[i1]._on = False
-                self.wait(T)
-                dots[i2]._on = False
-                dots[i2].update(0)
-
+            def play(*idx):
+                for i in idx:
+                    dots[i]._on = True
+                    if i==idx[0]:
+                        self.wait(T)
+                    else: 
+                        self.wait(2*T)
+                self.wait(5*T)
+                for i in idx:
+                    dots[i]._on = False
+                    if i==idx[-1]:
+                        dots[i]._on = False
+                        dots[i].update(0)
+                    elif i==idx[-2]:
+                        dots[i]._on = False
+                        self.wait(T)
+                    else:
+                        dots[i]._on = False
+                        self.wait(T*2)
             self.wait(.5)
             self.add(*geoms[::-1], *dots[::-1])
-            dots[0]._on = True
-            self.wait(T)
-            dots[0]._on = False
-            dots[1]._on = True
-            self.wait(T)
-            dots[1]._on = False
-            dots[2]._on = True
-            self.wait(T)
-            dots[2]._on = False
-            dots[2].update(0)
-
-            play(2,1,0)
+            for i in range(N):
+                I = idx[i]
+                if i==0:
+                    dots[I]._on = True
+                    self.wait(T)
+                else:
+                    dots[idx[i-1]]._on = False
+                    dots[I]._on = True
+                    self.wait(T)
+                if i==N-1:
+                    dots[I]._on = False
+                    dots[I].update(0)
+            play(*idx[::-1])
             self.remove(*geoms[::-1], *dots[::-1])
             self.wait(.5)
+
     pb = Polybeat()
-    pb.render(preview=True)
+    pb.render(preview=preview)
+
+if __name__ == '__main__':
+    play(custom_order=[0,1,3,2], sounds=['sounds/kick_drum','sounds/open_conga','sounds/side_stick','sounds/low_bongo'], preview=False)
```

### Comparing `polybeat-0.0.1/polybeat/sounds/kick_drum.wav` & `polybeat-1.0.0/polybeat/sounds/kick_drum.wav`

 * *Files identical despite different names*

### Comparing `polybeat-0.0.1/polybeat/sounds/low_bongo.wav` & `polybeat-1.0.0/polybeat/sounds/low_bongo.wav`

 * *Files identical despite different names*

### Comparing `polybeat-0.0.1/polybeat/sounds/open_conga.wav` & `polybeat-1.0.0/polybeat/sounds/open_conga.wav`

 * *Files identical despite different names*

### Comparing `polybeat-0.0.1/setup.py` & `polybeat-1.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='polybeat',
-    version='0.0.1',
-    description='Toy for polyrhythm visualization',
+    version='1.0.0',
+    description='A toy for visualizing polyrhythms',
     url='https://github.com/chunribu/polybeat/',
     author='Jian Jiang',
-    author_email='jianjiang.bio@gmail.com',
+    author_email='pccfreespace@gmail.com',
     packages=find_packages(),
     license='MIT',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_data={'polybeat': ['sounds/*.wav']},
     include_package_data=True,
     install_requires=[],
@@ -21,9 +21,9 @@
     classifiers=[
         'Operating System :: POSIX :: Linux',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows',
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
     ],
-    keywords='polybeat polyrhythm PCC',
+    keywords='polybeat polyrhythm pccfs',
 )
```

