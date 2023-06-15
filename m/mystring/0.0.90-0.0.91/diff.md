# Comparing `tmp/mystring-0.0.90.tar.gz` & `tmp/mystring-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mystring-0.0.90.tar", last modified: Wed May 24 02:00:25 2023, max compression
+gzip compressed data, was "mystring-0.0.91.tar", last modified: Thu Jun 15 02:19:52 2023, max compression
```

## Comparing `mystring-0.0.90.tar` & `mystring-0.0.91.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:00:25.078575 mystring-0.0.90/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-24 02:00:20.000000 mystring-0.0.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-24 02:00:25.078575 mystring-0.0.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-24 02:00:20.000000 mystring-0.0.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:00:25.078575 mystring-0.0.90/mystring/
--rw-r--r--   0 runner    (1001) docker     (123)    17681 2023-05-24 02:00:20.000000 mystring-0.0.90/mystring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:00:25.078575 mystring-0.0.90/mystring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-24 02:00:25.000000 mystring-0.0.90/mystring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-24 02:00:25.000000 mystring-0.0.90/mystring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 02:00:25.000000 mystring-0.0.90/mystring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-24 02:00:25.000000 mystring-0.0.90/mystring.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 02:00:25.000000 mystring-0.0.90/mystring.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 02:00:25.078575 mystring-0.0.90/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3460 2023-05-24 02:00:20.000000 mystring-0.0.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:19:52.844059 mystring-0.0.91/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-15 02:19:47.000000 mystring-0.0.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-15 02:19:52.844059 mystring-0.0.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 02:19:47.000000 mystring-0.0.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:19:52.844059 mystring-0.0.91/mystring/
+-rw-r--r--   0 runner    (1001) docker     (123)    17734 2023-06-15 02:19:47.000000 mystring-0.0.91/mystring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:19:52.844059 mystring-0.0.91/mystring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-15 02:19:52.000000 mystring-0.0.91/mystring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-15 02:19:52.000000 mystring-0.0.91/mystring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 02:19:52.000000 mystring-0.0.91/mystring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 02:19:52.000000 mystring-0.0.91/mystring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 02:19:52.000000 mystring-0.0.91/mystring.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 02:19:52.844059 mystring-0.0.91/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3460 2023-06-15 02:19:47.000000 mystring-0.0.91/setup.py
```

### Comparing `mystring-0.0.90/LICENSE` & `mystring-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `mystring-0.0.90/mystring/__init__.py` & `mystring-0.0.91/mystring/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -625,15 +625,18 @@
 		
 		self.threads.put(obj)
 		obj.start()
 		return self
 	
 	@property
 	def complete(self):
-		return all([not x.isAlive() for x in list(self.threads.queue)])
+		for tread in iter(self.threads.queue, None):
+			if tread != None and tread.isAlive():
+				return False
+		return True
 
 	def wait_until_done(self, printout=False):
 		if printout:
 			print("[",end='',flush=True)
 
 		while not self.complete:
 			time.sleep(1)
```

### Comparing `mystring-0.0.90/setup.py` & `mystring-0.0.91/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.90"
+VERSION = "0.0.91"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

