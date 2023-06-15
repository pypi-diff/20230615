# Comparing `tmp/python-lorem-1.3.0.post1.tar.gz` & `tmp/python-lorem-1.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-lorem-1.3.0.post1.tar", last modified: Thu Jun 15 09:28:38 2023, max compression
+gzip compressed data, was "python-lorem-1.3.0rc1.tar", last modified: Sun Apr 23 06:32:02 2023, max compression
```

## Comparing `python-lorem-1.3.0.post1.tar` & `python-lorem-1.3.0rc1.tar`

### file list

```diff
@@ -1,21 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:28:38.114512 python-lorem-1.3.0.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-15 09:28:20.000000 python-lorem-1.3.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-15 09:28:20.000000 python-lorem-1.3.0.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-15 09:28:38.114512 python-lorem-1.3.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-15 09:28:20.000000 python-lorem-1.3.0.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-06-15 09:28:20.000000 python-lorem-1.3.0.post1/lorem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-15 09:28:20.000000 python-lorem-1.3.0.post1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:28:38.110512 python-lorem-1.3.0.post1/python_lorem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-15 09:28:38.000000 python-lorem-1.3.0.post1/python_lorem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-15 09:28:38.000000 python-lorem-1.3.0.post1/python_lorem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:28:38.000000 python-lorem-1.3.0.post1/python_lorem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-15 09:28:38.000000 python-lorem-1.3.0.post1/python_lorem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 09:28:38.000000 python-lorem-1.3.0.post1/python_lorem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:28:37.000000 python-lorem-1.3.0.post1/python_lorem.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-15 09:28:38.114512 python-lorem-1.3.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-15 09:28:20.000000 python-lorem-1.3.0.post1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-15 09:28:20.000000 python-lorem-1.3.0.post1/test_lorem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:28:38.114512 python-lorem-1.3.0.post1/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-15 09:28:20.000000 python-lorem-1.3.0.post1/util/bump_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-15 09:28:20.000000 python-lorem-1.3.0.post1/util/conda-build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-15 09:28:20.000000 python-lorem-1.3.0.post1/util/wheel_rename.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:32:02.891667 python-lorem-1.3.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-23 06:31:49.000000 python-lorem-1.3.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-23 06:31:49.000000 python-lorem-1.3.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-23 06:32:02.891667 python-lorem-1.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-23 06:31:49.000000 python-lorem-1.3.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17541 2023-04-23 06:31:49.000000 python-lorem-1.3.0rc1/lorem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-23 06:31:49.000000 python-lorem-1.3.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:32:02.891667 python-lorem-1.3.0rc1/python_lorem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-23 06:32:02.000000 python-lorem-1.3.0rc1/python_lorem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-23 06:32:02.000000 python-lorem-1.3.0rc1/python_lorem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 06:32:02.000000 python-lorem-1.3.0rc1/python_lorem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-23 06:32:02.000000 python-lorem-1.3.0rc1/python_lorem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 06:32:02.000000 python-lorem-1.3.0rc1/python_lorem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 06:32:02.000000 python-lorem-1.3.0rc1/python_lorem.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-23 06:32:02.891667 python-lorem-1.3.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-04-23 06:31:49.000000 python-lorem-1.3.0rc1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-23 06:31:49.000000 python-lorem-1.3.0rc1/test_lorem.py
```

### Comparing `python-lorem-1.3.0.post1/LICENSE` & `python-lorem-1.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-lorem-1.3.0.post1/PKG-INFO` & `python-lorem-1.3.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lorem
-Version: 1.3.0.post1
+Version: 1.3.0rc1
 Summary: Lorem ipsum generator.
 Author-email: Jarry Shaw <jarryshaw@icloud.com>
 Maintainer: Jarry Shaw
 License: BSD 3-Clause License
 Project-URL: homepage, https://jarryshaw.github.io/lorem/
 Project-URL: documentation, https://jarryshaw.github.io/lorem/
 Project-URL: repository, https://github.com/JarryShaw/lorem
```

### Comparing `python-lorem-1.3.0.post1/README.md` & `python-lorem-1.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `python-lorem-1.3.0.post1/lorem.py` & `python-lorem-1.3.0rc1/lorem.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 __all__ = [
     'LoremGenerator',
     'word', 'sentence', 'paragraph',
     'get_word', 'get_sentence', 'get_paragraph',
 ]
 
 # version string
-__version__ = '1.3.0.post1'
+__version__ = '1.3.0rc1'
 
 #: The original lorem ipsum text pool.
 _TEXT = ('ad', 'adipiscing', 'aliqua', 'aliquip', 'amet', 'anim', 'aute', 'cillum', 'commodo',
          'consectetur', 'consequat', 'culpa', 'cupidatat', 'deserunt', 'do', 'dolor', 'dolore',
          'duis', 'ea', 'eiusmod', 'elit', 'enim', 'esse', 'est', 'et', 'eu', 'ex', 'excepteur',
          'exercitation', 'fugiat', 'id', 'in', 'incididunt', 'ipsum', 'irure', 'labore', 'laboris',
          'laborum', 'lorem', 'magna', 'minim', 'mollit', 'nisi', 'non', 'nostrud', 'nulla',
```

### Comparing `python-lorem-1.3.0.post1/pyproject.toml` & `python-lorem-1.3.0rc1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 [build-system]
 requires = [
     "setuptools>=61.0.0",
-
-    # PyBPC
-    #"bpc-f2format; python_version < '3.6'",
-    #"bpc-poseur; python_version < '3.8'",
-    #"bpc-walrus; python_version < '3.8'",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-lorem"
 dynamic = [ "version", "readme" ]
 authors = [
@@ -36,19 +31,14 @@
     'Programming Language :: Python :: 3 :: Only',
     'Topic :: Software Development',
     'Topic :: Utilities',
     'Typing :: Typed',
 ]
 dependencies = [
     "typing-extensions; python_version < '3.8'",
-
-    # PyBPC
-    #"bpc-f2format; python_version < '3.6'",
-    #"bpc-poseur; python_version < '3.8'",
-    #"bpc-walrus; python_version < '3.8'",
 ]
 
 [project.urls]
 homepage = "https://jarryshaw.github.io/lorem/"
 documentation = "https://jarryshaw.github.io/lorem/"
 repository = "https://github.com/JarryShaw/lorem"
 changelog = "https://github.com/JarryShaw/lorem/releases"
```

### Comparing `python-lorem-1.3.0.post1/python_lorem.egg-info/PKG-INFO` & `python-lorem-1.3.0rc1/python_lorem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lorem
-Version: 1.3.0.post1
+Version: 1.3.0rc1
 Summary: Lorem ipsum generator.
 Author-email: Jarry Shaw <jarryshaw@icloud.com>
 Maintainer: Jarry Shaw
 License: BSD 3-Clause License
 Project-URL: homepage, https://jarryshaw.github.io/lorem/
 Project-URL: documentation, https://jarryshaw.github.io/lorem/
 Project-URL: repository, https://github.com/JarryShaw/lorem
```

### Comparing `python-lorem-1.3.0.post1/setup.py` & `python-lorem-1.3.0rc1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -68,16 +68,14 @@
 2. `get_paragraph` -- return random paragraphs
 
    ```python
    get_paragraph(count=1, comma=(0, 2), word_range=(4, 8), sentence_range=(5, 10), sep=os.linesep) -> Union[str]
    ```
 
 """
-import logging
-#import os
 import sys
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Any
 
 if sys.version_info[0] <= 2:
@@ -88,123 +86,92 @@
     from setuptools.command.build_py import build_py
     from setuptools.command.develop import develop
     from setuptools.command.install import install
     from setuptools.command.sdist import sdist
 except:
     raise ImportError("setuptools is required to install python-lorem!")
 
-try:
-    from wheel.bdist_wheel import bdist_wheel
-except ImportError:
-    bdist_wheel = None
-
-# get logger
-logger = logging.getLogger('lorem.setup')
-formatter = logging.Formatter(fmt='[%(levelname)s] %(asctime)s - %(message)s',
-                              datefmt='%m/%d/%Y %I:%M:%S %p')
-handler = logging.StreamHandler(sys.stderr)
-handler.setFormatter(formatter)
-logger.addHandler(handler)
-
 
 def refactor(path: 'str') -> 'None':
     """Refactor code."""
     import subprocess  # nosec: B404
 
     if sys.version_info < (3, 6):
         try:
             subprocess.check_call(  # nosec
                 [sys.executable, '-m', 'f2format', '--no-archive', path]
             )
         except subprocess.CalledProcessError as error:
-            logger.error('Failed to perform assignment expression backport compiling. '
-                         'Please consider manually install `bpc-f2format` and try again.')
+            print('Failed to perform assignment expression backport compiling.'
+                  'Please consider manually install `bpc-f2format` and try again.', file=sys.stderr)
             sys.exit(error.returncode)
 
     if sys.version_info < (3, 8):
         try:
             subprocess.check_call(  # nosec
                 [sys.executable, '-m', 'walrus', '--no-archive', path]
             )
         except subprocess.CalledProcessError as error:
-            logger.error('Failed to perform assignment expression backport compiling. '
-                         'Please consider manually install `bpc-walrus` and try again.')
+            print('Failed to perform assignment expression backport compiling.'
+                  'Please consider manually install `bpc-walrus` and try again.', file=sys.stderr)
             sys.exit(error.returncode)
 
         try:
             subprocess.check_call(  # nosec
                 [sys.executable, '-m', 'poseur', '--no-archive', path]
             )
         except subprocess.CalledProcessError as error:
-            logger.error('Failed to perform assignment expression backport compiling. '
-                         'Please consider manually install `bpc-poseur` and try again.')
+            print('Failed to perform assignment expression backport compiling.'
+                  'Please consider manually install `bpc-poseur` and try again.', file=sys.stderr)
             sys.exit(error.returncode)
 
 
 class lorem_sdist(sdist):
     """Modified sdist to run PyBPC conversion."""
 
     def make_release_tree(self, base_dir: 'str', *args: 'Any', **kwargs: 'Any') -> 'None':
         super(lorem_sdist, self).make_release_tree(base_dir, *args, **kwargs)
-        logger.info('running sdist')
 
         # PyBPC compatibility enforcement
         #refactor(os.path.join(base_dir, 'lorem'))
 
 
 class lorem_build_py(build_py):
     """Modified build_py to run PyBPC conversion."""
 
     def build_package_data(self) -> 'None':
         super(lorem_build_py, self).build_package_data()
-        logger.info('running build_py')
 
         # PyBPC compatibility enforcement
         #refactor(os.path.join(self.build_lib, 'lorem'))
 
 
 class lorem_develop(develop):
     """Modified develop to run PyBPC conversion."""
 
     def run(self) -> 'None':  # type: ignore[override]
         super(lorem_develop, self).run()
-        logger.info('running develop')
 
         # PyBPC compatibility enforcement
         #refactor(os.path.join(self.install_lib, 'lorem'))
 
 
 class lorem_install(install):
     """Modified install to run PyBPC conversion."""
 
     def run(self) -> 'None':
         super(lorem_install, self).run()
-        logger.info('running install')
 
         # PyBPC compatibility enforcement
         #refactor(os.path.join(self.install_lib, 'lorem'))  # type: ignore[arg-type]
 
 
-if bdist_wheel is not None:
-    class lorem_bdist_wheel(bdist_wheel):
-        """Modified bdist_wheel to run PyBPC conversion."""
-
-        def run(self) -> 'None':
-            super(lorem_bdist_wheel, self).run()
-            logger.info('running bdist_wheel')
-
-            # PyBPC compatibility enforcement
-            #refactor(os.path.join(self.dist_dir, 'lorem'))
-else:
-    lorem_bdist_wheel = None  # type: ignore[misc,assignment]
-
 setup(
     cmdclass={
         'sdist': lorem_sdist,
         'build_py': lorem_build_py,
         'develop': lorem_develop,
         'install': lorem_install,
-        'bdist_wheel': lorem_bdist_wheel,
     },
     long_description=__doc__,
     long_description_content_type='text/markdown',
 )
```

### Comparing `python-lorem-1.3.0.post1/test_lorem.py` & `python-lorem-1.3.0rc1/test_lorem.py`

 * *Files identical despite different names*

