# Comparing `tmp/agenta-0.1.7.tar.gz` & `tmp/agenta-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agenta-0.1.7.tar", max compression
+gzip compressed data, was "agenta-0.1.8.tar", max compression
```

## Comparing `agenta-0.1.7.tar` & `agenta-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,30 @@
--rw-r--r--   0        0        0      187 2023-05-31 15:39:19.179107 agenta-0.1.7/README.md
--rw-r--r--   0        0        0       48 2023-06-07 08:35:40.016460 agenta-0.1.7/agenta/__init__.py
--rw-r--r--   0        0        0     3198 2023-06-07 08:35:40.016930 agenta-0.1.7/agenta/agenta.py
--rw-r--r--   0        0        0     2378 2023-06-05 14:29:35.924380 agenta-0.1.7/agenta/cli/helper.py
--rw-r--r--   0        0        0     2108 2023-06-05 14:29:35.924670 agenta-0.1.7/agenta/cli/main.py
--rw-r--r--   0        0        0     8450 2023-06-05 14:29:35.924942 agenta-0.1.7/agenta/cli/variant_commands.py
--rw-r--r--   0        0        0      131 2023-05-15 11:40:40.483678 agenta-0.1.7/agenta/client/Readme.md
--rw-r--r--   0        0        0        0 2023-05-15 11:36:10.263480 agenta-0.1.7/agenta/client/__init__.py
--rw-r--r--   0        0        0      325 2023-05-26 07:42:52.867662 agenta-0.1.7/agenta/client/api_models.py
--rw-r--r--   0        0        0     4355 2023-06-05 14:29:35.925335 agenta-0.1.7/agenta/client/client.py
--rw-r--r--   0        0        0      641 2023-06-05 14:29:35.925644 agenta-0.1.7/agenta/config.py
--rw-r--r--   0        0        0      131 2023-06-05 14:29:35.926009 agenta-0.1.7/agenta/config.toml
--rw-r--r--   0        0        0      372 2023-06-07 09:28:19.623624 agenta-0.1.7/agenta/docker/docker-assets/Dockerfile.template
--rw-r--r--   0        0        0      102 2023-05-11 15:47:22.031685 agenta-0.1.7/agenta/docker/docker-assets/README.md
--rwxr-xr-x   0        0        0       43 2023-06-07 09:27:57.848261 agenta-0.1.7/agenta/docker/docker-assets/entrypoint.sh
--rw-r--r--   0        0        0      239 2023-06-07 09:45:05.306275 agenta-0.1.7/agenta/docker/docker-assets/main.py
--rw-r--r--   0        0        0     2804 2023-06-07 09:47:39.138898 agenta-0.1.7/agenta/docker/docker_utils.py
--rw-r--r--   0        0        0       43 2023-06-07 08:37:18.934913 agenta-0.1.7/agenta/templates/simple_prompt/.env.example
--rw-r--r--   0        0        0      482 2023-05-31 17:12:43.842983 agenta-0.1.7/agenta/templates/simple_prompt/README.md
--rw-r--r--   0        0        0      660 2023-05-31 17:02:48.853909 agenta-0.1.7/agenta/templates/simple_prompt/app.py
--rw-r--r--   0        0        0       31 2023-05-10 09:29:53.673600 agenta-0.1.7/agenta/templates/simple_prompt/requirements.txt
--rw-r--r--   0        0        0       60 2023-05-15 11:25:55.227110 agenta-0.1.7/agenta/templates/simple_prompt/template.toml
--rw-r--r--   0        0        0      570 2023-06-07 11:00:17.459057 agenta-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 agenta-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-05-31 15:39:19.179107 agenta-0.1.8/README.md
+-rw-r--r--   0        0        0      167 2023-06-15 11:20:19.125778 agenta-0.1.8/agenta/__init__.py
+-rw-r--r--   0        0        0     2378 2023-06-05 14:29:35.924380 agenta-0.1.8/agenta/cli/helper.py
+-rw-r--r--   0        0        0     2108 2023-06-05 14:29:35.924670 agenta-0.1.8/agenta/cli/main.py
+-rw-r--r--   0        0        0     9048 2023-06-14 16:46:45.333385 agenta-0.1.8/agenta/cli/variant_commands.py
+-rw-r--r--   0        0        0      131 2023-05-15 11:40:40.483678 agenta-0.1.8/agenta/client/Readme.md
+-rw-r--r--   0        0        0        0 2023-05-15 11:36:10.263480 agenta-0.1.8/agenta/client/__init__.py
+-rw-r--r--   0        0        0      325 2023-05-26 07:42:52.867662 agenta-0.1.8/agenta/client/api_models.py
+-rw-r--r--   0        0        0     4355 2023-06-05 14:29:35.925335 agenta-0.1.8/agenta/client/client.py
+-rw-r--r--   0        0        0      641 2023-06-14 09:00:50.278508 agenta-0.1.8/agenta/config.py
+-rw-r--r--   0        0        0      131 2023-06-14 09:00:50.278836 agenta-0.1.8/agenta/config.toml
+-rw-r--r--   0        0        0     3556 2023-06-13 16:45:28.867392 agenta-0.1.8/agenta/docker/backup.py
+-rw-r--r--   0        0        0      416 2023-06-14 16:37:25.543970 agenta-0.1.8/agenta/docker/docker-assets/Dockerfile.template
+-rw-r--r--   0        0        0      102 2023-05-11 15:47:22.031685 agenta-0.1.8/agenta/docker/docker-assets/README.md
+-rwxr-xr-x   0        0        0       43 2023-06-07 09:27:57.848261 agenta-0.1.8/agenta/docker/docker-assets/entrypoint.sh
+-rw-r--r--   0        0        0      325 2023-06-14 16:38:07.035581 agenta-0.1.8/agenta/docker/docker-assets/main.py
+-rw-r--r--   0        0        0     2905 2023-06-15 11:41:57.531394 agenta-0.1.8/agenta/docker/docker_utils.py
+-rw-r--r--   0        0        0      241 2023-06-15 11:10:04.129954 agenta-0.1.8/agenta/sdk/__init__.py
+-rw-r--r--   0        0        0     6531 2023-06-15 11:10:04.140988 agenta-0.1.8/agenta/sdk/agenta.py
+-rw-r--r--   0        0        0      864 2023-06-15 11:10:04.152507 agenta-0.1.8/agenta/sdk/context.py
+-rw-r--r--   0        0        0       87 2023-06-15 11:10:04.169035 agenta-0.1.8/agenta/sdk/init.py
+-rw-r--r--   0        0        0      202 2023-06-15 11:40:20.994457 agenta-0.1.8/agenta/sdk/router.py
+-rw-r--r--   0        0        0      760 2023-06-15 11:41:35.771121 agenta-0.1.8/agenta/sdk/types.py
+-rw-r--r--   0        0        0       43 2023-06-07 08:37:18.934913 agenta-0.1.8/agenta/templates/simple_prompt/.env.example
+-rw-r--r--   0        0        0      482 2023-05-31 17:12:43.842983 agenta-0.1.8/agenta/templates/simple_prompt/README.md
+-rw-r--r--   0        0        0      660 2023-05-31 17:02:48.853909 agenta-0.1.8/agenta/templates/simple_prompt/app.py
+-rw-r--r--   0        0        0       31 2023-05-10 09:29:53.673600 agenta-0.1.8/agenta/templates/simple_prompt/requirements.txt
+-rw-r--r--   0        0        0       60 2023-05-15 11:25:55.227110 agenta-0.1.8/agenta/templates/simple_prompt/template.toml
+-rw-r--r--   0        0        0      598 2023-06-15 11:44:11.433222 agenta-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 agenta-0.1.8/PKG-INFO
```

### Comparing `agenta-0.1.7/agenta/cli/helper.py` & `agenta-0.1.8/agenta/cli/helper.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.7/agenta/cli/main.py` & `agenta-0.1.8/agenta/cli/main.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.7/agenta/cli/variant_commands.py` & `agenta-0.1.8/agenta/cli/variant_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,17 +120,32 @@
     else:
         variant_name = questionary.select(
             'Please choose a variant',
             choices=config['variants']
         ).ask()
 
     endpoint = client.start_variant(app_name, variant_name)
+    click.echo("\n" + click.style("Congratulations! 🎉", bold=True, fg='green'))
     click.echo(
-        f"""You app has been deployed locally as an api: {endpoint}/openapi.json \n\n
-Go to the playground to experiment with your app : http://localhost:3000/apps/{app_name}/playground \n"""
+        click.style(f"Your app has been deployed locally as an API. 🚀", fg='cyan') +
+        click.style(f" You can access it here: ", fg='white') +
+        click.style(f"{endpoint}/", bold=True, fg='yellow')
+    )
+
+    click.echo(
+        click.style(f"\nRead the API documentation. 📚", fg='cyan') +
+        click.style(f" It's available at: ", fg='white') +
+        click.style(f"{endpoint}/docs", bold=True, fg='yellow')
+    )
+
+    click.echo(
+        click.style("\nStart experimenting with your app in the playground. 🎮", fg='cyan') +
+        click.style(" Go to: ", fg='white') +
+        click.style(f"http://localhost:3000/apps/{app_name}/playground", bold=True, fg='yellow') +
+        "\n"
     )
 
 
 def remove_variant(variant_name: str, app_folder: str):
     """
     Removes a variant from the server
     Args:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `agenta-0.1.7/agenta/client/client.py` & `agenta-0.1.8/agenta/client/client.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.7/agenta/config.py` & `agenta-0.1.8/agenta/config.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.7/agenta/docker/docker_utils.py` & `agenta-0.1.8/agenta/docker/docker_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,20 +36,21 @@
         The image object
     TODO: Check that the variant name does not exist
     TODO: Deal with different app names (probably we need to look then at multiple tags)
     TODO: Error handling
     """
     # Initialize Docker client
     client = docker.from_env()
+    print(folder)
 
     with TemporaryDirectory() as temp_dir:
         # Create a Dockerfile for the app
         # TODO: Later do this in the temp dir
         dockerfile_path = create_dockerfile(folder)
-        shutil.copy(Path(__file__).parent.parent / "agenta.py", folder)
+        shutil.copytree(Path(__file__).parent.parent / "sdk", folder / "agenta",)
         shutil.copy(Path(__file__).parent /
                     "docker-assets" / "main.py", folder)
         shutil.copy(Path(__file__).parent /
                     "docker-assets" / "entrypoint.sh", folder)
 
         # Copy the app files to a temporary directory
         shutil.copytree(folder, temp_dir, dirs_exist_ok=True)
@@ -58,14 +59,16 @@
         registry = settings.registry
         tag = f"{registry}/{app_name.lower()}_{variant_name.lower()}:latest"
         print("Building Docker image...")
         try:
             image, build_log = client.images.build(
                 path=temp_dir,
                 tag=tag,
+                buildargs={"ROOT_PATH": f"/{app_name}/{variant_name}"},
+
                 rm=True  # Remove intermediate containers after a successful build
             )
 
         except docker.errors.BuildError as ex:
             logger.error("Error building Docker image:\n")
             # Print the build log
             for line in ex.build_log:
```

### Comparing `agenta-0.1.7/agenta/templates/simple_prompt/app.py` & `agenta-0.1.8/agenta/templates/simple_prompt/app.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.7/PKG-INFO` & `agenta-0.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: agenta
-Version: 0.1.7
+Version: 0.1.8
 Summary: Code for the SDK and CLI for the Agenta Lab platform
 Author: Mahmoud Mabrouk
 Author-email: mahmoudmabrouk.mail@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: docker (>=6.1.1,<7.0.0)
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
 Requires-Dist: ipdb (>=0.13.13,<0.14.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # Agenta SDK and CLI 
 
 This directory contains the code source for the python SDK and CLI for Agenta AI.
```

