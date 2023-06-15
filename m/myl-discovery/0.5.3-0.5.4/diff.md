# Comparing `tmp/myl-discovery-0.5.3.tar.gz` & `tmp/myl-discovery-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myl-discovery-0.5.3.tar", last modified: Thu Jun 15 06:31:44 2023, max compression
+gzip compressed data, was "myl-discovery-0.5.4.tar", last modified: Thu Jun 15 07:10:27 2023, max compression
```

## Comparing `myl-discovery-0.5.3.tar` & `myl-discovery-0.5.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:31:44.733097 myl-discovery-0.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:31:44.729097 myl-discovery-0.5.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:31:44.729097 myl-discovery-0.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44811 2023-06-15 06:31:44.733097 myl-discovery-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:31:44.733097 myl-discovery-0.5.3/myl_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44811 2023-06-15 06:31:44.000000 myl-discovery-0.5.3/myl_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-15 06:31:44.000000 myl-discovery-0.5.3/myl_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:31:44.000000 myl-discovery-0.5.3/myl_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 06:31:44.000000 myl-discovery-0.5.3/myl_discovery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-15 06:31:44.000000 myl-discovery-0.5.3/myl_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 06:31:44.000000 myl-discovery-0.5.3/myl_discovery.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:31:44.733097 myl-discovery-0.5.3/myldiscovery/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/myldiscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/myldiscovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/myldiscovery/discovery.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2016 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/myldiscovery/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 06:31:44.733097 myl-discovery-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:10:27.458107 myl-discovery-0.5.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:10:27.458107 myl-discovery-0.5.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:10:27.458107 myl-discovery-0.5.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/HACKING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43621 2023-06-15 07:10:27.458107 myl-discovery-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:10:27.458107 myl-discovery-0.5.4/myl_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43621 2023-06-15 07:10:27.000000 myl-discovery-0.5.4/myl_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-15 07:10:27.000000 myl-discovery-0.5.4/myl_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:10:27.000000 myl-discovery-0.5.4/myl_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 07:10:27.000000 myl-discovery-0.5.4/myl_discovery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-15 07:10:27.000000 myl-discovery-0.5.4/myl_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 07:10:27.000000 myl-discovery-0.5.4/myl_discovery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:10:27.458107 myl-discovery-0.5.4/myldiscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/myldiscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/myldiscovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/myldiscovery/discovery.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2016 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/myldiscovery/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-15 07:10:14.000000 myl-discovery-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 07:10:27.458107 myl-discovery-0.5.4/setup.cfg
```

### Comparing `myl-discovery-0.5.3/.github/workflows/pypi.yaml` & `myl-discovery-0.5.4/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.5.3/.github/workflows/release.yaml` & `myl-discovery-0.5.4/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.5.3/LICENSE` & `myl-discovery-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.5.3/PKG-INFO` & `myl-discovery-0.5.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl-discovery
-Version: 0.5.3
+Version: 0.5.4
 Summary: email autodiscovery
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,134 +680,96 @@
         
 Keywords: email-discovery,autodiscover,autoconfig,smtp,imap,email,discovery
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# myl-discovery
+# 📩 myl-discovery
 
-Email autoconfig library
+myl-discovery is a Python library designed to detect email settings of a given 
+email address or domain.
 
-## Installation
+## 📥 Installation
 
-```shell
+To install myl-discovery, run the following command:
+
+```bash
 pip install myl-discovery
 ```
 
-## Usage
+## 📖 Usage
+
+After installing the package, you can use the `autodiscover` function to 
+discover the email settings for a domain. Here's an example:
 
 ```python
 from myldiscovery import autodiscover
-autodiscover("me@example.com")
-# {'imap': {'server': 'mail.example.com', 'port': 993, 'starttls': False},
-#  'smtp': {'server': 'mail.example.com', 'port': 587, 'starttls': False}}
-```
-
 
-## Development
+settings = autodiscover("yourdomain.com")  # or me@yourdomain.com
+print(settings)
 
-### Autodiscovery
-
-#### autoconfig
-
-```shell
-curl -L https://mail.example.com/mail/config-v1.1.xml
+# For Exchange autodiscovery you need to provide credentials
+settings = autodiscover(
+    'me@yourdomain.com', 
+    username='WORKGROUP\me', 
+    password='mypassword1234'
+)
 ```
 
-Response:
+## 📄 Output
 
-```xml
-<?xml version="1.0" encoding="UTF-8"?>
-<clientConfig version="1.1">
-	<emailProvider id="example.com">
-	    <domain>example.com</domain>
-
-	    <displayName>example.com Email</displayName>
-	    <displayShortName>%EMAILLOCALPART%</displayShortName>
-	    <incomingServer type="imap">
-			<hostname>mail.example.com</hostname>
-			<port>143</port>
-			<socketType>STARTTLS</socketType>
-			<authentication>password-cleartext</authentication>
-			<username>%EMAILADDRESS%</username>
-		</incomingServer>
-	    <outgoingServer type="smtp">
-			<hostname>mail.example.com</hostname>
-			<port>587</port>
-			<socketType>STARTTLS</socketType>
-			<authentication>password-cleartext</authentication>
-			<username>%EMAILADDRESS%</username>
-	    </outgoingServer>
-		<documentation url="https://autodiscover.example.com">
-			<descr lang="en">Generic settings page</descr>
-			<descr lang="fr">Paramètres généraux</descr>
-			<descr lang="es">Configuraciones genéricas</descr>
-			<descr lang="de">Allgemeine Beschreibung der Einstellungen</descr>
-			<descr lang="ru">Страница общих настроек</descr>
-		</documentation>
-	</emailProvider>
-</clientConfig>
+The `autodiscover` function returns a dictionary with the detected settings. 
+The dictionary contains two keys, `imap` and `smtp`, each containing a 
+dictionary with the keys `server`, `port`, and `starttls`. 
+
+Here's an example:
+
+```json
+{
+  "imap": {
+    "server": "imap.yourdomain.com",
+    "port": 993,
+    "starttls": false
+  },
+  "smtp": {
+    "server": "smtp.yourdomain.com",
+    "port": 587,
+    "starttls": true
+  }
+}
 ```
 
-### autodiscover
+## 🧩 Autodiscover Functions
 
-```shell
-curl -L mail.example.com/autodiscover/autodiscover.xml
-```
+myl-discovery exposes several functions to discover email settings:
 
-Response:
+- `autodiscover`: This function wraps the below function do automatically detect
+the right settings. (See Autodiscover strategy for more information)
+- `autodiscover_srv`: This function attempts to resolve SRV records for 
+the domain to discover IMAP and SMTP servers.
+- `autodiscover_exchange`: This function attempts to use the Exchange 
+Autodiscover service to discover email settings. It requires a username and 
+password.
+- `autodiscover_autoconfig`: This function attempts to fetch and parse an 
+autoconfig XML file from a URL specified in the domain's TXT records.
+- `autodiscover_port_scan`: This function performs a port scan on the domain 
+to discover open IMAP and SMTP ports.
+
+## 🧠 Autodiscover Strategy
+
+The `autodiscover` function uses the following strategy to discover 
+email settings:
+
+1. It first attempts to use `autodiscover_autoconfig` to discover settings 
+from an autoconfig/autodiscover URL specified in the domain's TXT records.
+2. If that fails, it attempts to use `autodiscover_srv` to discover settings 
+from the domain's SRV records.
+3. If that fails and a password is provided, it attempts to use 
+`autodiscover_exchange` to discover settings using the 
+Exchange Autodiscover service (only if credentials were provided)
+4. If all else fails, it uses `autodiscover_port_scan` to discover settings by 
+performing a port scan on the domain.
 
-```xml
-<?xml version="1.0" encoding="utf-8" ?>
-<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
-        <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
-                <User>
-                        <DisplayName>example.com Email</DisplayName>
-                </User>
-                <Account>
-                        <AccountType>email</AccountType>
-                        <Action>settings</Action>
-                        <ServiceHome>https://autodiscover.example.com</ServiceHome>
-
-                        <Protocol>
-                                <Type>IMAP</Type>
-                                <TTL>1</TTL>
-
-                                <Server>mail.example.com</Server>
-                                <Port>143</Port>
-
-                                <LoginName></LoginName>
-
-                                <DomainRequired>on</DomainRequired>
-                                <DomainName>example.com</DomainName>
-
-                                <SPA>off</SPA>
-                                <Encryption>TLS</Encryption>
-                                <AuthRequired>on</AuthRequired>
-                        </Protocol>
-                </Account>
-                <Account>
-                        <AccountType>email</AccountType>
-                        <Action>settings</Action>
-                        <ServiceHome>https://autodiscover.example.com</ServiceHome>
-
-                        <Protocol>
-                                <Type>SMTP</Type>
-                                <TTL>1</TTL>
-
-                                <Server>mail.example.com</Server>
-                                <Port>587</Port>
-
-                                <LoginName></LoginName>
-
-                                <DomainRequired>on</DomainRequired>
-                                <DomainName>example.com</DomainName>
-
-                                <SPA>off</SPA>
-                                <Encryption>TLS</Encryption>
-                                <AuthRequired>on</AuthRequired>
-                        </Protocol>
-                </Account></Response>
-</Autodiscover>
-```
+## 📜 License
 
+myl-discovery is licensed under the [GNU General Public License v3.0](LICENSE).
```

### Comparing `myl-discovery-0.5.3/README.md` & `myl-discovery-0.5.4/HACKING.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-# myl-discovery
-
-Email autoconfig library
-
-## Installation
-
-```shell
-pip install myl-discovery
-```
-
-## Usage
-
-```python
-from myldiscovery import autodiscover
-autodiscover("me@example.com")
-# {'imap': {'server': 'mail.example.com', 'port': 993, 'starttls': False},
-#  'smtp': {'server': 'mail.example.com', 'port': 587, 'starttls': False}}
-```
-
-
 ## Development
 
 ### Autodiscovery
 
 #### autoconfig
 
 ```shell
```

### Comparing `myl-discovery-0.5.3/myl_discovery.egg-info/PKG-INFO` & `myl-discovery-0.5.4/myl_discovery.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl-discovery
-Version: 0.5.3
+Version: 0.5.4
 Summary: email autodiscovery
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,134 +680,96 @@
         
 Keywords: email-discovery,autodiscover,autoconfig,smtp,imap,email,discovery
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# myl-discovery
+# 📩 myl-discovery
 
-Email autoconfig library
+myl-discovery is a Python library designed to detect email settings of a given 
+email address or domain.
 
-## Installation
+## 📥 Installation
 
-```shell
+To install myl-discovery, run the following command:
+
+```bash
 pip install myl-discovery
 ```
 
-## Usage
+## 📖 Usage
+
+After installing the package, you can use the `autodiscover` function to 
+discover the email settings for a domain. Here's an example:
 
 ```python
 from myldiscovery import autodiscover
-autodiscover("me@example.com")
-# {'imap': {'server': 'mail.example.com', 'port': 993, 'starttls': False},
-#  'smtp': {'server': 'mail.example.com', 'port': 587, 'starttls': False}}
-```
-
 
-## Development
+settings = autodiscover("yourdomain.com")  # or me@yourdomain.com
+print(settings)
 
-### Autodiscovery
-
-#### autoconfig
-
-```shell
-curl -L https://mail.example.com/mail/config-v1.1.xml
+# For Exchange autodiscovery you need to provide credentials
+settings = autodiscover(
+    'me@yourdomain.com', 
+    username='WORKGROUP\me', 
+    password='mypassword1234'
+)
 ```
 
-Response:
+## 📄 Output
 
-```xml
-<?xml version="1.0" encoding="UTF-8"?>
-<clientConfig version="1.1">
-	<emailProvider id="example.com">
-	    <domain>example.com</domain>
-
-	    <displayName>example.com Email</displayName>
-	    <displayShortName>%EMAILLOCALPART%</displayShortName>
-	    <incomingServer type="imap">
-			<hostname>mail.example.com</hostname>
-			<port>143</port>
-			<socketType>STARTTLS</socketType>
-			<authentication>password-cleartext</authentication>
-			<username>%EMAILADDRESS%</username>
-		</incomingServer>
-	    <outgoingServer type="smtp">
-			<hostname>mail.example.com</hostname>
-			<port>587</port>
-			<socketType>STARTTLS</socketType>
-			<authentication>password-cleartext</authentication>
-			<username>%EMAILADDRESS%</username>
-	    </outgoingServer>
-		<documentation url="https://autodiscover.example.com">
-			<descr lang="en">Generic settings page</descr>
-			<descr lang="fr">Paramètres généraux</descr>
-			<descr lang="es">Configuraciones genéricas</descr>
-			<descr lang="de">Allgemeine Beschreibung der Einstellungen</descr>
-			<descr lang="ru">Страница общих настроек</descr>
-		</documentation>
-	</emailProvider>
-</clientConfig>
+The `autodiscover` function returns a dictionary with the detected settings. 
+The dictionary contains two keys, `imap` and `smtp`, each containing a 
+dictionary with the keys `server`, `port`, and `starttls`. 
+
+Here's an example:
+
+```json
+{
+  "imap": {
+    "server": "imap.yourdomain.com",
+    "port": 993,
+    "starttls": false
+  },
+  "smtp": {
+    "server": "smtp.yourdomain.com",
+    "port": 587,
+    "starttls": true
+  }
+}
 ```
 
-### autodiscover
+## 🧩 Autodiscover Functions
 
-```shell
-curl -L mail.example.com/autodiscover/autodiscover.xml
-```
+myl-discovery exposes several functions to discover email settings:
 
-Response:
+- `autodiscover`: This function wraps the below function do automatically detect
+the right settings. (See Autodiscover strategy for more information)
+- `autodiscover_srv`: This function attempts to resolve SRV records for 
+the domain to discover IMAP and SMTP servers.
+- `autodiscover_exchange`: This function attempts to use the Exchange 
+Autodiscover service to discover email settings. It requires a username and 
+password.
+- `autodiscover_autoconfig`: This function attempts to fetch and parse an 
+autoconfig XML file from a URL specified in the domain's TXT records.
+- `autodiscover_port_scan`: This function performs a port scan on the domain 
+to discover open IMAP and SMTP ports.
+
+## 🧠 Autodiscover Strategy
+
+The `autodiscover` function uses the following strategy to discover 
+email settings:
+
+1. It first attempts to use `autodiscover_autoconfig` to discover settings 
+from an autoconfig/autodiscover URL specified in the domain's TXT records.
+2. If that fails, it attempts to use `autodiscover_srv` to discover settings 
+from the domain's SRV records.
+3. If that fails and a password is provided, it attempts to use 
+`autodiscover_exchange` to discover settings using the 
+Exchange Autodiscover service (only if credentials were provided)
+4. If all else fails, it uses `autodiscover_port_scan` to discover settings by 
+performing a port scan on the domain.
 
-```xml
-<?xml version="1.0" encoding="utf-8" ?>
-<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
-        <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
-                <User>
-                        <DisplayName>example.com Email</DisplayName>
-                </User>
-                <Account>
-                        <AccountType>email</AccountType>
-                        <Action>settings</Action>
-                        <ServiceHome>https://autodiscover.example.com</ServiceHome>
-
-                        <Protocol>
-                                <Type>IMAP</Type>
-                                <TTL>1</TTL>
-
-                                <Server>mail.example.com</Server>
-                                <Port>143</Port>
-
-                                <LoginName></LoginName>
-
-                                <DomainRequired>on</DomainRequired>
-                                <DomainName>example.com</DomainName>
-
-                                <SPA>off</SPA>
-                                <Encryption>TLS</Encryption>
-                                <AuthRequired>on</AuthRequired>
-                        </Protocol>
-                </Account>
-                <Account>
-                        <AccountType>email</AccountType>
-                        <Action>settings</Action>
-                        <ServiceHome>https://autodiscover.example.com</ServiceHome>
-
-                        <Protocol>
-                                <Type>SMTP</Type>
-                                <TTL>1</TTL>
-
-                                <Server>mail.example.com</Server>
-                                <Port>587</Port>
-
-                                <LoginName></LoginName>
-
-                                <DomainRequired>on</DomainRequired>
-                                <DomainName>example.com</DomainName>
-
-                                <SPA>off</SPA>
-                                <Encryption>TLS</Encryption>
-                                <AuthRequired>on</AuthRequired>
-                        </Protocol>
-                </Account></Response>
-</Autodiscover>
-```
+## 📜 License
 
+myl-discovery is licensed under the [GNU General Public License v3.0](LICENSE).
```

### Comparing `myl-discovery-0.5.3/myldiscovery/discovery.py` & `myl-discovery-0.5.4/myldiscovery/discovery.py`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.5.3/myldiscovery/main.py` & `myl-discovery-0.5.4/myldiscovery/main.py`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.5.3/pyproject.toml` & `myl-discovery-0.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 dependencies = [
   "dnspython == 2.3.0",
   "exchangelib == 5.0.3",
   "requests == 2.31.0",
   "rich == 13.4.2",
   "xmltodict == 0.13.0"
 ]
-version = "0.5.3"
+version = "0.5.4"
 
 [project.scripts]
 myl-discovery = "myldiscovery:main"
 
 [tool.black]
 line-length = 79
```

