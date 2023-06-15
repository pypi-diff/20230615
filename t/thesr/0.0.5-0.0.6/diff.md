# Comparing `tmp/thesr-0.0.5.tar.gz` & `tmp/thesr-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thesr-0.0.5.tar", last modified: Mon Apr 24 15:10:55 2023, max compression
+gzip compressed data, was "thesr-0.0.6.tar", last modified: Thu Jun 15 20:37:16 2023, max compression
```

## Comparing `thesr-0.0.5.tar` & `thesr-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-04-24 15:10:55.380911 thesr-0.0.5/
--rwxrwxrwx   0 john      (1000) john      (1000)    35147 2023-03-30 21:36:33.000000 thesr-0.0.5/LICENSE.txt
--rwxrwxrwx   0 john      (1000) john      (1000)     3833 2023-04-24 15:10:55.383917 thesr-0.0.5/PKG-INFO
--rwxrwxrwx   0 john      (1000) john      (1000)     3447 2023-04-24 15:10:31.000000 thesr-0.0.5/README.md
--rwxrwxrwx   0 john      (1000) john      (1000)      100 2023-03-30 21:36:33.000000 thesr-0.0.5/pyproject.toml
--rwxrwxrwx   0 john      (1000) john      (1000)       78 2023-04-24 15:10:55.399768 thesr-0.0.5/setup.cfg
--rwxrwxrwx   0 john      (1000) john      (1000)      870 2023-04-24 15:06:28.000000 thesr-0.0.5/setup.py
-drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-04-24 15:10:55.001505 thesr-0.0.5/thesr/
--rwxrwxrwx   0 john      (1000) john      (1000)        0 2023-03-30 21:36:33.000000 thesr-0.0.5/thesr/__init__.py
--rwxrwxrwx   0 john      (1000) john      (1000)     8379 2023-04-24 15:01:30.000000 thesr-0.0.5/thesr/thesr.py
-drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-04-24 15:10:55.320950 thesr-0.0.5/thesr.egg-info/
--rwxrwxrwx   0 john      (1000) john      (1000)     3833 2023-04-24 15:10:54.000000 thesr-0.0.5/thesr.egg-info/PKG-INFO
--rwxrwxrwx   0 john      (1000) john      (1000)      232 2023-04-24 15:10:54.000000 thesr-0.0.5/thesr.egg-info/SOURCES.txt
--rwxrwxrwx   0 john      (1000) john      (1000)        1 2023-04-24 15:10:54.000000 thesr-0.0.5/thesr.egg-info/dependency_links.txt
--rwxrwxrwx   0 john      (1000) john      (1000)       44 2023-04-24 15:10:54.000000 thesr-0.0.5/thesr.egg-info/requires.txt
--rwxrwxrwx   0 john      (1000) john      (1000)        6 2023-04-24 15:10:54.000000 thesr-0.0.5/thesr.egg-info/top_level.txt
+drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-06-15 20:37:16.235585 thesr-0.0.6/
+-rwxrwxrwx   0 john      (1000) john      (1000)    35147 2023-03-30 21:36:33.000000 thesr-0.0.6/LICENSE.txt
+-rwxrwxrwx   0 john      (1000) john      (1000)     5497 2023-06-15 20:37:16.235585 thesr-0.0.6/PKG-INFO
+-rwxrwxrwx   0 john      (1000) john      (1000)     5130 2023-05-17 19:53:14.000000 thesr-0.0.6/README.md
+-rwxrwxrwx   0 john      (1000) john      (1000)      100 2023-06-15 20:34:36.000000 thesr-0.0.6/pyproject.toml
+-rwxrwxrwx   0 john      (1000) john      (1000)       78 2023-06-15 20:37:16.254830 thesr-0.0.6/setup.cfg
+-rwxrwxrwx   0 john      (1000) john      (1000)      870 2023-06-15 20:34:31.000000 thesr-0.0.6/setup.py
+drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-06-15 20:37:15.850430 thesr-0.0.6/thesr/
+-rwxrwxrwx   0 john      (1000) john      (1000)        0 2023-03-30 21:36:33.000000 thesr-0.0.6/thesr/__init__.py
+-rwxrwxrwx   0 john      (1000) john      (1000)     8426 2023-06-15 20:32:49.000000 thesr-0.0.6/thesr/thesr.py
+drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-06-15 20:37:16.167059 thesr-0.0.6/thesr.egg-info/
+-rwxrwxrwx   0 john      (1000) john      (1000)     5497 2023-06-15 20:37:15.000000 thesr-0.0.6/thesr.egg-info/PKG-INFO
+-rwxrwxrwx   0 john      (1000) john      (1000)      232 2023-06-15 20:37:15.000000 thesr-0.0.6/thesr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 john      (1000) john      (1000)        1 2023-06-15 20:37:15.000000 thesr-0.0.6/thesr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 john      (1000) john      (1000)       44 2023-06-15 20:37:15.000000 thesr-0.0.6/thesr.egg-info/requires.txt
+-rwxrwxrwx   0 john      (1000) john      (1000)        6 2023-06-15 20:37:15.000000 thesr-0.0.6/thesr.egg-info/top_level.txt
```

### Comparing `thesr-0.0.5/LICENSE.txt` & `thesr-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thesr-0.0.5/setup.py` & `thesr-0.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="thesr",
-    version="0.0.5",
+    version="0.0.6",
     license="gpl-3.0",
     author="John Hupperts",
     author_email="jrock4503@hotmail.com",
     description="thesaurus (and also dictionary)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/treatmesubj/Thesaurus_Rex",
-    download_url="https://github.com/treatmesubj/Thesaurus_Rex/archive/refs/tags/v0.0.5.tar.gz",
+    download_url="https://github.com/treatmesubj/Thesaurus_Rex/archive/refs/tags/v0.0.6.tar.gz",
     packages=["thesr"],
     package_dir={"Thesaurus_Rex": "thesr"},
     project_urls={
         "Source": "https://github.com/treatmesubj/Thesaurus_Rex",
     },
     install_requires=[
         "requests",
```

### Comparing `thesr-0.0.5/thesr/thesr.py` & `thesr-0.0.6/thesr/thesr.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,25 +70,24 @@
 
 def get_syns_ants(word):
     response = requests.get(f"http://www.thesaurus.com/browse/{word}")
     soup = BeautifulSoup(
         response.text,
         "html.parser",
     )
-    script = re.search(
-        r"<script>[\s\S]*window\.INITIAL_STATE = (.+);[\s\S]*</script>", soup.prettify()
-    ).group(1)
+    script_elem = soup.select_one("script#preloaded-state")
+    script = re.search(r"window.__PRELOADED_STATE__ = ({.*})", script_elem.text).group(1)
     # clean JSON
     script = script.replace(":undefined", ':"undefined"')
     script = script.replace(":null", ':"null"')
 
-    j = json.loads(script)
+    sanjay = json.loads(script)
 
     try:
-        posTabs = j["searchData"]["tunaApiData"]["posTabs"]
+        posTabs = sanjay['tuna']['resultsData']['definitionData']['definitions']
     except TypeError:
         return
 
     homonyms = []
     for tab in posTabs:
         homonyms.append(
             {
```

