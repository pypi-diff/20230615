# Comparing `tmp/rico-0.2.2.tar.gz` & `tmp/rico-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rico-0.2.2.tar", last modified: Tue Jun 13 17:20:45 2023, max compression
+gzip compressed data, was "rico-0.2.3.tar", last modified: Thu Jun 15 16:18:20 2023, max compression
```

## Comparing `rico-0.2.2.tar` & `rico-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-06-13 17:20:06.004287 rico-0.2.2/LICENSE
--rw-r--r--   0        0        0      706 2023-06-13 17:20:06.004287 rico-0.2.2/README.md
--rw-r--r--   0        0        0     2870 2023-06-13 17:20:45.016727 rico-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      491 2023-06-13 17:20:06.008287 rico-0.2.2/src/rico/__init__.py
--rw-r--r--   0        0        0     5471 2023-06-13 17:20:06.008287 rico-0.2.2/src/rico/_config.py
--rw-r--r--   0        0        0     5605 2023-06-13 17:20:06.008287 rico-0.2.2/src/rico/_container.py
--rw-r--r--   0        0        0    14546 2023-06-13 17:20:06.008287 rico-0.2.2/src/rico/_content.py
--rw-r--r--   0        0        0     7015 2023-06-13 17:20:06.008287 rico-0.2.2/src/rico/_html.py
--rw-r--r--   0        0        0      340 2023-06-13 17:20:06.008287 rico-0.2.2/src/rico/_version.py
--rw-r--r--   0        0        0       18 2023-06-13 17:20:06.008287 rico-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     1476 2023-06-13 17:20:06.008287 rico-0.2.2/tests/test__config.py
--rw-r--r--   0        0        0    10251 2023-06-13 17:20:06.008287 rico-0.2.2/tests/test__container.py
--rw-r--r--   0        0        0    16739 2023-06-13 17:20:06.008287 rico-0.2.2/tests/test__content.py
--rw-r--r--   0        0        0     9501 2023-06-13 17:20:06.008287 rico-0.2.2/tests/test__html.py
--rw-r--r--   0        0        0      730 2023-06-13 17:20:06.008287 rico-0.2.2/tests/test__version.py
--rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 rico-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-15 16:17:52.853613 rico-0.2.3/LICENSE
+-rw-r--r--   0        0        0      706 2023-06-15 16:17:52.853613 rico-0.2.3/README.md
+-rw-r--r--   0        0        0     2870 2023-06-15 16:18:20.949893 rico-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      491 2023-06-15 16:17:52.853613 rico-0.2.3/src/rico/__init__.py
+-rw-r--r--   0        0        0     5471 2023-06-15 16:17:52.853613 rico-0.2.3/src/rico/_config.py
+-rw-r--r--   0        0        0     5605 2023-06-15 16:17:52.853613 rico-0.2.3/src/rico/_container.py
+-rw-r--r--   0        0        0    14794 2023-06-15 16:17:52.853613 rico-0.2.3/src/rico/_content.py
+-rw-r--r--   0        0        0     7015 2023-06-15 16:17:52.853613 rico-0.2.3/src/rico/_html.py
+-rw-r--r--   0        0        0      340 2023-06-15 16:17:52.853613 rico-0.2.3/src/rico/_version.py
+-rw-r--r--   0        0        0       18 2023-06-15 16:17:52.853613 rico-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     1476 2023-06-15 16:17:52.853613 rico-0.2.3/tests/test__config.py
+-rw-r--r--   0        0        0    10251 2023-06-15 16:17:52.853613 rico-0.2.3/tests/test__container.py
+-rw-r--r--   0        0        0    17097 2023-06-15 16:17:52.853613 rico-0.2.3/tests/test__content.py
+-rw-r--r--   0        0        0     9501 2023-06-15 16:17:52.853613 rico-0.2.3/tests/test__html.py
+-rw-r--r--   0        0        0      730 2023-06-15 16:17:52.853613 rico-0.2.3/tests/test__version.py
+-rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 rico-0.2.3/PKG-INFO
```

### Comparing `rico-0.2.2/LICENSE` & `rico-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rico-0.2.2/README.md` & `rico-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `rico-0.2.2/pyproject.toml` & `rico-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Text Processing",
     "Topic :: Text Processing :: Markup",
     "Topic :: Text Processing :: Markup :: HTML",
     "Topic :: Text Processing :: Markup :: Markdown",
 ]
-version = "0.2.2"
+version = "0.2.3"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 source = "https://github.com/e10v/rico"
 "release notes" = "https://github.com/e10v/rico/releases"
```

### Comparing `rico-0.2.2/src/rico/_config.py` & `rico-0.2.3/src/rico/_config.py`

 * *Files identical despite different names*

### Comparing `rico-0.2.2/src/rico/_container.py` & `rico-0.2.3/src/rico/_container.py`

 * *Files identical despite different names*

### Comparing `rico-0.2.2/src/rico/_content.py` & `rico-0.2.3/src/rico/_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,14 +264,17 @@
         """
         super().__init__(class_)
 
         if isinstance(data, str):
             data = data.encode()
         encoded_image = base64.b64encode(data).decode()
 
+        if format == "svg":
+            format = "svg+xml"  # noqa: A001
+
         element = ET.Element(
             "img",
             attrib={"src": f"data:image/{format};base64,{encoded_image}"},
         )
         self.container.append(element)
 
 
@@ -349,26 +352,31 @@
 
         Args:
             *objects: The objects which are used to create a content.
             class_: The container class attribute.
         """
         super().__init__(class_=class_)
         for obj in objects:
-            if (
+            if isinstance(obj, ContentBase):
+                elements = (obj.container,)
+            elif (
                 alt is not None and isinstance(obj, alt.TopLevelMixin) or
                 plt is not None and isinstance(obj, plt.Axes | plt.Figure) or  # type: ignore  # noqa: E501
                 so is not None and isinstance(obj, so.Plot)
             ):
-                content = Chart(obj)
+                elements = Chart(obj).container
             elif hasattr(obj, "_repr_html_") and callable(obj._repr_html_):
-                content = HTML(obj._repr_html_(), strip_dataframe_borders=True)
+                elements = HTML(
+                    obj._repr_html_(),
+                    strip_dataframe_borders=True,
+                ).container
             else:
-                content = Text(obj)
+                elements = Text(obj).container
 
-            for element in content.container:
+            for element in elements:
                 self.container.append(element)
 
 
 class Script(ContentBase):
     """A script definition.
 
     Attributes:
```

### Comparing `rico-0.2.2/src/rico/_html.py` & `rico-0.2.3/src/rico/_html.py`

 * *Files identical despite different names*

### Comparing `rico-0.2.2/tests/test__config.py` & `rico-0.2.3/tests/test__config.py`

 * *Files identical despite different names*

### Comparing `rico-0.2.2/tests/test__container.py` & `rico-0.2.3/tests/test__container.py`

 * *Files identical despite different names*

### Comparing `rico-0.2.2/tests/test__content.py` & `rico-0.2.3/tests/test__content.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,15 +328,15 @@
     assert div.text is None
     assert div.tail is None
     assert len(div) == 1
 
     img = tuple(div)[0]
     assert isinstance(img, ET.Element)
     assert img.tag == "img"
-    assert img.attrib == {"src": f"data:image/svg;base64,{encoded_image}"}
+    assert img.attrib == {"src": f"data:image/svg+xml;base64,{encoded_image}"}
     assert img.text is None
     assert img.tail is None
     assert len(img) == 0
 
 
 @pytest.mark.parametrize("data", [svg_data, svg_data.encode()], ids=["str", "bytes"])
 def test_image_png(data: str | bytes):
@@ -420,44 +420,60 @@
 
 
 def test_obj():
     class ReprHTML:
         def _repr_html_(self) -> str:
             return "<h1>Hello</h1>"
 
-    content = rico._content.Obj(ReprHTML(), "world", pyplot_axes, class_="row")
+    content_base = rico._content.ContentBase(class_="col")
 
-    div = content.container
-    assert isinstance(div, ET.Element)
-    assert div.tag == "div"
-    assert div.attrib == {"class": "row"}
-    assert div.text is None
-    assert div.tail is None
-    assert len(div) == 3
+    content = rico._content.Obj(
+        ReprHTML(),
+        "world",
+        pyplot_axes,
+        content_base,
+        class_="row",
+    )
+
+    div0 = content.container
+    assert isinstance(div0, ET.Element)
+    assert div0.tag == "div"
+    assert div0.attrib == {"class": "row"}
+    assert div0.text is None
+    assert div0.tail is None
+    assert len(div0) == 4
 
-    h1 = tuple(div)[0]
+    h1 = tuple(div0)[0]
     assert isinstance(h1, ET.Element)
     assert h1.tag == "h1"
     assert h1.attrib == {}
     assert h1.text == "Hello"
     assert h1.tail is None
     assert len(h1) == 0
 
-    p = tuple(div)[1]
+    p = tuple(div0)[1]
     assert isinstance(p, ET.Element)
     assert p.tag == "p"
     assert p.attrib == {}
     assert p.text == "world"
     assert p.tail is None
     assert len(p) == 0
 
-    img = tuple(div)[2]
+    img = tuple(div0)[2]
     assert isinstance(img, ET.Element)
     assert img.tag == "img"
 
+    div1 = tuple(div0)[3]
+    assert isinstance(div1, ET.Element)
+    assert div1.tag == "div"
+    assert div1.attrib == {"class": "col"}
+    assert div1.text is None
+    assert div1.tail is None
+    assert len(div1) == 0
+
 
 @pytest.mark.parametrize("defer", [True, False], ids=["defer", "not defer"])
 def test_script_text(defer: bool):
     text = "alert('Hello World!');"
     attrib = {"async": True}
     content = rico._content.Script(text=text, defer=defer, attrib=attrib)
```

### Comparing `rico-0.2.2/tests/test__html.py` & `rico-0.2.3/tests/test__html.py`

 * *Files identical despite different names*

### Comparing `rico-0.2.2/tests/test__version.py` & `rico-0.2.3/tests/test__version.py`

 * *Files identical despite different names*

### Comparing `rico-0.2.2/PKG-INFO` & `rico-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rico
-Version: 0.2.2
+Version: 0.2.3
 Summary: Rich content to HTML as easy as Doc(df, plot).
 Author-Email: Evgeny Ivanov <ivanov.evgeny.n@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

