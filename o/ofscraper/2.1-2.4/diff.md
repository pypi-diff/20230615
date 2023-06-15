# Comparing `tmp/ofscraper-2.1.tar.gz` & `tmp/ofscraper-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-2.1.tar", max compression
+gzip compressed data, was "ofscraper-2.4.tar", max compression
```

## Comparing `ofscraper-2.1.tar` & `ofscraper-2.4.tar`

### file list

```diff
@@ -1,41 +1,49 @@
--rw-r--r--   0        0        0     1067 2023-05-27 02:37:19.645984 ofscraper-2.1/LICENSE
--rw-r--r--   0        0        0     5192 2023-05-27 02:37:19.645984 ofscraper-2.1/README.md
--rw-r--r--   0        0        0      607 2023-05-27 02:37:20.529999 ofscraper-2.1/ofscraper/__init__.py
--rw-r--r--   0        0        0      999 2023-05-27 02:37:20.529999 ofscraper-2.1/ofscraper/__version__.py
--rw-r--r--   0        0        0        1 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/__init__.py
--rw-r--r--   0        0        0     1986 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/highlights.py
--rw-r--r--   0        0        0      979 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/init.py
--rw-r--r--   0        0        0     2264 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/me.py
--rw-r--r--   0        0        0     5599 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/messages.py
--rw-r--r--   0        0        0     1884 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/paid.py
--rw-r--r--   0        0        0     9037 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/posts.py
--rw-r--r--   0        0        0     2841 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/profile.py
--rw-r--r--   0        0        0     1867 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     7882 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/timeline.py
--rw-r--r--   0        0        0     5033 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/db/__init__.py
--rw-r--r--   0        0        0     6759 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3199 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     4028 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/interaction/like.py
--rw-r--r--   0        0        0     5477 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/prompts/prompt_functions.py
--rw-r--r--   0        0        0      359 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0    20976 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/prompts/prompts.py
--rwxr-xr-x   0        0        0    25673 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/scraper.py
--rw-r--r--   0        0        0        1 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0     4373 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/args.py
--rw-r--r--   0        0        0     8996 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/auth.py
--rw-r--r--   0        0        0    10857 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/config.py
--rw-r--r--   0        0        0      257 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/console.py
--rw-r--r--   0        0        0      993 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    18388 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     2865 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     2381 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/filters.py
--rw-r--r--   0        0        0     5105 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/logger.py
--rw-r--r--   0        0        0     5220 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     3060 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      779 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/separate.py
--rw-r--r--   0        0        0      674 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/stdout.py
--rw-r--r--   0        0        0     1509 2023-05-27 02:37:53.298575 ofscraper-2.1/pyproject.toml
--rw-r--r--   0        0        0     6554 1970-01-01 00:00:00.000000 ofscraper-2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-15 09:21:04.491317 ofscraper-2.4/LICENSE
+-rw-r--r--   0        0        0     5201 2023-06-15 09:21:04.491317 ofscraper-2.4/README.md
+-rw-r--r--   0        0        0      607 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/__init__.py
+-rw-r--r--   0        0        0      999 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/__version__.py
+-rw-r--r--   0        0        0        1 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/__init__.py
+-rw-r--r--   0        0        0     7060 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/archive.py
+-rw-r--r--   0        0        0     3944 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1067 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/init.py
+-rw-r--r--   0        0        0     2343 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/me.py
+-rw-r--r--   0        0        0     6515 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     8462 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     4570 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0    11157 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/posts.py
+-rw-r--r--   0        0        0     3593 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     3047 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     7707 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0    30895 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/commands/check.py
+-rwxr-xr-x   0        0        0    22495 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0     5769 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0     8581 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3253 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     4121 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0     1364 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/prompt model.md
+-rw-r--r--   0        0        0      463 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0     6754 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0    26253 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0      679 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/start.py
+-rw-r--r--   0        0        0        1 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0     9037 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/utils/args.py
+-rw-r--r--   0        0        0     9035 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0     6158 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0    10680 2023-06-15 09:21:04.499317 ofscraper-2.4/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      257 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      993 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    19571 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     2865 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     3137 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0     5622 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0     7649 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     3073 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      397 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/semaphoreDelayed.py
+-rw-r--r--   0        0        0     1358 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0      554 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/stdout.py
+-rw-r--r--   0        0        0     6092 2023-06-15 09:21:04.503317 ofscraper-2.4/ofscraper/utils/userselector.py
+-rw-r--r--   0        0        0     1518 2023-06-15 09:21:45.754020 ofscraper-2.4/pyproject.toml
+-rw-r--r--   0        0        0     6605 1970-01-01 00:00:00.000000 ofscraper-2.4/PKG-INFO
```

### Comparing `ofscraper-2.1/LICENSE` & `ofscraper-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-2.1/README.md` & `ofscraper-2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Intro
+
 A fork of onlyfans-scraper. It has been optimized to make it more feature complete with digitalcriminal's onlyfans script.
 A matter of fact with the right settings transitioning between the two scripts should be a easy enough process
 
 In addition there are numerous filtering features to control exactly which type of content you want to scrape.
 https://github.com/datawhores/OF-Scraper/blob/main/CHANGES.md
 
 <h3>DISCLAIMERS:</h3>
```

### Comparing `ofscraper-2.1/ofscraper/__init__.py` & `ofscraper-2.4/ofscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.1/ofscraper/__version__.py` & `ofscraper-2.4/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.1/ofscraper/api/highlights.py` & `ofscraper-2.4/ofscraper/api/me.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,58 +4,58 @@
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
-import asyncio
-from itertools import chain
 import logging
 import httpx
+from rich.console import Console
 from tenacity import retry,stop_after_attempt,wait_random
 import ofscraper.constants as constants
 import ofscraper.utils.auth as auth
+import ofscraper.utils.encoding as encoding
+import ofscraper.utils.stdout as stdout
+from ofscraper.utils.logger import updateSenstiveDict
 log=logging.getLogger(__package__)
+console=Console()
 
-
-
-
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
-def scrape_highlights(headers, user_id) -> list:
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MAX, max=constants.OF_MAX),reraise=True,after=lambda retry_state:print(f"Attempting to login attempt:{retry_state.attempt_number}/{constants.NUM_TRIES}")) 
+def scrape_user(headers):
     with httpx.Client(http2=True, headers=headers) as c:
-        url_stories = constants.highlightsWithStoriesEP.format(user_id)
-        url_story = constants.highlightsWithAStoryEP.format(user_id)
+        url = constants.meEP
 
         auth.add_cookies(c)
-        c.headers.update(auth.create_sign(url_stories, headers))
-        r_multiple = c.get(url_stories, timeout=None)
-
-        c.headers.update(auth.create_sign(url_story, headers))
-        r_one = c.get(url_story, timeout=None)
-
-        # highlights_, stories
-        if not r_multiple.is_error and not r_one.is_error:
-            log.debug(f"[bold]Highlight Post Count without Dupes[/bold] {len(r_multiple.json())} found")
-            log.debug(f"[bold]Story Post Count without Dupes[/bold] {len(r_one.json())} found")
-            return get_highlightList(r_multiple.json()),r_one.json()
-
-        r_multiple.raise_for_status()
-        r_one.raise_for_status()
-
-def get_highlightList(data):
-    for ele in list(filter(lambda x:isinstance(x,list),data.values())):
-        if len(list(filter(lambda x:isinstance(x.get("id"),int) and data.get("hasMore")!=None,ele)))>0:
-               return ele
-    return []
-
-
-    
-
-
+        c.headers.update(auth.create_sign(url, headers))
 
+        r = c.get(url, timeout=None)
+        if not r.is_error:
+            updateSenstiveDict(r.json()["id"],"userid")
+            updateSenstiveDict(r.json()["username"],"username")
+            updateSenstiveDict(r.json()["name"],"name")
+            return r.json()
+        r.raise_for_status()
 
 
+def parse_user(profile):
+    name = encoding.encode_utf_16(profile['name'])
+    username = profile['username']
 
+    return (name, username)
 
 
+def print_user(name, username):
+    with stdout.lowstdout():
+        console.print(f'Welcome, {name} | {username}')
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+def parse_subscriber_count(headers):
+    with httpx.Client(http2=True, headers=headers) as c:
+        url = constants.subscribeCountEP
+        auth.add_cookies(c)
+        c.headers.update(auth.create_sign(url, headers))
+        r = c.get(url, timeout=None)
+        if not r.is_error:
+            data=r.json()
+            return data["subscriptions"]["all"]
+        r.raise_for_status()
```

### Comparing `ofscraper-2.1/ofscraper/api/init.py` & `ofscraper-2.4/ofscraper/api/init.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,14 +5,15 @@
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 from . import me
+import traceback
 from rich.console import Console
 import ofscraper.utils.stdout as stdout
 import logging
 
 log=logging.getLogger(__package__)
 
 
@@ -27,8 +28,10 @@
 
 
 def getstatus(headers):
     try:
         resp = me.scrape_user(headers)
         return "UP"
     except Exception as e:
+        log.traceback(e)
+        log.traceback(traceback.format_exc())
         return "DOWN"
```

### Comparing `ofscraper-2.1/ofscraper/api/messages.py` & `ofscraper-2.4/ofscraper/api/messages.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,111 +26,140 @@
 import arrow
 import arrow
 import ofscraper.constants as constants
 import ofscraper.utils.auth as auth
 import ofscraper.utils.paths as paths
 from ..utils import auth
 import ofscraper.utils.console as console
+from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 
 from diskcache import Cache
 cache = Cache(paths.getcachepath())
 log=logging.getLogger(__package__)
 attempt = contextvars.ContextVar("attempt")
 
+sem = semaphoreDelayed(constants.MAX_SEMAPHORE)
+
 
 
 async def get_messages(headers, model_id):
-    global sem
-    sem = asyncio.Semaphore(8)
     overall_progress=Progress(SpinnerColumn(style=Style(color="blue"),),TextColumn("Getting Messages...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
-    with Live(progress_group, refresh_per_second=constants.refreshScreen,console=console.shared_console): 
 
+    global tasks
+    
+
+
+    tasks=[]
+    responseArray=[]
+    page_count=0
+    #require a min num of posts to be returned
+    min_posts=50
+    with Live(progress_group, refresh_per_second=constants.refreshScreen,console=console.shared_console): 
         oldmessages=cache.get(f"messages_{model_id}",default=[]) 
         oldmsgset=set(map(lambda x:x.get("id"),oldmessages))
         log.debug(f"[bold]Messages Cache[/bold] {len(oldmessages)} found")
         oldmessages=list(filter(lambda x:x.get("createdAt")!=None,oldmessages))
         postedAtArray=list(map(lambda x:x["id"],sorted(oldmessages,key=lambda x:arrow.get(x["createdAt"]).float_timestamp,reverse=True)))
-        global tasks
-        tasks=[]
+    
         
-        #split and interval can't match because of breakpoints
-        split=40
-        interval=30
-        if len(postedAtArray)>split:
-            splitArrays=[postedAtArray[i:i+split] for i in range(0, len(postedAtArray), interval)]
-            tasks.append(asyncio.create_task(scrape_messages(headers,model_id,job_progress)))
-            tasks.extend(list(map(lambda x:asyncio.create_task(scrape_messages(headers,model_id,job_progress,message_id=x[0])),splitArrays[1:-1])))
-            tasks.append(asyncio.create_task(scrape_messages(headers,model_id,job_progress,message_id=splitArrays[-1][0],recursive=True)))
+     
+        if len(postedAtArray)>min_posts:
+            splitArrays=[postedAtArray[i:i+min_posts] for i in range(0, len(postedAtArray), min_posts)]
+            #use the previous split for message_id
+            tasks.append(asyncio.create_task(scrape_messages(headers,model_id,job_progress,required_ids=set(splitArrays[0]))))
+            [tasks.append(asyncio.create_task(scrape_messages(headers,model_id,job_progress,required_ids=set(splitArrays[i]),message_id=splitArrays[i-1][-1])))
+            for i in range(1,len(splitArrays)-1)]
+            # keeping grabbing until nothign left
+            tasks.append(asyncio.create_task(scrape_messages(headers,model_id,job_progress,message_id=splitArrays[-2][-1])))
         else:
-            tasks.append(asyncio.create_task(scrape_messages(headers,model_id,job_progress,recursive=True)))
+            tasks.append(asyncio.create_task(scrape_messages(headers,model_id,job_progress)))
     
     
         
         
-        responseArray=[]
-        page_count=0 
+
         page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True)
 
 
         while len(tasks)!=0:
-                    for coro in asyncio.as_completed(tasks):
-                        result=await coro or []
-                        page_count=page_count+1
-                        overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
-                        responseArray.extend(result)
-                    time.sleep(2)
-                    tasks=list(filter(lambda x:x.done()==False,tasks))
+            for coro in asyncio.as_completed(tasks):
+                result=await coro or []
+                page_count=page_count+1
+                overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
+                responseArray.extend(result)
+            tasks=list(filter(lambda x:x.done()==False,tasks))
+        overall_progress.remove_task(page_task)  
     unduped=[]
     dupeSet=set()
     log.debug(f"[bold]Messages Count with Dupes[/bold] {len(responseArray)} found")
     for message in responseArray:
         if message["id"] in dupeSet:
             continue
         dupeSet.add(message["id"])
         oldmsgset.discard(message["id"])       
         unduped.append(message)
     if len(oldmsgset)==0:
         cache.set(f"messages_{model_id}",unduped,expire=constants.RESPONSE_EXPIRY)
+        cache.set(f"message_check_{model_id}",oldmessages,expire=constants.CHECK_EXPIRY)
+
         cache.close()
     else:
         cache.set(f"messages_{model_id}",[],expire=constants.RESPONSE_EXPIRY)
+        cache.set(f"message_check_{model_id}",[],expire=constants.CHECK_EXPIRY)
         cache.close()
         log.debug("Some messages where not retrived resetting cache")
 
     return unduped    
 
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
-async def scrape_messages(headers, user_id, progress,message_id=None,recursive=False) -> list:
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+async def scrape_messages(headers, model_id, progress,message_id=None,required_ids=None) -> list:
     global sem
+    global tasks
+    messages=None
     attempt.set(attempt.get(0) + 1)
     ep = constants.messagesNextEP if message_id else constants.messagesEP
-    url = ep.format(user_id, message_id)
+    url = ep.format(model_id, message_id)
     log.debug(url)
+
+
     async with sem:
         task=progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}: Message ID-> {message_id if message_id else 'initial'}")
         async with httpx.AsyncClient(http2=True, headers=headers) as c:
             auth.add_cookies(c)
             c.headers.update(auth.create_sign(url, headers))
             r = await c.get(url, timeout=None)
-            if not r.is_error:
-                progress.remove_task(task)
-                messages = r.json()['list']
-                if not messages:
-                    return []
-                elif len(messages)==0:
-                    return messages
-                elif not recursive:
-                    return messages
-                global tasks
+    if not r.is_error:
+        messages = r.json()['list']
+
+        if not messages:
+            messages=[]
+        elif len(messages)==0:
+            messages=[]
+        elif required_ids==None:
+            attempt.set(0)
+            tasks.append(asyncio.create_task(scrape_messages(headers, model_id,progress,message_id=messages[-1]['id'])))
+        else:
+            [required_ids.discard(ele["id"]) for ele in messages]
+            #try once more to grab, else quit
+            if len(required_ids)==1:
+                attempt.set(0)
+                tasks.append(asyncio.create_task(scrape_messages(headers, model_id,progress,message_id=messages[-1]['id'],required_ids=set())))
+
+            elif len(required_ids)>0:
                 attempt.set(0)
-                tasks.append(asyncio.create_task(scrape_messages(headers, user_id,progress, recursive=True,message_id=messages[-1]['id'])))
-                return messages
-            log.debug(f"[bold]message request status code:[/bold]{r.status_code}")
-            log.debug(f"[bold]message response:[/bold] {r.content.decode()}")
-            r.raise_for_status()
+                tasks.append(asyncio.create_task(scrape_messages(headers, model_id,progress,message_id=messages[-1]['id'],required_ids=required_ids)))
+            progress.remove_task(task)
+    else:
+        log.debug(f"[bold]message request status code:[/bold]{r.status_code}")
+        log.debug(f"[bold]message response:[/bold] {r.content.decode()}")
+        log.debug(f"[bold]message headers:[/bold] {r.headers}")
+
+        progress.remove_task(task)
+        r.raise_for_status()
+    return messages
```

### Comparing `ofscraper-2.1/ofscraper/api/posts.py` & `ofscraper-2.4/ofscraper/api/posts.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import re
 import logging
 import httpx
+import arrow
 from ..constants import LICENCE_URL
 import ofscraper.utils.args as args_
 import ofscraper.utils.auth as auth
 from mpegdash.parser import MPEGDASHParser
 import ofscraper.utils.config as config
 
+
 log=logging.getLogger(__package__)
 
 class Post():
     def __init__(self, post, model_id, username, responsetype=None):
         self._post = post
         self._model_id = model_id
         self._username = username
         self._responsetype_ = responsetype or post.get("responseType")
 
+    #All media return from API dict
     @property
-    def allmedia(self):
+    def post_media(self):
         if self._responsetype_ == "highlights":
             return [{"url": self.post["cover"], "type":"photo"}]
         return self._post.get("media") or []
 
     @property
     def post(self):
         return self._post
@@ -39,17 +42,15 @@
         if self.post.get("isArchived"):
             return 1
         return 0
 
     @property
     def text(self):
         if self._responsetype_ == "highlights":
-            return ""
-        elif self._responsetype_ == "stories":
-            return ""
+            return self.post.get("title") 
         return self._post.get("text")
 
     @property
     def title(self):
         return self._post.get("title")
 
     # original responsetype for database
@@ -63,27 +64,31 @@
             if config.get_archived_responsetype(config.read_config()) == "":
                 return "achived"
             return config.get_archived_responsetype(config.read_config())
 
         else:
             response=config.read_config().get("responsetype", {}).get(self._responsetype_) 
             if  response == "":
-                return self._responsetype_
+                return self._responsetype_.capitalize()
             elif  response == None:
-                return self._responsetype_
+                return self._responsetype_.capitalize()
             elif  response != "":
-                return  response
+                return  response.capitalize()
 
     @property
     def id(self):
         return self._post["id"]
 
     @property
     def date(self):
         return self._post.get("createdAt") or self._post.get("postedAt")
+    #modify verison of post date
+    @property
+    def date_(self):
+        return arrow.get(self.date).format("YYYY-MM-DD hh:mm:ss")
 
     @property
     def value(self):
         if self.price == 0:
             return "free"
         elif self.price > 0:
             return "paid"
@@ -105,38 +110,61 @@
         else:
             return self._model_id
 
     @property
     def preview(self):
         return self._post.get("preview")
 
+    #media object array for media that is unlocked or viewable
     @property
     def media(self):
         if (self.fromuser != self.model_id):
             return []
         else:
             media = map(lambda x: Media(
-                x[1], x[0], self), enumerate(self.allmedia))
+                x[1], x[0], self), enumerate(self.post_media))
             return list(filter(lambda x: x.canview == True, media))
-
-
+    #media object array for all media
+    @property
+    def all_media(self):
+        return list(map(lambda x: Media(
+            x[1], x[0], self), enumerate(self.post_media)))
+    @property
+    def expires(self):
+        return (self._post.get("expiredAt",{}) or self._post.get("expiresAt",None))!=None
 class Media():
     def __init__(self, media, count, post):
         self._media = media
         self._count = count
         self._post = post
 
     @property
+    def expires(self):
+        return self._post.expires
+
+    @property
     def mediatype(self):
         if self.responsetype_ == "highlights":
             return "images"
         if self._media["type"] == "gif" or self._media["type"] == "photo":
             return "images"
         else:
             return f"{self._media['type']}s"
+    @property
+    def length(self):
+        return self._media.get("duration") or self._media.get("source",{}).get("duration")
+    @property
+    def length_(self):
+        if not self.length:
+            return "N/A"
+        return str((arrow.get(self.length)-arrow.get(0)))
+
+   
+
+      
 
     @property
     def url(self):
         if self.responsetype_ == "stories":
             return self._media.get("files", {}).get("source", {}).get("url")
         elif self.responsetype_ == "highlights":
             return self._media.get("url")
@@ -151,16 +179,16 @@
 
     @property
     def id(self):
         return self._media["id"]
 
     # ID for use in dynamic names
     @property
-    def id_(self):
-        if self.count != None and len(self._post.allmedia) > 1:
+    def postid_(self):
+        if self.count != None and len(self._post.post_media) > 1:
             return f"{self._post._post['id']}_{self.count}"
         return self._post._post['id']
 
     @property
     def canview(self):
         if self.responsetype_ == "highlights":
             return True
@@ -177,19 +205,31 @@
     @property
     def value(self):
         return self._post.value
 
     @property
     def postdate(self):
         return self._post.date
+    #modified verison of post date
+    @property
+    def postdate_(self):
+        return self._post.date_ 
 
     @property
     def date(self):
         return self._media.get("createdAt") or self._media.get("postedAt") or self.postdate
+    
+    #modified verison of media date
+    @property
+    def date_(self):
+        if self._media.get("createdAt") or self._media.get("postedAt"):
+            return arrow.get(self._media.get("createdAt") or self._media.get("postedAt")).format("YYYY-MM-DD hh:mm:ss")()
+        return self.postdate_
 
+ 
     @property
     def id(self):
         return self._media.get("id")
 
     @property
     def postid(self):
         return self._post.id
@@ -228,24 +268,28 @@
         if not self.mpd:
             return None
 
 
 
     @property
     def text_(self):
-        text = self.text
+        if self.responsetype_!="Profile":
+            text = self.text or self.filename or arrow.get(self.date).format(config.get_date(config.read_config()))
+        elif self.responsetype_=="Profile":
+            text=f"{arrow.get(self.date).format(config.get_date(config.read_config()))} {self.text or self.filename}"
         if len(text)==0:
             return text
         # this is for removing emojis
         # text=re.sub("[^\x00-\x7F]","",text)
         # this is for removing html tags
         text = re.sub("<[^>]*>", "", text)
         # this for remove random special invalid special characters
         text = re.sub('[\n<>:"/\|?*]+', '', text)
         text = re.sub(" +", " ", text)
+        text=re.sub(" ",config.get_spacereplacer(config.read_config()),text)
         length = int(config.get_textlength(config.read_config()))
         if length==0 and self._addcount():
                 return f"{text}_{self.count}"
         elif length==0 and not self._addcount():
                 return text
  
         elif args_.getargs().letter_count:
@@ -280,15 +324,21 @@
 
     @property
     def count(self):
         return self._count+1
 
     @property
     def filename(self):
-        return  re.sub("\.mpd$","",(self.url or self.mpd).split('.')[-2].split('/')[-1].strip("/,.;!_-@#$%^&*()+\\ "))
+        if not self.url or self.mpd:
+            return None
+        elif not self.responsetype=="Profile":
+            return  re.sub("\.mpd$","",(self.url or self.mpd).split('.')[-2].split('/')[-1].strip("/,.;!_-@#$%^&*()+\\ "))
+        else:
+            filename= re.sub("\.mpd$","",(self.url or self.mpd).split('.')[-2].split('/')[-1].strip("/,.;!_-@#$%^&*()+\\ "))
+            return f"{filename}_{arrow.get(self.date).format(config.get_date(config.read_config()))}"
 
     @property
     def preview(self):
         if self.post.preview:
             return 1
         else:
             return 0
@@ -297,31 +347,34 @@
     def linked(self):
         return None
 
     @property
     def media(self):
         return self._media
     @property
-    def parse_mpd(self): 
+    async def parse_mpd(self): 
         if not self.mpd:
             return
         headers = auth.make_headers(auth.read_auth())
         params={"Policy":self.policy,"Key-Pair-Id":self.keypair,"Signature":self.signature}
-        with httpx.Client(http2=True, headers=headers,params=params) as c:
+        async with httpx.AsyncClient(http2=True, headers=headers,params=params) as c:
             auth.add_cookies(c)
             c.headers.update(auth.create_sign(self.mpd, headers))
-            r = c.get(self.mpd, timeout=None)
+            r = await c.get(self.mpd, timeout=None)
             if r.status_code!=200:
                 return None
             return MPEGDASHParser.parse(r.content.decode())
     @property
     def license(self):
+        if not self.mpd:
+            return None
         responsetype=self.post.post["responseType"]
         if responsetype in ["timeline","archived","pinned"]:
             responsetype="post"
         return LICENCE_URL.format(self.id,responsetype,self.postid)
 
+
     # for use in dynamic names
     def _addcount(self):
-        if len(self._post.allmedia) > 1 or self.responsetype_ in ["stories", "highlights"]:
+        if len(self._post.post_media) > 1 or self.responsetype_ in ["stories", "highlights"]:
             return True
         return False
```

### Comparing `ofscraper-2.1/ofscraper/api/profile.py` & `ofscraper-2.4/ofscraper/api/profile.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,47 +4,64 @@
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 import logging
+import contextvars
+
+from typing import Union
 import httpx
 from rich.console import Console
 from tenacity import retry,stop_after_attempt,wait_random
-from ..constants import profileEP,NUM_TRIES
+from ..constants import profileEP,NUM_TRIES,DAILY_EXPIRY
 from ..utils import auth, encoding
-from xxhash import xxh32
+from xxhash import xxh128
+from diskcache import Cache
+from ..utils.paths import getcachepath
+import ofscraper.constants as constants
+cache = Cache(getcachepath())
+
 
 log=logging.getLogger(__package__)
 console=Console()
+attempt = contextvars.ContextVar("attempt")
+
+
 
-@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
-def scrape_profile(headers, username) -> dict:
+# can get profile from username or id
+@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+def scrape_profile(headers, username:Union[int, str]) -> dict:
+    attempt.set(attempt.get(0) + 1)
+    log.info(f"Attempt {attempt.get()}/{constants.NUM_TRIES} to get profile {username}")
     with httpx.Client(http2=True, headers=headers) as c:
         url = profileEP.format(username)
 
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
 
         r = c.get(profileEP.format(username), timeout=None)
         if not r.is_error:
+            attempt.set(0)
             return r.json()
+        elif r.status_code==404:
+            return {"username":"modeldeleted"}
         r.raise_for_status()
 
 
 def parse_profile(profile: dict) -> tuple:
     media = []
     media.append(profile.get('avatar'))
     media.append(profile.get('profile'))
     media=list(filter(lambda x:x!=None,media))
 
     output=[]
     for ele in media:
-        output.append({"url":ele,"responsetype":"profile","mediatype":"photo","value":"free","createdAt":profile["joinDate"],"text":profile["about"],"id":xxh32(ele).hexdigest()})
+        output.append({"url":ele,"responsetype":"profile","mediatype":"photo","value":"free","createdAt":profile["joinDate"],"text":profile["about"],"id":xxh128(ele).hexdigest()})
 
 
     name = encoding.encode_utf_16(profile['name'])
     username = profile['username']
     id_ = profile['id']
     join_date = profile['joinDate']
     posts_count = profile['postsCount']
@@ -64,22 +81,28 @@
 def print_profile_info(info):
     header_fmt = 'Name: {} | Username: {} | ID: {} | Joined: {}\n'
     info_fmt = '- {} posts\n -- {} photos\n -- {} videos\n -- {} audios\n- {} archived posts'
     final_fmt = header_fmt + info_fmt
     log.info(final_fmt.format(*info))
 
 
-@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
+@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 def get_id(headers, username):
+    id=cache.get(f"model_id_{username}",None)
+    if id:
+        return id
     with httpx.Client(http2=True, headers=headers) as c:
         url = profileEP.format(username)
 
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
 
         r = c.get(url, timeout=None)
         if not r.is_error:
-            return r.json()['id']
+            id=r.json()['id']
+            cache.set(f"model_id_{username}",id,DAILY_EXPIRY)
+            return id
+        
         r.raise_for_status()
```

### Comparing `ofscraper-2.1/ofscraper/api/subscriptions.py` & `ofscraper-2.4/ofscraper/api/subscriptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,40 +9,67 @@
 """
 
 import asyncio
 from itertools import chain
 import logging
 import httpx
 from rich.console import Console
+import arrow
 console=Console()
 from tenacity import retry,stop_after_attempt,wait_random
 from ..constants import subscriptionsEP,NUM_TRIES
 from ..utils import auth, dates
+import ofscraper.constants as constants
 log=logging.getLogger(__package__)
 
 
 async def get_subscriptions(headers, subscribe_count):
     offsets = range(0, subscribe_count, 10)
     tasks = [scrape_subscriptions(headers, offset) for offset in offsets]
     subscriptions = await asyncio.gather(*tasks)
     return list(chain.from_iterable(subscriptions))
 
 
-@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
+@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def scrape_subscriptions(headers, offset=500) -> list:
     async with httpx.AsyncClient(http2=True, headers=headers) as c:
         url = subscriptionsEP.format(offset)
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
 
         r = await c.get(subscriptionsEP.format(offset), timeout=None)
         if not r.is_error:
             subscriptions = r.json()
             return subscriptions
         r.raise_for_status()
 
 def parse_subscriptions(subscriptions: list) -> list:
-    data = [{"name":profile['username'],"id":profile['id'],"date":dates.convert_date_to_mdyhms(
-        profile['subscribedByExpireDate']),"active":not profile['subscribedIsExpiredNow'],"data":profile} for profile in subscriptions]
+    datenow=arrow.now()
+    data = [
+        {"name":profile['username']
+         ,"id":profile['id'],
+         "sub-price":profile.get("currentSubscribePrice",{}),
+         "regular-price":profile.get("subscribedByData").get("regularPrice") if profile.get("subscribedByData") else None,
+         "promo-price": sorted(list(filter(lambda x: x.get("canClaim") == True,profile.get("promotions") or [])), key=lambda x: x["price"]),
+         "expired":profile.get("subscribedByData").get("expiredAt") if profile.get("subscribedByData") else None,
+         "subscribed":(profile.get("subscribedByData").get("subscribes") or [{}])[0].get("startDate") if profile.get("subscribedByData") else None ,
+         "renewed":profile.get("subscribedByData").get("renewedAt") if profile.get("subscribedByData") else None,
+        "active" :  arrow.get(profile.get("subscribedByData").get("expiredAt"))>datenow if profile.get("subscribedByData") else None
+
+
+         } for profile in subscriptions]
+    data=setpricehelper(data)
+    return data
+
+def setpricehelper(data):
+    for ele in data:
+        prices=list(filter(lambda x:x!=None,[ele.get("sub-price"),(ele.get("promo-price") or [{}])[0].get("price"),ele["regular-price"]]))
+        if len(prices)==0:
+            ele["price"]=None
+        else:
+            ele["price"]=min(prices)
     return data
+    
+
+
```

### Comparing `ofscraper-2.1/ofscraper/api/timeline.py` & `ofscraper-2.4/ofscraper/api/timeline.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 import time
 import asyncio
+from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 import logging
 import contextvars
 import math
 import httpx
 from tenacity import retry,stop_after_attempt,wait_random
 from rich.progress import Progress
 from rich.progress import (
@@ -24,166 +25,151 @@
 from rich.live import Live
 from rich.style import Style
 import arrow
 import ofscraper.constants as constants
 from ..utils import auth
 from ..utils.paths import getcachepath
 import ofscraper.utils.console as console
+import ofscraper.utils.config as config_
+import ofscraper.utils.args as args_
 
 from diskcache import Cache
 cache = Cache(getcachepath())
 log=logging.getLogger(__package__)
 attempt = contextvars.ContextVar("attempt")
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
-def scrape_pinned_posts(headers, model_id,timestamp=0) -> list:
-    with httpx.Client(http2=True, headers=headers) as c:
-        ep = constants.timelinePinnedNextEP if timestamp else constants.timelinePinnedEP
-        url = ep.format(model_id, timestamp)
-        # url = timelinePinnedEP.format(model_id)
-
-        auth.add_cookies(c)
-        c.headers.update(auth.create_sign(url, headers))
 
-        r = c.get(url, timeout=None)
-        if not r.is_error:
-            return r.json()['list']
-        r.raise_for_status()
-        log.debug(f"[bold]pinned request status code:[/bold]{r.status_code}")
-        log.debug(f"[bold]pinned response:[/bold] {r.content.decode()}")
-
-def get_pinned_post(headers,model_id,username):
-    return scrape_pinned_posts(headers,model_id)
-   
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
-async def scrape_timeline_posts(headers, model_id,progress, timestamp=None,recursive=False) -> list:
-    global sem 
+sem = semaphoreDelayed(constants.MAX_SEMAPHORE)
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+async def scrape_timeline_posts(headers, model_id,progress, timestamp=None,required_ids=None) -> list:
+    global tasks
+    global sem
+    posts=None
     attempt.set(attempt.get(0) + 1)
+    if timestamp and   (float(timestamp)>(args_.getargs().before or arrow.now()).float_timestamp):
+        return []
     if timestamp:
         log.debug(arrow.get(math.trunc(float(timestamp))))
         timestamp=str(timestamp)
         ep = constants.timelineNextEP
         url = ep.format(model_id, timestamp)
     else:
         ep=constants.timelineEP
         url=ep.format(model_id)
     log.debug(url)
     async with sem:
         task=progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}: Timestamp -> {arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}",visible=True)
-
         async with httpx.AsyncClient(http2=True, headers=headers) as c:
             auth.add_cookies(c)
             c.headers.update(auth.create_sign(url, headers))
             r = await c.get(url , timeout=None)
-            if not r.is_error:
-                progress.remove_task(task)
-                posts = r.json()['list']
-    
-                if not posts:
-                    return []
-                elif len(posts)==0:
-                    return posts
-                elif not recursive:
-                    return posts
-                # recursive search for posts
+    if not r.is_error:
+        progress.remove_task(task)
+        posts = r.json()['list']
+        if not posts:
+            posts= []
+        elif len(posts)==0:
+            posts= []
+        elif required_ids==None:
+            attempt.set(0)
+            tasks.append(asyncio.create_task(scrape_timeline_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'])))
+        else:
+            [required_ids.discard(float(ele["postedAtPrecise"])) for ele in posts]
+
+
+            #try once more to get id if only 1 left
+            if len(required_ids)==1:
                 attempt.set(0)
-                global tasks
-                tasks.append(asyncio.create_task( scrape_timeline_posts(headers, model_id,progress,posts[-1]['postedAtPrecise'],recursive=True)))
-                return posts
+                tasks.append(asyncio.create_task(scrape_timeline_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=set())))
+
+            elif len(required_ids)>0:
+                attempt.set(0)
+                tasks.append(asyncio.create_task(scrape_timeline_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=required_ids)))
+    else:
             log.debug(f"[bold]timeline request status code:[/bold]{r.status_code}")
             log.debug(f"[bold]timeline response:[/bold] {r.content.decode()}")
+            log.debug(f"[bold]timeline headers:[/bold] {r.headers}")
+
+            progress.remove_task(task)
             r.raise_for_status()
+    return posts
 
-async def get_timeline_post(headers,model_id):
-    global sem
-    sem = asyncio.Semaphore(8)
+async def get_timeline_post(headers,model_id): 
     overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting timeline media...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
+
+    global tasks
+    tasks=[]
+    min_posts=50
+    responseArray=[]
+    page_count=0
     with Live(progress_group, refresh_per_second=5,console=console.shared_console): 
 
-        oldtimeline=cache.get(f"timeline_{model_id}",default=[]) 
+        oldtimeline=cache.get(f"timeline_{model_id}",default=[])
         oldtimeset=set(map(lambda x:x.get("id"),oldtimeline))
         log.debug(f"[bold]Timeline Cache[/bold] {len(oldtimeline)} found")
         oldtimeline=list(filter(lambda x:x.get("postedAtPrecise")!=None,oldtimeline))
         postedAtArray=sorted(list(map(lambda x:float(x["postedAtPrecise"]),oldtimeline)))
-        global tasks
-        tasks=[]
-        #max result is 50, try to get 40 in each async task for leeway
-        # Also need to grab new posts
-        #add differing splits and interval for inclusivity and potential breakpoints
-        split=40
-        interval=30
-        if len(postedAtArray)>split:
-            split=40
-            interval=30
-            splitArrays=[postedAtArray[i:i+split] for i in range(0, len(postedAtArray), interval)]
-            
-            tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress)))
-            tasks.extend(list(map(lambda x:asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,timestamp=x[0]-100)),splitArrays[1:-1])))
-            tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,timestamp=splitArrays[-1][0],recursive=True)))
-        else:
-            tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,recursive=True)))
-
-        responseArray=[]
+        filteredArray=list(filter(lambda x:x>=(args_.getargs().after or arrow.get(0)).float_timestamp,postedAtArray))
+        
     
+       
+        if len(filteredArray)>min_posts:
+            splitArrays=[filteredArray[i:i+min_posts] for i in range(0, len(filteredArray), min_posts)]
+            #use the previous split for timesamp
+            tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,required_ids=set(splitArrays[0]),timestamp= splitArrays[0][0]-20000)))
+            [tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,required_ids=set(splitArrays[i]),timestamp=splitArrays[i-1][-1])))
+            for i in range(1,len(splitArrays)-1)]
+            # keeping grabbing until nothign left
+            tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,timestamp=splitArrays[-2][-1])))
+        else:
+            tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,timestamp=args_.getargs().float_timestamp if args_.getargs().after else None)))
     
-        page_count=0 
+
         page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True)
         while len(tasks)!=0:
             for coro in asyncio.as_completed(tasks):
                 result=await coro or []
                 page_count=page_count+1
                 overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
                 responseArray.extend(result)
-            time.sleep(2)
+            time.sleep(1)
             tasks=list(filter(lambda x:x.done()==False,tasks))
         overall_progress.remove_task(page_task)
     unduped=[]
     dupeSet=set()
     log.debug(f"[bold]Timeline Count with Dupes[/bold] {len(responseArray)} found")
-    for post in sorted(responseArray,key=lambda x:x["postedAtPrecise"]):
+    for post in responseArray:
         if post["id"] in dupeSet:
             continue
         dupeSet.add(post["id"])
         oldtimeset.discard(post["id"])
         unduped.append(post)
     log.debug(f"[bold]Timeline Count without Dupes[/bold] {len(unduped)} found")
-    if len(oldtimeset)==0:
+    if len(oldtimeset)==0 and not (args_.getargs().before or args_.getargs().after):
         cache.set(f"timeline_{model_id}",unduped,expire=constants.RESPONSE_EXPIRY)
+        cache.set(f"timeline_check_{model_id}",unduped,expire=constants.CHECK_EXPIRY)
         cache.close()
-    else:
+    elif len(oldtimeset)>0 and not (args_.getargs().before or args_.getargs().after):
         cache.set(f"timeline_{model_id}",[],expire=constants.RESPONSE_EXPIRY)
+        cache.set(f"timeline_check_{model_id}",[],expire=constants.CHECK_EXPIRY)
+
         cache.close()
         log.debug("Some post where not retrived resetting cache")
 
     return unduped                                
 
-def get_archive_post(headers,model_id):
-    return scrape_archived_posts(headers,model_id)
-   
-
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
-def scrape_archived_posts(headers, model_id, timestamp=0) -> list:
-    ep = constants.archivedNextEP if timestamp else constants.archivedEP
-    url = ep.format(model_id, timestamp)
-    with httpx.Client(http2=True, headers=headers) as c:
+
+def get_individual_post(id,client=None):
+    headers = auth.make_headers(auth.read_auth())
+    with client or httpx.Client(http2=True, headers=headers) as c:
+        url=f"https://onlyfans.com/api2/v2/posts/{id}?skip_users=all"
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
-
-        r = c.get(url, timeout=None)
+        r=c.get(url)
         if not r.is_error:
-            posts = r.json()['list']
-            if not posts:
-                return posts
-            posts += scrape_archived_posts(
-                headers, model_id, posts[-1]['postedAtPrecise'])
-            return posts
-        r.raise_for_status()
-        log.debug(f"[bold]archived request status code:[/bold]{r.status_code}")
-        log.debug(f"[bold]archived response:[/bold] {r.content.decode()}")
-
-
-
-               
+            return r.json()
+        log.debug(f"{r.status_code}")
+        log.debug(f"{r.content.decode()}")
```

### Comparing `ofscraper-2.1/ofscraper/constants.py` & `ofscraper-2.4/ofscraper/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,34 +28,36 @@
 
 subscriptionsEP = 'https://onlyfans.com/api2/v2/subscriptions/subscribes?offset={}&type=all&sort=asc&field=expire_date&limit=10'
 subscribeCountEP='https://onlyfans.com/api2/v2/subscriptions/count/all'
 profileEP = 'https://onlyfans.com/api2/v2/users/{}'
 
 timelineEP = 'https://onlyfans.com/api2/v2/users/{}/posts?limit=100&order=publish_date_asc&skip_users=all&skip_users_dups=1&pinned=0&format=infinite'
 timelineNextEP = 'https://onlyfans.com/api2/v2/users/{}/posts?limit=100&order=publish_date_asc&skip_users=all&skip_users_dups=1&afterPublishTime={}&pinned=0&format=infinite'
-timelinePinnedEP = 'https://onlyfans.com/api2/v2/users/{}/posts?limit=100&order=publish_date_asc&skip_users=all&skip_users_dups=1&pinned=1&format=infinite'
+timelinePinnedEP = 'https://onlyfans.com/api2/v2/users/{}/posts?limit=100&order=publish_date_asc&skip_users=all&skip_users_dups=1&pinnedf=1&format=infinite'
 timelinePinnedNextEP = 'https://onlyfans.com/api2/v2/users/{}/posts?limit=100&order=publish_date_asc&skip_users=all&skip_users_dups=1&pinned=1&afterPublishTime={}&format=infinite'
 archivedEP = 'https://onlyfans.com/api2/v2/users/{}/posts/archived?limit=100&order=publish_date_asc&skip_users=all&skip_users_dups=1&format=infinite'
 archivedNextEP = 'https://onlyfans.com/api2/v2/users/{}/posts/archived?limit=100&order=publish_date_asc&skip_users=all&skip_users_dups=1&afterPublishTime={}&format=infinite'
 
 highlightsWithStoriesEP = 'https://onlyfans.com/api2/v2/users/{}/stories/highlights?limit=5&offset=0&unf=1'
 highlightsWithAStoryEP = 'https://onlyfans.com/api2/v2/users/{}/stories?unf=1'
 storyEP = 'https://onlyfans.com/api2/v2/stories/highlights/{}?unf=1'
 
 messagesEP = 'https://onlyfans.com/api2/v2/chats/{}/messages?limit=100&offset=0&order=desc&skip_users=all&skip_users_dups=1'
 messagesNextEP = 'https://onlyfans.com/api2/v2/chats/{}/messages?limit=100&offset=0&id={}&order=desc&skip_users=all&skip_users_dups=1'
 
 favoriteEP = 'https://onlyfans.com/api2/v2/posts/{}/favorites/{}'
 postURL = 'https://onlyfans.com/{}/{}'
 
-DC_EP = 'https://raw.githubusercontent.com/DATAHOARDERS/dynamic-rules/main/onlyfans.json'
+DYNAMIC = 'https://raw.githubusercontent.com/deviint/onlyfans-dynamic-rules/main/dynamicRules.json'
 
 donateEP = "https://www.buymeacoffee.com/excludedBittern"
 
 purchased_contentEP = "https://onlyfans.com/api2/v2/posts/paid?limit=100&skip_users=all&format=infinite&offset={}&user_id={}"
+purchased_contentALL = "https://onlyfans.com/api2/v2/posts/paid?limit=100&skip_users=all&format=infinite&offset={}"
+
 
 mainPromptChoices = {
     'Download content from a user': 0,
     'Like all of a user\'s posts': 1,
     'Unlike all of a user\'s posts': 2,
     'Edit auth.json file': 3,
     'Edit config.json file': 4,
@@ -92,22 +94,39 @@
 PROFILE_DEFAULT="main_profile"
 PREMIUM_DEFAULT="Premium"
 MP4DECRYPT_DEFAULT=""
 FFMPEG_DEFAULT =""
 DISCORD_DEFAULT =""
 SUPPRESS_LOG_LEVEL=21
 RESPONSE_TYPE_DEFAULT= {
-            "message":"messages",
-            "timeline":"posts",
-            "archived":"archived",
-            "paid":"messages",
-            "stories":"stories",
-            "highlights":"stories",
-            "profile":"profile",
-            "pinned":"posts"
+            "message":"Messages",
+            "timeline":"Posts",
+            "archived":"Archived",
+            "paid":"Messages",
+            "stories":"Stories",
+            "highlights":"Stories",
+            "profile":"Profile",
+            "pinned":"Posts"
         }
-NUM_TRIES=5
+NUM_TRIES=10
 RESPONSE_EXPIRY=5000000
+CHECK_EXPIRY=86400
+DAILY_EXPIRY=86400
+DISCORDWAIT=5
+OF_MIN=15
+OF_MAX=50
 LICENCE_URL="https://onlyfans.com/api2/v2/users/media/{}/drm/{}/{}?type=widevine"
 logname="ofscraper"
 PATH_STR_MAX=200
-refreshScreen=20
+TABLE_STR_MAX=100
+
+refreshScreen=20
+
+MP4DECRYPT_LINUX="https://www.bok.net/Bento4/binaries/Bento4-SDK-1-6-0-640.x86_64-unknown-linux.zip"
+MP4DECRYPT_WINDOWS="https://www.bok.net/Bento4/binaries/Bento4-SDK-1-6-0-640.x86_64-microsoft-win32.zip"
+FFMPEG_LINUX="https://github.com/BtbN/FFmpeg-Builds/releases/download/latest/ffmpeg-master-latest-linux64-gpl.tar.xz"
+FFMPEG_WINDOWS="https://github.com/BtbN/FFmpeg-Builds/releases/download/latest/ffmpeg-master-latest-win64-gpl.zip"
+
+THREADS_DEFAULT=8
+MAX_SEMAPHORE=8
+AlT_SEM=4
+CODE_EXECUTION_DEFAULT =False
```

### Comparing `ofscraper-2.1/ofscraper/db/queries.py` & `ofscraper-2.4/ofscraper/db/queries.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,14 +135,21 @@
 """
 
 allIDCheck=\
 """
 SELECT media_id FROM medias
 """
 
+
+allPOSTCheck=\
+"""
+SELECT post_id FROM medias
+"""
+
+
 mediaInsert=\
 f"""INSERT INTO 'medias'(
 media_id,post_id,link,directory,filename,size,api_type,media_type,preview,linked,downloaded,created_at)
             VALUES (?, ?,?,?,?,?,?,?,?,?,?,?);"""
 
 mediaDupeCheck=\
 """
@@ -171,7 +178,8 @@
 
 profileUpdate=\
 f"""Update 'profiles'
 SET
 user_id=?,username=?
 WHERE user_id=(?);"""
 
+
```

### Comparing `ofscraper-2.1/ofscraper/interaction/like.py` & `ofscraper-2.4/ofscraper/interaction/like.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,22 +25,24 @@
     TextColumn,
     SpinnerColumn
 )
 from rich.style import Style
 from ..api import timeline
 from ..constants import favoriteEP, postURL
 from ..utils import auth
+import ofscraper.api.archive as archive
+import ofscraper.api.pinned as pinned
 import ofscraper.utils.console as console
 
 
 
 def get_posts(headers, model_id):
-    pinned_posts = timeline.scrape_pinned_posts(headers, model_id)
+    pinned_posts = asyncio.run(pinned.get_pinned_post(headers, model_id))
     timeline_posts = asyncio.run(timeline.get_timeline_post(headers, model_id))
-    archived_posts = timeline.scrape_archived_posts(headers, model_id)
+    archived_posts = asyncio.run(archive.get_archived_post(headers, model_id))
     log.debug(f"[bold]Number of Post Found[/bold] {len(pinned_posts) + len(timeline_posts) + len(archived_posts)}")
     return pinned_posts + timeline_posts + archived_posts
 
 
 def filter_for_unfavorited(posts: list) -> list:
     output=list(filter(lambda x:x.get("isFavorite")==False,posts))
     log.debug(f"[bold]Number of unliked post[/bold] {len(output)}")
```

### Comparing `ofscraper-2.1/ofscraper/prompts/prompts.py` & `ofscraper-2.4/ofscraper/prompts/prompts.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,22 +6,27 @@
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 import sys
 from rich.console import Console
 import pathlib
+import re
+import arrow
 from InquirerPy.resolver import prompt
+from InquirerPy import inquirer
 from InquirerPy.separator import Separator
 from InquirerPy.base import Choice
+from InquirerPy import get_style
 from InquirerPy.validator import EmptyInputValidator,PathValidator
 import ofscraper.constants as constants
 import ofscraper.prompts.prompt_strings as prompt_strings
-import ofscraper.prompts.prompt_functions as prompt_functions
+import ofscraper.prompts.prompt_validators as prompt_validators
 import ofscraper.utils.config as config
+import ofscraper.utils.args as args_
 
 console=Console()
 def main_prompt() -> int:
     main_prompt_choices = [*constants.mainPromptChoices]
     main_prompt_choices.insert(3, Separator())
 
     name = 'action'
@@ -52,16 +57,17 @@
 
     questions = [
         {
             'type': 'checkbox',
             'qmark': '[?]',
             'name': name,
             'message': 'Which area(s) would you like to scrape? (Press ENTER to continue)',
-             "validate":prompt_functions.emptyListValidator(),
+             "validate":prompt_validators.emptyListValidator(),
             'choices': [
+                Choice("Profile"),
                 Choice('Timeline'),
                 Choice('Pinned'),
                 Choice('Archived'),
                 Choice('Highlights'),
                 Choice('Stories'),
                 Choice('Messages'),
                 Choice("Purchased")
@@ -166,41 +172,41 @@
 def user_agent_prompt(current):
     questions = [
         {
             'type': 'input',
             'message':'Enter User_Agent from browser',
             'default':current,
             'validate':EmptyInputValidator(),
-            'filter':lambda x:prompt_functions.cleanTextInput(x)
+            'filter':lambda x:prompt_validators.cleanTextInput(x)
         }
     ]
     return  prompt(questions)[0]
 
 def xbc_prompt():
     questions = [
         {
             'type': 'input',
             'message':'Enter x-bc request header',
             'instruction':f"\nGo to browser network tools to view\nFor more instructions visit https://github.com/datawhores/ofscraper\n\n"
             ,'validate':EmptyInputValidator(),
-            'filter':lambda x:prompt_functions.cleanTextInput(x)
+            'filter':lambda x:prompt_validators.cleanTextInput(x)
         }
     ]
     return  prompt(questions)[0]
 
 
 
 
 def auth_full_paste():
     questions = [
         {
             'type': 'input',
             'message':'Paste Text from Extension',
-            "validate": prompt_functions.jsonValidator(),
-            "filter":prompt_functions.jsonloader,
+            "validate": prompt_validators.jsonValidator(),
+            "filter":prompt_validators.jsonloader,
              "instruction":\
 """
 Cookie Helper Repo:https://github.com/M-rcus/OnlyFans-Cookie-Helper
 """
              
 
         }
@@ -265,15 +271,15 @@
             'type': 'input',
             'name': name,
             'message': 
 """
 What would you like to name your new profile?
 only letters, numbers, and underscores are allowed
 """,
-            'validator':prompt_functions.namevalitator()
+            'validator':prompt_validators.namevalitator()
 
         }
     ]
 
     answer = prompt(questions)
     return answer[name]
 
@@ -283,15 +289,15 @@
 
     questions = [
         {
             'type': 'list',
             'name': name,
             'message': 'Select Profile',
             'choices':profiles
-            ,"validate":prompt_functions.emptyListValidator()
+            ,"validate":prompt_validators.emptyListValidator()
         }
     ]
     answer = prompt(questions)
     profile = answer[name]
     return profile
 
 
@@ -299,24 +305,24 @@
 
     questions = [
         {
             'type': 'input',
             'name': 'main_profile',
             'message': 'What would you like your main profile to be?',
             'default': config.get_main_profile(config_),
-            "validate":lambda x:prompt_functions.emptyListValidator() and  isinstance(x[0],str)
+            "validate":EmptyInputValidator()
         },
         {
             'type': 'filepath',
             'name': 'save_location',
             'message':"save_location: ",
             'long_instruction': 'Where would you like to set as the root save downloaded directory?',
             'default':config.get_save_location(config_),
-            "filter":lambda x:prompt_functions.cleanTextInput(x),
-            "validate": lambda x:pathlib.Path(x).is_dir() and PathValidator()
+            "filter":lambda x:prompt_validators.cleanTextInput(x),
+            "validate": PathValidator(is_dir=True)
         },
         {
             'type': 'number',
             'name': 'file_size_limit',
             'message':"file_size_limit: ",
             'long_instruction':
 """
@@ -330,86 +336,116 @@
         },
            {
             'type': 'input',
             'name': 'dir_format',
             'message':"dir_format: ",
             'long_instruction': 'What format do you want for download directories',
             'default': config.get_dirformat(config_),
-             "validate":prompt_functions.dirformatvalidator()
+             "validate":prompt_validators.dirformatvalidator()
         },
               {
             'type': 'input',
             'name': 'file_format',
             'message': 'What format do you want for downloaded files',
             'default':config.get_fileformat(config_),
-             "validate":prompt_functions.fileformatvalidator()
+             "validate":prompt_validators.fileformatvalidator()
         },
                      {
             'type': 'number',
             'name': 'textlength',
             'message':"textlength: ",
             'long_instruction': 'Enter the max length to extract for post text, 0 means unlimited\n',
             'default': config.get_textlength(config_),
             'min_allowed':0,
              "validate":EmptyInputValidator()
         },
+                {
+        'type': 'input',
+            'name': 'space-replacer',
+            'message':"space-replacer: ",
+            'long_instruction': 'Replace any spaces in text with this character\n',
+            'default': config.get_spacereplacer(config_),
+             "validate":EmptyInputValidator()
+        },
          {
             'type': 'input',
             'name': 'date',
             'message': 'date: ',
             "long_instruction":"Enter Date format",
             'default': config.get_date(config_),
-             "validate":prompt_functions.dateplaceholdervalidator()
+             "validate":prompt_validators.dateplaceholdervalidator()
         },
         {
             'type': 'input',
             'name': 'metadata',
             "message":"metadata: ",
             'long_instruction': 'Where should metadata files be saved',
             'default':config.get_metadata(config_),
-             "validate":prompt_functions.metadatavalidator()
+             "validate":prompt_validators.metadatavalidator()
         },
         {
             'type': 'checkbox',
             'name': 'filter',
             "message":"filter: ",
             'choices':list(map(lambda x:Choice(name=x,value=x, enabled=x.capitalize() in set(config.get_filter(config_))),constants.FILTER_DEFAULT)),
-             "validate":prompt_functions.emptyListValidator()
+             "validate":prompt_validators.emptyListValidator()
+        },
+        {
+            'type': 'number',
+            'name': 'threads',
+            "message":"Number of Download Theads: ",
+            'min_allowed':1,
+            'max_allowed':10,
+             "validate":EmptyInputValidator(),
+             'long_instruction':"Value can be 1-10",
+             'default':config.get_threads(config_),
+        },
+          {
+            'type': 'list',
+            'name':"code-execution",
+            'message': "Enable Code Execution:",
+            'choices':[Choice(True,"Yes"),Choice(False,"No",enabled=True)],
+            "default":config.get_allow_code_execution(config_),
+            "long_instruction":"Be careful if turning this on this only effects file_format,metadata, and dir_format"
+
+
         },
 
+
+
         {
             'type': 'filepath',
             'name': 'mp4decrypt',
             "message":"mp4decrypt path: ",
-             "validate":PathValidator() and  EmptyInputValidator() and prompt_functions.mp4decryptvalidator(),
+             "validate":prompt_validators.MultiValidator(EmptyInputValidator(),prompt_validators.mp4decryptpathvalidator(),prompt_validators.mp4decryptexecutevalidator()),
             "default":config.get_mp4decrypt(config_),
             "long_instruction":             """
 Certain content requires decryption to process please provide the full path to mp4decrypt
 Linux version [mp4decrypt] and windows version [mp4decrypt.exe] are provided in the repo         
 """
         },
         {
                         'type': 'filepath',
             'name': 'ffmpeg',
             "message":"ffmpeg path: ",
-             "validate":PathValidator() and  EmptyInputValidator() and prompt_functions.ffmpegvalidator(),
+             "validate":prompt_validators.MultiValidator(EmptyInputValidator(),prompt_validators.ffmpegpathvalidator(),prompt_validators.ffmpegexecutevalidator()),
              "long_instruction": 
              """
 Certain content requires decryption to process please provide the full path to ffmpeg
 Linux version [ffmpeg] and windows version [ffmpeg.exe] are provided in the repo         
 """,
 "default":config.get_ffmpeg(config_)
         
         },
 
         {
             'type': 'input',
             'name': 'discord',
             "message":"discord webhook: ",
-             "validate":prompt_functions.DiscordValidator(),
+             "validate":prompt_validators.DiscordValidator(),
              "default":config.get_discord(config_)
         },
   
     ]
 
     questions2 = [
         {
@@ -521,15 +557,15 @@
     return answer[name]
 def mp4_prompt(config_):
     questions = [
          {
             'type': 'filepath',
             'name': 'mp4decrypt',
             "message":"mp4decrypt path: ",
-             "validate":PathValidator() and  EmptyInputValidator() and prompt_functions.mp4decryptvalidator(),
+             "validate":prompt_validators.MultiValidator(EmptyInputValidator(),prompt_validators.mp4decryptpathvalidator(),prompt_validators.mp4decryptexecutevalidator()),
              "long_instruction": 
              """
 Certain content requires decryption to process please provide the full path to mp4decrypt
 Linux version [mp4decrypt] and windows version [mp4decrypt.exe] are provided in the repo
 
 https://www.bento4.com/documentation/mp4decrypt/
 """,
@@ -542,104 +578,219 @@
 
 def ffmpeg_prompt(config_):
     questions = [
          {
             'type': 'filepath',
             'name': 'ffmpeg',
             "message":"ffmpeg path: ",
-             "validate":PathValidator() and  EmptyInputValidator() and prompt_functions.ffmpegvalidator(),
+             "validate":prompt_validators.MultiValidator(EmptyInputValidator(),prompt_validators.ffmpegpathvalidator(),prompt_validators.ffmpegexecutevalidator()),
              "long_instruction": 
              """
 Certain content requires decryption to process please provide the full path to ffmpeg
 Linux version [ffmpeg] and windows version [ffmpeg.exe] are provided in the repo 
 
 https://ffmpeg.org/download.html
 """,
 "default":config.get_ffmpeg(config_)
         },
     ]
 
     answer = prompt(questions)
     return answer["ffmpeg"] 
+def auto_download_mp4_decrypt()-> bool:
+    name = 'manual download'
+    questions = [
+        {
+            'type': 'list',
+            'name': name,
+            'message': "mp4decrypt not found would you like to auto install?",
+            'choices':["Yes","No"]
+        }
+    ]
+
+    answer = prompt(questions)
+    return answer[name]
+
+def auto_download_ffmpeg()-> bool:
+    name = 'manual download'
+    questions = [
+        {
+            'type': 'list',
+            'name': name,
+            'message': "ffmpeg not found would you like to auto install?",
+            'choices':["Yes","No"]
+        }
+    ]
+
+    answer = prompt(questions)
+    return answer[name]
 
 def continue_prompt() -> bool:
     name = 'reset username'
     questions = [
         {
             'type': 'list',
             'name': name,
             'message': "Do you want to continue with script",
             'choices':["Yes","No"]
         }
     ]
 
     answer = prompt(questions)
     return answer[name]
-def model_selector(models) -> bool:
-    questions = [
-    {"type": "fuzzy", "message": "Which models do you want to scrape:",
-      "keybindings":{
-                             "toggle": [{"key": "s-right"},{"key": ["pagedown","right"]},{"key": ["home","right"]}],
-
-                              
-                         }
-                         
-     ,"multiselect":True
-      ,"validate":prompt_functions.emptyListValidator(),
-      "instruction":prompt_strings.FUZZY_INSTRUCTION,
-      "choices":list(map(lambda x:Choice(x,name=f"{x['name']} {x['date'] } {x['active']}")   ,sorted(models,key=lambda x:x['name']))),"transformer":lambda result:",".join(map(lambda x:x.split(" ")[0],result))
-       ,"prompt":'Filter: ',
-       "marker":"\u25c9 ",
-       "marker_pl":"\u25cb "
-
-      },
+def model_selector(models,selected=None) -> bool:
+    choices=list(map(lambda x:model_selectorHelper(x[0],x[1])  ,enumerate(models)))
+    selectedSet=set(map(lambda x:re.search("^[0-9]+: ([^ ]+)",x["name"]).group(1),selected or []))
+    for model in choices:
+        name=re.search("^[0-9]+: ([^ ]+)",model.name).group(1)
+        if name in selectedSet:
+            model.enabled=True
+    
+    style=get_style({
+     "questionmark": "fg:#e5c07b bg:#ffffff",
+    "answermark": "#e5c07b",
+    "answer": "#61afef",
+    "input": "#98c379",
+    "question": "",
+    "answered_question": "",
+    "instruction": "#abb2bf",
+    "long_instruction": "#abb2bf",
+    "pointer": "#61afef",
+    "checkbox": "#98c379",
+    "separator": "",
+    "skipped": "#5c6370",
+    "validator": "",
+    "marker": "#e5c07b",
+    "fuzzy_prompt": "#c678dd",
+    "fuzzy_info": "#abb2bf",
+    "fuzzy_border": "#4b5263",
+    "fuzzy_match": "#c678dd bold",
+    "spinner_pattern": "#e5c07b",
+    "spinner_text": "",
+})
+
+    p=inquirer.fuzzy(
+        long_instruction=prompt_strings.FUZZY_INSTRUCTION.format(sort=args_.getargs().sort.capitalize(),
+                                                                 desc=args_.getargs().desc,
+                                                                 type=(args_.getargs().account_type or "All").capitalize(),
+                                                                status=(args_.getargs().sub_status or "Both").capitalize(),
+                                                                renewal=(args_.getargs().renewal or "Both").capitalize()
+
+                                                                
+                                                                ),
+
+                                                                 
+        choices=choices,
+        transformer=lambda result:",".join(map(lambda x:x.split(" ")[0],result)),
+        multiselect=True,
+        validate=prompt_validators.emptyListValidator(),
+        prompt='Filter: ',
+        marker="\u25c9 ",
+        marker_pl="\u25cb ",
+        message= "Which models do you want to scrape\n:",
+        mandatory=False,
+        style=style,
+        keybindings=  {
+                                "toggle": [{"key": "s-right"},{"key": ["pagedown","right"]},{"key": ["home","right"]}],
+
+                                
+                        }
+                            
     
-]
+    )
+        
+    answers=p.execute()
+    return answers,p
+        
 
-    return prompt(questions)[0]
+def model_selectorHelper(count,x):
+    format='YYYY-MM-DD'
+    expired=arrow.get(x['expired']).format(format) if x['expired'] else None
+    renewed=arrow.get(x['renewed']).format(format)  if x['renewed'] else None
+    subscribed=arrow.get(x['subscribed']).format(format)  if x['subscribed'] else None
+    price=x["price"] if x["price"]!=None else "Unknown"
+    name=x["name"]
+    active=x["active"]
+
+    return Choice(x,name=f"{count+1}: {name}  renewed={renewed}  subdate={subscribed}  exprdate={expired} subprice={price} active={active}")
+    
 
 
 
-def decide_filters_prompts():
+def decide_filters_prompt():
     questions = [
         {
             'type': 'list',
             'message': "Modify filters for your accounts list?\nSome usage examples are scraping free accounts only or paid accounts without renewal",
             'choices':["Yes","No"]
         }
     ]
 
     answer = prompt(questions)
     return answer[0]
 def modify_filters_prompt(args):
     questions = [
         {
             'type': 'list',
-            'message': "Filter account by renewal of subscription status",
+            'message': "Filter account by whether it has a renewal date",
             'choices':[Choice("active","Active Only"),Choice("disabled","Disabled Only"),Choice(None,"Both")]
         },
         {
             'type': 'list',
             'message': "Filter accounts based on access to content via a subscription",
             'choices':[Choice("active","Active Only"),Choice("expired","Expired Only"),Choice(None,"Both")]
         },
 
      
             {
             'type': 'list',
             'message': "Filter accounts by the type of subscription",
-            'choices':[Choice("paid","Paid Only"),Choice("free","Free Only"),Choice(None,"Both")]
+            'choices':[Choice("paid","Paid Subscription Only"),Choice("free","Free Subscription Only"),Choice(None,"Both")]
         }
     ]
     answer = prompt(questions)
     args.renewal=answer[0]
     args.sub_status=answer[1]
     args.account_type=answer[2]
     return args
 
+
+def decide_sort_prompt():
+    questions = [
+        {
+            'type': 'list',
+            'message': f"Change the Order or the Criteria for how the model list is sorted\nCurrent setting are {'Ascending' if not args_.getargs().desc else 'Descending'} in {args_.getargs().sort.capitalize()} order",
+            'choices':["Yes","No"]
+        }
+    ]
+
+    answer = prompt(questions)
+    return answer[0]
+def modify_sort_prompt(args):
+    questions = [
+        {
+            'type': 'list',
+            'message': "Sort Accounts by..",
+            'choices':[Choice("name","By Name"),Choice("subscribed","Subscribed Date"),Choice("expired","Expiring Date"),Choice("price","Price")],
+        },
+        {
+            'type': 'list',
+            'message': "Sort Direction",
+            'choices':[Choice(True,"Ascending"),Choice(False,"Descending",enabled=True)],
+            "default":True
+
+        },
+
+    ]
+
+    answer = prompt(questions)
+    args.sort=answer[0]
+    args.desc=answer[1]==False
+    return args
+
 def change_default_profile() -> bool:
     name = 'reset username'
     questions = [
         {
             'type': 'list',
             'name': name,
             'message': "Set this as the new default profile",
```

### Comparing `ofscraper-2.1/ofscraper/scraper.py` & `ofscraper-2.4/ofscraper/commands/scraper.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,271 +15,223 @@
 import platform
 import time
 import traceback
 import schedule
 import threading
 import queue
 import logging
-import textwrap
 from contextlib import contextmanager
 import timeit
 from itertools import chain
-import re
-from rich.console import Console
-import webbrowser
 import arrow
-from rich.progress import (
-    Progress,
-    TextColumn,
-    SpinnerColumn
-)
-from rich.style import Style
-
 import ofscraper.prompts.prompts as prompts
 import ofscraper.api.messages as messages
 import ofscraper.db.operations as operations
 import ofscraper.api.posts as posts_
 import ofscraper.utils.args as args_
 import ofscraper.utils.paths as paths
 import ofscraper.utils.exit as exit
 import ofscraper.api.paid as paid
 import ofscraper.api.highlights as highlights
 import ofscraper.api.timeline as timeline
 import ofscraper.api.profile as profile
 import ofscraper.utils.config as config
-import ofscraper.api.subscriptions as subscriptions
-import ofscraper.api.me as me
 import ofscraper.utils.auth as auth
 import ofscraper.utils.profiles as profiles
 import ofscraper.api.init as init
 import ofscraper.utils.download as download
 import ofscraper.interaction.like as like
 import ofscraper.utils.logger as logger
 import ofscraper.utils.args as args_
 import ofscraper.utils.filters as filters
 import ofscraper.utils.stdout as stdout
 import ofscraper.utils.console as console
+import ofscraper.api.archive as archive
+import ofscraper.api.pinned as pinned
+import ofscraper.utils.userselector as userselector
+import ofscraper.utils.console as console
 
-log=logger.init_logger(logging.getLogger(__package__))
+log=logging.getLogger(__package__)
 args=args_.getargs()
 log.debug(args)
 def process_messages(headers, model_id,username):
     with stdout.lowstdout():
-        with Progress(  SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}")) as progress:
-
-            messages_ =asyncio.run(messages.get_messages(headers,  model_id)) 
-            messages_=list(map(lambda x:posts_.Post(x,model_id,username),messages_))
-            log.debug(f"[bold]Messages Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),messages_))}")
-            log.debug("Removing locked messages media")
-            for message in messages_:
-                operations.write_messages_table(message)
-            output=[]
-            [ output.extend(message.media) for message in messages_]
-            return list(filter(lambda x:isinstance(x,posts_.Media),output))
+        messages_ =asyncio.run(messages.get_messages(headers,  model_id)) 
+        messages_=list(map(lambda x:posts_.Post(x,model_id,username),messages_))
+        log.debug(f"[bold]Messages Media Count with locked[/bold] {sum(map(lambda x:len(x.post_media),messages_))}")
+        log.debug("Removing locked messages media")
+        for message in messages_:
+            operations.write_messages_table(message)
+        output=[]
+        [ output.extend(message.media) for message in messages_]
+        return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
 def process_paid_post(model_id,username):
     with stdout.lowstdout():
-        with Progress(  SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}")) as progress:
-            task1=progress.add_task("Getting Paid Media....")
-            paid_content=paid.scrape_paid(username)
-            paid_content=list(map(lambda x:posts_.Post(x,model_id,username,responsetype="paid"),paid_content))
-            log.debug(f"[bold]Paid Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),paid_content))}")
-            log.debug("Removing locked paid media")
-            for post in paid_content:
-                operations.write_post_table(post,model_id,username)
-            output=[]
-            [output.extend(post.media) for post in paid_content]
-            progress.remove_task(task1)
-            return list(filter(lambda x:isinstance(x,posts_.Media),output))
+        paid_content=asyncio.run(paid.get_paid_posts(username,model_id))
+        paid_content=list(map(lambda x:posts_.Post(x,model_id,username,responsetype="paid"),paid_content))
+        log.debug(f"[bold]Paid Media Count with locked[/bold] {sum(map(lambda x:len(x.post_media),paid_content))}")
+        log.debug("Removing locked paid media")
+        for post in paid_content:
+            operations.write_post_table(post,model_id,username)
+        output=[]
+        [output.extend(post.media) for post in paid_content]
+        return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
          
 
 def process_highlights(headers, model_id,username):
     with stdout.lowstdout():
-        with Progress(  SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}")) as progress:
-            task1=progress.add_task("Highlights and Stories....")
-            highlights_, stories = highlights.scrape_highlights(headers, model_id)
-            highlights_, stories=list(map(lambda x:posts_.Post(x,model_id,username,responsetype="highlights"),highlights_)),\
-            list(map(lambda x:posts_.Post(x,model_id,username,responsetype="stories"),stories))
-            log.debug(f"[bold]Combined Story and Highlight Media count[/bold] {sum(map(lambda x:len(x.allmedia), highlights_))+sum(map(lambda x:len(x.allmedia), stories))}")
-            for post in highlights_:
-                operations.write_stories_table(post,model_id,username)
-            for post in stories:
-                operations.write_stories_table(post,model_id,username)   
-            output=[]
-            output2=[]
-            [ output.extend(highlight.media) for highlight in highlights_]
-            [ output2.extend(stories.media) for stories in stories]
-            progress.remove_task(task1)
-            return list(filter(lambda x:isinstance(x,posts_.Media),output)),list(filter(lambda x:isinstance(x,posts_.Media),output2))
+        highlights_, stories = asyncio.run(highlights.get_highlight_post(headers, model_id))
+        highlights_, stories=list(map(lambda x:posts_.Post(x,model_id,username,responsetype="highlights"),highlights_)),\
+        list(map(lambda x:posts_.Post(x,model_id,username,responsetype="stories"),stories))
+        log.debug(f"[bold]Combined Story and Highlight Media count[/bold] {sum(map(lambda x:len(x.post_media), highlights_))+sum(map(lambda x:len(x.post_media), stories))}")
+        for post in highlights_:
+            operations.write_stories_table(post,model_id,username)
+        for post in stories:
+            operations.write_stories_table(post,model_id,username)   
+        output=[]
+        output2=[]
+        [ output.extend(highlight.media) for highlight in highlights_]
+        [ output2.extend(stories.media) for stories in stories]
+        return list(filter(lambda x:isinstance(x,posts_.Media),output)),list(filter(lambda x:isinstance(x,posts_.Media),output2))
 
-            
+        
 
 
 
 
 
 
 def process_timeline_posts(headers, model_id,username):
     with stdout.lowstdout():
-        with Progress(  SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}")) as progress:
-            timeline_posts = asyncio.run(timeline.get_timeline_post(headers, model_id))
-            timeline_posts  =list(map(lambda x:posts_.Post(x,model_id,username,"timeline"), timeline_posts ))
-            log.debug(f"[bold]Timeline Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),timeline_posts))}")
-            log.debug("Removing locked timeline media")
-            for post in timeline_posts:
-                operations.write_post_table(post,model_id,username)
-            output=[]
-            [output.extend(post.media) for post in  timeline_posts ]
-            return list(filter(lambda x:isinstance(x,posts_.Media),output))
+        timeline_posts = asyncio.run(timeline.get_timeline_post(headers, model_id))
+        timeline_posts  =list(map(lambda x:posts_.Post(x,model_id,username,"timeline"), timeline_posts ))
+        log.debug(f"[bold]Timeline Media Count with locked[/bold] {sum(map(lambda x:len(x.post_media),timeline_posts))}")
+        log.debug("Removing locked timeline media")
+        for post in timeline_posts:
+            operations.write_post_table(post,model_id,username)
+        output=[]
+        [output.extend(post.media) for post in  timeline_posts ]
+        return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
 def process_archived_posts(headers, model_id,username):
     with stdout.lowstdout():
-        with Progress(  SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}")) as progress:
-            task1=progress.add_task("Getting Archived Media....")
-            archived_posts = timeline.get_archive_post(headers, model_id)
-            archived_posts =list(map(lambda x:posts_.Post(x,model_id,username),archived_posts ))
-            log.debug(f"[bold]Archived Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),archived_posts))}")
-            log.debug("Removing locked archived media")
+        archived_posts = asyncio.run(archive.get_archived_post(headers, model_id))
+        archived_posts =list(map(lambda x:posts_.Post(x,model_id,username),archived_posts ))
+        log.debug(f"[bold]Archived Media Count with locked[/bold] {sum(map(lambda x:len(x.post_media),archived_posts))}")
+        log.debug("Removing locked archived media")
 
-            for post in archived_posts:
-                operations.write_post_table(post,model_id,username)
-            output=[]
-            [ output.extend(post.media) for post in archived_posts ]
-            progress.remove_task(task1)
-            return list(filter(lambda x:isinstance(x,posts_.Media),output))
+        for post in archived_posts:
+            operations.write_post_table(post,model_id,username)
+        output=[]
+        [ output.extend(post.media) for post in archived_posts ]
+        return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
 
 
 
 def process_pinned_posts(headers, model_id,username):
     with stdout.lowstdout():
-        with Progress(  SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}")) as progress:
-            task1=progress.add_task("Getting Pinned Media....")
-            pinned_posts = timeline.get_pinned_post(headers, model_id,username)
-            pinned_posts =list(map(lambda x:posts_.Post(x,model_id,username,"pinned"),pinned_posts ))
-            log.debug(f"[bold]Pinned Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),pinned_posts))}")
-            log.debug("Removing locked pinned media")
-            for post in  pinned_posts:
-                operations.write_post_table(post,model_id,username)
-            output=[]
-            [ output.extend(post.media) for post in pinned_posts ]
-            progress.remove_task(task1)
-            return list(filter(lambda x:isinstance(x,posts_.Media),output))
+        pinned_posts = asyncio.run(pinned.get_pinned_post(headers, model_id))
+        pinned_posts =list(map(lambda x:posts_.Post(x,model_id,username,"pinned"),pinned_posts ))
+        log.debug(f"[bold]Pinned Media Count with locked[/bold] {sum(map(lambda x:len(x.post_media),pinned_posts))}")
+        log.debug("Removing locked pinned media")
+        for post in  pinned_posts:
+            operations.write_post_table(post,model_id,username)
+        output=[]
+        [ output.extend(post.media) for post in pinned_posts ]
+        return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
 def process_profile(headers, username) -> list:
     with stdout.lowstdout():
         user_profile = profile.scrape_profile(headers, username)
         urls, info = profile.parse_profile(user_profile)
         profile.print_profile_info(info)       
         output=[]
         for ele in enumerate(urls):
             count=ele[0]
             data=ele[1]
             output.append(posts_.Media({"url":data["url"],"type":data["mediatype"]},count,posts_.Post(data,info[2],username,responsetype="profile")))
-        avatars=list(filter(lambda x:x.filename=='avatar',output))
+        avatars=list(filter(lambda x:x.filename.find('avatar')!=-1,output))
         if len(avatars)>0:
             log.warning(f"Avatar : {avatars[0].url}")
         return output
 
+def process_all_paid():
+    with stdout.lowstdout():
+        paid_content=asyncio.run(paid.get_all_paid_posts())
+        user_dict={}
+        post_array=[]
+        headers = auth.make_headers(auth.read_auth())
+        [user_dict.update({(ele.get("fromUser",None) or ele.get("author",None) or {} ).get("id"):user_dict.get((ele.get("fromUser",None) or ele.get("author",None) or {} ).get("id"),[])+[ele]}) for ele in paid_content]
+
+        for model_id,value in user_dict.items():
+            username=profile.scrape_profile(headers,model_id).get("username")
+            if username=="modeldeleted":
+                username=operations.get_profile_info(model_id,username) or username
+            log.info(f"Processing {username}_{model_id}")
+            operations.create_tables(model_id,username)
+            log.debug(f"Created table for {username}")
+            new_posts=list(map(lambda x:posts_.Post(x,model_id,username,responsetype="paid"),value))
+            post_array.extend(new_posts)
+            [operations.write_post_table(post,model_id,username) for post in new_posts]
+            log.debug(f"Added Paid media for {username}_{model_id}")
+
+                     
+        log.debug(f"[bold]Paid Media for all models[/bold] {sum(map(lambda x:len(x.media),post_array))}")
+        output=[]
+        [output.extend(post.media) for post in post_array]
+        return output
 
 
 def process_areas(headers, ele, model_id) -> list:
     args.posts = list(map(lambda x:x.capitalize(),(args.posts or prompts.areas_prompt())
 ))
     timeline_posts_dicts  = []
     pinned_post_dict=[]
     archived_posts_dicts  = []
     highlights_dicts  = []
     messages_dicts  = []
     stories_dicts=[]
     purchased_dict=[]
     pinned_post_dict=[]
+    profile_dicts=[]
 
-    username=ele['name']
-    profile_dicts  = process_profile(headers,username)
 
-     
-    if ('Pinned' in args.posts or 'All' in args.posts) and ele["active"]:
+    username=ele['name']
+    if "NONE" in args.posts:
+        return []
+  
+    if ('Profile' in args.posts or 'All' in args.posts):
+        profile_dicts  = process_profile(headers,username)
+    if ('Pinned' in args.posts or 'All' in args.posts):
             pinned_post_dict = process_pinned_posts(headers, model_id,username)
-    if ('Timeline' in args.posts or 'All' in args.posts) and ele["active"]:
+    if ('Timeline' in args.posts or 'All' in args.posts):
             timeline_posts_dicts = process_timeline_posts(headers, model_id,username)
-    if ('Archived' in args.posts or 'All' in args.posts) and ele["active"]:
+    if ('Archived' in args.posts or 'All' in args.posts):
             archived_posts_dicts = process_archived_posts(headers, model_id,username)
     if 'Messages' in args.posts or 'All' in args.posts:
             messages_dicts = process_messages(headers, model_id,username)
     if "Purchased" in args.posts or "All" in args.posts:
             purchased_dict=process_paid_post(model_id,username)
-    if ('Highlights'  in args.posts or 'Stories'  in args.posts or 'All' in args.posts)   and ele["active"]:
+    if ('Highlights'  in args.posts or 'Stories'  in args.posts or 'All' in args.posts):
             highlights_tuple = process_highlights(headers, model_id,username)  
             if 'Highlights'  in args.posts:
                 highlights_dicts=highlights_tuple[0]
             if 'Stories'  in args.posts:
                 stories_dicts=highlights_tuple[1]   
             if 'All' in args.posts:
                 highlights_dicts=highlights_tuple[0]
                 stories_dicts=highlights_tuple[1]               
     return filters.filterMedia(list(chain(*[profile_dicts  , timeline_posts_dicts ,pinned_post_dict,purchased_dict,
             archived_posts_dicts , highlights_dicts , messages_dicts,stories_dicts]))
 
 )
 
-
-        
-
-
-
-def get_usernames(parsed_subscriptions: list) -> list:
-    usernames = [sub[0] for sub in parsed_subscriptions]
-    log.debug(f"[bold]Usernames on account:[/bold] {usernames}")
-    return usernames
-
-
-def get_model(parsed_subscriptions: list) -> tuple:
-    """
-    Prints user's subscriptions to console and accepts input from user corresponding 
-    to the model(s) whose content they would like to scrape.
-    """
-    return prompts.model_selector(parsed_subscriptions)
-
-  
-def get_model_inputsplit(commaString):
-    def hyphenRange(hyphenString):
-        x = [int(x) for x in hyphenString.split('-')]
-        return range(x[0], x[-1]+1)
-    return chain(*[hyphenRange(r) for r in list(filter(lambda x:x.isdigit(),re.split(',| ',commaString)))])
-
-def get_models(headers, subscribe_count) -> list:
-    """
-    Get user's subscriptions in form of a list.
-    """
-    with stdout.lowstdout():
-        with Progress(  SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}")) as progress:
-            task1=progress.add_task('Getting your subscriptions (this may take awhile)...')
-            list_subscriptions = asyncio.run(
-                subscriptions.get_subscriptions(headers, subscribe_count))
-            parsed_subscriptions = subscriptions.parse_subscriptions(
-                list_subscriptions)
-            progress.remove_task(task1)
-            return parsed_subscriptions
-
-#check if auth is valid
-def process_me(headers):
-    my_profile = me.scrape_user(headers)
-    name, username = me.parse_user(my_profile)
-    subscribe_count=me.parse_subscriber_count(headers)
-    me.print_user(name, username)
-    return subscribe_count
-
-def setfilter():
-    if prompts.decide_filters_prompts()=="Yes":
-        global args
-        args=prompts.modify_filters_prompt(args)
-        args_.changeargs(args)
-
 def process_prompts():
     
     while  True:
         args.posts=[]
         result_main_prompt = prompts.main_prompt()
      
         #download
@@ -341,94 +293,127 @@
                 profiles.print_profiles()
         if prompts.continue_prompt()=="No":
             break
   
         
 
 
+
+
+
+
+
 def process_post():
-    with scrape_context_manager():
+    if args.users_first:
+         process_post_user_first()
+    else:
+        normal_post_process()
+           
+def process_post_user_first():
+     with scrape_context_manager():
         profiles.print_current_profile()
         headers = auth.make_headers(auth.read_auth())
         init.print_sign_status(headers)
-        userdata=getselected_usernames()
+        userdata=userselector.getselected_usernames()
         length=len(userdata)
         if args.users_first:
-            eleDict={}
+            output=[]
             for count,ele in enumerate(userdata):
-                key=ele['name']
-                eleDict[key]={}
-                eleDict[key]["name"]=ele['name']
                 log.debug(f"getting content for {count+1}/{length} model")
                 if args.posts:
                     log.info(f"Getting {','.join(args.posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
                 try:
                     model_id = profile.get_id(headers, ele["name"])
-                    eleDict[key]["id"]=model_id
-                    create_tables(model_id,ele['name'])
+                    operations.create_tables(model_id,ele['name'])
                     operations.write_profile_table(model_id,ele['name'])
-                    eleDict[key]["combined"]=process_areas(headers, ele, model_id)
-                
+                    output.extend(process_areas(headers, ele, model_id)) 
+                    if args.scrape_paid:
+                        output.extend(process_all_paid())
                 except Exception as e:
                     log.traceback(f"failed with exception: {e}")
-                    log.traceback(traceback.format_exc())      
-            for key in eleDict.keys():
-                try:
+                    log.traceback(traceback.format_exc())               
+                user_dict={}
+                [user_dict.update({ele.post.model_id:user_dict.get(ele.post.model_id,[])+[ele]}) for ele in output]
+                for value in user_dict.values():
+                    model_id =value[0].post.model_id
+                    username=value[0].post.username
+                    operations.create_tables(model_id,username)
+                    operations.write_profile_table(model_id,username)
                     asyncio.run(download.process_dicts(
-                        eleDict[key]["name"],
-                        eleDict[key]["id"],
-                        eleDict[key]["combined"],
-                        forced=args.dupe,
-                        ))
-                except Exception as e:
-                    log.traceback(f"failed with exception: {e}")
-                    log.traceback(traceback.format_exc())   
-        else:
-            for count,ele in enumerate(userdata):
-                log.debug(f"Getting content+downloading {count+1}/{length} model")
-
-                if args.posts:
-                    log.info(f"Getting {','.join(args.posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
-                try:
-                    model_id = profile.get_id(headers, ele["name"])
-                    create_tables(model_id,ele['name'])
-                    operations.write_profile_table(model_id,ele['name'])
-                    combined_urls=process_areas(headers, ele, model_id)
+                    username,
+                    model_id,
+                    value,
+                    forced=args.dupe,
+                    ))  
+def normal_post_process():
+    with scrape_context_manager():
+        profiles.print_current_profile()
+        headers = auth.make_headers(auth.read_auth())
+        init.print_sign_status(headers)
+        userdata=userselector.getselected_usernames()
+        length=len(userdata)
+        for count,ele in enumerate(userdata):
+            log.debug(f"Getting content+downloading {count+1}/{length} model")
+            if args.posts:
+                log.info(f"Getting {','.join(args.posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
+            try:
+                model_id = profile.get_id(headers, ele["name"])
+                operations.create_tables(model_id,ele['name'])
+                operations.write_profile_table(model_id,ele['name'])
+                combined_urls=process_areas(headers, ele, model_id)
+                asyncio.run(download.process_dicts(
+                ele["name"],
+                model_id,
+                combined_urls,
+                forced=args.dupe,
+                ))
+            except Exception as e:
+                log.traceback(f"failed with exception: {e}")
+                log.traceback(traceback.format_exc())
+        
+        if args.scrape_paid:
+            try:
+                user_dict={}
+                [user_dict.update({ele.post.model_id:user_dict.get(ele.post.model_id,[])+[ele]}) for ele in process_all_paid()]
+                for value in user_dict.values():
+                    model_id =value[0].post.model_id
+                    username=value[0].post.username
+                    operations.create_tables(model_id,username)
+                    operations.write_profile_table(model_id,username)
                     asyncio.run(download.process_dicts(
-                    ele["name"],
+                    username,
                     model_id,
-                    combined_urls,
+                    value,
                     forced=args.dupe,
                     ))
-                except Exception as e:
-                    log.traceback(f"failed with exception: {e}")
-                    log.traceback(traceback.format_exc())
-        
-        
+            except Exception as e:
+                log.traceback(f"failed with exception: {e}")
+                log.traceback(traceback.format_exc())     
+            
 
 def process_like():
     with scrape_context_manager():
         profiles.print_current_profile()
         headers = auth.make_headers(auth.read_auth())
-        userdata=getselected_usernames()
+        userdata=userselector.getselected_usernames()
         with stdout.lowstdout():
             for ele in list(filter(lambda x: x["active"],userdata)):
                     model_id = profile.get_id(headers, ele["name"])
                     posts = like.get_posts(headers, model_id)
                     unfavorited_posts = like.filter_for_unfavorited(posts)  
                     unfavorited_posts=filters.timeline_array_filter(unfavorited_posts)             
                     post_ids = like.get_post_ids(unfavorited_posts)
                     like.like(headers, model_id, ele["name"], post_ids)
 
 def process_unlike():
     with scrape_context_manager(): 
         profiles.print_current_profile()
         headers = auth.make_headers(auth.read_auth())
         init.print_sign_status(headers)
-        userdata=getselected_usernames()
+        userdata=userselector.getselected_usernames()
         with stdout.lowstdout():
             for ele in list(filter(lambda x: x["active"],userdata)):
                     model_id = profile.get_id(headers, ele["name"])
                     posts = like.get_posts(headers, model_id)
                     favorited_posts = like.filter_for_favorited(posts)
                     favorited_posts=filters.timeline_array_filter(favorited_posts) 
                     post_ids = like.get_post_ids(favorited_posts)
@@ -442,15 +427,15 @@
 
 
 
 ## run script once or on schedule based on args
 def run(*functs):
     # get usernames prior to potentially supressing output
     check_auth()
-    getselected_usernames()
+    userselector.getselected_usernames()
    
     if args.output=="PROMPT":
         log.info(f"[bold]silent-mode on[/bold]")    
     if args.daemon:
         log.info(f"[bold]daemon mode on[/bold]")   
     run_helper(*functs)
 
@@ -491,90 +476,14 @@
         console.shared_console.print("You need to select path for ffmpeg\n\n")
         log.debug(f"[bold]current ffmpeg path[/bold] {config.get_ffmpeg(config.read_config())}")
         config.update_ffmpeg()
     log.debug(f"[bold]final mp4decrypt path[/bold] {config.get_mp4decrypt(config.read_config())}")
     log.debug(f"[bold]final ffmpeg path[/bold] {config.get_ffmpeg(config.read_config())}")
 
 
-def getselected_usernames():
-    #username list will be retrived once per daemon run
-    # manual prompt will need to recertify options every call
-    global selectedusers
-    scraper_bool=len(args.posts)>0 or args.action
-    #always return with correct args
-    if selectedusers and scraper_bool:
-            return selectedusers
-    if scraper_bool:
-        selectedusers=selectuserhelper()
-    #create in these situations
-    elif not selectedusers and not scraper_bool:
-        setfilter()
-        selectedusers=selectuserhelper()
-    elif selectedusers and not scraper_bool:
-        if prompts.reset_username_prompt()=="Yes":
-            setfilter()
-            selectedusers=selectuserhelper()
-    return selectedusers
-
-def selectuserhelper():
-    headers = auth.make_headers(auth.read_auth())
-    subscribe_count = process_me(headers)
-    parsed_subscriptions = get_models(headers, subscribe_count)
-    filter_subscriptions=filteruserHelper(parsed_subscriptions )
-    if args.username and "ALL" in args.username:
-        selectedusers=filter_subscriptions
-        
-    elif args.username:
-        userSelect=set(args.username)
-        selectedusers=list(filter(lambda x:x["name"] in userSelect,filter_subscriptions))
-    #manually select usernames
-    else:
-        selectedusers= get_model(filter_subscriptions)
-    return selectedusers
-
-        
-
-        
-
-                  
-    # else:
-    #     if len(args.posts)==0 or args.action:
-           
-
-  
-    # #remove dupes
-    return selectedusers
-def filteruserHelper(usernames):
-    #paid/free
-    filterusername=usernames
-    if args.account_type=="paid":
-        filterusername=list(filter(lambda x:x["data"]["subscribePrice"]>0,filterusername))
-    if args.account_type=="free":
-        filterusername=list(filter(lambda x:x["data"]["subscribePrice"]==0,filterusername))
-    if args.renewal=="active":
-        filterusername=list(filter(lambda x:x["data"]["subscribedOn"]==True,filterusername))     
-    if args.renewal=="disabled":
-        filterusername=list(filter(lambda x:x["data"]["subscribedOn"]==False,filterusername))      
-    if args.sub_status=="active":
-        filterusername=list(filter(lambda x:x["data"]["subscribedIsExpiredNow"]==False,filterusername))     
-    if args.sub_status=="expired":
-        filterusername=list(filter(lambda x:x["data"]["subscribedIsExpiredNow"]==True,filterusername))      
-    return filterusername
-
-
-def create_tables(model_id,username):
-    operations.create_post_table(model_id,username)
-    operations.create_message_table(model_id,username)
-    operations.create_media_table(model_id,username)
-    operations.create_products_table(model_id,username)
-    operations.create_others_table(model_id,username)
-    operations.create_profile_table(model_id,username)
-    operations.create_stories_table(model_id,username)
-
-
 
 @contextmanager
 def scrape_context_manager():
         
         # Before yield as the enter method
 
         start = timeit.default_timer()
@@ -600,14 +509,15 @@
         console.shared_console.print(
             f"[bold green]Welcome to OF-Scraper Version {args.version}[/bold green]"
         )                
 def main():
  
         try:
             print_start()
+            logger.start_discord_queue()
             scrapper()
             paths.cleanup()
             logger.discord_cleanup()
         except KeyboardInterrupt as E:
             try:
                 with exit.DelayedKeyboardInterrupt():
                     paths.cleanup()
@@ -633,22 +543,22 @@
     # try:
     #     webbrowser.open(donateEP)
     # except:
     #     pass
     global selectedusers
     selectedusers=None
     functs=[]
-    if len(args.posts)==0 and not args.action:
+    if len(args.posts)==0 and not args.action and not args.scrape_paid:
         if args.daemon:
                     log.error("You need to pass at least one scraping method\n--action\n--posts\n--purchase\nAre all valid options. Skipping and going to menu")
         process_prompts()
         return
     check_auth()
     check_config()
-    if len(args.posts)>0: 
+    if len(args.posts)>0 or args.scrape_paid: 
         functs.append(process_post)      
     elif args.action=="like":
         functs.append(process_like)
     elif args.action=="unlike":
         functs.append(process_unlike)
     run(*functs)
```

### Comparing `ofscraper-2.1/ofscraper/utils/auth.py` & `ofscraper-2.4/ofscraper/utils/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from urllib.parse import urlparse
 import requests
 from rich.console import Console
 import httpx
 import browser_cookie3
 from .profiles import get_current_profile
 from ..prompts.prompts import *
-from ..constants import configPath, authFile, DC_EP, requestAuth
+from ..constants import configPath, authFile, DYNAMIC, requestAuth
 
 console=Console()
 
 
 
 def read_auth():
     make_request_auth()
@@ -211,14 +211,15 @@
 
     checksum_indexes = content['checksum_indexes']
     checksum_constant = content['checksum_constant']
     checksum = sum(sha_1_b[i] for i in checksum_indexes) + checksum_constant
 
     final_sign = content['format'].format(sha_1_sign, abs(checksum))
 
+
     headers.update(
         {
             'sign': final_sign,
             'time': time2
         }
     )
     return headers
@@ -255,17 +256,17 @@
 
         with open(p / requestAuth, 'w') as f:
             f.write(json.dumps(request_auth, indent=4))
 
 
 def get_request_auth():
     with httpx.Client(http2=True) as c:
-        r = c.get(DC_EP)
+        r = c.get(DYNAMIC)
     if not r.is_error:
         content = r.json()
         static_param = content['static_param']
-        fmt = content['format']
+        fmt = f"{content['start']}:{{}}:{{:x}}:{content['end']}" 
         checksum_indexes = content['checksum_indexes']
         checksum_constant = content['checksum_constant']
         return (static_param, fmt, checksum_indexes, checksum_constant)
     else:
         return []
```

### Comparing `ofscraper-2.1/ofscraper/utils/config.py` & `ofscraper-2.4/ofscraper/utils/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,42 +7,45 @@
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 import json
 import pathlib
 import logging
-from rich.console import Console
 import ofscraper.constants as constants
 import ofscraper.prompts.prompts as prompts 
+import ofscraper.utils.binaries as binaries
+import ofscraper.utils.args as args_
+import ofscraper.utils.paths as paths_
+import ofscraper.utils.console as console_
 
-console=Console()
+console=console_.shared_console
 log=logging.getLogger(__package__)
 
 def read_config():
-    p = pathlib.Path.home() / constants.configPath
-    if not p.is_dir():
-        p.mkdir(parents=True, exist_ok=True)
+    p = pathlib.Path(paths_.get_config_path())
+    if not p.parent.is_dir():
+        p.parent.mkdir(parents=True, exist_ok=True)
 
     config = {}
     while True:
         try:
-            with open(p / constants.configFile, 'r') as f:
+            with open(p , 'r') as f:
                 configText=f.read()
                 config = json.loads(configText)
 
             try:
                 if [*config['config']] != [*get_current_config_schema(config)['config']]:
                     config = auto_update_config(p, config)
             except KeyError:
                 raise FileNotFoundError
 
             break
         except FileNotFoundError:
-            file_not_found_message = f"You don't seem to have a `config.json` file. One has been automatically created for you at: '{p / constants.configFile}'"
+            file_not_found_message = f"You don't seem to have a `config.json` file. One has been automatically created for you at: '{p}'"
             make_config(p)
             console.print(file_not_found_message)
         except json.JSONDecodeError as e:
             print("You config.json has a syntax error")
             if prompts.reset_config_prompt()=="Reset Default":
                 make_config(p)
             else:
@@ -50,31 +53,38 @@
                 try:
                     make_config(p, prompts.manual_config_prompt(configText))
                 except:
                    continue
     return config["config"]
 
 
-def get_current_config_schema(config: dict) -> dict:
-    config = config['config']
+def get_current_config_schema(config:dict=None) -> dict:
+    
+    if config:
+        config = config['config']
 
     new_config = {
         'config': {
             constants.mainProfile: get_main_profile(config),
             'save_location':get_save_location(config) ,
             'file_size_limit': get_filesize(config),
             'dir_format': get_dirformat(config),
             'file_format':get_fileformat(config),
             'textlength':get_textlength(config),
+            'space-replacer':get_spacereplacer(config),
             'date': get_date(config),
             "metadata": get_metadata(config),
             "filter":get_filter(config),
+            "threads":get_threads(config),
+                "code-execution":get_allow_code_execution(config),
+
             "mp4decrypt":get_mp4decrypt(config),
             "ffmpeg":get_ffmpeg(config),
              "discord":get_discord(config),
+
             "responsetype":{
            "timeline":get_timeline_responsetype(config),
          "message":get_messages_responsetype(config),
             "archived":get_archived_responsetype(config),
             "paid":get_paid_responsetype(config),
             "stories":get_stories_responsetype(config),
             "highlights":get_highlights_responsetype(config),
@@ -83,73 +93,48 @@
             }
         }
     }
     return new_config
 
 
 def make_config(path, config=None):
-    config = config or  {
-        'config': {
-            constants.mainProfile: constants.mainProfile,
-            'save_location': get_save_location(config),
-            'file_size_limit':get_filesize(config),
-            'dir_format':get_dirformat(config),
-            'file_format': get_fileformat(config),
-            'textlength':get_textlength(config),
-            'date':get_date(config),
-            'metadata':get_metadata(config),
-            "filter":get_filter(config),
-            "mp4decrypt":get_mp4decrypt(config=None),
-            "ffmpeg":get_ffmpeg(config),
-            "discord":get_discord(config=None),
-            "responsetype":{
-        "timeline":get_timeline_responsetype(config),
-         "message":get_messages_responsetype(config),
-            "archived":get_archived_responsetype(config),
-            "paid":get_paid_responsetype(config),
-            "stories":get_stories_responsetype(config),
-            "highlights":get_highlights_responsetype(config),
-            "profile":get_profile_responsetype(config),
-            "pinned":get_pinned_responsetype(config),
-
-            }
-        }
-    }
+    config = get_current_config_schema(config) 
+    
     if isinstance(config,str):
         config=json.loads(config)
+        
 
-    with open(path / constants.configFile, 'w') as f:
+    with open(path, 'w') as f:
         f.write(json.dumps(config, indent=4))
 
 
 def update_config(field: str, value):
-    p = pathlib.Path.home() / constants.configPath / constants.configFile
-
+    p = paths_.get_config_path() 
     with open(p, 'r') as f:
         config = json.load(f)
 
     config['config'].update({field: value})
 
     with open(p, 'w') as f:
         f.write(json.dumps(config, indent=4))
 
 
 def auto_update_config(path, config: dict) -> dict:
     log.error("Auto updating config...")
     new_config = get_current_config_schema(config)
 
-    with open(path / constants.configFile, 'w') as f:
+    with open(path , 'w') as f:
         f.write(json.dumps(new_config, indent=4))
 
     return new_config
 
 
 def edit_config():
     try:
-        p = pathlib.Path.home() / constants.configPath / constants.configFile
+        p = paths_.get_config_path() 
         with open(p, 'r') as f:
             configText=f.read()
             config = json.loads(configText)
 
         updated_config = {
             'config': prompts.config_prompt(config['config'])
         }
@@ -172,23 +157,29 @@
                         config = json.loads(configText)
                     break
                 except:
                     continue
 
 def update_mp4decrypt():
     config={"config":read_config()}
-    config["config"]["mp4decrypt"]=prompts.mp4_prompt(config)
-    p = pathlib.Path.home() / constants.configPath / constants.configFile
+    if prompts.auto_download_mp4_decrypt()=="Yes":
+        config["config"]["mp4decrypt"]=binaries.mp4decrypt_download()
+    else:
+        config["config"]["mp4decrypt"]=prompts.mp4_prompt(config["config"])
+    p = paths_.get_config_path() 
     with open(p, 'w') as f:
         f.write(json.dumps(config, indent=4))
 
 def update_ffmpeg():
     config={"config":read_config()}
-    config["config"]["ffmpeg"]=prompts.ffmpeg_prompt(config)
-    p = pathlib.Path.home() / constants.configPath / constants.configFile
+    if prompts.auto_download_ffmpeg()=="Yes":
+        config["config"]["ffmpeg"]=binaries.ffmpeg_download()
+    else:
+        config["config"]["ffmpeg"]=prompts.ffmpeg_prompt((config["config"]))
+    p = paths_.get_config_path() 
     with open(p, 'w') as f:
         f.write(json.dumps(config, indent=4))
 
     
 def get_save_location(config=None):
     if config==None:
         return constants.SAVE_PATH_DEFAULT   
@@ -225,19 +216,26 @@
     except:
         return 0
 
 def get_date(config=None):
     if config==None:
         return constants.DATE_DEFAULT     
     return config.get('date', constants.DATE_DEFAULT)
-
+def get_allow_code_execution(config=None):
+    if config==None:
+        return constants.CODE_EXECUTION_DEFAULT  
+    return config.get('code-execution', constants.CODE_EXECUTION_DEFAULT)
 def get_metadata(config=None):
     if config==None:
         return constants.METADATA_DEFAULT      
     return config.get('metadata', constants.METADATA_DEFAULT)
+def get_threads(config=None):
+    if config==None:
+        return constants.MP4DECRYPT_DEFAULT    
+    return int(config.get('threads', constants.THREADS_DEFAULT) or constants.THREADS_DEFAULT)
 
 def get_mp4decrypt(config=None):
     if config==None:
         return constants.MP4DECRYPT_DEFAULT    
     return config.get('mp4decrypt', constants.MP4DECRYPT_DEFAULT) or ""
 
 def get_ffmpeg(config=None):
@@ -295,8 +293,12 @@
         return constants.RESPONSE_TYPE_DEFAULT["profile"]       
     return config.get('responsetype',{}).get("profile") or constants.RESPONSE_TYPE_DEFAULT["profile"]
 
 
 def get_pinned_responsetype(config=None):
     if config==None:
         return constants.RESPONSE_TYPE_DEFAULT["pinned"]       
-    return config.get('responsetype',{}).get("pinned") or constants.RESPONSE_TYPE_DEFAULT["pinned"]
+    return config.get('responsetype',{}).get("pinned") or constants.RESPONSE_TYPE_DEFAULT["pinned"]
+def get_spacereplacer(config=None):
+    if config==None:
+        return " "      
+    return config.get('space-replacer'," ") or " "
```

### Comparing `ofscraper-2.1/ofscraper/utils/dates.py` & `ofscraper-2.4/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.1/ofscraper/utils/download.py` & `ofscraper-2.4/ofscraper/utils/download.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,19 +51,23 @@
 import ofscraper.utils.paths as paths
 import ofscraper.utils.auth as auth
 import ofscraper.constants as constants
 import ofscraper.utils.dates as dates
 import ofscraper.utils.logger as logger
 import ofscraper.utils.console as console
 import ofscraper.utils.stdout as stdout
+import ofscraper.utils.config as config_
+
 from diskcache import Cache
 
 cache = Cache(paths.getcachepath())
 attempt = contextvars.ContextVar("attempt")
 log=logging.getLogger(__package__)
+from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
+sem = semaphoreDelayed(config_.get_threads(config_.read_config()))
 
 
 async def process_dicts(username, model_id, medialist,forced=False):
     with stdout.lowstdout():
         overall_progress=Progress(  TextColumn("{task.description}"),
         BarColumn(),TaskProgressColumn(),TimeElapsedColumn())
         job_progress=Progress(TextColumn("{task.description}",table_column=Column(ratio=2)),BarColumn(),
@@ -71,20 +75,22 @@
         progress_group = Group(
         overall_progress
         , Panel(Group(job_progress,fit=True)))
         with Live(progress_group, refresh_per_second=constants.refreshScreen,console=console.shared_console):    
                 if not forced:
                     media_ids = set(operations.get_media_ids(model_id,username))
                     medialist = seperate.separate_by_id(medialist, media_ids)
+                    medialist=seperate.seperate_avatars(medialist)
+
                     log.info(f"Skipping previously downloaded\nMedia left for download {len(medialist)}")
                 else:
                     log.info("forcing all downloads")
                 file_size_limit = config_.get_filesize()
                 global sem
-                sem = asyncio.Semaphore(8)
+               
             
                 aws=[]
                 photo_count = 0
                 video_count = 0
                 audio_count=0
                 skipped = 0
                 total_bytes_downloaded = 0
@@ -122,22 +128,22 @@
                         overall_progress.update(task1,description=desc.format(
                                     p_count=photo_count, v_count=video_count, a_count=audio_count,skipped=skipped, data=data,mediacount=len(medialist), sumcount=video_count+audio_count+photo_count+skipped), refresh=True, advance=1)
         overall_progress.remove_task(task1)
     log.error(f'[bold]{username}[/bold] ({photo_count} photos, {video_count} videos, {audio_count} audios,  {skipped} skipped)' )
 def retry_required(value):
     return value == ('skipped', 1)
 
-@retry(retry=retry_if_result(retry_required),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=20, max=40),reraise=True) 
+@retry(retry=retry_if_result(retry_required),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True) 
 async def download(ele,path,model_id,username,file_size_limit,progress):
     attempt.set(attempt.get(0) + 1)
     
     try:
         if ele.url:
            return await main_download_helper(ele,path,file_size_limit,username,model_id,progress)
-        elif ele.mpd:  
+        elif ele.mpd:
             return await alt_download_helper(ele,path,file_size_limit,username,model_id,progress)
         else:
             return "skipped",1
     except Exception as e:
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] exception {e}")   
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] exception {traceback.format_exc()}")   
         return 'skipped', 1
@@ -188,25 +194,27 @@
             newDate=dates.convert_local_time(ele.postdate)
             log.debug(f"Media:{ele.id} Post:{ele.postid} Attempt to set Date to {arrow.get(newDate).format('YYYY-MM-DD HH:mm')}")  
             set_time(path_to_file,newDate )
             log.debug(f"Media:{ele.id} Post:{ele.postid} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}")  
 
         if ele.id:
             operations.write_media_table(ele,path_to_file,model_id,username)
+        set_cache_helper(ele)
         return ele.mediatype,total
 
 async def alt_download_helper(ele,path,file_size_limit,username,model_id,progress):
     async with sem:
         log.debug(f"Media:{ele.id} Post:{ele.postid} Downloading with protected media downloader")      
         log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {ele.filename} with {ele.mpd}")
         video = None
         audio = None
         base_url=re.sub("[0-9a-z]*\.mpd$","",ele.mpd,re.IGNORECASE)
-        mpd=ele.parse_mpd
-        path_to_file = paths.trunicate(pathlib.Path(path,f'{createfilename(ele,username,model_id,"mp4")}')) 
+        mpd=await ele.parse_mpd
+        path_to_file = paths.trunicate(pathlib.Path(path,f'{createfilename(ele,username,model_id,"mp4")}'))
+        temp_path=paths.trunicate(pathlib.Path(path,f"{ele.id}.mkv"))
 
         for period in mpd.periods:
             for adapt_set in filter(lambda x:x.mime_type=="video/mp4",period.adaptation_sets):             
                 kId=None
                 for prot in adapt_set.content_protections:
                     if prot.value==None:
                         kId = prot.pssh[0].pssh 
@@ -271,26 +279,32 @@
             return "skipped",1 
         log.debug(f"Media:{ele.id} Post:{ele.postid} got key")
         newpath=pathlib.Path(re.sub("\.part$","",str(item["path"]),re.IGNORECASE))
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] renaming {pathlib.Path(item['path']).absolute()} -> {newpath}")   
         subprocess.run([config_.get_mp4decrypt(config_.read_config()),"--key",key,str(item["path"]),str(newpath)])
         pathlib.Path(item["path"]).unlink(missing_ok=True)
         item["path"]=newpath
+    
     path_to_file.unlink(missing_ok=True)
-   
-    ffmpeg.output( ffmpeg.input(str(video["path"])), ffmpeg.input(str(audio["path"])), str(path_to_file),codec='copy',loglevel="quiet").overwrite_output().run(capture_stdout=True,cmd=config_.get_ffmpeg(config_.read_config()))
+    temp_path.unlink(missing_ok=True)
+    t=subprocess.run([config_.get_ffmpeg(config_.read_config()),"-i",str(video["path"]),"-i",str(audio["path"]),"-c","copy",str(temp_path)],stdout=subprocess.PIPE,stderr=subprocess.PIPE)
+    if t.stderr.decode().find("Output")==-1:
+        log.debug(t.stdout.decode())
+        log.debug(t.stderr.decode())
     video["path"].unlink(missing_ok=True)
     audio["path"].unlink(missing_ok=True)
+    shutil.move(temp_path,path_to_file)
     if ele.postdate:
         newDate=dates.convert_local_time(ele.postdate)
         log.debug(f"Media:{ele.id} Post:{ele.postid} Attempt to set Date to {arrow.get(newDate).format('YYYY-MM-DD HH:mm')}")  
         set_time(path_to_file,newDate )
         log.debug(f"Media:{ele.id} Post:{ele.postid} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}")  
     if ele.id:
         operations.write_media_table(ele,path_to_file,model_id,username)
+    set_cache_helper(ele)
     return ele.mediatype,total
 
 async def key_helper(pssh,licence_url,id):
     out=cache.get(licence_url)
     log.debug(f"ID:{id} pssh: {pssh!=None}")
     log.debug(f"ID:{id} licence: {licence_url}")
     if not out:
@@ -339,15 +353,36 @@
 def get_error_message(content):
     error_content = content.get('error', 'No error message available')
     try:
         return error_content.get('message', 'No error message available')
     except AttributeError:
         return error_content
 def createfilename(ele,username,model_id,ext):
-    if ele.responsetype =="profile":
-        return "{filename}.{ext}".format(ext=ext,filename=ele.filename)
-    return (config_.get_fileformat(config_.read_config())).format(filename=ele.filename,sitename="Onlyfans",site_name="Onlyfans",post_id=ele.id_,media_id=ele.id,first_letter=username[0],mediatype=ele.mediatype,value=ele.value,text=ele.text_,date=arrow.get(ele.postdate).format(config_.get_date(config_.read_config())),ext=ext,model_username=username,model_id=model_id,responsetype=ele.responsetype) 
-
-
-
+    filename=ele.filename
+    sitename="Onlyfans"
+    site_name="Onlyfans"
+    post_id=ele.postid_
+    media_id=ele.id
+    first_letter=username[0]
+    mediatype=ele.mediatype,
+    value=ele.value
+    text=ele.text_
+    date=arrow.get(ele.postdate).format(config_.get_date(config_.read_config()))
+    model_username=username
+    responsetype=ele.responsetype
+
+    if ele.responsetype_ =="profile":
+        return f"{filename}.{ext}"
+    elif config_.get_allow_code_execution(config_.read_config()):
+        return eval("f'{}'".format(config_.get_fileformat(config_.read_config())))
+    else:
+        return config_.get_fileformat(config_.read_config()).format(filename=filename,sitename=sitename,site_name=sitename,post_id=post_id,media_id=media_id,first_letter=first_letter,mediatype=mediatype,value=value,text=text,date=date,ext=ext,model_username=username,model_id=model_id,responsetype=responsetype) 
 
+    
 
+def set_cache_helper(ele):
+    if  ele.postid and ele.responsetype_=="profile":
+        cache.set(ele.postid ,True)
+        cache.close()
+    elif  ele.filename and ele.responsetype_=="highlights":
+        cache.set(ele.filename,True)
+        cache.close()
```

### Comparing `ofscraper-2.1/ofscraper/utils/encoding.py` & `ofscraper-2.4/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.1/ofscraper/utils/exit.py` & `ofscraper-2.4/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.1/ofscraper/utils/filters.py` & `ofscraper-2.4/ofscraper/utils/filters.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 
 import logging
+import re
 import arrow
 import ofscraper.utils.config as config
 import ofscraper.utils.args as args_
 
 args=args_.getargs()
 log=logging.getLogger(__package__)
 def filterMedia(media):
     media=dupefilter(media)
     media=post_datesorter(media)
     media=posts_type_filter(media)
     media=posts_date_filter(media)
+    media=post_timed_filter(media)
+    media=post_user_filter(media)
+    media=sort_media(media)
+    # if args.manual_download():
+    #     args.dupe=True
+    #     args_.changeargs(args)
+    #     media=post_manual_filter(media)
     return media
 
+def sort_media(media):
+    return sorted(media,key=lambda x:x.date)
+
+def post_manual_filter():
+    None
 
 def dupefilter(media):
     output=[]
     ids=set()
     log.info("Removing duplicate media")
     log.debug(f"[bold]Combined Media Count with dupes[/bold]  {len(media)}")
     for item in media:
@@ -61,7 +74,18 @@
 
 def posts_date_filter(media):
     if args.before:
         media=filter(lambda x:x.postdate==None or arrow.get(x.postdate)<=args.before,media)
     if args.after:
         media=filter(lambda x:x.postdate==None or arrow.get(x.postdate)>=args.after,media)
     return list(media)
+
+def post_timed_filter(media):
+    if args.skip_timed:
+        return list(filter(lambda x:not x.expires,media))
+    return media
+def post_user_filter(media):
+    userfilter=args.filter
+    if not userfilter.islower():
+        return list(filter(lambda x:re.search(userfilter,x.text or "")!=None,media))
+    else:
+        return list(filter(lambda x:re.search(userfilter,x.text or "",re.IGNORECASE)!=None,media))
```

### Comparing `ofscraper-2.1/ofscraper/utils/logger.py` & `ofscraper-2.4/ofscraper/utils/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 import re
 import httpx
 import logging
 import threading
 import time
 import queue
 from rich.logging import RichHandler
+from tenacity import retry,stop_after_attempt,wait_fixed
+
 import ofscraper.utils.paths as paths
 import ofscraper.utils.config as config_
 import ofscraper.utils.args as args
 import ofscraper.utils.console as console
-
+import ofscraper.constants as constants
 senstiveDict={}
 discord_queue=queue.Queue()
 
 
 class DebugOnly(logging.Filter):
     def filter(self, record):
         if record.levelname=="DEBUG" or record.levelname=="TRACEBACK":
@@ -37,40 +39,52 @@
         #convert markup
         log_entry=re.sub("\[bold\]|\[/bold\]","**",log_entry)
         discord_queue.put((url,log_entry))
 
 def discord_messenger():
     with httpx.Client() as c:
         while True:
-            url,entry=discord_queue.get()   
+            url,message=discord_queue.get()   
             if url=="exit":
-                return 
-            c.post(url, headers={"Content-type": "application/json"},json={"content":entry})
+                return
+            try:
+                discord_pusher(url,message,c)
+            except httpx.HTTPError as E:
+                console.shared_console.print("Discord Error")
+
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_fixed(constants.DISCORDWAIT),reraise=True) 
+def discord_pusher(url,message,c):
+    c.post(url, headers={"Content-type": "application/json"},json={"content":message})
+
+
+
 def discord_cleanup():
     logging.getLogger("ofscraper").info("Pushing Discord Queue")
     with httpx.Client() as c:
         while True:
             if discord_queue.empty:
                 discord_queue.put(("exit",None))
                 break
             time.sleep(.5)
              
-
-
-worker_thread = threading.Thread(target=discord_messenger)
-worker_thread.start()
+def start_discord_queue():
+    worker_thread = threading.Thread(target=discord_messenger)
+    worker_thread.start()
 class SensitiveFormatter(logging.Formatter):
     """Formatter that removes sensitive information in logs."""
     @staticmethod
     def _filter(s):
-        s=re.sub("&Policy=[^&\"]+", "&Policy={hidden}", s)
-        s=re.sub("&Signature=[^&\"]+", "&Signature={hidden}", s)
-        s=re.sub("&Key-Pair-Id=[^&\"]+", "&Key-Pair-Id={hidden}", s)
-        for ele in senstiveDict.items():
-             s=re.sub(re.escape(str(ele[0])),str(ele[1]),s)
+        if s.find("Avatar :"):
+            None
+        else:
+            s=re.sub("&Policy=[^&\"]+", "&Policy={hidden}", s)
+            s=re.sub("&Signature=[^&\"]+", "&Signature={hidden}", s)
+            s=re.sub("&Key-Pair-Id=[^&\"]+", "&Key-Pair-Id={hidden}", s)
+            for ele in senstiveDict.items():
+                s=re.sub(re.escape(str(ele[0])),str(ele[1]),s)
         return s
 
     def format(self, record):
         original = logging.Formatter.format(self, record)  # call parent method
         return self._filter(original)
```

### Comparing `ofscraper-2.1/ofscraper/utils/profiles.py` & `ofscraper-2.4/ofscraper/utils/profiles.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,28 @@
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
-import pathlib
 import shutil
+import logging
 from rich.console import Console
 from rich import print
 import ofscraper.utils.config as config_
 import ofscraper.prompts.prompts as prompts
 import ofscraper.constants as constants
-import logging
+import ofscraper.utils.paths as paths_
 log=logging.getLogger(__package__)
 console=Console()
 
 
 def get_profile_path():
-    config_path = pathlib.Path.home() / constants.configPath
+    config_path = paths_.get_config_path().parent
     return config_path
 
 
 def get_profiles() -> list:
     config_path = get_profile_path()
     dir_contents = config_path.glob('*')
     profiles = [item for item in dir_contents if item.is_dir()]
```

### Comparing `ofscraper-2.1/pyproject.toml` & `ofscraper-2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [tool.poetry]
 name = "ofscraper"
-version = "2.1"
+version = "2.4"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
-packages = [{include = "ofscraper"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
 httpx = {extras = ["http2"], version = "^0.23.3"}
 inquirerpy = "^0.3.4"
 setuptools = "^67.6.0"
 schedule = "^1.1.0"
@@ -22,14 +21,15 @@
 pathvalidate = "^2.5.2"
 xxhash = "^3.2.0"
 mpegdash = "^0.3.1"
 diskcache = "^5.6.1"
 ffmpeg-python = "^0.2.0"
 dunamai = "^1.17.0"
 poetry-dynamic-versioning = "^0.22.0"
+textual = "^0.27.0"
 
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
 
 
 [tool.poetry.group.test]
@@ -37,24 +37,25 @@
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-check = { version = "2.1.4", python = ">3.7" }
 coverage = "^7.2.3"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
+random-unicode-emoji = "^2.8"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry.scripts]
-ofscraper = "ofscraper.scraper:main"
+ofscraper = "ofscraper.start:main"
 
 [project.scripts]
-ofscraper = "ofscraper.scraper:main"
+ofscraper = "ofscraper.start:main"
 
 [tool.poetry.urls]
 "Homepage" = "https://github.com/datawhores/OF-Scraper"
 
 # pyproject.toml
 [tool.pytest.ini_options]
 minversion = "6.0"
```

### Comparing `ofscraper-2.1/PKG-INFO` & `ofscraper-2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 2.1
+Version: 2.4
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -23,19 +23,22 @@
 Requires-Dist: pathvalidate (>=2.5.2,<3.0.0)
 Requires-Dist: poetry-dynamic-versioning (>=0.22.0,<0.23.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: schedule (>=1.1.0,<2.0.0)
 Requires-Dist: setuptools (>=67.6.0,<68.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
+Requires-Dist: textual (>=0.27.0,<0.28.0)
 Requires-Dist: win32-setctime (>=1.1.0,<2.0.0)
 Requires-Dist: xxhash (>=3.2.0,<4.0.0)
 Project-URL: Homepage, https://github.com/datawhores/OF-Scraper
 Description-Content-Type: text/markdown
 
+# Intro
+
 A fork of onlyfans-scraper. It has been optimized to make it more feature complete with digitalcriminal's onlyfans script.
 A matter of fact with the right settings transitioning between the two scripts should be a easy enough process
 
 In addition there are numerous filtering features to control exactly which type of content you want to scrape.
 https://github.com/datawhores/OF-Scraper/blob/main/CHANGES.md
 
 <h3>DISCLAIMERS:</h3>
```

