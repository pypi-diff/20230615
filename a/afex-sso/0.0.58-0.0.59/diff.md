# Comparing `tmp/afex-sso-0.0.58.tar.gz` & `tmp/afex-sso-0.0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afex-sso-0.0.58.tar", last modified: Wed Jun 14 09:23:05 2023, max compression
+gzip compressed data, was "afex-sso-0.0.59.tar", last modified: Thu Jun 15 09:28:37 2023, max compression
```

## Comparing `afex-sso-0.0.58.tar` & `afex-sso-0.0.59.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 09:23:05.525362 afex-sso-0.0.58/
--rw-rw-rw-   0        0        0     1069 2023-04-05 13:47:57.000000 afex-sso-0.0.58/LICENSE
--rw-rw-rw-   0        0        0     2315 2023-06-14 09:23:05.525362 afex-sso-0.0.58/PKG-INFO
--rw-rw-rw-   0        0        0     1289 2023-06-08 16:38:28.000000 afex-sso-0.0.58/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 09:23:05.493651 afex-sso-0.0.58/app/
-drwxrwxrwx   0        0        0        0 2023-06-14 09:23:05.500157 afex-sso-0.0.58/app/AFEX_SSO/
--rw-rw-rw-   0        0        0       36 2023-04-05 13:47:57.000000 afex-sso-0.0.58/app/AFEX_SSO/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:23:05.509715 afex-sso-0.0.58/app/AFEX_SSO/src/
--rw-rw-rw-   0        0        0        0 2023-04-05 13:47:57.000000 afex-sso-0.0.58/app/AFEX_SSO/src/__init__.py
--rw-rw-rw-   0        0        0      270 2023-06-07 09:13:59.000000 afex-sso-0.0.58/app/AFEX_SSO/src/get_hash_key.py
--rw-rw-rw-   0        0        0     2155 2023-06-08 16:53:35.000000 afex-sso-0.0.58/app/AFEX_SSO/src/sso.py
--rw-rw-rw-   0        0        0     1938 2023-06-14 09:22:50.000000 afex-sso-0.0.58/app/AFEX_SSO/src/views.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:23:05.509715 afex-sso-0.0.58/app/afex_sso.egg-info/
--rw-rw-rw-   0        0        0     2315 2023-06-14 09:23:05.000000 afex-sso-0.0.58/app/afex_sso.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-06-14 09:23:05.000000 afex-sso-0.0.58/app/afex_sso.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 09:23:05.000000 afex-sso-0.0.58/app/afex_sso.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-14 09:23:05.000000 afex-sso-0.0.58/app/afex_sso.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 09:23:05.000000 afex-sso-0.0.58/app/afex_sso.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      142 2023-04-05 13:47:57.000000 afex-sso-0.0.58/pyproject.toml
--rw-rw-rw-   0        0        0      497 2023-06-14 09:23:05.525362 afex-sso-0.0.58/setup.cfg
--rw-rw-rw-   0        0        0      802 2023-06-14 09:22:56.000000 afex-sso-0.0.58/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:28:37.383061 afex-sso-0.0.59/
+-rw-rw-rw-   0        0        0     1069 2023-04-05 13:47:57.000000 afex-sso-0.0.59/LICENSE
+-rw-rw-rw-   0        0        0     2315 2023-06-15 09:28:37.383061 afex-sso-0.0.59/PKG-INFO
+-rw-rw-rw-   0        0        0     1289 2023-06-08 16:38:28.000000 afex-sso-0.0.59/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 09:28:37.285704 afex-sso-0.0.59/app/
+drwxrwxrwx   0        0        0        0 2023-06-15 09:28:37.316775 afex-sso-0.0.59/app/AFEX_SSO/
+-rw-rw-rw-   0        0        0       36 2023-04-05 13:47:57.000000 afex-sso-0.0.59/app/AFEX_SSO/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:28:37.355975 afex-sso-0.0.59/app/AFEX_SSO/src/
+-rw-rw-rw-   0        0        0        0 2023-04-05 13:47:57.000000 afex-sso-0.0.59/app/AFEX_SSO/src/__init__.py
+-rw-rw-rw-   0        0        0      270 2023-06-07 09:13:59.000000 afex-sso-0.0.59/app/AFEX_SSO/src/get_hash_key.py
+-rw-rw-rw-   0        0        0     2155 2023-06-08 16:53:35.000000 afex-sso-0.0.59/app/AFEX_SSO/src/sso.py
+-rw-rw-rw-   0        0        0     2218 2023-06-14 13:06:41.000000 afex-sso-0.0.59/app/AFEX_SSO/src/views.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:28:37.383061 afex-sso-0.0.59/app/afex_sso.egg-info/
+-rw-rw-rw-   0        0        0     2315 2023-06-15 09:28:37.000000 afex-sso-0.0.59/app/afex_sso.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-06-15 09:28:37.000000 afex-sso-0.0.59/app/afex_sso.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 09:28:37.000000 afex-sso-0.0.59/app/afex_sso.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-15 09:28:37.000000 afex-sso-0.0.59/app/afex_sso.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 09:28:37.000000 afex-sso-0.0.59/app/afex_sso.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      142 2023-04-05 13:47:57.000000 afex-sso-0.0.59/pyproject.toml
+-rw-rw-rw-   0        0        0      497 2023-06-15 09:28:37.383061 afex-sso-0.0.59/setup.cfg
+-rw-rw-rw-   0        0        0      802 2023-06-15 09:27:12.000000 afex-sso-0.0.59/setup.py
```

### Comparing `afex-sso-0.0.58/LICENSE` & `afex-sso-0.0.59/LICENSE`

 * *Files identical despite different names*

### Comparing `afex-sso-0.0.58/PKG-INFO` & `afex-sso-0.0.59/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-sso
-Version: 0.0.58
+Version: 0.0.59
 Summary: For integrating sso
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@africaexchange.com
 License: MIT
 Description: 
         # AFEX SSO (DJANGO)
```

### Comparing `afex-sso-0.0.58/README.md` & `afex-sso-0.0.59/README.md`

 * *Files identical despite different names*

### Comparing `afex-sso-0.0.58/app/AFEX_SSO/src/sso.py` & `afex-sso-0.0.59/app/AFEX_SSO/src/sso.py`

 * *Files identical despite different names*

### Comparing `afex-sso-0.0.58/app/AFEX_SSO/src/views.py` & `afex-sso-0.0.59/app/AFEX_SSO/src/views.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,19 +13,25 @@
 UserModel = get_user_model()
 
 
 
 class AdminLoginView(View):
 
     def get(self, request, *kwargs):
+        url = f"{request.scheme}://{request.get_host()}{request.path}"
         request_url = base64.b64encode(
-            request.build_absolute_uri().encode('utf-8')
+            url.encode('utf-8')
         ).decode('utf-8')
+
+        if 'next' in request.GET.keys():
+            request.session['next'] = request.GET.get('next')
+
         if 'q' in request.GET.keys() or request.session.get('state'):
             ses_id = request.GET.get('q') or request.session.get('state')
+
             if not request.session.get('state'):
                 request.session['state'] = ses_id
             validate_sso = sso.check_credentials(session_key=ses_id)
             try:
                 response_data = validate_sso['data']
             except:
                 return redirect(f"{sso_url}?qz={request_url}")
@@ -33,21 +39,24 @@
             user_data = response_data.get('user')
             if user_data.get('email') and not UserModel.objects.filter(email=user_data.get('email')).exists():
                 user = UserModel.objects.create(
                     email=user_data.get('email'),
                     username=user_data.get('email'),
                     first_name=user_data.get('first_name'),
                     last_name=user_data.get('last_name'),
+                    is_staff=True
                 )
             else:
                 user = UserModel.objects.get(email=user_data.get('email'))
+                if not user.is_staff:
+                    user.is_staff = True
+                    user.save()
 
-            if not user.is_staff:
-                user.is_staff = True
-                user.save()
             login(request, user)
 
+            if request.session.get('next'):
+                return redirect(request.session.get('next'))
             return redirect("admin:index")
 
-        elif 'ec' in request.GET.keys() or 'next' in request.GET.keys():
+        elif 'ec' in request.GET.keys():
             return redirect(f"/?ec={request.GET.get('ec')}")
         return redirect(f"{sso_url}?qz={request_url}")
```

### Comparing `afex-sso-0.0.58/app/afex_sso.egg-info/PKG-INFO` & `afex-sso-0.0.59/app/afex_sso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-sso
-Version: 0.0.58
+Version: 0.0.59
 Summary: For integrating sso
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@africaexchange.com
 License: MIT
 Description: 
         # AFEX SSO (DJANGO)
```

### Comparing `afex-sso-0.0.58/setup.py` & `afex-sso-0.0.59/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("./README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="afex-sso",
-    version="0.0.58",
+    version="0.0.59",
     description="For integrating sso",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="AFEX NIGERIA",
```

