# Comparing `tmp/babelfont-3.0.0a9.tar.gz` & `tmp/babelfont-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "babelfont-3.0.0a9.tar", max compression
+gzip compressed data, was "babelfont-3.0.1.tar", max compression
```

## Comparing `babelfont-3.0.0a9.tar` & `babelfont-3.0.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0      504 2022-04-26 13:22:00.511695 babelfont-3.0.0a9/pyproject.toml
--rw-r--r--   0        0        0      211 2021-04-13 13:38:17.795023 babelfont-3.0.0a9/src/babelfont/Anchor.py
--rw-r--r--   0        0        0     3477 2021-10-28 13:42:25.366959 babelfont-3.0.0a9/src/babelfont/Axis.py
--rw-r--r--   0        0        0     7627 2021-06-29 14:17:05.952504 babelfont-3.0.0a9/src/babelfont/BaseObject.py
--rw-r--r--   0        0        0      224 2021-03-26 08:47:16.134910 babelfont-3.0.0a9/src/babelfont/Component.py
--rw-r--r--   0        0        0     7323 2021-11-18 14:07:46.920584 babelfont-3.0.0a9/src/babelfont/Font.py
--rw-r--r--   0        0        0     1539 2021-06-16 09:47:35.088433 babelfont-3.0.0a9/src/babelfont/Glyph.py
--rw-r--r--   0        0        0      242 2021-03-26 08:47:16.135842 babelfont-3.0.0a9/src/babelfont/Guide.py
--rw-r--r--   0        0        0     1256 2021-06-16 08:57:34.386721 babelfont-3.0.0a9/src/babelfont/Instance.py
--rw-r--r--   0        0        0     4554 2021-07-22 19:32:53.117800 babelfont-3.0.0a9/src/babelfont/Layer.py
--rw-r--r--   0        0        0     3123 2021-06-16 08:15:20.619157 babelfont-3.0.0a9/src/babelfont/Master.py
--rw-r--r--   0        0        0     1318 2021-03-26 08:47:16.137014 babelfont-3.0.0a9/src/babelfont/Names.py
--rw-r--r--   0        0        0      767 2021-03-26 08:47:16.137415 babelfont-3.0.0a9/src/babelfont/Node.py
--rw-r--r--   0        0        0     1469 2021-06-16 09:34:41.198921 babelfont-3.0.0a9/src/babelfont/Shape.py
--rw-r--r--   0        0        0      566 2021-03-26 08:47:16.138048 babelfont-3.0.0a9/src/babelfont/__init__.py
--rw-r--r--   0        0        0      738 2021-04-13 13:16:34.081580 babelfont-3.0.0a9/src/babelfont/__main__.py
--rw-r--r--   0        0        0     2102 2021-06-16 08:39:49.625024 babelfont-3.0.0a9/src/babelfont/convertors/__init__.py
--rw-r--r--   0        0        0     7497 2021-11-18 14:07:28.520851 babelfont-3.0.0a9/src/babelfont/convertors/designspace.py
--rw-r--r--   0        0        0     6096 2021-03-26 08:47:16.143284 babelfont-3.0.0a9/src/babelfont/convertors/fontlab.py
--rw-r--r--   0        0        0    30196 2022-04-26 13:21:48.345914 babelfont-3.0.0a9/src/babelfont/convertors/glyphs.py
--rw-r--r--   0        0        0    14799 2021-04-13 13:34:57.422507 babelfont-3.0.0a9/src/babelfont/convertors/gsobject.py
--rw-r--r--   0        0        0     3867 2021-06-16 09:05:16.916020 babelfont-3.0.0a9/src/babelfont/convertors/nfsf.py
--rw-r--r--   0        0        0    15373 2021-11-28 21:55:26.075196 babelfont-3.0.0a9/src/babelfont/convertors/truetype.py
--rw-r--r--   0        0        0      436 2021-03-09 15:00:23.952332 babelfont-3.0.0a9/src/babelfont/convertors/ufo.py
--rw-r--r--   0        0        0        0 2021-03-26 08:47:16.144437 babelfont-3.0.0a9/src/babelfont/fontFilters/__init__.py
--rw-r--r--   0        0        0     2456 2021-11-18 14:05:57.835730 babelfont-3.0.0a9/src/babelfont/fontFilters/featureWriters.py
--rw-r--r--   0        0        0      733 2021-06-29 21:02:26.629124 babelfont-3.0.0a9/src/babelfont/names.rs
--rw-r--r--   0        0        0      922 2022-04-26 13:22:26.667578 babelfont-3.0.0a9/setup.py
--rw-r--r--   0        0        0      836 2022-04-26 13:22:26.667780 babelfont-3.0.0a9/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-06 14:10:29.366930 babelfont-3.0.1/LICENSE
+-rw-r--r--   0        0        0     1487 2022-10-19 21:49:42.369264 babelfont-3.0.1/README.md
+-rw-r--r--   0        0        0      601 2023-06-15 09:25:27.322460 babelfont-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0      211 2022-10-19 21:49:42.371205 babelfont-3.0.1/src/babelfont/Anchor.py
+-rw-r--r--   0        0        0     3493 2023-06-06 15:32:36.882623 babelfont-3.0.1/src/babelfont/Axis.py
+-rw-r--r--   0        0        0     7637 2022-10-19 21:49:42.371911 babelfont-3.0.1/src/babelfont/BaseObject.py
+-rw-r--r--   0        0        0      224 2022-10-19 21:49:42.372255 babelfont-3.0.1/src/babelfont/Component.py
+-rw-r--r--   0        0        0     7461 2022-10-19 21:49:42.372605 babelfont-3.0.1/src/babelfont/Font.py
+-rw-r--r--   0        0        0     1544 2022-10-19 21:49:42.373015 babelfont-3.0.1/src/babelfont/Glyph.py
+-rw-r--r--   0        0        0      242 2022-10-19 21:49:42.373332 babelfont-3.0.1/src/babelfont/Guide.py
+-rw-r--r--   0        0        0     1256 2022-10-19 21:49:42.373694 babelfont-3.0.1/src/babelfont/Instance.py
+-rw-r--r--   0        0        0     4549 2022-10-19 21:49:42.374044 babelfont-3.0.1/src/babelfont/Layer.py
+-rw-r--r--   0        0        0     3123 2022-10-19 21:49:42.374368 babelfont-3.0.1/src/babelfont/Master.py
+-rw-r--r--   0        0        0     1318 2022-10-19 21:49:42.374742 babelfont-3.0.1/src/babelfont/Names.py
+-rw-r--r--   0        0        0      767 2022-10-19 21:49:42.375075 babelfont-3.0.1/src/babelfont/Node.py
+-rw-r--r--   0        0        0     1469 2022-10-19 21:49:42.375377 babelfont-3.0.1/src/babelfont/Shape.py
+-rw-r--r--   0        0        0      566 2022-10-19 21:49:42.375788 babelfont-3.0.1/src/babelfont/__init__.py
+-rw-r--r--   0        0        0      738 2022-10-19 21:49:42.376105 babelfont-3.0.1/src/babelfont/__main__.py
+-rw-r--r--   0        0        0     2194 2022-10-19 21:49:42.376432 babelfont-3.0.1/src/babelfont/convertors/__init__.py
+-rw-r--r--   0        0        0     7521 2022-10-19 21:49:42.376767 babelfont-3.0.1/src/babelfont/convertors/designspace.py
+-rw-r--r--   0        0        0     6822 2022-10-19 21:49:42.377119 babelfont-3.0.1/src/babelfont/convertors/fontlab.py
+-rw-r--r--   0        0        0    30419 2023-05-22 11:43:03.853417 babelfont-3.0.1/src/babelfont/convertors/glyphs.py
+-rw-r--r--   0        0        0    14882 2023-05-22 11:36:45.328197 babelfont-3.0.1/src/babelfont/convertors/gsobject.py
+-rw-r--r--   0        0        0     3887 2022-10-19 21:49:42.378291 babelfont-3.0.1/src/babelfont/convertors/nfsf.py
+-rw-r--r--   0        0        0    16280 2023-06-06 15:32:22.421394 babelfont-3.0.1/src/babelfont/convertors/truetype.py
+-rw-r--r--   0        0        0      718 2022-10-19 21:49:42.378991 babelfont-3.0.1/src/babelfont/convertors/ufo.py
+-rw-r--r--   0        0        0        0 2022-10-19 21:49:42.379066 babelfont-3.0.1/src/babelfont/fontFilters/__init__.py
+-rw-r--r--   0        0        0     2456 2022-10-19 21:49:42.379370 babelfont-3.0.1/src/babelfont/fontFilters/featureWriters.py
+-rw-r--r--   0        0        0     2534 1970-01-01 00:00:00.000000 babelfont-3.0.1/setup.py
+-rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 babelfont-3.0.1/PKG-INFO
```

### Comparing `babelfont-3.0.0a9/src/babelfont/Axis.py` & `babelfont-3.0.1/src/babelfont/Axis.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     # Stolen from fontTools.designspaceLib
 
     def map_forward(self, v):
         from fontTools.varLib.models import piecewiseLinearMap
 
         if not self.map:
             return v
-        return piecewiseLinearMap(v, {k: v for k, v in self.map})
+        return piecewiseLinearMap(v, {k: v for k, v in self.map.items()})
 
     def map_backward(self, v):
         from fontTools.varLib.models import piecewiseLinearMap
 
         if not self.map:
             return v
-        return piecewiseLinearMap(v, {v: k for k, v in self.map})
+        return piecewiseLinearMap(v, {v: k for k, v in self.map.items()})
```

### Comparing `babelfont-3.0.0a9/src/babelfont/BaseObject.py` & `babelfont-3.0.1/src/babelfont/BaseObject.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,24 +84,24 @@
 
     _formatspecific: dict = field(
         default_factory=dict,
         repr=False,
         metadata={
             "skip_serialize": True,
             "description": """
-Each object in NFSF has an optional attached dictionary to allow the storage
+Each object in Babelfont has an optional attached dictionary to allow the storage
 of format-specific information. Font creation software may store any additional
 information that they wish to have preserved on import and export under a
 namespaced (reverse-domain) key in this dictionary. For example, information
 specific to the Glyphs software should be stored under the key `com.glyphsapp`.
 The value stored under this key may be any data serializable in JSON; typically
 it will be a `dict`.
 
 Note that there is an important distinction between the Python object format
-of this field and the NFSF-JSON representation. When stored to JSON, this key
+of this field and the Babelfont-JSON representation. When stored to JSON, this key
 is exported not as `_formatspecific` but as a simple underscore (`_`).
 """,
         },
     )
     _: dict = field(default=None, repr=False, metadata={"skip_serialize": True})
 
     def __post_init__(self):
```

### Comparing `babelfont-3.0.0a9/src/babelfont/Font.py` & `babelfont-3.0.1/src/babelfont/Font.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     note: str = field(
         default=None,
         metadata={"description": "Any user-defined textual note about this font."},
     )
     date: datetime = field(
         default_factory=datetime.now,
         metadata={
-            "description": """The font's date. When writing to NFSF-JSON, this
+            "description": """The font's date. When writing to Babelfont-JSON, this
 should be stored in the format `%Y-%m-%d %H:%M:%S`. *If not provided, defaults
 to the current date/time*.""",
             "json_type": "str",
         },
     )
     names: Names = field(default_factory=Names, metadata={"skip_serialize": True})
     customOpenTypeValues: [OTValue] = field(
@@ -137,14 +137,17 @@
 
     @functools.cached_property
     def default_master(self):
         default_loc = {a.tag: a.map_forward(a.default) for a in self.axes}
         for m in self.masters:
             if m.location == default_loc:
                 return m
+        if len(self.masters) == 1:
+            return self.masters[0]
+        raise ValueError("Could not determine default master")
 
     @functools.cached_property
     def _master_map(self):
         return {m.id: m for m in self.masters}
 
     @functools.cached_property
     def unicode_map(self):
```

### Comparing `babelfont-3.0.0a9/src/babelfont/Glyph.py` & `babelfont-3.0.1/src/babelfont/Glyph.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,10 +47,10 @@
 
 @dataclass
 class Glyph(BaseObject, _GlyphFields):
 
     _write_one_line = True
 
     @property
-    def nfsf_filename(self):
+    def babelfont_filename(self):
         return os.path.join("glyphs", (userNameToFileName(self.name) + ".nfsglyph"))
```

### Comparing `babelfont-3.0.0a9/src/babelfont/Instance.py` & `babelfont-3.0.1/src/babelfont/Instance.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.0a9/src/babelfont/Layer.py` & `babelfont-3.0.1/src/babelfont/Layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,8 +146,8 @@
         ourtype = Node._from_pen_type[segmentType]
         if smooth:
             ourtype = ourtype + "s"
         self.curPath.append(Node(pt[0], pt[1], ourtype))
 
     def addComponent(self, baseGlyphName, transformation, identifier=None,
                      **kwargs):
-        self.target.shapes.append(Shape(ref=baseGlyphName, transformation=transformation))
+        self.target.shapes.append(Shape(ref=baseGlyphName, transform=transformation))
```

### Comparing `babelfont-3.0.0a9/src/babelfont/Master.py` & `babelfont-3.0.1/src/babelfont/Master.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.0a9/src/babelfont/Names.py` & `babelfont-3.0.1/src/babelfont/Names.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.0a9/src/babelfont/Node.py` & `babelfont-3.0.1/src/babelfont/Node.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.0a9/src/babelfont/Shape.py` & `babelfont-3.0.1/src/babelfont/Shape.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.0a9/src/babelfont/__init__.py` & `babelfont-3.0.1/src/babelfont/__init__.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.0a9/src/babelfont/__main__.py` & `babelfont-3.0.1/src/babelfont/__main__.py`

 * *Files identical despite different names*

### Comparing `babelfont-3.0.0a9/src/babelfont/convertors/__init__.py` & `babelfont-3.0.1/src/babelfont/convertors/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import sys
 import pkgutil
 import inspect
+import importlib
 from babelfont import Font
 
 class BaseConvertor:
     suffix = ".XXX"
 
     @classmethod
     def can_load(self, other, **kwargs):
@@ -44,15 +45,17 @@
             os.path.dirname(sys.modules[cls.__module__].__file__)
         )
         # Additional plugin path here?
         loaders = pkgutil.iter_modules([convertorpath])
         for loader, module_name, is_pkg in loaders:
             if is_pkg:
                 continue
-            _module = loader.find_module(module_name).load_module(module_name)
+            spec = loader.find_spec(module_name)
+            _module = importlib.util.module_from_spec(spec)
+            spec.loader.exec_module(_module)
             classes = [
                 x[1]
                 for x in inspect.getmembers(_module, inspect.isclass)
                 if issubclass(x[1], BaseConvertor)
             ]
             cls.convertors.extend(classes)
```

### Comparing `babelfont-3.0.0a9/src/babelfont/convertors/designspace.py` & `babelfont-3.0.1/src/babelfont/convertors/designspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         self.font = Font()
         return self._load()
 
     def _load(self):
         self._load_axes()
 
         for source in self.ds.sources:
-            source._nfsf_master = self._load_master(source)
-            self.font.masters.append(source._nfsf_master)
+            source._babelfont_master = self._load_master(source)
+            self.font.masters.append(source._babelfont_master)
 
         for instance in self.ds.instances:
             self.font.instances.append(self._load_instance(instance))
 
         firstmaster = self.ds.sources[0].font
         self._load_metadata(firstmaster)
         glyphs_dict = self._load_glyphs(firstmaster)
@@ -131,15 +131,15 @@
             g.production_name = lib["public.postscriptNames"][g.name]
         return g
 
     def _load_layer(self, source, ufo_layer, glyphname):
         ufo_glyph = ufo_layer[glyphname]
         width = ufo_glyph.width
         l = Layer(width=width, id=uuid.uuid1())
-        l._master = source._nfsf_master.id
+        l._master = source._babelfont_master.id
         l._font = self.font
         for contour in ufo_glyph:
             l.shapes.append(self._load_contour(contour))
         for component in ufo_glyph.components:
             l.shapes.append(self._load_component(component))
         for anchor in ufo_glyph.anchors:
             l.anchors.append(self._load_anchor(anchor))
@@ -193,11 +193,11 @@
     }
 
     def _load_metadata(self, ufo):
         firstfontinfo = ufo.info
         self.font.upm = firstfontinfo.unitsPerEm
         self.font.version = (firstfontinfo.versionMajor, firstfontinfo.versionMinor)
         self.font.note = firstfontinfo.note
-        for ours, theirs in self.names_dict:
-            their_value = firstfontinfo.getattr(theirs)
+        for ours, theirs in self.names_dict.items():
+            their_value = getattr(firstfontinfo, theirs)
             if their_value:
                 getattr(self.font.names, ours).set_default(their_value)
```

### Comparing `babelfont-3.0.0a9/src/babelfont/convertors/fontlab.py` & `babelfont-3.0.1/src/babelfont/convertors/fontlab.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,16 +8,25 @@
 
 
 class Fontlab(BaseConvertor):
     suffix = ".vfj"
 
     def _load(self):
         self.fontlab = orjson.loads(open(self.filename).read())["font"]
+        self.known_transforms = {}
         self._load_axes()
         self._load_masters()
+        if "defaultMaster" in self.fontlab:
+            default = self.font.master(self.fontlab["defaultMaster"])
+            if self.font.axes:
+                def_loc = self.font.map_backward(default.location)
+                for axis in self.font.axes:
+                    if axis.tag in default.location:
+                        axis.default = def_loc[axis.tag]
+            assert self.font.default_master
         for g in self.fontlab.get("glyphs", []):
             glyph = self._load_thing(g, self.glyph_loader)
             self.font.glyphs.append(glyph)
         self.font.upm = self.fontlab.get("upm", 1000)
         return self.font
 
     axis_loader = (
@@ -44,27 +53,33 @@
     def _convert_color(_, col):
         r, g, b = int(col[1:3], 16), int(col[3:5], 16), int(col[5:7], 16)
         return Color(r, g, b, 0)
 
     def _convert_shapes(self, flshapes):
         shapes = []
         for shape in flshapes:
+            transform_j = shape.get("transform", {})
+            if "id" in transform_j:
+                self.known_transforms[transform_j["id"]] = transform_j
+            if isinstance(transform_j, str):
+                transform_j = self.known_transforms[transform_j]
+            transform = Transform().translate(
+                            transform_j.get("xOffset", 0),
+                            transform_j.get("yOffset", 0),
+                        )
             if "component" in shape:
                 shapes.append(
                     Shape(
                         ref=shape["component"]["glyphName"],
-                        transform=Transform().translate(
-                            shape.get("transform", {}).get("xOffset", 0),
-                            shape.get("transform", {}).get("yOffset", 0),
-                        ),
+                        transform=transform,
                         _=shape["component"],
                     )
                 )
             else:
-                for flcontour in shape["elementData"]["contours"]:
+                for flcontour in shape["elementData"].get("contours",[]):
                     contour = Shape(nodes=[])
                     for n in flcontour["nodes"]:
                         contour.nodes.extend(self._load_node(n))
                     shapes.append(contour)
         return shapes
 
     def _load_node(self, input_):
```

### Comparing `babelfont-3.0.0a9/src/babelfont/convertors/glyphs.py` & `babelfont-3.0.1/src/babelfont/convertors/glyphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,17 @@
             or convertor.scratch["plist"][".formatVersion"] < 3
         )
 
     @classmethod
     def can_save(cls, convertor, **kwargs):
         if not super().can_save(convertor, **kwargs):
             return False
-        if "format" in kwargs and kwargs["format"] == 2:
-            return True
+        if "format" in kwargs:
+            return kwargs["format"] == 2
+        return True
 
     @classmethod
     def can_load(cls, convertor):
         if not super().can_load(convertor):
             return False
         if not "plist" in convertor.scratch:
             convertor.scratch["plist"] = openstep_plist.load(
@@ -323,14 +324,16 @@
 
     def _load_anchor(self, ganchor):
         pos = ganchor.get("position", "{0, 0}")
         m = re.match(r"^\{(\S+), (\S+)\}", pos)
         return Anchor(name=ganchor["name"], x=float(m[1]), y=float(m[2]))
 
     def _load_instance(self, ginstance):
+        if ginstance.get("type") == "variable":
+            return
         if "axesValues" in ginstance:
             location = ginstance["axesValues"]
             instance_location = {k.tag: v for k, v in zip(self.font.axes, location)}
         elif "instanceInterpolations" in ginstance:
             # All right then.
             instance_location = {k.tag: 0 for k in self.font.axes}
             for mId, factor in ginstance["instanceInterpolations"].items():
@@ -482,15 +485,16 @@
         for f in self.glyphs.get("featurePrefixes", []):
             featurefile = featurefile + f.get("code")
         for f in self.glyphs.get("features", []):
             tag = f.get("tag", f.get("name", ""))
             feacode = "feature %s { %s\n} %s;" % (tag, f["code"], tag)
             featurefile = featurefile + feacode
 
-        feaparser = FeaParser(featurefile)
+        glyphNames = {g.name for g in self.font.glyphs}
+        feaparser = FeaParser(featurefile, glyphNames=glyphNames)
         ast = feaparser.parser.ast
         for name, members in self.font.features.namedClasses.items():
             glyphclass = ast.GlyphClassDefinition(
                 name, ast.GlyphClass([m for m in members])
             )
             feaparser.parser.glyphclasses_.define(name, glyphclass)
         feaparser.parse()
@@ -505,16 +509,17 @@
             and convertor.scratch["plist"][".formatVersion"] >= 3
         )
 
     @classmethod
     def can_save(cls, convertor, **kwargs):
         if not convertor.filename.endswith(".glyphs"):
             return False
-        if "format" in kwargs and kwargs["format"] == 3:
-            return True
+        if "format" in kwargs:
+            return kwargs["format"] == 3
+        return True
 
     def _load_axes(self):
         self.axis_name_map = {}
         for gaxis in self.glyphs.get("axes", []):
             axis = Axis(name=gaxis["name"], tag=gaxis["tag"])
             self.axis_name_map[gaxis["name"]] = axis
             _maybesetformatspecific(axis, gaxis, "hidden")
@@ -678,15 +683,15 @@
             if pos:
                 metric["pos"] = pos
             if over:
                 metric["over"] = over
             gmaster["metricValues"].append(metric)
         if master.guides:
             gmaster["guides"] = [self._save_guide(g) for g in master.guides]
-        _copyattrs(master, gmaster, ["name", "id"])
+        _copyattrs(master, gmaster, ["name", "id"], convertor=str)
         return gmaster
 
     def _save_guide(self, guide):
         gguide = _moveformatspecific(guide)
         gguide["pos"] = tuple(guide.pos[0:2])
         if guide.pos[2]:
             gguide["angle"] = guide.pos[2]
@@ -708,15 +713,15 @@
         if not glyph.exported:
             gglyph["export"] = 0
         return gglyph
 
     def _save_layer(self, layer):
         glayer = _moveformatspecific(layer)
         _copyattrs(layer, glayer, ["width", "name"])
-        glayer["layerId"] = layer.id
+        glayer["layerId"] = str(layer.id)
         if layer.guides:
             glayer["guides"] = [self._save_guide(g) for g in layer.guides]
         if layer.shapes:
             glayer["shapes"] = [self._save_shape(s) for s in layer.shapes]
         if layer._master and layer._master != layer.id:
             glayer["associatedMasterId"] = layer._master
         return glayer
@@ -777,14 +782,14 @@
 def _moveformatspecific(item):
     rv = {}
     if "com.glyphsapp" in item._formatspecific:
         rv = {**item._formatspecific.get("com.glyphsapp", {})}
     return rv
 
 
-def _copyattrs(src, dst, attrs):
+def _copyattrs(src, dst, attrs, convertor = lambda x:x):
     for a in attrs:
         v = getattr(src, a)
         if isinstance(v, I18NDictionary):
             v = v.get_default()
         if v:
-            dst[a] = v
+            dst[a] = convertor(v)
```

### Comparing `babelfont-3.0.0a9/src/babelfont/convertors/gsobject.py` & `babelfont-3.0.1/src/babelfont/convertors/gsobject.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,15 +344,16 @@
             featurefile = featurefile + f.code
         for f in self.gsfont.features:
             tag = f.name
             feacode = "feature %s { %s\n} %s;" % (tag, f.code, tag)
             featurefile = featurefile + feacode
 
         try:
-            feaparser = FeaParser(featurefile)
+            glyphNames = {g.name for g in self.font.glyphs}
+            feaparser = FeaParser(featurefile, glyphNames=glyphNames)
             ast = feaparser.parser.ast
             for name, members in self.font.features.namedClasses.items():
                 glyphclass = ast.GlyphClassDefinition(
                     name, ast.GlyphClass([m for m in members])
                 )
                 feaparser.parser.glyphclasses_.define(name, glyphclass)
             feaparser.parse()
```

### Comparing `babelfont-3.0.0a9/src/babelfont/convertors/nfsf.py` & `babelfont-3.0.1/src/babelfont/convertors/nfsf.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import orjson
 import os
 
 
 # One would hope this would be easy.
 
 
-class NFSF(BaseConvertor):
-    suffix = ".nfsf"
+class Babelfont(BaseConvertor):
+    suffix = ".babelfont"
 
     def _load_file(self, filename):
         contents = open(os.path.join(self.filename, filename), "r").read()
         return orjson.loads(contents)
 
     def _load(self):
         names = self._load_file("names.json")
@@ -34,15 +34,15 @@
         self.font.instances = [Instance(**j) for j in info.get("instances", [])]
 
         self._load_masters(info.get("masters", []))
 
         for g in glyphs:
             glyph = Glyph(**g)
             self.font.glyphs.append(glyph)
-            for json_layer in self._load_file(glyph.nfsf_filename):
+            for json_layer in self._load_file(glyph.babelfont_filename):
                 layer = self._inflate_layer(json_layer)
                 glyph.layers.append(layer)
 
         self._load_metadata(info)
         self._load_features()
         return self.font
 
@@ -100,10 +100,10 @@
         with open(path / "features.xml", "wb") as f:
             f.write(etree.tostring(self.font.features.toXML(), pretty_print=True))
 
         with open(path / "glyphs.json", "wb") as f:
             for g in self.font.glyphs:
                 glyphpath = path / "glyphs"
                 glyphpath.mkdir(parents=True, exist_ok=True)
-                with open(path / g.nfsf_filename, "wb") as f2:
+                with open(path / g.babelfont_filename, "wb") as f2:
                     g._write_value(f2, "layers", g.layers)
             self.font._write_value(f, "glyphs", self.font.glyphs)
```

### Comparing `babelfont-3.0.0a9/src/babelfont/convertors/truetype.py` & `babelfont-3.0.1/src/babelfont/convertors/truetype.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from datetime import datetime
 from babelfont import *
 from fontTools.fontBuilder import FontBuilder
 from fontTools.pens.ttGlyphPen import TTGlyphPen
 from fontTools.pens.recordingPen import RecordingPen
 from cu2qu.ufo import glyphs_to_quadratic
 from fontTools.misc.timeTools import epoch_diff, timestampSinceEpoch
-from fontTools.ttLib.ttFont import _TTGlyphGlyf, _TTGlyphSet
 from fontTools.ttLib.tables.TupleVariation import TupleVariation
 from babelfont.fontFilters.featureWriters import build_all_features
 from fontTools.ttLib import TTFont
 from fontTools.ttLib.tables._g_l_y_f import GlyphCoordinates
 from fontTools.varLib.iup import iup_delta_optimize
 from fontTools.misc.fixedTools import otRound
+from fontFeatures.ttLib import unparse
+from fontFeatures import Attachment
 import uuid
 from itertools import chain
 
 
 def _categorize_glyph(font,glyphname):
     if "GDEF" not in font: return None
+    if not font["GDEF"].table.GlyphClassDef:
+        return None
     classdefs = font["GDEF"].table.GlyphClassDef.classDefs
     if glyphname not in classdefs:
         return None
     if classdefs[glyphname] == 1: return "base"
     if classdefs[glyphname] == 2: return "ligature"
     if classdefs[glyphname] == 3: return "mark"
     if classdefs[glyphname] == 4: return "component"
@@ -38,14 +41,15 @@
     def _load(self):
         self.tt = TTFont(self.filename)
         self._load_fvar()
         self._load_head()
         self._load_masters()
         self._load_names()
         self._load_glyphs()
+        self._load_features()
         return self.font
 
     def _load_fvar(self):
         avar = self.tt.get("avar")
         if "fvar" in self.tt:
             for axis in self.tt["fvar"].axes:
                 name = self.tt["name"].getDebugName(axis.axisNameID)  # XXX multilingual
@@ -72,16 +76,16 @@
                     )
                 )
 
     def _load_masters(self):
         m = Master(location={},name="Default", id=str(uuid.uuid1()) )
         # Metrics
         m.metrics = {
-            "xHeight": self.tt["OS/2"].sxHeight,
-            "capHeight": self.tt["OS/2"].sCapHeight,
+            "xHeight": self.tt["OS/2"].sxHeight if hasattr(self.tt["OS/2"], "sxHeight") else None,
+            "capHeight": self.tt["OS/2"].sCapHeight  if hasattr(self.tt["OS/2"], "capHeight") else None,
             "ascender": self.tt["hhea"].ascender,
             "descender": self.tt["hhea"].descender
         }
         m.font = self.font
         self.font.masters = [m]
         if "fvar" in self.tt:
             m.location = {axis.tag: axis.default for axis in self.font.axes}
@@ -111,26 +115,21 @@
             category = _categorize_glyph(self.tt, glyph) or "base"
             glyphs_dict[glyph] = Glyph(name=glyph, codepoints=list(mapping.get(glyph, [])), category=category)
             self.font.glyphs.append(glyphs_dict[glyph])
             glyphs_dict[glyph].layers = self._load_layers(glyph)
         return glyphs_dict
 
     def _load_layers(self, g):
-        ttglyph = self.tt.getGlyphSet()[g]._glyph  # _TTGlyphGlyf object
+        ttglyph = self.tt.getGlyphSet()[g]  # _TTGlyphGlyf object
         width = self.tt["hmtx"][g][0]
         # leftMargin = self.tt["hmtx"][g][1]
         layer = Layer(width=width, id=str(uuid.uuid1()) )
         layer._master = self.font.masters[0].id
         layer._font = self.font
-        for i in range(0, max(ttglyph.numberOfContours, 0)):
-            layer.shapes.append(self._load_contour(ttglyph, i))
-        if hasattr(ttglyph, "components"):
-            for c in ttglyph.components:
-                comp = self._load_component(c)
-                layer.shapes.append(comp)
+        ttglyph.draw(layer.getPen())
         return [layer]
 
 
     def _load_contour(self, ttglyph, index):
         shape = Shape()
         shape.nodes = []
         endPt = ttglyph.endPtsOfContours[index]
@@ -190,15 +189,15 @@
             layer = f.default_master.get_glyph_layer(g)
             metrics[g] = (layer.width, layer.lsb)
 
         fb.setupHorizontalMetrics(metrics)
 
         for m in f.masters:
             glyf = {}
-            m.ttglyphset = _TTGlyphSet(fb.font, glyf, _TTGlyphGlyf)
+            m.ttglyphset = {}
 
         done = {}
 
         def do_a_glyph(g):
             if g in done:
                 return
             layer = f.default_master.get_glyph_layer(g)
@@ -213,34 +212,34 @@
             try:
                 glyphs_to_quadratic(all_outlines[g], reverse_direction=True)
                 for ix, m in enumerate(f.masters):
                     layer = m.get_glyph_layer(g)
                     pen = TTGlyphPen(m.ttglyphset)
                     layer.draw(pen)
 
-                    m.ttglyphset._glyphs[g] = pen.glyph()
+                    m.ttglyphset[g] = pen.glyph()
 
             except Exception as e:
                 print(
                     "Problem converting glyph %s to quadratic. (Probably incompatible) "
                     % g
                 )
                 for m in f.masters:
-                    m.ttglyphset._glyphs[g] = TTGlyphPen(m.ttglyphset).glyph()
+                    m.ttglyphset[g] = TTGlyphPen(m.ttglyphset).glyph()
             done[g] = True
 
         for g in exportable:
             do_a_glyph(g)
 
         fb.updateHead(
             fontRevision=f.version[0] + f.version[1] / 10 ** len(str(f.version[1])),
             created=timestampSinceEpoch(f.date.timestamp()),
             lowestRecPPEM=10,
         )
-        fb.setupGlyf(f.default_master.ttglyphset._glyphs)
+        fb.setupGlyf(f.default_master.ttglyphset)
         fb.setupHorizontalHeader(
             ascent=int(f.default_master.ascender),
             descent=int(f.default_master.descender),
         )
 
         f.names.typographicSubfamily = f.default_master.name
         f.names.typographicFamily = f.names.familyName
@@ -292,50 +291,73 @@
             if "post" in font and font["post"].formatType == 2.0:
                 font["post"].extraNames = []
                 font["post"].compile(font)
             font.save(self.filename)
 
     def calculate_a_gvar(self, f, model, g, default_width):
         master_layer = f.default_master.get_glyph_layer(g)
-        if not g in f.default_master.ttglyphset._glyphs:
+        if not g in f.default_master.ttglyphset:
             return None
-        default_g = f.default_master.ttglyphset._glyphs[g]
+        default_g = f.default_master.ttglyphset[g]
         all_coords = []
         for m in f.masters:
             layer = m.get_glyph_layer(g)
-            basecoords = GlyphCoordinates(m.ttglyphset._glyphs[g].coordinates)
-            if m.ttglyphset._glyphs[g].isComposite():
+            basecoords = GlyphCoordinates(m.ttglyphset[g].coordinates)
+            if m.ttglyphset[g].isComposite():
                 component_point = GlyphCoordinates(
                     [
-                        (layer_comp.pos[0], layer_comp.pos[1])
+                        (otRound(layer_comp.pos[0]), otRound(layer_comp.pos[1]))
                         for layer_comp in layer.components
                     ]
                 )
                 basecoords.extend(component_point)
-            phantomcoords = GlyphCoordinates([(0, 0), (layer.width, 0), (0, 0), (0, 0)])
+            phantomcoords = GlyphCoordinates([(0, 0), (otRound(layer.width), 0), (0, 0), (0, 0)])
             basecoords.extend(phantomcoords)
             all_coords.append(basecoords)
+        for ix,c in enumerate(all_coords):
+            all_ok = True
+            if len(c) != len(all_coords[0]):
+                print("Incompatible master %i in glyph %s" % (ix, g))
+                all_ok = False
+            if not all_ok:
+                return []
         deltas = model.getDeltas(all_coords)
         gvar_entry = []
         if default_g.isComposite():
             endPts = list(range(len(default_g.components)))
         else:
             endPts = default_g.endPtsOfContours
 
         for delta, sup in zip(deltas, model.supports):
             if not sup:
                 continue
-            var = TupleVariation(sup, delta)
+            var = TupleVariation(sup, round(delta))
             # This assumes we do the default master first, which may not be true
-            delta_opt = iup_delta_optimize(delta, deltas[0], endPts, tolerance=0.5)
+            delta_opt = iup_delta_optimize(round(delta), round(deltas[0]), endPts, tolerance=0.5)
             if None in delta_opt:
                 var = TupleVariation(sup, delta_opt)
             gvar_entry.append(var)
         return gvar_entry
 
+    def _load_features(self):
+        self.font.features = unparse(self.tt)
+        # Load anchors
+        for routine in self.font.features.routines:
+            for rule in routine.rules:
+                if isinstance(rule, Attachment):
+                    for glyphname, pos in rule.bases.items():
+                        self._add_anchor(glyphname, pos, rule.base_name)
+                    for glyphname, pos in rule.marks.items():
+                        self._add_anchor(glyphname, pos, rule.mark_name)
+
+    def _add_anchor(self, glyphname, pos, name):
+        # Would be nice if this was variable.
+        layer = self.font.default_master.get_glyph_layer(glyphname)
+        layer.anchors.append(Anchor(name=name, x=pos[0], y=pos[1]))
+
     # import numpy as np
     # def calculate_a_gvar(self, f, model, g, default_width):
     #     if not g in f.default_master.ttglyphset._glyphs:
     #         return None
 
     #     all_coords = []
     #     master_ix = f.masters.index(f.default_master)
```

### Comparing `babelfont-3.0.0a9/src/babelfont/fontFilters/featureWriters.py` & `babelfont-3.0.1/src/babelfont/fontFilters/featureWriters.py`

 * *Files identical despite different names*

