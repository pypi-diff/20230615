# Comparing `tmp/myl-discovery-0.5.2.tar.gz` & `tmp/myl-discovery-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myl-discovery-0.5.2.tar", last modified: Thu Jun 15 06:05:31 2023, max compression
+gzip compressed data, was "myl-discovery-0.5.3.tar", last modified: Thu Jun 15 06:31:44 2023, max compression
```

## Comparing `myl-discovery-0.5.2.tar` & `myl-discovery-0.5.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:05:31.574865 myl-discovery-0.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:05:31.570865 myl-discovery-0.5.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-15 06:05:17.000000 myl-discovery-0.5.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:05:31.570865 myl-discovery-0.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-15 06:05:17.000000 myl-discovery-0.5.2/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-15 06:05:17.000000 myl-discovery-0.5.2/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-15 06:05:17.000000 myl-discovery-0.5.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 06:05:17.000000 myl-discovery-0.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 06:05:17.000000 myl-discovery-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44811 2023-06-15 06:05:31.574865 myl-discovery-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-15 06:05:17.000000 myl-discovery-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:05:31.574865 myl-discovery-0.5.2/myl_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44811 2023-06-15 06:05:31.000000 myl-discovery-0.5.2/myl_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-15 06:05:31.000000 myl-discovery-0.5.2/myl_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:05:31.000000 myl-discovery-0.5.2/myl_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 06:05:31.000000 myl-discovery-0.5.2/myl_discovery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-15 06:05:31.000000 myl-discovery-0.5.2/myl_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 06:05:31.000000 myl-discovery-0.5.2/myl_discovery.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:05:31.574865 myl-discovery-0.5.2/myldiscovery/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-15 06:05:17.000000 myl-discovery-0.5.2/myldiscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 06:05:17.000000 myl-discovery-0.5.2/myldiscovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-06-15 06:05:17.000000 myl-discovery-0.5.2/myldiscovery/discovery.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2016 2023-06-15 06:05:17.000000 myl-discovery-0.5.2/myldiscovery/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-15 06:05:17.000000 myl-discovery-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 06:05:31.574865 myl-discovery-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:31:44.733097 myl-discovery-0.5.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:31:44.729097 myl-discovery-0.5.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:31:44.729097 myl-discovery-0.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44811 2023-06-15 06:31:44.733097 myl-discovery-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:31:44.733097 myl-discovery-0.5.3/myl_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44811 2023-06-15 06:31:44.000000 myl-discovery-0.5.3/myl_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-15 06:31:44.000000 myl-discovery-0.5.3/myl_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:31:44.000000 myl-discovery-0.5.3/myl_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 06:31:44.000000 myl-discovery-0.5.3/myl_discovery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-15 06:31:44.000000 myl-discovery-0.5.3/myl_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 06:31:44.000000 myl-discovery-0.5.3/myl_discovery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:31:44.733097 myl-discovery-0.5.3/myldiscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/myldiscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/myldiscovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/myldiscovery/discovery.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2016 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/myldiscovery/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-15 06:31:31.000000 myl-discovery-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 06:31:44.733097 myl-discovery-0.5.3/setup.cfg
```

### Comparing `myl-discovery-0.5.2/.github/workflows/pypi.yaml` & `myl-discovery-0.5.3/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.5.2/.github/workflows/release.yaml` & `myl-discovery-0.5.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.5.2/LICENSE` & `myl-discovery-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.5.2/PKG-INFO` & `myl-discovery-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl-discovery
-Version: 0.5.2
+Version: 0.5.3
 Summary: email autodiscovery
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-discovery-0.5.2/README.md` & `myl-discovery-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.5.2/myl_discovery.egg-info/PKG-INFO` & `myl-discovery-0.5.3/myl_discovery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl-discovery
-Version: 0.5.2
+Version: 0.5.3
 Summary: email autodiscovery
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-discovery-0.5.2/myldiscovery/discovery.py` & `myl-discovery-0.5.3/myldiscovery/discovery.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,18 +62,21 @@
         }
         data.append(entry)
 
     return data
 
 
 def autodiscover_txt(domain):
-    res = resolve_txt(domain, criteria="^mailconf=")
-    if not res:
-        return
-    return res.split("=")[1]
+    try:
+        res = resolve_txt(domain, criteria="^mailconf=")
+        if not res:
+            return
+        return res.split("=")[1]
+    except Exception:
+        LOGGER.warning("Failed to resolve TXT record")
 
 
 def parse_autoconfig(content):
     data = xmltodict.parse(content)
 
     imap = (
         data.get("clientConfig", {})
@@ -143,37 +146,43 @@
             "port": int(smtp.get("Port")),
             "starttls": smtp.get("Encryption", "").lower() == "tls",
         },
     }
 
 
 def autodiscover_srv(domain):
-    imap = resolve_srv(f"_imaps._tcp.{domain}")
-    smtp = resolve_srv(f"_submission._tcp.{domain}")
+    try:
+        imap = resolve_srv(f"_imaps._tcp.{domain}")
+        smtp = resolve_srv(f"_submission._tcp.{domain}")
 
-    return {
-        "imap": {
-            "server": imap[0].get("hostname"),
-            "port": int(imap[0].get("port")),
-            # FIXME We might want to "smartly" guess if starttls should be
-            # enabled or not, depending on the port:
-            # 143 -> starttls
-            # 993 -> no
-            "starttls": False,
-        },
-        "smtp": {
-            "server": smtp[0].get("hostname"),
-            "port": int(smtp[0].get("port")),
-            # FIXME We might want to "smartly" guess if starttls should be
-            # enabled or not, depending on the port:
-            # 465 -> starttls
-            # 587 -> no
-            "starttls": False,
-        },
-    }
+        assert imap is not None
+        assert smtp is not None
+
+        return {
+            "imap": {
+                "server": imap[0].get("hostname"),
+                "port": int(imap[0].get("port")),
+                # FIXME We might want to "smartly" guess if starttls should be
+                # enabled or not, depending on the port:
+                # 143 -> starttls
+                # 993 -> no
+                "starttls": False,
+            },
+            "smtp": {
+                "server": smtp[0].get("hostname"),
+                "port": int(smtp[0].get("port")),
+                # FIXME We might want to "smartly" guess if starttls should be
+                # enabled or not, depending on the port:
+                # 465 -> starttls
+                # 587 -> no
+                "starttls": False,
+            },
+        }
+    except Exception as e:
+        LOGGER.warning(f"Failed to resolve SRV records: {e}")
 
 
 def port_check(host, port):
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     result = sock.connect_ex((host, int(port)))
     sock.close()
     return result == 0
@@ -183,22 +192,27 @@
     res = {}
     for port in [25, 465, 587, 993]:
         res[port] = port_check(host, port)
     return res
 
 
 def autodiscover_exchange(email, password, username=None):
-    if not username:
-        username = email
-    creds = Credentials(username=username, password=password)
-    account = Account(
-        primary_smtp_address=email, credentials=creds, autodiscover=True
-    )
-    server = account.protocol.server
+    try:
+        if not username:
+            username = email
+        creds = Credentials(username=username, password=password)
+        account = Account(
+            primary_smtp_address=email, credentials=creds, autodiscover=True
+        )
+        return autodiscover_port_scan(account.protocol.server)
+    except Exception as e:
+        LOGGER.warning(f"Failed to autodiscover Exchange: {e}")
+
 
+def autodiscover_port_scan(server):
     portscan = check_email_ports(server)
     LOGGER.info(f"Port scan results: {portscan}")
 
     imap_port = imap_starttls = None
     if portscan.get(993):
         imap_port = 993
         imap_starttls = False
@@ -224,37 +238,44 @@
             "server": server,
             "port": smtp_port,
             "starttls": smtp_starttls,
         },
     }
 
 
-def autodiscover(email_addr, srv_only=False, username=None, password=None):
-    domain = email_addr.split("@")[-1]
-    if not domain:
-        raise ValueError(f"Invalid email address {email_addr}")
-
-    if srv_only:
-        return autodiscover_srv(domain)
-
+def autodiscover_autoconfig(domain):
     autoconfig = autodiscover_txt(domain)
 
     if not autoconfig:
-        try:
-            return autodiscover_srv(domain)
-        except Exception:
-            LOGGER.warning("Failed to autodiscover using SRV records")
-            if password:
-                LOGGER.info("Trying autodiscover using Exchange credentials")
-                return autodiscover_exchange(
-                    email=email_addr, username=username, password=password
-                )
-            return
+        LOGGER.warning("Failed to autodiscover using TXT records")
+        return
 
     res = requests.get(autoconfig)
     res.raise_for_status()
 
     try:
         return parse_autoconfig(res.text)
     except Exception:
         LOGGER.warning("Failed to parse autoconfig, trying autodiscover")
         return parse_autodiscover(res.text)
+
+
+def autodiscover(email_addr, username=None, password=None):
+    domain = email_addr.split("@")[-1]
+    if not domain:
+        raise ValueError(f"Invalid email address {email_addr}")
+
+    res = autodiscover_autoconfig(domain)
+
+    if not res:
+        res = autodiscover_srv(domain)
+
+    if not res and password:
+        res = autodiscover_srv(domain)
+        autodiscover_exchange(
+            email=email_addr, username=username, password=password
+        )
+
+    if not res:
+        res = autodiscover_port_scan(domain)
+
+    return res
```

### Comparing `myl-discovery-0.5.2/myldiscovery/main.py` & `myl-discovery-0.5.3/myldiscovery/main.py`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.5.2/pyproject.toml` & `myl-discovery-0.5.3/pyproject.toml`

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
-version = "0.5.2"
+version = "0.5.3"
 
 [project.scripts]
 myl-discovery = "myldiscovery:main"
 
 [tool.black]
 line-length = 79
```

