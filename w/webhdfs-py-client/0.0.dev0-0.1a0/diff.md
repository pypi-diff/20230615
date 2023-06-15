# Comparing `tmp/webhdfs-py-client-0.0.dev0.tar.gz` & `tmp/webhdfs-py-client-0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webhdfs-py-client-0.0.dev0.tar", last modified: Thu Jun 15 19:07:15 2023, max compression
+gzip compressed data, was "webhdfs-py-client-0.1a0.tar", last modified: Thu Jun 15 19:03:41 2023, max compression
```

## Comparing `webhdfs-py-client-0.0.dev0.tar` & `webhdfs-py-client-0.1a0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 19:07:16.000000 webhdfs-py-client-0.0.dev0/
--rw-rw-rw-   0        0        0     3497 2023-06-15 19:07:16.000000 webhdfs-py-client-0.0.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     2756 2023-06-07 20:51:38.000000 webhdfs-py-client-0.0.dev0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 19:07:16.000000 webhdfs-py-client-0.0.dev0/setup.cfg
--rw-rw-rw-   0        0        0     1707 2023-06-15 19:06:46.000000 webhdfs-py-client-0.0.dev0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:07:16.000000 webhdfs-py-client-0.0.dev0/src/
-drwxrwxrwx   0        0        0        0 2023-06-15 19:07:16.000000 webhdfs-py-client-0.0.dev0/src/webhdfs_py/
--rw-rw-rw-   0        0        0       35 2023-06-15 16:19:56.000000 webhdfs-py-client-0.0.dev0/src/webhdfs_py/__init__.py
--rw-rw-rw-   0        0        0      493 2023-06-01 19:50:36.000000 webhdfs-py-client-0.0.dev0/src/webhdfs_py/errors.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:07:16.000000 webhdfs-py-client-0.0.dev0/src/webhdfs_py/example/
--rw-rw-rw-   0        0        0        0 2023-06-15 14:38:50.000000 webhdfs-py-client-0.0.dev0/src/webhdfs_py/example/__init__.py
--rw-rw-rw-   0        0        0     2483 2023-06-15 15:14:52.000000 webhdfs-py-client-0.0.dev0/src/webhdfs_py/example/example.py
--rw-rw-rw-   0        0        0     1160 2023-06-01 02:02:20.000000 webhdfs-py-client-0.0.dev0/src/webhdfs_py/example/hello.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:07:16.000000 webhdfs-py-client-0.0.dev0/src/webhdfs_py/example/pages/
--rw-rw-rw-   0        0        0     1648 2023-06-15 17:57:58.000000 webhdfs-py-client-0.0.dev0/src/webhdfs_py/example/pages/dataframe.py
--rw-rw-rw-   0        0        0      360 2023-06-15 14:45:00.000000 webhdfs-py-client-0.0.dev0/src/webhdfs_py/example/run.py
--rw-rw-rw-   0        0        0      390 2023-06-01 02:08:52.000000 webhdfs-py-client-0.0.dev0/src/webhdfs_py/example/utils.py
--rw-rw-rw-   0        0        0      406 2023-06-07 19:36:30.000000 webhdfs-py-client-0.0.dev0/src/webhdfs_py/operations.py
--rw-rw-rw-   0        0        0    27361 2023-06-15 15:14:52.000000 webhdfs-py-client-0.0.dev0/src/webhdfs_py/webhdfs.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:07:16.000000 webhdfs-py-client-0.0.dev0/src/webhdfs_py_client.egg-info/
--rw-rw-rw-   0        0        0     3497 2023-06-15 19:07:16.000000 webhdfs-py-client-0.0.dev0/src/webhdfs_py_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      554 2023-06-15 19:07:16.000000 webhdfs-py-client-0.0.dev0/src/webhdfs_py_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 19:07:16.000000 webhdfs-py-client-0.0.dev0/src/webhdfs_py_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-15 19:07:16.000000 webhdfs-py-client-0.0.dev0/src/webhdfs_py_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-15 19:07:16.000000 webhdfs-py-client-0.0.dev0/src/webhdfs_py_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 19:03:42.000000 webhdfs-py-client-0.1a0/
+-rw-rw-rw-   0        0        0     3552 2023-06-15 19:03:42.000000 webhdfs-py-client-0.1a0/PKG-INFO
+-rw-rw-rw-   0        0        0     2756 2023-06-07 20:51:38.000000 webhdfs-py-client-0.1a0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 19:03:42.000000 webhdfs-py-client-0.1a0/setup.cfg
+-rw-rw-rw-   0        0        0     1394 2023-06-15 19:02:50.000000 webhdfs-py-client-0.1a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:03:42.000000 webhdfs-py-client-0.1a0/src/
+drwxrwxrwx   0        0        0        0 2023-06-15 19:03:42.000000 webhdfs-py-client-0.1a0/src/webhdfs_py/
+-rw-rw-rw-   0        0        0       35 2023-06-15 16:19:56.000000 webhdfs-py-client-0.1a0/src/webhdfs_py/__init__.py
+-rw-rw-rw-   0        0        0      493 2023-06-01 19:50:36.000000 webhdfs-py-client-0.1a0/src/webhdfs_py/errors.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:03:42.000000 webhdfs-py-client-0.1a0/src/webhdfs_py/example/
+-rw-rw-rw-   0        0        0        0 2023-06-15 14:38:50.000000 webhdfs-py-client-0.1a0/src/webhdfs_py/example/__init__.py
+-rw-rw-rw-   0        0        0     2483 2023-06-15 15:14:52.000000 webhdfs-py-client-0.1a0/src/webhdfs_py/example/example.py
+-rw-rw-rw-   0        0        0     1160 2023-06-01 02:02:20.000000 webhdfs-py-client-0.1a0/src/webhdfs_py/example/hello.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:03:42.000000 webhdfs-py-client-0.1a0/src/webhdfs_py/example/pages/
+-rw-rw-rw-   0        0        0     1648 2023-06-15 17:57:58.000000 webhdfs-py-client-0.1a0/src/webhdfs_py/example/pages/dataframe.py
+-rw-rw-rw-   0        0        0      360 2023-06-15 14:45:00.000000 webhdfs-py-client-0.1a0/src/webhdfs_py/example/run.py
+-rw-rw-rw-   0        0        0      390 2023-06-01 02:08:52.000000 webhdfs-py-client-0.1a0/src/webhdfs_py/example/utils.py
+-rw-rw-rw-   0        0        0      406 2023-06-07 19:36:30.000000 webhdfs-py-client-0.1a0/src/webhdfs_py/operations.py
+-rw-rw-rw-   0        0        0    27361 2023-06-15 15:14:52.000000 webhdfs-py-client-0.1a0/src/webhdfs_py/webhdfs.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:03:42.000000 webhdfs-py-client-0.1a0/src/webhdfs_py_client.egg-info/
+-rw-rw-rw-   0        0        0     3552 2023-06-15 19:03:42.000000 webhdfs-py-client-0.1a0/src/webhdfs_py_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-06-15 19:03:42.000000 webhdfs-py-client-0.1a0/src/webhdfs_py_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 19:03:42.000000 webhdfs-py-client-0.1a0/src/webhdfs_py_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-15 19:03:42.000000 webhdfs-py-client-0.1a0/src/webhdfs_py_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-15 19:03:42.000000 webhdfs-py-client-0.1a0/src/webhdfs_py_client.egg-info/top_level.txt
```

### Comparing `webhdfs-py-client-0.0.dev0/PKG-INFO` & `webhdfs-py-client-0.1a0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webhdfs-py-client
-Version: 0.0.dev0
+Version: 0.1a0
 Summary: Python wrapper for the Hadoop WebHDFS REST API
 Home-page: 
 Author: Erik Alejandro Abdala
 Author-email: e.ale.abdala@gmail.com
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,55 +16,55 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7, <=3.10
 Description-Content-Type: text/markdown
 
 # webhdfspy
 
 
-## Descripción 📄
+## DescripciÃ³n ðŸ“„
 
-El webhdfspy es una biblioteca que proporciona una interfaz conveniente para interactuar con WebHDFS, el servicio de sistema de archivos distribuido de Hadoop a través de HTTP. Este wrapper simplifica el proceso de realizar operaciones como crear archivos, leer y escribir datos, crear directorios y administrar permisos en el clúster Hadoop utilizando la API de WebHDFS.
+El webhdfspy es una biblioteca que proporciona una interfaz conveniente para interactuar con WebHDFS, el servicio de sistema de archivos distribuido de Hadoop a travÃ©s de HTTP. Este wrapper simplifica el proceso de realizar operaciones como crear archivos, leer y escribir datos, crear directorios y administrar permisos en el clÃºster Hadoop utilizando la API de WebHDFS.
 
-Características principales:
+CaracterÃ­sticas principales:
 
-- Conexión y autenticación sencillas con clústeres Hadoop a través de HTTP.
-- Métodos simples y intuitivos para realizar operaciones básicas de sistema de archivos, como crear, leer y escribir archivos, así como también crear y administrar directorios.
-- Compatibilidad con las operaciones más comunes de WebHDFS, como agregar datos a un archivo existente, obtener información sobre archivos y directorios, cambiar permisos y propietarios, y más.
+- ConexiÃ³n y autenticaciÃ³n sencillas con clÃºsteres Hadoop a travÃ©s de HTTP.
+- MÃ©todos simples y intuitivos para realizar operaciones bÃ¡sicas de sistema de archivos, como crear, leer y escribir archivos, asÃ­ como tambiÃ©n crear y administrar directorios.
+- Compatibilidad con las operaciones mÃ¡s comunes de WebHDFS, como agregar datos a un archivo existente, obtener informaciÃ³n sobre archivos y directorios, cambiar permisos y propietarios, y mÃ¡s.
 - Manejo de errores y excepciones para una experiencia de uso robusta y segura.
 
-El webhdfspy es una herramienta útil para desarrolladores que deseen interactuar con clústeres Hadoop y realizar operaciones en HDFS de forma sencilla y eficiente. 
+El webhdfspy es una herramienta Ãºtil para desarrolladores que deseen interactuar con clÃºsteres Hadoop y realizar operaciones en HDFS de forma sencilla y eficiente. 
 
 ### TODO
 
 - [ ] Generarlizar el proyecto.
 
 ### In Progress
 
 - [ ] Implementar para instalar con PIP
 
-### Done ✓
+### Done âœ“
 
 - [x] Generar el primer desarrollo
 - [X] Implementar 
 
 
 
-##  Tabla de Métodos y Descripciones 📑
+##  Tabla de MÃ©todos y Descripciones ðŸ“‘
 
-| Método | Descripción |
+| MÃ©todo | DescripciÃ³n |
 | ------ | ----------- |
 | create_file | Crea un nuevo archivo en HDFS en la ruta especificada |
 | append_file | Realiza un append de datos en un archivo dentro de HDFS |
 | read_file | Abre el archivo completo (permite guardar en destino), tener en cuenta el peso del archivo |
 | stream_file | Genera un iterable del archivo permitiendo guardar los datos del archivo en bloques |
 | make_dir | Crea un nuevo directorio |
 | rename_file_dir | Renombra un archivo o un directorio |
 | delete_file_dir | Elimina un archivo o directorio |
 | get_file_dir_status | Retorna en JSON el estado de un archivo o directorio (Permisos, replicaciones, etc.) |
-| get_content_summary | Retorna en JSON un resumen de un directorio en específico (Cantidad de archivos, peso, cantidad de archivos) |
+| get_content_summary | Retorna en JSON un resumen de un directorio en especÃ­fico (Cantidad de archivos, peso, cantidad de archivos) |
 | get_file_checksum | Retorna en JSON el checksum y el algoritmo |
 | list_dir | Retorna en JSON el estado de los archivos o directorios de la ruta en HDFS |
 | exists_file_dir | Retorna BOOL si existe el directorio o archivo |
 | set_permission | Setea los permisos de un archivo o directorio |
 | set_owner | Setea el owner y/o el grupo |
```

### Comparing `webhdfs-py-client-0.0.dev0/README.md` & `webhdfs-py-client-0.1a0/README.md`

 * *Files identical despite different names*

### Comparing `webhdfs-py-client-0.0.dev0/setup.py` & `webhdfs-py-client-0.1a0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,15 @@
 from setuptools import setup, find_namespace_packages
 from pathlib import Path
 
 # Load the local files
 
-source_root = Path(".")
-with (source_root / "README.md").open(encoding="utf-8") as f:
-    long_description = f.read()
-
-# Read the requirements
-with (source_root / "requirements.txt").open(encoding="utf8") as f:
-    requirements = f.readlines()
-
-try:
-    version = (source_root / "VERSION").read_text().rstrip("\n")
-except FileNotFoundError:
-    version = "0.0.dev0"
-with open(source_root / "VERSION", "w") as version_file:
-    version_file.write(f"{version}")
+requirements = open("./requirements.txt", 'r').read()
+long_description = open("./README.md", 'r').read()
+version = open('./VERSION', 'r').read().rstrip("\n")
 
 setup(name='webhdfs-py-client',
       version=version,
       description='Python wrapper for the Hadoop WebHDFS REST API',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Erik Alejandro Abdala',
```

### Comparing `webhdfs-py-client-0.0.dev0/src/webhdfs_py/example/example.py` & `webhdfs-py-client-0.1a0/src/webhdfs_py/example/example.py`

 * *Files identical despite different names*

### Comparing `webhdfs-py-client-0.0.dev0/src/webhdfs_py/example/hello.py` & `webhdfs-py-client-0.1a0/src/webhdfs_py/example/hello.py`

 * *Files identical despite different names*

### Comparing `webhdfs-py-client-0.0.dev0/src/webhdfs_py/example/pages/dataframe.py` & `webhdfs-py-client-0.1a0/src/webhdfs_py/example/pages/dataframe.py`

 * *Files identical despite different names*

### Comparing `webhdfs-py-client-0.0.dev0/src/webhdfs_py/webhdfs.py` & `webhdfs-py-client-0.1a0/src/webhdfs_py/webhdfs.py`

 * *Files identical despite different names*

### Comparing `webhdfs-py-client-0.0.dev0/src/webhdfs_py_client.egg-info/PKG-INFO` & `webhdfs-py-client-0.1a0/src/webhdfs_py_client.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webhdfs-py-client
-Version: 0.0.dev0
+Version: 0.1a0
 Summary: Python wrapper for the Hadoop WebHDFS REST API
 Home-page: 
 Author: Erik Alejandro Abdala
 Author-email: e.ale.abdala@gmail.com
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,55 +16,55 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7, <=3.10
 Description-Content-Type: text/markdown
 
 # webhdfspy
 
 
-## Descripción 📄
+## DescripciÃ³n ðŸ“„
 
-El webhdfspy es una biblioteca que proporciona una interfaz conveniente para interactuar con WebHDFS, el servicio de sistema de archivos distribuido de Hadoop a través de HTTP. Este wrapper simplifica el proceso de realizar operaciones como crear archivos, leer y escribir datos, crear directorios y administrar permisos en el clúster Hadoop utilizando la API de WebHDFS.
+El webhdfspy es una biblioteca que proporciona una interfaz conveniente para interactuar con WebHDFS, el servicio de sistema de archivos distribuido de Hadoop a travÃ©s de HTTP. Este wrapper simplifica el proceso de realizar operaciones como crear archivos, leer y escribir datos, crear directorios y administrar permisos en el clÃºster Hadoop utilizando la API de WebHDFS.
 
-Características principales:
+CaracterÃ­sticas principales:
 
-- Conexión y autenticación sencillas con clústeres Hadoop a través de HTTP.
-- Métodos simples y intuitivos para realizar operaciones básicas de sistema de archivos, como crear, leer y escribir archivos, así como también crear y administrar directorios.
-- Compatibilidad con las operaciones más comunes de WebHDFS, como agregar datos a un archivo existente, obtener información sobre archivos y directorios, cambiar permisos y propietarios, y más.
+- ConexiÃ³n y autenticaciÃ³n sencillas con clÃºsteres Hadoop a travÃ©s de HTTP.
+- MÃ©todos simples y intuitivos para realizar operaciones bÃ¡sicas de sistema de archivos, como crear, leer y escribir archivos, asÃ­ como tambiÃ©n crear y administrar directorios.
+- Compatibilidad con las operaciones mÃ¡s comunes de WebHDFS, como agregar datos a un archivo existente, obtener informaciÃ³n sobre archivos y directorios, cambiar permisos y propietarios, y mÃ¡s.
 - Manejo de errores y excepciones para una experiencia de uso robusta y segura.
 
-El webhdfspy es una herramienta útil para desarrolladores que deseen interactuar con clústeres Hadoop y realizar operaciones en HDFS de forma sencilla y eficiente. 
+El webhdfspy es una herramienta Ãºtil para desarrolladores que deseen interactuar con clÃºsteres Hadoop y realizar operaciones en HDFS de forma sencilla y eficiente. 
 
 ### TODO
 
 - [ ] Generarlizar el proyecto.
 
 ### In Progress
 
 - [ ] Implementar para instalar con PIP
 
-### Done ✓
+### Done âœ“
 
 - [x] Generar el primer desarrollo
 - [X] Implementar 
 
 
 
-##  Tabla de Métodos y Descripciones 📑
+##  Tabla de MÃ©todos y Descripciones ðŸ“‘
 
-| Método | Descripción |
+| MÃ©todo | DescripciÃ³n |
 | ------ | ----------- |
 | create_file | Crea un nuevo archivo en HDFS en la ruta especificada |
 | append_file | Realiza un append de datos en un archivo dentro de HDFS |
 | read_file | Abre el archivo completo (permite guardar en destino), tener en cuenta el peso del archivo |
 | stream_file | Genera un iterable del archivo permitiendo guardar los datos del archivo en bloques |
 | make_dir | Crea un nuevo directorio |
 | rename_file_dir | Renombra un archivo o un directorio |
 | delete_file_dir | Elimina un archivo o directorio |
 | get_file_dir_status | Retorna en JSON el estado de un archivo o directorio (Permisos, replicaciones, etc.) |
-| get_content_summary | Retorna en JSON un resumen de un directorio en específico (Cantidad de archivos, peso, cantidad de archivos) |
+| get_content_summary | Retorna en JSON un resumen de un directorio en especÃ­fico (Cantidad de archivos, peso, cantidad de archivos) |
 | get_file_checksum | Retorna en JSON el checksum y el algoritmo |
 | list_dir | Retorna en JSON el estado de los archivos o directorios de la ruta en HDFS |
 | exists_file_dir | Retorna BOOL si existe el directorio o archivo |
 | set_permission | Setea los permisos de un archivo o directorio |
 | set_owner | Setea el owner y/o el grupo |
```

### Comparing `webhdfs-py-client-0.0.dev0/src/webhdfs_py_client.egg-info/SOURCES.txt` & `webhdfs-py-client-0.1a0/src/webhdfs_py_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

