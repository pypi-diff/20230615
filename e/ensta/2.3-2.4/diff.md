# Comparing `tmp/ensta-2.3.tar.gz` & `tmp/ensta-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensta-2.3.tar", last modified: Wed Jun 14 16:39:03 2023, max compression
+gzip compressed data, was "ensta-2.4.tar", last modified: Thu Jun 15 10:12:24 2023, max compression
```

## Comparing `ensta-2.3.tar` & `ensta-2.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:39:03.365608 ensta-2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-14 16:38:51.000000 ensta-2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-14 16:39:03.365608 ensta-2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-14 16:38:51.000000 ensta-2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:39:03.361608 ensta-2.3/ensta/
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-14 16:38:51.000000 ensta-2.3/ensta/Authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-06-14 16:38:51.000000 ensta-2.3/ensta/Guest.py
--rw-r--r--   0 runner    (1001) docker     (123)    22025 2023-06-14 16:38:51.000000 ensta-2.3/ensta/Host.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-14 16:38:51.000000 ensta-2.3/ensta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:39:03.365608 ensta-2.3/ensta/containers/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-14 16:38:51.000000 ensta-2.3/ensta/containers/FollowPerson.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-14 16:38:51.000000 ensta-2.3/ensta/containers/FollowedStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-14 16:38:51.000000 ensta-2.3/ensta/containers/Profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-14 16:38:51.000000 ensta-2.3/ensta/containers/UnfollowedStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-14 16:38:51.000000 ensta-2.3/ensta/containers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:39:03.365608 ensta-2.3/ensta/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-14 16:38:51.000000 ensta-2.3/ensta/lib/Commons.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-14 16:38:51.000000 ensta-2.3/ensta/lib/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-14 16:38:51.000000 ensta-2.3/ensta/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:39:03.361608 ensta-2.3/ensta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-14 16:39:03.000000 ensta-2.3/ensta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-14 16:39:03.000000 ensta-2.3/ensta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:39:03.000000 ensta-2.3/ensta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-14 16:39:03.000000 ensta-2.3/ensta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 16:39:03.000000 ensta-2.3/ensta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-14 16:39:03.365608 ensta-2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-14 16:38:51.000000 ensta-2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:12:24.238098 ensta-2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-15 10:12:03.000000 ensta-2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-15 10:12:24.238098 ensta-2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-06-15 10:12:03.000000 ensta-2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:12:24.238098 ensta-2.4/ensta/
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-15 10:12:03.000000 ensta-2.4/ensta/Authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-06-15 10:12:03.000000 ensta-2.4/ensta/Guest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22025 2023-06-15 10:12:03.000000 ensta-2.4/ensta/Host.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-15 10:12:03.000000 ensta-2.4/ensta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:12:24.238098 ensta-2.4/ensta/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-15 10:12:03.000000 ensta-2.4/ensta/containers/FollowPerson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-15 10:12:03.000000 ensta-2.4/ensta/containers/FollowedStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-15 10:12:03.000000 ensta-2.4/ensta/containers/Profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-15 10:12:03.000000 ensta-2.4/ensta/containers/UnfollowedStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-15 10:12:03.000000 ensta-2.4/ensta/containers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:12:24.238098 ensta-2.4/ensta/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-15 10:12:03.000000 ensta-2.4/ensta/lib/Commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-15 10:12:03.000000 ensta-2.4/ensta/lib/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-15 10:12:03.000000 ensta-2.4/ensta/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:12:24.238098 ensta-2.4/ensta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-15 10:12:24.000000 ensta-2.4/ensta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-15 10:12:24.000000 ensta-2.4/ensta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:12:24.000000 ensta-2.4/ensta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 10:12:24.000000 ensta-2.4/ensta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 10:12:24.000000 ensta-2.4/ensta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-15 10:12:24.238098 ensta-2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-15 10:12:03.000000 ensta-2.4/setup.py
```

### Comparing `ensta-2.3/LICENSE.txt` & `ensta-2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ensta-2.3/PKG-INFO` & `ensta-2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 2.3
+Version: 2.4
 Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
 Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.3.tar.gz
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.4.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram-client,instagram,api-wrapper,instagram-scraper,instagram-api,instagram-sdk,instagram-photos,instagram-api-python,instabot,instagram-stories,instagram-bot,instapy,instagram-downloader,instagram-account,instagram-crawler,instagram-private-api,igtv,instagram-automation,reels,instagram-feed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -28,15 +28,15 @@
 This package lets you use Instagram's Internal Web API through simple functions and classes. Ensta uses Instagram's Original Web API to scrape data which makes it a reliable choice over other third-party scrapers. This library mainly focuses on Simplicity & Reliability.
 
 Two type of classes are supported - ***Guest & Host***.
 
 [<img style="margin-top: 10px" src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="160"/>](https://buymeacoffee.com/diezo)
 
 ## 📢 Announcement
-Users can now log in through their **Username** and **Password** to generate SessionId!
+Users can now log in through their **Username** and **Password** to generate SessionId! [See this](https://github.com/diezo/ensta#:~:text=NewSessionID(%22username%22%2C%20%22password%22))
 
 ## Installation
 To install this package using [Python's PIP](https://pypi.org/project/pip/), run this command in a terminal window:
 ```shell
 $ pip install ensta
 ```
```

### Comparing `ensta-2.3/README.md` & `ensta-2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 This package lets you use Instagram's Internal Web API through simple functions and classes. Ensta uses Instagram's Original Web API to scrape data which makes it a reliable choice over other third-party scrapers. This library mainly focuses on Simplicity & Reliability.
 
 Two type of classes are supported - ***Guest & Host***.
 
 [<img style="margin-top: 10px" src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="160"/>](https://buymeacoffee.com/diezo)
 
 ## 📢 Announcement
-Users can now log in through their **Username** and **Password** to generate SessionId!
+Users can now log in through their **Username** and **Password** to generate SessionId! [See this](https://github.com/diezo/ensta#:~:text=NewSessionID(%22username%22%2C%20%22password%22))
 
 ## Installation
 To install this package using [Python's PIP](https://pypi.org/project/pip/), run this command in a terminal window:
 ```shell
 $ pip install ensta
 ```
```

### Comparing `ensta-2.3/ensta/Authentication.py` & `ensta-2.4/ensta/Authentication.py`

 * *Files identical despite different names*

### Comparing `ensta-2.3/ensta/Host.py` & `ensta-2.4/ensta/Host.py`

 * *Files identical despite different names*

### Comparing `ensta-2.3/ensta/containers/Profile.py` & `ensta-2.4/ensta/containers/Profile.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 from dataclasses import dataclass
 
 
 @dataclass(frozen=True)
 class Profile:
 
     biography: str = None
+    biography_links: list = None
     country_block: bool = None
     full_name: str = None
     follower_count: int = None
     following_count: int = None
     user_id: str = None
     is_business_account: bool = None
     is_professional_account: bool = None
     is_supervision_enabled: bool = None
     is_joined_recently: bool = None
     is_private: bool = None
     is_verified: bool = None
     profile_picture_url: str = None
     profile_picture_url_hd: str = None
-    pronouns: list[str] = None
+    pronouns: list[str] = None,
+    has_ar_effects: bool = None,
+    has_clips: bool = None,
+    has_guides: bool = None,
+    has_channel: bool = None,
+    highlight_count: int = None,
+    hide_like_and_view_counts: bool = None,
+    is_embeds_disabled: bool = None,
+    is_verified_by_mv4b: bool = None,
+    should_show_category: bool = None,
+    should_show_public_contacts: bool = None,
+    show_account_transparency_details: bool = None,
+    total_post_count: int = None
```

### Comparing `ensta-2.3/ensta/lib/Commons.py` & `ensta-2.4/ensta/lib/Commons.py`

 * *Files identical despite different names*

### Comparing `ensta-2.3/ensta/lib/Exceptions.py` & `ensta-2.4/ensta/lib/Exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,7 +28,13 @@
         super().__init__(message)
 
 
 class ChallengeError(Exception):
 
     def __init__(self, message):
         super().__init__(message)
+
+
+class APIError(Exception):
+
+    def __init__(self):
+        super().__init__("Looks like Instagram has made changes to the API Response. Please raise this as an issue on GitHub.")
```

### Comparing `ensta-2.3/ensta.egg-info/PKG-INFO` & `ensta-2.4/ensta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 2.3
+Version: 2.4
 Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
 Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.3.tar.gz
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.4.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram-client,instagram,api-wrapper,instagram-scraper,instagram-api,instagram-sdk,instagram-photos,instagram-api-python,instabot,instagram-stories,instagram-bot,instapy,instagram-downloader,instagram-account,instagram-crawler,instagram-private-api,igtv,instagram-automation,reels,instagram-feed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -28,15 +28,15 @@
 This package lets you use Instagram's Internal Web API through simple functions and classes. Ensta uses Instagram's Original Web API to scrape data which makes it a reliable choice over other third-party scrapers. This library mainly focuses on Simplicity & Reliability.
 
 Two type of classes are supported - ***Guest & Host***.
 
 [<img style="margin-top: 10px" src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-1.svg" width="160"/>](https://buymeacoffee.com/diezo)
 
 ## 📢 Announcement
-Users can now log in through their **Username** and **Password** to generate SessionId!
+Users can now log in through their **Username** and **Password** to generate SessionId! [See this](https://github.com/diezo/ensta#:~:text=NewSessionID(%22username%22%2C%20%22password%22))
 
 ## Installation
 To install this package using [Python's PIP](https://pypi.org/project/pip/), run this command in a terminal window:
 ```shell
 $ pip install ensta
 ```
```

### Comparing `ensta-2.3/setup.py` & `ensta-2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ensta",
     packages=["ensta", "ensta.lib", "ensta.containers"],
-    version="2.3",
+    version="2.4",
     license="MIT",
     description="🔥 Fastest & Simplest Python Package For Instagram Automation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Deepak Soni",
     author_email="lonelycube@proton.me",
     url="https://github.com/diezo/ensta",
-    download_url="https://github.com/diezo/ensta/archive/refs/tags/v2.3.tar.gz",
+    download_url="https://github.com/diezo/ensta/archive/refs/tags/v2.4.tar.gz",
     keywords=["instagram-client", "instagram", "api-wrapper", "instagram-scraper", "instagram-api", "instagram-sdk", "instagram-photos", "instagram-api-python", "instabot", "instagram-stories", "instagram-bot", "instapy", "instagram-downloader", "instagram-account", "instagram-crawler", "instagram-private-api", "igtv", "instagram-automation", "reels", "instagram-feed"],
     install_requires=["requests", "selenium"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
```

