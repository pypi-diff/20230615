# Comparing `tmp/jerryrigserialgen-0.10.tar.gz` & `tmp/jerryrigserialgen-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jerryrigserialgen-0.10.tar", last modified: Thu Mar 23 13:23:32 2023, max compression
+gzip compressed data, was "jerryrigserialgen-0.11.tar", last modified: Thu Jun 15 03:00:41 2023, max compression
```

## Comparing `jerryrigserialgen-0.10.tar` & `jerryrigserialgen-0.11.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 13:23:32.383285 jerryrigserialgen-0.10/
--rw-rw-rw-   0        0        0     1148 2023-03-23 13:23:05.000000 jerryrigserialgen-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      157 2023-03-23 13:23:04.000000 jerryrigserialgen-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     4175 2023-03-23 13:23:32.384282 jerryrigserialgen-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     3122 2023-03-23 13:19:37.000000 jerryrigserialgen-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-03-23 13:23:32.379295 jerryrigserialgen-0.10/jerryrigserialgen/
--rw-rw-rw-   0        0        0     1090 2022-10-05 20:27:47.000000 jerryrigserialgen-0.10/jerryrigserialgen/LICENSE
--rw-rw-rw-   0        0        0     3122 2023-03-23 13:19:37.000000 jerryrigserialgen-0.10/jerryrigserialgen/README.MD
--rw-rw-rw-   0        0        0    11436 2023-03-23 12:43:20.000000 jerryrigserialgen-0.10/jerryrigserialgen/__init__.py
--rw-rw-rw-   0        0        0       71 2023-03-23 13:23:30.000000 jerryrigserialgen-0.10/jerryrigserialgen/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-03-23 13:23:30.000000 jerryrigserialgen-0.10/jerryrigserialgen/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-03-23 13:23:32.383285 jerryrigserialgen-0.10/jerryrigserialgen.egg-info/
--rw-rw-rw-   0        0        0     4175 2023-03-23 13:23:32.000000 jerryrigserialgen-0.10/jerryrigserialgen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-03-23 13:23:32.000000 jerryrigserialgen-0.10/jerryrigserialgen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 13:23:32.000000 jerryrigserialgen-0.10/jerryrigserialgen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-03-23 13:23:32.000000 jerryrigserialgen-0.10/jerryrigserialgen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-03-23 13:23:32.000000 jerryrigserialgen-0.10/jerryrigserialgen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-03-23 13:23:32.384781 jerryrigserialgen-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1637 2023-03-23 13:23:30.000000 jerryrigserialgen-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 03:00:41.591423 jerryrigserialgen-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-06-15 03:00:31.000000 jerryrigserialgen-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      157 2023-06-15 03:00:30.000000 jerryrigserialgen-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     4039 2023-06-15 03:00:41.591423 jerryrigserialgen-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     3314 2023-06-15 02:58:57.000000 jerryrigserialgen-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 03:00:41.587433 jerryrigserialgen-0.11/jerryrigserialgen/
+-rw-rw-rw-   0        0        0     1090 2023-04-15 00:18:29.000000 jerryrigserialgen-0.11/jerryrigserialgen/LICENSE
+-rw-rw-rw-   0        0        0     3314 2023-06-15 02:58:57.000000 jerryrigserialgen-0.11/jerryrigserialgen/README.MD
+-rw-rw-rw-   0        0        0    11586 2023-06-15 02:56:00.000000 jerryrigserialgen-0.11/jerryrigserialgen/__init__.py
+-rw-rw-rw-   0        0        0       71 2023-06-15 03:00:40.000000 jerryrigserialgen-0.11/jerryrigserialgen/requirements.txt
+-rw-rw-rw-   0        0        0    19812 2023-06-15 03:00:40.000000 jerryrigserialgen-0.11/jerryrigserialgen/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-06-15 03:00:41.590425 jerryrigserialgen-0.11/jerryrigserialgen.egg-info/
+-rw-rw-rw-   0        0        0     4039 2023-06-15 03:00:41.000000 jerryrigserialgen-0.11/jerryrigserialgen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-06-15 03:00:41.000000 jerryrigserialgen-0.11/jerryrigserialgen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 03:00:41.000000 jerryrigserialgen-0.11/jerryrigserialgen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-06-15 03:00:41.000000 jerryrigserialgen-0.11/jerryrigserialgen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-15 03:00:41.000000 jerryrigserialgen-0.11/jerryrigserialgen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-06-15 03:00:41.591423 jerryrigserialgen-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1537 2023-06-15 03:00:40.000000 jerryrigserialgen-0.11/setup.py
```

### Comparing `jerryrigserialgen-0.10/LICENSE.rst` & `jerryrigserialgen-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `jerryrigserialgen-0.10/PKG-INFO` & `jerryrigserialgen-0.11/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,86 @@
 Metadata-Version: 2.1
 Name: jerryrigserialgen
-Version: 0.10
+Version: 0.11
 Summary: jerry-rigged license system with UUID check (preventing more than one installation) and expiration date
 Home-page: https://github.com/hansalemaos/jerryrigserialgen
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: UUID,license system,expiration date,serial number
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Editors :: Text Processing
-Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
 
-# jerry-rigged license system with UUID check (preventing more than one installation) and expiration date
-
-### Tested against Python 3.9.16 (Anaconda) -  Windows 10
-
-#### jerry-rigged???
-
-From https://www.urbandictionary.com/define.php?term=jerry-rig
-jerry-rig - To put together in a way that works, but is contrary to the "norm" or specific directions (instructions)
-
-The serial number system can be cracked easily (which one can't?), but it should be secure enough for any average user.
-
-### pip install jerryrigserialgen - if you want to generate serial numbers
-
-### pip install jerryrigserialver - if you want to verify serial numbers (client)
-
-
-```python
-from jerryrigserialgen import Serialgenerator
-
-# Generates serial numbers
-# pip install jerryrigserialgen
-seri = Serialgenerator(
-    product="myproduct",  # Name of the product
-    savefolder="c:\\mynicefolder\\new",  # just for the record - files are not needed
-    hardcodedpasswort_transfer="topsecret",  # for transfer.sh - must be hard-coded in the app the client uses
-    hardcodedpasswort_url="5248614597016233",  # 16 digits to encrypt the URL - must be hard-coded in the app the client uses
-    addinformationtoserial=(
-        "info1",
-        "info2",
-    ),  # extra information you want to transmit to the app the client uses
-    licensedays=17,  # duration of the license - from today on
-    subtract_from_time=0,  # for debugging - to create expired licenses
-)
-serialnumber, debuginfo = seri.upload()
-print(serialnumber) # This is the serial number you are going to give to your client, like: 566978376a4b356956775955427a4779636e533856705a59534d314369387735526e59744230396f6c6771795256675a31365a756947344753616d3757536d5961704f736a362f63506871724a792f3845664d4845773d3d475ac18a6927938b4ede1613058f253e
-
-# output
-# File written to: c:\mynicefolder\new\2023_03_23_09_23_18_28484401.cfg
-# 566978376a4b356956775955427a4779636e533856705a59534d314369387735526e59744230396f6c6771795256675a31365a756947344753616d3757536d5961704f736a362f63506871724a792f3845664d4845773d3d475ac18a6927938b4ede1613058f253e
-
-##########################################################################
-
-# Check serial numbers - client's PC
-
-# pip install jerryrigserialver
-from jerryrigserialver import check_serial
-
-isvalid, daysleft, duration_of_license, product, otherinfos = check_serial(
-    hardcodedpasswort_transfer="topsecret",
-    # hardcodedpasswort_transfer for transfer.sh - must be hard-coded
-    hardcodedpasswort_url="5248614597016233",  # 16 digits to encrypt the url - must be hard-coded
-    serialnumber=serialnumber,
-    notvalidanymore=f"The license you're using is not valid anymore. It expired %d day[s] ago",
-    stillvalid=f"The license you're using is valid for %d more day[s].",
-    serialusedanotherpc="The license has been used on another PC",
-)
-print(isvalid, daysleft, duration_of_license, product, otherinfos)
-
-
-# The license you're using is valid for 17 more day[s].
-# True 17 17 myproduct ['info1', 'info2']
-
-# Compile the code of your app using PyInstaller or some other tool
+# jerry-rigged license system with UUID check (preventing more than one installation) and expiration date
+
+### Tested against Python 3.9.16 (Anaconda) -  Windows 10
+
+#### jerry-rigged???
+
+From https://www.urbandictionary.com/define.php?term=jerry-rig
+jerry-rig - To put together in a way that works, but is contrary to the "norm" or specific directions (instructions)
+
+The serial number system can be cracked easily (which one can't?), but it should be secure enough for any average user.
+
+### pip install jerryrigserialgen - if you want to generate serial numbers
+
+### pip install jerryrigserialver - if you want to verify serial numbers (client)
+
+
+```python
+from jerryrigserialgen import Serialgenerator, serialgenconfig
+
+# transfer.sh seems to be offline (https://github.com/dutchcoders/transfer.sh/issues/556), that's why i added this:
+serialgenconfig.transfershdomain = 'https://temp.sh'
+
+# Generates serial numbers
+# pip install jerryrigserialgen
+seri = Serialgenerator(
+    product="myproduct",  # Name of the product
+    savefolder="c:\\mynicefolder\\new",  # just for the record - files are not needed
+    hardcodedpasswort_transfer="topsecret",  # for transfer.sh - must be hard-coded in the app the client uses
+    hardcodedpasswort_url="5248614597016233",  # 16 digits to encrypt the URL - must be hard-coded in the app the client uses
+    addinformationtoserial=(
+        "info1",
+        "info2",
+    ),  # extra information you want to transmit to the app the client uses
+    licensedays=17,  # duration of the license - from today on
+    subtract_from_time=0,  # for debugging - to create expired licenses
+)
+serialnumber, debuginfo = seri.upload()
+print(serialnumber) # This is the serial number you are going to give to your client, like: 566978376a4b356956775955427a4779636e533856705a59534d314369387735526e59744230396f6c6771795256675a31365a756947344753616d3757536d5961704f736a362f63506871724a792f3845664d4845773d3d475ac18a6927938b4ede1613058f253e
+
+
+# output
+# File written to: c:\mynicefolder\new\2023_03_23_09_23_18_28484401.cfg
+# 566978376a4b356956775955427a4779636e533856705a59534d314369387735526e59744230396f6c6771795256675a31365a756947344753616d3757536d5961704f736a362f63506871724a792f3845664d4845773d3d475ac18a6927938b4ede1613058f253e
+
+##########################################################################
+
+# Check serial numbers - client's PC
+
+# pip install jerryrigserialver
+from jerryrigserialver import check_serial
+
+isvalid, daysleft, duration_of_license, product, otherinfos = check_serial(
+    hardcodedpasswort_transfer="topsecret",
+    # hardcodedpasswort_transfer for transfer.sh - must be hard-coded
+    hardcodedpasswort_url="5248614597016233",  # 16 digits to encrypt the url - must be hard-coded
+    serialnumber=serialnumber,
+    notvalidanymore=f"The license you're using is not valid anymore. It expired %d day[s] ago",
+    stillvalid=f"The license you're using is valid for %d more day[s].",
+    serialusedanotherpc="The license has been used on another PC",
+)
+print(isvalid, daysleft, duration_of_license, product, otherinfos)
+
+
+# The license you're using is valid for 17 more day[s].
+# True 17 17 myproduct ['info1', 'info2']
+
+# Compile the code of your app using PyInstaller or some other tool
 ```
```

### Comparing `jerryrigserialgen-0.10/README.md` & `jerryrigserialgen-0.11/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 
 ### pip install jerryrigserialgen - if you want to generate serial numbers
 
 ### pip install jerryrigserialver - if you want to verify serial numbers (client)
 
 
 ```python
-from jerryrigserialgen import Serialgenerator
+from jerryrigserialgen import Serialgenerator, serialgenconfig
+
+# transfer.sh seems to be offline (https://github.com/dutchcoders/transfer.sh/issues/556), that's why i added this:
+serialgenconfig.transfershdomain = 'https://temp.sh'
 
 # Generates serial numbers
 # pip install jerryrigserialgen
 seri = Serialgenerator(
     product="myproduct",  # Name of the product
     savefolder="c:\\mynicefolder\\new",  # just for the record - files are not needed
     hardcodedpasswort_transfer="topsecret",  # for transfer.sh - must be hard-coded in the app the client uses
@@ -30,14 +33,15 @@
     ),  # extra information you want to transmit to the app the client uses
     licensedays=17,  # duration of the license - from today on
     subtract_from_time=0,  # for debugging - to create expired licenses
 )
 serialnumber, debuginfo = seri.upload()
 print(serialnumber) # This is the serial number you are going to give to your client, like: 566978376a4b356956775955427a4779636e533856705a59534d314369387735526e59744230396f6c6771795256675a31365a756947344753616d3757536d5961704f736a362f63506871724a792f3845664d4845773d3d475ac18a6927938b4ede1613058f253e
 
+
 # output
 # File written to: c:\mynicefolder\new\2023_03_23_09_23_18_28484401.cfg
 # 566978376a4b356956775955427a4779636e533856705a59534d314369387735526e59744230396f6c6771795256675a31365a756947344753616d3757536d5961704f736a362f63506871724a792f3845664d4845773d3d475ac18a6927938b4ede1613058f253e
 
 ##########################################################################
 
 # Check serial numbers - client's PC
```

### Comparing `jerryrigserialgen-0.10/jerryrigserialgen/LICENSE` & `jerryrigserialgen-0.11/jerryrigserialgen/LICENSE`

 * *Files identical despite different names*

### Comparing `jerryrigserialgen-0.10/jerryrigserialgen/README.MD` & `jerryrigserialgen-0.11/jerryrigserialgen/README.MD`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 
 ### pip install jerryrigserialgen - if you want to generate serial numbers
 
 ### pip install jerryrigserialver - if you want to verify serial numbers (client)
 
 
 ```python
-from jerryrigserialgen import Serialgenerator
+from jerryrigserialgen import Serialgenerator, serialgenconfig
+
+# transfer.sh seems to be offline (https://github.com/dutchcoders/transfer.sh/issues/556), that's why i added this:
+serialgenconfig.transfershdomain = 'https://temp.sh'
 
 # Generates serial numbers
 # pip install jerryrigserialgen
 seri = Serialgenerator(
     product="myproduct",  # Name of the product
     savefolder="c:\\mynicefolder\\new",  # just for the record - files are not needed
     hardcodedpasswort_transfer="topsecret",  # for transfer.sh - must be hard-coded in the app the client uses
@@ -30,14 +33,15 @@
     ),  # extra information you want to transmit to the app the client uses
     licensedays=17,  # duration of the license - from today on
     subtract_from_time=0,  # for debugging - to create expired licenses
 )
 serialnumber, debuginfo = seri.upload()
 print(serialnumber) # This is the serial number you are going to give to your client, like: 566978376a4b356956775955427a4779636e533856705a59534d314369387735526e59744230396f6c6771795256675a31365a756947344753616d3757536d5961704f736a362f63506871724a792f3845664d4845773d3d475ac18a6927938b4ede1613058f253e
 
+
 # output
 # File written to: c:\mynicefolder\new\2023_03_23_09_23_18_28484401.cfg
 # 566978376a4b356956775955427a4779636e533856705a59534d314369387735526e59744230396f6c6771795256675a31365a756947344753616d3757536d5961704f736a362f63506871724a792f3845664d4845773d3d475ac18a6927938b4ede1613058f253e
 
 ##########################################################################
 
 # Check serial numbers - client's PC
```

### Comparing `jerryrigserialgen-0.10/jerryrigserialgen/__init__.py` & `jerryrigserialgen-0.11/jerryrigserialgen/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from Cryptodome.Util.Padding import pad, unpad
 
 ver = sys.version_info
 out = sys.stdout.flush
 import base64
 from cryptography.hazmat.primitives import serialization, hashes
 from cryptography.hazmat.primitives.asymmetric import rsa, padding
+serialgenconfig = sys.modules[__name__]
+serialgenconfig.transfershdomain = 'https://temp.sh'
 
 
 def iter_get_random_values_with_max_rep(list_, howmany, maxrep):
     resi = []
     resistr = []
     numbers = list_
     alldi = {f"{repr(x)}{x}": x for x in numbers}
@@ -181,15 +183,15 @@
     else:
         headers = {"Max-Downloads": str(maxdownloads)}
 
     fileonly = filepath.split(os.sep)[-1]
     with open(filepath, "rb") as f:
         data = f.read()
     response = requests.put(
-        f"https://transfer.sh/{fileonly}", headers=headers, data=data
+        f"{serialgenconfig.transfershdomain.rstrip('/')}/{fileonly}", headers=headers, data=data
     )
     newlink = response.content.decode("utf-8", "ignore")
     return newlink
 
 
 def write_message_to_hd(message):
     bintmpfile = get_tmpfile(suffix=".bin")
@@ -336,9 +338,10 @@
             "days_left": self.registered_daysleft,
             "serial_number ": text + signature_hex,
             "signature_hex": signature_hex,
             "content_of_second_file": self.serialnumberk,
             "uploaded_file_on_local_HDD ": self.forclient,
             "decrypted_serial_number ": cryptor.decrypt(hex_to_str(text)),
         }
+        print(returninfos)
         return text + signature_hex, returninfos
```

### Comparing `jerryrigserialgen-0.10/jerryrigserialgen.egg-info/PKG-INFO` & `jerryrigserialgen-0.11/jerryrigserialgen.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,86 @@
 Metadata-Version: 2.1
 Name: jerryrigserialgen
-Version: 0.10
+Version: 0.11
 Summary: jerry-rigged license system with UUID check (preventing more than one installation) and expiration date
 Home-page: https://github.com/hansalemaos/jerryrigserialgen
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: UUID,license system,expiration date,serial number
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Editors :: Text Processing
-Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
 
-# jerry-rigged license system with UUID check (preventing more than one installation) and expiration date
-
-### Tested against Python 3.9.16 (Anaconda) -  Windows 10
-
-#### jerry-rigged???
-
-From https://www.urbandictionary.com/define.php?term=jerry-rig
-jerry-rig - To put together in a way that works, but is contrary to the "norm" or specific directions (instructions)
-
-The serial number system can be cracked easily (which one can't?), but it should be secure enough for any average user.
-
-### pip install jerryrigserialgen - if you want to generate serial numbers
-
-### pip install jerryrigserialver - if you want to verify serial numbers (client)
-
-
-```python
-from jerryrigserialgen import Serialgenerator
-
-# Generates serial numbers
-# pip install jerryrigserialgen
-seri = Serialgenerator(
-    product="myproduct",  # Name of the product
-    savefolder="c:\\mynicefolder\\new",  # just for the record - files are not needed
-    hardcodedpasswort_transfer="topsecret",  # for transfer.sh - must be hard-coded in the app the client uses
-    hardcodedpasswort_url="5248614597016233",  # 16 digits to encrypt the URL - must be hard-coded in the app the client uses
-    addinformationtoserial=(
-        "info1",
-        "info2",
-    ),  # extra information you want to transmit to the app the client uses
-    licensedays=17,  # duration of the license - from today on
-    subtract_from_time=0,  # for debugging - to create expired licenses
-)
-serialnumber, debuginfo = seri.upload()
-print(serialnumber) # This is the serial number you are going to give to your client, like: 566978376a4b356956775955427a4779636e533856705a59534d314369387735526e59744230396f6c6771795256675a31365a756947344753616d3757536d5961704f736a362f63506871724a792f3845664d4845773d3d475ac18a6927938b4ede1613058f253e
-
-# output
-# File written to: c:\mynicefolder\new\2023_03_23_09_23_18_28484401.cfg
-# 566978376a4b356956775955427a4779636e533856705a59534d314369387735526e59744230396f6c6771795256675a31365a756947344753616d3757536d5961704f736a362f63506871724a792f3845664d4845773d3d475ac18a6927938b4ede1613058f253e
-
-##########################################################################
-
-# Check serial numbers - client's PC
-
-# pip install jerryrigserialver
-from jerryrigserialver import check_serial
-
-isvalid, daysleft, duration_of_license, product, otherinfos = check_serial(
-    hardcodedpasswort_transfer="topsecret",
-    # hardcodedpasswort_transfer for transfer.sh - must be hard-coded
-    hardcodedpasswort_url="5248614597016233",  # 16 digits to encrypt the url - must be hard-coded
-    serialnumber=serialnumber,
-    notvalidanymore=f"The license you're using is not valid anymore. It expired %d day[s] ago",
-    stillvalid=f"The license you're using is valid for %d more day[s].",
-    serialusedanotherpc="The license has been used on another PC",
-)
-print(isvalid, daysleft, duration_of_license, product, otherinfos)
-
-
-# The license you're using is valid for 17 more day[s].
-# True 17 17 myproduct ['info1', 'info2']
-
-# Compile the code of your app using PyInstaller or some other tool
+# jerry-rigged license system with UUID check (preventing more than one installation) and expiration date
+
+### Tested against Python 3.9.16 (Anaconda) -  Windows 10
+
+#### jerry-rigged???
+
+From https://www.urbandictionary.com/define.php?term=jerry-rig
+jerry-rig - To put together in a way that works, but is contrary to the "norm" or specific directions (instructions)
+
+The serial number system can be cracked easily (which one can't?), but it should be secure enough for any average user.
+
+### pip install jerryrigserialgen - if you want to generate serial numbers
+
+### pip install jerryrigserialver - if you want to verify serial numbers (client)
+
+
+```python
+from jerryrigserialgen import Serialgenerator, serialgenconfig
+
+# transfer.sh seems to be offline (https://github.com/dutchcoders/transfer.sh/issues/556), that's why i added this:
+serialgenconfig.transfershdomain = 'https://temp.sh'
+
+# Generates serial numbers
+# pip install jerryrigserialgen
+seri = Serialgenerator(
+    product="myproduct",  # Name of the product
+    savefolder="c:\\mynicefolder\\new",  # just for the record - files are not needed
+    hardcodedpasswort_transfer="topsecret",  # for transfer.sh - must be hard-coded in the app the client uses
+    hardcodedpasswort_url="5248614597016233",  # 16 digits to encrypt the URL - must be hard-coded in the app the client uses
+    addinformationtoserial=(
+        "info1",
+        "info2",
+    ),  # extra information you want to transmit to the app the client uses
+    licensedays=17,  # duration of the license - from today on
+    subtract_from_time=0,  # for debugging - to create expired licenses
+)
+serialnumber, debuginfo = seri.upload()
+print(serialnumber) # This is the serial number you are going to give to your client, like: 566978376a4b356956775955427a4779636e533856705a59534d314369387735526e59744230396f6c6771795256675a31365a756947344753616d3757536d5961704f736a362f63506871724a792f3845664d4845773d3d475ac18a6927938b4ede1613058f253e
+
+
+# output
+# File written to: c:\mynicefolder\new\2023_03_23_09_23_18_28484401.cfg
+# 566978376a4b356956775955427a4779636e533856705a59534d314369387735526e59744230396f6c6771795256675a31365a756947344753616d3757536d5961704f736a362f63506871724a792f3845664d4845773d3d475ac18a6927938b4ede1613058f253e
+
+##########################################################################
+
+# Check serial numbers - client's PC
+
+# pip install jerryrigserialver
+from jerryrigserialver import check_serial
+
+isvalid, daysleft, duration_of_license, product, otherinfos = check_serial(
+    hardcodedpasswort_transfer="topsecret",
+    # hardcodedpasswort_transfer for transfer.sh - must be hard-coded
+    hardcodedpasswort_url="5248614597016233",  # 16 digits to encrypt the url - must be hard-coded
+    serialnumber=serialnumber,
+    notvalidanymore=f"The license you're using is not valid anymore. It expired %d day[s] ago",
+    stillvalid=f"The license you're using is valid for %d more day[s].",
+    serialusedanotherpc="The license has been used on another PC",
+)
+print(isvalid, daysleft, duration_of_license, product, otherinfos)
+
+
+# The license you're using is valid for 17 more day[s].
+# True 17 17 myproduct ['info1', 'info2']
+
+# Compile the code of your app using PyInstaller or some other tool
 ```
```

### Comparing `jerryrigserialgen-0.10/setup.py` & `jerryrigserialgen-0.11/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from setuptools import setup, find_packages
 import codecs
 import os
-
-#change to dict
+# 
 here = os.path.abspath(os.path.dirname(__file__))
+# 
+with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
+    long_description = "\n" + fh.read()\
 
-with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
-    long_description = "\n" + fh.read()
+from pathlib import Path
+this_directory = Path(__file__).parent
+#long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.10'
-DESCRIPTION = "jerry-rigged license system with UUID check (preventing more than one installation) and expiration date"
+VERSION = '''0.11'''
+DESCRIPTION = '''jerry-rigged license system with UUID check (preventing more than one installation) and expiration date'''
 
 # Setting up
 setup(
     name="jerryrigserialgen",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/jerryrigserialgen',
     author="Johannes Fischer",
-    author_email="<aulasparticularesdealemaosp@gmail.com>",
+    author_email="aulasparticularesdealemaosp@gmail.com",
     description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=long_description,
+long_description = long_description,
+long_description_content_type="text/markdown",
     #packages=['cryptography', 'dill', 'isiter', 'pycryptodomex', 'requests', 'touchtouch', 'xxhash'],
     keywords=['UUID', 'license system', 'expiration date', 'serial number'],
-    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.9', 'Topic :: Scientific/Engineering :: Visualization', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Text Editors :: Text Processing', 'Topic :: Text Processing :: General', 'Topic :: Text Processing :: Indexing', 'Topic :: Text Processing :: Filters', 'Topic :: Utilities'],
+    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
     install_requires=['cryptography', 'dill', 'isiter', 'pycryptodomex', 'requests', 'touchtouch', 'xxhash'],
     include_package_data=True
 )
 #python setup.py sdist bdist_wheel
 #twine upload dist/*
```

