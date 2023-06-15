# Comparing `tmp/cpfr-rattlesnake-1.0.2.tar.gz` & `tmp/cpfr-rattlesnake-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpfr-rattlesnake-1.0.2.tar", last modified: Wed Jun  7 21:39:08 2023, max compression
+gzip compressed data, was "cpfr-rattlesnake-1.0.3.tar", last modified: Thu Jun 15 15:36:00 2023, max compression
```

## Comparing `cpfr-rattlesnake-1.0.2.tar` & `cpfr-rattlesnake-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 carsten   (1000) carsten   (1000)        0 2023-06-07 21:39:08.850902 cpfr-rattlesnake-1.0.2/
--rw-rw-r--   0 carsten   (1000) carsten   (1000)      854 2023-02-02 19:41:19.000000 cpfr-rattlesnake-1.0.2/LICENSE
--rw-rw-r--   0 carsten   (1000) carsten   (1000)     3531 2023-06-07 21:39:08.850902 cpfr-rattlesnake-1.0.2/PKG-INFO
-drwxrwxr-x   0 carsten   (1000) carsten   (1000)        0 2023-06-07 21:39:08.850902 cpfr-rattlesnake-1.0.2/cpfr_rattlesnake.egg-info/
--rw-rw-r--   0 carsten   (1000) carsten   (1000)     3531 2023-06-07 21:39:08.000000 cpfr-rattlesnake-1.0.2/cpfr_rattlesnake.egg-info/PKG-INFO
--rw-rw-r--   0 carsten   (1000) carsten   (1000)      298 2023-06-07 21:39:08.000000 cpfr-rattlesnake-1.0.2/cpfr_rattlesnake.egg-info/SOURCES.txt
--rw-rw-r--   0 carsten   (1000) carsten   (1000)        1 2023-06-07 21:39:08.000000 cpfr-rattlesnake-1.0.2/cpfr_rattlesnake.egg-info/dependency_links.txt
--rw-rw-r--   0 carsten   (1000) carsten   (1000)       48 2023-06-07 21:39:08.000000 cpfr-rattlesnake-1.0.2/cpfr_rattlesnake.egg-info/entry_points.txt
--rw-rw-r--   0 carsten   (1000) carsten   (1000)       84 2023-06-07 21:39:08.000000 cpfr-rattlesnake-1.0.2/cpfr_rattlesnake.egg-info/requires.txt
--rw-rw-r--   0 carsten   (1000) carsten   (1000)       12 2023-06-07 21:39:08.000000 cpfr-rattlesnake-1.0.2/cpfr_rattlesnake.egg-info/top_level.txt
--rw-rw-r--   0 carsten   (1000) carsten   (1000)      738 2023-06-07 21:38:43.000000 cpfr-rattlesnake-1.0.2/pyproject.toml
-drwxrwxr-x   0 carsten   (1000) carsten   (1000)        0 2023-06-07 21:39:08.850902 cpfr-rattlesnake-1.0.2/rattlesnake/
--rw-rw-r--   0 carsten   (1000) carsten   (1000)    15400 2023-06-07 20:32:12.000000 cpfr-rattlesnake-1.0.2/rattlesnake/__init__.py
--rw-rw-r--   0 carsten   (1000) carsten   (1000)     3166 2023-06-07 21:38:53.000000 cpfr-rattlesnake-1.0.2/readme.md
--rw-rw-r--   0 carsten   (1000) carsten   (1000)       38 2023-06-07 21:39:08.850902 cpfr-rattlesnake-1.0.2/setup.cfg
+drwxrwxr-x   0 carsten   (1000) carsten   (1000)        0 2023-06-15 15:36:00.504945 cpfr-rattlesnake-1.0.3/
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)      854 2023-02-02 19:41:19.000000 cpfr-rattlesnake-1.0.3/LICENSE
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)     3756 2023-06-15 15:36:00.504945 cpfr-rattlesnake-1.0.3/PKG-INFO
+drwxrwxr-x   0 carsten   (1000) carsten   (1000)        0 2023-06-15 15:36:00.504945 cpfr-rattlesnake-1.0.3/cpfr_rattlesnake.egg-info/
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)     3756 2023-06-15 15:36:00.000000 cpfr-rattlesnake-1.0.3/cpfr_rattlesnake.egg-info/PKG-INFO
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)      298 2023-06-15 15:36:00.000000 cpfr-rattlesnake-1.0.3/cpfr_rattlesnake.egg-info/SOURCES.txt
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)        1 2023-06-15 15:36:00.000000 cpfr-rattlesnake-1.0.3/cpfr_rattlesnake.egg-info/dependency_links.txt
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)       48 2023-06-15 15:36:00.000000 cpfr-rattlesnake-1.0.3/cpfr_rattlesnake.egg-info/entry_points.txt
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)       84 2023-06-15 15:36:00.000000 cpfr-rattlesnake-1.0.3/cpfr_rattlesnake.egg-info/requires.txt
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)       12 2023-06-15 15:36:00.000000 cpfr-rattlesnake-1.0.3/cpfr_rattlesnake.egg-info/top_level.txt
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)      738 2023-06-15 15:35:23.000000 cpfr-rattlesnake-1.0.3/pyproject.toml
+drwxrwxr-x   0 carsten   (1000) carsten   (1000)        0 2023-06-15 15:36:00.504945 cpfr-rattlesnake-1.0.3/rattlesnake/
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)    15934 2023-06-15 15:30:58.000000 cpfr-rattlesnake-1.0.3/rattlesnake/__init__.py
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)     3391 2023-06-15 15:35:11.000000 cpfr-rattlesnake-1.0.3/readme.md
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)       38 2023-06-15 15:36:00.504945 cpfr-rattlesnake-1.0.3/setup.cfg
```

### Comparing `cpfr-rattlesnake-1.0.2/LICENSE` & `cpfr-rattlesnake-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cpfr-rattlesnake-1.0.2/PKG-INFO` & `cpfr-rattlesnake-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpfr-rattlesnake
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple static-site generator for Python3, using markdown and the Jinja2 templating engine
 Author-email: Carsten Pfeffer <pfeffer.carsten@gmail.com>
 Keywords: static site generator,website,gitlab pages,jinja
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -47,11 +47,14 @@
 - By default, `./config.yml` is used as the config file for parameters and template variables. This can be changed by specifying a different file path using the `--config-file` option.
 - The `--watch` option keeps the script running after the build process and watches the source directory for file changes. Further, it starts an HTTP server that serves the built website.
 - The `--port` option allows the user to specify a port if the --watch flag is given. If no custom port is provided, port `8000` is used.
 - The `--additional-config` option can be used in order to load an additional config yaml file that supplement or overrides the default values. This can be useful for different deployment targets.
 
 # Version History
 
+- 1.0.3: introducing meta-variables for page paths
+  - `_target_path` points to the path of the page relative to the website's base url
+  - `_source_path` points to the path of the source file relative to the input directory
 - 1.0.2: Bugfixes
   - directories starting with an underscore are also skipped (not just files)
   - adding date formatting filter to Jinja parser (`{{ some_date | format_date("%d.%m.%Y") }}`)
 - 1.0.0: Initial Implementation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cpfr-rattlesnake Version: 1.0.2 Summary: A simple
+Metadata-Version: 2.1 Name: cpfr-rattlesnake Version: 1.0.3 Summary: A simple
 static-site generator for Python3, using markdown and the Jinja2 templating
 engine Author-email: Carsten Pfeffer
 carsten@gmail.com> Keywords: static site generator,website,gitlab pages,jinja
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE # Rattlesnake Static Site Generator Rattlesnake is a static website
 generator. It is written in the Python programming language and utilizes the
 Jinja templating engine, pySCSS for SCSS support, as well as the pyYaml library
@@ -36,11 +36,14 @@
 using the `--config-file` option. - The `--watch` option keeps the script
 running after the build process and watches the source directory for file
 changes. Further, it starts an HTTP server that serves the built website. - The
 `--port` option allows the user to specify a port if the --watch flag is given.
 If no custom port is provided, port `8000` is used. - The `--additional-config`
 option can be used in order to load an additional config yaml file that
 supplement or overrides the default values. This can be useful for different
-deployment targets. # Version History - 1.0.2: Bugfixes - directories starting
-with an underscore are also skipped (not just files) - adding date formatting
-filter to Jinja parser (`{{ some_date | format_date("%d.%m.%Y") }}`) - 1.0.0:
-Initial Implementation
+deployment targets. # Version History - 1.0.3: introducing meta-variables for
+page paths - `_target_path` points to the path of the page relative to the
+website's base url - `_source_path` points to the path of the source file
+relative to the input directory - 1.0.2: Bugfixes - directories starting with
+an underscore are also skipped (not just files) - adding date formatting filter
+to Jinja parser (`{{ some_date | format_date("%d.%m.%Y") }}`) - 1.0.0: Initial
+Implementation
```

### Comparing `cpfr-rattlesnake-1.0.2/cpfr_rattlesnake.egg-info/PKG-INFO` & `cpfr-rattlesnake-1.0.3/cpfr_rattlesnake.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpfr-rattlesnake
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple static-site generator for Python3, using markdown and the Jinja2 templating engine
 Author-email: Carsten Pfeffer <pfeffer.carsten@gmail.com>
 Keywords: static site generator,website,gitlab pages,jinja
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -47,11 +47,14 @@
 - By default, `./config.yml` is used as the config file for parameters and template variables. This can be changed by specifying a different file path using the `--config-file` option.
 - The `--watch` option keeps the script running after the build process and watches the source directory for file changes. Further, it starts an HTTP server that serves the built website.
 - The `--port` option allows the user to specify a port if the --watch flag is given. If no custom port is provided, port `8000` is used.
 - The `--additional-config` option can be used in order to load an additional config yaml file that supplement or overrides the default values. This can be useful for different deployment targets.
 
 # Version History
 
+- 1.0.3: introducing meta-variables for page paths
+  - `_target_path` points to the path of the page relative to the website's base url
+  - `_source_path` points to the path of the source file relative to the input directory
 - 1.0.2: Bugfixes
   - directories starting with an underscore are also skipped (not just files)
   - adding date formatting filter to Jinja parser (`{{ some_date | format_date("%d.%m.%Y") }}`)
 - 1.0.0: Initial Implementation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cpfr-rattlesnake Version: 1.0.2 Summary: A simple
+Metadata-Version: 2.1 Name: cpfr-rattlesnake Version: 1.0.3 Summary: A simple
 static-site generator for Python3, using markdown and the Jinja2 templating
 engine Author-email: Carsten Pfeffer
 carsten@gmail.com> Keywords: static site generator,website,gitlab pages,jinja
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE # Rattlesnake Static Site Generator Rattlesnake is a static website
 generator. It is written in the Python programming language and utilizes the
 Jinja templating engine, pySCSS for SCSS support, as well as the pyYaml library
@@ -36,11 +36,14 @@
 using the `--config-file` option. - The `--watch` option keeps the script
 running after the build process and watches the source directory for file
 changes. Further, it starts an HTTP server that serves the built website. - The
 `--port` option allows the user to specify a port if the --watch flag is given.
 If no custom port is provided, port `8000` is used. - The `--additional-config`
 option can be used in order to load an additional config yaml file that
 supplement or overrides the default values. This can be useful for different
-deployment targets. # Version History - 1.0.2: Bugfixes - directories starting
-with an underscore are also skipped (not just files) - adding date formatting
-filter to Jinja parser (`{{ some_date | format_date("%d.%m.%Y") }}`) - 1.0.0:
-Initial Implementation
+deployment targets. # Version History - 1.0.3: introducing meta-variables for
+page paths - `_target_path` points to the path of the page relative to the
+website's base url - `_source_path` points to the path of the source file
+relative to the input directory - 1.0.2: Bugfixes - directories starting with
+an underscore are also skipped (not just files) - adding date formatting filter
+to Jinja parser (`{{ some_date | format_date("%d.%m.%Y") }}`) - 1.0.0: Initial
+Implementation
```

### Comparing `cpfr-rattlesnake-1.0.2/pyproject.toml` & `cpfr-rattlesnake-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [project]
 name = "cpfr-rattlesnake"
 authors = [
     { name = "Carsten Pfeffer", email = "pfeffer.carsten@gmail.com" }
 ]
 description = "A simple static-site generator for Python3, using markdown and the Jinja2 templating engine"
-version = "1.0.2"
+version = "1.0.3"
 readme = "readme.md"
 requires-python = ">= 3.7"
 keywords = ["static site generator", "website", "gitlab pages", "jinja"]
 dependencies = [
     "watchdog",
     "jinja2",
     "pyyaml",
```

### Comparing `cpfr-rattlesnake-1.0.2/rattlesnake/__init__.py` & `cpfr-rattlesnake-1.0.3/rattlesnake/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,38 +172,48 @@
 
     def process_file(source_path, target_path, full_path, config, process_dependencies):
         rel_path = os.path.relpath(full_path, source_path)
         file_path = os.path.basename(full_path)
         if os.path.isfile(full_path):
             if not file_path.startswith("_"):
                 target_file_path = get_target_path(rel_path, source_path, target_path)
+                target_path2 = get_target_path(rel_path, source_path, "/")
+                if target_path2.endswith("index.html"):
+                    target_path2 = target_path2[:-10]
+
                 try:
                     os.makedirs(os.path.dirname(target_file_path))
                 except:
                     pass
 
                 if file_path.lower().endswith(".html"):
                     dependencies[file_path] = []
                     print(colored("Processing HTML file %s, target is %s" % (file_path, target_file_path), "blue"))
                     metadata = frontmatter.load(full_path).metadata
+                    metadata["_source_path"] = rel_path
+                    metadata["_target_path"] = target_path2
                     rendered_html = render_template(source_path, {**config, **metadata}, rel_path, dependencies[file_path])
                     with open(target_file_path, "w") as stream:
                         stream.write(rendered_html)
                 elif file_path.lower().endswith(".xml"):
                     dependencies[file_path] = []
                     print(colored("Processing XML file %s, target is %s" % (file_path, target_file_path), "blue"))
                     metadata = frontmatter.load(full_path).metadata
+                    metadata["_source_path"] = rel_path
+                    metadata["_target_path"] = target_path2
                     rendered_xml = render_template(source_path, {**config, **metadata}, rel_path, dependencies[file_path])
                     with open(target_file_path, "w") as stream:
                         stream.write(rendered_xml)
                 elif file_path.lower().endswith(".md") or file_path.lower().endswith(".markdown"):
                     dependencies[file_path] = []
                     print(colored("Processing Markdown file %s, target is %s" % (file_path, target_file_path), "blue"))
                     front_matter = frontmatter.load(full_path)
                     metadata = front_matter.metadata
+                    metadata["_source_path"] = rel_path
+                    metadata["_target_path"] = target_path2
                     rendered_markdown = markdown.markdown(front_matter.content)
 
                     with open(os.path.join(source_path, front_matter["_template"])) as f:
                         template_text = f.read()
                     template_text = content_block_regex.sub("{% block content %}\n" + rendered_markdown + "\n{% endblock %}", template_text)
                     if "_template" in front_matter.keys():
                         dependencies[rel_path] = [front_matter["_template"]]
```

### Comparing `cpfr-rattlesnake-1.0.2/readme.md` & `cpfr-rattlesnake-1.0.3/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -37,11 +37,14 @@
 - By default, `./config.yml` is used as the config file for parameters and template variables. This can be changed by specifying a different file path using the `--config-file` option.
 - The `--watch` option keeps the script running after the build process and watches the source directory for file changes. Further, it starts an HTTP server that serves the built website.
 - The `--port` option allows the user to specify a port if the --watch flag is given. If no custom port is provided, port `8000` is used.
 - The `--additional-config` option can be used in order to load an additional config yaml file that supplement or overrides the default values. This can be useful for different deployment targets.
 
 # Version History
 
+- 1.0.3: introducing meta-variables for page paths
+  - `_target_path` points to the path of the page relative to the website's base url
+  - `_source_path` points to the path of the source file relative to the input directory
 - 1.0.2: Bugfixes
   - directories starting with an underscore are also skipped (not just files)
   - adding date formatting filter to Jinja parser (`{{ some_date | format_date("%d.%m.%Y") }}`)
 - 1.0.0: Initial Implementation
```

#### html2text {}

```diff
@@ -31,11 +31,14 @@
 using the `--config-file` option. - The `--watch` option keeps the script
 running after the build process and watches the source directory for file
 changes. Further, it starts an HTTP server that serves the built website. - The
 `--port` option allows the user to specify a port if the --watch flag is given.
 If no custom port is provided, port `8000` is used. - The `--additional-config`
 option can be used in order to load an additional config yaml file that
 supplement or overrides the default values. This can be useful for different
-deployment targets. # Version History - 1.0.2: Bugfixes - directories starting
-with an underscore are also skipped (not just files) - adding date formatting
-filter to Jinja parser (`{{ some_date | format_date("%d.%m.%Y") }}`) - 1.0.0:
-Initial Implementation
+deployment targets. # Version History - 1.0.3: introducing meta-variables for
+page paths - `_target_path` points to the path of the page relative to the
+website's base url - `_source_path` points to the path of the source file
+relative to the input directory - 1.0.2: Bugfixes - directories starting with
+an underscore are also skipped (not just files) - adding date formatting filter
+to Jinja parser (`{{ some_date | format_date("%d.%m.%Y") }}`) - 1.0.0: Initial
+Implementation
```

