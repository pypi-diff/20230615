# Comparing `tmp/xdev-1.2.0.tar.gz` & `tmp/xdev-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdev-1.2.0.tar", last modified: Wed Apr  5 14:56:52 2023, max compression
+gzip compressed data, was "xdev-1.3.3.tar", last modified: Thu Jun 15 04:22:29 2023, max compression
```

## Comparing `xdev-1.2.0.tar` & `xdev-1.3.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:56:52.009062 xdev-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-05 14:56:45.000000 xdev-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-05 14:56:52.009062 xdev-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-05 14:56:45.000000 xdev-1.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-05 14:56:45.000000 xdev-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 14:56:52.009062 xdev-1.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     9128 2023-04-05 14:56:45.000000 xdev-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:56:52.005061 xdev-1.2.0/xdev/
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/_ipython_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    15157 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/autojit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:56:52.005061 xdev-1.2.0/xdev/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6262 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/bin/freshpyenv.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/class_reloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:56:52.005061 xdev-1.2.0/xdev/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27825 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/cli/available_package_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)    40978 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/cli/docstr_stubgen.py
--rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/desktop_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/embeding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/format_quotes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10457 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/interactive_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/introspect.py
--rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)    19209 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/regex_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16068 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/search_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/tracebacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    19216 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/util_networkx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-04-05 14:56:45.000000 xdev-1.2.0/xdev/util_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:56:52.005061 xdev-1.2.0/xdev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-05 14:56:51.000000 xdev-1.2.0/xdev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-05 14:56:51.000000 xdev-1.2.0/xdev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:56:51.000000 xdev-1.2.0/xdev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-05 14:56:51.000000 xdev-1.2.0/xdev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-04-05 14:56:51.000000 xdev-1.2.0/xdev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-05 14:56:51.000000 xdev-1.2.0/xdev.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:22:29.250279 xdev-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-15 04:22:23.000000 xdev-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-06-15 04:22:29.250279 xdev-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-06-15 04:22:23.000000 xdev-1.3.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-15 04:22:23.000000 xdev-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 04:22:29.250279 xdev-1.3.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10396 2023-06-15 04:22:23.000000 xdev-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:22:29.250279 xdev-1.3.3/xdev/
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/_ipython_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15157 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/autojit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:22:29.250279 xdev-1.3.3/xdev/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6261 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/bin/freshpyenv.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/class_reloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:22:29.250279 xdev-1.3.3/xdev/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28155 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/cli/available_package_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41149 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/cli/docstr_stubgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/desktop_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/embeding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/format_quotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10457 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/interactive_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/introspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19250 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/regex_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/search_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/tracebacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19207 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/util_networkx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-06-15 04:22:23.000000 xdev-1.3.3/xdev/util_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:22:29.250279 xdev-1.3.3/xdev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-06-15 04:22:29.000000 xdev-1.3.3/xdev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-15 04:22:29.000000 xdev-1.3.3/xdev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 04:22:29.000000 xdev-1.3.3/xdev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 04:22:29.000000 xdev-1.3.3/xdev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-15 04:22:29.000000 xdev-1.3.3/xdev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 04:22:29.000000 xdev-1.3.3/xdev.egg-info/top_level.txt
```

### Comparing `xdev-1.2.0/LICENSE` & `xdev-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xdev-1.2.0/pyproject.toml` & `xdev-1.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xdev-1.2.0/setup.py` & `xdev-1.3.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -246,8 +246,39 @@
         "console_scripts": [
             "xdev = xdev.__main__:main",
         ],
     }
     setupkw["scripts"] = [
         "xdev/bin/freshpyenv.sh",
     ]
+    # setupkw['package_data'] = {"xdev": ["bash_completion.d/xdev-complete", "py.typed"]}
+    # setupkw['include_package_data'] = True
+    # setupkw['data_files'] = [('bash-completion', [
+    #     'xdev/share/bash-completion/xdev-complete.sh'
+    # ])]
     setup(**setupkw)
+
+"""
+# https://github.com/kislyuk/argcomplete/blob/develop/setup.py
+
+
+mkdir -p $HOME/code/xdev/xdev/bash_completion.d
+register-python-argcomplete xdev --external-argcomplete-script xdev-complete > $HOME/code/xdev/xdev/bash_completion.d/xdev-complete
+
+# Notes on bash completion:
+# https://unix.stackexchange.com/questions/416185/where-to-install-bash-completion-scripts-for-out-of-tree-packages
+
+# https://github.com/scop/bash-completion#faq
+# Put them in the completions subdir of $BASH_COMPLETION_USER_DIR (
+#     defaults to $XDG_DATA_HOME/bash-completion or
+#     ~/.local/share/bash-completion if $XDG_DATA_HOME is not set) to have them
+# loaded automatically on demand when the respective command is being completed.
+
+
+From JFC:
+When installing within the system python, the user scheme will be used. See [1][2]
+
+I think listing you file as data file will do it.
+
+[1] https://packaging.python.org/en/latest/guides/installing-using-linux-tools/
+[2] https://pip.pypa.io/en/stable/user_guide/#user-installs
+"""
```

### Comparing `xdev-1.2.0/xdev/__init__.py` & `xdev-1.3.3/xdev/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     - [ ] Perhaps let submodules specify a 2-tuple with the second item
         being a dict that indicates: (nomod, noattr)?
 
     - [ ] Automatically add custom defined names in this file to __all__
 """
 
-__version__ = '1.2.0'
+__version__ = '1.3.3'
 
 
 # __submodules__ = [
 #     'embeding',
 #     'interactive_iter',
 #     'desktop_interaction',
 #     'introspect',
@@ -130,14 +130,16 @@
             'editfile',
             'startfile',
             'view_directory',
         ],
         'embeding': [
             'EmbedOnException',
             'embed',
+            'embed_if_requested',
+            'embed_on_exception',
             'embed_on_exception_context',
             'fix_embed_globals',
         ],
         'format_quotes': [
             'format_quotes',
             'format_quotes_in_file',
             'format_quotes_in_text',
@@ -219,19 +221,19 @@
 __all__ = ['AsciiDirectedGlyphs', 'AsciiUndirectedGlyphs', 'ChDir',
            'EmbedOnException', 'GrepResult', 'IS_PROFILING', 'InteractiveIter',
            'MultiPattern', 'Pattern', 'PatternBase', 'PythonRegexBuilder',
            'RE_Pattern', 'RegexBuilder', 'UtfDirectedGlyphs',
            'UtfUndirectedGlyphs', 'VimRegexBuilder', 'algo', 'autojit',
            'bubbletext', 'byte_str', 'class_reloader', 'cli', 'conj_phrase',
            'desktop_interaction', 'difftext', 'distext', 'edit_distance',
-           'editfile', 'embed', 'embed_on_exception_context', 'embeding',
-           'find', 'fix_embed_globals', 'format_quotes',
-           'format_quotes_in_file', 'format_quotes_in_text',
-           'generate_network_text', 'get_func_kwargs', 'get_stack_frame',
-           'graph_str', 'grep', 'grepfile', 'greptext',
+           'editfile', 'embed', 'embed_if_requested', 'embed_on_exception',
+           'embed_on_exception_context', 'embeding', 'find',
+           'fix_embed_globals', 'format_quotes', 'format_quotes_in_file',
+           'format_quotes_in_text', 'generate_network_text', 'get_func_kwargs',
+           'get_stack_frame', 'graph_str', 'grep', 'grepfile', 'greptext',
            'import_module_from_pyx', 'interactive_iter', 'introspect',
            'iter_object_tree', 'knapsack', 'knapsack_greedy', 'knapsack_ilp',
            'knapsack_iterative', 'knapsack_iterative_int',
            'knapsack_iterative_numpy', 'make_warnings_print_tracebacks',
            'misc', 'nested_type', 'number_of_decimals',
            'our_extended_regex_compile', 'patterns', 'profile',
            'profile_globals', 'profile_now', 'profiler', 'quantum_random',
```

### Comparing `xdev-1.2.0/xdev/_ipython_ext.py` & `xdev-1.3.3/xdev/_ipython_ext.py`

 * *Files identical despite different names*

### Comparing `xdev-1.2.0/xdev/algo.py` & `xdev-1.3.3/xdev/algo.py`

 * *Files identical despite different names*

### Comparing `xdev-1.2.0/xdev/autojit.py` & `xdev-1.3.3/xdev/autojit.py`

 * *Files identical despite different names*

### Comparing `xdev-1.2.0/xdev/bin/freshpyenv.sh` & `xdev-1.3.3/xdev/bin/freshpyenv.sh`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     # the interactive session starts
     echo "source \"venv$PYVER/bin/activate\"" >> "$HOME"/.bashrc
 
     #pip install pip -U
     #pip install pip setuptools -U
 
     echo "
-Fresh development environment has been setup. 
+Fresh development environment has been setup.
 
 You can now run some variant to install your repo. For example typical
 xcookie-style repos can be installed via. E.g.
 
 # FULL STRICT VARIANT
 pip install -e .[all-strict] -v
```

### Comparing `xdev-1.2.0/xdev/class_reloader.py` & `xdev-1.3.3/xdev/class_reloader.py`

 * *Files identical despite different names*

### Comparing `xdev-1.2.0/xdev/cli/__main__.py` & `xdev-1.3.3/xdev/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `xdev-1.2.0/xdev/cli/available_package_versions.py` & `xdev-1.3.3/xdev/cli/available_package_versions.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     xdev availpkg scipy
     xdev availpkg kwimage
     xdev availpkg kwcoco
     xdev availpkg torch
     xdev availpkg line_profiler
     xdev availpkg uritools
     xdev availpkg textual
+    xdev availpkg networkx
 """
 import scriptconfig as scfg
 import ubelt as ub
 from packaging.version import parse as Version
 
 
 class AvailablePackageConfig(scfg.DataConfig):
@@ -558,14 +559,16 @@
 
                 # Declared support is generally only good for the python
                 # versions that existed at the time.
                 declared_support = [v for v in python_vstrings if reqspec.matches(v)]
                 heuristic_support = set(contemporary_pyvers) & set(declared_support)
                 max_pyver = max(heuristic_support, key=Version)
 
+            if min_pyver == 'any':
+                min_pyver = '2.7'
             if min_pyver == 'py2.py3':
                 min_pyver = '2.7'
             if min_pyver == 'py3':
                 min_pyver = '3.6'
 
             if max_pyver == 'py2.py3':
                 max_pyver = '2.7'
@@ -631,35 +634,40 @@
     chosen_minmax_for = {}
     chosen_minimum_for = {}
 
     # groups = dict(list(new_table.groupby('min_pyver')))
 
     for min_pyver, subdf in sorted(new_table.groupby('min_pyver'), key=lambda x: Version(x[0])):
         # print('--- min_pyver = {!r} --- '.format(min_pyver))
-        version_to_support = dict(list(subdf.groupby('version')))
+
+        if 'version' in subdf.columns:
+            version_to_support = dict(list(subdf.groupby('version')))
+        else:
+            version_to_support = dict(list(subdf.groupby('pkg_version')))
 
         cand_to_score = {}
         try:
             version_to_support = ub.sorted_keys(version_to_support, key=Version)
         except Exception:
             maybe_bad_keys = list(version_to_support.keys())
             print('version_to_support = {!r}'.format(maybe_bad_keys))
             maybe_ok_keys = [k for k in maybe_bad_keys if '.dev0' not in k]
             version_to_support = ub.dict_subset(version_to_support, maybe_ok_keys)
 
-        combo_values = {
-            ('linux', 'x86_64'): 101,
-            ('macosx', 'x86_64'): 5,
-            ('win', 'x86_64'): 11,
-        }
-        for cand, support in version_to_support.items():
-            has_combos = support.value_counts(['os', 'arch']).index.tolist()
-            total_have = sum(combo_values.get(k, 0) for k in has_combos)
-            score = total_have
-            cand_to_score[cand] = score
+        if 'os' in subdf.columns and 'arch' in subdf.columns:
+            combo_values = {
+                ('linux', 'x86_64'): 101,
+                ('macosx', 'x86_64'): 5,
+                ('win', 'x86_64'): 11,
+            }
+            for cand, support in version_to_support.items():
+                has_combos = support.value_counts(['os', 'arch']).index.tolist()
+                total_have = sum(combo_values.get(k, 0) for k in has_combos)
+                score = total_have
+                cand_to_score[cand] = score
 
         cand_to_score = ub.sorted_vals(cand_to_score)
         cand_to_score = ub.sorted_keys(cand_to_score, key=Version)
 
         # Filter to only the versions we requested, but if
         # none exist, return something
         if request_min is not None:
```

### Comparing `xdev-1.2.0/xdev/cli/docstr_stubgen.py` & `xdev-1.3.3/xdev/cli/docstr_stubgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,14 +82,19 @@
 
 Stub = ...  # hack for mypy. Not sure why it is generated in the first place.
 
 
 def _hack_away_compiled_mypy():
     """
     Worked with: mypy-0.970+dev.ddbea6988c0913c70ed16cd2fda6064e301b4b63
+
+    Note:
+        # Can also do
+        pip uninstall mypy
+        pip install -U mypy --no-binary :all:
     """
     # This doesn't seem to work. The only thing that has worked so far is a
     # custom checkout and developer install. Not sure why that is the case.
     modpath = ub.Path(ub.modname_to_modpath('mypy'))
     print(f'modpath={modpath}')
     compiled_modules = list(modpath.glob('*.so'))
     print(f'compiled_modules={compiled_modules}')
@@ -826,18 +831,19 @@
             if arg_.initializer is not None:
                 # TODO: find a better way of checking if the default value
                 # matches the type of the given doctype and extend the
                 # doctype if needbe. For now we are hacking it to
                 # handle None specificaly.
                 if hasattr(arg_.initializer, 'name') and arg_.initializer.name == 'None':
                     info = name_to_parsed_docstr_info[name]
-                    doctype_str = info['type'].replace(' ', '')
-                    if all(n not in doctype_str for n in {'None', 'Optional'}):
-                        info['type'] = info['type'] + ' | None'
-                        self.add_typing_import('Union')
+                    if info['type'] is not None:
+                        doctype_str = info['type'].replace(' ', '')
+                        if all(n not in doctype_str for n in {'None', 'Optional'}):
+                            info['type'] = info['type'] + ' | None'
+                            self.add_typing_import('Union')
         # ------------------------------------------
 
         args: List[str] = []
         for i, arg_ in enumerate(o.arguments):
             var = arg_.variable
             kind = arg_.kind
             name = var.name
```

### Comparing `xdev-1.2.0/xdev/cli/main.py` & `xdev-1.3.3/xdev/cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,470 +13,473 @@
 import scriptconfig as scfg
 import ubelt as ub
 import os
 import sys
 from scriptconfig.modal import ModalCLI
 from xdev.cli import available_package_versions
 
-modal = ModalCLI(description=ub.codeblock(
-    '''
+
+class XdevCLI(ModalCLI):
+    """
     The XDEV CLI
 
     A collection of excellent developer tools for excellent developers.
-    '''))
-
-
-@modal
-class InfoCLI(scfg.DataConfig):
     """
-    Info about xdev
-    """
-    __command__ = 'info'
 
-    @classmethod
-    def main(cls, cmdline=False, **kwargs):
-        import xdev
-        print('sys.version_info = {!r}'.format(sys.version_info))
-        print('xdev.__version__ = {!r}'.format(xdev.__version__))
-        print('xdev.__file__ = {!r}'.format(xdev.__file__))
+    class InfoCLI(scfg.DataConfig):
+        """
+        Info about xdev
+        """
+        __command__ = 'info'
 
+        @classmethod
+        def main(cls, cmdline=False, **kwargs):
+            import xdev
+            print('sys.version_info = {!r}'.format(sys.version_info))
+            print('xdev.__version__ = {!r}'.format(xdev.__version__))
+            print('xdev.__file__ = {!r}'.format(xdev.__file__))
 
-@modal
-class CodeblockCLI(scfg.DataConfig):
-    """
-    Remove indentation from text.
-
-    Useful for writing subscripts (e.g. python -c code) in shell files without
-    having to resort to ugly indentation.
-    """
-    __command__ = 'codeblock'
-    __epilog__ = """
-    Example Usage
-    -------------
-
-    python -c "$(xdev codeblock "
-        import pathlib
-        print(list(pathlib.Path('.').glob('*')))
-        ")"
-    """
-    text = scfg.Value('', type=str, position=1,
-                      help='text to remove indentation from (i.e. dedent)')
+    class CodeblockCLI(scfg.DataConfig):
+        """
+        Remove indentation from text.
 
-    @classmethod
-    def main(cls, cmdline=False, **kwargs):
+        Useful for writing subscripts (e.g. python -c code) in shell files without
+        having to resort to ugly indentation.
         """
-        Example:
-            >>> from xdev.cli.main import *  # NOQA
-            >>> CodeblockCLI.main(cmdline=0, text='foobar')
+        __command__ = 'codeblock'
+        __epilog__ = """
+        Example Usage
+        -------------
+
+        python -c "$(xdev codeblock "
+            import pathlib
+            print(list(pathlib.Path('.').glob('*')))
+            ")"
         """
-        config = cls.cli(cmdline=cmdline, data=kwargs)
-        print(ub.codeblock(config['text']))
+        text = scfg.Value('', type=str, position=1,
+                          help='text to remove indentation from (i.e. dedent)')
 
+        @classmethod
+        def main(cls, cmdline=False, **kwargs):
+            """
+            Example:
+                >>> from xdev.cli.main import *  # NOQA
+                >>> CodeblockCLI.main(cmdline=0, text='foobar')
+            """
+            config = cls.cli(cmdline=cmdline, data=kwargs)
+            print(ub.codeblock(config['text']))
 
-@modal
-class SedCLI(scfg.DataConfig):
-    """
-    Search and replace text in files
-    """
-    __command__ = 'sed'
-    __default__ = {
-        'regexpr': scfg.Value('', position=1, help=ub.paragraph(
-            '''
-            The pattern to search for.
-            ''')),
-        'repl': scfg.Value('', position=2, help=ub.paragraph(
-            '''
-            The pattern to replace with.
-            ''')),
-        'dpath': scfg.Value(None, position=3, help=ub.paragraph(
-            '''
-            The directory to recursively search or a file pattern to match.
-            '''
-        )),
-        'dry': scfg.Value('ask', position=4, help=ub.paragraph(
-            '''
-            if 1, show what would be done. if 0, execute the change, if "ask",
-            then show the dry run and then ask for confirmation.
-            '''
-        )),
-        'include': scfg.Value(None),
-        'exclude': scfg.Value(None),
-        'recursive': scfg.Value(True),
-        'verbose': scfg.Value(1),
-    }
-
-    @classmethod
-    def main(cls, cmdline=False, **kwargs):
-        from xdev import search_replace
-        config = cls.cli(cmdline=cmdline, data=kwargs)
-        if config['verbose'] > 2:
-            print('config = {}'.format(ub.repr2(dict(config), nl=1, sort=0)))
-
-        if config['dry'] in {'ask', 'auto'}:
-            from rich.prompt import Confirm
-            config['dry'] = True
-            search_replace.sed(**config)
-            flag = Confirm.ask('Do you want to execute this sed?')
-            if flag:
-                config['dry'] = False
+    class SedCLI(scfg.DataConfig):
+        """
+        Search and replace text in files
+        """
+        __command__ = 'sed'
+        __default__ = {
+            'regexpr': scfg.Value('', position=1, help=ub.paragraph(
+                '''
+                The pattern to search for.
+                ''')),
+            'repl': scfg.Value('', position=2, help=ub.paragraph(
+                '''
+                The pattern to replace with.
+                ''')),
+            'dpath': scfg.Value(None, position=3, help=ub.paragraph(
+                '''
+                The directory to recursively search or a file pattern to match.
+                '''
+            )),
+            'dry': scfg.Value('ask', position=4, help=ub.paragraph(
+                '''
+                if 1, show what would be done. if 0, execute the change, if "ask",
+                then show the dry run and then ask for confirmation.
+                '''
+            )),
+            'include': scfg.Value(None),
+            'exclude': scfg.Value(None),
+            'recursive': scfg.Value(True),
+            'verbose': scfg.Value(1),
+        }
+
+        @classmethod
+        def main(cls, cmdline=False, **kwargs):
+            from xdev import search_replace
+            config = cls.cli(cmdline=cmdline, data=kwargs)
+            if config['verbose'] > 2:
+                print('config = {}'.format(ub.repr2(dict(config), nl=1, sort=0)))
+
+            if config['dry'] in {'ask', 'auto'}:
+                from rich.prompt import Confirm
+                config['dry'] = True
+                search_replace.sed(**config)
+                flag = Confirm.ask('Do you want to execute this sed?')
+                if flag:
+                    config['dry'] = False
+                    search_replace.sed(**config)
+            else:
                 search_replace.sed(**config)
-        else:
-            search_replace.sed(**config)
-
-
-@modal
-class FindCLI(scfg.DataConfig):
-    """
-    Find matching files or paths in a directory.
-
-    This is similar to the GNU find program, but written in Python.  Important
-    differences are that this program is:
-
-    * has pattern first argument and uses the cwd by default.
 
-    * recursive by default
+    class FindCLI(scfg.DataConfig):
+        """
+        Find matching files or paths in a directory.
 
-    * has explicit include / exclude options
+        This is similar to the GNU find program, but written in Python.  Important
+        differences are that this program is:
 
-    Example
-    -------
-    xdev find "*.py"
-    """
-    __command__ = 'find'
-    __default__ = {
-        'pattern': scfg.Value('', position=1),
-        'dpath': scfg.Value(None, position=2, help='the path to search. Defaults to cwd'),
-        'include': scfg.Value(None, help='If specified, only list results with matching basenames'),
-        'exclude': scfg.Value(None, help='If specified, do not list results with matching basenames'),
-        'type': scfg.Value('f', help="can be f and/or d"),
-        'recursive': scfg.Value(True),
-        'dirblocklist': scfg.Value(
-            'Any directory matching this pattern will be removed from '
-            'traveral.'),
-        'followlinks': scfg.Value(False),
-    }
-
-    @classmethod
-    def main(cls, cmdline=False, **kwargs):
-        from xdev import search_replace
-        config = cls.cli(cmdline=cmdline, data=kwargs)
-        for found in search_replace.find(**config):
-            print(found)
+        * has pattern first argument and uses the cwd by default.
 
+        * recursive by default
 
-@modal
-class TreeCLI(scfg.DataConfig):
-    """
-    List a directory like a tree
+        * has explicit include / exclude options
 
-    See Also
-    --------
-    The apt-installable tree command
-
-    Example
-    -------
-    xdev tree
-    """
-    __command__ = 'tree'
+        Example
+        -------
+        xdev find "*.py"
+        """
+        __command__ = 'find'
+        __default__ = {
+            'pattern': scfg.Value('', position=1),
+            'dpath': scfg.Value(None, position=2, help='the path to search. Defaults to cwd'),
+            'include': scfg.Value(None, help='If specified, only list results with matching basenames'),
+            'exclude': scfg.Value(None, help='If specified, do not list results with matching basenames'),
+            'type': scfg.Value('f', help="can be f and/or d"),
+            'recursive': scfg.Value(True),
+            'dirblocklist': scfg.Value(
+                'Any directory matching this pattern will be removed from '
+                'traveral.'),
+            'followlinks': scfg.Value(False),
+        }
+
+        @classmethod
+        def main(cls, cmdline=False, **kwargs):
+            from xdev import search_replace
+            config = cls.cli(cmdline=cmdline, data=kwargs)
+            for found in search_replace.find(**config):
+                print(found)
 
-    __default__ = {
-        'cwd': scfg.Value('.', position=1),
-        'max_files': scfg.Value(100),
-        'colors': scfg.Value(not ub.NO_COLOR, isflag=True),
-        'dirblocklist': scfg.Value(None),
-        'max_depth': scfg.Value(
-            None, help='maximum depth to recurse', short_alias=['L']),
-    }
-
-    @classmethod
-    def main(cls, cmdline=False, **kwargs):
-        import xdev
-        config = cls.cli(cmdline=cmdline, data=kwargs)
-        xdev.tree_repr(**config)
-        # print()
+    class TreeCLI(scfg.DataConfig):
+        """
+        List a directory like a tree
 
+        See Also
+        --------
+        The apt-installable tree command
+
+        Example
+        -------
+        xdev tree
+        """
+        __command__ = 'tree'
 
-@modal
-class PintCLI(scfg.DataConfig):
-    """
-    Converts one type of unit to another via the pint library.
+        __default__ = {
+            'cwd': scfg.Value('.', position=1),
+            'max_files': scfg.Value(100),
+            'colors': scfg.Value(not ub.NO_COLOR, isflag=True),
+            'dirblocklist': scfg.Value(None),
+            'max_depth': scfg.Value(
+                None, help='maximum depth to recurse', short_alias=['L']),
+        }
+
+        @classmethod
+        def main(cls, cmdline=False, **kwargs):
+            import xdev
+            config = cls.cli(cmdline=cmdline, data=kwargs)
+            xdev.tree_repr(**config)
+            # print()
 
-    Notes:
+    class PintCLI(scfg.DataConfig):
+        """
+        Converts one type of unit to another via the pint library.
 
-    See Also
-    --------
-    The pint-convert tool comes pre-installed with pint but isn't as useful for
-    in-bash computation unless you munge the output. The idea here is that when
-    something like GDAL wants an environ in bytes, we can specify it in
-    megabytes.
-
-    Example Usage
-    -------------
-    xdev pint "10 megabytes" "bytes" --precision=0
+        Notes:
 
-    """
-    __command__ = 'pint'
-    __alias__ = ['convert_unit']
-    __default__ = {
-        'input_expr': scfg.Value(None, position=1, help='A parsable pint expression with magnitude and units'),
-        'output_unit': scfg.Value(None, position=2, help='The output unit to convert to'),
-        'precision': scfg.Value(0, type=int, help='number of decimal places to use'),
-    }
-
-    @classmethod
-    def main(cls, cmdline=False, **kwargs):
-        import pint
-        ureg = pint.UnitRegistry()
-        args = cls.cli(cmdline=cmdline, data=kwargs)
-        input = ureg.parse_expression(args['input_expr'])
-        output_unit = args['output_unit']
-        if output_unit is None:
-            output_unit = input.unit
-        output = input.to(output_unit)
-        if args['precision'] == 0:
-            print(int(output.magnitude))
-        else:
-            print(output.magnitude)
+        See Also
+        --------
+        The pint-convert tool comes pre-installed with pint but isn't as useful for
+        in-bash computation unless you munge the output. The idea here is that when
+        something like GDAL wants an environ in bytes, we can specify it in
+        megabytes.
+
+        Example Usage
+        -------------
+        xdev pint "10 megabytes" "bytes" --precision=0
 
+        """
+        __command__ = 'pint'
+        __alias__ = ['convert_unit']
+        __default__ = {
+            'input_expr': scfg.Value(None, position=1, help='A parsable pint expression with magnitude and units'),
+            'output_unit': scfg.Value(None, position=2, help='The output unit to convert to'),
+            'precision': scfg.Value(0, type=int, help='number of decimal places to use'),
+        }
+
+        @classmethod
+        def main(cls, cmdline=False, **kwargs):
+            import pint
+            ureg = pint.UnitRegistry()
+            args = cls.cli(cmdline=cmdline, data=kwargs)
+            input = ureg.parse_expression(args['input_expr'])
+            output_unit = args['output_unit']
+            if output_unit is None:
+                output_unit = input.unit
+            output = input.to(output_unit)
+            if args['precision'] == 0:
+                print(int(output.magnitude))
+            else:
+                print(output.magnitude)
 
-@modal
-class PyfileCLI(scfg.DataConfig):
-    """
-    Prints the path corresponding to a Python module.
+    class PyfileCLI(scfg.DataConfig):
+        """
+        Prints the path corresponding to a Python module.
 
-    This uses the ``ubelt.modname_to_modpath`` mechanism that does not require
-    importing of your package.
+        This uses the ``ubelt.modname_to_modpath`` mechanism that does not require
+        importing of your package.
 
-    Alternatives
-    ------------
-    An alternative with no dependencies is to use the one-liner:
-
-    python -c "import <modname>; print(<modname>.__file__)"
-
-    Example Usage
-    -------------
-    xdev pyfile xdev
-    xdev pyfile numpy
-
-    # Use this feature in scripts for developement to avoid referencing
-    # machine-specific paths.
-    MODPATH=$(xdev pyfile ubelt)
-    echo "MODPATH = $MODPATH"
-    """
-    __command__ = 'pyfile'
-    __alias__ = ['modpath']
-    # input_expr = scfg.Value(None, position=1)
-    # output_expr = scfg.Value(None, position=2)
-    __default__ = {
-        'modname': scfg.Value(None, position=1),
-    }
-
-    @classmethod
-    def main(cls, cmdline=False, **kwargs):
-        args = cls.cli(cmdline=cmdline, data=kwargs)
-        modpath = ub.modname_to_modpath(args['modname'])
-        print(modpath)
+        Alternatives
+        ------------
+        An alternative with no dependencies is to use the one-liner:
+
+        python -c "import <modname>; print(<modname>.__file__)"
+
+        Example Usage
+        -------------
+        xdev pyfile xdev
+        xdev pyfile numpy
+
+        # Use this feature in scripts for developement to avoid referencing
+        # machine-specific paths.
+        MODPATH=$(xdev pyfile ubelt)
+        echo "MODPATH = $MODPATH"
+        """
+        __command__ = 'pyfile'
+        __alias__ = ['modpath']
+        # input_expr = scfg.Value(None, position=1)
+        # output_expr = scfg.Value(None, position=2)
+        __default__ = {
+            'modname': scfg.Value(None, position=1),
+        }
+
+        @classmethod
+        def main(cls, cmdline=False, **kwargs):
+            args = cls.cli(cmdline=cmdline, data=kwargs)
+            modpath = ub.modname_to_modpath(args['modname'])
+            print(modpath)
 
+    class PyVersionCLI(scfg.DataConfig):
+        """
+        Detect and print the version of a Python module or package.
 
-@modal
-class PyVersionCLI(scfg.DataConfig):
-    """
-    Detect and print the version of a Python module or package.
+        Note
+        ----
+        Different backends may produce different results, especially for packages
+        that are in development and were installed in development mode.
+
+        Alternatives
+        ------------
+        An alternative with no dependencies is to use the one-liner:
+
+        python -c "import <modname>; print(<modname>.__version__)"
+
+        Example Usage
+        -------------
+        xdev pyversion xdev
+        xdev pyversion numpy
+
+        # Both the module name and the package name can be used.
+        xdev pyversion cv2
+        xdev pyversion opencv-python-headless
 
-    Note
-    ----
-    Different backends may produce different results, especially for packages
-    that are in development and were installed in development mode.
-
-    Alternatives
-    ------------
-    An alternative with no dependencies is to use the one-liner:
-
-    python -c "import <modname>; print(<modname>.__version__)"
-
-    Example Usage
-    -------------
-    xdev pyversion xdev
-    xdev pyversion numpy
-
-    # Both the module name and the package name can be used.
-    xdev pyversion cv2
-    xdev pyversion opencv-python-headless
+        xdev pyversion xdev --backend=import
+        xdev pyversion xdev --backend=pkg_resources
+        """
+        __command__ = 'pyversion'
+        __alias__ = ['modversion']
+        __default__ = {
+            'modname': scfg.Value(None, position=1, help='The name of the module or package'),
+            'backend': scfg.Value('auto', help=ub.paragraph(
+                '''
+                The method to lookup the version. The core methods are 'import'
+                which imports the module and looks for a ``__version__`` attribute
+                or 'pkg_resources', which uses pip metadata. Can also be 'auto'
+                which tries to find the first one that works.
+                '''), choices=['auto', 'import', 'pkg_resources']),
+        }
+
+        @classmethod
+        def main(cls, cmdline=False, **kwargs):
+            args = cls.cli(cmdline=cmdline, data=kwargs)
+            modname = args['modname']
 
-    xdev pyversion xdev --backend=import
-    xdev pyversion xdev --backend=pkg_resources
-    """
-    __command__ = 'pyversion'
-    __alias__ = ['modversion']
-    __default__ = {
-        'modname': scfg.Value(None, position=1, help='The name of the module or package'),
-        'backend': scfg.Value('auto', help=ub.paragraph(
-            '''
-            The method to lookup the version. The core methods are 'import'
-            which imports the module and looks for a ``__version__`` attribute
-            or 'pkg_resources', which uses pip metadata. Can also be 'auto'
-            which tries to find the first one that works.
-            '''), choices=['auto', 'import', 'pkg_resources']),
-    }
-
-    @classmethod
-    def main(cls, cmdline=False, **kwargs):
-        args = cls.cli(cmdline=cmdline, data=kwargs)
-        modname = args['modname']
-
-        if args['backend'] == 'auto':
-            candidate_backends  = ['import', 'pkg_resources']
-        else:
-            candidate_backends = [args['backend']]
-
-        def _getversion(modname, backend):
-            if backend == 'import':
-                module = ub.import_module_from_name(modname)
-                version = module.__version__
-            elif backend == 'pkg_resources':
-                import pkg_resources
-                version = pkg_resources.get_distribution(modname).version
+            if args['backend'] == 'auto':
+                candidate_backends  = ['import', 'pkg_resources']
             else:
-                raise KeyError(backend)
-            return version
+                candidate_backends = [args['backend']]
 
-        version = None
-        for backend in candidate_backends:
-            try:
-                version = _getversion(modname, backend)
-            except KeyError:
-                raise
-            except Exception:
-                ...
-            else:
-                break
-        print(version)
-        if version is None:
-            raise Exception(f'No version was found for {modname}')
+            def _getversion(modname, backend):
+                if backend == 'import':
+                    module = ub.import_module_from_name(modname)
+                    version = module.__version__
+                elif backend == 'pkg_resources':
+                    import pkg_resources
+                    version = pkg_resources.get_distribution(modname).version
+                else:
+                    raise KeyError(backend)
+                return version
+
+            version = None
+            for backend in candidate_backends:
+                try:
+                    version = _getversion(modname, backend)
+                except KeyError:
+                    raise
+                except Exception:
+                    ...
+                else:
+                    break
+            print(version)
+            if version is None:
+                raise Exception(f'No version was found for {modname}')
 
+    class EditfileCLI(scfg.DataConfig):
+        """
+        Opens a file in your visual editor determined by the ``VISUAL``
+        environment variable.
 
-@modal
-class FormatQuotesCLI(scfg.DataConfig):
-    """
-    Use single quotes for code and double quotes for docs.
+        If ``VISUAL`` is unspecified it attempts to default to the first known
+        existing editor.
 
-    This is useful for "fixing" quotations after running a code formater like
-    black on a module.
-    """
-    __command__ = 'format_quotes'
-    __default__ = {
-        'path': scfg.Value('', position=1, help=ub.paragraph(
-            '''
-            ''')),
-        'diff': scfg.Value(True, help=ub.paragraph(
-            '''
-            The pattern to replace with.
-            ''')),
-        'write': scfg.Value(False, short_alias=['-w'], help=ub.paragraph(
-            '''
-            The directory to recursively search or a file pattern to match.
-            '''
-        )),
-        'verbose': scfg.Value(3, help=ub.paragraph(
-            '''
-            '''
-        )),
-        'recursive': scfg.Value(True),
-    }
-
-    @classmethod
-    def main(cls, cmdline=False, **kwargs):
-        from xdev import format_quotes
-        config = cls.cli(cmdline=cmdline, data=kwargs)
-        format_quotes.format_quotes(**config)
+        Example Usage
+        -------------
+        xdev edit xdev
+        xdev edit numpy
+        """
+        __command__ = 'editfile'
+        __alias__ = ['edit']
+        __default__ = {
+            'target': scfg.Value(None, position=1, help='a path or a module name'),
+        }
+
+        @classmethod
+        def main(cls, cmdline=False, **kwargs):
+            import xdev
+            args = cls.cli(cmdline=cmdline, data=kwargs)
+            xdev.editfile(args.target)
 
+    class FormatQuotesCLI(scfg.DataConfig):
+        """
+        Use single quotes for code and double quotes for docs.
 
-@modal
-class FreshPyenvCLI(scfg.DataConfig):
-    """
-    Create a fresh environment in a docker container to test a Python package.
+        This is useful for "fixing" quotations after running a code formater like
+        black on a module.
+        """
+        __command__ = 'format_quotes'
+        __default__ = {
+            'path': scfg.Value('', position=1, help=ub.paragraph(
+                '''
+                ''')),
+            'diff': scfg.Value(True, help=ub.paragraph(
+                '''
+                The pattern to replace with.
+                ''')),
+            'write': scfg.Value(False, isflag=True, short_alias=['w'], help=ub.paragraph(
+                '''
+                The directory to recursively search or a file pattern to match.
+                '''
+            )),
+            'verbose': scfg.Value(3, help=ub.paragraph(
+                '''
+                '''
+            )),
+            'recursive': scfg.Value(True),
+        }
+
+        @classmethod
+        def main(cls, cmdline=False, **kwargs):
+            from xdev import format_quotes
+            config = cls.cli(cmdline=cmdline, data=kwargs)
+            format_quotes.format_quotes(**config)
 
-    SeeAlso
-    -------
-    The generic freshpyenv.sh bash script also installed with this package.
-    """
-    __command__ = 'freshpyenv'
-    __default__ = {
-        'image': scfg.Value('__default__', help='The docker image to use')
-    }
-
-    @classmethod
-    def main(cls, cmdline=False, **kwargs):
-        config = cls.cli(cmdline=cmdline, data=kwargs)
-        import ubelt as ub
-        ub.cmd(f'freshpyenv.sh --image={config["image"]}', system=True)
+    class FreshPyenvCLI(scfg.DataConfig):
+        """
+        Create a fresh environment in a docker container to test a Python package.
 
+        SeeAlso
+        -------
+        The generic freshpyenv.sh bash script also installed with this package.
+        """
+        __command__ = 'freshpyenv'
+        __default__ = {
+            'image': scfg.Value('__default__', help='The docker image to use')
+        }
+
+        @classmethod
+        def main(cls, cmdline=False, **kwargs):
+            config = cls.cli(cmdline=cmdline, data=kwargs)
+            import ubelt as ub
+            ub.cmd(f'freshpyenv.sh --image={config["image"]}', system=True)
 
-@modal
-class DocstrStubgenCLI(scfg.DataConfig):
-    """
-    Generate Typed Stubs from Docstrings (experimental)
+    class DocstrStubgenCLI(scfg.DataConfig):
+        """
+        Generate Typed Stubs from Docstrings (experimental)
 
-    Note
-    ----
-    This is an experimental command and currently requires a specialized patch
-    to mypy to work correctly.
-    """
-    __command__ = 'docstubs'
-    __alias__ = ['doctypes']
-    __default__ = {
-        'module': scfg.Value(None, position=1, help=ub.paragraph(
-            '''
-            The name of a module in the PYTHONPATH or an explicit path to that
-            module.
-            ''')),
-    }
-
-    @classmethod
-    def main(cls, cmdline=False, **kwargs):
-        from xdev.cli import docstr_stubgen
-        config = cls.cli(cmdline=cmdline, data=kwargs)
-        print(f'config={config}')
-        modname_or_path = config['module']
-        print(f'modname_or_path={modname_or_path}')
-        if modname_or_path is None:
-            raise ValueError('Must specify the module')
-        modpath = docstr_stubgen.modpath_coerce(modname_or_path)
-        modpath = ub.Path(modpath)
-        generated = docstr_stubgen.generate_typed_stubs(modpath)
-
-        for fpath, text in generated.items():
-            fpath = ub.Path(fpath)
-            print(f'Write fpath={fpath}')
-            fpath.write_text(text)
-
-        # Generate a py.typed file to mark the package as typed
-        if modpath.is_dir():
-            pytyped_fpath = (modpath / 'py.typed')
-            print(f'touch pytyped_fpath={pytyped_fpath}')
-            pytyped_fpath.touch()
-
-
-@modal
-class AvailablePackageCLI(scfg.DataConfig):
-    __command__ = 'available_package_versions'
-    __alias__ = ['availpkg']
-    __default__ = available_package_versions.AvailablePackageConfig.__default__
-    __doc__ = available_package_versions.AvailablePackageConfig.__doc__
-
-    @classmethod
-    def main(cls, cmdline=False, **kwargs):
-        available_package_versions.main(cmdline=cmdline, **kwargs)
+        Note
+        ----
+        This is an experimental command and currently requires a specialized patch
+        to mypy to work correctly.
+        """
+        __command__ = 'docstubs'
+        __alias__ = ['doctypes']
+        __default__ = {
+            'module': scfg.Value(None, position=1, help=ub.paragraph(
+                '''
+                The name of a module in the PYTHONPATH or an explicit path to that
+                module.
+                ''')),
+        }
+
+        @classmethod
+        def main(cls, cmdline=False, **kwargs):
+            from xdev.cli import docstr_stubgen
+            config = cls.cli(cmdline=cmdline, data=kwargs)
+            print(f'config={config}')
+            modname_or_path = config['module']
+            print(f'modname_or_path={modname_or_path}')
+            if modname_or_path is None:
+                raise ValueError('Must specify the module')
+            modpath = docstr_stubgen.modpath_coerce(modname_or_path)
+            modpath = ub.Path(modpath)
+            generated = docstr_stubgen.generate_typed_stubs(modpath)
+
+            for fpath, text in generated.items():
+                fpath = ub.Path(fpath)
+                print(f'Write fpath={fpath}')
+                fpath.write_text(text)
+
+            # Generate a py.typed file to mark the package as typed
+            if modpath.is_dir():
+                pytyped_fpath = (modpath / 'py.typed')
+                print(f'touch pytyped_fpath={pytyped_fpath}')
+                pytyped_fpath.touch()
+
+    class AvailablePackageCLI(scfg.DataConfig):
+        __command__ = 'available_package_versions'
+        __alias__ = ['availpkg']
+        __default__ = available_package_versions.AvailablePackageConfig.__default__
+        __doc__ = available_package_versions.AvailablePackageConfig.__doc__
+
+        @classmethod
+        def main(cls, cmdline=False, **kwargs):
+            available_package_versions.main(cmdline=cmdline, **kwargs)
 
 
 def main():
     import xdev
-    modal.version = xdev.__version__
+    cli = XdevCLI()
+    cli.version = xdev.__version__
     XDEV_LOOSE_CLI = os.environ.get('XDEV_LOOSE_CLI', '')
-    modal.run(strict=not XDEV_LOOSE_CLI)
+    cli.main(strict=not XDEV_LOOSE_CLI)
 
 
 if __name__ == '__main__':
     """
     CommandLine:
         xdev --help
         xdev --version
```

### Comparing `xdev-1.2.0/xdev/embeding.py` & `xdev-1.3.3/xdev/embeding.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,7 +225,8 @@
     # Hack all of the local variables to be global variables
     frame.f_globals.update(frame.f_locals)
     # Leave some trace that we did this
     frame.f_globals['_did_xdev_fix_embed_globals'] = True
 
 
 embed_on_exception_context = EmbedOnException()
+embed_on_exception = embed_on_exception_context
```

### Comparing `xdev-1.2.0/xdev/interactive_iter.py` & `xdev-1.3.3/xdev/interactive_iter.py`

 * *Files identical despite different names*

### Comparing `xdev-1.2.0/xdev/introspect.py` & `xdev-1.3.3/xdev/introspect.py`

 * *Files identical despite different names*

### Comparing `xdev-1.2.0/xdev/misc.py` & `xdev-1.3.3/xdev/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -463,7 +463,18 @@
             rprint(text)
         else:
             print(text)
 
     if return_tree:
         info['tree'] = tree
     return info
+
+
+def textfind(text, pattern):
+    """
+    Return a colored text that highlights the pattern
+    """
+    import re
+    pat = re.compile('(' + pattern + ')')
+    parts = pat.split(text)
+    new_text = ''.join([p if idx % 2 == 0 else ub.color_text(p, 'red') for idx, p in enumerate(parts)])
+    print(new_text)
```

### Comparing `xdev-1.2.0/xdev/patterns.py` & `xdev-1.3.3/xdev/patterns.py`

 * *Files identical despite different names*

### Comparing `xdev-1.2.0/xdev/profiler.py` & `xdev-1.3.3/xdev/profiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 __all__ = [
     'profile',
     'profile_now',
     'profile_globals',
     'IS_PROFILING',
 ]
 
-IS_PROFILING = os.environ.get('XDEV_PROFILE', '').lower() in {'1', 'on', 'true', 'yes'}
+_FALSY_STRINGS = {'', '0', 'off', 'false', 'no'}
+IS_PROFILING = os.environ.get('XDEV_PROFILE', '').lower() not in _FALSY_STRINGS
 IS_PROFILING = IS_PROFILING or '--profile' in sys.argv
 
 
 class DummyProfiler:
     """
     A profiler that does nothing.
     """
```

### Comparing `xdev-1.2.0/xdev/search_replace.py` & `xdev-1.3.3/xdev/search_replace.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,39 +105,41 @@
         print('num_files_checked = {}'.format(num_files_checked))
         print('num probable binary files skipped = {}'.format(num_skipped))
         print('fpaths_changed = {}'.format(ub.repr2(sorted(fpaths_changed))))
         print('total lines changed = {!r}'.format(num_changed))
 
 
 def grep(regexpr, dpath=None, include=None, exclude=None, recursive=True,
-         verbose=1):
+         dirblocklist=None, verbose=1):
     r"""
     Execute a grep on multiple files.
 
     Args:
         regexpr (str | Pattern): pattern to find
         dpath (str | None): passed to :func:`find`.
         include (str | List[str] | MultiPattern | None): passed to :func:`find`.
         exclude (str | List[str] | MultiPattern | None): passed to :func:`find`.
         recursive (bool): passed to :func:`find`.
+        dirblocklist (str | List[str] | MultiPattern | None): passed to :func:`find`.
         verbose (int): verbosity level
 
     Returns:
         List[GrepResult]:
 
     Example:
         >>> from xdev.search_replace import *  # NOQA
         >>> from xdev.search_replace import _create_test_filesystem
         >>> dpath = _create_test_filesystem()['root']
         >>> grep('a', dpath=dpath)
     """
     grep_results = []
 
     fpath_generator = find(dpath=dpath, type='f', include=include,
-                           exclude=exclude, recursive=recursive)
+                           exclude=exclude, recursive=recursive,
+                           dirblocklist=dirblocklist)
 
     for fpath in fpath_generator:
         grepres = grepfile(fpath, regexpr, verbose=verbose)
         if grepres:
             grep_results.append(grepres)
 
     if verbose:
```

### Comparing `xdev-1.2.0/xdev/tracebacks.py` & `xdev-1.3.3/xdev/tracebacks.py`

 * *Files identical despite different names*

### Comparing `xdev-1.2.0/xdev/util.py` & `xdev-1.3.3/xdev/util.py`

 * *Files identical despite different names*

### Comparing `xdev-1.2.0/xdev/util_networkx.py` & `xdev-1.3.3/xdev/util_networkx.py`

 * *Files 0% similar despite different names*

```diff
@@ -499,15 +499,15 @@
     -------
     str | None :
         utf8 representation of the tree / forest
 
     Example
     -------
     >>> graph = nx.balanced_tree(r=2, h=3, create_using=nx.DiGraph)
-    >>> print(nx.graph_str(graph))
+    >>> print(graph_str(graph))
     ╙── 0
         ├─╼ 1
         │   ├─╼ 3
         │   │   ├─╼ 7
         │   │   └─╼ 8
         │   └─╼ 4
         │       ├─╼ 9
@@ -518,20 +518,20 @@
             │   └─╼ 12
             └─╼ 6
                 ├─╼ 13
                 └─╼ 14
 
 
     >>> graph = nx.balanced_tree(r=1, h=2, create_using=nx.Graph)
-    >>> print(nx.graph_str(graph))
+    >>> print(graph_str(graph))
     ╙── 0
         └── 1
             └── 2
 
-    >>> print(nx.graph_str(graph, ascii_only=True))
+    >>> print(graph_str(graph, ascii_only=True))
     +-- 0
         L-- 1
             L-- 2
     """
     printbuf = []
     if write is None:
         _write = printbuf.append
```

### Comparing `xdev-1.2.0/xdev/util_path.py` & `xdev-1.3.3/xdev/util_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,43 +89,44 @@
         When the pattern does not include a .dvc suffix, we include all those
         files, for other files that exist by adding a .dvc suffix.
 
         With the pattern matches both a dvc and non-dvc file, they are grouped
         together.
 
     Example:
+        >>> from xdev.util_path import *  # NOQA
         >>> dpath = ub.Path.appdir('xdev/tests/sidecar_glob')
         >>> dpath.delete().ensuredir()
         >>> (dpath / 'file1').touch()
         >>> (dpath / 'file1.ext').touch()
         >>> (dpath / 'file1.ext.car').touch()
         >>> (dpath / 'file2.ext').touch()
         >>> (dpath / 'file3.ext.car').touch()
         >>> (dpath / 'file4.car').touch()
         >>> (dpath / 'file5').touch()
         >>> (dpath / 'file6').touch()
         >>> (dpath / 'file6.car').touch()
         >>> (dpath / 'file7.bike').touch()
-        >>> def _handle_resulst(results):
+        >>> def _handle_results(results):
         ...     results = list(results)
         ...     for row in results:
         ...         for k, v in row.items():
         ...             if v is not None:
         ...                 row[k] = v.relative_to(dpath)
         ...     print(ub.repr2(results, sv=1))
         ...     return results
         >>> main_key = 'main',
         >>> sidecar_key = '.car'
         >>> sidecar_ext = '.car'
         >>> main_pat = dpath / '*'
-        >>> _handle_resulst(sidecar_glob(main_pat, sidecar_ext))
-        >>> _handle_resulst(sidecar_glob(dpath / '*.ext', '.car'))
-        >>> _handle_resulst(sidecar_glob(dpath / '*.car', '.car'))
-        >>> _handle_resulst(sidecar_glob(dpath / 'file*.ext', '.car'))
-        >>> _handle_resulst(sidecar_glob(dpath / '*', '.ext'))
+        >>> _handle_results(sidecar_glob(main_pat, sidecar_ext))
+        >>> _handle_results(sidecar_glob(dpath / '*.ext', '.car'))
+        >>> _handle_results(sidecar_glob(dpath / '*.car', '.car'))
+        >>> _handle_results(sidecar_glob(dpath / 'file*.ext', '.car'))
+        >>> _handle_results(sidecar_glob(dpath / '*', '.ext'))
     """
     from xdev import patterns as util_pattern
     import warnings
     import os
     _len_ext = len(sidecar_ext)
     main_pat = os.fspath(main_pat)
     glob_patterns = [main_pat]
```

### Comparing `xdev-1.2.0/xdev.egg-info/SOURCES.txt` & `xdev-1.3.3/xdev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xdev-1.2.0/xdev.egg-info/requires.txt` & `xdev-1.3.3/xdev.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 IPython>=7.16.2
 parse>=1.19.0
 pyfiglet>=0.7
 pyflakes>=2.5.0
 pygments>=2.12.0
-scriptconfig>=0.7.4
+scriptconfig>=0.7.9
 ubelt>=1.2.3
 xinspect>=0.2.0
 
 [:python_version < "3.10" and python_version >= "3.9"]
 numpy>=1.19.3
 
 [:python_version < "3.11" and python_version >= "3.10"]
@@ -19,53 +19,56 @@
 [:python_version < "3.8" and python_version >= "3.7"]
 numpy>=1.14.5
 
 [:python_version < "3.9" and python_version >= "3.8"]
 numpy>=1.19.2
 
 [:python_version < "4.0" and python_version >= "3.11"]
-numpy>=1.23.5
+numpy>=1.23.2
 
 [all]
 IPython>=7.16.2
 autoflake>=1.5.0
 fire>=0.4.0
 parse>=1.19.0
 pyfiglet>=0.7
 pyflakes>=2.5.0
 pygments>=2.12.0
-scriptconfig>=0.7.4
+scriptconfig>=0.7.9
 ubelt>=1.2.3
 xdoctest>=0.14.0
 xinspect>=0.2.0
 yapf>=0.16.3
 
 [all-strict]
 IPython==7.16.2
 autoflake==1.5.0
 fire==0.4.0
 parse==1.19.0
 pyfiglet==0.7
 pyflakes==2.5.0
 pygments==2.12.0
-scriptconfig==0.7.4
+scriptconfig==0.7.9
 ubelt==1.2.3
 xdoctest==0.14.0
 xinspect==0.2.0
 yapf==0.16.3
 
 [all-strict:python_version < "3.10" and python_version >= "3.9"]
 Levenshtein==0.18.0
 coverage==5.3.1
 line_profiler==3.4.0
 numpy==1.19.3
 
 [all-strict:python_version < "3.10.0" and python_version >= "3.7.0"]
 pytest==4.6.0
 
+[all-strict:python_version < "3.11"]
+parso==0.8.0
+
 [all-strict:python_version < "3.11" and python_version >= "3.10"]
 Levenshtein==0.18.2
 line_profiler==3.4.0
 numpy==1.21.1
 pytest==6.2.5
 
 [all-strict:python_version < "3.7" and python_version >= "3.6"]
@@ -88,15 +91,16 @@
 coverage==6.1.1
 line_profiler==3.4.0
 numpy==1.19.2
 
 [all-strict:python_version < "4.0" and python_version >= "3.11"]
 Levenshtein==0.20.3
 line_profiler==4.0.0
-numpy==1.23.5
+numpy==1.23.2
+parso==0.8.3
 pytest==7.0.0
 
 [all-strict:python_version >= "3.10"]
 coverage==6.1.1
 
 [all-strict:python_version >= "3.6.0"]
 pytest-cov==3.0.0
@@ -106,14 +110,17 @@
 coverage>=5.3.1
 line_profiler>=3.4.0
 numpy>=1.19.3
 
 [all:python_version < "3.10.0" and python_version >= "3.7.0"]
 pytest>=4.6.0
 
+[all:python_version < "3.11"]
+parso>=0.8.0
+
 [all:python_version < "3.11" and python_version >= "3.10"]
 Levenshtein>=0.18.2
 line_profiler>=3.4.0
 numpy>=1.21.1
 pytest>=6.2.5
 
 [all:python_version < "3.7" and python_version >= "3.6"]
@@ -136,15 +143,16 @@
 coverage>=6.1.1
 line_profiler>=3.4.0
 numpy>=1.19.2
 
 [all:python_version < "4.0" and python_version >= "3.11"]
 Levenshtein>=0.20.3
 line_profiler>=4.0.0
-numpy>=1.23.5
+numpy>=1.23.2
+parso>=0.8.3
 pytest>=7.0.0
 
 [all:python_version >= "3.10"]
 coverage>=6.1.1
 
 [all:python_version >= "3.6.0"]
 pytest-cov>=3.0.0
@@ -159,14 +167,17 @@
 fire==0.4.0
 yapf==0.16.3
 
 [optional-strict:python_version < "3.10" and python_version >= "3.9"]
 Levenshtein==0.18.0
 line_profiler==3.4.0
 
+[optional-strict:python_version < "3.11"]
+parso==0.8.0
+
 [optional-strict:python_version < "3.11" and python_version >= "3.10"]
 Levenshtein==0.18.2
 line_profiler==3.4.0
 
 [optional-strict:python_version < "3.7" and python_version >= "3.6"]
 Levenshtein==0.18.0
 line_profiler==3.4.0
@@ -178,19 +189,23 @@
 [optional-strict:python_version < "3.9" and python_version >= "3.8"]
 Levenshtein==0.18.0
 line_profiler==3.4.0
 
 [optional-strict:python_version < "4.0" and python_version >= "3.11"]
 Levenshtein==0.20.3
 line_profiler==4.0.0
+parso==0.8.3
 
 [optional:python_version < "3.10" and python_version >= "3.9"]
 Levenshtein>=0.18.0
 line_profiler>=3.4.0
 
+[optional:python_version < "3.11"]
+parso>=0.8.0
+
 [optional:python_version < "3.11" and python_version >= "3.10"]
 Levenshtein>=0.18.2
 line_profiler>=3.4.0
 
 [optional:python_version < "3.7" and python_version >= "3.6"]
 Levenshtein>=0.18.0
 line_profiler>=3.4.0
@@ -202,22 +217,23 @@
 [optional:python_version < "3.9" and python_version >= "3.8"]
 Levenshtein>=0.18.0
 line_profiler>=3.4.0
 
 [optional:python_version < "4.0" and python_version >= "3.11"]
 Levenshtein>=0.20.3
 line_profiler>=4.0.0
+parso>=0.8.3
 
 [runtime-strict]
 IPython==7.16.2
 parse==1.19.0
 pyfiglet==0.7
 pyflakes==2.5.0
 pygments==2.12.0
-scriptconfig==0.7.4
+scriptconfig==0.7.9
 ubelt==1.2.3
 xinspect==0.2.0
 
 [runtime-strict:python_version < "3.10" and python_version >= "3.9"]
 numpy==1.19.3
 
 [runtime-strict:python_version < "3.11" and python_version >= "3.10"]
@@ -229,15 +245,15 @@
 [runtime-strict:python_version < "3.8" and python_version >= "3.7"]
 numpy==1.14.5
 
 [runtime-strict:python_version < "3.9" and python_version >= "3.8"]
 numpy==1.19.2
 
 [runtime-strict:python_version < "4.0" and python_version >= "3.11"]
-numpy==1.23.5
+numpy==1.23.2
 
 [tests]
 xdoctest>=0.14.0
 
 [tests-strict]
 xdoctest==0.14.0
```

