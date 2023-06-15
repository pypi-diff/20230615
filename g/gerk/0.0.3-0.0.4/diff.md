# Comparing `tmp/gerk-0.0.3.tar.gz` & `tmp/gerk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerk-0.0.3.tar", last modified: Thu Jun 15 20:09:11 2023, max compression
+gzip compressed data, was "gerk-0.0.4.tar", last modified: Thu Jun 15 20:33:53 2023, max compression
```

## Comparing `gerk-0.0.3.tar` & `gerk-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-15 20:09:11.646698 gerk-0.0.3/
--rw-r--r--   0 yasser     (501) staff       (20)     1093 2023-06-15 19:06:49.000000 gerk-0.0.3/LICENSE
--rw-r--r--   0 yasser     (501) staff       (20)    14902 2023-06-15 20:09:11.646016 gerk-0.0.3/PKG-INFO
--rw-r--r--   0 yasser     (501) staff       (20)    14441 2023-06-15 19:03:01.000000 gerk-0.0.3/README.md
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-15 20:09:11.641341 gerk-0.0.3/gerk/
--rw-r--r--   0 yasser     (501) staff       (20)       23 2023-06-15 20:05:46.000000 gerk-0.0.3/gerk/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)     3277 2023-01-04 23:34:49.000000 gerk-0.0.3/gerk/_gerk_error.py
--rw-r--r--   0 yasser     (501) staff       (20)    10257 2023-06-15 19:26:27.000000 gerk-0.0.3/gerk/gerk.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-15 20:09:11.645235 gerk-0.0.3/gerk.egg-info/
--rw-r--r--   0 yasser     (501) staff       (20)    14902 2023-06-15 20:09:11.000000 gerk-0.0.3/gerk.egg-info/PKG-INFO
--rw-r--r--   0 yasser     (501) staff       (20)      215 2023-06-15 20:09:11.000000 gerk-0.0.3/gerk.egg-info/SOURCES.txt
--rw-r--r--   0 yasser     (501) staff       (20)        1 2023-06-15 20:09:11.000000 gerk-0.0.3/gerk.egg-info/dependency_links.txt
--rw-r--r--   0 yasser     (501) staff       (20)       22 2023-06-15 20:09:11.000000 gerk-0.0.3/gerk.egg-info/requires.txt
--rw-r--r--   0 yasser     (501) staff       (20)        5 2023-06-15 20:09:11.000000 gerk-0.0.3/gerk.egg-info/top_level.txt
--rw-r--r--   0 yasser     (501) staff       (20)       38 2023-06-15 20:09:11.646863 gerk-0.0.3/setup.cfg
--rw-r--r--   0 yasser     (501) staff       (20)      852 2023-06-15 20:09:02.000000 gerk-0.0.3/setup.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-15 20:33:53.859611 gerk-0.0.4/
+-rw-r--r--   0 yasser     (501) staff       (20)     1093 2023-06-15 19:06:49.000000 gerk-0.0.4/LICENSE
+-rw-r--r--   0 yasser     (501) staff       (20)    15435 2023-06-15 20:33:53.858801 gerk-0.0.4/PKG-INFO
+-rw-r--r--   0 yasser     (501) staff       (20)    14974 2023-06-15 20:32:47.000000 gerk-0.0.4/README.md
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-15 20:33:53.854754 gerk-0.0.4/gerk/
+-rw-r--r--   0 yasser     (501) staff       (20)       23 2023-06-15 20:05:46.000000 gerk-0.0.4/gerk/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)     3277 2023-01-04 23:34:49.000000 gerk-0.0.4/gerk/_gerk_error.py
+-rw-r--r--   0 yasser     (501) staff       (20)    10257 2023-06-15 19:26:27.000000 gerk-0.0.4/gerk/gerk.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-15 20:33:53.858209 gerk-0.0.4/gerk.egg-info/
+-rw-r--r--   0 yasser     (501) staff       (20)    15435 2023-06-15 20:33:53.000000 gerk-0.0.4/gerk.egg-info/PKG-INFO
+-rw-r--r--   0 yasser     (501) staff       (20)      215 2023-06-15 20:33:53.000000 gerk-0.0.4/gerk.egg-info/SOURCES.txt
+-rw-r--r--   0 yasser     (501) staff       (20)        1 2023-06-15 20:33:53.000000 gerk-0.0.4/gerk.egg-info/dependency_links.txt
+-rw-r--r--   0 yasser     (501) staff       (20)       22 2023-06-15 20:33:53.000000 gerk-0.0.4/gerk.egg-info/requires.txt
+-rw-r--r--   0 yasser     (501) staff       (20)        5 2023-06-15 20:33:53.000000 gerk-0.0.4/gerk.egg-info/top_level.txt
+-rw-r--r--   0 yasser     (501) staff       (20)       38 2023-06-15 20:33:53.859776 gerk-0.0.4/setup.cfg
+-rw-r--r--   0 yasser     (501) staff       (20)      852 2023-06-15 20:33:46.000000 gerk-0.0.4/setup.py
```

### Comparing `gerk-0.0.3/LICENSE` & `gerk-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gerk-0.0.3/PKG-INFO` & `gerk-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerk
-Version: 0.0.3
+Version: 0.0.4
 Summary: Generalized Explicit Runge-Kutta
 Author: Yasser Naji
 Author-email: yfnaji@gmail.com
 Keywords: runge-kutta,runge,kutta,numerical,integration,approximation
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
@@ -40,37 +40,40 @@
 $$
 \frac{\text{d}y}{\text{d}x}=f(x,y)
 $$
 
 with a given initial condition $(x_0, y_0)$. 
 
 We define a member of the Runge-Kutta family with a *Butcher tableau*:
-
+<!-- 
 $$
   \begin{array}{c| c c c c}
     0\\
     c_2 & a_{21}\\
     c_3 & a_{31} & a_{32}\\
     \vdots & \vdots &  & \ddots\\
     c_r & a_{r1} & a_{r2} & \cdots & a_{rr-1}\\
     \hline
       & b_1 & b_2 & \cdots & b_{r-1} & b_r
   \end{array}\\ \\
-$$
+$$ -->
 
+<img width="247" alt="genrk" src="https://github.com/yfnaji/Gerk/assets/59436765/c35b7df0-0080-41bf-8f1d-04a53ad9dac5">
 
 The above tableau is often abbreviated to
 
-$$
+<!-- $$
   \begin{array}{c| c}
     c & A\\
     \hline
       & b
   \end{array}\\ \\
-$$
+$$ -->
+
+<img width="103" alt="abbrk" src="https://github.com/yfnaji/Gerk/assets/59436765/561bd4fb-d488-44cf-9246-56cb392ad66d">
 
 The Butcher tableau presents the categories of coefficients that will be used in our Runge-Kutta method.
 
 The $n^\text{th}$ evaluation of the solution will be denoted as $(x_n, y_n)$. We also define $h$ as the time step i.e. the step size from the previous approximation to the next, and therefore
 
 $$
 x_{n+1} = x_{n} + h
@@ -151,25 +154,26 @@
 \frac{\text{d}y}{\text{d}x} = y
 $$
 
 with the initial condition $(0, 1)$ and will be making approximations up to $x=5$ with 1000 time steps.
 
 The 3/8-th rule has the following Butcher tableau:
 
-$$
+<!-- $$
   \begin{array}{c| c c c}
     0\\
     1/3 & 1/3\\
     2/3 & -1/3 & 1\\
     1 & 1 & -1 & 1\\
     \hline
       & 1/8 & 3/8 & 3/8 & 1/8
   \end{array}\\ \\
-$$
+$$ -->
 
+<img width="236" alt="rk_eg" src="https://github.com/yfnaji/Gerk/assets/59436765/0105ab38-e0b3-4b97-b5d7-d3fcc1eddb2b">
 
 The $A$ lower triangular matrix in the Butcher tableau above can be implemented in the following way:
 
 ```
 A = [ 
         ["1/3"], # Remember, fractions must be passed as strings
         ["-1/3", 1],
@@ -204,14 +208,16 @@
 lambda x,y: math.exp(x)
 ```
 
 
 Now we are ready to create the `Gerk` object:
 
 ```
+import math
+
 rk_obj = Gerk(
         A=A, 
         b=b, 
         c=c, 
         initial_conditions=(0, 1), 
         time_steps=1000, 
         final=5,
@@ -332,24 +338,26 @@
 \frac{\text{d}y}{\text{d}x}=-2xy
 $$
 
 with initial conditions $(-5, 1.3887943865\times 10^{-11})$. Note that the exact solution is $y=e^{-x^2}$.
 
 Here we will use the Fehlberg RK1(2) method which has the following Butcher tableau:
 
-$$
+<!-- $$
   \begin{array}{c| c c c}
     0 \\
     1/2 & 1/2\\
     1 & 1/256 & 255/256\\
     \hline
       & 1/512 & 255/256 & 1/512\\
       & 1/512 & 255/256 & 0\\
   \end{array}\\ \\
-$$
+$$ -->
+
+<img width="252" alt="adaptrk" src="https://github.com/yfnaji/Gerk/assets/59436765/bd1e8482-0153-49b2-809e-5a9424ecccd2">
 
 We require an additional argument for the $b^*$ vector, which in `Gerk` is called `b_star`:
 
 ```
 A = [
         ["1/2"], # Remember, fractions need to be in strings
         ["1/256", "255/256"]
```

### Comparing `gerk-0.0.3/README.md` & `gerk-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -26,37 +26,40 @@
 $$
 \frac{\text{d}y}{\text{d}x}=f(x,y)
 $$
 
 with a given initial condition $(x_0, y_0)$. 
 
 We define a member of the Runge-Kutta family with a *Butcher tableau*:
-
+<!-- 
 $$
   \begin{array}{c| c c c c}
     0\\
     c_2 & a_{21}\\
     c_3 & a_{31} & a_{32}\\
     \vdots & \vdots &  & \ddots\\
     c_r & a_{r1} & a_{r2} & \cdots & a_{rr-1}\\
     \hline
       & b_1 & b_2 & \cdots & b_{r-1} & b_r
   \end{array}\\ \\
-$$
+$$ -->
 
+<img width="247" alt="genrk" src="https://github.com/yfnaji/Gerk/assets/59436765/c35b7df0-0080-41bf-8f1d-04a53ad9dac5">
 
 The above tableau is often abbreviated to
 
-$$
+<!-- $$
   \begin{array}{c| c}
     c & A\\
     \hline
       & b
   \end{array}\\ \\
-$$
+$$ -->
+
+<img width="103" alt="abbrk" src="https://github.com/yfnaji/Gerk/assets/59436765/561bd4fb-d488-44cf-9246-56cb392ad66d">
 
 The Butcher tableau presents the categories of coefficients that will be used in our Runge-Kutta method.
 
 The $n^\text{th}$ evaluation of the solution will be denoted as $(x_n, y_n)$. We also define $h$ as the time step i.e. the step size from the previous approximation to the next, and therefore
 
 $$
 x_{n+1} = x_{n} + h
@@ -137,25 +140,26 @@
 \frac{\text{d}y}{\text{d}x} = y
 $$
 
 with the initial condition $(0, 1)$ and will be making approximations up to $x=5$ with 1000 time steps.
 
 The 3/8-th rule has the following Butcher tableau:
 
-$$
+<!-- $$
   \begin{array}{c| c c c}
     0\\
     1/3 & 1/3\\
     2/3 & -1/3 & 1\\
     1 & 1 & -1 & 1\\
     \hline
       & 1/8 & 3/8 & 3/8 & 1/8
   \end{array}\\ \\
-$$
+$$ -->
 
+<img width="236" alt="rk_eg" src="https://github.com/yfnaji/Gerk/assets/59436765/0105ab38-e0b3-4b97-b5d7-d3fcc1eddb2b">
 
 The $A$ lower triangular matrix in the Butcher tableau above can be implemented in the following way:
 
 ```
 A = [ 
         ["1/3"], # Remember, fractions must be passed as strings
         ["-1/3", 1],
@@ -190,14 +194,16 @@
 lambda x,y: math.exp(x)
 ```
 
 
 Now we are ready to create the `Gerk` object:
 
 ```
+import math
+
 rk_obj = Gerk(
         A=A, 
         b=b, 
         c=c, 
         initial_conditions=(0, 1), 
         time_steps=1000, 
         final=5,
@@ -318,24 +324,26 @@
 \frac{\text{d}y}{\text{d}x}=-2xy
 $$
 
 with initial conditions $(-5, 1.3887943865\times 10^{-11})$. Note that the exact solution is $y=e^{-x^2}$.
 
 Here we will use the Fehlberg RK1(2) method which has the following Butcher tableau:
 
-$$
+<!-- $$
   \begin{array}{c| c c c}
     0 \\
     1/2 & 1/2\\
     1 & 1/256 & 255/256\\
     \hline
       & 1/512 & 255/256 & 1/512\\
       & 1/512 & 255/256 & 0\\
   \end{array}\\ \\
-$$
+$$ -->
+
+<img width="252" alt="adaptrk" src="https://github.com/yfnaji/Gerk/assets/59436765/bd1e8482-0153-49b2-809e-5a9424ecccd2">
 
 We require an additional argument for the $b^*$ vector, which in `Gerk` is called `b_star`:
 
 ```
 A = [
         ["1/2"], # Remember, fractions need to be in strings
         ["1/256", "255/256"]
```

### Comparing `gerk-0.0.3/gerk/_gerk_error.py` & `gerk-0.0.4/gerk/_gerk_error.py`

 * *Files identical despite different names*

### Comparing `gerk-0.0.3/gerk/gerk.py` & `gerk-0.0.4/gerk/gerk.py`

 * *Files identical despite different names*

### Comparing `gerk-0.0.3/gerk.egg-info/PKG-INFO` & `gerk-0.0.4/gerk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerk
-Version: 0.0.3
+Version: 0.0.4
 Summary: Generalized Explicit Runge-Kutta
 Author: Yasser Naji
 Author-email: yfnaji@gmail.com
 Keywords: runge-kutta,runge,kutta,numerical,integration,approximation
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
@@ -40,37 +40,40 @@
 $$
 \frac{\text{d}y}{\text{d}x}=f(x,y)
 $$
 
 with a given initial condition $(x_0, y_0)$. 
 
 We define a member of the Runge-Kutta family with a *Butcher tableau*:
-
+<!-- 
 $$
   \begin{array}{c| c c c c}
     0\\
     c_2 & a_{21}\\
     c_3 & a_{31} & a_{32}\\
     \vdots & \vdots &  & \ddots\\
     c_r & a_{r1} & a_{r2} & \cdots & a_{rr-1}\\
     \hline
       & b_1 & b_2 & \cdots & b_{r-1} & b_r
   \end{array}\\ \\
-$$
+$$ -->
 
+<img width="247" alt="genrk" src="https://github.com/yfnaji/Gerk/assets/59436765/c35b7df0-0080-41bf-8f1d-04a53ad9dac5">
 
 The above tableau is often abbreviated to
 
-$$
+<!-- $$
   \begin{array}{c| c}
     c & A\\
     \hline
       & b
   \end{array}\\ \\
-$$
+$$ -->
+
+<img width="103" alt="abbrk" src="https://github.com/yfnaji/Gerk/assets/59436765/561bd4fb-d488-44cf-9246-56cb392ad66d">
 
 The Butcher tableau presents the categories of coefficients that will be used in our Runge-Kutta method.
 
 The $n^\text{th}$ evaluation of the solution will be denoted as $(x_n, y_n)$. We also define $h$ as the time step i.e. the step size from the previous approximation to the next, and therefore
 
 $$
 x_{n+1} = x_{n} + h
@@ -151,25 +154,26 @@
 \frac{\text{d}y}{\text{d}x} = y
 $$
 
 with the initial condition $(0, 1)$ and will be making approximations up to $x=5$ with 1000 time steps.
 
 The 3/8-th rule has the following Butcher tableau:
 
-$$
+<!-- $$
   \begin{array}{c| c c c}
     0\\
     1/3 & 1/3\\
     2/3 & -1/3 & 1\\
     1 & 1 & -1 & 1\\
     \hline
       & 1/8 & 3/8 & 3/8 & 1/8
   \end{array}\\ \\
-$$
+$$ -->
 
+<img width="236" alt="rk_eg" src="https://github.com/yfnaji/Gerk/assets/59436765/0105ab38-e0b3-4b97-b5d7-d3fcc1eddb2b">
 
 The $A$ lower triangular matrix in the Butcher tableau above can be implemented in the following way:
 
 ```
 A = [ 
         ["1/3"], # Remember, fractions must be passed as strings
         ["-1/3", 1],
@@ -204,14 +208,16 @@
 lambda x,y: math.exp(x)
 ```
 
 
 Now we are ready to create the `Gerk` object:
 
 ```
+import math
+
 rk_obj = Gerk(
         A=A, 
         b=b, 
         c=c, 
         initial_conditions=(0, 1), 
         time_steps=1000, 
         final=5,
@@ -332,24 +338,26 @@
 \frac{\text{d}y}{\text{d}x}=-2xy
 $$
 
 with initial conditions $(-5, 1.3887943865\times 10^{-11})$. Note that the exact solution is $y=e^{-x^2}$.
 
 Here we will use the Fehlberg RK1(2) method which has the following Butcher tableau:
 
-$$
+<!-- $$
   \begin{array}{c| c c c}
     0 \\
     1/2 & 1/2\\
     1 & 1/256 & 255/256\\
     \hline
       & 1/512 & 255/256 & 1/512\\
       & 1/512 & 255/256 & 0\\
   \end{array}\\ \\
-$$
+$$ -->
+
+<img width="252" alt="adaptrk" src="https://github.com/yfnaji/Gerk/assets/59436765/bd1e8482-0153-49b2-809e-5a9424ecccd2">
 
 We require an additional argument for the $b^*$ vector, which in `Gerk` is called `b_star`:
 
 ```
 A = [
         ["1/2"], # Remember, fractions need to be in strings
         ["1/256", "255/256"]
```

### Comparing `gerk-0.0.3/setup.py` & `gerk-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 DESCRIPTION = "Generalized Explicit Runge-Kutta"
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="gerk",
```

