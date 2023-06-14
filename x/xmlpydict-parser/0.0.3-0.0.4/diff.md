# Comparing `tmp/xmlpydict_parser-0.0.3.tar.gz` & `tmp/xmlpydict_parser-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmlpydict_parser-0.0.3.tar", last modified: Wed Jun 14 04:11:27 2023, max compression
+gzip compressed data, was "xmlpydict_parser-0.0.4.tar", last modified: Wed Jun 14 23:40:29 2023, max compression
```

## Comparing `xmlpydict_parser-0.0.3.tar` & `xmlpydict_parser-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 04:11:27.515644 xmlpydict_parser-0.0.3/
--rw-rw-rw-   0        0        0     1096 2023-06-14 04:08:31.000000 xmlpydict_parser-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       34 2023-06-14 04:08:31.000000 xmlpydict_parser-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1686 2023-06-14 04:11:27.515127 xmlpydict_parser-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      660 2023-06-14 04:08:31.000000 xmlpydict_parser-0.0.3/README.md
--rw-rw-rw-   0        0        0     1164 2023-06-14 04:08:31.000000 xmlpydict_parser-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 04:11:27.515644 xmlpydict_parser-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-06-14 04:08:31.000000 xmlpydict_parser-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:11:27.499052 xmlpydict_parser-0.0.3/src/
--rw-rw-rw-   0        0        0     6216 2023-06-14 04:08:31.000000 xmlpydict_parser-0.0.3/src/xmlparse.cpp
-drwxrwxrwx   0        0        0        0 2023-06-14 04:11:27.513052 xmlpydict_parser-0.0.3/src/xmlpydict_parser.egg-info/
--rw-rw-rw-   0        0        0     1686 2023-06-14 04:11:27.000000 xmlpydict_parser-0.0.3/src/xmlpydict_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2023-06-14 04:11:27.000000 xmlpydict_parser-0.0.3/src/xmlpydict_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 04:11:27.000000 xmlpydict_parser-0.0.3/src/xmlpydict_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-14 04:11:27.000000 xmlpydict_parser-0.0.3/src/xmlpydict_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-14 04:11:27.000000 xmlpydict_parser-0.0.3/src/xmlpydict_parser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-14 04:11:27.514052 xmlpydict_parser-0.0.3/tests/
--rw-rw-rw-   0        0        0     6359 2023-06-14 04:08:31.000000 xmlpydict_parser-0.0.3/tests/test_parse.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:40:29.965183 xmlpydict_parser-0.0.4/
+-rw-rw-rw-   0        0        0     1096 2023-06-14 04:08:31.000000 xmlpydict_parser-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-06-14 04:08:31.000000 xmlpydict_parser-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1776 2023-06-14 23:40:29.965183 xmlpydict_parser-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      739 2023-06-14 23:35:07.000000 xmlpydict_parser-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1178 2023-06-14 23:36:14.000000 xmlpydict_parser-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 23:40:29.966184 xmlpydict_parser-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-06-14 21:11:19.000000 xmlpydict_parser-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:40:29.951185 xmlpydict_parser-0.0.4/src/
+-rw-rw-rw-   0        0        0     6663 2023-06-14 23:31:43.000000 xmlpydict_parser-0.0.4/src/xmlparse.cpp
+drwxrwxrwx   0        0        0        0 2023-06-14 23:40:29.963183 xmlpydict_parser-0.0.4/src/xmlpydict_parser.egg-info/
+-rw-rw-rw-   0        0        0     1776 2023-06-14 23:40:29.000000 xmlpydict_parser-0.0.4/src/xmlpydict_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2023-06-14 23:40:29.000000 xmlpydict_parser-0.0.4/src/xmlpydict_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 23:40:29.000000 xmlpydict_parser-0.0.4/src/xmlpydict_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-14 23:40:29.000000 xmlpydict_parser-0.0.4/src/xmlpydict_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-14 23:40:29.000000 xmlpydict_parser-0.0.4/src/xmlpydict_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 23:40:29.964182 xmlpydict_parser-0.0.4/tests/
+-rw-rw-rw-   0        0        0     6359 2023-06-14 04:08:31.000000 xmlpydict_parser-0.0.4/tests/test_parse.py
```

### Comparing `xmlpydict_parser-0.0.3/LICENSE` & `xmlpydict_parser-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xmlpydict_parser-0.0.3/PKG-INFO` & `xmlpydict_parser-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: xmlpydict_parser
-Version: 0.0.3
+Version: 0.0.4
 Summary: xml to dictionary tool for python
 Author-email: Matthew Taylor <matthew.taylor.andre@gmail.com>
 Project-URL: Homepage, https://github.com/MatthewAndreTaylor/xml-to-pydict
-Keywords: xml
+Keywords: xml,dictionary
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -40,13 +40,11 @@
 ```
 
 ## Quickstart
 
 ```py
 >>> from xmlpydict_parser import parse
 >>> parse("<package><xmlpydict_parser language='python'/></package>")
-{
-    'package': {
-        'xmlpydict_parser' : { '@language' = 'python'}
-    }
-}
+{'package': {'xmlpydict_parser': {'@language': 'python'}}}
+>>> parse("<person name='Matthew'>Hello!</person>")
+{'person': {'@name': 'Matthew', '#text': 'Hello!'}}
 ```
```

### Comparing `xmlpydict_parser-0.0.3/README.md` & `xmlpydict_parser-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -16,13 +16,11 @@
 ```
 
 ## Quickstart
 
 ```py
 >>> from xmlpydict_parser import parse
 >>> parse("<package><xmlpydict_parser language='python'/></package>")
-{
-    'package': {
-        'xmlpydict_parser' : { '@language' = 'python'}
-    }
-}
+{'package': {'xmlpydict_parser': {'@language': 'python'}}}
+>>> parse("<person name='Matthew'>Hello!</person>")
+{'person': {'@name': 'Matthew', '#text': 'Hello!'}}
 ```
```

### Comparing `xmlpydict_parser-0.0.3/pyproject.toml` & `xmlpydict_parser-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = [ "setuptools>=61.0", "wheel" ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xmlpydict_parser"
-version = "0.0.3"
+version = "0.0.4"
 description="xml to dictionary tool for python"
 authors = [
     {name = "Matthew Taylor", email = "matthew.taylor.andre@gmail.com"},
 ]
 urls = {Homepage = "https://github.com/MatthewAndreTaylor/xml-to-pydict"}
 requires-python = ">=3.7"
-keywords = [ "xml" ]
+keywords = [ "xml", "dictionary" ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
```

### Comparing `xmlpydict_parser-0.0.3/setup.py` & `xmlpydict_parser-0.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,10 +15,9 @@
 
 setup(
     include_package_data=True,
     ext_modules=[
         Extension("xmlpydict_parser", ["src/xmlparse.cpp"]),
     ],
     cmdclass={"build_ext": build_ext},
-    package_data={"xmlpydict_parser": ["py.typed"]},
-    universal=True,
+    package_data={"xmlpydict_parser": ["py.typed"]}
 )
```

### Comparing `xmlpydict_parser-0.0.3/src/xmlparse.cpp` & `xmlpydict_parser-0.0.4/src/xmlparse.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 typedef struct Node {
   PrimitiveType type;
   std::string elementName;
   std::vector<Pair> attr;
 } PathNode;
 
 std::regex primitiveRegex(".*<([a-zA-Z_]+)", std::regex_constants::icase);
-std::regex attrRegex(R"(([a-zA-Z][a-zA-Z0-9_-]*)=\"([^\"]*)\")",
+std::regex attrRegex(R"(([a-zA-Z][a-zA-Z0-9_-]*)\s*=\s*\"([^\"]*)\")",
+                     std::regex_constants::icase);
+std::regex attrRegexSingle(R"(([a-zA-Z][a-zA-Z0-9_-]*)\s*=\s*\'([^\']*)\')",
                      std::regex_constants::icase);
 std::regex selfclosingRegex(R"(\/>)", std::regex_constants::icase);
 std::regex closingtagRegex(R"(</\w+>)", std::regex_constants::icase);
 std::regex notCommentRegex("^(?!<!--)[\\s\\S]*?(?!-->)$");
 
 PathNode ParsePrimitive(std::string &input) {
   std::smatch match;
@@ -49,23 +51,32 @@
     return p;
   }
   std::string::size_type pos = (match.size() > 0) ? match[0].length() : 0;
 
   std::string attributes = input.substr(pos);
 
   std::sregex_iterator it(attributes.begin(), attributes.end(), attrRegex);
+  std::sregex_iterator itt(attributes.begin(), attributes.end(), attrRegexSingle);
   std::sregex_iterator end;
 
   while (it != end) {
     std::smatch match = *it;
     std::string attrName = match.str(1);
     std::string attrValue = match.str(2);
     p.attr.push_back({std::move(attrName), std::move(attrValue)});
     ++it;
   }
+
+  while (itt != end) {
+    std::smatch match = *itt;
+    std::string attrName = match.str(1);
+    std::string attrValue = match.str(2);
+    p.attr.push_back({std::move(attrName), std::move(attrValue)});
+    ++itt;
+  }
   return p;
 }
 
 std::vector<std::string> splitNodes(const std::string &xmlContent) {
   std::vector<std::string> nodes;
   std::istringstream xmlStream(xmlContent);
   std::string line;
```

### Comparing `xmlpydict_parser-0.0.3/src/xmlpydict_parser.egg-info/PKG-INFO` & `xmlpydict_parser-0.0.4/src/xmlpydict_parser.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: xmlpydict-parser
-Version: 0.0.3
+Version: 0.0.4
 Summary: xml to dictionary tool for python
 Author-email: Matthew Taylor <matthew.taylor.andre@gmail.com>
 Project-URL: Homepage, https://github.com/MatthewAndreTaylor/xml-to-pydict
-Keywords: xml
+Keywords: xml,dictionary
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -40,13 +40,11 @@
 ```
 
 ## Quickstart
 
 ```py
 >>> from xmlpydict_parser import parse
 >>> parse("<package><xmlpydict_parser language='python'/></package>")
-{
-    'package': {
-        'xmlpydict_parser' : { '@language' = 'python'}
-    }
-}
+{'package': {'xmlpydict_parser': {'@language': 'python'}}}
+>>> parse("<person name='Matthew'>Hello!</person>")
+{'person': {'@name': 'Matthew', '#text': 'Hello!'}}
 ```
```

### Comparing `xmlpydict_parser-0.0.3/tests/test_parse.py` & `xmlpydict_parser-0.0.4/tests/test_parse.py`

 * *Files identical despite different names*

