# Comparing `tmp/py_to_proto-0.3.0-py39-none-any.whl.zip` & `tmp/py_to_proto-0.3.1-py39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 32196 bytes, number of entries: 15
--rw-r--r--  2.0 unx     1174 b- defN 23-May-23 23:09 py_to_proto/__init__.py
--rw-r--r--  2.0 unx      251 b- defN 23-May-23 23:09 py_to_proto/compat_annotated.py
--rw-r--r--  2.0 unx    26041 b- defN 23-May-23 23:09 py_to_proto/converter_base.py
--rw-r--r--  2.0 unx    12098 b- defN 23-May-23 23:09 py_to_proto/dataclass_to_proto.py
--rw-r--r--  2.0 unx     9686 b- defN 23-May-23 23:09 py_to_proto/descriptor_to_file.py
--rw-r--r--  2.0 unx     5265 b- defN 23-May-23 23:09 py_to_proto/descriptor_to_message_class.py
--rw-r--r--  2.0 unx    12474 b- defN 23-May-23 23:09 py_to_proto/json_to_service.py
--rw-r--r--  2.0 unx     8288 b- defN 23-May-23 23:09 py_to_proto/jtd_to_proto.py
--rw-r--r--  2.0 unx    12598 b- defN 23-May-23 23:09 py_to_proto/utils.py
--rw-r--r--  2.0 unx    14885 b- defN 23-May-23 23:09 py_to_proto/validation.py
--rw-r--r--  2.0 unx     1088 b- defN 23-May-23 23:10 py_to_proto-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     6777 b- defN 23-May-23 23:10 py_to_proto-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 23-May-23 23:10 py_to_proto-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-23 23:10 py_to_proto-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1273 b- defN 23-May-23 23:10 py_to_proto-0.3.0.dist-info/RECORD
-15 files, 112003 bytes uncompressed, 30090 bytes compressed:  73.1%
+Zip file size: 32349 bytes, number of entries: 15
+-rw-r--r--  2.0 unx     1174 b- defN 23-Jun-14 22:47 py_to_proto/__init__.py
+-rw-r--r--  2.0 unx      251 b- defN 23-Jun-14 22:47 py_to_proto/compat_annotated.py
+-rw-r--r--  2.0 unx    26041 b- defN 23-Jun-14 22:47 py_to_proto/converter_base.py
+-rw-r--r--  2.0 unx    12764 b- defN 23-Jun-14 22:47 py_to_proto/dataclass_to_proto.py
+-rw-r--r--  2.0 unx     9686 b- defN 23-Jun-14 22:47 py_to_proto/descriptor_to_file.py
+-rw-r--r--  2.0 unx     5265 b- defN 23-Jun-14 22:47 py_to_proto/descriptor_to_message_class.py
+-rw-r--r--  2.0 unx    12474 b- defN 23-Jun-14 22:47 py_to_proto/json_to_service.py
+-rw-r--r--  2.0 unx     8288 b- defN 23-Jun-14 22:47 py_to_proto/jtd_to_proto.py
+-rw-r--r--  2.0 unx    12598 b- defN 23-Jun-14 22:47 py_to_proto/utils.py
+-rw-r--r--  2.0 unx    14885 b- defN 23-Jun-14 22:47 py_to_proto/validation.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-Jun-14 22:48 py_to_proto-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6777 b- defN 23-Jun-14 22:48 py_to_proto-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-14 22:48 py_to_proto-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-14 22:48 py_to_proto-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1273 b- defN 23-Jun-14 22:48 py_to_proto-0.3.1.dist-info/RECORD
+15 files, 112669 bytes uncompressed, 30243 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: py_to_proto/utils.py
 Comment: 
 
 Filename: py_to_proto/validation.py
 Comment: 
 
-Filename: py_to_proto-0.3.0.dist-info/LICENSE
+Filename: py_to_proto-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: py_to_proto-0.3.0.dist-info/METADATA
+Filename: py_to_proto-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: py_to_proto-0.3.0.dist-info/WHEEL
+Filename: py_to_proto-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: py_to_proto-0.3.0.dist-info/top_level.txt
+Filename: py_to_proto-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: py_to_proto-0.3.0.dist-info/RECORD
+Filename: py_to_proto-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## py_to_proto/dataclass_to_proto.py

```diff
@@ -247,16 +247,29 @@
         definitions for its
         """
         field_type = self._resolve_wrapped_type(field_def.type)
         oneof_fields = []
         if get_origin(field_type) is Union:
             for arg in get_args(field_type):
                 oneof_field_name = self._get_unique_annotation(arg, OneofField)
-                if oneof_field_name is None:
-                    res_type = self._resolve_wrapped_type(arg)
+                res_type = self._resolve_wrapped_type(arg)
+                # handle list type separately
+                if get_origin(res_type) is list:
+                    assert get_args(
+                        res_type
+                    ), f"List {arg} does not have any type argument"
+                    field_type = get_args(res_type)[0]
+                    oneof_field_name = oneof_field_name or (
+                        f"{field_def.name}_{str(field_type.__name__)}_sequence".lower()
+                    )
+                    arg = dataclasses.make_dataclass(
+                        f"{str(field_type.__name__).capitalize()}Sequence",
+                        [("values", List[field_type])],
+                    )
+                elif oneof_field_name is None:
                     oneof_field_name = (
                         f"{field_def.name}_{str(res_type.__name__)}".lower()
                     )
                     log.debug3("Using default oneof field name: %s", oneof_field_name)
                 oneof_fields.append((oneof_field_name, arg))
         return oneof_fields
```

## Comparing `py_to_proto-0.3.0.dist-info/LICENSE` & `py_to_proto-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `py_to_proto-0.3.0.dist-info/METADATA` & `py_to_proto-0.3.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-to-proto
-Version: 0.3.0
+Version: 0.3.1
 Summary: A tool to dynamically create protobuf message classes from python data schemas
 Home-page: https://github.com/IBM/py-to-proto
 Author: Gabe Goodhart
 Author-email: gabe.l.hart@gmail.com
 License: MIT
 Keywords: json,json typedef,jtd,protobuf,proto,dataclass
 Platform: UNKNOWN
```

## Comparing `py_to_proto-0.3.0.dist-info/RECORD` & `py_to_proto-0.3.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 py_to_proto/__init__.py,sha256=0xvSrTlGuMSPzey0U_v2i1ehBcFVzQRk3Z2qbFZiXO4,1174
 py_to_proto/compat_annotated.py,sha256=-JMeTz4v2hSkrRKVfQVqOlI1Az6IVqXoIC3ma2Fu2XI,251
 py_to_proto/converter_base.py,sha256=M_fO8qin-dklE19hPs9gyDTnjmjYvrRlwHdBOgzGLEw,26041
-py_to_proto/dataclass_to_proto.py,sha256=0nBudJ3PnH9v4GftjJYNBQFeGGCM5HkJRw54xAYFCAE,12098
+py_to_proto/dataclass_to_proto.py,sha256=hDndFVGkXw27-fMJ0vrv8DAeL5j_O3y072xX673sHM0,12764
 py_to_proto/descriptor_to_file.py,sha256=aVOJGMulF_xppS1n3MdjB8hStRXdnSH7Fkmhui6Xd2Q,9686
 py_to_proto/descriptor_to_message_class.py,sha256=2gJfz38W0_XLS4I3XI4Vtycok0-9q6kfSK7A_OYW2X4,5265
 py_to_proto/json_to_service.py,sha256=zzbJnXnXLeCPwRQsFYWnbzSKFgUBe-SpUeWYIKd7HCU,12474
 py_to_proto/jtd_to_proto.py,sha256=dmRj35Z5rfFgfeP2QRTaJ2sF1tZrYBD7KsyNY5yrCQ0,8288
 py_to_proto/utils.py,sha256=7bj45FqYORAzS-Yx0JmXFWeAuBSKFgubiOr628UX8o0,12598
 py_to_proto/validation.py,sha256=ssTE17roJwMYwTkRSuDUKL_JGAf1C3Ua0bcAsSPEtLE,14885
-py_to_proto-0.3.0.dist-info/LICENSE,sha256=t-ZkY-vak1QWjzid8VIzMds6wT0xEafbk406cLmdj_Q,1088
-py_to_proto-0.3.0.dist-info/METADATA,sha256=v8jJQpNtcNrLRU6P4eo51dVMHrKwjdZxqvoZGGpsTGE,6777
-py_to_proto-0.3.0.dist-info/WHEEL,sha256=ijjRDmPkGsL9eKpOeSzmTjLbiyw0Dy8TY4QGa2Zy9J8,93
-py_to_proto-0.3.0.dist-info/top_level.txt,sha256=AScY99r2vRxOMZGEg6sfYg7B5BlIyy9sXKc6CrlBR5s,12
-py_to_proto-0.3.0.dist-info/RECORD,,
+py_to_proto-0.3.1.dist-info/LICENSE,sha256=t-ZkY-vak1QWjzid8VIzMds6wT0xEafbk406cLmdj_Q,1088
+py_to_proto-0.3.1.dist-info/METADATA,sha256=LpDznfMXgKTYP6mOlz-XplTqbER_Qlbpm8WkiY8rWNA,6777
+py_to_proto-0.3.1.dist-info/WHEEL,sha256=ijjRDmPkGsL9eKpOeSzmTjLbiyw0Dy8TY4QGa2Zy9J8,93
+py_to_proto-0.3.1.dist-info/top_level.txt,sha256=AScY99r2vRxOMZGEg6sfYg7B5BlIyy9sXKc6CrlBR5s,12
+py_to_proto-0.3.1.dist-info/RECORD,,
```

