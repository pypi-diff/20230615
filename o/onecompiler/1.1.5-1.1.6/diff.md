# Comparing `tmp/onecompiler-1.1.5.tar.gz` & `tmp/onecompiler-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onecompiler-1.1.5.tar", max compression
+gzip compressed data, was "onecompiler-1.1.6.tar", max compression
```

## Comparing `onecompiler-1.1.5.tar` & `onecompiler-1.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-06-06 14:12:34.685634 onecompiler-1.1.5/LICENSE
--rw-r--r--   0        0        0     1036 2023-06-11 17:03:52.315001 onecompiler-1.1.5/README.md
--rw-r--r--   0        0        0      134 2023-06-11 17:03:52.319001 onecompiler-1.1.5/onecompiler/__init__.py
--rw-r--r--   0        0        0      143 2023-06-11 17:03:52.323001 onecompiler-1.1.5/onecompiler/api/__init__.py
--rw-r--r--   0        0        0     1752 2023-06-11 17:03:52.323001 onecompiler-1.1.5/onecompiler/api/async_compiler.py
--rw-r--r--   0        0        0     1645 2023-06-11 17:03:52.327001 onecompiler-1.1.5/onecompiler/api/compiler.py
--rw-r--r--   0        0        0      228 2023-06-06 18:35:35.538435 onecompiler-1.1.5/onecompiler/base_errors/LangNotFound.py
--rw-r--r--   0        0        0       89 2023-06-06 18:30:01.850435 onecompiler-1.1.5/onecompiler/base_errors/__init__.py
--rw-r--r--   0        0        0       90 2023-06-06 19:02:01.546434 onecompiler-1.1.5/onecompiler/base_models/__init__.py
--rw-r--r--   0        0        0     1781 2023-06-11 17:03:52.327001 onecompiler-1.1.5/onecompiler/base_models/base_compiler.py
--rw-r--r--   0        0        0     2493 2023-06-11 17:03:52.331001 onecompiler-1.1.5/onecompiler/data.py
--rw-r--r--   0        0        0      175 2023-06-11 17:03:52.331001 onecompiler-1.1.5/onecompiler/pydantic_models/__init__.py
--rw-r--r--   0        0        0      602 2023-06-11 17:03:52.335001 onecompiler-1.1.5/onecompiler/pydantic_models/lang.py
--rw-r--r--   0        0        0      791 2023-06-11 17:03:52.335001 onecompiler-1.1.5/onecompiler/pydantic_models/response.py
--rw-r--r--   0        0        0       14 2023-06-06 18:12:06.070434 onecompiler-1.1.5/onecompiler/requirements.txt
--rw-r--r--   0        0        0      385 2023-06-11 20:22:27.746813 onecompiler-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1756 1970-01-01 00:00:00.000000 onecompiler-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-06 14:12:34.685634 onecompiler-1.1.6/LICENSE
+-rw-r--r--   0        0        0     1034 2023-06-14 12:35:32.572296 onecompiler-1.1.6/README.md
+-rw-r--r--   0        0        0      134 2023-06-11 17:03:52.319001 onecompiler-1.1.6/onecompiler/__init__.py
+-rw-r--r--   0        0        0      143 2023-06-11 17:03:52.323001 onecompiler-1.1.6/onecompiler/api/__init__.py
+-rw-r--r--   0        0        0     1605 2023-06-14 12:35:32.572296 onecompiler-1.1.6/onecompiler/api/async_compiler.py
+-rw-r--r--   0        0        0     1561 2023-06-15 18:24:38.443050 onecompiler-1.1.6/onecompiler/api/compiler.py
+-rw-r--r--   0        0        0      239 2023-06-14 12:35:32.572296 onecompiler-1.1.6/onecompiler/base_errors/LangNotFound.py
+-rw-r--r--   0        0        0       89 2023-06-06 18:30:01.850435 onecompiler-1.1.6/onecompiler/base_errors/__init__.py
+-rw-r--r--   0        0        0       90 2023-06-06 19:02:01.546434 onecompiler-1.1.6/onecompiler/base_models/__init__.py
+-rw-r--r--   0        0        0     2289 2023-06-14 12:35:32.572296 onecompiler-1.1.6/onecompiler/base_models/base_compiler.py
+-rw-r--r--   0        0        0     1098 2023-06-14 12:35:32.572296 onecompiler-1.1.6/onecompiler/data.py
+-rw-r--r--   0        0        0      175 2023-06-11 17:03:52.331001 onecompiler-1.1.6/onecompiler/pydantic_models/__init__.py
+-rw-r--r--   0        0        0      602 2023-06-11 17:03:52.335001 onecompiler-1.1.6/onecompiler/pydantic_models/lang.py
+-rw-r--r--   0        0        0      791 2023-06-11 17:03:52.335001 onecompiler-1.1.6/onecompiler/pydantic_models/response.py
+-rw-r--r--   0        0        0       14 2023-06-06 18:12:06.070434 onecompiler-1.1.6/onecompiler/requirements.txt
+-rw-r--r--   0        0        0      385 2023-06-15 18:25:57.363051 onecompiler-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 onecompiler-1.1.6/PKG-INFO
```

### Comparing `onecompiler-1.1.5/LICENSE` & `onecompiler-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `onecompiler-1.1.5/README.md` & `onecompiler-1.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,18 +47,18 @@
 # Sample MySQL code
 res2 = compiler.query.mysql('SELECT 10')
 print(res2.stdout)
 # 10
 ```	
 Or
 ```
-res = compiler.compiler(lang='js', code='console.log("Hello");')
+res = compiler.compile(lang='js', code='console.log("Hello");')
 print(res.stdout)
 # Hello
 
-res2 = compiler.compiler(lang='mysql', code='SELECT 10')
+res2 = compiler.compile(lang='mysql', code='SELECT 10')
 print(res2.stdout)
 # 10
 ```
```

### Comparing `onecompiler-1.1.5/onecompiler/api/async_compiler.py` & `onecompiler-1.1.6/onecompiler/api/async_compiler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,50 @@
-from typing import Coroutine, Any
 from httpx import AsyncClient
 from onecompiler.base_models import BaseCompiler
 from onecompiler.pydantic_models import Response
+from onecompiler.base_errors import LangNotFound
+from onecompiler import data
 
 
 class ToLang:
     """Wrapper wrapper, for requests, programming languages type, when the request is known"""
-    def __init__(self, compiler) -> None:
-        self.compiler = compiler
+    def __init__(self, compiler, lang_type: str) -> None:
+        self.compiler: Compiler = compiler
+        self.lang_type = lang_type
 
     def __getattr__(self, lang: str):
-        async def func(code: str) -> Coroutine[Any, Any, Response]:
-            return await self.compiler.compiler(lang, code) 
+        async def func(code: str) -> Response:
+            _, lang_type = self.compiler._get_full_lang_name(lang)
+            
+            if lang_type is None:
+                raise LangNotFound
+            
+            if lang_type == self.lang_type:
+                return await self.compiler.compile(lang, code)
         return func
-	
-class QueryLang:
-    """Wrapper wrapper, for requests, database languages type, when the request is known"""
-    def __init__(self, compiler)  -> None:
-        self.compiler = compiler
 
-    def __getattr__(self, lang: str):
-        async def func(code: str) -> Coroutine[Any, Any, Response]:
-            if lang in self.compiler.query_langs:
-                return await self.compiler.compiler(lang, code) 
-        return func
 
 class AsyncCompiler(BaseCompiler):
-    """Asynchronous compiler execution"""
+    """Synchronous compiler execution"""
     def __init__(self) -> None:
         super().__init__()
         self._client = AsyncClient()
-        self.to = ToLang(self)
-        self.query = QueryLang(self)
-	
-    async def compiler(self, lang: str, code: str) -> Response:
+        
+        self.to = ToLang(self, 'programming')
+        self.query = ToLang(self, 'query')
+
+
+    async def compile(self, lang: str, code: str) -> Response:
         """
         compiles your code
 
         Args:
             lang (str): Programing language
             code (str): Сode that will be sent for compilation
 
         Returns:
             Response: Pydantic model
         """
-        lang_data = self._get_lang_data(lang, code)
-        lang_data.properties.files[0].content = code
-        res = await self._client.post(self._url, json=lang_data.dict(), headers=self._headers)
-        return Response.parse_obj(res.json())
-    
+        lang_data = self._get_lang_data(lang, code)        
+        
+        res = (await self._client.post(self._url, json=lang_data.dict(), headers=self._headers)).json()
+        return Response.parse_obj(res)
```

### Comparing `onecompiler-1.1.5/onecompiler/api/compiler.py` & `onecompiler-1.1.6/onecompiler/api/compiler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 from httpx import Client
 from onecompiler.base_models import BaseCompiler
 from onecompiler.pydantic_models import Response
+from onecompiler.base_errors import LangNotFound
+from onecompiler import data
 
 
 class ToLang:
     """Wrapper wrapper, for requests, programming languages type, when the request is known"""
-    def __init__(self, compiler) -> None:
+    def __init__(self, compiler, lang_type: str) -> None:
         self.compiler: Compiler = compiler
+        self.lang_type = lang_type
 
     def __getattr__(self, lang: str):
         def func(code: str) -> Response:
-            if lang in self.compiler.programming_langs:
-                return self.compiler.compiler(lang, code)
+            _, lang_type = self.compiler._get_full_lang_name(lang)
+            
+            if lang_type is None:
+                raise LangNotFound
+            
+            if lang_type == self.lang_type:
+                return self.compiler.compile(lang, code)
         return func
 
-class QueryLang:
-    """Wrapper wrapper, for requests, database languages type, when the request is known"""
-    def __init__(self, compiler) -> None:
-        self.compiler = compiler
-
-    def __getattr__(self, lang: str):
-        def func(code: str) -> Response:
-            if lang in self.compiler.query_langs:
-                return self.compiler.compiler(lang, code)
-        return func
 
 class Compiler(BaseCompiler):
     """Synchronous compiler execution"""
     def __init__(self) -> None:
         super().__init__()
 
         self._client = Client()
-        self.to = ToLang(self)
-        self.query = QueryLang(self)
+        self.to = ToLang(self, 'programming')
+        self.query = ToLang(self, 'query')
+
 
-    def compiler(self, lang: str, code: str) -> Response:
+    def compile(self, lang: str, code: str) -> Response:
         """
         compiles your code
 
         Args:
             lang (str): Programing language
             code (str): Сode that will be sent for compilation
 
         Returns:
             Response: Pydantic model
         """
         lang_data = self._get_lang_data(lang, code)        
+        
         res = self._client.post(self._url, json=lang_data.dict(), headers=self._headers).json()
         return Response.parse_obj(res)
```

### Comparing `onecompiler-1.1.5/onecompiler/base_models/base_compiler.py` & `onecompiler-1.1.6/onecompiler/base_models/base_compiler.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,44 +18,64 @@
 	programming_langs = data['programming'].keys()
 	query_langs = data['query'].keys()
 
 	all_languages = {i: list(data[i]) for i in data}
 
 
 	def _create_lang_data(self, lang, lang_type, code) -> dict:
-		full_name, extension = data[lang_type][lang]
+		#full_name = data[lang_type][lang]
 		
 		finall_data = {
-	    			"name": full_name,
-	    			"title": f"{full_name} Hello World",
+	    			"name": lang,
+	    			"title": f"{lang} Hello World",
 	    			"version": "latest",
-	    			"mode": full_name,
+	    			"mode": lang,
 	    			#"description": None,
-	    			"extension": extension,
+	    			"extension": lang,
 	    			"languageType": ("programming" if lang_type != 'query' else 'database'),
 	    			"active": True,
 	    			"properties": {
-	    				"language": full_name,
+	    				"language": lang,
 	    				"docs": True,
 	    				"tutorials": True,
 	    				"cheatsheets": True,
-	    				"files": [{"name": f"file.{extension}", "content": code}],
+	    				"files": [{"name": f"file.{lang}", "content": code}],
 	    			},
 	    			"visibility": "public",
-    		    }
+		    }
 
 		return finall_data
 
 
-	def _get_lang_data(self, lang: str, code: str) -> Lang:
-		""" You get a language config to send a POST request to the compiler """
+	def _get_full_lang_name(self, lang: str):
+		full_name = None
 		lang_type = None
-		
-		for lang_types in self.all_languages:
-			if lang in self.all_languages[lang_types]:
-				lang_type = lang_types
+
+		for langs in self.programming_langs:
+			if (lang == langs) or (lang in data['programming'][langs]):
+				lang_type = 'programming'
+				full_name = langs
 
 		if lang_type is None:
-			raise LangNotFound
+			for langs in self.query_langs:
+				if (lang == langs) or (lang in data['query'][langs]):
+					lang_type = 'query'
+					full_name = langs
+
+		if lang_type and full_name:
+			return (full_name, lang_type)
+		raise LangNotFound
+
 
-		lang_data = self._create_lang_data(lang, lang_type, code)#data[lang_type][lang]
+	def _get_lang_data(self, lang: str, code: str) -> Lang:
+		""" You get a language config to send a POST request to the compiler """
+		lang, lang_type = self._get_full_lang_name(lang)
+
+		lang_data = self._create_lang_data(lang, lang_type, code)
 		return Lang.parse_obj(lang_data)
+
+
+	def get_lang_reductions(self, lang):
+		""" Gets a list of abbreviated names for a specific language """
+		if lang in self.programming_langs:
+			return data['programming'].get(lang)
+		return data['query'].get(lang)
```

### Comparing `onecompiler-1.1.5/onecompiler/pydantic_models/lang.py` & `onecompiler-1.1.6/onecompiler/pydantic_models/lang.py`

 * *Files identical despite different names*

### Comparing `onecompiler-1.1.5/onecompiler/pydantic_models/response.py` & `onecompiler-1.1.6/onecompiler/pydantic_models/response.py`

 * *Files identical despite different names*

### Comparing `onecompiler-1.1.5/PKG-INFO` & `onecompiler-1.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onecompiler
-Version: 1.1.5
+Version: 1.1.6
 Summary: 
 Home-page: https://github.com/pokedim13/OneCompiler
 License: Apache-2.0
 Author: pokedim13
 Author-email: skinxedovich@vk.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -67,19 +67,19 @@
 # Sample MySQL code
 res2 = compiler.query.mysql('SELECT 10')
 print(res2.stdout)
 # 10
 ```	
 Or
 ```
-res = compiler.compiler(lang='js', code='console.log("Hello");')
+res = compiler.compile(lang='js', code='console.log("Hello");')
 print(res.stdout)
 # Hello
 
-res2 = compiler.compiler(lang='mysql', code='SELECT 10')
+res2 = compiler.compile(lang='mysql', code='SELECT 10')
 print(res2.stdout)
 # 10
 ```
```

