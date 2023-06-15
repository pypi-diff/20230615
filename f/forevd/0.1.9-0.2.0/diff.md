# Comparing `tmp/forevd-0.1.9.tar.gz` & `tmp/forevd-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forevd-0.1.9.tar", max compression
+gzip compressed data, was "forevd-0.2.0.tar", max compression
```

## Comparing `forevd-0.1.9.tar` & `forevd-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-06-12 22:39:08.047007 forevd-0.1.9/LICENSE
--rw-r--r--   0        0        0     4065 2023-06-12 22:39:08.047007 forevd-0.1.9/README.md
--rw-r--r--   0        0        0        0 2023-06-12 22:39:08.047007 forevd-0.1.9/forevd/__init__.py
--rw-r--r--   0        0        0     6247 2023-06-12 22:39:08.047007 forevd-0.1.9/forevd/__main__.py
--rw-r--r--   0        0        0     1543 2023-06-12 22:39:08.047007 forevd-0.1.9/forevd/apache/__init__.py
--rw-r--r--   0        0        0     4836 2023-06-12 22:39:08.047007 forevd-0.1.9/forevd/apache/httpd.conf
--rw-r--r--   0        0        0      216 2023-06-12 22:39:08.047007 forevd-0.1.9/forevd/app.py
--rw-r--r--   0        0        0        0 2023-06-12 22:39:08.047007 forevd-0.1.9/forevd/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 22:39:08.047007 forevd-0.1.9/forevd/resources/logging/__init__.py
--rw-r--r--   0        0        0      387 2023-06-12 22:39:08.047007 forevd-0.1.9/forevd/resources/logging/cli.conf
--rw-r--r--   0        0        0      884 2023-06-12 22:39:08.047007 forevd-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     4770 1970-01-01 00:00:00.000000 forevd-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-15 11:21:15.919592 forevd-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5628 2023-06-15 11:21:15.919592 forevd-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-15 11:21:15.919592 forevd-0.2.0/forevd/__init__.py
+-rw-r--r--   0        0        0     6589 2023-06-15 11:21:15.919592 forevd-0.2.0/forevd/__main__.py
+-rw-r--r--   0        0        0     1543 2023-06-15 11:21:15.919592 forevd-0.2.0/forevd/apache/__init__.py
+-rw-r--r--   0        0        0     4840 2023-06-15 11:21:15.919592 forevd-0.2.0/forevd/apache/httpd.conf
+-rw-r--r--   0        0        0      216 2023-06-15 11:21:15.919592 forevd-0.2.0/forevd/app.py
+-rw-r--r--   0        0        0        0 2023-06-15 11:21:15.919592 forevd-0.2.0/forevd/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 11:21:15.919592 forevd-0.2.0/forevd/resources/logging/__init__.py
+-rw-r--r--   0        0        0      387 2023-06-15 11:21:15.919592 forevd-0.2.0/forevd/resources/logging/cli.conf
+-rw-r--r--   0        0        0      884 2023-06-15 11:21:15.919592 forevd-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6333 1970-01-01 00:00:00.000000 forevd-0.2.0/PKG-INFO
```

### Comparing `forevd-0.1.9/LICENSE` & `forevd-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `forevd-0.1.9/README.md` & `forevd-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,36 @@
+Metadata-Version: 2.1
+Name: forevd
+Version: 0.2.0
+Summary: Forward and reverse proxy using apache or nginx
+License: LICENSE
+Author: Erick Bourgeois
+Author-email: erick@jeb.ca
+Requires-Python: >=3.9,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: fastapi (>=0.95.2,<0.96.0)
+Requires-Dist: firestone-lib (>=0.1.8,<0.2.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
+Description-Content-Type: text/markdown
+
 # Table of contents
 1. [Intro](#intro)
-2. [Dependencies](#dependencies)
-3. [Running `forevd`](#running-forevd)
-    1. [Config Files](#config-files)
-    2. [Mutual TLS](#mutual-tls)
+1. [Dependencies](#dependencies)
+1. [Running `forevd`](#running-forevd)
+1. [Config Files](#config-files)
+    1. [OIDC Config](#oidc-config)
+    1. [LDAP](#ldap-config)
+1. [Mutual TLS](#mutual-tls)
+1. [Authorization](#authorization)
 
 # Intro
 
 `forevd` is a forward and reverse proxy that helps deliver authentication and, optionally,
 authorization as a sidecar.
 
 This project was created to help eliminate any need to add authentication into your application
@@ -19,38 +42,59 @@
 available at runtime.
 
 - Apache
 - nginx (TBD)
 
 # Running `forevd`
 
-The following proivides some details on how to run `forevd`. The way the options work are that
+The following proivides some details on how to run `forevd`. The way the options work is that
 anything provided immediately on the CLI, are "global" defaults; if you then provide config
 (optionally files), via the `--locations`, `--ldap` or `--oidc` options, then those will override
-the CLI options, of, e.g. `--backend` and `--location`
+the CLI options, of, e.g. `--backend` and `--location`.
 
-## Config Files
+# Config Files
 
 You can optionally provide config files for more complicated setups; this section provides soem
 examples, which can be found in the `etc` directory.
 
 The config files use Jinja2 templating via environment variables, so, instead of putting values in
 directly, you can use the form `{{ ENV_VAR_NAME }}` to have the environment varibale injected at
 runtime.
 
 The following command line options support files: `--locations`, `--ldap` or `--oidc`, via the `@`
 symbol, similar to `curl`'s command line option `--data`, for example, `--oidc @etc/oidc.yaml`
 
-### Locations Config
+## Locations Config
 
 This config allows you to provide much more control over each "location" or "endpoint" to your
 reverse proxy. For example, using different backends for different URLs or adding authorization. The
 format of the file is a dictionary of locations, or endpoints, and their correspondign data.
 
-#### Example
+### Keys
+
+There are 5 key config options for each location:
+
+1. `path`: the path, location or endpoint of what to protect or unprotect
+1. `match`: whether the path value is a regex or *match*
+1. `authc`: this is the authentication (aka `authc`) key, representing what authc to enable; this is
+   dictionary with keys being either `mtls` or `oidc`.
+1. `authz`: this is the authorization (aka `authz`) key, representing what authz to enable; this is
+   dictionary with keys, see below example and details at the [Authorization](#authorization)
+    section.
+
+Note: remember that global authentication options `--oidc` and `mtls`, so if you want to set OIDC
+across all endpoints, except, say, `/api`, you would need to disable it explicitly with:
+
+```yaml
+- path: /api
+  authc:
+    oidc: false
+```
+
+### Example
 
 The following adds LDAP group **and** static user authorization to `/`
 
 ```yaml
 - path: /
   authz:
     join_type: "any"
@@ -69,47 +113,47 @@
 - the high level keys are endpoints
 - the next level is authorization config
 - the `join_type` key word tells `forevd` how to "combine" or join the two different authorizations,
   values are:
   - `any`: if any of the authorization types match, allow connection through
   - `all`: all of the authorization types **must** match to allow connection through
 
-### OIDC Config
+## OIDC Config
 
 This is useful for adding any other global OIDC config; there are required fields for the auth to
 work, e.g. `ClientID` and `ClientSecret`.
 
-#### Example
+### Example
 
 ```yaml
 ProviderMetadataUrl: "https://{{ OIDC_PROVIDER_NAME }}.us.auth0.com/.well-known/openid-configuration"
 RedirectURI: "https://erick-pro.jeb.ca:8080/secure/redirect_uri"
 ClientId: "{{ OIDC_CLIENT_ID }}"
 ClientSecret: "{{ OIDC_CLIENT_SECRET }}"
 Scope: '"openid profile"'
 PKCEMethod: S256
 RemoteUserClaim: nickname
 ```
 
-### LDAP Config
+## LDAP Config
 
 This is used for global LDAP config, e.g. setting cache information for `mod_ldap`. Note: The `LDAP`
 prefix is stripped, as it's redundant and it's added as part of the config generation.
 
-#### Example
+### Example
 
 ```yaml
 SharedCacheSize: 500000
 CacheEntries: 1024
 CacheTTL: 600
 OpCacheEntries: 1024
 OpCacheTTL: 600
 ```
 
-## Mutual TLS
+# Mutual TLS
 
 The following command provides termination of mTLS on `/` and passes connections to a backend at
 `http://0.0.0.0:8080`
 
 ```
 forevd --debug --listen 0.0.0.0:8080 \
     --ca-cert $PWD/../certs/ca/ca-cert.pem
@@ -118,14 +162,27 @@
     --backend http://localhost:8081
     --location /
     --mtls require
     --server-name example.com
     --var-dir /var/tmp/apache
 ```
 
-## Authorization
+# Authorization
 
 To add authorization, it's recommended you use a config file for the `--locations` command line.
 
-There is currently support for LDAP group lookup and static user names.
+There is currently support for LDAP group lookups, static user names, or allow all valid users. Here
+are the keys supported:
+
+1. `allow_all`: this key let's `forevd` know to allow all valid users through
+1. `join_type`: this is the "join" type between all authorizations setup
+  - `any`: if any of the authorization types match, allow connection through
+  - `all`: all of the authorization types **must** match to allow connection through
+1. `ldap`: this is the LDAP configuration for group lookups, keys are:
+   - `url`: LDAP URL, e.g. `ldaps://127.0.0.1/DC=foo,DC=example,DC=com`
+   - `bind-dn`: the DN for bind operation
+   - `bind-pw`: the password for bind operation
+   - `groups`: a list of groups DNs
+1. `users`: a list of user names to verify against
 
 See [Locations Example](#example) for more detail.
+
```

### Comparing `forevd-0.1.9/forevd/__main__.py` & `forevd-0.2.0/forevd/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     return None
 
 
 def _nomalize_locations(
     locations: dict,
     backend: str,
     location: str,
+    oidc: bool,
     mtls: bool,
     http_methods: list,
     set_access_token: bool,
 ):
     if not locations:
         locations = []
 
@@ -58,24 +59,32 @@
         missing_cli_loc = True
     _LOGGER.debug(f"endpoints: {endpoints}")
 
     for endpoint in endpoints:
         config = _get_loc_by_path(locations, endpoint)
         if not config:
             config = {"path": endpoint}
+        authc = config.get("authc", {})
+        authz = config.get("authz", {})
+
+        if "allow_all" in authz and "join_type" in authz:
+            raise click.UsageError("Locations must contain a path")
 
         if "backend" not in config:
             config["backend"] = backend
-        if "mtls" not in config:
-            config["mtls"] = mtls
+        if mtls and "mtls" not in authc:
+            authc["mtls"] = mtls
+        if oidc and "oidc" not in authc:
+            authc["oidc"] = oidc
         if "http_methods" not in config:
             config["http_methods"] = http_methods
         if "set_access_token" not in config:
             config["set_access_token"] = set_access_token
 
+        config["authc"] = authc
         if missing_cli_loc:
             locations.append(config)
 
     _LOGGER.debug(f"locations: {locations}")
 
     return locations
 
@@ -234,15 +243,15 @@
         "ca_cert": ca_cert,
         "cert": cert,
         "cert_key": cert_key,
         "httpd_include": httpd_include,
         "debug": debug,
         "ldap": ldap,
         "locations": _nomalize_locations(
-            locations, backend, location, mtls, http_methods, set_access_token
+            locations, backend, location, oidc, mtls, http_methods, set_access_token
         ),
         "listen": listen,
         "oidc": oidc,
         "server_name": server_name,
     }
     _LOGGER.debug(f"config: {config}")
```

### Comparing `forevd-0.1.9/forevd/apache/__init__.py` & `forevd-0.2.0/forevd/apache/__init__.py`

 * *Files identical despite different names*

### Comparing `forevd-0.1.9/forevd/apache/httpd.conf` & `forevd-0.2.0/forevd/apache/httpd.conf`

 * *Files 4% similar despite different names*

```diff
@@ -85,28 +85,29 @@
 LDAP{{ key }} {{ value }}
 {% endfor %}
 {% endif -%}
 
 {% for location in locations -%}
 {% set path = location["path"] -%}
 {% set authz = location.get("authz", {}) -%}
+{% set authc = location.get("authc", {}) -%}
 
 {# Setup the required users #}
 {% if authz -%}
     {% set authz_required_users = [] -%}
     {% if "users" in authz -%}
         {% set users = authz["users"]|join(" ") -%}
         {% do authz_required_users.append("Require user " ~ users) %}
     {% endif -%}
     {% if "ldap" in authz -%}
         {% for group in authz["ldap"]["groups"] -%}
         {% do authz_required_users.append("Require ldap-group " ~ group) %}
         {% endfor -%}
     {% endif -%}
-    {% if not authz_required_users -%}
+    {% if authz["allow_all"] -%}
         {% set authz_required_users = ["Require valid-user"] -%}
     {% endif -%}
 
     {% set join_type = authz.get("join_type") -%}
     {% if join_type == "any" -%}
         {% do authz_required_users.insert(0, "<RequireAny>") %}
         {% do authz_required_users.append("</RequireAny>") %}
@@ -122,35 +123,35 @@
     {% if "include" in location -%}
     {{ location["include"] }}
     {% endif -%}
 
     ProxyPass {{ location["backend"] }}
     ProxyPassReverse {{ location["backend"] }}
 
-    {% if location["mtls"] %}
+    {% if authc["mtls"] and cert -%}
     SSLOptions +StdEnvVars
     SSLUserName SSL_CLIENT_S_DN_CN
-    SSLVerifyCLient {{ location["mtls"] }}
+    SSLVerifyCLient {{ authc["mtls"] }}
 
     RequestHeader set X-Remote-User %{SSL_CLIENT_S_DN_CN}e
     RequestHeader set X-SSL-certificate "%{SSL_CLIENT_CERT}s" "expr=-n %{SSL_CLIENT_CERT}"
     {% endif %}
 
-    {% if oidc -%}
+    {% if authc["oidc"] -%}
     AuthType openid-connect
     RequestHeader set X-Remote-User %{REMOTE_USER}s "expr=-n %{REMOTE_USER}"
     {% if location["set_access_token"] -%}
     RequestHeader set Authorization "Bearer %{OIDC_access_token}e" env=OIDC_access_token
     {% endif %}
     {% endif %}
 
-    {% if "ldap" in location["authz"] -%}
-    AuthLDAPURL {{ location["authz"]["ldap"]["url"] }}
-    AuthLDAPBindDN {{ location["authz"]["ldap"]["bind-dn"] }}
-    AuthLDAPBindPassword {{ location["authz"]["ldap"]["bind-pw"] }}
+    {% if "ldap" in authz -%}
+    AuthLDAPURL {{ authz["ldap"]["url"] }}
+    AuthLDAPBindDN {{ authz["ldap"]["bind-dn"] }}
+    AuthLDAPBindPassword {{ authz["ldap"]["bind-pw"] }}
     {% endif %}
 
     {% if not location["http_methods"] %}
     {{ required_users }}
     {% else -%}
     <Limit {{ location["http_methods"]|join(" ") }}>
         {{ required_users }}
```

### Comparing `forevd-0.1.9/pyproject.toml` & `forevd-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "forevd"
-version = "0.1.9"
+version = "0.2.0"
 description = "Forward and reverse proxy using apache or nginx"
 authors = ["Erick Bourgeois <erick@jeb.ca>"]
 license = "LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `forevd-0.1.9/PKG-INFO` & `forevd-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,16 @@
-Metadata-Version: 2.1
-Name: forevd
-Version: 0.1.9
-Summary: Forward and reverse proxy using apache or nginx
-License: LICENSE
-Author: Erick Bourgeois
-Author-email: erick@jeb.ca
-Requires-Python: >=3.9,<4.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: fastapi (>=0.95.2,<0.96.0)
-Requires-Dist: firestone-lib (>=0.1.8,<0.2.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
-Description-Content-Type: text/markdown
-
 # Table of contents
 1. [Intro](#intro)
-2. [Dependencies](#dependencies)
-3. [Running `forevd`](#running-forevd)
-    1. [Config Files](#config-files)
-    2. [Mutual TLS](#mutual-tls)
+1. [Dependencies](#dependencies)
+1. [Running `forevd`](#running-forevd)
+1. [Config Files](#config-files)
+    1. [OIDC Config](#oidc-config)
+    1. [LDAP](#ldap-config)
+1. [Mutual TLS](#mutual-tls)
+1. [Authorization](#authorization)
 
 # Intro
 
 `forevd` is a forward and reverse proxy that helps deliver authentication and, optionally,
 authorization as a sidecar.
 
 This project was created to help eliminate any need to add authentication into your application
@@ -39,38 +22,59 @@
 available at runtime.
 
 - Apache
 - nginx (TBD)
 
 # Running `forevd`
 
-The following proivides some details on how to run `forevd`. The way the options work are that
+The following proivides some details on how to run `forevd`. The way the options work is that
 anything provided immediately on the CLI, are "global" defaults; if you then provide config
 (optionally files), via the `--locations`, `--ldap` or `--oidc` options, then those will override
-the CLI options, of, e.g. `--backend` and `--location`
+the CLI options, of, e.g. `--backend` and `--location`.
 
-## Config Files
+# Config Files
 
 You can optionally provide config files for more complicated setups; this section provides soem
 examples, which can be found in the `etc` directory.
 
 The config files use Jinja2 templating via environment variables, so, instead of putting values in
 directly, you can use the form `{{ ENV_VAR_NAME }}` to have the environment varibale injected at
 runtime.
 
 The following command line options support files: `--locations`, `--ldap` or `--oidc`, via the `@`
 symbol, similar to `curl`'s command line option `--data`, for example, `--oidc @etc/oidc.yaml`
 
-### Locations Config
+## Locations Config
 
 This config allows you to provide much more control over each "location" or "endpoint" to your
 reverse proxy. For example, using different backends for different URLs or adding authorization. The
 format of the file is a dictionary of locations, or endpoints, and their correspondign data.
 
-#### Example
+### Keys
+
+There are 5 key config options for each location:
+
+1. `path`: the path, location or endpoint of what to protect or unprotect
+1. `match`: whether the path value is a regex or *match*
+1. `authc`: this is the authentication (aka `authc`) key, representing what authc to enable; this is
+   dictionary with keys being either `mtls` or `oidc`.
+1. `authz`: this is the authorization (aka `authz`) key, representing what authz to enable; this is
+   dictionary with keys, see below example and details at the [Authorization](#authorization)
+    section.
+
+Note: remember that global authentication options `--oidc` and `mtls`, so if you want to set OIDC
+across all endpoints, except, say, `/api`, you would need to disable it explicitly with:
+
+```yaml
+- path: /api
+  authc:
+    oidc: false
+```
+
+### Example
 
 The following adds LDAP group **and** static user authorization to `/`
 
 ```yaml
 - path: /
   authz:
     join_type: "any"
@@ -89,47 +93,47 @@
 - the high level keys are endpoints
 - the next level is authorization config
 - the `join_type` key word tells `forevd` how to "combine" or join the two different authorizations,
   values are:
   - `any`: if any of the authorization types match, allow connection through
   - `all`: all of the authorization types **must** match to allow connection through
 
-### OIDC Config
+## OIDC Config
 
 This is useful for adding any other global OIDC config; there are required fields for the auth to
 work, e.g. `ClientID` and `ClientSecret`.
 
-#### Example
+### Example
 
 ```yaml
 ProviderMetadataUrl: "https://{{ OIDC_PROVIDER_NAME }}.us.auth0.com/.well-known/openid-configuration"
 RedirectURI: "https://erick-pro.jeb.ca:8080/secure/redirect_uri"
 ClientId: "{{ OIDC_CLIENT_ID }}"
 ClientSecret: "{{ OIDC_CLIENT_SECRET }}"
 Scope: '"openid profile"'
 PKCEMethod: S256
 RemoteUserClaim: nickname
 ```
 
-### LDAP Config
+## LDAP Config
 
 This is used for global LDAP config, e.g. setting cache information for `mod_ldap`. Note: The `LDAP`
 prefix is stripped, as it's redundant and it's added as part of the config generation.
 
-#### Example
+### Example
 
 ```yaml
 SharedCacheSize: 500000
 CacheEntries: 1024
 CacheTTL: 600
 OpCacheEntries: 1024
 OpCacheTTL: 600
 ```
 
-## Mutual TLS
+# Mutual TLS
 
 The following command provides termination of mTLS on `/` and passes connections to a backend at
 `http://0.0.0.0:8080`
 
 ```
 forevd --debug --listen 0.0.0.0:8080 \
     --ca-cert $PWD/../certs/ca/ca-cert.pem
@@ -138,15 +142,26 @@
     --backend http://localhost:8081
     --location /
     --mtls require
     --server-name example.com
     --var-dir /var/tmp/apache
 ```
 
-## Authorization
+# Authorization
 
 To add authorization, it's recommended you use a config file for the `--locations` command line.
 
-There is currently support for LDAP group lookup and static user names.
+There is currently support for LDAP group lookups, static user names, or allow all valid users. Here
+are the keys supported:
 
-See [Locations Example](#example) for more detail.
+1. `allow_all`: this key let's `forevd` know to allow all valid users through
+1. `join_type`: this is the "join" type between all authorizations setup
+  - `any`: if any of the authorization types match, allow connection through
+  - `all`: all of the authorization types **must** match to allow connection through
+1. `ldap`: this is the LDAP configuration for group lookups, keys are:
+   - `url`: LDAP URL, e.g. `ldaps://127.0.0.1/DC=foo,DC=example,DC=com`
+   - `bind-dn`: the DN for bind operation
+   - `bind-pw`: the password for bind operation
+   - `groups`: a list of groups DNs
+1. `users`: a list of user names to verify against
 
+See [Locations Example](#example) for more detail.
```

