# Comparing `tmp/evalidate-1.0.3.tar.gz` & `tmp/evalidate-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evalidate-1.0.3.tar", last modified: Wed Jun  7 10:57:35 2023, max compression
+gzip compressed data, was "evalidate-1.1.0.tar", last modified: Thu Jun 15 17:26:21 2023, max compression
```

## Comparing `evalidate-1.0.3.tar` & `evalidate-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-07 10:57:35.030697 evalidate-1.0.3/
--rw-r--r--   0 xenon     (1000) xenon     (1000)    16301 2023-06-07 10:57:35.030697 evalidate-1.0.3/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)    12915 2023-06-07 10:56:21.000000 evalidate-1.0.3/README.md
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-07 10:57:35.030697 evalidate-1.0.3/evalidate/
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     5480 2023-05-30 08:23:52.000000 evalidate-1.0.3/evalidate/__init__.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)     2376 2023-05-30 08:23:52.000000 evalidate-1.0.3/evalidate/security.py
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-07 10:57:35.030697 evalidate-1.0.3/evalidate.egg-info/
--rw-r--r--   0 xenon     (1000) xenon     (1000)    16301 2023-06-07 10:57:34.000000 evalidate-1.0.3/evalidate.egg-info/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)      226 2023-06-07 10:57:34.000000 evalidate-1.0.3/evalidate.egg-info/SOURCES.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-06-07 10:57:34.000000 evalidate-1.0.3/evalidate.egg-info/dependency_links.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2021-09-12 11:08:09.000000 evalidate-1.0.3/evalidate.egg-info/not-zip-safe
--rw-r--r--   0 xenon     (1000) xenon     (1000)       10 2023-06-07 10:57:34.000000 evalidate-1.0.3/evalidate.egg-info/top_level.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-06-07 10:57:35.030697 evalidate-1.0.3/setup.cfg
--rw-r--r--   0 xenon     (1000) xenon     (1000)      876 2023-06-07 10:56:28.000000 evalidate-1.0.3/setup.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-15 17:26:21.318591 evalidate-1.1.0/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    11506 2023-06-15 17:26:21.318591 evalidate-1.1.0/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     8896 2023-06-15 17:25:08.000000 evalidate-1.1.0/README.md
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-15 17:26:21.318591 evalidate-1.1.0/evalidate/
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     7363 2023-06-15 16:52:05.000000 evalidate-1.1.0/evalidate/__init__.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     2406 2023-06-15 17:02:24.000000 evalidate-1.1.0/evalidate/security.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-15 17:26:21.318591 evalidate-1.1.0/evalidate.egg-info/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    11506 2023-06-15 17:26:21.000000 evalidate-1.1.0/evalidate.egg-info/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      226 2023-06-15 17:26:21.000000 evalidate-1.1.0/evalidate.egg-info/SOURCES.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-06-15 17:26:21.000000 evalidate-1.1.0/evalidate.egg-info/dependency_links.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2021-09-12 11:08:09.000000 evalidate-1.1.0/evalidate.egg-info/not-zip-safe
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       10 2023-06-15 17:26:21.000000 evalidate-1.1.0/evalidate.egg-info/top_level.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-06-15 17:26:21.318591 evalidate-1.1.0/setup.cfg
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     1077 2023-06-15 17:03:02.000000 evalidate-1.1.0/setup.py
```

### Comparing `evalidate-1.0.3/README.md` & `evalidate-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,350 +1,270 @@
-﻿# Evalidate
-Evalidate is simple python module for safe eval()'uating user-supplied (possible malicious) logical expressions in python syntax.
-
-## Purpose
-Originally it's developed for filtering complex data structures e.g. 
-
-Find cheap smartphones available for sale:
-```python
-category="smartphones" and price<300 and stock>0
-```
-
-But also, it can be used for other expressions, e.g. arithmetical, like
-```python
-a+b-100
-```
-
-Evalidate tries to be both secure and fast (when properly used).
-
-## Install
-
-```shell
-pip3 install evalidate
-```
-    
-## Security
-
-Built-in python features such as compile() or eval() are quite powerful to run any kind of user-supplied code, but could be insecure if used code is malicious like `os.system("rm -rf /")`. Evalidate works on whitelist principle, allowing code only if it consist only of safe operations (based on authors views about what is safe and what is not, your mileage may vary - but you can supply your list of safe operations)
-
-
-## TL;DR. Just give me safe eval!
-```python       
-from evalidate import safeeval, EvalException
-
-src="a+b" # source code
-# src="__import__('os').system('clear')"
-c={'a': 1, 'b': 2} # context, variables which will be available for code
-
-try:
-    result = safeeval(src,c)
-    print(result)
-except EvalException as e:
-    print("ERR:", e)
-```
-
-Gives output:
-
-    3
-
-In case of dangerous code:
-```python
-src="__import__('os').system('clear')"
-```    
-    
-output will be: `ERR: Operation type Call is not allowed`
-
-
-## Exceptions
-Evalidate throws exceptions `CompilationException`, `ValidationException`, `ExecutionException`. All of them
-inherit from base exception class `EvalException`.
-
-## Configure validation
-Evalidate is very flexible, depending on parameters, same code can either pass validation or raise exception.
-
-### Safenodes and addnodes
-Evalidate has built-in set of python operations, which are considered 'safe' (from author point of view). Code is considered valid only if all of it's operations are in this list. You can override this list by adding argument `safenodes` like:
-```python
-result = evalidate.safeeval(src, context, safenodes=['Expression','BinOp','Num','Add'])
-```
-this will be enough for `1+1` expression (in src argument), but not for `1-1`. If you will try '1-1', it will report error: `ERROR: Validation error: Operaton type Sub is not allowed`
-
-This way you can start from scratch and allow only required operations. As an alternative, you can use built-in list of allowed operations and extend it if needed, using `addnodes` argument.
-
-For example, "1*1" will give error:
-
-  ERROR: Validation error: Operaton type Mult is not allowed
-
-
-But it will work with addnodes:
-```python
-result = evalidate.safeeval(src,c, addnodes=['Mult'])
-```    
-Please note, using 'Mult' operation isn't very secure, because for strings it can lead to Out-of-memory:
-```python
-src='"a"*1000000*1000000*1000000*1000000'
-```    
-and will raise runtime exception: `ERROR: Runtime error (OverflowError): repeated string is too long`
-
-### Allowing function calls
-Evalidate does not allow any function calls by default:
-```python
->>> from evalidate import safeeval, EvalException
->>> try:
-...   safeeval('int(1)')
-... except EvalException as e:
-...   print(e)
-... 
-Operation type Call is not allowed
-```
-
-To enable int() function, need to allow 'Call' node and  add this function to list of allowed function:
-```python
->>> evalidate.safeeval('int(1)', addnodes=['Call'], funcs=['int'])
-1
-```
-Attempt to call other functions will fail (because it's not in funcs list):
-```python
-evalidate.safeeval('1+round(2)', addnodes=['Call'], funcs=['int'])
-```
-This will throw `ValidationException`.
-
-Attributes calls (`"aaa".startswith("a")`) could be allowed (with proper `addnodes` and `attrs`) but
-other indirect function calls (like: `__builtins__['eval']("print(1)")`) are not allowed,
-
-
-### Accessing attributes (attrs parameter); data as classes
-
-If data represented as object with attributes (not as dictionary) we have to add 'Attribute' to safe nodes. Increase salary for person for 200, and additionaly 25 for each year (s)he works in company.
-
-```python
-from evalidate import safeeval, EvalException
-                        
-class Person:
-    pass
-                        
-p = Person()
-p.salary=1000
-p.age=5
-                        
-data = {'p':p}
-src = 'p.salary+200+p.age*25'
-try:                        
-    result = safeeval(src,data,addnodes=['Attribute','Mult'], attrs=['salary', 'age'])                        
-    print("result", result)
-except EvalException as e:
-    print("ERR:",e)
-```
-
-### Calling attributes
-This code will not work:
-~~~python
-safeeval('"abc".startswith("a")')
-~~~
-Because: `evalidate.ValidationException: Operation type Call is not allowed`
-
-To make it working:
-~~~python
-print(safeeval('"abc".startswith("a")', addnodes=['Call', 'Attribute'], attrs=['startswith']))
-~~~
-
-## Functions
-
-`safeeval()` is simplest possible replacement to `eval()`. It is good to evaluate something once or few times, where speed is not an issue. If you need to eval same code 2nd time, it will take same 'long' time to parse/validate code. 
-
-`evalidate()` is just little more complex, but returns validated safe python AST node, which can be compiled to python bytecode, and executed at full speed. (And this code is safe after evalidate)
-
-`security.test_security()` checks configuration(nodes, funcs, attrs) against set of attacks.
-
-
-### evalidate.safeeval()
-
-```python
-result = safeeval(expression, context={}, safenodes=None, addnodes=None, funcs=None, attrs=None)
-```
-
-`safeeval` is higher-level wrapper of evalidate(), which validates code and runs it (if validation is successful). Throws exception if compilation(parsing), validation or execution fails.
-
-`expression` - python expression like `salary+100` or `category="smartphones" and price<300 and stock>0`.
-
-`context` - dictionary of variables, available for evaluated code.
-
-`safenodes`, `addnodes`, `funcs` and `attrs` are same as in `evalidate()`
-
-returns result of evaluation of expression. 
-
-### evalidate.evalidate()     
-```python
-node = evalidate(expression, safenodes=None, addnodes=None, funcs=None, attrs=None)
-```
-`evalidate()` is main (and recommended to use) method, performs parsing of python expession, validates it, and returns python AST (Abstract Syntax Tree) structure, which can be later compiled and executed. Evalidate does not evaluates code, use `compile()` and `eval()` after `evalidate()`.
-
-
-```python            
-
->>> import evalidate
->>> node = evalidate.evalidate('1+2')
->>> code = compile(node,'<usercode>','eval')
->>> eval(code)
-3
-```    
-    
-- `expression` - python expression `salary+100` or `category="smartphones" and price<300 and stock>0`.
-- `safenodes` - list of allowed nodes. This will *override* built-in list of allowed nodes. e.g. `safenodes=['Expression','BinOp','Num','Add'])`
-- `addnodes` - list of allowed nodes. This will *extend* built-in lsit of allowed nodes. e.g. `addnodes=['Mult']`
-- `funcs` - list of allowed function calls. You need to add 'Call' to safe nodes. e.g. `funcs=['int']`
-- `attrs` - list of allowed attributes. You need to add 'Attribute' to attrs. e.g. `attrs=['salary']`.
-
-    
-evalidate() throws `CompilationException` if cannot parse source code and `ValidationException` if it doesn't like source code (if code has unsafe operations).
-    
-Even if evalidate is successful, this doesn't guarantees that code will run well, For example, code still can have `NameError` (if tries to access undefined variable) or `ZeroDivisionError`.
-
-evalidate uses [ast.parse()](https://docs.python.org/3/library/ast.html#ast.parse) and returns [AST node](https://docs.python.org/3/library/ast.html#node-classes).
-
->Warning
->
->It is possible to crash the Python interpreter with a sufficiently large/complex string due to stack depth limitations in Python’s AST compiler. 
-
-In my test, works well with 200 nested int(): `int(int(.... int(1)...))` but not with 201. Source code is 1000+ characters. But even if evalidate will get such code, it will just raise `CompilationException`.
-
-
-### evalidate.security.test_security()
-Evalidate is very flexible and it's possible to shoot yourself in foot if you will try hard. `test_security()` checks your configuration (addnodes/safenodes, funcs, attrs) against given list of possible attack code or against built-in list of attacks. `test_security()` returns True if everything is OK (all attacks raised ValidationException) or False if something passed.
-
-This code will never print (I hope).
-~~~python
-from evalidate.security import test_security
-
-test_security() or print("default rules are vulnerable!")
-~~~
-
-But this will fail because nodes/funcs leads to successful validation for attack (suppose you do not want anyone to call `int()`)
-~~~python
-from evalidate.security import test_security
-
-attacks = ['int(1)']
-
-test_security(attacks, addnodes=['Call'], funcs=['int'], verbose=True)
-~~~
-
-It will print:
-~~~
-Testing attack code:
-int(1)
-Problem! Attack passed validation without exception!
-Code:
-int(1)
-~~~
-
-
-
-
-## Example
-
-### Filtering by user-supplied condition ###
-
-This is code of `examples/products.py`. Expression is validated and compiled once and executed (as byte-code, very fast) many times, so filtering is both fast and secure.
-
-
-~~~python
-#!/usr/bin/env python3
-
-import requests
-from evalidate import evalidate, ValidationException, CompilationException
-import json
-import sys
-
-data = requests.get('https://dummyjson.com/products?limit=100').json()
-
-try:
-    src = sys.argv[1]
-except IndexError:
-    src = 'True'
-
-try:
-    node = evalidate(src)
-except (ValidationException, CompilationException) as e:
-    print(e)
-    sys.exit(1)
-
-
-code = compile(node, '<user filter>', 'eval')
-
-c=0
-for p in data['products']:
-    # print(p)
-    try:
-        r = eval(code, p.copy())
-        if r:
-            print(json.dumps(p, indent=2))
-            c+=1
-    except Exception as e:
-        print("Runtime exception:", e)
-print("# {} products matches".format(c))
-~~~
-
-~~~shell
-# print all 100 products
-./products.py
-
-# Only cheap products, 8 matches
-./products.py 'price<20'
-
-# smartphones (5)
-./products.py 'category=="smartphones"'
-
-# good smartphones
-./products.py 'category=="smartphones" and rating>4.5'
-
-# cheap smartphones
-./products.py 'category=="smartphones" and price<300'
-~~~
-                                       
-
-## Similar projects and benchmark
-
-[asteval](https://newville.github.io/asteval/)
-
-While asteval can compute much more complex code (define functions, use python math libraries) it has drawbacks:
-- asteval is much slower (evalidate can be used at speed of eval() python bytecode)
-- user can provide source code which runs very long time and consumes many resources 
-
-
-[simpleeval](https://github.com/danthedeckie/simpleeval)
-Very similar project, using AST approach too and optimized to re-evaluate pre-parsed expressions. But parsed expressions are stored as more high-level [ast.Expr](https://docs.python.org/3/library/ast.html#ast.Expr) type and this approach is ~10 times slower, while evalidate uses python native `code` type and evaluation itself goes at speed of python eval()
-
-
-evalidate is good to run short same code against different data.
-
-## Benchmarking
-We use `evalidate-vs-asteval.py` which is in benchmark/ directory of repository.
-We prepare list of 1 million of products (actually, we take just 100 products sample, but repeat it 10 000 times to get 1 million), and then filter it, finding only specific products on "untrusted user-supplied expression" (`price < 20` in this case)
-
-~~~
-Products: 1000000 items
-test_asteval_products(): 25.920s
-test_simpleeval_products(): 1.779s
-test_evalidate_products(): 0.160s
-~~~
-
-As you see, evalidate is almost 10 times faster then simpleeval and both are much faster then asteval.
-
-Maybe my test is not perfectly optimized (I'm not expert with simpleeval/asteval), if you can suggest better filtering sample code (which produces faster result), I will include it. But benchmark code must assume expression as unknown and untrusted.
-
-
-## Read about eval() risks
-
-- https://nedbatchelder.com/blog/201206/eval_really_is_dangerous.html
-- https://netsec.expert/posts/breaking-python3-eval-protections/
-- https://realpython.com/python-eval-function/
-
-Note: realpython article shows example with nice short method of validation source (using `code.co_names`), 
-but it's vulnerable, it passes "bomb" from Ned Batchelder article (bomb has empty `co_names` tuple) and crash interpreter. Evalidate can block this code and similar bombs (unless you will intentionally configure evalidate to pass specific bomb code. Yes, with evalidate it is hard to shoot yourself in the foot, but it is possible if you will try hard).
-
-## More info
-
-Want more info? Check source code of module, it's very short and simple, easy to modify
-
-## Contact
-
-Write me: yaroslaff at gmail.com
+Metadata-Version: 2.1
+Name: evalidate
+Version: 1.1.0
+Summary: Validation and secure evaluation of untrusted python expressions
+Home-page: http://github.com/yaroslaff/evalidate
+Author: Yaroslav Polyakov
+Author-email: xenon@sysattack.com
+License: MIT
+Description: ﻿# Evalidate
+        Evalidate is simple python module for safe and very fast eval()'uating user-supplied (possible malicious) python expressions.
+        
+        ## Purpose
+        Originally it's developed for filtering complex data structures e.g. 
+        
+        Find cheap smartphones available for sale:
+        ```python
+        category="smartphones" and price<300 and stock>0
+        ```
+        
+        But also, it can be used for other expressions, e.g. arithmetical, like
+        ```python
+        a+b-100
+        ```
+        
+        Evalidate is fastest among all (known to me) secure eval pythong modules.
+        
+        ## Install
+        
+        ```shell
+        pip3 install evalidate
+        ```
+            
+        ## Security
+        
+        Built-in python features such as compile() or eval() are quite powerful to run any kind of user-supplied code, but could be insecure if used code is malicious like `os.system("rm -rf /")`. Evalidate works on whitelist principle, allowing code only if it consist only of safe operations (based on authors views about what is safe and what is not, your mileage may vary - but you can supply your list of safe operations)
+        
+        
+        ## TL;DR. Just give me safe eval!
+        ```python       
+        from evalidate import Expr, EvalException
+        
+        src = 'a + 40 > b'
+        # src = "__import__('os').system('clear')"
+        
+        try:
+            print(Expr(src).eval({'a':10, 'b':42}))
+        except EvalException as e:
+            print(e)
+        ```
+        
+        Gives output: `True`
+        
+        In case of dangerous code (uncomment second src line to test):
+          
+        output will be: `ERR: Operation type Call is not allowed`
+        
+        
+        ## Exceptions
+        Evalidate throws exceptions `CompilationException`, `ValidationException`, `ExecutionException`. All of them
+        inherit from base exception class `EvalException`.
+        
+        ## Configure validation
+        Evalidate is very flexible, depending on parameters, same code can either pass validation or raise exception.
+        
+        ### Allowing other nodes (operations)
+        
+        Evalidate has built-in set of python operations, which are considered 'safe' (from author point of view). 
+        Code is considered valid only if all of it's operations are in this list. You can override this list by adding argument `nodes` like:
+        ```python
+        Expr('2*2', nodes=['Mult']).eval()
+        ```
+        
+        If you want to start from blank whitelist (discard built-in whitelist), use `Expr(expression, blank=True, nodes=[...])` and then add each node manually (only what you really need) 
+        
+        ### Allowing function calls
+        Evalidate does not allow any function calls by default.
+        
+        To enable `int()` function, need to allow 'Call' node and add this function to list of allowed function:
+        ```python
+        Expr('int(36.6)', nodes=['Call'], funcs=['int']).eval()
+        ```
+        If you want to call str methods:
+        ```python
+        Expr('name.startswith("John")', nodes=['Attribute', 'Call'], attrs=['startswith']).eval(dict(name='John Doe'))
+        ```
+        
+        But even with this settings, exploiting it with expression like `__builtins__["eval"](1)` will fail (good!).
+        
+        
+        ### Exporting my functions to eval code
+        ~~~
+        def one():
+          return 1
+        
+        Expr('one()', nodes=['Call'], my_funcs={"one": one}).eval()
+        ~~~
+        
+        ## Improve speed by using native eval() with validated code
+        Evalidate is very fast, but it's still takes CPU cycles... If you want to achieve maximal possible speed, you can use python native [eval](https://docs.python.org/3/library/functions.html#eval) with this kind of code:
+        
+        ~~~
+        from evalidate import Expr
+        
+        d = dict(a=1, b=2)
+        expr = Expr('a+b')
+        eval(expr.code, None, d) # <-- native python eval, will run at eval() speed
+        ~~~
+        
+        This is as secure as expr.eval(), because `expr.code` is already validated to be secure.
+        
+        Difference is very little: execution of `expr.code` can throw any exception, while `expr.eval()` can throw only ExecutionException. Also, if you want to export your functions to eval, you should do this manually. 
+        
+        ## Limitations
+        
+        evalidate uses [ast.parse()](https://docs.python.org/3/library/ast.html#ast.parse) and returns [AST node](https://docs.python.org/3/library/ast.html#node-classes).
+        
+        >Warning
+        >
+        >It is possible to crash the Python interpreter with a sufficiently large/complex string due to stack depth limitations in Python’s AST compiler. 
+        
+        In my test, works well with 200 nested int(): `int(int(.... int(1)...))` but not with 201. Source code is 1000+ characters. But even if evalidate will get such code, it will just raise `CompilationException`.
+        
+        
+        ### evalidate.security.test_security()
+        Evalidate is very flexible and it's possible to shoot yourself in foot if you will try hard. `test_security()` checks your configuration (addnodes/safenodes, funcs, attrs) against given list of possible attack code or against built-in list of attacks. `test_security()` returns True if everything is OK (all attacks raised ValidationException) or False if something passed.
+        
+        This code will never print (I hope).
+        ~~~python
+        from evalidate.security import test_security
+        
+        test_security() or print("default rules are vulnerable!")
+        ~~~
+        
+        But this will fail because nodes/funcs leads to successful validation for attack (suppose you do not want anyone to call `int()`)
+        ~~~python
+        from evalidate.security import test_security
+        
+        attacks = ['int(1)']
+        
+        test_security(attacks, addnodes=['Call'], funcs=['int'], verbose=True)
+        ~~~
+        
+        It will print:
+        ~~~
+        Testing attack code:
+        int(1)
+        Problem! Attack passed validation without exception!
+        Code:
+        int(1)
+        ~~~
+        
+        
+        
+        
+        ## Example
+        
+        ### Filtering by user-supplied condition ###
+        
+        This is code of `examples/products.py`. Expression is validated and compiled once and executed (as byte-code, very fast) many times, so filtering is both fast and secure.
+        
+        
+        ~~~python
+        #!/usr/bin/env python3
+        
+        import requests
+        from evalidate import Expr, ValidationException, CompilationException, ExecutionException
+        import json
+        import sys
+        
+        data = requests.get('https://dummyjson.com/products?limit=100').json()
+        
+        try:
+            src = sys.argv[1]
+        except IndexError:
+            src = 'True'
+        
+        try:
+            expr = Expr(src)
+        except (ValidationException, CompilationException) as e:
+            print(e)
+            sys.exit(1)
+        
+        c=0
+        for p in data['products']:
+            # print(p)
+            try:
+                r = expr.eval(p)
+                if r:
+                    print(json.dumps(p, indent=2))
+                    c+=1
+            except ExecutionException as e:
+                print("Runtime exception:", e)
+        print("# {} products matches".format(c))
+        ~~~
+        
+        ~~~shell
+        # print all 100 products
+        ./products.py
+        
+        # Only cheap products, 8 matches
+        ./products.py 'price<20'
+        
+        # smartphones (5)
+        ./products.py 'category=="smartphones"'
+        
+        # good smartphones
+        ./products.py 'category=="smartphones" and rating>4.5'
+        
+        # cheap smartphones
+        ./products.py 'category=="smartphones" and price<300'
+        ~~~
+                                               
+        
+        ## Similar projects and benchmark
+        
+        [asteval](https://newville.github.io/asteval/)
+        
+        While asteval can compute much more complex code (define functions, use python math libraries) it has drawbacks:
+        - asteval is much slower (evalidate can be used at speed of eval() python bytecode)
+        - user can provide source code which runs very long time and consumes many resources 
+        
+        
+        [simpleeval](https://github.com/danthedeckie/simpleeval)
+        Very similar project, using AST approach too and optimized to re-evaluate pre-parsed expressions. But parsed expressions are stored as more high-level [ast.Expr](https://docs.python.org/3/library/ast.html#ast.Expr) type and this approach is ~10 times slower, while evalidate uses python native `code` type and evaluation itself goes at speed of python eval()
+        
+        
+        evalidate is good to run short same code against different data.
+        
+        ## Benchmarking
+        We use `benchmark/benchmark.py` in this repository.
+        We prepare list of 1 million of products (actually, we take just 100 products sample, but repeat it 10 000 times to get 1 million), and then filter it, finding only specific products on "untrusted user-supplied expression" (`price < 20` in this case)
+        
+        ~~~
+        Products: 1000000 items
+        evalidate_raw_eval(): 0.266s
+        evalidate_eval(): 0.326s
+        test_simpleeval(): 1.824s
+        test_asteval(): 26.106s
+        ~~~
+        
+        As you see, evalidate is few times faster then simpleeval and both are much faster then asteval.
+        
+        Maybe my test is not perfectly optimized (I'm not expert with simpleeval/asteval), if you can suggest better filtering sample code (which produces faster result), I will include it. But benchmark code must assume expression as unknown and untrusted.
+        
+        
+        ## Read about eval() risks
+        
+        - https://nedbatchelder.com/blog/201206/eval_really_is_dangerous.html
+        - https://netsec.expert/posts/breaking-python3-eval-protections/
+        - https://realpython.com/python-eval-function/
+        
+        Note: realpython article shows example with nice short method of validation source (using `code.co_names`), 
+        but it's vulnerable, it passes "bomb" from Ned Batchelder article (bomb has empty `co_names` tuple) and crash interpreter. Evalidate can block this code and similar bombs (unless you will intentionally configure evalidate to pass specific bomb code. Yes, with evalidate it is hard to shoot yourself in the foot, but it is possible if you will try hard).
+        
+        ## More info
+        
+        Want more info? Check source code of module, it's very short and simple, easy to modify
+        
+        ## Contact
+        
+        Write me: yaroslaff at gmail.com
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Utilities
+Classifier: Topic :: Security
+Classifier: Topic :: Software Development :: Interpreters
+Description-Content-Type: text/markdown
```

### Comparing `evalidate-1.0.3/evalidate/__init__.py` & `evalidate-1.1.0/evalidate/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/python
 
 """Safe user-supplied python expression evaluation."""
 
 import ast
 
-__version__ = '1.0.2'
+__version__ = '1.1.0'
 
 
 class EvalException(Exception):
     pass
 
 
 class ValidationException(EvalException):
@@ -93,18 +93,77 @@
                     # print("attr:", node.func.attr)
                 else:
                     raise ValidationException('Indirect function call')
 
             ast.NodeVisitor.generic_visit(self, node)
         else:
             raise ValidationException(
-                "Operation type {optype} is not allowed".format(
+                "Node type {optype!r} is not allowed. (whitelist it manually)".format(
                     optype=type(node).__name__))
 
 
+class Expr():
+    def __init__(self, expr, nodes=None, blank=False, funcs=None, my_funcs=None, attrs=None, filename=None):
+        self.expr = expr
+        self.my_funcs = my_funcs
+
+        # default nodes
+        if blank:
+            self.nodes = list()
+        else:
+            self.nodes = [
+                # 123, 'asdf'
+                'Num', 'Str',
+                # any expression or constant
+                'Expression', 'Constant',
+                # == ...
+                'Compare', 'Eq', 'NotEq', 'Gt', 'GtE', 'Lt', 'LtE',
+                # variable name
+                'Name', 'Load',
+                'BinOp',
+                'Add', 'Sub',
+                'Subscript', 'Index',  # person['name']
+                'BoolOp', 'And', 'Or', 'UnaryOp', 'Not',  # True and True
+                "In", "NotIn",  # "aaa" in i['list']
+                "IfExp",  # for if expressions, like: expr1 if expr2 else expr3
+                "NameConstant",  # for True and False constants
+                "Div", "Mod"
+            ]
+
+        self.funcs = funcs or list()
+        if self.my_funcs:
+            self.funcs.extend(self.my_funcs.keys())
+
+        self.attrs = attrs or list()
+
+        if nodes:
+            self.nodes.extend(nodes)
+
+        try:
+            self.node = ast.parse(self.expr, '<usercode>', 'eval')
+        except SyntaxError as e:
+            raise CompilationException(e)
+
+        v = SafeAST(safenodes=self.nodes, funcs=self.funcs, attrs=attrs)
+        v.visit(self.node)
+
+        self.code = compile(self.node, filename or '<usercode>', 'eval')
+
+    def eval(self, ctx=None):
+        
+        try:
+            result = eval(self.code, self.my_funcs, ctx)
+        except Exception as e:
+            raise ExecutionException(e)
+
+        return result
+    
+    def __str__(self):
+        return("Expr(expr={expr!r})".format(expr=self.expr))
+
 def evalidate(expression, safenodes=None, addnodes=None, funcs=None, attrs=None):
     """Validate expression.
 
     return node if it passes our checks
     or pass exception from SafeAST visit.
     """
     try:
```

### Comparing `evalidate-1.0.3/evalidate/security.py` & `evalidate-1.1.0/evalidate/security.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from . import ValidationException, evalidate
+from . import ValidationException, evalidate, Expr
 
 simple_attacks = [
 """
 os.system("clear")
 """,
 """
 __import__('os').system('clear')
@@ -40,50 +40,50 @@
     
     # 3.11:         
     '0,0,0,0,0,0,b"BOOM",(),(),(),"","","",0,b"",b"",b"",b"",(),()'
 
 ]
 
 
-def test_attack(attack, safenodes=None, addnodes=None, funcs=None, attrs=None, verbose=False):
+def test_attack(attack, nodes=None, blank=False, funcs=None, attrs=None, verbose=False):
     '''
         test attack. return True if attack detected on validation, good. (False if passed, bad)
     '''
 
     if verbose:
         print("Testing attack code:\n{}".format(attack))
 
     try:
-        node = evalidate(attack, safenodes=safenodes, addnodes=addnodes, funcs=funcs, attrs=attrs)
+        e = Expr(attack, nodes=nodes, blank=blank, funcs=funcs, attrs=attrs)
+        # node = evalidate(attack, safenodes=safenodes, addnodes=addnodes, funcs=funcs, attrs=attrs)
     except ValidationException as e:
         if verbose:
             print("Good! Attack blocked: {}".format(e))
         return True
     else:
         print("Problem! Attack passed validation without exception!\nCode:\n{}".format(attack))
         return False
 
 
 
 
-def test_security(attacks=None, safenodes=None, addnodes=None, funcs=None, attrs=None, verbose=False):
+def test_security(attacks=None, nodes=None, blank=False, funcs=None, attrs=None, verbose=False):
     ''' 
     test all user-given attacks, or built-in attacks.
     Return value: True if good (all attacks detected), False if at least one attack passes validation
     '''
 
     # test user-supplied attacks
     if attacks:
-        return all( [test_attack(attack=attack, safenodes=safenodes, addnodes=addnodes, funcs=funcs, attrs=attrs, verbose=verbose) for attack in attacks] )
+        return all( [test_attack(attack=attack, nodes=nodes, blank=blank, funcs=funcs, attrs=attrs, verbose=verbose) for attack in attacks] )
 
 
     # test built-in set of attacks
-    if not all([test_attack(attack=attack, safenodes=safenodes, addnodes=addnodes, funcs=funcs, attrs=attrs, verbose=verbose) for attack in simple_attacks]):
+    if not all([test_attack(attack=attack, nodes=nodes, blank=blank, funcs=funcs, attrs=attrs, verbose=verbose) for attack in simple_attacks]):
         return False
 
     for payload in boom_payload:
         attack = boom.format(payload=payload)
-        if not test_attack(attack=attack, safenodes=safenodes, addnodes=addnodes, funcs=funcs, attrs=attrs, verbose=verbose):
+        if not test_attack(attack=attack, nodes=nodes, blank=blank, funcs=funcs, attrs=attrs, verbose=verbose):
             return False
         
-
     return True
```

