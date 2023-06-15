# Comparing `tmp/playwrightcapture-1.20.4.tar.gz` & `tmp/playwrightcapture-1.20.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.20.4.tar", max compression
+gzip compressed data, was "playwrightcapture-1.20.5.tar", max compression
```

## Comparing `playwrightcapture-1.20.4.tar` & `playwrightcapture-1.20.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.20.4/LICENSE
--rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.20.4/README.md
--rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.20.4/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    36479 2023-06-07 12:40:02.326124 playwrightcapture-1.20.4/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.20.4/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     1734 2023-06-06 09:15:52.098307 playwrightcapture-1.20.4/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.20.4/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1828 2023-06-07 12:42:00.258731 playwrightcapture-1.20.4/pyproject.toml
--rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 playwrightcapture-1.20.4/PKG-INFO
+-rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.20.5/LICENSE
+-rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.20.5/README.md
+-rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.20.5/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    36844 2023-06-15 16:17:17.999029 playwrightcapture-1.20.5/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.20.5/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     1734 2023-06-06 09:15:52.098307 playwrightcapture-1.20.5/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.20.5/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1828 2023-06-15 16:20:12.123618 playwrightcapture-1.20.5/pyproject.toml
+-rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 playwrightcapture-1.20.5/PKG-INFO
```

### Comparing `playwrightcapture-1.20.4/LICENSE` & `playwrightcapture-1.20.5/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.4/README.md` & `playwrightcapture-1.20.5/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.4/playwrightcapture/capture.py` & `playwrightcapture-1.20.5/playwrightcapture/capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,38 +423,43 @@
             try:
                 # NOTE 2022-12-02: allow 15s less than the general timeout to get a DOM
                 await page.goto(url, wait_until='domcontentloaded', timeout=self.general_timeout - 15000, referer=referer if referer else '')
             except Error as initial_error:
                 self._update_exceptions(initial_error)
                 if self._exception_is_network_error(initial_error):
                     raise initial_error
-                try:
-                    # page.goto failed, but it (might have) triggered a download event.
-                    # If it is the case, let's try to save it.
-                    async with page.expect_download(timeout=self.general_timeout - 15000) as download_info:
-                        tmp_f = NamedTemporaryFile(delete=False)
-                        download = await download_info.value
-                        await download.save_as(tmp_f.name)
-                        to_return["downloaded_filename"] = download.suggested_filename
-                        with open(tmp_f.name, "rb") as f:
-                            to_return["downloaded_file"] = f.read()
-                        os.unlink(tmp_f.name)
-                except PlaywrightTimeoutError:
-                    self.logger.debug('No download has been triggered.')
-                    raise initial_error
-                except Error as e:
+                elif initial_error.name == 'Download is starting':
+                    # page.goto failed, but it triggered a download event.
+                    # Let's re-trigger it.
                     try:
-                        error_msg = download.failure()
-                        if not error_msg:
+                        async with page.expect_download(timeout=self.general_timeout - 15000) as download_info:
+                            try:
+                                await page.goto(url, timeout=self.general_timeout - 15000, referer=referer if referer else '')
+                            except Exception:
+                                pass
+                            tmp_f = NamedTemporaryFile(delete=False)
+                            download = await download_info.value
+                            await download.save_as(tmp_f.name)
+                            to_return["downloaded_filename"] = download.suggested_filename
+                            with open(tmp_f.name, "rb") as f:
+                                to_return["downloaded_file"] = f.read()
+                            os.unlink(tmp_f.name)
+                    except PlaywrightTimeoutError:
+                        self.logger.debug('No download has been triggered.')
+                        raise initial_error
+                    except Error as e:
+                        try:
+                            error_msg = download.failure()
+                            if not error_msg:
+                                raise e
+                            to_return['error'] = f"Error while downloading: {error_msg}"
+                            self.logger.info(to_return['error'])
+                            self.should_retry = True
+                        except Exception:
                             raise e
-                        to_return['error'] = f"Error while downloading: {error_msg}"
-                        self.logger.info(to_return['error'])
-                        self.should_retry = True
-                    except Exception:
-                        raise e
             else:
                 await page.bring_to_front()
 
                 # page instrumentation
                 await page.wait_for_timeout(5000)  # Wait 5 sec after document loaded
 
                 # ==== recaptcha
```

### Comparing `playwrightcapture-1.20.4/playwrightcapture/helpers.py` & `playwrightcapture-1.20.5/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.4/pyproject.toml` & `playwrightcapture-1.20.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.20.4"
+version = "1.20.5"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
@@ -17,15 +17,15 @@
     'Topic :: Internet',
 ]
 
 include = ['README.md']
 
 [tool.poetry.dependencies]
 python = "^3.8"
-playwright = "^1.34.0"
+playwright = "^1.35.0"
 dateparser = "^1.1.8"
 beautifulsoup4 = "^4.12.2"
 w3lib = "^2.1.1"
 lxml = "^4.9.2"
 requests = {version = "^2.31.0", optional = true}
 pydub = {version = "^0.25.1", optional = true}
 SpeechRecognition = {version = "^3.10.0", optional = true}
```

### Comparing `playwrightcapture-1.20.4/PKG-INFO` & `playwrightcapture-1.20.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwrightcapture
-Version: 1.20.4
+Version: 1.20.5
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
@@ -19,15 +19,15 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: recaptcha
 Requires-Dist: SpeechRecognition (>=3.10.0,<4.0.0) ; extra == "recaptcha"
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: dateparser (>=1.1.8,<2.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: playwright (>=1.34.0,<2.0.0)
+Requires-Dist: playwright (>=1.35.0,<2.0.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0) ; extra == "recaptcha"
 Requires-Dist: pytz (>=2023.3,<2024.0) ; python_version < "3.9"
 Requires-Dist: requests (>=2.31.0,<3.0.0) ; extra == "recaptcha"
 Requires-Dist: tzdata (>=2023.3,<2024.0)
 Requires-Dist: w3lib (>=2.1.1,<3.0.0)
 Project-URL: Repository, https://github.com/Lookyloo/PlaywrightCapture
 Description-Content-Type: text/markdown
```

