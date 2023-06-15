# Comparing `tmp/Shandows-1.0.0.tar.gz` & `tmp/Shandows-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shandows-1.0.0.tar", last modified: Thu Jun 15 13:32:36 2023, max compression
+gzip compressed data, was "Shandows-1.1.tar", last modified: Thu Jun 15 13:43:34 2023, max compression
```

## Comparing `Shandows-1.0.0.tar` & `Shandows-1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 13:32:36.877488 Shandows-1.0.0/
--rw-rw-rw-   0        0        0      109 2023-06-15 13:32:36.876492 Shandows-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 13:32:36.876492 Shandows-1.0.0/Shandows.egg-info/
--rw-rw-rw-   0        0        0      109 2023-06-15 13:32:36.000000 Shandows-1.0.0/Shandows.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2023-06-15 13:32:36.000000 Shandows-1.0.0/Shandows.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 13:32:36.000000 Shandows-1.0.0/Shandows.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 13:32:36.000000 Shandows-1.0.0/Shandows.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-06-15 13:32:36.000000 Shandows-1.0.0/Shandows.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2034 2023-06-15 12:56:18.000000 Shandows-1.0.0/Shandows.py
--rw-rw-rw-   0        0        0       42 2023-06-15 13:32:36.877488 Shandows-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      220 2023-06-15 13:32:11.000000 Shandows-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:43:34.178552 Shandows-1.1/
+-rw-rw-rw-   0        0        0      107 2023-06-15 13:43:34.177555 Shandows-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 13:43:34.177555 Shandows-1.1/Shandows.egg-info/
+-rw-rw-rw-   0        0        0      107 2023-06-15 13:43:34.000000 Shandows-1.1/Shandows.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2023-06-15 13:43:34.000000 Shandows-1.1/Shandows.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 13:43:34.000000 Shandows-1.1/Shandows.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 13:43:34.000000 Shandows-1.1/Shandows.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 13:43:34.000000 Shandows-1.1/Shandows.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2036 2023-06-15 13:42:56.000000 Shandows-1.1/Shandows.py
+-rw-rw-rw-   0        0        0       42 2023-06-15 13:43:34.178552 Shandows-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      218 2023-06-15 13:43:18.000000 Shandows-1.1/setup.py
```

### Comparing `Shandows-1.0.0/Shandows.py` & `Shandows-1.1/Shandows.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,19 @@
 			origPa.unlink(True)
 			origPa.symlink_to(destPa, isDir)
 		pass
 
 	def linkApp(self, appTitle: str, jobs: dict):
 		print('\n\n\n[%s]' % appTitle)
 		appDiPa: Path = self.shadowDiPa / ('$' + appTitle)
+		appDiPa.mkdir(exist_ok=True)
+
 		for pa, isDir in jobs.items():
 			origPa = self.homeDiPa / pa
 			destPa = appDiPa / pa
-			destPa.mkdir(exist_ok=True)
 			self.linkPath(origPa, destPa, isDir)
 			pass
 		pass
 
 	def run(self):
 		for appTitle, jobs in self.conf.items():
 			self.linkApp(appTitle, jobs)
```

