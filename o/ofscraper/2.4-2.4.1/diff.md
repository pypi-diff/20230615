# Comparing `tmp/ofscraper-2.4.tar.gz` & `tmp/ofscraper-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-2.4.tar", max compression
+gzip compressed data, was "ofscraper-2.4.1.tar", max compression
```

## Comparing `ofscraper-2.4.tar` & `ofscraper-2.4.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1067 2023-06-15 09:21:04.491317 ofscraper-2.4/LICENSE
--rw-r--r--   0        0        0     5201 2023-06-15 09:21:04.491317 ofscraper-2.4/README.md
--rw-r--r--   0        0        0      607 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/__init__.py
--rw-r--r--   0        0        0      999 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/__version__.py
--rw-r--r--   0        0        0        1 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/__init__.py
--rw-r--r--   0        0        0     7060 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/archive.py
--rw-r--r--   0        0        0     3944 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1067 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/init.py
--rw-r--r--   0        0        0     2343 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/me.py
--rw-r--r--   0        0        0     6515 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/messages.py
--rw-r--r--   0        0        0     8462 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/paid.py
--rw-r--r--   0        0        0     4570 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/pinned.py
--rw-r--r--   0        0        0    11157 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/posts.py
--rw-r--r--   0        0        0     3593 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/profile.py
--rw-r--r--   0        0        0     3047 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     7707 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/timeline.py
--rw-r--r--   0        0        0    30895 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/commands/check.py
--rwxr-xr-x   0        0        0    22495 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0     5769 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/db/__init__.py
--rw-r--r--   0        0        0     8581 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3253 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     4121 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/interaction/like.py
--rw-r--r--   0        0        0     1364 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/prompt model.md
--rw-r--r--   0        0        0      463 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0     6754 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0    26253 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0      679 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/start.py
--rw-r--r--   0        0        0        1 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0     9037 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/utils/args.py
--rw-r--r--   0        0        0     9035 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/utils/auth.py
--rw-r--r--   0        0        0     6158 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0    10680 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/utils/config.py
--rw-r--r--   0        0        0      257 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/console.py
--rw-r--r--   0        0        0      993 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    19571 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     2865 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     3137 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/filters.py
--rw-r--r--   0        0        0     5622 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/logger.py
--rw-r--r--   0        0        0     7649 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     3073 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      397 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/semaphoreDelayed.py
--rw-r--r--   0        0        0     1358 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/separate.py
--rw-r--r--   0        0        0      554 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/stdout.py
--rw-r--r--   0        0        0     6092 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/userselector.py
--rw-r--r--   0        0        0     1518 2023-06-15 09:21:45.754020 ofscraper-2.4/pyproject.toml
--rw-r--r--   0        0        0     6605 1970-01-01 00:00:00.000000 ofscraper-2.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-15 14:23:11.103686 ofscraper-2.4.1/LICENSE
+-rw-r--r--   0        0        0     5201 2023-06-15 14:23:11.103686 ofscraper-2.4.1/README.md
+-rw-r--r--   0        0        0      607 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/__init__.py
+-rw-r--r--   0        0        0      999 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/__version__.py
+-rw-r--r--   0        0        0        1 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/__init__.py
+-rw-r--r--   0        0        0     7066 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/archive.py
+-rw-r--r--   0        0        0     3944 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1067 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/init.py
+-rw-r--r--   0        0        0     2343 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/me.py
+-rw-r--r--   0        0        0     6515 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     8462 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     4576 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0    11157 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/posts.py
+-rw-r--r--   0        0        0     3593 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     3047 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     7713 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0    31071 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/commands/check.py
+-rwxr-xr-x   0        0        0    22507 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0     5769 2023-06-15 14:23:11.111686 ofscraper-2.4.1/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0     8581 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3253 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     4121 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0     1364 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/prompt model.md
+-rw-r--r--   0        0        0      463 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0     6754 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0    26253 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0      679 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/start.py
+-rw-r--r--   0        0        0        1 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0     9162 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/args.py
+-rw-r--r--   0        0        0     9035 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0     6158 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0    10680 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      257 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      993 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    19571 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     2865 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     3137 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0     5622 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0     7654 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     3073 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      397 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/semaphoreDelayed.py
+-rw-r--r--   0        0        0     1358 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0      554 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/stdout.py
+-rw-r--r--   0        0        0     6042 2023-06-15 14:23:11.115687 ofscraper-2.4.1/ofscraper/utils/userselector.py
+-rw-r--r--   0        0        0     1520 2023-06-15 14:23:54.123770 ofscraper-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6607 1970-01-01 00:00:00.000000 ofscraper-2.4.1/PKG-INFO
```

### Comparing `ofscraper-2.4/LICENSE` & `ofscraper-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/README.md` & `ofscraper-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/__init__.py` & `ofscraper-2.4.1/ofscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/__version__.py` & `ofscraper-2.4.1/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/api/archive.py` & `ofscraper-2.4.1/ofscraper/api/archive.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             #use the previous split for timesamp
             tasks.append(asyncio.create_task(scrape_archived_posts(headers,model_id,job_progress,required_ids=set(splitArrays[0]),timestamp= splitArrays[0][0]-20000)))
             [tasks.append(asyncio.create_task(scrape_archived_posts(headers,model_id,job_progress,required_ids=set(splitArrays[i]),timestamp=splitArrays[i-1][-1])))
             for i in range(1,len(splitArrays)-1)]
             # keeping grabbing until nothign left
             tasks.append(asyncio.create_task(scrape_archived_posts(headers,model_id,job_progress,timestamp=splitArrays[-2][-1])))
         else:
-            tasks.append(asyncio.create_task(scrape_archived_posts(headers,model_id,job_progress,timestamp=args_.getargs().float_timestamp if args_.getargs().after else None)))
+            tasks.append(asyncio.create_task(scrape_archived_posts(headers,model_id,job_progress,timestamp=args_.getargs().after.float_timestamp if args_.getargs().after else None)))
     
 
         page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True)
         while len(tasks)!=0:
             for coro in asyncio.as_completed(tasks):
                 result=await coro or []
                 page_count=page_count+1
```

### Comparing `ofscraper-2.4/ofscraper/api/highlights.py` & `ofscraper-2.4.1/ofscraper/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/api/init.py` & `ofscraper-2.4.1/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/api/me.py` & `ofscraper-2.4.1/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/api/messages.py` & `ofscraper-2.4.1/ofscraper/api/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/api/paid.py` & `ofscraper-2.4.1/ofscraper/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/api/pinned.py` & `ofscraper-2.4.1/ofscraper/api/pinned.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     global tasks
     tasks=[]
     min_posts=50
     responseArray=[]
     page_count=0
     with Live(progress_group, refresh_per_second=5,console=console.shared_console): 
 
-        tasks.append(asyncio.create_task(scrape_pinned_posts(headers,model_id,job_progress,timestamp=args_.getargs().float_timestamp if args_.getargs().after else None)))
+        tasks.append(asyncio.create_task(scrape_pinned_posts(headers,model_id,job_progress,timestamp=args_.getargs().after.float_timestamp if args_.getargs().after else None)))
     
 
         page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True)
         while len(tasks)!=0:
             for coro in asyncio.as_completed(tasks):
                 result=await coro or []
                 page_count=page_count+1
```

### Comparing `ofscraper-2.4/ofscraper/api/posts.py` & `ofscraper-2.4.1/ofscraper/api/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/api/profile.py` & `ofscraper-2.4.1/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/api/subscriptions.py` & `ofscraper-2.4.1/ofscraper/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/api/timeline.py` & `ofscraper-2.4.1/ofscraper/api/timeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
             #use the previous split for timesamp
             tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,required_ids=set(splitArrays[0]),timestamp= splitArrays[0][0]-20000)))
             [tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,required_ids=set(splitArrays[i]),timestamp=splitArrays[i-1][-1])))
             for i in range(1,len(splitArrays)-1)]
             # keeping grabbing until nothign left
             tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,timestamp=splitArrays[-2][-1])))
         else:
-            tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,timestamp=args_.getargs().float_timestamp if args_.getargs().after else None)))
+            tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,timestamp=args_.getargs().after.float_timestamp if args_.getargs().after else None)))
     
 
         page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True)
         while len(tasks)!=0:
             for coro in asyncio.as_completed(tasks):
                 result=await coro or []
                 page_count=page_count+1
```

### Comparing `ofscraper-2.4/ofscraper/commands/check.py` & `ofscraper-2.4.1/ofscraper/commands/check.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,43 +26,48 @@
 
 from diskcache import Cache
 from ..utils.paths import getcachepath
 cache = Cache(getcachepath())
 
 log = logging.getLogger(__package__)
 args = args_.getargs()
-ROW_NAMES = "Number", "UserName", "Downloaded", "Unlocked", "Times_detected", "Length", "Mediatype", "Post_Date", "Post_Media_Count", "Responsetype", "Price", "Post_ID", "Media_ID", "Text"
+ROW_NAMES = "Number", "UserName", "Downloaded", "Unlocked", "Times_Detected", "Length", "Mediatype", "Post_Date", "Post_Media_Count", "Responsetype", "Price", "Post_ID", "Media_ID", "Text"
 ROWS = []
 
 
 def post_checker():
     headers = auth.make_headers(auth.read_auth())
     user_dict = {}
     client = httpx.Client(http2=True, headers=headers)
     links = list(url_helper())
-    for ele in list(filter(lambda x: re.search("onlyfans.com/[a-z_]+$", x), links)):
+    for ele in links:
         name_match = re.search("/([a-z_]+$)", ele)
         if name_match:
             user_name = name_match.group(1)
             log.info(f"Getting Full Timeline for {user_name}")
             model_id = profile.get_id(headers, user_name)
-            oldtimeline = cache.get(f"timeline_check_{model_id}", default=[])
-            if len(oldtimeline) > 0 and not args.force:
-                user_dict[user_name] = oldtimeline
-            elif not user_dict.get(user_name):
-                user_dict[user_name] = {}
-                user_dict[user_name] = user_dict[user_name] or []
-                user_dict[user_name].extend(asyncio.run(
-                    timeline.get_timeline_post(headers, model_id)))
-                user_dict[user_name].extend(asyncio.run(
-                    pinned.get_pinned_post(headers, model_id)))
-                user_dict[user_name].extend(asyncio.run(
-                    archive.get_archived_post(headers, model_id)))
-                cache.set(
-                    f"timeline_check_{model_id}", user_dict[user_name], expire=constants.CHECK_EXPIRY)
+        name_match = re.search("^[a-z]+$", ele)
+        if name_match:
+            user_name = name_match.group(0)
+            model_id = profile.get_id(headers, user_name)
+
+        oldtimeline = cache.get(f"timeline_check_{model_id}", default=[])
+        if len(oldtimeline) > 0 and not args.force:
+            user_dict[user_name] = oldtimeline
+        elif not user_dict.get(user_name):
+            user_dict[user_name] = {}
+            user_dict[user_name] = user_dict[user_name] or []
+            user_dict[user_name].extend(asyncio.run(
+                timeline.get_timeline_post(headers, model_id)))
+            user_dict[user_name].extend(asyncio.run(
+                pinned.get_pinned_post(headers, model_id)))
+            user_dict[user_name].extend(asyncio.run(
+                archive.get_archived_post(headers, model_id)))
+            cache.set(
+                f"timeline_check_{model_id}", user_dict[user_name], expire=constants.CHECK_EXPIRY)
 
     # individual links
     for ele in list(filter(lambda x: re.search("onlyfans.com/[0-9]+/[a-z_]+$", x), links)):
         name_match = re.search("/([a-z]+$)", ele)
         num_match = re.search("/([0-9]+)", ele)
         if name_match and num_match:
             model_id = num_match.group(1)
@@ -90,30 +95,34 @@
     ROWS=[]
     for item in links:
         num_match = re.search("/([0-9]+)", item)
         headers = auth.make_headers(auth.read_auth())
         if num_match:
             model_id = num_match.group(1)
             user_name = profile.scrape_profile(headers, model_id)['username']
-            user_dict[user_name] = user_dict.get(user_name, [])
-            log.info(f"Getting Messages for {user_name}")
-            messages = None
-            oldmessages = cache.get(f"message_check_{model_id}", default=[])
+        name_match = re.search("^[a-z]+$", item)
+        if name_match:
+            user_name = name_match.group(0)
+            model_id = profile.get_id(headers, user_name)     
+        user_dict[user_name] = user_dict.get(user_name, [])
+        log.info(f"Getting Messages for {user_name}")
+        messages = None
+        oldmessages = cache.get(f"message_check_{model_id}", default=[])
 
-            
-            if len(oldmessages) > 0 and not args.force:
-                messages = oldmessages
-            else:
-                messages = asyncio.run(
-                    messages_.get_messages(headers,  model_id))
-                cache.set(f"message_check_{model_id}",
-                          messages, expire=constants.CHECK_EXPIRY)
-            downloaded = get_downloaded(user_name, model_id)
-            media = get_all_found_media(user_name, messages)
-            ROWS.extend(row_gather(media, downloaded, user_name))
+        
+        if len(oldmessages) > 0 and not args.force:
+            messages = oldmessages
+        else:
+            messages = asyncio.run(
+                messages_.get_messages(headers,  model_id))
+            cache.set(f"message_check_{model_id}",
+                        messages, expire=constants.CHECK_EXPIRY)
+        downloaded = get_downloaded(user_name, model_id)
+        media = get_all_found_media(user_name, messages)
+        ROWS.extend(row_gather(media, downloaded, user_name))
 
     app_run_helper(ROWS)
 
 
 
 def purchase_checker():
     user_dict = {}
@@ -687,15 +696,15 @@
         #     self.make_table()
 
     def compose(self) -> ComposeResult:
         with VerticalScroll():
             with Horizontal():
                 for ele in ["Text"]:
                     yield StringField(ele)
-                for ele in ["Times_detected"]:
+                for ele in ["Times_Detected"]:
                     yield NumField(ele)
                 for ele in ["Media_ID", "Post_ID", "Post_Media_Count"]:
                     yield NumField(ele)
             with Horizontal():
                 for ele in ["Price"]:
                     yield PriceField(ele)
                 for ele in ["Post_Date"]:
```

### Comparing `ofscraper-2.4/ofscraper/commands/scraper.py` & `ofscraper-2.4.1/ofscraper/commands/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,51 +309,51 @@
         normal_post_process()
            
 def process_post_user_first():
      with scrape_context_manager():
         profiles.print_current_profile()
         headers = auth.make_headers(auth.read_auth())
         init.print_sign_status(headers)
-        userdata=userselector.getselected_usernames()
-        length=len(userdata)
         if args.users_first:
             output=[]
+            userdata=userselector.getselected_usernames() if "None" not in args.posts else []
+            length=len(userdata)
             for count,ele in enumerate(userdata):
                 log.debug(f"getting content for {count+1}/{length} model")
                 if args.posts:
                     log.info(f"Getting {','.join(args.posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
                 try:
                     model_id = profile.get_id(headers, ele["name"])
                     operations.create_tables(model_id,ele['name'])
                     operations.write_profile_table(model_id,ele['name'])
                     output.extend(process_areas(headers, ele, model_id)) 
-                    if args.scrape_paid:
-                        output.extend(process_all_paid())
                 except Exception as e:
                     log.traceback(f"failed with exception: {e}")
                     log.traceback(traceback.format_exc())               
-                user_dict={}
-                [user_dict.update({ele.post.model_id:user_dict.get(ele.post.model_id,[])+[ele]}) for ele in output]
-                for value in user_dict.values():
-                    model_id =value[0].post.model_id
-                    username=value[0].post.username
-                    operations.create_tables(model_id,username)
-                    operations.write_profile_table(model_id,username)
-                    asyncio.run(download.process_dicts(
-                    username,
-                    model_id,
-                    value,
-                    forced=args.dupe,
-                    ))  
+            if args.scrape_paid:
+                output.extend(process_all_paid())
+            user_dict={}
+            [user_dict.update({ele.post.model_id:user_dict.get(ele.post.model_id,[])+[ele]}) for ele in output]
+            for value in user_dict.values():
+                model_id =value[0].post.model_id
+                username=value[0].post.username
+                operations.create_tables(model_id,username)
+                operations.write_profile_table(model_id,username)
+                asyncio.run(download.process_dicts(
+                username,
+                model_id,
+                value,
+                forced=args.dupe,
+                ))  
 def normal_post_process():
     with scrape_context_manager():
         profiles.print_current_profile()
         headers = auth.make_headers(auth.read_auth())
         init.print_sign_status(headers)
-        userdata=userselector.getselected_usernames()
+        userdata=userselector.getselected_usernames() if "None" not in args.posts else []
         length=len(userdata)
         for count,ele in enumerate(userdata):
             log.debug(f"Getting content+downloading {count+1}/{length} model")
             if args.posts:
                 log.info(f"Getting {','.join(args.posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
             try:
                 model_id = profile.get_id(headers, ele["name"])
```

### Comparing `ofscraper-2.4/ofscraper/constants.py` & `ofscraper-2.4.1/ofscraper/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/db/operations.py` & `ofscraper-2.4.1/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/db/queries.py` & `ofscraper-2.4.1/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/interaction/like.py` & `ofscraper-2.4.1/ofscraper/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/prompt model.md` & `ofscraper-2.4.1/ofscraper/prompt model.md`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/prompts/prompt_validators.py` & `ofscraper-2.4.1/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/prompts/prompts.py` & `ofscraper-2.4.1/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/start.py` & `ofscraper-2.4.1/ofscraper/start.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/utils/args.py` & `ofscraper-2.4.1/ofscraper/utils/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,16 @@
     message_check.add_argument("-f","--file",
     help = 'Check if media is in library via file',default=None,required=False,type = check_filehelper
     )
     
 
     message_check.add_argument("-u","--url",
     help = 'link to conversation',type = check_strhelper,action="extend")
+    message_check.add_argument("-un","--username",
+    help = 'link to conversation',type = check_strhelper,action="extend")
 
     paid_check=subparser.add_parser("paid_check",help="Parse Purchases sent from a user\nCache last for 24 hours")
     paid_check.add_argument(
         '-fo', '--force', help = 'force retrival of new posts info from API', default=False,action="store_true"
     )
     paid_check.add_argument("-f","--file",
     help = 'Check if media is in library via file',default=None,required=False,type = check_filehelper
```

### Comparing `ofscraper-2.4/ofscraper/utils/auth.py` & `ofscraper-2.4.1/ofscraper/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/utils/binaries.py` & `ofscraper-2.4.1/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/utils/config.py` & `ofscraper-2.4.1/ofscraper/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/utils/dates.py` & `ofscraper-2.4.1/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/utils/download.py` & `ofscraper-2.4.1/ofscraper/utils/download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/utils/encoding.py` & `ofscraper-2.4.1/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/utils/exit.py` & `ofscraper-2.4.1/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/utils/filters.py` & `ofscraper-2.4.1/ofscraper/utils/filters.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/utils/logger.py` & `ofscraper-2.4.1/ofscraper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/utils/paths.py` & `ofscraper-2.4.1/ofscraper/utils/paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         ext=match.group(0)
     else:
         ext=""
     #-1 is for / between parentdirs and file
     fileLength=256-len(ext)-len(str(dir))-1
     newFile=f"{re.sub(ext,'',file)[fileLength]}{ext}"
     final=pathlib.Path(dir,newFile)
-    log.debug(f"path: {final} path size: {len(final)}")
+    log.debug(f"path: {final} path size: {len(str(final))}")
     return pathlib.Path(dir,newFile)
 
 def _linux_trunicateHelper(path):
     path=pathlib.Path(path)
     dir=path.parent
     match=re.search("_[0-9]+\.[a-z]*$",path.name,re.IGNORECASE) or re.search("\.[a-z]*$",path.name,re.IGNORECASE)
     ext= match.group(0) if match else ""
```

### Comparing `ofscraper-2.4/ofscraper/utils/profiles.py` & `ofscraper-2.4.1/ofscraper/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/utils/separate.py` & `ofscraper-2.4.1/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/utils/stdout.py` & `ofscraper-2.4.1/ofscraper/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.4/ofscraper/utils/userselector.py` & `ofscraper-2.4.1/ofscraper/utils/userselector.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,14 @@
 
 def getselected_usernames():
     #username list will be retrived once per daemon run
     # manual prompt will need to recertify options every call
     global selectedusers
     scraper_bool=len(args.posts)>0 or args.action
     #always return with correct args
-    if "NONE" in args.username:
-        return []
     if selectedusers and scraper_bool:
             return selectedusers
     if scraper_bool:
         selectedusers=selectuserhelper()
     #create in these situations
     #set at least once
     elif args.username and not selectedusers:
```

### Comparing `ofscraper-2.4/pyproject.toml` & `ofscraper-2.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "2.4"
+version = "2.4.1"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
 httpx = {extras = ["http2"], version = "^0.23.3"}
```

### Comparing `ofscraper-2.4/PKG-INFO` & `ofscraper-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 2.4
+Version: 2.4.1
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

