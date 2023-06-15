# Comparing `tmp/mauth_client-1.5.0.tar.gz` & `tmp/mauth_client-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mauth_client-1.5.0.tar", max compression
+gzip compressed data, was "mauth_client-1.5.1.tar", max compression
```

## Comparing `mauth_client-1.5.0.tar` & `mauth_client-1.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1062 2023-04-18 17:30:43.630772 mauth_client-1.5.0/LICENSE.txt
--rw-r--r--   0        0        0     6084 2023-04-18 17:30:43.630772 mauth_client-1.5.0/README.md
--rw-r--r--   0        0        0      243 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/__init__.py
--rw-r--r--   0        0        0     9672 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/authenticator.py
--rw-r--r--   0        0        0      434 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/config.py
--rw-r--r--   0        0        0      479 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/consts.py
--rw-r--r--   0        0        0      633 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/exceptions.py
--rw-r--r--   0        0        0     2046 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/key_holder.py
--rw-r--r--   0        0        0       54 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/lambda_authenticator/__init__.py
--rw-r--r--   0        0        0      761 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/lambda_authenticator/lambda_authenticator.py
--rw-r--r--   0        0        0      679 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/lambda_helper.py
--rw-r--r--   0        0        0       76 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/middlewares/__init__.py
--rw-r--r--   0        0        0     4082 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/middlewares/asgi.py
--rw-r--r--   0        0        0     2114 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/middlewares/wsgi.py
--rw-r--r--   0        0        0       26 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/requests_mauth/__init__.py
--rw-r--r--   0        0        0     1304 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/requests_mauth/client.py
--rw-r--r--   0        0        0     2795 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/rsa_signer.py
--rw-r--r--   0        0        0     2324 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/rsa_verifier.py
--rw-r--r--   0        0        0     6196 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/signable.py
--rw-r--r--   0        0        0     1731 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/signed.py
--rw-r--r--   0        0        0     2849 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/signer.py
--rw-r--r--   0        0        0      820 2023-04-18 17:30:43.630772 mauth_client-1.5.0/mauth_client/utils.py
--rw-r--r--   0        0        0     1421 2023-04-18 17:30:43.634772 mauth_client-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     7647 1970-01-01 00:00:00.000000 mauth_client-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-15 15:49:38.533899 mauth_client-1.5.1/LICENSE.txt
+-rw-r--r--   0        0        0     6084 2023-06-15 15:49:38.533899 mauth_client-1.5.1/README.md
+-rw-r--r--   0        0        0      243 2023-06-15 15:49:38.533899 mauth_client-1.5.1/mauth_client/__init__.py
+-rw-r--r--   0        0        0     9672 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/authenticator.py
+-rw-r--r--   0        0        0      434 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/config.py
+-rw-r--r--   0        0        0      479 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/consts.py
+-rw-r--r--   0        0        0      633 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/exceptions.py
+-rw-r--r--   0        0        0     2046 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/key_holder.py
+-rw-r--r--   0        0        0       54 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/lambda_authenticator/__init__.py
+-rw-r--r--   0        0        0      761 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/lambda_authenticator/lambda_authenticator.py
+-rw-r--r--   0        0        0      679 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/lambda_helper.py
+-rw-r--r--   0        0        0       76 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/middlewares/__init__.py
+-rw-r--r--   0        0        0     4082 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/middlewares/asgi.py
+-rw-r--r--   0        0        0     3864 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/middlewares/wsgi.py
+-rw-r--r--   0        0        0       26 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/requests_mauth/__init__.py
+-rw-r--r--   0        0        0     1304 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/requests_mauth/client.py
+-rw-r--r--   0        0        0     2795 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/rsa_signer.py
+-rw-r--r--   0        0        0     2324 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/rsa_verifier.py
+-rw-r--r--   0        0        0     6196 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/signable.py
+-rw-r--r--   0        0        0     1731 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/signed.py
+-rw-r--r--   0        0        0     2849 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/signer.py
+-rw-r--r--   0        0        0      820 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/utils.py
+-rw-r--r--   0        0        0     1421 2023-06-15 15:49:38.537899 mauth_client-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     7647 1970-01-01 00:00:00.000000 mauth_client-1.5.1/PKG-INFO
```

### Comparing `mauth_client-1.5.0/LICENSE.txt` & `mauth_client-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.0/README.md` & `mauth_client-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.0/mauth_client/authenticator.py` & `mauth_client-1.5.1/mauth_client/authenticator.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.0/mauth_client/exceptions.py` & `mauth_client-1.5.1/mauth_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.0/mauth_client/key_holder.py` & `mauth_client-1.5.1/mauth_client/key_holder.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.0/mauth_client/lambda_authenticator/lambda_authenticator.py` & `mauth_client-1.5.1/mauth_client/lambda_authenticator/lambda_authenticator.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.0/mauth_client/lambda_helper.py` & `mauth_client-1.5.1/mauth_client/lambda_helper.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.0/mauth_client/middlewares/asgi.py` & `mauth_client-1.5.1/mauth_client/middlewares/asgi.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.0/mauth_client/requests_mauth/client.py` & `mauth_client-1.5.1/mauth_client/requests_mauth/client.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.0/mauth_client/rsa_signer.py` & `mauth_client-1.5.1/mauth_client/rsa_signer.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.0/mauth_client/rsa_verifier.py` & `mauth_client-1.5.1/mauth_client/rsa_verifier.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.0/mauth_client/signable.py` & `mauth_client-1.5.1/mauth_client/signable.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.0/mauth_client/signed.py` & `mauth_client-1.5.1/mauth_client/signed.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.0/mauth_client/signer.py` & `mauth_client-1.5.1/mauth_client/signer.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.0/mauth_client/utils.py` & `mauth_client-1.5.1/mauth_client/utils.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.0/pyproject.toml` & `mauth_client-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mauth-client"
-version = "1.5.0"
+version = "1.5.1"
 description = "MAuth Client for Python"
 repository = "https://github.com/mdsol/mauth-client-python"
 authors = ["Medidata Solutions <support@mdsol.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `mauth_client-1.5.0/PKG-INFO` & `mauth_client-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mauth-client
-Version: 1.5.0
+Version: 1.5.1
 Summary: MAuth Client for Python
 Home-page: https://github.com/mdsol/mauth-client-python
 License: MIT
 Author: Medidata Solutions
 Author-email: support@mdsol.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

