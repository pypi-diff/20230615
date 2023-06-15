# Comparing `tmp/rpn_calc-0.2.2.tar.gz` & `tmp/rpn_calc-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpn_calc-0.2.2.tar", last modified: Mon Oct 18 18:56:26 2021, max compression
+gzip compressed data, was "rpn_calc-0.2.3.tar", last modified: Thu Jun 15 08:53:21 2023, max compression
```

## Comparing `rpn_calc-0.2.2.tar` & `rpn_calc-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 18:56:26.343115 rpn_calc-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2021-10-18 18:56:12.000000 rpn_calc-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7641 2021-10-18 18:56:26.343115 rpn_calc-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5254 2021-10-18 18:56:12.000000 rpn_calc-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 18:56:26.343115 rpn_calc-0.2.2/rpn_calc/
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-10-18 18:56:12.000000 rpn_calc-0.2.2/rpn_calc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1982 2021-10-18 18:56:12.000000 rpn_calc-0.2.2/rpn_calc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18128 2021-10-18 18:56:12.000000 rpn_calc-0.2.2/rpn_calc/calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 18:56:26.343115 rpn_calc-0.2.2/rpn_calc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7641 2021-10-18 18:56:25.000000 rpn_calc-0.2.2/rpn_calc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      309 2021-10-18 18:56:26.000000 rpn_calc-0.2.2/rpn_calc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-18 18:56:25.000000 rpn_calc-0.2.2/rpn_calc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-10-18 18:56:25.000000 rpn_calc-0.2.2/rpn_calc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-10-18 18:56:25.000000 rpn_calc-0.2.2/rpn_calc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-10-18 18:56:25.000000 rpn_calc-0.2.2/rpn_calc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-18 18:56:26.343115 rpn_calc-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2021-10-18 18:56:12.000000 rpn_calc-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 18:56:26.343115 rpn_calc-0.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (121)    18619 2021-10-18 18:56:12.000000 rpn_calc-0.2.2/test/test_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:53:21.650057 rpn_calc-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-15 08:53:09.000000 rpn_calc-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-15 08:53:21.650057 rpn_calc-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-06-15 08:53:09.000000 rpn_calc-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:53:21.650057 rpn_calc-0.2.3/rpn_calc/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-15 08:53:09.000000 rpn_calc-0.2.3/rpn_calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-15 08:53:09.000000 rpn_calc-0.2.3/rpn_calc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-06-15 08:53:09.000000 rpn_calc-0.2.3/rpn_calc/calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:53:21.650057 rpn_calc-0.2.3/rpn_calc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-15 08:53:21.000000 rpn_calc-0.2.3/rpn_calc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-15 08:53:21.000000 rpn_calc-0.2.3/rpn_calc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 08:53:21.000000 rpn_calc-0.2.3/rpn_calc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 08:53:21.000000 rpn_calc-0.2.3/rpn_calc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 08:53:21.000000 rpn_calc-0.2.3/rpn_calc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 08:53:21.000000 rpn_calc-0.2.3/rpn_calc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 08:53:21.650057 rpn_calc-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-15 08:53:09.000000 rpn_calc-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:53:21.650057 rpn_calc-0.2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-06-15 08:53:09.000000 rpn_calc-0.2.3/test/test_calculator.py
```

### Comparing `rpn_calc-0.2.2/LICENSE` & `rpn_calc-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rpn_calc-0.2.2/PKG-INFO` & `rpn_calc-0.2.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,208 +1,225 @@
 Metadata-Version: 2.1
 Name: rpn_calc
-Version: 0.2.2
+Version: 0.2.3
 Summary: RPN calculator
 Home-page: https://github.com/Allain18/pol
 Author: Alain Girard
 Author-email: alaingirardvd@gmail.com
 License: MIT License
-Description: # pol
-        [![Build Status](https://travis-ci.com/Allain18/pol.svg?branch=master)](https://travis-ci.com/Allain18/pol)
-        
-        Command line calculator using [reverse polish notation](https://en.wikipedia.org/wiki/Reverse_Polish_notation)
-        
-        Decimal, hexadecimal, binary and octal number are supported
-        
-        ## Usage
-        As a command line tool: __pol__
-        
-        ```
-        ~$ pol
-        Reverse polish notation calculator
-        >5 10 * dec
-        50
-        >0xA 0x6 + hex
-        0x10
-        >q //quit the program
-        ~$
-        ```
-        
-        Instructions are [below](#list-of-commands)
-        
-        pol can also be use as a module
-        ```python 
-        import rpn_calc
-        cal = rpn_calculator.Calculator()
-        cal.evaluate("1 2 + dec")
-        # print 3
-        ```
-        
-        ## Install
-        pol can be install from pip
-        ```
-        pip install rpn-calc
-        ```
-        If you want to install from a source distribution, extract the tarball and run the following command
-        ```
-        python setup.py install
-        ```
-        
-        ## Documentation
-        This README is the Documentation
-        
-        ## [Repo](https://github.com/Allain18/pol)
-        The code is on github
-        
-        ## Config file
-        You can write your own command
-        
-        By default commands from file ~/pol.yml (if exists) are add to the calculator
-        
-        You can add other files with the flag -f/--file
-        
-        Config files are written in YAML
-        
-        ### Currently supported parameters
-        - shortcut: shortcut to commands (see example below)
-        - rounding: parameter used to round number (default: 0)
-        
-        ### Example of a valid config file
-        ```YAML
-        shortcut:
-         - double = 2 * # double the last value of the stack
-         - 10* = 10 switch ** # same as 10 {x} **
-        rounding: 3
-        ```
-        Command must be on the format {name_of_command = command}
-        
-        ## Options
-        ```
-        usage: pol [-h] [-v] [-l] [--ignore-local-config] [-f FILE [FILE ...]]
-        
-        A RPN calculator written in python
-        Support decimal, hexadecimal, binary and octal
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -v, --version         show the version number and exit
-          -l, --list            list all commands available and exit
-          --ignore-local-config
-                                don't add commands from ~/.pol
-          -f FILE [FILE ...], --file FILE [FILE ...]
-                                file with customs commands
-        ```
-        ## List of commands
-        `+` : Take 2 numbers from the stack, add them and put the result in the stack
-        
-        `-` : Take 2 numbers from the stack, substracte them and put the result in the stack
-        
-        `*` : Take 2 numbers from the stack, mul them and put the result in the stack
-        
-        `/` : Take 2 numbers from the stack, divise them and put the result in the stack
-        
-        `//` : Take 2 numbers from the stack, divise them and put the integer result in the stack
-        
-        `%` : Take 2 numbers from the stack, divise them and put the remainder in the stack
-        
-        `**` : Take 2 numbers from the stack, apply power and put the result in the stack
-        
-        `sqrt` : Replace the last number in the stack with the square root of itself
-        
-        `exp` : Apply e**x to the last number of the stack
-        
-        `log10` : Apply log10 to the last number of the stack
-        
-        `log2` : Apply log2 to the last number of the stack
-        
-        `ln` : Apply natural logarithm to the last number of the stack
-        
-        `and` : Take 2 numbers from the stack, apply a bitwise "and" and put the result in the stack
-        
-        `or` : Take 2 numbers from the stack, apply a bitwise "or" and put the result in the stack
-        
-        `xor` : Take 2 numbers from the stack, apply a bitwise "xor" and put the result in the stack
-        
-        `<<` : Take 2 numbers from the stack, apply a left shift and put the result in the stack
-        
-        `>>` : Take 2 numbers from the stack, apply a right shift and put the result in the stack
-        
-        `abs` : Make absolute the last value of the stack
-        
-        `inv` : Inverse the last number of the stack
-        
-        `neg` : Change the sign of the last number in the stack
-        
-        `sin` : Replace the last number in the stack with the sine of itself (measured in radians)
-        
-        `cos` : Replace the last number in the stack with the cosine of itself (measured in radians)
-        
-        `tan` : Replace the last number in the stack with the tangent of itself (measured in radians)
-        
-        `asin` : Replace the last number in the stack with the arc sine of itself (measured in radians)
-        
-        `acos` : Replace the last number in the stack with the arc cosine of itself (measured in radians)
-        
-        `atan` : Replace the last number in the stack with the arc tangent of itself (measured in radians)
-        
-        `torad` : Convert the last number from degree to radian
-        
-        `todeg` : Convert the last number from radian to degree
-        
-        `switch` : Switch the last 2 numbers of the stack
-        
-        `del` : Delete the last number in the stack
-        
-        `copy` : Copy the last number of the stack and add it to the stack
-        
-        `pi` : Add pi to the stack
-        
-        `tau` : Add tau to the stack
-        
-        `e` : Add e to the stack
-        
-        `sum` : Take all the number of the stack and add the sum
-        
-        `fact` : Replace the last number in the stack with its factorial
-        
-        `round` : Round the last number in the stack
-        
-        `ave` : Take all the number of the stack and add the average
-        
-        `dec` : Print the last number of the stack and remove it
-        
-        `hex` : Print in hexadecimal format the last number of the stack and remove it
-        
-        `bin` : Print in binary format the last number of the stack and remove it
-        
-        `oct` : Print in octal format the last number of the stack and remove it
-        
-        `ratio` : Print in integer ratio format the last number of the stack and remove it
-        
-        `s` : Print the stack
-        
-        `clear` : Empty the stack
-        
-        `help` : Print help; Same as pol --list
-        
-        `q` : Quit the program
-        
-        ## License
-        
-        MIT
-        
 Keywords: rpn,calculator,reverse polish notation
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pol
+[![Build Status](https://travis-ci.com/Allain18/pol.svg?branch=master)](https://travis-ci.com/Allain18/pol)
+
+Command line calculator using [reverse polish notation](https://en.wikipedia.org/wiki/Reverse_Polish_notation)
+
+Decimal, hexadecimal, binary and octal number are supported
+
+## Usage
+As a command line tool: __pol__
+
+```
+~$ pol
+Reverse polish notation calculator
+>5 10 * dec
+50
+>0xA 0x6 + hex
+0x10
+>q //quit the program
+~$
+```
+
+Instructions are [below](#list-of-commands)
+
+pol can also be use as a module
+```python 
+import rpn_calc
+cal = rpn_calculator.Calculator()
+cal.evaluate("1 2 + dec")
+# print 3
+```
+
+## Install
+pol can be install from pip
+```
+pip install rpn-calc
+```
+If you want to install from a source distribution, extract the tarball and run the following command
+```
+python setup.py install
+```
+
+## Documentation
+This README is the Documentation
+
+## [Repo](https://github.com/Allain18/pol)
+The code is on github
+
+## Config file
+You can write your own command
+
+By default commands from file ~/pol.yml (if exists) are add to the calculator
+
+You can add other files with the flag -f/--file
+
+Config files are written in YAML
+
+### Currently supported parameters
+- shortcut: shortcut to commands (see example below)
+- rounding: parameter used to round number (default: 0)
+
+### Example of a valid config file
+```YAML
+shortcut:
+ - double = 2 * # double the last value of the stack
+ - 10* = 10 switch ** # same as 10 {x} **
+rounding: 3
+```
+Command must be on the format {name_of_command = command}
+
+## Options
+```
+usage: pol [-h] [-v] [-l] [--ignore-local-config] [-f FILE [FILE ...]]
+
+A RPN calculator written in python
+Support decimal, hexadecimal, binary and octal
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -v, --version         show the version number and exit
+  -l, --list            list all commands available and exit
+  --ignore-local-config
+                        don't add commands from ~/.pol
+  -f FILE [FILE ...], --file FILE [FILE ...]
+                        file with customs commands
+```
+## List of commands
+`+` : Take 2 numbers from the stack, add them and put the result in the stack
+
+`-` : Take 2 numbers from the stack, substracte them and put the result in the stack
+
+`*` : Take 2 numbers from the stack, mul them and put the result in the stack
+
+`/` : Take 2 numbers from the stack, divise them and put the result in the stack
+
+`//` : Take 2 numbers from the stack, divise them and put the integer result in the stack
+
+`%` : Take 2 numbers from the stack, divise them and put the remainder in the stack
+
+`**` : Take 2 numbers from the stack, apply power and put the result in the stack
+
+`sqrt` : Replace the last number in the stack with the square root of itself
+
+`exp` : Apply e**x to the last number of the stack
+
+`log10` : Apply log10 to the last number of the stack
+
+`log2` : Apply log2 to the last number of the stack
+
+`ln` : Apply natural logarithm to the last number of the stack
+
+`and` : Take 2 numbers from the stack, apply a bitwise "and" and put the result in the stack
+
+`or` : Take 2 numbers from the stack, apply a bitwise "or" and put the result in the stack
+
+`xor` : Take 2 numbers from the stack, apply a bitwise "xor" and put the result in the stack
+
+`<<` : Take 2 numbers from the stack, apply a left shift and put the result in the stack
+
+`>>` : Take 2 numbers from the stack, apply a right shift and put the result in the stack
+
+`abs` : Make absolute the last value of the stack
+
+`inv` : Inverse the last number of the stack
+
+`neg` : Change the sign of the last number in the stack
+
+`sin` : Replace the last number in the stack with the sine of itself (measured in radians)
+
+`cos` : Replace the last number in the stack with the cosine of itself (measured in radians)
+
+`tan` : Replace the last number in the stack with the tangent of itself (measured in radians)
+
+`asin` : Replace the last number in the stack with the arc sine of itself (measured in radians)
+
+`acos` : Replace the last number in the stack with the arc cosine of itself (measured in radians)
+
+`atan` : Replace the last number in the stack with the arc tangent of itself (measured in radians)
+
+`atan2` : Take 2 numbers from the stack, apply a atan2 function and put the result in the stack
+
+`sinh` : Replace the last number in the stack with the hyperbolic sine of itself
+
+`cosh` : Replace the last number in the stack with the hyperbolic cosine of itself
+
+`tanh` : Replace the last number in the stack with the hyperbolic tangent of itself
+
+`asinh` : Replace the last number in the stack with the asinh of itself
+
+`acosh` : Replace the last number in the stack with the acosh of itself
+
+`atanh` : Replace the last number in the stack with the atanh of itself
+
+`torad` : Convert the last number from degree to radian
+
+`todeg` : Convert the last number from radian to degree
+
+`switch` : Switch the last 2 numbers of the stack
+
+`del` : Delete the last number in the stack
+
+`copy` : Copy the last number of the stack and add it to the stack
+
+`pi` : Add pi to the stack
+
+`tau` : Add tau to the stack
+
+`e` : Add e to the stack
+
+`sum` : Take all the number of the stack and add the sum
+
+`fact` : Replace the last number in the stack with its factorial
+
+`round` : Round the last number in the stack
+
+`ave` : Take all the number of the stack and add the average
+
+`dec` : Print the last number of the stack and remove it
+
+`hex` : Print in hexadecimal format the last number of the stack and remove it
+
+`bin` : Print in binary format the last number of the stack and remove it
+
+`oct` : Print in octal format the last number of the stack and remove it
+
+`ratio` : Print in integer ratio format the last number of the stack and remove it
+
+`s` : Print the stack
+
+`clear` : Empty the stack
+
+`back` : Put back on the stack the last value that was printed
+
+`help` : Print help; Same as pol --list
+
+`q` : Quit the program
+
+## License
+
+MIT
```

### Comparing `rpn_calc-0.2.2/README.md` & `rpn_calc-0.2.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -132,14 +132,28 @@
 
 `asin` : Replace the last number in the stack with the arc sine of itself (measured in radians)
 
 `acos` : Replace the last number in the stack with the arc cosine of itself (measured in radians)
 
 `atan` : Replace the last number in the stack with the arc tangent of itself (measured in radians)
 
+`atan2` : Take 2 numbers from the stack, apply a atan2 function and put the result in the stack
+
+`sinh` : Replace the last number in the stack with the hyperbolic sine of itself
+
+`cosh` : Replace the last number in the stack with the hyperbolic cosine of itself
+
+`tanh` : Replace the last number in the stack with the hyperbolic tangent of itself
+
+`asinh` : Replace the last number in the stack with the asinh of itself
+
+`acosh` : Replace the last number in the stack with the acosh of itself
+
+`atanh` : Replace the last number in the stack with the atanh of itself
+
 `torad` : Convert the last number from degree to radian
 
 `todeg` : Convert the last number from radian to degree
 
 `switch` : Switch the last 2 numbers of the stack
 
 `del` : Delete the last number in the stack
@@ -170,14 +184,16 @@
 
 `ratio` : Print in integer ratio format the last number of the stack and remove it
 
 `s` : Print the stack
 
 `clear` : Empty the stack
 
+`back` : Put back on the stack the last value that was printed
+
 `help` : Print help; Same as pol --list
 
 `q` : Quit the program
 
 ## License
 
 MIT
```

### Comparing `rpn_calc-0.2.2/rpn_calc/__main__.py` & `rpn_calc-0.2.3/rpn_calc/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 import argparse
 import pathlib
 
 import rpn_calc
 
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 
 def get_args():
     """Get the args from argparse"""
     parser = argparse.ArgumentParser(
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description="A RPN calculator written in python\n"
```

### Comparing `rpn_calc-0.2.2/rpn_calc/calculator.py` & `rpn_calc-0.2.3/rpn_calc/calculator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """File containing the Calculator object and get_number function"""
 
 import math
 from fractions import Fraction
+from decimal import Decimal
 import yaml
 
 
 def get_number(num):
     """If possible return a number, else return num as a string"""
     for cast in (int, float):
         try:
@@ -26,14 +27,16 @@
 
 class Calculator:
     """Class Calculator"""
 
     def __init__(self):
         self.stack = []
 
+        self.last = None
+
         self.loop_flag = True
 
         self.rounding_value = None
 
         self.operation = {
             "+": self.add,
             "-": self.sub,
@@ -57,14 +60,21 @@
             "neg": self.neg,
             "sin": self.sin,
             "cos": self.cos,
             "tan": self.tan,
             "asin": self.asin,
             "acos": self.acos,
             "atan": self.atan,
+            "atan2": self.atan2,
+            "sinh": self.sinh,
+            "cosh": self.cosh,
+            "tanh": self.tanh,
+            "asinh": self.asinh,
+            "acosh": self.acosh,
+            "atanh": self.atanh,
             "torad": self.to_radian,
             "todeg": self.to_degree,
             "switch": self.switch,
             "del": self.del_,
             "copy": self.copy,
             "pi": self.const_pi,
             "tau": self.const_tau,
@@ -76,14 +86,15 @@
             "dec": self.print_dec,
             "hex": self.print_hex,
             "bin": self.print_bin,
             "oct": self.print_oct,
             "ratio": self.ratio,
             "s": self.print_stack,
             "clear": self.clear_stack,
+            "back": self.back,
             "help": self.help,
             "q": self.quit
         }
 
         self.custom_commands = {}
 
     def loop(self):
@@ -99,27 +110,32 @@
         except (KeyboardInterrupt, EOFError):
             pass
 
     def evaluate(self, string):
         """Evaluate the string and calls adequate method"""
         for i in string.split():
             i = get_number(i)
-            if isinstance(i, (int, float)):
+            if isinstance(i, int):
                 self.stack.append(i)
+            elif isinstance(i, float):
+                if i.is_integer():
+                    self.stack.append(int(i))
+                else:
+                    self.stack.append(i)
 
             elif isinstance(i, str):
                 if i in self.operation:
                     self.operation[i]()
                 elif i in self.custom_commands:
                     self.evaluate(self.custom_commands[i])
                 else:
                     print("Unknow command: {}".format(i))
 
             else:
-                raise Exception("Should never happend")
+                raise RuntimeError("Should never happend")
 
     def add_config(self, existing_path):
         """Add command from existing path
            Command must be on the format "{name_of_command} = {command}" """
         with open(existing_path, "r", encoding="UTF-8") as file:
             try:
                 config = yaml.safe_load(file)
@@ -146,145 +162,175 @@
         """Check if enough number are in the stack"""
         if len(self.stack) < num:
             print("Not enough numbers in the stack for {} command".format(command))
             return False
 
         return True
 
+    def add_stack(self, val):
+        """Convert to int if possible and add to stack"""
+        if isinstance(val, int):
+            self.stack.append(val)
+        elif isinstance(val, float):
+            if val.is_integer():
+                self.stack.append(int(val))
+            else:
+                self.stack.append(val)
+        else:
+            raise ValueError("Wrong data type")
+
     def add(self):
         """Take 2 numbers from the stack, add them and put the result in the stack"""
         if self.check_stack(2, "+"):
             value1 = self.stack.pop()
             value2 = self.stack.pop()
-            self.stack.append(value1 + value2)
+            self.add_stack(value1 + value2)
 
     def sub(self):
         """Take 2 numbers from the stack, substracte them and put the result in the stack"""
         if self.check_stack(2, "-"):
             value1 = self.stack.pop()
             value2 = self.stack.pop()
-            self.stack.append(value2 - value1)
+            self.add_stack(value2 - value1)
 
     def mul(self):
         """Take 2 numbers from the stack, mul them and put the result in the stack"""
         if self.check_stack(2, "*"):
             value1 = self.stack.pop()
             value2 = self.stack.pop()
-            self.stack.append(value1 * value2)
+            self.add_stack(value1 * value2)
 
     def div(self):
         """Take 2 numbers from the stack, divise them and put the result in the stack"""
         if self.check_stack(2, "/"):
             value1 = self.stack.pop()
             if value1 == 0:
                 print("Impossible to divise by 0")
                 self.stack.append(value1)
             else:
                 value2 = self.stack.pop()
-                res = value2 / value1
-                if res.is_integer():
-                    self.stack.append(int(res))
+                d_res = Decimal(value2) / Decimal(value1)
+                if d_res.to_integral_value() == d_res:
+                    self.stack.append(int(d_res))
                 else:
-                    self.stack.append(res)
+                    self.stack.append(float(d_res))
 
     def int_div(self):
         """Take 2 numbers from the stack, divise them and put the integer result in the stack"""
         if self.check_stack(2, "//"):
             value1 = self.stack.pop()
             if value1 == 0:
                 print("Impossible to divise by 0")
                 self.stack.append(value1)
             else:
                 value2 = self.stack.pop()
-                self.stack.append(value2 // value1)
+                self.add_stack(value2 // value1)
 
     def modulo(self):
         """Take 2 numbers from the stack, divise them and put the remainder in the stack"""
         if self.check_stack(2, "%"):
             value1 = self.stack.pop()
             if value1 == 0:
                 print("Impossible to divise by 0")
                 self.stack.append(value1)
             else:
                 value2 = self.stack.pop()
-                self.stack.append(value2 % value1)
+                self.add_stack(value2 % value1)
 
     def pow(self):
         """Take 2 numbers from the stack, apply power and put the result in the stack"""
         if self.check_stack(2, "**"):
-            value1 = self.stack.pop()
-            value2 = self.stack.pop()
-            self.stack.append(value2 ** value1)
+            if self.stack[-2] == 0 and self.stack[-1] < 0:
+                print("Impossible to divise by 0")
+            else:
+                value1 = self.stack.pop()
+                value2 = self.stack.pop()
+                self.add_stack(value2 ** value1)
 
     def sqrt(self):
         """Replace the last number in the stack with the square root of itself"""
         if self.check_stack(1, "sqrt"):
             value = self.stack.pop()
             if value < 0:
                 print("Square root require non-negative value")
                 self.stack.append(value)
             else:
-                self.stack.append(math.sqrt(value))
+                self.add_stack(math.sqrt(value))
 
     def exp(self):
         """Apply e**x to the last number of the stack"""
         if self.check_stack(1, "exp"):
             value = self.stack.pop()
-            self.stack.append(math.exp(value))
+            self.add_stack(math.exp(value))
 
     def log10(self):
         """Apply log10 to the last number of the stack"""
         if self.check_stack(1, "log10"):
             value = self.stack.pop()
             if value > 0:
-                self.stack.append(math.log10(value))
+                self.add_stack(math.log10(value))
             else:
                 print("Number out of domain for logarithm")
                 self.stack.append(value)
 
     def log2(self):
         """Apply log2 to the last number of the stack"""
         if self.check_stack(1, "log2"):
             value = self.stack.pop()
             if value > 0:
-                self.stack.append(math.log2(value))
+                self.add_stack(math.log2(value))
             else:
                 print("Number out of domain for logarithm")
                 self.stack.append(value)
 
     def loge(self):
         """Apply natural logarithm to the last number of the stack"""
         if self.check_stack(1, "loge"):
             value = self.stack.pop()
             if value > 0:
-                self.stack.append(math.log(value))
+                self.add_stack(math.log(value))
             else:
                 print("Number out of domain for logarithm")
                 self.stack.append(value)
 
     def and_(self):
         """Take 2 numbers from the stack, apply a bitwise "and" and put the result in the stack"""
         if self.check_stack(2, "and"):
             value1 = self.stack.pop()
             value2 = self.stack.pop()
-            self.stack.append(value1 & value2)
+            if isinstance(value1, int) and isinstance(value2, int):
+                self.stack.append(value1 & value2)
+            else:
+                print("This operation requires 2 int")
+                self.stack.append(value2)
+                self.stack.append(value1)
 
     def or_(self):
         """Take 2 numbers from the stack, apply a bitwise "or" and put the result in the stack"""
         if self.check_stack(2, "or"):
             value1 = self.stack.pop()
             value2 = self.stack.pop()
-            self.stack.append(value1 | value2)
+            if isinstance(value1, int) and isinstance(value2, int):
+                self.stack.append(value1 | value2)
+            else:
+                print("This operation requires 2 int")
+                self.stack.append(value2)
+                self.stack.append(value1)
 
     def xor(self):
         """Take 2 numbers from the stack, apply a bitwise "xor" and put the result in the stack"""
         if self.check_stack(2, "xor"):
             value1 = self.stack.pop()
             value2 = self.stack.pop()
-            self.stack.append(value1 ^ value2)
+            if isinstance(value1, int) and isinstance(value2, int):
+                self.stack.append(value1 ^ value2)
+            else:
+                print("This operation requires 2 int")
+                self.stack.append(value2)
+                self.stack.append(value1)
 
     def shift_left(self):
         """Take 2 numbers from the stack, apply a left shift and put the result in the stack"""
         if self.check_stack(2, "<<"):
             value2 = self.stack.pop()
             value1 = self.stack.pop()
             if isinstance(value1, int) and isinstance(value2, int):
@@ -311,79 +357,122 @@
         if self.check_stack(1, "abs"):
             self.stack.append(abs(self.stack.pop()))
 
     def inv(self):
         """Inverse the last number of the stack"""
         if self.check_stack(1, "inv"):
             value = self.stack.pop()
-            self.stack.append(1 / value)
+            self.add_stack(1 / value)
 
     def neg(self):
         """Change the sign of the last number in the stack"""
         if self.check_stack(1, "neg"):
             value = self.stack.pop()
             if value < 0:
                 self.stack.append(abs(value))
             else:
                 self.stack.append(0 - value)
 
     def sin(self):
         """Replace the last number in the stack with the sine of itself (measured in radians)"""
         if self.check_stack(1, "sin"):
-            self.stack.append(math.sin(self.stack.pop()))
+            self.add_stack(math.sin(self.stack.pop()))
 
     def cos(self):
         """Replace the last number in the stack with the cosine of itself (measured in radians)"""
         if self.check_stack(1, "cos"):
-            self.stack.append(math.cos(self.stack.pop()))
+            self.add_stack(math.cos(self.stack.pop()))
 
     def tan(self):
         """Replace the last number in the stack with the tangent of itself (measured in radians)"""
         if self.check_stack(1, "tan"):
-            self.stack.append(math.tan(self.stack.pop()))
+            self.add_stack(math.tan(self.stack.pop()))
 
     def asin(self):
         """Replace the last number in the stack with the arc sine of itself (measured in radians)"""
         if self.check_stack(1, "asin"):
             value = self.stack.pop()
             if value < -1 or value > 1:
                 print("Number out of domain for asin")
                 self.stack.append(value)
             else:
-                self.stack.append(math.asin(value))
+                self.add_stack(math.asin(value))
 
     def acos(self):
         """Replace the last number in the stack with the arc cosine of itself
         (measured in radians)"""
         if self.check_stack(1, "acos"):
             value = self.stack.pop()
             if value < -1 or value > 1:
                 print("Number out of domain for acos")
                 self.stack.append(value)
             else:
-                self.stack.append(math.acos(value))
+                self.add_stack(math.acos(value))
 
     def atan(self):
         """Replace the last number in the stack with the arc tangent of itself
         (measured in radians)"""
         if self.check_stack(1, "atan"):
             value = self.stack.pop()
-            self.stack.append(math.atan(value))
+            self.add_stack(math.atan(value))
+
+    def atan2(self):
+        """Take 2 numbers from the stack, apply a atan2 function and put the result in the stack"""
+        if self.check_stack(2, "atan2"):
+            x_val = self.stack.pop()
+            y_val = self.stack.pop()
+            self.add_stack(math.atan2(y_val, x_val))
+
+    def sinh(self):
+        """Replace the last number in the stack with the hyperbolic sine of itself"""
+        if self.check_stack(1, "sinh"):
+            value = self.stack.pop()
+            self.add_stack(math.sinh(value))
+
+    def cosh(self):
+        """Replace the last number in the stack with the hyperbolic cosine of itself"""
+        if self.check_stack(1, "cosh"):
+            value = self.stack.pop()
+            self.add_stack(math.cosh(value))
+
+    def tanh(self):
+        """Replace the last number in the stack with the hyperbolic tangent of itself"""
+        if self.check_stack(1, "tanh"):
+            value = self.stack.pop()
+            self.add_stack(math.tanh(value))
+
+    def asinh(self):
+        """Replace the last number in the stack with the asinh of itself"""
+        if self.check_stack(1, "asinh"):
+            value = self.stack.pop()
+            self.add_stack(math.asinh(value))
+
+    def acosh(self):
+        """Replace the last number in the stack with the acosh of itself"""
+        if self.check_stack(1, "acosh"):
+            value = self.stack.pop()
+            self.add_stack(math.acosh(value))
+
+    def atanh(self):
+        """Replace the last number in the stack with the atanh of itself"""
+        if self.check_stack(1, "atanh"):
+            value = self.stack.pop()
+            self.add_stack(math.atanh(value))
 
     def to_radian(self):
         """Convert the last number from degree to radian"""
         if self.check_stack(1, "torad"):
             value = self.stack.pop()
-            self.stack.append(value / 180 * math.pi)
+            self.add_stack(value / 180 * math.pi)
 
     def to_degree(self):
         """Convert the last number from radian to degree"""
         if self.check_stack(1, "todeg"):
             value = self.stack.pop()
-            self.stack.append(value * 180 / math.pi)
+            self.add_stack(value * 180 / math.pi)
 
     def switch(self):
         """Switch the last 2 numbers of the stack"""
         if self.check_stack(2, "switch"):
             value1 = self.stack.pop()
             value2 = self.stack.pop()
             self.stack.append(value1)
@@ -412,15 +501,15 @@
         self.stack.append(math.e)
 
     def sum(self):
         """Take all the number of the stack and add the sum"""
         if self.check_stack(1, "sum"):
             total = sum(self.stack)
             self.stack.clear()
-            self.stack.append(total)
+            self.add_stack(total)
 
     def factorial(self):
         """Replace the last number in the stack with its factorial"""
         if self.check_stack(1, "fact"):
             value = self.stack.pop()
             if value < 0:
                 print("Impossible to compute factorial for negative number")
@@ -439,63 +528,61 @@
 
     def average(self):
         """Take all the number of the stack and add the average"""
         if self.check_stack(1, "ave"):
             size = len(self.stack)
             total = sum(self.stack)
             self.stack.clear()
-            self.stack.append(total / size)
+
+            self.add_stack(total / size)
 
     def print_dec(self):
         """Print the last number of the stack and remove it"""
         if self.check_stack(1, "dec"):
-            print("{}".format(self.stack.pop()))
+            val = self.stack.pop()
+            self.last = val
+            print("{}".format(val))
 
     def print_hex(self):
         """Print in hexadecimal format the last number of the stack and remove it"""
         if self.check_stack(1, "hex"):
             i = self.stack.pop()
+            self.last = i
             if isinstance(i, int):
                 print("0x{:X}".format(i))
-            elif i.is_integer():
-                i = int(i)
-                print("0x{:X}".format(i))
             else:
                 print(float.hex(i))
 
     def print_bin(self):
         """Print in binary format the last number of the stack and remove it"""
         if self.check_stack(1, "bin"):
             i = self.stack.pop()
             if isinstance(i, int):
                 print("0b{:b}".format(i))
-            elif i.is_integer():
-                i = int(i)
-                print("0b{:b}".format(i))
+                self.last = i
             else:
                 self.stack.append(i)
                 print("Impossible to print a float in binary")
 
     def print_oct(self):
         """Print in octal format the last number of the stack and remove it"""
         if self.check_stack(1, "oct"):
             i = self.stack.pop()
             if isinstance(i, int):
                 print("0o{:o}".format(i))
-            elif i.is_integer():
-                i = int(i)
-                print("0o{:o}".format(i))
+                self.last = i
             else:
                 self.stack.append(i)
                 print("Impossible to print a float in octal")
 
     def ratio(self):
         """Print in integer ratio format the last number of the stack and remove it"""
         if self.check_stack(1, "ratio"):
             value = self.stack.pop()
+            self.last = value
             if isinstance(value, float):
                 print(Fraction(value).limit_denominator())
             else:
                 print("{}/1".format(value))
 
     def print_stack(self):
         """Print the stack"""
@@ -505,14 +592,23 @@
             print("{}".format(self.stack[-1]))
         else:
             print("Stack is empty")
 
     def clear_stack(self):
         """Empty the stack"""
         self.stack = []
+        self.last = None
+
+    def back(self):
+        """Put back on the stack the last value that was printed"""
+        if self.last is not None:
+            self.stack.append(self.last)
+            self.last = None
+        else:
+            print("No value was remove from the stack")
 
     def help(self):
         """Print help; Same as pol --list"""
         doc = ""
         for command, method in self.operation.items():
             doc += "`{}` : {}\n".format(command, method.__doc__)
```

### Comparing `rpn_calc-0.2.2/rpn_calc.egg-info/PKG-INFO` & `rpn_calc-0.2.3/rpn_calc.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,208 +1,225 @@
 Metadata-Version: 2.1
 Name: rpn-calc
-Version: 0.2.2
+Version: 0.2.3
 Summary: RPN calculator
 Home-page: https://github.com/Allain18/pol
 Author: Alain Girard
 Author-email: alaingirardvd@gmail.com
 License: MIT License
-Description: # pol
-        [![Build Status](https://travis-ci.com/Allain18/pol.svg?branch=master)](https://travis-ci.com/Allain18/pol)
-        
-        Command line calculator using [reverse polish notation](https://en.wikipedia.org/wiki/Reverse_Polish_notation)
-        
-        Decimal, hexadecimal, binary and octal number are supported
-        
-        ## Usage
-        As a command line tool: __pol__
-        
-        ```
-        ~$ pol
-        Reverse polish notation calculator
-        >5 10 * dec
-        50
-        >0xA 0x6 + hex
-        0x10
-        >q //quit the program
-        ~$
-        ```
-        
-        Instructions are [below](#list-of-commands)
-        
-        pol can also be use as a module
-        ```python 
-        import rpn_calc
-        cal = rpn_calculator.Calculator()
-        cal.evaluate("1 2 + dec")
-        # print 3
-        ```
-        
-        ## Install
-        pol can be install from pip
-        ```
-        pip install rpn-calc
-        ```
-        If you want to install from a source distribution, extract the tarball and run the following command
-        ```
-        python setup.py install
-        ```
-        
-        ## Documentation
-        This README is the Documentation
-        
-        ## [Repo](https://github.com/Allain18/pol)
-        The code is on github
-        
-        ## Config file
-        You can write your own command
-        
-        By default commands from file ~/pol.yml (if exists) are add to the calculator
-        
-        You can add other files with the flag -f/--file
-        
-        Config files are written in YAML
-        
-        ### Currently supported parameters
-        - shortcut: shortcut to commands (see example below)
-        - rounding: parameter used to round number (default: 0)
-        
-        ### Example of a valid config file
-        ```YAML
-        shortcut:
-         - double = 2 * # double the last value of the stack
-         - 10* = 10 switch ** # same as 10 {x} **
-        rounding: 3
-        ```
-        Command must be on the format {name_of_command = command}
-        
-        ## Options
-        ```
-        usage: pol [-h] [-v] [-l] [--ignore-local-config] [-f FILE [FILE ...]]
-        
-        A RPN calculator written in python
-        Support decimal, hexadecimal, binary and octal
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -v, --version         show the version number and exit
-          -l, --list            list all commands available and exit
-          --ignore-local-config
-                                don't add commands from ~/.pol
-          -f FILE [FILE ...], --file FILE [FILE ...]
-                                file with customs commands
-        ```
-        ## List of commands
-        `+` : Take 2 numbers from the stack, add them and put the result in the stack
-        
-        `-` : Take 2 numbers from the stack, substracte them and put the result in the stack
-        
-        `*` : Take 2 numbers from the stack, mul them and put the result in the stack
-        
-        `/` : Take 2 numbers from the stack, divise them and put the result in the stack
-        
-        `//` : Take 2 numbers from the stack, divise them and put the integer result in the stack
-        
-        `%` : Take 2 numbers from the stack, divise them and put the remainder in the stack
-        
-        `**` : Take 2 numbers from the stack, apply power and put the result in the stack
-        
-        `sqrt` : Replace the last number in the stack with the square root of itself
-        
-        `exp` : Apply e**x to the last number of the stack
-        
-        `log10` : Apply log10 to the last number of the stack
-        
-        `log2` : Apply log2 to the last number of the stack
-        
-        `ln` : Apply natural logarithm to the last number of the stack
-        
-        `and` : Take 2 numbers from the stack, apply a bitwise "and" and put the result in the stack
-        
-        `or` : Take 2 numbers from the stack, apply a bitwise "or" and put the result in the stack
-        
-        `xor` : Take 2 numbers from the stack, apply a bitwise "xor" and put the result in the stack
-        
-        `<<` : Take 2 numbers from the stack, apply a left shift and put the result in the stack
-        
-        `>>` : Take 2 numbers from the stack, apply a right shift and put the result in the stack
-        
-        `abs` : Make absolute the last value of the stack
-        
-        `inv` : Inverse the last number of the stack
-        
-        `neg` : Change the sign of the last number in the stack
-        
-        `sin` : Replace the last number in the stack with the sine of itself (measured in radians)
-        
-        `cos` : Replace the last number in the stack with the cosine of itself (measured in radians)
-        
-        `tan` : Replace the last number in the stack with the tangent of itself (measured in radians)
-        
-        `asin` : Replace the last number in the stack with the arc sine of itself (measured in radians)
-        
-        `acos` : Replace the last number in the stack with the arc cosine of itself (measured in radians)
-        
-        `atan` : Replace the last number in the stack with the arc tangent of itself (measured in radians)
-        
-        `torad` : Convert the last number from degree to radian
-        
-        `todeg` : Convert the last number from radian to degree
-        
-        `switch` : Switch the last 2 numbers of the stack
-        
-        `del` : Delete the last number in the stack
-        
-        `copy` : Copy the last number of the stack and add it to the stack
-        
-        `pi` : Add pi to the stack
-        
-        `tau` : Add tau to the stack
-        
-        `e` : Add e to the stack
-        
-        `sum` : Take all the number of the stack and add the sum
-        
-        `fact` : Replace the last number in the stack with its factorial
-        
-        `round` : Round the last number in the stack
-        
-        `ave` : Take all the number of the stack and add the average
-        
-        `dec` : Print the last number of the stack and remove it
-        
-        `hex` : Print in hexadecimal format the last number of the stack and remove it
-        
-        `bin` : Print in binary format the last number of the stack and remove it
-        
-        `oct` : Print in octal format the last number of the stack and remove it
-        
-        `ratio` : Print in integer ratio format the last number of the stack and remove it
-        
-        `s` : Print the stack
-        
-        `clear` : Empty the stack
-        
-        `help` : Print help; Same as pol --list
-        
-        `q` : Quit the program
-        
-        ## License
-        
-        MIT
-        
 Keywords: rpn,calculator,reverse polish notation
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pol
+[![Build Status](https://travis-ci.com/Allain18/pol.svg?branch=master)](https://travis-ci.com/Allain18/pol)
+
+Command line calculator using [reverse polish notation](https://en.wikipedia.org/wiki/Reverse_Polish_notation)
+
+Decimal, hexadecimal, binary and octal number are supported
+
+## Usage
+As a command line tool: __pol__
+
+```
+~$ pol
+Reverse polish notation calculator
+>5 10 * dec
+50
+>0xA 0x6 + hex
+0x10
+>q //quit the program
+~$
+```
+
+Instructions are [below](#list-of-commands)
+
+pol can also be use as a module
+```python 
+import rpn_calc
+cal = rpn_calculator.Calculator()
+cal.evaluate("1 2 + dec")
+# print 3
+```
+
+## Install
+pol can be install from pip
+```
+pip install rpn-calc
+```
+If you want to install from a source distribution, extract the tarball and run the following command
+```
+python setup.py install
+```
+
+## Documentation
+This README is the Documentation
+
+## [Repo](https://github.com/Allain18/pol)
+The code is on github
+
+## Config file
+You can write your own command
+
+By default commands from file ~/pol.yml (if exists) are add to the calculator
+
+You can add other files with the flag -f/--file
+
+Config files are written in YAML
+
+### Currently supported parameters
+- shortcut: shortcut to commands (see example below)
+- rounding: parameter used to round number (default: 0)
+
+### Example of a valid config file
+```YAML
+shortcut:
+ - double = 2 * # double the last value of the stack
+ - 10* = 10 switch ** # same as 10 {x} **
+rounding: 3
+```
+Command must be on the format {name_of_command = command}
+
+## Options
+```
+usage: pol [-h] [-v] [-l] [--ignore-local-config] [-f FILE [FILE ...]]
+
+A RPN calculator written in python
+Support decimal, hexadecimal, binary and octal
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -v, --version         show the version number and exit
+  -l, --list            list all commands available and exit
+  --ignore-local-config
+                        don't add commands from ~/.pol
+  -f FILE [FILE ...], --file FILE [FILE ...]
+                        file with customs commands
+```
+## List of commands
+`+` : Take 2 numbers from the stack, add them and put the result in the stack
+
+`-` : Take 2 numbers from the stack, substracte them and put the result in the stack
+
+`*` : Take 2 numbers from the stack, mul them and put the result in the stack
+
+`/` : Take 2 numbers from the stack, divise them and put the result in the stack
+
+`//` : Take 2 numbers from the stack, divise them and put the integer result in the stack
+
+`%` : Take 2 numbers from the stack, divise them and put the remainder in the stack
+
+`**` : Take 2 numbers from the stack, apply power and put the result in the stack
+
+`sqrt` : Replace the last number in the stack with the square root of itself
+
+`exp` : Apply e**x to the last number of the stack
+
+`log10` : Apply log10 to the last number of the stack
+
+`log2` : Apply log2 to the last number of the stack
+
+`ln` : Apply natural logarithm to the last number of the stack
+
+`and` : Take 2 numbers from the stack, apply a bitwise "and" and put the result in the stack
+
+`or` : Take 2 numbers from the stack, apply a bitwise "or" and put the result in the stack
+
+`xor` : Take 2 numbers from the stack, apply a bitwise "xor" and put the result in the stack
+
+`<<` : Take 2 numbers from the stack, apply a left shift and put the result in the stack
+
+`>>` : Take 2 numbers from the stack, apply a right shift and put the result in the stack
+
+`abs` : Make absolute the last value of the stack
+
+`inv` : Inverse the last number of the stack
+
+`neg` : Change the sign of the last number in the stack
+
+`sin` : Replace the last number in the stack with the sine of itself (measured in radians)
+
+`cos` : Replace the last number in the stack with the cosine of itself (measured in radians)
+
+`tan` : Replace the last number in the stack with the tangent of itself (measured in radians)
+
+`asin` : Replace the last number in the stack with the arc sine of itself (measured in radians)
+
+`acos` : Replace the last number in the stack with the arc cosine of itself (measured in radians)
+
+`atan` : Replace the last number in the stack with the arc tangent of itself (measured in radians)
+
+`atan2` : Take 2 numbers from the stack, apply a atan2 function and put the result in the stack
+
+`sinh` : Replace the last number in the stack with the hyperbolic sine of itself
+
+`cosh` : Replace the last number in the stack with the hyperbolic cosine of itself
+
+`tanh` : Replace the last number in the stack with the hyperbolic tangent of itself
+
+`asinh` : Replace the last number in the stack with the asinh of itself
+
+`acosh` : Replace the last number in the stack with the acosh of itself
+
+`atanh` : Replace the last number in the stack with the atanh of itself
+
+`torad` : Convert the last number from degree to radian
+
+`todeg` : Convert the last number from radian to degree
+
+`switch` : Switch the last 2 numbers of the stack
+
+`del` : Delete the last number in the stack
+
+`copy` : Copy the last number of the stack and add it to the stack
+
+`pi` : Add pi to the stack
+
+`tau` : Add tau to the stack
+
+`e` : Add e to the stack
+
+`sum` : Take all the number of the stack and add the sum
+
+`fact` : Replace the last number in the stack with its factorial
+
+`round` : Round the last number in the stack
+
+`ave` : Take all the number of the stack and add the average
+
+`dec` : Print the last number of the stack and remove it
+
+`hex` : Print in hexadecimal format the last number of the stack and remove it
+
+`bin` : Print in binary format the last number of the stack and remove it
+
+`oct` : Print in octal format the last number of the stack and remove it
+
+`ratio` : Print in integer ratio format the last number of the stack and remove it
+
+`s` : Print the stack
+
+`clear` : Empty the stack
+
+`back` : Put back on the stack the last value that was printed
+
+`help` : Print help; Same as pol --list
+
+`q` : Quit the program
+
+## License
+
+MIT
```

### Comparing `rpn_calc-0.2.2/setup.py` & `rpn_calc-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Environment :: Console",
         "Operating System :: OS Independent"
     ],
     python_requires=">=3.6",
     test_suite="test",
     packages=find_packages(exclude=["test"]),
```

### Comparing `rpn_calc-0.2.2/test/test_calculator.py` & `rpn_calc-0.2.3/test/test_calculator.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
     def test_get_number(self):
         """Test get_number function"""
         self.assertEqual(get_number("10"), 10)
         self.assertEqual(get_number("0b10"), 2)
         self.assertEqual(get_number("0x10"), 16)
         self.assertEqual(get_number("0o10"), 8)
+        self.assertEqual(get_number("10.0"), 10)
         self.assertEqual(get_number("0.25"), 0.25)
         self.assertEqual(get_number("0xaaa"), 2730)
         self.assertEqual(get_number("alc"), "alc")
 
     def test_loop(self):
         """Test loop method"""
         stdin = StringIO("2 8 * q\n")
@@ -59,14 +60,25 @@
         self.cal.stack.append(55)
         self.assertEqual(self.cal.check_stack(1, "test"), True)
         self.assertEqual(self.cal.check_stack(5, "test"), False)
 
         self.assertEqual(self.stdout.getvalue(),
                          "Not enough numbers in the stack for test command\n")
 
+    def test_add_stack(self):
+        """Test add stack method"""
+        self.cal.add_stack(5)
+        self.assertIsInstance(self.cal.stack.pop(), int)
+
+        self.cal.add_stack(10.5)
+        self.assertIsInstance(self.cal.stack.pop(), float)
+
+        self.cal.add_stack(5.0)
+        self.assertIsInstance(self.cal.stack.pop(), int)
+
     def test_add(self):
         """Test add method"""
         self.cal.stack.append(5)
         self.cal.stack.append(10)
         self.cal.add()
         self.assertEqual(self.cal.stack.pop(), 15)
 
@@ -169,14 +181,29 @@
         self.assertEqual(self.cal.stack.pop(), 5**10)
 
         self.cal.stack.append(5)
         self.cal.stack.append(0)
         self.cal.pow()
         self.assertEqual(self.cal.stack.pop(), 1)
 
+        self.cal.stack.append(0)
+        self.cal.stack.append(0)
+        self.cal.pow()
+        self.assertEqual(self.cal.stack.pop(), 1)
+
+        self.cal.stack.append(0)
+        self.cal.stack.append(-1)
+        self.cal.pow()
+        self.assertEqual(self.cal.stack.pop(), -1)
+
+        self.cal.stack.append(1)
+        self.cal.stack.append(-1)
+        self.cal.pow()
+        self.assertEqual(self.cal.stack.pop(), 1)
+
     def test_sqrt(self):
         """Test sqrt method"""
         self.cal.stack.append(16)
         self.cal.sqrt()
         self.cal.stack.append(0)
         self.cal.sqrt()
         self.cal.stack.append(-5)
@@ -235,38 +262,59 @@
         self.assertEqual(self.cal.stack.pop(), 0)
 
         self.cal.stack.append(7)
         self.cal.stack.append(15)
         self.cal.and_()
         self.assertEqual(self.cal.stack.pop(), 7)
 
+        self.cal.stack.append(7)
+        self.cal.stack.append(15.5)
+        self.cal.and_()
+        self.assertEqual(self.cal.stack.pop(), 15.5)
+        self.assertEqual(self.stdout.getvalue(),
+                         "This operation requires 2 int\n")
+
     def test_or(self):
         """Test _or method"""
         self.cal.stack.append(5)
         self.cal.stack.append(10)
         self.cal.or_()
         self.assertEqual(self.cal.stack.pop(), 15)
 
         self.cal.stack.append(7)
         self.cal.stack.append(15)
         self.cal.or_()
         self.assertEqual(self.cal.stack.pop(), 15)
 
+        self.cal.stack.append(7)
+        self.cal.stack.append(15.5)
+        self.cal.and_()
+        self.assertEqual(self.cal.stack.pop(), 15.5)
+        self.assertEqual(self.stdout.getvalue(),
+                         "This operation requires 2 int\n")
+
     def test_xor(self):
         """Test xor method"""
         self.cal.stack.append(5)
         self.cal.stack.append(10)
         self.cal.xor()
         self.assertEqual(self.cal.stack.pop(), 15)
 
         self.cal.stack.append(7)
         self.cal.stack.append(15)
         self.cal.xor()
         self.assertEqual(self.cal.stack.pop(), 8)
 
+        self.cal.stack.append(7)
+        self.cal.stack.append(15.5)
+        self.cal.and_()
+        self.assertEqual(self.cal.stack.pop(), 15.5)
+        self.assertEqual(self.stdout.getvalue(),
+                         "This operation requires 2 int\n")
+
     def test_shift_left(self):
         """Test shift_left method"""
         self.cal.stack.append(55)
         self.cal.stack.append(2)
         self.cal.shift_left()
         self.assertEqual(self.cal.stack.pop(), 220)
 
@@ -394,14 +442,86 @@
         self.cal.atan()
         self.assertAlmostEqual(self.cal.stack.pop(), math.pi/4)
 
         self.cal.stack.append(-1)
         self.cal.atan()
         self.assertAlmostEqual(self.cal.stack.pop(), - math.pi/4)
 
+    def test_atan2(self):
+        """Test atan2 method"""
+        self.cal.stack.append(0)
+        self.cal.stack.append(1)
+        self.cal.atan2()
+        self.assertAlmostEqual(self.cal.stack.pop(), 0)
+
+        self.cal.stack.append(-1)
+        self.cal.stack.append(-1)
+        self.cal.atan2()
+        self.assertAlmostEqual(self.cal.stack.pop(), -math.pi*3/4)
+
+    def test_sinh(self):
+        """Test sinh method"""
+        self.cal.stack.append(1)
+        self.cal.sinh()
+        self.assertEqual(self.cal.stack.pop(), (math.e**2 - 1)/(2 * math.e))
+
+        self.cal.stack.append(0)
+        self.cal.sinh()
+        self.assertEqual(self.cal.stack.pop(), 0)
+
+    def test_cosh(self):
+        """Test cosh method"""
+        self.cal.stack.append(1)
+        self.cal.cosh()
+        self.assertAlmostEqual(self.cal.stack.pop(), (math.e**2 + 1)/(2 * math.e))
+
+        self.cal.stack.append(0)
+        self.cal.cosh()
+        self.assertEqual(self.cal.stack.pop(), 1)
+
+    def test_tanh(self):
+        """Test tanh method"""
+        self.cal.stack.append(1)
+        self.cal.tanh()
+        self.assertAlmostEqual(self.cal.stack.pop(), (math.e**2 - 1)/(math.e**2 + 1))
+
+        self.cal.stack.append(0)
+        self.cal.tanh()
+        self.assertEqual(self.cal.stack.pop(), 0)
+
+    def test_asinh(self):
+        """Test asinh method"""
+        self.cal.stack.append((math.e**2 - 1)/(2 * math.e))
+        self.cal.asinh()
+        self.assertAlmostEqual(self.cal.stack.pop(), 1)
+
+        self.cal.stack.append(0)
+        self.cal.asinh()
+        self.assertEqual(self.cal.stack.pop(), 0)
+
+    def test_acosh(self):
+        """Test acosh method"""
+        self.cal.stack.append((math.e**2 + 1)/(2 * math.e))
+        self.cal.acosh()
+        self.assertAlmostEqual(self.cal.stack.pop(), 1)
+
+        self.cal.stack.append(1)
+        self.cal.acosh()
+        self.assertEqual(self.cal.stack.pop(), 0)
+
+    def test_atanh(self):
+        """Test atanh method"""
+        self.cal.stack.append((math.e**2 - 1)/(math.e**2 + 1))
+        self.cal.atanh()
+        self.assertAlmostEqual(self.cal.stack.pop(), 1)
+
+        self.cal.stack.append(0)
+        self.cal.atanh()
+        self.assertEqual(self.cal.stack.pop(), 0)
+
     def test_toreg(self):
         """Test to_radian method"""
         self.cal.stack.append(180)
         self.cal.to_radian()
 
         self.cal.stack.append(-90)
         self.cal.to_radian()
@@ -511,55 +631,61 @@
         self.cal.average()
         self.assertEqual(self.cal.stack.pop(), 5.3)
 
         self.cal.stack.extend([5.3, -3566.33])
         self.cal.average()
         self.assertAlmostEqual(self.cal.stack.pop(), -1780.515)
 
+        self.cal.stack.extend([2, 4])
+        self.cal.average()
+        val = self.cal.stack.pop()
+        self.assertEqual(val, 3)
+        self.assertIsInstance(val, int)
+
     def test_print_dec(self):
         """Test print method"""
         self.cal.stack.append(5)
         self.cal.stack.append(10.2)
 
         self.cal.print_dec()
         self.cal.print_dec()
 
         self.assertEqual(self.stdout.getvalue(), "10.2\n5\n")
 
     def test_print_hex(self):
         """Test print_hex method"""
         self.cal.stack.append(500)
-        self.cal.stack.append(10.0)
+        self.cal.stack.append(10)
         self.cal.stack.append(12.2)
 
         self.cal.print_hex()
         self.cal.print_hex()
         self.cal.print_hex()
 
         self.assertEqual(self.stdout.getvalue(),
                          "0x1.8666666666666p+3\n0xA\n0x1F4\n")
 
     def test_print_bin(self):
         """Test print_bin method"""
         self.cal.stack.append(500)
-        self.cal.stack.append(10.0)
+        self.cal.stack.append(10)
         self.cal.stack.append(2.5)
 
         self.cal.print_bin()
         self.cal.stack.pop()
         self.cal.print_bin()
         self.cal.print_bin()
 
         self.assertEqual(self.stdout.getvalue(),
                          "Impossible to print a float in binary\n0b1010\n0b111110100\n")
 
     def test_print_oct(self):
         """Test print_oct method"""
         self.cal.stack.append(500)
-        self.cal.stack.append(10.0)
+        self.cal.stack.append(10)
         self.cal.stack.append(2.5)
 
         self.cal.print_oct()
         self.cal.stack.pop()
         self.cal.print_oct()
         self.cal.print_oct()
 
@@ -582,27 +708,35 @@
         self.cal.ratio()
         self.cal.ratio()
 
         self.assertEqual(self.stdout.getvalue(),
                          "5/3\n3/4\n-41/4\n21/2\n-10/1\n10/1\n")
 
     def test_print_stack(self):
-        """Test print_stack"""
+        """Test print_stack method"""
         self.cal.stack.append(500)
         self.cal.stack.append(10.0)
         self.cal.stack.append(123.123)
 
         self.cal.print_stack()
 
         self.cal.clear_stack()
         self.cal.print_stack()
 
         self.assertEqual(self.stdout.getvalue(),
                          "500, 10.0, 123.123\nStack is empty\n")
 
+    def test_back(self):
+        """Test back method"""
+        self.cal.stack.append(500)
+        self.cal.print_dec()
+        self.cal.back()
+        self.assertEqual(self.stdout.getvalue(), "500\n")
+        self.assertEqual(self.cal.stack.pop(), 500)
+
     def test_evaluate(self):
         """Test evaluate method"""
         self.cal.evaluate("5 10 * dec")
         self.assertEqual(self.stdout.getvalue(), "50\n")
 
 
 if __name__ == "__main__":
```

