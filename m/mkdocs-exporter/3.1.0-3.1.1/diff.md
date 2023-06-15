# Comparing `tmp/mkdocs_exporter-3.1.0.tar.gz` & `tmp/mkdocs_exporter-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_exporter-3.1.0.tar", max compression
+gzip compressed data, was "mkdocs_exporter-3.1.1.tar", max compression
```

## Comparing `mkdocs_exporter-3.1.0.tar` & `mkdocs_exporter-3.1.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1071 2023-05-08 13:15:16.904792 mkdocs_exporter-3.1.0/LICENSE
--rw-r--r--   0        0        0     4007 2023-05-29 18:27:56.949905 mkdocs_exporter-3.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-08 15:45:32.453553 mkdocs_exporter-3.1.0/mkdocs_exporter/__init__.py
--rw-r--r--   0        0        0      264 2023-05-30 17:10:15.899396 mkdocs_exporter-3.1.0/mkdocs_exporter/config.py
--rw-r--r--   0        0        0       96 2023-05-08 19:25:05.801769 mkdocs_exporter-3.1.0/mkdocs_exporter/logging.py
--rw-r--r--   0        0        0      543 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/page.py
--rw-r--r--   0        0        0     1935 2023-05-30 17:10:15.899396 mkdocs_exporter-3.1.0/mkdocs_exporter/plugin.py
--rw-r--r--   0        0        0        0 2023-05-06 21:44:34.488343 mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 17:00:48.574613 mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/extras/__init__.py
--rw-r--r--   0        0        0      867 2023-05-30 17:10:15.899396 mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/extras/config.py
--rw-r--r--   0        0        0     1121 2023-05-30 17:10:15.899396 mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/extras/plugin.py
--rw-r--r--   0        0        0        0 2023-05-07 17:48:51.834620 mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/__init__.py
--rw-r--r--   0        0        0     2268 2023-06-13 18:22:11.411936 mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/browser.py
--rw-r--r--   0        0        0      526 2023-05-27 12:57:36.091210 mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/button.py
--rw-r--r--   0        0        0     1291 2023-06-13 18:20:29.951946 mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/config.py
--rw-r--r--   0        0        0     4912 2023-06-13 18:23:23.621929 mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/plugin.py
--rw-r--r--   0        0        0     2238 2023-06-13 18:12:31.191994 mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/renderer.py
--rw-r--r--   0        0        0     3845 2023-06-02 11:44:31.861490 mkdocs_exporter-3.1.0/mkdocs_exporter/preprocessor.py
--rw-r--r--   0        0        0      241 2023-05-07 12:23:00.605366 mkdocs_exporter-3.1.0/mkdocs_exporter/renderer.py
--rw-r--r--   0        0        0        0 2023-05-08 14:16:51.163540 mkdocs_exporter-3.1.0/mkdocs_exporter/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/resources/css/__init__.py
--rw-r--r--   0        0        0       93 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/resources/css/readthedocs.css
--rw-r--r--   0        0        0        0 2023-05-08 14:16:39.063540 mkdocs_exporter-3.1.0/mkdocs_exporter/resources/js/__init__.py
--rw-r--r--   0        0        0   504034 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/resources/js/pagedjs.min.js
--rw-r--r--   0        0        0      599 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/theme.py
--rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/themes/__init__.py
--rw-r--r--   0        0        0      650 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/themes/factory.py
--rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/themes/material/__init__.py
--rw-r--r--   0        0        0      681 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/themes/material/icons.py
--rw-r--r--   0        0        0     1317 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/themes/material/theme.py
--rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/themes/readthedocs/__init__.py
--rw-r--r--   0        0        0     1221 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/themes/readthedocs/theme.py
--rw-r--r--   0        0        0     1618 2023-06-13 18:26:55.291907 mkdocs_exporter-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     5357 1970-01-01 00:00:00.000000 mkdocs_exporter-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-08 13:15:16.904792 mkdocs_exporter-3.1.1/LICENSE
+-rw-r--r--   0        0        0     4007 2023-05-29 18:27:56.949905 mkdocs_exporter-3.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 15:45:32.453553 mkdocs_exporter-3.1.1/mkdocs_exporter/__init__.py
+-rw-r--r--   0        0        0      264 2023-05-30 17:10:15.899396 mkdocs_exporter-3.1.1/mkdocs_exporter/config.py
+-rw-r--r--   0        0        0       96 2023-05-08 19:25:05.801769 mkdocs_exporter-3.1.1/mkdocs_exporter/logging.py
+-rw-r--r--   0        0        0      543 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.1/mkdocs_exporter/page.py
+-rw-r--r--   0        0        0     1935 2023-05-30 17:10:15.899396 mkdocs_exporter-3.1.1/mkdocs_exporter/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-06 21:44:34.488343 mkdocs_exporter-3.1.1/mkdocs_exporter/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:00:48.574613 mkdocs_exporter-3.1.1/mkdocs_exporter/plugins/extras/__init__.py
+-rw-r--r--   0        0        0      867 2023-05-30 17:10:15.899396 mkdocs_exporter-3.1.1/mkdocs_exporter/plugins/extras/config.py
+-rw-r--r--   0        0        0     1121 2023-05-30 17:10:15.899396 mkdocs_exporter-3.1.1/mkdocs_exporter/plugins/extras/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:48:51.834620 mkdocs_exporter-3.1.1/mkdocs_exporter/plugins/pdf/__init__.py
+-rw-r--r--   0        0        0     2282 2023-06-15 12:58:56.312600 mkdocs_exporter-3.1.1/mkdocs_exporter/plugins/pdf/browser.py
+-rw-r--r--   0        0        0      526 2023-05-27 12:57:36.091210 mkdocs_exporter-3.1.1/mkdocs_exporter/plugins/pdf/button.py
+-rw-r--r--   0        0        0     1291 2023-06-13 18:20:29.951946 mkdocs_exporter-3.1.1/mkdocs_exporter/plugins/pdf/config.py
+-rw-r--r--   0        0        0     4932 2023-06-15 12:36:54.752732 mkdocs_exporter-3.1.1/mkdocs_exporter/plugins/pdf/plugin.py
+-rw-r--r--   0        0        0     2512 2023-06-15 12:37:14.902731 mkdocs_exporter-3.1.1/mkdocs_exporter/plugins/pdf/renderer.py
+-rw-r--r--   0        0        0     3845 2023-06-02 11:44:31.861490 mkdocs_exporter-3.1.1/mkdocs_exporter/preprocessor.py
+-rw-r--r--   0        0        0      241 2023-05-07 12:23:00.605366 mkdocs_exporter-3.1.1/mkdocs_exporter/renderer.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:16:51.163540 mkdocs_exporter-3.1.1/mkdocs_exporter/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.1/mkdocs_exporter/resources/css/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.1/mkdocs_exporter/resources/css/readthedocs.css
+-rw-r--r--   0        0        0        0 2023-05-08 14:16:39.063540 mkdocs_exporter-3.1.1/mkdocs_exporter/resources/js/__init__.py
+-rw-r--r--   0        0        0   504034 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.1/mkdocs_exporter/resources/js/pagedjs.min.js
+-rw-r--r--   0        0        0      237 2023-06-15 12:58:27.282604 mkdocs_exporter-3.1.1/mkdocs_exporter/resources/js/pdf.js
+-rw-r--r--   0        0        0      599 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.1/mkdocs_exporter/theme.py
+-rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.1/mkdocs_exporter/themes/__init__.py
+-rw-r--r--   0        0        0      650 2023-06-14 18:42:45.067998 mkdocs_exporter-3.1.1/mkdocs_exporter/themes/factory.py
+-rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.1/mkdocs_exporter/themes/material/__init__.py
+-rw-r--r--   0        0        0      681 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.1/mkdocs_exporter/themes/material/icons.py
+-rw-r--r--   0        0        0     1310 2023-06-14 18:33:07.838054 mkdocs_exporter-3.1.1/mkdocs_exporter/themes/material/theme.py
+-rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.1/mkdocs_exporter/themes/readthedocs/__init__.py
+-rw-r--r--   0        0        0     1219 2023-06-14 18:33:02.508055 mkdocs_exporter-3.1.1/mkdocs_exporter/themes/readthedocs/theme.py
+-rw-r--r--   0        0        0     1618 2023-06-15 13:00:17.142591 mkdocs_exporter-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5357 1970-01-01 00:00:00.000000 mkdocs_exporter-3.1.1/PKG-INFO
```

### Comparing `mkdocs_exporter-3.1.0/LICENSE` & `mkdocs_exporter-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.1.0/README.md` & `mkdocs_exporter-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.1.0/mkdocs_exporter/page.py` & `mkdocs_exporter-3.1.1/mkdocs_exporter/page.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.1.0/mkdocs_exporter/plugin.py` & `mkdocs_exporter-3.1.1/mkdocs_exporter/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/extras/config.py` & `mkdocs_exporter-3.1.1/mkdocs_exporter/plugins/extras/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/extras/plugin.py` & `mkdocs_exporter-3.1.1/mkdocs_exporter/plugins/extras/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/browser.py` & `mkdocs_exporter-3.1.1/mkdocs_exporter/plugins/pdf/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     page = await self.context.new_page()
     file = NamedTemporaryFile(suffix='.html', mode='w+', encoding='utf-8', delete=False)
 
     file.write(html)
     file.close()
 
     await page.goto('file://' + file.name, wait_until='networkidle')
-    await page.locator('.pagedjs_pages').wait_for(timeout=30000)
+    await page.locator('body[mkdocs-exporter="true"]').wait_for(timeout=30000)
 
     pdf = await page.pdf(prefer_css_page_size=True, print_background=True, display_header_footer=False)
 
     try:
       os.unlink(file)
     except Exception:
       pass
```

### Comparing `mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/button.py` & `mkdocs_exporter-3.1.1/mkdocs_exporter/plugins/pdf/button.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/config.py` & `mkdocs_exporter-3.1.1/mkdocs_exporter/plugins/pdf/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/plugin.py` & `mkdocs_exporter-3.1.1/mkdocs_exporter/plugins/pdf/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,23 +115,22 @@
       return html
 
     page.html = html
 
     async def render(page: Page) -> None:
       logger.info("[pdf] Rendering '%s'...", page.file.src_path)
 
-      pdf = await self.renderer.render(page)
-      fullpath = os.path.join(config['site_dir'], page.formats['pdf'])
+      html = self.renderer.preprocess(page)
+      pdf = await self.renderer.render(html)
 
       page.html = None
 
-      with open(fullpath, 'wb+') as file:
+      with open(os.path.join(config['site_dir'], page.formats['pdf']), 'wb+') as file:
         file.write(pdf)
-
-      logger.info("[pdf] File written to '%s'!", fullpath)
+        logger.info("[pdf] File written to '%s'!", file.name)
 
     self.tasks.append(render(page))
 
     return page.html
 
 
   def on_post_build(self, **kwargs) -> None:
```

### Comparing `mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/renderer.py` & `mkdocs_exporter-3.1.1/mkdocs_exporter/plugins/pdf/renderer.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,40 +42,48 @@
     """Renders a cover."""
 
     content = template.strip('\n')
 
     return f'<div data-decompose="true">{content}</div>' + '\n'
 
 
-  async def render(self, page: Page) -> bytes:
-    """Renders a page as a PDF document."""
-
-    if not self.browser.launched:
-      await self.browser.launch()
+  def preprocess(self, page: Page) -> str:
+    """Preprocesses a page, returning HTML that can be printed."""
 
     preprocessor = Preprocessor(theme=page.theme)
     base = os.path.dirname(page.file.abs_dest_path)
     root = base.replace(unquote(page.url).rstrip('/'), '', 1).rstrip('/')
 
     preprocessor.preprocess(page.html)
     preprocessor.set_attribute('details:not([open])', 'open', 'open')
     page.theme.preprocess(preprocessor)
 
+    preprocessor.script(importlib_resources.files(js).joinpath('pdf.js').read_text())
+
     for stylesheet in self.stylesheets:
       with open(stylesheet, 'r', encoding='utf-8') as file:
         preprocessor.stylesheet(file.read())
     for script in self.scripts:
       with open(script, 'r', encoding='utf-8') as file:
         preprocessor.script(file.read())
 
     preprocessor.script(importlib_resources.files(js).joinpath('pagedjs.min.js').read_text())
     preprocessor.teleport()
     preprocessor.update_links(base, root)
 
-    html = preprocessor.done()
+    return preprocessor.done()
+
+
+  async def render(self, page: str | Page) -> bytes:
+    """Renders a page as a PDF document."""
+
+    if not self.browser.launched:
+      await self.browser.launch()
+
+    html = page if isinstance(page, str) else self.preprocess(page)
 
     return await self.browser.print(html)
 
 
   async def dispose(self) -> None:
     """Dispose of the renderer."""
```

### Comparing `mkdocs_exporter-3.1.0/mkdocs_exporter/preprocessor.py` & `mkdocs_exporter-3.1.1/mkdocs_exporter/preprocessor.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.1.0/mkdocs_exporter/resources/js/pagedjs.min.js` & `mkdocs_exporter-3.1.1/mkdocs_exporter/resources/js/pagedjs.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.1.0/mkdocs_exporter/theme.py` & `mkdocs_exporter-3.1.1/mkdocs_exporter/theme.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.1.0/mkdocs_exporter/themes/factory.py` & `mkdocs_exporter-3.1.1/mkdocs_exporter/themes/factory.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.1.0/mkdocs_exporter/themes/material/icons.py` & `mkdocs_exporter-3.1.1/mkdocs_exporter/themes/material/icons.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.1.0/mkdocs_exporter/themes/material/theme.py` & `mkdocs_exporter-3.1.1/mkdocs_exporter/themes/material/theme.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from mkdocs_exporter.theme import Theme as BaseTheme
 from mkdocs_exporter.preprocessor import Preprocessor
 from mkdocs_exporter.themes.material.icons import get_icon
 
 
 class Theme(BaseTheme):
-  """The "MkDocs Material" theme."""
+  """The "material" theme."""
 
   name = 'material'
   """The name of the theme."""
 
 
   def preprocess(self, preprocessor: Preprocessor) -> None:
     """Preprocesses the DOM before rendering a document."""
```

### Comparing `mkdocs_exporter-3.1.0/mkdocs_exporter/themes/readthedocs/theme.py` & `mkdocs_exporter-3.1.1/mkdocs_exporter/themes/readthedocs/theme.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from mkdocs_exporter.resources import css
 from mkdocs_exporter.theme import Theme as BaseTheme
 from mkdocs_exporter.preprocessor import Preprocessor
 
 
 class Theme(BaseTheme):
-  """The "Read the Docs" theme."""
+  """The "readthedocs" theme."""
 
   name = 'readthedocs'
   """The name of the theme."""
 
 
   def preprocess(self, preprocessor: Preprocessor) -> None:
     """Preprocesses the DOM before rendering a document."""
```

### Comparing `mkdocs_exporter-3.1.0/pyproject.toml` & `mkdocs_exporter-3.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mkdocs-exporter"
-version = "3.1.0"
+version = "3.1.1"
 repository = "https://github.com/adrienbrignon/mkdocs-exporter"
 keywords = ["mkdocs", "pdf", "exporter"]
 description = "A highly-configurable plugin for MkDocs that exports your pages to PDF files."
 authors = ["Adrien Brignon <adrien@brignon.dev>"]
 readme = "README.md"
 classifiers = [
   "License :: OSI Approved :: MIT License",
```

### Comparing `mkdocs_exporter-3.1.0/PKG-INFO` & `mkdocs_exporter-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-exporter
-Version: 3.1.0
+Version: 3.1.1
 Summary: A highly-configurable plugin for MkDocs that exports your pages to PDF files.
 Home-page: https://github.com/adrienbrignon/mkdocs-exporter
 Keywords: mkdocs,pdf,exporter
 Author: Adrien Brignon
 Author-email: adrien@brignon.dev
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocs-exporter Version: 3.1.0 Summary: A highly-
+Metadata-Version: 2.1 Name: mkdocs-exporter Version: 3.1.1 Summary: A highly-
 configurable plugin for MkDocs that exports your pages to PDF files. Home-page:
 https://github.com/adrienbrignon/mkdocs-exporter Keywords: mkdocs,pdf,exporter
 Author: Adrien Brignon Author-email: adrien@brignon.dev Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

