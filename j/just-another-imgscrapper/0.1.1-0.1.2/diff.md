# Comparing `tmp/just-another-imgscrapper-0.1.1.tar.gz` & `tmp/just-another-imgscrapper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "just-another-imgscrapper-0.1.1.tar", last modified: Tue Jun  6 19:52:08 2023, max compression
+gzip compressed data, was "just-another-imgscrapper-0.1.2.tar", last modified: Thu Jun 15 11:02:07 2023, max compression
```

## Comparing `just-another-imgscrapper-0.1.1.tar` & `just-another-imgscrapper-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 deshrit   (1000) deshrit   (1000)        0 2023-06-06 19:52:08.711888 just-another-imgscrapper-0.1.1/
--rw-r--r--   0 deshrit   (1000) deshrit   (1000)     1070 2023-06-06 19:21:31.000000 just-another-imgscrapper-0.1.1/LICENSE
--rw-r--r--   0 deshrit   (1000) deshrit   (1000)       21 2023-06-06 11:53:22.000000 just-another-imgscrapper-0.1.1/MANIFEST.in
--rw-r--r--   0 deshrit   (1000) deshrit   (1000)     3117 2023-06-06 19:52:08.711888 just-another-imgscrapper-0.1.1/PKG-INFO
--rw-r--r--   0 deshrit   (1000) deshrit   (1000)     2337 2023-06-06 19:35:26.000000 just-another-imgscrapper-0.1.1/README.md
--rw-r--r--   0 deshrit   (1000) deshrit   (1000)     1429 2023-06-06 19:52:08.711888 just-another-imgscrapper-0.1.1/setup.cfg
--rw-r--r--   0 deshrit   (1000) deshrit   (1000)       69 2023-06-06 18:27:21.000000 just-another-imgscrapper-0.1.1/setup.py
-drwxr-xr-x   0 deshrit   (1000) deshrit   (1000)        0 2023-06-06 19:52:08.627887 just-another-imgscrapper-0.1.1/src/
-drwxr-xr-x   0 deshrit   (1000) deshrit   (1000)        0 2023-06-06 19:52:08.691888 just-another-imgscrapper-0.1.1/src/imgscrapper/
--rw-r--r--   0 deshrit   (1000) deshrit   (1000)      185 2023-06-06 19:26:57.000000 just-another-imgscrapper-0.1.1/src/imgscrapper/__init__.py
--rw-r--r--   0 deshrit   (1000) deshrit   (1000)     2079 2023-06-06 18:27:21.000000 just-another-imgscrapper-0.1.1/src/imgscrapper/__main__.py
--rw-r--r--   0 deshrit   (1000) deshrit   (1000)      523 2023-06-06 18:27:21.000000 just-another-imgscrapper-0.1.1/src/imgscrapper/errors.py
--rw-r--r--   0 deshrit   (1000) deshrit   (1000)     5929 2023-06-06 18:44:35.000000 just-another-imgscrapper-0.1.1/src/imgscrapper/imgscrapper.py
--rw-r--r--   0 deshrit   (1000) deshrit   (1000)      425 2023-06-06 17:37:54.000000 just-another-imgscrapper-0.1.1/src/imgscrapper/utils.py
-drwxr-xr-x   0 deshrit   (1000) deshrit   (1000)        0 2023-06-06 19:52:08.703888 just-another-imgscrapper-0.1.1/src/just_another_imgscrapper.egg-info/
--rw-r--r--   0 deshrit   (1000) deshrit   (1000)     3117 2023-06-06 19:52:08.000000 just-another-imgscrapper-0.1.1/src/just_another_imgscrapper.egg-info/PKG-INFO
--rw-r--r--   0 deshrit   (1000) deshrit   (1000)      560 2023-06-06 19:52:08.000000 just-another-imgscrapper-0.1.1/src/just_another_imgscrapper.egg-info/SOURCES.txt
--rw-r--r--   0 deshrit   (1000) deshrit   (1000)        1 2023-06-06 19:52:08.000000 just-another-imgscrapper-0.1.1/src/just_another_imgscrapper.egg-info/dependency_links.txt
--rw-r--r--   0 deshrit   (1000) deshrit   (1000)       58 2023-06-06 19:52:08.000000 just-another-imgscrapper-0.1.1/src/just_another_imgscrapper.egg-info/entry_points.txt
--rw-r--r--   0 deshrit   (1000) deshrit   (1000)      109 2023-06-06 19:52:08.000000 just-another-imgscrapper-0.1.1/src/just_another_imgscrapper.egg-info/requires.txt
--rw-r--r--   0 deshrit   (1000) deshrit   (1000)       12 2023-06-06 19:52:08.000000 just-another-imgscrapper-0.1.1/src/just_another_imgscrapper.egg-info/top_level.txt
-drwxr-xr-x   0 deshrit   (1000) deshrit   (1000)        0 2023-06-06 19:52:08.707888 just-another-imgscrapper-0.1.1/tests/
--rw-r--r--   0 deshrit   (1000) deshrit   (1000)     1118 2023-06-06 11:19:40.000000 just-another-imgscrapper-0.1.1/tests/test_get_html_doc.py
--rw-r--r--   0 deshrit   (1000) deshrit   (1000)     3434 2023-06-06 18:27:21.000000 just-another-imgscrapper-0.1.1/tests/test_img_tag_extraction.py
+drwxrwxr-x   0 deshrit   (1000) deshrit   (1000)        0 2023-06-15 11:02:07.023762 just-another-imgscrapper-0.1.2/
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)     1070 2023-06-08 05:25:44.000000 just-another-imgscrapper-0.1.2/LICENSE
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)       21 2023-06-08 05:25:44.000000 just-another-imgscrapper-0.1.2/MANIFEST.in
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)     3266 2023-06-15 11:02:07.023762 just-another-imgscrapper-0.1.2/PKG-INFO
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)     2486 2023-06-15 10:51:09.000000 just-another-imgscrapper-0.1.2/README.md
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)     1429 2023-06-15 11:02:07.027762 just-another-imgscrapper-0.1.2/setup.cfg
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)       69 2023-06-08 05:25:44.000000 just-another-imgscrapper-0.1.2/setup.py
+drwxrwxr-x   0 deshrit   (1000) deshrit   (1000)        0 2023-06-15 11:02:07.015761 just-another-imgscrapper-0.1.2/src/
+drwxrwxr-x   0 deshrit   (1000) deshrit   (1000)        0 2023-06-15 11:02:07.019761 just-another-imgscrapper-0.1.2/src/imgscrapper/
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)      185 2023-06-08 05:25:44.000000 just-another-imgscrapper-0.1.2/src/imgscrapper/__init__.py
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)     2079 2023-06-08 05:25:44.000000 just-another-imgscrapper-0.1.2/src/imgscrapper/__main__.py
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)      523 2023-06-08 05:25:44.000000 just-another-imgscrapper-0.1.2/src/imgscrapper/errors.py
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)     5929 2023-06-08 05:25:44.000000 just-another-imgscrapper-0.1.2/src/imgscrapper/imgscrapper.py
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)      425 2023-06-08 05:25:44.000000 just-another-imgscrapper-0.1.2/src/imgscrapper/utils.py
+drwxrwxr-x   0 deshrit   (1000) deshrit   (1000)        0 2023-06-15 11:02:07.023762 just-another-imgscrapper-0.1.2/src/just_another_imgscrapper.egg-info/
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)     3266 2023-06-15 11:02:06.000000 just-another-imgscrapper-0.1.2/src/just_another_imgscrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)      560 2023-06-15 11:02:07.000000 just-another-imgscrapper-0.1.2/src/just_another_imgscrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)        1 2023-06-15 11:02:06.000000 just-another-imgscrapper-0.1.2/src/just_another_imgscrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)       58 2023-06-15 11:02:06.000000 just-another-imgscrapper-0.1.2/src/just_another_imgscrapper.egg-info/entry_points.txt
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)      109 2023-06-15 11:02:06.000000 just-another-imgscrapper-0.1.2/src/just_another_imgscrapper.egg-info/requires.txt
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)       12 2023-06-15 11:02:06.000000 just-another-imgscrapper-0.1.2/src/just_another_imgscrapper.egg-info/top_level.txt
+drwxrwxr-x   0 deshrit   (1000) deshrit   (1000)        0 2023-06-15 11:02:07.023762 just-another-imgscrapper-0.1.2/tests/
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)     1118 2023-06-08 05:25:44.000000 just-another-imgscrapper-0.1.2/tests/test_get_html_doc.py
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)     3434 2023-06-08 05:25:44.000000 just-another-imgscrapper-0.1.2/tests/test_img_tag_extraction.py
```

### Comparing `just-another-imgscrapper-0.1.1/LICENSE` & `just-another-imgscrapper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `just-another-imgscrapper-0.1.1/PKG-INFO` & `just-another-imgscrapper-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: just-another-imgscrapper
-Version: 0.1.1
+Version: 0.1.2
 Summary: A utility for scrapping images from a HTML doc from  a URL.
 Home-page: https://github.com/deshrit/just-another-imgscrapper
 Author: Deshrit Baral
 Author-email: deshritbaral@gmail.com
 License: MIT
 Keywords: image,scrapper,asyncio,httpx,beautifulsoup4,lxml
 Classifier: Programming Language :: Python
@@ -23,14 +23,15 @@
 ![](https://github.com/deshrit/just-another-imgscrapper/actions/workflows/tests.yml/badge.svg)
 
 A utility for scrapping images from a HTML doc.
 
 Uses `asyncio` for fast concurrent download.
 
 ## Installation
+Binary installers for the latest released version are available at the [Python Package Index (PyPI)](https://pypi.org/project/just-another-imgscrapper/).
 ```bash
 $ pip install just-another-imgscrapper
 ```
 ## Usage
 ### 1. From cli
 ```bash
 $ imgscrapper -h
@@ -65,15 +66,15 @@
 >>> ...
 >>> d.request_header = {
     'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64; rv:102.0) Gecko/20100101 Firefox/102.0',
     'DNT': '1',
     }
 >>> ...
 ```
-You can specifically select specific type of `img` tags by specfying attribute of HTML element.
+You can select specific type of `img` tags only by passing `attrs` dict.
 ```html
 <!-- >http://helloworld.com<-->
 <html>
     <body>
         <img src="https://foo.com/bar.png" class="apple ball">
         <img src="/foo.jpg" class="cat bar">
     </body>
@@ -85,25 +86,25 @@
 >>> d.url = "http://helloworld.com"
 >>> d.attrs = {
     'class': 'cat',
     }
 >>> d.download()
 >>> 1 # http://helloworld.com/foo.jpg
 ```
-The downloader gives unique `uuid` to downloaded images preserving the image extension.
+The downloader gives unique `uuid` filename to downloaded images preserving the image extension.
 ```python
 >>> d = ImgScrapper(
     url = "http://helloworld.com",
     attrs = {'class': 'cat'},
     max = 5,
     path = "/home/images"
 )
 >>> d.download()
 >>> 5
 ```
-You can limit no. of image downloads by `max` value.
+Limit the no. of image downloads by passing `max` value.
 
 ## Liscense
 `just-another-imgscrapper` is released under the MIT liscense. See LISCENSE for details.
 
 ## Contact
-Follow me on twitter ![@deshritbaral](https://twitter.com/deshritbaral)
+Connect with me on twitter [@deshritbaral](https://twitter.com/deshritbaral)
```

#### html2text {}

```diff
@@ -1,40 +1,43 @@
-Metadata-Version: 2.1 Name: just-another-imgscrapper Version: 0.1.1 Summary: A
+Metadata-Version: 2.1 Name: just-another-imgscrapper Version: 0.1.2 Summary: A
 utility for scrapping images from a HTML doc from a URL. Home-page: https://
 github.com/deshrit/just-another-imgscrapper Author: Deshrit Baral Author-email:
 deshritbaral@gmail.com License: MIT Keywords:
 image,scrapper,asyncio,httpx,beautifulsoup4,lxml Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE # just-another-imgscrapper ![](https:
 //github.com/deshrit/just-another-imgscrapper/actions/workflows/tests.yml/
 badge.svg) A utility for scrapping images from a HTML doc. Uses `asyncio` for
-fast concurrent download. ## Installation ```bash $ pip install just-another-
-imgscrapper ``` ## Usage ### 1. From cli ```bash $ imgscrapper -h ``` To get
-HTML doc, extract image links from `src` attribute of `[Image]` tags and
+fast concurrent download. ## Installation Binary installers for the latest
+released version are available at the [Python Package Index (PyPI)](https://
+pypi.org/project/just-another-imgscrapper/). ```bash $ pip install just-
+another-imgscrapper ``` ## Usage ### 1. From cli ```bash $ imgscrapper -h ```
+To get HTML doc, extract image links from `src` attribute of `[Image]` tags and
 download. ``` $ imgscrapper "http://foo.com/bar" [2023-06-06 23:22:56]
 imgscrapper.utils:INFO: ### Initializing Scrapping ### [2023-06-06 23:23:01]
 imgscrapper.utils:INFO: ### Downloaded 41 images out of extracted 41 links ###
 ``` Downloads to `imgs/` dir in working dir. If dir does not exists, creates.
 ### 2. From module ```python >>> from imgscrapper import ImgScrapper >>> d =
 ImgScrapper() >>> d.download("http://foo.com/bar") >>> 3 ``` Specify path to
 store downloaded images. ```python >>> d = ImgScrapper() >>> d.url = "http://
 foo.com/bar" >>> d.path = "/path/download" >>> d.download() # returns no. of
 successful downloads >>> 3 ``` Some servers will block the scrapping, respect
 robots.txt and only used in allowed hosts. You can add request headers.
 ```python >>> ... >>> d.request_header = { 'User-Agent': 'Mozilla/5.0 (X11;
 Linux x86_64; rv:102.0) Gecko/20100101 Firefox/102.0', 'DNT': '1', } >>> ...
-``` You can specifically select specific type of `img` tags by specfying
-attribute of HTML element. ```html
+``` You can select specific type of `img` tags only by passing `attrs` dict.
+```html
 [https://foo.com/bar.png] [/foo.jpg]
 ``` To select only images with `class: cat` ```python >>> d = ImgScrapper() >>>
 d.url = "http://helloworld.com" >>> d.attrs = { 'class': 'cat', } >>>
 d.download() >>> 1 # http://helloworld.com/foo.jpg ``` The downloader gives
-unique `uuid` to downloaded images preserving the image extension. ```python
->>> d = ImgScrapper( url = "http://helloworld.com", attrs = {'class': 'cat'},
-max = 5, path = "/home/images" ) >>> d.download() >>> 5 ``` You can limit no.
-of image downloads by `max` value. ## Liscense `just-another-imgscrapper` is
-released under the MIT liscense. See LISCENSE for details. ## Contact Follow me
-on twitter ![@deshritbaral](https://twitter.com/deshritbaral)
+unique `uuid` filename to downloaded images preserving the image extension.
+```python >>> d = ImgScrapper( url = "http://helloworld.com", attrs = {'class':
+'cat'}, max = 5, path = "/home/images" ) >>> d.download() >>> 5 ``` Limit the
+no. of image downloads by passing `max` value. ## Liscense `just-another-
+imgscrapper` is released under the MIT liscense. See LISCENSE for details. ##
+Contact Connect with me on twitter [@deshritbaral](https://twitter.com/
+deshritbaral)
```

### Comparing `just-another-imgscrapper-0.1.1/README.md` & `just-another-imgscrapper-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 ![](https://github.com/deshrit/just-another-imgscrapper/actions/workflows/tests.yml/badge.svg)
 
 A utility for scrapping images from a HTML doc.
 
 Uses `asyncio` for fast concurrent download.
 
 ## Installation
+Binary installers for the latest released version are available at the [Python Package Index (PyPI)](https://pypi.org/project/just-another-imgscrapper/).
 ```bash
 $ pip install just-another-imgscrapper
 ```
 ## Usage
 ### 1. From cli
 ```bash
 $ imgscrapper -h
@@ -44,15 +45,15 @@
 >>> ...
 >>> d.request_header = {
     'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64; rv:102.0) Gecko/20100101 Firefox/102.0',
     'DNT': '1',
     }
 >>> ...
 ```
-You can specifically select specific type of `img` tags by specfying attribute of HTML element.
+You can select specific type of `img` tags only by passing `attrs` dict.
 ```html
 <!-- >http://helloworld.com<-->
 <html>
     <body>
         <img src="https://foo.com/bar.png" class="apple ball">
         <img src="/foo.jpg" class="cat bar">
     </body>
@@ -64,25 +65,25 @@
 >>> d.url = "http://helloworld.com"
 >>> d.attrs = {
     'class': 'cat',
     }
 >>> d.download()
 >>> 1 # http://helloworld.com/foo.jpg
 ```
-The downloader gives unique `uuid` to downloaded images preserving the image extension.
+The downloader gives unique `uuid` filename to downloaded images preserving the image extension.
 ```python
 >>> d = ImgScrapper(
     url = "http://helloworld.com",
     attrs = {'class': 'cat'},
     max = 5,
     path = "/home/images"
 )
 >>> d.download()
 >>> 5
 ```
-You can limit no. of image downloads by `max` value.
+Limit the no. of image downloads by passing `max` value.
 
 ## Liscense
 `just-another-imgscrapper` is released under the MIT liscense. See LISCENSE for details.
 
 ## Contact
-Follow me on twitter ![@deshritbaral](https://twitter.com/deshritbaral)
+Connect with me on twitter [@deshritbaral](https://twitter.com/deshritbaral)
```

#### html2text {}

```diff
@@ -1,29 +1,32 @@
 # just-another-imgscrapper ![](https://github.com/deshrit/just-another-
 imgscrapper/actions/workflows/tests.yml/badge.svg) A utility for scrapping
 images from a HTML doc. Uses `asyncio` for fast concurrent download. ##
-Installation ```bash $ pip install just-another-imgscrapper ``` ## Usage ### 1.
-From cli ```bash $ imgscrapper -h ``` To get HTML doc, extract image links from
-`src` attribute of `[Image]` tags and download. ``` $ imgscrapper "http://
+Installation Binary installers for the latest released version are available at
+the [Python Package Index (PyPI)](https://pypi.org/project/just-another-
+imgscrapper/). ```bash $ pip install just-another-imgscrapper ``` ## Usage ###
+1. From cli ```bash $ imgscrapper -h ``` To get HTML doc, extract image links
+from `src` attribute of `[Image]` tags and download. ``` $ imgscrapper "http://
 foo.com/bar" [2023-06-06 23:22:56] imgscrapper.utils:INFO: ### Initializing
 Scrapping ### [2023-06-06 23:23:01] imgscrapper.utils:INFO: ### Downloaded 41
 images out of extracted 41 links ### ``` Downloads to `imgs/` dir in working
 dir. If dir does not exists, creates. ### 2. From module ```python >>> from
 imgscrapper import ImgScrapper >>> d = ImgScrapper() >>> d.download("http://
 foo.com/bar") >>> 3 ``` Specify path to store downloaded images. ```python >>>
 d = ImgScrapper() >>> d.url = "http://foo.com/bar" >>> d.path = "/path/
 download" >>> d.download() # returns no. of successful downloads >>> 3 ``` Some
 servers will block the scrapping, respect robots.txt and only used in allowed
 hosts. You can add request headers. ```python >>> ... >>> d.request_header =
 { 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64; rv:102.0) Gecko/20100101
-Firefox/102.0', 'DNT': '1', } >>> ... ``` You can specifically select specific
-type of `img` tags by specfying attribute of HTML element. ```html
+Firefox/102.0', 'DNT': '1', } >>> ... ``` You can select specific type of `img`
+tags only by passing `attrs` dict. ```html
 [https://foo.com/bar.png] [/foo.jpg]
 ``` To select only images with `class: cat` ```python >>> d = ImgScrapper() >>>
 d.url = "http://helloworld.com" >>> d.attrs = { 'class': 'cat', } >>>
 d.download() >>> 1 # http://helloworld.com/foo.jpg ``` The downloader gives
-unique `uuid` to downloaded images preserving the image extension. ```python
->>> d = ImgScrapper( url = "http://helloworld.com", attrs = {'class': 'cat'},
-max = 5, path = "/home/images" ) >>> d.download() >>> 5 ``` You can limit no.
-of image downloads by `max` value. ## Liscense `just-another-imgscrapper` is
-released under the MIT liscense. See LISCENSE for details. ## Contact Follow me
-on twitter ![@deshritbaral](https://twitter.com/deshritbaral)
+unique `uuid` filename to downloaded images preserving the image extension.
+```python >>> d = ImgScrapper( url = "http://helloworld.com", attrs = {'class':
+'cat'}, max = 5, path = "/home/images" ) >>> d.download() >>> 5 ``` Limit the
+no. of image downloads by passing `max` value. ## Liscense `just-another-
+imgscrapper` is released under the MIT liscense. See LISCENSE for details. ##
+Contact Connect with me on twitter [@deshritbaral](https://twitter.com/
+deshritbaral)
```

### Comparing `just-another-imgscrapper-0.1.1/setup.cfg` & `just-another-imgscrapper-0.1.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = just-another-imgscrapper
-version = 0.1.1
+version = 0.1.2
 description = A utility for scrapping images from a HTML doc from  a URL.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/deshrit/just-another-imgscrapper
 author = Deshrit Baral
 author_email = deshritbaral@gmail.com
 license = MIT
```

### Comparing `just-another-imgscrapper-0.1.1/src/imgscrapper/__main__.py` & `just-another-imgscrapper-0.1.2/src/imgscrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `just-another-imgscrapper-0.1.1/src/imgscrapper/errors.py` & `just-another-imgscrapper-0.1.2/src/imgscrapper/errors.py`

 * *Files identical despite different names*

### Comparing `just-another-imgscrapper-0.1.1/src/imgscrapper/imgscrapper.py` & `just-another-imgscrapper-0.1.2/src/imgscrapper/imgscrapper.py`

 * *Files identical despite different names*

### Comparing `just-another-imgscrapper-0.1.1/src/just_another_imgscrapper.egg-info/PKG-INFO` & `just-another-imgscrapper-0.1.2/src/just_another_imgscrapper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: just-another-imgscrapper
-Version: 0.1.1
+Version: 0.1.2
 Summary: A utility for scrapping images from a HTML doc from  a URL.
 Home-page: https://github.com/deshrit/just-another-imgscrapper
 Author: Deshrit Baral
 Author-email: deshritbaral@gmail.com
 License: MIT
 Keywords: image,scrapper,asyncio,httpx,beautifulsoup4,lxml
 Classifier: Programming Language :: Python
@@ -23,14 +23,15 @@
 ![](https://github.com/deshrit/just-another-imgscrapper/actions/workflows/tests.yml/badge.svg)
 
 A utility for scrapping images from a HTML doc.
 
 Uses `asyncio` for fast concurrent download.
 
 ## Installation
+Binary installers for the latest released version are available at the [Python Package Index (PyPI)](https://pypi.org/project/just-another-imgscrapper/).
 ```bash
 $ pip install just-another-imgscrapper
 ```
 ## Usage
 ### 1. From cli
 ```bash
 $ imgscrapper -h
@@ -65,15 +66,15 @@
 >>> ...
 >>> d.request_header = {
     'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64; rv:102.0) Gecko/20100101 Firefox/102.0',
     'DNT': '1',
     }
 >>> ...
 ```
-You can specifically select specific type of `img` tags by specfying attribute of HTML element.
+You can select specific type of `img` tags only by passing `attrs` dict.
 ```html
 <!-- >http://helloworld.com<-->
 <html>
     <body>
         <img src="https://foo.com/bar.png" class="apple ball">
         <img src="/foo.jpg" class="cat bar">
     </body>
@@ -85,25 +86,25 @@
 >>> d.url = "http://helloworld.com"
 >>> d.attrs = {
     'class': 'cat',
     }
 >>> d.download()
 >>> 1 # http://helloworld.com/foo.jpg
 ```
-The downloader gives unique `uuid` to downloaded images preserving the image extension.
+The downloader gives unique `uuid` filename to downloaded images preserving the image extension.
 ```python
 >>> d = ImgScrapper(
     url = "http://helloworld.com",
     attrs = {'class': 'cat'},
     max = 5,
     path = "/home/images"
 )
 >>> d.download()
 >>> 5
 ```
-You can limit no. of image downloads by `max` value.
+Limit the no. of image downloads by passing `max` value.
 
 ## Liscense
 `just-another-imgscrapper` is released under the MIT liscense. See LISCENSE for details.
 
 ## Contact
-Follow me on twitter ![@deshritbaral](https://twitter.com/deshritbaral)
+Connect with me on twitter [@deshritbaral](https://twitter.com/deshritbaral)
```

#### html2text {}

```diff
@@ -1,40 +1,43 @@
-Metadata-Version: 2.1 Name: just-another-imgscrapper Version: 0.1.1 Summary: A
+Metadata-Version: 2.1 Name: just-another-imgscrapper Version: 0.1.2 Summary: A
 utility for scrapping images from a HTML doc from a URL. Home-page: https://
 github.com/deshrit/just-another-imgscrapper Author: Deshrit Baral Author-email:
 deshritbaral@gmail.com License: MIT Keywords:
 image,scrapper,asyncio,httpx,beautifulsoup4,lxml Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE # just-another-imgscrapper ![](https:
 //github.com/deshrit/just-another-imgscrapper/actions/workflows/tests.yml/
 badge.svg) A utility for scrapping images from a HTML doc. Uses `asyncio` for
-fast concurrent download. ## Installation ```bash $ pip install just-another-
-imgscrapper ``` ## Usage ### 1. From cli ```bash $ imgscrapper -h ``` To get
-HTML doc, extract image links from `src` attribute of `[Image]` tags and
+fast concurrent download. ## Installation Binary installers for the latest
+released version are available at the [Python Package Index (PyPI)](https://
+pypi.org/project/just-another-imgscrapper/). ```bash $ pip install just-
+another-imgscrapper ``` ## Usage ### 1. From cli ```bash $ imgscrapper -h ```
+To get HTML doc, extract image links from `src` attribute of `[Image]` tags and
 download. ``` $ imgscrapper "http://foo.com/bar" [2023-06-06 23:22:56]
 imgscrapper.utils:INFO: ### Initializing Scrapping ### [2023-06-06 23:23:01]
 imgscrapper.utils:INFO: ### Downloaded 41 images out of extracted 41 links ###
 ``` Downloads to `imgs/` dir in working dir. If dir does not exists, creates.
 ### 2. From module ```python >>> from imgscrapper import ImgScrapper >>> d =
 ImgScrapper() >>> d.download("http://foo.com/bar") >>> 3 ``` Specify path to
 store downloaded images. ```python >>> d = ImgScrapper() >>> d.url = "http://
 foo.com/bar" >>> d.path = "/path/download" >>> d.download() # returns no. of
 successful downloads >>> 3 ``` Some servers will block the scrapping, respect
 robots.txt and only used in allowed hosts. You can add request headers.
 ```python >>> ... >>> d.request_header = { 'User-Agent': 'Mozilla/5.0 (X11;
 Linux x86_64; rv:102.0) Gecko/20100101 Firefox/102.0', 'DNT': '1', } >>> ...
-``` You can specifically select specific type of `img` tags by specfying
-attribute of HTML element. ```html
+``` You can select specific type of `img` tags only by passing `attrs` dict.
+```html
 [https://foo.com/bar.png] [/foo.jpg]
 ``` To select only images with `class: cat` ```python >>> d = ImgScrapper() >>>
 d.url = "http://helloworld.com" >>> d.attrs = { 'class': 'cat', } >>>
 d.download() >>> 1 # http://helloworld.com/foo.jpg ``` The downloader gives
-unique `uuid` to downloaded images preserving the image extension. ```python
->>> d = ImgScrapper( url = "http://helloworld.com", attrs = {'class': 'cat'},
-max = 5, path = "/home/images" ) >>> d.download() >>> 5 ``` You can limit no.
-of image downloads by `max` value. ## Liscense `just-another-imgscrapper` is
-released under the MIT liscense. See LISCENSE for details. ## Contact Follow me
-on twitter ![@deshritbaral](https://twitter.com/deshritbaral)
+unique `uuid` filename to downloaded images preserving the image extension.
+```python >>> d = ImgScrapper( url = "http://helloworld.com", attrs = {'class':
+'cat'}, max = 5, path = "/home/images" ) >>> d.download() >>> 5 ``` Limit the
+no. of image downloads by passing `max` value. ## Liscense `just-another-
+imgscrapper` is released under the MIT liscense. See LISCENSE for details. ##
+Contact Connect with me on twitter [@deshritbaral](https://twitter.com/
+deshritbaral)
```

### Comparing `just-another-imgscrapper-0.1.1/src/just_another_imgscrapper.egg-info/SOURCES.txt` & `just-another-imgscrapper-0.1.2/src/just_another_imgscrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `just-another-imgscrapper-0.1.1/tests/test_get_html_doc.py` & `just-another-imgscrapper-0.1.2/tests/test_get_html_doc.py`

 * *Files identical despite different names*

### Comparing `just-another-imgscrapper-0.1.1/tests/test_img_tag_extraction.py` & `just-another-imgscrapper-0.1.2/tests/test_img_tag_extraction.py`

 * *Files identical despite different names*

