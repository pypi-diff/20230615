# Comparing `tmp/lpython_emulation-0.0.1.9.tar.gz` & `tmp/lpython_emulation-0.0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpython_emulation-0.0.1.9.tar", last modified: Tue May 23 15:23:41 2023, max compression
+gzip compressed data, was "lpython_emulation-0.0.16.0.tar", last modified: Wed Jun 14 23:36:42 2023, max compression
```

## Comparing `lpython_emulation-0.0.1.9.tar` & `lpython_emulation-0.0.16.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-05-23 15:23:41.743422 lpython_emulation-0.0.1.9/
--rw-r--r--   0 ubaid      (501) staff       (20)     1072 2023-05-06 13:31:30.000000 lpython_emulation-0.0.1.9/LICENSE
--rw-r--r--   0 ubaid      (501) staff       (20)     1019 2023-05-23 15:23:41.743295 lpython_emulation-0.0.1.9/PKG-INFO
--rw-r--r--   0 ubaid      (501) staff       (20)      556 2023-05-06 13:31:30.000000 lpython_emulation-0.0.1.9/README.md
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-05-23 15:23:41.742605 lpython_emulation-0.0.1.9/lpython/
--rw-r--r--   0 ubaid      (501) staff       (20)      262 2023-05-23 15:04:35.000000 lpython_emulation-0.0.1.9/lpython/__init__.py
--rw-r--r--   0 ubaid      (501) staff       (20)    28208 2023-05-23 15:02:24.000000 lpython_emulation-0.0.1.9/lpython/lpython.py
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-05-23 15:23:41.743131 lpython_emulation-0.0.1.9/lpython_emulation.egg-info/
--rw-r--r--   0 ubaid      (501) staff       (20)     1019 2023-05-23 15:23:41.000000 lpython_emulation-0.0.1.9/lpython_emulation.egg-info/PKG-INFO
--rw-r--r--   0 ubaid      (501) staff       (20)      229 2023-05-23 15:23:41.000000 lpython_emulation-0.0.1.9/lpython_emulation.egg-info/SOURCES.txt
--rw-r--r--   0 ubaid      (501) staff       (20)        1 2023-05-23 15:23:41.000000 lpython_emulation-0.0.1.9/lpython_emulation.egg-info/dependency_links.txt
--rw-r--r--   0 ubaid      (501) staff       (20)        8 2023-05-23 15:23:41.000000 lpython_emulation-0.0.1.9/lpython_emulation.egg-info/top_level.txt
--rw-r--r--   0 ubaid      (501) staff       (20)       38 2023-05-23 15:23:41.743463 lpython_emulation-0.0.1.9/setup.cfg
--rw-r--r--   0 ubaid      (501) staff       (20)     1794 2023-05-23 15:11:45.000000 lpython_emulation-0.0.1.9/setup.py
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-06-14 23:36:42.773525 lpython_emulation-0.0.16.0/
+-rw-r--r--   0 ubaid      (501) staff       (20)     1072 2023-05-06 13:31:30.000000 lpython_emulation-0.0.16.0/LICENSE
+-rw-r--r--   0 ubaid      (501) staff       (20)     1020 2023-06-14 23:36:42.773384 lpython_emulation-0.0.16.0/PKG-INFO
+-rw-r--r--   0 ubaid      (501) staff       (20)      556 2023-05-06 13:31:30.000000 lpython_emulation-0.0.16.0/README.md
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-06-14 23:36:42.772334 lpython_emulation-0.0.16.0/lpython/
+-rw-r--r--   0 ubaid      (501) staff       (20)      283 2023-06-14 19:02:55.000000 lpython_emulation-0.0.16.0/lpython/__init__.py
+-rw-r--r--   0 ubaid      (501) staff       (20)    30982 2023-06-14 23:34:35.000000 lpython_emulation-0.0.16.0/lpython/lpython.py
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-06-14 23:36:42.773175 lpython_emulation-0.0.16.0/lpython_emulation.egg-info/
+-rw-r--r--   0 ubaid      (501) staff       (20)     1020 2023-06-14 23:36:42.000000 lpython_emulation-0.0.16.0/lpython_emulation.egg-info/PKG-INFO
+-rw-r--r--   0 ubaid      (501) staff       (20)      229 2023-06-14 23:36:42.000000 lpython_emulation-0.0.16.0/lpython_emulation.egg-info/SOURCES.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)        1 2023-06-14 23:36:42.000000 lpython_emulation-0.0.16.0/lpython_emulation.egg-info/dependency_links.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)        8 2023-06-14 23:36:42.000000 lpython_emulation-0.0.16.0/lpython_emulation.egg-info/top_level.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)       38 2023-06-14 23:36:42.773573 lpython_emulation-0.0.16.0/setup.cfg
+-rw-r--r--   0 ubaid      (501) staff       (20)     1795 2023-06-14 23:34:00.000000 lpython_emulation-0.0.16.0/setup.py
```

### Comparing `lpython_emulation-0.0.1.9/LICENSE` & `lpython_emulation-0.0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lpython_emulation-0.0.1.9/PKG-INFO` & `lpython_emulation-0.0.16.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpython_emulation
-Version: 0.0.1.9
+Version: 0.0.16.0
 Summary: Package for adding type information to python
 Home-page: https://github.com/Shaikh-Ubaid/lpython_packages
 Author: Ondrej Certik
 Author-email: ondrej@certik.us
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lpython_emulation-0.0.1.9/README.md` & `lpython_emulation-0.0.16.0/README.md`

 * *Files identical despite different names*

### Comparing `lpython_emulation-0.0.1.9/lpython/lpython.py` & `lpython_emulation-0.0.16.0/lpython/lpython.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dataclasses import dataclass as py_dataclass, is_dataclass as py_is_dataclass
 
 # TODO: this does not seem to restrict other imports
 __slots__ = ["i8", "i16", "i32", "i64", "u8", "u16", "u32", "u64", "f32", "f64", "c32", "c64", "CPtr",
         "overload", "ccall", "TypeVar", "pointer", "c_p_pointer", "Pointer",
         "p_c_pointer", "vectorize", "inline", "Union", "static",
         "packed", "Const", "sizeof", "ccallable", "ccallback", "Callable",
-        "Allocatable"]
+        "Allocatable", "In", "Out", "InOut", "dataclass"]
 
 # data-types
 
 type_to_convert_func = {
     "i8": int,
     "i16": int,
     "i32": int,
@@ -453,14 +453,22 @@
     return ctypes_Structure
 
 def ccall(f):
     if isclass(f) and issubclass(f, Union):
         return f
     return CTypes(f)
 
+def pythoncall(*args, **kwargs):
+    def inner(fn):
+        import importlib
+        module = importlib.import_module(kwargs["module"])
+        fn_new = getattr(module, fn.__name__)
+        return fn_new
+    return inner
+
 def union(f):
     fields = []
     for name in f.__annotations__:
         ltype_ = f.__annotations__[name]
         fields.append((name, convert_type_to_ctype(ltype_)))
 
     f._fields_ = fields
@@ -548,17 +556,21 @@
                     value = value.flatten().tolist()
                     value = [c_double_complex(val.real, val.imag) for val in value]
                 value = type(name_)(*value)
         elif isinstance(value, Enum):
             value = value.value
         self.ctypes_ptr.contents.__setattr__(name, value)
 
-def c_p_pointer(cptr, targettype):
+def c_p_pointer(cptr, targettype, targetshape=None):
     targettype_ptr = convert_type_to_ctype(targettype)
     if isinstance(targettype, Array):
+        if targetshape is None:
+            raise ValueError("target shape must be "
+                             "provided if target type is an array.")
+        # TODO: Add support for multi-dimensional shape of target variable
         if py_is_dataclass(targettype._type):
             return ctypes.cast(cptr.value, ctypes.py_object).value
         newa = ctypes.cast(cptr, targettype_ptr)
         return newa
     else:
         if py_is_dataclass(targettype):
             if cptr.value is None:
@@ -587,14 +599,20 @@
             return self.value == value.value
 
         def __repr__(self):
             return str(self.value)
 
     return ctypes_c_void_p()
 
+def cptr_to_u64(cptr):
+    return ctypes.addressof(cptr)
+
+def u64_to_cptr(ivalue):
+    return ctypes.c_void_p(ivalue)
+
 def sizeof(arg):
     return ctypes.sizeof(convert_type_to_ctype(arg))
 
 def ccallable(f):
     if py_is_dataclass(f):
         return convert_to_ctypes_Structure(f)
     return f
@@ -615,39 +633,55 @@
     def __init__(self, function):
         def get_rtlib_dir():
             current_dir = os.path.dirname(os.path.abspath(__file__))
             return os.path.join(current_dir, "..")
 
         def get_type_info(arg):
             # return_type -> (`type_format`, `variable type`, `array struct name`)
-            # See: https://docs.python.org/3/c-api/arg.html for more info on type_format
+            # See: https://docs.python.org/3/c-api/arg.html for more info on `type_format`
+            # `array struct name`: used by the C backend
             if arg == f64:
                 return ('d', "double", 'r64')
             elif arg == f32:
                 return ('f', "float", 'r32')
             elif arg == i64:
                 return ('l', "long int", 'i64')
             elif arg == i32:
                 return ('i', "int", 'i32')
             elif arg == bool:
                 return ('p', "bool", '')
             elif isinstance(arg, Array):
                 t = get_type_info(arg._type)
                 if t[2] == '':
                     raise NotImplementedError("Type %r not implemented" % arg)
-                return ('O', ["PyArrayObject *", "struct "+t[2]+" *", t[1]+" *"], '')
+                n = ''
+                if not isinstance(arg._dims, slice):
+                    n = arg._dims._name
+                return ('O', ["PyArrayObject *", "struct "+t[2]+" *", t[1]+" *", n], '')
             else:
                 raise NotImplementedError("Type %r not implemented" % arg)
 
         def get_data_type(t):
             if isinstance(t, list):
                 return t[0]
             else:
                 return t + " "
 
+        def get_typenum(t):
+            if t == "int":
+                return "NPY_INT"
+            elif t == "long int":
+                return "NPY_LONG"
+            elif t == "float":
+                return "NPY_FLOAT"
+            elif t == "double":
+                return "NPY_DOUBLE"
+            else:
+                raise NotImplementedError("Type %s not implemented" % t)
+
         self.fn_name = function.__name__
         # Get the source code of the function
         source_code = getsource(function)
         source_code = source_code[source_code.find('\n'):]
 
         dir_name = "./lpython_decorator_" + self.fn_name
         if not os.path.exists(dir_name):
@@ -660,99 +694,134 @@
             file.write("@ccallable")
             file.write(source_code)
         # ----------------------------------------------------------------------
         types = function.__annotations__
         self.arg_type_formats = ""
         self.return_type = ""
         self.return_type_format = ""
+        self.array_as_return_type = ()
         self.arg_types = {}
-        counter = 1
         for t in types.keys():
             if t == "return":
                 type = get_type_info(types[t])
-                self.return_type_format = type[0]
-                self.return_type = type[1]
+                if type[0] == 'O':
+                    self.array_as_return_type = type
+                    continue
+                else:
+                    self.return_type_format = type[0]
+                    self.return_type = type[1]
             else:
                 type = get_type_info(types[t])
                 self.arg_type_formats += type[0]
-                self.arg_types[counter] = type[1]
-                counter += 1
+                self.arg_types[t] = type[1]
         # ----------------------------------------------------------------------
-        # `arg_0`: used as the return variables
-        # arguments are declared as `arg_1`, `arg_2`, ...
-        variables_decl = ""
+        # `_<fn_name>_return_value`: used as the return variables
+        variables_decl = "// Declare return variables and arguments\n"
         if self.return_type != "":
-            variables_decl = "// Declare return variables and arguments\n"
-            variables_decl += "    " + get_data_type(self.return_type) + "arg_" \
-                + str(0) + ";\n"
+            variables_decl += "    " + get_data_type(self.return_type)  \
+                + "_" + self.fn_name + "_return_value;\n"
+        elif self.array_as_return_type:
+            variables_decl += "    " + self.array_as_return_type[1][1] + "_" \
+                + self.fn_name + "_return_value = malloc(sizeof(" \
+                + self.array_as_return_type[1][1][:-2] + "));\n"
+        else:
+            variables_decl = ""
         # ----------------------------------------------------------------------
         # `PyArray_AsCArray` is used to convert NumPy Arrays to C Arrays
-        # `fill_array_details` contains arrays operations to be
+        # `fill_array_details` contains array operations to be
         # performed on the arguments
         # `parse_args` are used to capture the args from CPython
         # `pass_args` are the args that are passed to the shared library function
         fill_array_details = ""
         parse_args = ""
         pass_args = ""
         numpy_init = ""
+        prefix_comma = False
         for i, t in self.arg_types.items():
-            if i > 1:
+            if prefix_comma:
                 parse_args += ", "
                 pass_args += ", "
+            prefix_comma = True
             if isinstance(t, list):
                 if numpy_init == "":
                     numpy_init = "// Initialize NumPy\n    import_array();\n\n    "
                 fill_array_details += f"""\n
-    // fill array details for args[{i-1}]
-    if (PyArray_NDIM(arg_{i}) != 1) {{
+    // fill array details for {i}
+    if (PyArray_NDIM({i}) != 1) {{
         PyErr_SetString(PyExc_TypeError,
             "Only 1 dimension is implemented for now.");
         return NULL;
     }}
 
     {t[1]}s_array_{i} = malloc(sizeof(struct r64));
     {{
         {t[2]}array;
         // Create C arrays from numpy objects:
-        PyArray_Descr *descr = PyArray_DescrFromType(PyArray_TYPE(arg_{i}));
+        PyArray_Descr *descr = PyArray_DescrFromType(PyArray_TYPE({i}));
         npy_intp dims[1];
-        if (PyArray_AsCArray((PyObject **)&arg_{i}, (void *)&array, dims, 1, descr) < 0) {{
+        if (PyArray_AsCArray((PyObject **)&{i}, (void *)&array, dims, 1, descr) < 0) {{
             PyErr_SetString(PyExc_TypeError, "error converting to c array");
             return NULL;
         }}
 
         s_array_{i}->data = array;
         s_array_{i}->n_dims = 1;
         s_array_{i}->dims[0].lower_bound = 0;
         s_array_{i}->dims[0].length = dims[0];
         s_array_{i}->is_allocated = false;
     }}"""
-                pass_args += "s_array_" + str(i)
+                pass_args += "s_array_" + i
             else:
-                pass_args += "arg_" + str(i)
-            variables_decl += "    " + get_data_type(t) + "arg_" + str(i) + ";\n"
-            parse_args += "&arg_" + str(i)
+                pass_args += i
+            variables_decl += "    " + get_data_type(t) + i + ";\n"
+            parse_args += "&" + i
 
         if parse_args != "":
             parse_args = f"""\n    // Parse the arguments from Python
     if (!PyArg_ParseTuple(args, "{self.arg_type_formats}", {parse_args})) {{
         return NULL;
     }}"""
 
         # ----------------------------------------------------------------------
         # Handle the return variable if any; otherwise, return None
         fill_return_details = ""
         if self.return_type != "":
             fill_return_details = f"""\n\n    // Call the C function
-    arg_0 = {self.fn_name}({pass_args});
+    _{self.fn_name}_return_value = {self.fn_name}({pass_args});
 
     // Build and return the result as a Python object
-    return Py_BuildValue("{self.return_type_format}", arg_0);"""
+    return Py_BuildValue("{self.return_type_format}", _{self.fn_name}_return_value);"""
         else:
-            fill_return_details = f"""{self.fn_name}({pass_args});
+            if self.array_as_return_type:
+                fill_return_details = f"""\n
+    _{self.fn_name}_return_value->data = malloc({self.array_as_return_type[1][3]
+        } * sizeof({self.array_as_return_type[1][2][:-2]}));
+    _{self.fn_name}_return_value->n_dims = 1;
+    _{self.fn_name}_return_value->dims[0].lower_bound = 0;
+    _{self.fn_name}_return_value->dims[0].length = {
+        self.array_as_return_type[1][3]};
+    _{self.fn_name}_return_value->is_allocated = false;
+
+    // Call the C function
+    {self.fn_name}({pass_args}, &_{self.fn_name}_return_value[0]);
+
+    // Build and return the result as a Python object
+    {{
+        npy_intp dims[] = {{{self.array_as_return_type[1][3]}}};
+        PyObject* numpy_array = PyArray_SimpleNewFromData(1, dims, {
+            get_typenum(self.array_as_return_type[1][2][:-2])},
+            _{self.fn_name}_return_value->data);
+        if (numpy_array == NULL) {{
+            PyErr_SetString(PyExc_TypeError, "error creating an array");
+            return NULL;
+        }}
+        return numpy_array;
+    }}"""
+            else:
+                fill_return_details = f"""{self.fn_name}({pass_args});
     Py_RETURN_NONE;"""
 
         # ----------------------------------------------------------------------
         # Python wrapper for the Shared library
         template = f"""// Python headers
 #include <Python.h>
 
@@ -814,21 +883,23 @@
             gcc_flags = " -shared -fPIC "
         elif platform.system() == "Darwin":
             gcc_flags = " -bundle -flat_namespace -undefined suppress "
         else:
             raise NotImplementedError("Platform not implemented")
 
         from numpy import get_include
-        from distutils.sysconfig import get_python_inc, get_python_lib
+        from distutils.sysconfig import get_python_inc, get_python_lib, \
+            get_python_version
         python_path = "-I" + get_python_inc() + " "
         numpy_path = "-I" + get_include() + " "
         rt_path_01 = "-I" + get_rtlib_dir() + "/../libasr/runtime "
         rt_path_02 = "-L" + get_rtlib_dir() + " -Wl,-rpath " \
             + get_rtlib_dir() + " -llpython_runtime "
-        python_lib = "-L" + get_python_lib() + "/../.. -lpython3.10 -lm"
+        python_lib = "-L" + get_python_lib() + "/../.. -lpython" + \
+            get_python_version() + " -lm"
 
         r = os.system("gcc -g" +  gcc_flags + python_path + numpy_path +
             filename + ".c -o lpython_module_" + self.fn_name + ".so " +
             rt_path_01 + rt_path_02 + python_lib)
         assert r == 0, "Failed to create the shared library"
 
     def __call__(self, *args, **kwargs):
```

### Comparing `lpython_emulation-0.0.1.9/lpython_emulation.egg-info/PKG-INFO` & `lpython_emulation-0.0.16.0/lpython_emulation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpython-emulation
-Version: 0.0.1.9
+Version: 0.0.16.0
 Summary: Package for adding type information to python
 Home-page: https://github.com/Shaikh-Ubaid/lpython_packages
 Author: Ondrej Certik
 Author-email: ondrej@certik.us
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lpython_emulation-0.0.1.9/setup.py` & `lpython_emulation-0.0.16.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import setuptools
 
 # Define required packages. Alternatively, these could be defined in a separate
 # file and read in here.
 REQUIRED_PACKAGES=[]
 
-VERSION="0.0.1.9"
+VERSION="0.0.16.0"
 
 # Read in the project description. We define this in the README file.
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lpython_emulation",                                   # name of project
```

