# Comparing `tmp/geoinsight-0.5.1.tar.gz` & `tmp/geoinsight-0.5.3.tar.gz`

## Comparing `geoinsight-0.5.1.tar` & `geoinsight-0.5.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 geoinsight-0.5.1/geoinsight/src/__init__.py
--rw-r--r--   0        0        0    75247 2020-02-02 00:00:00.000000 geoinsight-0.5.1/geoinsight/src/api.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 geoinsight-0.5.1/geoinsight/src/geoinsight.py
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 geoinsight-0.5.1/geoinsight/src/util.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 geoinsight-0.5.1/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geoinsight-0.5.1/LICENSE
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 geoinsight-0.5.1/README.md
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 geoinsight-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 geoinsight-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 geoinsight-0.5.3/geoinsight/src/__init__.py
+-rw-r--r--   0        0        0    75207 2020-02-02 00:00:00.000000 geoinsight-0.5.3/geoinsight/src/api.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 geoinsight-0.5.3/geoinsight/src/geoinsight.py
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 geoinsight-0.5.3/geoinsight/src/util.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 geoinsight-0.5.3/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geoinsight-0.5.3/LICENSE
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 geoinsight-0.5.3/README.md
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 geoinsight-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 geoinsight-0.5.3/PKG-INFO
```

### Comparing `geoinsight-0.5.1/geoinsight/src/api.py` & `geoinsight-0.5.3/geoinsight/src/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     def is_online(self):
         r = requests.get(self.url)
         if 200 <= r.status_code <= 299:
             return True
         else:
             return False
 
-    def set_access_token(self, _refresh_token, _client_secret, _apiurl="https://api.geoinsight.ai",):
-        body = {"grant_type": "refresh_token", "client_id": AUTH0_CLIENT_ID, "refresh_token": _refresh_token, "client_secret": _client_secret}
+    def set_access_token(self, _gpt, _apk, _apiurl="https://api.geoinsight.ai",):
+        body = {"grant_type": "refresh_token", "client_id": AUTH0_CLIENT_ID, "refresh_token": _gpt, "client_secret": _apk}
         r = requests.post('https://{}/oauth/token'.format(AUTH0_DOMAIN), data=body)
         self.url = _apiurl
         if 200 <= r.status_code <= 299 and self.is_online():
             jwks_url = 'https://{}/.well-known/jwks.json'.format(AUTH0_DOMAIN)
             issuer = 'https://{}/'.format(AUTH0_DOMAIN)
             sv = AsymmetricSignatureVerifier(jwks_url)
             tv = TokenVerifier(signature_verifier=sv, issuer=issuer, audience=AUTH0_CLIENT_ID)
```

### Comparing `geoinsight-0.5.1/geoinsight/src/geoinsight.py` & `geoinsight-0.5.3/geoinsight/src/geoinsight.py`

 * *Files identical despite different names*

### Comparing `geoinsight-0.5.1/geoinsight/src/util.py` & `geoinsight-0.5.3/geoinsight/src/util.py`

 * *Files identical despite different names*

### Comparing `geoinsight-0.5.1/.gitignore` & `geoinsight-0.5.3/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -27,8 +27,9 @@
 **/*.ipynb_checkpoints/*
 /notebook/.ipynb_checkpoints/
 scratch.sql
 /public/python/dist
 /public/python/build
 /public/python/geoinsight/src/geoinsight.egg-info
 /core/notebooks/jupyterlab/.[a-zA-Z_]*
-run.sql
+run.sql
+/certs/
```

