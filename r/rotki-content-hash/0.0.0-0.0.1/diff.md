# Comparing `tmp/rotki-content-hash-0.0.0.tar.gz` & `tmp/rotki-content-hash-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotki-content-hash-0.0.0.tar", last modified: Thu Jun 15 18:25:29 2023, max compression
+gzip compressed data, was "rotki-content-hash-0.0.1.tar", last modified: Thu Jun 15 21:48:42 2023, max compression
```

## Comparing `rotki-content-hash-0.0.0.tar` & `rotki-content-hash-0.0.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 18:25:29.414561 rotki-content-hash-0.0.0/
--rw-r--r--   0 lefteris  (1000) users      (100)     1092 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.0/LICENSE
--rw-r--r--   0 lefteris  (1000) users      (100)      192 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.0/MANIFEST.in
--rw-r--r--   0 lefteris  (1000) users      (100)     7441 2023-06-15 18:25:29.414561 rotki-content-hash-0.0.0/PKG-INFO
--rw-r--r--   0 lefteris  (1000) users      (100)     6537 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.0/README.md
-drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 18:25:29.414561 rotki-content-hash-0.0.0/content_hash/
--rw-r--r--   0 lefteris  (1000) users      (100)     1189 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.0/content_hash/__init__.py
--rw-r--r--   0 lefteris  (1000) users      (100)     2407 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.0/content_hash/__main__.py
-drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 18:25:29.414561 rotki-content-hash-0.0.0/content_hash/decodes/
--rw-r--r--   0 lefteris  (1000) users      (100)      514 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.0/content_hash/decodes/__init__.py
--rw-r--r--   0 lefteris  (1000) users      (100)      331 2023-06-15 12:46:16.000000 rotki-content-hash-0.0.0/content_hash/decodes/b58_multi_hash.py
--rw-r--r--   0 lefteris  (1000) users      (100)      356 2023-06-15 12:46:16.000000 rotki-content-hash-0.0.0/content_hash/decodes/hex_multi_hash.py
--rw-r--r--   0 lefteris  (1000) users      (100)      211 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.0/content_hash/decodes/utf8.py
-drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 18:25:29.414561 rotki-content-hash-0.0.0/content_hash/encodes/
--rw-r--r--   0 lefteris  (1000) users      (100)      515 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.0/content_hash/encodes/__init__.py
--rw-r--r--   0 lefteris  (1000) users      (100)      326 2023-06-15 12:46:16.000000 rotki-content-hash-0.0.0/content_hash/encodes/ipfs.py
--rw-r--r--   0 lefteris  (1000) users      (100)      368 2023-06-15 12:46:16.000000 rotki-content-hash-0.0.0/content_hash/encodes/swarm.py
--rw-r--r--   0 lefteris  (1000) users      (100)      210 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.0/content_hash/encodes/utf8.py
-drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 18:25:29.414561 rotki-content-hash-0.0.0/content_hash/profiles/
--rw-r--r--   0 lefteris  (1000) users      (100)     1885 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.0/content_hash/profiles/__init__.py
--rw-r--r--   0 lefteris  (1000) users      (100)      719 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.0/example.py
-drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 18:25:29.414561 rotki-content-hash-0.0.0/rotki_content_hash.egg-info/
--rw-r--r--   0 lefteris  (1000) users      (100)     7441 2023-06-15 18:25:29.000000 rotki-content-hash-0.0.0/rotki_content_hash.egg-info/PKG-INFO
--rw-r--r--   0 lefteris  (1000) users      (100)      727 2023-06-15 18:25:29.000000 rotki-content-hash-0.0.0/rotki_content_hash.egg-info/SOURCES.txt
--rw-r--r--   0 lefteris  (1000) users      (100)        1 2023-06-15 18:25:29.000000 rotki-content-hash-0.0.0/rotki_content_hash.egg-info/dependency_links.txt
--rw-r--r--   0 lefteris  (1000) users      (100)       66 2023-06-15 18:25:29.000000 rotki-content-hash-0.0.0/rotki_content_hash.egg-info/entry_points.txt
--rw-r--r--   0 lefteris  (1000) users      (100)      116 2023-06-15 18:25:29.000000 rotki-content-hash-0.0.0/rotki_content_hash.egg-info/requires.txt
--rw-r--r--   0 lefteris  (1000) users      (100)       13 2023-06-15 18:25:29.000000 rotki-content-hash-0.0.0/rotki_content_hash.egg-info/top_level.txt
--rw-r--r--   0 lefteris  (1000) users      (100)       38 2023-06-15 18:25:29.414561 rotki-content-hash-0.0.0/setup.cfg
--rw-r--r--   0 lefteris  (1000) users      (100)     1483 2023-06-15 18:25:03.000000 rotki-content-hash-0.0.0/setup.py
-drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 18:25:29.414561 rotki-content-hash-0.0.0/tests/
--rw-r--r--   0 lefteris  (1000) users      (100)     1018 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.0/tests/test_command_program.py
--rw-r--r--   0 lefteris  (1000) users      (100)      410 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.0/tests/test_content_hash.py
--rw-r--r--   0 lefteris  (1000) users      (100)      785 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.0/tests/test_profile.py
+drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 21:48:42.028179 rotki-content-hash-0.0.1/
+-rw-r--r--   0 lefteris  (1000) users      (100)     1092 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.1/LICENSE
+-rw-r--r--   0 lefteris  (1000) users      (100)      192 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.1/MANIFEST.in
+-rw-r--r--   0 lefteris  (1000) users      (100)     7441 2023-06-15 21:48:42.028179 rotki-content-hash-0.0.1/PKG-INFO
+-rw-r--r--   0 lefteris  (1000) users      (100)     6537 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.1/README.md
+drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 21:48:42.024845 rotki-content-hash-0.0.1/content_hash/
+-rw-r--r--   0 lefteris  (1000) users      (100)     1214 2023-06-15 20:14:33.000000 rotki-content-hash-0.0.1/content_hash/__init__.py
+-rw-r--r--   0 lefteris  (1000) users      (100)     2407 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.1/content_hash/__main__.py
+drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 21:48:42.028179 rotki-content-hash-0.0.1/content_hash/decodes/
+-rw-r--r--   0 lefteris  (1000) users      (100)      514 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.1/content_hash/decodes/__init__.py
+-rw-r--r--   0 lefteris  (1000) users      (100)      319 2023-06-15 20:56:47.000000 rotki-content-hash-0.0.1/content_hash/decodes/b58_multi_hash.py
+-rw-r--r--   0 lefteris  (1000) users      (100)      299 2023-06-15 21:35:43.000000 rotki-content-hash-0.0.1/content_hash/decodes/hex_multi_hash.py
+-rw-r--r--   0 lefteris  (1000) users      (100)      211 2023-06-15 20:04:42.000000 rotki-content-hash-0.0.1/content_hash/decodes/utf8.py
+drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 21:48:42.028179 rotki-content-hash-0.0.1/content_hash/encodes/
+-rw-r--r--   0 lefteris  (1000) users      (100)      515 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.1/content_hash/encodes/__init__.py
+-rw-r--r--   0 lefteris  (1000) users      (100)      466 2023-06-15 21:32:49.000000 rotki-content-hash-0.0.1/content_hash/encodes/ipfs.py
+-rw-r--r--   0 lefteris  (1000) users      (100)      440 2023-06-15 21:35:54.000000 rotki-content-hash-0.0.1/content_hash/encodes/swarm.py
+-rw-r--r--   0 lefteris  (1000) users      (100)      209 2023-06-15 21:30:09.000000 rotki-content-hash-0.0.1/content_hash/encodes/utf8.py
+drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 21:48:42.028179 rotki-content-hash-0.0.1/content_hash/profiles/
+-rw-r--r--   0 lefteris  (1000) users      (100)     1876 2023-06-15 20:24:43.000000 rotki-content-hash-0.0.1/content_hash/profiles/__init__.py
+-rw-r--r--   0 lefteris  (1000) users      (100)      249 2023-06-15 21:33:00.000000 rotki-content-hash-0.0.1/content_hash/utils.py
+-rw-r--r--   0 lefteris  (1000) users      (100)      719 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.1/example.py
+drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 21:48:42.028179 rotki-content-hash-0.0.1/rotki_content_hash.egg-info/
+-rw-r--r--   0 lefteris  (1000) users      (100)     7441 2023-06-15 21:48:42.000000 rotki-content-hash-0.0.1/rotki_content_hash.egg-info/PKG-INFO
+-rw-r--r--   0 lefteris  (1000) users      (100)      749 2023-06-15 21:48:42.000000 rotki-content-hash-0.0.1/rotki_content_hash.egg-info/SOURCES.txt
+-rw-r--r--   0 lefteris  (1000) users      (100)        1 2023-06-15 21:48:42.000000 rotki-content-hash-0.0.1/rotki_content_hash.egg-info/dependency_links.txt
+-rw-r--r--   0 lefteris  (1000) users      (100)       66 2023-06-15 21:48:42.000000 rotki-content-hash-0.0.1/rotki_content_hash.egg-info/entry_points.txt
+-rw-r--r--   0 lefteris  (1000) users      (100)       98 2023-06-15 21:48:42.000000 rotki-content-hash-0.0.1/rotki_content_hash.egg-info/requires.txt
+-rw-r--r--   0 lefteris  (1000) users      (100)       13 2023-06-15 21:48:42.000000 rotki-content-hash-0.0.1/rotki_content_hash.egg-info/top_level.txt
+-rw-r--r--   0 lefteris  (1000) users      (100)       38 2023-06-15 21:48:42.028179 rotki-content-hash-0.0.1/setup.cfg
+-rw-r--r--   0 lefteris  (1000) users      (100)     1603 2023-06-15 21:47:47.000000 rotki-content-hash-0.0.1/setup.py
+drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 21:48:42.028179 rotki-content-hash-0.0.1/tests/
+-rw-r--r--   0 lefteris  (1000) users      (100)     1018 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.1/tests/test_command_program.py
+-rw-r--r--   0 lefteris  (1000) users      (100)      477 2023-06-15 20:35:10.000000 rotki-content-hash-0.0.1/tests/test_content_hash.py
+-rw-r--r--   0 lefteris  (1000) users      (100)      785 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.1/tests/test_profile.py
```

### Comparing `rotki-content-hash-0.0.0/LICENSE` & `rotki-content-hash-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rotki-content-hash-0.0.0/PKG-INFO` & `rotki-content-hash-0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotki-content-hash
-Version: 0.0.0
+Version: 0.0.1
 Summary: Python implementation of EIP 1577 content hash
 Home-page: https://github.com/filips123/ContentHashPy/
 Author: Filip Š
 Author-email: projects@filips.si
 License: MIT
 Keywords: ethereum,ethereum-name-service,ens,eip1577,web3,decentralized
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rotki-content-hash-0.0.0/README.md` & `rotki-content-hash-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `rotki-content-hash-0.0.0/content_hash/__init__.py` & `rotki-content-hash-0.0.1/content_hash/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 """Python implementation of EIP 1577 content hash."""
 
-import multihash
-import multicodec
+from multiformats import multicodec
 
 from .profiles import get_profile
 
 
 def decode(chash):
     """
     Decode a content hash.
 
     :param str hash: a hex string containing a content hash
 
     :return: the decoded content
     :rtype: str
     """
+    buffer = bytes.fromhex(chash.lstrip('0x'))
 
-    buffer = multihash.from_hex_string(chash.lstrip('0x'))
-
-    codec = multicodec.get_codec(buffer)
-    value = multicodec.remove_prefix(buffer)
-
-    profile = get_profile(codec)
-    return profile.decode(value)
+    codec, value = multicodec.unwrap(buffer)
+    profile = get_profile(codec.name)
+    result = profile.decode(value)
+    if isinstance(result, bytes):
+        result = result.decode()
+    return result
 
 
 def encode(codec, value):
     """
     Encode a content hash.
 
     :param str codec: a codec of a content hash
@@ -35,23 +34,24 @@
     :return: the resulting content hash
     :rtype: str
     """
 
     profile = get_profile(codec)
 
     value = profile.encode(value)
-    value = multicodec.add_prefix(codec, value)
-    return multihash.to_hex_string(value)
+    value = multicodec.wrap(codec, value)
+    return value.hex()
 
 
 def get_codec(chash):
     """
     Extract the codec of a content hash
 
     :param str hash: a hex string containing a content hash
 
     :return: the extracted codec
     :rtype: str
     """
 
-    buffer = multihash.from_hex_string(chash.lstrip('0x'))
-    return multicodec.get_codec(buffer)
+    buffer = bytes.fromhex(chash.lstrip('0x'))
+    codec, _ =  multicodec.unwrap(buffer)
+    return codec.name
```

### Comparing `rotki-content-hash-0.0.0/content_hash/__main__.py` & `rotki-content-hash-0.0.1/content_hash/__main__.py`

 * *Files identical despite different names*

### Comparing `rotki-content-hash-0.0.0/content_hash/decodes/__init__.py` & `rotki-content-hash-0.0.1/content_hash/decodes/__init__.py`

 * *Files identical despite different names*

### Comparing `rotki-content-hash-0.0.0/content_hash/encodes/__init__.py` & `rotki-content-hash-0.0.1/content_hash/encodes/__init__.py`

 * *Files identical despite different names*

### Comparing `rotki-content-hash-0.0.0/content_hash/profiles/__init__.py` & `rotki-content-hash-0.0.1/content_hash/profiles/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,17 +64,17 @@
     :rtype: Profile
     """
 
     return PROFILES.get(name, PROFILES['default'])
 
 
 PROFILES = {
-    'ipfs-ns': Profile(decode='b58_multi_hash', encode='ipfs'),
-    'ipns-ns': Profile(decode='b58_multi_hash', encode='ipfs'),
-    'swarm-ns': Profile(decode='hex_multi_hash', encode='swarm'),
+    'ipfs': Profile(decode='b58_multi_hash', encode='ipfs'),
+    'ipns': Profile(decode='b58_multi_hash', encode='ipfs'),
+    'swarm': Profile(decode='hex_multi_hash', encode='swarm'),
     'default': Profile(decode='utf8', encode='utf8'),
 }
 """
 dict: a dict of known profiles
 
 `encode` should be chosen among the `encode` modules
 `decode` should be chosen among the `decode` modules
```

### Comparing `rotki-content-hash-0.0.0/example.py` & `rotki-content-hash-0.0.1/example.py`

 * *Files identical despite different names*

### Comparing `rotki-content-hash-0.0.0/rotki_content_hash.egg-info/PKG-INFO` & `rotki-content-hash-0.0.1/rotki_content_hash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotki-content-hash
-Version: 0.0.0
+Version: 0.0.1
 Summary: Python implementation of EIP 1577 content hash
 Home-page: https://github.com/filips123/ContentHashPy/
 Author: Filip Š
 Author-email: projects@filips.si
 License: MIT
 Keywords: ethereum,ethereum-name-service,ens,eip1577,web3,decentralized
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rotki-content-hash-0.0.0/rotki_content_hash.egg-info/SOURCES.txt` & `rotki-content-hash-0.0.1/rotki_content_hash.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 example.py
 setup.py
 content_hash/__init__.py
 content_hash/__main__.py
+content_hash/utils.py
 content_hash/decodes/__init__.py
 content_hash/decodes/b58_multi_hash.py
 content_hash/decodes/hex_multi_hash.py
 content_hash/decodes/utf8.py
 content_hash/encodes/__init__.py
 content_hash/encodes/ipfs.py
 content_hash/encodes/swarm.py
```

### Comparing `rotki-content-hash-0.0.0/setup.py` & `rotki-content-hash-0.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,27 +7,28 @@
 
 setup(
     name = 'rotki-content-hash',
     description = 'Python implementation of EIP 1577 content hash',
     long_description = readme(),
     long_description_content_type='text/markdown',
     license = 'MIT',
-
+    version='0.0.1',
     setup_requires = ['setuptools-git-version'],
 
     packages = ['content_hash'],
 
     entry_points = {
         'console_scripts': ['rotki-content-hash=content_hash.__main__:main'],
     },
 
     install_requires = [
-        'py-multiformats-cid',
-        'py-multicodec>=0.2.1,<0.3.0',
-        'py-multihash>=0.2.3,<0.3.0',
+        'multiformats',
+        'base58check',  # for b58 encode/decode
+        'pysha3',  # for keccak-256
+        'typing_extensions==4.5.0',  # due to https://github.com/hashberg-io/multiformats/issues/10
     ],
 
     extras_require = {
         'lint': ['pylint'],
         'test': ['pytest', 'pytest-cov'],
     },
```

### Comparing `rotki-content-hash-0.0.0/tests/test_command_program.py` & `rotki-content-hash-0.0.1/tests/test_command_program.py`

 * *Files identical despite different names*

### Comparing `rotki-content-hash-0.0.0/tests/test_profile.py` & `rotki-content-hash-0.0.1/tests/test_profile.py`

 * *Files identical despite different names*

