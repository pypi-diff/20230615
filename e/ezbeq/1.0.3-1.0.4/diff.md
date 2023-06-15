# Comparing `tmp/ezbeq-1.0.3.tar.gz` & `tmp/ezbeq-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezbeq-1.0.3.tar", max compression
+gzip compressed data, was "ezbeq-1.0.4.tar", max compression
```

## Comparing `ezbeq-1.0.3.tar` & `ezbeq-1.0.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1066 2023-06-14 07:08:40.362351 ezbeq-1.0.3/LICENSE
--rw-r--r--   0        0        0    11494 2023-06-14 07:08:40.362351 ezbeq-1.0.3/README.md
--rw-r--r--   0        0        0        6 2023-06-14 07:10:34.445586 ezbeq-1.0.3/ezbeq/VERSION
--rw-r--r--   0        0        0        0 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/__init__.py
--rw-r--r--   0        0        0       57 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/__init__.py
--rw-r--r--   0        0        0      569 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/audiotypes.py
--rw-r--r--   0        0        0      510 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/authors.py
--rw-r--r--   0        0        0     1572 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/catalogue.py
--rw-r--r--   0        0        0      526 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/contenttypes.py
--rw-r--r--   0        0        0    26001 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/devices.py
--rw-r--r--   0        0        0      518 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/languages.py
--rw-r--r--   0        0        0      686 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/meta.py
--rw-r--r--   0        0        0     2439 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/search.py
--rw-r--r--   0        0        0      346 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/version.py
--rw-r--r--   0        0        0     6514 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/ws.py
--rw-r--r--   0        0        0      516 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/apis/years.py
--rw-r--r--   0        0        0    27881 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/camilladsp.py
--rw-r--r--   0        0        0    12896 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/catalogue.py
--rw-r--r--   0        0        0     8752 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/config.py
--rw-r--r--   0        0        0     8573 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/device.py
--rw-r--r--   0        0        0    12197 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/htp1.py
--rw-r--r--   0        0        0     4483 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/iir.py
--rw-r--r--   0        0        0    22779 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/jriver.py
--rw-r--r--   0        0        0     7014 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/main.py
--rw-r--r--   0        0        0    40966 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/minidsp.py
--rw-r--r--   0        0        0     8309 2023-06-14 07:08:40.406354 ezbeq-1.0.3/ezbeq/qsys.py
--rw-r--r--   0        0        0     4303 2023-06-14 07:10:33.033487 ezbeq-1.0.3/ezbeq/ui/android-chrome-192x192.png
--rw-r--r--   0        0        0    14091 2023-06-14 07:10:33.033487 ezbeq-1.0.3/ezbeq/ui/android-chrome-512x512.png
--rw-r--r--   0        0        0     3262 2023-06-14 07:10:33.033487 ezbeq-1.0.3/ezbeq/ui/apple-touch-icon.png
--rw-r--r--   0        0        0   852111 2023-06-14 07:10:33.973553 ezbeq-1.0.3/ezbeq/ui/assets/index-83ab9065.js
--rw-r--r--   0        0        0     5721 2023-06-14 07:10:33.973553 ezbeq-1.0.3/ezbeq/ui/assets/index-fce6f16f.css
--rw-r--r--   0        0        0    65456 2023-06-14 07:10:33.973553 ezbeq-1.0.3/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff
--rw-r--r--   0        0        0     9628 2023-06-14 07:10:33.973553 ezbeq-1.0.3/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2
--rw-r--r--   0        0        0    15344 2023-06-14 07:10:33.973553 ezbeq-1.0.3/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2
--rw-r--r--   0        0        0     7112 2023-06-14 07:10:33.973553 ezbeq-1.0.3/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2
--rw-r--r--   0        0        0    15744 2023-06-14 07:10:33.973553 ezbeq-1.0.3/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2
--rw-r--r--   0        0        0    11872 2023-06-14 07:10:33.973553 ezbeq-1.0.3/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2
--rw-r--r--   0        0        0     5560 2023-06-14 07:10:33.973553 ezbeq-1.0.3/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2
--rw-r--r--   0        0        0      246 2023-06-14 07:10:33.033487 ezbeq-1.0.3/ezbeq/ui/browserconfig.xml
--rw-r--r--   0        0        0      702 2023-06-14 07:10:33.033487 ezbeq-1.0.3/ezbeq/ui/favicon-16x16.png
--rw-r--r--   0        0        0     1310 2023-06-14 07:10:33.033487 ezbeq-1.0.3/ezbeq/ui/favicon-32x32.png
--rw-r--r--   0        0        0     7406 2023-06-14 07:10:33.037488 ezbeq-1.0.3/ezbeq/ui/favicon.ico
--rw-r--r--   0        0        0     1012 2023-06-14 07:10:33.973553 ezbeq-1.0.3/ezbeq/ui/index.html
--rw-r--r--   0        0        0     2533 2023-06-14 07:10:33.037488 ezbeq-1.0.3/ezbeq/ui/mstile-150x150.png
--rw-r--r--   0        0        0       67 2023-06-14 07:10:33.037488 ezbeq-1.0.3/ezbeq/ui/robots.txt
--rw-r--r--   0        0        0     3278 2023-06-14 07:10:33.037488 ezbeq-1.0.3/ezbeq/ui/safari-pinned-tab.svg
--rw-r--r--   0        0        0      436 2023-06-14 07:10:33.037488 ezbeq-1.0.3/ezbeq/ui/site.webmanifest
--rw-r--r--   0        0        0     1312 2023-06-14 07:08:40.410354 ezbeq-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    12528 1970-01-01 00:00:00.000000 ezbeq-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-15 20:17:31.228461 ezbeq-1.0.4/LICENSE
+-rw-r--r--   0        0        0    11494 2023-06-15 20:17:31.228461 ezbeq-1.0.4/README.md
+-rw-r--r--   0        0        0        6 2023-06-15 20:19:17.685068 ezbeq-1.0.4/ezbeq/VERSION
+-rw-r--r--   0        0        0        0 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/__init__.py
+-rw-r--r--   0        0        0       57 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/apis/__init__.py
+-rw-r--r--   0        0        0      569 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/apis/audiotypes.py
+-rw-r--r--   0        0        0      510 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/apis/authors.py
+-rw-r--r--   0        0        0     1572 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/apis/catalogue.py
+-rw-r--r--   0        0        0      526 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/apis/contenttypes.py
+-rw-r--r--   0        0        0    26001 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/apis/devices.py
+-rw-r--r--   0        0        0      518 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/apis/languages.py
+-rw-r--r--   0        0        0      686 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/apis/meta.py
+-rw-r--r--   0        0        0     2439 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/apis/search.py
+-rw-r--r--   0        0        0      346 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/apis/version.py
+-rw-r--r--   0        0        0     6514 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/apis/ws.py
+-rw-r--r--   0        0        0      516 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/apis/years.py
+-rw-r--r--   0        0        0    27881 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/camilladsp.py
+-rw-r--r--   0        0        0    12896 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/catalogue.py
+-rw-r--r--   0        0        0     8752 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/config.py
+-rw-r--r--   0        0        0     8573 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/device.py
+-rw-r--r--   0        0        0    12197 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/htp1.py
+-rw-r--r--   0        0        0     4483 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/iir.py
+-rw-r--r--   0        0        0    22779 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/jriver.py
+-rw-r--r--   0        0        0     7014 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/main.py
+-rw-r--r--   0        0        0    40966 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/minidsp.py
+-rw-r--r--   0        0        0     8309 2023-06-15 20:17:31.260461 ezbeq-1.0.4/ezbeq/qsys.py
+-rw-r--r--   0        0        0     4303 2023-06-15 20:19:14.781051 ezbeq-1.0.4/ezbeq/ui/android-chrome-192x192.png
+-rw-r--r--   0        0        0    14091 2023-06-15 20:19:14.781051 ezbeq-1.0.4/ezbeq/ui/android-chrome-512x512.png
+-rw-r--r--   0        0        0     3262 2023-06-15 20:19:14.781051 ezbeq-1.0.4/ezbeq/ui/apple-touch-icon.png
+-rw-r--r--   0        0        0   852194 2023-06-15 20:19:15.573056 ezbeq-1.0.4/ezbeq/ui/assets/index-7427ed0a.js
+-rw-r--r--   0        0        0     5721 2023-06-15 20:19:15.573056 ezbeq-1.0.4/ezbeq/ui/assets/index-fce6f16f.css
+-rw-r--r--   0        0        0    65456 2023-06-15 20:19:15.573056 ezbeq-1.0.4/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff
+-rw-r--r--   0        0        0     9628 2023-06-15 20:19:15.573056 ezbeq-1.0.4/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2
+-rw-r--r--   0        0        0    15344 2023-06-15 20:19:15.569056 ezbeq-1.0.4/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2
+-rw-r--r--   0        0        0     7112 2023-06-15 20:19:15.573056 ezbeq-1.0.4/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2
+-rw-r--r--   0        0        0    15744 2023-06-15 20:19:15.573056 ezbeq-1.0.4/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2
+-rw-r--r--   0        0        0    11872 2023-06-15 20:19:15.573056 ezbeq-1.0.4/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2
+-rw-r--r--   0        0        0     5560 2023-06-15 20:19:15.573056 ezbeq-1.0.4/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2
+-rw-r--r--   0        0        0      246 2023-06-15 20:19:14.781051 ezbeq-1.0.4/ezbeq/ui/browserconfig.xml
+-rw-r--r--   0        0        0      702 2023-06-15 20:19:14.781051 ezbeq-1.0.4/ezbeq/ui/favicon-16x16.png
+-rw-r--r--   0        0        0     1310 2023-06-15 20:19:14.781051 ezbeq-1.0.4/ezbeq/ui/favicon-32x32.png
+-rw-r--r--   0        0        0     7406 2023-06-15 20:19:14.781051 ezbeq-1.0.4/ezbeq/ui/favicon.ico
+-rw-r--r--   0        0        0     1012 2023-06-15 20:19:15.573056 ezbeq-1.0.4/ezbeq/ui/index.html
+-rw-r--r--   0        0        0     2533 2023-06-15 20:19:14.781051 ezbeq-1.0.4/ezbeq/ui/mstile-150x150.png
+-rw-r--r--   0        0        0       67 2023-06-15 20:19:14.781051 ezbeq-1.0.4/ezbeq/ui/robots.txt
+-rw-r--r--   0        0        0     3278 2023-06-15 20:19:14.781051 ezbeq-1.0.4/ezbeq/ui/safari-pinned-tab.svg
+-rw-r--r--   0        0        0      436 2023-06-15 20:19:14.781051 ezbeq-1.0.4/ezbeq/ui/site.webmanifest
+-rw-r--r--   0        0        0     1312 2023-06-15 20:17:31.260461 ezbeq-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    12528 1970-01-01 00:00:00.000000 ezbeq-1.0.4/PKG-INFO
```

### Comparing `ezbeq-1.0.3/LICENSE` & `ezbeq-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/README.md` & `ezbeq-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/apis/audiotypes.py` & `ezbeq-1.0.4/ezbeq/apis/audiotypes.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/apis/catalogue.py` & `ezbeq-1.0.4/ezbeq/apis/catalogue.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/apis/contenttypes.py` & `ezbeq-1.0.4/ezbeq/apis/contenttypes.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/apis/devices.py` & `ezbeq-1.0.4/ezbeq/apis/devices.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/apis/languages.py` & `ezbeq-1.0.4/ezbeq/apis/languages.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/apis/meta.py` & `ezbeq-1.0.4/ezbeq/apis/meta.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/apis/search.py` & `ezbeq-1.0.4/ezbeq/apis/search.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/apis/ws.py` & `ezbeq-1.0.4/ezbeq/apis/ws.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/apis/years.py` & `ezbeq-1.0.4/ezbeq/apis/years.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/camilladsp.py` & `ezbeq-1.0.4/ezbeq/camilladsp.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/catalogue.py` & `ezbeq-1.0.4/ezbeq/catalogue.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/config.py` & `ezbeq-1.0.4/ezbeq/config.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/device.py` & `ezbeq-1.0.4/ezbeq/device.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/htp1.py` & `ezbeq-1.0.4/ezbeq/htp1.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/iir.py` & `ezbeq-1.0.4/ezbeq/iir.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/jriver.py` & `ezbeq-1.0.4/ezbeq/jriver.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/main.py` & `ezbeq-1.0.4/ezbeq/main.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/minidsp.py` & `ezbeq-1.0.4/ezbeq/minidsp.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/qsys.py` & `ezbeq-1.0.4/ezbeq/qsys.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/ui/android-chrome-192x192.png` & `ezbeq-1.0.4/ezbeq/ui/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/ui/android-chrome-512x512.png` & `ezbeq-1.0.4/ezbeq/ui/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/ui/apple-touch-icon.png` & `ezbeq-1.0.4/ezbeq/ui/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/ui/assets/index-83ab9065.js` & `ezbeq-1.0.4/ezbeq/ui/assets/index-7427ed0a.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -25191,16 +25191,16 @@
     }), "SettingsApplications");
 ME = ub.default = q9;
 const tS = nt(w.jsx("path", {
         d: "M9 16.17 4.83 12l-1.42 1.41L9 19 21 7l-1.41-1.41z"
     }), "Check"),
     cb = ({
         availableDevices: e,
-        setSelectedDevice: t,
-        selectedDevice: n,
+        setSelectedDeviceName: t,
+        selectedDeviceName: n,
         selectedNav: r,
         setSelectedNav: o,
         children: l
     }) => {
         const s = "mobile-menu",
             [i, a] = zr.useState(null),
             u = !!i,
@@ -25215,15 +25215,15 @@
             g = k => {
                 h(k.currentTarget)
             },
             x = () => {
                 h(null)
             },
             b = ["Catalogue"];
-        n && (n.type === "minidsp" || n.type === "camilladsp") && b.push("Levels"), n && n.type === "minidsp" && b.push("Control");
+        n && e && (e[n].type === "minidsp" || e[n].type === "camilladsp") && b.push("Levels"), n && e && e[n].type === "minidsp" && b.push("Control");
         const y = {
                 Catalogue: w.jsx(RE, {}),
                 Levels: w.jsx(EE, {}),
                 Control: w.jsx(ME, {})
             },
             C = b.map(k => w.jsxs(Gn, {
                 onClick: O => o(k.toLowerCase()),
@@ -25232,19 +25232,19 @@
                 }) : null, w.jsx(ls, {
                     inset: r !== k.toLowerCase(),
                     children: k
                 }), y[k]]
             }, k)),
             S = e && Object.keys(e).length > 1 ? Object.keys(e).map(k => w.jsxs(Gn, {
                 value: k,
-                onClick: O => t(e[k]),
-                children: [n && k === n.name ? w.jsx(os, {
+                onClick: O => t(e[k].name),
+                children: [n && k === n ? w.jsx(os, {
                     children: w.jsx(tS, {})
                 }) : null, w.jsx(ls, {
-                    inset: !n || k !== n.name,
+                    inset: !n || k !== n,
                     children: k
                 })]
             }, k)) : null,
             I = w.jsxs(Xv, {
                 id: s,
                 anchorEl: i,
                 anchorOrigin: {
@@ -25298,15 +25298,15 @@
                 },
                 anchorOrigin: {
                     horizontal: "right",
                     vertical: "bottom"
                 },
                 children: [C, S ? w.jsx(Qv, {}) : null, S]
             }),
-            P = e.length > 1 || b.length > 1;
+            P = e && Object.keys(e).length > 1 || b.length > 1;
         return w.jsxs(Vl, {
             sx: {
                 flexGrow: 1
             },
             children: [w.jsx(M3, {
                 position: "static",
                 sx: {
@@ -37392,75 +37392,75 @@
         } else return null
     },
     qZ = ({
         entries: e,
         availableDevices: t,
         setErr: n,
         replaceDevice: r,
-        selectedDevice: o,
-        setSelectedDevice: l,
+        selectedDeviceName: o,
+        setSelectedDeviceName: l,
         selectedSlotId: s,
         setSelectedSlotId: i,
         useWide: a,
         setSelectedNav: u,
         selectedNav: c
     }) => {
         const [p, f] = Qu("selectedAuthors", []), [h, m] = d.useState([]), [g, x] = d.useState([]), [b, y] = d.useState([]), [C, S] = d.useState([]), [I, $] = d.useState([]), [P, k] = d.useState(""), [O, _] = d.useState(!1), [R, F] = d.useState(-1), [z, E] = d.useState(!1), [T, N] = d.useState([]), D = () => {
             _(H => !H)
         };
         d.useEffect(() => {
             if (t) {
                 const H = Object.keys(t);
-                H.length > 0 && !o && l(t[H[0]])
+                H.length > 0 && !o && l(H[0])
             }
         }, [t, o, l]), d.useEffect(() => {
             const H = W => {
                     const X = P.toLowerCase();
                     return !!(W.formattedTitle.toLowerCase().includes(X) || W.hasOwnProperty("altTitle") && W.altTitle.toLowerCase().includes(X) || W.hasOwnProperty("collection") && W.collection.toLowerCase().includes(X))
                 },
                 Y = W => !!((!p.length || p.indexOf(W.author) > -1) && (!g.length || g.indexOf(W.year) > -1) && (!b.length || W.audioTypes.some(X => b.indexOf(X) > -1)) && (!C.length || C.indexOf(W.contentType) > -1) && (!I.length || I.indexOf(W.freshness) > -1) && (!h.length || h.indexOf(W.language) > -1) && (!P || H(W)));
             br(N, () => e.filter(Y), n)
         }, [e, b, g, p, C, I, h, P, n]), d.useEffect(() => {
-            const H = o;
+            const H = t[o];
             if (H && z && H.hasOwnProperty("slots")) {
                 const Y = H.slots.find(W => W.id === s);
                 Y && Y.last && Y.last !== "ERROR" && Y.last !== "Empty" && k(Y.last)
             }
-        }, [o, s, k, z]);
+        }, [t, o, s, k, z]);
         const A = w.jsx(kW, {
-                selectedDevice: o,
+                selectedDevice: t[o],
                 selectedEntryId: R,
                 selectedSlotId: s,
                 useWide: a,
                 setSelectedSlotId: i,
                 setUserDriven: E,
                 setDevice: H => r(H),
                 setError: n
             }),
             L = w.jsx(EZ, {
                 entries: T,
                 setSelectedEntryId: F,
                 selectedEntryId: R,
                 useWide: a,
-                selectedDevice: o
+                selectedDevice: t[o]
             }),
             B = w.jsx(DZ, {
-                selectedDevice: o,
+                selectedDevice: t[o],
                 selectedEntry: R ? e.find(H => H.id === R) : null,
                 useWide: a,
                 setDevice: H => r(H),
                 selectedSlotId: s,
                 setError: n
             }),
             U = w.jsx(KZ, {});
         return w.jsxs(w.Fragment, {
             children: [w.jsx(cb, {
                 availableDevices: t,
-                setSelectedDevice: l,
-                selectedDevice: o,
+                setSelectedDeviceName: l,
+                selectedDeviceName: o,
                 selectedNav: c,
                 setSelectedNav: u,
                 children: w.jsx(UZ, {
                     txtFilter: P,
                     setTxtFilter: k,
                     showFilters: O,
                     toggleShowFilters: D
@@ -42504,16 +42504,16 @@
         options: e,
         data: [],
         onCreate: r => t.setChart(r),
         onDelete: r => t.setChart(null)
     })),
     _ge = ({
         availableDevices: e,
-        selectedDevice: t,
-        setSelectedDevice: n,
+        selectedDeviceName: t,
+        setSelectedDeviceName: n,
         levelsService: r,
         setSelectedNav: o,
         selectedNav: l,
         theme: s
     }) => {
         const [i, a] = d.useState(60), [u, c] = d.useState(!1), [p, f] = Qu("chartDuration", 60), h = d.useMemo(() => kpe.debounce(x => {
             a(x)
@@ -42562,16 +42562,16 @@
         const g = Object.assign({}, m, {
             width: window.innerWidth - 16,
             height: window.innerHeight - 233
         });
         return w.jsxs(w.Fragment, {
             children: [w.jsx(cb, {
                 availableDevices: e,
-                setSelectedDevice: n,
-                selectedDevice: t,
+                setSelectedDeviceName: n,
+                selectedDeviceName: t,
                 selectedNav: l,
                 setSelectedNav: o
             }), w.jsx(QZ, {
                 duration: p,
                 setDuration: f,
                 paused: u,
                 setPaused: c
@@ -42654,57 +42654,57 @@
                     children: a
                 }, `${e}-${a}`))
             })]
         })
     },
     Lge = ({
         availableDevices: e,
-        setSelectedDevice: t,
-        selectedDevice: n,
+        setSelectedDeviceName: t,
+        selectedDeviceName: n,
         selectedSlotId: r,
         setErr: o,
         setSelectedNav: l,
         selectedNav: s,
         theme: i
     }) => {
         const a = uT(),
-            [u, c] = Qu(`minidspInputs.${n.name}.${r}`, []),
-            [p, f] = Qu(`minidspOutputs.${n.name}.${r}`, []),
-            [h, m] = Qu(`minidsp.${n.name}.commandType`, "bq"),
+            [u, c] = Qu(`minidspInputs.${n}.${r}`, []),
+            [p, f] = Qu(`minidspOutputs.${n}.${r}`, []),
+            [h, m] = Qu(`minidsp.${n}.commandType`, "bq"),
             [g, x] = d.useState(r),
             [b, y] = d.useState(""),
             [C, S] = d.useState(!0),
             [I, $] = d.useState(!1),
             [P, k] = d.useState([]),
             [O, _] = d.useState([]),
             R = async () => {
                 $(!0);
                 try {
-                    const F = await cr.sendTextCommands(n.name, g, u, p, h, b, C);
+                    const F = await cr.sendTextCommands(n, g, u, p, h, b, C);
                     console.debug(F)
                 } catch (F) {
                     o(F)
                 } finally {
                     $(!1)
                 }
             };
         return d.useEffect(() => {
             if (e && n && r) {
-                const F = e[n.name].slots.find(z => z.id === r);
+                const F = e[n].slots.find(z => z.id === r);
                 k(Array.from(Array(F.inputs).keys()).map(z => z + 1)), _(Array.from(Array(F.outputs).keys()).map(z => z + 1))
             }
         }, [e, n, r]), d.useEffect(() => {
             u.some(F => !P.includes(F)) && c(u.filter(F => P.includes(F)))
         }, [c, P, u]), d.useEffect(() => {
             p.some(F => !O.includes(F)) && f(p.filter(F => O.includes(F)))
         }, [f, O, p]), w.jsxs(w.Fragment, {
             children: [w.jsx(cb, {
                 availableDevices: e,
-                setSelectedDevice: t,
-                selectedDevice: n,
+                setSelectedDeviceName: t,
+                selectedDeviceName: n,
                 selectedNav: s,
                 setSelectedNav: l
             }), w.jsx("form", {
                 className: a.root,
                 noValidate: !0,
                 autoComplete: "off",
                 children: w.jsxs(Tt, {
@@ -42902,15 +42902,15 @@
                             i.payload && i.payload.length > 0 ? i.payload = s.map((a, u) => u === 0 ? [...i.payload[u], a - i.first] : [...i.payload[u], a]) : (i.first = s[0], i.payload = s.map((a, u) => u === 0 ? [a - i.first] : [a])), this.dataByDeviceName[o] = this.trimToDuration(i, this.activeDuration), this.chart && o === this.activeDeviceName && (this.ensureAllSeriesAreLoadedToChart(o), this.paused || this.chart.setData(this.dataByDeviceName[o].payload))
                         } else console.warn(`No cached data for ${o}`)
                     } else this.setErr(new Error(`Unexpected data ${r}`))
                 }
             })
         });
         gt(this, "setActiveDevice", t => {
-            t && (this.devices.indexOf(t.name) > -1 ? this.activeDeviceName = t.name : this.setErr(new Error(`Unknown device ${t.name}`)))
+            t && (this.devices.indexOf(t) > -1 ? this.activeDeviceName = t : this.setErr(new Error(`Unknown device ${t}`)))
         });
         gt(this, "trimToDuration", (t, n) => {
             const r = t.payload[0],
                 o = r[0],
                 s = r[r.length - 1] - n;
             if (s > o) {
                 const i = r.findIndex(a => a >= s);
@@ -43000,16 +43000,16 @@
         d.useEffect(() => {
             br(l, cr.load, r)
         }, []), d.useEffect(() => {
             g.loadDevices(Object.keys(c))
         }, [g, c]), d.useEffect(() => {
             br(p, cr.getDevices, r)
         }, []), d.useEffect(() => {
-            if (s && s.hasOwnProperty("slots")) {
-                const b = s.slots.find(y => y.active === !0);
+            if (s && c[s].hasOwnProperty("slots")) {
+                const b = c[s].slots.find(y => y.active === !0);
                 b && h(b.id)
             }
         }, [s, c]);
         const x = AC("(orientation: landscape) and (min-height: 580px)");
         return w.jsx(OO, {
             injectFirst: !0,
             children: w.jsxs(GF, {
@@ -43021,33 +43021,33 @@
                     }), a === "catalogue" ? w.jsx(qZ, {
                         entries: o,
                         setErr: r,
                         replaceDevice: b => {
                             Om && Om.isConnected() ? console.debug("Discarding update, ws is connected") : (console.debug("Accepting update, ws is disconnected"), m(b))
                         },
                         availableDevices: c,
-                        selectedDevice: s,
-                        setSelectedDevice: i,
+                        selectedDeviceName: s,
+                        setSelectedDeviceName: i,
                         selectedSlotId: f,
                         setSelectedSlotId: h,
                         useWide: x,
                         selectedNav: a,
                         setSelectedNav: u
                     }) : a === "levels" ? w.jsx(_ge, {
                         availableDevices: c,
-                        selectedDevice: s,
-                        setSelectedDevice: i,
+                        selectedDeviceName: s,
+                        setSelectedDeviceName: i,
                         levelsService: g,
                         selectedNav: a,
                         setSelectedNav: u,
                         theme: t
                     }) : w.jsx(Lge, {
                         availableDevices: c,
-                        selectedDevice: s,
-                        setSelectedDevice: i,
+                        selectedDeviceName: s,
+                        setSelectedDeviceName: i,
                         selectedSlotId: f,
                         setErr: r,
                         selectedNav: a,
                         setSelectedNav: u,
                         theme: t
                     })]
                 })]
```

### Comparing `ezbeq-1.0.3/ezbeq/ui/assets/index-fce6f16f.css` & `ezbeq-1.0.4/ezbeq/ui/assets/index-fce6f16f.css`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff` & `ezbeq-1.0.4/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2` & `ezbeq-1.0.4/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2` & `ezbeq-1.0.4/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2` & `ezbeq-1.0.4/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2` & `ezbeq-1.0.4/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2` & `ezbeq-1.0.4/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2` & `ezbeq-1.0.4/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/ui/favicon-16x16.png` & `ezbeq-1.0.4/ezbeq/ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/ui/favicon-32x32.png` & `ezbeq-1.0.4/ezbeq/ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/ui/favicon.ico` & `ezbeq-1.0.4/ezbeq/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/ui/index.html` & `ezbeq-1.0.4/ezbeq/ui/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     <link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
     <link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
     <link rel="mask-icon" href="/safari-pinned-tab.svg" color="#5bbad5">
     <meta name="theme-color" content="#ffffff">
     <meta name="msapplication-TileColor" content="#da532c">
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto:300,400,500"/>
     <title>ezbeq</title>
-  <script type="module" crossorigin src="/assets/index-83ab9065.js"></script>
+  <script type="module" crossorigin src="/assets/index-7427ed0a.js"></script>
   <link rel="stylesheet" href="/assets/index-fce6f16f.css">
 </head>
 <body>
 <noscript>
     You need to enable JavaScript to run this app.
 </noscript>
 <div id="root"></div>
```

### Comparing `ezbeq-1.0.3/ezbeq/ui/mstile-150x150.png` & `ezbeq-1.0.4/ezbeq/ui/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/ezbeq/ui/safari-pinned-tab.svg` & `ezbeq-1.0.4/ezbeq/ui/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.3/pyproject.toml` & `ezbeq-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ezbeq"
-version = "1.0.3"
+version = "1.0.4"
 description = "A webapp which can send beqcatalogue filters to a DSP device"
 authors = ["3ll3d00d <mattkhan+ezbeq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://ezbeq.readthedocs.io/"
 repository = "https://github.com/3ll3d00d/ezbeq"
 include = [
```

### Comparing `ezbeq-1.0.3/PKG-INFO` & `ezbeq-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezbeq
-Version: 1.0.3
+Version: 1.0.4
 Summary: A webapp which can send beqcatalogue filters to a DSP device
 Home-page: https://ezbeq.readthedocs.io/
 License: MIT
 Author: 3ll3d00d
 Author-email: mattkhan+ezbeq@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

