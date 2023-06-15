# Comparing `tmp/oidc_client-0.2.5.tar.gz` & `tmp/oidc_client-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oidc_client-0.2.5.tar", max compression
+gzip compressed data, was "oidc_client-0.2.6.tar", max compression
```

## Comparing `oidc_client-0.2.5.tar` & `oidc_client-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1085 2023-04-26 15:38:59.194940 oidc_client-0.2.5/LICENSE.md
--rw-r--r--   0        0        0     1069 2023-04-26 15:38:59.194940 oidc_client-0.2.5/README.md
--rw-r--r--   0        0        0      541 2023-04-26 15:38:59.194940 oidc_client-0.2.5/oidc_client/__init__.py
--rw-r--r--   0        0        0       30 2023-04-26 15:38:59.194940 oidc_client-0.2.5/oidc_client/__main__.py
--rw-r--r--   0        0        0     5028 2023-04-26 15:38:59.194940 oidc_client-0.2.5/oidc_client/cli.py
--rw-r--r--   0        0        0     3717 2023-04-26 15:38:59.194940 oidc_client-0.2.5/oidc_client/config.py
--rw-r--r--   0        0        0      925 2023-04-26 15:38:59.194940 oidc_client-0.2.5/oidc_client/discovery.py
--rw-r--r--   0        0        0      488 2023-04-26 15:38:59.195940 oidc_client-0.2.5/oidc_client/error.py
--rw-r--r--   0        0        0      264 2023-04-26 15:38:59.195940 oidc_client-0.2.5/oidc_client/index.html
--rw-r--r--   0        0        0     1748 2023-04-26 15:38:59.195940 oidc_client-0.2.5/oidc_client/lib.py
--rw-r--r--   0        0        0     1123 2023-04-26 15:38:59.195940 oidc_client-0.2.5/oidc_client/localhost.crt
--rw-r--r--   0        0        0     1704 2023-04-26 15:38:59.195940 oidc_client-0.2.5/oidc_client/localhost.key
--rw-r--r--   0        0        0     8651 2023-04-26 15:38:59.195940 oidc_client-0.2.5/oidc_client/oauth.py
--rw-r--r--   0        0        0      807 2023-04-26 15:38:59.195940 oidc_client-0.2.5/oidc_client/pkce.py
--rw-r--r--   0        0        0        0 2023-04-26 15:38:59.195940 oidc_client-0.2.5/oidc_client/py.typed
--rw-r--r--   0        0        0      556 2023-04-26 15:38:59.195940 oidc_client-0.2.5/oidc_client/tls.py
--rw-r--r--   0        0        0     1325 2023-04-26 15:38:59.195940 oidc_client-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1926 1970-01-01 00:00:00.000000 oidc_client-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-06-15 11:06:27.808252 oidc_client-0.2.6/LICENSE.md
+-rw-r--r--   0        0        0     1069 2023-06-15 11:06:27.808252 oidc_client-0.2.6/README.md
+-rw-r--r--   0        0        0      541 2023-06-15 11:06:27.808252 oidc_client-0.2.6/oidc_client/__init__.py
+-rw-r--r--   0        0        0       30 2023-06-15 11:06:27.808252 oidc_client-0.2.6/oidc_client/__main__.py
+-rw-r--r--   0        0        0     5028 2023-06-15 11:06:27.808252 oidc_client-0.2.6/oidc_client/cli.py
+-rw-r--r--   0        0        0     3760 2023-06-15 11:06:27.808252 oidc_client-0.2.6/oidc_client/config.py
+-rw-r--r--   0        0        0      957 2023-06-15 11:06:27.808252 oidc_client-0.2.6/oidc_client/discovery.py
+-rw-r--r--   0        0        0      488 2023-06-15 11:06:27.808252 oidc_client-0.2.6/oidc_client/error.py
+-rw-r--r--   0        0        0      264 2023-06-15 11:06:27.808252 oidc_client-0.2.6/oidc_client/index.html
+-rw-r--r--   0        0        0     1748 2023-06-15 11:06:27.809252 oidc_client-0.2.6/oidc_client/lib.py
+-rw-r--r--   0        0        0     1123 2023-06-15 11:06:27.809252 oidc_client-0.2.6/oidc_client/localhost.crt
+-rw-r--r--   0        0        0     1704 2023-06-15 11:06:27.809252 oidc_client-0.2.6/oidc_client/localhost.key
+-rw-r--r--   0        0        0     8651 2023-06-15 11:06:27.809252 oidc_client-0.2.6/oidc_client/oauth.py
+-rw-r--r--   0        0        0      807 2023-06-15 11:06:27.809252 oidc_client-0.2.6/oidc_client/pkce.py
+-rw-r--r--   0        0        0        0 2023-06-15 11:06:27.831252 oidc_client-0.2.6/oidc_client/py.typed
+-rw-r--r--   0        0        0      556 2023-06-15 11:06:27.809252 oidc_client-0.2.6/oidc_client/tls.py
+-rw-r--r--   0        0        0     1325 2023-06-15 11:06:27.809252 oidc_client-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1824 1970-01-01 00:00:00.000000 oidc_client-0.2.6/PKG-INFO
```

### Comparing `oidc_client-0.2.5/LICENSE.md` & `oidc_client-0.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.5/README.md` & `oidc_client-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.5/oidc_client/__init__.py` & `oidc_client-0.2.6/oidc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.5/oidc_client/cli.py` & `oidc_client-0.2.6/oidc_client/cli.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.5/oidc_client/config.py` & `oidc_client-0.2.6/oidc_client/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,18 @@
 
     if not redirect_uri.hostname or not redirect_uri.port:
         raise ProviderConfigError("redirection URI must include hostname and port.")
 
     if redirect_uri.params or redirect_uri.query:
         raise ProviderConfigError("redirection URI must not include query params.")
 
-    if redirect_uri.hostname != "127.0.0.1" and redirect_uri.scheme == "http":
+    if (
+        redirect_uri.hostname not in ("127.0.0.1", "localhost")
+        and redirect_uri.scheme == "http"
+    ):
         raise ProviderConfigError("TLS must be enabled for non-loopback interfaces.")
 
 
 @dataclass(frozen=True)
 class ClientProfile:
     """OIDC client profile."""
```

### Comparing `oidc_client-0.2.5/oidc_client/discovery.py` & `oidc_client-0.2.6/oidc_client/discovery.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 
 
 def fetch_provider_config(issuer: str) -> ProviderConfig:
     """Fetch a provider configuration from an OIDC issuer (URL)."""
     if not issuer.startswith("https://"):
         raise ValueError("The issuer URL must be HTTPS.")
 
-    with urlopen(urljoin(issuer, ".well-known/openid-configuration")) as response:
+    with urlopen(
+        urljoin(issuer.rstrip("/") + "/", ".well-known/openid-configuration")
+    ) as response:
         data = json.load(response)
 
         if data["issuer"] != issuer:
             raise ProviderConfigError(
                 "The issuer value returned must be identical to the issuer URL."
             )
```

### Comparing `oidc_client-0.2.5/oidc_client/lib.py` & `oidc_client-0.2.6/oidc_client/lib.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.5/oidc_client/localhost.crt` & `oidc_client-0.2.6/oidc_client/localhost.crt`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.5/oidc_client/localhost.key` & `oidc_client-0.2.6/oidc_client/localhost.key`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.5/oidc_client/oauth.py` & `oidc_client-0.2.6/oidc_client/oauth.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.5/oidc_client/pkce.py` & `oidc_client-0.2.6/oidc_client/pkce.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.5/oidc_client/tls.py` & `oidc_client-0.2.6/oidc_client/tls.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.5/pyproject.toml` & `oidc_client-0.2.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oidc-client"
-version = "0.2.5"
+version = "0.2.6"
 description = "A pure-Python OpenID Connect client"
 readme = "README.md"
 keywords = ["openid", "oidc", "oauth", "oauth2"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Topic :: Internet :: WWW/HTTP",
```

### Comparing `oidc_client-0.2.5/PKG-INFO` & `oidc_client-0.2.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: oidc-client
-Version: 0.2.5
+Version: 0.2.6
 Summary: A pure-Python OpenID Connect client
 Home-page: https://gitlab.com/lzinsou/oidc-client
 Keywords: openid,oidc,oauth,oauth2
 Author: Loris Zinsou
 Author-email: lzinsou@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: StrEnum (>=0.4) ; python_version < "3.11"
 Requires-Dist: toml (>=0.10) ; python_version < "3.11"
 Project-URL: Repository, https://gitlab.com/lzinsou/oidc-client
 Description-Content-Type: text/markdown
 
 OIDC Client
```

