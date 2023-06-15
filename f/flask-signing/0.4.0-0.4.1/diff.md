# Comparing `tmp/flask_signing-0.4.0.tar.gz` & `tmp/flask_signing-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_signing-0.4.0.tar", last modified: Thu Jun 15 03:06:43 2023, max compression
+gzip compressed data, was "flask_signing-0.4.1.tar", last modified: Thu Jun 15 19:13:16 2023, max compression
```

## Comparing `flask_signing-0.4.0.tar` & `flask_signing-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 03:06:43.579990 flask_signing-0.4.0/
--rw-rw-r--   0 sig       (1000) sig       (1000)     1503 2023-06-11 20:13:39.000000 flask_signing-0.4.0/LICENSE
--rw-rw-r--   0 sig       (1000) sig       (1000)       81 2023-06-14 04:02:03.000000 flask_signing-0.4.0/MANIFEST.in
--rw-rw-r--   0 sig       (1000) sig       (1000)     3890 2023-06-15 03:06:43.579990 flask_signing-0.4.0/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)     3158 2023-06-14 12:49:49.000000 flask_signing-0.4.0/README.md
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 03:06:43.579990 flask_signing-0.4.0/docs/
--rw-rw-r--   0 sig       (1000) sig       (1000)    78889 2023-06-13 00:10:22.000000 flask_signing-0.4.0/docs/combined.png
--rw-rw-r--   0 sig       (1000) sig       (1000)    65777 2023-06-13 00:01:06.000000 flask_signing-0.4.0/docs/logo.png
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 03:06:43.579990 flask_signing-0.4.0/flask_signing/
--rw-rw-r--   0 sig       (1000) sig       (1000)    13487 2023-06-15 03:05:51.000000 flask_signing-0.4.0/flask_signing/__init__.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 03:06:43.579990 flask_signing-0.4.0/flask_signing.egg-info/
--rw-rw-r--   0 sig       (1000) sig       (1000)     3890 2023-06-15 03:06:43.000000 flask_signing-0.4.0/flask_signing.egg-info/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)      298 2023-06-15 03:06:43.000000 flask_signing-0.4.0/flask_signing.egg-info/SOURCES.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-06-15 03:06:43.000000 flask_signing-0.4.0/flask_signing.egg-info/dependency_links.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-15 03:06:43.000000 flask_signing-0.4.0/flask_signing.egg-info/requires.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       20 2023-06-15 03:06:43.000000 flask_signing-0.4.0/flask_signing.egg-info/top_level.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-06-15 03:06:43.579990 flask_signing-0.4.0/setup.cfg
--rw-rw-r--   0 sig       (1000) sig       (1000)     1237 2023-06-15 03:05:51.000000 flask_signing-0.4.0/setup.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 03:06:43.579990 flask_signing-0.4.0/tests/
--rw-rw-r--   0 sig       (1000) sig       (1000)     7999 2023-06-14 22:09:47.000000 flask_signing-0.4.0/tests/__init__.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 19:13:16.805594 flask_signing-0.4.1/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1503 2023-06-11 20:13:39.000000 flask_signing-0.4.1/LICENSE
+-rw-rw-r--   0 sig       (1000) sig       (1000)       81 2023-06-14 04:02:03.000000 flask_signing-0.4.1/MANIFEST.in
+-rw-rw-r--   0 sig       (1000) sig       (1000)     3890 2023-06-15 19:13:16.805594 flask_signing-0.4.1/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)     3158 2023-06-14 12:49:49.000000 flask_signing-0.4.1/README.md
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 19:13:16.805594 flask_signing-0.4.1/docs/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    78889 2023-06-13 00:10:22.000000 flask_signing-0.4.1/docs/combined.png
+-rw-rw-r--   0 sig       (1000) sig       (1000)    65777 2023-06-13 00:01:06.000000 flask_signing-0.4.1/docs/logo.png
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 19:13:16.805594 flask_signing-0.4.1/flask_signing/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    15435 2023-06-15 19:12:13.000000 flask_signing-0.4.1/flask_signing/__init__.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 19:13:16.805594 flask_signing-0.4.1/flask_signing.egg-info/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     3890 2023-06-15 19:13:16.000000 flask_signing-0.4.1/flask_signing.egg-info/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)      298 2023-06-15 19:13:16.000000 flask_signing-0.4.1/flask_signing.egg-info/SOURCES.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-06-15 19:13:16.000000 flask_signing-0.4.1/flask_signing.egg-info/dependency_links.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-15 19:13:16.000000 flask_signing-0.4.1/flask_signing.egg-info/requires.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       20 2023-06-15 19:13:16.000000 flask_signing-0.4.1/flask_signing.egg-info/top_level.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-06-15 19:13:16.805594 flask_signing-0.4.1/setup.cfg
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1237 2023-06-15 19:12:13.000000 flask_signing-0.4.1/setup.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 19:13:16.805594 flask_signing-0.4.1/tests/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     9760 2023-06-15 18:29:02.000000 flask_signing-0.4.1/tests/__init__.py
```

### Comparing `flask_signing-0.4.0/LICENSE` & `flask_signing-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_signing-0.4.0/PKG-INFO` & `flask_signing-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_signing
-Version: 0.4.0
+Version: 0.4.1
 Summary: a signing key extension for flask
 Home-page: https://github.com/signebedi/Flask-Signing
 Author: Sig Janoska-Bedi
 Author-email: signe@atreeus.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `flask_signing-0.4.0/README.md` & `flask_signing-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `flask_signing-0.4.0/docs/combined.png` & `flask_signing-0.4.1/docs/combined.png`

 * *Files identical despite different names*

### Comparing `flask_signing-0.4.0/docs/logo.png` & `flask_signing-0.4.1/docs/logo.png`

 * *Files identical despite different names*

### Comparing `flask_signing-0.4.0/flask_signing/__init__.py` & `flask_signing-0.4.1/flask_signing/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "flask_signing"
 __author__ = "Sig Janoska-Bedi"
 __credits__ = ["Sig Janoska-Bedi",]
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 __license__ = "BSD-3-Clause"
 __maintainer__ = "Sig Janoska-Bedi"
 __email__ = "signe@atreeus.com"
 
 import datetime, secrets
 from sqlalchemy import func, literal
 from sqlalchemy.exc import SQLAlchemyError
@@ -14,29 +14,31 @@
 
 class Signatures:
     """
     The Signatures class handles operations related to the creation, management, and validation 
     of signing keys in the database.
     """
     
-    def __init__(self, app, byte_len:int=24):
+    def __init__(self, app, safe_mode:bool=True, byte_len:int=24):
         """
         Initializes a new instance of the Signatures class.
 
         Args:
             app (Flask): A flask object to contain the context for database interactions. 
+            safe_mode (bool, optional): If safe_mode is enabled, we will prevent rotation of disabled or rotated keys. Defaults to True.
             byte_len (int, optional): The length of the generated signing keys. Defaults to 24.
         """
 
         self.db = SQLAlchemy(app)
         self.Signing = self.get_model()
         self.db.create_all()  # this will create all necessary tables
 
         # self.db = database
         self.byte_len = byte_len
+        self.safe_mode = safe_mode
 
     def generate_key(self, length:int=None) -> str:
         """
         Generates a signing key with the specified byte length. 
         Note: byte length generally translates to about 1.3 times as many chars,
         see https://docs.python.org/3/library/secrets.html.
 
@@ -47,26 +49,27 @@
             str: The generated signing key.
         """
 
         if not length: 
             length = self.byte_len
         return secrets.token_urlsafe(length)
 
-    def write_key_to_database(self, scope:str=None, expiration:int=1, active:bool=True, email:str=None) -> str:
+    def write_key_to_database(self, scope:str=None, expiration:int=1, active:bool=True, email:str=None, previous_key:str=None) -> str:
         """
         Writes a newly generated signing key to the database.
 
         This function will continuously attempt to generate a key until a unique one is created. 
 
         Args:
             scope (str): The scope within which the signing key will be valid. Defaults to None.
             expiration (int, optional): The number of hours after which the signing key will expire. 
                 If not provided or equals 0, the expiration will be set to zero. Defaults to 1.
             active (bool, optional): The status of the signing key. Defaults to True.
             email (str, optional): The email associated with the signing key. Defaults to None.
+            previous_key (str, optional): The previous key to associate with this key, in the case of key rotation. Defaults to None.
 
         Returns:
             str: The generated and written signing key.
         """
         Signing = self.get_model()
 
         # loop until a unique key is generated
@@ -74,23 +77,30 @@
             key = self.generate_key()
             if not Signing.query.filter_by(signature=key).first(): break
 
         # Convert scope to a list if it's a string
         if isinstance(scope, str):
             scope = [scope]
 
-        new_key = Signing(
-                        signature=key, 
-                        # scope=scope.lower() if scope else "",
-                        scope=[s.lower() for s in scope] if scope else [],
-                        email=email.lower() if email else "", 
-                        active=active,
-                        expiration=(datetime.datetime.utcnow() + datetime.timedelta(hours=expiration)) if expiration else 0,
-                        timestamp=datetime.datetime.utcnow(),
-        )
+        # Here we compile the fields for the new Signing table row
+        SIGNING_FIELDS = {  'signature':key, 
+                    'scope':[s.lower() for s in scope] if scope else [],
+                    'email':email.lower() if email else "", 
+                    'active':active,
+                    'rotated': False,
+                    'expiration':(datetime.datetime.utcnow() + datetime.timedelta(hours=expiration)) if expiration else 0,
+                    'timestamp':datetime.datetime.utcnow(),
+        }
+
+        # If we've passed a parent key, then we modify the new row with the parent ID
+        # Note: this defaults to NULL if not passed.
+        if previous_key:
+            SIGNING_FIELDS['previous_key'] = previous_key
+
+        new_key = Signing(**SIGNING_FIELDS)
 
         self.db.session.add(new_key)
         self.db.session.commit()
 
         return key
 
     def expire_key(self, key):
@@ -183,38 +193,44 @@
             expiration (datetime): The date and time when the signing key is set to expire.
         """
 
         if not hasattr(self, '_model'):
             class Signing(self.db.Model):
                 __tablename__ = 'signing'
                 signature = self.db.Column(self.db.String(1000), primary_key=True) 
-                email = self.db.Column(self.db.String(100))
+                email = self.db.Column(self.db.String(100)) 
                 # scope = self.db.Column(self.db.String(100))
                 # scope = self.db.Column(self.db.MutableList.as_mutable(self.db.String(100)), default=[]),
                 scope = self.db.Column(self.db.JSON())
                 active = self.db.Column(self.db.Boolean)
                 timestamp = self.db.Column(self.db.DateTime, nullable=False, default=datetime.datetime.utcnow)
                 expiration = self.db.Column(self.db.DateTime, nullable=False, default=datetime.datetime.utcnow)
+                # previous_key = self.db.Column(self.db.String(1000), db.ForeignKey('signing.signature'))
+                previous_key = self.db.Column(self.db.String(1000), self.db.ForeignKey('signing.signature'), nullable=True)
+                rotated = self.db.Column(self.db.Boolean)
+                # parent = db.relationship("Signing", remote_side=[signature]) # self referential relationship
+                children = self.db.relationship('Signing', backref=self.db.backref('parent', remote_side=[signature])) # self referential relationship
 
             self._model = Signing
 
         return self._model
 
 
-    def query_keys(self, active:bool=None, scope:str=None, email:str=None) -> Union[List[Dict[str, Any]], bool]:
+    def query_keys(self, active:bool=None, scope:str=None, email:str=None, previous_key:str=None) -> Union[List[Dict[str, Any]], bool]:
         """
-        Query signing keys by active status, scope, and email.
+        Query signing keys by active status, scope, email, and previous_key.
 
         This function returns a list of signing keys that match the provided parameters.
         If no keys are found, it returns False.
 
         Args:
             active (bool, optional): The active status of the signing keys. Defaults to None.
             scope (str, optional): The scope of the signing keys. Defaults to None.
             email (str, optional): The email associated with the signing keys. Defaults to None.
+            previous_key (str, optional): The previous_key associated with the signing keys. Defaults to None.
 
         Returns:
             Union[List[Dict[str, Any]], bool]: A list of dictionaries where each dictionary contains the details of a signing key,
             or False if no keys are found.
         """
 
         Signing = self.get_model()
@@ -242,32 +258,35 @@
             
         # if scope:
         #     query = query.filter(Signing.scope == scope)
 
         if email:
             query = query.filter(Signing.email == email)
 
+        if previous_key:
+            query = query.filter(Signing.previous_key == previous_key)
+
         result = query.all()
 
         if not result:
             return False
 
-        return [{'signature': key.signature, 'email': key.email, 'scope': key.scope, 'active': key.active, 'timestamp': key.timestamp, 'expiration': key.expiration} for key in result]
+        return [{'signature': key.signature, 'email': key.email, 'scope': key.scope, 'active': key.active, 'timestamp': key.timestamp, 'expiration': key.expiration, 'previous_key': key.previous_key, 'rotated': key.rotated} for key in result]
 
     def query_all(self) -> List[Dict[str, Any]]:
 
         """
         Query all values in the Signing table.
         If no keys are found, it returns an empty list.
 
         Returns:
             List[Dict[str, Any]]: A list of dictionaries where each dictionary contains the details of a signing key.
 
         """
-        return [{'signature': key.signature, 'email': key.email, 'scope': key.scope, 'active': key.active, 'timestamp': key.timestamp, 'expiration': key.expiration} for key in self.get_model().query.all()]
+        return [{'signature': key.signature, 'email': key.email, 'scope': key.scope, 'active': key.active, 'timestamp': key.timestamp, 'expiration': key.expiration, 'previous_key': key.previous_key, 'rotated': key.rotated} for key in self.get_model().query.all()]
 
 
     def rotate_keys(self, time_until:int=1, scope=None) -> bool:
         """
         Rotates all keys that are about to expire.
         This is written with the background processes in mind. This can be wrapped in a celerybeat schedule or celery task.
         Args:
@@ -333,24 +352,32 @@
             Signing = self.get_model()
 
             signing_key = Signing.query.filter_by(signature=key).first()
 
             if not signing_key:
                 raise ValueError("No such key exists")
 
+            if self.safe_mode and signing_key.rotated:
+                raise ValueError("Key has already been rotated")
+
+            if self.safe_mode and not signing_key.active:
+                raise ValueError("You cannot rotate a disabled key")
+
             # Disable old key
             signing_key.active = False
+            signing_key.rotated = True
             self.db.session.flush()
 
             # Generate a new key with the same properties
             new_key = self.write_key_to_database(
                 scope=signing_key.scope, 
                 expiration=expiration, 
                 active=True, 
-                email=signing_key.email
+                email=signing_key.email,
+                previous_key=signing_key.signature,  # Assign old key's signature to the previous_key field of new key
             )
             
             self.db.session.commit()
 
         except SQLAlchemyError as e:
             # print(f"An error occurred while rotating the key {key}: {e}")
             return False
```

### Comparing `flask_signing-0.4.0/flask_signing.egg-info/PKG-INFO` & `flask_signing-0.4.1/flask_signing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-signing
-Version: 0.4.0
+Version: 0.4.1
 Summary: a signing key extension for flask
 Home-page: https://github.com/signebedi/Flask-Signing
 Author: Sig Janoska-Bedi
 Author-email: signe@atreeus.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `flask_signing-0.4.0/setup.py` & `flask_signing-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # # Read requirements.txt for install_requires
 # with open("requirements.txt", "r", encoding="utf-8") as fr:
 #     install_requires = fr.read().splitlines()
 
 setup(
     name='flask_signing',
-    version='0.4.0',
+    version='0.4.1',
     url='https://github.com/signebedi/Flask-Signing',
     author='Sig Janoska-Bedi',
     author_email='signe@atreeus.com',
     description='a signing key extension for flask',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

### Comparing `flask_signing-0.4.0/tests/__init__.py` & `flask_signing-0.4.1/tests/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -86,38 +86,53 @@
 
     def test_query_keys(self):
         """
         Test if the query_keys method returns correct records.
         """
         with self.app.app_context():
             key1 = self.signatures.write_key_to_database(scope='test1', email='test1@example.com')
-            key2 = self.signatures.write_key_to_database(scope='test2', email='test2@example.com', active=False)
+            key2 = self.signatures.write_key_to_database(scope='test2', email='test2@example.com', active=True)
+            key3 = self.signatures.rotate_key(key2)  # Generate a new key using rotate_key which assigns previous_key
 
             # Test querying by active status
             result = self.signatures.query_keys(active=True)
             self.assertTrue(all(record['active'] for record in result))
 
             # Test querying by scope
             result = self.signatures.query_keys(scope='test1')
             self.assertTrue(all(record['scope'] == ['test1'] for record in result))
             self.assertTrue(all(type(record['scope']) == list for record in result))
 
             # Test querying by email
             result = self.signatures.query_keys(email='test2@example.com')
             self.assertTrue(all(record['email'] == 'test2@example.com' for record in result))
 
+            # # Test querying by previous_key
+            result = self.signatures.query_keys(previous_key=key2)
+            self.assertTrue(all(record['previous_key'] == key2 for record in result))
+            self.assertTrue(len(result) == 1)            
+            # if result is not False:
+            #     self.assertTrue(all(record['previous_key'] == key2 for record in result))
+            # else:
+            #     self.fail("No records found for previous_key")
+
+            # Check that the rotation does not occur if safe_mode is True and key is already rotated
+            # with self.assertRaises(ValueError):
+            #     self.signatures.rotate_key(key2)
+
             # Test querying by multiple fields
             result = self.signatures.query_keys(active=True, scope='test1', email='test1@example.com')
             self.assertEqual(len(result), 1)
             self.assertEqual(result[0]['signature'], key1)
 
             # Test querying with no results
             result = self.signatures.query_keys(active=True, scope='non-existent-scope')
             self.assertFalse(result)
 
+
     def test_rotate_key(self):
         """
         Test if a key can be rotated and replaced with a new one.
         """
         with self.app.app_context():
             key = self.signatures.write_key_to_database(scope='test')
             Signing = self.signatures.get_model()
@@ -128,26 +143,41 @@
 
             # Check that the new key is different
             self.assertNotEqual(new_key, key)
 
             # Check that the old key is now inactive
             self.assertFalse(signing_key.active)
 
+            # Check that the old key is now marked as rotated
+            self.assertTrue(signing_key.rotated)
+
+            # Check that the rotation does not occur if safe_mode is True and key is already rotated
+            # with self.assertRaises(ValueError):
+            #     self.signatures.rotate_key(key)
+
+            self.assertFalse(self.signatures.rotate_key(key))
+
+            # Check that the new key is not marked as rotated
+            self.assertFalse(Signing.query.filter_by(signature=new_key).first().rotated)
+
+
             # Check that the new key is in the database and active
             new_signing_key = Signing.query.filter_by(signature=new_key).first()
             self.assertIsNotNone(new_signing_key)
             self.assertTrue(new_signing_key.active)
 
             # Check that the new key has the same properties as the old one
             self.assertEqual(signing_key.scope, new_signing_key.scope)
             self.assertEqual(signing_key.email, new_signing_key.email)
             # convert expiration to hours for comparison
             self.assertEqual((signing_key.expiration - datetime.datetime.utcnow()).seconds // 3600, 
-                             (new_signing_key.expiration - datetime.datetime.utcnow()).seconds // 3600)
+                            (new_signing_key.expiration - datetime.datetime.utcnow()).seconds // 3600)
 
+            # Check that the new key's previous_key is the old key
+            self.assertEqual(new_signing_key.previous_key, key)
 
     def test_rotate_keys(self):
         """
         Test if multiple keys can be rotated.
         """
         with self.app.app_context():
             # Create keys that will expire soon
@@ -174,11 +204,15 @@
             # Test rotating keys with a specific scope
             self.signatures.rotate_keys(time_until=2, scope='test3')
 
             # Check that the key with the specific scope has been rotated
             late_expire_signing_key = Signing.query.filter_by(signature=late_expire_key).first()
             self.assertFalse(late_expire_signing_key.active)
 
+            # Get the new key that replaced the late_expire_key
+            new_late_expire_key = Signing.query.filter_by(previous_key=late_expire_key).first()
+            # Check that the new key's previous_key is the old key
+            self.assertEqual(new_late_expire_key.previous_key, late_expire_key)
 
 
 if __name__ == '__main__':
     unittest.main()
```

