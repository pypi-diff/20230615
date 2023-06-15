# Comparing `tmp/formsg-0.1.6.tar.gz` & `tmp/formsg-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formsg-0.1.6.tar", last modified: Fri Feb 11 05:23:53 2022, max compression
+gzip compressed data, was "formsg-0.1.7.tar", max compression
```

## Comparing `formsg-0.1.6.tar` & `formsg-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 05:23:53.847216 formsg-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-02-11 05:23:44.000000 formsg-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3302 2022-02-11 05:23:53.847216 formsg-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2738 2022-02-11 05:23:44.000000 formsg-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 05:23:53.847216 formsg-0.1.6/formsg/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-02-11 05:23:44.000000 formsg-0.1.6/formsg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-02-11 05:23:44.000000 formsg-0.1.6/formsg/django.py
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-02-11 05:23:44.000000 formsg-0.1.6/formsg/flask.py
--rw-r--r--   0 runner    (1001) docker     (121)     3654 2022-02-11 05:23:44.000000 formsg-0.1.6/formsg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 05:23:53.847216 formsg-0.1.6/formsg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3302 2022-02-11 05:23:53.000000 formsg-0.1.6/formsg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-02-11 05:23:53.000000 formsg-0.1.6/formsg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-11 05:23:53.000000 formsg-0.1.6/formsg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-02-11 05:23:53.000000 formsg-0.1.6/formsg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-02-11 05:23:53.000000 formsg-0.1.6/formsg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-02-11 05:23:53.847216 formsg-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      865 2022-02-11 05:23:44.000000 formsg-0.1.6/setup.py
+-rw-r--r--   0        0        0     1078 2023-06-15 15:59:42.638922 formsg-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2738 2023-06-15 15:59:42.639449 formsg-0.1.7/README.md
+-rw-r--r--   0        0        0       20 2023-06-15 15:59:42.639611 formsg-0.1.7/formsg/__init__.py
+-rw-r--r--   0        0        0      659 2023-06-15 16:08:25.457697 formsg-0.1.7/formsg/django.py
+-rw-r--r--   0        0        0      619 2023-06-15 16:09:01.909147 formsg-0.1.7/formsg/flask.py
+-rw-r--r--   0        0        0     3990 2023-06-15 16:17:43.607890 formsg-0.1.7/formsg/utils.py
+-rw-r--r--   0        0        0      413 2023-06-15 16:06:59.257223 formsg-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3220 1970-01-01 00:00:00.000000 formsg-0.1.7/PKG-INFO
```

### Comparing `formsg-0.1.6/LICENSE` & `formsg-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `formsg-0.1.6/PKG-INFO` & `formsg-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: formsg
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python SDK for handling FormSG webhooks.
-Home-page: https://github.com/fivehealth/formsg-python-sdk
 Author: 5 Health Inc
-Author-email: hello@botmd.io
-License: MIT License
-Keywords: django cache
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Author-email: engineers@botmd.io
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Framework :: Django
-Classifier: Framework :: Flask
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pynacl (>=1.4.0)
+Requires-Dist: requests
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # FormSG Python SDK
 
 [![PyPI version](https://img.shields.io/pypi/v/formsg.svg)](https://pypi.python.org/pypi/formsg/)
 [![PyPI license](https://img.shields.io/pypi/l/formsg.svg)](https://pypi.python.org/pypi/formsg/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/formsg.svg)](https://pypi.python.org/pypi/formsg/)
 [![PyPI status](https://img.shields.io/pypi/status/formsg.svg)](https://pypi.python.org/pypi/formsg/)
@@ -78,8 +74,7 @@
 #end if
 ```
 
 ## Contributions
 
 If you find any issues or would like to contribute improvements, please feel free to raise them in this repository directly.
 
-
```

### Comparing `formsg-0.1.6/README.md` & `formsg-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `formsg-0.1.6/formsg/utils.py` & `formsg-0.1.7/formsg/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,102 +1,130 @@
 __all__ = ['verify_signature', 'decrypt_content', 'decrypt_attachment']
 import json
 import logging
 import re
 from time import time
-from typing import Any
-from typing import Dict
-from typing import Mapping
-from typing import Optional
+from typing import Any, Dict, Mapping, Optional
 from urllib.parse import urlparse
 
 import requests
 from nacl.encoding import Base64Encoder
 from nacl.exceptions import BadSignatureError
-from nacl.public import Box
-from nacl.public import PrivateKey
-from nacl.public import PublicKey
+from nacl.public import Box, PrivateKey, PublicKey
 from nacl.signing import VerifyKey
 
 logger = logging.getLogger(__name__)
 
-formsg_webhook_public_key = VerifyKey('3Tt8VduXsjjd4IrpdCd7BAkdZl/vUCstu9UvTX84FWw=', encoder=Base64Encoder)  # https://github.com/opengovsg/formsg-javascript-sdk#step-3---verify-the-signature
-encrypted_content_regex = re.compile(r'^(?P<submission_public_key>[\w\+\/\=]*)\;(?P<nonce>[\w\+\/\=]*)\:(?P<encrypted_message>[\w\+\/\=]*)$')
-
-
-def verify_signature(webhook_uri: str, signature_header: str, signature_expiry_seconds: float = 60) -> Mapping[str, Any]:
+# See https://github.com/opengovsg/formsg-javascript-sdk#step-3---verify-the-signature  # noqa
+formsg_webhook_public_key = VerifyKey(
+    '3Tt8VduXsjjd4IrpdCd7BAkdZl/vUCstu9UvTX84FWw=',
+    encoder=Base64Encoder,
+)
+encrypted_content_regex = re.compile((
+    r'^(?P<submission_public_key>[\w\+\/\=]*)\;'
+    r'(?P<nonce>[\w\+\/\=]*)\:'
+    r'(?P<encrypted_message>[\w\+\/\=]*)$'
+))
+
+
+def verify_signature(
+    webhook_uri: str,
+    signature_header: str,
+    signature_expiry_seconds: float = 60,
+) -> Mapping[str, Any]:
     # v1 is signature, s is submissionId, f is formId, t is submission epoch
-    logger.debug(f'X-FormSG-Signature is <{signature_header}>.')
+    logger.debug('X-FormSG-Signature is <%s>.', signature_header)
 
     formsg_signature: Dict[str, Any] = {}
     for part in signature_header.split(','):
         k, v = part.split('=', 1)
         formsg_signature[k] = v
-    #end for
 
     formsg_signature['t'] = int(formsg_signature['t'])
 
     # Javascript url.href adds a trailing `/` to root domain urls
     # https://github.com/opengovsg/formsg-javascript-sdk/blob/master/src/webhooks.ts#L25
     u = urlparse(webhook_uri)
     if not u.path:
         u = u._replace(path='/')
     webhook_uri = u.geturl()
 
     formsg_webhook_public_key.verify(
-        smessage=f'{webhook_uri}.{formsg_signature["s"]}.{formsg_signature["f"]}.{formsg_signature["t"]}'.encode('ascii'),
+        smessage='.'.join((
+            webhook_uri,
+            formsg_signature['s'],
+            formsg_signature['f'],
+            formsg_signature['t'],
+        )).encode('ascii'),
         signature=Base64Encoder.decode(formsg_signature['v1']),
     )
 
     if time() - (formsg_signature['t'] / 1000) > signature_expiry_seconds:
         raise BadSignatureError('FormSG signature has expired.')
 
     return formsg_signature
-#end def
 
 
 def decrypt_content(
     body: Mapping[str, Any],
     secret_key: str,  # Base64 encoded secret key
 ) -> Mapping[str, Any]:
-    body = body.get('data', body)  # Some FormSG submissions are in a data field while others are not.
+    # Some FormSG submissions are in a data field while others are not.
+    body = body.get('data', body)
     encrypted_content = body['encryptedContent']
 
     m = encrypted_content_regex.match(encrypted_content)
-    assert m, 'Encrypted content has bad format.'
-    submission_public_key, nonce, encrypted_message = m.groups()
+    if not m:
+        raise ValueError('Encrypted content has bad format.')
+
+    submission_public_key = m.group('submission_public_key')
+    nonce = m.group('nonce')
+    encrypted_message = m.group('encrypted_message')
 
     box = Box(
         PrivateKey(secret_key, encoder=Base64Encoder),
         PublicKey(submission_public_key, encoder=Base64Encoder),
     )
 
-    plaintext = box.decrypt(encrypted_message, Base64Encoder.decode(nonce), encoder=Base64Encoder)
+    plaintext = box.decrypt(
+        encrypted_message,
+        Base64Encoder.decode(nonce),
+        encoder=Base64Encoder,
+    )
 
     return json.loads(plaintext)
-#end def
 
 
 def decrypt_attachment(
     body: Mapping[str, Any],
     field_id: str,
     secret_key: str,  # Base64 encoded secret key
+    timeout: float = 5,  # Default timeout for requests
 ) -> Optional[bytes]:
-    body = body.get('data', body)  # Some FormSG submissions are in a data field while others are not.
+    # Some FormSG submissions are in a data field while others are not.
+    body = body.get('data', body)
 
+    # DEVX-467: `field_id` did not include an attachment; its an optional field
     try:
+        # Either attachmentDownloadUrls or field_id can be missing
         url = body['attachmentDownloadUrls'][field_id]
-    except KeyError:  # DEVX-467: `field_id` did not include an attachment; its an optional field
+    except KeyError:
         return None
 
-    r = requests.get(url)
+    r = requests.get(url, timeout=timeout)
     r.raise_for_status()
 
     attachment_body = r.json()
     encrypted_file: Mapping[str, str] = attachment_body['encryptedFile']
     box = Box(
         PrivateKey(secret_key, encoder=Base64Encoder),
-        PublicKey(encrypted_file['submissionPublicKey'], encoder=Base64Encoder),
+        PublicKey(
+            encrypted_file['submissionPublicKey'],
+            encoder=Base64Encoder,
+        ),
     )
 
-    return box.decrypt(encrypted_file['binary'], Base64Encoder.decode(encrypted_file['nonce']), encoder=Base64Encoder)
-#end def
+    return box.decrypt(
+        encrypted_file['binary'],
+        Base64Encoder.decode(encrypted_file['nonce']),
+        encoder=Base64Encoder,
+    )
```

