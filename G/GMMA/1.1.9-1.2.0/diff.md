# Comparing `tmp/GMMA-1.1.9.tar.gz` & `tmp/GMMA-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GMMA-1.1.9.tar", last modified: Tue Mar 28 00:25:56 2023, max compression
+gzip compressed data, was "GMMA-1.2.0.tar", last modified: Thu Jun 15 20:08:14 2023, max compression
```

## Comparing `GMMA-1.1.9.tar` & `GMMA-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:25:56.970907 GMMA-1.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:25:56.966907 GMMA-1.1.9/GMMA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-28 00:25:56.000000 GMMA-1.1.9/GMMA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-28 00:25:56.000000 GMMA-1.1.9/GMMA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 00:25:56.000000 GMMA-1.1.9/GMMA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-28 00:25:56.000000 GMMA-1.1.9/GMMA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-28 00:25:56.000000 GMMA-1.1.9/GMMA.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-28 00:25:48.000000 GMMA-1.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-28 00:25:56.970907 GMMA-1.1.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:25:56.970907 GMMA-1.1.9/gamma/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-28 00:25:48.000000 GMMA-1.1.9/gamma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-03-28 00:25:48.000000 GMMA-1.1.9/gamma/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    37223 2023-03-28 00:25:48.000000 GMMA-1.1.9/gamma/_bayesian_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    33646 2023-03-28 00:25:48.000000 GMMA-1.1.9/gamma/_gaussian_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-03-28 00:25:48.000000 GMMA-1.1.9/gamma/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    16699 2023-03-28 00:25:48.000000 GMMA-1.1.9/gamma/seismic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-03-28 00:25:48.000000 GMMA-1.1.9/gamma/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 00:25:56.970907 GMMA-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-28 00:25:48.000000 GMMA-1.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:25:56.970907 GMMA-1.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-03-28 00:25:48.000000 GMMA-1.1.9/tests/test_seismoc_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:08:14.421778 GMMA-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:08:14.417778 GMMA-1.2.0/GMMA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-15 20:08:14.000000 GMMA-1.2.0/GMMA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-15 20:08:14.000000 GMMA-1.2.0/GMMA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 20:08:14.000000 GMMA-1.2.0/GMMA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 20:08:14.000000 GMMA-1.2.0/GMMA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 20:08:14.000000 GMMA-1.2.0/GMMA.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-15 20:08:02.000000 GMMA-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-15 20:08:14.421778 GMMA-1.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:08:14.421778 GMMA-1.2.0/gamma/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-15 20:08:02.000000 GMMA-1.2.0/gamma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19235 2023-06-15 20:08:02.000000 GMMA-1.2.0/gamma/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37223 2023-06-15 20:08:02.000000 GMMA-1.2.0/gamma/_bayesian_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33646 2023-06-15 20:08:02.000000 GMMA-1.2.0/gamma/_gaussian_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-06-15 20:08:02.000000 GMMA-1.2.0/gamma/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15603 2023-06-15 20:08:02.000000 GMMA-1.2.0/gamma/seismic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17019 2023-06-15 20:08:02.000000 GMMA-1.2.0/gamma/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 20:08:14.421778 GMMA-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-15 20:08:02.000000 GMMA-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:08:14.421778 GMMA-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-15 20:08:02.000000 GMMA-1.2.0/tests/test_seismoc_ops.py
```

### Comparing `GMMA-1.1.9/LICENSE` & `GMMA-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `GMMA-1.1.9/gamma/_base.py` & `GMMA-1.2.0/gamma/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,20 +268,22 @@
             self._print_verbose_msg_init_end(lower_bound)
 
             if lower_bound > max_lower_bound:
                 max_lower_bound = lower_bound
                 best_params = self._get_parameters()
                 best_n_iter = n_iter
 
+        # if not self.converged_:
+        #     warnings.warn('Initialization %d did not converge. '
+        #                   'Try different init parameters, '
+        #                   'or increase max_iter, tol '
+        #                   'or check for degenerate data.'
+        #                   % (init + 1), ConvergenceWarning)
         if not self.converged_:
-            warnings.warn('Initialization %d did not converge. '
-                          'Try different init parameters, '
-                          'or increase max_iter, tol '
-                          'or check for degenerate data.'
-                          % (init + 1), ConvergenceWarning)
+            print(f"\nInitialization {init + 1} did not converge.")
 
         self._set_parameters(best_params)
         self.n_iter_ = best_n_iter
         self.lower_bound_ = max_lower_bound
 
         # Always do a final e-step to guarantee that the labels returned by
         # fit_predict(X) are always consistent with fit(X).predict(X)
```

### Comparing `GMMA-1.1.9/gamma/_bayesian_mixture.py` & `GMMA-1.2.0/gamma/_bayesian_mixture.py`

 * *Files identical despite different names*

### Comparing `GMMA-1.1.9/gamma/_gaussian_mixture.py` & `GMMA-1.2.0/gamma/_gaussian_mixture.py`

 * *Files identical despite different names*

### Comparing `GMMA-1.1.9/gamma/app.py` & `GMMA-1.2.0/gamma/app.py`

 * *Files identical despite different names*

### Comparing `GMMA-1.1.9/gamma/seismic_ops.py` & `GMMA-1.2.0/gamma/seismic_ops.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,107 +1,138 @@
 import itertools
 import numpy as np
 import scipy.optimize
-try:
-    import torch
-    import torch.nn.functional as F
-    import torch.optim
-except:
-    pass
-
+import shelve
+from pathlib import Path
+from numba import njit
+from numba.typed import List
+import time
 
 ###################################### Eikonal Solver ######################################
 # |\nabla u| = f
 # ((u - a1)^+)^2 + ((u - a2)^+)^2 + ((u - a3)^+)^2 = f^2 h^2
 
 
+@njit
 def calculate_unique_solution(a, b, f, h):
     d = abs(a - b)
     if d >= f * h:
-        return min(a, b) + f * h
+        return min([a, b]) + f * h
     else:
         return (a + b + np.sqrt(2 * f * f * h * h - (a - b) ** 2)) / 2
 
 
+@njit
 def sweeping_over_I_J_K(u, I, J, f, h):
     m = len(I)
     n = len(J)
 
-    for i, j in itertools.product(I, J):
-        if i == 0:
-            uxmin = u[i + 1, j]
-        elif i == m - 1:
-            uxmin = u[i - 1, j]
-        else:
-            uxmin = np.min([u[i - 1, j], u[i + 1, j]])
+    # for i, j in itertools.product(I, J):
+    for i in I:
+        for j in J:
+            if i == 0:
+                uxmin = u[i + 1, j]
+            elif i == m - 1:
+                uxmin = u[i - 1, j]
+            else:
+                uxmin = min([u[i - 1, j], u[i + 1, j]])
+
+            if j == 0:
+                uymin = u[i, j + 1]
+            elif j == n - 1:
+                uymin = u[i, j - 1]
+            else:
+                uymin = min([u[i, j - 1], u[i, j + 1]])
 
-        if j == 0:
-            uymin = u[i, j + 1]
-        elif j == n - 1:
-            uymin = u[i, j - 1]
-        else:
-            uymin = np.min([u[i, j - 1], u[i, j + 1]])
+            u_new = calculate_unique_solution(uxmin, uymin, f[i, j], h)
 
-        u_new = calculate_unique_solution(uxmin, uymin, f[i, j], h)
-
-        u[i, j] = np.min([u_new, u[i, j]])
+            u[i, j] = min([u_new, u[i, j]])
 
     return u
 
 
+@njit
 def sweeping(u, v, h):
     f = 1.0 / v  ## slowness
 
     m, n = u.shape
-    I = list(range(m))
+    # I = list(range(m))
+    # I = List()
+    # [I.append(i) for i in range(m)]
+    I = np.arange(m)
     iI = I[::-1]
-    J = list(range(n))
+    # J = list(range(n))
+    # J = List()
+    # [J.append(j) for j in range(n)]
+    J = np.arange(n)
     iJ = J[::-1]
 
     u = sweeping_over_I_J_K(u, I, J, f, h)
     u = sweeping_over_I_J_K(u, iI, J, f, h)
     u = sweeping_over_I_J_K(u, iI, iJ, f, h)
     u = sweeping_over_I_J_K(u, I, iJ, f, h)
 
     return u
 
 
 def eikonal_solve(u, f, h):
     print("Eikonal Solver: ")
+    t0 = time.time()
     for i in range(50):
         u_old = np.copy(u)
         u = sweeping(u, f, h)
 
         err = np.max(np.abs(u - u_old))
-        print(f"iteration {i}, error = {err}")
+        print(f"Iter {i}, error = {err:.3f}")
         if err < 1e-6:
             break
-
+    print(f"Time: {time.time() - t0:.3f}")
     return u
 
 
 ###################################### Traveltime based on Eikonal Timetable ######################################
+@njit
+def _get_index(ir, iz, nr, nz, order="C"):
+    if order == "C":
+        return ir * nz + iz
+    elif order == "F":
+        return iz * nr + ir
+    else:
+        raise ValueError("order must be either C or F")
 
 
-def _interp(time_table, r, z, rgrid, zgrid, h):
-    ir0 = (r - rgrid[0, 0]).div(h, rounding_mode='floor').clamp(0, rgrid.shape[0] - 2).long()
-    iz0 = (z - zgrid[0, 0]).div(h, rounding_mode='floor').clamp(0, zgrid.shape[1] - 2).long()
+def test_get_index():
+    vr, vz = np.meshgrid(np.arange(10), np.arange(20), indexing="ij")
+    vr = vr.flatten()
+    vz = vz.flatten()
+    nr = 10
+    nz = 20
+    for ir in range(nr):
+        for iz in range(nz):
+            assert vr[_get_index(ir, iz, nr, nz)] == ir
+            assert vz[_get_index(ir, iz, nr, nz)] == iz
+
+
+@njit
+def _interp(time_table, r, z, rgrid0, zgrid0, nr, nz, h):
+    ir0 = np.floor((r - rgrid0) / h).clip(0, nr - 2).astype(np.int64)
+    iz0 = np.floor((z - zgrid0) / h).clip(0, nz - 2).astype(np.int64)
     ir1 = ir0 + 1
     iz1 = iz0 + 1
 
     ## https://en.wikipedia.org/wiki/Bilinear_interpolation
-    x1 = ir0 * h + rgrid[0, 0]
-    x2 = ir1 * h + rgrid[0, 0]
-    y1 = iz0 * h + zgrid[0, 0]
-    y2 = iz1 * h + zgrid[0, 0]
-
-    Q11 = time_table[ir0, iz0]
-    Q12 = time_table[ir0, iz1]
-    Q21 = time_table[ir1, iz0]
-    Q22 = time_table[ir1, iz1]
+    x1 = ir0 * h + rgrid0
+    x2 = ir1 * h + rgrid0
+    y1 = iz0 * h + zgrid0
+    y2 = iz1 * h + zgrid0
+
+    Q11 = time_table[_get_index(ir0, iz0, nr, nz)]
+    Q12 = time_table[_get_index(ir0, iz1, nr, nz)]
+    Q21 = time_table[_get_index(ir1, iz0, nr, nz)]
+    Q22 = time_table[_get_index(ir1, iz1, nr, nz)]
 
     t = (
         1
         / (x2 - x1)
         / (y2 - y1)
         * (
             Q11 * (x2 - r) * (y2 - z)
@@ -110,69 +141,77 @@
             + Q22 * (r - x1) * (z - y1)
         )
     )
 
     return t
 
 
-def traveltime(event_loc, station_loc, time_table, rgrid, zgrid, h, **kwargs):
-    r = torch.sqrt(torch.sum((event_loc[:, :2] - station_loc[:, :2]) ** 2, dim=-1, keepdims=True))
-    z = event_loc[:, 2:] - station_loc[:, 2:]
-    if (event_loc[:, 2:] < 0).any():
-        print(f"Warning: depth is defined as positive down: {event_loc[:, 2:].detach().numpy()}")
-
-    tt = _interp(time_table, r, z, rgrid, zgrid, h)
+def traveltime(event_loc, station_loc, phase_type, eikonal):
+    r = np.linalg.norm(event_loc[:, :2] - station_loc[:, :2], axis=-1, keepdims=False)
+    z = event_loc[:, 2] - station_loc[:, 2]
+
+    rgrid0 = eikonal["rgrid"][0]
+    zgrid0 = eikonal["zgrid"][0]
+    nr = eikonal["nr"]
+    nz = eikonal["nz"]
+    h = eikonal["h"]
+
+    p_index = phase_type == "p"
+    s_index = phase_type == "s"
+    tt = np.zeros(len(phase_type), dtype=np.float32)
+    tt[phase_type == "p"] = _interp(eikonal["up"], r[p_index], z[p_index], rgrid0, zgrid0, nr, nz, h)
+    tt[phase_type == "s"] = _interp(eikonal["us"], r[s_index], z[s_index], rgrid0, zgrid0, nr, nz, h)
+    tt = tt[:, np.newaxis]
 
     return tt
 
 
-##################################################################################################################
+def grad_traveltime(event_loc, station_loc, phase_type, eikonal):
+    r = np.linalg.norm(event_loc[:, :2] - station_loc[:, :2], axis=-1, keepdims=False)
+    z = event_loc[:, 2] - station_loc[:, 2]
+
+    rgrid0 = eikonal["rgrid"][0]
+    zgrid0 = eikonal["zgrid"][0]
+    nr = eikonal["nr"]
+    nz = eikonal["nz"]
+    h = eikonal["h"]
+
+    p_index = phase_type == "p"
+    s_index = phase_type == "s"
+    dt_dr = np.zeros(len(phase_type))
+    dt_dz = np.zeros(len(phase_type))
+    dt_dr[p_index] = _interp(eikonal["grad_up"][0], r[p_index], z[p_index], rgrid0, zgrid0, nr, nz, h)
+    dt_dr[s_index] = _interp(eikonal["grad_us"][0], r[s_index], z[s_index], rgrid0, zgrid0, nr, nz, h)
+    dt_dz[p_index] = _interp(eikonal["grad_up"][1], r[p_index], z[p_index], rgrid0, zgrid0, nr, nz, h)
+    dt_dz[s_index] = _interp(eikonal["grad_us"][1], r[s_index], z[s_index], rgrid0, zgrid0, nr, nz, h)
+
+    dr_dxy = (event_loc[:, :-2] - station_loc[:, :-1]) / (r[:, np.newaxis] + 1e-6)
+    dt_dxy = dt_dr[:, np.newaxis] * dr_dxy
 
+    grad = np.column_stack((dt_dxy, dt_dz[:, np.newaxis]))
+
+    return grad
 
-def calc_time(event_loc, station_loc, phase_type, vel={"p": 6.0, "s": 6.0 / 1.75}, eikonal=None, **kwargs):
 
+############################################# Seismic Ops for GaMMA #####################################################################
+
+
+def calc_time(event_loc, station_loc, phase_type, vel={"p": 6.0, "s": 6.0 / 1.75}, eikonal=None, **kwargs):
     ev_loc = event_loc[:, :-1]
     ev_t = event_loc[:, -1:]
 
     if eikonal is None:
         v = np.array([vel[x] for x in phase_type])[:, np.newaxis]
         tt = np.linalg.norm(ev_loc - station_loc, axis=-1, keepdims=True) / v + ev_t
     else:
-        ev_loc = torch.from_numpy(ev_loc).float()
-        station_locs = torch.from_numpy(station_loc).float()
-
-        tp = traveltime(
-            ev_loc,
-            station_locs[phase_type == "p"],
-            eikonal["up"],
-            eikonal["rgrid"],
-            eikonal["zgrid"],
-            eikonal["h"],
-            **kwargs,
-        )
-        ts = traveltime(
-            ev_loc,
-            station_locs[phase_type == "s"],
-            eikonal["us"],
-            eikonal["rgrid"],
-            eikonal["zgrid"],
-            eikonal["h"],
-            **kwargs,
-        )
-
-        tt = np.zeros(len(phase_type), dtype=np.float32)[:, np.newaxis]
-        tt[phase_type == "p"] = tp.numpy()
-        tt[phase_type == "s"] = ts.numpy()
-        tt = tt + ev_t
-
+        tt = traveltime(event_loc, station_loc, phase_type, eikonal) + ev_t
     return tt
 
 
 def calc_mag(data, event_loc, station_loc, weight, min=-2, max=8):
-
     dist = np.linalg.norm(event_loc[:, :-1] - station_loc, axis=-1, keepdims=True)
     # mag_ = ( data - 2.48 + 2.76 * np.log10(dist) )
     ## Picozzi et al. (2018) A rapid response magnitude scale...
     c0, c1, c2, c3 = 1.08, 0.93, -0.015, -1.68
     mag_ = (data - c0 - c3 * np.log10(np.maximum(dist, 0.1))) / c1 + 3.5
     ## Atkinson, G. M. (2015). Ground-Motion Prediction Equation...
     # c0, c1, c2, c3, c4 = (-4.151, 1.762, -0.09509, -1.669, -0.0006)
@@ -183,237 +222,162 @@
     mask = np.abs(mag_ - mu) <= 2 * std
     mag = np.sum(mag_[mask] * weight[mask]) / (np.sum(weight[mask]) + 1e-6)
     mag = np.clip(mag, min, max)
     return mag
 
 
 def calc_amp(mag, event_loc, station_loc):
-
     dist = np.linalg.norm(event_loc[:, :-1] - station_loc, axis=-1, keepdims=True)
     # logA = mag + 2.48 - 2.76 * np.log10(dist)
     ## Picozzi et al. (2018) A rapid response magnitude scale...
     c0, c1, c2, c3 = 1.08, 0.93, -0.015, -1.68
     logA = c0 + c1 * (mag - 3.5) + c3 * np.log10(np.maximum(dist, 0.1))
     ## Atkinson, G. M. (2015). Ground-Motion Prediction Equation...
     # c0, c1, c2, c3, c4 = (-4.151, 1.762, -0.09509, -1.669, -0.0006)
     # logA = c0 + c1*mag + c3*np.log10(dist)
     return logA
 
 
-## Huber loss
-def loss_and_grad(event_loc, phase_time, phase_type, station_loc, weight, vel={"p": 6.0, "s": 6.0 / 1.75}, sigma=1):
-    v = np.array([vel[p] for p in phase_type])[:, np.newaxis]
+################################################ Earthquake Location ################################################
+
+
+def huber_loss_grad(
+    event_loc, phase_time, phase_type, station_loc, weight, vel={"p": 6.0, "s": 6.0 / 1.75}, sigma=1, eikonal=None
+):
     event_loc = event_loc[np.newaxis, :]
-    dist = np.sqrt(np.sum((station_loc - event_loc[:, :-1]) ** 2, axis=1, keepdims=True))
+    predict_time = calc_time(event_loc, station_loc, phase_type, vel, eikonal)
+    t_diff = predict_time - phase_time
+
+    l1 = np.squeeze((np.abs(t_diff) > sigma))
+    l2 = np.squeeze((np.abs(t_diff) <= sigma))
+
+    # loss
+    loss = np.sum((sigma * np.abs(t_diff[l1]) - 0.5 * sigma**2) * weight[l1]) + np.sum(
+        0.5 * t_diff[l2] ** 2 * weight[l2]
+    )
     J = np.zeros([phase_time.shape[0], event_loc.shape[1]])
-    J[:, :-1] = (event_loc[:, :-1] - station_loc) / (dist + 1e-6) / v
-    J[:, -1] = 1
 
-    y = dist / v - (phase_time - event_loc[:, -1:])
+    # gradient
+    if eikonal is None:
+        v = np.array([vel[p] for p in phase_type])[:, np.newaxis]
+        dist = np.linalg.norm(event_loc[:, :-1] - station_loc, axis=-1, keepdims=True)
+        J[:, :-1] = (event_loc[:, :-1] - station_loc) / (dist + 1e-6) / v
+    else:
+        grad = grad_traveltime(event_loc, station_loc, phase_type, eikonal)
+        J[:, :-1] = grad
+    J[:, -1] = 1
 
-    # std = np.sqrt(np.sum(y**2 * weight) / (np.sum(weight)+1e-12))
-    # mask = (np.abs(y) <= 2*std)
-    # l1 = np.squeeze((np.abs(y) > sigma) & mask)
-    # l2 = np.squeeze((np.abs(y) <= sigma) & mask)
-
-    l1 = np.squeeze((np.abs(y) > sigma))
-    l2 = np.squeeze((np.abs(y) <= sigma))
-
-    loss = np.sum((sigma * np.abs(y[l1]) - 0.5 * sigma**2) * weight[l1]) + np.sum(0.5 * y[l2] ** 2 * weight[l2])
-    J_ = np.sum(sigma * np.sign(y[l1]) * J[l1] * weight[l1], axis=0, keepdims=True) + np.sum(
-        y[l2] * J[l2] * weight[l2], axis=0, keepdims=True
+    J_ = np.sum(sigma * np.sign(t_diff[l1]) * J[l1] * weight[l1], axis=0, keepdims=True) + np.sum(
+        t_diff[l2] * J[l2] * weight[l2], axis=0, keepdims=True
     )
 
     return loss, J_
 
 
-def linloc(
-    event_loc0,
+def calc_loc(
     phase_time,
     phase_type,
     station_loc,
     weight,
-    max_iter=10,
-    convergence=1e-3,
-    bounds=None,
+    event_loc0,
+    eikonal=None,
     vel={"p": 6.0, "s": 6.0 / 1.75},
+    bounds=None,
+    max_iter=100,
+    convergence=1e-6,
 ):
+    
     opt = scipy.optimize.minimize(
-        loss_and_grad,
+        huber_loss_grad,
         np.squeeze(event_loc0),
         method="L-BFGS-B",
         jac=True,
-        args=(phase_time, phase_type, station_loc, weight, vel, 1),
+        args=(phase_time, phase_type, station_loc, weight, vel, 1, eikonal),
         bounds=bounds,
         options={"maxiter": max_iter, "gtol": convergence, "iprint": -1},
     )
 
     return opt.x[np.newaxis, :], opt.fun
 
 
-def eikoloc(
-    event_loc0,
-    phase_time,
-    phase_type,
-    station_loc,
-    weight,
-    up,
-    us,
-    rgrid,
-    zgrid,
-    h,
-    bounds=None,
-    device="cpu",
-    add_eqt=False,
-    gamma=0.1,
-    max_iter=1000,
-    convergence=1e-9,
-):
-    event_loc = torch.tensor(event_loc0, dtype=torch.float32, requires_grad=True, device=device)
-    if bounds is not None:
-        bounds = torch.tensor(bounds, dtype=torch.float32, device=device)
-    p_index = torch.arange(len(phase_type), device=device)[phase_type == "p"]
-    s_index = torch.arange(len(phase_type), device=device)[phase_type == "s"]
-    time = torch.tensor(phase_time, dtype=torch.float32, device=device)
-    loc = torch.tensor(station_loc, dtype=torch.float32, device=device)
-    weight = torch.tensor(weight, dtype=torch.float32, device=device)
-    obs_p = time[p_index]
-    obs_s = time[s_index]
-    loc_p = loc[p_index]
-    loc_s = loc[s_index]
-    weight_p = weight[p_index]
-    weight_s = weight[s_index]
-
-    # %% optimization
-    optimizer = torch.optim.LBFGS(params=[event_loc], max_iter=max_iter, line_search_fn="strong_wolfe", tolerance_change=convergence)
-
-    def closure():
-        optimizer.zero_grad()
-        if bounds is not None:
-            loc0_ = torch.max(torch.min(event_loc[:, :-1], bounds[:, 1]), bounds[:, 0])
-        else:
-            loc0_ = event_loc[:, :-1]
-        loc0_ = torch.nan_to_num(loc0_, nan=0)
-        t0_ = event_loc[:, -1:]
-        if len(p_index) > 0:
-            tt_p = traveltime(loc0_, loc_p, up, rgrid, zgrid, h, sigma=1)
-            pred_p = t0_ + tt_p
-            loss_p = torch.mean(F.huber_loss(obs_p, pred_p, reduction="none") * weight_p)
-            if add_eqt:
-                dd_tt_p = tt_p.unsqueeze(-1) - tt_p.unsqueeze(-2)
-                dd_time_p = obs_p.unsqueeze(-1) - obs_p.unsqueeze(-2)
-                loss_p += gamma * torch.mean(
-                    F.huber_loss(dd_tt_p, dd_time_p, reduction="none") * weight_p.unsqueeze(-1) * weight_p.unsqueeze(-2)
-                )
-            # loss_p = F.mse_loss(time_p, tt_p)
-        else:
-            loss_p = 0
-        if len(s_index) > 0:
-            tt_s = traveltime(loc0_, loc_s, us, rgrid, zgrid, h, sigma=1)
-            pred_s = t0_ + tt_s
-            loss_s = torch.mean(F.huber_loss(obs_s, pred_s, reduction="none") * weight_s)
-            if add_eqt:
-                dd_tt_s = tt_s.unsqueeze(-1) - tt_s.unsqueeze(-2)
-                dd_time_s = obs_s.unsqueeze(-1) - obs_s.unsqueeze(-2)
-                loss_s += gamma * torch.mean(
-                    F.huber_loss(dd_tt_s, dd_time_s, reduction="none") * weight_s.unsqueeze(-1) * weight_s.unsqueeze(-2)
-                )
-            # loss_s = F.mse_loss(time_s, tt_s)
-        else:
-            loss_s = 0
-        loss = loss_p + loss_s
-        loss.backward()
-        return loss
-
-    optimizer.step(closure)
-    loss = closure().item()
-
-    event_loc = event_loc.detach().cpu()
-    if bounds is not None:
-        event_loc[:, :-1] = torch.max(torch.min(event_loc[:, :-1], bounds[:, 1]), bounds[:, 0])
-
-    return event_loc, loss
-
-
-def calc_loc(
-    phase_time,
-    phase_type,
-    station_loc,
-    weight,
-    event_loc0,
-    eikonal=None,
-    vel={"p": 6.0, "s": 6.0 / 1.75},
-    bounds=None,
-    max_iter=100,
-    convergence=1e-6,
-):
-    if eikonal is None:
-        event_loc, loss = linloc(
-            event_loc0,
-            phase_time,
-            phase_type,
-            station_loc,
-            weight,
-            vel=vel,
-            bounds=bounds,
-            max_iter=max_iter,
-            convergence=convergence,
-        )
-    else:
-        event_loc, loss = eikoloc(
-            event_loc0,
-            phase_time,
-            phase_type,
-            station_loc,
-            weight,
-            up=eikonal["up"],
-            us=eikonal["us"],
-            rgrid=eikonal["rgrid"],
-            zgrid=eikonal["zgrid"],
-            h=eikonal["h"],
-            bounds=bounds[:-1],
-            max_iter=max_iter,
-            convergence=convergence,
-        )
-
-    return event_loc, loss
-
 
 def initialize_eikonal(config):
+    path = Path("./eikonal")
+    path.mkdir(exist_ok=True)
     rlim = [0, np.sqrt((config["xlim"][1] - config["xlim"][0]) ** 2 + (config["ylim"][1] - config["ylim"][0]) ** 2)]
     zlim = config["zlim"]
     h = config["h"]
-    edge_grids = 3
 
-    rgrid = np.arange(rlim[0] - edge_grids * h, rlim[1], h)
-    zgrid = np.arange(zlim[0] - edge_grids * h, zlim[1], h)
-    m, n = len(rgrid), len(zgrid)
-
-    vel = config["vel"]
-    zz, vp, vs = vel["z"], vel["p"], vel["s"]
-    vp1d = np.interp(zgrid, zz, vp)
-    vs1d = np.interp(zgrid, zz, vs)
-    vp = np.ones((m, n)) * vp1d
-    vs = np.ones((m, n)) * vs1d
-
-    up = 1000 * np.ones((m, n))
-    up[edge_grids, edge_grids] = 0.0
-    up = eikonal_solve(up, vp, h)
-
-    us = 1000 * np.ones((m, n))
-    us[edge_grids, edge_grids] = 0.0
-    us = eikonal_solve(us, vs, h)
-
-    up = torch.tensor(up, dtype=torch.float32)
-    us = torch.tensor(us, dtype=torch.float32)
-    rgrid = torch.tensor(rgrid, dtype=torch.float32)
-    zgrid = torch.tensor(zgrid, dtype=torch.float32)
-    rgrid, zgrid = torch.meshgrid(rgrid, zgrid, indexing="ij")
+    filename = f"timetable_{rlim[0]:.0f}_{rlim[1]:.0f}_{zlim[0]:.0f}_{zlim[1]:.0f}_{h:.3f}"
+    if (path / (filename + ".dir")).is_file():
+        print("Loading precomputed timetable...")
+        with shelve.open(str(path / filename)) as db:
+            up = db["up"]
+            us = db["us"]
+            grad_up = db["grad_up"]
+            grad_us = db["grad_us"]
+            rgrid = db["rgrid"]
+            zgrid = db["zgrid"]
+            nr = db["nr"]
+            nz = db["nz"]
+            h = db["h"]
+    else:
+        edge_grids = 0
 
-    config.update({"up": up, "us": us, "rgrid": rgrid, "zgrid": zgrid, "h": h})
+        rgrid = np.arange(rlim[0] - edge_grids * h, rlim[1], h)
+        zgrid = np.arange(zlim[0] - edge_grids * h, zlim[1], h)
+        nr, nz = len(rgrid), len(zgrid)
+
+        vel = config["vel"]
+        zz, vp, vs = vel["z"], vel["p"], vel["s"]
+        vp1d = np.interp(zgrid, zz, vp)
+        vs1d = np.interp(zgrid, zz, vs)
+        vp = np.ones((nr, nz)) * vp1d
+        vs = np.ones((nr, nz)) * vs1d
+
+        up = 1000.0 * np.ones((nr, nz))
+        up[edge_grids, edge_grids] = 0.0
+        up = eikonal_solve(up, vp, h)
+
+        grad_up = np.gradient(up, h)
+
+        us = 1000.0 * np.ones((nr, nz))
+        us[edge_grids, edge_grids] = 0.0
+        us = eikonal_solve(us, vs, h)
+
+        grad_us = np.gradient(us, h)
+
+        with shelve.open(str(path / filename)) as db:
+            db["up"] = up
+            db["us"] = us
+            db["grad_up"] = grad_up
+            db["grad_us"] = grad_us
+            db["rgrid"] = rgrid
+            db["zgrid"] = zgrid
+            db["nr"] = nr
+            db["nz"] = nz
+            db["h"] = h
+
+    up = up.flatten()
+    us = us.flatten()
+    grad_up = np.array([grad_up[0].flatten(), grad_up[1].flatten()])
+    grad_us = np.array([grad_us[0].flatten(), grad_us[1].flatten()])
+    config.update(
+        {
+            "up": up,
+            "us": us,
+            "grad_up": grad_up,
+            "grad_us": grad_us,
+            "rgrid": rgrid,
+            "zgrid": zgrid,
+            "nr": nr,
+            "nz": nz,
+            "h": h,
+        }
+    )
 
     return config
 
 
 def initialize_centers(X, phase_type, centers_init, station_locs, random_state):
     n_samples, n_features = X.shape
     n_components, _ = centers_init.shape
@@ -438,24 +402,23 @@
     ## performance is ok
     # sigma = np.array([1.0,1.0])
     # prob = np.sum(1.0/sigma * np.exp( - (means - X) ** 2 / (2 * sigma**2)), axis=-1).T # (n_components, n_samples, n_features) -> (n_samples, n_components)
     # prob_sum = np.sum(prob, axis=1, keepdims=True)
     # prob_sum[prob_sum == 0] = 1.0
     # resp = prob / prob_sum
 
-    # dist = np.linalg.norm(means - X, axis=-1).T  # (n_components, n_samples, n_features) -> (n_samples, n_components)
-    # resp = np.exp(-dist)
-    # resp_sum = resp.sum(axis=1, keepdims=True)
-    # resp_sum[resp_sum == 0] = 1.0
-    # resp = resp / resp_sum
-
-    # proposed by Yaqi
-    dist = np.linalg.norm(means - X, axis=-1) # (n_components, n_samples, n_features) -> (n_components, n_samples)
-    resp = np.exp(-dist/(np.median(dist, axis=0, keepdims=True)/10.0)).T 
-    resp /= np.sum(resp, axis=1, keepdims=True) # (n_components, n_samples)
+    dist = np.linalg.norm(means - X, axis=-1).T  # (n_components, n_samples, n_features) -> (n_samples, n_components)
+    resp = np.exp(-dist)
+    resp_sum = resp.sum(axis=1, keepdims=True)
+    resp_sum[resp_sum == 0] = 1.0
+    resp = resp / resp_sum
+
+    # dist = np.linalg.norm(means - X, axis=-1) # (n_components, n_samples, n_features) -> (n_components, n_samples)
+    # resp = np.exp(-dist/np.median(dist, axis=0, keepdims=True)).T
+    # resp /= np.sum(resp, axis=1, keepdims=True) # (n_components, n_samples)
 
     if n_features == 2:
         for i in range(n_components):
             centers[i, -1:] = calc_mag(X[:, 1:2], centers_init[i : i + 1, :-1], station_locs, resp[:, i : i + 1])
 
     return resp, centers, means
```

### Comparing `GMMA-1.1.9/gamma/utils.py` & `GMMA-1.2.0/gamma/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import multiprocessing as mp
 from collections import Counter
 from datetime import datetime
+import platform
 
 import numpy as np
 import pandas as pd
 from sklearn.cluster import DBSCAN
 
 from ._bayesian_mixture import BayesianGaussianMixture
 from ._gaussian_mixture import GaussianMixture
@@ -15,15 +16,15 @@
 # to_seconds = lambda t: datetime.strptime(t, "%Y-%m-%dT%H:%M:%S.%f").timestamp()
 # from_seconds = lambda t: [datetime.utcfromtimestamp(x).strftime("%Y-%m-%dT%H:%M:%S.%f")[:-3] for x in t]
 
 
 def convert_picks_csv(picks, stations, config):
     # t = picks["timestamp"].apply(lambda x: x.timestamp()).to_numpy()
     if type(picks["timestamp"].iloc[0]) is str:
-        picks["timestamp"] = picks["timestamp"].apply(lambda x: datetime.fromisoformat(x))
+        picks.loc[:,"timestamp"] = picks["timestamp"].apply(lambda x: datetime.fromisoformat(x))
     t = (
         picks["timestamp"]
         .apply(lambda x: x.tz_convert("UTC").timestamp() if x.tzinfo is not None else x.tz_localize("UTC").timestamp())
         .to_numpy()
     )
     # t = picks["timestamp"].apply(lambda x: x.timestamp()).to_numpy()
     timestamp0 = np.min(t)
@@ -72,32 +73,38 @@
     else:
         labels = np.zeros(len(data))
         unique_labels = [0]
 
     if "ncpu" not in config:
         config["ncpu"] = max(1, min(len(unique_labels)//4, mp.cpu_count() - 1))
 
-    if len(unique_labels) == 1:
-        event_idx = 0
+    if (config["ncpu"] == 1):
         print(f"Associating {len(data)} picks with {config['ncpu']} CPUs")
-        events, assignment = associate(
-            list(unique_labels)[0],
-            labels,
-            data,
-            locs,
-            phase_type,
-            phase_weight,
-            pick_idx,
-            pick_station_id,
-            config,
-            timestamp0,
-            vel,
-            method,
-            event_idx,
-        )
+        event_idx = 0
+        events = []
+        assignment = []
+        for unique_label in list(unique_labels):
+            events_, assignment_ = associate(
+                unique_label,
+                labels,
+                data,
+                locs,
+                phase_type,
+                phase_weight,
+                pick_idx,
+                pick_station_id,
+                config,
+                timestamp0,
+                vel,
+                method,
+                event_idx,
+            )
+            event_idx += len(events_)
+            events.extend(events_)
+            assignment.extend(assignment_)
     else:
         manager = mp.Manager()
         lock = manager.Lock()
         # event_idx0 - 1 as event_idx is increased before use
         event_idx = manager.Value("i", event_idx0 - 1)
 
         print(f"Associating {len(unique_labels)} clusters with {config['ncpu']} CPUs")
@@ -105,15 +112,23 @@
         # the following sort and shuffle is to make sure jobs are distributed evenly
         counter=Counter(labels)
         unique_labels = sorted(unique_labels, key=lambda x: counter[x], reverse=True)
         np.random.shuffle(unique_labels)
 
         # the default chunk_size is len(unique_labels)//(config["ncpu"]*4), which makes some jobs very heavy
         chunk_size = max(len(unique_labels)//(config["ncpu"]*20), 1)
-        with mp.get_context('spawn').Pool(config["ncpu"]) as p:
+        
+        # Check for OS to start a child process in multiprocessing
+        # https://superfastpython.com/multiprocessing-context-in-python/
+        if platform.system().lower() in ["darwin", "windows"]:
+            context = "spawn"
+        else:
+            context = "fork"
+        
+        with mp.get_context(context).Pool(config["ncpu"]) as p:
             results = p.starmap(
                 associate,
                 [
                     [
                         k,
                         labels,
                         data,
@@ -163,21 +178,23 @@
     data_=data[labels==k]
     locs_=locs[labels==k]
     phase_type_=phase_type[labels==k]
     phase_weight_=phase_weight[labels==k]
     pick_idx_=pick_idx[labels==k]
     pick_station_id_=pick_station_id[labels==k]
 
+    max_num_event = max(Counter(pick_station_id_).values())
+
     if len(pick_idx_) < max(3, config["min_picks_per_eq"]):
         return [], []
 
     time_range = max(data_[:, 0].max() - data_[:, 0].min(), 1)
 
-    ## initialization with 5 horizontal points and N//5 time points
-    centers_init = init_centers(config, data_, locs_, time_range)
+    ## initialization with [1,1,1] horizontal points and N time points
+    centers_init = init_centers(config, data_, locs_, time_range, max_num_event)
 
     ## run clustering
     mean_precision_prior = 0.01 / time_range
     if "covariance_prior" in config:
         covariance_prior_pre = config["covariance_prior"]
     else:
         covariance_prior_pre = [5.0, 2.0]
@@ -319,59 +336,65 @@
             ),
             # "time(s)": gmm.centers_[i, len(config["dims"])],
             "magnitude": gmm.centers_[i, len(config["dims"]) + 1] if config["use_amplitude"] else 999,
             "sigma_time": np.sqrt(gmm.covariances_[i, 0, 0]),
             "sigma_amp": np.sqrt(gmm.covariances_[i, 1, 1]) if config["use_amplitude"] else 0,
             "cov_time_amp": gmm.covariances_[i, 0, 1] if config["use_amplitude"] else 0,
             "gamma_score": prob_eq[i],
-            "number_picks": len(tmp_data[idx_filter]),
-            "number_p_picks": len(tmp_data[idx_filter & (tmp_phase_type == "p")]),
-            "number_s_picks": len(tmp_data[idx_filter & (tmp_phase_type == "s")]),
+            "num_picks": len(tmp_data[idx_filter]),
+            "num_p_picks": len(tmp_data[idx_filter & (tmp_phase_type == "p")]),
+            "num_s_picks": len(tmp_data[idx_filter & (tmp_phase_type == "s")]),
             "event_index": event_idx_value,
         }
         for j, k in enumerate(config["dims"]):  ## add location
             event[k] = gmm.centers_[i, j]
         events.append(event)
 
         for pi, pr in zip(pick_idx_[pred == i][idx_filter], prob):
             assignment.append((pi, event_idx_value, pr))
 
         if (event_idx_value + 1) % 100 == 0:
-            print(f"\nFinish {event_idx_value} events")
+            print(f"\nAssociated {event_idx_value + 1} events")
     return events, assignment
 
 
-def init_centers(config, data_, locs_, time_range):
+def init_centers(config, data_, locs_, time_range, max_num_event=1):
+    """
+    max_num_event: maximum number of events at one station
+    """
+
     if "initial_points" in config:
         initial_points = config["initial_points"]
         if not isinstance(initial_points, list):
             initial_points = [initial_points, initial_points, initial_points]
     else:
         initial_points = [1, 1, 1]
 
-    if ((np.prod(initial_points) + 1) * config["oversample_factor"]) > len(data_):
+    if (np.prod(initial_points) * max_num_event * config["oversample_factor"]) > len(data_):
         initial_points = [1, 1, 1]
 
     x_init = np.linspace(config["x(km)"][0], config["x(km)"][1], initial_points[0] + 2)[1:-1]
     y_init = np.linspace(config["y(km)"][0], config["y(km)"][1], initial_points[1] + 2)[1:-1]
-    z_init = np.linspace(config["z(km)"][0], config["z(km)"][1], initial_points[2]) + 1.0
+    z_init = np.linspace(config["z(km)"][0], config["z(km)"][1], initial_points[2] + 2)[1:-1]
+    # z_init = np.linspace(config["z(km)"][0], config["z(km)"][1], initial_points[2]) + 1.0
     x_init = np.broadcast_to(x_init[:, np.newaxis, np.newaxis], initial_points).reshape(-1)
     y_init = np.broadcast_to(y_init[np.newaxis, :, np.newaxis], initial_points).reshape(-1)
     z_init = np.broadcast_to(z_init[np.newaxis, np.newaxis, :], initial_points).reshape(-1)
 
     ## I found it helpful to add a point at the center of the area
     if (initial_points[0] == 2) and (initial_points[1] == 2):
         x_init = np.append(x_init, np.mean(config["x(km)"]))
         y_init = np.append(y_init, np.mean(config["y(km)"]))
         z_init = np.append(z_init, 0)
     num_xyz_init = len(x_init)
 
-    num_sta = len(np.unique(locs_, axis=0))
-    num_t_init = max(np.round(len(data_) / num_sta / num_xyz_init * config["oversample_factor"]), 1)
-    num_t_init = min(int(num_t_init), max(len(data_) // num_xyz_init, 1))
+    # num_sta = len(np.unique(locs_, axis=0))
+    # num_t_init = max(np.round(len(data_) / num_sta / num_xyz_init * config["oversample_factor"]), 1)
+    # num_t_init = min(int(num_t_init), max(len(data_) // num_xyz_init, 1))
+    num_t_init = min(max_num_event * config["oversample_factor"], max(len(data_) // num_xyz_init, 1))
     t_init = np.sort(data_[:, 0])[:: max(len(data_) // num_t_init, 1)][:num_t_init]
     # t_init = np.linspace(
     #         data_[:, 0].min() - 0.1 * time_range,
     #         data_[:, 0].max() + 0.1 * time_range,
     #         num_t_init)
 
     x_init = np.broadcast_to(x_init[:, np.newaxis], (num_xyz_init, num_t_init)).reshape(-1)
```

### Comparing `GMMA-1.1.9/tests/test_seismoc_ops.py` & `GMMA-1.2.0/tests/test_seismoc_ops.py`

 * *Files identical despite different names*

