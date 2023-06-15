# Comparing `tmp/decoratory-0.1.0.2.tar.gz` & `tmp/decoratory-0.1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoratory-0.1.0.2.tar", last modified: Tue Jun 13 16:28:40 2023, max compression
+gzip compressed data, was "decoratory-0.1.0.3.tar", last modified: Thu Jun 15 16:36:26 2023, max compression
```

## Comparing `decoratory-0.1.0.2.tar` & `decoratory-0.1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 16:28:40.070139 decoratory-0.1.0.2/
--rw-rw-rw-   0        0        0     2550 2023-06-02 20:50:35.000000 decoratory-0.1.0.2/License.txt
--rw-rw-rw-   0        0        0    18742 2023-06-13 16:28:40.070139 decoratory-0.1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    17129 2023-06-13 16:02:11.000000 decoratory-0.1.0.2/Readme.rst
--rw-rw-rw-   0        0        0        0 2023-06-10 04:00:34.000000 decoratory-0.1.0.2/Requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 16:28:40.038891 decoratory-0.1.0.2/Sources/
-drwxrwxrwx   0        0        0        0 2023-06-13 16:28:40.070139 decoratory-0.1.0.2/Sources/decoratory/
--rw-rw-rw-   0        0        0      249 2023-06-07 18:32:49.000000 decoratory-0.1.0.2/Sources/decoratory/__init__.py
--rw-rw-rw-   0        0        0     4621 2023-06-13 16:28:13.000000 decoratory-0.1.0.2/Sources/decoratory/__main__.py
--rw-rw-rw-   0        0        0     4855 2023-06-13 16:03:52.000000 decoratory-0.1.0.2/Sources/decoratory/banner.py
--rw-rw-rw-   0        0        0    14154 2023-06-13 16:03:52.000000 decoratory-0.1.0.2/Sources/decoratory/basic.py
--rw-rw-rw-   0        0        0    20586 2023-06-12 14:51:04.000000 decoratory-0.1.0.2/Sources/decoratory/multiton.py
--rw-rw-rw-   0        0        0    38553 2023-06-12 12:49:52.000000 decoratory-0.1.0.2/Sources/decoratory/observer.py
--rw-rw-rw-   0        0        0     7107 2023-06-13 15:03:41.000000 decoratory-0.1.0.2/Sources/decoratory/singleton.py
--rw-rw-rw-   0        0        0    14020 2023-06-13 16:23:56.000000 decoratory-0.1.0.2/Sources/decoratory/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:28:40.070139 decoratory-0.1.0.2/Sources/decoratory.egg-info/
--rw-rw-rw-   0        0        0    18742 2023-06-13 16:28:40.000000 decoratory-0.1.0.2/Sources/decoratory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-06-13 16:28:40.000000 decoratory-0.1.0.2/Sources/decoratory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 16:28:40.000000 decoratory-0.1.0.2/Sources/decoratory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-13 16:28:40.000000 decoratory-0.1.0.2/Sources/decoratory.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 16:28:40.070139 decoratory-0.1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     3944 2023-06-13 16:28:13.000000 decoratory-0.1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:36:26.159623 decoratory-0.1.0.3/
+-rw-rw-rw-   0        0        0     2550 2023-06-02 20:50:35.000000 decoratory-0.1.0.3/License.txt
+-rw-rw-rw-   0        0        0    22392 2023-06-15 16:36:26.159623 decoratory-0.1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    20767 2023-06-15 16:35:28.000000 decoratory-0.1.0.3/Readme.rst
+-rw-rw-rw-   0        0        0        0 2023-06-10 04:00:34.000000 decoratory-0.1.0.3/Requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 16:36:26.112747 decoratory-0.1.0.3/Sources/
+drwxrwxrwx   0        0        0        0 2023-06-15 16:36:26.143999 decoratory-0.1.0.3/Sources/decoratory/
+-rw-rw-rw-   0        0        0      249 2023-06-07 18:32:49.000000 decoratory-0.1.0.3/Sources/decoratory/__init__.py
+-rw-rw-rw-   0        0        0     4621 2023-06-15 16:35:51.000000 decoratory-0.1.0.3/Sources/decoratory/__main__.py
+-rw-rw-rw-   0        0        0     4855 2023-06-13 16:03:52.000000 decoratory-0.1.0.3/Sources/decoratory/banner.py
+-rw-rw-rw-   0        0        0    14152 2023-06-14 15:11:14.000000 decoratory-0.1.0.3/Sources/decoratory/basic.py
+-rw-rw-rw-   0        0        0    15763 2023-06-15 16:24:13.000000 decoratory-0.1.0.3/Sources/decoratory/multiton.py
+-rw-rw-rw-   0        0        0    38553 2023-06-12 12:49:52.000000 decoratory-0.1.0.3/Sources/decoratory/observer.py
+-rw-rw-rw-   0        0        0     9089 2023-06-15 16:24:13.000000 decoratory-0.1.0.3/Sources/decoratory/singleton.py
+-rw-rw-rw-   0        0        0    13845 2023-06-15 16:24:13.000000 decoratory-0.1.0.3/Sources/decoratory/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:36:26.143999 decoratory-0.1.0.3/Sources/decoratory.egg-info/
+-rw-rw-rw-   0        0        0    22392 2023-06-15 16:36:26.000000 decoratory-0.1.0.3/Sources/decoratory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-06-15 16:36:26.000000 decoratory-0.1.0.3/Sources/decoratory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 16:36:26.000000 decoratory-0.1.0.3/Sources/decoratory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-15 16:36:26.000000 decoratory-0.1.0.3/Sources/decoratory.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 16:36:26.159623 decoratory-0.1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     4017 2023-06-15 16:35:51.000000 decoratory-0.1.0.3/setup.py
```

### Comparing `decoratory-0.1.0.2/License.txt` & `decoratory-0.1.0.3/License.txt`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.0.2/PKG-INFO` & `decoratory-0.1.0.3/Readme.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,18 @@
-Metadata-Version: 2.1
-Name: decoratory
-Version: 0.1.0.2
-Summary: Decorators: Singleton, Multiton, Observer, generic Wrapper.
-Home-page: http://evation.eu
-Download-URL: http://evation.eu
-Author: Martin Abel
-Author-email: Martin Abel <python@evation.eu>
-Maintainer: Martin Abel
-Maintainer-email: Martin Abel <python@evation.eu>
-License: PSF
-Project-URL: Projekt, http://evation.eu
-Project-URL: Release Notes, http://evation.eu
-Project-URL: Download, http://evation.eu
-Keywords: decorator singleton multiton observer observable wrapper
-Platform: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Information Technology
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation
-Classifier: License :: OSI Approved :: Python Software Foundation License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Education
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: License.txt
-
 
 .. _top:
 
 ==============================================================================
 Decoratory
 ==============================================================================
 
 
 **Introduction**
 
-The "decoratory" package is based on the `Decorator Arguments Pattern`_, an 
+The *decoratory package* is based on the `Decorator Arguments Pattern`_, an 
 integrated concept for Python decorators with and without parameters. In
 addition, all decorators created with it support complex arguments, e.g. 
 lists of values and functions, without unnecessarily complicating the 
 decoration of simple cases by these extensions. All implementation details 
 are described on the `project homepage`_.
 
 
@@ -60,18 +21,19 @@
     pip install --upgrade decoratory
 
 After installation, basic information about the package, the individual 
 modules and their methods is also available from the command line. ::
 
     python -m decoratory --help
 
+.. _toc:
 
-**Package Content**
+**Package Contents**
 
-The decoratory package available here includes some classic decorators
+The *decoratory package* available here includes some classic decorators
 implemented and functionally extended with this concept, e.g.
 
 * `Singleton`_
 * `Multiton`_
 * `Wrapper`_
 * `Observer`_   (coming soon...)
 
@@ -117,50 +79,107 @@
 
     # Create Instances
     a = Animal(name='Bello')        # Creates Bello
     b = Animal(name='Tessa')        # Returns Bello
 
 If instances of the class ``Animal`` are now created, this is only done for the 
 very first instantiation, and for all further instantiations always this 
-"primary instance" is given back.
+*primary instance* is given back.
             
 .. code-block:: python
 
     # *** example_singleton.py - verfication of the unique instance
 
     # Case 1: Static decoration using @Singleton or @Singleton()
     print(f"a = {a}")               # a = Animal('Bello')
     print(f"b = {b}")               # b = Animal('Bello')
     print(f"a is b: {a is b}")      # a is b: True
     print(f"a == b: {a == b}")      # a == b: True
 
-If instead of the above "static decoration" using pie-notation, i.e. with 
-@-notation at the class declaration, the "dynamic decoration" within Python 
+If instead of the above *static decoration* using pie-notation, i.e. with 
+@-notation at the class declaration, the *dynamic decoration* within Python 
 code is used, additional parameters can be passed to the decorator for 
 passing to the class constructor.
 
 .. code-block:: python
 
     # *** example_singleton.py - dynamic decoration with extra parameters
 
     # Case 2: Dynamic decoration providing extra initial default values 
     Animal = Singleton(Animal, 'Bello')
     Animal()                        # Using the decorator's default 'Bello'
-    Animal(name='Tessa')            # Returns Bello
-    print(Animal.instance)          # Animal('Bello')
+    a = Animal(name='Tessa')        # Returns Bello
+    print(a)                        # Animal('Bello')
 
 Quite generally, for all the following decorators based on this 
 `Decorator Arguments Pattern`_, these two properties are always fulfilled:
 
-.. note::
+#. Decoration as a class (without parentheses) and Decoration as an instance 
+   (with empty parentheses) are equivalent
+#. For dynamic decoration, extra parameters can be passed, e.g. for the 
+   class constructor
+
+So far, this singleton implementation follows the concept of *once and 
+forever*, i.e. whenever a new instance of a class is created, one always
+gets the *primary instance* back - without any possibility of ever changing 
+it again.
+
+Although this behavior is consistent with the basic concept of a singleton, 
+there are situations where it might be useful to reset a *singleton*. Such 
+a *resettable singleton* could be useful to express in code that an instance 
+is often retrieved but rarely changed.
+
+.. code-block:: python
+
+    # *** example_singleton.py - decoration as 'resettable singleton'
+
+    from decoratory.singleton import Singleton
+
+    @Singleton(resettable=True)     # Exposes an additional reset method 
+    class Animal:
+        def __init__(self, name):
+            self.name = name
 
-    * Decoration as a class (without parentheses) and Decoration as an instance 
-      (with empty parentheses) are equivalent
-    * For dynamic decoration, extra parameters can be passed, e.g. for the 
-      class constructor
+        def __repr__(self):
+            return f"{self.__class__.__name__}('{self.name}')"
+
+    # Case 3: Decoration using @Singleton(resettable=True)
+    print(Animal(name='Bello'))     # Animal('Bello')
+    print(Animal(name='Tessa'))     # Animal('Bello')   (=primary instance)
+    Animal.reset()                  # Reset the singleton
+    print(Animal(name='Tessa'))     # Animal('Tessa')
+    print(Animal(name='Bello'))     # Animal('Tessa')   (=primary instance)
+
+Without ``resettable=True`` decoration ``Animal`` has no ``reset`` method and 
+the call ``Animal.reset()`` will fail raising an ``AttributeError``.
+
+With the same intention, the retrieval of the *primary instance* is also 
+locked by default, but can be unlocked during decoration with the 
+``accessible=True`` parameter, which allows ``Animal`` to expose the 
+``get_instance()`` method.
+
+.. code-block:: python
+
+    # *** example_singleton.py - decoration as 'accessible singleton'
+
+    from decoratory.singleton import Singleton
+
+    @Singleton(accessible=True)     # Exposes a get_instance method 
+    class Animal:
+        def __init__(self, name):
+            self.name = name
+
+        def __repr__(self):
+            return f"{self.__class__.__name__}('{self.name}')"
+
+    # Case 4: Decoration using @Singleton(accessible=True)
+    a = Animal(name='Bello')        # Animal('Bello')
+    b = Animal.get_instance()       # Animal('Bello')   (=primary instance)
+    print(a)                        # Animal('Bello')
+    print(b)                        # Animal('Bello')
 
 
 ******************************************************************************
 Multiton
 ******************************************************************************
 
 A `multiton pattern`_ is a design pattern that extends the singleton pattern.
@@ -168,28 +187,29 @@
 ensures one single (unique) *instance per key value of a dictionary*.
 
 In this implementation the key parameter can be either any immutable type
 or a callable returning such an immutable type which can be used as a key
 of a dictionary. In case of an invalid key, key is set ``None`` and with only 
 one key value the multiton simply collapses to a singleton, therefore the 
 decoration ``@Multiton`` resp. ``@Multiton()`` or even ``@Multiton(key=17)`` 
-or  ``@Multiton(key='some fixed value')`` and so on always creates a singleton.
+or  ``@Multiton(key='some constant value')`` and so on always creates a 
+singleton.
 
-Usually the key is independent of the classified object. However, it is not 
-uncommon for it to be part of the classified object itself, as in the 
-following example, where the key string matches the parameter ``name`` of 
-the constructor of the class ``Animal``.
+Normally, the key is part of or is composed from the initial values of the 
+classified object, as in the following example, where the key function matches 
+the signature of the constructor and uses the initial value of the ``name`` 
+parameter to construct a key value for the instances of ``Animal``.
 
 .. code-block:: python
    
     # *** example_multitonton.py - class Animal with Multiton decoration
 
     from decoratory.multiton import Multiton
 
-    @Multiton(key='name')           # uses kwargs['name'] as key
+    @Multiton(key=lambda spec, name: name)
     class Animal:
         def __init__(self, spec, name):
             self.spec = spec
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.spec}', '{self.name}')"
@@ -197,72 +217,105 @@
     # Create Instances
     a = Animal('dog', name='Bello')
     b = Animal('cat', name='Mausi')
     c = Animal('dog', name='Tessa')
 
 When instances of the class ``Animal`` are now created, this only happens for 
 the *first instantiation per key value*, the initial name of the animal. For 
-all subsequent instantiations, this "primary instance per key value" is 
+all subsequent instantiations, this *primary instance per key value* is 
 returned. But for each new key value, a new ``Animal`` instance is created 
 and stored in the internal directory.
 
 .. code-block:: python
 
     # *** example_multitonton.py - One unique instance per name
 
-    # Case 1: key='name' references kwargs['name'] from __init__(..,name)
+    # Case 1: decoration @Multiton(key=lambda spec, name: name)
     print(a)                        # Animal('dog', 'Bello')
     print(b)                        # Animal('cat', 'Mausi')
     print(c)                        # Animal('dog', 'Tessa')
 
 With three different names, a separate instance is created in each case. 
 In contrast, the following variant distinguishes only two types (equivalence 
 classes): animals with a character 'a' in their name and those without and 
 thus the key values can only be ``True`` or ``False``.
 
 .. code-block:: python
 
     # *** example_multitonton.py - One unique instance per equivalence class
 
-    # Case 2: with decoration @Multiton(key=lambda spec, name: 'a' in name)
-    print(a)                        # Animal('dog', 'Bello'), key=False
-    print(b)                        # Animal('cat', 'Mausi'), key=True
-    print(c)                        # Animal('cat', 'Mausi'), key=True
+    # Case 2: decoration @Multiton(key=lambda spec, name: 'a' in name)
+    print(a)                        # Animal('dog', 'Bello')
+    print(b)                        # Animal('cat', 'Mausi')
+    print(c)                        # Animal('cat', 'Mausi')
+
+The initial parameter values of the constructor can also be accessed by their 
+``args``-index or ``kwargs``-name. So the following decorations are also 
+possible:
+
+.. code-block:: python
+
+    # *** example_multitonton.py - Alternative decoration examples
+
+    # Case 3: One unique instance per specie
+    @Multiton(key="{0}".format)     # spec is args[0]
+    class Animal:
+        ...
 
+    # Case 4: One unique instance per name
+    @Multiton(key="{name}".format)  # name is kwargs['name']
+    class Animal:
+        ...
+
+    # Case 5: One unique instance for all init values, i.e. no duplicates
+    @Multiton(key=lambda spec, name: (spec, name))
+    class Animal:
+        ...
+
+    # Case 6: One unique instance from a @staticmethod or @classmethod
+    @Multiton(key=F("my_key"))      # Late binding with F(classmethod_string)
+    class Animal:
+        ...
+
+        @classmethod
+        def my_key(cls, spec, name):
+            return 'a' in name
+        
 To actively control access to new equivalence classes, ``Multiton`` provides 
 the ``seal()``, ``unseal()``, and ``issealed()`` methods for sealing, unsealing,
-and checking the sealing state of the ``Multiton``. By default, the sealed 
+and checking the sealing state of the ``Multiton``. By default, the sealing 
 state is set ``False``, so for every new key a new (unique) object is 
 instantiated. When sealed (e.g. later in the process) is set ``True`` the 
 dictionary has completed, i.e. restricted to the current object set and 
 any new key raises a ``KeyError``.
 
 For deeper, special requirements on the equivalence classes of a multiton 
-then by means of the method ``instances()`` the internal directory can also 
-be actively manipulated, which of course should be done with caution and 
-generally is not recommended. 
-
-For this reason, each object knows its multiton: Setting ``Multiton``'s ``attrib`` 
-parameter while decoration to a valid attribute name string the multiton is 
-attributed in the new instantiated substitute object, is the chosen name 
-invalid or missing, the default attribute name ``multiton`` is chosen. 
+by setting the decorator parameter ``accessible=True``, the method 
+``get_instances()`` is enabled, which grants direct access to the internal 
+directory of the instances. This can be actively manipulated in this way, 
+which of course should be done with care and is generally not recommended.  
 
 .. code-block:: python
 
-    # *** example_multitonton.py - One unique instance per equivalence class
-
-    # Case 3: with decoration @Multiton(key=lambda spec, name: 'a' in name)
-    print(a)                        # Animal('dog', 'Bello')
-    print(a.multiton)               # <decoratory.multiton.Multiton object..>
-    print(a.multiton.instances())   # {False: Animal('dog', 'Bello'), 
-                                    #   True: Animal('cat', 'Mausi')}
-
-Thus, in the above example, ``a.multiton`` would be the multiton of ``a`` 
-('Bello') and ``a.multiton.instances()`` would be the directory of equivalence 
-classes to which it belongs.
+    # *** example_multitonton.py - Accessibility to the internal directory
+
+    # Case 7: with decoration @Multiton(key=lambda spec, name: 'a' in name,
+    #                                   accessible=True)
+    print(Animal.get_instances())   # {}
+    a = Animal('dog', name='Bello') # 
+    print(Animal.get_instances())   # {False: Animal('dog', 'Bello')}
+    b = Animal('cat', name='Mausi') # 
+    c = Animal('dog', name='Tessa') # 
+    print(Animal.get_instances())   # {False: Animal('dog', 'Bello'),  
+                                    #  True:  Animal('cat', 'Mausi')}
+
+In situations where it might be useful to reset the multiton to express in 
+code that instances are often retrieved but rarely modified, setting the 
+decorator parameter ``resettable=True`` will expose the ``reset()`` method, 
+by means of which the internal directory of instances can be completely cleared.
 
 .. warning::
  
     Classifications into the multiton directory are done only once on
     initial key data. Subsequent changes affecting a key value are not 
     reflected in the multiton directory, i.e. the directory may then be 
     corrupted by such modifications.
@@ -291,16 +344,16 @@
 ``before``, ``after`` and ``replace``, can be combined with each other and 
 support both single callables and (nested) lists of ``F``-types 
 (imported from module decoratory.basic, see below for details). 
 In addition, ``replace`` supports passing results from successive 
 replacement calls through an optional keyword argument named ``result`` 
 (defaut value is ``None``).
 
-Even without any of these arguments, such a "do nothing wrapper" can be used 
-to "overwrite" default values, for example.
+Even without any of these arguments, such a *do nothing wrapper* can be used 
+to *overwrite* default values, for example.
 
 .. code-block:: python
 
     # *** example_wrapper.py - overwrite default parameter values
 
     from decoratory.wrapper import Wrapper
 
@@ -411,15 +464,15 @@
 .. note::
 
     Decorations to ``@staticmethod`` or ``@classmethod`` can be done 
     analogously to the function decorations above, since they already exist 
     at compile time. Instance methods, on the other hand, do not exist until 
     an object instance is created and must be handled differently.
 
-With ``Wrapper`` and custom service functions, a "private wrapper library" 
+With ``Wrapper`` and custom service functions, a *private wrapper library* 
 can be built and reused.
 
 .. code-block:: python
 
     # *** example_wrapper.py - private wrapper library
 
     from decoratory.wrapper import Wrapper
@@ -447,24 +500,27 @@
 coming soon...
 
 
 ******************************************************************************
 Version History
 ******************************************************************************
 
+**Version: 0.1.0.3, Build: 2023-06-15**
+    
+- accessible parameter for singleton and multiton, incl. documentation
+- resettable parameter for singleton and multiton, incl. documentation
+
 **Version: 0.1.0.2, Build: 2023-06-13**
 
-- Documentation enhancements
+- Documentation enhancements for for singleton, multiton and wrapper
 
 **Version: 0.1.0.1, Build: 2023-06-12**
 
 - Initial version with Singleton, Multiton and Wrapper
 
 
 .. ===========================================================================
 .. _project homepage: http://evation.eu
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _Decorator Arguments Pattern: http://evation.eu
 
-`back to top <#top>`_
-
```

### Comparing `decoratory-0.1.0.2/Readme.rst` & `decoratory-0.1.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,57 @@
+Metadata-Version: 2.1
+Name: decoratory
+Version: 0.1.0.3
+Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
+Home-page: http://evation.eu
+Download-URL: http://evation.eu
+Author: Martin Abel
+Author-email: Martin Abel <python@evation.eu>
+Maintainer: Martin Abel
+Maintainer-email: Martin Abel <python@evation.eu>
+License: PSF
+Project-URL: Projekt, http://evation.eu
+Project-URL: Release Notes, http://evation.eu
+Project-URL: Download, http://evation.eu
+Keywords: decorator singleton multiton observer observable wrapper
+Platform: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Information Technology
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation
+Classifier: License :: OSI Approved :: Python Software Foundation License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Education
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: License.txt
+
 
 .. _top:
 
 ==============================================================================
 Decoratory
 ==============================================================================
 
 
 **Introduction**
 
-The "decoratory" package is based on the `Decorator Arguments Pattern`_, an 
+The *decoratory package* is based on the `Decorator Arguments Pattern`_, an 
 integrated concept for Python decorators with and without parameters. In
 addition, all decorators created with it support complex arguments, e.g. 
 lists of values and functions, without unnecessarily complicating the 
 decoration of simple cases by these extensions. All implementation details 
 are described on the `project homepage`_.
 
 
@@ -21,18 +60,19 @@
     pip install --upgrade decoratory
 
 After installation, basic information about the package, the individual 
 modules and their methods is also available from the command line. ::
 
     python -m decoratory --help
 
+.. _toc:
 
-**Package Content**
+**Package Contents**
 
-The decoratory package available here includes some classic decorators
+The *decoratory package* available here includes some classic decorators
 implemented and functionally extended with this concept, e.g.
 
 * `Singleton`_
 * `Multiton`_
 * `Wrapper`_
 * `Observer`_   (coming soon...)
 
@@ -78,50 +118,107 @@
 
     # Create Instances
     a = Animal(name='Bello')        # Creates Bello
     b = Animal(name='Tessa')        # Returns Bello
 
 If instances of the class ``Animal`` are now created, this is only done for the 
 very first instantiation, and for all further instantiations always this 
-"primary instance" is given back.
+*primary instance* is given back.
             
 .. code-block:: python
 
     # *** example_singleton.py - verfication of the unique instance
 
     # Case 1: Static decoration using @Singleton or @Singleton()
     print(f"a = {a}")               # a = Animal('Bello')
     print(f"b = {b}")               # b = Animal('Bello')
     print(f"a is b: {a is b}")      # a is b: True
     print(f"a == b: {a == b}")      # a == b: True
 
-If instead of the above "static decoration" using pie-notation, i.e. with 
-@-notation at the class declaration, the "dynamic decoration" within Python 
+If instead of the above *static decoration* using pie-notation, i.e. with 
+@-notation at the class declaration, the *dynamic decoration* within Python 
 code is used, additional parameters can be passed to the decorator for 
 passing to the class constructor.
 
 .. code-block:: python
 
     # *** example_singleton.py - dynamic decoration with extra parameters
 
     # Case 2: Dynamic decoration providing extra initial default values 
     Animal = Singleton(Animal, 'Bello')
     Animal()                        # Using the decorator's default 'Bello'
-    Animal(name='Tessa')            # Returns Bello
-    print(Animal.instance)          # Animal('Bello')
+    a = Animal(name='Tessa')        # Returns Bello
+    print(a)                        # Animal('Bello')
 
 Quite generally, for all the following decorators based on this 
 `Decorator Arguments Pattern`_, these two properties are always fulfilled:
 
-.. note::
+#. Decoration as a class (without parentheses) and Decoration as an instance 
+   (with empty parentheses) are equivalent
+#. For dynamic decoration, extra parameters can be passed, e.g. for the 
+   class constructor
+
+So far, this singleton implementation follows the concept of *once and 
+forever*, i.e. whenever a new instance of a class is created, one always
+gets the *primary instance* back - without any possibility of ever changing 
+it again.
+
+Although this behavior is consistent with the basic concept of a singleton, 
+there are situations where it might be useful to reset a *singleton*. Such 
+a *resettable singleton* could be useful to express in code that an instance 
+is often retrieved but rarely changed.
+
+.. code-block:: python
+
+    # *** example_singleton.py - decoration as 'resettable singleton'
+
+    from decoratory.singleton import Singleton
+
+    @Singleton(resettable=True)     # Exposes an additional reset method 
+    class Animal:
+        def __init__(self, name):
+            self.name = name
 
-    * Decoration as a class (without parentheses) and Decoration as an instance 
-      (with empty parentheses) are equivalent
-    * For dynamic decoration, extra parameters can be passed, e.g. for the 
-      class constructor
+        def __repr__(self):
+            return f"{self.__class__.__name__}('{self.name}')"
+
+    # Case 3: Decoration using @Singleton(resettable=True)
+    print(Animal(name='Bello'))     # Animal('Bello')
+    print(Animal(name='Tessa'))     # Animal('Bello')   (=primary instance)
+    Animal.reset()                  # Reset the singleton
+    print(Animal(name='Tessa'))     # Animal('Tessa')
+    print(Animal(name='Bello'))     # Animal('Tessa')   (=primary instance)
+
+Without ``resettable=True`` decoration ``Animal`` has no ``reset`` method and 
+the call ``Animal.reset()`` will fail raising an ``AttributeError``.
+
+With the same intention, the retrieval of the *primary instance* is also 
+locked by default, but can be unlocked during decoration with the 
+``accessible=True`` parameter, which allows ``Animal`` to expose the 
+``get_instance()`` method.
+
+.. code-block:: python
+
+    # *** example_singleton.py - decoration as 'accessible singleton'
+
+    from decoratory.singleton import Singleton
+
+    @Singleton(accessible=True)     # Exposes a get_instance method 
+    class Animal:
+        def __init__(self, name):
+            self.name = name
+
+        def __repr__(self):
+            return f"{self.__class__.__name__}('{self.name}')"
+
+    # Case 4: Decoration using @Singleton(accessible=True)
+    a = Animal(name='Bello')        # Animal('Bello')
+    b = Animal.get_instance()       # Animal('Bello')   (=primary instance)
+    print(a)                        # Animal('Bello')
+    print(b)                        # Animal('Bello')
 
 
 ******************************************************************************
 Multiton
 ******************************************************************************
 
 A `multiton pattern`_ is a design pattern that extends the singleton pattern.
@@ -129,28 +226,29 @@
 ensures one single (unique) *instance per key value of a dictionary*.
 
 In this implementation the key parameter can be either any immutable type
 or a callable returning such an immutable type which can be used as a key
 of a dictionary. In case of an invalid key, key is set ``None`` and with only 
 one key value the multiton simply collapses to a singleton, therefore the 
 decoration ``@Multiton`` resp. ``@Multiton()`` or even ``@Multiton(key=17)`` 
-or  ``@Multiton(key='some fixed value')`` and so on always creates a singleton.
+or  ``@Multiton(key='some constant value')`` and so on always creates a 
+singleton.
 
-Usually the key is independent of the classified object. However, it is not 
-uncommon for it to be part of the classified object itself, as in the 
-following example, where the key string matches the parameter ``name`` of 
-the constructor of the class ``Animal``.
+Normally, the key is part of or is composed from the initial values of the 
+classified object, as in the following example, where the key function matches 
+the signature of the constructor and uses the initial value of the ``name`` 
+parameter to construct a key value for the instances of ``Animal``.
 
 .. code-block:: python
    
     # *** example_multitonton.py - class Animal with Multiton decoration
 
     from decoratory.multiton import Multiton
 
-    @Multiton(key='name')           # uses kwargs['name'] as key
+    @Multiton(key=lambda spec, name: name)
     class Animal:
         def __init__(self, spec, name):
             self.spec = spec
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.spec}', '{self.name}')"
@@ -158,72 +256,105 @@
     # Create Instances
     a = Animal('dog', name='Bello')
     b = Animal('cat', name='Mausi')
     c = Animal('dog', name='Tessa')
 
 When instances of the class ``Animal`` are now created, this only happens for 
 the *first instantiation per key value*, the initial name of the animal. For 
-all subsequent instantiations, this "primary instance per key value" is 
+all subsequent instantiations, this *primary instance per key value* is 
 returned. But for each new key value, a new ``Animal`` instance is created 
 and stored in the internal directory.
 
 .. code-block:: python
 
     # *** example_multitonton.py - One unique instance per name
 
-    # Case 1: key='name' references kwargs['name'] from __init__(..,name)
+    # Case 1: decoration @Multiton(key=lambda spec, name: name)
     print(a)                        # Animal('dog', 'Bello')
     print(b)                        # Animal('cat', 'Mausi')
     print(c)                        # Animal('dog', 'Tessa')
 
 With three different names, a separate instance is created in each case. 
 In contrast, the following variant distinguishes only two types (equivalence 
 classes): animals with a character 'a' in their name and those without and 
 thus the key values can only be ``True`` or ``False``.
 
 .. code-block:: python
 
     # *** example_multitonton.py - One unique instance per equivalence class
 
-    # Case 2: with decoration @Multiton(key=lambda spec, name: 'a' in name)
-    print(a)                        # Animal('dog', 'Bello'), key=False
-    print(b)                        # Animal('cat', 'Mausi'), key=True
-    print(c)                        # Animal('cat', 'Mausi'), key=True
+    # Case 2: decoration @Multiton(key=lambda spec, name: 'a' in name)
+    print(a)                        # Animal('dog', 'Bello')
+    print(b)                        # Animal('cat', 'Mausi')
+    print(c)                        # Animal('cat', 'Mausi')
+
+The initial parameter values of the constructor can also be accessed by their 
+``args``-index or ``kwargs``-name. So the following decorations are also 
+possible:
+
+.. code-block:: python
+
+    # *** example_multitonton.py - Alternative decoration examples
+
+    # Case 3: One unique instance per specie
+    @Multiton(key="{0}".format)     # spec is args[0]
+    class Animal:
+        ...
 
+    # Case 4: One unique instance per name
+    @Multiton(key="{name}".format)  # name is kwargs['name']
+    class Animal:
+        ...
+
+    # Case 5: One unique instance for all init values, i.e. no duplicates
+    @Multiton(key=lambda spec, name: (spec, name))
+    class Animal:
+        ...
+
+    # Case 6: One unique instance from a @staticmethod or @classmethod
+    @Multiton(key=F("my_key"))      # Late binding with F(classmethod_string)
+    class Animal:
+        ...
+
+        @classmethod
+        def my_key(cls, spec, name):
+            return 'a' in name
+        
 To actively control access to new equivalence classes, ``Multiton`` provides 
 the ``seal()``, ``unseal()``, and ``issealed()`` methods for sealing, unsealing,
-and checking the sealing state of the ``Multiton``. By default, the sealed 
+and checking the sealing state of the ``Multiton``. By default, the sealing 
 state is set ``False``, so for every new key a new (unique) object is 
 instantiated. When sealed (e.g. later in the process) is set ``True`` the 
 dictionary has completed, i.e. restricted to the current object set and 
 any new key raises a ``KeyError``.
 
 For deeper, special requirements on the equivalence classes of a multiton 
-then by means of the method ``instances()`` the internal directory can also 
-be actively manipulated, which of course should be done with caution and 
-generally is not recommended. 
-
-For this reason, each object knows its multiton: Setting ``Multiton``'s ``attrib`` 
-parameter while decoration to a valid attribute name string the multiton is 
-attributed in the new instantiated substitute object, is the chosen name 
-invalid or missing, the default attribute name ``multiton`` is chosen. 
+by setting the decorator parameter ``accessible=True``, the method 
+``get_instances()`` is enabled, which grants direct access to the internal 
+directory of the instances. This can be actively manipulated in this way, 
+which of course should be done with care and is generally not recommended.  
 
 .. code-block:: python
 
-    # *** example_multitonton.py - One unique instance per equivalence class
-
-    # Case 3: with decoration @Multiton(key=lambda spec, name: 'a' in name)
-    print(a)                        # Animal('dog', 'Bello')
-    print(a.multiton)               # <decoratory.multiton.Multiton object..>
-    print(a.multiton.instances())   # {False: Animal('dog', 'Bello'), 
-                                    #   True: Animal('cat', 'Mausi')}
-
-Thus, in the above example, ``a.multiton`` would be the multiton of ``a`` 
-('Bello') and ``a.multiton.instances()`` would be the directory of equivalence 
-classes to which it belongs.
+    # *** example_multitonton.py - Accessibility to the internal directory
+
+    # Case 7: with decoration @Multiton(key=lambda spec, name: 'a' in name,
+    #                                   accessible=True)
+    print(Animal.get_instances())   # {}
+    a = Animal('dog', name='Bello') # 
+    print(Animal.get_instances())   # {False: Animal('dog', 'Bello')}
+    b = Animal('cat', name='Mausi') # 
+    c = Animal('dog', name='Tessa') # 
+    print(Animal.get_instances())   # {False: Animal('dog', 'Bello'),  
+                                    #  True:  Animal('cat', 'Mausi')}
+
+In situations where it might be useful to reset the multiton to express in 
+code that instances are often retrieved but rarely modified, setting the 
+decorator parameter ``resettable=True`` will expose the ``reset()`` method, 
+by means of which the internal directory of instances can be completely cleared.
 
 .. warning::
  
     Classifications into the multiton directory are done only once on
     initial key data. Subsequent changes affecting a key value are not 
     reflected in the multiton directory, i.e. the directory may then be 
     corrupted by such modifications.
@@ -252,16 +383,16 @@
 ``before``, ``after`` and ``replace``, can be combined with each other and 
 support both single callables and (nested) lists of ``F``-types 
 (imported from module decoratory.basic, see below for details). 
 In addition, ``replace`` supports passing results from successive 
 replacement calls through an optional keyword argument named ``result`` 
 (defaut value is ``None``).
 
-Even without any of these arguments, such a "do nothing wrapper" can be used 
-to "overwrite" default values, for example.
+Even without any of these arguments, such a *do nothing wrapper* can be used 
+to *overwrite* default values, for example.
 
 .. code-block:: python
 
     # *** example_wrapper.py - overwrite default parameter values
 
     from decoratory.wrapper import Wrapper
 
@@ -372,15 +503,15 @@
 .. note::
 
     Decorations to ``@staticmethod`` or ``@classmethod`` can be done 
     analogously to the function decorations above, since they already exist 
     at compile time. Instance methods, on the other hand, do not exist until 
     an object instance is created and must be handled differently.
 
-With ``Wrapper`` and custom service functions, a "private wrapper library" 
+With ``Wrapper`` and custom service functions, a *private wrapper library* 
 can be built and reused.
 
 .. code-block:: python
 
     # *** example_wrapper.py - private wrapper library
 
     from decoratory.wrapper import Wrapper
@@ -408,24 +539,27 @@
 coming soon...
 
 
 ******************************************************************************
 Version History
 ******************************************************************************
 
+**Version: 0.1.0.3, Build: 2023-06-15**
+    
+- accessible parameter for singleton and multiton, incl. documentation
+- resettable parameter for singleton and multiton, incl. documentation
+
 **Version: 0.1.0.2, Build: 2023-06-13**
 
-- Documentation enhancements
+- Documentation enhancements for for singleton, multiton and wrapper
 
 **Version: 0.1.0.1, Build: 2023-06-12**
 
 - Initial version with Singleton, Multiton and Wrapper
 
 
 .. ===========================================================================
 .. _project homepage: http://evation.eu
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _Decorator Arguments Pattern: http://evation.eu
 
-`back to top <#top>`_
-
```

### Comparing `decoratory-0.1.0.2/Sources/decoratory/__main__.py` & `decoratory-0.1.0.3/Sources/decoratory/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.0.2"
-__date__ = "2023-06-13"
-__time__ = "18:28:13"
+__version__ = "0.1.0.3"
+__date__ = "2023-06-15"
+__time__ = "18:35:51"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = []
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.1.0.2/Sources/decoratory/banner.py` & `decoratory-0.1.0.3/Sources/decoratory/banner.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.0.2/Sources/decoratory/basic.py` & `decoratory-0.1.0.3/Sources/decoratory/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.0.2"
-__date__ = "2023-06-13"
-__time__ = "18:03:50"
+__version__ = "0.1.0.3"
+__date__ = "2023-06-14"
+__time__ = "17:11:10"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Activation", "Parser", "F", "X"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -312,15 +312,15 @@
         for li in list_obj:
             if isinstance(li, list):
                 result.extend(cls.list(li))
             elif isinstance(li, tuple):
                 result.append(cls.tuple(li))
             elif isinstance(li, F):
                 result.append(li)
-            elif callable(li) or isinstance(item, str):
+            elif callable(li) or isinstance(li, str):
                 result.append(F(li))
             elif li is None:
                 pass
             else:
                 raise TypeError(f"List element '{li}' cannot be parsed.")
         return result
```

### Comparing `decoratory-0.1.0.2/Sources/decoratory/multiton.py` & `decoratory-0.1.0.3/Sources/decoratory/multiton.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,170 +1,145 @@
 #!/usr/bin/env python
 # -*- coding=UTF-8 -*-
 # vim: fileencoding=UTF-8 tabstop=8 expandtab shiftwidth=4 softtabstop=4
 # -----------------------------------------------------------------------------
 # Document Description
 """**Multiton**
 
-    A multiton is a design pattern that extends the singleton pattern.
+    A multiton pattern is a design pattern that extends the singleton pattern.
     Whereas the singleton allows for exactly one instance per class, the
-    multiton pattern ensures one single (unique) instance per key value
-    (of a dictionary).
-
-    In this implementation the key parameter can be either any immutable type
-    or a callable returning such an immutable type which can be used as a key
-    of a dictionary. In case of an invalid key, key is set None and the
-    multiton simply collapses to a singleton.
-
-    Setting the attrib parameter to a valid attribute name string the multiton
-    is attributed in the new instantiated substitute object, is the name
-    invalid, the attribute name 'multiton' is chosen.
-
-    By default, the sealed parameter is set False, so for every new key a new
-    (unique) object is instantiated. When sealed (e.g. later in the process)
-    is set True the dictionary has completed, i.e. restricted to the current
-    object set and any new key raises a KeyError.
-
-    Warning: Classifications into the multiton directory are done only once on
-             initial data, the object's __init__ parameters! Subsequent changes
-             affecting the key are not reflected in the multiton directory,
-             i.e. the directory may then be corrupted by such modifications.
-             Therefore, never change key related values of classified objects!
+    multiton ensures one single (unique) instance per key value of a
+    dictionary.
 
     Attributes
     ----------
-    substitute: object
-        A type to be made a multiton.
-
-    key: int or str or callable
-        Unique (immutable) key for the instance dictionary.
-
-    attrib: str
-        Name of the attribute containing the multiton instance.
+        None.
 
     Methods
     -------
     seal(self):
-        Seal multiton of unique key instances.
+        Seal multiton.
 
     unseal(self):
-        Unseal multiton of unique key instances.
+        Unseal multiton.
 
     issealed(self):
-        Is the multiton of unique key instances sealed?
+        Multiton sealing state
 
-    instances(self):
-        Dictionary of all instance representations.
+    get_instance():
+        Return the singleton instantce. (if accessible=True)
+
+    reset():
+        Resets the singleton instance.  (if resettable=True)
 
     Example
     -------
 
     from decoratory.multiton import Multiton
 
     # --- For alternative decorations see cases below!
-    @Multiton
+    @Multiton                       # Multiton(), Multiton(key=17), ...
     class Animal:
         def __init__(self, spec, name):
             self.spec = spec
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.spec}', '{self.name}')"
 
     # Create instances
     a = Animal('dog', name='Bello')
     b = Animal('cat', name='Mausi')
     c = Animal('dog', name='Tessa')
 
-    # Case 1: decoration @Multiton or @Multiton() or @Multiton(key=17) or ...
+    # Case 0: decoration @Multiton or @Multiton() or @Multiton(key=17) or ...
     #    ---> With no or fixed key the Multiton acts like a Singleton
-    print(a)                                # Animal('dog', 'Bello')
-    print(b)                                # Animal('dog', 'Bello')
-    print(c)                                # Animal('dog', 'Bello')
+    print(a)                        # Animal('dog', 'Bello')
+    print(b)                        # Animal('dog', 'Bello')
+    print(c)                        # Animal('dog', 'Bello')
+
+    # Case 1: decoration @Multiton(key=lambda spec, name: name)
+    #    ---> key is a function evaluating the attribute name from __init__(..)
+    print(a)                        # Animal('dog', 'Bello')
+    print(b)                        # Animal('cat', 'Mausi')
+    print(c)                        # Animal('dog', 'Tessa')
 
-    # Case 2: decoration Multiton(key=lambda spec, name: 'a' in name)
+    # Case 2: decoration @Multiton(key=lambda spec, name: 'a' in name)
     #    ---> key is a function evaluating the attribute name from __init__(..)
-    print(a)                                # Animal('dog', 'Bello')
-    print(b)                                # Animal('cat', 'Mausi')
-    print(c)                                # Animal('cat', 'Mausi')
-
-    # Case 3: decoration Multiton(key=0)    # take args[0]
-    #    ---> integer key=val references args[val] from __init__(.., spec,..)
-    print(a)                                # Animal('dog', 'Bello')
-    print(b)                                # Animal('cat', 'Mausi')
-    print(c)                                # Animal('dog', 'Bello')
-
-    # Case 4: decoration Multiton(key='0')  # take kwargs['0'] does not exist!
-    #    ---> string key=str references kwargs[str], here leading to None
-    print(a)                                # Animal('dog', 'Bello')
-    print(b)                                # Animal('dog', 'Bello')
-    print(c)                                # Animal('dog', 'Bello')
-
-    # Case 5: decoration Multiton(key='name') # take kwargs['name'] does exist!
-    #    ---> string key=str references kwargs[str] from __init__(..,.., name)
-    print(a)                                # Animal('dog', 'Bello')
-    print(b)                                # Animal('cat', 'Mausi')
-    print(c)                                # Animal('dog', 'Tessa')
-
-    # Case 6: decoration Multiton(key='name'): Seal after Bello
-    #    ---> string key=str references kwargs[str] (e.g. self.name)
-    Animal.instances().clear()              # Reset...
-    print(Animal.instances())               # ... to an empty dictionary
-    print(Animal.issealed())                # False
-    a = Animal('dog', name='Bello')         # Animal('dog', 'Bello')
-    Animal.seal()                           # seal it!
-    print(Animal.issealed())                # True
-    b = Animal('dog', name='Bello')         # Returns a-objekt from multiton
-    print(a is b)                           # True
+    print(a)                        # Animal('dog', 'Bello')
+    print(b)                        # Animal('cat', 'Mausi')
+    print(c)                        # Animal('cat', 'Mausi')
+
+    # Case 3: decoration @Multiton(key="{0}".format)
+    #    ---> Parameter spec is referenced as args[0] (positional)
+    print(a)                        # Animal('dog', 'Bello')
+    print(b)                        # Animal('cat', 'Mausi')
+    print(c)                        # Animal('dog', 'Bello')
+
+    # Case 4: decoration @Multiton(key="{name}".format)
+    #    ---> Parameter name is referenced as kwargs['name'] (keyword)
+    print(a)                        # Animal('dog', 'Bello')
+    print(b)                        # Animal('cat', 'Mausi')
+    print(c)                        # Animal('dog', 'Tessa')
+
+    # Case 5: decoration @Multiton(key=lambda spec, name: (spec, name))
+    #    ---> One unique instance for all init values, i.e. no duplicates
+    print(a)                        # Animal('dog', 'Bello')
+    print(b)                        # Animal('cat', 'Mausi')
+    print(c)                        # Animal('dog', 'Tessa')
+
+    # Case 6: decoration @Multiton(key=F("my_key"))
+    #    ---> Late binding with F(classmethod_string)
+    #         One unique instance from a @staticmethod or @classmethod
+    class Animal:
+        ...
+        @classmethod
+        def my_key(cls, spec, name):
+            return 'a' in name
+    print(a)                        # Animal('dog', 'Bello')
+    print(b)                        # Animal('cat', 'Mausi')
+    print(c)                        # Animal('cat', 'Mausi')
+
+    # Case 7: decoration @Multiton(key=lambda spec, name: name,
+    #                              accessible=True, resettable=True)
+    #    ---> Seal after Bello
+    Animal.reset()                  # Reset/Clear the instance dictionary
+    print(Animal.get_instances())   # {}
+    print(Animal.issealed())        # False
+    a = Animal('dog', name='Bello') # Animal('dog', 'Bello')
+    Animal.seal()                   # Seal it!
+    print(Animal.issealed())        # True
+    b = Animal('dog', name='Bello') # Returns primary instance
+    print(a is b)                   # True
     try:
-        c = Animal('dog', name='Tessa')     # KeyError, Animal is sealed!
-    except KeyError as ex:
+        c = Animal('dog', name='Tessa')
+    except KeyError as ex:          # KeyError, Animal is sealed!
         print(f"For '{ex.args[1]}' {ex.args[0]}")
-    print(Animal.instances())               # {'Bello': Animal('dog', 'Bello')}
-    Animal.unseal()                         # unseal it!
-    c = Animal('dog', name='Tessa')         # Animal('dog', 'Bello') now is ok!
-    print(Animal.instances())               # {'Bello': Animal('dog', 'Bello'),
-                                            #  'Tessa': Animal('dog', 'Tessa')}
-
-    # Case 7: Every instance knows its multiton
-    #    ---> By default object.multiton contains the multiton object
-    a = Animal('dog', name='Bello')         # Animal('dog', 'Bello')
-    print(a.multiton)                       # <decoratory.multiton.Multiton...>
-    print(a.multiton.instances())           # {'Bello': Animal('dog', 'Bello')}
-
-    # Case 8: Customize attribute name: Multiton(key='name', attrib='my_multi')
-    #    ---> Customized object.my_multi contains the multiton object
-    a = Animal('dog', name='Bello')         # Animal('dog', 'Bello')
-    print(a.my_multi)                       # <decoratory.multiton.Multiton...>
-    print(a.my_multi.instances())           # {'Bello': Animal('dog', 'Bello')}
-
-    # Case 9: decoration Multiton(key=lambda spec, name: 'a' in name)
-    #    ---> Warning: Corrupting the directory by changing the key!
-    a = Animal('dog', name='Bello')         # Animal('dog', 'Bello')
-    print(a.multiton.instances())           # {False: Animal('dog', 'Bello')}
-    a.name = 'Tessa'                        # Turns key from False to True, but
-    print(a.multiton.instances())           # {False: Animal('dog', 'Tessa')}
-                                            # only attribute self.name changed!
+    print(Animal.get_instances())   # {'Bello': Animal('dog', 'Bello')}
+    Animal.unseal()                 # Unseal it!
+    c = Animal('dog', name='Tessa') # Animal('dog', 'Bello') now it's ok!
+    print(Animal.get_instances())   # {'Bello': Animal('dog', 'Bello'),
+                                    #  'Tessa': Animal('dog', 'Tessa')}
 """
 
 # -----------------------------------------------------------------------------
 # Module Level Dunders
 __title__ = "Multiton"
 __module__ = "multiton.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.0.1"
-__date__ = "2023-06-12"
-__time__ = "14:49:52"
+__version__ = "0.1.0.5"
+__date__ = "2023-06-15"
+__time__ = "18:24:13"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Multiton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -174,242 +149,209 @@
 
 
 # -----------------------------------------------------------------------------
 # Classes
 class Multiton:
     """**Multiton**
 
-    A multiton is a design pattern that extends the singleton pattern.
+    A multiton pattern is a design pattern that extends the singleton pattern.
     Whereas the singleton allows for exactly one instance per class, the
-    multiton pattern ensures one single (unique) instance per key value
-    (of a dictionary).
-
-    In this implementation the key parameter can be either any immutable type
-    or a callable returning such an immutable type which can be used as a key
-    of a dictionary. In case of an invalid key, key is set None and the
-    multiton simply collapses to a singleton.
-
-    Setting the attrib parameter to a valid attribute name string the multiton
-    is attributed in the new instantiated substitute object, is the name
-    invalid, the attribute name 'multiton' is chosen.
-
-    By default, the sealed parameter is set False, so for every new key a new
-    (unique) object is instantiated. When sealed (e.g. later in the process)
-    is set True the dictionary has completed, i.e. restricted to the current
-    object set and any new key raises a KeyError.
-
-    Warning: Classifications into the multiton directory are done only once on
-             initial data, the object's __init__ parameters! Subsequent changes
-             affecting the key are not reflected in the multiton directory,
-             i.e. the directory may then be corrupted by such modifications.
-             Therefore, never change key related values of classified objects!
+    multiton ensures one single (unique) instance per key value of a
+    dictionary.
 
     Attributes
     ----------
-    substitute: object
-        A type to be made a multiton.
-
-    key: int or str or callable
-        Unique (immutable) key for the instance dictionary.
-
-    attrib: str
-        Name of the attribute containing the multiton instance.
+        None.
 
     Methods
     -------
     seal(self):
-        Seal multiton of unique key instances.
+        Seal multiton.
 
     unseal(self):
-        Unseal multiton of unique key instances.
+        Unseal multiton.
 
     issealed(self):
-        Is the multiton of unique key instances sealed?
+        Multiton sealing state
 
-    instances(self):
-        Dictionary of all instance representations.
+    get_instance():
+        Return the singleton instantce. (if accessible=True)
+
+    reset():
+        Resets the singleton instance.  (if resettable=True)
 
     Example
     -------
 
     from decoratory.multiton import Multiton
 
     # --- For alternative decorations see cases below!
-    @Multiton
+    @Multiton                       # Multiton(), Multiton(key=17), ...
     class Animal:
         def __init__(self, spec, name):
             self.spec = spec
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.spec}', '{self.name}')"
 
     # Create instances
     a = Animal('dog', name='Bello')
     b = Animal('cat', name='Mausi')
     c = Animal('dog', name='Tessa')
 
-    # Case 1: decoration @Multiton or @Multiton() or @Multiton(key=17) or ...
+    # Case 0: decoration @Multiton or @Multiton() or @Multiton(key=17) or ...
     #    ---> With no or fixed key the Multiton acts like a Singleton
-    print(a)                                # Animal('dog', 'Bello')
-    print(b)                                # Animal('dog', 'Bello')
-    print(c)                                # Animal('dog', 'Bello')
+    print(a)                        # Animal('dog', 'Bello')
+    print(b)                        # Animal('dog', 'Bello')
+    print(c)                        # Animal('dog', 'Bello')
+
+    # Case 1: decoration @Multiton(key=lambda spec, name: name)
+    #    ---> key is a function evaluating the attribute name from __init__(..)
+    print(a)                        # Animal('dog', 'Bello')
+    print(b)                        # Animal('cat', 'Mausi')
+    print(c)                        # Animal('dog', 'Tessa')
 
-    # Case 2: decoration Multiton(key=lambda spec, name: 'a' in name)
+    # Case 2: decoration @Multiton(key=lambda spec, name: 'a' in name)
     #    ---> key is a function evaluating the attribute name from __init__(..)
-    print(a)                                # Animal('dog', 'Bello')
-    print(b)                                # Animal('cat', 'Mausi')
-    print(c)                                # Animal('cat', 'Mausi')
-
-    # Case 3: decoration Multiton(key=0)    # take args[0]
-    #    ---> integer key=val references args[val] from __init__(.., spec,..)
-    print(a)                                # Animal('dog', 'Bello')
-    print(b)                                # Animal('cat', 'Mausi')
-    print(c)                                # Animal('dog', 'Bello')
-
-    # Case 4: decoration Multiton(key='0')  # take kwargs['0'] does not exist!
-    #    ---> string key=str references kwargs[str], here leading to None
-    print(a)                                # Animal('dog', 'Bello')
-    print(b)                                # Animal('dog', 'Bello')
-    print(c)                                # Animal('dog', 'Bello')
-
-    # Case 5: decoration Multiton(key='name') # take kwargs['name'] does exist!
-    #    ---> string key=str references kwargs[str] from __init__(..,.., name)
-    print(a)                                # Animal('dog', 'Bello')
-    print(b)                                # Animal('cat', 'Mausi')
-    print(c)                                # Animal('dog', 'Tessa')
-
-    # Case 6: decoration Multiton(key='name'): Seal after Bello
-    #    ---> string key=str references kwargs[str] (e.g. self.name)
-    Animal.instances().clear()              # Reset...
-    print(Animal.instances())               # ... to an empty dictionary
-    print(Animal.issealed())                # False
-    a = Animal('dog', name='Bello')         # Animal('dog', 'Bello')
-    Animal.seal()                           # seal it!
-    print(Animal.issealed())                # True
-    b = Animal('dog', name='Bello')         # Returns a-objekt from multiton
-    print(a is b)                           # True
+    print(a)                        # Animal('dog', 'Bello')
+    print(b)                        # Animal('cat', 'Mausi')
+    print(c)                        # Animal('cat', 'Mausi')
+
+    # Case 3: decoration @Multiton(key="{0}".format)
+    #    ---> Parameter spec is referenced as args[0] (positional)
+    print(a)                        # Animal('dog', 'Bello')
+    print(b)                        # Animal('cat', 'Mausi')
+    print(c)                        # Animal('dog', 'Bello')
+
+    # Case 4: decoration @Multiton(key="{name}".format)
+    #    ---> Parameter name is referenced as kwargs['name'] (keyword)
+    print(a)                        # Animal('dog', 'Bello')
+    print(b)                        # Animal('cat', 'Mausi')
+    print(c)                        # Animal('dog', 'Tessa')
+
+    # Case 5: decoration @Multiton(key=lambda spec, name: (spec, name))
+    #    ---> One unique instance for all init values, i.e. no duplicates
+    print(a)                        # Animal('dog', 'Bello')
+    print(b)                        # Animal('cat', 'Mausi')
+    print(c)                        # Animal('dog', 'Tessa')
+
+    # Case 6: decoration @Multiton(key=F("my_key"))
+    #    ---> Late binding with F(classmethod_string)
+    #         One unique instance from a @staticmethod or @classmethod
+    class Animal:
+        ...
+        @classmethod
+        def my_key(cls, spec, name):
+            return 'a' in name
+    print(a)                        # Animal('dog', 'Bello')
+    print(b)                        # Animal('cat', 'Mausi')
+    print(c)                        # Animal('cat', 'Mausi')
+
+    # Case 7: decoration @Multiton(key=lambda spec, name: name,
+    #                              accessible=True, resettable=True)
+    #    ---> Seal after Bello
+    Animal.reset()                  # Reset/Clear the instance dictionary
+    print(Animal.get_instances())   # {}
+    print(Animal.issealed())        # False
+    a = Animal('dog', name='Bello') # Animal('dog', 'Bello')
+    Animal.seal()                   # Seal it!
+    print(Animal.issealed())        # True
+    b = Animal('dog', name='Bello') # Returns primary instance
+    print(a is b)                   # True
     try:
-        c = Animal('dog', name='Tessa')     # KeyError, Animal is sealed!
-    except KeyError as ex:
+        c = Animal('dog', name='Tessa')
+    except KeyError as ex:          # KeyError, Animal is sealed!
         print(f"For '{ex.args[1]}' {ex.args[0]}")
-    print(Animal.instances())               # {'Bello': Animal('dog', 'Bello')}
-    Animal.unseal()                         # unseal it!
-    c = Animal('dog', name='Tessa')         # Animal('dog', 'Bello') now is ok!
-    print(Animal.instances())               # {'Bello': Animal('dog', 'Bello'),
-                                            #  'Tessa': Animal('dog', 'Tessa')}
-
-    # Case 7: Every instance knows its multiton
-    #    ---> By default object.multiton contains the multiton object
-    a = Animal('dog', name='Bello')         # Animal('dog', 'Bello')
-    print(a.multiton)                       # <decoratory.multiton.Multiton...>
-    print(a.multiton.instances())           # {'Bello': Animal('dog', 'Bello')}
-
-    # Case 8: Customize attribute name: Multiton(key='name', attrib='my_multi')
-    #    ---> Customized object.my_multi contains the multiton object
-    a = Animal('dog', name='Bello')         # Animal('dog', 'Bello')
-    print(a.my_multi)                       # <decoratory.multiton.Multiton...>
-    print(a.my_multi.instances())           # {'Bello': Animal('dog', 'Bello')}
-
-    # Case 9: decoration Multiton(key=lambda spec, name: 'a' in name)
-    #    ---> Warning: Corrupting the directory by changing the key!
-    a = Animal('dog', name='Bello')         # Animal('dog', 'Bello')
-    print(a.multiton.instances())           # {False: Animal('dog', 'Bello')}
-    a.name = 'Tessa'                        # Turns key from False to True, but
-    print(a.multiton.instances())           # {False: Animal('dog', 'Tessa')}
-                                            # only attribute self.name changed!
+    print(Animal.get_instances())   # {'Bello': Animal('dog', 'Bello')}
+    Animal.unseal()                 # Unseal it!
+    c = Animal('dog', name='Tessa') # Animal('dog', 'Bello') now it's ok!
+    print(Animal.get_instances())   # {'Bello': Animal('dog', 'Bello'),
+                                    #  'Tessa': Animal('dog', 'Tessa')}
     """
 
     def __init__(self,
                  substitute: type = None,
                  *args: object,
-                 key: Union[int, str, callable, None] = None,
-                 attrib: Union[str, None] = None,
+                 key: Union[F, callable, object, None] = None,
+                 accessible: bool = False,
+                 resettable: bool = False,
                  **kwargs: object) -> None:
         """Set up a multiton.
 
-        substitute is the first positional argument defining the type to be
-        decorated, in pie notation:  @Multiton class A <-> A = Multiton(A).
-
-        key is the first keyword argument and defines the dictionary key:
-         - key=int: references positional arguments args[int(key)]
-         - key=str: references keyword arguments kwargs[str(key)]
-         - key=callable: evaluates to an immutable object, e.g. str, tuple, ...
-
-        attrib is a string for renaming the multiton attribute name.
-
         Parameters:
-            substitute (object): A type to be made a multiton.
-            key: (int or str or callable): Unique (immutable) instance key.
-            attrib: str: Name of the attribute of the multiton instance.
+            substitute (object): A type to be made a multiton
+            key: (F|callable|object|None): Instance key.
+            accessible (bool): If True exposes a get_instance() method
+            resettable (bool): If True exposes a reset() method
 
         Returns:
             self (object): Multiton decorator instance
         """
         self.__set__substitute(substitute)
         self.__key = key
-        self.__attrib = attrib
 
-        self.__instances = dict()  # Dictionary for unique key instances
+        # Dictionary for unique key instances
+        self.__instances = dict()
+
+        # Sealing state
         self.__sealed = False
 
-        # Decorator Arguments Pattern
+        # If accessible == True exposes a get_instances() method
+        if bool(accessible):
+            def get_instances(s: object = self):
+                """Return dictionary of all instance representations."""
+                return s.__instances
+
+            # Add the instances method
+            setattr(self, 'get_instances', get_instances)
+
+        # If resettable == True exposes a reset() method
+        if bool(resettable):
+            def reset(s: object = self):
+                """Define reset method"""
+                s.__instances.clear()
+
+            # Add the reset method
+            setattr(self, 'reset', reset)
+
+        # --- Decorator Arguments Pattern (1/2)
         if self.__substitute is not None:
             # Decoration without parameter(s)
             self.__set__substitute(F(self.__substitute, *args, **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
 
-            # Add attribute
-            try:
-                setattr(self.__get__substitute().callee, self.__attrib, self)
-            except (TypeError, AttributeError, Exception):
-                setattr(self.__get__substitute().callee,
-                        self.__class__.__name__.lower(), self)
-
     def __call__(self, *args, **kwargs):
-        """Apply the decorator.
-
-        Parameters:
-            substitute (object): A type to be made a singleton.
-
-        Returns:
-            instance (object): A unique object instance from multiton key.
-        """
-        # Decorator Arguments Pattern
+        """Apply the decorator"""
+        # --- Decorator Arguments Pattern (2/2)
         if self.__substitute is None:
             # Decoration with parameter(s)
             self.__set__substitute(F(args[0], *args[1:], **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
-
-            # Add attribute
-            try:
-                setattr(self.__get__substitute().callee, self.__attrib, self)
-            except (TypeError, AttributeError, Exception):
-                setattr(self.__get__substitute().callee,
-                        self.__class__.__name__.lower(), self)
-
             return self
         else:  # *** Wrapper ***
             # If no current values, take defaults
             if args or kwargs:
                 subst = F(self.__get__substitute().callee, *args, **kwargs)
             else:
                 subst = self.__get__substitute()
 
             # Calculate key from callable or read key from arguments
             try:
-                if callable(self.__key):
-                    d_key = self.__key(*subst.callee_args,
-                                       **subst.callee_kwargs)
-                elif isinstance(self.__key, int):
-                    d_key = subst.callee_args[self.__key]
-                else:
-                    d_key = subst.callee_kwargs.get(self.__key, self.__key)
+                if isinstance(self.__key, F):  # classmethod or staticmethod
+                    d_key = F(
+                        getattr(self.substitute.callee, self.__key.callee),
+                        *subst.callee_args, **subst.callee_kwargs).eval()
+                elif callable(self.__key):  # function
+                    d_key = F(self.__key, *subst.callee_args,
+                              **subst.callee_kwargs).eval()
+                else:  # Value
+                    d_key = self.__key
                 instance = self.__instances.get(d_key, None)
-            except (IndexError, KeyError, TypeError, Exception):
+            except (TypeError, Exception):  # Default is None
                 d_key = None
                 instance = self.__instances.get(d_key, None)
 
             # Create and store new or return existing instance (by key)
             if instance is None:
                 if self.__sealed:
                     raise KeyError(f"{self.__name__} is sealed.", d_key)
@@ -424,57 +366,46 @@
     def __set__substitute(self, value):
         self.__substitute = value
 
     substitute = property(__get__substitute)
 
     # Methods
     def seal(self):
-        """Seal multiton of unique key instances.
+        """Seal multiton.
 
         Parameters:
             None.
 
         Returns:
             None.
         """
         self.__sealed = True
 
     def unseal(self):
-        """Unseal multiton of unique key instances.
+        """Unseal multiton .
 
         Parameters:
             None.
 
         Returns:
             None.
         """
         self.__sealed = False
 
     def issealed(self):
-        """Is the multiton of unique key instances sealed?
+        """Multiton sealing state
 
         Parameters:
             None.
 
         Returns:
-            True/False (bool): Seal state.
+            True/False (bool): Sealing state.
         """
         return self.__sealed
 
-    def instances(self):
-        """Dictionary of all instance representations.
-
-        Parameters:
-            None.
-
-        Returns:
-            Instance (dict): Dictionary of all multiton instances.
-        """
-        return self.__instances
-
 
 # -----------------------------------------------------------------------------
 # Entry Point
 if __name__ == '__main__':
     from decoratory.banner import __banner as banner
 
     banner(title=__title__,
```

### Comparing `decoratory-0.1.0.2/Sources/decoratory/observer.py` & `decoratory-0.1.0.3/Sources/decoratory/observer.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.0.2/Sources/decoratory/singleton.py` & `decoratory-0.1.0.3/Sources/decoratory/singleton.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 #!/usr/bin/env python
 # -*- coding=UTF-8 -*-
 # vim: fileencoding=UTF-8 tabstop=8 expandtab shiftwidth=4 softtabstop=4
 # -----------------------------------------------------------------------------
 # Document Description
 """**Singleton**
 
-    A singleton is a design pattern that limits the instantiation of a class
-    to a single (unique) instance. This is useful when exactly one unique
-    object is needed i.e. to manage/coordinate actions across modules.
+    A singleton pattern is a design pattern that limits the instantiation of a
+    class to a single (unique) instance. This is useful when exactly one
+    unique object is needed i.e. to manage an expensive resource or coordinate
+    actions across modules.
 
     Attributes
     ----------
-    substitute: object (get property)
-        A type to be made a singleton
-
-    instance: object (get property)
-        The unique singleton instance
+        None.
 
     Methods
     -------
-        None
+    get_instance():
+        Return the singleton instantce. (if accessible=True)
+
+    reset():
+        Resets the singleton instance.  (if resettable=True)
 
     Example
     -------
 
     from decoratory.singleton import Singleton
 
     @Singleton                      # or @Singleton()
@@ -34,44 +35,57 @@
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.name}')"
 
     # Create Instances
     a = Animal(name='Bello')        # Creates Bello
     b = Animal(name='Tessa')        # Returns Bello
 
-    # Case 1: Decoration @Singleton or @Singleton()
+    # Case 1: Static decoration using @Singleton or @Singleton()
     #    ---> One single object instance fits all.
     print(f"a = {a}")               # a = Animal('Bello')
     print(f"b = {b}")               # b = Animal('Bello')
     print(f"a is b: {a is b}")      # a is b: True
     print(f"a == b: {a == b}")      # a == b: True
 
-    # Case 2: Dynamic decoration of the native class with extra parameters.
+    # Case 2: Dynamic decoration providing extra initial default values
     #    ---> Initial default values provided via the decorator
     Animal = Singleton(Animal, 'Bello')
     Animal()                        # Using the decorator's default 'Bello'
-    Animal(name='Tessa')            # Returns Bello
-    print(Animal.instance)          # Animal('Bello')
+    a = Animal(name='Tessa')        # Returns Bello
+    print(a)                        # Animal('Bello')
+
+    # Case 3: Decoration using @Singleton(resettable=True)
+    print(Animal(name='Bello'))     # Animal('Bello')
+    print(Animal(name='Tessa'))     # Animal('Bello')   (=primary instance)
+    Animal.reset()                  # Reset the singleton
+    print(Animal(name='Tessa'))     # Animal('Tessa')
+    print(Animal(name='Bello'))     # Animal('Tessa')   (=primary instance)
+
+    # Case 4: Decoration using @Singleton(accessible=True)
+    a = Animal(name='Bello')        # Animal('Bello')
+    b = Animal.get_instance()       # Animal('Bello')   (=primary instance)
+    print(a)                        # Animal('Bello')
+    print(b)                        # Animal('Bello')
 """
 
 # -----------------------------------------------------------------------------
 # Module Level Dunders
 __title__ = "Singleton"
 __module__ = "singleton.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.0.1"
-__date__ = "2023-06-12"
-__time__ = "14:49:52"
+__version__ = "0.1.0.4"
+__date__ = "2023-06-15"
+__time__ = "18:24:13"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Singleton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -80,29 +94,27 @@
 
 
 # -----------------------------------------------------------------------------
 # Classes
 class Singleton:
     """**Singleton**
 
-    A singleton is a design pattern that limits the instantiation of a class
-    to a single (unique) instance. This is useful when exactly one unique
-    object is needed i.e. to manage/coordinate actions across modules.
+    A singleton pattern is a design pattern that limits the instantiation of a
+    class to a single (unique) instance. This is useful when exactly one
+    unique object is needed i.e. to manage an expensive resource or coordinate
+    actions across modules.
 
     Attributes
     ----------
-    substitute: object (get property)
-        A type to be made a singleton
-
-    instance: object (get property)
-        The unique singleton instance
+        None.
 
     Methods
     -------
-        None
+        get_instance(): Return the singleton instantce, (if accessible=True)
+        reset(): Resets the singleton instance.         (if resettable=True)
 
     Example
     -------
 
     from decoratory.singleton import Singleton
 
     @Singleton                      # or @Singleton()
@@ -113,61 +125,91 @@
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.name}')"
 
     # Create Instances
     a = Animal(name='Bello')        # Creates Bello
     b = Animal(name='Tessa')        # Returns Bello
 
-    # Case 1: Decoration @Singleton or @Singleton()
+    # Case 1: Static decoration using @Singleton or @Singleton()
     #    ---> One single object instance fits all.
     print(f"a = {a}")               # a = Animal('Bello')
     print(f"b = {b}")               # b = Animal('Bello')
     print(f"a is b: {a is b}")      # a is b: True
     print(f"a == b: {a == b}")      # a == b: True
 
-    # Case 2: Dynamic decoration of the native class with extra parameters.
+    # Case 2: Dynamic decoration providing extra initial default values
     #    ---> Initial default values provided via the decorator
     Animal = Singleton(Animal, 'Bello')
     Animal()                        # Using the decorator's default 'Bello'
-    Animal(name='Tessa')            # Returns Bello
-    print(Animal.instance)          # Animal('Bello')
+    a = Animal(name='Tessa')        # Returns Bello
+    print(a)                        # Animal('Bello')
+
+    # Case 3: Decoration using @Singleton(resettable=True)
+    print(Animal(name='Bello'))     # Animal('Bello')
+    print(Animal(name='Tessa'))     # Animal('Bello')   (=primary instance)
+    Animal.reset()                  # Reset the singleton
+    print(Animal(name='Tessa'))     # Animal('Tessa')
+    print(Animal(name='Bello'))     # Animal('Tessa')   (=primary instance)
+
+    # Case 4: Decoration using @Singleton(accessible=True)
+    a = Animal(name='Bello')        # Animal('Bello')
+    b = Animal.get_instance()       # Animal('Bello')   (=primary instance)
+    print(a)                        # Animal('Bello')
+    print(b)                        # Animal('Bello')
     """
 
     def __init__(self,
                  substitute: object = None,
                  *args: object,
+                 accessible: bool = False,
+                 resettable: bool = False,
                  **kwargs: object) -> None:
         """Set up a singleton.
 
         Parameters:
             substitute (object): A type to be made a singleton
+            accessible (bool): If True exposes a get_instance() method
+            resettable (bool): If True exposes a reset() method
 
         Returns:
             self (object): Singleton decorator instance
         """
         self.__set__substitute(substitute)
 
-        self.__instance = None  # The unique instance
+        # The unique instance
+        self.__instance = None
+
+        # If accessible == True exposes a get_instance() method
+        if bool(accessible):
+            def get_instance(s: object = self):
+                """Define get_instance method"""
+                return s.__instance
+
+            # Add the get_instance method
+            setattr(self, 'get_instance', get_instance)
+
+        # If resettable == True exposes a reset() method
+        if bool(resettable):
+            def reset(s: object = self):
+                """Define reset method"""
+                s.__instance = None
+
+            # Add the reset method
+            setattr(self, 'reset', reset)
 
-        # Decorator Arguments Pattern
+        # --- Decorator Arguments Pattern (1/2)
         if self.__substitute is not None:
             # Decoration without parameter(s)
             self.__set__substitute(F(self.__substitute, *args, **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
 
     def __call__(self, *args, **kwargs):
-        """Apply the decorator.
+        """Apply the decorator."""
 
-        Parameters:
-            substitute (object): A type to be made a singleton.
-
-        Returns:
-            instance (object): A unique object instance as a singleton.
-        """
-        # Decorator Arguments Pattern
+        # --- Decorator Arguments Pattern (2/2)
         if self.__substitute is None:
             # Decoration with parameter(s)
             self.__set__substitute(F(args[0], *args[1:], **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
             return self
         else:  # *** Wrapper ***
             # Create and store new or return existing instance
@@ -184,22 +226,14 @@
         return self.__substitute
 
     def __set__substitute(self, value):
         self.__substitute = value
 
     substitute = property(__get__substitute)
 
-    def __get__instance(self):
-        return self.__instance
-
-    def __set__instance(self, value):
-        self.self.__instance = value
-
-    instance = property(__get__instance)
-
 
 # -----------------------------------------------------------------------------
 # Entry Point
 if __name__ == '__main__':
     from decoratory.banner import __banner as banner
 
     banner(title=__title__,
```

### Comparing `decoratory-0.1.0.2/Sources/decoratory/wrapper.py` & `decoratory-0.1.0.3/Sources/decoratory/wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,43 +19,40 @@
     F-types (imported from module decoratory.basic, see below for details).
     In addition, replace supports passing results from successive replacement
     calls through an optional keyword argument named result (defaut value is
     None).
 
     Attributes
     ----------
-    substitute: object (getter)
+    substitute: object (getter property)
         A type to be made a multiton.
 
-    before: callable or list
+    before: callable or list (getter property)
         (List of) callable(s) to be executed before substitute.
 
-    replace: callable or list
+    replace: callable or list (getter property)
         (List of) callable(s) replacing the substitute.
 
-    after: callable or list
+    after: callable or list (getter property)
         (List of) callable(s) to be executed after substitute.
 
     Methods
     -------
         None.
 
     Example
     -------
 
     from decoratory.wrapper import Wrapper
     from decoratory.basic import F
 
-    # --- Overwrite default parameter values
-
     # Case 1: Dynamic decoration with decorator arguments, only
     def some_function(value: str = "original"):
         print(f"value = '{value}'")
 
-    # Function call with default parameters
     some_function()                 # value = 'original'
     some_function = Wrapper(some_function, value="changed")
     some_function()                 # value = 'changed'
 
     # Case 2: Static decoration with before and after functionalities
     def print_message(message: str = "ENTER"):
         print(message)
@@ -128,17 +125,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.0.2"
-__date__ = "2023-06-13"
-__time__ = "18:23:53"
+__version__ = "0.1.0.3"
+__date__ = "2023-06-15"
+__time__ = "18:24:13"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Wrapper"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -165,43 +162,40 @@
     F-types (imported from module decoratory.basic, see below for details).
     In addition, replace supports passing results from successive replacement
     calls through an optional keyword argument named result (defaut value is
     None).
 
     Attributes
     ----------
-    substitute: object (getter)
+    substitute: object (getter property)
         A type to be made a multiton.
 
-    before: callable or list
+    before: callable or list (getter property)
         (List of) callable(s) to be executed before substitute.
 
-    replace: callable or list
+    replace: callable or list (getter property)
         (List of) callable(s) replacing the substitute.
 
-    after: callable or list
+    after: callable or list (getter property)
         (List of) callable(s) to be executed after substitute.
 
     Methods
     -------
         None.
 
     Example
     -------
 
     from decoratory.wrapper import Wrapper
     from decoratory.basic import F
 
-    # --- Overwrite default parameter values
-
     # Case 1: Dynamic decoration with decorator arguments, only
     def some_function(value: str = "original"):
         print(f"value = '{value}'")
 
-    # Function call with default parameters
     some_function()                 # value = 'original'
     some_function = Wrapper(some_function, value="changed")
     some_function()                 # value = 'changed'
 
     # Case 2: Static decoration with before and after functionalities
     def print_message(message: str = "ENTER"):
         print(message)
@@ -269,17 +263,15 @@
     def __init__(self,
                  substitute: callable or type = None,
                  *args: object,
                  before: callable or list = None,
                  replace: callable or list = None,
                  after: callable or list = None,
                  **kwargs: object) -> None:
-        """
-        substitute is the first positional argument defining the type to be
-        decorated, in pie notation:  @Wrapper class A <-> A = Wrapper(A).
+        """Set up a wrapper.
 
         Parameters:
             substitute (object): A type to be made a wrapper.
             before (object): (List of) callable(s) to be executed before
             replace (object): (List of) callable(s) replacing the substitute
             after (object): (List of) callable(s) to be executed after
 
@@ -287,22 +279,22 @@
             self (object): Wrapper decorator instance
         """
         self.__set__substitute(substitute)
         self.__set__before(before)
         self.__set__replace(replace)
         self.__set__after(after)
 
-        # Decorator Arguments Pattern
+        # --- Decorator Arguments Pattern (1/2)
         if self.__substitute is not None:
             # Decoration without parameter(s)
             self.__set__substitute(F(self.__substitute, *args, **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
 
     def __call__(self, *args, **kwargs):
-        # Decorator Arguments Pattern
+        # --- Decorator Arguments Pattern (2/2)
         if self.__substitute is None:
             # Decoration with parameter(s)
             self.__set__substitute(F(args[0], *args[1:], **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
             return self
         else:  # *** Wrapper ***
             # Action BEFORE
```

### Comparing `decoratory-0.1.0.2/Sources/decoratory.egg-info/PKG-INFO` & `decoratory-0.1.0.3/Sources/decoratory.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.1.0.2
-Summary: Decorators: Singleton, Multiton, Observer, generic Wrapper.
+Version: 0.1.0.3
+Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
 Home-page: http://evation.eu
 Download-URL: http://evation.eu
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
 License: PSF
@@ -43,15 +43,15 @@
 ==============================================================================
 Decoratory
 ==============================================================================
 
 
 **Introduction**
 
-The "decoratory" package is based on the `Decorator Arguments Pattern`_, an 
+The *decoratory package* is based on the `Decorator Arguments Pattern`_, an 
 integrated concept for Python decorators with and without parameters. In
 addition, all decorators created with it support complex arguments, e.g. 
 lists of values and functions, without unnecessarily complicating the 
 decoration of simple cases by these extensions. All implementation details 
 are described on the `project homepage`_.
 
 
@@ -60,18 +60,19 @@
     pip install --upgrade decoratory
 
 After installation, basic information about the package, the individual 
 modules and their methods is also available from the command line. ::
 
     python -m decoratory --help
 
+.. _toc:
 
-**Package Content**
+**Package Contents**
 
-The decoratory package available here includes some classic decorators
+The *decoratory package* available here includes some classic decorators
 implemented and functionally extended with this concept, e.g.
 
 * `Singleton`_
 * `Multiton`_
 * `Wrapper`_
 * `Observer`_   (coming soon...)
 
@@ -117,50 +118,107 @@
 
     # Create Instances
     a = Animal(name='Bello')        # Creates Bello
     b = Animal(name='Tessa')        # Returns Bello
 
 If instances of the class ``Animal`` are now created, this is only done for the 
 very first instantiation, and for all further instantiations always this 
-"primary instance" is given back.
+*primary instance* is given back.
             
 .. code-block:: python
 
     # *** example_singleton.py - verfication of the unique instance
 
     # Case 1: Static decoration using @Singleton or @Singleton()
     print(f"a = {a}")               # a = Animal('Bello')
     print(f"b = {b}")               # b = Animal('Bello')
     print(f"a is b: {a is b}")      # a is b: True
     print(f"a == b: {a == b}")      # a == b: True
 
-If instead of the above "static decoration" using pie-notation, i.e. with 
-@-notation at the class declaration, the "dynamic decoration" within Python 
+If instead of the above *static decoration* using pie-notation, i.e. with 
+@-notation at the class declaration, the *dynamic decoration* within Python 
 code is used, additional parameters can be passed to the decorator for 
 passing to the class constructor.
 
 .. code-block:: python
 
     # *** example_singleton.py - dynamic decoration with extra parameters
 
     # Case 2: Dynamic decoration providing extra initial default values 
     Animal = Singleton(Animal, 'Bello')
     Animal()                        # Using the decorator's default 'Bello'
-    Animal(name='Tessa')            # Returns Bello
-    print(Animal.instance)          # Animal('Bello')
+    a = Animal(name='Tessa')        # Returns Bello
+    print(a)                        # Animal('Bello')
 
 Quite generally, for all the following decorators based on this 
 `Decorator Arguments Pattern`_, these two properties are always fulfilled:
 
-.. note::
+#. Decoration as a class (without parentheses) and Decoration as an instance 
+   (with empty parentheses) are equivalent
+#. For dynamic decoration, extra parameters can be passed, e.g. for the 
+   class constructor
+
+So far, this singleton implementation follows the concept of *once and 
+forever*, i.e. whenever a new instance of a class is created, one always
+gets the *primary instance* back - without any possibility of ever changing 
+it again.
+
+Although this behavior is consistent with the basic concept of a singleton, 
+there are situations where it might be useful to reset a *singleton*. Such 
+a *resettable singleton* could be useful to express in code that an instance 
+is often retrieved but rarely changed.
+
+.. code-block:: python
+
+    # *** example_singleton.py - decoration as 'resettable singleton'
+
+    from decoratory.singleton import Singleton
+
+    @Singleton(resettable=True)     # Exposes an additional reset method 
+    class Animal:
+        def __init__(self, name):
+            self.name = name
+
+        def __repr__(self):
+            return f"{self.__class__.__name__}('{self.name}')"
+
+    # Case 3: Decoration using @Singleton(resettable=True)
+    print(Animal(name='Bello'))     # Animal('Bello')
+    print(Animal(name='Tessa'))     # Animal('Bello')   (=primary instance)
+    Animal.reset()                  # Reset the singleton
+    print(Animal(name='Tessa'))     # Animal('Tessa')
+    print(Animal(name='Bello'))     # Animal('Tessa')   (=primary instance)
+
+Without ``resettable=True`` decoration ``Animal`` has no ``reset`` method and 
+the call ``Animal.reset()`` will fail raising an ``AttributeError``.
+
+With the same intention, the retrieval of the *primary instance* is also 
+locked by default, but can be unlocked during decoration with the 
+``accessible=True`` parameter, which allows ``Animal`` to expose the 
+``get_instance()`` method.
+
+.. code-block:: python
+
+    # *** example_singleton.py - decoration as 'accessible singleton'
+
+    from decoratory.singleton import Singleton
+
+    @Singleton(accessible=True)     # Exposes a get_instance method 
+    class Animal:
+        def __init__(self, name):
+            self.name = name
 
-    * Decoration as a class (without parentheses) and Decoration as an instance 
-      (with empty parentheses) are equivalent
-    * For dynamic decoration, extra parameters can be passed, e.g. for the 
-      class constructor
+        def __repr__(self):
+            return f"{self.__class__.__name__}('{self.name}')"
+
+    # Case 4: Decoration using @Singleton(accessible=True)
+    a = Animal(name='Bello')        # Animal('Bello')
+    b = Animal.get_instance()       # Animal('Bello')   (=primary instance)
+    print(a)                        # Animal('Bello')
+    print(b)                        # Animal('Bello')
 
 
 ******************************************************************************
 Multiton
 ******************************************************************************
 
 A `multiton pattern`_ is a design pattern that extends the singleton pattern.
@@ -168,28 +226,29 @@
 ensures one single (unique) *instance per key value of a dictionary*.
 
 In this implementation the key parameter can be either any immutable type
 or a callable returning such an immutable type which can be used as a key
 of a dictionary. In case of an invalid key, key is set ``None`` and with only 
 one key value the multiton simply collapses to a singleton, therefore the 
 decoration ``@Multiton`` resp. ``@Multiton()`` or even ``@Multiton(key=17)`` 
-or  ``@Multiton(key='some fixed value')`` and so on always creates a singleton.
+or  ``@Multiton(key='some constant value')`` and so on always creates a 
+singleton.
 
-Usually the key is independent of the classified object. However, it is not 
-uncommon for it to be part of the classified object itself, as in the 
-following example, where the key string matches the parameter ``name`` of 
-the constructor of the class ``Animal``.
+Normally, the key is part of or is composed from the initial values of the 
+classified object, as in the following example, where the key function matches 
+the signature of the constructor and uses the initial value of the ``name`` 
+parameter to construct a key value for the instances of ``Animal``.
 
 .. code-block:: python
    
     # *** example_multitonton.py - class Animal with Multiton decoration
 
     from decoratory.multiton import Multiton
 
-    @Multiton(key='name')           # uses kwargs['name'] as key
+    @Multiton(key=lambda spec, name: name)
     class Animal:
         def __init__(self, spec, name):
             self.spec = spec
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.spec}', '{self.name}')"
@@ -197,72 +256,105 @@
     # Create Instances
     a = Animal('dog', name='Bello')
     b = Animal('cat', name='Mausi')
     c = Animal('dog', name='Tessa')
 
 When instances of the class ``Animal`` are now created, this only happens for 
 the *first instantiation per key value*, the initial name of the animal. For 
-all subsequent instantiations, this "primary instance per key value" is 
+all subsequent instantiations, this *primary instance per key value* is 
 returned. But for each new key value, a new ``Animal`` instance is created 
 and stored in the internal directory.
 
 .. code-block:: python
 
     # *** example_multitonton.py - One unique instance per name
 
-    # Case 1: key='name' references kwargs['name'] from __init__(..,name)
+    # Case 1: decoration @Multiton(key=lambda spec, name: name)
     print(a)                        # Animal('dog', 'Bello')
     print(b)                        # Animal('cat', 'Mausi')
     print(c)                        # Animal('dog', 'Tessa')
 
 With three different names, a separate instance is created in each case. 
 In contrast, the following variant distinguishes only two types (equivalence 
 classes): animals with a character 'a' in their name and those without and 
 thus the key values can only be ``True`` or ``False``.
 
 .. code-block:: python
 
     # *** example_multitonton.py - One unique instance per equivalence class
 
-    # Case 2: with decoration @Multiton(key=lambda spec, name: 'a' in name)
-    print(a)                        # Animal('dog', 'Bello'), key=False
-    print(b)                        # Animal('cat', 'Mausi'), key=True
-    print(c)                        # Animal('cat', 'Mausi'), key=True
+    # Case 2: decoration @Multiton(key=lambda spec, name: 'a' in name)
+    print(a)                        # Animal('dog', 'Bello')
+    print(b)                        # Animal('cat', 'Mausi')
+    print(c)                        # Animal('cat', 'Mausi')
+
+The initial parameter values of the constructor can also be accessed by their 
+``args``-index or ``kwargs``-name. So the following decorations are also 
+possible:
+
+.. code-block:: python
+
+    # *** example_multitonton.py - Alternative decoration examples
+
+    # Case 3: One unique instance per specie
+    @Multiton(key="{0}".format)     # spec is args[0]
+    class Animal:
+        ...
 
+    # Case 4: One unique instance per name
+    @Multiton(key="{name}".format)  # name is kwargs['name']
+    class Animal:
+        ...
+
+    # Case 5: One unique instance for all init values, i.e. no duplicates
+    @Multiton(key=lambda spec, name: (spec, name))
+    class Animal:
+        ...
+
+    # Case 6: One unique instance from a @staticmethod or @classmethod
+    @Multiton(key=F("my_key"))      # Late binding with F(classmethod_string)
+    class Animal:
+        ...
+
+        @classmethod
+        def my_key(cls, spec, name):
+            return 'a' in name
+        
 To actively control access to new equivalence classes, ``Multiton`` provides 
 the ``seal()``, ``unseal()``, and ``issealed()`` methods for sealing, unsealing,
-and checking the sealing state of the ``Multiton``. By default, the sealed 
+and checking the sealing state of the ``Multiton``. By default, the sealing 
 state is set ``False``, so for every new key a new (unique) object is 
 instantiated. When sealed (e.g. later in the process) is set ``True`` the 
 dictionary has completed, i.e. restricted to the current object set and 
 any new key raises a ``KeyError``.
 
 For deeper, special requirements on the equivalence classes of a multiton 
-then by means of the method ``instances()`` the internal directory can also 
-be actively manipulated, which of course should be done with caution and 
-generally is not recommended. 
-
-For this reason, each object knows its multiton: Setting ``Multiton``'s ``attrib`` 
-parameter while decoration to a valid attribute name string the multiton is 
-attributed in the new instantiated substitute object, is the chosen name 
-invalid or missing, the default attribute name ``multiton`` is chosen. 
+by setting the decorator parameter ``accessible=True``, the method 
+``get_instances()`` is enabled, which grants direct access to the internal 
+directory of the instances. This can be actively manipulated in this way, 
+which of course should be done with care and is generally not recommended.  
 
 .. code-block:: python
 
-    # *** example_multitonton.py - One unique instance per equivalence class
-
-    # Case 3: with decoration @Multiton(key=lambda spec, name: 'a' in name)
-    print(a)                        # Animal('dog', 'Bello')
-    print(a.multiton)               # <decoratory.multiton.Multiton object..>
-    print(a.multiton.instances())   # {False: Animal('dog', 'Bello'), 
-                                    #   True: Animal('cat', 'Mausi')}
-
-Thus, in the above example, ``a.multiton`` would be the multiton of ``a`` 
-('Bello') and ``a.multiton.instances()`` would be the directory of equivalence 
-classes to which it belongs.
+    # *** example_multitonton.py - Accessibility to the internal directory
+
+    # Case 7: with decoration @Multiton(key=lambda spec, name: 'a' in name,
+    #                                   accessible=True)
+    print(Animal.get_instances())   # {}
+    a = Animal('dog', name='Bello') # 
+    print(Animal.get_instances())   # {False: Animal('dog', 'Bello')}
+    b = Animal('cat', name='Mausi') # 
+    c = Animal('dog', name='Tessa') # 
+    print(Animal.get_instances())   # {False: Animal('dog', 'Bello'),  
+                                    #  True:  Animal('cat', 'Mausi')}
+
+In situations where it might be useful to reset the multiton to express in 
+code that instances are often retrieved but rarely modified, setting the 
+decorator parameter ``resettable=True`` will expose the ``reset()`` method, 
+by means of which the internal directory of instances can be completely cleared.
 
 .. warning::
  
     Classifications into the multiton directory are done only once on
     initial key data. Subsequent changes affecting a key value are not 
     reflected in the multiton directory, i.e. the directory may then be 
     corrupted by such modifications.
@@ -291,16 +383,16 @@
 ``before``, ``after`` and ``replace``, can be combined with each other and 
 support both single callables and (nested) lists of ``F``-types 
 (imported from module decoratory.basic, see below for details). 
 In addition, ``replace`` supports passing results from successive 
 replacement calls through an optional keyword argument named ``result`` 
 (defaut value is ``None``).
 
-Even without any of these arguments, such a "do nothing wrapper" can be used 
-to "overwrite" default values, for example.
+Even without any of these arguments, such a *do nothing wrapper* can be used 
+to *overwrite* default values, for example.
 
 .. code-block:: python
 
     # *** example_wrapper.py - overwrite default parameter values
 
     from decoratory.wrapper import Wrapper
 
@@ -411,15 +503,15 @@
 .. note::
 
     Decorations to ``@staticmethod`` or ``@classmethod`` can be done 
     analogously to the function decorations above, since they already exist 
     at compile time. Instance methods, on the other hand, do not exist until 
     an object instance is created and must be handled differently.
 
-With ``Wrapper`` and custom service functions, a "private wrapper library" 
+With ``Wrapper`` and custom service functions, a *private wrapper library* 
 can be built and reused.
 
 .. code-block:: python
 
     # *** example_wrapper.py - private wrapper library
 
     from decoratory.wrapper import Wrapper
@@ -447,24 +539,27 @@
 coming soon...
 
 
 ******************************************************************************
 Version History
 ******************************************************************************
 
+**Version: 0.1.0.3, Build: 2023-06-15**
+    
+- accessible parameter for singleton and multiton, incl. documentation
+- resettable parameter for singleton and multiton, incl. documentation
+
 **Version: 0.1.0.2, Build: 2023-06-13**
 
-- Documentation enhancements
+- Documentation enhancements for for singleton, multiton and wrapper
 
 **Version: 0.1.0.1, Build: 2023-06-12**
 
 - Initial version with Singleton, Multiton and Wrapper
 
 
 .. ===========================================================================
 .. _project homepage: http://evation.eu
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _Decorator Arguments Pattern: http://evation.eu
 
-`back to top <#top>`_
-
```

### Comparing `decoratory-0.1.0.2/setup.py` & `decoratory-0.1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.0.2"
-__date__ = "2023-06-13"
-__time__ = "18:28:13"
+__version__ = "0.1.0.3"
+__date__ = "2023-06-15"
+__time__ = "18:35:51"
 __state__ = "Beta"
 __license__ = "PSF"
 
 # -----------------------------------------------------------------------------
 # Libraries
 from os.path import join
 from setuptools import setup, find_packages
@@ -37,14 +37,15 @@
 
 with open("Requirements.txt", "r") as f:
     requirements = [str(req) for req in f.read().splitlines() if req]
 
 
 def version_check():
     """Keep versions in sync"""
+    # noinspection PyProtectedMember
     from Sources.decoratory.__main__ import __version__ as version
     assert version == __version__, (
         f"\n\n{'':=^79s}\n"
         f"{' Version mismatch: __main__.version != setup.version ':=^79s}\n"
         f"{'':=^79s}")
 
 
@@ -56,15 +57,16 @@
     version=__version__,
     author=__author__,
     author_email=f'{__author__} <{__email__}>',
     maintainer=f'{__author__}',
     maintainer_email=f'{__author__} <{__email__}>',
     url=__url__,
     download_url=__url__,
-    description='Decorators: Singleton, Multiton, Observer, generic Wrapper.',
+    description=('Decorators: Singleton, Multiton, Observer, Observable, '
+                 'generic Wrapper.'),
     long_description=description,
     long_description_content_type='text/x-rst',
     project_urls={
         'Projekt': __url__,
         'Release Notes': __url__,
         'Download': __url__},
     keywords='decorator singleton multiton observer observable wrapper',
```

