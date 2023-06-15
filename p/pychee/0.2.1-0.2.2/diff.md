# Comparing `tmp/pychee-0.2.1-py3-none-any.whl.zip` & `tmp/pychee-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 19284 bytes, number of entries: 8
+Zip file size: 31567 bytes, number of entries: 8
 -rw-r--r--  2.0 unx      175 b- defN 23-Feb-19 10:21 pychee/__init__.py
--rw-r--r--  2.0 unx    15035 b- defN 23-Apr-12 21:27 pychee/pychee.py
+-rw-r--r--  2.0 unx    15330 b- defN 23-Jun-15 10:09 pychee/pychee.py
 -rw-r--r--  2.0 unx      766 b- defN 23-Apr-12 21:26 pychee/test.py
--rw-r--r--  2.0 unx    34523 b- defN 23-Apr-12 21:28 pychee-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2687 b- defN 23-Apr-12 21:28 pychee-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 21:28 pychee-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-12 21:28 pychee-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      599 b- defN 23-Apr-12 21:28 pychee-0.2.1.dist-info/RECORD
-8 files, 53884 bytes uncompressed, 18250 bytes compressed:  66.1%
+-rw-r--r--  2.0 unx    34523 b- defN 23-Jun-15 10:21 pychee-0.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    42985 b- defN 23-Jun-15 10:21 pychee-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 10:21 pychee-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-15 10:21 pychee-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      600 b- defN 23-Jun-15 10:21 pychee-0.2.2.dist-info/RECORD
+8 files, 94478 bytes uncompressed, 30533 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: pychee/pychee.py
 Comment: 
 
 Filename: pychee/test.py
 Comment: 
 
-Filename: pychee-0.2.1.dist-info/LICENSE
+Filename: pychee-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: pychee-0.2.1.dist-info/METADATA
+Filename: pychee-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: pychee-0.2.1.dist-info/WHEEL
+Filename: pychee-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: pychee-0.2.1.dist-info/top_level.txt
+Filename: pychee-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pychee-0.2.1.dist-info/RECORD
+Filename: pychee-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pychee/pychee.py

```diff
@@ -1,26 +1,27 @@
 #!/usr/bin/env python
 # coding=utf-8
 """
 # pychee: Client for Lychee, written in Python.
 
-For additonal information, visit: https://github.com/LycheeOrg/Lychee.
+For additional information, visit: https://github.com/LycheeOrg/Lychee.
 """
 from posixpath import join
 from typing import List
-from requests import Session
 from urllib.parse import unquote
 
-__version__ = '0.2.1'
+from requests import Session
+
+__version__ = '0.2.2'
 
 class LycheeForbidden(Exception):
     """Raised when the Lychee request is unauthorized."""
 
 class LycheeNotFound(Exception):
-    """Raised when the requested ressource was not found."""
+    """Raised when the requested resource was not found."""
 
 class LycheeError(Exception):
     """Raised for general Lychee errors."""
 
 #FIXME add error code handling
 #FIXME adjust to API sending JSON because we changed Accept
 #FIXME fix type hints...
@@ -50,15 +51,15 @@
     def __init__(self, prefix_url: str, *args, **kwargs):
         """Initialize the `requests.session`."""
         super().__init__(*args, **kwargs)
         self._prefix_url = prefix_url
         # Initial CSRF
         super().request('GET', self._prefix_url)
         self._set_csrf_header()
-        # Lychee now explicitely requires client to accept JSON,
+        # Lychee now explicitly requires client to accept JSON,
         # else throws exception
         self.headers['Accept'] = 'application/json, text/javascript, */*; q=0.01'
 
     def request(self, method, url, *args, **kwargs):
         """Make an HTTP request with the configured session."""
         url = join(self._prefix_url, self.BASE_API_FRAGMENT, url)
         response = super().request(method, url, *args, **kwargs)
@@ -70,27 +71,29 @@
             raise LycheeNotFound(response.text)
         if response.text == 'false' or response.text is None:
             raise LycheeError('Could be unauthorized, wrong args, who knows?')
         return response
 
     def _set_csrf_header(self) -> None:
         """
-        Sets CSRF header from cookie for the whole session.
+        Set CSRF header from cookie for the whole session.
 
         CSRF generally prevents an attacker from forging a request
         sent from another website, e.g. in a JS script, by forcing
         requests to contain a specific value which has been set
         as a cookie in a previous GET request.
 
         Thus, a previous GET request is needed so this method works.
         """
         csrf_token = self.cookies.get(self._CSRF_COOKIE)
         if csrf_token is not None:
             if csrf_token != self.headers.get(self._CSRF_HEADER):
-                self.headers[self._CSRF_HEADER] = unquote(csrf_token).replace('=', '')
+                self.headers[self._CSRF_HEADER] = unquote(
+                    csrf_token
+                ).replace('=', '')
 
 class LycheeClient:
     """
     Lychee API Client.
 
     The primary [Lychee API](https://lycheeorg.github.io/docs/api.html) client
     to interact with the specified Lychee server.
@@ -116,14 +119,23 @@
         """
         Get List of Available Albums in Lychee.
 
         Returns an array of albums or false on failure.
         """
         return self._session.post('Albums::get', json={}).json()
 
+    def get_albums_tree(self):
+        """
+        Get List of Album Trees in Lychee.
+
+        Returns a list of albums dictionaries or an informative message on
+        failure.
+        """
+        return self._session.post('Albums::tree', json={}).json()
+
     def get_albums_position_data(self) -> dict:
         """
         Get List of Available Album Data.
 
         Returns the album with only map related data.
         """
         return self._session.post('Albums::getPositionData', json={}).json()
```

## Comparing `pychee-0.2.1.dist-info/LICENSE` & `pychee-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

