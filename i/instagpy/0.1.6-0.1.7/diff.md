# Comparing `tmp/instagpy-0.1.6.tar.gz` & `tmp/instagpy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagpy-0.1.6.tar", last modified: Wed Jun 14 12:10:26 2023, max compression
+gzip compressed data, was "instagpy-0.1.7.tar", last modified: Thu Jun 15 06:13:21 2023, max compression
```

## Comparing `instagpy-0.1.6.tar` & `instagpy-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 12:10:26.445726 instagpy-0.1.6/
--rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 instagpy-0.1.6/LICENSE
--rw-rw-rw-   0        0        0       21 2023-05-20 05:58:51.000000 instagpy-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     3318 2023-06-14 12:10:26.445726 instagpy-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2256 2023-05-22 12:22:05.000000 instagpy-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 12:10:26.427076 instagpy-0.1.6/instagpy/
--rw-rw-rw-   0        0        0       32 2023-06-07 10:27:42.000000 instagpy-0.1.6/instagpy/__init__.py
--rw-rw-rw-   0        0        0      685 2023-06-14 12:05:31.000000 instagpy-0.1.6/instagpy/config.py
--rw-rw-rw-   0        0        0    22022 2023-06-14 12:04:32.000000 instagpy-0.1.6/instagpy/instagpy.py
--rw-rw-rw-   0        0        0     2086 2023-06-07 10:41:45.000000 instagpy-0.1.6/instagpy/path.py
--rw-rw-rw-   0        0        0     1332 2023-06-14 10:38:27.000000 instagpy-0.1.6/instagpy/request_util.py
--rw-rw-rw-   0        0        0     2729 2023-06-07 14:13:48.000000 instagpy-0.1.6/instagpy/session_util.py
--rw-rw-rw-   0        0        0     2914 2023-06-14 09:37:23.000000 instagpy-0.1.6/instagpy/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-14 12:10:26.445726 instagpy-0.1.6/instagpy.egg-info/
--rw-rw-rw-   0        0        0     3318 2023-06-14 12:10:26.000000 instagpy-0.1.6/instagpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-06-14 12:10:26.000000 instagpy-0.1.6/instagpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 12:10:26.000000 instagpy-0.1.6/instagpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-14 12:10:26.000000 instagpy-0.1.6/instagpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 12:10:26.000000 instagpy-0.1.6/instagpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 12:10:26.445726 instagpy-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1486 2023-06-14 12:09:54.000000 instagpy-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:13:21.587460 instagpy-0.1.7/
+-rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 instagpy-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0       21 2023-05-20 05:58:51.000000 instagpy-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     3318 2023-06-15 06:13:21.587460 instagpy-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2256 2023-05-22 12:22:05.000000 instagpy-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 06:13:21.571818 instagpy-0.1.7/instagpy/
+-rw-rw-rw-   0        0        0       32 2023-06-07 10:27:42.000000 instagpy-0.1.7/instagpy/__init__.py
+-rw-rw-rw-   0        0        0      685 2023-06-15 05:59:08.000000 instagpy-0.1.7/instagpy/config.py
+-rw-rw-rw-   0        0        0    24200 2023-06-15 06:06:38.000000 instagpy-0.1.7/instagpy/instagpy.py
+-rw-rw-rw-   0        0        0     2140 2023-06-14 13:31:23.000000 instagpy-0.1.7/instagpy/path.py
+-rw-rw-rw-   0        0        0     1332 2023-06-15 05:49:06.000000 instagpy-0.1.7/instagpy/request_util.py
+-rw-rw-rw-   0        0        0     2729 2023-06-07 14:13:48.000000 instagpy-0.1.7/instagpy/session_util.py
+-rw-rw-rw-   0        0        0     2914 2023-06-14 09:37:23.000000 instagpy-0.1.7/instagpy/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:13:21.587460 instagpy-0.1.7/instagpy.egg-info/
+-rw-rw-rw-   0        0        0     3318 2023-06-15 06:13:21.000000 instagpy-0.1.7/instagpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-06-15 06:13:21.000000 instagpy-0.1.7/instagpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 06:13:21.000000 instagpy-0.1.7/instagpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-15 06:13:21.000000 instagpy-0.1.7/instagpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 06:13:21.000000 instagpy-0.1.7/instagpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 06:13:21.587460 instagpy-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1486 2023-06-15 06:12:37.000000 instagpy-0.1.7/setup.py
```

### Comparing `instagpy-0.1.6/LICENSE` & `instagpy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.6/PKG-INFO` & `instagpy-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagpy
-Version: 0.1.6
+Version: 0.1.7
 Summary: InstaGPy is an Instagram Unofficial API to extract data from Instargam Profiles. Scrape data from user's profile like username, userid, bio, email, phone, followers/followings list, profile media, account_type, etc.
 Home-page: https://github.com/iSarabjitDhiman/InstaGPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: instagpy,instagram scraper,instagram email scraper,insta data extraction,instagram api,instagram python
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: instagpy Version: 0.1.6 Summary: InstaGPy is an
+Metadata-Version: 2.1 Name: instagpy Version: 0.1.7 Summary: InstaGPy is an
 Instagram Unofficial API to extract data from Instargam Profiles. Scrape data
 from user's profile like username, userid, bio, email, phone, followers/
 followings list, profile media, account_type, etc. Home-page: https://
 github.com/iSarabjitDhiman/InstaGPy Author: Sarabjit Dhiman Author-email:
 hello@sarabjitdhiman.com License: MIT Keywords: instagpy,instagram
 scraper,instagram email scraper,insta data extraction,instagram api,instagram
 python Classifier: Development Status :: 3 - Alpha Classifier: Intended
```

### Comparing `instagpy-0.1.6/README.md` & `instagpy-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.6/instagpy/config.py` & `instagpy-0.1.7/instagpy/config.py`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.6/instagpy/instagpy.py` & `instagpy-0.1.7/instagpy/instagpy.py`

 * *Files 10% similar despite different names*

```diff
@@ -120,15 +120,15 @@
                 change_session = True
         if change_session:
             if not self.session_ids_container:
                 self.session_ids_container = self.session_ids.copy()
             session_id = self.session_ids_container.pop()
             return self.generate_session(session_id=session_id)
 
-    def generate_query(self, query=None, count=None, user_id=None, end_cursor=None, search_surface=None, shortcode=None, is_graphql=False):
+    def generate_query(self, query=None, count=None, user_id=None, end_cursor=None, search_surface=None, shortcode=None, hashtag=None, is_graphql=False):
         """Generates query paramters for instagram api requests.
 
         Args:
             query (str, optional): Query endpoint. Defaults to None.
             count (int, optional): Number of results per request to extract from Instagram Database. Defaults to None.
             user_id (int, optional): User Profile ID. Defaults to None.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
@@ -147,14 +147,16 @@
                 data['id'] = user_id
             if count:
                 data['first'] = count
             if end_cursor:
                 data['after'] = end_cursor
             if shortcode:
                 data['shortcode'] = shortcode
+            if hashtag:
+                data['tag_name'] = hashtag
 
             params["variables"] = json.dumps(data)
         else:
             if count:
                 params["count"] = count
             if search_surface is not None:
                 params["search_surface"] = search_surface
@@ -485,10 +487,59 @@
         response = make_request(path.ABOUT_USER_URL, method='POST', data=data,
                                 session=self.session, max_retries=self.max_retries)
         if print_formatted:
             return utils.format_about_data(response)
         self.shuffle_session()
         return response
 
+    def get_hashtag_posts(self, hashtag=None, end_cursor=None, max=None):
+        """Get media posts from hashtags.
+
+        Args:
+            hashtag (str): Hashtag that you want to extract data from. Accepts both formats i.e. hashtag or #hashtag. Defaults to None.
+            end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
+            max (int, optional): Number of results per request to extract from Instagram Database. Defaults to None.
+
+        Returns:
+            dict: Hashtag posts data.
+        """
+        if hashtag is None:
+            raise Exception("No hashtag was given.")
+        if not self.logged_in():
+            self.login()
+        hashtag = hashtag.lstrip("#")
+        hashtag_posts = []
+        url = path.GRAPHQL_URL
+        max_data = 50
+        print(f'Started at : {utils.format_datetime(time.time())}\n')
+        while True:
+            query_params = self.generate_query(
+                query=path.HASHTAG_QUERY, hashtag=hashtag, count=max_data, end_cursor=end_cursor, is_graphql=True)
+
+            try:
+                response = make_request(
+                    url, params=query_params, session=self.session, max_retries=self.max_retries)
+                data = response['data']['hashtag']['edge_hashtag_to_media']
+                has_next_page = data['page_info']['has_next_page']
+                end_cursor = data['page_info']['end_cursor']
+                count = data['count']
+                data = data['edges']
+
+                hashtag_posts.extend(data)
+                print(
+                    f"#{hashtag} : {len(hashtag_posts)} / {count}", end="\r")
+                if not has_next_page or (max is not None and len(hashtag_posts) >= max):
+                    return hashtag_posts
+
+                self.shuffle_session()
+
+            except ConnectionError as error:
+                print(error)
+                continue
+
+            except Exception as error:
+                print(error)
+                return hashtag_posts
+
 
 if __name__ == "__main__":
     pass
```

### Comparing `instagpy-0.1.6/instagpy/path.py` & `instagpy-0.1.7/instagpy/path.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,9 +31,11 @@
 # followers_list_query & following_list_query - both return max 50 results in a single request but work with blue tick verified accounts.
 FOLLOWERS_LIST_QUERY = "7dd9a7e2160524fd85f50317462cff9f"
 FOLLOWING_LIST_QUERY = "c56ee0ae1f89cdbd1c89e2bc6b8f3d18"
 
 ABOUT_USER_URL = "https://i.instagram.com/api/v1/bloks/apps/com.instagram.interactions.about_this_account/"
 ABOUT_USER_QUERY = "8ca96ca267e30c02cf90888d91eeff09627f0e3fd2bd9df472278c9a6c022cbb"
 
+HASHTAG_QUERY = "9b498c08113f1e09617a1703c22b2f32"
+
 if __name__ == '__main__':
     pass
```

### Comparing `instagpy-0.1.6/instagpy/request_util.py` & `instagpy-0.1.7/instagpy/request_util.py`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.6/instagpy/session_util.py` & `instagpy-0.1.7/instagpy/session_util.py`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.6/instagpy/utils.py` & `instagpy-0.1.7/instagpy/utils.py`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.6/instagpy.egg-info/PKG-INFO` & `instagpy-0.1.7/instagpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagpy
-Version: 0.1.6
+Version: 0.1.7
 Summary: InstaGPy is an Instagram Unofficial API to extract data from Instargam Profiles. Scrape data from user's profile like username, userid, bio, email, phone, followers/followings list, profile media, account_type, etc.
 Home-page: https://github.com/iSarabjitDhiman/InstaGPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: instagpy,instagram scraper,instagram email scraper,insta data extraction,instagram api,instagram python
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: instagpy Version: 0.1.6 Summary: InstaGPy is an
+Metadata-Version: 2.1 Name: instagpy Version: 0.1.7 Summary: InstaGPy is an
 Instagram Unofficial API to extract data from Instargam Profiles. Scrape data
 from user's profile like username, userid, bio, email, phone, followers/
 followings list, profile media, account_type, etc. Home-page: https://
 github.com/iSarabjitDhiman/InstaGPy Author: Sarabjit Dhiman Author-email:
 hello@sarabjitdhiman.com License: MIT Keywords: instagpy,instagram
 scraper,instagram email scraper,insta data extraction,instagram api,instagram
 python Classifier: Development Status :: 3 - Alpha Classifier: Intended
```

### Comparing `instagpy-0.1.6/setup.py` & `instagpy-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.1.6"
+VERSION = "0.1.7"
 SHORT_DESCRIPTION = "InstaGPy is an Instagram Unofficial API to extract data from Instargam Profiles. Scrape data from user's profile like username, userid, bio, email, phone, followers/followings list, profile media, account_type, etc."
 
 with open("requirements.txt") as file:
     dependencies = file.read().splitlines()
 with open("README.md", "r") as file:
     DESCRIPTION = file.read()
```

