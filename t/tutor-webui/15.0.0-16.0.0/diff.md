# Comparing `tmp/tutor-webui-15.0.0.tar.gz` & `tmp/tutor-webui-16.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tutor-webui-15.0.0.tar", last modified: Mon Dec 12 18:05:10 2022, max compression
+gzip compressed data, was "tutor-webui-16.0.0.tar", last modified: Thu Jun 15 01:29:23 2023, max compression
```

## Comparing `tutor-webui-15.0.0.tar` & `tutor-webui-16.0.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 18:05:10.000000 tutor-webui-15.0.0/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2022-12-12 18:04:47.000000 tutor-webui-15.0.0/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     3595 2022-12-12 18:05:10.000000 tutor-webui-15.0.0/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     2104 2022-12-12 18:04:35.000000 tutor-webui-15.0.0/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2022-12-12 18:05:10.000000 tutor-webui-15.0.0/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1890 2022-12-12 18:04:47.000000 tutor-webui-15.0.0/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 18:05:10.000000 tutor-webui-15.0.0/tutor_webui.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     3595 2022-12-12 18:05:10.000000 tutor-webui-15.0.0/tutor_webui.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)      329 2022-12-12 18:05:10.000000 tutor-webui-15.0.0/tutor_webui.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2022-12-12 18:05:10.000000 tutor-webui-15.0.0/tutor_webui.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       45 2022-12-12 18:05:10.000000 tutor-webui-15.0.0/tutor_webui.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       40 2022-12-12 18:05:10.000000 tutor-webui-15.0.0/tutor_webui.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       11 2022-12-12 18:05:10.000000 tutor-webui-15.0.0/tutor_webui.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 18:05:10.000000 tutor-webui-15.0.0/tutorwebui/
--rw-r--r--   0 ci        (1000) ci        (1000)       23 2022-12-12 18:04:47.000000 tutor-webui-15.0.0/tutorwebui/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2022-12-12 18:04:35.000000 tutor-webui-15.0.0/tutorwebui/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5939 2022-12-12 18:04:47.000000 tutor-webui-15.0.0/tutorwebui/cli.py
--rw-r--r--   0 ci        (1000) ci        (1000)      189 2022-12-12 18:04:35.000000 tutor-webui-15.0.0/tutorwebui/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 01:29:23.851639 tutor-webui-16.0.0/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-06-15 01:29:13.000000 tutor-webui-16.0.0/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-15 01:29:13.000000 tutor-webui-16.0.0/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     3169 2023-06-15 01:29:23.851639 tutor-webui-16.0.0/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     2122 2023-06-15 01:29:13.000000 tutor-webui-16.0.0/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-06-15 01:29:13.000000 tutor-webui-16.0.0/pyproject.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-15 01:29:23.854973 tutor-webui-16.0.0/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1891 2023-06-15 01:29:13.000000 tutor-webui-16.0.0/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 01:29:23.851639 tutor-webui-16.0.0/tutor_webui.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     3169 2023-06-15 01:29:23.000000 tutor-webui-16.0.0/tutor_webui.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)      356 2023-06-15 01:29:23.000000 tutor-webui-16.0.0/tutor_webui.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-06-15 01:29:23.000000 tutor-webui-16.0.0/tutor_webui.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       44 2023-06-15 01:29:23.000000 tutor-webui-16.0.0/tutor_webui.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       40 2023-06-15 01:29:23.000000 tutor-webui-16.0.0/tutor_webui.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       11 2023-06-15 01:29:23.000000 tutor-webui-16.0.0/tutor_webui.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 01:29:23.851639 tutor-webui-16.0.0/tutorwebui/
+-rw-r--r--   0 ci        (1000) ci        (1000)      176 2023-06-15 01:29:13.000000 tutor-webui-16.0.0/tutorwebui/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-15 01:29:13.000000 tutor-webui-16.0.0/tutorwebui/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     6126 2023-06-15 01:29:13.000000 tutor-webui-16.0.0/tutorwebui/cli.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      189 2023-06-15 01:29:13.000000 tutor-webui-16.0.0/tutorwebui/plugin.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tutor-webui-15.0.0/PKG-INFO` & `tutor-webui-16.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: tutor-webui
-Version: 15.0.0
+Version: 16.0.0
 Summary: Web-based user interface plugin for Tutor
 Home-page: https://overhang.io/overhangio/tutor-webui
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: Overhang.IO
 Maintainer-email: regis@overhang.io
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
 Project-URL: Code, https://github.com/overhangio/tutor-webui
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-webui/issues
 Project-URL: Community, https://discuss.openedx.org
-Description: WebUI plugin for `Tutor <https://docs.tutor.overhang.io>`__
-        ============================================================
-        
-        This is a plugin for Tutor that allows you to manage a Tutor-powered `Open edX <https://open.edx.org/>`__ installation from a browser -- a web user interface! In other words, it is no longer necessary to SSH to a remote server to manage a running instance.
-        
-        Installation
-        ------------
-        
-        ::
-        
-            pip install tutor-webui
-        
-        Usage
-        -----
-        
-        Enable the plugin::
-        
-            tutor plugins enable webui
-        
-        Start the web user interface::
-        
-            tutor webui start
-        
-        You can then access the interface at http://localhost:3737, or http://youserverurl:3737.
-        
-        .. image:: https://overhang.io/static/catalog/screenshots/webui.png
-        
-        All ``tutor`` commands can be executed from this web UI: you just don't need to prefix the commands with ``tutor``. For instance, to deploy a local Open edX instance, run::
-        
-            local launch
-        
-        instead of ``tutor local launch``.
-        
-        Instead of running the interactive `repl <https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop>`__ in a web browser, you can also run tutor interactively directly from your shell::
-        
-            tutor shell
-        
-        Authentication
-        ~~~~~~~~~~~~~~
-        
-        **WARNING** Once you launch the web UI, it is accessible by everyone, which means that your Open edX platform is at risk. If you are planning to leave the web UI up for a long time, you should setup a user and password for authentication::
-        
-            tutor webui configure
-        
-        Troubleshooting
-        ---------------
-        
-        This Tutor plugin is maintained by Régis Behmo from `Overhang.IO <https://overhang.io>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
-        
-        License
-        -------
-        
-        This software is licensed under the terms of the AGPLv3.
-        
-        This project depends on the `Gotty <https://github.com/yudai/gotty/>`_ binary, which is provided under the terms of the `MIT license <https://github.com/yudai/gotty/blob/master/LICENSE>`_.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+License-File: LICENSE.txt
+
+WebUI plugin for `Tutor <https://docs.tutor.overhang.io>`__
+============================================================
+
+This is a plugin for Tutor that allows you to manage a Tutor-powered `Open edX <https://open.edx.org/>`__ installation from a browser -- a web user interface! In other words, it is no longer necessary to SSH to a remote server to manage a running instance.
+
+Installation
+------------
+
+::
+
+    tutor plugins install webui
+
+Usage
+-----
+
+Enable the plugin::
+
+    tutor plugins enable webui
+
+Start the web user interface::
+
+    tutor webui start
+
+You can then access the interface at http://localhost:3737, or http://youserverurl:3737.
+
+.. image:: https://overhang.io/static/catalog/screenshots/webui.png
+
+All ``tutor`` commands can be executed from this web UI: you just don't need to prefix the commands with ``tutor``. For instance, to deploy a local Open edX instance, run::
+
+    local launch
+
+instead of ``tutor local launch``.
+
+Instead of running the interactive `repl <https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop>`__ in a web browser, you can also run tutor interactively directly from your shell::
+
+    tutor shell
+
+Authentication
+~~~~~~~~~~~~~~
+
+**WARNING** Once you launch the web UI, it is accessible by everyone, which means that your Open edX platform is at risk. If you are planning to leave the web UI up for a long time, you should setup a user and password for authentication::
+
+    tutor webui configure
+
+Troubleshooting
+---------------
+
+This Tutor plugin is maintained by Régis Behmo from `Overhang.IO <https://overhang.io>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
+
+License
+-------
+
+This software is licensed under the terms of the AGPLv3.
+
+This project depends on the `Gotty <https://github.com/sorenisanerd/gotty/>`_ binary, which is provided under the terms of the `MIT license <https://github.com/sorenisanerd/gotty/blob/master/LICENSE>`_.
```

### Comparing `tutor-webui-15.0.0/README.rst` & `tutor-webui-16.0.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This is a plugin for Tutor that allows you to manage a Tutor-powered `Open edX <https://open.edx.org/>`__ installation from a browser -- a web user interface! In other words, it is no longer necessary to SSH to a remote server to manage a running instance.
 
 Installation
 ------------
 
 ::
 
-    pip install tutor-webui
+    tutor plugins install webui
 
 Usage
 -----
 
 Enable the plugin::
 
     tutor plugins enable webui
@@ -48,8 +48,8 @@
 This Tutor plugin is maintained by Régis Behmo from `Overhang.IO <https://overhang.io>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
 
 License
 -------
 
 This software is licensed under the terms of the AGPLv3.
 
-This project depends on the `Gotty <https://github.com/yudai/gotty/>`_ binary, which is provided under the terms of the `MIT license <https://github.com/yudai/gotty/blob/master/LICENSE>`_.
+This project depends on the `Gotty <https://github.com/sorenisanerd/gotty/>`_ binary, which is provided under the terms of the `MIT license <https://github.com/sorenisanerd/gotty/blob/master/LICENSE>`_.
```

### Comparing `tutor-webui-15.0.0/setup.py` & `tutor-webui-16.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,24 +39,24 @@
     author_email="contact@overhang.io",
     maintainer="Overhang.IO",
     maintainer_email="regis@overhang.io",
     description="Web-based user interface plugin for Tutor",
     long_description=load_readme(),
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
-    python_requires=">=3.7",
-    install_requires=["tutor>=15.0.0,<16.0.0", "click_repl>=0.2.0"],
+    python_requires=">=3.8",
+    install_requires=["tutor>=16.0.0,<17.0.0", "click_repl>=0.2.0"],
     entry_points={
         "tutor.plugin.v1": ["webui = tutorwebui.plugin"],
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `tutor-webui-15.0.0/tutor_webui.egg-info/PKG-INFO` & `tutor-webui-16.0.0/tutor_webui.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: tutor-webui
-Version: 15.0.0
+Version: 16.0.0
 Summary: Web-based user interface plugin for Tutor
 Home-page: https://overhang.io/overhangio/tutor-webui
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: Overhang.IO
 Maintainer-email: regis@overhang.io
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
 Project-URL: Code, https://github.com/overhangio/tutor-webui
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-webui/issues
 Project-URL: Community, https://discuss.openedx.org
-Description: WebUI plugin for `Tutor <https://docs.tutor.overhang.io>`__
-        ============================================================
-        
-        This is a plugin for Tutor that allows you to manage a Tutor-powered `Open edX <https://open.edx.org/>`__ installation from a browser -- a web user interface! In other words, it is no longer necessary to SSH to a remote server to manage a running instance.
-        
-        Installation
-        ------------
-        
-        ::
-        
-            pip install tutor-webui
-        
-        Usage
-        -----
-        
-        Enable the plugin::
-        
-            tutor plugins enable webui
-        
-        Start the web user interface::
-        
-            tutor webui start
-        
-        You can then access the interface at http://localhost:3737, or http://youserverurl:3737.
-        
-        .. image:: https://overhang.io/static/catalog/screenshots/webui.png
-        
-        All ``tutor`` commands can be executed from this web UI: you just don't need to prefix the commands with ``tutor``. For instance, to deploy a local Open edX instance, run::
-        
-            local launch
-        
-        instead of ``tutor local launch``.
-        
-        Instead of running the interactive `repl <https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop>`__ in a web browser, you can also run tutor interactively directly from your shell::
-        
-            tutor shell
-        
-        Authentication
-        ~~~~~~~~~~~~~~
-        
-        **WARNING** Once you launch the web UI, it is accessible by everyone, which means that your Open edX platform is at risk. If you are planning to leave the web UI up for a long time, you should setup a user and password for authentication::
-        
-            tutor webui configure
-        
-        Troubleshooting
-        ---------------
-        
-        This Tutor plugin is maintained by Régis Behmo from `Overhang.IO <https://overhang.io>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
-        
-        License
-        -------
-        
-        This software is licensed under the terms of the AGPLv3.
-        
-        This project depends on the `Gotty <https://github.com/yudai/gotty/>`_ binary, which is provided under the terms of the `MIT license <https://github.com/yudai/gotty/blob/master/LICENSE>`_.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+License-File: LICENSE.txt
+
+WebUI plugin for `Tutor <https://docs.tutor.overhang.io>`__
+============================================================
+
+This is a plugin for Tutor that allows you to manage a Tutor-powered `Open edX <https://open.edx.org/>`__ installation from a browser -- a web user interface! In other words, it is no longer necessary to SSH to a remote server to manage a running instance.
+
+Installation
+------------
+
+::
+
+    tutor plugins install webui
+
+Usage
+-----
+
+Enable the plugin::
+
+    tutor plugins enable webui
+
+Start the web user interface::
+
+    tutor webui start
+
+You can then access the interface at http://localhost:3737, or http://youserverurl:3737.
+
+.. image:: https://overhang.io/static/catalog/screenshots/webui.png
+
+All ``tutor`` commands can be executed from this web UI: you just don't need to prefix the commands with ``tutor``. For instance, to deploy a local Open edX instance, run::
+
+    local launch
+
+instead of ``tutor local launch``.
+
+Instead of running the interactive `repl <https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop>`__ in a web browser, you can also run tutor interactively directly from your shell::
+
+    tutor shell
+
+Authentication
+~~~~~~~~~~~~~~
+
+**WARNING** Once you launch the web UI, it is accessible by everyone, which means that your Open edX platform is at risk. If you are planning to leave the web UI up for a long time, you should setup a user and password for authentication::
+
+    tutor webui configure
+
+Troubleshooting
+---------------
+
+This Tutor plugin is maintained by Régis Behmo from `Overhang.IO <https://overhang.io>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
+
+License
+-------
+
+This software is licensed under the terms of the AGPLv3.
+
+This project depends on the `Gotty <https://github.com/sorenisanerd/gotty/>`_ binary, which is provided under the terms of the `MIT license <https://github.com/sorenisanerd/gotty/blob/master/LICENSE>`_.
```

### Comparing `tutor-webui-15.0.0/tutorwebui/cli.py` & `tutor-webui-16.0.0/tutorwebui/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,25 +8,23 @@
 from urllib.request import urlopen
 
 import click
 import click_repl
 
 # Note: it is important that this module does not depend on config, such that
 # the web ui can be launched even where there is no configuration.
-from tutor import fmt
 from tutor import env as tutor_env
-from tutor import exceptions
-from tutor import serialize
-from tutor.types import Config
+from tutor import exceptions, fmt, serialize
 from tutor.commands.context import Context
+from tutor.types import Config
 
+# Check if it was upgraded since 2022
+# https://github.com/sorenisanerd/gotty/releases
+GOTTY_RELEASE = "v1.5.0"
 
-# Check if it was upgraded since 2017
-# https://github.com/yudai/gotty/releases
-GOTTY_RELEASE = "v1.0.1"
 
 @click.group(
     short_help="Web user interface", help="""Run Tutor commands from a web terminal"""
 )
 def webui() -> None:
     pass
 
@@ -137,17 +135,25 @@
 def check_gotty_binary(root: str) -> None:
     path = gotty_path(root)
     if os.path.exists(path):
         return
     fmt.echo_info(f"Downloading gotty to {path}...")
 
     # Generate release url
-    # Note: I don't know how to handle arm
-    architecture = "amd64" if platform.architecture()[0] == "64bit" else "386"
-    url = f"https://github.com/yudai/gotty/releases/download/{GOTTY_RELEASE}/gotty_{platform.system().lower()}_{architecture}.tar.gz"
+    architecture_map = {"x86_64": "amd64", "i386": "386", "aarch64": "arm64"}
+    architecture = architecture_map.get(platform.uname().machine)
+    if not architecture:
+        raise exceptions.TutorError(
+            f"Unsupported architecture: {platform.uname().machine}"
+        )
+
+    url = (
+        f"https://github.com/sorenisanerd/gotty/releases/download/{GOTTY_RELEASE}/"
+        f"gotty_{GOTTY_RELEASE}_{platform.system().lower()}_{architecture}.tar.gz"
+    )
 
     # Download
     response = urlopen(url)
 
     # Decompress
     dirname = os.path.dirname(path)
     if not os.path.exists(dirname):
```

