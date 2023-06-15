# Comparing `tmp/myl-discovery-0.5.4.tar.gz` & `tmp/myl-discovery-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myl-discovery-0.5.4.tar", last modified: Thu Jun 15 07:10:27 2023, max compression
+gzip compressed data, was "myl-discovery-0.5.5.tar", last modified: Thu Jun 15 07:19:24 2023, max compression
```

## Comparing `myl-discovery-0.5.4.tar` & `myl-discovery-0.5.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:10:27.458107 myl-discovery-0.5.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:10:27.458107 myl-discovery-0.5.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:10:27.458107 myl-discovery-0.5.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/HACKING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43621 2023-06-15 07:10:27.458107 myl-discovery-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:10:27.458107 myl-discovery-0.5.4/myl_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43621 2023-06-15 07:10:27.000000 myl-discovery-0.5.4/myl_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-15 07:10:27.000000 myl-discovery-0.5.4/myl_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:10:27.000000 myl-discovery-0.5.4/myl_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 07:10:27.000000 myl-discovery-0.5.4/myl_discovery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-15 07:10:27.000000 myl-discovery-0.5.4/myl_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 07:10:27.000000 myl-discovery-0.5.4/myl_discovery.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:10:27.458107 myl-discovery-0.5.4/myldiscovery/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/myldiscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/myldiscovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/myldiscovery/discovery.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2016 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/myldiscovery/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 07:10:27.458107 myl-discovery-0.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:19:24.599272 myl-discovery-0.5.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:19:24.595272 myl-discovery-0.5.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-15 07:19:11.000000 myl-discovery-0.5.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:19:24.595272 myl-discovery-0.5.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-15 07:19:11.000000 myl-discovery-0.5.5/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-15 07:19:11.000000 myl-discovery-0.5.5/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-15 07:19:11.000000 myl-discovery-0.5.5/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 07:19:11.000000 myl-discovery-0.5.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-15 07:19:11.000000 myl-discovery-0.5.5/HACKING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 07:19:11.000000 myl-discovery-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44501 2023-06-15 07:19:24.599272 myl-discovery-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-15 07:19:11.000000 myl-discovery-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:19:24.599272 myl-discovery-0.5.5/myl_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44501 2023-06-15 07:19:24.000000 myl-discovery-0.5.5/myl_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-15 07:19:24.000000 myl-discovery-0.5.5/myl_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:19:24.000000 myl-discovery-0.5.5/myl_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 07:19:24.000000 myl-discovery-0.5.5/myl_discovery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-15 07:19:24.000000 myl-discovery-0.5.5/myl_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 07:19:24.000000 myl-discovery-0.5.5/myl_discovery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:19:24.599272 myl-discovery-0.5.5/myldiscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-15 07:19:11.000000 myl-discovery-0.5.5/myldiscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 07:19:11.000000 myl-discovery-0.5.5/myldiscovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-06-15 07:19:11.000000 myl-discovery-0.5.5/myldiscovery/discovery.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2016 2023-06-15 07:19:11.000000 myl-discovery-0.5.5/myldiscovery/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-15 07:19:11.000000 myl-discovery-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 07:19:24.599272 myl-discovery-0.5.5/setup.cfg
```

### Comparing `myl-discovery-0.5.4/.github/workflows/pypi.yaml` & `myl-discovery-0.5.5/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.5.4/.github/workflows/release.yaml` & `myl-discovery-0.5.5/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.5.4/HACKING.md` & `myl-discovery-0.5.5/HACKING.md`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.5.4/LICENSE` & `myl-discovery-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.5.4/PKG-INFO` & `myl-discovery-0.5.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl-discovery
-Version: 0.5.4
+Version: 0.5.5
 Summary: email autodiscovery
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,49 +682,49 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 📩 myl-discovery
 
-myl-discovery is a Python library designed to detect email settings of a given 
+myl-discovery is a Python library designed to detect email settings of a given
 email address or domain.
 
 ## 📥 Installation
 
 To install myl-discovery, run the following command:
 
 ```bash
 pip install myl-discovery
 ```
 
 ## 📖 Usage
 
-After installing the package, you can use the `autodiscover` function to 
+After installing the package, you can use the `autodiscover` function to
 discover the email settings for a domain. Here's an example:
 
 ```python
 from myldiscovery import autodiscover
 
 settings = autodiscover("yourdomain.com")  # or me@yourdomain.com
 print(settings)
 
 # For Exchange autodiscovery you need to provide credentials
 settings = autodiscover(
-    'me@yourdomain.com', 
-    username='WORKGROUP\me', 
+    'me@yourdomain.com',
+    username='WORKGROUP\me',
     password='mypassword1234'
 )
 ```
 
 ## 📄 Output
 
-The `autodiscover` function returns a dictionary with the detected settings. 
-The dictionary contains two keys, `imap` and `smtp`, each containing a 
-dictionary with the keys `server`, `port`, and `starttls`. 
+The `autodiscover` function returns a dictionary with the detected settings.
+The dictionary contains two keys, `imap` and `smtp`, each containing a
+dictionary with the keys `server`, `port`, and `starttls`.
 
 Here's an example:
 
 ```json
 {
   "imap": {
     "server": "imap.yourdomain.com",
@@ -741,35 +741,75 @@
 
 ## 🧩 Autodiscover Functions
 
 myl-discovery exposes several functions to discover email settings:
 
 - `autodiscover`: This function wraps the below function do automatically detect
 the right settings. (See Autodiscover strategy for more information)
-- `autodiscover_srv`: This function attempts to resolve SRV records for 
+- `autodiscover_srv`: This function attempts to resolve SRV records for
 the domain to discover IMAP and SMTP servers.
-- `autodiscover_exchange`: This function attempts to use the Exchange 
-Autodiscover service to discover email settings. It requires a username and 
+- `autodiscover_exchange`: This function attempts to use the Exchange
+Autodiscover service to discover email settings. It requires a username and
 password.
-- `autodiscover_autoconfig`: This function attempts to fetch and parse an 
+- `autodiscover_autoconfig`: This function attempts to fetch and parse an
 autoconfig XML file from a URL specified in the domain's TXT records.
-- `autodiscover_port_scan`: This function performs a port scan on the domain 
+- `autodiscover_port_scan`: This function performs a port scan on the domain
 to discover open IMAP and SMTP ports.
 
 ## 🧠 Autodiscover Strategy
 
-The `autodiscover` function uses the following strategy to discover 
+The `autodiscover` function uses the following strategy to discover
 email settings:
 
-1. It first attempts to use `autodiscover_autoconfig` to discover settings 
+1. It first attempts to use `autodiscover_autoconfig` to discover settings
 from an autoconfig/autodiscover URL specified in the domain's TXT records.
-2. If that fails, it attempts to use `autodiscover_srv` to discover settings 
+2. If that fails, it attempts to use `autodiscover_srv` to discover settings
 from the domain's SRV records.
-3. If that fails and a password is provided, it attempts to use 
-`autodiscover_exchange` to discover settings using the 
+3. If that fails and a password is provided, it attempts to use
+`autodiscover_exchange` to discover settings using the
 Exchange Autodiscover service (only if credentials were provided)
-4. If all else fails, it uses `autodiscover_port_scan` to discover settings by 
+4. If all else fails, it uses `autodiscover_port_scan` to discover settings by
 performing a port scan on the domain.
 
+## 💻 CLI usage
+
+If you do not intend to use the Python library and just want to detect the
+connection settings of an arbitrary email, myl-discovery also ships with a
+CLI tool.
+
+### 📥 Installation
+
+```shell
+pipx install myl-discovery
+```
+
+### 📖 Usage
+
+```
+$ myl-discovery --help
+usage: myl-discovery [-h] [-j] [-d] [-u USERNAME] [-p PASSWORD] EMAIL
+
+positional arguments:
+  EMAIL
+
+options:
+  -h, --help            show this help message and exit
+  -j, --json
+  -d, --debug
+  -u USERNAME, --username USERNAME
+                        Username (Exchange only)
+  -p PASSWORD, --password PASSWORD
+                        Password (Exchange only)
+```
+
+Example:
+
+```
+$ myl-discovery user01@gmail.com
+ Service          Host                           Port       TLS
+ imap             imap.gmail.com                 993        tls
+ smtp             smtp.gmail.com                 587        tls
+```
+
 ## 📜 License
 
 myl-discovery is licensed under the [GNU General Public License v3.0](LICENSE).
```

### Comparing `myl-discovery-0.5.4/README.md` & `myl-discovery-0.5.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # 📩 myl-discovery
 
-myl-discovery is a Python library designed to detect email settings of a given 
+myl-discovery is a Python library designed to detect email settings of a given
 email address or domain.
 
 ## 📥 Installation
 
 To install myl-discovery, run the following command:
 
 ```bash
 pip install myl-discovery
 ```
 
 ## 📖 Usage
 
-After installing the package, you can use the `autodiscover` function to 
+After installing the package, you can use the `autodiscover` function to
 discover the email settings for a domain. Here's an example:
 
 ```python
 from myldiscovery import autodiscover
 
 settings = autodiscover("yourdomain.com")  # or me@yourdomain.com
 print(settings)
 
 # For Exchange autodiscovery you need to provide credentials
 settings = autodiscover(
-    'me@yourdomain.com', 
-    username='WORKGROUP\me', 
+    'me@yourdomain.com',
+    username='WORKGROUP\me',
     password='mypassword1234'
 )
 ```
 
 ## 📄 Output
 
-The `autodiscover` function returns a dictionary with the detected settings. 
-The dictionary contains two keys, `imap` and `smtp`, each containing a 
-dictionary with the keys `server`, `port`, and `starttls`. 
+The `autodiscover` function returns a dictionary with the detected settings.
+The dictionary contains two keys, `imap` and `smtp`, each containing a
+dictionary with the keys `server`, `port`, and `starttls`.
 
 Here's an example:
 
 ```json
 {
   "imap": {
     "server": "imap.yourdomain.com",
@@ -55,35 +55,75 @@
 
 ## 🧩 Autodiscover Functions
 
 myl-discovery exposes several functions to discover email settings:
 
 - `autodiscover`: This function wraps the below function do automatically detect
 the right settings. (See Autodiscover strategy for more information)
-- `autodiscover_srv`: This function attempts to resolve SRV records for 
+- `autodiscover_srv`: This function attempts to resolve SRV records for
 the domain to discover IMAP and SMTP servers.
-- `autodiscover_exchange`: This function attempts to use the Exchange 
-Autodiscover service to discover email settings. It requires a username and 
+- `autodiscover_exchange`: This function attempts to use the Exchange
+Autodiscover service to discover email settings. It requires a username and
 password.
-- `autodiscover_autoconfig`: This function attempts to fetch and parse an 
+- `autodiscover_autoconfig`: This function attempts to fetch and parse an
 autoconfig XML file from a URL specified in the domain's TXT records.
-- `autodiscover_port_scan`: This function performs a port scan on the domain 
+- `autodiscover_port_scan`: This function performs a port scan on the domain
 to discover open IMAP and SMTP ports.
 
 ## 🧠 Autodiscover Strategy
 
-The `autodiscover` function uses the following strategy to discover 
+The `autodiscover` function uses the following strategy to discover
 email settings:
 
-1. It first attempts to use `autodiscover_autoconfig` to discover settings 
+1. It first attempts to use `autodiscover_autoconfig` to discover settings
 from an autoconfig/autodiscover URL specified in the domain's TXT records.
-2. If that fails, it attempts to use `autodiscover_srv` to discover settings 
+2. If that fails, it attempts to use `autodiscover_srv` to discover settings
 from the domain's SRV records.
-3. If that fails and a password is provided, it attempts to use 
-`autodiscover_exchange` to discover settings using the 
+3. If that fails and a password is provided, it attempts to use
+`autodiscover_exchange` to discover settings using the
 Exchange Autodiscover service (only if credentials were provided)
-4. If all else fails, it uses `autodiscover_port_scan` to discover settings by 
+4. If all else fails, it uses `autodiscover_port_scan` to discover settings by
 performing a port scan on the domain.
 
+## 💻 CLI usage
+
+If you do not intend to use the Python library and just want to detect the
+connection settings of an arbitrary email, myl-discovery also ships with a
+CLI tool.
+
+### 📥 Installation
+
+```shell
+pipx install myl-discovery
+```
+
+### 📖 Usage
+
+```
+$ myl-discovery --help
+usage: myl-discovery [-h] [-j] [-d] [-u USERNAME] [-p PASSWORD] EMAIL
+
+positional arguments:
+  EMAIL
+
+options:
+  -h, --help            show this help message and exit
+  -j, --json
+  -d, --debug
+  -u USERNAME, --username USERNAME
+                        Username (Exchange only)
+  -p PASSWORD, --password PASSWORD
+                        Password (Exchange only)
+```
+
+Example:
+
+```
+$ myl-discovery user01@gmail.com
+ Service          Host                           Port       TLS
+ imap             imap.gmail.com                 993        tls
+ smtp             smtp.gmail.com                 587        tls
+```
+
 ## 📜 License
 
 myl-discovery is licensed under the [GNU General Public License v3.0](LICENSE).
```

### Comparing `myl-discovery-0.5.4/myl_discovery.egg-info/PKG-INFO` & `myl-discovery-0.5.5/myl_discovery.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl-discovery
-Version: 0.5.4
+Version: 0.5.5
 Summary: email autodiscovery
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,49 +682,49 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 📩 myl-discovery
 
-myl-discovery is a Python library designed to detect email settings of a given 
+myl-discovery is a Python library designed to detect email settings of a given
 email address or domain.
 
 ## 📥 Installation
 
 To install myl-discovery, run the following command:
 
 ```bash
 pip install myl-discovery
 ```
 
 ## 📖 Usage
 
-After installing the package, you can use the `autodiscover` function to 
+After installing the package, you can use the `autodiscover` function to
 discover the email settings for a domain. Here's an example:
 
 ```python
 from myldiscovery import autodiscover
 
 settings = autodiscover("yourdomain.com")  # or me@yourdomain.com
 print(settings)
 
 # For Exchange autodiscovery you need to provide credentials
 settings = autodiscover(
-    'me@yourdomain.com', 
-    username='WORKGROUP\me', 
+    'me@yourdomain.com',
+    username='WORKGROUP\me',
     password='mypassword1234'
 )
 ```
 
 ## 📄 Output
 
-The `autodiscover` function returns a dictionary with the detected settings. 
-The dictionary contains two keys, `imap` and `smtp`, each containing a 
-dictionary with the keys `server`, `port`, and `starttls`. 
+The `autodiscover` function returns a dictionary with the detected settings.
+The dictionary contains two keys, `imap` and `smtp`, each containing a
+dictionary with the keys `server`, `port`, and `starttls`.
 
 Here's an example:
 
 ```json
 {
   "imap": {
     "server": "imap.yourdomain.com",
@@ -741,35 +741,75 @@
 
 ## 🧩 Autodiscover Functions
 
 myl-discovery exposes several functions to discover email settings:
 
 - `autodiscover`: This function wraps the below function do automatically detect
 the right settings. (See Autodiscover strategy for more information)
-- `autodiscover_srv`: This function attempts to resolve SRV records for 
+- `autodiscover_srv`: This function attempts to resolve SRV records for
 the domain to discover IMAP and SMTP servers.
-- `autodiscover_exchange`: This function attempts to use the Exchange 
-Autodiscover service to discover email settings. It requires a username and 
+- `autodiscover_exchange`: This function attempts to use the Exchange
+Autodiscover service to discover email settings. It requires a username and
 password.
-- `autodiscover_autoconfig`: This function attempts to fetch and parse an 
+- `autodiscover_autoconfig`: This function attempts to fetch and parse an
 autoconfig XML file from a URL specified in the domain's TXT records.
-- `autodiscover_port_scan`: This function performs a port scan on the domain 
+- `autodiscover_port_scan`: This function performs a port scan on the domain
 to discover open IMAP and SMTP ports.
 
 ## 🧠 Autodiscover Strategy
 
-The `autodiscover` function uses the following strategy to discover 
+The `autodiscover` function uses the following strategy to discover
 email settings:
 
-1. It first attempts to use `autodiscover_autoconfig` to discover settings 
+1. It first attempts to use `autodiscover_autoconfig` to discover settings
 from an autoconfig/autodiscover URL specified in the domain's TXT records.
-2. If that fails, it attempts to use `autodiscover_srv` to discover settings 
+2. If that fails, it attempts to use `autodiscover_srv` to discover settings
 from the domain's SRV records.
-3. If that fails and a password is provided, it attempts to use 
-`autodiscover_exchange` to discover settings using the 
+3. If that fails and a password is provided, it attempts to use
+`autodiscover_exchange` to discover settings using the
 Exchange Autodiscover service (only if credentials were provided)
-4. If all else fails, it uses `autodiscover_port_scan` to discover settings by 
+4. If all else fails, it uses `autodiscover_port_scan` to discover settings by
 performing a port scan on the domain.
 
+## 💻 CLI usage
+
+If you do not intend to use the Python library and just want to detect the
+connection settings of an arbitrary email, myl-discovery also ships with a
+CLI tool.
+
+### 📥 Installation
+
+```shell
+pipx install myl-discovery
+```
+
+### 📖 Usage
+
+```
+$ myl-discovery --help
+usage: myl-discovery [-h] [-j] [-d] [-u USERNAME] [-p PASSWORD] EMAIL
+
+positional arguments:
+  EMAIL
+
+options:
+  -h, --help            show this help message and exit
+  -j, --json
+  -d, --debug
+  -u USERNAME, --username USERNAME
+                        Username (Exchange only)
+  -p PASSWORD, --password PASSWORD
+                        Password (Exchange only)
+```
+
+Example:
+
+```
+$ myl-discovery user01@gmail.com
+ Service          Host                           Port       TLS
+ imap             imap.gmail.com                 993        tls
+ smtp             smtp.gmail.com                 587        tls
+```
+
 ## 📜 License
 
 myl-discovery is licensed under the [GNU General Public License v3.0](LICENSE).
```

### Comparing `myl-discovery-0.5.4/myldiscovery/discovery.py` & `myl-discovery-0.5.5/myldiscovery/discovery.py`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.5.4/myldiscovery/main.py` & `myl-discovery-0.5.5/myldiscovery/main.py`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.5.4/pyproject.toml` & `myl-discovery-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 dependencies = [
   "dnspython == 2.3.0",
   "exchangelib == 5.0.3",
   "requests == 2.31.0",
   "rich == 13.4.2",
   "xmltodict == 0.13.0"
 ]
-version = "0.5.4"
+version = "0.5.5"
 
 [project.scripts]
 myl-discovery = "myldiscovery:main"
 
 [tool.black]
 line-length = 79
```

