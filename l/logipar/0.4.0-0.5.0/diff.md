# Comparing `tmp/logipar-0.4.0.tar.gz` & `tmp/logipar-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\logipar-0.4.0.tar", last modified: Sat Aug 31 23:21:37 2019, max compression
+gzip compressed data, was "dist\logipar-0.5.0.tar", last modified: Thu Jun 15 02:31:09 2023, max compression
```

## Comparing `logipar-0.4.0.tar` & `logipar-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2019-08-31 23:21:37.000000 logipar-0.4.0/
-drwxrwxrwx   0        0        0        0 2019-08-31 23:21:37.000000 logipar-0.4.0/logipar/
--rw-rw-rw-   0        0        0    33889 2019-08-31 22:48:35.000000 logipar-0.4.0/logipar/logipar.py
--rw-rw-rw-   0        0        0       68 2019-08-22 16:52:04.000000 logipar-0.4.0/logipar/__init__.py
-drwxrwxrwx   0        0        0        0 2019-08-31 23:21:37.000000 logipar-0.4.0/logipar.egg-info/
--rw-rw-rw-   0        0        0        1 2019-08-31 23:21:37.000000 logipar-0.4.0/logipar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0    20313 2019-08-31 23:21:37.000000 logipar-0.4.0/logipar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2019-08-31 23:21:37.000000 logipar-0.4.0/logipar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2019-08-31 23:21:37.000000 logipar-0.4.0/logipar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    20313 2019-08-31 23:21:37.000000 logipar-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2019-08-31 23:21:37.000000 logipar-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      589 2019-08-31 23:21:08.000000 logipar-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:31:09.011197 logipar-0.5.0/
+-rw-rw-rw-   0        0        0    20313 2023-06-15 02:31:09.008412 logipar-0.5.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 02:31:08.989060 logipar-0.5.0/logipar/
+-rw-rw-rw-   0        0        0       66 2023-06-15 01:57:32.000000 logipar-0.5.0/logipar/__init__.py
+-rw-rw-rw-   0        0        0    39640 2023-06-15 02:14:12.000000 logipar-0.5.0/logipar/logipar.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:31:09.007415 logipar-0.5.0/logipar.egg-info/
+-rw-rw-rw-   0        0        0    20313 2023-06-15 02:31:08.000000 logipar-0.5.0/logipar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2023-06-15 02:31:08.000000 logipar-0.5.0/logipar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 02:31:08.000000 logipar-0.5.0/logipar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-15 02:31:08.000000 logipar-0.5.0/logipar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 02:31:09.011197 logipar-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      569 2023-06-15 02:29:15.000000 logipar-0.5.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `logipar-0.4.0/logipar/logipar.py` & `logipar-0.5.0/logipar/logipar.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-# Generated by Haxe 4.0.0-rc.2+77068e10c
-# coding: utf-8
+import sys
 
 import math as python_lib_Math
 import math as Math
 import inspect as python_lib_Inspect
+import sys as python_lib_Sys
+import traceback as python_lib_Traceback
 from io import StringIO as python_lib_io_StringIO
 
 
 class Enum:
     _hx_class_name = "Enum"
     __slots__ = ("tag", "index", "params")
     _hx_fields = ["tag", "index", "params"]
@@ -18,29 +19,129 @@
         self.index = index
         self.params = params
 
     def __str__(self):
         if (self.params is None):
             return self.tag
         else:
-            _this = self.params
-            return (((HxOverrides.stringOrNull(self.tag) + "(") + HxOverrides.stringOrNull(",".join([python_Boot.toString1(x1,'') for x1 in _this]))) + ")")
+            return self.tag + '(' + (', '.join(str(v) for v in self.params)) + ')'
 
 
 
+class Class: pass
+
+
 class Std:
     _hx_class_name = "Std"
     __slots__ = ()
-    _hx_statics = ["string"]
+    _hx_statics = ["isOfType", "string"]
+
+    @staticmethod
+    def isOfType(v,t):
+        if ((v is None) and ((t is None))):
+            return False
+        if (t is None):
+            return False
+        if (t == Dynamic):
+            return (v is not None)
+        isBool = isinstance(v,bool)
+        if ((t == Bool) and isBool):
+            return True
+        if ((((not isBool) and (not (t == Bool))) and (t == Int)) and isinstance(v,int)):
+            return True
+        vIsFloat = isinstance(v,float)
+        tmp = None
+        tmp1 = None
+        if (((not isBool) and vIsFloat) and (t == Int)):
+            f = v
+            tmp1 = (((f != Math.POSITIVE_INFINITY) and ((f != Math.NEGATIVE_INFINITY))) and (not python_lib_Math.isnan(f)))
+        else:
+            tmp1 = False
+        if tmp1:
+            tmp1 = None
+            try:
+                tmp1 = int(v)
+            except BaseException as _g:
+                None
+                tmp1 = None
+            tmp = (v == tmp1)
+        else:
+            tmp = False
+        if ((tmp and ((v <= 2147483647))) and ((v >= -2147483648))):
+            return True
+        if (((not isBool) and (t == Float)) and isinstance(v,(float, int))):
+            return True
+        if (t == str):
+            return isinstance(v,str)
+        isEnumType = (t == Enum)
+        if ((isEnumType and python_lib_Inspect.isclass(v)) and hasattr(v,"_hx_constructs")):
+            return True
+        if isEnumType:
+            return False
+        isClassType = (t == Class)
+        if ((((isClassType and (not isinstance(v,Enum))) and python_lib_Inspect.isclass(v)) and hasattr(v,"_hx_class_name")) and (not hasattr(v,"_hx_constructs"))):
+            return True
+        if isClassType:
+            return False
+        tmp = None
+        try:
+            tmp = isinstance(v,t)
+        except BaseException as _g:
+            None
+            tmp = False
+        if tmp:
+            return True
+        if python_lib_Inspect.isclass(t):
+            cls = t
+            loop = None
+            def _hx_local_1(intf):
+                f = (intf._hx_interfaces if (hasattr(intf,"_hx_interfaces")) else [])
+                if (f is not None):
+                    _g = 0
+                    while (_g < len(f)):
+                        i = (f[_g] if _g >= 0 and _g < len(f) else None)
+                        _g = (_g + 1)
+                        if (i == cls):
+                            return True
+                        else:
+                            l = loop(i)
+                            if l:
+                                return True
+                    return False
+                else:
+                    return False
+            loop = _hx_local_1
+            currentClass = v.__class__
+            result = False
+            while (currentClass is not None):
+                if loop(currentClass):
+                    result = True
+                    break
+                currentClass = python_Boot.getSuperClass(currentClass)
+            return result
+        else:
+            return False
 
     @staticmethod
     def string(s):
         return python_Boot.toString1(s,"")
 
 
+class Float: pass
+
+
+class Int: pass
+
+
+class Bool: pass
+
+
+class Dynamic: pass
+
+
 class StringTools:
     _hx_class_name = "StringTools"
     __slots__ = ()
     _hx_statics = ["isSpace", "ltrim", "rtrim", "trim"]
 
     @staticmethod
     def isSpace(s,pos):
@@ -81,14 +182,110 @@
 
 class haxe_IMap:
     _hx_class_name = "haxe.IMap"
     __slots__ = ()
     _hx_methods = ["toString"]
 
 
+class haxe_Exception(Exception):
+    _hx_class_name = "haxe.Exception"
+    __slots__ = ("_hx___nativeStack", "_hx___skipStack", "_hx___nativeException", "_hx___previousException")
+    _hx_fields = ["__nativeStack", "__skipStack", "__nativeException", "__previousException"]
+    _hx_methods = ["unwrap", "get_native"]
+    _hx_statics = ["caught", "thrown"]
+    _hx_interfaces = []
+    _hx_super = Exception
+
+
+    def __init__(self,message,previous = None,native = None):
+        self._hx___previousException = None
+        self._hx___nativeException = None
+        self._hx___nativeStack = None
+        self._hx___skipStack = 0
+        super().__init__(message)
+        self._hx___previousException = previous
+        if ((native is not None) and Std.isOfType(native,BaseException)):
+            self._hx___nativeException = native
+            self._hx___nativeStack = haxe_NativeStackTrace.exceptionStack()
+        else:
+            self._hx___nativeException = self
+            infos = python_lib_Traceback.extract_stack()
+            if (len(infos) != 0):
+                infos.pop()
+            infos.reverse()
+            self._hx___nativeStack = infos
+
+    def unwrap(self):
+        return self._hx___nativeException
+
+    def get_native(self):
+        return self._hx___nativeException
+
+    @staticmethod
+    def caught(value):
+        if Std.isOfType(value,haxe_Exception):
+            return value
+        elif Std.isOfType(value,BaseException):
+            return haxe_Exception(str(value),None,value)
+        else:
+            return haxe_ValueException(value,None,value)
+
+    @staticmethod
+    def thrown(value):
+        if Std.isOfType(value,haxe_Exception):
+            return value.get_native()
+        elif Std.isOfType(value,BaseException):
+            return value
+        else:
+            e = haxe_ValueException(value)
+            e._hx___skipStack = (e._hx___skipStack + 1)
+            return e
+
+
+
+class haxe_NativeStackTrace:
+    _hx_class_name = "haxe.NativeStackTrace"
+    __slots__ = ()
+    _hx_statics = ["saveStack", "exceptionStack"]
+
+    @staticmethod
+    def saveStack(exception):
+        pass
+
+    @staticmethod
+    def exceptionStack():
+        exc = python_lib_Sys.exc_info()
+        if (exc[2] is not None):
+            infos = python_lib_Traceback.extract_tb(exc[2])
+            infos.reverse()
+            return infos
+        else:
+            return []
+
+
+class haxe_ValueException(haxe_Exception):
+    _hx_class_name = "haxe.ValueException"
+    __slots__ = ("value",)
+    _hx_fields = ["value"]
+    _hx_methods = ["unwrap"]
+    _hx_statics = []
+    _hx_interfaces = []
+    _hx_super = haxe_Exception
+
+
+    def __init__(self,value,previous = None,native = None):
+        self.value = None
+        super().__init__(Std.string(value),previous,native)
+        self.value = value
+
+    def unwrap(self):
+        return self.value
+
+
+
 class haxe_ds_GenericCell:
     _hx_class_name = "haxe.ds.GenericCell"
     __slots__ = ("elt", "next")
     _hx_fields = ["elt", "next"]
 
     def __init__(self,elt,next):
         self.elt = elt
@@ -107,14 +304,15 @@
 
 
 class haxe_ds_StringMap:
     _hx_class_name = "haxe.ds.StringMap"
     __slots__ = ("h",)
     _hx_fields = ["h"]
     _hx_methods = ["keys", "iterator", "toString"]
+    _hx_interfaces = [haxe_IMap]
 
     def __init__(self):
         self.h = dict()
 
     def keys(self):
         return python_HaxeIterator(iter(self.h.keys()))
 
@@ -134,14 +332,39 @@
             if it.hasNext():
                 s_b.write(", ")
         s_b.write("}")
         return s_b.getvalue()
 
 
 
+class haxe_iterators_ArrayIterator:
+    _hx_class_name = "haxe.iterators.ArrayIterator"
+    __slots__ = ("array", "current")
+    _hx_fields = ["array", "current"]
+    _hx_methods = ["hasNext", "next"]
+
+    def __init__(self,array):
+        self.current = 0
+        self.array = array
+
+    def hasNext(self):
+        return (self.current < len(self.array))
+
+    def next(self):
+        def _hx_local_3():
+            def _hx_local_2():
+                _hx_local_0 = self
+                _hx_local_1 = _hx_local_0.current
+                _hx_local_0.current = (_hx_local_1 + 1)
+                return _hx_local_1
+            return python_internal_ArrayImpl._get(self.array, _hx_local_2())
+        return _hx_local_3()
+
+
+
 class Logipar:
     _hx_class_name = "Logipar"
     __slots__ = ("quotations", "caseSensitive", "mergeAdjacentLiterals", "syntax", "tree")
     _hx_fields = ["quotations", "caseSensitive", "mergeAdjacentLiterals", "syntax", "tree"]
     _hx_methods = ["overwrite", "parse", "stringify", "walk", "filterFunction", "toString", "equals", "mergeLiterals", "treeify", "shunt", "tentativelyLower", "tokenize", "tokenType", "typeize"]
 
     def __init__(self):
@@ -218,46 +441,45 @@
         while (_g < _g1):
             i = _g
             _g = (_g + 1)
             token = (tokens[i] if i >= 0 and i < len(tokens) else None)
             n = Node(token)
             if (token.type != "LITERAL"):
                 if (stack.head is None):
-                    raise _HxException((("An '" + HxOverrides.stringOrNull(self.syntax.h.get(token.type,None))) + "' is missing a value to operate on (on its right)."))
+                    raise haxe_Exception.thrown((("An '" + HxOverrides.stringOrNull(self.syntax.h.get(token.type,None))) + "' is missing a value to operate on (on its right)."))
                 k = stack.head
                 tmp = None
                 if (k is None):
                     tmp = None
                 else:
                     stack.head = k.next
                     tmp = k.elt
                 n.set_right(tmp)
                 if (token.type != "NOT"):
                     if (stack.head is None):
-                        raise _HxException((("An '" + HxOverrides.stringOrNull(self.syntax.h.get(token.type,None))) + "' is missing a value to operate on (on its left)."))
+                        raise haxe_Exception.thrown((("An '" + HxOverrides.stringOrNull(self.syntax.h.get(token.type,None))) + "' is missing a value to operate on (on its left)."))
                     k1 = stack.head
                     tmp1 = None
                     if (k1 is None):
                         tmp1 = None
                     else:
                         stack.head = k1.next
                         tmp1 = k1.elt
                     n.set_left(tmp1)
             stack.head = haxe_ds_GenericCell(n,stack.head)
-        k2 = stack.head
+        k = stack.head
         parsetree = None
-        if (k2 is None):
+        if (k is None):
             parsetree = None
         else:
-            stack.head = k2.next
-            parsetree = k2.elt
-        parsetree1 = parsetree
+            stack.head = k.next
+            parsetree = k.elt
         if (stack.head is not None):
-            raise _HxException("Invalid logic string.  Do you have parentheses in your literals?")
-        return parsetree1
+            raise haxe_Exception.thrown("Invalid logic string.  Do you have parentheses in your literals?")
+        return parsetree
 
     def shunt(self,tokens):
         output = list()
         operators = haxe_ds_GenericStack()
         _g = 0
         _g1 = len(tokens)
         while (_g < _g1):
@@ -272,20 +494,19 @@
                         k = operators.head
                         op = None
                         if (k is None):
                             op = None
                         else:
                             operators.head = k.next
                             op = k.elt
-                        op1 = op
-                        if (op1.type == "OPEN"):
+                        if (op.type == "OPEN"):
                             break
                         if (operators.head is None):
-                            raise _HxException("Mismatched parentheses.")
-                        output.append(op1)
+                            raise haxe_Exception.thrown("Mismatched parentheses.")
+                        output.append(op)
                 else:
                     while (operators.head is not None):
                         prev = (None if ((operators.head is None)) else operators.head.elt)
                         if (prev.type == "OPEN"):
                             break
                         if (prev.precedence() <= token.precedence()):
                             break
@@ -349,25 +570,24 @@
                         x = None
                     else:
                         operators.head = k1.next
                         x = k1.elt
                     output.append(x)
                 operators.head = haxe_ds_GenericCell(token,operators.head)
         while (operators.head is not None):
-            k2 = operators.head
+            k = operators.head
             o = None
-            if (k2 is None):
+            if (k is None):
                 o = None
             else:
-                operators.head = k2.next
-                o = k2.elt
-            o1 = o
-            if (o1.type == "OPEN"):
-                raise _HxException("Mismatched parentheses.")
-            output.append(o1)
+                operators.head = k.next
+                o = k.elt
+            if (o.type == "OPEN"):
+                raise haxe_Exception.thrown("Mismatched parentheses.")
+            output.append(o)
         return output
 
     def tentativelyLower(self,s):
         if self.caseSensitive:
             return s
         else:
             return Std.string(s).lower()
@@ -379,19 +599,19 @@
         while x.hasNext():
             x1 = x.next()
             x2 = self.tentativelyLower(x1)
             _g.append(x2)
         keys = _g
         quotation = None
         current = ""
-        _g1 = 0
-        _g2 = len(_hx_str)
-        while (_g1 < _g2):
-            i = _g1
-            _g1 = (_g1 + 1)
+        _g = 0
+        _g1 = len(_hx_str)
+        while (_g < _g1):
+            i = _g
+            _g = (_g + 1)
             c = ("" if (((i < 0) or ((i >= len(_hx_str))))) else _hx_str[i])
             if (python_internal_ArrayImpl.indexOf(self.quotations,c,None) != -1):
                 if (quotation is None):
                     quotation = c
                 elif (quotation == c):
                     quotation = None
             if ((quotation is not None) or ((python_internal_ArrayImpl.indexOf(keys,self.tentativelyLower(c),None) == -1))):
@@ -403,16 +623,16 @@
                     current = (("null" if current is None else current) + ("null" if c is None else c))
             else:
                 if (len(current) > 0):
                     tokens.append(current)
                 current = ""
                 tokens.append(c)
         if (len(StringTools.trim(current)) > 0):
-            x3 = StringTools.trim(current)
-            tokens.append(x3)
+            x = StringTools.trim(current)
+            tokens.append(x)
         return tokens
 
     def tokenType(self,token):
         key = self.syntax.keys()
         while key.hasNext():
             key1 = key.next()
             if (self.tentativelyLower(token) == self.tentativelyLower(self.syntax.h.get(key1,None))):
@@ -486,44 +706,44 @@
             else:
                 return False
         return False
 
     def walk(self,f):
         f(self)
         if (self.left is not None):
-            f(self.left)
+            self.left.walk(f)
         if (self.right is not None):
-            f(self.right)
+            self.right.walk(f)
 
     def bracket(self,_hx_str):
         if ((self.bracketing == "MAXIMAL_BRACKETS") or (((self.parent is not None) and ((self.parent.token.precedence() > self.token.precedence()))))):
             return (("(" + ("null" if _hx_str is None else _hx_str)) + ")")
         return _hx_str
 
     def _fancyString(self,n,f = None):
         s = None
         if (f is not None):
-            f1 = self._fancyString
-            f2 = f
-            def _hx_local_0(n1):
-                return f1(n1,f2)
+            _g = self._fancyString
+            f1 = f
+            def _hx_local_0(n):
+                return _g(n,f1)
             n.f = _hx_local_0
             s = f(n)
             n.f = None
         if (s is not None):
             return s
-        _g = n.token.type
-        _hx_local_1 = len(_g)
+        _g1 = n.token.type
+        _hx_local_1 = len(_g1)
         if (_hx_local_1 == 7):
-            if (_g == "LITERAL"):
+            if (_g1 == "LITERAL"):
                 return (("{" + HxOverrides.stringOrNull(n.token.literal)) + "}")
             else:
                 return self.bracket(((((HxOverrides.stringOrNull(n.left.fancyString(f)) + " ") + Std.string(n.token.type)) + " ") + HxOverrides.stringOrNull(n.right.fancyString(f))))
         elif (_hx_local_1 == 3):
-            if (_g == "NOT"):
+            if (_g1 == "NOT"):
                 return self.bracket(("NOT " + HxOverrides.stringOrNull(n.right.fancyString(f))))
             else:
                 return self.bracket(((((HxOverrides.stringOrNull(n.left.fancyString(f)) + " ") + Std.string(n.token.type)) + " ") + HxOverrides.stringOrNull(n.right.fancyString(f))))
         else:
             return self.bracket(((((HxOverrides.stringOrNull(n.left.fancyString(f)) + " ") + Std.string(n.token.type)) + " ") + HxOverrides.stringOrNull(n.right.fancyString(f))))
 
     def check(self,a,f):
@@ -544,30 +764,30 @@
                     if l:
                         return (not r)
                     else:
                         return False
                 else:
                     return True
             else:
-                raise _HxException("Unexpected token encountered.")
+                raise haxe_Exception.thrown("Unexpected token encountered.")
         elif (_hx_local_0 == 7):
             if (_g == "LITERAL"):
                 return f(a,self.token.literal)
             else:
-                raise _HxException("Unexpected token encountered.")
+                raise haxe_Exception.thrown("Unexpected token encountered.")
         elif (_hx_local_0 == 2):
             if (_g == "OR"):
                 if (not self.left.check(a,f)):
                     return self.right.check(a,f)
                 else:
                     return True
             else:
-                raise _HxException("Unexpected token encountered.")
+                raise haxe_Exception.thrown("Unexpected token encountered.")
         else:
-            raise _HxException("Unexpected token encountered.")
+            raise haxe_Exception.thrown("Unexpected token encountered.")
 
 
 
 class Token:
     _hx_class_name = "Token"
     __slots__ = ("type", "literal")
     _hx_fields = ["type", "literal"]
@@ -640,17 +860,16 @@
             return str(o)
         if isinstance(o,float):
             try:
                 if (o == int(o)):
                     return str(Math.floor((o + 0.5)))
                 else:
                     return str(o)
-            except Exception as _hx_e:
-                _hx_e1 = _hx_e.val if isinstance(_hx_e, _HxException) else _hx_e
-                e = _hx_e1
+            except BaseException as _g:
+                None
                 return str(o)
         if isinstance(o,list):
             o1 = o
             l = len(o1)
             st = "["
             s = (("null" if s is None else s) + "\t")
             _g = 0
@@ -663,119 +882,117 @@
                     prefix = ","
                 st = (("null" if st is None else st) + HxOverrides.stringOrNull(((("null" if prefix is None else prefix) + HxOverrides.stringOrNull(python_Boot.toString1((o1[i] if i >= 0 and i < len(o1) else None),s))))))
             st = (("null" if st is None else st) + "]")
             return st
         try:
             if hasattr(o,"toString"):
                 return o.toString()
-        except Exception as _hx_e:
-            _hx_e1 = _hx_e.val if isinstance(_hx_e, _HxException) else _hx_e
-            pass
-        if (python_lib_Inspect.isfunction(o) or python_lib_Inspect.ismethod(o)):
-            return "<function>"
+        except BaseException as _g:
+            None
         if hasattr(o,"__class__"):
             if isinstance(o,_hx_AnonObject):
                 toStr = None
                 try:
                     fields = python_Boot.fields(o)
-                    _g2 = []
-                    _g11 = 0
-                    while (_g11 < len(fields)):
-                        f = (fields[_g11] if _g11 >= 0 and _g11 < len(fields) else None)
-                        _g11 = (_g11 + 1)
+                    _g = []
+                    _g1 = 0
+                    while (_g1 < len(fields)):
+                        f = (fields[_g1] if _g1 >= 0 and _g1 < len(fields) else None)
+                        _g1 = (_g1 + 1)
                         x = ((("" + ("null" if f is None else f)) + " : ") + HxOverrides.stringOrNull(python_Boot.toString1(python_Boot.simpleField(o,f),(("null" if s is None else s) + "\t"))))
-                        _g2.append(x)
-                    fieldsStr = _g2
+                        _g.append(x)
+                    fieldsStr = _g
                     toStr = (("{ " + HxOverrides.stringOrNull(", ".join([x1 for x1 in fieldsStr]))) + " }")
-                except Exception as _hx_e:
-                    _hx_e1 = _hx_e.val if isinstance(_hx_e, _HxException) else _hx_e
-                    e2 = _hx_e1
+                except BaseException as _g:
+                    None
                     return "{ ... }"
                 if (toStr is None):
                     return "{ ... }"
                 else:
                     return toStr
             if isinstance(o,Enum):
-                o2 = o
-                l1 = len(o2.params)
-                hasParams = (l1 > 0)
+                o1 = o
+                l = len(o1.params)
+                hasParams = (l > 0)
                 if hasParams:
                     paramsStr = ""
-                    _g3 = 0
-                    _g12 = l1
-                    while (_g3 < _g12):
-                        i1 = _g3
-                        _g3 = (_g3 + 1)
-                        prefix1 = ""
-                        if (i1 > 0):
-                            prefix1 = ","
-                        paramsStr = (("null" if paramsStr is None else paramsStr) + HxOverrides.stringOrNull(((("null" if prefix1 is None else prefix1) + HxOverrides.stringOrNull(python_Boot.toString1((o2.params[i1] if i1 >= 0 and i1 < len(o2.params) else None),s))))))
-                    return (((HxOverrides.stringOrNull(o2.tag) + "(") + ("null" if paramsStr is None else paramsStr)) + ")")
+                    _g = 0
+                    _g1 = l
+                    while (_g < _g1):
+                        i = _g
+                        _g = (_g + 1)
+                        prefix = ""
+                        if (i > 0):
+                            prefix = ","
+                        paramsStr = (("null" if paramsStr is None else paramsStr) + HxOverrides.stringOrNull(((("null" if prefix is None else prefix) + HxOverrides.stringOrNull(python_Boot.toString1(o1.params[i],s))))))
+                    return (((HxOverrides.stringOrNull(o1.tag) + "(") + ("null" if paramsStr is None else paramsStr)) + ")")
                 else:
-                    return o2.tag
+                    return o1.tag
             if hasattr(o,"_hx_class_name"):
                 if (o.__class__.__name__ != "type"):
-                    fields1 = python_Boot.getInstanceFields(o)
-                    _g4 = []
-                    _g13 = 0
-                    while (_g13 < len(fields1)):
-                        f1 = (fields1[_g13] if _g13 >= 0 and _g13 < len(fields1) else None)
-                        _g13 = (_g13 + 1)
-                        x1 = ((("" + ("null" if f1 is None else f1)) + " : ") + HxOverrides.stringOrNull(python_Boot.toString1(python_Boot.simpleField(o,f1),(("null" if s is None else s) + "\t"))))
-                        _g4.append(x1)
-                    fieldsStr1 = _g4
-                    toStr1 = (((HxOverrides.stringOrNull(o._hx_class_name) + "( ") + HxOverrides.stringOrNull(", ".join([x1 for x1 in fieldsStr1]))) + " )")
-                    return toStr1
-                else:
-                    fields2 = python_Boot.getClassFields(o)
-                    _g5 = []
-                    _g14 = 0
-                    while (_g14 < len(fields2)):
-                        f2 = (fields2[_g14] if _g14 >= 0 and _g14 < len(fields2) else None)
-                        _g14 = (_g14 + 1)
-                        x2 = ((("" + ("null" if f2 is None else f2)) + " : ") + HxOverrides.stringOrNull(python_Boot.toString1(python_Boot.simpleField(o,f2),(("null" if s is None else s) + "\t"))))
-                        _g5.append(x2)
-                    fieldsStr2 = _g5
-                    toStr2 = (((("#" + HxOverrides.stringOrNull(o._hx_class_name)) + "( ") + HxOverrides.stringOrNull(", ".join([x1 for x1 in fieldsStr2]))) + " )")
-                    return toStr2
+                    fields = python_Boot.getInstanceFields(o)
+                    _g = []
+                    _g1 = 0
+                    while (_g1 < len(fields)):
+                        f = (fields[_g1] if _g1 >= 0 and _g1 < len(fields) else None)
+                        _g1 = (_g1 + 1)
+                        x = ((("" + ("null" if f is None else f)) + " : ") + HxOverrides.stringOrNull(python_Boot.toString1(python_Boot.simpleField(o,f),(("null" if s is None else s) + "\t"))))
+                        _g.append(x)
+                    fieldsStr = _g
+                    toStr = (((HxOverrides.stringOrNull(o._hx_class_name) + "( ") + HxOverrides.stringOrNull(", ".join([x1 for x1 in fieldsStr]))) + " )")
+                    return toStr
+                else:
+                    fields = python_Boot.getClassFields(o)
+                    _g = []
+                    _g1 = 0
+                    while (_g1 < len(fields)):
+                        f = (fields[_g1] if _g1 >= 0 and _g1 < len(fields) else None)
+                        _g1 = (_g1 + 1)
+                        x = ((("" + ("null" if f is None else f)) + " : ") + HxOverrides.stringOrNull(python_Boot.toString1(python_Boot.simpleField(o,f),(("null" if s is None else s) + "\t"))))
+                        _g.append(x)
+                    fieldsStr = _g
+                    toStr = (((("#" + HxOverrides.stringOrNull(o._hx_class_name)) + "( ") + HxOverrides.stringOrNull(", ".join([x1 for x1 in fieldsStr]))) + " )")
+                    return toStr
             if (o == str):
                 return "#String"
             if (o == list):
                 return "#Array"
             if callable(o):
                 return "function"
             try:
                 if hasattr(o,"__repr__"):
                     return o.__repr__()
-            except Exception as _hx_e:
-                _hx_e1 = _hx_e.val if isinstance(_hx_e, _HxException) else _hx_e
-                pass
+            except BaseException as _g:
+                None
             if hasattr(o,"__str__"):
                 return o.__str__([])
             if hasattr(o,"__name__"):
                 return o.__name__
             return "???"
         else:
             return str(o)
 
     @staticmethod
     def fields(o):
         a = []
         if (o is not None):
             if hasattr(o,"_hx_fields"):
-                return list(o._hx_fields)
+                fields = o._hx_fields
+                if (fields is not None):
+                    return list(fields)
             if isinstance(o,_hx_AnonObject):
                 d = o.__dict__
                 keys = d.keys()
                 handler = python_Boot.unhandleKeywords
                 for k in keys:
-                    a.append(handler(k))
+                    if (k != '_hx_disable_getattr'):
+                        a.append(handler(k))
             elif hasattr(o,"__dict__"):
-                d1 = o.__dict__
-                keys1 = d1.keys()
+                d = o.__dict__
+                keys1 = d.keys()
                 for k in keys1:
                     a.append(k)
         return a
 
     @staticmethod
     def simpleField(o,field):
         if (field is None):
@@ -809,17 +1026,16 @@
     def getSuperClass(c):
         if (c is None):
             return None
         try:
             if hasattr(c,"_hx_super"):
                 return c._hx_super
             return None
-        except Exception as _hx_e:
-            _hx_e1 = _hx_e.val if isinstance(_hx_e, _HxException) else _hx_e
-            pass
+        except BaseException as _g:
+            None
         return None
 
     @staticmethod
     def getClassFields(c):
         if hasattr(c,"_hx_statics"):
             x = c._hx_statics
             return list(x)
@@ -854,22 +1070,21 @@
         return self.x
 
     def hasNext(self):
         if (not self.checked):
             try:
                 self.x = self.it.__next__()
                 self.has = True
-            except Exception as _hx_e:
-                _hx_e1 = _hx_e.val if isinstance(_hx_e, _HxException) else _hx_e
-                if isinstance(_hx_e1, StopIteration):
-                    s = _hx_e1
+            except BaseException as _g:
+                None
+                if Std.isOfType(haxe_Exception.caught(_g).unwrap(),StopIteration):
                     self.has = False
                     self.x = None
                 else:
-                    raise _hx_e
+                    raise _g
             self.checked = True
         return self.has
 
 
 
 class _hx_AnonObject:
     _hx_class_name = "_hx_AnonObject"
@@ -900,31 +1115,14 @@
     def _get(x,idx):
         if ((idx > -1) and ((idx < len(x)))):
             return x[idx]
         else:
             return None
 
 
-class _HxException(Exception):
-    _hx_class_name = "_HxException"
-    __slots__ = ("val",)
-    _hx_fields = ["val"]
-    _hx_methods = []
-    _hx_statics = []
-    _hx_super = Exception
-
-
-    def __init__(self,val):
-        self.val = None
-        message = str(val)
-        super().__init__(message)
-        self.val = val
-
-
-
 class HxOverrides:
     _hx_class_name = "HxOverrides"
     __slots__ = ()
     _hx_statics = ["eq", "stringOrNull"]
 
     @staticmethod
     def eq(a,b):
```

### Comparing `logipar-0.4.0/logipar.egg-info/PKG-INFO` & `logipar-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logipar
-Version: 0.4.0
+Version: 0.5.0
 Summary: A logic string parser
 Home-page: https://github.com/altef/logipar
 Author: Brad Gill
 Author-email: brad@alteredeffect.com
 License: UNKNOWN
 Description: [![npm](https://img.shields.io/npm/v/logipar)](https://npmjs.com/package/logipar) [![pypi](https://img.shields.io/pypi/v/logipar)](https://pypi.org/project/logipar/) [![haxelib install logipar](https://img.shields.io/badge/haxelib-logipar-orange, "haxelib install logipar")](https://lib.haxe.org/p/logipar/) [![php phar](https://img.shields.io/badge/php-Logipar.phar-orange, "PHP Logipar.phar")](https://github.com/altef/logipar/blob/master/php/Logipar.phar)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logipar Version: 0.4.0 Summary: A logic string
+Metadata-Version: 2.1 Name: logipar Version: 0.5.0 Summary: A logic string
 parser Home-page: https://github.com/altef/logipar Author: Brad Gill Author-
 email: brad@alteredeffect.com License: UNKNOWN Description: [![npm](https://
 img.shields.io/npm/v/logipar)](https://npmjs.com/package/logipar) [![pypi]
 (https://img.shields.io/pypi/v/logipar)](https://pypi.org/project/logipar/) [!
 [haxelib install logipar](https://img.shields.io/badge/haxelib-logipar-orange,
 "haxelib install logipar")](https://lib.haxe.org/p/logipar/) [![php phar]
 (https://img.shields.io/badge/php-Logipar.phar-orange, "PHP Logipar.phar")]
```

### Comparing `logipar-0.4.0/PKG-INFO` & `logipar-0.5.0/logipar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logipar
-Version: 0.4.0
+Version: 0.5.0
 Summary: A logic string parser
 Home-page: https://github.com/altef/logipar
 Author: Brad Gill
 Author-email: brad@alteredeffect.com
 License: UNKNOWN
 Description: [![npm](https://img.shields.io/npm/v/logipar)](https://npmjs.com/package/logipar) [![pypi](https://img.shields.io/pypi/v/logipar)](https://pypi.org/project/logipar/) [![haxelib install logipar](https://img.shields.io/badge/haxelib-logipar-orange, "haxelib install logipar")](https://lib.haxe.org/p/logipar/) [![php phar](https://img.shields.io/badge/php-Logipar.phar-orange, "PHP Logipar.phar")](https://github.com/altef/logipar/blob/master/php/Logipar.phar)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logipar Version: 0.4.0 Summary: A logic string
+Metadata-Version: 2.1 Name: logipar Version: 0.5.0 Summary: A logic string
 parser Home-page: https://github.com/altef/logipar Author: Brad Gill Author-
 email: brad@alteredeffect.com License: UNKNOWN Description: [![npm](https://
 img.shields.io/npm/v/logipar)](https://npmjs.com/package/logipar) [![pypi]
 (https://img.shields.io/pypi/v/logipar)](https://pypi.org/project/logipar/) [!
 [haxelib install logipar](https://img.shields.io/badge/haxelib-logipar-orange,
 "haxelib install logipar")](https://lib.haxe.org/p/logipar/) [![php phar]
 (https://img.shields.io/badge/php-Logipar.phar-orange, "PHP Logipar.phar")]
```

### Comparing `logipar-0.4.0/setup.py` & `logipar-0.5.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import setuptools
-
-with open("../../readme.md", "r", encoding="utf-8") as fh:
-	long_description = fh.read()
-
-setuptools.setup(
-	name="logipar",
-	version="0.4.0",
-	author="Brad Gill",
-	author_email="brad@alteredeffect.com",
-	description="A logic string parser",
-	long_description=long_description,
-	long_description_content_type="text/markdown",
-	url="https://github.com/altef/logipar",
-	packages=setuptools.find_packages(),
-	classifiers=[
-		"Programming Language :: Python :: 3",
-		"License :: OSI Approved :: MIT License",
-		"Operating System :: OS Independent",
-	],
+import setuptools
+
+with open("../../readme.md", "r", encoding="utf-8") as fh:
+	long_description = fh.read()
+
+setuptools.setup(
+	name="logipar",
+	version="0.5.0",
+	author="Brad Gill",
+	author_email="brad@alteredeffect.com",
+	description="A logic string parser",
+	long_description=long_description,
+	long_description_content_type="text/markdown",
+	url="https://github.com/altef/logipar",
+	packages=setuptools.find_packages(),
+	classifiers=[
+		"Programming Language :: Python :: 3",
+		"License :: OSI Approved :: MIT License",
+		"Operating System :: OS Independent",
+	],
 )
```
