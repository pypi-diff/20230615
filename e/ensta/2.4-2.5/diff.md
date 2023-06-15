# Comparing `tmp/ensta-2.4.tar.gz` & `tmp/ensta-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensta-2.4.tar", last modified: Thu Jun 15 10:12:24 2023, max compression
+gzip compressed data, was "ensta-2.5.tar", last modified: Thu Jun 15 14:36:48 2023, max compression
```

## Comparing `ensta-2.4.tar` & `ensta-2.5.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:12:24.238098 ensta-2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-15 10:12:03.000000 ensta-2.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-15 10:12:24.238098 ensta-2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-06-15 10:12:03.000000 ensta-2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:12:24.238098 ensta-2.4/ensta/
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-15 10:12:03.000000 ensta-2.4/ensta/Authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-06-15 10:12:03.000000 ensta-2.4/ensta/Guest.py
--rw-r--r--   0 runner    (1001) docker     (123)    22025 2023-06-15 10:12:03.000000 ensta-2.4/ensta/Host.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-15 10:12:03.000000 ensta-2.4/ensta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:12:24.238098 ensta-2.4/ensta/containers/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-15 10:12:03.000000 ensta-2.4/ensta/containers/FollowPerson.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-15 10:12:03.000000 ensta-2.4/ensta/containers/FollowedStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-15 10:12:03.000000 ensta-2.4/ensta/containers/Profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-15 10:12:03.000000 ensta-2.4/ensta/containers/UnfollowedStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-15 10:12:03.000000 ensta-2.4/ensta/containers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:12:24.238098 ensta-2.4/ensta/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-15 10:12:03.000000 ensta-2.4/ensta/lib/Commons.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-15 10:12:03.000000 ensta-2.4/ensta/lib/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-15 10:12:03.000000 ensta-2.4/ensta/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:12:24.238098 ensta-2.4/ensta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-15 10:12:24.000000 ensta-2.4/ensta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-15 10:12:24.000000 ensta-2.4/ensta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:12:24.000000 ensta-2.4/ensta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 10:12:24.000000 ensta-2.4/ensta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 10:12:24.000000 ensta-2.4/ensta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-15 10:12:24.238098 ensta-2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-15 10:12:03.000000 ensta-2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:48.465971 ensta-2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-15 14:36:30.000000 ensta-2.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-15 14:36:48.465971 ensta-2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-06-15 14:36:30.000000 ensta-2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:48.465971 ensta-2.5/ensta/
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-15 14:36:30.000000 ensta-2.5/ensta/Authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-06-15 14:36:30.000000 ensta-2.5/ensta/Guest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19848 2023-06-15 14:36:30.000000 ensta-2.5/ensta/Host.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-15 14:36:30.000000 ensta-2.5/ensta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:48.465971 ensta-2.5/ensta/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-15 14:36:30.000000 ensta-2.5/ensta/containers/FollowPerson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-15 14:36:30.000000 ensta-2.5/ensta/containers/FollowedStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-15 14:36:30.000000 ensta-2.5/ensta/containers/Profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-15 14:36:30.000000 ensta-2.5/ensta/containers/ProfileHost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-15 14:36:30.000000 ensta-2.5/ensta/containers/UnfollowedStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-15 14:36:30.000000 ensta-2.5/ensta/containers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:48.465971 ensta-2.5/ensta/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-15 14:36:30.000000 ensta-2.5/ensta/lib/Commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-15 14:36:30.000000 ensta-2.5/ensta/lib/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-15 14:36:30.000000 ensta-2.5/ensta/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:48.465971 ensta-2.5/ensta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-15 14:36:48.000000 ensta-2.5/ensta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-15 14:36:48.000000 ensta-2.5/ensta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:36:48.000000 ensta-2.5/ensta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 14:36:48.000000 ensta-2.5/ensta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 14:36:48.000000 ensta-2.5/ensta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-15 14:36:48.465971 ensta-2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-15 14:36:30.000000 ensta-2.5/setup.py
```

### Comparing `ensta-2.4/LICENSE.txt` & `ensta-2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ensta-2.4/PKG-INFO` & `ensta-2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 2.4
+Version: 2.5
 Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
 Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.4.tar.gz
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.5.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram-client,instagram,api-wrapper,instagram-scraper,instagram-api,instagram-sdk,instagram-photos,instagram-api-python,instabot,instagram-stories,instagram-bot,instapy,instagram-downloader,instagram-account,instagram-crawler,instagram-private-api,igtv,instagram-automation,reels,instagram-feed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `ensta-2.4/README.md` & `ensta-2.5/README.md`

 * *Files identical despite different names*

### Comparing `ensta-2.4/ensta/Authentication.py` & `ensta-2.5/ensta/Authentication.py`

 * *Files identical despite different names*

### Comparing `ensta-2.4/ensta/Guest.py` & `ensta-2.5/ensta/Guest.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     update_app_id,
     refresh_csrf_token,
     format_username,
     format_uid
 )
 from .lib.Exceptions import APIError
 from .containers.Profile import Profile
+from .containers.ProfileHost import ProfileHost
+import dataclasses
 
 
 class Guest:
     request_session: requests.Session = None
     homepage_source: str = None
     insta_app_id: str = None
     csrf_token: str = None
@@ -70,15 +72,15 @@
             response_json = http_response.json()
 
             if "errors" in response_json:
                 return "username" not in response_json["errors"]
         except JSONDecodeError:
             return None
 
-    def profile(self, username: str, __session__: requests.Session = None) -> Profile | None:
+    def profile(self, username: str, __session__: requests.Session | None = None) -> Profile | ProfileHost | None:
         username: str = format_username(username)
         refresh_csrf_token(self)
         request_headers: dict = {
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.9",
             "sec-ch-prefers-color-scheme": random.choice(["light", "dark"]),
             "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
@@ -111,15 +113,18 @@
 
             if "status" in response_json:
                 if response_json["status"] == "ok" and "data" in response_json:
                     if "user" in response_json["data"]:
                         try:
                             data: dict = response_json["data"]["user"]
 
-                            return Profile(
+                            if data is None:
+                                return None
+
+                            profile = Profile(
                                 biography=data["biography"],
                                 biography_links=data["bio_links"],
                                 country_block=data["country_block"],
                                 full_name=data["full_name"],
                                 follower_count=data["edge_followed_by"]["count"],
                                 following_count=data["edge_follow"]["count"],
                                 user_id=data["id"],
@@ -141,35 +146,58 @@
                                 is_embeds_disabled=data["is_embeds_disabled"],
                                 is_verified_by_mv4b=data["is_verified_by_mv4b"],
                                 should_show_category=data["should_show_category"],
                                 should_show_public_contacts=data["should_show_public_contacts"],
                                 show_account_transparency_details=data["show_account_transparency_details"],
                                 total_post_count=data["edge_owner_to_timeline_media"]["count"]
                             )
+
+                            if __session__ is not None:
+                                profile_host = ProfileHost()
+
+                                for key, value in dataclasses.asdict(profile).items():
+                                    setattr(profile_host, key, value)
+
+                                profile_host.blocked_by_viewer = data["blocked_by_viewer"]
+                                profile_host.followed_by_viewer = data["followed_by_viewer"]
+                                profile_host.follows_viewer = data["follows_viewer"]
+                                profile_host.has_blocked_viewer = data["has_blocked_viewer"]
+                                profile_host.has_requested_viewer = data["has_requested_viewer"]
+                                profile_host.is_guardian_of_viewer = data["is_guardian_of_viewer"]
+                                profile_host.is_supervised_by_viewer = data["is_supervised_by_viewer"]
+                                profile_host.requested_by_viewer = data["requested_by_viewer"]
+                                profile_host.mutual_follower_count = data["edge_mutual_followed_by"]["count"]
+
+                                return profile_host
+
+                            return profile
                         except KeyError:
                             raise APIError()
         except JSONDecodeError:
             return None
 
     def get_uid(self, username: str) -> str | None:
         username: str = username.strip().lower().replace(" ", "")
         response: Profile | None = self.profile(username)
 
         if response.user_id is not None:
             return format_uid(response.user_id)
 
-    def get_username(self, uid: str | int) -> str | None:
+    def get_username(self, uid: str | int, __session__: requests.Session | None = None) -> str | None:
         uid = format_uid(uid)
         refresh_csrf_token(self)
         request_headers = {
             "User-Agent": "Instagram 76.0.0.15.395 Android (24/7.0; 640dpi; 1440x2560; samsung; SM-G930F; herolte; samsungexynos8890; en_US; 138226743)"
         }
 
         try:
-            http_response = self.request_session.get(f"https://i.instagram.com/api/v1/users/{uid}/info/", headers=request_headers)
+            session: requests.Session = __session__
+            if __session__ is None: session: requests.Session = self.request_session
+
+            http_response = session.get(f"https://i.instagram.com/api/v1/users/{uid}/info/", headers=request_headers)
             response_json = http_response.json()
 
             if "status" in response_json and response_json["status"] == "ok" and "user" in response_json and "username" in response_json["user"]:
                 return format_username(response_json["user"]["username"])
 
         except JSONDecodeError:
             return None
```

### Comparing `ensta-2.4/ensta/Host.py` & `ensta-2.5/ensta/Host.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,18 +11,19 @@
     update_session,
     format_identifier
 )
 from .lib import (
     SessionError,
     NetworkError,
     IdentifierError,
-    DevelopmentError
+    DevelopmentError,
+    APIError
 )
 from .containers import (FollowedStatus, UnfollowedStatus, FollowPerson)
-from .containers.Profile import Profile
+from .containers.ProfileHost import ProfileHost
 
 USERNAME = 0
 UID = 1
 
 
 class Host:
     request_session: requests.Session = None
@@ -197,15 +198,15 @@
         conversion_success, identifier = self._identifier(identifier, UID)
         if not conversion_success:
             yield None
             return None
 
         # Actual Request
         refresh_csrf_token(self)
-        request_headers = {
+        request_headers: dict = {
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.9",
             "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
             "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
             "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
             "sec-ch-ua-mobile": "?0",
             "sec-ch-ua-platform": "\"Windows\"",
@@ -219,22 +220,22 @@
             "x-ig-app-id": self.insta_app_id,
             "x-ig-www-claim": self.x_ig_www_claim,
             "x-requested-with": "XMLHttpRequest",
             "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=6))}/followers/",
             "Referrer-Policy": "strict-origin-when-cross-origin"
         }
 
-        current_max_id = ""
-        generated_count = 0
+        current_max_id: str = ""
+        generated_count: int = 0
 
         while True:
-            current_max_id_text = ""
+            current_max_id_text: str = ""
 
             if current_max_id != "":
-                current_max_id_text = f"&max_id={current_max_id}"
+                current_max_id_text: str = f"&max_id={current_max_id}"
 
             try:
                 count_text = 35
 
                 if count < 35:
                     count_text = count
 
@@ -248,57 +249,30 @@
                 if response_json["status"] != "ok":
                     yield None
                     return None
 
                 for each_item in response_json["users"]:
                     if generated_count < count or count == 0:
 
-                        prop_has_anonymous_profile_picture = None
-                        prop_user_id = None
-                        prop_username = None
-                        prop_full_name = None
-                        prop_is_private = None
-                        prop_is_verified = None
-                        prop_profile_picture_url = None
-                        prop_is_possible_scammer = None
-
-                        if "has_anonymous_profile_picture" in each_item:
-                            prop_has_anonymous_profile_picture = each_item["has_anonymous_profile_picture"]
-
-                        if "pk" in each_item:
-                            prop_user_id = each_item["pk"]
-
-                        if "username" in each_item:
-                            prop_username = each_item["username"]
-
-                        if "full_name" in each_item:
-                            prop_full_name = each_item["full_name"]
-
-                        if "is_private" in each_item:
-                            prop_is_private = each_item["is_private"]
-
-                        if "is_verified" in each_item:
-                            prop_is_verified = each_item["is_verified"]
-
-                        if "profile_pic_url" in each_item:
-                            prop_profile_picture_url = each_item["profile_pic_url"]
-
-                        if "is_possible_scammer" in each_item:
-                            prop_is_possible_scammer = each_item["is_possible_scammer"]
-
-                        yield FollowPerson(
-                            has_anonymous_profile_picture=prop_has_anonymous_profile_picture,
-                            user_id=prop_user_id,
-                            username=prop_username,
-                            full_name=prop_full_name,
-                            is_private=prop_is_private,
-                            is_verified=prop_is_verified,
-                            profile_picture_url=prop_profile_picture_url,
-                            is_possible_scammer=prop_is_possible_scammer
-                        )
+                        try:
+                            yield FollowPerson(
+                                has_anonymous_profile_picture=each_item["has_anonymous_profile_picture"],
+                                user_id=each_item["pk"],
+                                username=each_item["username"],
+                                full_name=each_item["full_name"],
+                                is_private=each_item["is_private"],
+                                is_verified=each_item["is_verified"],
+                                profile_picture_url=each_item["profile_pic_url"],
+                                badges=each_item["account_badges"],
+                                third_party_downloads_enabled=each_item["third_party_downloads_enabled"],
+                                is_possible_scammer=each_item["is_possible_scammer"]
+                            )
+
+                        except KeyError:
+                            raise APIError()
 
                         generated_count += 1
 
                 if (generated_count < count or count == 0) and "next_max_id" in response_json:
                     current_max_id = response_json["next_max_id"]
                 else:
                     return None
@@ -363,57 +337,28 @@
                 if response_json["status"] != "ok":
                     yield None
                     return None
 
                 for each_item in response_json["users"]:
                     if generated_count < count or count == 0:
 
-                        prop_has_anonymous_profile_picture = None
-                        prop_user_id = None
-                        prop_username = None
-                        prop_full_name = None
-                        prop_is_private = None
-                        prop_is_verified = None
-                        prop_profile_picture_url = None
-                        prop_is_possible_scammer = None
-
-                        if "has_anonymous_profile_picture" in each_item:
-                            prop_has_anonymous_profile_picture = each_item["has_anonymous_profile_picture"]
-
-                        if "pk" in each_item:
-                            prop_user_id = each_item["pk"]
-
-                        if "username" in each_item:
-                            prop_username = each_item["username"]
-
-                        if "full_name" in each_item:
-                            prop_full_name = each_item["full_name"]
-
-                        if "is_private" in each_item:
-                            prop_is_private = each_item["is_private"]
-
-                        if "is_verified" in each_item:
-                            prop_is_verified = each_item["is_verified"]
-
-                        if "profile_pic_url" in each_item:
-                            prop_profile_picture_url = each_item["profile_pic_url"]
-
-                        if "is_possible_scammer" in each_item:
-                            prop_is_possible_scammer = each_item["is_possible_scammer"]
-
-                        yield FollowPerson(
-                            has_anonymous_profile_picture=prop_has_anonymous_profile_picture,
-                            user_id=prop_user_id,
-                            username=prop_username,
-                            full_name=prop_full_name,
-                            is_private=prop_is_private,
-                            is_verified=prop_is_verified,
-                            profile_picture_url=prop_profile_picture_url,
-                            is_possible_scammer=prop_is_possible_scammer
-                        )
+                        try:
+                            yield FollowPerson(
+                                has_anonymous_profile_picture=each_item["has_anonymous_profile_picture"],
+                                user_id=each_item["pk"],
+                                username=each_item["username"],
+                                full_name=each_item["full_name"],
+                                is_private=each_item["is_private"],
+                                is_verified=each_item["is_verified"],
+                                profile_picture_url=each_item["profile_pic_url"],
+                                is_possible_scammer=each_item["is_possible_scammer"]
+                            )
+
+                        except KeyError:
+                            raise APIError()
 
                         generated_count += 1
 
                 if (generated_count < count or count == 0) and "next_max_id" in response_json:
                     current_max_id = response_json["next_max_id"]
                 else:
                     return None
@@ -509,9 +454,12 @@
 
     def switch_to_private_account(self) -> bool:
         return self._set_account_privacy("private")
 
     def switch_to_public_account(self) -> bool:
         return self._set_account_privacy("public")
 
-    def profile(self, username: str) -> Profile | None:
-        return self.guest.profile(username, self.request_session)
+    def profile(self, username: str) -> ProfileHost | None:
+        return self.guest.profile(username, __session__=self.request_session)
+
+    def get_username(self, uid: str | int) -> str | None:
+        return self.guest.get_username(uid, __session__=self.request_session)
```

### Comparing `ensta-2.4/ensta/containers/Profile.py` & `ensta-2.5/ensta/containers/Profile.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=False)
 class Profile:
 
     biography: str = None
     biography_links: list = None
     country_block: bool = None
     full_name: str = None
     follower_count: int = None
```

### Comparing `ensta-2.4/ensta/lib/Commons.py` & `ensta-2.5/ensta/lib/Commons.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 import string
 import requests
 import requests.cookies
 import random
+from requests.cookies import RequestsCookieJar
 from .Exceptions import NetworkError
 
 
 def update_app_id(self) -> None:
     app_id_occurrence_string = "\"APP_ID\":\""
     app_id_first_occurrence = self.homepage_source.index(app_id_occurrence_string)
     app_id_raw_text = self.homepage_source[
                       app_id_first_occurrence + len(app_id_occurrence_string): app_id_first_occurrence + 30]
     self.insta_app_id = app_id_raw_text[: app_id_raw_text.index("\"")]
 
 
 def refresh_csrf_token(self) -> None:
     self.csrf_token = "".join(random.choices(string.ascii_letters + string.digits, k=32))
-    cookie_object = requests.cookies.create_cookie(domain="instagram.com", name="csrftoken", value=self.csrf_token)
-    self.request_session.cookies.set_cookie(cookie_object)
+
+    cookie_jar: RequestsCookieJar = self.request_session.cookies
+    cookies = list(cookie_jar.items())
+    cookie_jar.clear()
+    final_cookies = {}
+
+    for key, value in cookies:
+        final_cookies[key] = value
+
+    final_cookies["csrftoken"] = self.csrf_token
+
+    for key in final_cookies:
+        cookie_jar.set(key, final_cookies[key])
 
 
 def update_session(self) -> None:
     self.request_session = requests.Session()
 
 
 def update_homepage_source(self) -> None:
```

### Comparing `ensta-2.4/ensta/lib/Exceptions.py` & `ensta-2.5/ensta/lib/Exceptions.py`

 * *Files identical despite different names*

### Comparing `ensta-2.4/ensta.egg-info/PKG-INFO` & `ensta-2.5/ensta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 2.4
+Version: 2.5
 Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
 Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.4.tar.gz
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.5.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram-client,instagram,api-wrapper,instagram-scraper,instagram-api,instagram-sdk,instagram-photos,instagram-api-python,instabot,instagram-stories,instagram-bot,instapy,instagram-downloader,instagram-account,instagram-crawler,instagram-private-api,igtv,instagram-automation,reels,instagram-feed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `ensta-2.4/setup.py` & `ensta-2.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ensta",
     packages=["ensta", "ensta.lib", "ensta.containers"],
-    version="2.4",
+    version="2.5",
     license="MIT",
     description="🔥 Fastest & Simplest Python Package For Instagram Automation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Deepak Soni",
     author_email="lonelycube@proton.me",
     url="https://github.com/diezo/ensta",
-    download_url="https://github.com/diezo/ensta/archive/refs/tags/v2.4.tar.gz",
+    download_url="https://github.com/diezo/ensta/archive/refs/tags/v2.5.tar.gz",
     keywords=["instagram-client", "instagram", "api-wrapper", "instagram-scraper", "instagram-api", "instagram-sdk", "instagram-photos", "instagram-api-python", "instabot", "instagram-stories", "instagram-bot", "instapy", "instagram-downloader", "instagram-account", "instagram-crawler", "instagram-private-api", "igtv", "instagram-automation", "reels", "instagram-feed"],
     install_requires=["requests", "selenium"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
```

