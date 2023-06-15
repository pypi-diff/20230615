# Comparing `tmp/dash_deckgl-0.1.3.tar.gz` & `tmp/dash_deckgl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_deckgl-0.1.3.tar", last modified: Tue Jun 13 04:46:09 2023, max compression
+gzip compressed data, was "dash_deckgl-0.2.0.tar", last modified: Thu Jun 15 03:52:04 2023, max compression
```

## Comparing `dash_deckgl-0.1.3.tar` & `dash_deckgl-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-13 04:46:09.984181 dash_deckgl-0.1.3/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-23 00:50:44.000000 dash_deckgl-0.1.3/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)      226 2023-05-25 20:46:42.000000 dash_deckgl-0.1.3/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)      589 2023-06-13 04:46:09.984181 dash_deckgl-0.1.3/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     3899 2023-05-25 19:30:16.000000 dash_deckgl-0.1.3/README.md
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-13 04:46:09.980181 dash_deckgl-0.1.3/dash_deckgl/
--rw-rw-r--   0 dave      (1000) dave      (1000)     2849 2023-06-13 04:37:29.000000 dash_deckgl-0.1.3/dash_deckgl/DashDeckgl.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2513 2023-05-25 20:45:04.000000 dash_deckgl-0.1.3/dash_deckgl/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)       66 2023-06-13 04:37:29.000000 dash_deckgl-0.1.3/dash_deckgl/_imports_.py
--rw-rw-r--   0 dave      (1000) dave      (1000)  1202621 2023-06-13 04:44:39.000000 dash_deckgl-0.1.3/dash_deckgl/dash_deckgl.min.js
--rw-rw-r--   0 dave      (1000) dave      (1000)    17693 2023-06-13 04:44:39.000000 dash_deckgl-0.1.3/dash_deckgl/deckgl.js
--rw-rw-r--   0 dave      (1000) dave      (1000)     2796 2023-06-13 04:37:29.000000 dash_deckgl-0.1.3/dash_deckgl/metadata.json
--rw-rw-r--   0 dave      (1000) dave      (1000)     2806 2023-06-13 04:37:29.000000 dash_deckgl-0.1.3/dash_deckgl/package-info.json
--rw-rw-r--   0 dave      (1000) dave      (1000)   800972 2023-05-25 20:45:12.000000 dash_deckgl-0.1.3/dash_deckgl/vendor.js
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-13 04:46:09.984181 dash_deckgl-0.1.3/dash_deckgl.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)      589 2023-06-13 04:46:09.000000 dash_deckgl-0.1.3/dash_deckgl.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      417 2023-06-13 04:46:09.000000 dash_deckgl-0.1.3/dash_deckgl.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-13 04:46:09.000000 dash_deckgl-0.1.3/dash_deckgl.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       12 2023-06-13 04:46:09.000000 dash_deckgl-0.1.3/dash_deckgl.egg-info/top_level.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)     2806 2023-06-13 04:19:09.000000 dash_deckgl-0.1.3/package.json
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-06-13 04:46:09.984181 dash_deckgl-0.1.3/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)      653 2023-05-25 20:56:07.000000 dash_deckgl-0.1.3/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-13 04:46:09.984181 dash_deckgl-0.1.3/tests/
--rw-rw-r--   0 dave      (1000) dave      (1000)      329 2023-05-25 21:17:05.000000 dash_deckgl-0.1.3/tests/test_usage.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-15 03:52:04.524285 dash_deckgl-0.2.0/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-23 00:50:44.000000 dash_deckgl-0.2.0/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)      226 2023-05-25 20:46:42.000000 dash_deckgl-0.2.0/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)      589 2023-06-15 03:52:04.524285 dash_deckgl-0.2.0/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3899 2023-05-25 19:30:16.000000 dash_deckgl-0.2.0/README.md
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-15 03:52:04.520285 dash_deckgl-0.2.0/dash_deckgl/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2981 2023-06-15 03:43:04.000000 dash_deckgl-0.2.0/dash_deckgl/DashDeckgl.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2513 2023-05-25 20:45:04.000000 dash_deckgl-0.2.0/dash_deckgl/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)       66 2023-06-15 03:43:04.000000 dash_deckgl-0.2.0/dash_deckgl/_imports_.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)  1202621 2023-06-15 03:43:02.000000 dash_deckgl-0.2.0/dash_deckgl/dash_deckgl.min.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)    16774 2023-06-15 03:43:02.000000 dash_deckgl-0.2.0/dash_deckgl/deckgl.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2917 2023-06-15 03:43:04.000000 dash_deckgl-0.2.0/dash_deckgl/metadata.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2806 2023-06-15 03:43:03.000000 dash_deckgl-0.2.0/dash_deckgl/package-info.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)   800972 2023-05-25 20:45:12.000000 dash_deckgl-0.2.0/dash_deckgl/vendor.js
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-15 03:52:04.524285 dash_deckgl-0.2.0/dash_deckgl.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      589 2023-06-15 03:52:04.000000 dash_deckgl-0.2.0/dash_deckgl.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      417 2023-06-15 03:52:04.000000 dash_deckgl-0.2.0/dash_deckgl.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-15 03:52:04.000000 dash_deckgl-0.2.0/dash_deckgl.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       12 2023-06-15 03:52:04.000000 dash_deckgl-0.2.0/dash_deckgl.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2806 2023-06-15 03:51:39.000000 dash_deckgl-0.2.0/package.json
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-06-15 03:52:04.524285 dash_deckgl-0.2.0/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)      653 2023-05-25 20:56:07.000000 dash_deckgl-0.2.0/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-15 03:52:04.524285 dash_deckgl-0.2.0/tests/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      329 2023-05-25 21:17:05.000000 dash_deckgl-0.2.0/tests/test_usage.py
```

### Comparing `dash_deckgl-0.1.3/PKG-INFO` & `dash_deckgl-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash_deckgl
-Version: 0.1.3
+Version: 0.2.0
 Summary: Deck.gl component for Dash
 Author: Oceanum developers <developers@oceanum.science>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dash_deckgl-0.1.3/README.md` & `dash_deckgl-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.1.3/dash_deckgl/DashDeckgl.py` & `dash_deckgl-0.2.0/dash_deckgl/DashDeckgl.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,29 +37,31 @@
 
 - overlay (string; optional):
     JSON spec of the overlay deck.gl instance (optional).
 
 - spec (string; required):
     JSON spec of the primary deck.gl instance.
 
-- tooltip (dict; optional):
-    A tooltip object that follows he pydeck tooltip specifcation.
+- tooltips (list; optional):
+    An array of tooltip objects that follows he pydeck tooltip
+    specifcation. An additonal 'layer' property can be added to the
+    tooltip objects to restrict their action to that layer ID.
 
 - width (number; optional):
     width of the map component container as pixels or CSS string
     (optional) Default 100% of parent container."""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'dash_deckgl'
     _type = 'DashDeckgl'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, spec=Component.REQUIRED, tooltip=Component.UNDEFINED, width=Component.UNDEFINED, height=Component.UNDEFINED, customLibraries=Component.UNDEFINED, configuration=Component.UNDEFINED, description=Component.UNDEFINED, events=Component.UNDEFINED, overlay=Component.UNDEFINED, lastEvent=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'configuration', 'customLibraries', 'description', 'events', 'height', 'lastEvent', 'overlay', 'spec', 'tooltip', 'width']
+    def __init__(self, id=Component.UNDEFINED, spec=Component.REQUIRED, tooltips=Component.UNDEFINED, width=Component.UNDEFINED, height=Component.UNDEFINED, customLibraries=Component.UNDEFINED, configuration=Component.UNDEFINED, description=Component.UNDEFINED, events=Component.UNDEFINED, overlay=Component.UNDEFINED, lastEvent=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'configuration', 'customLibraries', 'description', 'events', 'height', 'lastEvent', 'overlay', 'spec', 'tooltips', 'width']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'configuration', 'customLibraries', 'description', 'events', 'height', 'lastEvent', 'overlay', 'spec', 'tooltip', 'width']
+        self.available_properties = ['id', 'configuration', 'customLibraries', 'description', 'events', 'height', 'lastEvent', 'overlay', 'spec', 'tooltips', 'width']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
         for k in ['spec']:
```

### Comparing `dash_deckgl-0.1.3/dash_deckgl/__init__.py` & `dash_deckgl-0.2.0/dash_deckgl/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.1.3/dash_deckgl/dash_deckgl.min.js` & `dash_deckgl-0.2.0/dash_deckgl/dash_deckgl.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -50007,15 +50007,15 @@
         var l = jsonpScriptSrc;
         jsonpScriptSrc = function(t) {
             var e, n = (e = A(), /\/_dash-component-suites\//.test(e.src)),
                 i = l(t);
             if (!n) return i;
             var r = i.split("/"),
                 s = r.slice(-1)[0].split(".");
-            return s.splice(1, 0, "v0_1_3m1686631460"), r.splice(-1, 1, s.join(".")), r.join("/")
+            return s.splice(1, 0, "v0_1_3m1686800560"), r.splice(-1, 1, s.join(".")), r.join("/")
         }
     }(() => {
         var t = {
             179: 0
         };
         o.f.j = (e, n) => {
             var i = o.o(t, e) ? t[e] : void 0;
@@ -50064,15 +50064,15 @@
                 return e().createElement(e().Suspense, {
                     fallback: e().createElement("div", null, "Loading map...")
                 }, e().createElement(r, t))
             };
         s.defaultProps = {}, s.propTypes = {
             id: i().string,
             spec: i().string.isRequired,
-            tooltip: i().object,
+            tooltips: i().array,
             width: i().number,
             height: i().number,
             customLibraries: i().array,
             configuration: i().object,
             description: i().object,
             events: i().array,
             overlay: i().string,
```

### Comparing `dash_deckgl-0.1.3/dash_deckgl/deckgl.js` & `dash_deckgl-0.2.0/dash_deckgl/deckgl.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 "use strict";
 (self.webpackChunkdash_deckgl = self.webpackChunkdash_deckgl || []).push([
     [707], {
         1167: (e, r, t) => {
             t.r(r), t.d(r, {
-                default: () => q
+                default: () => R
             });
             var n = {};
             t.r(n), t.d(n, {
                 AGGREGATION_OPERATION: () => p.AGGREGATION_OPERATION,
                 AmbientLight: () => p.AmbientLight,
                 ArcLayer: () => p.ArcLayer,
                 AttributeManager: () => p.AttributeManager,
@@ -218,21 +218,21 @@
             }
 
             function L(e, r) {
                 (null == r || r > e.length) && (r = e.length);
                 for (var t = 0, n = new Array(r); t < r; t++) n[t] = e[t];
                 return n
             }
-            var S, w, O = function(e) {
+            var S = function(e) {
                     return e.charAt(0) === e.charAt(0).toUpperCase()
                 },
-                T = function(e) {
+                w = function(e) {
                     return e.charAt(0) === e.charAt(0).toLowerCase() && "_" !== e.charAt(0)
                 },
-                P = function() {
+                O = function() {
                     var e, r = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {},
                         t = arguments.length > 1 ? arguments[1] : void 0,
                         n = {},
                         o = function(e, r) {
                             var t = "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
                             if (!t) {
                                 if (Array.isArray(e) || (t = v(e))) {
@@ -287,28 +287,28 @@
                     } catch (e) {
                         o.e(e)
                     } finally {
                         o.f()
                     }
                     return n
                 },
-                C = {
-                    classes: P(n, O),
+                T = {
+                    classes: O(n, S),
                     enumerations: {
                         COORDINATE_SYSTEM: u.COORDINATE_SYSTEM,
                         GL: s.Z
                     }
                 },
-                E = (0, o.createContext)(),
-                _ = function(e) {
+                P = (0, o.createContext)(),
+                E = function(e) {
                     var r, t, n = e.configuration,
                         i = e.customLibraries,
                         l = e.children,
                         c = (r = (0, o.useState)(new y.Z({
-                            configuration: C
+                            configuration: T
                         })), t = 2, function(e) {
                             if (Array.isArray(e)) return e
                         }(r) || function(e, r) {
                             var t = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
                             if (null != t) {
                                 var n, o, a, i, l = [],
                                     c = !0,
@@ -352,16 +352,16 @@
                             }
                         };
                     (0, o.useEffect)((function() {
                         p(n)
                     }), [n]);
                     var m = function(e, r) {
                         var t = {
-                            classes: P(r, O),
-                            functions: P(r, T)
+                            classes: O(r, S),
+                            functions: O(r, w)
                         };
                         p(t)
                     };
                     return (0, o.useEffect)((function() {
                         if (i) {
                             var e = {};
                             i.forEach((function(r) {
@@ -383,23 +383,23 @@
                                                 r.onload = e
                                             }))
                                         }
                                         f[e]
                                     }(n)
                             }))
                         }
-                    }), [i]), a().createElement(E.Provider, {
+                    }), [i]), a().createElement(P.Provider, {
                         value: u
                     }, l)
                 };
 
-            function j(e, r) {
+            function _(e, r) {
                 var t = "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
                 if (!t) {
-                    if (Array.isArray(e) || (t = A(e)) || r && e && "number" == typeof e.length) {
+                    if (Array.isArray(e) || (t = C(e)) || r && e && "number" == typeof e.length) {
                         t && (e = t);
                         var n = 0,
                             o = function() {};
                         return {
                             s: o,
                             n: function() {
                                 return n >= e.length ? {
@@ -436,114 +436,54 @@
                         } finally {
                             if (l) throw a
                         }
                     }
                 }
             }
 
-            function A(e, r) {
+            function C(e, r) {
                 if (e) {
-                    if ("string" == typeof e) return x(e, r);
+                    if ("string" == typeof e) return A(e, r);
                     var t = Object.prototype.toString.call(e).slice(8, -1);
-                    return "Object" === t && e.constructor && (t = e.constructor.name), "Map" === t || "Set" === t ? Array.from(e) : "Arguments" === t || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(t) ? x(e, r) : void 0
+                    return "Object" === t && e.constructor && (t = e.constructor.name), "Map" === t || "Set" === t ? Array.from(e) : "Arguments" === t || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(t) ? A(e, r) : void 0
                 }
             }
 
-            function x(e, r) {
+            function A(e, r) {
                 (null == r || r > e.length) && (r = e.length);
                 for (var t = 0, n = new Array(r); t < r; t++) n[t] = e[t];
                 return n
             }
             var G = {
                 fontFamily: '"Helvetica Neue", Helvetica, Arial, sans-serif',
                 display: "flex",
                 flex: "wrap",
                 maxWidth: "500px",
                 flexDirection: "column",
                 zIndex: 2
             };
 
-            function I() {
-                return document.createElement("div")
-            }
-
-            function k(e) {
-                if (!e.picked) return null;
-                if (e.object === S) return w;
-                var r = {
-                    html: N(e.object),
-                    style: G
-                };
-                return w = r, S = e.object, r
-            }
-            var D = new Set(["position", "index"]);
-
-            function N(e) {
-                var r = I();
-                for (var t in e)
-                    if (!D.has(t)) {
-                        var n = I();
-                        n.className = "header", n.textContent = t;
-                        var o = I();
-                        o.className = "value", o.textContent = V(e[t]);
-                        var a = I();
-                        M(a, n, o), a.appendChild(n), a.appendChild(o), r.appendChild(a)
-                    } return r.innerHTML
-            }
-
-            function M(e, r, t) {
-                Object.assign(r.style, {
-                    fontWeight: 700,
-                    marginRight: "10px",
-                    flex: "1 1 0%"
-                }), Object.assign(t.style, {
-                    flex: "none",
-                    maxWidth: "250px",
-                    overflow: "hidden",
-                    whiteSpace: "nowrap",
-                    textOverflow: "ellipsis"
-                }), Object.assign(e.style, {
-                    display: "flex",
-                    flexDirection: "row",
-                    justifyContent: "space-between",
-                    alignItems: "stretch"
-                })
-            }
-
-            function V(e) {
-                var r;
-                if (Array.isArray(e) && e.length > 4) r = "Array<".concat(e.length, ">");
-                else if ("string" == typeof e) r = e;
-                else if ("number" == typeof e) r = String(e);
-                else try {
-                    r = JSON.stringify(e)
-                } catch (e) {
-                    r = "<Non-Serializable Object>"
-                }
-                return r.length > 50 && (r = r.slice(0, 50)), r
-            }
-
-            function R(e, r) {
+            function j(e, r) {
                 var t, n, o, a = e,
                     i = "properties",
-                    l = j(function(e) {
-                        if (Array.isArray(e)) return x(e)
+                    l = _(function(e) {
+                        if (Array.isArray(e)) return A(e)
                     }(o = new Set(e.match(/{[^}]*}/g).map((function(e) {
                         return e.replace(/[{}]/g, "")
                     })))) || function(e) {
                         if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
-                    }(o) || A(o) || function() {
+                    }(o) || C(o) || function() {
                         throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                     }());
                 try {
                     for (l.s(); !(n = l.n()).done;) {
                         var c = n.value;
                         if (c.includes(".")) {
                             t = r;
-                            var u, s = j(c.split("."));
+                            var u, s = _(c.split("."));
                             try {
                                 for (s.s(); !(u = s.n()).done;) {
                                     var y = u.value;
                                     if (!t.hasOwnProperty(y)) {
                                         t = void 0;
                                         break
                                     }
@@ -561,77 +501,77 @@
                     l.e(e)
                 } finally {
                     l.f()
                 }
                 return a
             }
 
-            function F(e) {
-                return F = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+            function x(e) {
+                return x = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                     return typeof e
                 } : function(e) {
                     return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-                }, F(e)
+                }, x(e)
             }
 
-            function U() {
-                return U = Object.assign ? Object.assign.bind() : function(e) {
+            function I() {
+                return I = Object.assign ? Object.assign.bind() : function(e) {
                     for (var r = 1; r < arguments.length; r++) {
                         var t = arguments[r];
                         for (var n in t) Object.prototype.hasOwnProperty.call(t, n) && (e[n] = t[n])
                     }
                     return e
-                }, U.apply(this, arguments)
+                }, I.apply(this, arguments)
             }
 
-            function H(e, r) {
+            function k(e, r) {
                 var t = Object.keys(e);
                 if (Object.getOwnPropertySymbols) {
                     var n = Object.getOwnPropertySymbols(e);
                     r && (n = n.filter((function(r) {
                         return Object.getOwnPropertyDescriptor(e, r).enumerable
                     }))), t.push.apply(t, n)
                 }
                 return t
             }
 
-            function B(e) {
+            function D(e) {
                 for (var r = 1; r < arguments.length; r++) {
                     var t = null != arguments[r] ? arguments[r] : {};
-                    r % 2 ? H(Object(t), !0).forEach((function(r) {
-                        W(e, r, t[r])
-                    })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(t)) : H(Object(t)).forEach((function(r) {
+                    r % 2 ? k(Object(t), !0).forEach((function(r) {
+                        V(e, r, t[r])
+                    })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(t)) : k(Object(t)).forEach((function(r) {
                         Object.defineProperty(e, r, Object.getOwnPropertyDescriptor(t, r))
                     }))
                 }
                 return e
             }
 
-            function W(e, r, t) {
+            function V(e, r, t) {
                 return (r = function(e) {
                     var r = function(e, r) {
-                        if ("object" !== F(e) || null === e) return e;
+                        if ("object" !== x(e) || null === e) return e;
                         var t = e[Symbol.toPrimitive];
                         if (void 0 !== t) {
                             var n = t.call(e, "string");
-                            if ("object" !== F(n)) return n;
+                            if ("object" !== x(n)) return n;
                             throw new TypeError("@@toPrimitive must return a primitive value.")
                         }
                         return String(e)
                     }(e);
-                    return "symbol" === F(r) ? r : String(r)
+                    return "symbol" === x(r) ? r : String(r)
                 }(r)) in e ? Object.defineProperty(e, r, {
                     value: t,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : e[r] = t, e
             }
 
-            function J(e, r) {
+            function M(e, r) {
                 return function(e) {
                     if (Array.isArray(e)) return e
                 }(e) || function(e, r) {
                     var t = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
                     if (null != t) {
                         var n, o, a, i, l = [],
                             c = !0,
@@ -651,115 +591,119 @@
                                 if (u) throw o
                             }
                         }
                         return l
                     }
                 }(e, r) || function(e, r) {
                     if (e) {
-                        if ("string" == typeof e) return z(e, r);
+                        if ("string" == typeof e) return N(e, r);
                         var t = Object.prototype.toString.call(e).slice(8, -1);
-                        return "Object" === t && e.constructor && (t = e.constructor.name), "Map" === t || "Set" === t ? Array.from(e) : "Arguments" === t || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(t) ? z(e, r) : void 0
+                        return "Object" === t && e.constructor && (t = e.constructor.name), "Map" === t || "Set" === t ? Array.from(e) : "Arguments" === t || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(t) ? N(e, r) : void 0
                     }
                 }(e, r) || function() {
                     throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                 }()
             }
 
-            function z(e, r) {
+            function N(e, r) {
                 (null == r || r > e.length) && (r = e.length);
                 for (var t = 0, n = new Array(r); t < r; t++) n[t] = e[t];
                 return n
             }
-            var Z = function(e) {
+            new Set(["position", "index"]);
+            var F = function(e) {
                 var r = e.spec,
-                    t = e.tooltip,
+                    t = e.tooltips,
                     n = e.width,
                     u = void 0 === n ? "100%" : n,
                     s = e.height,
                     y = void 0 === s ? 500 : s,
                     f = e.events,
                     p = void 0 === f ? [] : f,
                     m = e.description,
                     g = e.overlay,
                     d = e.mapbox_key,
                     b = e.google_maps_key,
                     h = e.setProps,
-                    v = (e.lastEvent, J((0, o.useState)({}), 2)),
+                    v = (e.lastEvent, M((0, o.useState)({}), 2)),
                     L = v[0],
                     S = v[1],
-                    w = J((0, o.useState)({}), 2),
+                    w = M((0, o.useState)({}), 2),
                     O = w[0],
                     T = w[1],
-                    P = J((0, o.useState)(!1), 2),
-                    C = (P[0], P[1], J((0, o.useState)(!1), 2)),
-                    _ = (C[0], C[1], (0, o.useContext)(E)),
-                    j = J((0, o.useState)(null), 2),
-                    A = j[0],
-                    x = j[1],
-                    I = [];
+                    E = M((0, o.useState)(!1), 2),
+                    _ = (E[0], E[1], M((0, o.useState)(!1), 2)),
+                    C = (_[0], _[1], (0, o.useContext)(P)),
+                    A = M((0, o.useState)(null), 2),
+                    x = A[0],
+                    k = A[1],
+                    N = [];
                 if (m)
-                    for (var D in m)
-                        if (["top-right", "top-left", "bottom-right", "bottom-left"].includes(D)) {
-                            var N = D.split("-");
-                            I.push({
-                                pos: N,
-                                content: m[D]
+                    for (var F in m)
+                        if (["top-right", "top-left", "bottom-right", "bottom-left"].includes(F)) {
+                            var R = F.split("-");
+                            N.push({
+                                pos: R,
+                                content: m[F]
                             })
-                        } var M = (0, o.useCallback)((function(e, r) {
+                        } var U = (0, o.useCallback)((function(e, r) {
                         p.includes(e) && h({
-                            lastEvent: B(B({}, r.object), {}, {
+                            lastEvent: D(D({}, r.object), {}, {
                                 coordinate: r.coordinate,
                                 eventType: e
                             })
                         })
                     }), [p]),
-                    V = {
+                    H = {
                         onClick: function(e) {
-                            return M("click", e)
+                            return U("click", e)
                         },
                         onHover: function(e) {
-                            return M("hover", e)
+                            return U("hover", e)
                         },
                         onDragStart: function(e) {
-                            return M("drag-start", e)
+                            return U("drag-start", e)
                         },
                         onDrag: function(e) {
-                            return M("drag", e)
+                            return U("drag", e)
                         },
                         onDragEnd: function(e) {
-                            return M("drag-end", e)
+                            return U("drag-end", e)
                         }
                     },
-                    F = function(e) {
-                        return e ? e.html || e.text ? function(r) {
+                    B = function(e) {
+                        return e ? e.length ? function(r) {
                             if (!r.picked) return null;
-                            var t = {
-                                style: e.style || G
-                            };
-                            return e.html ? t.html = R(e.html, r.object) : t.text = R(e.text, r.object), t
-                        } : k : null
+                            var t = null;
+                            return e.map((function(e) {
+                                if (e.layer && r.layer.id != e.layer) return null;
+                                t = {
+                                    style: e.style || G
+                                }, e.html ? t.html = j(e.html, r.object) : t.text = j(e.text, r.object)
+                            })), t
+                        } : getTooltipDefault : null
                     }(t),
-                    H = B(B({}, V), {}, {
-                        getTooltip: F
+                    J = D(D({}, H), {}, {
+                        getTooltip: B
                     });
                 (0, o.useEffect)((function() {
                     ! function() {
                         var e, r;
                         e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "https://api.tiles.mapbox.com/mapbox-gl-js/v1.13.2/mapbox-gl.css", (r = document.createElement("link")).type = "text/css", r.rel = "stylesheet", r.href = e, document.getElementsByTagName("head")[0].appendChild(r)
                     }()
                 }), []), (0, o.useEffect)((function() {
-                    var e = _.convert(r);
-                    !A && e.initialViewState && x(e.initialViewState), S(B(B({}, L), e))
-                }), [r, _]), (0, o.useEffect)((function() {
-                    var e = _.convert(g);
-                    T(B(B({}, O), e))
-                }), [g, _]);
-                var z = (0, o.useCallback)((function(e) {
+                    var e = C.convert(r);
+                    !x && e.initialViewState && k(e.initialViewState), S(D(D({}, L), e))
+                }), [r, C]), (0, o.useEffect)((function() {
+                    var e = C.convert(g);
+                    T(D(D({}, O), e))
+                }), [g, C]);
+                var W = (0, o.useCallback)((function(e) {
                     var r = e.viewState;
-                    x(r)
+                    k(r)
                 }), []);
                 return b ? a().createElement("div", null, "Google map overlays not supported") : a().createElement("div", {
                     className: "deckgl-map",
                     style: {
                         height: y,
                         width: u,
                         position: "relative"
@@ -767,57 +711,57 @@
                 }, a().createElement("div", {
                     id: "deckgl-primary",
                     style: {
                         width: "100%",
                         height: "100%",
                         position: "relative"
                     }
-                }, A && a().createElement(i.Z, U({
-                    viewState: A,
-                    onViewStateChange: z
-                }, H, L), a().createElement(c.D5, {
+                }, x && a().createElement(i.Z, I({
+                    viewState: x,
+                    onViewStateChange: W
+                }, J, L), a().createElement(c.D5, {
                     mapStyle: L.mapStyle || l.Z.POSITRON,
                     mapboxAccessToken: d
                 }))), g && a().createElement("div", {
                     id: "deckgl-overlay",
                     style: {
                         width: "100%",
                         height: "100%",
                         position: "relative",
                         pointerEvents: "none"
                     }
-                }, a().createElement(i.Z, U({
-                    viewState: A,
+                }, a().createElement(i.Z, I({
+                    viewState: x,
                     contoller: !1
-                }, H, O, {
-                    style: B(B({}, O.style), {}, {
+                }, J, O, {
+                    style: D(D({}, O.style), {}, {
                         zIndex: 1,
                         pointerEvents: "none"
                     })
                 }), a().createElement(c.D5, {
                     mapStyle: O.mapStyle,
                     mapboxAccessToken: d
-                }))), I.map((function(e, r) {
+                }))), N.map((function(e, r) {
                     var t;
                     return a().createElement("div", {
                         key: r,
                         className: "description",
                         style: (t = {
                             position: "absolute",
                             zIndex: 10
-                        }, W(t, e.pos[0], 10), W(t, e.pos[1], 10), t),
+                        }, V(t, e.pos[0], 10), V(t, e.pos[1], 10), t),
                         dangerouslySetInnerHTML: {
                             __html: e.content
                         }
                     })
                 })))
             };
-            const q = function(e) {
-                return a().createElement(_, {
+            const R = function(e) {
+                return a().createElement(E, {
                     customLibraries: e.customLibraries,
                     configuration: e.configuration
-                }, a().createElement(Z, e))
+                }, a().createElement(F, e))
             }
         }
     }
 ]);
 //# sourceMappingURL=deckgl.js.map
```

### Comparing `dash_deckgl-0.1.3/dash_deckgl/metadata.json` & `dash_deckgl-0.2.0/dash_deckgl/metadata.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9903846153846154%*

 * *Differences: {"'src/lib/components/DashDeckgl.react.js'": "{'props': {'tooltips': OrderedDict([('type', "*

 * *                                             "OrderedDict([('name', 'array')])), ('required', "*

 * *                                             'False), (\'description\', "An array of tooltip '*

 * *                                             'objects that follows he pydeck tooltip '*

 * *                                             "specifcation.\\nAn additonal 'layer' property can be "*

 * *                                         […]*

```diff
@@ -70,19 +70,19 @@
             "spec": {
                 "description": "JSON spec of the primary deck.gl instance",
                 "required": true,
                 "type": {
                     "name": "string"
                 }
             },
-            "tooltip": {
-                "description": "A tooltip object that follows he pydeck tooltip specifcation.",
+            "tooltips": {
+                "description": "An array of tooltip objects that follows he pydeck tooltip specifcation.\nAn additonal 'layer' property can be added to the tooltip objects to restrict their action to that layer ID.",
                 "required": false,
                 "type": {
-                    "name": "object"
+                    "name": "array"
                 }
             },
             "width": {
                 "description": "width of the map component container as pixels or CSS string\n(optional) Default 100% of parent container",
                 "required": false,
                 "type": {
                     "name": "number"
```

### Comparing `dash_deckgl-0.1.3/dash_deckgl/package-info.json` & `dash_deckgl-0.2.0/dash_deckgl/package-info.json`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.1.3/dash_deckgl/vendor.js` & `dash_deckgl-0.2.0/dash_deckgl/vendor.js`

 * *Files identical despite different names*

### Comparing `dash_deckgl-0.1.3/dash_deckgl.egg-info/PKG-INFO` & `dash_deckgl-0.2.0/dash_deckgl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-deckgl
-Version: 0.1.3
+Version: 0.2.0
 Summary: Deck.gl component for Dash
 Author: Oceanum developers <developers@oceanum.science>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dash_deckgl-0.1.3/package.json` & `dash_deckgl-0.2.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.2.0'"}*

```diff
@@ -66,9 +66,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_deckgl -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.1.3"
+    "version": "0.2.0"
 }
```

### Comparing `dash_deckgl-0.1.3/setup.py` & `dash_deckgl-0.2.0/setup.py`

 * *Files identical despite different names*

