# Comparing `tmp/pybox-toolkit-0.1.6.dev4.tar.gz` & `tmp/pybox-toolkit-0.1.7.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybox-toolkit-0.1.6.dev4.tar", last modified: Sun Jun 11 12:18:48 2023, max compression
+gzip compressed data, was "pybox-toolkit-0.1.7.dev3.tar", last modified: Thu Jun 15 14:02:40 2023, max compression
```

## Comparing `pybox-toolkit-0.1.6.dev4.tar` & `pybox-toolkit-0.1.7.dev3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:18:47.998732 pybox-toolkit-0.1.6.dev4/
--rw-r--r--   0 root         (0) root         (0)      479 2023-06-11 12:18:47.998732 pybox-toolkit-0.1.6.dev4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-05-30 13:22:09.000000 pybox-toolkit-0.1.6.dev4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-24 11:45:04.000000 pybox-toolkit-0.1.6.dev4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-11 12:18:47.998732 pybox-toolkit-0.1.6.dev4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:18:47.986732 pybox-toolkit-0.1.6.dev4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:18:47.986732 pybox-toolkit-0.1.6.dev4/src/pybox_toolkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      479 2023-06-11 12:18:47.000000 pybox-toolkit-0.1.6.dev4/src/pybox_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      398 2023-06-11 12:18:47.000000 pybox-toolkit-0.1.6.dev4/src/pybox_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-11 12:18:47.000000 pybox-toolkit-0.1.6.dev4/src/pybox_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-11 12:18:47.000000 pybox-toolkit-0.1.6.dev4/src/pybox_toolkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-11 12:18:47.000000 pybox-toolkit-0.1.6.dev4/src/pybox_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:18:47.986732 pybox-toolkit-0.1.6.dev4/src/toolkit/
--rw-rw-rw-   0 root         (0) root         (0)    15619 2023-06-11 12:18:08.000000 pybox-toolkit-0.1.6.dev4/src/toolkit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:18:47.986732 pybox-toolkit-0.1.6.dev4/src/toolkit/graphing/
--rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-05 18:07:33.000000 pybox-toolkit-0.1.6.dev4/src/toolkit/graphing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:18:47.986732 pybox-toolkit-0.1.6.dev4/src/toolkit/test/
--rw-rw-rw-   0 root         (0) root         (0)     5222 2023-05-30 15:20:01.000000 pybox-toolkit-0.1.6.dev4/src/toolkit/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:18:47.998732 pybox-toolkit-0.1.6.dev4/src/toolkit/typing/
--rw-rw-rw-   0 root         (0) root         (0)     7471 2023-06-11 12:18:08.000000 pybox-toolkit-0.1.6.dev4/src/toolkit/typing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-01 16:04:17.000000 pybox-toolkit-0.1.6.dev4/src/toolkit/typing/si.py
--rw-rw-rw-   0 root         (0) root         (0)     6861 2023-06-11 12:18:08.000000 pybox-toolkit-0.1.6.dev4/src/toolkit/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:02:40.644549 pybox-toolkit-0.1.7.dev3/
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-15 14:02:40.644549 pybox-toolkit-0.1.7.dev3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-05-30 13:22:09.000000 pybox-toolkit-0.1.7.dev3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-24 11:45:04.000000 pybox-toolkit-0.1.7.dev3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 14:02:40.644549 pybox-toolkit-0.1.7.dev3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:02:40.640549 pybox-toolkit-0.1.7.dev3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:02:40.644549 pybox-toolkit-0.1.7.dev3/src/pybox_toolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-15 14:02:40.000000 pybox-toolkit-0.1.7.dev3/src/pybox_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      398 2023-06-15 14:02:40.000000 pybox-toolkit-0.1.7.dev3/src/pybox_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 14:02:40.000000 pybox-toolkit-0.1.7.dev3/src/pybox_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-15 14:02:40.000000 pybox-toolkit-0.1.7.dev3/src/pybox_toolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-15 14:02:40.000000 pybox-toolkit-0.1.7.dev3/src/pybox_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:02:40.644549 pybox-toolkit-0.1.7.dev3/src/toolkit/
+-rw-rw-rw-   0 root         (0) root         (0)    15087 2023-06-15 14:02:16.000000 pybox-toolkit-0.1.7.dev3/src/toolkit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:02:40.644549 pybox-toolkit-0.1.7.dev3/src/toolkit/graphing/
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-05 18:07:33.000000 pybox-toolkit-0.1.7.dev3/src/toolkit/graphing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:02:40.644549 pybox-toolkit-0.1.7.dev3/src/toolkit/test/
+-rw-rw-rw-   0 root         (0) root         (0)     5222 2023-05-30 15:20:01.000000 pybox-toolkit-0.1.7.dev3/src/toolkit/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:02:40.644549 pybox-toolkit-0.1.7.dev3/src/toolkit/typing/
+-rw-rw-rw-   0 root         (0) root         (0)     9875 2023-06-12 14:14:27.000000 pybox-toolkit-0.1.7.dev3/src/toolkit/typing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-01 16:04:17.000000 pybox-toolkit-0.1.7.dev3/src/toolkit/typing/si.py
+-rw-rw-rw-   0 root         (0) root         (0)     7802 2023-06-12 14:14:27.000000 pybox-toolkit-0.1.7.dev3/src/toolkit/utils.py
```

### Comparing `pybox-toolkit-0.1.6.dev4/pyproject.toml` & `pybox-toolkit-0.1.7.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.6.dev4/src/toolkit/__init__.py` & `pybox-toolkit-0.1.7.dev3/src/toolkit/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 """Toolkit is a library for creating and testing formulas."""
 
-import sys
-from collections import defaultdict
 from typing import Any, Callable, Optional, Union
 from sys import stdout
+import mpmath
 
 import sympy
 from sympy.core.basic import Basic as SympyBasic
-from typing_extensions import Type, TypeVar, Self
-
+from typing_extensions import Type, Self
 
 from toolkit import test
-from toolkit.typing import Unit, _UnitClassParser
+from toolkit.typing import Unit, BaseUnit, _UnitClassParser
 from toolkit.utils import (
     parse_interval,
+    map_dictionary_value,
+    map_dictionary_key,
     ArgumentException,
     DocumentationException,
     RangeException,
     RuntimeException,
     TestingException,
     ex_assert,
 )
 
-T = TypeVar("T")
-U = TypeVar("U")
-V = TypeVar("V")
-
 class BaseFormula:
     """
     Contains information about a formula, including:
             - Parameter ranges
             - Labels
             - Documentation
     """
 
     formulas: list[Self] = []
     outputs: list[tuple[str, Unit]] = []
-    tentative_ranges: dict[str, str] = {}
     test_class: test.ToolkitTests = None
 
     def __init__(self, function: Callable[..., Any], **kwargs):
         if "outputs" not in kwargs:
             raise ArgumentException(
                 f"Function '{function.__qualname__}' does not have any outputs defined"
             )
@@ -58,97 +53,78 @@
 
         self.__dict__.update(kwargs)
         self.docs: str = function.__doc__
         self.function: Callable[..., Any] = function
         self.num_args: int = function.__code__.co_argcount
         self.arg_names: list[str] = function.__code__.co_varnames[:self.num_args]
         self.name: str = function.__qualname__.replace("_", " ").title()
-        self.parsed_ranges: defaultdict[str, tuple[float, float]] = defaultdict(dict)
-        self.variable_types: dict[str, Unit] = {}
+        self.variable_types: dict[str, BaseUnit] = {}
 
         for variable in self.arg_names:
             if variable not in function.__annotations__:
                 raise ArgumentException(
                     f"Variable '{variable}' in '{function.__qualname__}' is missing a type"
                 )
 
             self.variable_types[variable] = function.__annotations__[variable]
-            self.parse_variable(variable, self.variable_types[variable])
+            self.check_variable(variable, self.variable_types[variable])
 
         for output_name, output_type in self.outputs:
             self.variable_types[output_name] = output_type
-            self.parse_variable(output_name, output_type)
-
-        if "tentative_ranges" in self.__dict__:
-            for variable, tentative_range in self.tentative_ranges.items():
-                self.parsed_ranges[variable]["tentative"] = parse_interval(
-                    tentative_range
-                )
+            self.check_variable(output_name, output_type)
 
         BaseFormula.formulas.append(self)
 
+    def prepare_output_list(self, output_list: list[dict[str, BaseUnit]]) -> list[dict[str, BaseUnit]]:
+        """Prepare a list of dictionaries of outputs by:
+            1. Checking variables are in their physical range or are a choice
+            2. Variables are not a complex type returned by mpmath
+            3. Converting all mpmath specific types to default types
+
+        Args:
+            output_list (list[dict[str, BaseUnit]]]): list of outputs
+
+        Returns:
+            list[dict[str, BaseUnit]]: lists of outputs in their physical range
+        """
+        results = list(filter(self.filter_variable_dictionary, output_list))
+
+        if len(results) == 0:
+            raise RuntimeException(
+                f"No outputs were produced for '{self.name}'. The arguments may have been insufficient to solve the equation"  # pylint: disable=line-too-long
+            )
+
+        return results
+
     def filter_variable_dictionary(
         self, variable_dic: dict[str, Union[float, int]]
     ) -> bool:
         """Filter a dictionary of variables to see if they are in the physical range
 
         Args:
             variable_dic (dict[str, Union[float, int]]): Dictionary of variables to be checked
 
         Returns:
             bool: True if all variables are in the physical range, False otherwise
         """
         for name, value in variable_dic.items():
-            if not self.in_physical_range(name, value):
+            if not self.variable_types[name].possible(value):
                 return False
         return True
 
-    def in_physical_range(self, name: str, value: Union[float, int]) -> bool:
-        """Check if a value is in the physical range of a variable
-
-        Args:
-            name (str): Dictionary key of the variable
-            value (Union[float, int]): Value to be checked
-
-        Raises:
-            RangeException: If the variable range was not parsed.
-
-        Returns:
-            bool: True if the value is in the physical range, False otherwise.
-        """
-        if name not in self.parsed_ranges:
-            raise RangeException(
-                f"Could not check the physical range of '{name}', it was not parsed"
-            )
-
-        physical_range = self.parsed_ranges[name]["physical"]
-
-        return physical_range[0] <= value <= physical_range[1]
-
-    def parse_variable(self, variable: str, variable_type_instance: Unit):
-        """Parse a variable and add it to the parsed_ranges dictionary
+    def check_variable(self, variable: str, variable_type_instance: Unit):
+        """Checks a variable is an appropriate type
 
         Args:
             variable (str): Name of the variable
             variable_class (Unit): Unit class of the variable
 
         Raises:
             ArgumentException: If the variable class is not derived from Unit
         """
-        if not isinstance(variable_type_instance, Unit):
-            if isinstance(variable_type_instance, _UnitClassParser):
-                raise ArgumentException(
-                    f"Variable '{variable}' does not have an argument description"
-                )
-
-            raise ArgumentException(
-                f"Variable '{variable}' has a class not derived from Unit"
-            )
-
-        self.parsed_ranges[variable]["physical"] = variable_type_instance.parsed_physical_range
 
     def run_tests(self, output_stream = stdout) -> bool:
         """Run all tests for this formula
 
         Raises:
             TestingException: If the formula does not have a test class
 
@@ -183,45 +159,14 @@
         return function_class(function)
 
     def wrapper(function: Optional[Callable[..., Any]]) -> BaseFormula:
         return function_class(function, **kwargs)
 
     return wrapper
 
-
-def map_dictionary_value(
-    function: Callable[[U], V], dictionary: dict[T, U]
-) -> dict[T, V]:
-    """Map a function over the values of a dictionary
-
-    Args:
-        function (Callable[[U], V]): Mapping function
-        dictionary (dict[T, U]): Dictionary to be mapped over
-
-    Returns:
-        dict[T, V]: Mapped dictionary
-    """
-    return dict(map(lambda t: (t[0], function(t[1])), dictionary.items()))
-
-
-def map_dictionary_key(
-    function: Callable[[T], V], dictionary: dict[T, U]
-) -> dict[V, U]:
-    """Map a function over the keys of a dictionary
-
-    Args:
-        function (Callable[[T], V]): Mapping function
-        dictionary (dict[T, U]): Dictionary to be mapped over
-
-    Returns:
-        dict[V, U]: Mapped dictionary
-    """
-    return dict(map(lambda t: (function(t[0]), t[1]), dictionary.items()))
-
-
 class _PureFormula(BaseFormula):
     def __init__(self, function: Callable[..., SympyBasic], **kwargs):
         super().__init__(function, **kwargs)
         self.variable_symbols: dict[str, sympy.Symbol] = {}
 
         for variable in self.variable_types:
             self.variable_symbols[variable] = sympy.Symbol(variable)
@@ -235,14 +180,34 @@
 
         self.sympy_equations = tuple(
             sympy.Eq(equation, self.variable_symbols[output[0]])
             for (equation, output) in zip(sympy_function, self.outputs)
         )
         self.cached_lambdas = {}
 
+    def check_variable(self, variable: str, variable_type_instance: Unit):
+        """Parse a variable and add it to the parsed_ranges dictionary
+
+        Args:
+            variable (str): Name of the variable
+            variable_class (Unit): Unit class of the variable
+
+        Raises:
+            ArgumentException: If the variable class is not derived from Unit
+        """
+        if not isinstance(variable_type_instance, Unit):
+            if isinstance(variable_type_instance, _UnitClassParser):
+                raise ArgumentException(
+                    f"Variable '{variable}' does not have an argument description"
+                )
+
+            raise ArgumentException(
+                f"Variable '{variable}' has a class not derived from Unit"
+            )
+
     def execute_lambda_dictionary_list(
         self,
         dic_list: list[dict[str, SympyBasic]],
         kwargs: dict[str, int],
         argument_list: list[str],
     ) -> list[dict[str, Union[float, int]]]:
         """Execute a list of dictionaries of lambdified functions over provided arguments.
@@ -262,31 +227,23 @@
         Returns:
             list[dict[str, Union[float, int]]]: List of dictionaries containing the outputs of the lambdified functions
         """
         # Please do not write code like this, thank you and bye
         results = list(
             map(
                 lambda dic: map_dictionary_value(
-                    lambda lambdified: float(lambdified(
+                    lambda lambdified: lambdified(
                         *(kwargs[arg] for arg in argument_list)
-                    )),
+                    ),
                     dic,
                 ),
                 dic_list,
             )
         )
 
-        # Add a filter to check that the outputs are physically possible
-        results = list(filter(self.filter_variable_dictionary, results))
-
-        if len(results) == 0:
-            raise RuntimeException(
-                f"No outputs were produced for '{self.name}' with arguments {argument_list}. It may have been insufficient to solve the equation"  # pylint: disable=line-too-long
-            )
-
         return results
 
     def __call__(
         self, *args: tuple[Unit, ...], **kwargs
     ) -> list[dict[str, float]]:
         """Execute the formula with the provided arguments
 
@@ -296,36 +253,36 @@
         Returns:
             list[dict[str, float]]: List of dictionaries containing outputs of the formula
                                           (one dictionary per possible solution)
         """
         if len(args) == self.num_args or set(kwargs) == set(self.arg_names):
             inputs = args if len(args) == self.num_args else [kwargs[i] for i in self.arg_names]
             for name, value in zip(self.arg_names, inputs):
-                if not self.in_physical_range(name, value):
+                if not self.variable_types[name].possible(value):
                     raise RangeException(
-                        f"Variable '{name}' outside of physical range: {self.parsed_ranges[name]['physical']}"
+                        f"Variable '{name}' outside of physical range or choices."
                     )
 
             result = self.function(*args, **kwargs)
             if not isinstance(result, tuple):
                 result = (result,)
-            return [dict(zip(map(lambda x: x[0], self.outputs), result))]
+            return self.prepare_output_list([dict(zip(map(lambda x: x[0], self.outputs), result))])
 
         for name, value in kwargs.items():
-            if not self.in_physical_range(name, value):
+            if not self.variable_types[name].possible(value):
                 raise RangeException(
-                    f"Variable '{name}' outside of physical range: {self.parsed_ranges[name]['physical']}"
+                    f"Variable '{name}' outside of physical range or choices."
                 )
 
         argument_list = tuple(sorted((i for i in kwargs)))
         non_argument_list = sorted((i for i in self.variable_types if i not in kwargs))
         if argument_list in self.cached_lambdas:
-            return self.execute_lambda_dictionary_list(
+            return self.prepare_output_list(self.execute_lambda_dictionary_list(
                 self.cached_lambdas[argument_list], kwargs, argument_list
-            )
+            ))
 
         known_symbols = [self.variable_symbols[arg] for arg in argument_list]
         unknown_symbols = [self.variable_symbols[sym] for sym in non_argument_list]
 
         # This shit either returns a dictionary of independent variables
         # or a list of tuples of dependent equations
         solved = sympy.solve(self.sympy_equations, *unknown_symbols)
@@ -342,24 +299,24 @@
             # in physical range checks
             solved = [map_dictionary_key(str, solved)]
 
         # We map over the dictionaries entries to get the lambdas tied to each variable
         lambdifieds = list(
             map(
                 lambda dic: map_dictionary_value(
-                    lambda equation: sympy.lambdify(known_symbols, equation),
+                    lambda equation: sympy.lambdify(known_symbols, equation, modules = ["math"]),
                     dic,
                 ),
                 solved,
             )
         )
 
         self.cached_lambdas[argument_list] = lambdifieds
 
-        return self.execute_lambda_dictionary_list(lambdifieds, kwargs, argument_list)
+        return self.prepare_output_list(self.execute_lambda_dictionary_list(lambdifieds, kwargs, argument_list))
 
 
 class _ImpureFormula(BaseFormula):
     def __call__(self, *args: tuple[Unit, ...], **kwargs) -> list[dict[str, float, int]]:
         """Call the impure formula.
 
         Raises:
@@ -374,23 +331,39 @@
         else:
             if set(kwargs) != set(function_arguments):
                 raise ArgumentException(f"""Keyword arguments for impure expression must match its arguments:
                 {tuple(kwargs)} does not match {function_arguments} for {self.name}.""")
             inputs = [kwargs[i] for i in self.arg_names]
 
         for name, value in zip(self.arg_names, inputs):
-            if not self.in_physical_range(name, value):
+            if not self.variable_types[name].possible(value):
                 raise RangeException(
-                    f"Variable '{name}' outside of physical range: {self.parsed_ranges[name]['physical']}"
+                    # Idea, add function to get the last part of the error message
+                    f"Variable '{name}' outside of physical range or choices." 
                 )
 
         result = self.function(*args, **kwargs)
         if not isinstance(result, tuple):
             result = (result,)
-        return [dict(zip(map(lambda x: x[0], self.outputs), result))]
+        return self.prepare_output_list([dict(zip(map(lambda x: x[0], self.outputs), result))])
+
+    def check_variable(self, variable: str, variable_type_instance: Unit):
+        """Parse a variable and add it to the parsed_ranges dictionary
+
+        Args:
+            variable (str): Name of the variable
+            variable_class (Unit): Unit class of the variable
+
+        Raises:
+            ArgumentException: If the variable class is not derived from Unit
+        """
+        if not isinstance(variable_type_instance, BaseUnit):
+            raise ArgumentException(
+                f"Variable '{variable}' has a class not derived from BaseUnit"
+            )
 
 def PureFormula(  # pylint: disable=invalid-name
     func: Optional[Callable[..., SympyBasic]] = None, **kwargs
 ) -> _PureFormula:
     """Annotation for the pure formulas.
     These formulas can only contain sympy functions and operations, and must return a single sympy expression.
```

### Comparing `pybox-toolkit-0.1.6.dev4/src/toolkit/graphing/__init__.py` & `pybox-toolkit-0.1.7.dev3/src/toolkit/graphing/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.6.dev4/src/toolkit/test/__init__.py` & `pybox-toolkit-0.1.7.dev3/src/toolkit/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.6.dev4/src/toolkit/typing/__init__.py` & `pybox-toolkit-0.1.7.dev3/src/toolkit/typing/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Data types and underlying mechanisms """
-
-from typing_extensions import Self
+from dataclasses import dataclass
+from typing import Union
 
 from toolkit.utils import (
     parse_interval,
     stringify_interval,
     physical_range_power,
     physical_range_division,
     physical_range_multiplication,
@@ -177,24 +177,85 @@
 
         # We do not check hasattr here, because the Unit base class is guaranteed to have a type list
         if "type_list" not in new_type.__dict__:
             new_type.type_list = ((new_type, 1),)
 
         return new_type
 
-class Unit(float, metaclass=_UnitClassParser):
+class BaseUnit:
+    """ Base units from which all units derive """
+    def __init__(self, description: str, default: Union[str, float, int] = None):
+        self.description = description
+        self.default = default
+
+@dataclass
+class ChoiceEntry:
+    """ A choice in a multiple-choice parameter """
+    value: Union[str, float, int]
+    name: str = None
+    description: str = None
+
+    def __init__(self, value, name = None, description = None):
+        self.value = value
+        self.name = str(value) if name is None else name
+        self.description = description
+
+class Choice(BaseUnit):
+    """ Represents a multiple-choice parameter type in an impure formula """
+    def __init__(self, choices: list[ChoiceEntry], description: str, default = None):
+        self.choices = choices
+        super().__init__(description, default)
+
+        used_names = set()
+
+        if not isinstance(choices, list):
+            raise ArgumentException(
+                f"Choices should be a list, '{type(choices)}' given."
+            )
+
+        if len(choices) < 2:
+            raise ArgumentException(
+                f"Choice parameter should have more than 2 available options, {len(choices)} given."
+            )
+
+        choice_type = type(self.choices[0].value)
+        for choice in self.choices:
+            if choice.name in used_names:
+                raise ArgumentException(
+                    f"Choice entries cannot have duplicate names, duplicate found for '{choice.name}'."
+                )
+            used_names.add(choice.name)
+
+            if not isinstance(choice.value, choice_type):
+                raise ArgumentException(
+                    f"Types of choice entries should be homogenous, '{choice_type}' and '{type(choice.value)}' differ."
+                )
+
+        self.possible_values = set(choice.value for choice in self.choices)
+
+    def possible(self, value: Union[float, str]) -> bool:
+        """ Checks whether a unit is possible (in physical range) """
+        return value in self.possible_values
+
+class Unit(BaseUnit, metaclass=_UnitClassParser):
     """Base class for all units"""
 
     units: str = ""
     physical_range: str = "(-inf, inf)"
+    parsed_tentative_range: tuple[float, float] = (float("-inf"), float("inf"))
 
-    def __new__(cls, description: str, physical_range: str = None): # pylint: disable=unused-argument
-        return super().__new__(cls, 0)
-
-    def __init__(self, description: str, physical_range: str = None):
-        super().__init__()
+    def __init__(self, description: str, tentative_range: str = None,
+                 default: Union[str, float, int] = None, physical_range: str = None):
+        super().__init__(description, default)
 
         self.description = description
 
+        if tentative_range is not None:
+            self.parsed_tentative_range = parse_interval(tentative_range)
+
         if physical_range is not None:
-            self.__class__.parsed_physical_range = parse_interval(physical_range)
-            self.__class__.physical_range = physical_range
+            self.parsed_physical_range = parse_interval(physical_range)
+            self.physical_range = physical_range
+
+    def possible(self, value: float) -> bool:
+        """ Checks whether a unit is possible (in physical range) """
+        return self.parsed_physical_range[0] <= value <= self.parsed_physical_range[1]
```

### Comparing `pybox-toolkit-0.1.6.dev4/src/toolkit/typing/si.py` & `pybox-toolkit-0.1.7.dev3/src/toolkit/typing/si.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.6.dev4/src/toolkit/utils.py` & `pybox-toolkit-0.1.7.dev3/src/toolkit/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 """Miscelaneous utilities for the toolkit"""
 
 from math import copysign, isnan
 from collections.abc import Iterable
+from typing import Callable
+from typing_extensions import TypeVar
+
+T = TypeVar("T")
+U = TypeVar("U")
+V = TypeVar("V")
 
 class ToolkitException(Exception):
     """Base class for exceptions in the toolkit."""
 
 
 class RangeException(ToolkitException):
     """Exception raised for invalid range or out-of range variables."""
@@ -207,8 +213,36 @@
     Args:
         exponent (int): integer exponent
 
     Returns:
         str: exponent unicode
     """
     return "".join(_UNICODE_DIGITS[digit] for digit in str(exponent))
-    
+
+def map_dictionary_value(
+    function: Callable[[U], V], dictionary: dict[T, U]
+) -> dict[T, V]:
+    """Map a function over the values of a dictionary
+
+    Args:
+        function (Callable[[U], V]): Mapping function
+        dictionary (dict[T, U]): Dictionary to be mapped over
+
+    Returns:
+        dict[T, V]: Mapped dictionary
+    """
+    return dict(map(lambda t: (t[0], function(t[1])), dictionary.items()))
+
+
+def map_dictionary_key(
+    function: Callable[[T], V], dictionary: dict[T, U]
+) -> dict[V, U]:
+    """Map a function over the keys of a dictionary
+
+    Args:
+        function (Callable[[T], V]): Mapping function
+        dictionary (dict[T, U]): Dictionary to be mapped over
+
+    Returns:
+        dict[V, U]: Mapped dictionary
+    """
+    return dict(map(lambda t: (function(t[0]), t[1]), dictionary.items()))
```

