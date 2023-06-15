# Comparing `tmp/CodeChat_Server-0.2.8.tar.gz` & `tmp/CodeChat_Server-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CodeChat_Server-0.2.8.tar", last modified: Wed Dec  7 21:04:28 2022, max compression
+gzip compressed data, was "CodeChat_Server-0.2.9.tar", last modified: Fri Dec 16 00:43:25 2022, max compression
```

## Comparing `CodeChat_Server-0.2.8.tar` & `CodeChat_Server-0.2.9.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.984975 CodeChat_Server-0.2.8/
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.828974 CodeChat_Server-0.2.8/CodeChat_Server/
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.771058 CodeChat_Server-0.2.8/CodeChat_Server/CodeChat_Client/
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.863974 CodeChat_Server-0.2.8/CodeChat_Server/CodeChat_Client/static/
--rw-rw-rw-   0        0        0     3239 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/CodeChat_Client/static/CodeChat_client.css
--rw-rw-rw-   0        0        0    21437 2022-12-07 19:36:49.000000 CodeChat_Server-0.2.8/CodeChat_Server/CodeChat_Client/static/CodeChat_client.js
--rw-rw-rw-   0        0        0    14149 2022-08-31 04:12:06.000000 CodeChat_Server-0.2.8/CodeChat_Server/CodeChat_Client/static/ReconnectingWebsocket.js
--rw-rw-rw-   0        0        0      883 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/CodeChat_Client/static/splitter.css
--rw-rw-rw-   0        0        0     6183 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/CodeChat_Client/static/splitter.js
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.870990 CodeChat_Server-0.2.8/CodeChat_Server/CodeChat_Client/templates/
--rw-rw-rw-   0        0        0     3151 2022-12-07 21:00:03.000000 CodeChat_Server-0.2.8/CodeChat_Server/CodeChat_Client/templates/CodeChat_client.html
--rw-rw-rw-   0        0        0     1229 2022-08-31 04:12:06.000000 CodeChat_Server-0.2.8/CodeChat_Server/CodeChat_Client/templates/insecure.html
--rw-rw-rw-   0        0        0     1258 2022-12-07 21:02:05.000000 CodeChat_Server-0.2.8/CodeChat_Server/__init__.py
--rw-rw-rw-   0        0        0    15014 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/__main__.py
--rw-rw-rw-   0        0        0      482 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/constants.py
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.873974 CodeChat_Server-0.2.8/CodeChat_Server/gen_py/
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.886980 CodeChat_Server-0.2.8/CodeChat_Server/gen_py/CodeChat_Services/
--rw-rw-rw-   0        0        0    28216 2022-08-31 04:12:06.000000 CodeChat_Server-0.2.8/CodeChat_Server/gen_py/CodeChat_Services/EditorPlugin.py
--rw-rw-rw-   0        0        0       51 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/gen_py/CodeChat_Services/__init__.py
--rw-rw-rw-   0        0        0      401 2022-08-31 04:12:06.000000 CodeChat_Server-0.2.8/CodeChat_Server/gen_py/CodeChat_Services/constants.py
--rw-rw-rw-   0        0        0     3895 2022-08-31 04:12:06.000000 CodeChat_Server-0.2.8/CodeChat_Server/gen_py/CodeChat_Services/ttypes.py
--rw-rw-rw-   0        0        0        0 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/gen_py/__init__.py
--rw-rw-rw-   0        0        0    26823 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/render_manager.py
--rw-rw-rw-   0        0        0    28343 2022-08-31 04:12:06.000000 CodeChat_Server-0.2.8/CodeChat_Server/renderer.py
--rw-rw-rw-   0        0        0    18045 2022-12-07 19:36:49.000000 CodeChat_Server-0.2.8/CodeChat_Server/server.py
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.792974 CodeChat_Server-0.2.8/CodeChat_Server/templates/
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.896975 CodeChat_Server-0.2.8/CodeChat_Server/templates/doxygen/
--rw-rw-rw-   0        0        0   118862 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/doxygen/Doxyfile
--rw-rw-rw-   0        0        0     2433 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/doxygen/codechat_config.yaml
--rw-rw-rw-   0        0        0     1024 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/doxygen/main.c
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.903977 CodeChat_Server-0.2.8/CodeChat_Server/templates/javadoc/
--rw-rw-rw-   0        0        0      839 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/javadoc/Simple.java
--rw-rw-rw-   0        0        0     2465 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/javadoc/codechat_config.yaml
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.913975 CodeChat_Server-0.2.8/CodeChat_Server/templates/mdbook/
--rw-rw-rw-   0        0        0        6 2022-07-05 20:44:18.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/mdbook/.gitignore
--rw-rw-rw-   0        0        0     1174 2022-07-05 20:44:18.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/mdbook/book.toml
--rw-rw-rw-   0        0        0     2400 2022-07-05 20:44:18.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/mdbook/codechat_config.yaml
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.928974 CodeChat_Server-0.2.8/CodeChat_Server/templates/mdbook/src/
--rw-rw-rw-   0        0        0      201 2022-08-31 04:12:06.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/mdbook/src/SUMMARY.md
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.930974 CodeChat_Server-0.2.8/CodeChat_Server/templates/mdbook/src/__pycache__/
--rw-rw-rw-   0        0        0      223 2022-07-05 20:44:15.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/mdbook/src/__pycache__/chapter_2.cpython-38.pyc
--rw-rw-rw-   0        0        0      222 2022-07-05 20:44:18.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/mdbook/src/book.toml
--rw-rw-rw-   0        0        0      882 2022-07-05 20:44:18.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/mdbook/src/chapter_1.md
--rw-rw-rw-   0        0        0      263 2022-07-05 20:44:18.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/mdbook/src/chapter_2.py
--rw-rw-rw-   0        0        0      487 2022-07-05 20:44:18.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/mdbook/src/codechat-config.yaml
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.937976 CodeChat_Server-0.2.8/CodeChat_Server/templates/mkdocs/
--rw-rw-rw-   0        0        0     2433 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/mkdocs/codechat_config.yaml
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.940982 CodeChat_Server-0.2.8/CodeChat_Server/templates/mkdocs/docs/
--rw-rw-rw-   0        0        0     1014 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/mkdocs/docs/index.md
--rw-rw-rw-   0        0        0       20 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/mkdocs/mkdocs.yml
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.951991 CodeChat_Server-0.2.8/CodeChat_Server/templates/pretext/
--rw-rw-rw-   0        0        0      172 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/pretext/.gitignore
--rw-rw-rw-   0        0        0      224 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/pretext/README.md
--rw-rw-rw-   0        0        0     2452 2022-08-31 04:12:06.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/pretext/codechat_config.yaml
--rw-rw-rw-   0        0        0     1273 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/pretext/project.ptx
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.954978 CodeChat_Server-0.2.8/CodeChat_Server/templates/pretext/publication/
--rw-rw-rw-   0        0        0     3485 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/pretext/publication/publication.ptx
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.957975 CodeChat_Server-0.2.8/CodeChat_Server/templates/pretext/source/
--rw-rw-rw-   0        0        0     4494 2022-08-31 04:12:06.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/pretext/source/minimal.ptx
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.965983 CodeChat_Server-0.2.8/CodeChat_Server/templates/runestone/
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.968977 CodeChat_Server-0.2.8/CodeChat_Server/templates/runestone/_sources/
--rw-rw-rw-   0        0        0     4899 2022-07-05 20:44:18.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/runestone/_sources/index.rst
--rw-rw-rw-   0        0        0     2499 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/runestone/codechat_config.yaml
--rw-rw-rw-   0        0        0    12309 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/runestone/conf.py
--rw-rw-rw-   0        0        0     2090 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/runestone/pavement.py
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.976975 CodeChat_Server-0.2.8/CodeChat_Server/templates/sphinx/
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.979978 CodeChat_Server-0.2.8/CodeChat_Server/templates/sphinx/__pycache__/
--rw-rw-rw-   0        0        0      979 2022-07-05 20:44:14.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/sphinx/__pycache__/conf.cpython-38.pyc
--rw-rw-rw-   0        0        0     3097 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/sphinx/codechat_config.yaml
--rw-rw-rw-   0        0        0    14432 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/sphinx/conf.py
--rw-rw-rw-   0        0        0     1271 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.8/CodeChat_Server/templates/sphinx/index.rst
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.846974 CodeChat_Server-0.2.8/CodeChat_Server.egg-info/
--rw-rw-rw-   0        0        0     3545 2022-12-07 21:04:28.000000 CodeChat_Server-0.2.8/CodeChat_Server.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2700 2022-12-07 21:04:28.000000 CodeChat_Server-0.2.8/CodeChat_Server.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-07 21:04:28.000000 CodeChat_Server-0.2.8/CodeChat_Server.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2022-12-07 21:04:28.000000 CodeChat_Server-0.2.8/CodeChat_Server.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      131 2022-12-07 21:04:28.000000 CodeChat_Server-0.2.8/CodeChat_Server.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-12-07 21:04:28.000000 CodeChat_Server-0.2.8/CodeChat_Server.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1694 2022-01-29 23:01:37.000000 CodeChat_Server-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3545 2022-12-07 21:04:28.985979 CodeChat_Server-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     2486 2022-01-29 23:01:40.000000 CodeChat_Server-0.2.8/README.rst
-drwxrwxrwx   0        0        0        0 2022-12-07 21:04:28.981975 CodeChat_Server-0.2.8/docs/
--rw-rw-rw-   0        0        0    35998 2020-08-10 17:03:41.000000 CodeChat_Server-0.2.8/docs/LICENSE.rst
--rw-rw-rw-   0        0        0      641 2022-01-29 17:45:44.000000 CodeChat_Server-0.2.8/pyproject.toml
--rw-rw-rw-   0        0        0      682 2022-12-07 21:04:28.987976 CodeChat_Server-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     5962 2022-12-07 20:00:18.000000 CodeChat_Server-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.323427 CodeChat_Server-0.2.9/
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.135429 CodeChat_Server-0.2.9/CodeChat_Server/
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.087929 CodeChat_Server-0.2.9/CodeChat_Server/CodeChat_Client/
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.175428 CodeChat_Server-0.2.9/CodeChat_Server/CodeChat_Client/static/
+-rw-rw-rw-   0        0        0     3239 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/CodeChat_Client/static/CodeChat_client.css
+-rw-rw-rw-   0        0        0    21437 2022-12-07 19:36:49.000000 CodeChat_Server-0.2.9/CodeChat_Server/CodeChat_Client/static/CodeChat_client.js
+-rw-rw-rw-   0        0        0    14149 2022-08-31 04:12:06.000000 CodeChat_Server-0.2.9/CodeChat_Server/CodeChat_Client/static/ReconnectingWebsocket.js
+-rw-rw-rw-   0        0        0      883 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/CodeChat_Client/static/splitter.css
+-rw-rw-rw-   0        0        0     6183 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/CodeChat_Client/static/splitter.js
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.182431 CodeChat_Server-0.2.9/CodeChat_Server/CodeChat_Client/templates/
+-rw-rw-rw-   0        0        0     3151 2022-12-07 21:00:03.000000 CodeChat_Server-0.2.9/CodeChat_Server/CodeChat_Client/templates/CodeChat_client.html
+-rw-rw-rw-   0        0        0     1229 2022-08-31 04:12:06.000000 CodeChat_Server-0.2.9/CodeChat_Server/CodeChat_Client/templates/insecure.html
+-rw-rw-rw-   0        0        0     1258 2022-12-16 00:42:28.000000 CodeChat_Server-0.2.9/CodeChat_Server/__init__.py
+-rw-rw-rw-   0        0        0    15014 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/__main__.py
+-rw-rw-rw-   0        0        0      482 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/constants.py
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.187428 CodeChat_Server-0.2.9/CodeChat_Server/gen_py/
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.200753 CodeChat_Server-0.2.9/CodeChat_Server/gen_py/CodeChat_Services/
+-rw-rw-rw-   0        0        0    28216 2022-08-31 04:12:06.000000 CodeChat_Server-0.2.9/CodeChat_Server/gen_py/CodeChat_Services/EditorPlugin.py
+-rw-rw-rw-   0        0        0       51 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/gen_py/CodeChat_Services/__init__.py
+-rw-rw-rw-   0        0        0      401 2022-08-31 04:12:06.000000 CodeChat_Server-0.2.9/CodeChat_Server/gen_py/CodeChat_Services/constants.py
+-rw-rw-rw-   0        0        0     3895 2022-08-31 04:12:06.000000 CodeChat_Server-0.2.9/CodeChat_Server/gen_py/CodeChat_Services/ttypes.py
+-rw-rw-rw-   0        0        0        0 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/gen_py/__init__.py
+-rw-rw-rw-   0        0        0    26823 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/render_manager.py
+-rw-rw-rw-   0        0        0    29440 2022-12-15 21:04:55.000000 CodeChat_Server-0.2.9/CodeChat_Server/renderer.py
+-rw-rw-rw-   0        0        0    18045 2022-12-13 17:48:48.000000 CodeChat_Server-0.2.9/CodeChat_Server/server.py
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.100427 CodeChat_Server-0.2.9/CodeChat_Server/templates/
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.211426 CodeChat_Server-0.2.9/CodeChat_Server/templates/doxygen/
+-rw-rw-rw-   0        0        0   118862 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/doxygen/Doxyfile
+-rw-rw-rw-   0        0        0     2433 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/doxygen/codechat_config.yaml
+-rw-rw-rw-   0        0        0     1024 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/doxygen/main.c
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.220429 CodeChat_Server-0.2.9/CodeChat_Server/templates/javadoc/
+-rw-rw-rw-   0        0        0      839 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/javadoc/Simple.java
+-rw-rw-rw-   0        0        0     2465 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/javadoc/codechat_config.yaml
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.228438 CodeChat_Server-0.2.9/CodeChat_Server/templates/mdbook/
+-rw-rw-rw-   0        0        0        6 2022-07-05 20:44:18.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/mdbook/.gitignore
+-rw-rw-rw-   0        0        0     1174 2022-07-05 20:44:18.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/mdbook/book.toml
+-rw-rw-rw-   0        0        0     2400 2022-07-05 20:44:18.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/mdbook/codechat_config.yaml
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.246427 CodeChat_Server-0.2.9/CodeChat_Server/templates/mdbook/src/
+-rw-rw-rw-   0        0        0      201 2022-08-31 04:12:06.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/mdbook/src/SUMMARY.md
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.251427 CodeChat_Server-0.2.9/CodeChat_Server/templates/mdbook/src/__pycache__/
+-rw-rw-rw-   0        0        0      223 2022-07-05 20:44:15.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/mdbook/src/__pycache__/chapter_2.cpython-38.pyc
+-rw-rw-rw-   0        0        0      222 2022-07-05 20:44:18.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/mdbook/src/book.toml
+-rw-rw-rw-   0        0        0      882 2022-07-05 20:44:18.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/mdbook/src/chapter_1.md
+-rw-rw-rw-   0        0        0      263 2022-07-05 20:44:18.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/mdbook/src/chapter_2.py
+-rw-rw-rw-   0        0        0      487 2022-07-05 20:44:18.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/mdbook/src/codechat-config.yaml
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.258426 CodeChat_Server-0.2.9/CodeChat_Server/templates/mkdocs/
+-rw-rw-rw-   0        0        0     2433 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/mkdocs/codechat_config.yaml
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.261430 CodeChat_Server-0.2.9/CodeChat_Server/templates/mkdocs/docs/
+-rw-rw-rw-   0        0        0     1014 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/mkdocs/docs/index.md
+-rw-rw-rw-   0        0        0       20 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/mkdocs/mkdocs.yml
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.277426 CodeChat_Server-0.2.9/CodeChat_Server/templates/pretext/
+-rw-rw-rw-   0        0        0      172 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/pretext/.gitignore
+-rw-rw-rw-   0        0        0      224 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/pretext/README.md
+-rw-rw-rw-   0        0        0     2452 2022-08-31 04:12:06.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/pretext/codechat_config.yaml
+-rw-rw-rw-   0        0        0     1273 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/pretext/project.ptx
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.280439 CodeChat_Server-0.2.9/CodeChat_Server/templates/pretext/publication/
+-rw-rw-rw-   0        0        0     3485 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/pretext/publication/publication.ptx
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.285427 CodeChat_Server-0.2.9/CodeChat_Server/templates/pretext/source/
+-rw-rw-rw-   0        0        0     4494 2022-08-31 04:12:06.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/pretext/source/minimal.ptx
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.297426 CodeChat_Server-0.2.9/CodeChat_Server/templates/runestone/
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.300427 CodeChat_Server-0.2.9/CodeChat_Server/templates/runestone/_sources/
+-rw-rw-rw-   0        0        0     4899 2022-07-05 20:44:18.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/runestone/_sources/index.rst
+-rw-rw-rw-   0        0        0     2499 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/runestone/codechat_config.yaml
+-rw-rw-rw-   0        0        0    12309 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/runestone/conf.py
+-rw-rw-rw-   0        0        0     2090 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/runestone/pavement.py
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.311428 CodeChat_Server-0.2.9/CodeChat_Server/templates/sphinx/
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.314428 CodeChat_Server-0.2.9/CodeChat_Server/templates/sphinx/__pycache__/
+-rw-rw-rw-   0        0        0      979 2022-07-05 20:44:14.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/sphinx/__pycache__/conf.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3097 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/sphinx/codechat_config.yaml
+-rw-rw-rw-   0        0        0    14432 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/sphinx/conf.py
+-rw-rw-rw-   0        0        0     1271 2022-07-05 20:44:17.000000 CodeChat_Server-0.2.9/CodeChat_Server/templates/sphinx/index.rst
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.155428 CodeChat_Server-0.2.9/CodeChat_Server.egg-info/
+-rw-rw-rw-   0        0        0     3545 2022-12-16 00:43:24.000000 CodeChat_Server-0.2.9/CodeChat_Server.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2700 2022-12-16 00:43:25.000000 CodeChat_Server-0.2.9/CodeChat_Server.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-16 00:43:24.000000 CodeChat_Server-0.2.9/CodeChat_Server.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2022-12-16 00:43:24.000000 CodeChat_Server-0.2.9/CodeChat_Server.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      131 2022-12-16 00:43:24.000000 CodeChat_Server-0.2.9/CodeChat_Server.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2022-12-16 00:43:24.000000 CodeChat_Server-0.2.9/CodeChat_Server.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1694 2022-01-29 23:01:37.000000 CodeChat_Server-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3545 2022-12-16 00:43:25.324439 CodeChat_Server-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2486 2022-01-29 23:01:40.000000 CodeChat_Server-0.2.9/README.rst
+drwxrwxrwx   0        0        0        0 2022-12-16 00:43:25.320427 CodeChat_Server-0.2.9/docs/
+-rw-rw-rw-   0        0        0    35998 2020-08-10 17:03:41.000000 CodeChat_Server-0.2.9/docs/LICENSE.rst
+-rw-rw-rw-   0        0        0      641 2022-01-29 17:45:44.000000 CodeChat_Server-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0      682 2022-12-16 00:43:25.326429 CodeChat_Server-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     5962 2022-12-07 20:00:18.000000 CodeChat_Server-0.2.9/setup.py
```

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/CodeChat_Client/static/CodeChat_client.css` & `CodeChat_Server-0.2.9/CodeChat_Server/CodeChat_Client/static/CodeChat_client.css`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/CodeChat_Client/static/CodeChat_client.js` & `CodeChat_Server-0.2.9/CodeChat_Server/CodeChat_Client/static/CodeChat_client.js`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/CodeChat_Client/static/ReconnectingWebsocket.js` & `CodeChat_Server-0.2.9/CodeChat_Server/CodeChat_Client/static/ReconnectingWebsocket.js`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/CodeChat_Client/static/splitter.css` & `CodeChat_Server-0.2.9/CodeChat_Server/CodeChat_Client/static/splitter.css`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/CodeChat_Client/static/splitter.js` & `CodeChat_Server-0.2.9/CodeChat_Server/CodeChat_Client/static/splitter.js`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/CodeChat_Client/templates/CodeChat_client.html` & `CodeChat_Server-0.2.9/CodeChat_Server/CodeChat_Client/templates/CodeChat_client.html`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/CodeChat_Client/templates/insecure.html` & `CodeChat_Server-0.2.9/CodeChat_Server/CodeChat_Client/templates/insecure.html`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/__init__.py` & `CodeChat_Server-0.2.9/CodeChat_Server/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #
 # *****************************
 # |docname| - Module definition
 # *****************************
 # Give the version number, which is read by `../setup.py` during packaging.
 # This is chosen following the `version convention
 # <http://packaging.python.org/en/latest/tutorial.html#version>`_.
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 
 # Contents:
 #
 # .. toctree::
 #   :maxdepth: 2
 #
 #   server.py
```

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/__main__.py` & `CodeChat_Server-0.2.9/CodeChat_Server/__main__.py`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/gen_py/CodeChat_Services/EditorPlugin.py` & `CodeChat_Server-0.2.9/CodeChat_Server/gen_py/CodeChat_Services/EditorPlugin.py`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/gen_py/CodeChat_Services/ttypes.py` & `CodeChat_Server-0.2.9/CodeChat_Server/gen_py/CodeChat_Services/ttypes.py`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/render_manager.py` & `CodeChat_Server-0.2.9/CodeChat_Server/render_manager.py`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/renderer.py` & `CodeChat_Server-0.2.9/CodeChat_Server/renderer.py`

 * *Files 3% similar despite different names*

```diff
@@ -244,21 +244,36 @@
     general = auto()
     PreTeXt = auto()
     Doxygen = auto()
 
 
 # This class reads and interprets a project configuration file.
 class ProjectConfFile:
+    # The type of the project declared in this project's configuration file.
+    project_type: ProjectTypeEnum
+    # The absolute path to this project's root directory.
+    project_path: Path
+    # The extension for HTML files.
+    html_ext: str
+    # The absolute path to this project's source files.
+    source_path: Path
+    # The absolute path to this project's output files.
+    output_path: Path
+    # Arguments used to invoke this project's renderer.
+    args: Union[list, str]
+
     # Read and process a CodeChat project configuration file.
-    def __init__(self, project_path: Path):
+    def __init__(self, project_config_file_path: Path):
         try:
-            with open(project_path, encoding="utf-8") as f:
+            with open(project_config_file_path, encoding="utf-8") as f:
                 data = f.read()
         except Exception as e:
-            raise RuntimeError(f"{project_path}:: ERROR: Unable to open. {e}")
+            raise RuntimeError(
+                f"{project_config_file_path}:: ERROR: Unable to open. {e}"
+            )
 
         schema = strictyaml.Map(
             {
                 strictyaml.Optional("source_path", default="."): strictyaml.Str(),
                 "output_path": strictyaml.Str(),
                 "args": strictyaml.Str() | strictyaml.Seq(strictyaml.Str()),
                 strictyaml.Optional("html_ext", default=".html"): strictyaml.Str(),
@@ -266,36 +281,38 @@
                     [x.name for x in list(ProjectTypeEnum)]
                 ),
             }
         )
         try:
             data_dict = strictyaml.load(data, schema).data
         except strictyaml.YAMLError as e:
-            raise RuntimeError(f"{project_path}:: ERROR: Unable to parse. {e}")
+            raise RuntimeError(
+                f"{project_config_file_path}:: ERROR: Unable to parse. {e}"
+            )
 
         # Save items that don't need processing.
         self.project_type = ProjectTypeEnum[data_dict["project_type"]]
         self.html_ext = data_dict["html_ext"]
 
         # Make paths absolute.
-        project_path = project_path.parent
+        self.project_path = project_config_file_path.parent
 
         def abs_path(path: Union[str, Path]) -> Path:
             path_ = Path(path)
             if not path_.is_absolute():
-                path_ = project_path / path_
+                path_ = self.project_path / path_
             return path_
 
         self.source_path = abs_path(data_dict["source_path"])
         self.output_path = abs_path(data_dict["output_path"])
 
         # Perform replacement on the args.
         def args_format(arg):
             return arg.format(
-                project_path=project_path,
+                project_path=self.project_path,
                 source_path=self.source_path,
                 output_path=self.output_path,
                 sys_executable=sys.executable,
             )
 
         args = data_dict["args"]
         self.args = (
@@ -339,16 +356,18 @@
         # For PreTeXt, use the mapping of source files to XML IDs == output file name.
         if self.project_type == ProjectTypeEnum.PreTeXt:
             try:
                 mapping = self.load_pretext_mapping()
             except Exception:
                 pass
             else:
-                # Before looking up the file, ``resolve()`` it to get the canonical representation (fix case on Windows).
-                xml_id_list = mapping.get(str(source_file.resolve()))
+                # Before looking up the file, ``resolve()`` it to get the canonical representation (fix case on Windows), then make this relative to the project directory.
+                xml_id_list = mapping.get(
+                    str(source_file.resolve().relative_to(self.project_path))
+                )
                 if xml_id_list:
                     # See if any of the mappings match the currently-displayed file. If so, use that one. Otherwise, pick the first mapping.
                     for id_ in reversed(xml_id_list):
                         base_html_file = self.output_path / id_
                         if html_path and base_html_file == html_path.with_suffix(""):
                             break
         # For Doxygen, rename certain characters in the file name. See `util.cpp::escapeCharsInString <https://github.com/doxygen/doxygen/blob/master/src/util.cpp#L3443>`_.
@@ -421,15 +440,15 @@
                 error_arr
                 + [
                     f"{source_file}:: ERROR: CodeChat renderer - unable to check modification time of the HTML file {html_file}: {e}."
                 ],
             )
 
     def load_pretext_mapping(self):
-        return json.loads((self.output_path / "mapping.json").read_text())
+        return json.loads((self.output_path / ".mapping.json").read_text())
 
 
 # Convert an project using an external renderer.
 async def _render_external_project(
     # See text_.
     text: str,
     # See file_path_.
@@ -442,14 +461,17 @@
 ) -> Tuple[str, str]:
     # Run from the directory containing the project file.
     project_conf_file_path = Path(_tool_or_project_path)
     await co_build(
         f"Loading project file {project_conf_file_path}.\n",
     )
 
+    # The ``text`` argument isn't used, since this is an external project, meaning that everything must be saved to disk, instead of rendering the ``text`` currently being edited.
+    del text
+
     # Read the project configuration.
     try:
         project_conf = ProjectConfFile(project_conf_file_path)
     except RuntimeError as e:
         return "", str(e)
 
     file_path = Path(file_path_)
@@ -639,49 +661,50 @@
         ),
     }
 )
 
 
 # Return the converter for the provided file.
 def _select_renderer(
+    # See file_path_.
     file_path: Path,
 ) -> Tuple[
     # _`renderer`: a function or coroutine which will perform the render.
     Callable,
-    # tool_or_project_path:
+    # tool_or_project_config_file_path:
     #
     # - The path to the CodeChat System configuration file if this is a project.
     # - A sequence of parameters used to invoke a single-file renderer if one was found.
     # - None if no renderer was found for ``file_path``.
     Union[str, List[Union[bool, str]], None],
     # is_project: True if this is a project; False if not.
     bool,
 ]:
     # If this is a directory, start searching there. Otherwise, assume it's a file and remove the file name to produce a directory.
     project_path_search = file_path if file_path.is_dir() else file_path.parent
 
     # Search for an external builder configuration file. I can't find an equivalent of `parents <https://docs.python.org/3/library/pathlib.html#pathlib.PurePath.parents>`_ that includes the full path, so the list below constructs it.
     for project_path in [project_path_search, *project_path_search.parents]:
-        project_file = project_path / "codechat_config.yaml"
-        if project_file.exists():
-            return _render_external_project, str(project_file), True
+        project_config_file_path = project_path / "codechat_config.yaml"
+        if project_config_file_path.exists():
+            return _render_external_project, str(project_config_file_path), True
 
     # Otherwise, look for a single-file converter.
     str_file_path = str(file_path)
-    for glob, (converter, tool_or_project_path) in GLOB_TO_RENDERER.items():
+    for glob, (converter, tool_or_project_config_file_path) in GLOB_TO_RENDERER.items():
         if fnmatch.fnmatch(str_file_path, glob):
-            return converter, tool_or_project_path, False
+            return converter, tool_or_project_config_file_path, False
     return _error_renderer, None, False
 
 
 # Run the appropriate converter for the provided file or return an error.
 async def render_file(
     # _`text`: The text to be converted. If this is a project, the text will be loaded from the disk by the external renderer instead.
     text: str,
-    # _`file_path`: The path to the file which (mostly -- see ``is_dirty``) contains this text.
+    # _`file_path`: The path to the file which (mostly -- see ``is_dirty``) contains this text OR a directory containing a CodeChat project.
     file_path: str,
     # _`html_path`: The html file currently being displayed (if available).
     html_path: Optional[Path],
     # _`co_build`: A coroutine that an external renderer should call to stream build output.
     co_build: Co_Build,
     # True if the provided text hasn't been saved to disk.
     is_dirty: bool,
```

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/server.py` & `CodeChat_Server-0.2.9/CodeChat_Server/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
             )
         )
         if self.render_manager.threadsafe_start_render(text, path, id, is_dirty):
             # Indicate success.
             logger.info(" => (empty string)")
             return ""
         else:
-            # If the client specified an non-existant ID, create it.
+            # If the client specified an non-existent ID, create it.
             if id < 0:
                 if self.render_manager.threadsafe_create_client(id) != id:
                     ret = f"Duplicate id {id}."
                     logger.info(f" => {ret}")
                     return ret
                 else:
                     # Since we just created this id, start the CodeChat Client in an external browser.
```

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/doxygen/Doxyfile` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/doxygen/Doxyfile`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/doxygen/codechat_config.yaml` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/doxygen/codechat_config.yaml`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/doxygen/main.c` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/doxygen/main.c`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/javadoc/Simple.java` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/javadoc/Simple.java`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/javadoc/codechat_config.yaml` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/javadoc/codechat_config.yaml`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/mdbook/book.toml` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/mdbook/book.toml`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/mdbook/codechat_config.yaml` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/mdbook/codechat_config.yaml`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/mdbook/src/chapter_1.md` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/mdbook/src/chapter_1.md`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/mkdocs/codechat_config.yaml` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/mkdocs/codechat_config.yaml`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/mkdocs/docs/index.md` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/mkdocs/docs/index.md`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/pretext/codechat_config.yaml` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/pretext/codechat_config.yaml`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/pretext/project.ptx` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/pretext/project.ptx`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/pretext/publication/publication.ptx` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/pretext/publication/publication.ptx`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/pretext/source/minimal.ptx` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/pretext/source/minimal.ptx`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/runestone/_sources/index.rst` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/runestone/_sources/index.rst`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/runestone/codechat_config.yaml` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/runestone/codechat_config.yaml`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/runestone/conf.py` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/runestone/conf.py`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/runestone/pavement.py` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/runestone/pavement.py`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/sphinx/__pycache__/conf.cpython-38.pyc` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/sphinx/__pycache__/conf.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/sphinx/codechat_config.yaml` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/sphinx/codechat_config.yaml`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/sphinx/conf.py` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server/templates/sphinx/index.rst` & `CodeChat_Server-0.2.9/CodeChat_Server/templates/sphinx/index.rst`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server.egg-info/PKG-INFO` & `CodeChat_Server-0.2.9/CodeChat_Server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodeChat-Server
-Version: 0.2.8
+Version: 0.2.9
 Summary: The CodeChat Server for software documentation
 Home-page: http://codechat.readthedocs.io/en/latest/
 Author: Bryan A. Jones
 Author-email: bjones@ece.msstate.edu
 License: GPLv3+
 Keywords: literate programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `CodeChat_Server-0.2.8/CodeChat_Server.egg-info/SOURCES.txt` & `CodeChat_Server-0.2.9/CodeChat_Server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/MANIFEST.in` & `CodeChat_Server-0.2.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/PKG-INFO` & `CodeChat_Server-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodeChat_Server
-Version: 0.2.8
+Version: 0.2.9
 Summary: The CodeChat Server for software documentation
 Home-page: http://codechat.readthedocs.io/en/latest/
 Author: Bryan A. Jones
 Author-email: bjones@ece.msstate.edu
 License: GPLv3+
 Keywords: literate programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `CodeChat_Server-0.2.8/README.rst` & `CodeChat_Server-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/docs/LICENSE.rst` & `CodeChat_Server-0.2.9/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/pyproject.toml` & `CodeChat_Server-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/setup.cfg` & `CodeChat_Server-0.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `CodeChat_Server-0.2.8/setup.py` & `CodeChat_Server-0.2.9/setup.py`

 * *Files identical despite different names*

