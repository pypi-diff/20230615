# Comparing `tmp/prelude-cli-1.2.4.tar.gz` & `tmp/prelude-cli-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-cli-1.2.4.tar", last modified: Thu Jun  8 13:37:11 2023, max compression
+gzip compressed data, was "prelude-cli-1.2.5.tar", last modified: Thu Jun 15 14:40:17 2023, max compression
```

## Comparing `prelude-cli-1.2.4.tar` & `prelude-cli-1.2.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-08 13:37:11.401651 prelude-cli-1.2.4/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.2.4/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.2.4/MANIFEST.in
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-06-08 13:37:11.401730 prelude-cli-1.2.4/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.2.4/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-08 13:37:11.398112 prelude-cli-1.2.4/prelude_cli/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.4/prelude_cli/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      775 2023-05-02 14:19:17.000000 prelude-cli-1.2.4/prelude_cli/cli.py
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-05-03 13:30:52.000000 prelude-cli-1.2.4/prelude_cli/spinner.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-08 13:37:11.398974 prelude-cli-1.2.4/prelude_cli/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.4/prelude_cli/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      249 2023-06-01 16:01:25.000000 prelude-cli-1.2.4/prelude_cli/templates/template.go
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-08 13:37:11.401430 prelude-cli-1.2.4/prelude_cli/views/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.4/prelude_cli/views/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     4036 2023-06-06 22:22:58.000000 prelude-cli-1.2.4/prelude_cli/views/build.py
--rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.2.4/prelude_cli/views/configure.py
--rw-r--r--   0 pack       (501) staff       (20)     7960 2023-06-07 20:52:19.000000 prelude-cli-1.2.4/prelude_cli/views/detect.py
--rw-r--r--   0 pack       (501) staff       (20)     3879 2023-06-07 20:52:19.000000 prelude-cli-1.2.4/prelude_cli/views/iam.py
--rw-r--r--   0 pack       (501) staff       (20)     2279 2023-05-18 19:30:30.000000 prelude-cli-1.2.4/prelude_cli/views/partner.py
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-03 13:30:52.000000 prelude-cli-1.2.4/prelude_cli/views/shared.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-08 13:37:11.398784 prelude-cli-1.2.4/prelude_cli.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-06-08 13:37:11.000000 prelude-cli-1.2.4/prelude_cli.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      598 2023-06-08 13:37:11.000000 prelude-cli-1.2.4/prelude_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-06-08 13:37:11.000000 prelude-cli-1.2.4/prelude_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2023-06-08 13:37:11.000000 prelude-cli-1.2.4/prelude_cli.egg-info/entry_points.txt
--rw-r--r--   0 pack       (501) staff       (20)       32 2023-06-08 13:37:11.000000 prelude-cli-1.2.4/prelude_cli.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2023-06-08 13:37:11.000000 prelude-cli-1.2.4/prelude_cli.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.2.4/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      663 2023-06-08 13:37:11.401959 prelude-cli-1.2.4/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-15 14:40:17.097532 prelude-cli-1.2.5/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.2.5/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.2.5/MANIFEST.in
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-06-15 14:40:17.097576 prelude-cli-1.2.5/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.2.5/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-15 14:40:17.094597 prelude-cli-1.2.5/prelude_cli/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.5/prelude_cli/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      775 2023-05-02 14:19:17.000000 prelude-cli-1.2.5/prelude_cli/cli.py
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-05-03 13:30:52.000000 prelude-cli-1.2.5/prelude_cli/spinner.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-15 14:40:17.095378 prelude-cli-1.2.5/prelude_cli/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.5/prelude_cli/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      249 2023-06-01 16:01:25.000000 prelude-cli-1.2.5/prelude_cli/templates/template.go
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-15 14:40:17.097311 prelude-cli-1.2.5/prelude_cli/views/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.5/prelude_cli/views/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     4036 2023-06-06 22:22:58.000000 prelude-cli-1.2.5/prelude_cli/views/build.py
+-rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.2.5/prelude_cli/views/configure.py
+-rw-r--r--   0 pack       (501) staff       (20)     7956 2023-06-12 21:16:47.000000 prelude-cli-1.2.5/prelude_cli/views/detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     3895 2023-06-12 21:16:47.000000 prelude-cli-1.2.5/prelude_cli/views/iam.py
+-rw-r--r--   0 pack       (501) staff       (20)     2279 2023-05-18 19:30:30.000000 prelude-cli-1.2.5/prelude_cli/views/partner.py
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-03 13:30:52.000000 prelude-cli-1.2.5/prelude_cli/views/shared.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-15 14:40:17.095201 prelude-cli-1.2.5/prelude_cli.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-06-15 14:40:17.000000 prelude-cli-1.2.5/prelude_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      598 2023-06-15 14:40:17.000000 prelude-cli-1.2.5/prelude_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-06-15 14:40:17.000000 prelude-cli-1.2.5/prelude_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2023-06-15 14:40:17.000000 prelude-cli-1.2.5/prelude_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pack       (501) staff       (20)       32 2023-06-15 14:40:17.000000 prelude-cli-1.2.5/prelude_cli.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2023-06-15 14:40:17.000000 prelude-cli-1.2.5/prelude_cli.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.2.5/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      663 2023-06-15 14:40:17.097787 prelude-cli-1.2.5/setup.cfg
```

### Comparing `prelude-cli-1.2.4/LICENSE` & `prelude-cli-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.4/PKG-INFO` & `prelude-cli-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.2.4
+Version: 1.2.5
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.2.4/prelude_cli/cli.py` & `prelude-cli-1.2.5/prelude_cli/cli.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.4/prelude_cli/views/build.py` & `prelude-cli-1.2.5/prelude_cli/views/build.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.4/prelude_cli/views/configure.py` & `prelude-cli-1.2.5/prelude_cli/views/configure.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.4/prelude_cli/views/detect.py` & `prelude-cli-1.2.5/prelude_cli/views/detect.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
                     f.write(code)
 
     async def start_cloning():
         await asyncio.gather(*[fetch(test) for test in controller.list_tests()])
 
     with Spinner():
         asyncio.run(start_cloning())
-        click.secho('Project cloned successfully', fg='green')
+    click.secho('Project cloned successfully', fg='green')
 
 
 @detect.command('activity')
 @click.option('-v', '--view',
               help='retrieve a specific result view',
               default='logs', show_default=True,
               type=click.Choice(['logs', 'days', 'insights', 'probes', 'advisories', 'tests', 'metrics']))
```

### Comparing `prelude-cli-1.2.4/prelude_cli/views/iam.py` & `prelude-cli-1.2.5/prelude_cli/views/iam.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,16 @@
 
 @iam.command('account')
 @click.pass_obj
 @handle_api_error
 def describe_account(controller):
     """ Get account details """
     with Spinner():
-        print_json(data=controller.get_account())
+        data = controller.get_account()
+    print_json(data=data)
 
 
 @iam.command('create-user')
 @click.option('-d', '--days', help='days this user will remain active', default=365, type=int)
 @click.option('-p', '--permission', help='user permission level', default=Permission.SERVICE.name,
               type=click.Choice([p.name for p in Permission if p != Permission.INVALID], case_sensitive=False), show_default=True)
 @click.option('-n', '--name', help='name of user', default=None, show_default=False, type=str)
```

### Comparing `prelude-cli-1.2.4/prelude_cli/views/partner.py` & `prelude-cli-1.2.5/prelude_cli/views/partner.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.4/prelude_cli/views/shared.py` & `prelude-cli-1.2.5/prelude_cli/views/shared.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.4/prelude_cli.egg-info/PKG-INFO` & `prelude-cli-1.2.5/prelude_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.2.4
+Version: 1.2.5
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.2.4/prelude_cli.egg-info/SOURCES.txt` & `prelude-cli-1.2.5/prelude_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.4/setup.cfg` & `prelude-cli-1.2.5/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-cli
-version = 1.2.4
+version = 1.2.5
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers = 
@@ -13,15 +13,15 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
-	prelude-sdk == 1.2.4
+	prelude-sdk == 1.2.5
 	click > 8
 	rich
 
 [options.entry_points]
 console_scripts = 
 	prelude = prelude_cli.cli:cli
```

