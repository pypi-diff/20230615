# Comparing `tmp/flask_signing-0.3.2.tar.gz` & `tmp/flask_signing-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_signing-0.3.2.tar", last modified: Wed Jun 14 04:51:39 2023, max compression
+gzip compressed data, was "flask_signing-0.4.0.tar", last modified: Thu Jun 15 03:06:43 2023, max compression
```

## Comparing `flask_signing-0.3.2.tar` & `flask_signing-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-14 04:51:39.478585 flask_signing-0.3.2/
--rw-rw-r--   0 sig       (1000) sig       (1000)     1503 2023-06-11 20:13:39.000000 flask_signing-0.3.2/LICENSE
--rw-rw-r--   0 sig       (1000) sig       (1000)       81 2023-06-14 04:02:03.000000 flask_signing-0.3.2/MANIFEST.in
--rw-rw-r--   0 sig       (1000) sig       (1000)     3690 2023-06-14 04:51:39.478585 flask_signing-0.3.2/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)     2958 2023-06-14 04:02:56.000000 flask_signing-0.3.2/README.md
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-14 04:51:39.478585 flask_signing-0.3.2/docs/
--rw-rw-r--   0 sig       (1000) sig       (1000)    78889 2023-06-13 00:10:22.000000 flask_signing-0.3.2/docs/combined.png
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-14 04:51:39.478585 flask_signing-0.3.2/docs/flask_signing/
--rw-rw-r--   0 sig       (1000) sig       (1000)    45030 2023-06-14 04:50:41.000000 flask_signing-0.3.2/docs/flask_signing/index.html
--rw-rw-r--   0 sig       (1000) sig       (1000)    65777 2023-06-13 00:01:06.000000 flask_signing-0.3.2/docs/logo.png
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-14 04:51:39.478585 flask_signing-0.3.2/flask_signing/
--rw-rw-r--   0 sig       (1000) sig       (1000)    10013 2023-06-14 04:50:41.000000 flask_signing-0.3.2/flask_signing/__init__.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-14 04:51:39.478585 flask_signing-0.3.2/flask_signing.egg-info/
--rw-rw-r--   0 sig       (1000) sig       (1000)     3690 2023-06-14 04:51:39.000000 flask_signing-0.3.2/flask_signing.egg-info/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)      328 2023-06-14 04:51:39.000000 flask_signing-0.3.2/flask_signing.egg-info/SOURCES.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-06-14 04:51:39.000000 flask_signing-0.3.2/flask_signing.egg-info/dependency_links.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-14 04:51:39.000000 flask_signing-0.3.2/flask_signing.egg-info/requires.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       20 2023-06-14 04:51:39.000000 flask_signing-0.3.2/flask_signing.egg-info/top_level.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-06-14 04:51:39.478585 flask_signing-0.3.2/setup.cfg
--rw-rw-r--   0 sig       (1000) sig       (1000)     1237 2023-06-14 04:50:41.000000 flask_signing-0.3.2/setup.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-14 04:51:39.478585 flask_signing-0.3.2/tests/
--rw-rw-r--   0 sig       (1000) sig       (1000)     4964 2023-06-13 22:43:17.000000 flask_signing-0.3.2/tests/__init__.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 03:06:43.579990 flask_signing-0.4.0/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1503 2023-06-11 20:13:39.000000 flask_signing-0.4.0/LICENSE
+-rw-rw-r--   0 sig       (1000) sig       (1000)       81 2023-06-14 04:02:03.000000 flask_signing-0.4.0/MANIFEST.in
+-rw-rw-r--   0 sig       (1000) sig       (1000)     3890 2023-06-15 03:06:43.579990 flask_signing-0.4.0/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)     3158 2023-06-14 12:49:49.000000 flask_signing-0.4.0/README.md
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 03:06:43.579990 flask_signing-0.4.0/docs/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    78889 2023-06-13 00:10:22.000000 flask_signing-0.4.0/docs/combined.png
+-rw-rw-r--   0 sig       (1000) sig       (1000)    65777 2023-06-13 00:01:06.000000 flask_signing-0.4.0/docs/logo.png
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 03:06:43.579990 flask_signing-0.4.0/flask_signing/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    13487 2023-06-15 03:05:51.000000 flask_signing-0.4.0/flask_signing/__init__.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 03:06:43.579990 flask_signing-0.4.0/flask_signing.egg-info/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     3890 2023-06-15 03:06:43.000000 flask_signing-0.4.0/flask_signing.egg-info/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)      298 2023-06-15 03:06:43.000000 flask_signing-0.4.0/flask_signing.egg-info/SOURCES.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-06-15 03:06:43.000000 flask_signing-0.4.0/flask_signing.egg-info/dependency_links.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-15 03:06:43.000000 flask_signing-0.4.0/flask_signing.egg-info/requires.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       20 2023-06-15 03:06:43.000000 flask_signing-0.4.0/flask_signing.egg-info/top_level.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-06-15 03:06:43.579990 flask_signing-0.4.0/setup.cfg
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1237 2023-06-15 03:05:51.000000 flask_signing-0.4.0/setup.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 03:06:43.579990 flask_signing-0.4.0/tests/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     7999 2023-06-14 22:09:47.000000 flask_signing-0.4.0/tests/__init__.py
```

### Comparing `flask_signing-0.3.2/LICENSE` & `flask_signing-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_signing-0.3.2/PKG-INFO` & `flask_signing-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_signing
-Version: 0.3.2
+Version: 0.4.0
 Summary: a signing key extension for flask
 Home-page: https://github.com/signebedi/Flask-Signing
 Author: Sig Janoska-Bedi
 Author-email: signe@atreeus.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -19,14 +19,15 @@
 
 ![Signing logo](https://raw.githubusercontent.com/signebedi/Flask-Signing/master/docs/combined.png)
 
 ## Flask-Signing
 
 [![License: BSD-3-Clause](https://img.shields.io/github/license/signebedi/Flask-Signing?color=dark-green)](https://github.com/signebedi/Flask-Signing/blob/master/LICENSE) 
 [![PyPI version](https://badge.fury.io/py/Flask-Signing.svg)](https://pypi.org/project/flask-signing/)
+[![Downloads](https://static.pepy.tech/personalized-badge/flask-signing?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/flask-signing)
 [![Flask-Signing tests](https://github.com/signebedi/Flask-Signing/workflows/tests/badge.svg)](https://github.com/signebedi/Flask-Signing/actions)
 
 a signing key extension for flask
 
 
 ### About
 
@@ -80,8 +81,8 @@
 
 In this example, a new signing key is generated and written to the database when you visit the /sign route, and the key is displayed on the page. Then, when you visit the /verify/<key> route (replace <key> with the actual key), the validity of the key is checked and displayed. You can expire a key using the /expire/<key> route, and view all records with the /all route.
 
 Please note that this is a very basic example and your actual use of the flask_signing package may be more complex depending on your needs. It's important to secure your signing keys and handle them appropriately according to your application's security requirements.
 
 ### Developers
 
-Contributions are welcome! You can read the developer docs at https://signebedi.github.io/Flask-Signing/flask_signing/. If you're interested, review (or add to) the feature ideas at https://github.com/signebedi/Flask-Signing/issues.
+Contributions are welcome! You can read the developer docs at https://signebedi.github.io/Flask-Signing. If you're interested, review (or add to) the feature ideas at https://github.com/signebedi/Flask-Signing/issues.
```

### Comparing `flask_signing-0.3.2/README.md` & `flask_signing-0.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ![Signing logo](https://raw.githubusercontent.com/signebedi/Flask-Signing/master/docs/combined.png)
 
 ## Flask-Signing
 
 [![License: BSD-3-Clause](https://img.shields.io/github/license/signebedi/Flask-Signing?color=dark-green)](https://github.com/signebedi/Flask-Signing/blob/master/LICENSE) 
 [![PyPI version](https://badge.fury.io/py/Flask-Signing.svg)](https://pypi.org/project/flask-signing/)
+[![Downloads](https://static.pepy.tech/personalized-badge/flask-signing?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/flask-signing)
 [![Flask-Signing tests](https://github.com/signebedi/Flask-Signing/workflows/tests/badge.svg)](https://github.com/signebedi/Flask-Signing/actions)
 
 a signing key extension for flask
 
 
 ### About
 
@@ -61,8 +62,8 @@
 
 In this example, a new signing key is generated and written to the database when you visit the /sign route, and the key is displayed on the page. Then, when you visit the /verify/<key> route (replace <key> with the actual key), the validity of the key is checked and displayed. You can expire a key using the /expire/<key> route, and view all records with the /all route.
 
 Please note that this is a very basic example and your actual use of the flask_signing package may be more complex depending on your needs. It's important to secure your signing keys and handle them appropriately according to your application's security requirements.
 
 ### Developers
 
-Contributions are welcome! You can read the developer docs at https://signebedi.github.io/Flask-Signing/flask_signing/. If you're interested, review (or add to) the feature ideas at https://github.com/signebedi/Flask-Signing/issues.
+Contributions are welcome! You can read the developer docs at https://signebedi.github.io/Flask-Signing. If you're interested, review (or add to) the feature ideas at https://github.com/signebedi/Flask-Signing/issues.
```

### Comparing `flask_signing-0.3.2/docs/combined.png` & `flask_signing-0.4.0/docs/combined.png`

 * *Files identical despite different names*

### Comparing `flask_signing-0.3.2/docs/logo.png` & `flask_signing-0.4.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `flask_signing-0.3.2/flask_signing/__init__.py` & `flask_signing-0.4.0/flask_signing/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 __name__ = "flask_signing"
 __author__ = "Sig Janoska-Bedi"
 __credits__ = ["Sig Janoska-Bedi",]
-__version__ = "0.3.2"
+__version__ = "0.4.0"
 __license__ = "BSD-3-Clause"
 __maintainer__ = "Sig Janoska-Bedi"
 __email__ = "signe@atreeus.com"
 
 import datetime, secrets
 from sqlalchemy import func, literal
+from sqlalchemy.exc import SQLAlchemyError
 from flask_sqlalchemy import SQLAlchemy
 from typing import Union, List, Dict, Any
 
 class Signatures:
     """
     The Signatures class handles operations related to the creation, management, and validation 
     of signing keys in the database.
@@ -258,8 +259,104 @@
         Query all values in the Signing table.
         If no keys are found, it returns an empty list.
 
         Returns:
             List[Dict[str, Any]]: A list of dictionaries where each dictionary contains the details of a signing key.
 
         """
-        return [{'signature': key.signature, 'email': key.email, 'scope': key.scope, 'active': key.active, 'timestamp': key.timestamp, 'expiration': key.expiration} for key in self.get_model().query.all()]
+        return [{'signature': key.signature, 'email': key.email, 'scope': key.scope, 'active': key.active, 'timestamp': key.timestamp, 'expiration': key.expiration} for key in self.get_model().query.all()]
+
+
+    def rotate_keys(self, time_until:int=1, scope=None) -> bool:
+        """
+        Rotates all keys that are about to expire.
+        This is written with the background processes in mind. This can be wrapped in a celerybeat schedule or celery task.
+        Args:
+            time_until (int): rotate keys that are set to expire in this many hours.
+            scope (str, list): rotate keys within this scope. If None, all scopes are considered.
+        Returns:
+            bool: operation succeeded/failed.
+        """
+        try:
+            Signing = self.get_model()
+
+            # get keys that will expire in the next time_until hours
+            query = Signing.query.filter(
+                Signing.expiration <= (datetime.datetime.utcnow() + datetime.timedelta(hours=time_until)),
+                Signing.active == True
+            )
+
+            # if scope is not None:
+            #     if isinstance(scope, list):
+            #         query = query.filter(Signing.scope.in_(scope))
+            #     else:
+            #         query = query.filter_by(scope=scope)
+
+            # Convert scope to a list if it's a string
+            if isinstance(scope, str):
+                scope = [scope]
+
+            if scope:
+
+                for s in scope:
+                    # https://stackoverflow.com/a/44250678/13301284
+                    query = query.filter(Signing.scope.comparator.contains(s))
+
+            expiring_keys = query.all()
+
+            for key in expiring_keys:
+                self.rotate_key(key.signature)
+
+        except SQLAlchemyError as e:
+            # This will catch any SQLAlchemy related exceptions
+            print(f"An error occurred while rotating keys: {e}")
+            return False
+
+        except Exception as e:
+            # This will catch any other kind of unexpected exceptions
+            print(f"An unexpected error occurred: {e}")
+            return False
+
+        # We may need to potentially modify the return behavior to provide greater detail ... 
+        # for example, a list of old keys mapped to their new keys and emails.
+        return True
+
+    def rotate_key(self, key: str, expiration:int=1) -> str:
+        """
+        Replaces an active key with a new key with the same properties, and sets the old key as inactive.
+        Args:
+            key (str): The signing key to be rotated.
+            expiration (int): The number of hours until the new key will expire.
+        Returns:
+            str: The new signing key.
+        """
+        try:
+            Signing = self.get_model()
+
+            signing_key = Signing.query.filter_by(signature=key).first()
+
+            if not signing_key:
+                raise ValueError("No such key exists")
+
+            # Disable old key
+            signing_key.active = False
+            self.db.session.flush()
+
+            # Generate a new key with the same properties
+            new_key = self.write_key_to_database(
+                scope=signing_key.scope, 
+                expiration=expiration, 
+                active=True, 
+                email=signing_key.email
+            )
+            
+            self.db.session.commit()
+
+        except SQLAlchemyError as e:
+            # print(f"An error occurred while rotating the key {key}: {e}")
+            return False
+
+        except Exception as e:
+            # print(f"An unexpected error occurred: {e}")
+            return False
+
+        return new_key
```

### Comparing `flask_signing-0.3.2/flask_signing.egg-info/PKG-INFO` & `flask_signing-0.4.0/flask_signing.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-signing
-Version: 0.3.2
+Version: 0.4.0
 Summary: a signing key extension for flask
 Home-page: https://github.com/signebedi/Flask-Signing
 Author: Sig Janoska-Bedi
 Author-email: signe@atreeus.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -19,14 +19,15 @@
 
 ![Signing logo](https://raw.githubusercontent.com/signebedi/Flask-Signing/master/docs/combined.png)
 
 ## Flask-Signing
 
 [![License: BSD-3-Clause](https://img.shields.io/github/license/signebedi/Flask-Signing?color=dark-green)](https://github.com/signebedi/Flask-Signing/blob/master/LICENSE) 
 [![PyPI version](https://badge.fury.io/py/Flask-Signing.svg)](https://pypi.org/project/flask-signing/)
+[![Downloads](https://static.pepy.tech/personalized-badge/flask-signing?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/flask-signing)
 [![Flask-Signing tests](https://github.com/signebedi/Flask-Signing/workflows/tests/badge.svg)](https://github.com/signebedi/Flask-Signing/actions)
 
 a signing key extension for flask
 
 
 ### About
 
@@ -80,8 +81,8 @@
 
 In this example, a new signing key is generated and written to the database when you visit the /sign route, and the key is displayed on the page. Then, when you visit the /verify/<key> route (replace <key> with the actual key), the validity of the key is checked and displayed. You can expire a key using the /expire/<key> route, and view all records with the /all route.
 
 Please note that this is a very basic example and your actual use of the flask_signing package may be more complex depending on your needs. It's important to secure your signing keys and handle them appropriately according to your application's security requirements.
 
 ### Developers
 
-Contributions are welcome! You can read the developer docs at https://signebedi.github.io/Flask-Signing/flask_signing/. If you're interested, review (or add to) the feature ideas at https://github.com/signebedi/Flask-Signing/issues.
+Contributions are welcome! You can read the developer docs at https://signebedi.github.io/Flask-Signing. If you're interested, review (or add to) the feature ideas at https://github.com/signebedi/Flask-Signing/issues.
```

### Comparing `flask_signing-0.3.2/setup.py` & `flask_signing-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # # Read requirements.txt for install_requires
 # with open("requirements.txt", "r", encoding="utf-8") as fr:
 #     install_requires = fr.read().splitlines()
 
 setup(
     name='flask_signing',
-    version='0.3.2',
+    version='0.4.0',
     url='https://github.com/signebedi/Flask-Signing',
     author='Sig Janoska-Bedi',
     author_email='signe@atreeus.com',
     description='a signing key extension for flask',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

